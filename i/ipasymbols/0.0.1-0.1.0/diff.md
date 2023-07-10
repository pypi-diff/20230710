# Comparing `tmp/ipasymbols-0.0.1.tar.gz` & `tmp/ipasymbols-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ipasymbols-0.0.1.tar", last modified: Thu Nov 25 18:24:58 2021, max compression
+gzip compressed data, was "ipasymbols-0.1.0.tar", last modified: Mon Jul 10 15:19:09 2023, max compression
```

## Comparing `ipasymbols-0.0.1.tar` & `ipasymbols-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/
--rw-r--r--   0 uh         (501) staff       (20)    11340 2021-11-25 09:16:12.000000 ipasymbols-0.0.1/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2021-11-25 18:23:40.000000 ipasymbols-0.0.1/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)     4801 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     3924 2021-11-25 18:20:09.000000 ipasymbols-0.0.1/README.md
--rw-r--r--   0 uh         (501) staff       (20)     4497 2021-11-25 18:21:09.000000 ipasymbols-0.0.1/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/ipasymbols/
--rw-r--r--   0 uh         (501) staff       (20)      108 2021-11-25 18:05:52.000000 ipasymbols-0.0.1/ipasymbols/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)    48234 2021-11-25 17:20:36.000000 ipasymbols-0.0.1/ipasymbols/ipasymbols.py
--rw-r--r--   0 uh         (501) staff       (20)     3920 2021-11-25 18:13:50.000000 ipasymbols-0.0.1/ipasymbols/utils.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/ipasymbols.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)     4801 2021-11-25 18:24:56.000000 ipasymbols-0.0.1/ipasymbols.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      348 2021-11-25 18:24:57.000000 ipasymbols-0.0.1/ipasymbols.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-11-25 18:24:56.000000 ipasymbols-0.0.1/ipasymbols.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       17 2021-11-25 18:24:56.000000 ipasymbols-0.0.1/ipasymbols.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       11 2021-11-25 18:24:56.000000 ipasymbols-0.0.1/ipasymbols.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-11-25 18:24:56.000000 ipasymbols-0.0.1/ipasymbols.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)       38 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)      939 2021-11-25 18:00:55.000000 ipasymbols-0.0.1/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-11-25 18:24:58.000000 ipasymbols-0.0.1/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2021-11-25 09:15:17.000000 ipasymbols-0.0.1/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     3524 2021-11-25 18:14:18.000000 ipasymbols-0.0.1/test/test_db.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5146 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     4808 2023-07-10 15:18:43.000000 ipasymbols-0.1.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/ipasymbols/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      108 2023-07-10 14:25:36.000000 ipasymbols-0.1.0/ipasymbols/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    48234 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/ipasymbols/ipasymbols.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3920 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/ipasymbols/utils.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/ipasymbols.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     5146 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      337 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       17 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       11 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:19:09.000000 ipasymbols-0.1.0/ipasymbols.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      983 2023-07-10 14:25:36.000000 ipasymbols-0.1.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:19:09.146946 ipasymbols-0.1.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3524 2023-07-10 10:01:21.000000 ipasymbols-0.1.0/test/test_db.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ipasymbols-0.0.1/LICENSE` & `ipasymbols-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipasymbols-0.0.1/README.md` & `ipasymbols-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI version](https://badge.fury.io/py/ipasymbols.svg)](https://badge.fury.io/py/ipasymbols)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/linguistik/ipasymbols.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/linguistik/ipasymbols/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/linguistik/ipasymbols.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/linguistik/ipasymbols/context:python)
+[![PyPi downloads](https://img.shields.io/pypi/dm/ipasymbols)](https://img.shields.io/pypi/dm/ipasymbols)
+[![DOI](https://zenodo.org/badge/431771809.svg)](https://zenodo.org/badge/latestdoi/431771809)
 
 
-# ipasymbols
+# ipasymbols: Properties of IPA symbols for data analysis
 A simple JSON database to lookup the properties of IPA symbols.
 
 ## Warning: Under Development! (25.Nov.2021)
 Version `0.0.*` is **not** ready to use. Non-Pulmonic consonants, affricates, co-articulated consonants, and dipthongs are **not** implemented yet. This kind of software is very prone to human errors, and required unit tests are not implemented so far.
 
 ## Usage
 
@@ -72,19 +72,19 @@
 mydict = ipasymbols.db
 ```
 
 
 ## Appendix
 
 ### Installation
-The `ipasymbols` [git repo](http://github.com/linguistik/ipasymbols) is available as [PyPi package](https://pypi.org/project/ipasymbols)
+The `ipasymbols` [git repo](http://github.com/ulf1/ipasymbols) is available as [PyPi package](https://pypi.org/project/ipasymbols)
 
 ```sh
 pip install ipasymbols
-pip install git+ssh://git@github.com/linguistik/ipasymbols.git
+pip install git+ssh://git@github.com/ulf1/ipasymbols.git
 ```
 
 ### Install a virtual environment
 
 ```sh
 python3 -m venv .venv
 source .venv/bin/activate
@@ -101,15 +101,14 @@
 * Jupyter for the examples: `jupyter lab`
 * Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g'),./ipasymbols/ipasymbols.py`
 * Run Unit Tests: `PYTHONPATH=. pytest`
 
 Publish
 
 ```sh
-pandoc README.md --from markdown --to rst -s -o README.rst
 python setup.py sdist 
 twine upload -r pypi dist/*
 ```
 
 ### Clean up 
 
 ```sh
@@ -117,12 +116,36 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/linguistik/ipasymbols/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/ipasymbols/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/linguistik/ipasymbols/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/ipasymbols/compare/).
+
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.0.1) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.1.0) the code repository is maintained by Ulf Hamster.
+
+### Citation
+You can cite the following paper if you want to use this repository in your research work.
+
+```
+@inproceedings{hamster-2022-everybody,
+    title = "Everybody likes short sentences - A Data Analysis for the Text Complexity {DE} Challenge 2022",
+    author = "Hamster, Ulf A.",
+    booktitle = "Proceedings of the GermEval 2022 Workshop on Text Complexity Assessment of German Text",
+    month = sep,
+    year = "2022",
+    address = "Potsdam, Germany",
+    publisher = "Association for Computational Linguistics",
+    url = "https://aclanthology.org/2022.germeval-1.2",
+    pages = "10--14",
+}
+```
```

### Comparing `ipasymbols-0.0.1/ipasymbols/ipasymbols.py` & `ipasymbols-0.1.0/ipasymbols/ipasymbols.py`

 * *Files identical despite different names*

### Comparing `ipasymbols-0.0.1/ipasymbols/utils.py` & `ipasymbols-0.1.0/ipasymbols/utils.py`

 * *Files identical despite different names*

### Comparing `ipasymbols-0.0.1/setup.py` & `ipasymbols-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     raise RuntimeError("Unable to find version string.")
 
 
 setuptools.setup(
     name='ipasymbols',
     version=get_version("ipasymbols/__init__.py"),
     description='Properties of IPA symbols for data analysis.',
-    long_description=read('README.rst'),
-    url='http://github.com/linguistik/ipasymbols',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/ipasymbols',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['ipasymbols'],
     install_requires=[
         'numpy>=1.21.4,<2'
     ],
```

### Comparing `ipasymbols-0.0.1/test/test_db.py` & `ipasymbols-0.1.0/test/test_db.py`

 * *Files identical despite different names*

