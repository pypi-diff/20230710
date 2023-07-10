# Comparing `tmp/sequence_modelling-0.1.3.tar.gz` & `tmp/sequence_modelling-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequence_modelling-0.1.3.tar", max compression
+gzip compressed data, was "sequence_modelling-0.1.4.tar", max compression
```

## Comparing `sequence_modelling-0.1.3.tar` & `sequence_modelling-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1500 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/LICENSE
--rw-r--r--   0        0        0     2306 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/README.md
--rw-r--r--   0        0        0      841 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9871 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/DiscreteOptim.py
--rw-r--r--   0        0        0        0 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/__init__.py
--rw-r--r--   0        0        0     5887 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/emissionplus.py
--rw-r--r--   0        0        0     5211 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/emmissions.py
--rw-r--r--   0        0        0    18426 2023-05-31 11:57:22.882421 sequence_modelling-0.1.3/src/sequence_modelling/hmm.py
--rw-r--r--   0        0        0     5900 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/hmmviz.py
--rw-r--r--   0        0        0    14709 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/qdhmm.py
--rw-r--r--   0        0        0    11895 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/qdhmm_logscaled.py
--rw-r--r--   0        0        0     1531 2023-05-31 11:57:22.886421 sequence_modelling-0.1.3/src/sequence_modelling/utils.py
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 sequence_modelling-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2306 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/README.md
+-rw-r--r--   0        0        0      863 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9871 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/DiscreteOptim.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/__init__.py
+-rw-r--r--   0        0        0     5887 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/emissionplus.py
+-rw-r--r--   0        0        0     5211 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/emmissions.py
+-rw-r--r--   0        0        0    18426 2023-07-10 17:50:48.137160 sequence_modelling-0.1.4/src/sequence_modelling/hmm.py
+-rw-r--r--   0        0        0     5900 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/hmmviz.py
+-rw-r--r--   0        0        0    14709 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/qdhmm.py
+-rw-r--r--   0        0        0    11895 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/qdhmm_logscaled.py
+-rw-r--r--   0        0        0     1531 2023-07-10 17:50:48.141160 sequence_modelling-0.1.4/src/sequence_modelling/utils.py
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 sequence_modelling-0.1.4/PKG-INFO
```

### Comparing `sequence_modelling-0.1.3/LICENSE` & `sequence_modelling-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/README.md` & `sequence_modelling-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/DiscreteOptim.py` & `sequence_modelling-0.1.4/src/sequence_modelling/DiscreteOptim.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/emissionplus.py` & `sequence_modelling-0.1.4/src/sequence_modelling/emissionplus.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/emmissions.py` & `sequence_modelling-0.1.4/src/sequence_modelling/emmissions.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/hmm.py` & `sequence_modelling-0.1.4/src/sequence_modelling/hmm.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/hmmviz.py` & `sequence_modelling-0.1.4/src/sequence_modelling/hmmviz.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/qdhmm.py` & `sequence_modelling-0.1.4/src/sequence_modelling/qdhmm.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/qdhmm_logscaled.py` & `sequence_modelling-0.1.4/src/sequence_modelling/qdhmm_logscaled.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/src/sequence_modelling/utils.py` & `sequence_modelling-0.1.4/src/sequence_modelling/utils.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.3/PKG-INFO` & `sequence_modelling-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: sequence-modelling
-Version: 0.1.3
+Version: 0.1.4
 Summary: sequence modelling using HMMs
 License: BSD-2-Clause
 Author: Nitin Bhushan
 Author-email: bhushan.nitin@posteo.net
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: Sphinx (==4.2.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (==1.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (==0.7) ; extra == "docs"
 Description-Content-Type: text/markdown
 
 [![tests](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/app-test.yml) [![docs](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml/badge.svg?branch=master)](https://github.com/nbhushan/Quasi-Deterministic-HMMs/actions/workflows/docs-pages.yaml) [![build](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml/badge.svg?branch=master)](https://github.com/nbhushan/sequence-modelling/actions/workflows/build-publish.yml)
```

