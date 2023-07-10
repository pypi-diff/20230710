# Comparing `tmp/gisting_test-0.2.2.tar.gz` & `tmp/gisting_test-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting_test-0.2.2.tar", last modified: Sat Jun 17 04:55:02 2023, max compression
+gzip compressed data, was "gisting_test-0.2.3.tar", last modified: Mon Jul 10 18:43:28 2023, max compression
```

## Comparing `gisting_test-0.2.2.tar` & `gisting_test-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:55:02.773727 gisting_test-0.2.2/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 04:55:02.773598 gisting_test-0.2.2/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:55:02.769687 gisting_test-0.2.2/gisting_test/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.2.2/gisting_test/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:55:02.772868 gisting_test-0.2.2/gisting_test/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.2.2/gisting_test/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8864 2023-06-17 04:52:01.000000 gisting_test-0.2.2/gisting_test/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:55:02.773382 gisting_test-0.2.2/gisting_test/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41432 2023-06-17 04:54:38.000000 gisting_test-0.2.2/gisting_test/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.2.2/gisting_test/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-17 04:55:02.770374 gisting_test-0.2.2/gisting_test.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-17 04:55:02.000000 gisting_test-0.2.2/gisting_test.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-17 04:55:02.000000 gisting_test-0.2.2/gisting_test.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-17 04:55:02.000000 gisting_test-0.2.2/gisting_test.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-17 04:55:02.000000 gisting_test-0.2.2/gisting_test.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-17 04:55:02.773772 gisting_test-0.2.2/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-17 04:54:47.000000 gisting_test-0.2.2/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-07-10 18:43:28.581474 gisting_test-0.2.3/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-07-10 18:43:28.581369 gisting_test-0.2.3/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-07-10 18:43:28.576453 gisting_test-0.2.3/gisting_test/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.2.3/gisting_test/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-07-10 18:43:28.580726 gisting_test-0.2.3/gisting_test/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.2.3/gisting_test/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8860 2023-07-10 18:10:51.000000 gisting_test-0.2.3/gisting_test/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-07-10 18:43:28.581124 gisting_test-0.2.3/gisting_test/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41437 2023-06-17 16:58:23.000000 gisting_test-0.2.3/gisting_test/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.2.3/gisting_test/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-07-10 18:43:28.577092 gisting_test-0.2.3/gisting_test.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-07-10 18:43:28.000000 gisting_test-0.2.3/gisting_test.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-07-10 18:43:28.000000 gisting_test-0.2.3/gisting_test.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-07-10 18:43:28.000000 gisting_test-0.2.3/gisting_test.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-07-10 18:43:28.000000 gisting_test-0.2.3/gisting_test.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-07-10 18:43:28.581586 gisting_test-0.2.3/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-07-10 18:10:56.000000 gisting_test-0.2.3/setup.py
```

### Comparing `gisting_test-0.2.2/gisting_test/src/arguments.py` & `gisting_test-0.2.3/gisting_test/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/benchmarking.py` & `gisting_test-0.2.3/gisting_test/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/compress.py` & `gisting_test-0.2.3/gisting_test/src/compress.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             cache_dir=cache_dir,
         )
     else:
         
         model = model_cls.from_pretrained(
             model_name_or_path,
             config=config,
-            device_map = "balanced"
+            cache_dir=cache_dir
         )
         
 
     dtypes = {
         "bf16": torch.bfloat16,
         "fp16": torch.float16,
         "fp32": torch.float,
```

### Comparing `gisting_test-0.2.2/gisting_test/src/data/gist.py` & `gisting_test-0.2.3/gisting_test/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/data/utils.py` & `gisting_test-0.2.3/gisting_test/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/generation_utils.py` & `gisting_test-0.2.3/gisting_test/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/gist_caching.py` & `gisting_test-0.2.3/gisting_test/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/gist_llama.py` & `gisting_test-0.2.3/gisting_test/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/gist_t5.py` & `gisting_test-0.2.3/gisting_test/src/gist_t5.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,16 +429,16 @@
             config.d_model, eps=config.layer_norm_epsilon
         )
         self.dropout = nn.Dropout(config.dropout_rate)
 
         # Initialize weights and apply final processing
         self.post_init()
         # Model parallel
-        self.model_parallel = False
-        self.device_map = None
+        self.model_parallel = True
+        self.device_map = "balanced"
         self.gradient_checkpointing = False
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         encoder_hidden_states=None,
```

### Comparing `gisting_test-0.2.2/gisting_test/src/integrations.py` & `gisting_test-0.2.3/gisting_test/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/metrics.py` & `gisting_test-0.2.3/gisting_test/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/train.py` & `gisting_test-0.2.3/gisting_test/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/trainer_seq2seq.py` & `gisting_test-0.2.3/gisting_test/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test/src/weight_diff.py` & `gisting_test-0.2.3/gisting_test/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.2.2/gisting_test.egg-info/SOURCES.txt` & `gisting_test-0.2.3/gisting_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

