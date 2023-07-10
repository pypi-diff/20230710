# Comparing `tmp/treesimi-0.2.0.tar.gz` & `tmp/treesimi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/treesimi-0.2.0.tar", last modified: Wed Sep 21 13:42:53 2022, max compression
+gzip compressed data, was "treesimi-0.3.0.tar", last modified: Mon Jul 10 15:28:37 2023, max compression
```

## Comparing `treesimi-0.2.0.tar` & `treesimi-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-09-21 13:42:53.000000 treesimi-0.2.0/
--rw-r--r--   0 uh         (501) staff       (20)    11341 2022-09-21 13:39:23.000000 treesimi-0.2.0/LICENSE
--rw-r--r--   0 uh         (501) staff       (20)       65 2022-09-21 13:39:23.000000 treesimi-0.2.0/MANIFEST.in
--rw-r--r--   0 uh         (501) staff       (20)      285 2022-09-21 13:42:53.000000 treesimi-0.2.0/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)     6787 2022-09-21 13:39:23.000000 treesimi-0.2.0/README.md
--rw-r--r--   0 uh         (501) staff       (20)     7565 2022-09-21 13:42:47.000000 treesimi-0.2.0/README.rst
--rw-r--r--   0 uh         (501) staff       (20)       38 2022-09-21 13:42:53.000000 treesimi-0.2.0/setup.cfg
--rw-r--r--   0 uh         (501) staff       (20)      946 2022-09-21 13:39:23.000000 treesimi-0.2.0/setup.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-09-21 13:42:53.000000 treesimi-0.2.0/test/
--rw-r--r--   0 uh         (501) staff       (20)        0 2022-09-21 13:39:23.000000 treesimi-0.2.0/test/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     2309 2022-09-21 13:39:23.000000 treesimi-0.2.0/test/test_convert.py
--rw-r--r--   0 uh         (501) staff       (20)      393 2022-09-21 13:39:23.000000 treesimi-0.2.0/test/test_encode.py
--rw-r--r--   0 uh         (501) staff       (20)     1963 2022-09-21 13:39:23.000000 treesimi-0.2.0/test/test_extract.py
--rw-r--r--   0 uh         (501) staff       (20)     3045 2022-09-21 13:39:23.000000 treesimi-0.2.0/test/test_shingleset.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-09-21 13:42:53.000000 treesimi-0.2.0/treesimi/
--rw-r--r--   0 uh         (501) staff       (20)      500 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/__init__.py
--rw-r--r--   0 uh         (501) staff       (20)     8020 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/convert.py
--rw-r--r--   0 uh         (501) staff       (20)      802 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/encode.py
--rw-r--r--   0 uh         (501) staff       (20)     7006 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/extract.py
--rw-r--r--   0 uh         (501) staff       (20)     2710 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/shingleset.py
--rw-r--r--   0 uh         (501) staff       (20)     3899 2022-09-21 13:39:23.000000 treesimi-0.2.0/treesimi/utils_for_depparser.py
-drwxr-xr-x   0 uh         (501) staff       (20)        0 2022-09-21 13:42:53.000000 treesimi-0.2.0/treesimi.egg-info/
--rw-r--r--   0 uh         (501) staff       (20)      285 2022-09-21 13:42:52.000000 treesimi-0.2.0/treesimi.egg-info/PKG-INFO
--rw-r--r--   0 uh         (501) staff       (20)      442 2022-09-21 13:42:52.000000 treesimi-0.2.0/treesimi.egg-info/SOURCES.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-09-21 13:42:52.000000 treesimi-0.2.0/treesimi.egg-info/dependency_links.txt
--rw-r--r--   0 uh         (501) staff       (20)        9 2022-09-21 13:42:52.000000 treesimi-0.2.0/treesimi.egg-info/top_level.txt
--rw-r--r--   0 uh         (501) staff       (20)        1 2022-09-21 13:42:52.000000 treesimi-0.2.0/treesimi.egg-info/zip-safe
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:28:37.413969 treesimi-0.3.0/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)    11341 2023-07-10 08:47:51.000000 treesimi-0.3.0/LICENSE
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       65 2023-07-10 08:47:51.000000 treesimi-0.3.0/MANIFEST.in
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     7538 2023-07-10 15:28:37.413969 treesimi-0.3.0/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     7197 2023-07-10 14:53:06.000000 treesimi-0.3.0/README.md
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)       38 2023-07-10 15:28:37.413969 treesimi-0.3.0/setup.cfg
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      970 2023-07-10 14:24:54.000000 treesimi-0.3.0/setup.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:28:37.413969 treesimi-0.3.0/test/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        0 2023-07-10 08:47:51.000000 treesimi-0.3.0/test/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2309 2023-07-10 08:47:51.000000 treesimi-0.3.0/test/test_convert.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      393 2023-07-10 08:47:51.000000 treesimi-0.3.0/test/test_encode.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     1963 2023-07-10 08:47:51.000000 treesimi-0.3.0/test/test_extract.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3045 2023-07-10 08:47:51.000000 treesimi-0.3.0/test/test_shingleset.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:28:37.413969 treesimi-0.3.0/treesimi/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      500 2023-07-10 14:24:54.000000 treesimi-0.3.0/treesimi/__init__.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     8020 2023-07-10 08:47:51.000000 treesimi-0.3.0/treesimi/convert.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      802 2023-07-10 08:47:51.000000 treesimi-0.3.0/treesimi/encode.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     7006 2023-07-10 08:47:51.000000 treesimi-0.3.0/treesimi/extract.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     2710 2023-07-10 08:47:51.000000 treesimi-0.3.0/treesimi/shingleset.py
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     3899 2023-07-10 08:47:51.000000 treesimi-0.3.0/treesimi/utils_for_depparser.py
+drwxrwxr-x   0 hamster   (1000) hamster   (1000)        0 2023-07-10 15:28:37.413969 treesimi-0.3.0/treesimi.egg-info/
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)     7538 2023-07-10 15:28:37.000000 treesimi-0.3.0/treesimi.egg-info/PKG-INFO
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)      431 2023-07-10 15:28:37.000000 treesimi-0.3.0/treesimi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:28:37.000000 treesimi-0.3.0/treesimi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        9 2023-07-10 15:28:37.000000 treesimi-0.3.0/treesimi.egg-info/top_level.txt
+-rw-rw-r--   0 hamster   (1000) hamster   (1000)        1 2023-07-10 15:28:37.000000 treesimi-0.3.0/treesimi.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `treesimi-0.2.0/LICENSE` & `treesimi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/README.md` & `treesimi-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI version](https://badge.fury.io/py/treesimi.svg)](https://badge.fury.io/py/treesimi)
 [![PyPi downloads](https://img.shields.io/pypi/dm/treesimi)](https://img.shields.io/pypi/dm/treesimi)
 [![DOI](https://zenodo.org/badge/318838452.svg)](https://zenodo.org/badge/latestdoi/318838452)
 
 
-# treesimi
+# treesimi: Shingling for measuring tree similarity
 Compute similarity between trees, e.g. dependency trees
 
 
 ## Convert an Adjacency List into a Nested Set Table
 For example, CoNLL-U's `['id', 'head']` fields form an adjacency list of a dependency tree.
 Traversing an adjacency list is slower than reading a nested set.
 Thus, converting a adjacency list to a nested set table once, makes sense if we need to read the three several times lateron.
@@ -134,33 +134,33 @@
 #   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, '[MASK]']]
 # ]
 ```
 
 ## Demo Notebooks about Shingling for MinHash
 We recommend using the `mmh3` hash function, and 32 permutations in `datasketch.MinHash`.
 
