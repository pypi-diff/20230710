# Comparing `tmp/unitxt-0.0.1.tar.gz` & `tmp/unitxt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-0.0.1.tar", last modified: Mon Jun 19 13:19:14 2023, max compression
+gzip compressed data, was "unitxt-1.0.0.tar", last modified: Mon Jul 10 13:08:10 2023, max compression
```

## Comparing `unitxt-0.0.1.tar` & `unitxt-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,46 @@
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-06-19 13:19:14.194241 unitxt-0.0.1/
--rw-rw-r--   0 elron    (605371) tslm      (3127)      232 2023-06-19 13:19:14.193908 unitxt-0.0.1/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)       42 2023-06-19 13:07:43.000000 unitxt-0.0.1/README.md
--rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-06-19 13:19:14.194340 unitxt-0.0.1/setup.cfg
--rw-rw-r--   0 elron    (605371) tslm      (3127)      305 2023-06-19 13:17:47.000000 unitxt-0.0.1/setup.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-06-19 13:19:14.189140 unitxt-0.0.1/src/
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-06-19 13:19:14.190997 unitxt-0.0.1/src/unitxt/
--rw-rw-r--   0 elron    (605371) tslm      (3127)       44 2023-06-19 13:13:26.000000 unitxt-0.0.1/src/unitxt/__init__.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-06-19 13:19:14.193435 unitxt-0.0.1/src/unitxt.egg-info/
--rw-rw-r--   0 elron    (605371) tslm      (3127)      232 2023-06-19 13:19:13.000000 unitxt-0.0.1/src/unitxt.egg-info/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)      177 2023-06-19 13:19:13.000000 unitxt-0.0.1/src/unitxt.egg-info/SOURCES.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-06-19 13:19:13.000000 unitxt-0.0.1/src/unitxt.egg-info/dependency_links.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-06-19 13:19:13.000000 unitxt-0.0.1/src/unitxt.egg-info/top_level.txt
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.126247 unitxt-1.0.0/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-06-19 13:07:43.000000 unitxt-1.0.0/LICENSE
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-10 12:37:43.000000 unitxt-1.0.0/MANIFEST.in
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2204 2023-07-10 13:08:10.125508 unitxt-1.0.0/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1446 2023-07-10 12:46:11.000000 unitxt-1.0.0/README.md
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       56 2023-07-10 12:37:46.000000 unitxt-1.0.0/pyproject.toml
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-10 13:08:10.126356 unitxt-1.0.0/setup.cfg
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      829 2023-07-10 12:37:52.000000 unitxt-1.0.0/setup.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.069353 unitxt-1.0.0/src/
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.120679 unitxt-1.0.0/src/unitxt/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      164 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/__init__.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     5949 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/artifact.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1141 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/blocks.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/card.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2670 2023-07-10 12:59:31.000000 unitxt-1.0.0/src/unitxt/catalog.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      946 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/collections.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2933 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/common.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3034 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/dataset.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/file_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      414 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/fusion.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/generator_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/instructions.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      658 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/load.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      668 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/loaders.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4564 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/metric.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/metrics.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/normalizers.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/operator.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     7105 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/operators.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/processors.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/recipe.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      487 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/register.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/schema.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)    11071 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/split_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     3557 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/splitters.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/stream.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/task.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/templates.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/text_utils.py
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     1401 2023-07-10 12:35:56.000000 unitxt-1.0.0/src/unitxt/validate.py
+drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-10 13:08:10.124646 unitxt-1.0.0/src/unitxt.egg-info/
+-rw-rw-r--   0 elron    (605371) tslm      (3127)     2204 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/PKG-INFO
+-rw-rw-r--   0 elron    (605371) tslm      (3127)      911 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/requires.txt
+-rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-10 13:08:09.000000 unitxt-1.0.0/src/unitxt.egg-info/top_level.txt
```

