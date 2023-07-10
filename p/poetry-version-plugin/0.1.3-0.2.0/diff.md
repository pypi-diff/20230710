# Comparing `tmp/poetry-version-plugin-0.1.3.tar.gz` & `tmp/poetry_version_plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-version-plugin-0.1.3.tar", max compression
+gzip compressed data, was "poetry_version_plugin-0.2.0.tar", max compression
```

## Comparing `poetry-version-plugin-0.1.3.tar` & `poetry_version_plugin-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1086 2021-05-27 12:45:31.898231 poetry-version-plugin-0.1.3/LICENSE
--rw-r--r--   0        0        0    12677 2021-05-27 12:45:31.898231 poetry-version-plugin-0.1.3/README.md
--rw-r--r--   0        0        0        0 2021-05-27 12:45:31.898231 poetry-version-plugin-0.1.3/poetry_version_plugin/__init__.py
--rw-r--r--   0        0        0     4746 2021-05-27 12:45:31.898231 poetry-version-plugin-0.1.3/poetry_version_plugin/plugin.py
--rw-r--r--   0        0        0     2082 2021-05-27 12:45:31.898231 poetry-version-plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    13994 2021-05-27 12:46:26.011617 poetry-version-plugin-0.1.3/setup.py
--rw-r--r--   0        0        0    14336 2021-05-27 12:46:26.012154 poetry-version-plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-07-10 15:46:03.522501 poetry_version_plugin-0.2.0/LICENSE
+-rw-r--r--   0        0        0    13045 2023-07-10 15:46:03.522501 poetry_version_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 15:46:03.522501 poetry_version_plugin-0.2.0/poetry_version_plugin/__init__.py
+-rw-r--r--   0        0        0     4737 2023-07-10 15:46:03.522501 poetry_version_plugin-0.2.0/poetry_version_plugin/plugin.py
+-rw-r--r--   0        0        0     2001 2023-07-10 15:46:03.522501 poetry_version_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14703 1970-01-01 00:00:00.000000 poetry_version_plugin-0.2.0/PKG-INFO
```

### Comparing `poetry-version-plugin-0.1.3/LICENSE` & `poetry_version_plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-version-plugin-0.1.3/README.md` & `poetry_version_plugin-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 
 ```python
 # __init__.py
 
 __version__ = "0.1.0"
 ```
 
-or alternatively, it can read it from a **git tag**, set with a GitHub release or with:
+Alternatively, it can read it from a **git tag**, set with a GitHub release or with:
 
 ```console
 $ git tag 0.1.0
 ```
 
