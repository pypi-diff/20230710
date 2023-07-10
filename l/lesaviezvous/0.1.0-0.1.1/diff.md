# Comparing `tmp/lesaviezvous-0.1.0.tar.gz` & `tmp/lesaviezvous-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesaviezvous-0.1.0.tar", last modified: Mon Jul 10 06:42:23 2023, max compression
+gzip compressed data, was "lesaviezvous-0.1.1.tar", last modified: Mon Jul 10 07:06:03 2023, max compression
```

## Comparing `lesaviezvous-0.1.0.tar` & `lesaviezvous-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 06:42:23.568877 lesaviezvous-0.1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      191 2023-07-10 06:42:23.568877 lesaviezvous-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 06:42:23.564877 lesaviezvous-0.1.0/lesaviezvous/
--rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.0/lesaviezvous/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 06:39:07.000000 lesaviezvous-0.1.0/lesaviezvous/lesaviezvous.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 06:42:23.568877 lesaviezvous-0.1.0/lesaviezvous.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      191 2023-07-10 06:42:23.000000 lesaviezvous-0.1.0/lesaviezvous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      264 2023-07-10 06:42:23.000000 lesaviezvous-0.1.0/lesaviezvous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 06:42:23.000000 lesaviezvous-0.1.0/lesaviezvous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 06:42:23.000000 lesaviezvous-0.1.0/lesaviezvous.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 06:42:23.000000 lesaviezvous-0.1.0/lesaviezvous.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 lesaviezvous-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 06:42:23.568877 lesaviezvous-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-10 06:40:39.000000 lesaviezvous-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:06:03.546322 lesaviezvous-0.1.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 lesaviezvous-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1641 2023-07-10 07:06:03.546322 lesaviezvous-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      544 2023-07-10 07:01:15.000000 lesaviezvous-0.1.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:06:03.546322 lesaviezvous-0.1.1/lesaviezvous/
+-rw-r--r--   0 runner    (1000) runner    (1000)      214 2023-07-10 06:39:24.000000 lesaviezvous-0.1.1/lesaviezvous/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-10 06:39:07.000000 lesaviezvous-0.1.1/lesaviezvous/lesaviezvous.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 07:06:03.546322 lesaviezvous-0.1.1/lesaviezvous.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1641 2023-07-10 07:06:03.000000 lesaviezvous-0.1.1/lesaviezvous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      274 2023-07-10 07:06:03.000000 lesaviezvous-0.1.1/lesaviezvous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 07:06:03.000000 lesaviezvous-0.1.1/lesaviezvous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-10 07:06:03.000000 lesaviezvous-0.1.1/lesaviezvous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-10 07:06:03.000000 lesaviezvous-0.1.1/lesaviezvous.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 lesaviezvous-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 07:06:03.546322 lesaviezvous-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      860 2023-07-10 07:06:00.000000 lesaviezvous-0.1.1/setup.py
```

### Comparing `lesaviezvous-0.1.0/LICENSE` & `lesaviezvous-0.1.1/LICENSE`

 * *Files identical despite different names*

