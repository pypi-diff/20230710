# Comparing `tmp/numalogic-0.5.0.tar.gz` & `tmp/numalogic-0.5.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.5.0.tar", max compression
+gzip compressed data, was "numalogic-0.5.0.post1.tar", max compression
```

## Comparing `numalogic-0.5.0.tar` & `numalogic-0.5.0.post1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    11357 2023-07-06 18:42:43.473405 numalogic-0.5.0/LICENSE
--rw-r--r--   0        0        0     5244 2023-07-06 18:42:43.473405 numalogic-0.5.0/README.md
--rw-r--r--   0        0        0      676 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/_constants.py
--rw-r--r--   0        0        0     1636 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/base.py
--rw-r--r--   0        0        0     1102 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3231 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1048 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2473 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/_config.py
--rw-r--r--   0        0        0     4680 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3772 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     3146 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11561 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8702 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4043 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2463 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       78 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/numaflow/__init__.py
--rw-r--r--   0        0        0     1925 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/numaflow/_base.py
--rw-r--r--   0        0        0     1282 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      328 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     5777 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15562 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     2828 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13638 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    12507 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11784 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1870 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     8422 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/data.py
--rw-r--r--   0        0        0     1740 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1973 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/types.py
--rw-r--r--   0        0        0     1153 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     5090 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     1861 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     2600 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     1771 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     2771 2023-07-06 18:42:43.537406 numalogic-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6686 1970-01-01 00:00:00.000000 numalogic-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 21:40:34.007861 numalogic-0.5.0.post1/LICENSE
+-rw-r--r--   0        0        0     5244 2023-07-10 21:40:34.007861 numalogic-0.5.0.post1/README.md
+-rw-r--r--   0        0        0      676 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/_constants.py
+-rw-r--r--   0        0        0     1636 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3231 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1048 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2473 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/config/_config.py
+-rw-r--r--   0        0        0     4680 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3772 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     3146 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11561 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8702 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4043 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2463 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       78 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/numaflow/__init__.py
+-rw-r--r--   0        0        0     1925 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/numaflow/_base.py
+-rw-r--r--   0        0        0     1282 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     5777 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15562 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3017 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13638 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    12507 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1870 2023-07-10 21:40:34.063862 numalogic-0.5.0.post1/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     8422 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/tools/data.py
+-rw-r--r--   0        0        0     1740 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     2049 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1153 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     5090 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     1861 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     2600 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     1771 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     2777 2023-07-10 21:40:34.067863 numalogic-0.5.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     6692 1970-01-01 00:00:00.000000 numalogic-0.5.0.post1/PKG-INFO
```

### Comparing `numalogic-0.5.0/LICENSE` & `numalogic-0.5.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/README.md` & `numalogic-0.5.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/__init__.py` & `numalogic-0.5.0.post1/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/_constants.py` & `numalogic-0.5.0.post1/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/base.py` & `numalogic-0.5.0.post1/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/blocks/__init__.py` & `numalogic-0.5.0.post1/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/blocks/_base.py` & `numalogic-0.5.0.post1/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/blocks/_nn.py` & `numalogic-0.5.0.post1/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/blocks/_transform.py` & `numalogic-0.5.0.post1/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/blocks/pipeline.py` & `numalogic-0.5.0.post1/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/config/__init__.py` & `numalogic-0.5.0.post1/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/config/_config.py` & `numalogic-0.5.0.post1/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/config/factory.py` & `numalogic-0.5.0.post1/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/__init__.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/base.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/trainer.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.5.0.post1/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/forecast/variants/naive.py` & `numalogic-0.5.0.post1/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/threshold/_static.py` & `numalogic-0.5.0.post1/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/models/threshold/_std.py` & `numalogic-0.5.0.post1/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/numaflow/_base.py` & `numalogic-0.5.0.post1/numalogic/numaflow/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/registry/__init__.py` & `numalogic-0.5.0.post1/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/registry/artifact.py` & `numalogic-0.5.0.post1/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/registry/dynamodb_registry.py` & `numalogic-0.5.0.post1/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/registry/localcache.py` & `numalogic-0.5.0.post1/numalogic/registry/localcache.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,40 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from copy import deepcopy
+from threading import Lock
 from typing import Optional
 
 from cachetools import TTLCache
 
 from numalogic.registry.artifact import ArtifactCache, ArtifactData
 from numalogic.tools.types import Singleton
 
 
 class LocalLRUCache(ArtifactCache, metaclass=Singleton):
