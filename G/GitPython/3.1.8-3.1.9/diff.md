# Comparing `tmp/GitPython-3.1.8.tar.gz` & `tmp/GitPython-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GitPython-3.1.8.tar", last modified: Fri Sep  4 02:04:49 2020, max compression
+gzip compressed data, was "dist/GitPython-3.1.9.tar", last modified: Thu Oct  1 03:19:37 2020, max compression
```

## Comparing `GitPython-3.1.8.tar` & `GitPython-3.1.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.525039 GitPython-3.1.8/
--rw-r--r--   0 byron      (501) staff       (20)     1875 2020-09-01 02:48:38.000000 GitPython-3.1.8/AUTHORS
--rw-r--r--   0 byron      (501) staff       (20)      147 2020-01-31 04:46:36.000000 GitPython-3.1.8/CHANGES
--rw-r--r--   0 byron      (501) staff       (20)      443 2020-09-03 02:21:08.000000 GitPython-3.1.8/CONTRIBUTING.md
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.485140 GitPython-3.1.8/GitPython.egg-info/
--rw-r--r--   0 byron      (501) staff       (20)     1086 2020-09-04 02:04:49.000000 GitPython-3.1.8/GitPython.egg-info/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)     1198 2020-09-04 02:04:49.000000 GitPython-3.1.8/GitPython.egg-info/SOURCES.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2020-09-04 02:04:49.000000 GitPython-3.1.8/GitPython.egg-info/dependency_links.txt
--rw-r--r--   0 byron      (501) staff       (20)        1 2020-02-08 03:14:00.000000 GitPython-3.1.8/GitPython.egg-info/not-zip-safe
--rw-r--r--   0 byron      (501) staff       (20)       16 2020-09-04 02:04:49.000000 GitPython-3.1.8/GitPython.egg-info/requires.txt
--rw-r--r--   0 byron      (501) staff       (20)        4 2020-09-04 02:04:49.000000 GitPython-3.1.8/GitPython.egg-info/top_level.txt
--rw-r--r--   0 byron      (501) staff       (20)     1521 2020-01-31 04:46:36.000000 GitPython-3.1.8/LICENSE
--rw-r--r--   0 byron      (501) staff       (20)      215 2020-07-13 02:09:59.000000 GitPython-3.1.8/MANIFEST.in
--rw-r--r--   0 byron      (501) staff       (20)     1086 2020-09-04 02:04:49.524558 GitPython-3.1.8/PKG-INFO
--rw-r--r--   0 byron      (501) staff       (20)     8564 2020-09-02 02:01:00.000000 GitPython-3.1.8/README.md
--rw-r--r--   0 byron      (501) staff       (20)        6 2020-09-04 01:53:35.000000 GitPython-3.1.8/VERSION
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.486719 GitPython-3.1.8/doc/
--rw-r--r--   0 byron      (501) staff       (20)        7 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/.gitignore
--rw-r--r--   0 byron      (501) staff       (20)     2347 2020-08-12 12:03:55.000000 GitPython-3.1.8/doc/Makefile
--rw-r--r--   0 byron      (501) staff       (20)       28 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/requirements.txt
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.491980 GitPython-3.1.8/doc/source/
--rw-r--r--   0 byron      (501) staff       (20)    36526 2020-09-04 01:53:29.000000 GitPython-3.1.8/doc/source/changes.rst
--rw-r--r--   0 byron      (501) staff       (20)     6112 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/source/conf.py
--rw-r--r--   0 byron      (501) staff       (20)      445 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/source/index.rst
--rw-r--r--   0 byron      (501) staff       (20)     3923 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/source/intro.rst
--rw-r--r--   0 byron      (501) staff       (20)     3319 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/source/reference.rst
--rw-r--r--   0 byron      (501) staff       (20)      237 2020-05-04 09:48:58.000000 GitPython-3.1.8/doc/source/roadmap.rst
--rw-r--r--   0 byron      (501) staff       (20)    24639 2020-07-13 06:21:22.000000 GitPython-3.1.8/doc/source/tutorial.rst
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.502481 GitPython-3.1.8/git/
--rw-r--r--   0 byron      (501) staff       (20)     2399 2020-09-04 02:04:49.525465 GitPython-3.1.8/git/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)    42316 2020-07-06 07:36:41.000000 GitPython-3.1.8/git/cmd.py
--rw-r--r--   0 byron      (501) staff       (20)     1928 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/compat.py
--rw-r--r--   0 byron      (501) staff       (20)    30292 2020-09-04 01:51:46.000000 GitPython-3.1.8/git/config.py
--rw-r--r--   0 byron      (501) staff       (20)     1975 2020-07-06 07:36:41.000000 GitPython-3.1.8/git/db.py
--rw-r--r--   0 byron      (501) staff       (20)    19782 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/diff.py
--rw-r--r--   0 byron      (501) staff       (20)     4841 2020-04-11 05:38:55.000000 GitPython-3.1.8/git/exc.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.507797 GitPython-3.1.8/git/index/
--rw-r--r--   0 byron      (501) staff       (20)      129 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/index/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)    52258 2020-08-12 12:03:55.000000 GitPython-3.1.8/git/index/base.py
--rw-r--r--   0 byron      (501) staff       (20)    14226 2020-07-06 07:36:41.000000 GitPython-3.1.8/git/index/fun.py
--rw-r--r--   0 byron      (501) staff       (20)     4976 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/index/typ.py
--rw-r--r--   0 byron      (501) staff       (20)     2902 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/index/util.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.514666 GitPython-3.1.8/git/objects/
--rw-r--r--   0 byron      (501) staff       (20)      683 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/objects/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)     6689 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/objects/base.py
--rw-r--r--   0 byron      (501) staff       (20)      927 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/objects/blob.py
--rw-r--r--   0 byron      (501) staff       (20)    20722 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/objects/commit.py
--rw-r--r--   0 byron      (501) staff       (20)     7257 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/objects/fun.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.518025 GitPython-3.1.8/git/objects/submodule/
--rw-r--r--   0 byron      (501) staff       (20)       93 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/objects/submodule/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)    54288 2020-08-12 12:03:55.000000 GitPython-3.1.8/git/objects/submodule/base.py
--rw-r--r--   0 byron      (501) staff       (20)    17659 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/objects/submodule/root.py
--rw-r--r--   0 byron      (501) staff       (20)     2745 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/objects/submodule/util.py
--rw-r--r--   0 byron      (501) staff       (20)     3138 2020-02-23 23:31:24.000000 GitPython-3.1.8/git/objects/tag.py
--rw-r--r--   0 byron      (501) staff       (20)    10996 2020-07-06 07:36:41.000000 GitPython-3.1.8/git/objects/tree.py
--rw-r--r--   0 byron      (501) staff       (20)    12778 2020-09-01 02:48:38.000000 GitPython-3.1.8/git/objects/util.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.521974 GitPython-3.1.8/git/refs/
--rw-r--r--   0 byron      (501) staff       (20)      242 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/refs/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)     8706 2020-02-18 04:23:39.000000 GitPython-3.1.8/git/refs/head.py
--rw-r--r--   0 byron      (501) staff       (20)    10625 2020-04-11 05:38:55.000000 GitPython-3.1.8/git/refs/log.py
--rw-r--r--   0 byron      (501) staff       (20)     4408 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/refs/reference.py
--rw-r--r--   0 byron      (501) staff       (20)     1670 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/refs/remote.py
--rw-r--r--   0 byron      (501) staff       (20)    26966 2020-08-12 12:45:10.000000 GitPython-3.1.8/git/refs/symbolic.py
--rw-r--r--   0 byron      (501) staff       (20)     2964 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/refs/tag.py
--rw-r--r--   0 byron      (501) staff       (20)    36047 2020-08-12 12:03:55.000000 GitPython-3.1.8/git/remote.py
-drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-09-04 02:04:49.523767 GitPython-3.1.8/git/repo/
--rw-r--r--   0 byron      (501) staff       (20)      108 2020-01-31 04:46:36.000000 GitPython-3.1.8/git/repo/__init__.py
--rw-r--r--   0 byron      (501) staff       (20)    44495 2020-09-04 01:51:46.000000 GitPython-3.1.8/git/repo/base.py
--rw-r--r--   0 byron      (501) staff       (20)    11492 2020-07-06 07:36:41.000000 GitPython-3.1.8/git/repo/fun.py
--rw-r--r--   0 byron      (501) staff       (20)    31353 2020-08-12 12:03:55.000000 GitPython-3.1.8/git/util.py
--rw-r--r--   0 byron      (501) staff       (20)       16 2020-02-24 11:39:24.000000 GitPython-3.1.8/requirements.txt
--rw-r--r--   0 byron      (501) staff       (20)       38 2020-09-04 02:04:49.525138 GitPython-3.1.8/setup.cfg
--rwxr-xr-x   0 byron      (501) staff       (20)     4392 2020-07-13 02:09:59.000000 GitPython-3.1.8/setup.py
--rw-r--r--   0 byron      (501) staff       (20)       47 2020-08-12 12:03:55.000000 GitPython-3.1.8/test-requirements.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.463770 GitPython-3.1.9/
+-rw-r--r--   0 byron      (501) staff       (20)     1875 2020-09-01 02:48:38.000000 GitPython-3.1.9/AUTHORS
+-rw-r--r--   0 byron      (501) staff       (20)      147 2020-01-31 04:46:36.000000 GitPython-3.1.9/CHANGES
+-rw-r--r--   0 byron      (501) staff       (20)      443 2020-09-03 02:21:08.000000 GitPython-3.1.9/CONTRIBUTING.md
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.410354 GitPython-3.1.9/GitPython.egg-info/
+-rw-r--r--   0 byron      (501) staff       (20)     1086 2020-10-01 03:19:37.000000 GitPython-3.1.9/GitPython.egg-info/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)     1198 2020-10-01 03:19:37.000000 GitPython-3.1.9/GitPython.egg-info/SOURCES.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2020-10-01 03:19:37.000000 GitPython-3.1.9/GitPython.egg-info/dependency_links.txt
+-rw-r--r--   0 byron      (501) staff       (20)        1 2020-02-08 03:14:00.000000 GitPython-3.1.9/GitPython.egg-info/not-zip-safe
+-rw-r--r--   0 byron      (501) staff       (20)       16 2020-10-01 03:19:37.000000 GitPython-3.1.9/GitPython.egg-info/requires.txt
+-rw-r--r--   0 byron      (501) staff       (20)        4 2020-10-01 03:19:37.000000 GitPython-3.1.9/GitPython.egg-info/top_level.txt
+-rw-r--r--   0 byron      (501) staff       (20)     1521 2020-01-31 04:46:36.000000 GitPython-3.1.9/LICENSE
+-rw-r--r--   0 byron      (501) staff       (20)      215 2020-07-13 02:09:59.000000 GitPython-3.1.9/MANIFEST.in
+-rw-r--r--   0 byron      (501) staff       (20)     1086 2020-10-01 03:19:37.463068 GitPython-3.1.9/PKG-INFO
+-rw-r--r--   0 byron      (501) staff       (20)     8583 2020-09-07 01:22:35.000000 GitPython-3.1.9/README.md
+-rw-r--r--   0 byron      (501) staff       (20)        6 2020-10-01 03:18:02.000000 GitPython-3.1.9/VERSION
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.413344 GitPython-3.1.9/doc/
+-rw-r--r--   0 byron      (501) staff       (20)        7 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/.gitignore
+-rw-r--r--   0 byron      (501) staff       (20)     2347 2020-08-12 12:03:55.000000 GitPython-3.1.9/doc/Makefile
+-rw-r--r--   0 byron      (501) staff       (20)       28 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/requirements.txt
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.420497 GitPython-3.1.9/doc/source/
+-rw-r--r--   0 byron      (501) staff       (20)    36646 2020-10-01 03:17:57.000000 GitPython-3.1.9/doc/source/changes.rst
+-rw-r--r--   0 byron      (501) staff       (20)     6112 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/source/conf.py
+-rw-r--r--   0 byron      (501) staff       (20)      445 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/source/index.rst
+-rw-r--r--   0 byron      (501) staff       (20)     3923 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/source/intro.rst
+-rw-r--r--   0 byron      (501) staff       (20)     3319 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/source/reference.rst
+-rw-r--r--   0 byron      (501) staff       (20)      237 2020-05-04 09:48:58.000000 GitPython-3.1.9/doc/source/roadmap.rst
+-rw-r--r--   0 byron      (501) staff       (20)    24639 2020-07-13 06:21:22.000000 GitPython-3.1.9/doc/source/tutorial.rst
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.434082 GitPython-3.1.9/git/
+-rw-r--r--   0 byron      (501) staff       (20)     2399 2020-10-01 03:19:37.464396 GitPython-3.1.9/git/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)    42316 2020-07-06 07:36:41.000000 GitPython-3.1.9/git/cmd.py
+-rw-r--r--   0 byron      (501) staff       (20)     1928 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/compat.py
+-rw-r--r--   0 byron      (501) staff       (20)    30292 2020-09-04 01:51:46.000000 GitPython-3.1.9/git/config.py
+-rw-r--r--   0 byron      (501) staff       (20)     1975 2020-07-06 07:36:41.000000 GitPython-3.1.9/git/db.py
+-rw-r--r--   0 byron      (501) staff       (20)    19782 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/diff.py
+-rw-r--r--   0 byron      (501) staff       (20)     4841 2020-04-11 05:38:55.000000 GitPython-3.1.9/git/exc.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.441717 GitPython-3.1.9/git/index/
+-rw-r--r--   0 byron      (501) staff       (20)      129 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/index/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)    52258 2020-08-12 12:03:55.000000 GitPython-3.1.9/git/index/base.py
+-rw-r--r--   0 byron      (501) staff       (20)    14226 2020-07-06 07:36:41.000000 GitPython-3.1.9/git/index/fun.py
+-rw-r--r--   0 byron      (501) staff       (20)     4976 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/index/typ.py
+-rw-r--r--   0 byron      (501) staff       (20)     2902 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/index/util.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.450106 GitPython-3.1.9/git/objects/
+-rw-r--r--   0 byron      (501) staff       (20)      683 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/objects/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)     6689 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/objects/base.py
+-rw-r--r--   0 byron      (501) staff       (20)      927 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/objects/blob.py
+-rw-r--r--   0 byron      (501) staff       (20)    20722 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/objects/commit.py
+-rw-r--r--   0 byron      (501) staff       (20)     7257 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/objects/fun.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.454002 GitPython-3.1.9/git/objects/submodule/
+-rw-r--r--   0 byron      (501) staff       (20)       93 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/objects/submodule/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)    54288 2020-08-12 12:03:55.000000 GitPython-3.1.9/git/objects/submodule/base.py
+-rw-r--r--   0 byron      (501) staff       (20)    17659 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/objects/submodule/root.py
+-rw-r--r--   0 byron      (501) staff       (20)     2745 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/objects/submodule/util.py
+-rw-r--r--   0 byron      (501) staff       (20)     3138 2020-02-23 23:31:24.000000 GitPython-3.1.9/git/objects/tag.py
+-rw-r--r--   0 byron      (501) staff       (20)    10996 2020-07-06 07:36:41.000000 GitPython-3.1.9/git/objects/tree.py
+-rw-r--r--   0 byron      (501) staff       (20)    12778 2020-09-01 02:48:38.000000 GitPython-3.1.9/git/objects/util.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.458332 GitPython-3.1.9/git/refs/
+-rw-r--r--   0 byron      (501) staff       (20)      242 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/refs/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)     8706 2020-02-18 04:23:39.000000 GitPython-3.1.9/git/refs/head.py
+-rw-r--r--   0 byron      (501) staff       (20)    10625 2020-04-11 05:38:55.000000 GitPython-3.1.9/git/refs/log.py
+-rw-r--r--   0 byron      (501) staff       (20)     4408 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/refs/reference.py
+-rw-r--r--   0 byron      (501) staff       (20)     1670 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/refs/remote.py
+-rw-r--r--   0 byron      (501) staff       (20)    26966 2020-08-12 12:45:10.000000 GitPython-3.1.9/git/refs/symbolic.py
+-rw-r--r--   0 byron      (501) staff       (20)     2964 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/refs/tag.py
+-rw-r--r--   0 byron      (501) staff       (20)    36047 2020-08-12 12:03:55.000000 GitPython-3.1.9/git/remote.py
+drwxr-xr-x   0 byron      (501) staff       (20)        0 2020-10-01 03:19:37.461844 GitPython-3.1.9/git/repo/
+-rw-r--r--   0 byron      (501) staff       (20)      108 2020-01-31 04:46:36.000000 GitPython-3.1.9/git/repo/__init__.py
+-rw-r--r--   0 byron      (501) staff       (20)    44977 2020-10-01 03:16:50.000000 GitPython-3.1.9/git/repo/base.py
+-rw-r--r--   0 byron      (501) staff       (20)    11492 2020-07-06 07:36:41.000000 GitPython-3.1.9/git/repo/fun.py
+-rw-r--r--   0 byron      (501) staff       (20)    31353 2020-08-12 12:03:55.000000 GitPython-3.1.9/git/util.py
+-rw-r--r--   0 byron      (501) staff       (20)       16 2020-02-24 11:39:24.000000 GitPython-3.1.9/requirements.txt
+-rw-r--r--   0 byron      (501) staff       (20)       38 2020-10-01 03:19:37.463961 GitPython-3.1.9/setup.cfg
+-rwxr-xr-x   0 byron      (501) staff       (20)     4392 2020-07-13 02:09:59.000000 GitPython-3.1.9/setup.py
+-rw-r--r--   0 byron      (501) staff       (20)       47 2020-08-12 12:03:55.000000 GitPython-3.1.9/test-requirements.txt
```

### Comparing `GitPython-3.1.8/AUTHORS` & `GitPython-3.1.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/GitPython.egg-info/PKG-INFO` & `GitPython-3.1.9/GitPython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: GitPython
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python Git Library
 Home-page: https://github.com/gitpython-developers/GitPython
 Author: Sebastian Thiel, Michael Trier
 Author-email: byronimo@gmail.com, mtrier@gmail.com
 License: UNKNOWN
 Description: GitPython is a python library used to interact with Git repositories
 Platform: UNKNOWN
