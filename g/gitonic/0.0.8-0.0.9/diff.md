# Comparing `tmp/gitonic-0.0.8.tar.gz` & `tmp/gitonic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitonic-0.0.8.tar", last modified: Tue Aug  2 06:54:50 2022, max compression
+gzip compressed data, was "gitonic-0.0.9.tar", last modified: Sat Oct  8 04:52:23 2022, max compression
```

## Comparing `gitonic-0.0.8.tar` & `gitonic-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-08-02 06:54:50.804938 gitonic-0.0.8/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1675 2022-07-30 06:59:49.000000 gitonic-0.0.8/BACKLOG.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1329 2022-08-02 06:53:12.000000 gitonic-0.0.8/CHANGELOG.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:43:45.000000 gitonic-0.0.8/LICENSE.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       77 2022-07-30 03:47:27.000000 gitonic-0.0.8/MANIFEST.in
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    41597 2022-08-02 06:54:50.804938 gitonic-0.0.8/PKG-INFO
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3695 2022-07-30 21:12:03.000000 gitonic-0.0.8/README.md
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-08-02 06:54:50.800938 gitonic-0.0.8/gitonic/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      147 2022-08-01 18:12:09.000000 gitonic-0.0.8/gitonic/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      155 2022-08-02 06:43:08.000000 gitonic-0.0.8/gitonic/__main__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       19 2022-08-02 06:53:25.000000 gitonic-0.0.8/gitonic/const.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    10329 2022-07-30 06:56:25.000000 gitonic-0.0.8/gitonic/file.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     5843 2022-08-01 19:16:10.000000 gitonic-0.0.8/gitonic/gitutil.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    33789 2022-08-01 17:03:19.000000 gitonic-0.0.8/gitonic/gui.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      172 2022-07-30 20:52:07.000000 gitonic-0.0.8/gitonic/icons.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2559 2022-08-01 18:12:09.000000 gitonic-0.0.8/gitonic/main.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1996 2021-11-07 11:28:33.000000 gitonic-0.0.8/gitonic/singleinstance.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      266 2021-11-06 18:39:18.000000 gitonic-0.0.8/gitonic/sysutil.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2121 2022-07-30 06:56:40.000000 gitonic-0.0.8/gitonic/task.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-08-02 06:54:50.804938 gitonic-0.0.8/gitonic/tile/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      462 2022-08-01 18:02:26.000000 gitonic-0.0.8/gitonic/tile/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    31760 2022-08-01 17:03:20.000000 gitonic-0.0.8/gitonic/tile/core.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1941 2022-07-30 06:56:05.000000 gitonic-0.0.8/gitonic/tile/tkcmd.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-08-02 06:54:50.804938 gitonic-0.0.8/gitonic.egg-info/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    41597 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/PKG-INFO
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      547 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/SOURCES.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/dependency_links.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       55 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/entry_points.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       45 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/requires.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        8 2022-08-02 06:54:50.000000 gitonic-0.0.8/gitonic.egg-info/top_level.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      123 2022-07-31 05:58:55.000000 gitonic-0.0.8/pyproject.toml
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      667 2022-08-02 06:54:50.804938 gitonic-0.0.8/setup.cfg
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      716 2022-07-31 05:19:20.000000 gitonic-0.0.8/setup.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-10-08 04:52:23.080022 gitonic-0.0.9/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1982 2022-08-16 09:15:16.000000 gitonic-0.0.9/BACKLOG.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1419 2022-10-08 04:50:42.000000 gitonic-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:43:45.000000 gitonic-0.0.9/LICENSE.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       77 2022-07-30 03:47:27.000000 gitonic-0.0.9/MANIFEST.in
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    43220 2022-10-08 04:52:23.080022 gitonic-0.0.9/PKG-INFO
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     4921 2022-09-17 07:46:40.000000 gitonic-0.0.9/README.md
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-10-08 04:52:23.076022 gitonic-0.0.9/gitonic/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      147 2022-08-01 18:12:09.000000 gitonic-0.0.9/gitonic/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      155 2022-08-02 06:43:08.000000 gitonic-0.0.9/gitonic/__main__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       19 2022-10-08 04:50:51.000000 gitonic-0.0.9/gitonic/const.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    10329 2022-07-30 06:56:25.000000 gitonic-0.0.9/gitonic/file.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     6826 2022-08-11 08:08:38.000000 gitonic-0.0.9/gitonic/gitutil.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    35559 2022-08-09 09:14:21.000000 gitonic-0.0.9/gitonic/gui.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      172 2022-08-02 07:44:36.000000 gitonic-0.0.9/gitonic/icons.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2559 2022-08-08 15:59:29.000000 gitonic-0.0.9/gitonic/main.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1996 2021-11-07 11:28:33.000000 gitonic-0.0.9/gitonic/singleinstance.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      447 2022-08-11 08:09:58.000000 gitonic-0.0.9/gitonic/sysutil.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2823 2022-08-08 16:58:42.000000 gitonic-0.0.9/gitonic/task.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-10-08 04:52:23.080022 gitonic-0.0.9/gitonic/tile/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      462 2022-08-01 18:02:26.000000 gitonic-0.0.9/gitonic/tile/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    32538 2022-08-08 16:05:19.000000 gitonic-0.0.9/gitonic/tile/core.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1941 2022-07-30 06:56:05.000000 gitonic-0.0.9/gitonic/tile/tkcmd.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2022-10-08 04:52:23.080022 gitonic-0.0.9/gitonic.egg-info/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    43220 2022-10-08 04:52:22.000000 gitonic-0.0.9/gitonic.egg-info/PKG-INFO
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      547 2022-10-08 04:52:23.000000 gitonic-0.0.9/gitonic.egg-info/SOURCES.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2022-10-08 04:52:22.000000 gitonic-0.0.9/gitonic.egg-info/dependency_links.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       55 2022-10-08 04:52:22.000000 gitonic-0.0.9/gitonic.egg-info/entry_points.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       44 2022-10-08 04:52:22.000000 gitonic-0.0.9/gitonic.egg-info/requires.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        8 2022-10-08 04:52:22.000000 gitonic-0.0.9/gitonic.egg-info/top_level.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      130 2022-08-07 15:00:47.000000 gitonic-0.0.9/pyproject.toml
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      667 2022-10-08 04:52:23.080022 gitonic-0.0.9/setup.cfg
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      716 2022-08-09 09:16:32.000000 gitonic-0.0.9/setup.py
```

### Comparing `gitonic-0.0.8/BACKLOG.md` & `gitonic-0.0.9/BACKLOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 - revert changes / git checkout support
 - git branch support
   - create
   - switch
 - git tag support
 - git stash support (list, show, push, pop/apply, drop, clear)
 - merge tool integration
