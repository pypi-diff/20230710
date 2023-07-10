# Comparing `tmp/merkly-0.7.2.tar.gz` & `tmp/merkly-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.7.2.tar", max compression
+gzip compressed data, was "merkly-0.8.0.tar", max compression
```

## Comparing `merkly-0.7.2.tar` & `merkly-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-07-06 03:26:05.839926 merkly-0.7.2/LICENSE
--rw-r--r--   0        0        0     5392 2023-07-06 03:26:05.839926 merkly-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/__init__.py
--rw-r--r--   0        0        0     4554 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/mtree.py
--rw-r--r--   0        0        0     2769 2023-07-06 03:26:05.839926 merkly-0.7.2/merkly/utils.py
--rw-r--r--   0        0        0      878 2023-07-06 03:26:05.839926 merkly-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 merkly-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-10 03:05:43.283259 merkly-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5392 2023-07-10 03:05:43.283259 merkly-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 03:05:43.287259 merkly-0.8.0/merkly/__init__.py
+-rw-r--r--   0        0        0     5224 2023-07-10 03:05:43.287259 merkly-0.8.0/merkly/mtree.py
+-rw-r--r--   0        0        0      259 2023-07-10 03:05:43.287259 merkly-0.8.0/merkly/node.py
+-rw-r--r--   0        0        0     2775 2023-07-10 03:05:43.287259 merkly-0.8.0/merkly/utils.py
+-rw-r--r--   0        0        0      878 2023-07-10 03:05:43.287259 merkly-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 merkly-0.8.0/PKG-INFO
```

### Comparing `merkly-0.7.2/LICENSE` & `merkly-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.7.2/README.md` & `merkly-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,17 @@
 
 | Feature                                                                                                   | Status | Priority |
 | --------------------------------------------------------------------------------------------------------- | ------ | -------- |
 | Create Root                                                                                               | ✅     | 🔥       |
 | Create Proof                                                                                              | ✅     | 🔥       |
 | Verify Proof                                                                                              | ✅     | 🔥       |
 | Use any Hash function                                                                                     | ✅     | 🧐       |
+| Leafs of any size                                                                                         | ✅     | 🧐       |
 | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/utilities#verifying_merkle_proofs)** | ⏰     | 🔥       |
 | Compatible with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)**                            | ⏰     | 🔥       |
-| Leafs of any size                                                                                         | ⏰     | 🧐       |
 
 ## Contributing
 
 - Before read a code of conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)**
 - Follow the guide of development: **[CONTRIBUTING](CONTRIBUTING.md)**
 
 ## License
```

#### html2text {}

```diff
@@ -42,14 +42,14 @@
 'b555...'), Node(right: '6467...') ] ``` **Verify Proof of a leaf** ```python
 from merkly.mtree import MerkleTree # create a Merkle Tree mtree = MerkleTree(
 ['a', 'b', 'c', 'd']) # get proof of a raw leaf p = mtree.proof('b') # verify
 your proof of raw leaf assert mtree.verify(p, 'b') == True ``` ## Roadmap |
 Feature | Status | Priority | | -----------------------------------------------
 ---------------------------------------------------------- | ------ | -------
 - | | Create Root | â | ð¥ | | Create Proof | â | ð¥ | | Verify Proof |
-â | ð¥ | | Use any Hash function | â | ð§ | | Support **[OpenZeppelin]
-(https://docs.openzeppelin.com/contracts/4.x/
+â | ð¥ | | Use any Hash function | â | ð§ | | Leafs of any size | â |
+ð§ | | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/
 utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible with **
-[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | |
-Leafs of any size | â° | ð§ | ## Contributing - Before read a code of
-conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)** - Follow the guide of
-development: **[CONTRIBUTING](CONTRIBUTING.md)** ## License [MIT](LICENSE)
+[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | ##
+Contributing - Before read a code of conduct: **[CODE_OF_CONDUCT]
+(CODE_OF_CONDUCT.md)** - Follow the guide of development: **[CONTRIBUTING]
+(CONTRIBUTING.md)** ## License [MIT](LICENSE)
```

