# Comparing `tmp/keras-bcr-0.2.0.tar.gz` & `tmp/keras-bcr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keras-bcr-0.2.0.tar", last modified: Fri May 27 08:05:31 2022, max compression
+gzip compressed data, was "keras-bcr-0.3.0.tar", last modified: Mon Jul 10 15:50:33 2023, max compression
```

## Comparing `keras-bcr-0.2.0.tar` & `keras-bcr-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/
--rw-r--r--   0 uh         (501) staff       (20)    11340 2022-05-09 15:20:45.000000 keras-bcr-0.2.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2022-05-09 15:20:45.000000 keras-bcr-0.2.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)      307 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     3894 2022-05-27 07:39:30.000000 keras-bcr-0.2.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-05-09 18:49:35.000000 keras-bcr-0.2.0/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/keras_bcr/
--rw-r--r--   0 uh         (501) staff       (20)       61 2022-05-27 07:40:24.000000 keras-bcr-0.2.0/keras_bcr/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     2302 2022-05-27 08:01:08.000000 keras-bcr-0.2.0/keras_bcr/bcr.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/keras_bcr.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)      307 2022-05-27 08:05:29.000000 keras-bcr-0.2.0/keras_bcr.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      314 2022-05-27 08:05:30.000000 keras-bcr-0.2.0/keras_bcr.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-05-27 08:05:30.000000 keras-bcr-0.2.0/keras_bcr.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       21 2022-05-27 08:05:30.000000 keras-bcr-0.2.0/keras_bcr.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       10 2022-05-27 08:05:30.000000 keras-bcr-0.2.0/keras_bcr.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-05-09 18:50:38.000000 keras-bcr-0.2.0/keras_bcr.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)      937 2022-05-09 18:50:17.000000 keras-bcr-0.2.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-27 08:05:31.000000 keras-bcr-0.2.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-05-09 15:19:40.000000 keras-bcr-0.2.0/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     1806 2022-05-27 07:59:54.000000 keras-bcr-0.2.0/test/test_bcr.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-07-10 08:48:40.000000 keras-bcr-0.3.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 08:48:40.000000 keras-bcr-0.3.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3928 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3593 2023-07-10 15:49:24.000000 keras-bcr-0.3.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/keras_bcr/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       61 2023-07-10 14:25:20.000000 keras-bcr-0.3.0/keras_bcr/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2305 2023-07-10 08:48:40.000000 keras-bcr-0.3.0/keras_bcr/bcr.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/keras_bcr.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3928 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      303 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       21 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       10 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:50:33.000000 keras-bcr-0.3.0/keras_bcr.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      982 2023-07-10 14:25:20.000000 keras-bcr-0.3.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:50:33.618688 keras-bcr-0.3.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:48:40.000000 keras-bcr-0.3.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1806 2023-07-10 08:48:40.000000 keras-bcr-0.3.0/test/test_bcr.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keras-bcr-0.2.0/LICENSE` & `keras-bcr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-bcr-0.2.0/README.md` & `keras-bcr-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 [![PyPI version](https://badge.fury.io/py/keras-bcr.svg)](https://badge.fury.io/py/keras-bcr)
 [![PyPi downloads](https://img.shields.io/pypi/dm/keras-bcr)](https://img.shields.io/pypi/dm/keras-bcr)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/satzbeleg/keras-bcr.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/keras-bcr/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/satzbeleg/keras-bcr.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/keras-bcr/context:python)
+
 
 # keras-bcr : Batch Correlation Regularizer for TF2/Keras
 The batch correlation regularization (BCR) technique adds a penalty loss
 if the inputs and outputs before the skip-connection of a specific feature element are correlated.
 The correlation coefficients are computed for each feature element seperatly across the current batch.
 
-~~For further information please read Ch.??? in [link to paper]().~~
-
 ## Usage
 
 ```py
 from keras_bcr import BatchCorrRegularizer
 import tensorflow as tf
 
 # The BCR layer is added before the addition of the skip-connection
@@ -46,25 +43,25 @@
 history = model.fit(X_train, y_train, verbose=1, epochs=2)
 ```
 
 
 ## Appendix
 
 ### Installation
-The `keras-bcr` [git repo](http://github.com/satzbeleg/keras-bcr) is available as [PyPi package](https://pypi.org/project/keras-bcr)
+The `keras-bcr` [git repo](http://github.com/ulf1/keras-bcr) is available as [PyPi package](https://pypi.org/project/keras-bcr)
 
 ```sh
 pip install keras-bcr
-pip install git+ssh://git@github.com/satzbeleg/keras-bcr.git
+pip install git+ssh://git@github.com/ulf1/keras-bcr.git
 ```
 
 ### Install a virtual environment
 
 ```sh
-python3.7 -m venv .venv
+python3 -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip
 pip install -r requirements.txt --no-cache-dir
 pip install -r requirements-dev.txt --no-cache-dir
 pip install -r requirements-demo.txt --no-cache-dir
 ```
 
@@ -75,15 +72,14 @@
 * Jupyter for the examples: `jupyter lab`
 * Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
 * Run Unit Tests: `PYTHONPATH=. pytest`
 
 Publish
 
 ```sh
-pandoc README.md --from markdown --to rst -s -o README.rst
 python setup.py sdist 
 twine upload -r pypi dist/*
 ```
 
 ### Clean up 
 
 ```sh
@@ -91,24 +87,21 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/keras-bcr/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/keras-bcr/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/keras-bcr/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/keras-bcr/compare/).
 
 
 ### Acknowledgements
-This work was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742). Project duration: 2020-2023.
-
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
-### Citation
-Please considering citing 
+### Maintenance
+- till 31.Aug.2023 (v0.2.0) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.3.0) the code repository is maintained by Ulf Hamster.
 
-```
-Forthcoming
-```
```

### Comparing `keras-bcr-0.2.0/keras_bcr/bcr.py` & `keras-bcr-0.3.0/keras_bcr/bcr.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     Example:
     --------
     The BatchCorrRegularizer must be integrated within a ResNet block. It
       cannot be attached between ResNet layers. Here is an example how to
       design a ResNet block using the Keras Functional API
 
     def ...(self, inputs, ...):
-        h = tf.keras.Dense(...)(h)
-        h = h = tf.keras.layers.Activation(...)(h)
+        h = tf.keras.layers.Dense(...)(h)
+        h = tf.keras.layers.Activation(...)(h)
         h = tf.keras.layers.Dropout(...)(h)
         h = BatchCorrRegularizer(bcr_rate)([h, inputs])
         outputs = tf.keras.layers.Add(...)([h, inputs])
         return outputs
     """
     def __init__(self, bcr_rate: float = 1e-6):
         super(BatchCorrRegularizer, self).__init__()
```

### Comparing `keras-bcr-0.2.0/setup.py` & `keras-bcr-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     raise RuntimeError("Unable to find version string.")
 
 
 setuptools.setup(
     name='keras-bcr',
     version=get_version("keras_bcr/__init__.py"),
     description='Batch Correlation Regularizer for TF2/Keras',
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/keras-bcr',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/keras-bcr',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['keras_bcr'],
     install_requires=[
         "tensorflow>=2.4.0,<3"
     ],
```

### Comparing `keras-bcr-0.2.0/test/test_bcr.py` & `keras-bcr-0.3.0/test/test_bcr.py`

 * *Files identical despite different names*

