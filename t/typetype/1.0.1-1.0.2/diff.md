# Comparing `tmp/typetype-1.0.1.tar.gz` & `tmp/typetype-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.1.tar", last modified: Mon Jul 10 05:36:44 2023, max compression
+gzip compressed data, was "typetype-1.0.2.tar", last modified: Mon Jul 10 05:47:37 2023, max compression
```

## Comparing `typetype-1.0.1.tar` & `typetype-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.248934 typetype-1.0.1/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:36:44.248828 typetype-1.0.1/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.1/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 05:36:44.248971 typetype-1.0.1/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      438 2023-07-10 05:36:05.000000 typetype-1.0.1/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.247927 typetype-1.0.1/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.1/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.1/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.248667 typetype-1.0.1/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      225 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:47:37.872549 typetype-1.0.2/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:47:37.872439 typetype-1.0.2/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.2/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 05:47:37.872587 typetype-1.0.2/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      477 2023-07-10 05:46:39.000000 typetype-1.0.2/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:47:37.871036 typetype-1.0.2/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.2/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.2/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:47:37.872238 typetype-1.0.2/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10348 2023-07-10 04:56:06.000000 typetype-1.0.2/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8879 2023-07-10 04:56:06.000000 typetype-1.0.2/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7939 2023-07-10 04:56:06.000000 typetype-1.0.2/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:47:37.871833 typetype-1.0.2/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:47:37.000000 typetype-1.0.2/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      335 2023-07-10 05:47:37.000000 typetype-1.0.2/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 05:47:37.000000 typetype-1.0.2/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 05:47:37.000000 typetype-1.0.2/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 05:47:37.000000 typetype-1.0.2/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.1/README.md` & `typetype-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.1/typetype/ahmetsgame.py` & `typetype-1.0.2/typetype/ahmetsgame.py`

 * *Files identical despite different names*

