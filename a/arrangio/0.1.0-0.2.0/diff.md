# Comparing `tmp/arrangio-0.1.0.tar.gz` & `tmp/arrangio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrangio-0.1.0.tar", last modified: Wed Jun 21 15:53:44 2023, max compression
+gzip compressed data, was "arrangio-0.2.0.tar", last modified: Mon Jul 10 10:26:14 2023, max compression
```

## Comparing `arrangio-0.1.0.tar` & `arrangio-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-06-21 15:53:44.278575 arrangio-0.1.0/
--rw-r--r--   0 fscm       (501) staff       (20)     1089 2023-06-13 12:35:35.000000 arrangio-0.1.0/LICENSE
--rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-06-21 15:53:44.277967 arrangio-0.1.0/PKG-INFO
--rw-r--r--   0 fscm       (501) staff       (20)     2864 2023-06-21 15:52:17.000000 arrangio-0.1.0/README.md
--rw-r--r--   0 fscm       (501) staff       (20)     6616 2023-06-21 15:36:55.000000 arrangio-0.1.0/pyproject.toml
--rw-r--r--   0 fscm       (501) staff       (20)       38 2023-06-21 15:53:44.278767 arrangio-0.1.0/setup.cfg
--rw-r--r--   0 fscm       (501) staff       (20)      266 2023-06-13 12:35:00.000000 arrangio-0.1.0/setup.py
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-06-21 15:53:44.257655 arrangio-0.1.0/src/
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-06-21 15:53:44.265451 arrangio-0.1.0/src/arrangio/
--rw-r--r--   0 fscm       (501) staff       (20)     1647 2023-06-21 15:52:07.000000 arrangio-0.1.0/src/arrangio/__init__.py
--rw-r--r--   0 fscm       (501) staff       (20)      143 2023-06-20 17:04:15.000000 arrangio-0.1.0/src/arrangio/__init__.pyi
--rw-r--r--   0 fscm       (501) staff       (20)     1126 2023-06-21 15:36:11.000000 arrangio-0.1.0/src/arrangio/__main__.py
--rw-r--r--   0 fscm       (501) staff       (20)     1928 2023-06-21 15:39:17.000000 arrangio-0.1.0/src/arrangio/_parser_.py
--rw-r--r--   0 fscm       (501) staff       (20)      112 2023-06-20 17:04:08.000000 arrangio-0.1.0/src/arrangio/_parser_.pyi
--rw-r--r--   0 fscm       (501) staff       (20)     5056 2023-06-20 17:06:28.000000 arrangio-0.1.0/src/arrangio/_utils_.py
--rw-r--r--   0 fscm       (501) staff       (20)      203 2023-06-20 17:04:08.000000 arrangio-0.1.0/src/arrangio/_utils_.pyi
--rw-r--r--   0 fscm       (501) staff       (20)        0 2023-06-13 13:25:12.000000 arrangio-0.1.0/src/arrangio/py.typed
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-06-21 15:53:44.269947 arrangio-0.1.0/src/arrangio.egg-info/
--rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/PKG-INFO
--rw-r--r--   0 fscm       (501) staff       (20)      525 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/SOURCES.txt
--rw-r--r--   0 fscm       (501) staff       (20)        1 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/dependency_links.txt
--rw-r--r--   0 fscm       (501) staff       (20)       52 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/entry_points.txt
--rw-r--r--   0 fscm       (501) staff       (20)      177 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/requires.txt
--rw-r--r--   0 fscm       (501) staff       (20)        9 2023-06-21 15:53:44.000000 arrangio-0.1.0/src/arrangio.egg-info/top_level.txt
-drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-06-21 15:53:44.276049 arrangio-0.1.0/tests/
--rw-r--r--   0 fscm       (501) staff       (20)     3282 2023-06-21 15:18:19.000000 arrangio-0.1.0/tests/test___main__.py
--rw-r--r--   0 fscm       (501) staff       (20)     1822 2023-06-21 13:59:31.000000 arrangio-0.1.0/tests/test__parser_.py
--rw-r--r--   0 fscm       (501) staff       (20)     4423 2023-06-21 13:06:12.000000 arrangio-0.1.0/tests/test__utils_.py
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.877805 arrangio-0.2.0/
+-rw-r--r--   0 fscm       (501) staff       (20)     1089 2023-06-13 12:35:35.000000 arrangio-0.2.0/LICENSE
+-rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-10 10:26:14.877240 arrangio-0.2.0/PKG-INFO
+-rw-r--r--   0 fscm       (501) staff       (20)     2864 2023-06-21 15:52:17.000000 arrangio-0.2.0/README.md
+-rw-r--r--   0 fscm       (501) staff       (20)     6616 2023-06-21 15:36:55.000000 arrangio-0.2.0/pyproject.toml
+-rw-r--r--   0 fscm       (501) staff       (20)       38 2023-07-10 10:26:14.878100 arrangio-0.2.0/setup.cfg
+-rw-r--r--   0 fscm       (501) staff       (20)      266 2023-06-13 12:35:00.000000 arrangio-0.2.0/setup.py
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.855676 arrangio-0.2.0/src/
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.866629 arrangio-0.2.0/src/arrangio/
+-rw-r--r--   0 fscm       (501) staff       (20)     1647 2023-07-10 10:23:47.000000 arrangio-0.2.0/src/arrangio/__init__.py
+-rw-r--r--   0 fscm       (501) staff       (20)      143 2023-06-20 17:04:15.000000 arrangio-0.2.0/src/arrangio/__init__.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)     1126 2023-06-21 15:36:11.000000 arrangio-0.2.0/src/arrangio/__main__.py
+-rw-r--r--   0 fscm       (501) staff       (20)     1928 2023-06-21 15:39:17.000000 arrangio-0.2.0/src/arrangio/_parser_.py
+-rw-r--r--   0 fscm       (501) staff       (20)      112 2023-06-20 17:04:08.000000 arrangio-0.2.0/src/arrangio/_parser_.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)     4588 2023-07-10 10:03:19.000000 arrangio-0.2.0/src/arrangio/_utils_.py
+-rw-r--r--   0 fscm       (501) staff       (20)      203 2023-06-20 17:04:08.000000 arrangio-0.2.0/src/arrangio/_utils_.pyi
+-rw-r--r--   0 fscm       (501) staff       (20)        0 2023-06-13 13:25:12.000000 arrangio-0.2.0/src/arrangio/py.typed
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.872349 arrangio-0.2.0/src/arrangio.egg-info/
+-rw-r--r--   0 fscm       (501) staff       (20)     3951 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/PKG-INFO
+-rw-r--r--   0 fscm       (501) staff       (20)      525 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/SOURCES.txt
+-rw-r--r--   0 fscm       (501) staff       (20)        1 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/dependency_links.txt
+-rw-r--r--   0 fscm       (501) staff       (20)       52 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/entry_points.txt
+-rw-r--r--   0 fscm       (501) staff       (20)      177 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/requires.txt
+-rw-r--r--   0 fscm       (501) staff       (20)        9 2023-07-10 10:26:14.000000 arrangio-0.2.0/src/arrangio.egg-info/top_level.txt
+drwxr-xr-x   0 fscm       (501) staff       (20)        0 2023-07-10 10:26:14.875229 arrangio-0.2.0/tests/
+-rw-r--r--   0 fscm       (501) staff       (20)     3282 2023-07-10 10:18:03.000000 arrangio-0.2.0/tests/test___main__.py
+-rw-r--r--   0 fscm       (501) staff       (20)     1822 2023-06-21 13:59:31.000000 arrangio-0.2.0/tests/test__parser_.py
+-rw-r--r--   0 fscm       (501) staff       (20)     4435 2023-07-10 10:09:47.000000 arrangio-0.2.0/tests/test__utils_.py
```

### Comparing `arrangio-0.1.0/LICENSE` & `arrangio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/PKG-INFO` & `arrangio-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrangio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Arranges a set of songs in groups with similar total play time.
 Author: Frederico Martins
 License: MIT
 Project-URL: Documentation, http://electric-mass.github.io/arrangio
 Project-URL: Homepage, https://github.com/electric-mass//arrangio
 Project-URL: Source, https://github.com/electric-mass/arrangio
 Keywords: songs,grouping
