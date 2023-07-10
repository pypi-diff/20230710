# Comparing `tmp/typetype-1.0.3.tar.gz` & `tmp/typetype-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.3.tar", last modified: Mon Jul 10 05:59:39 2023, max compression
+gzip compressed data, was "typetype-1.0.4.tar", last modified: Mon Jul 10 06:19:37 2023, max compression
```

## Comparing `typetype-1.0.3.tar` & `typetype-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:59:39.297170 typetype-1.0.3/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:59:39.297032 typetype-1.0.3/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.3/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 05:59:39.297222 typetype-1.0.3/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      504 2023-07-10 05:58:39.000000 typetype-1.0.3/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:59:39.292221 typetype-1.0.3/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.3/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:59:39.293533 typetype-1.0.3/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.3/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:59:39.294570 typetype-1.0.3/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.3/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:59:39.292999 typetype-1.0.3/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:59:39.000000 typetype-1.0.3/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      507 2023-07-10 05:59:39.000000 typetype-1.0.3/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 05:59:39.000000 typetype-1.0.3/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 05:59:39.000000 typetype-1.0.3/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 05:59:39.000000 typetype-1.0.3/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:19:37.828988 typetype-1.0.4/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 06:19:37.828864 typetype-1.0.4/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.4/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 06:19:37.829028 typetype-1.0.4/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      651 2023-07-10 06:18:34.000000 typetype-1.0.4/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:19:37.823917 typetype-1.0.4/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.4/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:19:37.825399 typetype-1.0.4/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.0.4/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:19:37.826502 typetype-1.0.4/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.0.4/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 06:19:37.824856 typetype-1.0.4/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 06:19:37.000000 typetype-1.0.4/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      507 2023-07-10 06:19:37.000000 typetype-1.0.4/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 06:19:37.000000 typetype-1.0.4/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 06:19:37.000000 typetype-1.0.4/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 06:19:37.000000 typetype-1.0.4/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.3/README.md` & `typetype-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/ahmetsgame.py` & `typetype-1.0.4/typetype/ahmetsgame.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/functions/game_selection.py` & `typetype-1.0.4/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/functions/refresh_update.py` & `typetype-1.0.4/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/functions/setup_results.py` & `typetype-1.0.4/typetype/functions/setup_results.py`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/words/200words.txt` & `typetype-1.0.4/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/words/25000words.txt` & `typetype-1.0.4/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/words/5000words.txt` & `typetype-1.0.4/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.0.3/typetype/words/text.txt` & `typetype-1.0.4/typetype/words/text.txt`

 * *Files identical despite different names*