```

### Comparing `GitPython-3.1.8/GitPython.egg-info/SOURCES.txt` & `GitPython-3.1.9/GitPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/LICENSE` & `GitPython-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/PKG-INFO` & `GitPython-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: GitPython
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python Git Library
 Home-page: https://github.com/gitpython-developers/GitPython
 Author: Sebastian Thiel, Michael Trier
 Author-email: byronimo@gmail.com, mtrier@gmail.com
 License: UNKNOWN
 Description: GitPython is a python library used to interact with Git repositories
 Platform: UNKNOWN
```

### Comparing `GitPython-3.1.8/README.md` & `GitPython-3.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -138,26 +138,26 @@
 Please only use releases from `pypi` as you can verify the respective source
 tarballs.
 
 This script shows how to verify the tarball was indeed created by the authors of
 this project:
 
 ```
-curl https://pypi.python.org/packages/5b/38/0433c06feebbfbb51d644129dbe334031c33d55af0524326266f847ae907/GitPython-2.1.8-py2.py3-none-any.whl#md5=6b73ae86ee2dbab6da8652b2d875013a  > gitpython.whl
-curl https://pypi.python.org/packages/5b/38/0433c06feebbfbb51d644129dbe334031c33d55af0524326266f847ae907/GitPython-2.1.8-py2.py3-none-any.whl.asc > gitpython-signature.asc
+curl https://files.pythonhosted.org/packages/09/bc/ae32e07e89cc25b9e5c793d19a1e5454d30a8e37d95040991160f942519e/GitPython-3.1.8-py3-none-any.whl > gitpython.whl
+curl https://files.pythonhosted.org/packages/09/bc/ae32e07e89cc25b9e5c793d19a1e5454d30a8e37d95040991160f942519e/GitPython-3.1.8-py3-none-any.whl.asc >  gitpython-signature.asc
 gpg --verify gitpython-signature.asc gitpython.whl
 ```
 
 which outputs
 
 ```
-gpg: Signature made Mon Dec 11 17:34:17 2017 CET
-gpg:                using RSA key C3BC52BD76E2C23BAC6EC06A665F99FA9D99966C
-gpg:                issuer "byronimo@gmail.com"
-gpg: Good signature from "Sebastian Thiel (I do trust in Rust!) <byronimo@gmail.com>" [ultimate]
+gpg: Signature made Fr  4 Sep 10:04:50 2020 CST
+gpg:                using RSA key 27C50E7F590947D7273A741E85194C08421980C9
+gpg: Good signature from "Sebastian Thiel (YubiKey USB-C) <byronimo@gmail.com>" [ultimate]
+gpg:                 aka "Sebastian Thiel (In Rust I trust) <sebastian.thiel@icloud.com>" [ultimate]
 ```
 
 You can verify that the keyid indeed matches the release-signature key provided in this
 repository by looking at the keys details:
 
 ```
 gpg --list-packets ./release-verification-key.asc
@@ -169,15 +169,15 @@
 git show --show-signature  ./release-verification-key.asc
 ```
 
 If you would like to trust it permanently, you can import and sign it:
 
 ```
 gpg --import ./release-verification-key.asc
-gpg --edit-key 88710E60
+gpg --edit-key 4C08421980C9
 
 > sign
 > save
 ```
 
 ### Projects using GitPython