+- diff-tool blocks main screen
 - settings tabs
   - check for installed git
   - ~~git exe configuration in settings~~
   - check for latest version of gitonic
   - 
 - ~~config file for last known config~~
 - gui rework
   - theme support
   - resize behavior -> expand
-  - icons
-  - 
+  - ~~icons~~
+  - grid layout / less floating 
+  -
 - background task and event loop -> freezing gui when running git utils
   - use TkCmd also for Cmd runners
   - status bar with running background tasks overview?
   -
 - refact for integration in other tools
 - filter git on 'changes' tab
 - rework logging
@@ -34,15 +36,16 @@
   - black PEP8 support
   - desktop integration
     - open shell at repo path
     - open file management too at repo path
 - ~~history of commit texts~~
   - ~~in combo box~~
   - git log / show integration?
-
+- git error handling
+- 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
 
 # LIMITATIONS
@@ -53,10 +56,13 @@
  commited changes (same behavior as cmd-line `git difftool`)
 - git credentials basic support, 
  you need to use https://git-scm.com/docs/git-credential-store.
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
-- 
+- `gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
```

### Comparing `gitonic-0.0.8/CHANGELOG.md` & `gitonic-0.0.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 # Changelog
 
 
+# version v0.0.9 - 20221008
+
+- git current branch in changes tab
+- support for black
+- 
+
+
 # version v0.0.8 - 20220802
 
 - bug fix, due to corrupted local env
 - double click in changes view will stage/ unstage a file
 -
```

### Comparing `gitonic-0.0.8/LICENSE.md` & `gitonic-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/PKG-INFO` & `gitonic-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitonic
-Version: 0.0.8
+Version: 0.0.9
 Summary: manage a multi git workspace
 Home-page: https://github.com/kr-g/gitonic
 Author: k. goger
 Author-email: k.r.goger+gitonic@gmail.com
 License: AGPLv3+
 Keywords: python utility shell git git-workspace tkinter
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,14 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Publish Python 🐍 distributions 📦 to PyPI](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml)
-
 # gitonic 
 
 gitonic simplifies working with multiple git repositories.
 
 gitonic comes with an easy to use Tkinter GUI.
 
 there is also a plugin for thonny 
