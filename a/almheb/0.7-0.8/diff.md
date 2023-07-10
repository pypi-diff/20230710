# Comparing `tmp/almheb-0.7.tar.gz` & `tmp/almheb-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almheb-0.7.tar", last modified: Mon Jul 10 21:10:39 2023, max compression
+gzip compressed data, was "almheb-0.8.tar", last modified: Mon Jul 10 21:28:57 2023, max compression
```

## Comparing `almheb-0.7.tar` & `almheb-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 21:10:39.022234 almheb-0.7/
--rw-rw-rw-   0        0        0        0 2023-07-10 20:07:01.000000 almheb-0.7/LICENSE
--rw-rw-rw-   0        0        0      455 2023-07-10 21:10:39.022234 almheb-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2199 2023-07-10 21:09:29.000000 almheb-0.7/README.md
--rw-rw-rw-   0        0        0      103 2023-07-10 20:07:01.000000 almheb-0.7/pyproject.toml
--rw-rw-rw-   0        0        0      576 2023-07-10 21:10:39.023233 almheb-0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 21:10:39.010233 almheb-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 21:10:39.021233 almheb-0.7/src/almheb.egg-info/
--rw-rw-rw-   0        0        0      455 2023-07-10 21:10:38.000000 almheb-0.7/src/almheb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-10 21:10:39.000000 almheb-0.7/src/almheb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:10:38.000000 almheb-0.7/src/almheb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:10:38.000000 almheb-0.7/src/almheb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 21:28:57.734099 almheb-0.8/
+-rw-rw-rw-   0        0        0        0 2023-07-10 20:07:01.000000 almheb-0.8/LICENSE
+-rw-rw-rw-   0        0        0      455 2023-07-10 21:28:57.734099 almheb-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2199 2023-07-10 21:09:29.000000 almheb-0.8/README.md
+-rw-rw-rw-   0        0        0      103 2023-07-10 20:07:01.000000 almheb-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      576 2023-07-10 21:28:57.735098 almheb-0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 21:28:57.720097 almheb-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 21:28:57.733097 almheb-0.8/src/almheb.egg-info/
+-rw-rw-rw-   0        0        0      455 2023-07-10 21:28:57.000000 almheb-0.8/src/almheb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-10 21:28:57.000000 almheb-0.8/src/almheb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:28:57.000000 almheb-0.8/src/almheb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:28:57.000000 almheb-0.8/src/almheb.egg-info/top_level.txt
```

### Comparing `almheb-0.7/README.md` & `almheb-0.8/README.md`

 * *Files identical despite different names*

### Comparing `almheb-0.7/setup.cfg` & `almheb-0.8/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6c6d 6865 620d 0a76 6572 7369   = almheb..versi
-00000020: 6f6e 203d 2030 2e37 0d0a 6175 7468 6f72  on = 0.7..author
+00000020: 6f6e 203d 2030 2e38 0d0a 6175 7468 6f72  on = 0.8..author
 00000030: 203d 2041 6c6d 6865 620d 0a61 7574 686f   = Almheb..autho
 00000040: 725f 656d 6169 6c20 3d20 6170 7061 7371  r_email = appasq
 00000050: 7731 3037 4067 6d61 696c 2e63 6f6d 0d0a  w107@gmail.com..
 00000060: 6465 7363 7269 7074 696f 6e20 3d20 5079  description = Py
 00000070: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
 00000080: 2065 7874 7261 6374 696e 6720 496e 7374   extracting Inst
 00000090: 6167 7261 6d20 636f 6f6b 6965 7320 616e  agram cookies an
```

