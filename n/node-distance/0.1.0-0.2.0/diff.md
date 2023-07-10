# Comparing `tmp/node-distance-0.1.0.tar.gz` & `tmp/node-distance-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/node-distance-0.1.0.tar", last modified: Wed Dec  1 16:40:30 2021, max compression
+gzip compressed data, was "node-distance-0.2.0.tar", last modified: Mon Jul 10 15:36:31 2023, max compression
```

## Comparing `node-distance-0.1.0.tar` & `node-distance-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,21 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/.github/
--rw-r--r--   0 uh         (501) staff       (20)       15 2021-12-01 11:42:52.000000 node-distance-0.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/.github/workflows/
--rw-r--r--   0 uh         (501) staff       (20)      806 2021-12-01 15:53:59.000000 node-distance-0.1.0/.github/workflows/syntax-and-unit-tests.yml
--rw-r--r--   0 uh         (501) staff       (20)     1279 2021-12-01 16:39:59.000000 node-distance-0.1.0/.gitignore
--rw-r--r--   0 uh         (501) staff       (20)      449 2021-12-01 11:41:19.000000 node-distance-0.1.0/.zenodo.json
--rw-r--r--   0 uh         (501) staff       (20)       43 2021-12-01 11:38:39.000000 node-distance-0.1.0/CHANGES.md
--rw-r--r--   0 uh         (501) staff       (20)    11340 2021-12-01 11:38:39.000000 node-distance-0.1.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2021-12-01 11:38:38.000000 node-distance-0.1.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)     6601 2021-12-01 16:40:30.000000 node-distance-0.1.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     5599 2021-12-01 15:32:59.000000 node-distance-0.1.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)     6218 2021-12-01 16:37:53.000000 node-distance-0.1.0/README.rst
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/demo/
--rw-r--r--   0 uh         (501) staff       (20)   137456 2021-12-01 16:36:28.000000 node-distance-0.1.0/demo/Usage Examples.ipynb
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/node_distance/
--rw-r--r--   0 uh         (501) staff       (20)      260 2021-12-01 15:48:30.000000 node-distance-0.1.0/node_distance/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     1605 2021-12-01 14:27:27.000000 node-distance-0.1.0/node_distance/distances.py
--rw-r--r--   0 uh         (501) staff       (20)     2697 2021-12-01 15:48:44.000000 node-distance-0.1.0/node_distance/distributions.py
--rw-r--r--   0 uh         (501) staff       (20)     2528 2021-12-01 15:48:56.000000 node-distance-0.1.0/node_distance/extract.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/node_distance.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)     6601 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      576 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)       36 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/requires.txt
--rw-r--r--   0 uh         (501) staff       (20)       14 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2021-12-01 16:40:29.000000 node-distance-0.1.0/node_distance.egg-info/zip-safe
--rw-r--r--   0 uh         (501) staff       (20)      171 2021-12-01 15:25:28.000000 node-distance-0.1.0/requirements-demo.txt
--rw-r--r--   0 uh         (501) staff       (20)      135 2021-12-01 11:38:39.000000 node-distance-0.1.0/requirements-dev.txt
--rw-r--r--   0 uh         (501) staff       (20)       69 2021-12-01 15:34:08.000000 node-distance-0.1.0/requirements.txt
--rw-r--r--   0 uh         (501) staff       (20)       38 2021-12-01 16:40:30.000000 node-distance-0.1.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)     1076 2021-12-01 16:39:40.000000 node-distance-0.1.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2021-12-01 16:40:30.000000 node-distance-0.1.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2021-12-01 11:37:16.000000 node-distance-0.1.0/test/__init__.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:36:31.498698 node-distance-0.2.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11340 2023-07-10 14:26:44.000000 node-distance-0.2.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 14:26:44.000000 node-distance-0.2.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6889 2023-07-10 15:36:31.498698 node-distance-0.2.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6471 2023-07-10 15:36:03.000000 node-distance-0.2.0/README.md
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:36:31.494698 node-distance-0.2.0/node_distance/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      260 2023-07-10 14:26:44.000000 node-distance-0.2.0/node_distance/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1605 2023-07-10 14:26:44.000000 node-distance-0.2.0/node_distance/distances.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2697 2023-07-10 14:26:44.000000 node-distance-0.2.0/node_distance/distributions.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2528 2023-07-10 14:26:44.000000 node-distance-0.2.0/node_distance/extract.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:36:31.498698 node-distance-0.2.0/node_distance.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     6889 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      380 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       36 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/requires.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       14 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:36:31.000000 node-distance-0.2.0/node_distance.egg-info/zip-safe
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:36:31.498698 node-distance-0.2.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1121 2023-07-10 14:26:44.000000 node-distance-0.2.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:36:31.498698 node-distance-0.2.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 14:26:44.000000 node-distance-0.2.0/test/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `node-distance-0.1.0/LICENSE` & `node-distance-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `node-distance-0.1.0/README.md` & `node-distance-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI version](https://badge.fury.io/py/node-distance.svg)](https://badge.fury.io/py/node-distance)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/satzbeleg/node-distance.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/node-distance/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/satzbeleg/node-distance.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/satzbeleg/node-distance/context:python)
+[![PyPi downloads](https://img.shields.io/pypi/dm/node-distance)](https://img.shields.io/pypi/dm/node-distance)
+[![DOI](https://zenodo.org/badge/433801845.svg)](https://zenodo.org/badge/latestdoi/433801845)
 
 
-# node-distance
+# node-distance: Tree node distances as features
 Compute distance between all nodes of a tree, and estimate an histogram that can be used as features for other models.
 
 ### Toy Text Corpus
 
 ```py
 corpus = "Als Ada Lovelace auf einem Ball den Mathematiker Charles Babbage traf, der sie einlud, die von ihm erfundene „Differenzmaschine“ anzusehen, war sie hellauf begeistert. Die Maschine konnte selbstständig addieren und subtrahieren, doch Ada war klar, dass die Möglichkeiten damit noch lange nicht erschöpft waren. Sie träumte davon, dass eine solche Maschine eines Tages sogar Musik abspielen könnte, und ersann so die Idee eines modernen Computers. 1845 legte sie den ersten Algorithmus zur maschinellen Berechnung der Bernoulli-Zahlen vor und wird daher von vielen als erste Computerprogrammiererin der Welt gefeiert."
 ```
@@ -98,26 +98,26 @@
 plt.show();
 ```
 
 
 ## Appendix
 
 ### Installation
-The `node-distance` [git repo](http://github.com/satzbeleg/node-distance) is available as [PyPi package](https://pypi.org/project/node-distance)
+The `node-distance` [git repo](http://github.com/ulf1/node-distance) is available as [PyPi package](https://pypi.org/project/node-distance)
 
 ```sh
 pip install node-distance
-pip install git+ssh://git@github.com/satzbeleg/node-distance.git
+pip install git+ssh://git@github.com/ulf1/node-distance.git
 ```
 
 ### Install a virtual environment
 It is recommended to install python packages into a seperate virtual environement. (If your git repo is stored in a folder with whitespaces, then don't use the subfolder `.venv`. Use an absolute path without whitespaces.)
 
 ```sh
-python3.7 -m venv .venv
+python3 -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip
 pip install -r requirements.txt --no-cache-dir
 pip install -r requirements-dev.txt --no-cache-dir
 pip install -r requirements-demo.txt --no-cache-dir
 ```
 
@@ -134,28 +134,50 @@
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
 find . -type f -name "*.pyc" | xargs rm
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
-
 ### Support
-Please [open an issue](https://github.com/satzbeleg/node-distance/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/node-distance/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/node-distance/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/node-distance/compare/).
+
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.1.0) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by Ulf Hamster.
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

### Comparing `node-distance-0.1.0/README.rst` & `node-distance-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,201 +1,198 @@
-|PyPI version| |Total alerts| |Language grade: Python|
+Metadata-Version: 2.1
+Name: node-distance
+Version: 0.2.0
+Summary: Compute distance between all nodes of a tree, and estimate an histogram that can be used as features for other models.
+Home-page: http://github.com/ulf1/node-distance
+Author: Ulf Hamster
+Author-email: 554c46@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/node-distance.svg)](https://badge.fury.io/py/node-distance)
+[![PyPi downloads](https://img.shields.io/pypi/dm/node-distance)](https://img.shields.io/pypi/dm/node-distance)
+[![DOI](https://zenodo.org/badge/433801845.svg)](https://zenodo.org/badge/latestdoi/433801845)
+
+
+# node-distance: Tree node distances as features
+Compute distance between all nodes of a tree, and estimate an histogram that can be used as features for other models.
+
+### Toy Text Corpus
+
+```py
+corpus = "Als Ada Lovelace auf einem Ball den Mathematiker Charles Babbage traf, der sie einlud, die von ihm erfundene „Differenzmaschine“ anzusehen, war sie hellauf begeistert. Die Maschine konnte selbstständig addieren und subtrahieren, doch Ada war klar, dass die Möglichkeiten damit noch lange nicht erschöpft waren. Sie träumte davon, dass eine solche Maschine eines Tages sogar Musik abspielen könnte, und ersann so die Idee eines modernen Computers. 1845 legte sie den ersten Algorithmus zur maschinellen Berechnung der Bernoulli-Zahlen vor und wird daher von vielen als erste Computerprogrammiererin der Welt gefeiert."
+```
+(Source: DWDS, Wort des Tages, "Algorithmus, der", 27.11.2021, URL: https://www.dwds.de/adt )
+
+
+### Extract the graph edges from a dependency tree with SpaCy/Stanza/Trankit
+- We assume that NodeIDs are numbers `[1,2,3,...]` starting with 1. 
+  The NodeIDs are equivalent to the TokenIDs in Conll-U.
+- An graph edge is a tuple `(ParentID, NodeID)`
 
-node-distance
-=============
-
-Compute distance between all nodes of a tree, and estimate an histogram
-that can be used as features for other models.
-
-Toy Text Corpus
----------------
-
-.. code:: py
-
-   corpus = "Als Ada Lovelace auf einem Ball den Mathematiker Charles Babbage traf, der sie einlud, die von ihm erfundene „Differenzmaschine“ anzusehen, war sie hellauf begeistert. Die Maschine konnte selbstständig addieren und subtrahieren, doch Ada war klar, dass die Möglichkeiten damit noch lange nicht erschöpft waren. Sie träumte davon, dass eine solche Maschine eines Tages sogar Musik abspielen könnte, und ersann so die Idee eines modernen Computers. 1845 legte sie den ersten Algorithmus zur maschinellen Berechnung der Bernoulli-Zahlen vor und wird daher von vielen als erste Computerprogrammiererin der Welt gefeiert."
-
-(Source: DWDS, Wort des Tages, “Algorithmus, der”, 27.11.2021, URL:
-https://www.dwds.de/adt )
-
-Extract the graph edges from a dependency tree with SpaCy/Stanza/Trankit
-------------------------------------------------------------------------
-
--  We assume that NodeIDs are numbers ``[1,2,3,...]`` starting with 1.
-   The NodeIDs are equivalent to the TokenIDs in Conll-U.
--  An graph edge is a tuple ``(ParentID, NodeID)``
 
 Example, SpaCy:
-
-.. code:: py
-
-   # load the SpaCy model
-   import de_dep_news_trf
-   model = de_dep_news_trf.load()
-   # extract the edges for each sentence
-   import node_distance as nd
-   all_edges, num_nodes = nd.extract_edges_from_spacy(corpus, model)
+```py
+# load the SpaCy model
+import de_dep_news_trf
+model = de_dep_news_trf.load()
+# extract the edges for each sentence
+import node_distance as nd
+all_edges, num_nodes = nd.extract_edges_from_spacy(corpus, model)
+```
 
 Example, stanza:
-
-.. code:: py
-
-   # load the stanza model
-   import stanza
-   model = stanza.Pipeline(
-       lang='de', processors='tokenize,mwt,pos,lemma,depparse',
-       tokenize_pretokenized=False)
-   # extract the edges for each sentence
-   import node_distance as nd
-   all_edges, num_nodes = nd.extract_edges_from_stanza(corpus, model)
+```py
+# load the stanza model
+import stanza
+model = stanza.Pipeline(
+    lang='de', processors='tokenize,mwt,pos,lemma,depparse',
+    tokenize_pretokenized=False)
+# extract the edges for each sentence
+import node_distance as nd
+all_edges, num_nodes = nd.extract_edges_from_stanza(corpus, model)
+```
 
 Example, trankit:
+```py
+# load the trankit model
+import trankit
+model = trankit.Pipeline(lang='german', gpu=False, cache_dir='./cache')
+# extract the edges for each sentence
+import node_distance as nd
+all_edges, num_nodes = nd.extract_edges_from_trankit(corpus, model)
+```
+
+`num_nodes` with the number of tokens/nodes in each sentence.
+`all_edges` contains lists of edges for each sentence, e.g.
+```py
+# Edges of the 3rd sentence
+edges = all_edges[2]
+# Edge between the 6th token/node and its parent node
+edge = edges[6]
+parent_id, node_id = edge
+```
 
-.. code:: py
-
-   # load the trankit model
-   import trankit
-   model = trankit.Pipeline(lang='german', gpu=False, cache_dir='./cache')
-   # extract the edges for each sentence
-   import node_distance as nd
-   all_edges, num_nodes = nd.extract_edges_from_trankit(corpus, model)
-
-``num_nodes`` with the number of tokens/nodes in each sentence.
-``all_edges`` contains lists of edges for each sentence, e.g.
-
-.. code:: py
-
-   # Edges of the 3rd sentence
-   edges = all_edges[2]
-   # Edge between the 6th token/node and its parent node
-   edge = edges[6]
-   parent_id, node_id = edge
-
-Compute Shortest Paths between Nodes
-------------------------------------
-
+### Compute Shortest Paths between Nodes
 Compute node distances and the corresponding token distances
 
-.. code:: py
+```py
+import node_distance as nd
+nodedist, tokendist, indicies = nd.node_token_distances(all_edges, num_nodes, cutoff=25)
+```
 
-   import node_distance as nd
-   nodedist, tokendist, indicies = nd.node_token_distances(all_edges, num_nodes, cutoff=25)
-
-Histograms as Features
-----------------------
+### Histograms as Features
 
 The Distribution of node distances:
-
-.. code:: py
-
-   import node_distance as nd
-   xobs, pdf, _ = nd.nodedist_distribution(nodedist, xmin=1, xmax=12)
-
-   import matplotlib.pyplot as plt
-   plt.bar(xobs, pdf);
-   plt.title("distribution of node distances");
-   plt.xlabel("node distance");
-   plt.ylabel("PDF");
-   plt.show();
+```py
+import node_distance as nd
+xobs, pdf, _ = nd.nodedist_distribution(nodedist, xmin=1, xmax=12)
+
+import matplotlib.pyplot as plt
+plt.bar(xobs, pdf);
+plt.title("distribution of node distances");
+plt.xlabel("node distance");
+plt.ylabel("PDF");
+plt.show();
+```
 
 Distribution of token distance vs node distance:
-
-.. code:: py
-
-   import node_distance as nd
-   xobs, pdf, _ = nd.tokenvsnode_distribution(tokendist, nodedist, xmin=-5, xmax=15)
-
-   import matplotlib.pyplot as plt
-   plt.bar(xobs, pdf);
-   plt.title("Distribution of token distance vs node distance");
-   plt.xlabel("token distance minus node distance");
-   plt.ylabel("PDF");
-   plt.show();
-
-Appendix
---------
-
-Installation
-~~~~~~~~~~~~
-
-The ``node-distance`` `git
-repo <http://github.com/satzbeleg/node-distance>`__ is available as
-`PyPi package <https://pypi.org/project/node-distance>`__
-
-.. code:: sh
-
-   pip install node-distance
-   pip install git+ssh://git@github.com/satzbeleg/node-distance.git
-
-Install a virtual environment
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-It is recommended to install python packages into a seperate virtual
-environement. (If your git repo is stored in a folder with whitespaces,
-then don’t use the subfolder ``.venv``. Use an absolute path without
-whitespaces.)
-
-.. code:: sh
-
-   python3.7 -m venv .venv
-   source .venv/bin/activate
-   pip install --upgrade pip
-   pip install -r requirements.txt --no-cache-dir
-   pip install -r requirements-dev.txt --no-cache-dir
-   pip install -r requirements-demo.txt --no-cache-dir
-
-The usage example and demo notebooks might require spacy, stanza and
-trankit to be installed. You should download the pretrained models
-beforehand, e.g. pretrained models for German:
-
-.. code:: sh
-
-   python -m spacy download de_dep_news_trf
-   python -c "import stanza; stanza.download(lang='de')"
-   python -c "import trankit; trankit.Pipeline(lang='german', gpu=False, cache_dir='./cache')"
-
-Python commands
-~~~~~~~~~~~~~~~
-
--  Jupyter for the examples: ``jupyter lab``
--  Check syntax:
-   ``flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')``
--  Run Unit Tests: ``PYTHONPATH=. pytest``
+```py
+import node_distance as nd
+xobs, pdf, _ = nd.tokenvsnode_distribution(tokendist, nodedist, xmin=-5, xmax=15)
+
+import matplotlib.pyplot as plt
+plt.bar(xobs, pdf);
+plt.title("Distribution of token distance vs node distance");
+plt.xlabel("token distance minus node distance");
+plt.ylabel("PDF");
+plt.show();
+```
+
+
+## Appendix
+
+### Installation
+The `node-distance` [git repo](http://github.com/ulf1/node-distance) is available as [PyPi package](https://pypi.org/project/node-distance)
+
+```sh
+pip install node-distance
+pip install git+ssh://git@github.com/ulf1/node-distance.git
+```
+
+### Install a virtual environment
+It is recommended to install python packages into a seperate virtual environement. (If your git repo is stored in a folder with whitespaces, then don't use the subfolder `.venv`. Use an absolute path without whitespaces.)
+
+```sh
+python3 -m venv .venv
+source .venv/bin/activate
+pip install --upgrade pip
+pip install -r requirements.txt --no-cache-dir
+pip install -r requirements-dev.txt --no-cache-dir
+pip install -r requirements-demo.txt --no-cache-dir
+```
+
+The usage example and demo notebooks might require spacy, stanza and trankit to be installed. You should download the pretrained models beforehand, e.g. pretrained models for German:
+
+```sh
+python -m spacy download de_dep_news_trf
+python -c "import stanza; stanza.download(lang='de')"
+python -c "import trankit; trankit.Pipeline(lang='german', gpu=False, cache_dir='./cache')"
+```
+
+### Python commands
+
+* Jupyter for the examples: `jupyter lab`
+* Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
+* Run Unit Tests: `PYTHONPATH=. pytest`
 
 Publish
 
-.. code:: sh
+```sh
+python setup.py sdist 
+twine upload -r pypi dist/*
+```
+
+### Clean up 
+
+```sh
+find . -type f -name "*.pyc" | xargs rm
+find . -type d -name "__pycache__" | xargs rm -r
+rm -r .pytest_cache
+rm -r .venv
+```
+
+### Support
+Please [open an issue](https://github.com/ulf1/node-distance/issues/new) for support.
+
+
+### Contributing
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/node-distance/compare/).
+
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.1.0) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.2.0) the code repository is maintained by Ulf Hamster.
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
+
 
-   pandoc README.md --from markdown --to rst -s -o README.rst
-   python setup.py sdist 
-   twine upload -r pypi dist/*
-
-Clean up
-~~~~~~~~
-
-.. code:: sh
-
-   find . -type f -name "*.pyc" | xargs rm
-   find . -type d -name "__pycache__" | xargs rm -r
-   rm -r .pytest_cache
-   rm -r .venv
-
-Support
-~~~~~~~
-
-Please `open an
-issue <https://github.com/satzbeleg/node-distance/issues/new>`__ for
-support.
-
-Contributing
-~~~~~~~~~~~~
-
-Please contribute using `Github
-Flow <https://guides.github.com/introduction/flow/>`__. Create a branch,
-add commits, and `open a pull
-request <https://github.com/satzbeleg/node-distance/compare/>`__.
-
-.. |PyPI version| image:: https://badge.fury.io/py/node-distance.svg
-   :target: https://badge.fury.io/py/node-distance
-.. |Total alerts| image:: https://img.shields.io/lgtm/alerts/g/satzbeleg/node-distance.svg?logo=lgtm&logoWidth=18
-   :target: https://lgtm.com/projects/g/satzbeleg/node-distance/alerts/
-.. |Language grade: Python| image:: https://img.shields.io/lgtm/grade/python/g/satzbeleg/node-distance.svg?logo=lgtm&logoWidth=18
-   :target: https://lgtm.com/projects/g/satzbeleg/node-distance/context:python
```

### Comparing `node-distance-0.1.0/node_distance/distances.py` & `node-distance-0.2.0/node_distance/distances.py`

 * *Files identical despite different names*

### Comparing `node-distance-0.1.0/node_distance/distributions.py` & `node-distance-0.2.0/node_distance/distributions.py`

 * *Files identical despite different names*

### Comparing `node-distance-0.1.0/node_distance/extract.py` & `node-distance-0.2.0/node_distance/extract.py`

 * *Files identical despite different names*

### Comparing `node-distance-0.1.0/setup.py` & `node-distance-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 setuptools.setup(
     name='node-distance',
     version=get_version("node_distance/__init__.py"),
     description=(
         "Compute distance between all nodes of a tree, and estimate an "
         "histogram that can be used as features for other models."),
-    long_description=read('README.rst'),
-    url='http://github.com/satzbeleg/node-distance',
+    long_description=read('README.md'),
+    long_description_content_type='text/markdown',
+    url='http://github.com/ulf1/node-distance',
     author='Ulf Hamster',
     author_email='554c46@gmail.com',
     license='Apache License 2.0',
     packages=['node_distance'],
     install_requires=[
         'numpy>=1.19.5,<2',
         'networkx>=2.5.1,<3'
```

