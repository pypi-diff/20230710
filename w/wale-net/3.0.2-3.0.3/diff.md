# Comparing `tmp/wale-net-3.0.2.tar.gz` & `tmp/wale-net-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wale-net-3.0.2.tar", last modified: Thu Apr 20 07:25:45 2023, max compression
+gzip compressed data, was "wale-net-3.0.3.tar", last modified: Mon Jul 10 08:11:15 2023, max compression
```

## Comparing `wale-net-3.0.2.tar` & `wale-net-3.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1071 2022-12-19 14:40:59.000000 wale-net-3.0.2/LICENSE
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      175 2022-12-19 14:40:59.000000 wale-net-3.0.2/MANIFEST.in
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-04-20 07:25:45.108377 wale-net-3.0.2/PKG-INFO
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     4151 2022-12-19 14:40:59.000000 wale-net-3.0.2/README.md
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.104377 wale-net-3.0.2/prediction/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)       62 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/__init__.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     4623 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/bayesian_optimization.py
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/configs/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1694 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/README.md
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      898 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/best_config.json
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      824 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/default.json
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/configs/online/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1309 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online/README.md
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      394 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online/default.json
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      747 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/configs/online_learning.json
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     8629 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/evaluate.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     8336 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/evaluate_online_learning.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)    35277 2023-03-23 12:22:12.000000 wale-net-3.0.2/prediction/main.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1479 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/nvrgrad.py
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/tools/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/__init__.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)    10634 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/commonroad_dataset.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     9387 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/eval_analysis.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     5946 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/grad_variance.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      296 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/tools/rename.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)    13978 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/train.py
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/trained_models/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)   446790 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/trained_models/best_model.tar
--rw-rw-r--   0 rainer    (1000) rainer    (1000)  1468458 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/trained_models/online_learning.tar
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/prediction/utils/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/__init__.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      373 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/cuda.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     3890 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/dataset.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     5345 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/geometry.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)    11490 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/model.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     6076 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/neural_network.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     9618 2023-01-17 18:38:18.000000 wale-net-3.0.2/prediction/utils/preprocessing.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)    14173 2022-12-19 14:40:59.000000 wale-net-3.0.2/prediction/utils/visualization.py
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      185 2023-03-23 12:22:46.000000 wale-net-3.0.2/requirements.txt
--rw-rw-r--   0 rainer    (1000) rainer    (1000)       38 2023-04-20 07:25:45.108377 wale-net-3.0.2/setup.cfg
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1512 2023-04-20 07:19:07.000000 wale-net-3.0.2/setup.py
-drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-20 07:25:45.108377 wale-net-3.0.2/wale_net.egg-info/
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/PKG-INFO
--rw-rw-r--   0 rainer    (1000) rainer    (1000)     1098 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/SOURCES.txt
--rw-rw-r--   0 rainer    (1000) rainer    (1000)        1 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/dependency_links.txt
--rw-rw-r--   0 rainer    (1000) rainer    (1000)      184 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/requires.txt
--rw-rw-r--   0 rainer    (1000) rainer    (1000)       11 2023-04-20 07:25:45.000000 wale-net-3.0.2/wale_net.egg-info/top_level.txt
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.647906 wale-net-3.0.3/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1071 2022-12-19 14:40:59.000000 wale-net-3.0.3/LICENSE
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      175 2022-12-19 14:40:59.000000 wale-net-3.0.3/MANIFEST.in
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-07-10 08:11:15.643906 wale-net-3.0.3/PKG-INFO
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     4151 2022-12-19 14:40:59.000000 wale-net-3.0.3/README.md
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.639906 wale-net-3.0.3/prediction/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       62 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     4623 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/bayesian_optimization.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.639906 wale-net-3.0.3/prediction/configs/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1694 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/README.md
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      898 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/best_config.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      824 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/default.json
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.643906 wale-net-3.0.3/prediction/configs/online/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1309 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/online/README.md
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      394 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/online/default.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      747 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/configs/online_learning.json
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     8629 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/evaluate.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     8336 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/evaluate_online_learning.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    35277 2023-03-23 12:22:12.000000 wale-net-3.0.3/prediction/main.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1479 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/nvrgrad.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.643906 wale-net-3.0.3/prediction/tools/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/tools/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    10634 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/tools/commonroad_dataset.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     9387 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/tools/eval_analysis.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     5946 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/tools/grad_variance.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      296 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/tools/rename.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    13978 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/train.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.643906 wale-net-3.0.3/prediction/trained_models/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)   446790 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/trained_models/best_model.tar
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)  1468458 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/trained_models/online_learning.tar
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.643906 wale-net-3.0.3/prediction/utils/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        0 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/__init__.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      373 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/cuda.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     3890 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/dataset.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     5345 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/geometry.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    11490 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/model.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     6076 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/neural_network.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     9618 2023-01-17 18:38:18.000000 wale-net-3.0.3/prediction/utils/preprocessing.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)    14173 2022-12-19 14:40:59.000000 wale-net-3.0.3/prediction/utils/visualization.py
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      185 2023-07-10 08:07:44.000000 wale-net-3.0.3/requirements.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       38 2023-07-10 08:11:15.647906 wale-net-3.0.3/setup.cfg
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1512 2023-07-10 08:07:56.000000 wale-net-3.0.3/setup.py
+drwxrwxr-x   0 rainer    (1000) rainer    (1000)        0 2023-07-10 08:11:15.643906 wale-net-3.0.3/wale_net.egg-info/
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      891 2023-07-10 08:11:15.000000 wale-net-3.0.3/wale_net.egg-info/PKG-INFO
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)     1098 2023-07-10 08:11:15.000000 wale-net-3.0.3/wale_net.egg-info/SOURCES.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)        1 2023-07-10 08:11:15.000000 wale-net-3.0.3/wale_net.egg-info/dependency_links.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)      184 2023-07-10 08:11:15.000000 wale-net-3.0.3/wale_net.egg-info/requires.txt
+-rw-rw-r--   0 rainer    (1000) rainer    (1000)       11 2023-07-10 08:11:15.000000 wale-net-3.0.3/wale_net.egg-info/top_level.txt
```

### Comparing `wale-net-3.0.2/LICENSE` & `wale-net-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/PKG-INFO` & `wale-net-3.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wale-net
-Version: 3.0.2
+Version: 3.0.3
 Summary: Prediction module for CommonRoad
 Home-page: https://github.com/TUMFTM/Wale-Net
 Author: Maximilian Geisslinger, Phillip Karle
 Author-email: maximilian.geisslinger@tum.de, karle@ftm.mw.tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wale-net-3.0.2/README.md` & `wale-net-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/bayesian_optimization.py` & `wale-net-3.0.3/prediction/bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/configs/README.md` & `wale-net-3.0.3/prediction/configs/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/configs/best_config.json` & `wale-net-3.0.3/prediction/configs/best_config.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/configs/default.json` & `wale-net-3.0.3/prediction/configs/default.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/configs/online/README.md` & `wale-net-3.0.3/prediction/configs/online/README.md`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/configs/online_learning.json` & `wale-net-3.0.3/prediction/configs/online_learning.json`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/evaluate.py` & `wale-net-3.0.3/prediction/evaluate.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/evaluate_online_learning.py` & `wale-net-3.0.3/prediction/evaluate_online_learning.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/main.py` & `wale-net-3.0.3/prediction/main.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/nvrgrad.py` & `wale-net-3.0.3/prediction/nvrgrad.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/tools/commonroad_dataset.py` & `wale-net-3.0.3/prediction/tools/commonroad_dataset.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/tools/eval_analysis.py` & `wale-net-3.0.3/prediction/tools/eval_analysis.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/tools/grad_variance.py` & `wale-net-3.0.3/prediction/tools/grad_variance.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/train.py` & `wale-net-3.0.3/prediction/train.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/trained_models/best_model.tar` & `wale-net-3.0.3/prediction/trained_models/best_model.tar`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/trained_models/online_learning.tar` & `wale-net-3.0.3/prediction/trained_models/online_learning.tar`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/dataset.py` & `wale-net-3.0.3/prediction/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/geometry.py` & `wale-net-3.0.3/prediction/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/model.py` & `wale-net-3.0.3/prediction/utils/model.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/neural_network.py` & `wale-net-3.0.3/prediction/utils/neural_network.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/preprocessing.py` & `wale-net-3.0.3/prediction/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/prediction/utils/visualization.py` & `wale-net-3.0.3/prediction/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `wale-net-3.0.2/setup.py` & `wale-net-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return subprocess.check_output(["git"] + list(args))
 
 
 # get latest tag
 latest = git("describe", "--tags").decode().strip()
 latest = latest.split("-")[0]
 # for pypi package the tag must be set manually
-latest = "3.0.2"
+latest = "3.0.3"
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 long_description = """
 This package provides a Recurrent Neural Network (RNN) for vehicle trajectory prediction with uncertainties.
```

### Comparing `wale-net-3.0.2/wale_net.egg-info/PKG-INFO` & `wale-net-3.0.3/wale_net.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wale-net
-Version: 3.0.2
+Version: 3.0.3
 Summary: Prediction module for CommonRoad
 Home-page: https://github.com/TUMFTM/Wale-Net
 Author: Maximilian Geisslinger, Phillip Karle
 Author-email: maximilian.geisslinger@tum.de, karle@ftm.mw.tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wale-net-3.0.2/wale_net.egg-info/SOURCES.txt` & `wale-net-3.0.3/wale_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