-- [Create subtrees as shingle sets](https://github.com/satzbeleg/treesimi/blob/master/demo/Create%20subtrees%20as%20shingle%20sets.ipynb)
-- [Jaccard Similarity between Dependency Trees](https://github.com/satzbeleg/treesimi/blob/master/demo/Jaccard%20Similarity%20between%20Dependency%20Trees.ipynb)
-- [Shingle Dependency Trees for datasketch's Minhash](https://github.com/satzbeleg/treesimi/blob/master/demo/Shingle%20Dependency%20Trees%20for%20datasketch's%20Minhash.ipynb)
+- [Create subtrees as shingle sets](https://github.com/ulf1/treesimi/blob/master/demo/Create%20subtrees%20as%20shingle%20sets.ipynb)
+- [Jaccard Similarity between Dependency Trees](https://github.com/ulf1/treesimi/blob/master/demo/Jaccard%20Similarity%20between%20Dependency%20Trees.ipynb)
+- [Shingle Dependency Trees for datasketch's Minhash](https://github.com/ulf1/treesimi/blob/master/demo/Shingle%20Dependency%20Trees%20for%20datasketch's%20Minhash.ipynb)
 
 Start jupyter to run the demo notebook
 
 ```sh
 source .venv/bin/activate
 jupyter lab
 ```
 
 ## Appendix
 
 ### Installation
-The `treesimi` [git repo](http://github.com/satzbeleg/treesimi) is available as [PyPi package](https://pypi.org/project/treesimi)
+The `treesimi` [git repo](http://github.com/ulf1/treesimi) is available as [PyPi package](https://pypi.org/project/treesimi)
 
 ```sh
 pip install treesimi
-pip install git+ssh://git@github.com/satzbeleg/treesimi.git
+pip install git+ssh://git@github.com/ulf1/treesimi.git
 ```
 
 ### Commands
 Install a virtual environment
 
 ```sh
 python3 -m venv .venv
@@ -177,15 +177,14 @@
 
 * Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
 * Run Unit Tests: `pytest`
 
 Publish
 
 ```sh
-pandoc README.md --from markdown --to rst -s -o README.rst
 python setup.py sdist 
 twine upload -r pypi dist/*
 ```
 
 ### Clean up 
 
 ```sh
@@ -193,12 +192,20 @@
 find . -type d -name "__pycache__" | xargs rm -r
 rm -r .pytest_cache
 rm -r .venv
 ```
 
 
 ### Support
-Please [open an issue](https://github.com/satzbeleg/treesimi/issues/new) for support.
+Please [open an issue](https://github.com/ulf1/treesimi/issues/new) for support.
 
 
 ### Contributing
-Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/satzbeleg/treesimi/compare/).
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/treesimi/compare/).
+
+
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
+
+### Maintenance
+- till 31.Aug.2023 (v0.2.0) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.3.0) the code repository is maintained by Ulf Hamster.
```

### Comparing `treesimi-0.2.0/README.rst` & `treesimi-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,258 +1,226 @@
-|PyPI version| |PyPi downloads| |DOI|
+Metadata-Version: 2.1
+Name: treesimi
+Version: 0.3.0
+Summary: Compute similarity between netsted set based trees.
+Home-page: http://github.com/ulf1/treesimi
+Author: Ulf Hamster
+Author-email: 554c46@gmail.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/treesimi.svg)](https://badge.fury.io/py/treesimi)
+[![PyPi downloads](https://img.shields.io/pypi/dm/treesimi)](https://img.shields.io/pypi/dm/treesimi)
+[![DOI](https://zenodo.org/badge/318838452.svg)](https://zenodo.org/badge/latestdoi/318838452)
+
+
+# treesimi: Shingling for measuring tree similarity
+Compute similarity between trees, e.g. dependency trees
+
+
+## Convert an Adjacency List into a Nested Set Table
+For example, CoNLL-U's `['id', 'head']` fields form an adjacency list of a dependency tree.
+Traversing an adjacency list is slower than reading a nested set.
+Thus, converting a adjacency list to a nested set table once, makes sense if we need to read the three several times lateron.
+
+```py
+import treesimi as ts
+adjac = [(1, 0), (2, 1), (3, 1), (4, 2)]
+nested = ts.adjac_to_nested(adjac)
+# columns: node id, left, right, depth
+# [[1, 1, 8, 0], [2, 2, 5, 1], [4, 3, 4, 2], [3, 6, 7, 1]]
+```
+
+### Demo: Query a nested set table
+To extract a subtree we just need to iterate through the list ($O(n)$)
+
+```py
+_, lft0, rgt0, _ = nested[1]
+subtree = [(i, l, r, d) for i, l, r, d in nested if (l >= lft0) and (r <= rgt0)]
+# [[2, 2, 5, 1], [4, 3, 4, 2]]
+```
+
+or `ts.get_subtree(nested, sub_id=2)`
+
+### Set node attributes
+
+```py
+import treesimi as ts
+nested = [[1, 1, 8, 0], [2, 2, 5, 1], [4, 3, 4, 2], [3, 6, 7, 1]]
+attrs = [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd')]
+nested = ts.set_attr(nested, attrs)
+# columns: node id, left, right, depth, attributes
+# [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
+```
+
+### Convert Adjacency List with attributes
+
+```py
+import treesimi as ts
+adjac = [(1, 0, 'dat1'), (2, 1, 'dat2'), (3, 1, 'dat3'), (4, 2, 'dat3')]
+nested = ts.adjac_to_nested_with_attr(adjac)
+# columns: node id, left, right, depth
+# [[1, 1, 8, 0, 'dat1'], [2, 2, 5, 1, 'dat2'], [4, 3, 4, 2, 'dat2'], [3, 6, 7, 1, 'dat4']]
+```
 
-treesimi
-========
 
-Compute similarity between trees, e.g. dependency trees
-
-Convert an Adjacency List into a Nested Set Table
--------------------------------------------------
-
-For example, CoNLL-U’s ``['id', 'head']`` fields form an adjacency list
-of a dependency tree. Traversing an adjacency list is slower than
-reading a nested set. Thus, converting a adjacency list to a nested set
-table once, makes sense if we need to read the three several times
-lateron.
-
-.. code:: py
-
-   import treesimi as ts
-   adjac = [(1, 0), (2, 1), (3, 1), (4, 2)]
-   nested = ts.adjac_to_nested(adjac)
-   # columns: node id, left, right, depth
-   # [[1, 1, 8, 0], [2, 2, 5, 1], [4, 3, 4, 2], [3, 6, 7, 1]]
-
-Demo: Query a nested set table
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-To extract a subtree we just need to iterate through the list
-(:math:`O(n)`)
-
-.. code:: py
-
-   _, lft0, rgt0, _ = nested[1]
-   subtree = [(i, l, r, d) for i, l, r, d in nested if (l >= lft0) and (r <= rgt0)]
-   # [[2, 2, 5, 1], [4, 3, 4, 2]]
-
-or ``ts.get_subtree(nested, sub_id=2)``
-
-Set node attributes
-~~~~~~~~~~~~~~~~~~~
-
-.. code:: py
-
-   import treesimi as ts
-   nested = [[1, 1, 8, 0], [2, 2, 5, 1], [4, 3, 4, 2], [3, 6, 7, 1]]
-   attrs = [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd')]
-   nested = ts.set_attr(nested, attrs)
-   # columns: node id, left, right, depth, attributes
-   # [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
-
-Convert Adjacency List with attributes
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: py
-
-   import treesimi as ts
-   adjac = [(1, 0, 'dat1'), (2, 1, 'dat2'), (3, 1, 'dat3'), (4, 2, 'dat3')]
-   nested = ts.adjac_to_nested_with_attr(adjac)
-   # columns: node id, left, right, depth
-   # [[1, 1, 8, 0, 'dat1'], [2, 2, 5, 1, 'dat2'], [4, 3, 4, 2, 'dat2'], [3, 6, 7, 1, 'dat4']]
+## Extract subtree patterns
+We can extract the following patterns from one tree:
 
-Extract subtree patterns
-------------------------
+* Depth dimension
+    * Full subtrees
+    * Truncate leaves
+* Sibling dimension
+    * All siblings
+    * Drop siblings (and their subtree)
+* Placeholder attribute field
+
+
+### Full subtrees
+The function `extract_subtrees` returns all subtrees of a tree.
+The depth information is adjusted accordingly for each subtree.
+
+```py
+import treesimi as ts
+nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
+nested = ts.remove_node_ids(nested)
+subtrees = ts.extract_subtrees(nested)
+# [
+#    [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, 'c']],
+#    [[1, 4, 0, 'b'], [2, 3, 1, 'd']],
+#    [[1, 2, 0, 'd']],
+#    [[1, 2, 0, 'c']]
+# ]
+```
+
+### Truncate leaves
+In the first step, the function `trunc_leaves` removes leaves of the largest depth level.
+The result is always an incomplete tree, and the `lft` and `rgt` values are **not adjusted** to indicate that **there is a missing node**.
+In the next steps, the depth level is further removed down to `depth=1`.
+
+```py
+import treesimi as ts
+nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
+nested = ts.remove_node_ids(nested)
+subtrees = ts.trunc_leaves(nested)
+# [
+#   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [6, 7, 1, 'c']]
+# ]
+```
+
+Hint: Run `trunc_leaves` for each subtree extracted by `extract_subtrees`. Call `unique_trees` after each step.
+
+
+### Drop sibling nodes
+Generate variants of a tree by dropping each node once.
+Again, the result is always an incomplete tree, and the `lft` and `rgt` values are **not adjusted** to indicate that **there is a missing node**.
+
+```py
+import treesimi as ts
+nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
+nested = ts.remove_node_ids(nested)
+subtrees = ts.drop_nodes(nested)
+# [
+#   [[1, 8, 0, 'a']],
+#   [[1, 8, 0, 'a'], [2, 5, 1, 'b']],
+#   [[1, 8, 0, 'a']]
+# ]
+```
+
+Hints: Create subtrees with `extract_subtrees` and `trunc_leaves`, and run `drop_nodes` on these subtrees. If you want to drop N nodes/leaves of a tree, then call the function twice, e.g. `drop_nodes(drop_nodes(...))`.
+
+
+### Placeholder attribute field
+The `replace_attr` removes the data attribute of a node with a generic placeholder.
+
+```py
+import treesimi as ts
+nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
+nested = ts.remove_node_ids(nested)
+subtrees = ts.replace_attr(nested, placeholder='[MASK]')
+# [
+#   [[1, 8, 0, '[MASK]'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, 'c']],
+#   [[1, 8, 0, 'a'], [2, 5, 1, '[MASK]'], [3, 4, 2, 'd'], [6, 7, 1, 'c']], 
+#   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, '[MASK]'], [6, 7, 1, 'c']], 
+#   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, '[MASK]']]
+# ]
+```
+
+## Demo Notebooks about Shingling for MinHash
+We recommend using the `mmh3` hash function, and 32 permutations in `datasketch.MinHash`.
+
+- [Create subtrees as shingle sets](https://github.com/ulf1/treesimi/blob/master/demo/Create%20subtrees%20as%20shingle%20sets.ipynb)
+- [Jaccard Similarity between Dependency Trees](https://github.com/ulf1/treesimi/blob/master/demo/Jaccard%20Similarity%20between%20Dependency%20Trees.ipynb)
+- [Shingle Dependency Trees for datasketch's Minhash](https://github.com/ulf1/treesimi/blob/master/demo/Shingle%20Dependency%20Trees%20for%20datasketch's%20Minhash.ipynb)
 
-We can extract the following patterns from one tree:
+Start jupyter to run the demo notebook
 
--  Depth dimension
+```sh
+source .venv/bin/activate
+jupyter lab
+```
+
+## Appendix
+
+### Installation
+The `treesimi` [git repo](http://github.com/ulf1/treesimi) is available as [PyPi package](https://pypi.org/project/treesimi)
+
+```sh
+pip install treesimi
+pip install git+ssh://git@github.com/ulf1/treesimi.git
+```
 
-   -  Full subtrees
-   -  Truncate leaves
+### Commands
+Install a virtual environment
 
--  Sibling dimension
+```sh
+python3 -m venv .venv
+source .venv/bin/activate
+pip install --upgrade pip
+pip install -r requirements.txt --no-cache-dir
+pip install -r requirements-dev.txt --no-cache-dir
+pip install -r requirements-demo.txt --no-cache-dir
+```
 
-   -  All siblings
-   -  Drop siblings (and their subtree)
-
--  Placeholder attribute field
-
-Full subtrees
-~~~~~~~~~~~~~
-
-The function ``extract_subtrees`` returns all subtrees of a tree. The
-depth information is adjusted accordingly for each subtree.
-
-.. code:: py
-
-   import treesimi as ts
-   nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
-   nested = ts.remove_node_ids(nested)
-   subtrees = ts.extract_subtrees(nested)
-   # [
-   #    [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, 'c']],
-   #    [[1, 4, 0, 'b'], [2, 3, 1, 'd']],
-   #    [[1, 2, 0, 'd']],
-   #    [[1, 2, 0, 'c']]
-   # ]
-
-Truncate leaves
-~~~~~~~~~~~~~~~
-
-In the first step, the function ``trunc_leaves`` removes leaves of the
-largest depth level. The result is always an incomplete tree, and the
-``lft`` and ``rgt`` values are **not adjusted** to indicate that **there
-is a missing node**. In the next steps, the depth level is further
-removed down to ``depth=1``.
-
-.. code:: py
-
-   import treesimi as ts
-   nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
-   nested = ts.remove_node_ids(nested)
-   subtrees = ts.trunc_leaves(nested)
-   # [
-   #   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [6, 7, 1, 'c']]
-   # ]
-
-Hint: Run ``trunc_leaves`` for each subtree extracted by
-``extract_subtrees``. Call ``unique_trees`` after each step.
-
-Drop sibling nodes
-~~~~~~~~~~~~~~~~~~
-
-Generate variants of a tree by dropping each node once. Again, the
-result is always an incomplete tree, and the ``lft`` and ``rgt`` values
-are **not adjusted** to indicate that **there is a missing node**.
-
-.. code:: py
-
-   import treesimi as ts
-   nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
-   nested = ts.remove_node_ids(nested)
-   subtrees = ts.drop_nodes(nested)
-   # [
-   #   [[1, 8, 0, 'a']],
-   #   [[1, 8, 0, 'a'], [2, 5, 1, 'b']],
-   #   [[1, 8, 0, 'a']]
-   # ]
-
-Hints: Create subtrees with ``extract_subtrees`` and ``trunc_leaves``,
-and run ``drop_nodes`` on these subtrees. If you want to drop N
-nodes/leaves of a tree, then call the function twice,
-e.g. ``drop_nodes(drop_nodes(...))``.
-
-Placeholder attribute field
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The ``replace_attr`` removes the data attribute of a node with a generic
-placeholder.
-
-.. code:: py
-
-   import treesimi as ts
-   nested = [[1, 1, 8, 0, 'a'], [2, 2, 5, 1, 'b'], [4, 3, 4, 2, 'd'], [3, 6, 7, 1, 'c']]
-   nested = ts.remove_node_ids(nested)
-   subtrees = ts.replace_attr(nested, placeholder='[MASK]')
-   # [
-   #   [[1, 8, 0, '[MASK]'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, 'c']],
-   #   [[1, 8, 0, 'a'], [2, 5, 1, '[MASK]'], [3, 4, 2, 'd'], [6, 7, 1, 'c']], 
-   #   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, '[MASK]'], [6, 7, 1, 'c']], 
-   #   [[1, 8, 0, 'a'], [2, 5, 1, 'b'], [3, 4, 2, 'd'], [6, 7, 1, '[MASK]']]
-   # ]
-
-Demo Notebooks about Shingling for MinHash
-------------------------------------------
-
-We recommend using the ``mmh3`` hash function, and 32 permutations in
-``datasketch.MinHash``.
-
--  `Create subtrees as shingle
-   sets <https://github.com/satzbeleg/treesimi/blob/master/demo/Create%20subtrees%20as%20shingle%20sets.ipynb>`__
--  `Jaccard Similarity between Dependency
-   Trees <https://github.com/satzbeleg/treesimi/blob/master/demo/Jaccard%20Similarity%20between%20Dependency%20Trees.ipynb>`__
--  `Shingle Dependency Trees for datasketch’s
-   Minhash <https://github.com/satzbeleg/treesimi/blob/master/demo/Shingle%20Dependency%20Trees%20for%20datasketch's%20Minhash.ipynb>`__
+(If your git repo is stored in a folder with whitespaces, then don't use the subfolder `.venv`. Use an absolute path without whitespaces.)
 
-Start jupyter to run the demo notebook
+### Python commands
 
-.. code:: sh
+* Check syntax: `flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')`
+* Run Unit Tests: `pytest`
 
-   source .venv/bin/activate
-   jupyter lab
+Publish
 
-Appendix
---------
+```sh
+python setup.py sdist 
+twine upload -r pypi dist/*
+```
 
-Installation
-~~~~~~~~~~~~
+### Clean up 
 
-The ``treesimi`` `git repo <http://github.com/satzbeleg/treesimi>`__ is
-available as `PyPi package <https://pypi.org/project/treesimi>`__
+```sh
+find . -type f -name "*.pyc" | xargs rm
+find . -type d -name "__pycache__" | xargs rm -r
+rm -r .pytest_cache
+rm -r .venv
+```
 
-.. code:: sh
 
-   pip install treesimi
-   pip install git+ssh://git@github.com/satzbeleg/treesimi.git
+### Support
+Please [open an issue](https://github.com/ulf1/treesimi/issues/new) for support.
 
-Commands
-~~~~~~~~
 
-Install a virtual environment
+### Contributing
+Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/ulf1/treesimi/compare/).
 
-.. code:: sh
 
-   python3 -m venv .venv
-   source .venv/bin/activate
-   pip install --upgrade pip
-   pip install -r requirements.txt --no-cache-dir
-   pip install -r requirements-dev.txt --no-cache-dir
-   pip install -r requirements-demo.txt --no-cache-dir
-
-(If your git repo is stored in a folder with whitespaces, then don’t use
-the subfolder ``.venv``. Use an absolute path without whitespaces.)
-
-Python commands
-~~~~~~~~~~~~~~~
-
--  Check syntax:
-   ``flake8 --ignore=F401 --exclude=$(grep -v '^#' .gitignore | xargs | sed -e 's/ /,/g')``
--  Run Unit Tests: ``pytest``
+### Acknowledgements
+The "Evidence" project was funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) - [433249742](https://gepris.dfg.de/gepris/projekt/433249742) (GU 798/27-1; GE 1119/11-1).
 
-Publish
+### Maintenance
+- till 31.Aug.2023 (v0.2.0) the code repository was maintained within the DFG project [433249742](https://gepris.dfg.de/gepris/projekt/433249742)
+- since 01.Sep.2023 (v0.3.0) the code repository is maintained by Ulf Hamster.
 
-.. code:: sh
 
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
-issue <https://github.com/satzbeleg/treesimi/issues/new>`__ for support.
-
-Contributing
-~~~~~~~~~~~~
-
-Please contribute using `Github
-Flow <https://guides.github.com/introduction/flow/>`__. Create a branch,
-add commits, and `open a pull
-request <https://github.com/satzbeleg/treesimi/compare/>`__.
-
-.. |PyPI version| image:: https://badge.fury.io/py/treesimi.svg
-   :target: https://badge.fury.io/py/treesimi
-.. |PyPi downloads| image:: https://img.shields.io/pypi/dm/treesimi
-   :target: https://img.shields.io/pypi/dm/treesimi
-.. |DOI| image:: https://zenodo.org/badge/318838452.svg
-   :target: https://zenodo.org/badge/latestdoi/318838452
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `treesimi-0.2.0/setup.py` & `treesimi-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,17 @@
             return line.split(delim)[1]
     raise RuntimeError("Unable to find version string.")
 
 
 setup(name='treesimi',
       version=get_version("treesimi/__init__.py"),
       description='Compute similarity between netsted set based trees.',
-      # long_description=read('README.rst'),  # still not working
-      url='http://github.com/satzbeleg/treesimi',
+      long_description=read('README.md'),
+      long_description_content_type='text/markdown',
+      url='http://github.com/ulf1/treesimi',
       author='Ulf Hamster',
       author_email='554c46@gmail.com',
       license='Apache License 2.0',
       packages=['treesimi'],
       # install_requires=[],
       python_requires='>=3.6',
       zip_safe=True)
```

### Comparing `treesimi-0.2.0/test/test_convert.py` & `treesimi-0.3.0/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/test/test_extract.py` & `treesimi-0.3.0/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/test/test_shingleset.py` & `treesimi-0.3.0/test/test_shingleset.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/treesimi/convert.py` & `treesimi-0.3.0/treesimi/convert.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/treesimi/encode.py` & `treesimi-0.3.0/treesimi/encode.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/treesimi/extract.py` & `treesimi-0.3.0/treesimi/extract.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/treesimi/shingleset.py` & `treesimi-0.3.0/treesimi/shingleset.py`

 * *Files identical despite different names*

### Comparing `treesimi-0.2.0/treesimi/utils_for_depparser.py` & `treesimi-0.3.0/treesimi/utils_for_depparser.py`

 * *Files identical despite different names*