-🚨 Consider this in alpha stage. Read the warning below.
+🚨 Consider this in the alpha stage. Read the warning below.
 
 ## When to use
 
 This is useful mainly if you are building a package library for others to use and you want to set the version in a place different than `pyproject.toml`, but you still want to keep a [single source of truth](https://en.wikipedia.org/wiki/Single_source_of_truth).
 
-It won't be useful in other use cases like managing local app environments with Poetry.
+It won't be helpful in other use cases like managing local app environments with Poetry.
 
 ## How to use
 
-Make sure you have Poetry version `1.2.0a1` or above. Read below for instructions to install it if you haven't.
+Make sure you have Poetry version `1.2.0` or above. Read below for instructions to install it if you haven't.
 
 ### Install Poetry Version Plugin
 
 Install this plugin to your Poetry:
 
 ```console
 $ poetry plugin add poetry-version-plugin
@@ -64,15 +64,15 @@
 And then edit your `pyproject.toml` with a section containing:
 
 ```toml
 [tool.poetry-version-plugin]
 source = "init"
 ```
 
-Next, build your project, it will show an output like:
+Next, build your project. It will show an output like:
 
 ```console
 $ poetry build
 Using __init__.py file at my_awesome_package/__init__.py for dynamic version
 Setting package dynamic version to __version__ variable from __init__.py: 0.1.9
 Building my-awesome-package (0.1.9)
   - Building sdist
@@ -92,15 +92,15 @@
 
 Then create a git tag, for example:
 
 ```console
 $ git tag 0.1.3
 ```
 
-In this case, when building your project it will show an output like:
+In this case, when building your project, it will show an output like:
 
 ```console
 $ poetry build
 Git tag found, setting dynamic version to: 0.1.3
 Building my-awesome-package (0.1.3)
   - Building sdist
   - Built my-awesome-package-0.1.3.tar.gz
@@ -110,15 +110,15 @@
 
 ## Version in `pyproject.toml`
 
 Currently (2021-05-24) Poetry requires a `version` configuration in the `pyproject.toml`, even if you use this plugin.
 
 When using this plugin, that `version` config won't be used, but Poetry still requires it to be present in the `pyproject.toml`.
 
-To make it more obvious that you are not really using that `version` you can set it to `0`.
+To make it more evident that you are not using that `version` you can set it to `0`.
 
 ```toml
 [tool.poetry]
 name = "my-awesome-package"
 version = "0"
 ```
 
@@ -133,29 +133,29 @@
 name = "my-awesome-package"
 version = "0"
 description = ""
 authors = ["Rick Sanchez <rick@rick-citadel.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-version-plugin]
 source = "init"
 ```
 
 ## Why
 
-By default Poetry expects you to set your package version in `pyproject.toml`. And that would work in most cases.
+By default, Poetry expects you to set your package version in `pyproject.toml`. And that would work in most cases.
 
-But imagine you want to expose the version of your package in a `__version__` variable, so that your users can do things like:
+But imagine you want to expose the version of your package in a `__version__` variable so that your users can do things like:
 
 ```python
 import my_awesome_package
 print(my_awesome_package.__version__)
 ```
 
 You could manually write the `__version__` variable and handle the synchronization between it and the `pyproject.toml` yourself, which is very **error-prone**.
@@ -165,15 +165,15 @@
 But that module is only available in Python 3.8 and above. So, for Python 3.7 and 3.6 you have to install a backport as a dependency of your package:
 
 ```toml
 [tool.poetry.dependencies]
 importlib-metadata = {version = "^1.0", python = "<3.8"}
 ```
 
-But then, when they release each new version of the backport (currently `4.0.1`), you have to update it (or not). And your users would have to manually handle conflicts with any other packages that also depend on `importlib-metadata`, which could be multiple, as many packages could be doing the same trick (I've dealt with that).
+But then, when they release each new version of the backport (currently `4.0.1`), you have to update it (or not). And your users would have to manually handle conflicts with any other packages that also depend on `importlib-metadata` which could be multiple, as many packages could be doing the same trick (I've dealt with that).
 
 The other option is not to pin any version range of your `importlib-metadata` in your `pyproject.toml` and hope for the best.
 
 And then your `__init__.py` would have to include code using it, like:
 
 ```python
 # I don't want this extra complexity 😔
@@ -202,19 +202,19 @@
 
 Alternatively, this plugin can also extract the version from a Git tag.
 
 So, you could only create each version in a Git tag (for example, a GitHub release) instead of writing it in code.
 
 And then build the package on Continuous Integration (e.g. GitHub Actions). And this plugin would get the version of the package from that Git tag.
 
-## Install Poetry `1.2.0a1`
+## Install Poetry `1.2.0`
 
-For this plugin to work, you need Poetry version `1.2.0a1` or above.
+For this plugin to work, you need Poetry version `1.2.0` or above.
 
-[Poetry `1.2.0a1` was released recently](https://python-poetry.org/blog/announcing-poetry-1-2-0a1.html).
+[Poetry `1.2.0` was released recently](https://python-poetry.org/blog/announcing-poetry-1.2.0/).
 
 There's a high chance you already have installed Poetry `1.1.x`.
 
 The first step is to uninstall it:
 
 ```console
 $ curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -O
@@ -230,36 +230,36 @@
 $ curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py -O
 --> 100%
 
 $ python install-poetry.py --preview
 --> 100%
 ```
 
-🔍 Notice that the new installer file is named `install-poetry.py` instead of `get-poetry.py`. Also notice that, currently, you need to set `--preview` for it to install the alpha version `1.2.0a1`.
+🔍 Notice that the new installer file is named `install-poetry.py` instead of `get-poetry.py`. Also, notice that, currently, you need to set `--preview` for it to install the alpha version `1.2.0`.
 
 You can check that it worked with:
 
 ```console
 $ poetry --version
-Poetry (version 1.2.0a1)
+Poetry (version 1.2.0)
 ```
 
 ## Support for version in init file
 
 When using a `__version__` variable in your `__init__.py` you can have more logic in that file, import modules, and do more things above and below the declaration of that variable.
 
 But the value has to be a literal string, like:
 
 ```python
 ___version___ = "0.2.0"
 ```
 
 ...instead of calling a function or something similar.
 
-And the variable has to be in the top-level, so it can't be inside an `if` statement or similar.
+And the variable has to be at the top-level, so it can't be inside an `if` statement or similar.
 
 This is all fine and supported in your `__init__.py`:
 
 ```python
 # __init__.py
 
 # This is all valid 👍✅
@@ -305,37 +305,37 @@
     return "0.2.0"
 
 __version__ = get_version()
 ```
 
 ## How the plugin works
 
-Poetry runs the plugin when building a package, and it sets the version right before creating the "package distributable" (e.g. the wheel).
+Poetry runs the plugin when building a package, and it sets the version right before creating the "package distributable" (e.g., the wheel).
 
 ### How the version variable works
 
 If you have a package (a single package) declared in the `packages` config in your `pyproject.toml`, the plugin will use that package's `__init__.py` to find the `__version__` variable.
 
 If you don't have any `packages` config, the plugin will assume that you have a single package named as your project, but in the module version (changing `-` for `_`). So, if your package is `my-awesome-project`, the plugin will use the file at `my_awesome_project/__init__.py` to find the `__version__` variable.
 
-This file structure is the default if you create a new project with the command `poetry new`, so it should just work as expected. ✨
+This file structure is the default if you create a new project with the command `poetry new`, so it should work as expected. ✨
 
 The way the plugin works internally is by parsing the `__init__.py` file. Reading the Python's "Abstract Syntax Tree" using the `ast` standard module and extracting the literal value of the string. So, it doesn't execute the code in `__init__.py`, it only reads it as Python code.
 
 The plugin doesn't try to import and execute that `__init__.py` file because that could require extra computation, external dependencies, etc. And it doesn't try to extract the `__version__` with regular expressions, as that would be prone to errors if, for example, there was some other `__version__` somewhere in the code, in a comment or inside a string.
 
 ## Warning
 
-🚨 Consider this in alpha stage. Poetry `1.2.0a1` with support for plugins was released on 2021-05-21, I started writing this plugin 3 days later, on 2021-05-24.
+🚨 Consider this in the alpha stage. Poetry `1.2.0a1` with support for plugins was released on 2021-05-21. I started writing this plugin 3 days later, on 2021-05-24.
 
 Things might break in Poetry or in this plugin. So, please try it and test it very carefully before fully adopting it for delicate systems.
 
 The way it works might change, and the specific configuration might change.
 
-Also, if you don't find intuitive the sections:
+Also, if you don't find the following sections intuitive:
 
 ```toml
 [tool.poetry-version-plugin]
 source = "init"
 ```
 
 and
@@ -349,14 +349,20 @@
 
 👍 The good news is, assuming you are building packages to then upload them to PyPI for your users to download and use them, the **worst that could happen** if something broke is that you wouldn't be able to build a new version until something is fixed or changed. But your users shouldn't be affected in any way.
 
 ## Release Notes
 
 ### Latest Changes
 
+
+### 0.2.0
+
+* ✨ Add support for Poetry 1.2.0 and above (including 1.5.1), deprecate support for Python 3.6. PR [#28](https://github.com/tiangolo/poetry-version-plugin/pull/28) by [@mbeacom](https://github.com/mbeacom).
+* ✏️ Fix typos and rewording in README.md. PR [#8](https://github.com/tiangolo/poetry-version-plugin/pull/8) by [@Gl0deanR](https://github.com/Gl0deanR).
+
 ### 0.1.3
 
 * ✨ Improve logs, prefix with plugin name. PR [#6](https://github.com/tiangolo/poetry-version-plugin/pull/6) by [@tiangolo](https://github.com/tiangolo).
 * 🔧 Update pyproject metadata. PR [#5](https://github.com/tiangolo/poetry-version-plugin/pull/5) by [@tiangolo](https://github.com/tiangolo).
 * ✅ Fix coverage. PR [#4](https://github.com/tiangolo/poetry-version-plugin/pull/4) by [@tiangolo](https://github.com/tiangolo).
 * 📝 Improve docs. PR [#3](https://github.com/tiangolo/poetry-version-plugin/pull/3) by [@tiangolo](https://github.com/tiangolo).
 * 🐛 Fix tests for CI. PR [#1](https://github.com/tiangolo/poetry-version-plugin/pull/1) by [@tiangolo](https://github.com/tiangolo).
```

### Comparing `poetry-version-plugin-0.1.3/poetry_version_plugin/plugin.py` & `poetry_version_plugin-0.2.0/poetry_version_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import ast
 import subprocess
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from cleo.io.io import IO
+from poetry.core.utils.helpers import module_name
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
-from poetry.utils.helpers import module_name
 
 
-class VersionPlugin(Plugin):  # type: ignore
+class VersionPlugin(Plugin):
     def activate(self, poetry: Poetry, io: IO) -> None:
         poetry_version_config: Optional[Dict[str, Any]] = poetry.pyproject.data.get(
             "tool", {}
         ).get("poetry-version-plugin")
         if poetry_version_config is None:
             return
         version_source = poetry_version_config.get("source")
@@ -70,15 +70,15 @@
                                     # Ref: https://github.com/nedbat/coveragepy/issues/198
                                     continue
                                 io.write_line(
                                     "<b>poetry-version-plugin</b>: Setting package "
                                     "dynamic version to __version__ "
                                     f"variable from __init__.py: <b>{version}</b>"
                                 )
-                                poetry.package.set_version(version)
+                                poetry.package._set_version(version)
                                 return
             message = (
                 "<b>poetry-version-plugin</b>: No valid __version__ variable found "
                 "in __init__.py, cannot extract dynamic version"
             )
             io.write_error_line(message)
             raise RuntimeError(message)
@@ -91,15 +91,15 @@
             )
             if result.returncode == 0:
                 tag = result.stdout.strip()
                 io.write_line(
                     "<b>poetry-version-plugin</b>: Git tag found, setting "
                     f"dynamic version to: {tag}"
                 )
-                poetry.package.set_version(tag)
+                poetry.package._set_version(tag)
                 return
             else:
                 message = (
                     "<b>poetry-version-plugin</b>: No Git tag found, not "
                     "extracting dynamic version"
                 )
                 io.write_error_line(message)
```

### Comparing `poetry-version-plugin-0.1.3/pyproject.toml` & `poetry_version_plugin-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-version-plugin"
-version = "0.1.3"
+version = "0.2.0"
 description = "Poetry plugin for dynamically extracting the package version from a __version__ variable or a Git tag."
 authors = ["Sebastián Ramírez <tiangolo@gmail.com>"]
 homepage = "https://github.com/tiangolo/poetry-version-plugin"
 documentation = "https://github.com/tiangolo/poetry-version-plugin"
 readme = "README.md"
 packages = [{include = "poetry_version_plugin"}]
 classifiers = [
@@ -20,31 +20,30 @@
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: Software Development",
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Software Distribution",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-poetry = "^1.2.0a1"
+python = "^3.7"
+poetry = "^1.2.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-mypy = "^0.812"
+mypy = "^1.4.1"
+pytest = "^7.1.2"
 flake8 = "^3.9.2"
-black = {version = "^21.5-beta.1", python = ">3.6.2"}
+black = "^23.3.0"
 coverage = {extras = ["toml"], version = "^5.5"}
 pkginfo = "^1.7.0"
 autoflake = "^1.4"
 isort = "^5.8.0"
 
 [tool.poetry.plugins."poetry.plugin"]
 poetry-version-plugin = "poetry_version_plugin.plugin:VersionPlugin"
```

### Comparing `poetry-version-plugin-0.1.3/setup.py` & `poetry_version_plugin-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,875 +1,919 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2770 6f65 7472 795f 7665 7273   \.['poetry_vers
-00000050: 696f 6e5f 706c 7567 696e 275d 0a0a 7061  ion_plugin']..pa
-00000060: 636b 6167 655f 6461 7461 203d 205c 0a7b  ckage_data = \.{
-00000070: 2727 3a20 5b27 2a27 5d7d 0a0a 696e 7374  '': ['*']}..inst
-00000080: 616c 6c5f 7265 7175 6972 6573 203d 205c  all_requires = \
-00000090: 0a5b 2770 6f65 7472 793e 3d31 2e32 2e30  .['poetry>=1.2.0
-000000a0: 6131 2c3c 322e 302e 3027 5d0a 0a65 6e74  a1,<2.0.0']..ent
-000000b0: 7279 5f70 6f69 6e74 7320 3d20 5c0a 7b27  ry_points = \.{'
-000000c0: 706f 6574 7279 2e70 6c75 6769 6e27 3a20  poetry.plugin': 
-000000d0: 5b27 706f 6574 7279 2d76 6572 7369 6f6e  ['poetry-version
-000000e0: 2d70 6c75 6769 6e20 3d20 270a 2020 2020  -plugin = '.    
-000000f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000100: 706f 6574 7279 5f76 6572 7369 6f6e 5f70  poetry_version_p
-00000110: 6c75 6769 6e2e 706c 7567 696e 3a56 6572  lugin.plugin:Ver
-00000120: 7369 6f6e 506c 7567 696e 275d 7d0a 0a73  sionPlugin']}..s
-00000130: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-00000140: 2020 2020 276e 616d 6527 3a20 2770 6f65      'name': 'poe
-00000150: 7472 792d 7665 7273 696f 6e2d 706c 7567  try-version-plug
-00000160: 696e 272c 0a20 2020 2027 7665 7273 696f  in',.    'versio
-00000170: 6e27 3a20 2730 2e31 2e33 272c 0a20 2020  n': '0.1.3',.   
-00000180: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-00000190: 2750 6f65 7472 7920 706c 7567 696e 2066  'Poetry plugin f
-000001a0: 6f72 2064 796e 616d 6963 616c 6c79 2065  or dynamically e
-000001b0: 7874 7261 6374 696e 6720 7468 6520 7061  xtracting the pa
-000001c0: 636b 6167 6520 7665 7273 696f 6e20 6672  ckage version fr
-000001d0: 6f6d 2061 205f 5f76 6572 7369 6f6e 5f5f  om a __version__
-000001e0: 2076 6172 6961 626c 6520 6f72 2061 2047   variable or a G
-000001f0: 6974 2074 6167 2e27 2c0a 2020 2020 276c  it tag.',.    'l
-00000200: 6f6e 675f 6465 7363 7269 7074 696f 6e27  ong_description'
-00000210: 3a20 2723 2050 6f65 7472 7920 5665 7273  : '# Poetry Vers
-00000220: 696f 6e20 506c 7567 696e 5c6e 5c6e 3c61  ion Plugin\n\n<a
-00000230: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000240: 6974 6875 622e 636f 6d2f 7469 616e 676f  ithub.com/tiango
-00000250: 6c6f 2f70 6f65 7472 792d 7665 7273 696f  lo/poetry-versio
-00000260: 6e2d 706c 7567 696e 2f61 6374 696f 6e73  n-plugin/actions
-00000270: 3f71 7565 7279 3d77 6f72 6b66 6c6f 7725  ?query=workflow%
-00000280: 3341 5465 7374 2220 7461 7267 6574 3d22  3ATest" target="
-00000290: 5f62 6c61 6e6b 223e 5c6e 2020 2020 3c69  _blank">\n    <i
-000002a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000002b0: 6769 7468 7562 2e63 6f6d 2f74 6961 6e67  github.com/tiang
-000002c0: 6f6c 6f2f 706f 6574 7279 2d76 6572 7369  olo/poetry-versi
-000002d0: 6f6e 2d70 6c75 6769 6e2f 776f 726b 666c  on-plugin/workfl
-000002e0: 6f77 732f 5465 7374 2f62 6164 6765 2e73  ows/Test/badge.s
-000002f0: 7667 2220 616c 743d 2254 6573 7422 3e5c  vg" alt="Test">\
-00000300: 6e3c 2f61 3e5c 6e3c 6120 6872 6566 3d22  n</a>\n<a href="
-00000310: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000320: 6f6d 2f74 6961 6e67 6f6c 6f2f 706f 6574  om/tiangolo/poet
-00000330: 7279 2d76 6572 7369 6f6e 2d70 6c75 6769  ry-version-plugi
-00000340: 6e2f 6163 7469 6f6e 733f 7175 6572 793d  n/actions?query=
-00000350: 776f 726b 666c 6f77 2533 4150 7562 6c69  workflow%3APubli
-00000360: 7368 2220 7461 7267 6574 3d22 5f62 6c61  sh" target="_bla
-00000370: 6e6b 223e 5c6e 2020 2020 3c69 6d67 2073  nk">\n    <img s
-00000380: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-00000390: 7562 2e63 6f6d 2f74 6961 6e67 6f6c 6f2f  ub.com/tiangolo/
-000003a0: 706f 6574 7279 2d76 6572 7369 6f6e 2d70  poetry-version-p
-000003b0: 6c75 6769 6e2f 776f 726b 666c 6f77 732f  lugin/workflows/
-000003c0: 5075 626c 6973 682f 6261 6467 652e 7376  Publish/badge.sv
-000003d0: 6722 2061 6c74 3d22 5075 626c 6973 6822  g" alt="Publish"
-000003e0: 3e5c 6e3c 2f61 3e5c 6e3c 6120 6872 6566  >\n</a>\n<a href
-000003f0: 3d22 6874 7470 733a 2f2f 636f 6465 636f  ="https://codeco
-00000400: 762e 696f 2f67 682f 7469 616e 676f 6c6f  v.io/gh/tiangolo
-00000410: 2f70 6f65 7472 792d 7665 7273 696f 6e2d  /poetry-version-
-00000420: 706c 7567 696e 2220 7461 7267 6574 3d22  plugin" target="
-00000430: 5f62 6c61 6e6b 223e 5c6e 2020 2020 3c69  _blank">\n    <i
-00000440: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000450: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
-00000460: 6f64 6563 6f76 2f63 2f67 6974 6875 622f  odecov/c/github/
-00000470: 7469 616e 676f 6c6f 2f70 6f65 7472 792d  tiangolo/poetry-
-00000480: 7665 7273 696f 6e2d 706c 7567 696e 3f63  version-plugin?c
-00000490: 6f6c 6f72 3d25 3233 3334 4430 3538 2220  olor=%2334D058" 
-000004a0: 616c 743d 2243 6f76 6572 6167 6522 3e5c  alt="Coverage">\
-000004b0: 6e3c 2f61 3e5c 6e3c 6120 6872 6566 3d22  n</a>\n<a href="
-000004c0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000004d0: 2f70 726f 6a65 6374 2f70 6f65 7472 792d  /project/poetry-
-000004e0: 7665 7273 696f 6e2d 706c 7567 696e 2220  version-plugin" 
-000004f0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000500: 5c6e 2020 2020 3c69 6d67 2073 7263 3d22  \n    <img src="
-00000510: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000520: 6c64 732e 696f 2f70 7970 692f 762f 706f  lds.io/pypi/v/po
-00000530: 6574 7279 2d76 6572 7369 6f6e 2d70 6c75  etry-version-plu
-00000540: 6769 6e3f 636f 6c6f 723d 2532 3333 3444  gin?color=%2334D
-00000550: 3035 3826 6c61 6265 6c3d 7079 7069 2532  058&label=pypi%2
-00000560: 3070 6163 6b61 6765 2220 616c 743d 2250  0package" alt="P
-00000570: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
-00000580: 5c6e 3c2f 613e 5c6e 5c6e 4120 5b2a 2a50  \n</a>\n\nA [**P
-00000590: 6f65 7472 792a 2a5d 2868 7474 7073 3a2f  oetry**](https:/
-000005a0: 2f70 7974 686f 6e2d 706f 6574 7279 2e6f  /python-poetry.o
-000005b0: 7267 2f29 2070 6c75 6769 6e20 666f 7220  rg/) plugin for 
-000005c0: 6479 6e61 6d69 6361 6c6c 7920 6578 7472  dynamically extr
-000005d0: 6163 7469 6e67 2074 6865 2070 6163 6b61  acting the packa
-000005e0: 6765 202a 2a76 6572 7369 6f6e 2a2a 2e5c  ge **version**.\
-000005f0: 6e5c 6e49 7420 6361 6e20 7265 6164 2074  n\nIt can read t
-00000600: 6865 2076 6572 7369 6f6e 2066 726f 6d20  he version from 
-00000610: 6120 6669 6c65 2060 5f5f 696e 6974 5f5f  a file `__init__
-00000620: 2e70 7960 2077 6974 683a 5c6e 5c6e 6060  .py` with:\n\n``
-00000630: 6070 7974 686f 6e5c 6e23 205f 5f69 6e69  `python\n# __ini
-00000640: 745f 5f2e 7079 5c6e 5c6e 5f5f 7665 7273  t__.py\n\n__vers
-00000650: 696f 6e5f 5f20 3d20 2230 2e31 2e30 225c  ion__ = "0.1.0"\
-00000660: 6e60 6060 5c6e 5c6e 6f72 2061 6c74 6572  n```\n\nor alter
-00000670: 6e61 7469 7665 6c79 2c20 6974 2063 616e  natively, it can
-00000680: 2072 6561 6420 6974 2066 726f 6d20 6120   read it from a 
-00000690: 2a2a 6769 7420 7461 672a 2a2c 2073 6574  **git tag**, set
-000006a0: 2077 6974 6820 6120 4769 7448 7562 2072   with a GitHub r
-000006b0: 656c 6561 7365 206f 7220 7769 7468 3a5c  elease or with:\
-000006c0: 6e5c 6e60 6060 636f 6e73 6f6c 655c 6e24  n\n```console\n$
-000006d0: 2067 6974 2074 6167 2030 2e31 2e30 5c6e   git tag 0.1.0\n
-000006e0: 6060 605c 6e5c 6ef0 9f9a a820 436f 6e73  ```\n\n.... Cons
-000006f0: 6964 6572 2074 6869 7320 696e 2061 6c70  ider this in alp
-00000700: 6861 2073 7461 6765 2e20 5265 6164 2074  ha stage. Read t
-00000710: 6865 2077 6172 6e69 6e67 2062 656c 6f77  he warning below
-00000720: 2e5c 6e5c 6e23 2320 5768 656e 2074 6f20  .\n\n## When to 
-00000730: 7573 655c 6e5c 6e54 6869 7320 6973 2075  use\n\nThis is u
-00000740: 7365 6675 6c20 6d61 696e 6c79 2069 6620  seful mainly if 
-00000750: 796f 7520 6172 6520 6275 696c 6469 6e67  you are building
-00000760: 2061 2070 6163 6b61 6765 206c 6962 7261   a package libra
-00000770: 7279 2066 6f72 206f 7468 6572 7320 746f  ry for others to
-00000780: 2075 7365 2061 6e64 2079 6f75 2077 616e   use and you wan
-00000790: 7420 746f 2073 6574 2074 6865 2076 6572  t to set the ver
-000007a0: 7369 6f6e 2069 6e20 6120 706c 6163 6520  sion in a place 
-000007b0: 6469 6666 6572 656e 7420 7468 616e 2060  different than `
-000007c0: 7079 7072 6f6a 6563 742e 746f 6d6c 602c  pyproject.toml`,
-000007d0: 2062 7574 2079 6f75 2073 7469 6c6c 2077   but you still w
-000007e0: 616e 7420 746f 206b 6565 7020 6120 5b73  ant to keep a [s
-000007f0: 696e 676c 6520 736f 7572 6365 206f 6620  ingle source of 
-00000800: 7472 7574 685d 2868 7474 7073 3a2f 2f65  truth](https://e
-00000810: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00000820: 7769 6b69 2f53 696e 676c 655f 736f 7572  wiki/Single_sour
-00000830: 6365 5f6f 665f 7472 7574 6829 2e5c 6e5c  ce_of_truth).\n\
-00000840: 6e49 7420 776f 6e5c 2774 2062 6520 7573  nIt won\'t be us
-00000850: 6566 756c 2069 6e20 6f74 6865 7220 7573  eful in other us
-00000860: 6520 6361 7365 7320 6c69 6b65 206d 616e  e cases like man
-00000870: 6167 696e 6720 6c6f 6361 6c20 6170 7020  aging local app 
-00000880: 656e 7669 726f 6e6d 656e 7473 2077 6974  environments wit
-00000890: 6820 506f 6574 7279 2e5c 6e5c 6e23 2320  h Poetry.\n\n## 
-000008a0: 486f 7720 746f 2075 7365 5c6e 5c6e 4d61  How to use\n\nMa
-000008b0: 6b65 2073 7572 6520 796f 7520 6861 7665  ke sure you have
-000008c0: 2050 6f65 7472 7920 7665 7273 696f 6e20   Poetry version 
-000008d0: 6031 2e32 2e30 6131 6020 6f72 2061 626f  `1.2.0a1` or abo
-000008e0: 7665 2e20 5265 6164 2062 656c 6f77 2066  ve. Read below f
-000008f0: 6f72 2069 6e73 7472 7563 7469 6f6e 7320  or instructions 
-00000900: 746f 2069 6e73 7461 6c6c 2069 7420 6966  to install it if
-00000910: 2079 6f75 2068 6176 656e 5c27 742e 5c6e   you haven\'t.\n
-00000920: 5c6e 2323 2320 496e 7374 616c 6c20 506f  \n### Install Po
-00000930: 6574 7279 2056 6572 7369 6f6e 2050 6c75  etry Version Plu
-00000940: 6769 6e5c 6e5c 6e49 6e73 7461 6c6c 2074  gin\n\nInstall t
-00000950: 6869 7320 706c 7567 696e 2074 6f20 796f  his plugin to yo
-00000960: 7572 2050 6f65 7472 793a 5c6e 5c6e 6060  ur Poetry:\n\n``
-00000970: 6063 6f6e 736f 6c65 5c6e 2420 706f 6574  `console\n$ poet
-00000980: 7279 2070 6c75 6769 6e20 6164 6420 706f  ry plugin add po
-00000990: 6574 7279 2d76 6572 7369 6f6e 2d70 6c75  etry-version-plu
-000009a0: 6769 6e5c 6e5c 6e2d 2d3e 2031 3030 255c  gin\n\n--> 100%\
-000009b0: 6e60 6060 5c6e 5c6e 2323 2320 5365 7420  n```\n\n### Set 
-000009c0: 7665 7273 696f 6e20 696e 2069 6e69 7420  version in init 
-000009d0: 6669 6c65 5c6e 5c6e 5365 7420 796f 7572  file\n\nSet your
-000009e0: 2070 6163 6b61 6765 2076 6572 7369 6f6e   package version
-000009f0: 2069 6e20 796f 7572 2066 696c 6520 605f   in your file `_
-00000a00: 5f69 6e69 745f 5f2e 7079 602c 2066 6f72  _init__.py`, for
-00000a10: 2065 7861 6d70 6c65 3a5c 6e5c 6e60 6060   example:\n\n```
-00000a20: 7079 7468 6f6e 5c6e 6672 6f6d 202e 6d61  python\nfrom .ma
-00000a30: 696e 2069 6d70 6f72 7420 646f 5f61 7765  in import do_awe
-00000a40: 736f 6d65 5f73 7475 6666 2c20 4177 6573  some_stuff, Awes
-00000a50: 6f6d 6543 6c61 7373 5c6e 5c6e 5f5f 7665  omeClass\n\n__ve
-00000a60: 7273 696f 6e5f 5f20 3d20 2230 2e32 2e33  rsion__ = "0.2.3
-00000a70: 225c 6e60 6060 5c6e 5c6e 416e 6420 7468  "\n```\n\nAnd th
-00000a80: 656e 2065 6469 7420 796f 7572 2060 7079  en edit your `py
-00000a90: 7072 6f6a 6563 742e 746f 6d6c 6020 7769  project.toml` wi
-00000aa0: 7468 2061 2073 6563 7469 6f6e 2063 6f6e  th a section con
-00000ab0: 7461 696e 696e 673a 5c6e 5c6e 6060 6074  taining:\n\n```t
-00000ac0: 6f6d 6c5c 6e5b 746f 6f6c 2e70 6f65 7472  oml\n[tool.poetr
-00000ad0: 792d 7665 7273 696f 6e2d 706c 7567 696e  y-version-plugin
-00000ae0: 5d5c 6e73 6f75 7263 6520 3d20 2269 6e69  ]\nsource = "ini
-00000af0: 7422 5c6e 6060 605c 6e5c 6e4e 6578 742c  t"\n```\n\nNext,
-00000b00: 2062 7569 6c64 2079 6f75 7220 7072 6f6a   build your proj
-00000b10: 6563 742c 2069 7420 7769 6c6c 2073 686f  ect, it will sho
-00000b20: 7720 616e 206f 7574 7075 7420 6c69 6b65  w an output like
-00000b30: 3a5c 6e5c 6e60 6060 636f 6e73 6f6c 655c  :\n\n```console\
-00000b40: 6e24 2070 6f65 7472 7920 6275 696c 645c  n$ poetry build\
-00000b50: 6e55 7369 6e67 205f 5f69 6e69 745f 5f2e  nUsing __init__.
-00000b60: 7079 2066 696c 6520 6174 206d 795f 6177  py file at my_aw
-00000b70: 6573 6f6d 655f 7061 636b 6167 652f 5f5f  esome_package/__
-00000b80: 696e 6974 5f5f 2e70 7920 666f 7220 6479  init__.py for dy
-00000b90: 6e61 6d69 6320 7665 7273 696f 6e5c 6e53  namic version\nS
-00000ba0: 6574 7469 6e67 2070 6163 6b61 6765 2064  etting package d
-00000bb0: 796e 616d 6963 2076 6572 7369 6f6e 2074  ynamic version t
-00000bc0: 6f20 5f5f 7665 7273 696f 6e5f 5f20 7661  o __version__ va
-00000bd0: 7269 6162 6c65 2066 726f 6d20 5f5f 696e  riable from __in
-00000be0: 6974 5f5f 2e70 793a 2030 2e31 2e39 5c6e  it__.py: 0.1.9\n
-00000bf0: 4275 696c 6469 6e67 206d 792d 6177 6573  Building my-awes
-00000c00: 6f6d 652d 7061 636b 6167 6520 2830 2e31  ome-package (0.1
-00000c10: 2e39 295c 6e20 202d 2042 7569 6c64 696e  .9)\n  - Buildin
-00000c20: 6720 7364 6973 745c 6e20 202d 2042 7569  g sdist\n  - Bui
-00000c30: 6c74 206d 792d 6177 6573 6f6d 652d 7061  lt my-awesome-pa
-00000c40: 636b 6167 652d 302e 312e 392e 7461 722e  ckage-0.1.9.tar.
-00000c50: 677a 5c6e 2020 2d20 4275 696c 6469 6e67  gz\n  - Building
-00000c60: 2077 6865 656c 5c6e 2020 2d20 4275 696c   wheel\n  - Buil
-00000c70: 7420 6d79 2d61 7765 736f 6d65 2d70 6163  t my-awesome-pac
-00000c80: 6b61 6765 2d30 2e31 2e39 2d70 7933 2d6e  kage-0.1.9-py3-n
-00000c90: 6f6e 652d 616e 792e 7768 6c5c 6e60 6060  one-any.whl\n```
-00000ca0: 5c6e 5c6e 2323 2320 5365 7420 7468 6520  \n\n### Set the 
-00000cb0: 7665 7273 696f 6e20 696e 2061 2047 6974  version in a Git
-00000cc0: 2074 6167 5c6e 5c6e 416c 7465 726e 6174   tag\n\nAlternat
-00000cd0: 6976 656c 792c 2074 6f20 6578 7472 6163  ively, to extrac
-00000ce0: 7420 7468 6520 7665 7273 696f 6e20 746f  t the version to
-00000cf0: 2075 7365 2066 726f 6d20 6120 4769 7420   use from a Git 
-00000d00: 7461 672c 2061 6464 2061 2073 6563 7469  tag, add a secti
-00000d10: 6f6e 3a5c 6e5c 6e60 6060 746f 6d6c 5c6e  on:\n\n```toml\n
-00000d20: 5b74 6f6f 6c2e 706f 6574 7279 2d76 6572  [tool.poetry-ver
-00000d30: 7369 6f6e 2d70 6c75 6769 6e5d 5c6e 736f  sion-plugin]\nso
-00000d40: 7572 6365 203d 2022 6769 742d 7461 6722  urce = "git-tag"
-00000d50: 5c6e 6060 605c 6e5c 6e54 6865 6e20 6372  \n```\n\nThen cr
-00000d60: 6561 7465 2061 2067 6974 2074 6167 2c20  eate a git tag, 
-00000d70: 666f 7220 6578 616d 706c 653a 5c6e 5c6e  for example:\n\n
-00000d80: 6060 6063 6f6e 736f 6c65 5c6e 2420 6769  ```console\n$ gi
-00000d90: 7420 7461 6720 302e 312e 335c 6e60 6060  t tag 0.1.3\n```
-00000da0: 5c6e 5c6e 496e 2074 6869 7320 6361 7365  \n\nIn this case
-00000db0: 2c20 7768 656e 2062 7569 6c64 696e 6720  , when building 
-00000dc0: 796f 7572 2070 726f 6a65 6374 2069 7420  your project it 
-00000dd0: 7769 6c6c 2073 686f 7720 616e 206f 7574  will show an out
-00000de0: 7075 7420 6c69 6b65 3a5c 6e5c 6e60 6060  put like:\n\n```
-00000df0: 636f 6e73 6f6c 655c 6e24 2070 6f65 7472  console\n$ poetr
-00000e00: 7920 6275 696c 645c 6e47 6974 2074 6167  y build\nGit tag
-00000e10: 2066 6f75 6e64 2c20 7365 7474 696e 6720   found, setting 
-00000e20: 6479 6e61 6d69 6320 7665 7273 696f 6e20  dynamic version 
-00000e30: 746f 3a20 302e 312e 335c 6e42 7569 6c64  to: 0.1.3\nBuild
-00000e40: 696e 6720 6d79 2d61 7765 736f 6d65 2d70  ing my-awesome-p
-00000e50: 6163 6b61 6765 2028 302e 312e 3329 5c6e  ackage (0.1.3)\n
-00000e60: 2020 2d20 4275 696c 6469 6e67 2073 6469    - Building sdi
-00000e70: 7374 5c6e 2020 2d20 4275 696c 7420 6d79  st\n  - Built my
-00000e80: 2d61 7765 736f 6d65 2d70 6163 6b61 6765  -awesome-package
-00000e90: 2d30 2e31 2e33 2e74 6172 2e67 7a5c 6e20  -0.1.3.tar.gz\n 
-00000ea0: 202d 2042 7569 6c64 696e 6720 7768 6565   - Building whee
-00000eb0: 6c5c 6e20 202d 2042 7569 6c74 206d 792d  l\n  - Built my-
-00000ec0: 6177 6573 6f6d 652d 7061 636b 6167 652d  awesome-package-
-00000ed0: 302e 312e 332d 7079 332d 6e6f 6e65 2d61  0.1.3-py3-none-a
-00000ee0: 6e79 2e77 686c 5c6e 6060 605c 6e5c 6e23  ny.whl\n```\n\n#
-00000ef0: 2320 5665 7273 696f 6e20 696e 2060 7079  # Version in `py
-00000f00: 7072 6f6a 6563 742e 746f 6d6c 605c 6e5c  project.toml`\n\
-00000f10: 6e43 7572 7265 6e74 6c79 2028 3230 3231  nCurrently (2021
-00000f20: 2d30 352d 3234 2920 506f 6574 7279 2072  -05-24) Poetry r
-00000f30: 6571 7569 7265 7320 6120 6076 6572 7369  equires a `versi
-00000f40: 6f6e 6020 636f 6e66 6967 7572 6174 696f  on` configuratio
-00000f50: 6e20 696e 2074 6865 2060 7079 7072 6f6a  n in the `pyproj
-00000f60: 6563 742e 746f 6d6c 602c 2065 7665 6e20  ect.toml`, even 
-00000f70: 6966 2079 6f75 2075 7365 2074 6869 7320  if you use this 
-00000f80: 706c 7567 696e 2e5c 6e5c 6e57 6865 6e20  plugin.\n\nWhen 
-00000f90: 7573 696e 6720 7468 6973 2070 6c75 6769  using this plugi
-00000fa0: 6e2c 2074 6861 7420 6076 6572 7369 6f6e  n, that `version
-00000fb0: 6020 636f 6e66 6967 2077 6f6e 5c27 7420  ` config won\'t 
-00000fc0: 6265 2075 7365 642c 2062 7574 2050 6f65  be used, but Poe
-00000fd0: 7472 7920 7374 696c 6c20 7265 7175 6972  try still requir
-00000fe0: 6573 2069 7420 746f 2062 6520 7072 6573  es it to be pres
-00000ff0: 656e 7420 696e 2074 6865 2060 7079 7072  ent in the `pypr
-00001000: 6f6a 6563 742e 746f 6d6c 602e 5c6e 5c6e  oject.toml`.\n\n
-00001010: 546f 206d 616b 6520 6974 206d 6f72 6520  To make it more 
-00001020: 6f62 7669 6f75 7320 7468 6174 2079 6f75  obvious that you
-00001030: 2061 7265 206e 6f74 2072 6561 6c6c 7920   are not really 
-00001040: 7573 696e 6720 7468 6174 2060 7665 7273  using that `vers
-00001050: 696f 6e60 2079 6f75 2063 616e 2073 6574  ion` you can set
-00001060: 2069 7420 746f 2060 3060 2e5c 6e5c 6e60   it to `0`.\n\n`
-00001070: 6060 746f 6d6c 5c6e 5b74 6f6f 6c2e 706f  ``toml\n[tool.po
-00001080: 6574 7279 5d5c 6e6e 616d 6520 3d20 226d  etry]\nname = "m
-00001090: 792d 6177 6573 6f6d 652d 7061 636b 6167  y-awesome-packag
-000010a0: 6522 5c6e 7665 7273 696f 6e20 3d20 2230  e"\nversion = "0
-000010b0: 225c 6e60 6060 5c6e 5c6e 5468 6174 2077  "\n```\n\nThat w
-000010c0: 6179 2c20 796f 7520 7769 6c6c 206d 6f72  ay, you will mor
-000010d0: 6520 6561 7369 6c79 206e 6f74 6963 6520  e easily notice 
-000010e0: 6966 2074 6865 2070 6c75 6769 6e20 6973  if the plugin is
-000010f0: 206e 6f74 2069 6e73 7461 6c6c 6564 2c20   not installed, 
-00001100: 6173 2069 7420 7769 6c6c 2073 686f 7720  as it will show 
-00001110: 7468 6174 2079 6f75 2061 7265 2062 7569  that you are bui
-00001120: 6c64 696e 6720 6120 7061 636b 6167 6520  lding a package 
-00001130: 7769 7468 2076 6572 7369 6f6e 2060 3060  with version `0`
-00001140: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-00001150: 6479 6e61 6d69 6320 7665 7273 696f 6e20  dynamic version 
-00001160: 7365 742e 5c6e 5c6e 2323 2041 6e20 6578  set.\n\n## An ex
-00001170: 616d 706c 6520 6070 7970 726f 6a65 6374  ample `pyproject
-00001180: 2e74 6f6d 6c60 5c6e 5c6e 4120 7368 6f72  .toml`\n\nA shor
-00001190: 742c 206d 696e 696d 616c 2065 7861 6d70  t, minimal examp
-000011a0: 6c65 2060 7079 7072 6f6a 6563 742e 746f  le `pyproject.to
-000011b0: 6d6c 6020 636f 756c 6420 6c6f 6f6b 206c  ml` could look l
-000011c0: 696b 653a 5c6e 5c6e 6060 6074 6f6d 6c5c  ike:\n\n```toml\
-000011d0: 6e5b 746f 6f6c 2e70 6f65 7472 795d 5c6e  n[tool.poetry]\n
-000011e0: 6e61 6d65 203d 2022 6d79 2d61 7765 736f  name = "my-aweso
-000011f0: 6d65 2d70 6163 6b61 6765 225c 6e76 6572  me-package"\nver
-00001200: 7369 6f6e 203d 2022 3022 5c6e 6465 7363  sion = "0"\ndesc
-00001210: 7269 7074 696f 6e20 3d20 2222 5c6e 6175  ription = ""\nau
-00001220: 7468 6f72 7320 3d20 5b22 5269 636b 2053  thors = ["Rick S
-00001230: 616e 6368 657a 203c 7269 636b 4072 6963  anchez <rick@ric
-00001240: 6b2d 6369 7461 6465 6c2e 636f 6d3e 225d  k-citadel.com>"]
-00001250: 5c6e 7265 6164 6d65 203d 2022 5245 4144  \nreadme = "READ
-00001260: 4d45 2e6d 6422 5c6e 5c6e 5b74 6f6f 6c2e  ME.md"\n\n[tool.
-00001270: 706f 6574 7279 2e64 6570 656e 6465 6e63  poetry.dependenc
-00001280: 6965 735d 5c6e 7079 7468 6f6e 203d 2022  ies]\npython = "
-00001290: 5e33 2e36 225c 6e5c 6e5b 6275 696c 642d  ^3.6"\n\n[build-
-000012a0: 7379 7374 656d 5d5c 6e72 6571 7569 7265  system]\nrequire
-000012b0: 7320 3d20 5b22 706f 6574 7279 2d63 6f72  s = ["poetry-cor
-000012c0: 6522 5d5c 6e62 7569 6c64 2d62 6163 6b65  e"]\nbuild-backe
-000012d0: 6e64 203d 2022 706f 6574 7279 2e63 6f72  nd = "poetry.cor
-000012e0: 652e 6d61 736f 6e72 792e 6170 6922 5c6e  e.masonry.api"\n
-000012f0: 5c6e 5b74 6f6f 6c2e 706f 6574 7279 2d76  \n[tool.poetry-v
-00001300: 6572 7369 6f6e 2d70 6c75 6769 6e5d 5c6e  ersion-plugin]\n
-00001310: 736f 7572 6365 203d 2022 696e 6974 225c  source = "init"\
-00001320: 6e60 6060 5c6e 5c6e 2323 2057 6879 5c6e  n```\n\n## Why\n
-00001330: 5c6e 4279 2064 6566 6175 6c74 2050 6f65  \nBy default Poe
-00001340: 7472 7920 6578 7065 6374 7320 796f 7520  try expects you 
-00001350: 746f 2073 6574 2079 6f75 7220 7061 636b  to set your pack
-00001360: 6167 6520 7665 7273 696f 6e20 696e 2060  age version in `
-00001370: 7079 7072 6f6a 6563 742e 746f 6d6c 602e  pyproject.toml`.
-00001380: 2041 6e64 2074 6861 7420 776f 756c 6420   And that would 
-00001390: 776f 726b 2069 6e20 6d6f 7374 2063 6173  work in most cas
-000013a0: 6573 2e5c 6e5c 6e42 7574 2069 6d61 6769  es.\n\nBut imagi
-000013b0: 6e65 2079 6f75 2077 616e 7420 746f 2065  ne you want to e
-000013c0: 7870 6f73 6520 7468 6520 7665 7273 696f  xpose the versio
-000013d0: 6e20 6f66 2079 6f75 7220 7061 636b 6167  n of your packag
-000013e0: 6520 696e 2061 2060 5f5f 7665 7273 696f  e in a `__versio
-000013f0: 6e5f 5f60 2076 6172 6961 626c 652c 2073  n__` variable, s
-00001400: 6f20 7468 6174 2079 6f75 7220 7573 6572  o that your user
-00001410: 7320 6361 6e20 646f 2074 6869 6e67 7320  s can do things 
-00001420: 6c69 6b65 3a5c 6e5c 6e60 6060 7079 7468  like:\n\n```pyth
-00001430: 6f6e 5c6e 696d 706f 7274 206d 795f 6177  on\nimport my_aw
-00001440: 6573 6f6d 655f 7061 636b 6167 655c 6e70  esome_package\np
-00001450: 7269 6e74 286d 795f 6177 6573 6f6d 655f  rint(my_awesome_
-00001460: 7061 636b 6167 652e 5f5f 7665 7273 696f  package.__versio
-00001470: 6e5f 5f29 5c6e 6060 605c 6e5c 6e59 6f75  n__)\n```\n\nYou
-00001480: 2063 6f75 6c64 206d 616e 7561 6c6c 7920   could manually 
-00001490: 7772 6974 6520 7468 6520 605f 5f76 6572  write the `__ver
-000014a0: 7369 6f6e 5f5f 6020 7661 7269 6162 6c65  sion__` variable
-000014b0: 2061 6e64 2068 616e 646c 6520 7468 6520   and handle the 
-000014c0: 7379 6e63 6872 6f6e 697a 6174 696f 6e20  synchronization 
-000014d0: 6265 7477 6565 6e20 6974 2061 6e64 2074  between it and t
-000014e0: 6865 2060 7079 7072 6f6a 6563 742e 746f  he `pyproject.to
-000014f0: 6d6c 6020 796f 7572 7365 6c66 2c20 7768  ml` yourself, wh
-00001500: 6963 6820 6973 2076 6572 7920 2a2a 6572  ich is very **er
-00001510: 726f 722d 7072 6f6e 652a 2a2e 5c6e 5c6e  ror-prone**.\n\n
-00001520: 5468 6520 6375 7272 656e 7420 5b6f 6666  The current [off
-00001530: 6963 6961 6c20 7761 7920 6f66 2064 6f69  icial way of doi
-00001540: 6e67 2069 7420 7769 7468 6f75 7420 6475  ng it without du
-00001550: 706c 6963 6174 696e 6720 7468 6520 7661  plicating the va
-00001560: 6c75 655d 2868 7474 7073 3a2f 2f67 6974  lue](https://git
-00001570: 6875 622e 636f 6d2f 7079 7468 6f6e 2d70  hub.com/python-p
-00001580: 6f65 7472 792f 706f 6574 7279 2f70 756c  oetry/poetry/pul
-00001590: 6c2f 3233 3636 2369 7373 7565 636f 6d6d  l/2366#issuecomm
-000015a0: 656e 742d 3635 3234 3138 3039 3429 2069  ent-652418094) i
-000015b0: 7320 7769 7468 2060 696d 706f 7274 6c69  s with `importli
-000015c0: 622e 6d65 7461 6461 7461 602e 5c6e 5c6e  b.metadata`.\n\n
-000015d0: 4275 7420 7468 6174 206d 6f64 756c 6520  But that module 
-000015e0: 6973 206f 6e6c 7920 6176 6169 6c61 626c  is only availabl
-000015f0: 6520 696e 2050 7974 686f 6e20 332e 3820  e in Python 3.8 
-00001600: 616e 6420 6162 6f76 652e 2053 6f2c 2066  and above. So, f
-00001610: 6f72 2050 7974 686f 6e20 332e 3720 616e  or Python 3.7 an
-00001620: 6420 332e 3620 796f 7520 6861 7665 2074  d 3.6 you have t
-00001630: 6f20 696e 7374 616c 6c20 6120 6261 636b  o install a back
-00001640: 706f 7274 2061 7320 6120 6465 7065 6e64  port as a depend
-00001650: 656e 6379 206f 6620 796f 7572 2070 6163  ency of your pac
-00001660: 6b61 6765 3a5c 6e5c 6e60 6060 746f 6d6c  kage:\n\n```toml
-00001670: 5c6e 5b74 6f6f 6c2e 706f 6574 7279 2e64  \n[tool.poetry.d
-00001680: 6570 656e 6465 6e63 6965 735d 5c6e 696d  ependencies]\nim
-00001690: 706f 7274 6c69 622d 6d65 7461 6461 7461  portlib-metadata
-000016a0: 203d 207b 7665 7273 696f 6e20 3d20 225e   = {version = "^
-000016b0: 312e 3022 2c20 7079 7468 6f6e 203d 2022  1.0", python = "
-000016c0: 3c33 2e38 227d 5c6e 6060 605c 6e5c 6e42  <3.8"}\n```\n\nB
-000016d0: 7574 2074 6865 6e2c 2077 6865 6e20 7468  ut then, when th
-000016e0: 6579 2072 656c 6561 7365 2065 6163 6820  ey release each 
-000016f0: 6e65 7720 7665 7273 696f 6e20 6f66 2074  new version of t
-00001700: 6865 2062 6163 6b70 6f72 7420 2863 7572  he backport (cur
-00001710: 7265 6e74 6c79 2060 342e 302e 3160 292c  rently `4.0.1`),
-00001720: 2079 6f75 2068 6176 6520 746f 2075 7064   you have to upd
-00001730: 6174 6520 6974 2028 6f72 206e 6f74 292e  ate it (or not).
-00001740: 2041 6e64 2079 6f75 7220 7573 6572 7320   And your users 
-00001750: 776f 756c 6420 6861 7665 2074 6f20 6d61  would have to ma
-00001760: 6e75 616c 6c79 2068 616e 646c 6520 636f  nually handle co
-00001770: 6e66 6c69 6374 7320 7769 7468 2061 6e79  nflicts with any
-00001780: 206f 7468 6572 2070 6163 6b61 6765 7320   other packages 
-00001790: 7468 6174 2061 6c73 6f20 6465 7065 6e64  that also depend
-000017a0: 206f 6e20 6069 6d70 6f72 746c 6962 2d6d   on `importlib-m
-000017b0: 6574 6164 6174 6160 2c20 7768 6963 6820  etadata`, which 
-000017c0: 636f 756c 6420 6265 206d 756c 7469 706c  could be multipl
-000017d0: 652c 2061 7320 6d61 6e79 2070 6163 6b61  e, as many packa
-000017e0: 6765 7320 636f 756c 6420 6265 2064 6f69  ges could be doi
-000017f0: 6e67 2074 6865 2073 616d 6520 7472 6963  ng the same tric
-00001800: 6b20 2849 5c27 7665 2064 6561 6c74 2077  k (I\'ve dealt w
-00001810: 6974 6820 7468 6174 292e 5c6e 5c6e 5468  ith that).\n\nTh
-00001820: 6520 6f74 6865 7220 6f70 7469 6f6e 2069  e other option i
-00001830: 7320 6e6f 7420 746f 2070 696e 2061 6e79  s not to pin any
-00001840: 2076 6572 7369 6f6e 2072 616e 6765 206f   version range o
-00001850: 6620 796f 7572 2060 696d 706f 7274 6c69  f your `importli
-00001860: 622d 6d65 7461 6461 7461 6020 696e 2079  b-metadata` in y
-00001870: 6f75 7220 6070 7970 726f 6a65 6374 2e74  our `pyproject.t
-00001880: 6f6d 6c60 2061 6e64 2068 6f70 6520 666f  oml` and hope fo
-00001890: 7220 7468 6520 6265 7374 2e5c 6e5c 6e41  r the best.\n\nA
-000018a0: 6e64 2074 6865 6e20 796f 7572 2060 5f5f  nd then your `__
-000018b0: 696e 6974 5f5f 2e70 7960 2077 6f75 6c64  init__.py` would
-000018c0: 2068 6176 6520 746f 2069 6e63 6c75 6465   have to include
-000018d0: 2063 6f64 6520 7573 696e 6720 6974 2c20   code using it, 
-000018e0: 6c69 6b65 3a5c 6e5c 6e60 6060 7079 7468  like:\n\n```pyth
-000018f0: 6f6e 5c6e 2320 4920 646f 6e5c 2774 2077  on\n# I don\'t w
-00001900: 616e 7420 7468 6973 2065 7874 7261 2063  ant this extra c
-00001910: 6f6d 706c 6578 6974 7920 f09f 9894 5c6e  omplexity ....\n
-00001920: 2320 416e 6420 6974 2064 6f65 736e 5c27  # And it doesn\'
-00001930: 7420 776f 726b 2069 6e20 446f 636b 6572  t work in Docker
-00001940: 20f0 9f90 8b5c 6e74 7279 3a5c 6e20 2020   ....\ntry:\n   
-00001950: 2069 6d70 6f72 7420 696d 706f 7274 6c69   import importli
-00001960: 622e 6d65 7461 6461 7461 2061 7320 696d  b.metadata as im
-00001970: 706f 7274 6c69 625f 6d65 7461 6461 7461  portlib_metadata
-00001980: 5c6e 6578 6365 7074 204d 6f64 756c 654e  \nexcept ModuleN
-00001990: 6f74 466f 756e 6445 7272 6f72 3a5c 6e20  otFoundError:\n 
-000019a0: 2020 2069 6d70 6f72 7420 696d 706f 7274     import import
-000019b0: 6c69 625f 6d65 7461 6461 7461 5c6e 5c6e  lib_metadata\n\n
-000019c0: 5f5f 7665 7273 696f 6e5f 5f20 3d20 696d  __version__ = im
-000019d0: 706f 7274 6c69 625f 6d65 7461 6461 7461  portlib_metadata
-000019e0: 2e76 6572 7369 6f6e 285f 5f6e 616d 655f  .version(__name_
-000019f0: 5f29 5c6e 6060 605c 6e5c 6e42 7574 2074  _)\n```\n\nBut t
-00001a00: 6861 7420 636f 6465 2069 7320 6578 7472  hat code is extr
-00001a10: 6120 636f 6d70 6c65 7869 7479 2061 6e64  a complexity and
-00001a20: 206c 6f67 6963 206e 6565 6465 6420 696e   logic needed in
-00001a30: 2079 6f75 7220 636f 6465 2c20 696e 2065   your code, in e
-00001a40: 6163 6820 6f66 2079 6f75 7220 7061 636b  ach of your pack
-00001a50: 6167 6573 2e5c 6e5c 6ef0 9f9a a820 4164  ages.\n\n.... Ad
-00001a60: 6469 7469 6f6e 616c 6c79 2c20 7468 6973  ditionally, this
-00001a70: 206f 6e6c 7920 776f 726b 7320 7768 656e   only works when
-00001a80: 2079 6f75 7220 7061 636b 6167 6520 6973   your package is
-00001a90: 2069 6e73 7461 6c6c 6564 2069 6e20 6120   installed in a 
-00001aa0: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
-00001ab0: 6e74 2e20 4974 2077 6f6e 5c27 7420 776f  nt. It won\'t wo
-00001ac0: 726b 2069 662c 2066 6f72 2065 7861 6d70  rk if, for examp
-00001ad0: 6c65 2c20 796f 7520 7369 6d70 6c79 2070  le, you simply p
-00001ae0: 7574 2079 6f75 7220 636f 6465 2069 6e20  ut your code in 
-00001af0: 6120 2a2a 636f 6e74 6169 6e65 722a 2a2c  a **container**,
-00001b00: 2077 6869 6368 2069 7320 636f 6d6d 6f6e   which is common
-00001b10: 2066 6f72 2077 6562 2061 7070 7320 616e   for web apps an
-00001b20: 6420 6469 7374 7269 6275 7465 6420 7379  d distributed sy
-00001b30: 7374 656d 732e 5c6e 5c6e 2323 2320 486f  stems.\n\n### Ho
-00001b40: 7720 7468 6973 2070 6c75 6769 6e20 736f  w this plugin so
-00001b50: 6c76 6573 2069 745c 6e5c 6e57 6974 6820  lves it\n\nWith 
-00001b60: 7468 6973 2070 6c75 6769 6e2c 2079 6f75  this plugin, you
-00001b70: 7220 7061 636b 6167 6520 646f 6573 6e5c  r package doesn\
-00001b80: 2774 2064 6570 656e 6420 6f6e 2060 696d  't depend on `im
-00001b90: 706f 7274 6c69 622d 6d65 7461 6461 7461  portlib-metadata
-00001ba0: 602c 2073 6f20 796f 7572 2075 7365 7273  `, so your users
-00001bb0: 2077 6f6e 5c27 7420 6e65 6564 2074 6f20   won\'t need to 
-00001bc0: 6861 6e64 6c65 2063 6f6e 666c 6963 7473  handle conflicts
-00001bd0: 206f 7220 6578 7472 6120 6465 7065 6e64   or extra depend
-00001be0: 656e 6369 6573 2e5c 6e5c 6e49 6e73 7465  encies.\n\nInste
-00001bf0: 6164 2c20 796f 7572 2062 7569 6c64 2073  ad, your build s
-00001c00: 7973 7465 6d20 2850 6f65 7472 7929 2069  ystem (Poetry) i
-00001c10: 7320 7768 6174 206e 6565 6473 2074 6f20  s what needs to 
-00001c20: 6861 7665 2074 6869 7320 706c 7567 696e  have this plugin
-00001c30: 2069 6e73 7461 6c6c 6564 2e5c 6e5c 6e54   installed.\n\nT
-00001c40: 6861 7420 6176 6f69 6473 2074 6865 2065  hat avoids the e
-00001c50: 7874 7261 2063 6f64 6520 636f 6d70 6c65  xtra code comple
-00001c60: 7869 7479 206f 6e20 796f 7572 2073 6964  xity on your sid
-00001c70: 652c 2064 6570 656e 6465 6e63 7920 636f  e, dependency co
-00001c80: 6e66 6c69 6374 7320 666f 7220 796f 7572  nflicts for your
-00001c90: 2075 7365 7273 2c20 616e 6420 7375 7070   users, and supp
-00001ca0: 6f72 7420 666f 7220 6f74 6865 7220 7573  ort for other us
-00001cb0: 6520 6361 7365 7320 6c69 6b65 2063 6f64  e cases like cod
-00001cc0: 6520 636f 7069 6564 2064 6972 6563 746c  e copied directl
-00001cd0: 7920 696e 7369 6465 2061 2063 6f6e 7461  y inside a conta
-00001ce0: 696e 6572 2e5c 6e5c 6e23 2323 2056 6572  iner.\n\n### Ver
-00001cf0: 7369 6f6e 2066 726f 6d20 4769 7420 7461  sion from Git ta
-00001d00: 675c 6e5c 6e41 6c74 6572 6e61 7469 7665  g\n\nAlternative
-00001d10: 6c79 2c20 7468 6973 2070 6c75 6769 6e20  ly, this plugin 
-00001d20: 6361 6e20 616c 736f 2065 7874 7261 6374  can also extract
-00001d30: 2074 6865 2076 6572 7369 6f6e 2066 726f   the version fro
-00001d40: 6d20 6120 4769 7420 7461 672e 5c6e 5c6e  m a Git tag.\n\n
-00001d50: 536f 2c20 796f 7520 636f 756c 6420 6f6e  So, you could on
-00001d60: 6c79 2063 7265 6174 6520 6561 6368 2076  ly create each v
-00001d70: 6572 7369 6f6e 2069 6e20 6120 4769 7420  ersion in a Git 
-00001d80: 7461 6720 2866 6f72 2065 7861 6d70 6c65  tag (for example
-00001d90: 2c20 6120 4769 7448 7562 2072 656c 6561  , a GitHub relea
-00001da0: 7365 2920 696e 7374 6561 6420 6f66 2077  se) instead of w
-00001db0: 7269 7469 6e67 2069 7420 696e 2063 6f64  riting it in cod
-00001dc0: 652e 5c6e 5c6e 416e 6420 7468 656e 2062  e.\n\nAnd then b
-00001dd0: 7569 6c64 2074 6865 2070 6163 6b61 6765  uild the package
-00001de0: 206f 6e20 436f 6e74 696e 756f 7573 2049   on Continuous I
-00001df0: 6e74 6567 7261 7469 6f6e 2028 652e 672e  ntegration (e.g.
-00001e00: 2047 6974 4875 6220 4163 7469 6f6e 7329   GitHub Actions)
-00001e10: 2e20 416e 6420 7468 6973 2070 6c75 6769  . And this plugi
-00001e20: 6e20 776f 756c 6420 6765 7420 7468 6520  n would get the 
-00001e30: 7665 7273 696f 6e20 6f66 2074 6865 2070  version of the p
-00001e40: 6163 6b61 6765 2066 726f 6d20 7468 6174  ackage from that
-00001e50: 2047 6974 2074 6167 2e5c 6e5c 6e23 2320   Git tag.\n\n## 
-00001e60: 496e 7374 616c 6c20 506f 6574 7279 2060  Install Poetry `
-00001e70: 312e 322e 3061 3160 5c6e 5c6e 466f 7220  1.2.0a1`\n\nFor 
-00001e80: 7468 6973 2070 6c75 6769 6e20 746f 2077  this plugin to w
-00001e90: 6f72 6b2c 2079 6f75 206e 6565 6420 506f  ork, you need Po
-00001ea0: 6574 7279 2076 6572 7369 6f6e 2060 312e  etry version `1.
-00001eb0: 322e 3061 3160 206f 7220 6162 6f76 652e  2.0a1` or above.
-00001ec0: 5c6e 5c6e 5b50 6f65 7472 7920 6031 2e32  \n\n[Poetry `1.2
-00001ed0: 2e30 6131 6020 7761 7320 7265 6c65 6173  .0a1` was releas
-00001ee0: 6564 2072 6563 656e 746c 795d 2868 7474  ed recently](htt
-00001ef0: 7073 3a2f 2f70 7974 686f 6e2d 706f 6574  ps://python-poet
-00001f00: 7279 2e6f 7267 2f62 6c6f 672f 616e 6e6f  ry.org/blog/anno
-00001f10: 756e 6369 6e67 2d70 6f65 7472 792d 312d  uncing-poetry-1-
-00001f20: 322d 3061 312e 6874 6d6c 292e 5c6e 5c6e  2-0a1.html).\n\n
-00001f30: 5468 6572 655c 2773 2061 2068 6967 6820  There\'s a high 
-00001f40: 6368 616e 6365 2079 6f75 2061 6c72 6561  chance you alrea
-00001f50: 6479 2068 6176 6520 696e 7374 616c 6c65  dy have installe
-00001f60: 6420 506f 6574 7279 2060 312e 312e 7860  d Poetry `1.1.x`
-00001f70: 2e5c 6e5c 6e54 6865 2066 6972 7374 2073  .\n\nThe first s
-00001f80: 7465 7020 6973 2074 6f20 756e 696e 7374  tep is to uninst
-00001f90: 616c 6c20 6974 3a5c 6e5c 6e60 6060 636f  all it:\n\n```co
-00001fa0: 6e73 6f6c 655c 6e24 2063 7572 6c20 2d73  nsole\n$ curl -s
-00001fb0: 534c 2068 7474 7073 3a2f 2f72 6177 2e67  SL https://raw.g
-00001fc0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001fd0: 2e63 6f6d 2f70 7974 686f 6e2d 706f 6574  .com/python-poet
-00001fe0: 7279 2f70 6f65 7472 792f 6d61 7374 6572  ry/poetry/master
-00001ff0: 2f67 6574 2d70 6f65 7472 792e 7079 202d  /get-poetry.py -
-00002000: 4f5c 6e2d 2d3e 2031 3030 255c 6e5c 6e24  O\n--> 100%\n\n$
-00002010: 2070 7974 686f 6e20 6765 742d 706f 6574   python get-poet
-00002020: 7279 2e70 7920 2d2d 756e 696e 7374 616c  ry.py --uninstal
-00002030: 6c5c 6e2d 2d3e 2031 3030 255c 6e60 6060  l\n--> 100%\n```
-00002040: 5c6e 5c6e 416e 6420 7468 656e 2069 6e73  \n\nAnd then ins
-00002050: 7461 6c6c 2074 6865 206e 6577 2050 6f65  tall the new Poe
-00002060: 7472 7920 7769 7468 2074 6865 206e 6577  try with the new
-00002070: 2069 6e73 7461 6c6c 6572 3a5c 6e5c 6e60   installer:\n\n`
-00002080: 6060 636f 6e73 6f6c 655c 6e24 2063 7572  ``console\n$ cur
-00002090: 6c20 2d73 534c 2068 7474 7073 3a2f 2f72  l -sSL https://r
-000020a0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000020b0: 7465 6e74 2e63 6f6d 2f70 7974 686f 6e2d  tent.com/python-
-000020c0: 706f 6574 7279 2f70 6f65 7472 792f 6d61  poetry/poetry/ma
-000020d0: 7374 6572 2f69 6e73 7461 6c6c 2d70 6f65  ster/install-poe
-000020e0: 7472 792e 7079 202d 4f5c 6e2d 2d3e 2031  try.py -O\n--> 1
-000020f0: 3030 255c 6e5c 6e24 2070 7974 686f 6e20  00%\n\n$ python 
-00002100: 696e 7374 616c 6c2d 706f 6574 7279 2e70  install-poetry.p
-00002110: 7920 2d2d 7072 6576 6965 775c 6e2d 2d3e  y --preview\n-->
-00002120: 2031 3030 255c 6e60 6060 5c6e 5c6e f09f   100%\n```\n\n..
-00002130: 948d 204e 6f74 6963 6520 7468 6174 2074  .. Notice that t
-00002140: 6865 206e 6577 2069 6e73 7461 6c6c 6572  he new installer
-00002150: 2066 696c 6520 6973 206e 616d 6564 2060   file is named `
-00002160: 696e 7374 616c 6c2d 706f 6574 7279 2e70  install-poetry.p
-00002170: 7960 2069 6e73 7465 6164 206f 6620 6067  y` instead of `g
-00002180: 6574 2d70 6f65 7472 792e 7079 602e 2041  et-poetry.py`. A
-00002190: 6c73 6f20 6e6f 7469 6365 2074 6861 742c  lso notice that,
-000021a0: 2063 7572 7265 6e74 6c79 2c20 796f 7520   currently, you 
-000021b0: 6e65 6564 2074 6f20 7365 7420 602d 2d70  need to set `--p
-000021c0: 7265 7669 6577 6020 666f 7220 6974 2074  review` for it t
-000021d0: 6f20 696e 7374 616c 6c20 7468 6520 616c  o install the al
-000021e0: 7068 6120 7665 7273 696f 6e20 6031 2e32  pha version `1.2
-000021f0: 2e30 6131 602e 5c6e 5c6e 596f 7520 6361  .0a1`.\n\nYou ca
-00002200: 6e20 6368 6563 6b20 7468 6174 2069 7420  n check that it 
-00002210: 776f 726b 6564 2077 6974 683a 5c6e 5c6e  worked with:\n\n
-00002220: 6060 6063 6f6e 736f 6c65 5c6e 2420 706f  ```console\n$ po
-00002230: 6574 7279 202d 2d76 6572 7369 6f6e 5c6e  etry --version\n
-00002240: 506f 6574 7279 2028 7665 7273 696f 6e20  Poetry (version 
-00002250: 312e 322e 3061 3129 5c6e 6060 605c 6e5c  1.2.0a1)\n```\n\
-00002260: 6e23 2320 5375 7070 6f72 7420 666f 7220  n## Support for 
-00002270: 7665 7273 696f 6e20 696e 2069 6e69 7420  version in init 
-00002280: 6669 6c65 5c6e 5c6e 5768 656e 2075 7369  file\n\nWhen usi
-00002290: 6e67 2061 2060 5f5f 7665 7273 696f 6e5f  ng a `__version_
-000022a0: 5f60 2076 6172 6961 626c 6520 696e 2079  _` variable in y
-000022b0: 6f75 7220 605f 5f69 6e69 745f 5f2e 7079  our `__init__.py
-000022c0: 6020 796f 7520 6361 6e20 6861 7665 206d  ` you can have m
-000022d0: 6f72 6520 6c6f 6769 6320 696e 2074 6861  ore logic in tha
-000022e0: 7420 6669 6c65 2c20 696d 706f 7274 206d  t file, import m
-000022f0: 6f64 756c 6573 2c20 616e 6420 646f 206d  odules, and do m
-00002300: 6f72 6520 7468 696e 6773 2061 626f 7665  ore things above
-00002310: 2061 6e64 2062 656c 6f77 2074 6865 2064   and below the d
-00002320: 6563 6c61 7261 7469 6f6e 206f 6620 7468  eclaration of th
-00002330: 6174 2076 6172 6961 626c 652e 5c6e 5c6e  at variable.\n\n
-00002340: 4275 7420 7468 6520 7661 6c75 6520 6861  But the value ha
-00002350: 7320 746f 2062 6520 6120 6c69 7465 7261  s to be a litera
-00002360: 6c20 7374 7269 6e67 2c20 6c69 6b65 3a5c  l string, like:\
-00002370: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 5f5f  n\n```python\n__
-00002380: 5f76 6572 7369 6f6e 5f5f 5f20 3d20 2230  _version___ = "0
-00002390: 2e32 2e30 225c 6e60 6060 5c6e 5c6e 2e2e  .2.0"\n```\n\n..
-000023a0: 2e69 6e73 7465 6164 206f 6620 6361 6c6c  .instead of call
-000023b0: 696e 6720 6120 6675 6e63 7469 6f6e 206f  ing a function o
-000023c0: 7220 736f 6d65 7468 696e 6720 7369 6d69  r something simi
-000023d0: 6c61 722e 5c6e 5c6e 416e 6420 7468 6520  lar.\n\nAnd the 
-000023e0: 7661 7269 6162 6c65 2068 6173 2074 6f20  variable has to 
-000023f0: 6265 2069 6e20 7468 6520 746f 702d 6c65  be in the top-le
-00002400: 7665 6c2c 2073 6f20 6974 2063 616e 5c27  vel, so it can\'
-00002410: 7420 6265 2069 6e73 6964 6520 616e 2060  t be inside an `
-00002420: 6966 6020 7374 6174 656d 656e 7420 6f72  if` statement or
-00002430: 2073 696d 696c 6172 2e5c 6e5c 6e54 6869   similar.\n\nThi
-00002440: 7320 6973 2061 6c6c 2066 696e 6520 616e  s is all fine an
-00002450: 6420 7375 7070 6f72 7465 6420 696e 2079  d supported in y
-00002460: 6f75 7220 605f 5f69 6e69 745f 5f2e 7079  our `__init__.py
-00002470: 603a 5c6e 5c6e 6060 6070 7974 686f 6e5c  `:\n\n```python\
-00002480: 6e23 205f 5f69 6e69 745f 5f2e 7079 5c6e  n# __init__.py\n
-00002490: 5c6e 2320 5468 6973 2069 7320 616c 6c20  \n# This is all 
-000024a0: 7661 6c69 6420 f09f 918d e29c 855c 6e5c  valid .......\n\
-000024b0: 6e66 726f 6d20 2e6d 6169 6e20 696d 706f  nfrom .main impo
-000024c0: 7274 2064 6f5f 6177 6573 6f6d 655f 7374  rt do_awesome_st
-000024d0: 7566 662c 2041 7765 736f 6d65 436c 6173  uff, AwesomeClas
-000024e0: 735c 6e5c 6e61 7765 736f 6d65 203d 2041  s\n\nawesome = A
-000024f0: 7765 736f 6d65 436c 6173 7328 295c 6e5c  wesomeClass()\n\
-00002500: 6e23 2053 6f6d 6520 636f 6d6d 656e 7420  n# Some comment 
-00002510: 6578 706c 6169 6e69 6e67 2077 6879 2074  explaining why t
-00002520: 6869 7320 6973 2063 6f6d 6d65 6e74 6564  his is commented
-00002530: 206f 7574 5c6e 2320 5f5f 7665 7273 696f   out\n# __versio
-00002540: 6e5f 5f20 3d20 2231 2e30 2e30 225c 6e5c  n__ = "1.0.0"\n\
-00002550: 6e5f 5f76 6572 7369 6f6e 5f5f 203d 2022  n__version__ = "
-00002560: 302e 322e 3322 5c6e 5c6e 6966 205f 5f6e  0.2.3"\n\nif __n
-00002570: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
-00002580: 5f5f 223a 5c6e 2020 2020 6177 6573 6f6d  __":\n    awesom
-00002590: 652e 7275 6e28 295c 6e60 6060 5c6e 5c6e  e.run()\n```\n\n
-000025a0: 5468 6973 2065 7861 6d70 6c65 2069 7320  This example is 
-000025b0: 616c 6c20 7661 6c69 6420 616e 6420 7375  all valid and su
-000025c0: 7070 6f72 7465 642c 2061 6e64 2069 7420  pported, and it 
-000025d0: 696e 636c 7564 6573 3a5c 6e5c 6e2a 2049  includes:\n\n* I
-000025e0: 6d70 6f72 7473 5c6e 2a20 4f74 6865 7220  mports\n* Other 
-000025f0: 6f62 6a65 6374 7320 616e 6420 7661 7269  objects and vari
-00002600: 6162 6c65 735c 6e2a 2043 6f6d 6d65 6e74  ables\n* Comment
-00002610: 735c 6e2a 2054 6865 2073 616d 6520 7374  s\n* The same st
-00002620: 7269 6e67 2060 5f5f 7665 7273 696f 6e5f  ring `__version_
-00002630: 5f60 2069 6e73 6964 6520 6120 636f 6d6d  _` inside a comm
-00002640: 656e 745c 6e2a 2049 6620 626c 6f63 6b73  ent\n* If blocks
-00002650: 2061 726f 756e 645c 6e5c 6e2d 2d2d 5c6e   around\n\n---\n
-00002660: 5c6e 4275 7420 7468 6973 2069 7320 6e6f  \nBut this is no
-00002670: 7420 7375 7070 6f72 7465 643a 5c6e 5c6e  t supported:\n\n
-00002680: 6060 6070 7974 686f 6e5c 6e23 20f0 9f9a  ```python\n# ...
-00002690: a820 4e6f 7420 7375 7070 6f72 7465 645c  . Not supported\
-000026a0: 6e5c 6e69 6620 3220 3d3d 2032 3a5c 6e20  n\nif 2 == 2:\n 
-000026b0: 2020 205f 5f76 6572 7369 6f6e 5f5f 203d     __version__ =
-000026c0: 2022 302e 312e 305c 6e60 6060 5c6e 5c6e   "0.1.0\n```\n\n
-000026d0: 416e 6420 7468 6973 2069 7320 6e6f 7420  And this is not 
-000026e0: 7375 7070 6f72 7465 643a 5c6e 5c6e 6060  supported:\n\n``
-000026f0: 6070 7974 686f 6e5c 6e23 20f0 9f9a a820  `python\n# .... 
-00002700: 4e6f 7420 7375 7070 6f72 7465 645c 6e5c  Not supported\n\
-00002710: 6e64 6566 2067 6574 5f76 6572 7369 6f6e  ndef get_version
-00002720: 2829 3a5c 6e20 2020 2072 6574 7572 6e20  ():\n    return 
-00002730: 2230 2e32 2e30 225c 6e5c 6e5f 5f76 6572  "0.2.0"\n\n__ver
-00002740: 7369 6f6e 5f5f 203d 2067 6574 5f76 6572  sion__ = get_ver
-00002750: 7369 6f6e 2829 5c6e 6060 605c 6e5c 6e23  sion()\n```\n\n#
-00002760: 2320 486f 7720 7468 6520 706c 7567 696e  # How the plugin
-00002770: 2077 6f72 6b73 5c6e 5c6e 506f 6574 7279   works\n\nPoetry
-00002780: 2072 756e 7320 7468 6520 706c 7567 696e   runs the plugin
-00002790: 2077 6865 6e20 6275 696c 6469 6e67 2061   when building a
-000027a0: 2070 6163 6b61 6765 2c20 616e 6420 6974   package, and it
-000027b0: 2073 6574 7320 7468 6520 7665 7273 696f   sets the versio
-000027c0: 6e20 7269 6768 7420 6265 666f 7265 2063  n right before c
-000027d0: 7265 6174 696e 6720 7468 6520 2270 6163  reating the "pac
-000027e0: 6b61 6765 2064 6973 7472 6962 7574 6162  kage distributab
-000027f0: 6c65 2220 2865 2e67 2e20 7468 6520 7768  le" (e.g. the wh
-00002800: 6565 6c29 2e5c 6e5c 6e23 2323 2048 6f77  eel).\n\n### How
-00002810: 2074 6865 2076 6572 7369 6f6e 2076 6172   the version var
-00002820: 6961 626c 6520 776f 726b 735c 6e5c 6e49  iable works\n\nI
-00002830: 6620 796f 7520 6861 7665 2061 2070 6163  f you have a pac
-00002840: 6b61 6765 2028 6120 7369 6e67 6c65 2070  kage (a single p
-00002850: 6163 6b61 6765 2920 6465 636c 6172 6564  ackage) declared
-00002860: 2069 6e20 7468 6520 6070 6163 6b61 6765   in the `package
-00002870: 7360 2063 6f6e 6669 6720 696e 2079 6f75  s` config in you
-00002880: 7220 6070 7970 726f 6a65 6374 2e74 6f6d  r `pyproject.tom
-00002890: 6c60 2c20 7468 6520 706c 7567 696e 2077  l`, the plugin w
-000028a0: 696c 6c20 7573 6520 7468 6174 2070 6163  ill use that pac
-000028b0: 6b61 6765 5c27 7320 605f 5f69 6e69 745f  kage\'s `__init_
-000028c0: 5f2e 7079 6020 746f 2066 696e 6420 7468  _.py` to find th
-000028d0: 6520 605f 5f76 6572 7369 6f6e 5f5f 6020  e `__version__` 
-000028e0: 7661 7269 6162 6c65 2e5c 6e5c 6e49 6620  variable.\n\nIf 
-000028f0: 796f 7520 646f 6e5c 2774 2068 6176 6520  you don\'t have 
-00002900: 616e 7920 6070 6163 6b61 6765 7360 2063  any `packages` c
-00002910: 6f6e 6669 672c 2074 6865 2070 6c75 6769  onfig, the plugi
-00002920: 6e20 7769 6c6c 2061 7373 756d 6520 7468  n will assume th
-00002930: 6174 2079 6f75 2068 6176 6520 6120 7369  at you have a si
-00002940: 6e67 6c65 2070 6163 6b61 6765 206e 616d  ngle package nam
-00002950: 6564 2061 7320 796f 7572 2070 726f 6a65  ed as your proje
-00002960: 6374 2c20 6275 7420 696e 2074 6865 206d  ct, but in the m
-00002970: 6f64 756c 6520 7665 7273 696f 6e20 2863  odule version (c
-00002980: 6861 6e67 696e 6720 602d 6020 666f 7220  hanging `-` for 
-00002990: 605f 6029 2e20 536f 2c20 6966 2079 6f75  `_`). So, if you
-000029a0: 7220 7061 636b 6167 6520 6973 2060 6d79  r package is `my
-000029b0: 2d61 7765 736f 6d65 2d70 726f 6a65 6374  -awesome-project
-000029c0: 602c 2074 6865 2070 6c75 6769 6e20 7769  `, the plugin wi
-000029d0: 6c6c 2075 7365 2074 6865 2066 696c 6520  ll use the file 
-000029e0: 6174 2060 6d79 5f61 7765 736f 6d65 5f70  at `my_awesome_p
-000029f0: 726f 6a65 6374 2f5f 5f69 6e69 745f 5f2e  roject/__init__.
-00002a00: 7079 6020 746f 2066 696e 6420 7468 6520  py` to find the 
-00002a10: 605f 5f76 6572 7369 6f6e 5f5f 6020 7661  `__version__` va
-00002a20: 7269 6162 6c65 2e5c 6e5c 6e54 6869 7320  riable.\n\nThis 
-00002a30: 6669 6c65 2073 7472 7563 7475 7265 2069  file structure i
-00002a40: 7320 7468 6520 6465 6661 756c 7420 6966  s the default if
-00002a50: 2079 6f75 2063 7265 6174 6520 6120 6e65   you create a ne
-00002a60: 7720 7072 6f6a 6563 7420 7769 7468 2074  w project with t
-00002a70: 6865 2063 6f6d 6d61 6e64 2060 706f 6574  he command `poet
-00002a80: 7279 206e 6577 602c 2073 6f20 6974 2073  ry new`, so it s
-00002a90: 686f 756c 6420 6a75 7374 2077 6f72 6b20  hould just work 
-00002aa0: 6173 2065 7870 6563 7465 642e 20e2 9ca8  as expected. ...
-00002ab0: 5c6e 5c6e 5468 6520 7761 7920 7468 6520  \n\nThe way the 
-00002ac0: 706c 7567 696e 2077 6f72 6b73 2069 6e74  plugin works int
-00002ad0: 6572 6e61 6c6c 7920 6973 2062 7920 7061  ernally is by pa
-00002ae0: 7273 696e 6720 7468 6520 605f 5f69 6e69  rsing the `__ini
-00002af0: 745f 5f2e 7079 6020 6669 6c65 2e20 5265  t__.py` file. Re
-00002b00: 6164 696e 6720 7468 6520 5079 7468 6f6e  ading the Python
-00002b10: 5c27 7320 2241 6273 7472 6163 7420 5379  \'s "Abstract Sy
-00002b20: 6e74 6178 2054 7265 6522 2075 7369 6e67  ntax Tree" using
-00002b30: 2074 6865 2060 6173 7460 2073 7461 6e64   the `ast` stand
-00002b40: 6172 6420 6d6f 6475 6c65 2061 6e64 2065  ard module and e
-00002b50: 7874 7261 6374 696e 6720 7468 6520 6c69  xtracting the li
-00002b60: 7465 7261 6c20 7661 6c75 6520 6f66 2074  teral value of t
-00002b70: 6865 2073 7472 696e 672e 2053 6f2c 2069  he string. So, i
-00002b80: 7420 646f 6573 6e5c 2774 2065 7865 6375  t doesn\'t execu
-00002b90: 7465 2074 6865 2063 6f64 6520 696e 2060  te the code in `
-00002ba0: 5f5f 696e 6974 5f5f 2e70 7960 2c20 6974  __init__.py`, it
-00002bb0: 206f 6e6c 7920 7265 6164 7320 6974 2061   only reads it a
-00002bc0: 7320 5079 7468 6f6e 2063 6f64 652e 5c6e  s Python code.\n
-00002bd0: 5c6e 5468 6520 706c 7567 696e 2064 6f65  \nThe plugin doe
-00002be0: 736e 5c27 7420 7472 7920 746f 2069 6d70  sn\'t try to imp
-00002bf0: 6f72 7420 616e 6420 6578 6563 7574 6520  ort and execute 
-00002c00: 7468 6174 2060 5f5f 696e 6974 5f5f 2e70  that `__init__.p
-00002c10: 7960 2066 696c 6520 6265 6361 7573 6520  y` file because 
-00002c20: 7468 6174 2063 6f75 6c64 2072 6571 7569  that could requi
-00002c30: 7265 2065 7874 7261 2063 6f6d 7075 7461  re extra computa
-00002c40: 7469 6f6e 2c20 6578 7465 726e 616c 2064  tion, external d
-00002c50: 6570 656e 6465 6e63 6965 732c 2065 7463  ependencies, etc
-00002c60: 2e20 416e 6420 6974 2064 6f65 736e 5c27  . And it doesn\'
-00002c70: 7420 7472 7920 746f 2065 7874 7261 6374  t try to extract
-00002c80: 2074 6865 2060 5f5f 7665 7273 696f 6e5f   the `__version_
-00002c90: 5f60 2077 6974 6820 7265 6775 6c61 7220  _` with regular 
-00002ca0: 6578 7072 6573 7369 6f6e 732c 2061 7320  expressions, as 
-00002cb0: 7468 6174 2077 6f75 6c64 2062 6520 7072  that would be pr
-00002cc0: 6f6e 6520 746f 2065 7272 6f72 7320 6966  one to errors if
-00002cd0: 2c20 666f 7220 6578 616d 706c 652c 2074  , for example, t
-00002ce0: 6865 7265 2077 6173 2073 6f6d 6520 6f74  here was some ot
-00002cf0: 6865 7220 605f 5f76 6572 7369 6f6e 5f5f  her `__version__
-00002d00: 6020 736f 6d65 7768 6572 6520 696e 2074  ` somewhere in t
-00002d10: 6865 2063 6f64 652c 2069 6e20 6120 636f  he code, in a co
-00002d20: 6d6d 656e 7420 6f72 2069 6e73 6964 6520  mment or inside 
-00002d30: 6120 7374 7269 6e67 2e5c 6e5c 6e23 2320  a string.\n\n## 
-00002d40: 5761 726e 696e 675c 6e5c 6ef0 9f9a a820  Warning\n\n.... 
-00002d50: 436f 6e73 6964 6572 2074 6869 7320 696e  Consider this in
-00002d60: 2061 6c70 6861 2073 7461 6765 2e20 506f   alpha stage. Po
-00002d70: 6574 7279 2060 312e 322e 3061 3160 2077  etry `1.2.0a1` w
-00002d80: 6974 6820 7375 7070 6f72 7420 666f 7220  ith support for 
-00002d90: 706c 7567 696e 7320 7761 7320 7265 6c65  plugins was rele
-00002da0: 6173 6564 206f 6e20 3230 3231 2d30 352d  ased on 2021-05-
-00002db0: 3231 2c20 4920 7374 6172 7465 6420 7772  21, I started wr
-00002dc0: 6974 696e 6720 7468 6973 2070 6c75 6769  iting this plugi
-00002dd0: 6e20 3320 6461 7973 206c 6174 6572 2c20  n 3 days later, 
-00002de0: 6f6e 2032 3032 312d 3035 2d32 342e 5c6e  on 2021-05-24.\n
-00002df0: 5c6e 5468 696e 6773 206d 6967 6874 2062  \nThings might b
-00002e00: 7265 616b 2069 6e20 506f 6574 7279 206f  reak in Poetry o
-00002e10: 7220 696e 2074 6869 7320 706c 7567 696e  r in this plugin
-00002e20: 2e20 536f 2c20 706c 6561 7365 2074 7279  . So, please try
-00002e30: 2069 7420 616e 6420 7465 7374 2069 7420   it and test it 
-00002e40: 7665 7279 2063 6172 6566 756c 6c79 2062  very carefully b
-00002e50: 6566 6f72 6520 6675 6c6c 7920 6164 6f70  efore fully adop
-00002e60: 7469 6e67 2069 7420 666f 7220 6465 6c69  ting it for deli
-00002e70: 6361 7465 2073 7973 7465 6d73 2e5c 6e5c  cate systems.\n\
-00002e80: 6e54 6865 2077 6179 2069 7420 776f 726b  nThe way it work
-00002e90: 7320 6d69 6768 7420 6368 616e 6765 2c20  s might change, 
-00002ea0: 616e 6420 7468 6520 7370 6563 6966 6963  and the specific
-00002eb0: 2063 6f6e 6669 6775 7261 7469 6f6e 206d   configuration m
-00002ec0: 6967 6874 2063 6861 6e67 652e 5c6e 5c6e  ight change.\n\n
-00002ed0: 416c 736f 2c20 6966 2079 6f75 2064 6f6e  Also, if you don
-00002ee0: 5c27 7420 6669 6e64 2069 6e74 7569 7469  \'t find intuiti
-00002ef0: 7665 2074 6865 2073 6563 7469 6f6e 733a  ve the sections:
-00002f00: 5c6e 5c6e 6060 6074 6f6d 6c5c 6e5b 746f  \n\n```toml\n[to
-00002f10: 6f6c 2e70 6f65 7472 792d 7665 7273 696f  ol.poetry-versio
-00002f20: 6e2d 706c 7567 696e 5d5c 6e73 6f75 7263  n-plugin]\nsourc
-00002f30: 6520 3d20 2269 6e69 7422 5c6e 6060 605c  e = "init"\n```\
-00002f40: 6e5c 6e61 6e64 5c6e 5c6e 6060 6074 6f6d  n\nand\n\n```tom
-00002f50: 6c5c 6e5b 746f 6f6c 2e70 6f65 7472 792d  l\n[tool.poetry-
-00002f60: 7665 7273 696f 6e2d 706c 7567 696e 5d5c  version-plugin]\
-00002f70: 6e73 6f75 7263 6520 3d20 2267 6974 2d74  nsource = "git-t
-00002f80: 6167 225c 6e60 6060 5c6e 5c6e 6c65 7420  ag"\n```\n\nlet 
-00002f90: 6d65 206b 6e6f 7720 7768 6174 2061 6c74  me know what alt
-00002fa0: 6572 6e61 7469 7665 2063 6f6e 6669 6775  ernative configu
-00002fb0: 7261 7469 6f6e 2077 6f75 6c64 206d 616b  ration would mak
-00002fc0: 6520 6d6f 7265 2073 656e 7365 2061 6e64  e more sense and
-00002fd0: 2062 6520 6d6f 7265 2069 6e74 7569 7469   be more intuiti
-00002fe0: 7665 2074 6f20 796f 752e 5c6e 5c6e f09f  ve to you.\n\n..
-00002ff0: 918d 2054 6865 2067 6f6f 6420 6e65 7773  .. The good news
-00003000: 2069 732c 2061 7373 756d 696e 6720 796f   is, assuming yo
-00003010: 7520 6172 6520 6275 696c 6469 6e67 2070  u are building p
-00003020: 6163 6b61 6765 7320 746f 2074 6865 6e20  ackages to then 
-00003030: 7570 6c6f 6164 2074 6865 6d20 746f 2050  upload them to P
-00003040: 7950 4920 666f 7220 796f 7572 2075 7365  yPI for your use
-00003050: 7273 2074 6f20 646f 776e 6c6f 6164 2061  rs to download a
-00003060: 6e64 2075 7365 2074 6865 6d2c 2074 6865  nd use them, the
-00003070: 202a 2a77 6f72 7374 2074 6861 7420 636f   **worst that co
-00003080: 756c 6420 6861 7070 656e 2a2a 2069 6620  uld happen** if 
-00003090: 736f 6d65 7468 696e 6720 6272 6f6b 6520  something broke 
-000030a0: 6973 2074 6861 7420 796f 7520 776f 756c  is that you woul
-000030b0: 646e 5c27 7420 6265 2061 626c 6520 746f  dn\'t be able to
-000030c0: 2062 7569 6c64 2061 206e 6577 2076 6572   build a new ver
-000030d0: 7369 6f6e 2075 6e74 696c 2073 6f6d 6574  sion until somet
-000030e0: 6869 6e67 2069 7320 6669 7865 6420 6f72  hing is fixed or
-000030f0: 2063 6861 6e67 6564 2e20 4275 7420 796f   changed. But yo
-00003100: 7572 2075 7365 7273 2073 686f 756c 646e  ur users shouldn
-00003110: 5c27 7420 6265 2061 6666 6563 7465 6420  \'t be affected 
-00003120: 696e 2061 6e79 2077 6179 2e5c 6e5c 6e23  in any way.\n\n#
-00003130: 2320 5265 6c65 6173 6520 4e6f 7465 735c  # Release Notes\
-00003140: 6e5c 6e23 2323 204c 6174 6573 7420 4368  n\n### Latest Ch
-00003150: 616e 6765 735c 6e5c 6e23 2323 2030 2e31  anges\n\n### 0.1
-00003160: 2e33 5c6e 5c6e 2a20 e29c a820 496d 7072  .3\n\n* ... Impr
-00003170: 6f76 6520 6c6f 6773 2c20 7072 6566 6978  ove logs, prefix
-00003180: 2077 6974 6820 706c 7567 696e 206e 616d   with plugin nam
-00003190: 652e 2050 5220 5b23 365d 2868 7474 7073  e. PR [#6](https
-000031a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7469  ://github.com/ti
-000031b0: 616e 676f 6c6f 2f70 6f65 7472 792d 7665  angolo/poetry-ve
-000031c0: 7273 696f 6e2d 706c 7567 696e 2f70 756c  rsion-plugin/pul
-000031d0: 6c2f 3629 2062 7920 5b40 7469 616e 676f  l/6) by [@tiango
-000031e0: 6c6f 5d28 6874 7470 733a 2f2f 6769 7468  lo](https://gith
-000031f0: 7562 2e63 6f6d 2f74 6961 6e67 6f6c 6f29  ub.com/tiangolo)
-00003200: 2e5c 6e2a 20f0 9f94 a720 5570 6461 7465  .\n* .... Update
-00003210: 2070 7970 726f 6a65 6374 206d 6574 6164   pyproject metad
-00003220: 6174 612e 2050 5220 5b23 355d 2868 7474  ata. PR [#5](htt
-00003230: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003240: 7469 616e 676f 6c6f 2f70 6f65 7472 792d  tiangolo/poetry-
-00003250: 7665 7273 696f 6e2d 706c 7567 696e 2f70  version-plugin/p
-00003260: 756c 6c2f 3529 2062 7920 5b40 7469 616e  ull/5) by [@tian
-00003270: 676f 6c6f 5d28 6874 7470 733a 2f2f 6769  golo](https://gi
-00003280: 7468 7562 2e63 6f6d 2f74 6961 6e67 6f6c  thub.com/tiangol
-00003290: 6f29 2e5c 6e2a 20e2 9c85 2046 6978 2063  o).\n* ... Fix c
-000032a0: 6f76 6572 6167 652e 2050 5220 5b23 345d  overage. PR [#4]
-000032b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000032c0: 636f 6d2f 7469 616e 676f 6c6f 2f70 6f65  com/tiangolo/poe
-000032d0: 7472 792d 7665 7273 696f 6e2d 706c 7567  try-version-plug
-000032e0: 696e 2f70 756c 6c2f 3429 2062 7920 5b40  in/pull/4) by [@
-000032f0: 7469 616e 676f 6c6f 5d28 6874 7470 733a  tiangolo](https:
-00003300: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6961  //github.com/tia
-00003310: 6e67 6f6c 6f29 2e5c 6e2a 20f0 9f93 9d20  ngolo).\n* .... 
-00003320: 496d 7072 6f76 6520 646f 6373 2e20 5052  Improve docs. PR
-00003330: 205b 2333 5d28 6874 7470 733a 2f2f 6769   [#3](https://gi
-00003340: 7468 7562 2e63 6f6d 2f74 6961 6e67 6f6c  thub.com/tiangol
-00003350: 6f2f 706f 6574 7279 2d76 6572 7369 6f6e  o/poetry-version
-00003360: 2d70 6c75 6769 6e2f 7075 6c6c 2f33 2920  -plugin/pull/3) 
-00003370: 6279 205b 4074 6961 6e67 6f6c 6f5d 2868  by [@tiangolo](h
-00003380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003390: 6d2f 7469 616e 676f 6c6f 292e 5c6e 2a20  m/tiangolo).\n* 
-000033a0: f09f 909b 2046 6978 2074 6573 7473 2066  .... Fix tests f
-000033b0: 6f72 2043 492e 2050 5220 5b23 315d 2868  or CI. PR [#1](h
-000033c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000033d0: 6d2f 7469 616e 676f 6c6f 2f70 6f65 7472  m/tiangolo/poetr
-000033e0: 792d 7665 7273 696f 6e2d 706c 7567 696e  y-version-plugin
-000033f0: 2f70 756c 6c2f 3129 2062 7920 5b40 7469  /pull/1) by [@ti
-00003400: 616e 676f 6c6f 5d28 6874 7470 733a 2f2f  angolo](https://
-00003410: 6769 7468 7562 2e63 6f6d 2f74 6961 6e67  github.com/tiang
-00003420: 6f6c 6f29 2e5c 6e2a 20f0 9f91 b720 4669  olo).\n* .... Fi
-00003430: 7820 4c61 7465 7374 2043 6861 6e67 6573  x Latest Changes
-00003440: 2061 6374 696f 6e2c 2073 6574 2062 7261   action, set bra
-00003450: 6e63 6820 746f 206d 6169 6e2e 2050 5220  nch to main. PR 
-00003460: 5b23 325d 2868 7474 7073 3a2f 2f67 6974  [#2](https://git
-00003470: 6875 622e 636f 6d2f 7469 616e 676f 6c6f  hub.com/tiangolo
-00003480: 2f70 6f65 7472 792d 7665 7273 696f 6e2d  /poetry-version-
-00003490: 706c 7567 696e 2f70 756c 6c2f 3229 2062  plugin/pull/2) b
-000034a0: 7920 5b40 7469 616e 676f 6c6f 5d28 6874  y [@tiangolo](ht
-000034b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000034c0: 2f74 6961 6e67 6f6c 6f29 2e5c 6e5c 6e23  /tiangolo).\n\n#
-000034d0: 2320 4c69 6365 6e73 655c 6e5c 6e54 6869  # License\n\nThi
-000034e0: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
-000034f0: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
-00003500: 7465 726d 7320 6f66 2074 6865 204d 4954  terms of the MIT
-00003510: 206c 6963 656e 7365 2e5c 6e27 2c0a 2020   license.\n',.  
-00003520: 2020 2761 7574 686f 7227 3a20 2753 6562    'author': 'Seb
-00003530: 6173 7469 c3a1 6e20 5261 6dc3 ad72 657a  asti..n Ram..rez
-00003540: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
-00003550: 6d61 696c 273a 2027 7469 616e 676f 6c6f  mail': 'tiangolo
-00003560: 4067 6d61 696c 2e63 6f6d 272c 0a20 2020  @gmail.com',.   
-00003570: 2027 6d61 696e 7461 696e 6572 273a 204e   'maintainer': N
-00003580: 6f6e 652c 0a20 2020 2027 6d61 696e 7461  one,.    'mainta
-00003590: 696e 6572 5f65 6d61 696c 273a 204e 6f6e  iner_email': Non
-000035a0: 652c 0a20 2020 2027 7572 6c27 3a20 2768  e,.    'url': 'h
-000035b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000035c0: 6d2f 7469 616e 676f 6c6f 2f70 6f65 7472  m/tiangolo/poetr
-000035d0: 792d 7665 7273 696f 6e2d 706c 7567 696e  y-version-plugin
-000035e0: 272c 0a20 2020 2027 7061 636b 6167 6573  ',.    'packages
-000035f0: 273a 2070 6163 6b61 6765 732c 0a20 2020  ': packages,.   
-00003600: 2027 7061 636b 6167 655f 6461 7461 273a   'package_data':
-00003610: 2070 6163 6b61 6765 5f64 6174 612c 0a20   package_data,. 
-00003620: 2020 2027 696e 7374 616c 6c5f 7265 7175     'install_requ
-00003630: 6972 6573 273a 2069 6e73 7461 6c6c 5f72  ires': install_r
-00003640: 6571 7569 7265 732c 0a20 2020 2027 656e  equires,.    'en
-00003650: 7472 795f 706f 696e 7473 273a 2065 6e74  try_points': ent
-00003660: 7279 5f70 6f69 6e74 732c 0a20 2020 2027  ry_points,.    '
-00003670: 7079 7468 6f6e 5f72 6571 7569 7265 7327  python_requires'
-00003680: 3a20 273e 3d33 2e36 2c3c 342e 3027 2c0a  : '>=3.6,<4.0',.
-00003690: 7d0a 0a0a 7365 7475 7028 2a2a 7365 7475  }...setup(**setu
-000036a0: 705f 6b77 6172 6773 290a                 p_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 706f 6574  : 2.1.Name: poet
+00000020: 7279 2d76 6572 7369 6f6e 2d70 6c75 6769  ry-version-plugi
+00000030: 6e0a 5665 7273 696f 6e3a 2030 2e32 2e30  n.Version: 0.2.0
+00000040: 0a53 756d 6d61 7279 3a20 506f 6574 7279  .Summary: Poetry
+00000050: 2070 6c75 6769 6e20 666f 7220 6479 6e61   plugin for dyna
+00000060: 6d69 6361 6c6c 7920 6578 7472 6163 7469  mically extracti
+00000070: 6e67 2074 6865 2070 6163 6b61 6765 2076  ng the package v
+00000080: 6572 7369 6f6e 2066 726f 6d20 6120 5f5f  ersion from a __
+00000090: 7665 7273 696f 6e5f 5f20 7661 7269 6162  version__ variab
+000000a0: 6c65 206f 7220 6120 4769 7420 7461 672e  le or a Git tag.
+000000b0: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+000000c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000000d0: 6961 6e67 6f6c 6f2f 706f 6574 7279 2d76  iangolo/poetry-v
+000000e0: 6572 7369 6f6e 2d70 6c75 6769 6e0a 4175  ersion-plugin.Au
+000000f0: 7468 6f72 3a20 5365 6261 7374 69c3 a16e  thor: Sebasti..n
+00000100: 2052 616d c3ad 7265 7a0a 4175 7468 6f72   Ram..rez.Author
+00000110: 2d65 6d61 696c 3a20 7469 616e 676f 6c6f  -email: tiangolo
+00000120: 4067 6d61 696c 2e63 6f6d 0a52 6571 7569  @gmail.com.Requi
+00000130: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+00000140: 372c 3c34 2e30 0a43 6c61 7373 6966 6965  7,<4.0.Classifie
+00000150: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000160: 7461 7475 7320 3a3a 2033 202d 2041 6c70  tatus :: 3 - Alp
+00000170: 6861 0a43 6c61 7373 6966 6965 723a 2049  ha.Classifier: I
+00000180: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000190: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
+000001a0: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+000001b0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+000001c0: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
+000001d0: 6e6f 6c6f 6779 0a43 6c61 7373 6966 6965  nology.Classifie
+000001e0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+000001f0: 656e 6365 203a 3a20 5379 7374 656d 2041  ence :: System A
+00000200: 646d 696e 6973 7472 6174 6f72 730a 436c  dministrators.Cl
+00000210: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000220: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000230: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000240: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000250: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000260: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000270: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000290: 203a 3a20 5079 7468 6f6e 0a43 6c61 7373   :: Python.Class
+000002a0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002c0: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+000002d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002f0: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
+00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000320: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
+00000330: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000350: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000360: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000370: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000380: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000390: 2e31 300a 436c 6173 7369 6669 6572 3a20  .10.Classifier: 
+000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003c0: 3a20 332e 3131 0a43 6c61 7373 6966 6965  : 3.11.Classifie
+000003d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000003e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000003f0: 6e20 3a3a 2033 203a 3a20 4f6e 6c79 0a43  n :: 3 :: Only.C
+00000400: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+00000410: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000420: 656c 6f70 6d65 6e74 0a43 6c61 7373 6966  elopment.Classif
+00000430: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
+00000440: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+00000450: 6e74 203a 3a20 4c69 6272 6172 6965 730a  nt :: Libraries.
+00000460: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000470: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000480: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000490: 7261 7269 6573 203a 3a20 4170 706c 6963  raries :: Applic
+000004a0: 6174 696f 6e20 4672 616d 6577 6f72 6b73  ation Frameworks
+000004b0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000004c0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+000004d0: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+000004e0: 6272 6172 6965 7320 3a3a 2050 7974 686f  braries :: Pytho
+000004f0: 6e20 4d6f 6475 6c65 730a 436c 6173 7369  n Modules.Classi
+00000500: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000510: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000520: 656e 7420 3a3a 2056 6572 7369 6f6e 2043  ent :: Version C
+00000530: 6f6e 7472 6f6c 203a 3a20 4769 740a 436c  ontrol :: Git.Cl
+00000540: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000550: 3a3a 2053 7973 7465 6d20 3a3a 2041 7263  :: System :: Arc
+00000560: 6869 7669 6e67 203a 3a20 5061 636b 6167  hiving :: Packag
+00000570: 696e 670a 436c 6173 7369 6669 6572 3a20  ing.Classifier: 
+00000580: 546f 7069 6320 3a3a 2053 7973 7465 6d20  Topic :: System 
+00000590: 3a3a 2049 6e73 7461 6c6c 6174 696f 6e2f  :: Installation/
+000005a0: 5365 7475 700a 436c 6173 7369 6669 6572  Setup.Classifier
+000005b0: 3a20 546f 7069 6320 3a3a 2053 7973 7465  : Topic :: Syste
+000005c0: 6d20 3a3a 2053 6f66 7477 6172 6520 4469  m :: Software Di
+000005d0: 7374 7269 6275 7469 6f6e 0a52 6571 7569  stribution.Requi
+000005e0: 7265 732d 4469 7374 3a20 706f 6574 7279  res-Dist: poetry
+000005f0: 2028 3e3d 312e 322e 302c 3c32 2e30 2e30   (>=1.2.0,<2.0.0
+00000600: 290a 5072 6f6a 6563 742d 5552 4c3a 2044  ).Project-URL: D
+00000610: 6f63 756d 656e 7461 7469 6f6e 2c20 6874  ocumentation, ht
+00000620: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000630: 2f74 6961 6e67 6f6c 6f2f 706f 6574 7279  /tiangolo/poetry
+00000640: 2d76 6572 7369 6f6e 2d70 6c75 6769 6e0a  -version-plugin.
+00000650: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000660: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000670: 6172 6b64 6f77 6e0a 0a23 2050 6f65 7472  arkdown..# Poetr
+00000680: 7920 5665 7273 696f 6e20 506c 7567 696e  y Version Plugin
+00000690: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+000006a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7469  ://github.com/ti
+000006b0: 616e 676f 6c6f 2f70 6f65 7472 792d 7665  angolo/poetry-ve
+000006c0: 7273 696f 6e2d 706c 7567 696e 2f61 6374  rsion-plugin/act
+000006d0: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
+000006e0: 6c6f 7725 3341 5465 7374 2220 7461 7267  low%3ATest" targ
+000006f0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+00000700: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000710: 3a2f 2f67 6974 6875 622e 636f 6d2f 7469  ://github.com/ti
+00000720: 616e 676f 6c6f 2f70 6f65 7472 792d 7665  angolo/poetry-ve
+00000730: 7273 696f 6e2d 706c 7567 696e 2f77 6f72  rsion-plugin/wor
+00000740: 6b66 6c6f 7773 2f54 6573 742f 6261 6467  kflows/Test/badg
+00000750: 652e 7376 6722 2061 6c74 3d22 5465 7374  e.svg" alt="Test
+00000760: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
+00000770: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000780: 636f 6d2f 7469 616e 676f 6c6f 2f70 6f65  com/tiangolo/poe
+00000790: 7472 792d 7665 7273 696f 6e2d 706c 7567  try-version-plug
+000007a0: 696e 2f61 6374 696f 6e73 3f71 7565 7279  in/actions?query
+000007b0: 3d77 6f72 6b66 6c6f 7725 3341 5075 626c  =workflow%3APubl
+000007c0: 6973 6822 2074 6172 6765 743d 225f 626c  ish" target="_bl
+000007d0: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
+000007e0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+000007f0: 7562 2e63 6f6d 2f74 6961 6e67 6f6c 6f2f  ub.com/tiangolo/
+00000800: 706f 6574 7279 2d76 6572 7369 6f6e 2d70  poetry-version-p
+00000810: 6c75 6769 6e2f 776f 726b 666c 6f77 732f  lugin/workflows/
+00000820: 5075 626c 6973 682f 6261 6467 652e 7376  Publish/badge.sv
+00000830: 6722 2061 6c74 3d22 5075 626c 6973 6822  g" alt="Publish"
+00000840: 3e0a 3c2f 613e 0a3c 6120 6872 6566 3d22  >.</a>.<a href="
+00000850: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000860: 696f 2f67 682f 7469 616e 676f 6c6f 2f70  io/gh/tiangolo/p
+00000870: 6f65 7472 792d 7665 7273 696f 6e2d 706c  oetry-version-pl
+00000880: 7567 696e 2220 7461 7267 6574 3d22 5f62  ugin" target="_b
+00000890: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+000008a0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000008b0: 2e73 6869 656c 6473 2e69 6f2f 636f 6465  .shields.io/code
+000008c0: 636f 762f 632f 6769 7468 7562 2f74 6961  cov/c/github/tia
+000008d0: 6e67 6f6c 6f2f 706f 6574 7279 2d76 6572  ngolo/poetry-ver
+000008e0: 7369 6f6e 2d70 6c75 6769 6e3f 636f 6c6f  sion-plugin?colo
+000008f0: 723d 2532 3333 3444 3035 3822 2061 6c74  r=%2334D058" alt
+00000900: 3d22 436f 7665 7261 6765 223e 0a3c 2f61  ="Coverage">.</a
+00000910: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+00000920: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000930: 6563 742f 706f 6574 7279 2d76 6572 7369  ect/poetry-versi
+00000940: 6f6e 2d70 6c75 6769 6e22 2074 6172 6765  on-plugin" targe
+00000950: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
+00000960: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000970: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000980: 2f70 7970 692f 762f 706f 6574 7279 2d76  /pypi/v/poetry-v
+00000990: 6572 7369 6f6e 2d70 6c75 6769 6e3f 636f  ersion-plugin?co
+000009a0: 6c6f 723d 2532 3333 3444 3035 3826 6c61  lor=%2334D058&la
+000009b0: 6265 6c3d 7079 7069 2532 3070 6163 6b61  bel=pypi%20packa
+000009c0: 6765 2220 616c 743d 2250 6163 6b61 6765  ge" alt="Package
+000009d0: 2076 6572 7369 6f6e 223e 0a3c 2f61 3e0a   version">.</a>.
+000009e0: 0a41 205b 2a2a 506f 6574 7279 2a2a 5d28  .A [**Poetry**](
+000009f0: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
+00000a00: 6f65 7472 792e 6f72 672f 2920 706c 7567  oetry.org/) plug
+00000a10: 696e 2066 6f72 2064 796e 616d 6963 616c  in for dynamical
+00000a20: 6c79 2065 7874 7261 6374 696e 6720 7468  ly extracting th
+00000a30: 6520 7061 636b 6167 6520 2a2a 7665 7273  e package **vers
+00000a40: 696f 6e2a 2a2e 0a0a 4974 2063 616e 2072  ion**...It can r
+00000a50: 6561 6420 7468 6520 7665 7273 696f 6e20  ead the version 
+00000a60: 6672 6f6d 2061 2066 696c 6520 605f 5f69  from a file `__i
+00000a70: 6e69 745f 5f2e 7079 6020 7769 7468 3a0a  nit__.py` with:.
+00000a80: 0a60 6060 7079 7468 6f6e 0a23 205f 5f69  .```python.# __i
+00000a90: 6e69 745f 5f2e 7079 0a0a 5f5f 7665 7273  nit__.py..__vers
+00000aa0: 696f 6e5f 5f20 3d20 2230 2e31 2e30 220a  ion__ = "0.1.0".
+00000ab0: 6060 600a 0a41 6c74 6572 6e61 7469 7665  ```..Alternative
+00000ac0: 6c79 2c20 6974 2063 616e 2072 6561 6420  ly, it can read 
+00000ad0: 6974 2066 726f 6d20 6120 2a2a 6769 7420  it from a **git 
+00000ae0: 7461 672a 2a2c 2073 6574 2077 6974 6820  tag**, set with 
+00000af0: 6120 4769 7448 7562 2072 656c 6561 7365  a GitHub release
+00000b00: 206f 7220 7769 7468 3a0a 0a60 6060 636f   or with:..```co
+00000b10: 6e73 6f6c 650a 2420 6769 7420 7461 6720  nsole.$ git tag 
+00000b20: 302e 312e 300a 6060 600a 0af0 9f9a a820  0.1.0.```...... 
+00000b30: 436f 6e73 6964 6572 2074 6869 7320 696e  Consider this in
+00000b40: 2074 6865 2061 6c70 6861 2073 7461 6765   the alpha stage
+00000b50: 2e20 5265 6164 2074 6865 2077 6172 6e69  . Read the warni
+00000b60: 6e67 2062 656c 6f77 2e0a 0a23 2320 5768  ng below...## Wh
+00000b70: 656e 2074 6f20 7573 650a 0a54 6869 7320  en to use..This 
+00000b80: 6973 2075 7365 6675 6c20 6d61 696e 6c79  is useful mainly
+00000b90: 2069 6620 796f 7520 6172 6520 6275 696c   if you are buil
+00000ba0: 6469 6e67 2061 2070 6163 6b61 6765 206c  ding a package l
+00000bb0: 6962 7261 7279 2066 6f72 206f 7468 6572  ibrary for other
+00000bc0: 7320 746f 2075 7365 2061 6e64 2079 6f75  s to use and you
+00000bd0: 2077 616e 7420 746f 2073 6574 2074 6865   want to set the
+00000be0: 2076 6572 7369 6f6e 2069 6e20 6120 706c   version in a pl
+00000bf0: 6163 6520 6469 6666 6572 656e 7420 7468  ace different th
+00000c00: 616e 2060 7079 7072 6f6a 6563 742e 746f  an `pyproject.to
+00000c10: 6d6c 602c 2062 7574 2079 6f75 2073 7469  ml`, but you sti
+00000c20: 6c6c 2077 616e 7420 746f 206b 6565 7020  ll want to keep 
+00000c30: 6120 5b73 696e 676c 6520 736f 7572 6365  a [single source
+00000c40: 206f 6620 7472 7574 685d 2868 7474 7073   of truth](https
+00000c50: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00000c60: 6f72 672f 7769 6b69 2f53 696e 676c 655f  org/wiki/Single_
+00000c70: 736f 7572 6365 5f6f 665f 7472 7574 6829  source_of_truth)
+00000c80: 2e0a 0a49 7420 776f 6e27 7420 6265 2068  ...It won't be h
+00000c90: 656c 7066 756c 2069 6e20 6f74 6865 7220  elpful in other 
+00000ca0: 7573 6520 6361 7365 7320 6c69 6b65 206d  use cases like m
+00000cb0: 616e 6167 696e 6720 6c6f 6361 6c20 6170  anaging local ap
+00000cc0: 7020 656e 7669 726f 6e6d 656e 7473 2077  p environments w
+00000cd0: 6974 6820 506f 6574 7279 2e0a 0a23 2320  ith Poetry...## 
+00000ce0: 486f 7720 746f 2075 7365 0a0a 4d61 6b65  How to use..Make
+00000cf0: 2073 7572 6520 796f 7520 6861 7665 2050   sure you have P
+00000d00: 6f65 7472 7920 7665 7273 696f 6e20 6031  oetry version `1
+00000d10: 2e32 2e30 6020 6f72 2061 626f 7665 2e20  .2.0` or above. 
+00000d20: 5265 6164 2062 656c 6f77 2066 6f72 2069  Read below for i
+00000d30: 6e73 7472 7563 7469 6f6e 7320 746f 2069  nstructions to i
+00000d40: 6e73 7461 6c6c 2069 7420 6966 2079 6f75  nstall it if you
+00000d50: 2068 6176 656e 2774 2e0a 0a23 2323 2049   haven't...### I
+00000d60: 6e73 7461 6c6c 2050 6f65 7472 7920 5665  nstall Poetry Ve
+00000d70: 7273 696f 6e20 506c 7567 696e 0a0a 496e  rsion Plugin..In
+00000d80: 7374 616c 6c20 7468 6973 2070 6c75 6769  stall this plugi
+00000d90: 6e20 746f 2079 6f75 7220 506f 6574 7279  n to your Poetry
+00000da0: 3a0a 0a60 6060 636f 6e73 6f6c 650a 2420  :..```console.$ 
+00000db0: 706f 6574 7279 2070 6c75 6769 6e20 6164  poetry plugin ad
+00000dc0: 6420 706f 6574 7279 2d76 6572 7369 6f6e  d poetry-version
+00000dd0: 2d70 6c75 6769 6e0a 0a2d 2d3e 2031 3030  -plugin..--> 100
+00000de0: 250a 6060 600a 0a23 2323 2053 6574 2076  %.```..### Set v
+00000df0: 6572 7369 6f6e 2069 6e20 696e 6974 2066  ersion in init f
+00000e00: 696c 650a 0a53 6574 2079 6f75 7220 7061  ile..Set your pa
+00000e10: 636b 6167 6520 7665 7273 696f 6e20 696e  ckage version in
+00000e20: 2079 6f75 7220 6669 6c65 2060 5f5f 696e   your file `__in
+00000e30: 6974 5f5f 2e70 7960 2c20 666f 7220 6578  it__.py`, for ex
+00000e40: 616d 706c 653a 0a0a 6060 6070 7974 686f  ample:..```pytho
+00000e50: 6e0a 6672 6f6d 202e 6d61 696e 2069 6d70  n.from .main imp
+00000e60: 6f72 7420 646f 5f61 7765 736f 6d65 5f73  ort do_awesome_s
+00000e70: 7475 6666 2c20 4177 6573 6f6d 6543 6c61  tuff, AwesomeCla
+00000e80: 7373 0a0a 5f5f 7665 7273 696f 6e5f 5f20  ss..__version__ 
+00000e90: 3d20 2230 2e32 2e33 220a 6060 600a 0a41  = "0.2.3".```..A
+00000ea0: 6e64 2074 6865 6e20 6564 6974 2079 6f75  nd then edit you
+00000eb0: 7220 6070 7970 726f 6a65 6374 2e74 6f6d  r `pyproject.tom
+00000ec0: 6c60 2077 6974 6820 6120 7365 6374 696f  l` with a sectio
+00000ed0: 6e20 636f 6e74 6169 6e69 6e67 3a0a 0a60  n containing:..`
+00000ee0: 6060 746f 6d6c 0a5b 746f 6f6c 2e70 6f65  ``toml.[tool.poe
+00000ef0: 7472 792d 7665 7273 696f 6e2d 706c 7567  try-version-plug
+00000f00: 696e 5d0a 736f 7572 6365 203d 2022 696e  in].source = "in
+00000f10: 6974 220a 6060 600a 0a4e 6578 742c 2062  it".```..Next, b
+00000f20: 7569 6c64 2079 6f75 7220 7072 6f6a 6563  uild your projec
+00000f30: 742e 2049 7420 7769 6c6c 2073 686f 7720  t. It will show 
+00000f40: 616e 206f 7574 7075 7420 6c69 6b65 3a0a  an output like:.
+00000f50: 0a60 6060 636f 6e73 6f6c 650a 2420 706f  .```console.$ po
+00000f60: 6574 7279 2062 7569 6c64 0a55 7369 6e67  etry build.Using
+00000f70: 205f 5f69 6e69 745f 5f2e 7079 2066 696c   __init__.py fil
+00000f80: 6520 6174 206d 795f 6177 6573 6f6d 655f  e at my_awesome_
+00000f90: 7061 636b 6167 652f 5f5f 696e 6974 5f5f  package/__init__
+00000fa0: 2e70 7920 666f 7220 6479 6e61 6d69 6320  .py for dynamic 
+00000fb0: 7665 7273 696f 6e0a 5365 7474 696e 6720  version.Setting 
+00000fc0: 7061 636b 6167 6520 6479 6e61 6d69 6320  package dynamic 
+00000fd0: 7665 7273 696f 6e20 746f 205f 5f76 6572  version to __ver
+00000fe0: 7369 6f6e 5f5f 2076 6172 6961 626c 6520  sion__ variable 
+00000ff0: 6672 6f6d 205f 5f69 6e69 745f 5f2e 7079  from __init__.py
+00001000: 3a20 302e 312e 390a 4275 696c 6469 6e67  : 0.1.9.Building
+00001010: 206d 792d 6177 6573 6f6d 652d 7061 636b   my-awesome-pack
+00001020: 6167 6520 2830 2e31 2e39 290a 2020 2d20  age (0.1.9).  - 
+00001030: 4275 696c 6469 6e67 2073 6469 7374 0a20  Building sdist. 
+00001040: 202d 2042 7569 6c74 206d 792d 6177 6573   - Built my-awes
+00001050: 6f6d 652d 7061 636b 6167 652d 302e 312e  ome-package-0.1.
+00001060: 392e 7461 722e 677a 0a20 202d 2042 7569  9.tar.gz.  - Bui
+00001070: 6c64 696e 6720 7768 6565 6c0a 2020 2d20  lding wheel.  - 
+00001080: 4275 696c 7420 6d79 2d61 7765 736f 6d65  Built my-awesome
+00001090: 2d70 6163 6b61 6765 2d30 2e31 2e39 2d70  -package-0.1.9-p
+000010a0: 7933 2d6e 6f6e 652d 616e 792e 7768 6c0a  y3-none-any.whl.
+000010b0: 6060 600a 0a23 2323 2053 6574 2074 6865  ```..### Set the
+000010c0: 2076 6572 7369 6f6e 2069 6e20 6120 4769   version in a Gi
+000010d0: 7420 7461 670a 0a41 6c74 6572 6e61 7469  t tag..Alternati
+000010e0: 7665 6c79 2c20 746f 2065 7874 7261 6374  vely, to extract
+000010f0: 2074 6865 2076 6572 7369 6f6e 2074 6f20   the version to 
+00001100: 7573 6520 6672 6f6d 2061 2047 6974 2074  use from a Git t
+00001110: 6167 2c20 6164 6420 6120 7365 6374 696f  ag, add a sectio
+00001120: 6e3a 0a0a 6060 6074 6f6d 6c0a 5b74 6f6f  n:..```toml.[too
+00001130: 6c2e 706f 6574 7279 2d76 6572 7369 6f6e  l.poetry-version
+00001140: 2d70 6c75 6769 6e5d 0a73 6f75 7263 6520  -plugin].source 
+00001150: 3d20 2267 6974 2d74 6167 220a 6060 600a  = "git-tag".```.
+00001160: 0a54 6865 6e20 6372 6561 7465 2061 2067  .Then create a g
+00001170: 6974 2074 6167 2c20 666f 7220 6578 616d  it tag, for exam
+00001180: 706c 653a 0a0a 6060 6063 6f6e 736f 6c65  ple:..```console
+00001190: 0a24 2067 6974 2074 6167 2030 2e31 2e33  .$ git tag 0.1.3
+000011a0: 0a60 6060 0a0a 496e 2074 6869 7320 6361  .```..In this ca
+000011b0: 7365 2c20 7768 656e 2062 7569 6c64 696e  se, when buildin
+000011c0: 6720 796f 7572 2070 726f 6a65 6374 2c20  g your project, 
+000011d0: 6974 2077 696c 6c20 7368 6f77 2061 6e20  it will show an 
+000011e0: 6f75 7470 7574 206c 696b 653a 0a0a 6060  output like:..``
+000011f0: 6063 6f6e 736f 6c65 0a24 2070 6f65 7472  `console.$ poetr
+00001200: 7920 6275 696c 640a 4769 7420 7461 6720  y build.Git tag 
+00001210: 666f 756e 642c 2073 6574 7469 6e67 2064  found, setting d
+00001220: 796e 616d 6963 2076 6572 7369 6f6e 2074  ynamic version t
+00001230: 6f3a 2030 2e31 2e33 0a42 7569 6c64 696e  o: 0.1.3.Buildin
+00001240: 6720 6d79 2d61 7765 736f 6d65 2d70 6163  g my-awesome-pac
+00001250: 6b61 6765 2028 302e 312e 3329 0a20 202d  kage (0.1.3).  -
+00001260: 2042 7569 6c64 696e 6720 7364 6973 740a   Building sdist.
+00001270: 2020 2d20 4275 696c 7420 6d79 2d61 7765    - Built my-awe
+00001280: 736f 6d65 2d70 6163 6b61 6765 2d30 2e31  some-package-0.1
+00001290: 2e33 2e74 6172 2e67 7a0a 2020 2d20 4275  .3.tar.gz.  - Bu
+000012a0: 696c 6469 6e67 2077 6865 656c 0a20 202d  ilding wheel.  -
+000012b0: 2042 7569 6c74 206d 792d 6177 6573 6f6d   Built my-awesom
+000012c0: 652d 7061 636b 6167 652d 302e 312e 332d  e-package-0.1.3-
+000012d0: 7079 332d 6e6f 6e65 2d61 6e79 2e77 686c  py3-none-any.whl
+000012e0: 0a60 6060 0a0a 2323 2056 6572 7369 6f6e  .```..## Version
+000012f0: 2069 6e20 6070 7970 726f 6a65 6374 2e74   in `pyproject.t
+00001300: 6f6d 6c60 0a0a 4375 7272 656e 746c 7920  oml`..Currently 
+00001310: 2832 3032 312d 3035 2d32 3429 2050 6f65  (2021-05-24) Poe
+00001320: 7472 7920 7265 7175 6972 6573 2061 2060  try requires a `
+00001330: 7665 7273 696f 6e60 2063 6f6e 6669 6775  version` configu
+00001340: 7261 7469 6f6e 2069 6e20 7468 6520 6070  ration in the `p
+00001350: 7970 726f 6a65 6374 2e74 6f6d 6c60 2c20  yproject.toml`, 
+00001360: 6576 656e 2069 6620 796f 7520 7573 6520  even if you use 
+00001370: 7468 6973 2070 6c75 6769 6e2e 0a0a 5768  this plugin...Wh
+00001380: 656e 2075 7369 6e67 2074 6869 7320 706c  en using this pl
+00001390: 7567 696e 2c20 7468 6174 2060 7665 7273  ugin, that `vers
+000013a0: 696f 6e60 2063 6f6e 6669 6720 776f 6e27  ion` config won'
+000013b0: 7420 6265 2075 7365 642c 2062 7574 2050  t be used, but P
+000013c0: 6f65 7472 7920 7374 696c 6c20 7265 7175  oetry still requ
+000013d0: 6972 6573 2069 7420 746f 2062 6520 7072  ires it to be pr
+000013e0: 6573 656e 7420 696e 2074 6865 2060 7079  esent in the `py
+000013f0: 7072 6f6a 6563 742e 746f 6d6c 602e 0a0a  project.toml`...
+00001400: 546f 206d 616b 6520 6974 206d 6f72 6520  To make it more 
+00001410: 6576 6964 656e 7420 7468 6174 2079 6f75  evident that you
+00001420: 2061 7265 206e 6f74 2075 7369 6e67 2074   are not using t
+00001430: 6861 7420 6076 6572 7369 6f6e 6020 796f  hat `version` yo
+00001440: 7520 6361 6e20 7365 7420 6974 2074 6f20  u can set it to 
+00001450: 6030 602e 0a0a 6060 6074 6f6d 6c0a 5b74  `0`...```toml.[t
+00001460: 6f6f 6c2e 706f 6574 7279 5d0a 6e61 6d65  ool.poetry].name
+00001470: 203d 2022 6d79 2d61 7765 736f 6d65 2d70   = "my-awesome-p
+00001480: 6163 6b61 6765 220a 7665 7273 696f 6e20  ackage".version 
+00001490: 3d20 2230 220a 6060 600a 0a54 6861 7420  = "0".```..That 
+000014a0: 7761 792c 2079 6f75 2077 696c 6c20 6d6f  way, you will mo
+000014b0: 7265 2065 6173 696c 7920 6e6f 7469 6365  re easily notice
+000014c0: 2069 6620 7468 6520 706c 7567 696e 2069   if the plugin i
+000014d0: 7320 6e6f 7420 696e 7374 616c 6c65 642c  s not installed,
+000014e0: 2061 7320 6974 2077 696c 6c20 7368 6f77   as it will show
+000014f0: 2074 6861 7420 796f 7520 6172 6520 6275   that you are bu
+00001500: 696c 6469 6e67 2061 2070 6163 6b61 6765  ilding a package
+00001510: 2077 6974 6820 7665 7273 696f 6e20 6030   with version `0
+00001520: 6020 696e 7374 6561 6420 6f66 2074 6865  ` instead of the
+00001530: 2064 796e 616d 6963 2076 6572 7369 6f6e   dynamic version
+00001540: 2073 6574 2e0a 0a23 2320 416e 2065 7861   set...## An exa
+00001550: 6d70 6c65 2060 7079 7072 6f6a 6563 742e  mple `pyproject.
+00001560: 746f 6d6c 600a 0a41 2073 686f 7274 2c20  toml`..A short, 
+00001570: 6d69 6e69 6d61 6c20 6578 616d 706c 6520  minimal example 
+00001580: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
+00001590: 2063 6f75 6c64 206c 6f6f 6b20 6c69 6b65   could look like
+000015a0: 3a0a 0a60 6060 746f 6d6c 0a5b 746f 6f6c  :..```toml.[tool
+000015b0: 2e70 6f65 7472 795d 0a6e 616d 6520 3d20  .poetry].name = 
+000015c0: 226d 792d 6177 6573 6f6d 652d 7061 636b  "my-awesome-pack
+000015d0: 6167 6522 0a76 6572 7369 6f6e 203d 2022  age".version = "
+000015e0: 3022 0a64 6573 6372 6970 7469 6f6e 203d  0".description =
+000015f0: 2022 220a 6175 7468 6f72 7320 3d20 5b22   "".authors = ["
+00001600: 5269 636b 2053 616e 6368 657a 203c 7269  Rick Sanchez <ri
+00001610: 636b 4072 6963 6b2d 6369 7461 6465 6c2e  ck@rick-citadel.
+00001620: 636f 6d3e 225d 0a72 6561 646d 6520 3d20  com>"].readme = 
+00001630: 2252 4541 444d 452e 6d64 220a 0a5b 746f  "README.md"..[to
+00001640: 6f6c 2e70 6f65 7472 792e 6465 7065 6e64  ol.poetry.depend
+00001650: 656e 6369 6573 5d0a 7079 7468 6f6e 203d  encies].python =
+00001660: 2022 5e33 2e37 220a 0a5b 6275 696c 642d   "^3.7"..[build-
+00001670: 7379 7374 656d 5d0a 7265 7175 6972 6573  system].requires
+00001680: 203d 205b 2270 6f65 7472 792d 636f 7265   = ["poetry-core
+00001690: 225d 0a62 7569 6c64 2d62 6163 6b65 6e64  "].build-backend
+000016a0: 203d 2022 706f 6574 7279 2e63 6f72 652e   = "poetry.core.
+000016b0: 6d61 736f 6e72 792e 6170 6922 0a0a 5b74  masonry.api"..[t
+000016c0: 6f6f 6c2e 706f 6574 7279 2d76 6572 7369  ool.poetry-versi
+000016d0: 6f6e 2d70 6c75 6769 6e5d 0a73 6f75 7263  on-plugin].sourc
+000016e0: 6520 3d20 2269 6e69 7422 0a60 6060 0a0a  e = "init".```..
+000016f0: 2323 2057 6879 0a0a 4279 2064 6566 6175  ## Why..By defau
+00001700: 6c74 2c20 506f 6574 7279 2065 7870 6563  lt, Poetry expec
+00001710: 7473 2079 6f75 2074 6f20 7365 7420 796f  ts you to set yo
+00001720: 7572 2070 6163 6b61 6765 2076 6572 7369  ur package versi
+00001730: 6f6e 2069 6e20 6070 7970 726f 6a65 6374  on in `pyproject
+00001740: 2e74 6f6d 6c60 2e20 416e 6420 7468 6174  .toml`. And that
+00001750: 2077 6f75 6c64 2077 6f72 6b20 696e 206d   would work in m
+00001760: 6f73 7420 6361 7365 732e 0a0a 4275 7420  ost cases...But 
+00001770: 696d 6167 696e 6520 796f 7520 7761 6e74  imagine you want
+00001780: 2074 6f20 6578 706f 7365 2074 6865 2076   to expose the v
+00001790: 6572 7369 6f6e 206f 6620 796f 7572 2070  ersion of your p
+000017a0: 6163 6b61 6765 2069 6e20 6120 605f 5f76  ackage in a `__v
+000017b0: 6572 7369 6f6e 5f5f 6020 7661 7269 6162  ersion__` variab
+000017c0: 6c65 2073 6f20 7468 6174 2079 6f75 7220  le so that your 
+000017d0: 7573 6572 7320 6361 6e20 646f 2074 6869  users can do thi
+000017e0: 6e67 7320 6c69 6b65 3a0a 0a60 6060 7079  ngs like:..```py
+000017f0: 7468 6f6e 0a69 6d70 6f72 7420 6d79 5f61  thon.import my_a
+00001800: 7765 736f 6d65 5f70 6163 6b61 6765 0a70  wesome_package.p
+00001810: 7269 6e74 286d 795f 6177 6573 6f6d 655f  rint(my_awesome_
+00001820: 7061 636b 6167 652e 5f5f 7665 7273 696f  package.__versio
+00001830: 6e5f 5f29 0a60 6060 0a0a 596f 7520 636f  n__).```..You co
+00001840: 756c 6420 6d61 6e75 616c 6c79 2077 7269  uld manually wri
+00001850: 7465 2074 6865 2060 5f5f 7665 7273 696f  te the `__versio
+00001860: 6e5f 5f60 2076 6172 6961 626c 6520 616e  n__` variable an
+00001870: 6420 6861 6e64 6c65 2074 6865 2073 796e  d handle the syn
+00001880: 6368 726f 6e69 7a61 7469 6f6e 2062 6574  chronization bet
+00001890: 7765 656e 2069 7420 616e 6420 7468 6520  ween it and the 
+000018a0: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
+000018b0: 2079 6f75 7273 656c 662c 2077 6869 6368   yourself, which
+000018c0: 2069 7320 7665 7279 202a 2a65 7272 6f72   is very **error
+000018d0: 2d70 726f 6e65 2a2a 2e0a 0a54 6865 2063  -prone**...The c
+000018e0: 7572 7265 6e74 205b 6f66 6669 6369 616c  urrent [official
+000018f0: 2077 6179 206f 6620 646f 696e 6720 6974   way of doing it
+00001900: 2077 6974 686f 7574 2064 7570 6c69 6361   without duplica
+00001910: 7469 6e67 2074 6865 2076 616c 7565 5d28  ting the value](
+00001920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001930: 6f6d 2f70 7974 686f 6e2d 706f 6574 7279  om/python-poetry
+00001940: 2f70 6f65 7472 792f 7075 6c6c 2f32 3336  /poetry/pull/236
+00001950: 3623 6973 7375 6563 6f6d 6d65 6e74 2d36  6#issuecomment-6
+00001960: 3532 3431 3830 3934 2920 6973 2077 6974  52418094) is wit
+00001970: 6820 6069 6d70 6f72 746c 6962 2e6d 6574  h `importlib.met
+00001980: 6164 6174 6160 2e0a 0a42 7574 2074 6861  adata`...But tha
+00001990: 7420 6d6f 6475 6c65 2069 7320 6f6e 6c79  t module is only
+000019a0: 2061 7661 696c 6162 6c65 2069 6e20 5079   available in Py
+000019b0: 7468 6f6e 2033 2e38 2061 6e64 2061 626f  thon 3.8 and abo
+000019c0: 7665 2e20 536f 2c20 666f 7220 5079 7468  ve. So, for Pyth
+000019d0: 6f6e 2033 2e37 2061 6e64 2033 2e36 2079  on 3.7 and 3.6 y
+000019e0: 6f75 2068 6176 6520 746f 2069 6e73 7461  ou have to insta
+000019f0: 6c6c 2061 2062 6163 6b70 6f72 7420 6173  ll a backport as
+00001a00: 2061 2064 6570 656e 6465 6e63 7920 6f66   a dependency of
+00001a10: 2079 6f75 7220 7061 636b 6167 653a 0a0a   your package:..
+00001a20: 6060 6074 6f6d 6c0a 5b74 6f6f 6c2e 706f  ```toml.[tool.po
+00001a30: 6574 7279 2e64 6570 656e 6465 6e63 6965  etry.dependencie
+00001a40: 735d 0a69 6d70 6f72 746c 6962 2d6d 6574  s].importlib-met
+00001a50: 6164 6174 6120 3d20 7b76 6572 7369 6f6e  adata = {version
+00001a60: 203d 2022 5e31 2e30 222c 2070 7974 686f   = "^1.0", pytho
+00001a70: 6e20 3d20 223c 332e 3822 7d0a 6060 600a  n = "<3.8"}.```.
+00001a80: 0a42 7574 2074 6865 6e2c 2077 6865 6e20  .But then, when 
+00001a90: 7468 6579 2072 656c 6561 7365 2065 6163  they release eac
+00001aa0: 6820 6e65 7720 7665 7273 696f 6e20 6f66  h new version of
+00001ab0: 2074 6865 2062 6163 6b70 6f72 7420 2863   the backport (c
+00001ac0: 7572 7265 6e74 6c79 2060 342e 302e 3160  urrently `4.0.1`
+00001ad0: 292c 2079 6f75 2068 6176 6520 746f 2075  ), you have to u
+00001ae0: 7064 6174 6520 6974 2028 6f72 206e 6f74  pdate it (or not
+00001af0: 292e 2041 6e64 2079 6f75 7220 7573 6572  ). And your user
+00001b00: 7320 776f 756c 6420 6861 7665 2074 6f20  s would have to 
+00001b10: 6d61 6e75 616c 6c79 2068 616e 646c 6520  manually handle 
+00001b20: 636f 6e66 6c69 6374 7320 7769 7468 2061  conflicts with a
+00001b30: 6e79 206f 7468 6572 2070 6163 6b61 6765  ny other package
+00001b40: 7320 7468 6174 2061 6c73 6f20 6465 7065  s that also depe
+00001b50: 6e64 206f 6e20 6069 6d70 6f72 746c 6962  nd on `importlib
+00001b60: 2d6d 6574 6164 6174 6160 2077 6869 6368  -metadata` which
+00001b70: 2063 6f75 6c64 2062 6520 6d75 6c74 6970   could be multip
+00001b80: 6c65 2c20 6173 206d 616e 7920 7061 636b  le, as many pack
+00001b90: 6167 6573 2063 6f75 6c64 2062 6520 646f  ages could be do
+00001ba0: 696e 6720 7468 6520 7361 6d65 2074 7269  ing the same tri
+00001bb0: 636b 2028 4927 7665 2064 6561 6c74 2077  ck (I've dealt w
+00001bc0: 6974 6820 7468 6174 292e 0a0a 5468 6520  ith that)...The 
+00001bd0: 6f74 6865 7220 6f70 7469 6f6e 2069 7320  other option is 
+00001be0: 6e6f 7420 746f 2070 696e 2061 6e79 2076  not to pin any v
+00001bf0: 6572 7369 6f6e 2072 616e 6765 206f 6620  ersion range of 
+00001c00: 796f 7572 2060 696d 706f 7274 6c69 622d  your `importlib-
+00001c10: 6d65 7461 6461 7461 6020 696e 2079 6f75  metadata` in you
+00001c20: 7220 6070 7970 726f 6a65 6374 2e74 6f6d  r `pyproject.tom
+00001c30: 6c60 2061 6e64 2068 6f70 6520 666f 7220  l` and hope for 
+00001c40: 7468 6520 6265 7374 2e0a 0a41 6e64 2074  the best...And t
+00001c50: 6865 6e20 796f 7572 2060 5f5f 696e 6974  hen your `__init
+00001c60: 5f5f 2e70 7960 2077 6f75 6c64 2068 6176  __.py` would hav
+00001c70: 6520 746f 2069 6e63 6c75 6465 2063 6f64  e to include cod
+00001c80: 6520 7573 696e 6720 6974 2c20 6c69 6b65  e using it, like
+00001c90: 3a0a 0a60 6060 7079 7468 6f6e 0a23 2049  :..```python.# I
+00001ca0: 2064 6f6e 2774 2077 616e 7420 7468 6973   don't want this
+00001cb0: 2065 7874 7261 2063 6f6d 706c 6578 6974   extra complexit
+00001cc0: 7920 f09f 9894 0a23 2041 6e64 2069 7420  y .....# And it 
+00001cd0: 646f 6573 6e27 7420 776f 726b 2069 6e20  doesn't work in 
+00001ce0: 446f 636b 6572 20f0 9f90 8b0a 7472 793a  Docker .....try:
+00001cf0: 0a20 2020 2069 6d70 6f72 7420 696d 706f  .    import impo
+00001d00: 7274 6c69 622e 6d65 7461 6461 7461 2061  rtlib.metadata a
+00001d10: 7320 696d 706f 7274 6c69 625f 6d65 7461  s importlib_meta
+00001d20: 6461 7461 0a65 7863 6570 7420 4d6f 6475  data.except Modu
+00001d30: 6c65 4e6f 7446 6f75 6e64 4572 726f 723a  leNotFoundError:
+00001d40: 0a20 2020 2069 6d70 6f72 7420 696d 706f  .    import impo
+00001d50: 7274 6c69 625f 6d65 7461 6461 7461 0a0a  rtlib_metadata..
+00001d60: 5f5f 7665 7273 696f 6e5f 5f20 3d20 696d  __version__ = im
+00001d70: 706f 7274 6c69 625f 6d65 7461 6461 7461  portlib_metadata
+00001d80: 2e76 6572 7369 6f6e 285f 5f6e 616d 655f  .version(__name_
+00001d90: 5f29 0a60 6060 0a0a 4275 7420 7468 6174  _).```..But that
+00001da0: 2063 6f64 6520 6973 2065 7874 7261 2063   code is extra c
+00001db0: 6f6d 706c 6578 6974 7920 616e 6420 6c6f  omplexity and lo
+00001dc0: 6769 6320 6e65 6564 6564 2069 6e20 796f  gic needed in yo
+00001dd0: 7572 2063 6f64 652c 2069 6e20 6561 6368  ur code, in each
+00001de0: 206f 6620 796f 7572 2070 6163 6b61 6765   of your package
+00001df0: 732e 0a0a f09f 9aa8 2041 6464 6974 696f  s....... Additio
+00001e00: 6e61 6c6c 792c 2074 6869 7320 6f6e 6c79  nally, this only
+00001e10: 2077 6f72 6b73 2077 6865 6e20 796f 7572   works when your
+00001e20: 2070 6163 6b61 6765 2069 7320 696e 7374   package is inst
+00001e30: 616c 6c65 6420 696e 2061 2050 7974 686f  alled in a Pytho
+00001e40: 6e20 656e 7669 726f 6e6d 656e 742e 2049  n environment. I
+00001e50: 7420 776f 6e27 7420 776f 726b 2069 662c  t won't work if,
+00001e60: 2066 6f72 2065 7861 6d70 6c65 2c20 796f   for example, yo
+00001e70: 7520 7369 6d70 6c79 2070 7574 2079 6f75  u simply put you
+00001e80: 7220 636f 6465 2069 6e20 6120 2a2a 636f  r code in a **co
+00001e90: 6e74 6169 6e65 722a 2a2c 2077 6869 6368  ntainer**, which
+00001ea0: 2069 7320 636f 6d6d 6f6e 2066 6f72 2077   is common for w
+00001eb0: 6562 2061 7070 7320 616e 6420 6469 7374  eb apps and dist
+00001ec0: 7269 6275 7465 6420 7379 7374 656d 732e  ributed systems.
+00001ed0: 0a0a 2323 2320 486f 7720 7468 6973 2070  ..### How this p
+00001ee0: 6c75 6769 6e20 736f 6c76 6573 2069 740a  lugin solves it.
+00001ef0: 0a57 6974 6820 7468 6973 2070 6c75 6769  .With this plugi
+00001f00: 6e2c 2079 6f75 7220 7061 636b 6167 6520  n, your package 
+00001f10: 646f 6573 6e27 7420 6465 7065 6e64 206f  doesn't depend o
+00001f20: 6e20 6069 6d70 6f72 746c 6962 2d6d 6574  n `importlib-met
+00001f30: 6164 6174 6160 2c20 736f 2079 6f75 7220  adata`, so your 
+00001f40: 7573 6572 7320 776f 6e27 7420 6e65 6564  users won't need
+00001f50: 2074 6f20 6861 6e64 6c65 2063 6f6e 666c   to handle confl
+00001f60: 6963 7473 206f 7220 6578 7472 6120 6465  icts or extra de
+00001f70: 7065 6e64 656e 6369 6573 2e0a 0a49 6e73  pendencies...Ins
+00001f80: 7465 6164 2c20 796f 7572 2062 7569 6c64  tead, your build
+00001f90: 2073 7973 7465 6d20 2850 6f65 7472 7929   system (Poetry)
+00001fa0: 2069 7320 7768 6174 206e 6565 6473 2074   is what needs t
+00001fb0: 6f20 6861 7665 2074 6869 7320 706c 7567  o have this plug
+00001fc0: 696e 2069 6e73 7461 6c6c 6564 2e0a 0a54  in installed...T
+00001fd0: 6861 7420 6176 6f69 6473 2074 6865 2065  hat avoids the e
+00001fe0: 7874 7261 2063 6f64 6520 636f 6d70 6c65  xtra code comple
+00001ff0: 7869 7479 206f 6e20 796f 7572 2073 6964  xity on your sid
+00002000: 652c 2064 6570 656e 6465 6e63 7920 636f  e, dependency co
+00002010: 6e66 6c69 6374 7320 666f 7220 796f 7572  nflicts for your
+00002020: 2075 7365 7273 2c20 616e 6420 7375 7070   users, and supp
+00002030: 6f72 7420 666f 7220 6f74 6865 7220 7573  ort for other us
+00002040: 6520 6361 7365 7320 6c69 6b65 2063 6f64  e cases like cod
+00002050: 6520 636f 7069 6564 2064 6972 6563 746c  e copied directl
+00002060: 7920 696e 7369 6465 2061 2063 6f6e 7461  y inside a conta
+00002070: 696e 6572 2e0a 0a23 2323 2056 6572 7369  iner...### Versi
+00002080: 6f6e 2066 726f 6d20 4769 7420 7461 670a  on from Git tag.
+00002090: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+000020a0: 7468 6973 2070 6c75 6769 6e20 6361 6e20  this plugin can 
+000020b0: 616c 736f 2065 7874 7261 6374 2074 6865  also extract the
+000020c0: 2076 6572 7369 6f6e 2066 726f 6d20 6120   version from a 
+000020d0: 4769 7420 7461 672e 0a0a 536f 2c20 796f  Git tag...So, yo
+000020e0: 7520 636f 756c 6420 6f6e 6c79 2063 7265  u could only cre
+000020f0: 6174 6520 6561 6368 2076 6572 7369 6f6e  ate each version
+00002100: 2069 6e20 6120 4769 7420 7461 6720 2866   in a Git tag (f
+00002110: 6f72 2065 7861 6d70 6c65 2c20 6120 4769  or example, a Gi
+00002120: 7448 7562 2072 656c 6561 7365 2920 696e  tHub release) in
+00002130: 7374 6561 6420 6f66 2077 7269 7469 6e67  stead of writing
+00002140: 2069 7420 696e 2063 6f64 652e 0a0a 416e   it in code...An
+00002150: 6420 7468 656e 2062 7569 6c64 2074 6865  d then build the
+00002160: 2070 6163 6b61 6765 206f 6e20 436f 6e74   package on Cont
+00002170: 696e 756f 7573 2049 6e74 6567 7261 7469  inuous Integrati
+00002180: 6f6e 2028 652e 672e 2047 6974 4875 6220  on (e.g. GitHub 
+00002190: 4163 7469 6f6e 7329 2e20 416e 6420 7468  Actions). And th
+000021a0: 6973 2070 6c75 6769 6e20 776f 756c 6420  is plugin would 
+000021b0: 6765 7420 7468 6520 7665 7273 696f 6e20  get the version 
+000021c0: 6f66 2074 6865 2070 6163 6b61 6765 2066  of the package f
+000021d0: 726f 6d20 7468 6174 2047 6974 2074 6167  rom that Git tag
+000021e0: 2e0a 0a23 2320 496e 7374 616c 6c20 506f  ...## Install Po
+000021f0: 6574 7279 2060 312e 322e 3060 0a0a 466f  etry `1.2.0`..Fo
+00002200: 7220 7468 6973 2070 6c75 6769 6e20 746f  r this plugin to
+00002210: 2077 6f72 6b2c 2079 6f75 206e 6565 6420   work, you need 
+00002220: 506f 6574 7279 2076 6572 7369 6f6e 2060  Poetry version `
+00002230: 312e 322e 3060 206f 7220 6162 6f76 652e  1.2.0` or above.
+00002240: 0a0a 5b50 6f65 7472 7920 6031 2e32 2e30  ..[Poetry `1.2.0
+00002250: 6020 7761 7320 7265 6c65 6173 6564 2072  ` was released r
+00002260: 6563 656e 746c 795d 2868 7474 7073 3a2f  ecently](https:/
+00002270: 2f70 7974 686f 6e2d 706f 6574 7279 2e6f  /python-poetry.o
+00002280: 7267 2f62 6c6f 672f 616e 6e6f 756e 6369  rg/blog/announci
+00002290: 6e67 2d70 6f65 7472 792d 312e 322e 302f  ng-poetry-1.2.0/
+000022a0: 292e 0a0a 5468 6572 6527 7320 6120 6869  )...There's a hi
+000022b0: 6768 2063 6861 6e63 6520 796f 7520 616c  gh chance you al
+000022c0: 7265 6164 7920 6861 7665 2069 6e73 7461  ready have insta
+000022d0: 6c6c 6564 2050 6f65 7472 7920 6031 2e31  lled Poetry `1.1
+000022e0: 2e78 602e 0a0a 5468 6520 6669 7273 7420  .x`...The first 
+000022f0: 7374 6570 2069 7320 746f 2075 6e69 6e73  step is to unins
+00002300: 7461 6c6c 2069 743a 0a0a 6060 6063 6f6e  tall it:..```con
+00002310: 736f 6c65 0a24 2063 7572 6c20 2d73 534c  sole.$ curl -sSL
+00002320: 2068 7474 7073 3a2f 2f72 6177 2e67 6974   https://raw.git
+00002330: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00002340: 6f6d 2f70 7974 686f 6e2d 706f 6574 7279  om/python-poetry
+00002350: 2f70 6f65 7472 792f 6d61 7374 6572 2f67  /poetry/master/g
+00002360: 6574 2d70 6f65 7472 792e 7079 202d 4f0a  et-poetry.py -O.
+00002370: 2d2d 3e20 3130 3025 0a0a 2420 7079 7468  --> 100%..$ pyth
+00002380: 6f6e 2067 6574 2d70 6f65 7472 792e 7079  on get-poetry.py
+00002390: 202d 2d75 6e69 6e73 7461 6c6c 0a2d 2d3e   --uninstall.-->
+000023a0: 2031 3030 250a 6060 600a 0a41 6e64 2074   100%.```..And t
+000023b0: 6865 6e20 696e 7374 616c 6c20 7468 6520  hen install the 
+000023c0: 6e65 7720 506f 6574 7279 2077 6974 6820  new Poetry with 
+000023d0: 7468 6520 6e65 7720 696e 7374 616c 6c65  the new installe
+000023e0: 723a 0a0a 6060 6063 6f6e 736f 6c65 0a24  r:..```console.$
+000023f0: 2063 7572 6c20 2d73 534c 2068 7474 7073   curl -sSL https
+00002400: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002410: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 7974  rcontent.com/pyt
+00002420: 686f 6e2d 706f 6574 7279 2f70 6f65 7472  hon-poetry/poetr
+00002430: 792f 6d61 7374 6572 2f69 6e73 7461 6c6c  y/master/install
+00002440: 2d70 6f65 7472 792e 7079 202d 4f0a 2d2d  -poetry.py -O.--
+00002450: 3e20 3130 3025 0a0a 2420 7079 7468 6f6e  > 100%..$ python
+00002460: 2069 6e73 7461 6c6c 2d70 6f65 7472 792e   install-poetry.
+00002470: 7079 202d 2d70 7265 7669 6577 0a2d 2d3e  py --preview.-->
+00002480: 2031 3030 250a 6060 600a 0af0 9f94 8d20   100%.```...... 
+00002490: 4e6f 7469 6365 2074 6861 7420 7468 6520  Notice that the 
+000024a0: 6e65 7720 696e 7374 616c 6c65 7220 6669  new installer fi
+000024b0: 6c65 2069 7320 6e61 6d65 6420 6069 6e73  le is named `ins
+000024c0: 7461 6c6c 2d70 6f65 7472 792e 7079 6020  tall-poetry.py` 
+000024d0: 696e 7374 6561 6420 6f66 2060 6765 742d  instead of `get-
+000024e0: 706f 6574 7279 2e70 7960 2e20 416c 736f  poetry.py`. Also
+000024f0: 2c20 6e6f 7469 6365 2074 6861 742c 2063  , notice that, c
+00002500: 7572 7265 6e74 6c79 2c20 796f 7520 6e65  urrently, you ne
+00002510: 6564 2074 6f20 7365 7420 602d 2d70 7265  ed to set `--pre
+00002520: 7669 6577 6020 666f 7220 6974 2074 6f20  view` for it to 
+00002530: 696e 7374 616c 6c20 7468 6520 616c 7068  install the alph
+00002540: 6120 7665 7273 696f 6e20 6031 2e32 2e30  a version `1.2.0
+00002550: 602e 0a0a 596f 7520 6361 6e20 6368 6563  `...You can chec
+00002560: 6b20 7468 6174 2069 7420 776f 726b 6564  k that it worked
+00002570: 2077 6974 683a 0a0a 6060 6063 6f6e 736f   with:..```conso
+00002580: 6c65 0a24 2070 6f65 7472 7920 2d2d 7665  le.$ poetry --ve
+00002590: 7273 696f 6e0a 506f 6574 7279 2028 7665  rsion.Poetry (ve
+000025a0: 7273 696f 6e20 312e 322e 3029 0a60 6060  rsion 1.2.0).```
+000025b0: 0a0a 2323 2053 7570 706f 7274 2066 6f72  ..## Support for
+000025c0: 2076 6572 7369 6f6e 2069 6e20 696e 6974   version in init
+000025d0: 2066 696c 650a 0a57 6865 6e20 7573 696e   file..When usin
+000025e0: 6720 6120 605f 5f76 6572 7369 6f6e 5f5f  g a `__version__
+000025f0: 6020 7661 7269 6162 6c65 2069 6e20 796f  ` variable in yo
+00002600: 7572 2060 5f5f 696e 6974 5f5f 2e70 7960  ur `__init__.py`
+00002610: 2079 6f75 2063 616e 2068 6176 6520 6d6f   you can have mo
+00002620: 7265 206c 6f67 6963 2069 6e20 7468 6174  re logic in that
+00002630: 2066 696c 652c 2069 6d70 6f72 7420 6d6f   file, import mo
+00002640: 6475 6c65 732c 2061 6e64 2064 6f20 6d6f  dules, and do mo
+00002650: 7265 2074 6869 6e67 7320 6162 6f76 6520  re things above 
+00002660: 616e 6420 6265 6c6f 7720 7468 6520 6465  and below the de
+00002670: 636c 6172 6174 696f 6e20 6f66 2074 6861  claration of tha
+00002680: 7420 7661 7269 6162 6c65 2e0a 0a42 7574  t variable...But
+00002690: 2074 6865 2076 616c 7565 2068 6173 2074   the value has t
+000026a0: 6f20 6265 2061 206c 6974 6572 616c 2073  o be a literal s
+000026b0: 7472 696e 672c 206c 696b 653a 0a0a 6060  tring, like:..``
+000026c0: 6070 7974 686f 6e0a 5f5f 5f76 6572 7369  `python.___versi
+000026d0: 6f6e 5f5f 5f20 3d20 2230 2e32 2e30 220a  on___ = "0.2.0".
+000026e0: 6060 600a 0a2e 2e2e 696e 7374 6561 6420  ```.....instead 
+000026f0: 6f66 2063 616c 6c69 6e67 2061 2066 756e  of calling a fun
+00002700: 6374 696f 6e20 6f72 2073 6f6d 6574 6869  ction or somethi
+00002710: 6e67 2073 696d 696c 6172 2e0a 0a41 6e64  ng similar...And
+00002720: 2074 6865 2076 6172 6961 626c 6520 6861   the variable ha
+00002730: 7320 746f 2062 6520 6174 2074 6865 2074  s to be at the t
+00002740: 6f70 2d6c 6576 656c 2c20 736f 2069 7420  op-level, so it 
+00002750: 6361 6e27 7420 6265 2069 6e73 6964 6520  can't be inside 
+00002760: 616e 2060 6966 6020 7374 6174 656d 656e  an `if` statemen
+00002770: 7420 6f72 2073 696d 696c 6172 2e0a 0a54  t or similar...T
+00002780: 6869 7320 6973 2061 6c6c 2066 696e 6520  his is all fine 
+00002790: 616e 6420 7375 7070 6f72 7465 6420 696e  and supported in
+000027a0: 2079 6f75 7220 605f 5f69 6e69 745f 5f2e   your `__init__.
+000027b0: 7079 603a 0a0a 6060 6070 7974 686f 6e0a  py`:..```python.
+000027c0: 2320 5f5f 696e 6974 5f5f 2e70 790a 0a23  # __init__.py..#
+000027d0: 2054 6869 7320 6973 2061 6c6c 2076 616c   This is all val
+000027e0: 6964 20f0 9f91 8de2 9c85 0a0a 6672 6f6d  id .........from
+000027f0: 202e 6d61 696e 2069 6d70 6f72 7420 646f   .main import do
+00002800: 5f61 7765 736f 6d65 5f73 7475 6666 2c20  _awesome_stuff, 
+00002810: 4177 6573 6f6d 6543 6c61 7373 0a0a 6177  AwesomeClass..aw
+00002820: 6573 6f6d 6520 3d20 4177 6573 6f6d 6543  esome = AwesomeC
+00002830: 6c61 7373 2829 0a0a 2320 536f 6d65 2063  lass()..# Some c
+00002840: 6f6d 6d65 6e74 2065 7870 6c61 696e 696e  omment explainin
+00002850: 6720 7768 7920 7468 6973 2069 7320 636f  g why this is co
+00002860: 6d6d 656e 7465 6420 6f75 740a 2320 5f5f  mmented out.# __
+00002870: 7665 7273 696f 6e5f 5f20 3d20 2231 2e30  version__ = "1.0
+00002880: 2e30 220a 0a5f 5f76 6572 7369 6f6e 5f5f  .0"..__version__
+00002890: 203d 2022 302e 322e 3322 0a0a 6966 205f   = "0.2.3"..if _
+000028a0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
+000028b0: 696e 5f5f 223a 0a20 2020 2061 7765 736f  in__":.    aweso
+000028c0: 6d65 2e72 756e 2829 0a60 6060 0a0a 5468  me.run().```..Th
+000028d0: 6973 2065 7861 6d70 6c65 2069 7320 616c  is example is al
+000028e0: 6c20 7661 6c69 6420 616e 6420 7375 7070  l valid and supp
+000028f0: 6f72 7465 642c 2061 6e64 2069 7420 696e  orted, and it in
+00002900: 636c 7564 6573 3a0a 0a2a 2049 6d70 6f72  cludes:..* Impor
+00002910: 7473 0a2a 204f 7468 6572 206f 626a 6563  ts.* Other objec
+00002920: 7473 2061 6e64 2076 6172 6961 626c 6573  ts and variables
+00002930: 0a2a 2043 6f6d 6d65 6e74 730a 2a20 5468  .* Comments.* Th
+00002940: 6520 7361 6d65 2073 7472 696e 6720 605f  e same string `_
+00002950: 5f76 6572 7369 6f6e 5f5f 6020 696e 7369  _version__` insi
+00002960: 6465 2061 2063 6f6d 6d65 6e74 0a2a 2049  de a comment.* I
+00002970: 6620 626c 6f63 6b73 2061 726f 756e 640a  f blocks around.
+00002980: 0a2d 2d2d 0a0a 4275 7420 7468 6973 2069  .---..But this i
+00002990: 7320 6e6f 7420 7375 7070 6f72 7465 643a  s not supported:
+000029a0: 0a0a 6060 6070 7974 686f 6e0a 2320 f09f  ..```python.# ..
+000029b0: 9aa8 204e 6f74 2073 7570 706f 7274 6564  .. Not supported
+000029c0: 0a0a 6966 2032 203d 3d20 323a 0a20 2020  ..if 2 == 2:.   
+000029d0: 205f 5f76 6572 7369 6f6e 5f5f 203d 2022   __version__ = "
+000029e0: 302e 312e 300a 6060 600a 0a41 6e64 2074  0.1.0.```..And t
+000029f0: 6869 7320 6973 206e 6f74 2073 7570 706f  his is not suppo
+00002a00: 7274 6564 3a0a 0a60 6060 7079 7468 6f6e  rted:..```python
+00002a10: 0a23 20f0 9f9a a820 4e6f 7420 7375 7070  .# .... Not supp
+00002a20: 6f72 7465 640a 0a64 6566 2067 6574 5f76  orted..def get_v
+00002a30: 6572 7369 6f6e 2829 3a0a 2020 2020 7265  ersion():.    re
+00002a40: 7475 726e 2022 302e 322e 3022 0a0a 5f5f  turn "0.2.0"..__
+00002a50: 7665 7273 696f 6e5f 5f20 3d20 6765 745f  version__ = get_
+00002a60: 7665 7273 696f 6e28 290a 6060 600a 0a23  version().```..#
+00002a70: 2320 486f 7720 7468 6520 706c 7567 696e  # How the plugin
+00002a80: 2077 6f72 6b73 0a0a 506f 6574 7279 2072   works..Poetry r
+00002a90: 756e 7320 7468 6520 706c 7567 696e 2077  uns the plugin w
+00002aa0: 6865 6e20 6275 696c 6469 6e67 2061 2070  hen building a p
+00002ab0: 6163 6b61 6765 2c20 616e 6420 6974 2073  ackage, and it s
+00002ac0: 6574 7320 7468 6520 7665 7273 696f 6e20  ets the version 
+00002ad0: 7269 6768 7420 6265 666f 7265 2063 7265  right before cre
+00002ae0: 6174 696e 6720 7468 6520 2270 6163 6b61  ating the "packa
+00002af0: 6765 2064 6973 7472 6962 7574 6162 6c65  ge distributable
+00002b00: 2220 2865 2e67 2e2c 2074 6865 2077 6865  " (e.g., the whe
+00002b10: 656c 292e 0a0a 2323 2320 486f 7720 7468  el)...### How th
+00002b20: 6520 7665 7273 696f 6e20 7661 7269 6162  e version variab
+00002b30: 6c65 2077 6f72 6b73 0a0a 4966 2079 6f75  le works..If you
+00002b40: 2068 6176 6520 6120 7061 636b 6167 6520   have a package 
+00002b50: 2861 2073 696e 676c 6520 7061 636b 6167  (a single packag
+00002b60: 6529 2064 6563 6c61 7265 6420 696e 2074  e) declared in t
+00002b70: 6865 2060 7061 636b 6167 6573 6020 636f  he `packages` co
+00002b80: 6e66 6967 2069 6e20 796f 7572 2060 7079  nfig in your `py
+00002b90: 7072 6f6a 6563 742e 746f 6d6c 602c 2074  project.toml`, t
+00002ba0: 6865 2070 6c75 6769 6e20 7769 6c6c 2075  he plugin will u
+00002bb0: 7365 2074 6861 7420 7061 636b 6167 6527  se that package'
+00002bc0: 7320 605f 5f69 6e69 745f 5f2e 7079 6020  s `__init__.py` 
+00002bd0: 746f 2066 696e 6420 7468 6520 605f 5f76  to find the `__v
+00002be0: 6572 7369 6f6e 5f5f 6020 7661 7269 6162  ersion__` variab
+00002bf0: 6c65 2e0a 0a49 6620 796f 7520 646f 6e27  le...If you don'
+00002c00: 7420 6861 7665 2061 6e79 2060 7061 636b  t have any `pack
+00002c10: 6167 6573 6020 636f 6e66 6967 2c20 7468  ages` config, th
+00002c20: 6520 706c 7567 696e 2077 696c 6c20 6173  e plugin will as
+00002c30: 7375 6d65 2074 6861 7420 796f 7520 6861  sume that you ha
+00002c40: 7665 2061 2073 696e 676c 6520 7061 636b  ve a single pack
+00002c50: 6167 6520 6e61 6d65 6420 6173 2079 6f75  age named as you
+00002c60: 7220 7072 6f6a 6563 742c 2062 7574 2069  r project, but i
+00002c70: 6e20 7468 6520 6d6f 6475 6c65 2076 6572  n the module ver
+00002c80: 7369 6f6e 2028 6368 616e 6769 6e67 2060  sion (changing `
+00002c90: 2d60 2066 6f72 2060 5f60 292e 2053 6f2c  -` for `_`). So,
+00002ca0: 2069 6620 796f 7572 2070 6163 6b61 6765   if your package
+00002cb0: 2069 7320 606d 792d 6177 6573 6f6d 652d   is `my-awesome-
+00002cc0: 7072 6f6a 6563 7460 2c20 7468 6520 706c  project`, the pl
+00002cd0: 7567 696e 2077 696c 6c20 7573 6520 7468  ugin will use th
+00002ce0: 6520 6669 6c65 2061 7420 606d 795f 6177  e file at `my_aw
+00002cf0: 6573 6f6d 655f 7072 6f6a 6563 742f 5f5f  esome_project/__
+00002d00: 696e 6974 5f5f 2e70 7960 2074 6f20 6669  init__.py` to fi
+00002d10: 6e64 2074 6865 2060 5f5f 7665 7273 696f  nd the `__versio
+00002d20: 6e5f 5f60 2076 6172 6961 626c 652e 0a0a  n__` variable...
+00002d30: 5468 6973 2066 696c 6520 7374 7275 6374  This file struct
+00002d40: 7572 6520 6973 2074 6865 2064 6566 6175  ure is the defau
+00002d50: 6c74 2069 6620 796f 7520 6372 6561 7465  lt if you create
+00002d60: 2061 206e 6577 2070 726f 6a65 6374 2077   a new project w
+00002d70: 6974 6820 7468 6520 636f 6d6d 616e 6420  ith the command 
+00002d80: 6070 6f65 7472 7920 6e65 7760 2c20 736f  `poetry new`, so
+00002d90: 2069 7420 7368 6f75 6c64 2077 6f72 6b20   it should work 
+00002da0: 6173 2065 7870 6563 7465 642e 20e2 9ca8  as expected. ...
+00002db0: 0a0a 5468 6520 7761 7920 7468 6520 706c  ..The way the pl
+00002dc0: 7567 696e 2077 6f72 6b73 2069 6e74 6572  ugin works inter
+00002dd0: 6e61 6c6c 7920 6973 2062 7920 7061 7273  nally is by pars
+00002de0: 696e 6720 7468 6520 605f 5f69 6e69 745f  ing the `__init_
+00002df0: 5f2e 7079 6020 6669 6c65 2e20 5265 6164  _.py` file. Read
+00002e00: 696e 6720 7468 6520 5079 7468 6f6e 2773  ing the Python's
+00002e10: 2022 4162 7374 7261 6374 2053 796e 7461   "Abstract Synta
+00002e20: 7820 5472 6565 2220 7573 696e 6720 7468  x Tree" using th
+00002e30: 6520 6061 7374 6020 7374 616e 6461 7264  e `ast` standard
+00002e40: 206d 6f64 756c 6520 616e 6420 6578 7472   module and extr
+00002e50: 6163 7469 6e67 2074 6865 206c 6974 6572  acting the liter
+00002e60: 616c 2076 616c 7565 206f 6620 7468 6520  al value of the 
+00002e70: 7374 7269 6e67 2e20 536f 2c20 6974 2064  string. So, it d
+00002e80: 6f65 736e 2774 2065 7865 6375 7465 2074  oesn't execute t
+00002e90: 6865 2063 6f64 6520 696e 2060 5f5f 696e  he code in `__in
+00002ea0: 6974 5f5f 2e70 7960 2c20 6974 206f 6e6c  it__.py`, it onl
+00002eb0: 7920 7265 6164 7320 6974 2061 7320 5079  y reads it as Py
+00002ec0: 7468 6f6e 2063 6f64 652e 0a0a 5468 6520  thon code...The 
+00002ed0: 706c 7567 696e 2064 6f65 736e 2774 2074  plugin doesn't t
+00002ee0: 7279 2074 6f20 696d 706f 7274 2061 6e64  ry to import and
+00002ef0: 2065 7865 6375 7465 2074 6861 7420 605f   execute that `_
+00002f00: 5f69 6e69 745f 5f2e 7079 6020 6669 6c65  _init__.py` file
+00002f10: 2062 6563 6175 7365 2074 6861 7420 636f   because that co
+00002f20: 756c 6420 7265 7175 6972 6520 6578 7472  uld require extr
+00002f30: 6120 636f 6d70 7574 6174 696f 6e2c 2065  a computation, e
+00002f40: 7874 6572 6e61 6c20 6465 7065 6e64 656e  xternal dependen
+00002f50: 6369 6573 2c20 6574 632e 2041 6e64 2069  cies, etc. And i
+00002f60: 7420 646f 6573 6e27 7420 7472 7920 746f  t doesn't try to
+00002f70: 2065 7874 7261 6374 2074 6865 2060 5f5f   extract the `__
+00002f80: 7665 7273 696f 6e5f 5f60 2077 6974 6820  version__` with 
+00002f90: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00002fa0: 6f6e 732c 2061 7320 7468 6174 2077 6f75  ons, as that wou
+00002fb0: 6c64 2062 6520 7072 6f6e 6520 746f 2065  ld be prone to e
+00002fc0: 7272 6f72 7320 6966 2c20 666f 7220 6578  rrors if, for ex
+00002fd0: 616d 706c 652c 2074 6865 7265 2077 6173  ample, there was
+00002fe0: 2073 6f6d 6520 6f74 6865 7220 605f 5f76   some other `__v
+00002ff0: 6572 7369 6f6e 5f5f 6020 736f 6d65 7768  ersion__` somewh
+00003000: 6572 6520 696e 2074 6865 2063 6f64 652c  ere in the code,
+00003010: 2069 6e20 6120 636f 6d6d 656e 7420 6f72   in a comment or
+00003020: 2069 6e73 6964 6520 6120 7374 7269 6e67   inside a string
+00003030: 2e0a 0a23 2320 5761 726e 696e 670a 0af0  ...## Warning...
+00003040: 9f9a a820 436f 6e73 6964 6572 2074 6869  ... Consider thi
+00003050: 7320 696e 2074 6865 2061 6c70 6861 2073  s in the alpha s
+00003060: 7461 6765 2e20 506f 6574 7279 2060 312e  tage. Poetry `1.
+00003070: 322e 3061 3160 2077 6974 6820 7375 7070  2.0a1` with supp
+00003080: 6f72 7420 666f 7220 706c 7567 696e 7320  ort for plugins 
+00003090: 7761 7320 7265 6c65 6173 6564 206f 6e20  was released on 
+000030a0: 3230 3231 2d30 352d 3231 2e20 4920 7374  2021-05-21. I st
+000030b0: 6172 7465 6420 7772 6974 696e 6720 7468  arted writing th
+000030c0: 6973 2070 6c75 6769 6e20 3320 6461 7973  is plugin 3 days
+000030d0: 206c 6174 6572 2c20 6f6e 2032 3032 312d   later, on 2021-
+000030e0: 3035 2d32 342e 0a0a 5468 696e 6773 206d  05-24...Things m
+000030f0: 6967 6874 2062 7265 616b 2069 6e20 506f  ight break in Po
+00003100: 6574 7279 206f 7220 696e 2074 6869 7320  etry or in this 
+00003110: 706c 7567 696e 2e20 536f 2c20 706c 6561  plugin. So, plea
+00003120: 7365 2074 7279 2069 7420 616e 6420 7465  se try it and te
+00003130: 7374 2069 7420 7665 7279 2063 6172 6566  st it very caref
+00003140: 756c 6c79 2062 6566 6f72 6520 6675 6c6c  ully before full
+00003150: 7920 6164 6f70 7469 6e67 2069 7420 666f  y adopting it fo
+00003160: 7220 6465 6c69 6361 7465 2073 7973 7465  r delicate syste
+00003170: 6d73 2e0a 0a54 6865 2077 6179 2069 7420  ms...The way it 
+00003180: 776f 726b 7320 6d69 6768 7420 6368 616e  works might chan
+00003190: 6765 2c20 616e 6420 7468 6520 7370 6563  ge, and the spec
+000031a0: 6966 6963 2063 6f6e 6669 6775 7261 7469  ific configurati
+000031b0: 6f6e 206d 6967 6874 2063 6861 6e67 652e  on might change.
+000031c0: 0a0a 416c 736f 2c20 6966 2079 6f75 2064  ..Also, if you d
+000031d0: 6f6e 2774 2066 696e 6420 7468 6520 666f  on't find the fo
+000031e0: 6c6c 6f77 696e 6720 7365 6374 696f 6e73  llowing sections
+000031f0: 2069 6e74 7569 7469 7665 3a0a 0a60 6060   intuitive:..```
+00003200: 746f 6d6c 0a5b 746f 6f6c 2e70 6f65 7472  toml.[tool.poetr
+00003210: 792d 7665 7273 696f 6e2d 706c 7567 696e  y-version-plugin
+00003220: 5d0a 736f 7572 6365 203d 2022 696e 6974  ].source = "init
+00003230: 220a 6060 600a 0a61 6e64 0a0a 6060 6074  ".```..and..```t
+00003240: 6f6d 6c0a 5b74 6f6f 6c2e 706f 6574 7279  oml.[tool.poetry
+00003250: 2d76 6572 7369 6f6e 2d70 6c75 6769 6e5d  -version-plugin]
+00003260: 0a73 6f75 7263 6520 3d20 2267 6974 2d74  .source = "git-t
+00003270: 6167 220a 6060 600a 0a6c 6574 206d 6520  ag".```..let me 
+00003280: 6b6e 6f77 2077 6861 7420 616c 7465 726e  know what altern
+00003290: 6174 6976 6520 636f 6e66 6967 7572 6174  ative configurat
+000032a0: 696f 6e20 776f 756c 6420 6d61 6b65 206d  ion would make m
+000032b0: 6f72 6520 7365 6e73 6520 616e 6420 6265  ore sense and be
+000032c0: 206d 6f72 6520 696e 7475 6974 6976 6520   more intuitive 
+000032d0: 746f 2079 6f75 2e0a 0af0 9f91 8d20 5468  to you....... Th
+000032e0: 6520 676f 6f64 206e 6577 7320 6973 2c20  e good news is, 
+000032f0: 6173 7375 6d69 6e67 2079 6f75 2061 7265  assuming you are
+00003300: 2062 7569 6c64 696e 6720 7061 636b 6167   building packag
+00003310: 6573 2074 6f20 7468 656e 2075 706c 6f61  es to then uploa
+00003320: 6420 7468 656d 2074 6f20 5079 5049 2066  d them to PyPI f
+00003330: 6f72 2079 6f75 7220 7573 6572 7320 746f  or your users to
+00003340: 2064 6f77 6e6c 6f61 6420 616e 6420 7573   download and us
+00003350: 6520 7468 656d 2c20 7468 6520 2a2a 776f  e them, the **wo
+00003360: 7273 7420 7468 6174 2063 6f75 6c64 2068  rst that could h
+00003370: 6170 7065 6e2a 2a20 6966 2073 6f6d 6574  appen** if somet
+00003380: 6869 6e67 2062 726f 6b65 2069 7320 7468  hing broke is th
+00003390: 6174 2079 6f75 2077 6f75 6c64 6e27 7420  at you wouldn't 
+000033a0: 6265 2061 626c 6520 746f 2062 7569 6c64  be able to build
+000033b0: 2061 206e 6577 2076 6572 7369 6f6e 2075   a new version u
+000033c0: 6e74 696c 2073 6f6d 6574 6869 6e67 2069  ntil something i
+000033d0: 7320 6669 7865 6420 6f72 2063 6861 6e67  s fixed or chang
+000033e0: 6564 2e20 4275 7420 796f 7572 2075 7365  ed. But your use
+000033f0: 7273 2073 686f 756c 646e 2774 2062 6520  rs shouldn't be 
+00003400: 6166 6665 6374 6564 2069 6e20 616e 7920  affected in any 
+00003410: 7761 792e 0a0a 2323 2052 656c 6561 7365  way...## Release
+00003420: 204e 6f74 6573 0a0a 2323 2320 4c61 7465   Notes..### Late
+00003430: 7374 2043 6861 6e67 6573 0a0a 0a23 2323  st Changes...###
+00003440: 2030 2e32 2e30 0a0a 2a20 e29c a820 4164   0.2.0..* ... Ad
+00003450: 6420 7375 7070 6f72 7420 666f 7220 506f  d support for Po
+00003460: 6574 7279 2031 2e32 2e30 2061 6e64 2061  etry 1.2.0 and a
+00003470: 626f 7665 2028 696e 636c 7564 696e 6720  bove (including 
+00003480: 312e 352e 3129 2c20 6465 7072 6563 6174  1.5.1), deprecat
+00003490: 6520 7375 7070 6f72 7420 666f 7220 5079  e support for Py
+000034a0: 7468 6f6e 2033 2e36 2e20 5052 205b 2332  thon 3.6. PR [#2
+000034b0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+000034c0: 622e 636f 6d2f 7469 616e 676f 6c6f 2f70  b.com/tiangolo/p
+000034d0: 6f65 7472 792d 7665 7273 696f 6e2d 706c  oetry-version-pl
+000034e0: 7567 696e 2f70 756c 6c2f 3238 2920 6279  ugin/pull/28) by
+000034f0: 205b 406d 6265 6163 6f6d 5d28 6874 7470   [@mbeacom](http
+00003500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00003510: 6265 6163 6f6d 292e 0a2a 20e2 9c8f efb8  beacom)..* .....
+00003520: 8f20 4669 7820 7479 706f 7320 616e 6420  . Fix typos and 
+00003530: 7265 776f 7264 696e 6720 696e 2052 4541  rewording in REA
+00003540: 444d 452e 6d64 2e20 5052 205b 2338 5d28  DME.md. PR [#8](
+00003550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003560: 6f6d 2f74 6961 6e67 6f6c 6f2f 706f 6574  om/tiangolo/poet
+00003570: 7279 2d76 6572 7369 6f6e 2d70 6c75 6769  ry-version-plugi
+00003580: 6e2f 7075 6c6c 2f38 2920 6279 205b 4047  n/pull/8) by [@G
+00003590: 6c30 6465 616e 525d 2868 7474 7073 3a2f  l0deanR](https:/
+000035a0: 2f67 6974 6875 622e 636f 6d2f 476c 3064  /github.com/Gl0d
+000035b0: 6561 6e52 292e 0a0a 2323 2320 302e 312e  eanR)...### 0.1.
+000035c0: 330a 0a2a 20e2 9ca8 2049 6d70 726f 7665  3..* ... Improve
+000035d0: 206c 6f67 732c 2070 7265 6669 7820 7769   logs, prefix wi
+000035e0: 7468 2070 6c75 6769 6e20 6e61 6d65 2e20  th plugin name. 
+000035f0: 5052 205b 2336 5d28 6874 7470 733a 2f2f  PR [#6](https://
+00003600: 6769 7468 7562 2e63 6f6d 2f74 6961 6e67  github.com/tiang
+00003610: 6f6c 6f2f 706f 6574 7279 2d76 6572 7369  olo/poetry-versi
+00003620: 6f6e 2d70 6c75 6769 6e2f 7075 6c6c 2f36  on-plugin/pull/6
+00003630: 2920 6279 205b 4074 6961 6e67 6f6c 6f5d  ) by [@tiangolo]
+00003640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003650: 636f 6d2f 7469 616e 676f 6c6f 292e 0a2a  com/tiangolo)..*
+00003660: 20f0 9f94 a720 5570 6461 7465 2070 7970   .... Update pyp
+00003670: 726f 6a65 6374 206d 6574 6164 6174 612e  roject metadata.
+00003680: 2050 5220 5b23 355d 2868 7474 7073 3a2f   PR [#5](https:/
+00003690: 2f67 6974 6875 622e 636f 6d2f 7469 616e  /github.com/tian
+000036a0: 676f 6c6f 2f70 6f65 7472 792d 7665 7273  golo/poetry-vers
+000036b0: 696f 6e2d 706c 7567 696e 2f70 756c 6c2f  ion-plugin/pull/
+000036c0: 3529 2062 7920 5b40 7469 616e 676f 6c6f  5) by [@tiangolo
+000036d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000036e0: 2e63 6f6d 2f74 6961 6e67 6f6c 6f29 2e0a  .com/tiangolo)..
+000036f0: 2a20 e29c 8520 4669 7820 636f 7665 7261  * ... Fix covera
+00003700: 6765 2e20 5052 205b 2334 5d28 6874 7470  ge. PR [#4](http
+00003710: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00003720: 6961 6e67 6f6c 6f2f 706f 6574 7279 2d76  iangolo/poetry-v
+00003730: 6572 7369 6f6e 2d70 6c75 6769 6e2f 7075  ersion-plugin/pu
+00003740: 6c6c 2f34 2920 6279 205b 4074 6961 6e67  ll/4) by [@tiang
+00003750: 6f6c 6f5d 2868 7474 7073 3a2f 2f67 6974  olo](https://git
+00003760: 6875 622e 636f 6d2f 7469 616e 676f 6c6f  hub.com/tiangolo
+00003770: 292e 0a2a 20f0 9f93 9d20 496d 7072 6f76  )..* .... Improv
+00003780: 6520 646f 6373 2e20 5052 205b 2333 5d28  e docs. PR [#3](
+00003790: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000037a0: 6f6d 2f74 6961 6e67 6f6c 6f2f 706f 6574  om/tiangolo/poet
+000037b0: 7279 2d76 6572 7369 6f6e 2d70 6c75 6769  ry-version-plugi
+000037c0: 6e2f 7075 6c6c 2f33 2920 6279 205b 4074  n/pull/3) by [@t
+000037d0: 6961 6e67 6f6c 6f5d 2868 7474 7073 3a2f  iangolo](https:/
+000037e0: 2f67 6974 6875 622e 636f 6d2f 7469 616e  /github.com/tian
+000037f0: 676f 6c6f 292e 0a2a 20f0 9f90 9b20 4669  golo)..* .... Fi
+00003800: 7820 7465 7374 7320 666f 7220 4349 2e20  x tests for CI. 
+00003810: 5052 205b 2331 5d28 6874 7470 733a 2f2f  PR [#1](https://
+00003820: 6769 7468 7562 2e63 6f6d 2f74 6961 6e67  github.com/tiang
+00003830: 6f6c 6f2f 706f 6574 7279 2d76 6572 7369  olo/poetry-versi
+00003840: 6f6e 2d70 6c75 6769 6e2f 7075 6c6c 2f31  on-plugin/pull/1
+00003850: 2920 6279 205b 4074 6961 6e67 6f6c 6f5d  ) by [@tiangolo]
+00003860: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003870: 636f 6d2f 7469 616e 676f 6c6f 292e 0a2a  com/tiangolo)..*
+00003880: 20f0 9f91 b720 4669 7820 4c61 7465 7374   .... Fix Latest
+00003890: 2043 6861 6e67 6573 2061 6374 696f 6e2c   Changes action,
+000038a0: 2073 6574 2062 7261 6e63 6820 746f 206d   set branch to m
+000038b0: 6169 6e2e 2050 5220 5b23 325d 2868 7474  ain. PR [#2](htt
+000038c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000038d0: 7469 616e 676f 6c6f 2f70 6f65 7472 792d  tiangolo/poetry-
+000038e0: 7665 7273 696f 6e2d 706c 7567 696e 2f70  version-plugin/p
+000038f0: 756c 6c2f 3229 2062 7920 5b40 7469 616e  ull/2) by [@tian
+00003900: 676f 6c6f 5d28 6874 7470 733a 2f2f 6769  golo](https://gi
+00003910: 7468 7562 2e63 6f6d 2f74 6961 6e67 6f6c  thub.com/tiangol
+00003920: 6f29 2e0a 0a23 2320 4c69 6365 6e73 650a  o)...## License.
+00003930: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
+00003940: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
+00003950: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
+00003960: 204d 4954 206c 6963 656e 7365 2e0a 0a     MIT license...
```

