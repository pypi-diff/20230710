# Comparing `tmp/lc-checkpoint-0.4.1.1.tar.gz` & `tmp/lc-checkpoint-0.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.4.1.1.tar", last modified: Mon Jul 10 22:41:17 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.4.1.2.tar", last modified: Mon Jul 10 22:52:04 2023, max compression
```

## Comparing `lc-checkpoint-0.4.1.1.tar` & `lc-checkpoint-0.4.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.740987 lc-checkpoint-0.4.1.1/
--rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.4.1.1/LICENSE
--rw-rw-rw-   0        0        0     5464 2023-07-10 22:41:17.740987 lc-checkpoint-0.4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4958 2023-06-06 17:29:43.000000 lc-checkpoint-0.4.1.1/README.md
--rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.4.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      637 2023-07-10 22:41:17.750992 lc-checkpoint-0.4.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.705711 lc-checkpoint-0.4.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.724198 lc-checkpoint-0.4.1.1/src/lc_checkpoint/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint/main.py
-drwxrwxrwx   0        0        0        0 2023-07-10 22:41:17.739987 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0        0        0     5464 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 22:41:17.000000 lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 22:52:04.129821 lc-checkpoint-0.4.1.2/
+-rw-rw-rw-   0        0        0     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.4.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5464 2023-07-10 22:52:04.130825 lc-checkpoint-0.4.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4958 2023-06-06 17:29:43.000000 lc-checkpoint-0.4.1.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.4.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      637 2023-07-10 22:52:04.136348 lc-checkpoint-0.4.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 22:52:04.082930 lc-checkpoint-0.4.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 22:52:04.098240 lc-checkpoint-0.4.1.2/src/lc_checkpoint/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0        0        0     4542 2023-06-06 17:09:16.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint/main.py
+drwxrwxrwx   0        0        0        0 2023-07-10 22:52:04.128715 lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0        0        0     5464 2023-07-10 22:52:04.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-10 22:52:04.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 22:52:04.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 22:52:04.000000 lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.4.1.1/LICENSE` & `lc-checkpoint-0.4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.4.1.1/PKG-INFO` & `lc-checkpoint-0.4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.4.1.1
+Version: 0.4.1.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lc-checkpoint-0.4.1.1/README.md` & `lc-checkpoint-0.4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.4.1.1/setup.cfg` & `lc-checkpoint-0.4.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 632d 6368 6563 6b70 6f69 6e74   = lc-checkpoint
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 342e  ..version = 0.4.
-00000030: 312e 310d 0a61 7574 686f 7220 3d20 4465  1.1..author = De
+00000030: 312e 320d 0a61 7574 686f 7220 3d20 4465  1.2..author = De
 00000040: 6479 2056 616e 2048 6175 7465 6e0d 0a61  dy Van Hauten..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6465  uthor_email = de
 00000060: 6479 2e76 616e 4075 692e 6163 2e69 640d  dy.van@ui.ac.id.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2070 6163 6b61 6765 2066 6f72 2063 6f6d   package for com
 00000090: 7072 6573 7369 6e67 2050 7954 6f72 6368  pressing PyTorch
 000000a0: 206d 6f64 656c 2063 6865 636b 706f 696e   model checkpoin
```

### Comparing `lc-checkpoint-0.4.1.1/src/lc_checkpoint/main.py` & `lc-checkpoint-0.4.1.2/src/lc_checkpoint/main.py`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.4.1.1/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.4.1.2/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.4.1.1
+Version: 0.4.1.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

