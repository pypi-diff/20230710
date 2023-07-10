# Comparing `tmp/ormstrorm-0.0.1.tar.gz` & `tmp/ormstrorm-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormstrorm-0.0.1.tar", last modified: Mon Jul 10 18:23:45 2023, max compression
+gzip compressed data, was "ormstrorm-0.0.1.1.tar", last modified: Mon Jul 10 18:34:40 2023, max compression
```

## Comparing `ormstrorm-0.0.1.tar` & `ormstrorm-0.0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:45.153507 ormstrorm-0.0.1/
--rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstrorm-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      521 2023-07-10 18:23:45.153507 ormstrorm-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:45.140100 ormstrorm-0.0.1/ormstorm/
--rw-rw-rw-   0        0        0     5563 2023-07-10 17:21:01.000000 ormstrorm-0.0.1/ormstorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:23:45.153507 ormstrorm-0.0.1/ormstrorm.egg-info/
--rw-rw-rw-   0        0        0      521 2023-07-10 18:23:45.000000 ormstrorm-0.0.1/ormstrorm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-07-10 18:23:45.000000 ormstrorm-0.0.1/ormstrorm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:23:45.000000 ormstrorm-0.0.1/ormstrorm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 18:23:45.000000 ormstrorm-0.0.1/ormstrorm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 18:23:45.153507 ormstrorm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-07-10 18:20:27.000000 ormstrorm-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:40.234435 ormstrorm-0.0.1.1/
+-rw-rw-rw-   0        0        0     1069 2023-07-10 18:22:37.000000 ormstrorm-0.0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2149 2023-07-10 18:34:40.234435 ormstrorm-0.0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:40.234435 ormstrorm-0.0.1.1/ormstorm/
+-rw-rw-rw-   0        0        0     5563 2023-07-10 17:21:01.000000 ormstrorm-0.0.1.1/ormstorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:34:40.234435 ormstrorm-0.0.1.1/ormstrorm.egg-info/
+-rw-rw-rw-   0        0        0     2149 2023-07-10 18:34:40.000000 ormstrorm-0.0.1.1/ormstrorm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-07-10 18:34:40.000000 ormstrorm-0.0.1.1/ormstrorm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:34:40.000000 ormstrorm-0.0.1.1/ormstrorm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 18:34:40.000000 ormstrorm-0.0.1.1/ormstrorm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:34:40.234435 ormstrorm-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-07-10 18:34:23.000000 ormstrorm-0.0.1.1/setup.py
```

### Comparing `ormstrorm-0.0.1/LICENSE.txt` & `ormstrorm-0.0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ormstrorm-0.0.1/ormstorm/__init__.py` & `ormstrorm-0.0.1.1/ormstorm/__init__.py`

 * *Files identical despite different names*