```

### Comparing `GitPython-3.1.8/doc/Makefile` & `GitPython-3.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/doc/source/changes.rst` & `GitPython-3.1.9/doc/source/changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+3.1.9
+=====
+
+See the following for details:
+https://github.com/gitpython-developers/gitpython/milestone/41?closed=1* 
+
+
 3.1.8
 =====
 
 * support for 'includeIf' in git configuration files
 * tests are now excluded from the package, making it conisderably smaller
```

### Comparing `GitPython-3.1.8/doc/source/conf.py` & `GitPython-3.1.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/doc/source/intro.rst` & `GitPython-3.1.9/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/doc/source/reference.rst` & `GitPython-3.1.9/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/doc/source/tutorial.rst` & `GitPython-3.1.9/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/__init__.py` & `GitPython-3.1.9/git/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import inspect
 import os
 import sys
 
 import os.path as osp
 
 
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 
 
 #{ Initialization
 def _init_externals():
     """Initialize external projects by putting them into the path"""
-    if __version__ == '3.1.8' and 'PYOXIDIZER' not in os.environ:
+    if __version__ == '3.1.9' and 'PYOXIDIZER' not in os.environ:
         sys.path.insert(0, osp.join(osp.dirname(__file__), 'ext', 'gitdb'))
 
     try:
         import gitdb
     except ImportError as e:
         raise ImportError("'gitdb' could not be found in your PYTHONPATH") from e
     # END verify import
