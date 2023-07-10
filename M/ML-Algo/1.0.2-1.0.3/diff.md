# Comparing `tmp/ML_Algo-1.0.2.tar.gz` & `tmp/ML_Algo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML_Algo-1.0.2.tar", last modified: Sun Jul  9 03:11:42 2023, max compression
+gzip compressed data, was "ML_Algo-1.0.3.tar", last modified: Mon Jul 10 11:18:49 2023, max compression
```

## Comparing `ML_Algo-1.0.2.tar` & `ML_Algo-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:42.742541 ML_Algo-1.0.2/
--rw-rw-rw-   0        0        0      164 2023-07-09 03:11:42.741542 ML_Algo-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 03:11:42.743556 ML_Algo-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-07-09 03:10:47.000000 ML_Algo-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:42.730452 ML_Algo-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:42.739541 ML_Algo-1.0.2/src/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-09 03:11:42.000000 ML_Algo-1.0.2/src/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-09 03:11:42.000000 ML_Algo-1.0.2/src/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:11:42.000000 ML_Algo-1.0.2/src/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-09 03:11:42.000000 ML_Algo-1.0.2/src/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:11:42.000000 ML_Algo-1.0.2/src/ML_Algo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 11:18:49.880647 ML_Algo-1.0.3/
+-rw-rw-rw-   0        0        0      164 2023-07-10 11:18:49.879645 ML_Algo-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-10 11:18:49.880647 ML_Algo-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-07-10 11:18:32.000000 ML_Algo-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:18:49.873645 ML_Algo-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 11:18:49.879645 ML_Algo-1.0.3/src/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-10 11:18:49.000000 ML_Algo-1.0.3/src/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-10 11:18:49.000000 ML_Algo-1.0.3/src/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 11:18:49.000000 ML_Algo-1.0.3/src/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 11:18:49.000000 ML_Algo-1.0.3/src/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 11:18:49.000000 ML_Algo-1.0.3/src/ML_Algo.egg-info/top_level.txt
```

