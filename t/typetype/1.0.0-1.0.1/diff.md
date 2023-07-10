# Comparing `tmp/typetype-1.0.0.tar.gz` & `tmp/typetype-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.0.0.tar", last modified: Mon Jul 10 05:09:28 2023, max compression
+gzip compressed data, was "typetype-1.0.1.tar", last modified: Mon Jul 10 05:36:44 2023, max compression
```

## Comparing `typetype-1.0.0.tar` & `typetype-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:09:28.269098 typetype-1.0.0/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      107 2023-07-10 05:09:28.268999 typetype-1.0.0/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.0/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 05:09:28.269135 typetype-1.0.0/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      385 2023-07-10 04:56:06.000000 typetype-1.0.0/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:09:28.268122 typetype-1.0.0/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.0/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.0/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:09:28.268843 typetype-1.0.0/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)      107 2023-07-10 05:09:28.000000 typetype-1.0.0/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      225 2023-07-10 05:09:28.000000 typetype-1.0.0/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 05:09:28.000000 typetype-1.0.0/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       54 2023-07-10 05:09:28.000000 typetype-1.0.0/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 05:09:28.000000 typetype-1.0.0/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.248934 typetype-1.0.1/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:36:44.248828 typetype-1.0.1/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1112 2023-07-10 04:56:06.000000 typetype-1.0.1/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-10 05:36:44.248971 typetype-1.0.1/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      438 2023-07-10 05:36:05.000000 typetype-1.0.1/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.247927 typetype-1.0.1/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:02:10.000000 typetype-1.0.1/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7769 2023-07-10 04:56:06.000000 typetype-1.0.1/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:36:44.248667 typetype-1.0.1/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      156 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      225 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-10 05:36:44.000000 typetype-1.0.1/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.0.0/README.md` & `typetype-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.0.0/typetype/ahmetsgame.py` & `typetype-1.0.1/typetype/ahmetsgame.py`

 * *Files identical despite different names*

