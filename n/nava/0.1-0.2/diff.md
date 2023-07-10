# Comparing `tmp/nava-0.1.tar.gz` & `tmp/nava-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nava-0.1.tar", last modified: Sat Jun 10 13:00:51 2023, max compression
+gzip compressed data, was "nava-0.2.tar", last modified: Mon Jul 10 12:26:14 2023, max compression
```

## Comparing `nava-0.1.tar` & `nava-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:00:51.919585 nava-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-10 13:00:39.000000 nava-0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-10 13:00:39.000000 nava-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-10 13:00:51.919585 nava-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-10 13:00:39.000000 nava-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:00:51.915584 nava-0.1/nava/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-10 13:00:39.000000 nava-0.1/nava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-10 13:00:39.000000 nava-0.1/nava/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 13:00:39.000000 nava-0.1/nava/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-10 13:00:39.000000 nava-0.1/nava/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-10 13:00:39.000000 nava-0.1/nava/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:00:51.915584 nava-0.1/nava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 13:00:51.000000 nava-0.1/nava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:00:51.919585 nava-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-10 13:00:39.000000 nava-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:26:14.601512 nava-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 12:26:04.000000 nava-0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-10 12:26:04.000000 nava-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 12:26:14.601512 nava-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-10 12:26:04.000000 nava-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:26:14.601512 nava-0.2/nava/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 12:26:04.000000 nava-0.2/nava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-10 12:26:04.000000 nava-0.2/nava/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 12:26:04.000000 nava-0.2/nava/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-10 12:26:04.000000 nava-0.2/nava/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 12:26:04.000000 nava-0.2/nava/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:26:14.601512 nava-0.2/nava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 12:26:14.000000 nava-0.2/nava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:26:14.601512 nava-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-10 12:26:04.000000 nava-0.2/setup.py
```

### Comparing `nava-0.1/LICENSE` & `nava-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nava-0.1/PKG-INFO` & `nava-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nava
-Version: 0.1
+Version: 0.2
 Summary: A Python library for playing sound everywhere natively and securely. 
 Home-page: https://github.com/openscilab/nava
-Download-URL: https://github.com/openscilab/nava/tarball/v0.1
+Download-URL: https://github.com/openscilab/nava/tarball/v0.2
 Author: OpenSciLab Development Team
 Author-email: info@openscilab.com
 License: MIT
 Project-URL: Webpage, https://openscilab.com/
 Project-URL: Source, https://github.com/openscilab/nava
 Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio
@@ -32,22 +32,26 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
+    <img src="https://github.com/openscilab/nava/raw/main/others/logo.png" width="300" height="300">
     <h1>Nava</h1>
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
+	<a href="https://codecov.io/gh/openscilab/nava">
+		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+	</a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
 ## Table of contents
    * [Overview](https://github.com/openscilab/nava#overview)
@@ -91,31 +95,47 @@
 <table>
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>
 		<td align="center">dev</td>
 	</tr>
     <tr>
-		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center">Linux CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">Windows CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">macOS CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.1` (Need root access)
+- Run `pip install nava==0.2`
 
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/nava/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/nava/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
+### Conda
+
+- Check [Conda Managing Package](https://conda.io/)
+- Update Conda using `conda update conda`
+- Run `conda install -c openscilab nava`
+
 ## Usage
 
 ### Basic
 ```python
 from nava import play
 play("alarm.wav")
 ```
@@ -159,19 +179,30 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.2] - 2023-07-10
+### Added
+- Logo
+- Anaconda package
+### Changed
+- `quote` decorator bug fixed
+- `path_check` decorator bug fixed
+- Test system modified
+- `README.md` modified 
 ## [0.1] - 2023-06-10
 ### Added
 - `README.md`
 - `__play_win` function
 - `__play_linux` function
 - `__play_mac` function
 - `quote` function
 - `path_check` function
 - `play` function
 
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.1...dev
+
+[Unreleased]: https://github.com/openscilab/nava/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/nava/compare/bd789cc...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nava Version: 0.1 Summary: A Python library for
+Metadata-Version: 2.1 Name: nava Version: 0.2 Summary: A Python library for
 playing sound everywhere natively and securely. Home-page: https://github.com/
-openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.1
+openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.2
 Author: OpenSciLab Development Team Author-email: info@openscilab.com License:
 MIT Project-URL: Webpage, https://openscilab.com/ Project-URL: Source, https://
 github.com/openscilab/nava Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -14,17 +14,18 @@
 Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Manufacturing Classifier: Topic :: Multimedia Classifier:
 Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Multimedia :: Sound/
 Audio :: Players Classifier: Topic :: Multimedia :: Sound/Audio :: Players ::
 MP3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE License-File: AUTHORS.md
+         [https://github.com/openscilab/nava/raw/main/others/logo.png]
                               ****** Nava ******
 
-             [built_with_Python3] [PyPI_version] [Discord_Channel]
+        [built_with_Python3] [PyPI_version] [Codecov] [Discord_Channel]
 ## Table of contents * [Overview](https://github.com/openscilab/nava#overview)
 * [Installation](https://github.com/openscilab/nava#installation) * [Usage]
 (https://github.com/openscilab/nava#usage) * [Issues & Bug Reports](https://
 github.com/openscilab/nava#issues--bug-reports) * [Contribution](https://
 github.com/openscilab/nava/blob/main/.github/CONTRIBUTING.md) * [Authors]
 (https://github.com/openscilab/nava/blob/main/AUTHORS.md) * [License](https://
 github.com/openscilab/nava/blob/main/LICENSE) * [Show Your Support](https://
@@ -35,36 +36,47 @@
 dependencies or platform restrictions. It is a cross-platform solution that
 runs on any operating system, including Windows, macOS, and Linux. Its
 lightweight and easy-to-use design makes Nava an ideal choice for developers
 looking to add sound functionality to their Python programs.
 PyPI Counter               [http://pepy.tech/badge/nava]
 Github Stars [https://img.shields.io/github/stars/openscilab/
                     nava.svg?style=social&label=Stars]
-Branch                     main                                dev
-       [https://github.com/openscilab/ [https://github.com/openscilab/nava/
-   CI        nava/workflows/CI/         workflows/CI/badge.svg?branch=dev]
-           badge.svg?branch=main]
+   Branch                      main                                dev
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+ Linux CI       nava/workflows/Linux/                workflows/Linux/
+               badge.svg?branch=main]             badge.svg?branch=dev]
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+Windows CI     nava/workflows/Windows/              workflows/Windows/
+               badge.svg?branch=main]             badge.svg?branch=dev]
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+ macOS CI       nava/workflows/macOS/                workflows/macOS/
+               badge.svg?branch=main]             badge.svg?branch=dev]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install nava==0.1` (Need root
-access) ### Source code - Download [Version 0.1](https://github.com/openscilab/
-nava/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/nava/
-archive/dev.zip) - Run `pip install .` ## Usage ### Basic ```python from nava
-import play play("alarm.wav") ``` ### Error ```python from nava import play,
-NavaBaseError try: play("alarm.wav") except NavaBaseError as e: print(str(e))
-``` ## Issues & bug reports Just fill an issue and describe it. We'll check it
-ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com
-"info@openscilab.com"). - Please complete the issue template You can also join
-our discord server [Discord_Channel] ## Show your support
+packaging.python.org/installing/) - Run `pip install nava==0.2` ### Source code
+- Download [Version 0.2](https://github.com/openscilab/nava/archive/v0.2.zip)
+or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip) - Run
+`pip install .` ### Conda - Check [Conda Managing Package](https://conda.io/) -
+Update Conda using `conda update conda` - Run `conda install -c openscilab
+nava` ## Usage ### Basic ```python from nava import play play("alarm.wav") ```
+### Error ```python from nava import play, NavaBaseError try: play("alarm.wav")
+except NavaBaseError as e: print(str(e)) ``` ## Issues & bug reports Just fill
+an issue and describe it. We'll check it ASAP! or send an email to
+[info@openscilab.com](mailto:info@openscilab.com "info@openscilab.com"). -
+Please complete the issue template You can also join our discord server
+[Discord_Channel] ## Show your support
 **** Star this repo ****
 Give a â­ï¸ if this project helped you!
 **** Donate to our project ****
 If you do like our project and we hope that you do, can you please support us?
 Our project is not and is never going to be working for profit. We need the
 money just so we can continue doing what we do ;-) . [Nava_Donation] #
 Changelog All notable changes to this project will be documented in this file.
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/
 ) and this project adheres to [Semantic Versioning](http://semver.org/spec/
-v2.0.0.html). ## [Unreleased] ## [0.1] - 2023-06-10 ### Added - `README.md` -
-`__play_win` function - `__play_linux` function - `__play_mac` function -
-`quote` function - `path_check` function - `play` function [Unreleased]: https:
-//github.com/openscilab/nava/compare/v0.1...dev [0.1]: https://github.com/
-openscilab/nava/compare/bd789cc...v0.1
+v2.0.0.html). ## [Unreleased] ## [0.2] - 2023-07-10 ### Added - Logo - Anaconda
+package ### Changed - `quote` decorator bug fixed - `path_check` decorator bug
+fixed - Test system modified - `README.md` modified ## [0.1] - 2023-06-10 ###
+Added - `README.md` - `__play_win` function - `__play_linux` function -
+`__play_mac` function - `quote` function - `path_check` function - `play`
+function [Unreleased]: https://github.com/openscilab/nava/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2 [0.1]: https://
+github.com/openscilab/nava/compare/bd789cc...v0.1
```