@@ -43,14 +41,20 @@
 
 # limitations
 
 Check 
 [`BACKLOG`](https://github.com/kr-g/gitonic/blob/main/BACKLOG.md)
 for open development tasks and limitations.
 
+IMPORTANT:
+
+`gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
 
 # recommended readings prior using gitonic
 
 an introduction on how git works in general can be found in the official git documentation in section
 [`Git-Basics`](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository).
 
 
@@ -77,14 +81,15 @@
 | F1 | refresh all in changed files view |
 | F2 | select all in changed files view |
 | F3 | un-select all in changed files view |
 | Alt-a | stage file(s) in git |
 | Alt-q | un-stage file(s) in git |
 | Alt-w | diff file(s) |
 | Alt-d | difftool file(s) |
+| Alt-f | auto format file(s) with `black` PEP08 |
 | Alt-x | commit file(s) |
 | Alt-s | push git(s) |
 | Alt-e | commit and push git(s), like pressing Alt-x and Alt-s |
 
 HINT:
 
 if not responding to a hotkey, make sure that CapsLock is disabled
@@ -122,23 +127,41 @@
     phyton3 -m pip install gitonic
 
 to use git difftool, and mergetool install a 3rd party tool like 
 [`meld merge`](https://meldmerge.org/)
 and configure like described below
 
 
+## installation on raspberry pi, or fedora
+
+when during startup an error is thrown, such as:
+
+    from PIL import Image, ImageTk, ImageDraw, ImageFont
+    ImportError: cannot import name 'ImageTk' from 'PIL' (/usr/lib64/python3.10/site-packages/PIL/__init__.py)
+
+here it is required to install imagetk in addtion 
+
+    # debian ubuntu etc
+    sudo apt-get install python3-pil python3-pil.imagetk
+
+    # fedora
+    sudo yum install python3-pillow python3-pillow-tk
+
+
 # git configuration
 
 add a `.git-credentials` file as described here 
 [`git-credentials`](https://git-scm.com/docs/git-credential-store#_storage_format)
 
 
 add a `.gitconfig` file as described here
 [`git-config`](https://git-scm.com/docs/git-config)
-and configure for diff and merge tools
+and configure for diff and merge tools. 
+NOTE: you need to install the diff-tool e.g. [`meld merge`](https://meldmerge.org/) manually, 
+if meld is not installed pressing the button will have no effect.
 
 
     [user]
         name = your name
         email = you@email.tld
         
     [credential]
@@ -164,24 +187,51 @@
 the following tools are part of the standard git distribution 
 
 - [`gitk`](https://git-scm.com/docs/gitk)
 git history browser
 - [`git-gui`](https://git-scm.com/docs/git-gui/)
 a git front end
 
+other gui-clients are listed on [`git-scm`](https://git-scm.com/downloads/guis)
+
+
+# internals
+
+following files are used:
+
+|file|description|
+|---|---|
+|~/.gitonic/commit.json|the last commit messages show in the combo box|
+|~/.gitonic/tracked.json|tracked git repositories|
+|~/.gitonic/config.json|configuration settings|
+|~/.gitonic/socket|internal use|
+
+
+HINT:
+crash after configuration change can be resolved by changing the setting manually in `config.json`, or delete the config file to fall back to the defaults
+
 
 # license
 
 gitonic is released under the following
 [`LICENSE`](https://github.com/kr-g/gitonic/blob/main/LICENSE.md)
 
 
+
+
 # Changelog
 
 
+# version v0.0.9 - 20221008
+
+- git current branch in changes tab
+- support for black
+- 
+
+
 # version v0.0.8 - 20220802
 
 - bug fix, due to corrupted local env
 - double click in changes view will stage/ unstage a file
 - 
 
 
@@ -255,25 +305,27 @@
 - revert changes / git checkout support
 - git branch support
   - create
   - switch
 - git tag support
 - git stash support (list, show, push, pop/apply, drop, clear)
 - merge tool integration
+- diff-tool blocks main screen
 - settings tabs
   - check for installed git
   - ~~git exe configuration in settings~~
   - check for latest version of gitonic
   - 
 - ~~config file for last known config~~
 - gui rework
   - theme support
   - resize behavior -> expand
-  - icons
-  - 
+  - ~~icons~~
+  - grid layout / less floating 
+  -
 - background task and event loop -> freezing gui when running git utils
   - use TkCmd also for Cmd runners
   - status bar with running background tasks overview?
   -
 - refact for integration in other tools
 - filter git on 'changes' tab
 - rework logging
@@ -283,15 +335,16 @@
   - black PEP8 support
   - desktop integration
     - open shell at repo path
     - open file management too at repo path
 - ~~history of commit texts~~
   - ~~in combo box~~
   - git log / show integration?
-
+- git error handling
+- 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
 
 # LIMITATIONS
@@ -302,15 +355,18 @@
  commited changes (same behavior as cmd-line `git difftool`)
 - git credentials basic support, 
  you need to use https://git-scm.com/docs/git-credential-store.
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
-- 
+- `gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
  
 
 
 ---
 
 Copyright (c) 2022 k. goger - https://github.com/kr-g
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gitonic-0.0.8/README.md` & `gitonic-0.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Publish Python 🐍 distributions 📦 to PyPI](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml)
-
 # gitonic 
 
 gitonic simplifies working with multiple git repositories.
 
 gitonic comes with an easy to use Tkinter GUI.
 
 there is also a plugin for thonny 