-    r"""A local in-memory LRU cache with per item Time-to-live support.
+    r"""A local in-memory LRU cache registry with per artifact Time-to-live support.
 
     Args:
     ----
         cachesize: Size of the cache,
                    i.e. number of elements the cache can hold
         ttl: Time to live for each item in seconds
     """
 
     __cache: Optional[TTLCache] = None
 
     def __init__(self, cachesize: int = 512, ttl: int = 300):
         super().__init__(cachesize, ttl)
         if not self.__cache:
             self.__cache = TTLCache(maxsize=cachesize, ttl=ttl)
+        self.__lock = Lock()
 
     def __contains__(self, artifact_key: str) -> bool:
         """Check if an artifact is in the cache."""
         return artifact_key in self.__cache
 
     def load(self, artifact_key: str) -> Optional[ArtifactData]:
         """
@@ -47,43 +49,47 @@
         ----
             artifact_key: The key of the artifact to load.
 
         Returns
         -------
             The artifact data instance if found, None otherwise.
         """
-        return self.__cache.get(artifact_key)
+        with self.__lock:
+            return self.__cache.get(artifact_key)
 
     def save(self, key: str, artifact: ArtifactData) -> None:
         """
         Save an artifact to the cache.
 
         Args:
         ----
             key: The key of the artifact to save.
             artifact: The artifact data instance to save.
         """
         artifact = deepcopy(artifact)
         artifact.extras["source"] = self._STORETYPE
-        self.__cache[key] = artifact
+        with self.__lock:
+            self.__cache[key] = artifact
 
     def delete(self, key: str) -> Optional[ArtifactData]:
         """
         Delete an artifact from the cache.
 
         Args:
         ----
             key: The key of the artifact to delete.
 
         Returns
         -------
             The deleted artifact data instance if found, None otherwise.
         """
-        return self.__cache.pop(key, default=None)
+        with self.__lock:
+            return self.__cache.pop(key, default=None)
 
     def clear(self) -> None:
         """Clears the whole cache."""
-        self.__cache.clear()
+        with self.__lock:
+            self.__cache.clear()
 
     def keys(self) -> list[str]:
         """Returns the current keys of the cache."""
         return list(_key for _key in self.__cache)
```

### Comparing `numalogic-0.5.0/numalogic/registry/mlflow_registry.py` & `numalogic-0.5.0.post1/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/registry/redis_registry.py` & `numalogic-0.5.0.post1/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/synthetic/__init__.py` & `numalogic-0.5.0.post1/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/synthetic/anomalies.py` & `numalogic-0.5.0.post1/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/synthetic/sparsity.py` & `numalogic-0.5.0.post1/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/synthetic/timeseries.py` & `numalogic-0.5.0.post1/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/tools/callbacks.py` & `numalogic-0.5.0.post1/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/tools/data.py` & `numalogic-0.5.0.post1/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/tools/exceptions.py` & `numalogic-0.5.0.post1/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/tools/types.py` & `numalogic-0.5.0.post1/numalogic/tools/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,11 @@
 
     _instances: ClassVar[dict] = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super().__call__(*args, **kwargs)
         return cls._instances[cls]
+
+    @classmethod
+    def clear_instances(cls):
+        cls._instances = {}
```

### Comparing `numalogic-0.5.0/numalogic/transforms/__init__.py` & `numalogic-0.5.0.post1/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/transforms/_movavg.py` & `numalogic-0.5.0.post1/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/transforms/_postprocess.py` & `numalogic-0.5.0.post1/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/transforms/_scaler.py` & `numalogic-0.5.0.post1/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/numalogic/transforms/_stateless.py` & `numalogic-0.5.0.post1/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.5.0/pyproject.toml` & `numalogic-0.5.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.5.0"
+version = "0.5.0.post1"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.5.0/PKG-INFO` & `numalogic-0.5.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.5.0
+Version: 0.5.0.post1
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