### Comparing `nava-0.1/README.md` & `nava-0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 <div align="center">
+    <img src="https://github.com/openscilab/nava/raw/main/others/logo.png" width="300" height="300">
     <h1>Nava</h1>
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
+	<a href="https://codecov.io/gh/openscilab/nava">
+		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+	</a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
 ## Table of contents
    * [Overview](https://github.com/openscilab/nava#overview)
@@ -54,31 +58,47 @@
 <table>
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>
 		<td align="center">dev</td>
 	</tr>
     <tr>
-		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center">Linux CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">Windows CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">macOS CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.1` (Need root access)
+- Run `pip install nava==0.2`
 
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/nava/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/nava/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
+### Conda
+
+- Check [Conda Managing Package](https://conda.io/)
+- Update Conda using `conda update conda`
+- Run `conda install -c openscilab nava`
+
 ## Usage
 
 ### Basic
 ```python
 from nava import play
 play("alarm.wav")
 ```
```

### Comparing `nava-0.1/nava/functions.py` & `nava-0.2/nava/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 """Nava functions."""
 import sys
 import subprocess
 import os
 import shlex
+from functools import wraps
 
-from .params import OVERVIEW, SOUND_FILE_PLAY_ERROR, SOUND_FILE_EXIST_ERROR, SOUND_FILE_PATH_TYPE_ERROR
+from .params import OVERVIEW
+from .params import SOUND_FILE_PLAY_ERROR, SOUND_FILE_EXIST_ERROR
+from .params import SOUND_FILE_PATH_TYPE_ERROR
 from .errors import NavaBaseError
 
 
 def nava_help():
     """
     Print nava details.
 
@@ -22,29 +25,30 @@
 
 def quote(func):
     """
     Quote the given shell string.
 
     :return: inner function
     """
-    def inner_function(*args, **kwargs):
+    @wraps(func)
+    def quoter(sound_path, *args, **kwargs):
         """
         Inner function.
 
+        :param sound_path: sound path
+        :type sound_path: str
         :param args: non-keyword arguments
         :type args: list
         :param kwargs: keyword arguments
         :type kwargs: dict
         :return: modified function result
         """
-        sound_path = args[0]
         sound_path = shlex.quote(sound_path)
-        args[0] = sound_path
-        return func(*args, **kwargs)
-    return inner_function
+        return func(sound_path, *args, **kwargs)
+    return quoter
 
 
 def __play_win(sound_path):
     """
     Play sound in Windows.
 
     :param sound_path: sound path
@@ -91,32 +95,34 @@
 
 def path_check(func):
     """
     Check the given path to be a string and a valid file directory.
 
     :return: inner function
     """
-    def inner_function(*args, **kwargs):
+    @wraps(func)
+    def path_checker(sound_path, *args, **kwargs):
         """
         Inner function.
 
+        :param sound_path: sound path
+        :type sound_path: str
         :param args: non-keyword arguments
         :type args: list
         :param kwargs: keyword arguments
         :type kwargs: dict
         :return: modified function result
         """
-        sound_path = args[0]
-        if not (isinstance(sound_path, str)):
+        if not isinstance(sound_path, str):
             raise NavaBaseError(SOUND_FILE_PATH_TYPE_ERROR)
         # check sound file existance
-        if not (os.path.isfile(sound_path)):
+        if not os.path.isfile(sound_path):
             raise NavaBaseError(SOUND_FILE_EXIST_ERROR)
-        return func(*args, **kwargs)
-    return inner_function
+        return func(sound_path, *args, **kwargs)
+    return path_checker
 
 
 @path_check
 def play(sound_path):
     """
     Play sound.
 
@@ -128,9 +134,9 @@
         sys_platform = sys.platform
         if sys_platform == "win32":
             __play_win(sound_path)
         elif sys_platform == "darwin":
             __play_mac(sound_path)
         else:
             __play_linux(sound_path)
-    except Exception:
+    except Exception: # pragma: no cover
         raise NavaBaseError(SOUND_FILE_PLAY_ERROR)
```

### Comparing `nava-0.1/nava.egg-info/PKG-INFO` & `nava-0.2/nava.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nava
-Version: 0.1
+Version: 0.2
 Summary: A Python library for playing sound everywhere natively and securely. 
 Home-page: https://github.com/openscilab/nava
-Download-URL: https://github.com/openscilab/nava/tarball/v0.1
+Download-URL: https://github.com/openscilab/nava/tarball/v0.2
 Author: OpenSciLab Development Team
 Author-email: info@openscilab.com
 License: MIT
 Project-URL: Webpage, https://openscilab.com/
 Project-URL: Source, https://github.com/openscilab/nava
 Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio
@@ -32,22 +32,26 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
+    <img src="https://github.com/openscilab/nava/raw/main/others/logo.png" width="300" height="300">
     <h1>Nava</h1>
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
+	<a href="https://codecov.io/gh/openscilab/nava">
+		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+	</a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
 ## Table of contents
    * [Overview](https://github.com/openscilab/nava#overview)
@@ -91,31 +95,47 @@
 <table>
 	<tr> 
 		<td align="center">Branch</td>
 		<td align="center">main</td>
 		<td align="center">dev</td>
 	</tr>
     <tr>
-		<td align="center">CI</td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=main"></td>
-		<td align="center"><img src="https://github.com/openscilab/nava/workflows/CI/badge.svg?branch=dev"></td>
+		<td align="center">Linux CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Linux/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">Windows CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/Windows/badge.svg?branch=dev"></td>
+	</tr>
+	<tr>
+		<td align="center">macOS CI</td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=main"></td>
+		<td align="center"><img src="https://github.com/openscilab/nava/workflows/macOS/badge.svg?branch=dev"></td>
 	</tr>
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.1` (Need root access)
+- Run `pip install nava==0.2`
 
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/nava/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/nava/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
+### Conda
+
+- Check [Conda Managing Package](https://conda.io/)
+- Update Conda using `conda update conda`
+- Run `conda install -c openscilab nava`
+
 ## Usage
 
 ### Basic
 ```python
 from nava import play
 play("alarm.wav")
 ```
@@ -159,19 +179,30 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.2] - 2023-07-10
+### Added
+- Logo
+- Anaconda package
+### Changed
+- `quote` decorator bug fixed
+- `path_check` decorator bug fixed
+- Test system modified
+- `README.md` modified 
 ## [0.1] - 2023-06-10
 ### Added
 - `README.md`
 - `__play_win` function
 - `__play_linux` function
 - `__play_mac` function
 - `quote` function
 - `path_check` function
 - `play` function
 
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.1...dev
+
+[Unreleased]: https://github.com/openscilab/nava/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/nava/compare/bd789cc...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nava Version: 0.1 Summary: A Python library for
+Metadata-Version: 2.1 Name: nava Version: 0.2 Summary: A Python library for
 playing sound everywhere natively and securely. Home-page: https://github.com/
-openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.1
+openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.2
 Author: OpenSciLab Development Team Author-email: info@openscilab.com License:
 MIT Project-URL: Webpage, https://openscilab.com/ Project-URL: Source, https://
 github.com/openscilab/nava Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio Classifier: Development Status :: 2
 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Natural
 Language :: English Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -14,17 +14,18 @@
 Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: End Users/Desktop Classifier:
 Intended Audience :: Manufacturing Classifier: Topic :: Multimedia Classifier:
 Topic :: Multimedia :: Sound/Audio Classifier: Topic :: Multimedia :: Sound/
 Audio :: Players Classifier: Topic :: Multimedia :: Sound/Audio :: Players ::
 MP3 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE License-File: AUTHORS.md
+         [https://github.com/openscilab/nava/raw/main/others/logo.png]
                               ****** Nava ******
 
-             [built_with_Python3] [PyPI_version] [Discord_Channel]
+        [built_with_Python3] [PyPI_version] [Codecov] [Discord_Channel]
 ## Table of contents * [Overview](https://github.com/openscilab/nava#overview)
 * [Installation](https://github.com/openscilab/nava#installation) * [Usage]
 (https://github.com/openscilab/nava#usage) * [Issues & Bug Reports](https://
 github.com/openscilab/nava#issues--bug-reports) * [Contribution](https://
 github.com/openscilab/nava/blob/main/.github/CONTRIBUTING.md) * [Authors]
 (https://github.com/openscilab/nava/blob/main/AUTHORS.md) * [License](https://
 github.com/openscilab/nava/blob/main/LICENSE) * [Show Your Support](https://
@@ -35,36 +36,47 @@
 dependencies or platform restrictions. It is a cross-platform solution that
 runs on any operating system, including Windows, macOS, and Linux. Its
 lightweight and easy-to-use design makes Nava an ideal choice for developers
 looking to add sound functionality to their Python programs.
 PyPI Counter               [http://pepy.tech/badge/nava]
 Github Stars [https://img.shields.io/github/stars/openscilab/
                     nava.svg?style=social&label=Stars]
-Branch                     main                                dev
-       [https://github.com/openscilab/ [https://github.com/openscilab/nava/
-   CI        nava/workflows/CI/         workflows/CI/badge.svg?branch=dev]
-           badge.svg?branch=main]
+   Branch                      main                                dev
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+ Linux CI       nava/workflows/Linux/                workflows/Linux/
+               badge.svg?branch=main]             badge.svg?branch=dev]
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+Windows CI     nava/workflows/Windows/              workflows/Windows/
+               badge.svg?branch=main]             badge.svg?branch=dev]
+           [https://github.com/openscilab/ [https://github.com/openscilab/nava/
+ macOS CI       nava/workflows/macOS/                workflows/macOS/
+               badge.svg?branch=main]             badge.svg?branch=dev]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install nava==0.1` (Need root
-access) ### Source code - Download [Version 0.1](https://github.com/openscilab/
-nava/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/nava/
-archive/dev.zip) - Run `pip install .` ## Usage ### Basic ```python from nava
-import play play("alarm.wav") ``` ### Error ```python from nava import play,
-NavaBaseError try: play("alarm.wav") except NavaBaseError as e: print(str(e))
-``` ## Issues & bug reports Just fill an issue and describe it. We'll check it
-ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com
-"info@openscilab.com"). - Please complete the issue template You can also join
-our discord server [Discord_Channel] ## Show your support
+packaging.python.org/installing/) - Run `pip install nava==0.2` ### Source code
+- Download [Version 0.2](https://github.com/openscilab/nava/archive/v0.2.zip)
+or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip) - Run
+`pip install .` ### Conda - Check [Conda Managing Package](https://conda.io/) -
+Update Conda using `conda update conda` - Run `conda install -c openscilab
+nava` ## Usage ### Basic ```python from nava import play play("alarm.wav") ```
+### Error ```python from nava import play, NavaBaseError try: play("alarm.wav")
+except NavaBaseError as e: print(str(e)) ``` ## Issues & bug reports Just fill
+an issue and describe it. We'll check it ASAP! or send an email to
+[info@openscilab.com](mailto:info@openscilab.com "info@openscilab.com"). -
+Please complete the issue template You can also join our discord server
+[Discord_Channel] ## Show your support
 **** Star this repo ****
 Give a â­ï¸ if this project helped you!
 **** Donate to our project ****
 If you do like our project and we hope that you do, can you please support us?
 Our project is not and is never going to be working for profit. We need the
 money just so we can continue doing what we do ;-) . [Nava_Donation] #
 Changelog All notable changes to this project will be documented in this file.
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/
 ) and this project adheres to [Semantic Versioning](http://semver.org/spec/
-v2.0.0.html). ## [Unreleased] ## [0.1] - 2023-06-10 ### Added - `README.md` -
-`__play_win` function - `__play_linux` function - `__play_mac` function -
-`quote` function - `path_check` function - `play` function [Unreleased]: https:
-//github.com/openscilab/nava/compare/v0.1...dev [0.1]: https://github.com/
-openscilab/nava/compare/bd789cc...v0.1
+v2.0.0.html). ## [Unreleased] ## [0.2] - 2023-07-10 ### Added - Logo - Anaconda
+package ### Changed - `quote` decorator bug fixed - `path_check` decorator bug
+fixed - Test system modified - `README.md` modified ## [0.1] - 2023-06-10 ###
+Added - `README.md` - `__play_win` function - `__play_linux` function -
+`__play_mac` function - `quote` function - `path_check` function - `play`
+function [Unreleased]: https://github.com/openscilab/nava/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2 [0.1]: https://
+github.com/openscilab/nava/compare/bd789cc...v0.1
```

### Comparing `nava-0.1/setup.py` & `nava-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
    It is a cross-platform solution that runs on any operating system, including Windows, macOS, and Linux.
    Its lightweight and easy-to-use design makes Nava an ideal choice for developers looking to add sound functionality to their Python programs.'''
 
 
 setup(
     name='nava',
     packages=['nava'],
-    version='0.1',
+    version='0.2',
     description='A Python library for playing sound everywhere natively and securely. ',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='OpenSciLab Development Team',
     author_email='info@openscilab.com',
     url='https://github.com/openscilab/nava',
-    download_url='https://github.com/openscilab/nava/tarball/v0.1',
+    download_url='https://github.com/openscilab/nava/tarball/v0.2',
     keywords="sound wav music mp3 player audio",
     project_urls={
         'Webpage': 'https://openscilab.com/',
         'Source': 'https://github.com/openscilab/nava',
         'Discord': 'https://discord.gg/MCbPKCFBs3',
     },
     install_requires=get_requires(),
```

