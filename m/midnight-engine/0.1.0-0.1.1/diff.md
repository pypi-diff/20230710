# Comparing `tmp/midnight-engine-0.1.0.tar.gz` & `tmp/midnight-engine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midnight-engine-0.1.0.tar", last modified: Fri Jun 30 15:19:00 2023, max compression
+gzip compressed data, was "midnight-engine-0.1.1.tar", last modified: Mon Jul 10 12:52:37 2023, max compression
```

## Comparing `midnight-engine-0.1.0.tar` & `midnight-engine-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:19:00.733131 midnight-engine-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-06-30 10:39:09.000000 midnight-engine-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      562 2023-06-30 15:19:00.733131 midnight-engine-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-06-30 10:39:09.000000 midnight-engine-0.1.0/README.md
--rw-rw-rw-   0        0        0       97 2023-06-30 10:39:09.000000 midnight-engine-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      641 2023-06-30 15:19:00.735134 midnight-engine-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 15:19:00.705927 midnight-engine-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 15:19:00.712990 midnight-engine-0.1.0/src/midnight/
--rw-rw-rw-   0        0        0        0 2023-06-30 10:39:09.000000 midnight-engine-0.1.0/src/midnight/__init__.py
--rw-rw-rw-   0        0        0     1681 2023-06-30 15:14:20.000000 midnight-engine-0.1.0/src/midnight/midnight.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:19:00.732135 midnight-engine-0.1.0/src/midnight_engine.egg-info/
--rw-rw-rw-   0        0        0      562 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 15:19:00.000000 midnight-engine-0.1.0/src/midnight_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:37.897785 midnight-engine-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-10 12:52:37.897785 midnight-engine-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:37.893785 midnight-engine-0.1.1/midnight/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/midnight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/midnight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/midnight/midnight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:52:37.897785 midnight-engine-0.1.1/midnight_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 12:52:37.000000 midnight-engine-0.1.1/midnight_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 12:52:26.000000 midnight-engine-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 12:52:37.897785 midnight-engine-0.1.1/setup.cfg
```

### Comparing `midnight-engine-0.1.0/LICENSE` & `midnight-engine-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Retaki
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Retaki
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