```

### Comparing `arrangio-0.1.0/README.md` & `arrangio-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/pyproject.toml` & `arrangio-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/src/arrangio/__init__.py` & `arrangio-0.2.0/src/arrangio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 from typing import Final
 
 __all__: Final[tuple] = ()
 
 __author__: Final[str] = 'Electric Mass Records'
 __license__: Final[str] = 'MIT'
 __project__: Final[str] = __package__
-__version__: Final[str] = '0.1.0'
+__version__: Final[str] = '0.2.0'
```

### Comparing `arrangio-0.1.0/src/arrangio/__main__.py` & `arrangio-0.2.0/src/arrangio/__main__.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/src/arrangio/_parser_.py` & `arrangio-0.2.0/src/arrangio/_parser_.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/src/arrangio/_utils_.py` & `arrangio-0.2.0/src/arrangio/_utils_.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 | get_subsets  | `list(tuple(int, list))`  | gets the subsets of songs |
 | show_results | `None`                    | shows the results         |
 
 All other resources in this module are considered implementation
 details.
 """
 
-# from functools import lru_cache as cache
+from functools import lru_cache as cache
 from datetime import datetime as _datetime, timedelta as _timedelta
 from re import compile as _compile
 from typing import Final
 
 
 REGXPR: Final[str] = (
     r'^(?P<label>\w+):'
@@ -53,24 +53,24 @@
 
     Returns:
         str: The timestamp string.
     """
     return str(_timedelta(seconds=seconds))
 
 
