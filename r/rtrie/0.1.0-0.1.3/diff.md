# Comparing `tmp/rtrie-0.1.0.tar.gz` & `tmp/rtrie-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrie-0.1.0.tar", max compression
+gzip compressed data, was "rtrie-0.1.3.tar", max compression
```

## Comparing `rtrie-0.1.0.tar` & `rtrie-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-26 01:40:17.717162 rtrie-0.1.0/README.md
--rw-r--r--   0        0        0      337 2023-06-26 01:50:51.627162 rtrie-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 01:40:17.717162 rtrie-0.1.0/rtrie/__init__.py
--rw-r--r--   0        0        0    25280 2023-06-26 01:45:51.807162 rtrie-0.1.0/rtrie/trie.py
--rw-r--r--   0        0        0      421 1970-01-01 00:00:00.000000 rtrie-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-06-26 02:07:13.317162 rtrie-0.1.3/README.md
+-rw-r--r--   0        0        0      886 2023-07-01 03:53:18.595569 rtrie-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-07-04 04:23:45.805946 rtrie-0.1.3/src/rtrie/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-01 06:07:54.375569 rtrie-0.1.3/src/rtrie/__main__.py
+-rw-r--r--   0        0        0     1136 2023-07-04 04:45:34.425946 rtrie-0.1.3/src/rtrie/array_trie.py
+-rw-r--r--   0        0        0     1029 2023-06-26 02:21:05.787162 rtrie-0.1.3/src/rtrie/stats.py
+-rw-r--r--   0        0        0      929 2023-07-04 04:45:40.315946 rtrie-0.1.3/src/rtrie/string_trie.py
+-rw-r--r--   0        0        0    27026 2023-07-04 03:28:25.925946 rtrie-0.1.3/src/rtrie/trie.py
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 rtrie-0.1.3/PKG-INFO
```

### Comparing `rtrie-0.1.0/rtrie/trie.py` & `rtrie-0.1.3/src/rtrie/trie.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import os
 import pickle
 import gc
 from itertools import chain, tee
 from collections import deque
 from collections.abc import MutableMapping
 from array import array
-from typing import Any, Callable, ItemsView, Iterator, Optional, TypeAlias, cast
+from typing import Any, Callable, ItemsView, Iterator, Literal, Optional, TypeAlias, cast
 from rapidfuzz import fuzz
+from rapidfuzz.distance.DamerauLevenshtein import distance
 # from rapidfuzz.distance.Levenshtein import distance
 
 Word: TypeAlias = str | tuple[str, Any]
 Words: TypeAlias = Iterator[Word]
 Attributes: TypeAlias = Any
 Entry: TypeAlias = tuple[str, 'Node']
 Record: TypeAlias = tuple[str, Attributes]
 Children: TypeAlias = dict[str, 'Node']
+Candidates: TypeAlias = list[tuple[int, str, 'Node']]
 
 def get_filename(string: str) -> str:
     return "".join([x if x.isalnum() else "_" for x in string])
 
 
 def get_longest_prefix_index(word1: str, word2: str):
     """
@@ -84,23 +86,17 @@
         for item in self.children.items():
             key: str = item[0]
             child: Node = item[1]
             string += "\n" + offset + "\t" + \
                 f"{key}({child.attributes}): {child.print(depth+1)}"
         return string
 
-class StoredNode(Node):
-    __slots__ = ('attributes', 'children', 'saved')
-
 class Trie(MutableMapping[str, Attributes]):
     def __init__(self, 
                  root: Node | None=None, 
-                 add_word: Optional[Callable[[Node, Attributes], int]]=None, 
-                 delete_word: Optional[Callable[[Node], int]]=None, 
-                 count: Optional[Callable[[Node], int]]=None, 
                  depth_to_store: Optional[int]=None, 
                  words: Optional[Words] = None, 
                  subtrie_path: str='./subtrie'):
         """
             Initialize a Trie.
 
             NOTE: `words` must be either a list of strings or a list of tuples of the form (word: str, attributes: Any). If `words` is a list of