@@ -21,14 +19,20 @@
 
 # limitations
 
 Check 
 [`BACKLOG`](https://github.com/kr-g/gitonic/blob/main/BACKLOG.md)
 for open development tasks and limitations.
 
+IMPORTANT:
+
+`gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
 
 # recommended readings prior using gitonic
 
 an introduction on how git works in general can be found in the official git documentation in section
 [`Git-Basics`](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository).
 
 
@@ -55,14 +59,15 @@
 | F1 | refresh all in changed files view |
 | F2 | select all in changed files view |
 | F3 | un-select all in changed files view |
 | Alt-a | stage file(s) in git |
 | Alt-q | un-stage file(s) in git |
 | Alt-w | diff file(s) |
 | Alt-d | difftool file(s) |
+| Alt-f | auto format file(s) with `black` PEP08 |
 | Alt-x | commit file(s) |
 | Alt-s | push git(s) |
 | Alt-e | commit and push git(s), like pressing Alt-x and Alt-s |
 
 HINT:
 
 if not responding to a hotkey, make sure that CapsLock is disabled
@@ -100,23 +105,41 @@
     phyton3 -m pip install gitonic
 
 to use git difftool, and mergetool install a 3rd party tool like 
 [`meld merge`](https://meldmerge.org/)
 and configure like described below
 
 
+## installation on raspberry pi, or fedora
+
+when during startup an error is thrown, such as:
+
+    from PIL import Image, ImageTk, ImageDraw, ImageFont
+    ImportError: cannot import name 'ImageTk' from 'PIL' (/usr/lib64/python3.10/site-packages/PIL/__init__.py)
+
+here it is required to install imagetk in addtion 
+
+    # debian ubuntu etc
+    sudo apt-get install python3-pil python3-pil.imagetk
+
+    # fedora
+    sudo yum install python3-pillow python3-pillow-tk
+
+
 # git configuration
 
 add a `.git-credentials` file as described here 
 [`git-credentials`](https://git-scm.com/docs/git-credential-store#_storage_format)
 
 
 add a `.gitconfig` file as described here
 [`git-config`](https://git-scm.com/docs/git-config)
-and configure for diff and merge tools
+and configure for diff and merge tools. 
+NOTE: you need to install the diff-tool e.g. [`meld merge`](https://meldmerge.org/) manually, 
+if meld is not installed pressing the button will have no effect.
 
 
     [user]
         name = your name
         email = you@email.tld
         
     [credential]
@@ -142,12 +165,32 @@
 the following tools are part of the standard git distribution 
 
 - [`gitk`](https://git-scm.com/docs/gitk)
 git history browser
 - [`git-gui`](https://git-scm.com/docs/git-gui/)
 a git front end
 
+other gui-clients are listed on [`git-scm`](https://git-scm.com/downloads/guis)
+
+
+# internals
+
+following files are used:
+
+|file|description|
+|---|---|
+|~/.gitonic/commit.json|the last commit messages show in the combo box|
+|~/.gitonic/tracked.json|tracked git repositories|
+|~/.gitonic/config.json|configuration settings|
+|~/.gitonic/socket|internal use|
+
+
+HINT:
+crash after configuration change can be resolved by changing the setting manually in `config.json`, or delete the config file to fall back to the defaults
+
 
 # license
 
 gitonic is released under the following
 [`LICENSE`](https://github.com/kr-g/gitonic/blob/main/LICENSE.md)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gitonic-0.0.8/gitonic/file.py` & `gitonic-0.0.9/gitonic/file.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/gitonic/gitutil.py` & `gitonic-0.0.9/gitonic/gitutil.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 
 import os
 import glob
 
 from .file import FileStat, PushDir
 from .task import Cmd, CmdTask
+from .sysutil import platform_windows
 
-GIT = "git"
+GIT = "git.exe" if platform_windows() else "git"
 BLACK = "black"
 
 
 join_wait = True
 
 
 def set_wait_mode(mode=True):
@@ -101,27 +102,51 @@
 
 git_checkout = lambda repo, files, callb=None: with_git_cmd(
     repo, f"checkout {join_files(files)}", callb=callb
 )
 git_checkout_ref = lambda repo, ref, callb=None: git_checkout(repo, [ref], callb=callb)
 
 git_tags = lambda repo, callb=None: with_git_cmd(repo, "tag", callb=callb)
-git_branches = lambda repo, callb=None: with_git_cmd(repo, "branch --all", callb=callb)
+
+git_branch = lambda repo, callb=None: with_git_cmd(repo, "branch", callb=callb)
+git_branch_all = lambda repo, callb=None: with_git_cmd(
+    repo, "branch --all", callb=callb
+)
 git_curbranch = lambda repo, callb=None: with_git_cmd(
     repo, "branch --show-current", callb=callb
 )
 
 git_make_tag = lambda repo, tag, callb=None: with_git_cmd(
     repo, f"tag {tag}", callb=callb
 )
 git_make_branch = lambda repo, branch, callb=None: with_git_cmd(
     repo, f"branch {branch}", callb=callb
 )
 
 
+class GitBranch(object):
+    def __init__(self, current=None, bnam=None):
+        self.set(current, bnam)
+
+    def set(self, current, bnam):
+        self.current = current
+        self.bnam = bnam
+
+        return self
+
+    def from_str(self, s):
+        current = s[0] == "*"
+        bnam = s[2:].strip()
+        self.set(current, bnam)
+        return self
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{ self.current }', '{ str(self.bnam) }' )"
+
+
 class GitStatus(object):
     def __init__(self, mode=None, staged=None, file=None):
         self.set(mode, staged, file)
 
     def set(self, mode, staged, file):
         self.mode = mode.upper() if mode else ""
         self.staged = staged.upper() if staged else ""
@@ -165,24 +190,37 @@
         return f"{self.__class__.__name__}('{ self.file }', '{ str(self.mode) }', '{ str(self.staged) }' )"
 
 
 class GitRepo(object):
     def __init__(self, repo):
         self.path = FileStat(repo).name
         self.status = []
+        self.branch = []
+        self.current_branch = None
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{ self.path }')"
 
     def refresh_status(self):
+
         file_status = git_stat(self.path)
         self.status.clear()
         for stat in file_status:
             gfs = GitStatus().from_str(stat)
             self.status.append(gfs)
+
+        self.current_branch = None
+        branches = git_branch(self.path)
+        self.branch.clear()
+        for branch in branches:
+            gb = GitBranch().from_str(branch)
+            self.branch.append(gb)
+            if gb.current:
+                self.current_branch = gb
+
         return self
 
     def stat(self, status):
         fs = FileStat(self.path).join([status.file])
         fs.stat()
         return fs
```

### Comparing `gitonic-0.0.8/gitonic/gui.py` & `gitonic-0.0.9/gitonic/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 from .file import FileStat
 from .sysutil import open_file_explorer
 
 from .gitutil import set_git_exe, GIT, GitWorkspace, git_diff, git_difftool
 from .gitutil import run_black, git_add, git_add_undo, git_commit
 from .gitutil import git_pull, git_push, git_push_tags, git_push_all
 
+from .gitutil import with_cmd
+from .task import run_proc
+
 
 # global
 
 url_homepage = "https://github.com/kr-g/gitonic"
 url_sponsor = "https://github.com/sponsors/kr-g"
 
 # configuration
@@ -52,14 +55,15 @@
 ICO_CLR = "xmark"
 ICO_PULL = "angle-down"
 ICO_PULL_ALL = "angles-down"
 ICO_FILE_ADD = "file-circle-plus"
 ICO_FILE_SUB = "file-circle-minus"
 ICO_FILE_DIFF = "file-waveform"
 ICO_FILE_DIFFTOOL = "code-compare"
+ICO_FILE_FORMATSOURCE = "indent"
 
 #
 
 
 def dgb_pr(*s):
     # print(*s)
     if dev_mode:
@@ -323,20 +327,21 @@
                             source=[
                                 TileLabel(caption=""),
                                 TileTreeView(
                                     caption="",
                                     idn="changes",
                                     header=[
                                         ("git", None),
+                                        ("branch", None),
                                         ("file", None),
                                         ("unstaged", None),
                                         ("staged", None),
                                         ("type", None),
                                     ],
-                                    header_width=(150, 250, 100, 100, 100),
+                                    header_width=(150, 100, 250, 100, 100, 100),
                                     height=13,
                                     on_double_click=lambda x: on_add_or_undo(x),
                                 ),
                                 TileCols(
                                     source=[
                                         TileLabelButton(
                                             caption="changes",
@@ -390,14 +395,23 @@
                                             caption="",
                                             commandtext="diff",
                                             icon=get_icon(ICO_FILE_DIFF),
                                             command=lambda: on_diff(),
                                             hotkey="<Alt-Key-w>",
                                         ),
                                         TileLabelButton(
+                                            idn="black",
+                                            caption="",
+                                            commandtext="autoformat source",
+                                            icon=get_icon(ICO_FILE_FORMATSOURCE),
+                                            command=lambda: on_black(),
+                                            hotkey="<Alt-Key-f>",
+                                        ),
+                                        TileLabelButton(
+                                            idn="difftool",
                                             caption="",
                                             commandtext="difftool",
                                             icon=get_icon(ICO_FILE_DIFFTOOL),
                                             command=lambda: on_difftool(),
                                             hotkey="<Alt-Key-d>",
                                         ),
                                     ]
@@ -605,14 +619,55 @@
     on_cmd_diff("on_diff", git_diff)
 
 
 def on_difftool():
     on_cmd_diff("on_difftool", git_difftool, True)
 
 
+def strip_non_ascii(s):
+    import string
+
+    rc = ""
+    for c in s:
+        if c in string.printable:
+            rc += c
+    return rc
+
+
+def on_black():
+    dgb_pr("on_black")
+    sel = gt("changes").get_selection_values()
+
+    s = []
+
+    def adder(st):
+        # todo tkinter cant handle all utf-8 chars
+        s.append(strip_non_ascii(st))
+
+    for rec in sel:
+        repo = FileStat(gws.base_repo_dir.name).join([rec["git"]]).name
+        fnam = rec["file"]
+        p = FileStat(repo).join([fnam])
+
+        if p.splitext()[1] not in [".py"]:
+            s.append("---skipping non python file---")
+            s.append(p.name)
+            continue
+
+        p = p.name
+
+        # todo tkinter cant handle all utf-8 chars
+        s.append("---checking---")
+        s.append(p)
+        rc = run_proc(["black", p], callb=adder)
+
+    do_log_time("running black", ignore_switch=False)
+    do_logs(s)
+
+
 def on_log_clr():
     gt("log").clr()
     dgb_pr("on_log_clr")
 
 
 def do_log_max_history():
     dgb_pr("do_log_max_history")
@@ -939,14 +994,15 @@
 
         if len(git.status) > 0:
             for stat in git.status:
                 fs = git.stat(stat)
                 fs_ex = fs.exists()
                 gst = {
                     "git": gitnam,
+                    "branch": git.current_branch.bnam,
                     "file": stat.file,
                     "unstaged": stat.mode,
                     "staged": stat.staged,
                     "type": ("file" if fs.is_file() else "dir")
                     if fs_ex
                     else "---deleted---",
                 }
@@ -955,14 +1011,17 @@
 
 
 def startup_gui():
     # read_config()
     read_commit()
     set_workspace(True)
 
+    #     gt("difftool").set_enabled(False)
+    #     gt("black").set_enabled(False)
+
     gt("follow").set_val(follow)
     gt("auto_switch").set_val(auto_switch)
     gt("push_tags").set_val(push_tags)
     gt("show_changes").set_val(show_changes)
     gt("dev_mode").set_val(dev_mode)
     if dev_mode:
         gt("dev_follow").set_val(dev_follow)
```

### Comparing `gitonic-0.0.8/gitonic/main.py` & `gitonic-0.0.9/gitonic/main.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/gitonic/singleinstance.py` & `gitonic-0.0.9/gitonic/singleinstance.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/gitonic/task.py` & `gitonic-0.0.9/gitonic/task.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,74 @@
 
 import os
 import subprocess
 import threading
 from queue import Queue
 
 
+def run_proc(
+    cmd,
+    stdin=None,
+    readline=True,
+    read_blk=5,
+    decode=True,
+    combine_stderr=True,
+    callb=None,
+    loopcallb=None,
+    shell=False,
+    env=-1,
+):
+
+    try:
+        rc = None
+        proc = subprocess.Popen(
+            cmd,
+            stdin=stdin,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT if combine_stderr else None,
+            shell=shell,
+            # todo
+            env=os.environ if env == -1 else env,
+        )
+
+        if proc:
+            while True:
+
+                if loopcallb:
+                    if loopcallb(proc):
+                        break
+
+                recv = None
+
+                if readline:
+                    recv = proc.stdout.readline()
+                else:
+                    recv = proc.stdout.read(read_blk)
+                if len(recv) == 0:
+                    break
+                if decode:
+                    recv = recv.decode()
+                if callb:
+                    callb(recv)
+
+            proc.wait()
+
+            if proc.returncode == 0:
+                return
+            return proc.returncode
+
+        else:
+            rc = 1
+
+    except Exception as ex:
+        rc = ex
+
+    return rc
+
+
 class Task(threading.Thread):
     def start(self):
         self.qu = Queue()
         self.rc = None
         self._stop_req = None
         super().start()
 
@@ -52,35 +112,20 @@
     def set_callb(self, callb=None):
         self._callb = callb
         return self
 
     def start(self):
         pass
 
+    def _loopcb(self, p):
+        if self._stop_req:
+            return self._stop_req
+
     def run(self):
-        try:
-            rc = 0
-            proc = subprocess.Popen(
-                self._cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True
-            )
-            # with os.popen(self._cmd) as f:
-            while True:
-                if self._stop_req:
-                    return self._stop_req
-                # line = f.readline()
-                line = proc.stdout.readline().decode()
-                if len(line) == 0:
-                    break
-                line = line.rstrip()
-                if self._callb:
-                    self._callb(line)
-            if proc.returncode:
-                rc = proc.returncode
-        except Exception as ex:
-            rc = ex
+        rc = run_proc(self._cmd, callb=self._callb, loopcallb=self._loopcb, shell=True)
         return rc
 
 
 class CmdTask(Cmd, Task):
     def start(self):
         if self._callb is None:
             self.set_callb(self._append_rc)
```

### Comparing `gitonic-0.0.8/gitonic/tile/core.py` & `gitonic-0.0.9/gitonic/tile/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,37 +104,44 @@
 
 
 def gt(name):
     return _global_reg.get(name, None)
 
 
 class Tile(TkMixin):
-    def __init__(self, parent=None, idn=None, tk_root=None, **kwargs):
+    def __init__(self, *a, **kw):
+        self.__init__tile__(*a, **kw)
 
+    def __init__tile__(self, parent=None, idn=None, tk_root=None, **kwargs):
+
+        self._kwargs = kwargs
         self.init(tk_root)
+        self.set_parent(parent)
+        self._set_idn(idn)
 
-        self.idn = idn
-        if idn != None:
-            if gt(idn) != None:
-                print_t("already defined", idn)
-            _global_reg[idn] = self
+        self.__init__core__()
+        self.__init__internal__()
 
-        self._kwargs = kwargs
+    def __init__core__(self):
 
         self.frame = None
         self._elems = []
         self._frame = []
 
         self._visible = self.pref("visible", True)
-
-        self.set_parent(parent)
+        self._enabled = self.pref("enabled", True)
 
         self._container = None
 
-        self.__init__internal__()
+    def _set_idn(self, idn):
+        self.idn = idn
+        if idn != None:
+            if gt(idn) != None:
+                print_t("already defined", idn)
+            _global_reg[idn] = self
 
     def __repr__(self):
         return self.__class__.__name__ + " " + (self.idn if self.idn else hex(id(self)))
 
     def __init__internal__(self):
         pass
 
@@ -198,14 +205,16 @@
             self._init_frame()
 
             self._build()
 
             self._pack_elems()
             self._pack_frame()
 
+            self._render_state()
+
         return self
 
     def _build(self):
         el = self.create_element()
         self._add_frames(el)
 
         for el in self._elems:
@@ -260,14 +269,32 @@
         return opts
 
     #
 
     def focus(self):
         if self.frame:
             self.frame.focus_set()
+        return self
+
+    #
+
+    def set_visible(self, en=True):
+        self._visible = en
+        self.layout()
+
+    def set_enabled(self, en=True):
+        self._enabled = en
+        self._render_state()
+        return self
+
+    def _render_state(self):
+        pass
+
+    def _set_state(self, w):
+        w["state"] = "normal" if self._enabled else "disabled"
 
     #
 
     def pref(self, name, defval=None):
         v = self._kwargs.setdefault(name, defval)
         return v
 
@@ -349,14 +376,17 @@
         if hotkey:
             _add_hotkey(hotkey)
             root = self.get_root()
             root.bind(hotkey, lambda x: command())
 
         return self._button
 
+    def _render_state(self):
+        self._set_state(self._button)
+
 
 class TileCheckbutton(Tile):
     def create_element(self):
         self._var = StringVar()
         self.set_val(self.pref(VALUE, False))
 
         self._var_str = StringVar()
@@ -394,14 +424,17 @@
     def create_element(
         self,
     ):
         TileLabel.create_element(self)
         TileButton.create_element(self)
         return [self._lbl, self._button]
 
+    def _render_state(self):
+        TileButton._render_state(self)
+
 
 class TileEntry(Tile):
     def create_element(self):
         width = self.pref_int(CAPTION_WIDTH, none_ok=True)
         self._lbl = ttk.Label(self.frame, text=self.get_caption(), width=width)
         self._var = self._create_var()
         self._entry = self._create_entry()
```

### Comparing `gitonic-0.0.8/gitonic/tile/tkcmd.py` & `gitonic-0.0.9/gitonic/tile/tkcmd.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/gitonic.egg-info/PKG-INFO` & `gitonic-0.0.9/gitonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitonic
-Version: 0.0.8
+Version: 0.0.9
 Summary: manage a multi git workspace
 Home-page: https://github.com/kr-g/gitonic
 Author: k. goger
 Author-email: k.r.goger+gitonic@gmail.com
 License: AGPLv3+
 Keywords: python utility shell git git-workspace tkinter
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,14 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-[![Publish Python 🐍 distributions 📦 to PyPI](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/kr-g/gitonic/actions/workflows/publish-to-pypi.yml)
-
 # gitonic 
 
 gitonic simplifies working with multiple git repositories.
 
 gitonic comes with an easy to use Tkinter GUI.
 
 there is also a plugin for thonny 
@@ -43,14 +41,20 @@
 
 # limitations
 
 Check 
 [`BACKLOG`](https://github.com/kr-g/gitonic/blob/main/BACKLOG.md)
 for open development tasks and limitations.
 
+IMPORTANT:
+
+`gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
 
 # recommended readings prior using gitonic
 
 an introduction on how git works in general can be found in the official git documentation in section
 [`Git-Basics`](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository).
 
 
@@ -77,14 +81,15 @@
 | F1 | refresh all in changed files view |
 | F2 | select all in changed files view |
 | F3 | un-select all in changed files view |
 | Alt-a | stage file(s) in git |
 | Alt-q | un-stage file(s) in git |
 | Alt-w | diff file(s) |
 | Alt-d | difftool file(s) |
+| Alt-f | auto format file(s) with `black` PEP08 |
 | Alt-x | commit file(s) |
 | Alt-s | push git(s) |
 | Alt-e | commit and push git(s), like pressing Alt-x and Alt-s |
 
 HINT:
 
 if not responding to a hotkey, make sure that CapsLock is disabled
@@ -122,23 +127,41 @@
     phyton3 -m pip install gitonic
 
 to use git difftool, and mergetool install a 3rd party tool like 
 [`meld merge`](https://meldmerge.org/)
 and configure like described below
 
 
+## installation on raspberry pi, or fedora
+
+when during startup an error is thrown, such as:
+
+    from PIL import Image, ImageTk, ImageDraw, ImageFont
+    ImportError: cannot import name 'ImageTk' from 'PIL' (/usr/lib64/python3.10/site-packages/PIL/__init__.py)
+
+here it is required to install imagetk in addtion 
+
+    # debian ubuntu etc
+    sudo apt-get install python3-pil python3-pil.imagetk
+
+    # fedora
+    sudo yum install python3-pillow python3-pillow-tk
+
+
 # git configuration
 
 add a `.git-credentials` file as described here 
 [`git-credentials`](https://git-scm.com/docs/git-credential-store#_storage_format)
 
 
 add a `.gitconfig` file as described here
 [`git-config`](https://git-scm.com/docs/git-config)
-and configure for diff and merge tools
+and configure for diff and merge tools. 
+NOTE: you need to install the diff-tool e.g. [`meld merge`](https://meldmerge.org/) manually, 
+if meld is not installed pressing the button will have no effect.
 
 
     [user]
         name = your name
         email = you@email.tld
         
     [credential]
@@ -164,24 +187,51 @@
 the following tools are part of the standard git distribution 
 
 - [`gitk`](https://git-scm.com/docs/gitk)
 git history browser
 - [`git-gui`](https://git-scm.com/docs/git-gui/)
 a git front end
 
+other gui-clients are listed on [`git-scm`](https://git-scm.com/downloads/guis)
+
+
+# internals
+
+following files are used:
+
+|file|description|
+|---|---|
+|~/.gitonic/commit.json|the last commit messages show in the combo box|
+|~/.gitonic/tracked.json|tracked git repositories|
+|~/.gitonic/config.json|configuration settings|
+|~/.gitonic/socket|internal use|
+
+
+HINT:
+crash after configuration change can be resolved by changing the setting manually in `config.json`, or delete the config file to fall back to the defaults
+
 
 # license
 
 gitonic is released under the following
 [`LICENSE`](https://github.com/kr-g/gitonic/blob/main/LICENSE.md)
 
 
+
+
 # Changelog
 
 
+# version v0.0.9 - 20221008
+
+- git current branch in changes tab
+- support for black
+- 
+
+
 # version v0.0.8 - 20220802
 
 - bug fix, due to corrupted local env
 - double click in changes view will stage/ unstage a file
 - 
 
 
@@ -255,25 +305,27 @@
 - revert changes / git checkout support
 - git branch support
   - create
   - switch
 - git tag support
 - git stash support (list, show, push, pop/apply, drop, clear)
 - merge tool integration
+- diff-tool blocks main screen
 - settings tabs
   - check for installed git
   - ~~git exe configuration in settings~~
   - check for latest version of gitonic
   - 
 - ~~config file for last known config~~
 - gui rework
   - theme support
   - resize behavior -> expand
-  - icons
-  - 
+  - ~~icons~~
+  - grid layout / less floating 
+  -
 - background task and event loop -> freezing gui when running git utils
   - use TkCmd also for Cmd runners
   - status bar with running background tasks overview?
   -
 - refact for integration in other tools
 - filter git on 'changes' tab
 - rework logging
@@ -283,15 +335,16 @@
   - black PEP8 support
   - desktop integration
     - open shell at repo path
     - open file management too at repo path
 - ~~history of commit texts~~
   - ~~in combo box~~
   - git log / show integration?
-
+- git error handling
+- 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
 
 # LIMITATIONS
@@ -302,15 +355,18 @@
  commited changes (same behavior as cmd-line `git difftool`)
 - git credentials basic support, 
  you need to use https://git-scm.com/docs/git-credential-store.
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
-- 
+- `gitonic` interacts with `git` just like starting in bash / commandline.
+at the present time there is _no_additional_ error checking. 
+this must be done by checking the log tab manually where all cmdline output goes.
+
  
 
 
 ---
 
 Copyright (c) 2022 k. goger - https://github.com/kr-g
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gitonic-0.0.8/gitonic.egg-info/SOURCES.txt` & `gitonic-0.0.9/gitonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/setup.cfg` & `gitonic-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.8/setup.py` & `gitonic-0.0.9/setup.py`

 * *Files identical despite different names*

