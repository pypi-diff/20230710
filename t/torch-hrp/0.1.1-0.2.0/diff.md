# Comparing `tmp/torch-hrp-0.1.1.tar.gz` & `tmp/torch-hrp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-hrp-0.1.1.tar", last modified: Sat May 13 06:07:45 2023, max compression
+gzip compressed data, was "torch-hrp-0.2.0.tar", last modified: Mon Jul 10 08:26:11 2023, max compression
```

## Comparing `torch-hrp-0.1.1.tar` & `torch-hrp-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 08:46:45.000000 torch-hrp-0.1.1/LICENSE
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 08:46:45.000000 torch-hrp-0.1.1/MANIFEST.in
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5884 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5545 2023-05-13 06:07:16.000000 torch-hrp-0.1.1/README.md
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/setup.cfg
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     1005 2023-05-10 09:48:41.000000 torch-hrp-0.1.1/setup.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/test/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 08:44:36.000000 torch-hrp-0.1.1/test/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     2233 2023-05-10 11:32:46.000000 torch-hrp-0.1.1/test/test_hrp.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/torch_hrp/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       71 2023-05-12 14:17:35.000000 torch-hrp-0.1.1/torch_hrp/__init__.py
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5947 2023-05-13 06:00:25.000000 torch-hrp-0.1.1/torch_hrp/hrp.py
-drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-05-13 06:07:45.241309 torch-hrp-0.1.1/torch_hrp.egg-info/
--rw-rw-r--   0 hamster   (1000) hamster   (1000)     5884 2023-05-13 06:07:45.000000 torch-hrp-0.1.1/torch_hrp.egg-info/PKG-INFO
--rw-rw-r--   0 hamster   (1000) hamster   (1000)      303 2023-05-13 06:07:45.000000 torch-hrp-0.1.1/torch_hrp.egg-info/SOURCES.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-13 06:07:45.000000 torch-hrp-0.1.1/torch_hrp.egg-info/dependency_links.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       29 2023-05-13 06:07:45.000000 torch-hrp-0.1.1/torch_hrp.egg-info/requires.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)       10 2023-05-13 06:07:45.000000 torch-hrp-0.1.1/torch_hrp.egg-info/top_level.txt
--rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-12 06:12:19.000000 torch-hrp-0.1.1/torch_hrp.egg-info/zip-safe
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:26:11.991953 torch-hrp-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-05-09 08:46:45.000000 torch-hrp-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-05-09 08:46:45.000000 torch-hrp-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6112 2023-07-10 08:26:11.991953 torch-hrp-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5778 2023-07-08 16:59:56.000000 torch-hrp-0.2.0/README.md
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 08:26:11.991953 torch-hrp-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1000 2023-07-08 16:55:14.000000 torch-hrp-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:26:11.987953 torch-hrp-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-05-09 08:44:36.000000 torch-hrp-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2233 2023-05-10 11:32:46.000000 torch-hrp-0.2.0/test/test_hrp.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:26:11.987953 torch-hrp-0.2.0/torch_hrp/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       71 2023-07-10 07:58:22.000000 torch-hrp-0.2.0/torch_hrp/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5947 2023-05-13 06:30:48.000000 torch-hrp-0.2.0/torch_hrp/hrp.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:26:11.987953 torch-hrp-0.2.0/torch_hrp.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6112 2023-07-10 08:26:11.000000 torch-hrp-0.2.0/torch_hrp.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      303 2023-07-10 08:26:11.000000 torch-hrp-0.2.0/torch_hrp.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 08:26:11.000000 torch-hrp-0.2.0/torch_hrp.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       29 2023-07-10 08:26:11.000000 torch-hrp-0.2.0/torch_hrp.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       10 2023-07-10 08:26:11.000000 torch-hrp-0.2.0/torch_hrp.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-05-12 06:12:19.000000 torch-hrp-0.2.0/torch_hrp.egg-info/zip-safe
```

### Comparing `torch-hrp-0.1.1/LICENSE` & `torch-hrp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-hrp-0.1.1/PKG-INFO` & `torch-hrp-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: torch-hrp
-Version: 0.1.1
+Version: 0.2.0
 Summary: Hashed Random Projection layer for PyTorch
