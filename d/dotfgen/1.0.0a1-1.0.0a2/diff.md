# Comparing `tmp/dotfgen-1.0.0a1.tar.gz` & `tmp/dotfgen-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotfgen-1.0.0a1.tar", max compression
+gzip compressed data, was "dotfgen-1.0.0a2.tar", max compression
```

## Comparing `dotfgen-1.0.0a1.tar` & `dotfgen-1.0.0a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35053 2019-04-08 05:35:43.054790 dotfgen-1.0.0a1/LICENSE
-drwxr-xr-x   0        0        0        0 2023-07-08 10:21:10.628913 dotfgen-1.0.0a1/LICENSES/
--rw-r--r--   0        0        0      400 2023-07-08 12:39:54.327794 dotfgen-1.0.0a1/README.md
--rw-r--r--   0        0        0    22351 2023-07-09 20:33:45.577520 dotfgen-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-08 10:19:25.396224 dotfgen-1.0.0a1/src/dotfgen/__init__.py
--rw-r--r--   0        0        0      238 2023-07-08 17:54:52.376131 dotfgen-1.0.0a1/src/dotfgen/__main__.py
--rw-r--r--   0        0        0     3872 2023-07-08 18:15:04.734103 dotfgen-1.0.0a1/src/dotfgen/cli.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 dotfgen-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    35053 2023-07-10 08:39:00.913705 dotfgen-1.0.0a2/LICENSE
+drwxr-xr-x   0        0        0        0 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/LICENSES/
+-rw-r--r--   0        0        0      400 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/README.md
+-rw-r--r--   0        0        0    22351 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/src/dotfgen/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-10 08:39:00.915705 dotfgen-1.0.0a2/src/dotfgen/__main__.py
+-rw-r--r--   0        0        0     3872 2023-07-10 08:39:00.915705 dotfgen-1.0.0a2/src/dotfgen/cli.py
+-rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 dotfgen-1.0.0a2/PKG-INFO
```

### Comparing `dotfgen-1.0.0a1/LICENSE` & `dotfgen-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotfgen-1.0.0a1/pyproject.toml` & `dotfgen-1.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2019 Rémy Taymans <remytms@tsmail.eu>
 #
 # SPDX-License-Identifier: CC0-1.0
 
 [tool.poetry]
 name = "dotfgen"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "Generate dotfiles based on a template. dotfgen lets you anonymise your dotfiles."
 authors = ["Rémy Taymans <remytms@tsmail.eu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/remytms/dotfgen"
 keywords = ["dotfiles", "generator", "unix"]
 classifiers = [
```

### Comparing `dotfgen-1.0.0a1/src/dotfgen/cli.py` & `dotfgen-1.0.0a2/src/dotfgen/cli.py`

 * *Files identical despite different names*

### Comparing `dotfgen-1.0.0a1/PKG-INFO` & `dotfgen-1.0.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotfgen
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Generate dotfiles based on a template. dotfgen lets you anonymise your dotfiles.
 Home-page: https://gitlab.com/remytms/dotfgen
 License: GPL-3.0-or-later
 Keywords: dotfiles,generator,unix
 Author: Rémy Taymans
 Author-email: remytms@tsmail.eu
 Requires-Python: >=3.7,<4.0
```

