# Comparing `tmp/graph-model-parser-0.1.3.tar.gz` & `tmp/graph-model-parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-model-parser-0.1.3.tar", last modified: Sun Apr 23 18:56:43 2023, max compression
+gzip compressed data, was "graph-model-parser-0.1.4.tar", last modified: Mon Jul 10 13:41:28 2023, max compression
```

## Comparing `graph-model-parser-0.1.3.tar` & `graph-model-parser-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964506 graph-model-parser-0.1.3/
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-04-23 18:56:43.964576 graph-model-parser-0.1.3/PKG-INFO
--rw-r--r--   0 albertbuchard   (501) staff       (20)     1767 2023-04-23 18:55:32.000000 graph-model-parser-0.1.3/README.md
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.963356 graph-model-parser-0.1.3/graph_model_parser/
--rw-r--r--   0 albertbuchard   (501) staff       (20)       49 2023-04-23 18:52:31.000000 graph-model-parser-0.1.3/graph_model_parser/__init__.py
--rw-r--r--   0 albertbuchard   (501) staff       (20)     8262 2023-04-23 18:03:02.000000 graph-model-parser-0.1.3/graph_model_parser/graph_model_parser.py
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964136 graph-model-parser-0.1.3/graph_model_parser.egg-info/
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/PKG-INFO
--rw-r--r--   0 albertbuchard   (501) staff       (20)      366 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/SOURCES.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)        1 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/dependency_links.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)       12 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/requires.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)       25 2023-04-23 18:56:43.000000 graph-model-parser-0.1.3/graph_model_parser.egg-info/top_level.txt
--rw-r--r--   0 albertbuchard   (501) staff       (20)      100 2023-04-23 18:19:22.000000 graph-model-parser-0.1.3/pyproject.toml
--rw-r--r--   0 albertbuchard   (501) staff       (20)      735 2023-04-23 18:56:43.964899 graph-model-parser-0.1.3/setup.cfg
-drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-04-23 18:56:43.964385 graph-model-parser-0.1.3/tests/
--rw-r--r--   0 albertbuchard   (501) staff       (20)        0 2023-04-23 16:23:02.000000 graph-model-parser-0.1.3/tests/__init__.py
--rw-r--r--   0 albertbuchard   (501) staff       (20)     2262 2023-04-23 18:52:52.000000 graph-model-parser-0.1.3/tests/test_graph_model_parser.py
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-07-10 13:41:28.738544 graph-model-parser-0.1.4/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-07-10 13:41:28.738600 graph-model-parser-0.1.4/PKG-INFO
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     1767 2023-04-23 18:55:32.000000 graph-model-parser-0.1.4/README.md
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-07-10 13:41:28.737465 graph-model-parser-0.1.4/graph_model_parser/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       49 2023-04-23 18:52:31.000000 graph-model-parser-0.1.4/graph_model_parser/__init__.py
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     8338 2023-05-02 09:12:50.000000 graph-model-parser-0.1.4/graph_model_parser/graph_model_parser.py
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-07-10 13:41:28.738141 graph-model-parser-0.1.4/graph_model_parser.egg-info/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2443 2023-07-10 13:41:28.000000 graph-model-parser-0.1.4/graph_model_parser.egg-info/PKG-INFO
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      366 2023-07-10 13:41:28.000000 graph-model-parser-0.1.4/graph_model_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)        1 2023-07-10 13:41:28.000000 graph-model-parser-0.1.4/graph_model_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       12 2023-07-10 13:41:28.000000 graph-model-parser-0.1.4/graph_model_parser.egg-info/requires.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)       25 2023-07-10 13:41:28.000000 graph-model-parser-0.1.4/graph_model_parser.egg-info/top_level.txt
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      100 2023-04-23 18:19:22.000000 graph-model-parser-0.1.4/pyproject.toml
+-rw-r--r--   0 albertbuchard   (501) staff       (20)      735 2023-07-10 13:41:28.738836 graph-model-parser-0.1.4/setup.cfg
+drwxr-xr-x   0 albertbuchard   (501) staff       (20)        0 2023-07-10 13:41:28.738413 graph-model-parser-0.1.4/tests/
+-rw-r--r--   0 albertbuchard   (501) staff       (20)        0 2023-04-23 16:23:02.000000 graph-model-parser-0.1.4/tests/__init__.py
+-rw-r--r--   0 albertbuchard   (501) staff       (20)     2262 2023-04-23 18:52:52.000000 graph-model-parser-0.1.4/tests/test_graph_model_parser.py
```

### Comparing `graph-model-parser-0.1.3/PKG-INFO` & `graph-model-parser-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-model-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for parsing and simulating dynamical graph models from string descriptions
 Home-page: https://github.com/albertbuchard/GraphModelParser
 Author: Albert Buchard
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graph-model-parser-0.1.3/README.md` & `graph-model-parser-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `graph-model-parser-0.1.3/graph_model_parser/graph_model_parser.py` & `graph-model-parser-0.1.4/graph_model_parser/graph_model_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from collections import deque
 
 import numpy as np
+import math
 from scipy.stats import norm, poisson, expon, binom, uniform
 
 
 class GraphModelParser:
     def __init__(self, model_description: str, initial_values: dict = None):
         """
         Class able to represent dynamical graph models from a string description, e.g.:
@@ -186,14 +187,16 @@
                 # Add custom functions for sampling
                 custom_functions = {
                     'normal': norm.rvs,
                     'uniform': uniform.rvs,
                     'poisson': poisson.rvs,
                     'binomial': binom.rvs,
                     'exponential': expon.rvs,
+                    'np': np,
+                    'math': math,
                     '__builtins__': None
                 }
 
                 # Extract variable names from the formula
                 var_pattern = re.compile(r"[a-zA-Z_\d^{]+_\d+")
                 formula_vars = set(var_pattern.findall(formula))
```

### Comparing `graph-model-parser-0.1.3/graph_model_parser.egg-info/PKG-INFO` & `graph-model-parser-0.1.4/graph_model_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-model-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for parsing and simulating dynamical graph models from string descriptions
 Home-page: https://github.com/albertbuchard/GraphModelParser
 Author: Albert Buchard
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graph-model-parser-0.1.3/setup.cfg` & `graph-model-parser-0.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graph-model-parser
-version = 0.1.3
+version = 0.1.4
 author = Albert Buchard
 description = A Python library for parsing and simulating dynamical graph models from string descriptions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/albertbuchard/GraphModelParser
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `graph-model-parser-0.1.3/tests/test_graph_model_parser.py` & `graph-model-parser-0.1.4/tests/test_graph_model_parser.py`

 * *Files identical despite different names*

