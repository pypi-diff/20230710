# Comparing `tmp/SwarAnuvad-2.4.0.tar.gz` & `tmp/SwarAnuvad-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwarAnuvad-2.4.0.tar", last modified: Mon Jul 10 06:43:03 2023, max compression
+gzip compressed data, was "SwarAnuvad-2.4.3.tar", last modified: Mon Jul 10 06:33:56 2023, max compression
```

## Comparing `SwarAnuvad-2.4.0.tar` & `SwarAnuvad-2.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:43:03.161433 SwarAnuvad-2.4.0/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     3511 2023-07-10 06:43:03.161433 SwarAnuvad-2.4.0/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1013 2023-07-10 06:27:32.000000 SwarAnuvad-2.4.0/README.md
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:43:03.161433 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     3511 2023-07-10 06:43:03.000000 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)      210 2023-07-10 06:43:03.000000 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/SOURCES.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 06:43:03.000000 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/dependency_links.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 06:43:03.000000 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/requires.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 06:43:03.000000 SwarAnuvad-2.4.0/SwarAnuvad.egg-info/top_level.txt
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:43:03.161433 SwarAnuvad-2.4.0/sWaraNuvad/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 SwarAnuvad-2.4.0/sWaraNuvad/__init__.py
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 06:43:03.161433 SwarAnuvad-2.4.0/setup.cfg
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     3803 2023-07-10 06:42:53.000000 SwarAnuvad-2.4.0/setup.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:33:56.195786 SwarAnuvad-2.4.3/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1589 2023-07-10 06:33:56.195786 SwarAnuvad-2.4.3/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1013 2023-07-10 06:27:32.000000 SwarAnuvad-2.4.3/README.md
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:33:56.195786 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1589 2023-07-10 06:33:56.000000 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      210 2023-07-10 06:33:56.000000 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/SOURCES.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 06:33:56.000000 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/dependency_links.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 06:33:56.000000 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/requires.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 06:33:56.000000 SwarAnuvad-2.4.3/SwarAnuvad.egg-info/top_level.txt
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:33:56.195786 SwarAnuvad-2.4.3/sWaraNuvad/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 SwarAnuvad-2.4.3/sWaraNuvad/__init__.py
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 06:33:56.199786 SwarAnuvad-2.4.3/setup.cfg
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1881 2023-07-10 06:33:55.000000 SwarAnuvad-2.4.3/setup.py
```

### Comparing `SwarAnuvad-2.4.0/README.md` & `SwarAnuvad-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `SwarAnuvad-2.4.0/sWaraNuvad/__init__.py` & `SwarAnuvad-2.4.3/sWaraNuvad/__init__.py`

 * *Files identical despite different names*