-def get_songs(songs: list) -> list:
+def get_songs(songs: list) -> tuple:
     """Parses the songs entered in the options.
 
     Args:
         songs (list(str)): The list of songs inputed by the user (as
             collected by the `_parser_` module).
 
     Returns:
-        list(tuple(str, int)): The list of songs defined as a tuple of
-            song name and song lenght (in seconds).
+        tuple(tuple(str, int)): The list of songs defined as a tuple of
+            tuples with the song name and the song lenght (in seconds).
 
     Raises:
         ValueError: If the song info is not in the form of
             'label:00h00m00s'.
     """
     pattern = _compile(REGXPR)
     unsorted_songs = []
@@ -78,80 +78,63 @@
         matched = pattern.match(song)
         if matched is None:
             raise ValueError(f'[ERROR] Invalid song information ({song}).')
         info = matched.groupdict(default='0')
         seconds = _to_seconds(
             f'{info["hours"]}:{info["minutes"]}:{info["seconds"]}')
         unsorted_songs.append((seconds, info['label']))
-    return sorted(unsorted_songs, reverse=True)
+    return tuple(sorted(unsorted_songs, reverse=True))
 
 
-# def __list_to_tuple(function):
-#     def wrapper(*args, **kwargs):
-#         args = [tuple(x) if isinstance(x, list) else x for x in args]
-#         kwargs = {
-#             k: tuple(x) if isinstance(x, list) else x
-#             for k, x in kwargs.items()}
-#         print('---->', args, kwargs)
-#         print('---->', *args, **kwargs)
-#         return function(*args, **kwargs)
-#     return wrapper
-
-
-# @__list_to_tuple
-# @cache(maxsize=None, typed=False)
+@cache(maxsize=None, typed=False)
 def __get_subsets(
-        songs: list,
+        songs: tuple,
         songs_length: int,
-        subsets: list) -> list:
+        subsets: tuple) -> tuple:
     """Auxiliar function for `get_subsets`.
 
     Args:
-        songs (list): The list of songs (from `get_songs`).
+        songs (tuple): The list of songs (from `get_songs`).
         songs_length (int): The length of `songs`.
-        subsets (list): The list of possible subsets.
+        subsets (tuple): The list of possible subsets.
 
     Returns:
-        tuple(int, list(tuple(int, str))): The list of subsets.
+        tuple(int, tuple(tuple(int, str))): The list of subsets.
     """
     if songs_length == 0:
         _min, _ = min(subsets)
         _max, _ = max(subsets)
         return (_max - _min, subsets)