-Home-page: http://github.com/satzbeleg/torch-hrp
+Home-page: http://github.com/ulf1/torch-hrp
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![PyPi downloads](https://img.shields.io/pypi/dm/torch-hrp)](https://img.shields.io/pypi/dm/torch-hrp)
 
 
 # torch-hrp
 Hashed Random Projection layer for PyTorch.
 
 ## Usage
-<a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
+<a href="https://github.com/ulf1/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
 
 
 ### Generate a HRP layer with a new hyperplane
 The random projection or hyperplane is randomly initialized.
 The initial state of the PRNG (`random_state`) is required (Default: 42) to ensure reproducibility.
 
 ```py
@@ -95,24 +95,24 @@
     x = torch.rand(int(20e6), 768)  # 20 Mio examples
     pool = model_hrp.start_pool()
     hashed = model_hrp.infer(x, pool, chunk_size=int(45e5))  # chunks of 4.5 Mio examples
     model_hrp.stop_pool(pool)
     torch.cuda.empty_cache()
 ```
 
-see <a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
+see <a href="https://github.com/ulf1/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
 
 ## Appendix
 
 ### Installation
-The `torch-hrp` [git repo](http://github.com/satzbeleg/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
+The `torch-hrp` [git repo](http://github.com/ulf1/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
 
 ```sh
 pip install torch-hrp
-pip install git+ssh://git@github.com/satzbeleg/torch-hrp.git
+pip install git+ssh://git@github.com/ulf1/torch-hrp.git
 ```
 
 ### Install a virtual environment (CPU)
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -164,23 +164,27 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/torch-hrp/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/torch-hrp/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/torch-hrp/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/torch-hrp/compare/).
 
 ### Acknowledgements
 The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
+### Maintenance
+- till 31.Aug.2023 (v0.1.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by [@ulf1](https://github.com/ulf1).
+
 ### Citation
 Please cite the arXiv Preprint when using this software for any purpose.
 
 ```
 @misc{hamster2023rediscovering,
       title={Rediscovering Hashed Random Projections for Efficient Quantization of Contextualized Sentence Embeddings}, 
       author={Ulf A. Hamster and Ji-Ung Lee and Alexander Geyken and Iryna Gurevych},
```

### Comparing `torch-hrp-0.1.1/README.md` & `torch-hrp-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![PyPi downloads](https://img.shields.io/pypi/dm/torch-hrp)](https://img.shields.io/pypi/dm/torch-hrp)
 
 
 # torch-hrp
 Hashed Random Projection layer for PyTorch.
 
 ## Usage
-<a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
+<a href="https://github.com/ulf1/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
 
 
 ### Generate a HRP layer with a new hyperplane
 The random projection or hyperplane is randomly initialized.
 The initial state of the PRNG (`random_state`) is required (Default: 42) to ensure reproducibility.
 
 ```py
@@ -82,24 +82,24 @@
     x = torch.rand(int(20e6), 768)  # 20 Mio examples
     pool = model_hrp.start_pool()
     hashed = model_hrp.infer(x, pool, chunk_size=int(45e5))  # chunks of 4.5 Mio examples
     model_hrp.stop_pool(pool)
     torch.cuda.empty_cache()
 ```
 
-see <a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
+see <a href="https://github.com/ulf1/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
 
 ## Appendix
 
 ### Installation
-The `torch-hrp` [git repo](http://github.com/satzbeleg/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
+The `torch-hrp` [git repo](http://github.com/ulf1/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
 
 ```sh
 pip install torch-hrp
-pip install git+ssh://git@github.com/satzbeleg/torch-hrp.git
+pip install git+ssh://git@github.com/ulf1/torch-hrp.git
 ```
 
 ### Install a virtual environment (CPU)
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -151,23 +151,27 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/torch-hrp/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/torch-hrp/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/torch-hrp/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/torch-hrp/compare/).
 
 ### Acknowledgements
 The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
+### Maintenance
+- till 31.Aug.2023 (v0.1.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by [@ulf1](https://github.com/ulf1).
+
 ### Citation
 Please cite the arXiv Preprint when using this software for any purpose.
 
 ```
 @misc{hamster2023rediscovering,
       title={Rediscovering Hashed Random Projections for Efficient Quantization of Contextualized Sentence Embeddings}, 
       author={Ulf A. Hamster and Ji-Ung Lee and Alexander Geyken and Iryna Gurevych},
```

### Comparing `torch-hrp-0.1.1/setup.py` & `torch-hrp-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setuptools.setup(
     name='torch-hrp',
     version=get_version("torch_hrp/__init__.py"),
     description='Hashed Random Projection layer for PyTorch',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
-    url='http://github.com/satzbeleg/torch-hrp',
+    url='http://github.com/ulf1/torch-hrp',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['torch_hrp'],
     install_requires=[
         'torch>=1,<2',
         'numpy>=1.19.5,<2'
```

### Comparing `torch-hrp-0.1.1/test/test_hrp.py` & `torch-hrp-0.2.0/test/test_hrp.py`

 * *Files identical despite different names*

### Comparing `torch-hrp-0.1.1/torch_hrp/hrp.py` & `torch-hrp-0.2.0/torch_hrp/hrp.py`

 * *Files identical despite different names*

### Comparing `torch-hrp-0.1.1/torch_hrp.egg-info/PKG-INFO` & `torch-hrp-0.2.0/torch_hrp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: torch-hrp
-Version: 0.1.1
+Version: 0.2.0
 Summary: Hashed Random Projection layer for PyTorch
-Home-page: http://github.com/satzbeleg/torch-hrp
+Home-page: http://github.com/ulf1/torch-hrp
 Author: Ulf Hamster
 Author-email: 554c46@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 [![PyPi downloads](https://img.shields.io/pypi/dm/torch-hrp)](https://img.shields.io/pypi/dm/torch-hrp)
 
 
 # torch-hrp
 Hashed Random Projection layer for PyTorch.
 
 ## Usage
-<a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
+<a href="https://github.com/ulf1/torch-hrp/blob/main/demo/Hashed%20Random%20Projections.ipynb">Hashed Random Projections (HRP), binary representations, encoding/decoding for storage</a> (notebook)
 
 
 ### Generate a HRP layer with a new hyperplane
 The random projection or hyperplane is randomly initialized.
 The initial state of the PRNG (`random_state`) is required (Default: 42) to ensure reproducibility.
 
 ```py
@@ -95,24 +95,24 @@
     x = torch.rand(int(20e6), 768)  # 20 Mio examples
     pool = model_hrp.start_pool()
     hashed = model_hrp.infer(x, pool, chunk_size=int(45e5))  # chunks of 4.5 Mio examples
     model_hrp.stop_pool(pool)
     torch.cuda.empty_cache()
 ```
 
-see <a href="https://github.com/satzbeleg/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
+see <a href="https://github.com/ulf1/torch-hrp/blob/main/demo/multiprocessing-on-gpu-server.py">demo/multiprocessing-on-gpu-server.py</a>
 
 ## Appendix
 
 ### Installation
-The `torch-hrp` [git repo](http://github.com/satzbeleg/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
+The `torch-hrp` [git repo](http://github.com/ulf1/torch-hrp) is available as [PyPi package](https://pypi.org/project/torch-hrp)
 
 ```sh
 pip install torch-hrp
-pip install git+ssh://git@github.com/satzbeleg/torch-hrp.git
+pip install git+ssh://git@github.com/ulf1/torch-hrp.git
 ```
 
 ### Install a virtual environment (CPU)
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -164,23 +164,27 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/torch-hrp/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/torch-hrp/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/torch-hrp/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/torch-hrp/compare/).
 
 ### Acknowledgements
 The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
+### Maintenance
+- till 31.Aug.2023 (v0.1.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by [@ulf1](https://github.com/ulf1).
+
 ### Citation
 Please cite the arXiv Preprint when using this software for any purpose.
 
 ```
 @misc{hamster2023rediscovering,
       title={Rediscovering Hashed Random Projections for Efficient Quantization of Contextualized Sentence Embeddings}, 
       author={Ulf A. Hamster and Ji-Ung Lee and Alexander Geyken and Iryna Gurevych},
```