@@ -111,17 +107,14 @@
             a word that already exists with other attributes, you may want to overwrite, merge, etc. The default is to simply assign
             the value `True`, indicating it is a word, and adding the same word again will not affect the trie.
 
             NOTE: if you supply custom add_word and delete_word functions, they MUST manage the `num_words` property if you want `len(trie)` to report the correct value.
         """
 
         self.root = root if root != None else Node()
-        self._add = add_word if add_word != None else self._default_add
-        self._delete = delete_word if delete_word != None else self._default_delete
-        self._count = count if count != None else self._default_count
         self.num_words: int = 0
         self.depth_to_store = depth_to_store
         self.subtrie_path = subtrie_path
         if self.depth_to_store != None:
             os.mkdir(self.subtrie_path)
         if words:
             self.add_words(words)
@@ -149,31 +142,31 @@
     def __contains__(self, word: object) -> bool:
         result = self._get_node(cast(str, word))
         return result != None and result[0][1].attributes != None
 
     def __iter__(self):
         return self.words()
 
-    def _default_add(self, node: Node, value: Attributes) -> int:
+    def add_attributes(self, node: Node, value: Attributes) -> int:
         """
           The default add method to use when one isn't provided. It uses True/None to indicate whether a node is a word or not
         """
         # if this is a new word, increment the number of words
         # otherwise we are just overwriting attributes which isn't a new word
-        is_new = True
+        is_new = 1
         if node.attributes != None:
-            is_new = False
+            is_new = 0
         node.attributes = value
-        return 1 if is_new else 0
+        return is_new
 
-    def _default_delete(self, node: Node) -> int:
+    def delete_attributes(self, node: Node) -> int:
         node.attributes = None
         return -1
 
-    def _default_count(self, node: Node) -> int:
+    def count_attributes(self, node: Node) -> int:
         return 1
 
     def add(self, word: str, attributes: Attributes=True):
         """
           Adds a single word to an already constructed Trie. You should use `add_words` to initialize a Trie for performance reasons
         """
         current: Node = self.root
@@ -187,21 +180,21 @@
 
             logging.debug(str(current.children.keys()))
 
             if len(current.children.keys()) == 0:
                 logging.debug(
                     f'Empty children, adding "{word}" with `attributes = {attributes}')
                 current.children[word] = Node()
-                self.num_words += self._add(current.children[word], attributes)
+                self.num_words += self.add_attributes(current.children[word], attributes)
                 break
 
             elif word in current.children.keys():
                 logging.debug(
                     f'"{word}" already exists, adding attributes {attributes}')
-                self.num_words += self._add(current.children[word], attributes)
+                self.num_words += self.add_attributes(current.children[word], attributes)
                 break
 
             else:
                 match_found = False
                 logging.debug("No exact match, checking remaining keys...")
                 for key in list(current.children.keys()):
                     index: int = get_longest_prefix_index(key, word)
@@ -229,15 +222,15 @@
 
                         else:
                             logging.debug(f'Creating new node "{key_suffix}"')
                             is_word = len(prefix) == len(word)
                             logging.debug(
                                 f'Creating new node "{prefix}", is it a word: {is_word}')
                             current.children[prefix] = Node(None, Children())
-                            self.num_words += self._add(
+                            self.num_words += self.add_attributes(
                                 current.children[prefix], attributes if is_word else None)
                             
                             # we know this is set to empty dict from above
                             current.children[prefix].children[key_suffix] = current.children[key] # type: ignore
                             logging.debug(f'Deleting old node "{key}"')
                             del current.children[key]
 
@@ -249,27 +242,27 @@
                         break
 
                 if not match_found:
                     logging.debug(
                         f'No overlapping prefixes in any key, adding "{word}" with `attributes` = {attributes}')
                     if current.children != None:
                         current.children[word] = Node()
-                        self.num_words += self._add(
+                        self.num_words += self.add_attributes(
                             current.children[word], attributes)
                     break
 
     def delete(self, word: str):
         prev: Node | None = None
         current = self.root
 
         while current != None:
             if word in current.children:
                 # handle node shifts
 
-                self._delete(node)
+                self.delete_attributes(node)
                 return
 
             for i in range(0, len(word)):
                 w = word[:i]
                 if w in node.children:
                     logging.debug(f"Prefix: {prefix}, Word: {word}")
                     prev = current
@@ -364,15 +357,15 @@
 
             # matching case, add to Trie
             if len(matches) == 1:
                 logging.debug("Single match - normal case")
                 logging.debug(
                     f"Adding word {first_label} with attributes {first_attributes}")
                 current.children[first_label] = Node()
-                self.num_words += self._add(
+                self.num_words += self.add_attributes(
                     current.children[first_label], first_attributes)
                 if last == None:
                     return
                 continue
 
             # recursive case
             else:
@@ -402,15 +395,15 @@
                     word = next(matches, None)
                     while word != None:
                         label, attributes = _get_values(word)
                         if label[offset:] != prefix:
                             break
                         logging.debug(
                             f"Adding word {label} with attributes {attributes}")
-                        self.num_words += self._add(
+                        self.num_words += self.add_attributes(
                             current.children[prefix], attributes)
                         word = next(matches, None)
 
                     if word != None:
                         matches = chain([word], matches)
 
                 # otherwise, it's just a node
@@ -514,51 +507,97 @@
 
                 if node.children != None:
                     for key, value in reversed(sorted(node.children.items())):
                         stack.append((prefix + key, value))
 
         return candidates
 
-    def search(self, word, max_distance: int):
+    def search(self, word, type: Literal['fuzzy', 'edit'] = 'edit', max_distance: int = 0) -> Candidates:
 
         # Pruning phase
         candidates = []
+        offset = 0
+        distance = 0
 
-        stack = deque()
-        if self.root.children != None:
-            for key, node in self.root.children.items():
-                stack.append((key, node))
+        if type == 'edit':
+          self._search_edit_recursive(self.root, word, "", offset, distance, max_distance, candidates)
+        else:
+          print('TODO: fuzzy')
 
-        while stack:
-            prefix, node = stack.pop()
-            prefix_length = len(key)
+        return candidates
 
-            prefix = word[:prefix_length]
-            logging.debug(f"Comparing {prefix} to {word}")
-            previous_row = array('b', range(prefix_length + 1))
-            for i in range(len(prefix) - 1):
-                current_row = array('b', range(prefix_length + 1))
-                current_row[0] = i + 1
-                for j in range(prefix_length - 1):
-                    deletion_cost = previous_row[j + 1] + 1
-                    insertion_cost = current_row[j] + 1
-                    substitution_cost = previous_row[j] if word[i] == prefix[j] else previous_row[j] + 1
-                    current_row[j + 1] = min(deletion_cost,
-                                             insertion_cost, substitution_cost)
-
-                previous_row = current_row
-
-            distance = previous_row[prefix_length - 1]
-            logging.debug(f"Distance: {distance}")
-            if previous_row[prefix_length - 1] < max_distance:
-                if node.children != None:
-                    for key, value in node.children.items():
-                        stack.append((prefix + key, value))
 
-        return candidates
+        # stack = deque()
+        # if self.root.children != None:
+        #     for key, node in self.root.children.items():
+        #         stack.append((key, node))
+
+        # while stack:
+        #     prefix, node = stack.pop()
+        #     prefix_length = len(prefix)
+        #     word_fragment = word[offset:prefix_length]
+
+        #     logging.debug(f"Prefix: {prefix}, Word: {word_fragment}")
+        #     score = distance(word_fragment, prefix)
+        #     logging.debug(f"Distance: {score}")
+
+        #     if score < max_distance:
+                
+
+        #     # prefix = word[:prefix_length]
+        #     logging.debug(f"Comparing {prefix} to {word}")
+        #     previous_row = array('b', range(prefix_length + 1))
+        #     for i in range(len(prefix) - 1):
+        #         current_row = array('b', range(prefix_length + 1))
+        #         current_row[0] = i + 1
+        #         for j in range(prefix_length - 1):
+        #             deletion_cost = previous_row[j + 1] + 1
+        #             insertion_cost = current_row[j] + 1
+        #             substitution_cost = previous_row[j] if word[i] == prefix[j] else previous_row[j] + 1
+        #             current_row[j + 1] = min(deletion_cost,
+        #                                      insertion_cost, substitution_cost)
+
+        #         previous_row = current_row
+
+        #     distance = previous_row[prefix_length - 1]
+        #     logging.debug(f"Distance: {distance}")
+        #     if previous_row[prefix_length - 1] < max_distance:
+        #         if node.children != None:
+        #             for key, value in node.children.items():
+        #                 stack.append((prefix + key, value))
+
+        # return candidates
+
+    def _search_edit_recursive(self, node: Node, word: str, prefix: str, offset: int, current_distance: int, max_distance: int, candidates: Candidates) -> Candidates:
+        if node == None or node.children == None or len(node.children) == 0:
+          return
+
+
+
+
+        # TODO: see if we can improve on this, since right now we're doing a lookup for each word and we could be doing lookup
+        # of each fragment of the word that lines up with key
+
+        for child in node.children:
+            fragment = word[offset:offset+len(child)]
+            d = distance(fragment, child)
+
+            # we want to be able to tell if the key has 0 difference
+            total = d + current_distance
+            logging.debug(f"Distance b/w {child} and {fragment}: {d}")
+            logging.debug(f"{current_distance} + {d} = {total}")
+            if total <= max_distance:
+                child_node = node.children[child]
+                new_prefix = prefix + child
+                logging.debug(f"{word}, {new_prefix}, {distance(word, prefix)}")
+                if child_node.attributes != None:
+                    total_distance = distance(word, new_prefix)
+                    if total_distance <= max_distance:
+                        candidates.append((total_distance, child_node))
+                self._search_edit_recursive(child_node, word, new_prefix, offset + len(child), total, max_distance, candidates)
 
     def stats(self, unique: bool = True):
         average_length: int = 0
         word_lengths: dict[int, int] = {}
         letter_frequency: dict[str, int] = {}
         letter_distribution: dict[str, dict[int, int]] = {}
         num_nodes: int = 0
@@ -586,15 +625,15 @@
             lengths_at_node_depths[depth][len(
                 prefix)] = lengths_at_node_depths[depth].get(len(prefix), 0) + 1
 
             if node.attributes != None:
                 # it's a word, so 'prefix' is the full word
                 length = len(prefix)
 
-                count = 1 if unique else self._count(node)
+                count = 1 if unique else self.count_attributes(node)
 
                 # TODO: just compute afterwards based on word lengths?
                 average_length += length * count
                 word_lengths[length] = word_lengths.get(length, 0) + count
 
                 for index, letter in enumerate(prefix):
                     letter_frequency[letter] = letter_frequency.get(
```