-    _songs = songs.copy()
+    _songs = songs[1:]
+    _song = songs[0]
     _songs_length = songs_length - 1
-    _song = _songs.pop(0)
-    _possible_subsets = []
-    for element in subsets:
-        _subset = element[1].copy()
-        _subset.append(_song)
+    _possible_subsets = ()
+    for index, element in enumerate(subsets):
+        _subset = (_song,) + element[1]
         _element = (element[0] + _song[0], _subset)
-        _subsets = subsets.copy()
-        _subsets.remove(element)
-        _subsets.append(_element)
-        _possible_subsets.append(_subsets)
-    return min([
+        _subsets = (_element,) + subsets[:index] + subsets[index+1:]
+        _possible_subsets = (_subsets,) + _possible_subsets
+    return min(
         __get_subsets(_songs, _songs_length, sub)
         for sub
-        in _possible_subsets])
+        in _possible_subsets)
 
 
-def get_subsets(songs: list, num: int) -> list:
+def get_subsets(songs: tuple, num: int) -> tuple:
     """Parses the songs entered in the options.
 
     Args:
-        songs (list): The list of songs (from `get_songs`).
+        songs (tuple): The list of songs (from `get_songs`).
         num (int): The number of subsets to divide the set into.
 
     Returns:
-        list(tuple(int, list(tuple(int, str)))): The list of subsets).
+        tuple(tuple(int, tuple(tuple(int, str)))): The list of subsets).
     """
-    # total_length = sum(l for l, _ in songs)
     songs_length = len(songs)
-    subsets = [(0, [])] * num
+    subsets = ((0, ()),) * num
     return __get_subsets(
         songs,
         songs_length,
         subsets)
 
 
 def show_results(result: tuple) -> None:
```

### Comparing `arrangio-0.1.0/src/arrangio.egg-info/PKG-INFO` & `arrangio-0.2.0/src/arrangio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrangio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Arranges a set of songs in groups with similar total play time.
 Author: Frederico Martins
 License: MIT
 Project-URL: Documentation, http://electric-mass.github.io/arrangio
 Project-URL: Homepage, https://github.com/electric-mass//arrangio
 Project-URL: Source, https://github.com/electric-mass/arrangio
 Keywords: songs,grouping