### Comparing `merkly-0.7.2/merkly/utils.py` & `merkly-0.8.0/merkly/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,20 +81,23 @@
     ```
     """
 
     return [list_item[i : i + 2] for i in range(0, len(list_item), 2)]
 
 
 def hash_function_type_checking(hash_function: Callable[[str], str]) -> bool:
-    is_valid = (
-        isinstance(hash_function, types.FunctionType)
-        and callable(hash_function)
-        and isinstance(hash_function(str()), str)
-    )
-    if hash_function is not None and not is_valid:
+    a = isinstance(hash_function, types.FunctionType)
+    b = callable(hash_function)
+    try:
+        c = isinstance(hash_function(str(), str()), str)
+    except TypeError:
+        c = False
+
+    valid = a and b and c
+    if not valid:
         raise InvalidHashFunctionError()
 
 
 def is_power_2(number: int) -> bool:
     """
     # Verify if `x: int` is power of 2
     - params `x: int`
@@ -109,8 +112,8 @@
     """
 
     left: bool = number & (number - 1) == 0
     right: bool = number != 0
     if left and right:
         return True
     else:
-        raise PowerOfTwoError(number)
+        return False
```

### Comparing `merkly-0.7.2/pyproject.toml` & `merkly-0.8.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merkly"
-version = "0.7.2"
+version = "0.8.0"
 description = "🌳 The simple and easy implementation of Merkle Tree"
 authors = ["Lucas Oliveira <olivmath@protonmail.com>"]
 repository = "https://github.com/olivmath/merkly.git"
 documentation = "https://pypi.org/project/merkly/"
 readme = "README.md"
 license = "MIT"
 keywords = [
```

### Comparing `merkly-0.7.2/PKG-INFO` & `merkly-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkly
-Version: 0.7.2
+Version: 0.8.0
 Summary: 🌳 The simple and easy implementation of Merkle Tree
 Home-page: https://github.com/olivmath/merkly.git
 License: MIT
 Keywords: merkle-tree,merkle-proof,merkle-root,keccak256,blockchain
 Author: Lucas Oliveira
 Author-email: olivmath@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -188,17 +188,17 @@
 
 | Feature                                                                                                   | Status | Priority |
 | --------------------------------------------------------------------------------------------------------- | ------ | -------- |
 | Create Root                                                                                               | ✅     | 🔥       |
 | Create Proof                                                                                              | ✅     | 🔥       |
 | Verify Proof                                                                                              | ✅     | 🔥       |
 | Use any Hash function                                                                                     | ✅     | 🧐       |
+| Leafs of any size                                                                                         | ✅     | 🧐       |
 | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/utilities#verifying_merkle_proofs)** | ⏰     | 🔥       |
 | Compatible with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)**                            | ⏰     | 🔥       |
-| Leafs of any size                                                                                         | ⏰     | 🧐       |
 
 ## Contributing
 
 - Before read a code of conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)**
 - Follow the guide of development: **[CONTRIBUTING](CONTRIBUTING.md)**
 
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: merkly Version: 0.7.2 Summary: ð³ The simple and
+Metadata-Version: 2.1 Name: merkly Version: 0.8.0 Summary: ð³ The simple and
 easy implementation of Merkle Tree Home-page: https://github.com/olivmath/
 merkly.git License: MIT Keywords: merkle-tree,merkle-proof,merkle-
 root,keccak256,blockchain Author: Lucas Oliveira Author-email:
 olivmath@protonmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -55,14 +55,14 @@
 'b555...'), Node(right: '6467...') ] ``` **Verify Proof of a leaf** ```python
 from merkly.mtree import MerkleTree # create a Merkle Tree mtree = MerkleTree(
 ['a', 'b', 'c', 'd']) # get proof of a raw leaf p = mtree.proof('b') # verify
 your proof of raw leaf assert mtree.verify(p, 'b') == True ``` ## Roadmap |
 Feature | Status | Priority | | -----------------------------------------------
 ---------------------------------------------------------- | ------ | -------
 - | | Create Root | â | ð¥ | | Create Proof | â | ð¥ | | Verify Proof |
-â | ð¥ | | Use any Hash function | â | ð§ | | Support **[OpenZeppelin]
-(https://docs.openzeppelin.com/contracts/4.x/
+â | ð¥ | | Use any Hash function | â | ð§ | | Leafs of any size | â |
+ð§ | | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/
 utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible with **
-[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | |
-Leafs of any size | â° | ð§ | ## Contributing - Before read a code of
-conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)** - Follow the guide of
-development: **[CONTRIBUTING](CONTRIBUTING.md)** ## License [MIT](LICENSE)
+[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | ##
+Contributing - Before read a code of conduct: **[CODE_OF_CONDUCT]
+(CODE_OF_CONDUCT.md)** - Follow the guide of development: **[CONTRIBUTING]
+(CONTRIBUTING.md)** ## License [MIT](LICENSE)
```

