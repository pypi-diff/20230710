# Comparing `tmp/diz-0.0.1.tar.gz` & `tmp/diz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.1.tar", last modified: Sun Jul  9 15:37:19 2023, max compression
+gzip compressed data, was "diz-0.0.2.tar", last modified: Mon Jul 10 03:33:56 2023, max compression
```

## Comparing `diz-0.0.1.tar` & `diz-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-09 15:37:19.157730 diz-0.0.1/
--rw-r--r--   0 mj         (501) staff       (20)      104 2023-07-09 15:37:19.157614 diz-0.0.1/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)        6 2023-07-09 15:30:43.000000 diz-0.0.1/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-09 15:37:19.155190 diz-0.0.1/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.1/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)     2067 2023-07-09 15:14:17.000000 diz-0.0.1/commands/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-09 15:37:19.155954 diz-0.0.1/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)      104 2023-07-09 15:37:19.000000 diz-0.0.1/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      287 2023-07-09 15:37:19.000000 diz-0.0.1/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-09 15:37:19.000000 diz-0.0.1/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-09 15:37:19.000000 diz-0.0.1/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)       15 2023-07-09 15:37:19.000000 diz-0.0.1/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-09 15:37:19.157768 diz-0.0.1/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      386 2023-07-09 15:36:49.000000 diz-0.0.1/setup.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-09 15:37:19.157292 diz-0.0.1/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.1/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.1/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.1/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      758 2023-07-09 15:11:55.000000 diz-0.0.1/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.1/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      313 2023-07-09 14:46:10.000000 diz-0.0.1/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.182610 diz-0.0.2/
+-rw-r--r--   0 mj         (501) staff       (20)      173 2023-07-10 03:33:56.182429 diz-0.0.2/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.2/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.179496 diz-0.0.2/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.2/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)     2067 2023-07-09 15:14:17.000000 diz-0.0.2/commands/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.180443 diz-0.0.2/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)      173 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      317 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       37 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)       15 2023-07-10 03:33:56.000000 diz-0.0.2/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 03:33:56.182687 diz-0.0.2/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      597 2023-07-10 03:33:34.000000 diz-0.0.2/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 03:33:56.181975 diz-0.0.2/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.2/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.2/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.2/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      758 2023-07-09 15:11:55.000000 diz-0.0.2/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.2/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      313 2023-07-09 14:46:10.000000 diz-0.0.2/utils/yaml.py
```

### Comparing `diz-0.0.1/commands/setup.py` & `diz-0.0.2/commands/setup.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.1/utils/pip.py` & `diz-0.0.2/utils/pip.py`

 * *Files identical despite different names*