```

### Comparing `arrangio-0.1.0/src/arrangio.egg-info/SOURCES.txt` & `arrangio-0.2.0/src/arrangio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/tests/test___main__.py` & `arrangio-0.2.0/tests/test___main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 @mark.parametrize('args,output,exception,exit_code', [
     ([__project__, '--dummy'], None, SystemExit, 2),
     ([__project__, '--quiet'], None, SystemExit, 2),
     ([__project__, '-s', '0:00:01'], None, SystemExit, 9),
     ([__project__, '--version'], f"{__version__}\n", SystemExit, 0),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s'],
-        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:41 ['song05 (0:05:54)', 'song06 (0:05:16)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [2] 0:18:49 ['song03 (0:05:37)', 'song04 (0:04:51)', 'song07 (0:03:45)', 'song02 (0:03:41)', 'song01 (0:00:55)']\n",
+        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:49 ['song01 (0:00:55)', 'song02 (0:03:41)', 'song07 (0:03:45)', 'song04 (0:04:51)', 'song03 (0:05:37)']\n  [2] 0:18:41 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song06 (0:05:16)', 'song05 (0:05:54)']\n",
         None,
         0
     ),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '2'],
-        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:41 ['song05 (0:05:54)', 'song06 (0:05:16)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [2] 0:18:49 ['song03 (0:05:37)', 'song04 (0:04:51)', 'song07 (0:03:45)', 'song02 (0:03:41)', 'song01 (0:00:55)']\n",
+        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 8\nGroups:\n  [1] 0:18:49 ['song01 (0:00:55)', 'song02 (0:03:41)', 'song07 (0:03:45)', 'song04 (0:04:51)', 'song03 (0:05:37)']\n  [2] 0:18:41 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song06 (0:05:16)', 'song05 (0:05:54)']\n",
         None,
         0
     ),
     (
         [__project__, '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '3'],
-        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 20\nGroups:\n  [1] 0:12:42 ['song06 (0:05:16)', 'song07 (0:03:45)', 'song02 (0:03:41)']\n  [2] 0:12:22 ['song04 (0:04:51)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [3] 0:12:26 ['song05 (0:05:54)', 'song03 (0:05:37)', 'song01 (0:00:55)']\n",
+        "arrangio version 0.1.0\nby Electric Mass Records under MIT license\nDifference (in seconds): 20\nGroups:\n  [1] 0:12:26 ['song01 (0:00:55)', 'song03 (0:05:37)', 'song05 (0:05:54)']\n  [2] 0:12:22 ['song09 (0:02:50)', 'song08 (0:04:41)', 'song04 (0:04:51)']\n  [3] 0:12:42 ['song02 (0:03:41)', 'song07 (0:03:45)', 'song06 (0:05:16)']\n",
         None,
         0
     ),
     (
         [__project__, '--quiet', '-s', 'song05:5m54s', '-s', 'song03:5m37s', '-s', 'song06:5m16s', '-s', 'song04:4m51s', '-s', 'song08:4m41s', '-s', 'song07:3m45s', '-s', 'song02:3m41s', '-s', 'song09:2m50s', '-s', 'song01:0m55s', '-g', '2'],
-        "(8, [(1121, [(354, 'song05'), (316, 'song06'), (281, 'song08'), (170, 'song09')]), (1129, [(337, 'song03'), (291, 'song04'), (225, 'song07'), (221, 'song02'), (55, 'song01')])])\n",
+        "(8, ((1129, ((55, 'song01'), (221, 'song02'), (225, 'song07'), (291, 'song04'), (337, 'song03'))), (1121, ((170, 'song09'), (281, 'song08'), (316, 'song06'), (354, 'song05')))))\n",
         None,
         0
     ),
 ])
 def test___main__(capsys, mocker, args, output, exception, exit_code):
     """test___main__."""
     mocker.patch.object(sys, 'argv', args)
```

### Comparing `arrangio-0.1.0/tests/test__parser_.py` & `arrangio-0.2.0/tests/test__parser_.py`

 * *Files identical despite different names*

### Comparing `arrangio-0.1.0/tests/test__utils_.py` & `arrangio-0.2.0/tests/test__utils_.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,61 +49,61 @@
 
 @mark.parametrize('args,result,exception', [
     (['01'], None, ValueError),
     (['00:01'], None, ValueError),
     (['label'], None, ValueError),
     (['label:'], None, ValueError),
     (['label:00:01'], None, ValueError),
-    (['song_01:0h0m1s'], [(1, 'song_01')], None),
-    (['song_01:00h00m01s'], [(1, 'song_01')], None),
-    (['song_01:00m01s'], [(1, 'song_01')], None),
-    (['song_01:01s'], [(1, 'song_01')], None),
-    (['song01:02s', 'song02:01s'], [(2, 'song01'), (1, 'song02')], None),
+    (['song_01:0h0m1s'], ((1, 'song_01'),), None),
+    (['song_01:00h00m01s'], ((1, 'song_01'),), None),
+    (['song_01:00m01s'], ((1, 'song_01'),), None),
+    (['song_01:01s'], ((1, 'song_01'),), None),
+    (['song01:02s', 'song02:01s'], ((2, 'song01'), (1, 'song02'),), None),
 ])
 def test__utils__get_songs(args, result, exception):
     """test__utils__get_songs."""
     if exception:
         with raises(exception):
             _ = utils.get_songs(args)
     else:
         assert result == utils.get_songs(args)
 
 
 @mark.parametrize('args,result', [
-    ([[], 0, [(0, [])]], (0, [(0, [])])),
-    ([[(2, 'song_01')], 1, [(0, [])]], (0, [(2, [(2, 'song_01')])])),
+    ([(), 0, ((0, ()),)], (0, ((0, ()),))),
+    ([((2, 'song_01'),), 1, ((0, ()),)], (0, ((2, ((2, 'song_01'),)),))),
 ])
 def test__utils____get_subsets(args, result):
     """test__utils____get_subsets."""
     assert result == utils.__get_subsets(*args)
 
 
 @mark.parametrize('args,result', [
-    ([[], 1], (0, [(0, [])])),
+    ([(), 1], (0, ((0, ()),))),
     (
-        [[(354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')], 2],
-        (8, [(1121, [(354, 'song05'), (316, 'song06'), (281, 'song08'), (170, 'song09')]), (1129, [(337, 'song03'), (291, 'song04'), (225, 'song07'), (221, 'song02'), (55, 'song01')])])
+        [((354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')), 2],
+        (8, ((1129, ((55, 'song01'), (221, 'song02'), (225, 'song07'), (291, 'song04'), (337, 'song03'))), (1121, ((170, 'song09'), (281, 'song08'), (316, 'song06'), (354, 'song05')))))
     ),
     (
-        [[(354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')], 3],
-        (20, [(762, [(316, 'song06'), (225, 'song07'), (221, 'song02')]), (742, [(291, 'song04'), (281, 'song08'), (170, 'song09')]), (746, [(354, 'song05'), (337, 'song03'), (55, 'song01')])])
+        [((354, 'song05'), (337, 'song03'), (316, 'song06'), (291, 'song04'), (281, 'song08'), (225, 'song07'), (221, 'song02'), (170, 'song09'), (55, 'song01')), 3],
+        (20, ((746, ((55, 'song01'), (337, 'song03'), (354, 'song05'))), (742, ((170, 'song09'), (281, 'song08'), (291, 'song04'))), (762, ((221, 'song02'), (225, 'song07'), (316, 'song06')))))
     ),
 ])
 def test__utils__get_subsets(args, result):
     """test__utils__get_subsets."""
     assert result == utils.get_subsets(*args)
 
 
 @mark.parametrize('args,result', [
     (
-        (8, [(1121, [(354, 'song05'), (316, 'song06'), (281, 'song08'), (170, 'song09')]), (1129, [(337, 'song03'), (291, 'song04'), (225, 'song07'), (221, 'song02'), (55, 'song01')])]),
+        (8, ((1121, ((354, 'song05'), (316, 'song06'), (281, 'song08'), (170, 'song09'))), (1129, ((337, 'song03'), (291, 'song04'), (225, 'song07'), (221, 'song02'), (55, 'song01'))))),
         "Difference (in seconds): 8\nGroups:\n  [1] 0:18:41 ['song05 (0:05:54)', 'song06 (0:05:16)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [2] 0:18:49 ['song03 (0:05:37)', 'song04 (0:04:51)', 'song07 (0:03:45)', 'song02 (0:03:41)', 'song01 (0:00:55)']\n"
     ),
     (
-        (20, [(762, [(316, 'song06'), (225, 'song07'), (221, 'song02')]), (742, [(291, 'song04'), (281, 'song08'), (170, 'song09')]), (746, [(354, 'song05'), (337, 'song03'), (55, 'song01')])]),
+        (20, ((762, ((316, 'song06'), (225, 'song07'), (221, 'song02'))), (742, ((291, 'song04'), (281, 'song08'), (170, 'song09'))), (746, ((354, 'song05'), (337, 'song03'), (55, 'song01'))))),
         "Difference (in seconds): 20\nGroups:\n  [1] 0:12:42 ['song06 (0:05:16)', 'song07 (0:03:45)', 'song02 (0:03:41)']\n  [2] 0:12:22 ['song04 (0:04:51)', 'song08 (0:04:41)', 'song09 (0:02:50)']\n  [3] 0:12:26 ['song05 (0:05:54)', 'song03 (0:05:37)', 'song01 (0:00:55)']\n"
     ),
 ])
 def test__utils__show_results(capsys, args, result):
     """test__utils__show_results."""
     utils.show_results(args)
     stdout, _ = capsys.readouterr()
```