```

### Comparing `GitPython-3.1.8/git/cmd.py` & `GitPython-3.1.9/git/cmd.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/compat.py` & `GitPython-3.1.9/git/compat.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/config.py` & `GitPython-3.1.9/git/config.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/db.py` & `GitPython-3.1.9/git/db.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/diff.py` & `GitPython-3.1.9/git/diff.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/exc.py` & `GitPython-3.1.9/git/exc.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/index/base.py` & `GitPython-3.1.9/git/index/base.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/index/fun.py` & `GitPython-3.1.9/git/index/fun.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/index/typ.py` & `GitPython-3.1.9/git/index/typ.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/index/util.py` & `GitPython-3.1.9/git/index/util.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/__init__.py` & `GitPython-3.1.9/git/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/base.py` & `GitPython-3.1.9/git/objects/base.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/blob.py` & `GitPython-3.1.9/git/objects/blob.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/commit.py` & `GitPython-3.1.9/git/objects/commit.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/fun.py` & `GitPython-3.1.9/git/objects/fun.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/submodule/base.py` & `GitPython-3.1.9/git/objects/submodule/base.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/submodule/root.py` & `GitPython-3.1.9/git/objects/submodule/root.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/submodule/util.py` & `GitPython-3.1.9/git/objects/submodule/util.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/tag.py` & `GitPython-3.1.9/git/objects/tag.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/tree.py` & `GitPython-3.1.9/git/objects/tree.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/objects/util.py` & `GitPython-3.1.9/git/objects/util.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/head.py` & `GitPython-3.1.9/git/refs/head.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/log.py` & `GitPython-3.1.9/git/refs/log.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/reference.py` & `GitPython-3.1.9/git/refs/reference.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/remote.py` & `GitPython-3.1.9/git/refs/remote.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/symbolic.py` & `GitPython-3.1.9/git/refs/symbolic.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/refs/tag.py` & `GitPython-3.1.9/git/refs/tag.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/remote.py` & `GitPython-3.1.9/git/remote.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/repo/base.py` & `GitPython-3.1.9/git/repo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,15 +635,15 @@
             return False
 
         # start from the one which is fastest to evaluate
         default_args = ['--abbrev=40', '--full-index', '--raw']
         if not submodules:
             default_args.append('--ignore-submodules')
         if path:
-            default_args.append(path)
+            default_args.extend(["--", path])
         if index:
             # diff index against HEAD
             if osp.isfile(self.index.path) and \
                     len(self.git.diff('--cached', *default_args)):
                 return True
         # END index handling
         if working_tree:
@@ -693,14 +693,27 @@
                 filename = filename[1:-1]
                 # WHATEVER ... it's a mess, but works for me
                 filename = filename.encode('ascii').decode('unicode_escape').encode('latin1').decode(defenc)
             untracked_files.append(filename)
         finalize_process(proc)
         return untracked_files
 
+    def ignored(self, *paths):
+        """Checks if paths are ignored via .gitignore
+        Doing so using the "git check-ignore" method.
+
+        :param paths: List of paths to check whether they are ignored or not
+        :return: subset of those paths which are ignored
+        """
+        try:
+            proc = self.git.check_ignore(*paths)
+        except GitCommandError:
+            return []
+        return proc.replace("\\\\", "\\").replace('"', "").split("\n")
+
     @property
     def active_branch(self):
         """The name of the currently active branch.
 
         :return: Head to the active branch"""
         return self.head.reference
```

### Comparing `GitPython-3.1.8/git/repo/fun.py` & `GitPython-3.1.9/git/repo/fun.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/git/util.py` & `GitPython-3.1.9/git/util.py`

 * *Files identical despite different names*

### Comparing `GitPython-3.1.8/setup.py` & `GitPython-3.1.9/setup.py`

 * *Files identical despite different names*

