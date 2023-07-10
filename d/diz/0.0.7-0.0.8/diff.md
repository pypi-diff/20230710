# Comparing `tmp/diz-0.0.7.tar.gz` & `tmp/diz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-0.0.7.tar", last modified: Mon Jul 10 04:17:13 2023, max compression
+gzip compressed data, was "diz-0.0.8.tar", last modified: Mon Jul 10 07:30:00 2023, max compression
```

## Comparing `diz-0.0.7.tar` & `diz-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.074743 diz-0.0.7/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 04:17:13.074635 diz-0.0.7/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)       63 2023-07-10 03:31:32.000000 diz-0.0.7/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.072886 diz-0.0.7/diz/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.7/diz/__init__.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.073802 diz-0.0.7/diz/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.7/diz/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.7/diz/commands/setup.py
--rw-r--r--   0 mj         (501) staff       (20)      772 2023-07-10 03:56:40.000000 diz-0.0.7/diz/main.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.074478 diz-0.0.7/diz/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.7/diz/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.7/diz/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.7/diz/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.7/diz/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.7/diz/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.7/diz/utils/yaml.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 04:17:13.073592 diz-0.0.7/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)      213 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      377 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)       98 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 04:17:13.000000 diz-0.0.7/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 04:17:13.074787 diz-0.0.7/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      649 2023-07-10 04:16:24.000000 diz-0.0.7/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.327637 diz-0.0.8/
+-rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:30:00.327514 diz-0.0.8/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)     1218 2023-07-10 07:28:47.000000 diz-0.0.8/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.324674 diz-0.0.8/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-0.0.8/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.325826 diz-0.0.8/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-0.0.8/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-0.0.8/diz/commands/install.py
+-rw-r--r--   0 mj         (501) staff       (20)     2108 2023-07-10 03:54:31.000000 diz-0.0.8/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)      870 2023-07-10 07:08:04.000000 diz-0.0.8/diz/commands/shell.py
+-rw-r--r--   0 mj         (501) staff       (20)     1572 2023-07-10 07:26:28.000000 diz-0.0.8/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.327211 diz-0.0.8/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-0.0.8/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-0.0.8/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-0.0.8/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      762 2023-07-10 04:14:00.000000 diz-0.0.8/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-0.0.8/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-0.0.8/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 07:30:00.325317 diz-0.0.8/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)     1368 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      423 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 07:30:00.000000 diz-0.0.8/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 07:30:00.327679 diz-0.0.8/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 07:29:17.000000 diz-0.0.8/setup.py
```

### Comparing `diz-0.0.7/diz/commands/setup.py` & `diz-0.0.8/diz/commands/setup.py`

 * *Files identical despite different names*

### Comparing `diz-0.0.7/diz/utils/pip.py` & `diz-0.0.8/diz/utils/pip.py`

 * *Files identical despite different names*

