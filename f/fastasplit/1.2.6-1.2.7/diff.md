# Comparing `tmp/fastasplit-1.2.6.tar.gz` & `tmp/fastasplit-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastasplit-1.2.6.tar", last modified: Sun Jul  9 02:42:40 2023, max compression
+gzip compressed data, was "fastasplit-1.2.7.tar", last modified: Mon Jul 10 19:21:49 2023, max compression
```

## Comparing `fastasplit-1.2.6.tar` & `fastasplit-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-09 02:42:40.240299 fastasplit-1.2.6/
--rw-rw-r--   0 josh      (1000) josh      (1000)    35149 2023-07-08 02:32:46.000000 fastasplit-1.2.6/LICENSE
--rw-rw-r--   0 josh      (1000) josh      (1000)      294 2023-07-09 02:42:40.240299 fastasplit-1.2.6/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      582 2023-07-08 16:32:00.000000 fastasplit-1.2.6/README.md
--rw-rw-r--   0 josh      (1000) josh      (1000)      301 2023-07-08 02:32:46.000000 fastasplit-1.2.6/changelog.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       80 2023-07-09 00:47:26.000000 fastasplit-1.2.6/pyproject.toml
--rw-rw-r--   0 josh      (1000) josh      (1000)      508 2023-07-09 02:42:40.244299 fastasplit-1.2.6/setup.cfg
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-09 02:42:40.240299 fastasplit-1.2.6/src/
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-09 02:42:40.240299 fastasplit-1.2.6/src/fastasplit/
--rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-07-09 02:03:27.000000 fastasplit-1.2.6/src/fastasplit/__init__.py
--rwxrwxr-x   0 josh      (1000) josh      (1000)     7834 2023-07-09 02:42:06.000000 fastasplit-1.2.6/src/fastasplit/fastasplit.py
--rw-rw-r--   0 josh      (1000) josh      (1000)       27 2023-07-09 02:32:52.000000 fastasplit-1.2.6/src/fastasplit/test.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-09 02:42:40.240299 fastasplit-1.2.6/src/fastasplit.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)      294 2023-07-09 02:42:40.000000 fastasplit-1.2.6/src/fastasplit.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      328 2023-07-09 02:42:40.000000 fastasplit-1.2.6/src/fastasplit.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-07-09 02:42:40.000000 fastasplit-1.2.6/src/fastasplit.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       58 2023-07-09 02:42:40.000000 fastasplit-1.2.6/src/fastasplit.egg-info/entry_points.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       11 2023-07-09 02:42:40.000000 fastasplit-1.2.6/src/fastasplit.egg-info/top_level.txt
+drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.829859 fastasplit-1.2.7/
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)    35149 2023-07-10 18:45:06.000000 fastasplit-1.2.7/LICENSE
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)     1140 2023-07-10 19:21:49.829975 fastasplit-1.2.7/PKG-INFO
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)      805 2023-07-10 18:45:06.000000 fastasplit-1.2.7/README.md
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)       80 2023-07-10 18:45:06.000000 fastasplit-1.2.7/pyproject.toml
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)      589 2023-07-10 19:21:49.830648 fastasplit-1.2.7/setup.cfg
+drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.823246 fastasplit-1.2.7/src/
+drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.825497 fastasplit-1.2.7/src/fastasplit/
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 18:45:06.000000 fastasplit-1.2.7/src/fastasplit/__init__.py
+-rwxr-xr-x   0 joshuabenoit   (501) staff       (20)     7834 2023-07-10 18:45:06.000000 fastasplit-1.2.7/src/fastasplit/fastasplit.py
+drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.829551 fastasplit-1.2.7/src/fastasplit.egg-info/
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)     1140 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/PKG-INFO
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)      291 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)        1 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)       58 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/entry_points.txt
+-rw-r--r--   0 joshuabenoit   (501) staff       (20)       11 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/top_level.txt
```

### Comparing `fastasplit-1.2.6/LICENSE` & `fastasplit-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastasplit-1.2.6/src/fastasplit/fastasplit.py` & `fastasplit-1.2.7/src/fastasplit/fastasplit.py`

 * *Files identical despite different names*

