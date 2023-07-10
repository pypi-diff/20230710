# Comparing `tmp/keras-cor-0.1.0.tar.gz` & `tmp/keras-cor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keras-cor-0.1.0.tar", last modified: Fri May 13 11:07:22 2022, max compression
+gzip compressed data, was "keras-cor-0.2.0.tar", last modified: Mon Jul 10 15:54:37 2023, max compression
```

## Comparing `keras-cor-0.1.0.tar` & `keras-cor-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-13 11:07:22.000000 keras-cor-0.1.0/
--rw-r--r--   0 uh         (501) staff       (20)    11340 2022-05-13 11:02:18.000000 keras-cor-0.1.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2022-05-13 11:02:18.000000 keras-cor-0.1.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)      506 2022-05-13 11:07:22.000000 keras-cor-0.1.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     3663 2022-05-13 11:02:18.000000 keras-cor-0.1.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-05-13 11:06:38.000000 keras-cor-0.1.0/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-13 11:07:22.000000 keras-cor-0.1.0/keras_cor/
--rw-r--r--   0 uh         (501) staff       (20)      106 2022-05-13 11:02:18.000000 keras-cor-0.1.0/keras_cor/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     2599 2022-05-13 11:02:18.000000 keras-cor-0.1.0/keras_cor/cor.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-13 11:07:22.000000 keras-cor-0.1.0/keras_cor.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)      506 2022-05-13 11:07:20.000000 keras-cor-0.1.0/keras_cor.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      314 2022-05-13 11:07:22.000000 keras-cor-0.1.0/keras_cor.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-05-13 11:07:20.000000 keras-cor-0.1.0/keras_cor.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       21 2022-05-13 11:07:21.000000 keras-cor-0.1.0/keras_cor.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       10 2022-05-13 11:07:21.000000 keras-cor-0.1.0/keras_cor.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-05-13 11:07:20.000000 keras-cor-0.1.0/keras_cor.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2022-05-13 11:07:22.000000 keras-cor-0.1.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)     1224 2022-05-13 11:02:18.000000 keras-cor-0.1.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-05-13 11:07:22.000000 keras-cor-0.1.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-05-13 11:02:18.000000 keras-cor-0.1.0/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     1389 2022-05-13 11:02:18.000000 keras-cor-0.1.0/test/test_cor.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:54:37.864073 keras-cor-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-07-10 08:50:52.000000 keras-cor-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 08:50:52.000000 keras-cor-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3802 2023-07-10 15:54:37.864073 keras-cor-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3240 2023-07-10 15:53:06.000000 keras-cor-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:54:37.864073 keras-cor-0.2.0/keras_cor/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      106 2023-07-10 14:25:30.000000 keras-cor-0.2.0/keras_cor/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2626 2023-07-10 08:50:52.000000 keras-cor-0.2.0/keras_cor/cor.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:54:37.864073 keras-cor-0.2.0/keras_cor.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3802 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      303 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       21 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       10 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:54:37.000000 keras-cor-0.2.0/keras_cor.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:54:37.864073 keras-cor-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1269 2023-07-10 14:25:30.000000 keras-cor-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:54:37.864073 keras-cor-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:50:52.000000 keras-cor-0.2.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1389 2023-07-10 08:50:52.000000 keras-cor-0.2.0/test/test_cor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `keras-cor-0.1.0/LICENSE` & `keras-cor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-cor-0.1.0/README.md` & `keras-cor-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/keras-cor.svg)](https://badge.fury.io/py/keras-cor)
 [![PyPi downloads](https://img.shields.io/pypi/dm/keras-cor)](https://img.shields.io/pypi/dm/keras-cor)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/satzbeleg/keras-cor.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/keras-cor/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/satzbeleg/keras-cor.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/keras-cor/context:python)
+
 
 # keras-cor : Correlated Outputs Regularization
 Add a regularization if the features/columns/neurons the hidden layer or output layer should be correlated. The vector with target correlation coefficient is computed before the optimization, and compared with correlation coefficients computed across the batch examples.
 
 ## Usage
 See [demo notebook](demo/Correlated%20Outputs%20Regularization.ipynb)
 
@@ -46,25 +45,25 @@
 rhos = pearson_vec(yhat)
 rhos
 ```
 
 ## Appendix
 
 ### Installation
-The `keras-cor` [git repo](http://github.com/satzbeleg/keras-cor) is available as [PyPi package](https://pypi.org/project/keras-cor)
+The `keras-cor` [git repo](http://github.com/ulf1/keras-cor) is available as [PyPi package](https://pypi.org/project/keras-cor)
 
 ```sh
 pip install keras-cor
-pip install git+ssh://git@github.com/satzbeleg/keras-cor.git
+pip install git+ssh://git@github.com/ulf1/keras-cor.git
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
 
@@ -75,15 +74,14 @@
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
@@ -91,12 +89,12 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/keras-cor/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/keras-cor/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/keras-cor/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/keras-cor/compare/).
```

### Comparing `keras-cor-0.1.0/keras_cor/cor.py` & `keras-cor-0.2.0/keras_cor/cor.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             h = tf.keras.layers.Dense(units=3)(h)
             h = tf.keras.layers.Activation("gelu")(h)
             h = CorrOutputsRegularizer(target_corrmat, cor_rate)(h)
             return h
     """
     def __init__(self, target_corr, cor_rate: float = 1e-3):
         super(CorrOutputsRegularizer, self).__init__()
-        self.target_corr = target_corr
+        self.target_corr = tf.cast(target_corr, dtype=tf.float32)
         self.cor_rate = cor_rate
 
     def call(self, h):
         d = self.target_corr - pearson_vec(h)
         d = tf.math.reduce_mean(tf.math.pow(d, 2))
         loss = self.cor_rate * d
         self.add_loss(loss)
```

### Comparing `keras-cor-0.1.0/setup.py` & `keras-cor-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     description=(
         "Add a regularization if the features/columns/neurons the hidden "
         "layer or output layer should be correlated. The vector with target "
         "correlation coefficient is computed before the optimization, "
         "and compared with correlation coefficients computed across the "
         "batch examples."
     ),
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/keras-cor',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/keras-cor',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['keras_cor'],
     install_requires=[
         "tensorflow>=2.4.0,<3"
     ],
```

### Comparing `keras-cor-0.1.0/test/test_cor.py` & `keras-cor-0.2.0/test/test_cor.py`

 * *Files identical despite different names*

