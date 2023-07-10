# Comparing `tmp/findpython-0.2.5.tar.gz` & `tmp/findpython-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpython-0.2.5.tar", last modified: Wed May 10 08:28:07 2023, max compression
+gzip compressed data
```

## Comparing `findpython-0.2.5.tar` & `findpython-1.0.0a0.tar`

### file list

```diff
@@ -1,27 +1,21 @@
--rw-r--r--   0        0        0     1075 2023-05-10 08:27:49.053817 findpython-0.2.5/LICENSE
--rw-r--r--   0        0        0     4389 2023-05-10 08:27:49.053817 findpython-0.2.5/README.md
--rw-r--r--   0        0        0     1291 2023-05-10 08:27:49.053817 findpython-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1474 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__init__.py
--rw-r--r--   0        0        0     2335 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__main__.py
--rw-r--r--   0        0        0       22 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__version__.py
--rw-r--r--   0        0        0     6201 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/finder.py
--rw-r--r--   0        0        0      442 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/__init__.py
--rw-r--r--   0        0        0      254 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/__main__.py
--rw-r--r--   0        0        0     6631 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/_registry.py
--rw-r--r--   0        0        0     4637 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/environment.py
--rw-r--r--   0        0        0      724 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/__init__.py
--rw-r--r--   0        0        0     1078 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/asdf.py
--rw-r--r--   0        0        0     1555 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/base.py
--rw-r--r--   0        0        0      779 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/macos.py
--rw-r--r--   0        0        0      682 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/path.py
--rw-r--r--   0        0        0     1269 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/pep514.py
--rw-r--r--   0        0        0     1092 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/pyenv.py
--rw-r--r--   0        0        0     6344 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/python.py
--rw-r--r--   0        0        0     4056 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1689 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0      613 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_cli.py
--rw-r--r--   0        0        0     4814 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_finder.py
--rw-r--r--   0        0        0     1489 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_posix.py
--rw-r--r--   0        0        0      681 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_utils.py
--rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 findpython-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 findpython-1.0.0a0/Cargo.toml
+-rw-r--r--   0      501       20     3863 2023-07-10 10:24:01.000000 findpython-1.0.0a0/.github/workflows/build.yaml
+-rw-r--r--   0      501       20       92 2023-07-10 10:24:01.000000 findpython-1.0.0a0/.gitignore
+-rw-r--r--   0      501       20    20768 2023-07-10 10:24:01.000000 findpython-1.0.0a0/Cargo.lock
+-rw-r--r--   0      501       20     1075 2023-07-10 10:24:01.000000 findpython-1.0.0a0/LICENSE
+-rw-r--r--   0      501       20     5118 2023-07-10 10:24:01.000000 findpython-1.0.0a0/README.md
+-rw-r--r--   0      501       20     2056 2023-07-10 10:24:01.000000 findpython-1.0.0a0/findpython.pyi
+-rw-r--r--   0      501       20     4121 2023-07-10 10:24:01.000000 findpython-1.0.0a0/pdm.lock
+-rw-r--r--   0      501       20      762 2023-07-10 10:24:01.000000 findpython-1.0.0a0/pyproject.toml
+-rw-r--r--   0      501       20     2849 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/cli.rs
+-rw-r--r--   0      501       20     8831 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/finder.rs
+-rw-r--r--   0      501       20     2354 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/helpers.rs
+-rw-r--r--   0      501       20      662 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/lib.rs
+-rw-r--r--   0      501       20      130 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/main.rs
+-rw-r--r--   0      501       20     1688 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/asdf.rs
+-rw-r--r--   0      501       20     2003 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/mod.rs
+-rw-r--r--   0      501       20     1110 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/path.rs
+-rw-r--r--   0      501       20     1662 2023-07-10 10:24:01.000000 findpython-1.0.0a0/src/providers/pyenv.rs
+-rw-r--r--   0      501       20     1306 2023-07-10 10:24:02.000000 findpython-1.0.0a0/src/providers/rye.rs
+-rw-r--r--   0      501       20    14411 2023-07-10 10:24:02.000000 findpython-1.0.0a0/src/python.rs
+-rw-r--r--   0        0        0     5586 1970-01-01 00:00:00.000000 findpython-1.0.0a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `findpython-0.2.5/LICENSE` & `findpython-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-0.2.5/README.md` & `findpython-1.0.0a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,29 +13,43 @@
 It simplifies the whole code structure while preserving most of the original features.
 
 [pythonfinder]: https://github.com/sarugaku/pythonfinder
 [techalchemy]: https://github.com/techalchemy
 
 ## Installation
 
-FindPython is installable via any kind of package manager including `pip`:
+FindPython can be used in both Python and Rust projects.
+
+To install FindPython in Python:
 
 ```bash
 pip install findpython
 ```
 
+To install FindPython in Rust:
+
+```bash
+cargo install findpyhton
+```
+
+Or use FindPython library in a Rust project:
+
+```bash
+cargo add findpython
+```
+
 <details>
 <summary>Expand this section to see findpython's availability in the package ecosystem</summary>
 
 <a href="https://repology.org/project/python:findpython/versions">
     <img src="https://repology.org/badge/vertical-allrepos/python:findpython.svg?header=python%3Afindpython" alt="Packaging status">
 </a>
 </details>
 
-## Usage
+## Python Usage
 
 ```python
 >>> import findpython
 >>> findpython.find(3, 9)  # Find by major and minor version
 <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
 >>> findpython.find("3.9")  # Find by version string
 <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
@@ -45,42 +59,63 @@
 <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
 >>> findpython.find("python3")  # Find by executable name without keyword argument, same as above
 <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
 >>> findpython.find_all(major=3, minor=9)  # Same arguments as `find()`, but return all matches
 [<PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/cmd/python3.9'), version=<Version('3.9.9')>, architecture='64bit', major=3, minor=9, patch=9>, <PythonVersion executable=PosixPath('/usr/local/bin/python3.9'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>, <PythonVersion executable=PosixPath('/usr/local/bin/python3'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>]
 ```
 
+## Rust Usage
+
+```rust
+use findpython::Finder;
+
+fn main() {
+    let finder = Finder::default();
+
+    // Find by major and minor version
+    let py = finder.find(3, 9).unwrap();
+    println!("{:?}", py);
+    // Find all matches
+    let all_pythons = finder.find_all();
+    println!("{:?}", all_pythons);
+}
+```
+
 ## CLI Usage
 
 In addition, FindPython provides a CLI interface to find python versions:
 
 ```
-usage: findpython [-h] [-V] [-a] [--resolve-symlink] [-v] [--no-same-file] [--no-same-python] [version_spec]
+Find python executables on your system
 
-Find python files in a directory
+Usage: findpython [OPTIONS] [VERSION_SPEC]
 
-positional arguments:
-  version_spec       Python version spec or name
+Arguments:
+  [VERSION_SPEC]  The version spec to find, e.g. 3|3.8|python3
 
-options:
-  -h, --help         show this help message and exit
-  -V, --version      show program's version number and exit
-  -a, --all          Show all matching python versions
-  --resolve-symlink  Resolve all symlinks
-  -v, --verbose      Verbose output
-  --no-same-file     Eliminate the duplicated results with the same file contents
-  --no-same-python   Eliminate the duplicated results with the same sys.executable
+Options:
+  -a, --all                    Return all matching Python versions
+      --resolve-symlinks       Resolve symlinks and remove duplicate results
+      --no-same-file           Remove duplicate results that are the same binary
+      --no-same-python         Remove duplicate results that wrap the same Python interpreter
+      --providers <PROVIDERS>  Select provider names(comma-separated) to use
+  -o, --output <OUTPUT>        The output format [default: default] [possible values: default, json, path]
+  -h, --help                   Print help
+  -V, --version                Print version
 ```
 
 ## Integration
 
 FindPython finds Python from the following places:
 
 -   `PATH` environment variable
 -   pyenv
 -   asdf
--   `/Library/Frameworks/Python.framework/Versions` (MacOS)
--   winreg (Windows)
+-   winreg (Windows) (🚧 WIP 🚧)
+-   [Rye] project manager backed by [python-build-standalone]
+
+[rye]: https://rye-up.com
+[python-build-standalone]: https://github.com/indygreg/python-build-standalone
 
 ## License
 
 FindPython is released under MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -7,36 +7,44 @@
 pypi/pyversions/findpython?logo=python&logoColor=%23cccccc&style=flat-square)]
 (https://pypi.org/project/findpython) [![pdm-managed](https://img.shields.io/
 badge/pdm-managed-blueviolet?style=flat-square)](https://github.com/frostming/
 findpython) ## Description This library is a rewrite of [pythonfinder] project
 by [@techalchemy][techalchemy]. It simplifies the whole code structure while
 preserving most of the original features. [pythonfinder]: https://github.com/
 sarugaku/pythonfinder [techalchemy]: https://github.com/techalchemy ##
-Installation FindPython is installable via any kind of package manager
-including `pip`: ```bash pip install findpython ```  Expand this section to see
-findpython's availability in the package ecosystem [Packaging_status]  ## Usage
-```python >>> import findpython >>> findpython.find(3, 9) # Find by major and
-minor version , architecture='64bit', major=3, minor=9, patch=10> >>>
-findpython.find("3.9") # Find by version string , architecture='64bit',
-major=3, minor=9, patch=10> >>> findpython.find("3.9-32") # Find by version
-string and architecture , architecture='32bit', major=3, minor=9, patch=10> >>>
-findpython.find(name="python3") # Find by executable name ,
-architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find
+Installation FindPython can be used in both Python and Rust projects. To
+install FindPython in Python: ```bash pip install findpython ``` To install
+FindPython in Rust: ```bash cargo install findpyhton ``` Or use FindPython
+library in a Rust project: ```bash cargo add findpython ```  Expand this
+section to see findpython's availability in the package ecosystem [Packaging
+status]  ## Python Usage ```python >>> import findpython >>> findpython.find(3,
+9) # Find by major and minor version , architecture='64bit', major=3, minor=9,
+patch=10> >>> findpython.find("3.9") # Find by version string ,
+architecture='64bit', major=3, minor=9, patch=10> >>> findpython.find("3.9-32")
+# Find by version string and architecture , architecture='32bit', major=3,
+minor=9, patch=10> >>> findpython.find(name="python3") # Find by executable
+name , architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find
 ("python3") # Find by executable name without keyword argument, same as above ,
 architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find_all
 (major=3, minor=9) # Same arguments as `find()`, but return all matches [,
 architecture='64bit', major=3, minor=9, patch=10>, , architecture='64bit',
 major=3, minor=9, patch=10>, , architecture='64bit', major=3, minor=9,
 patch=9>, , architecture='64bit', major=3, minor=9, patch=5>, ,
-architecture='64bit', major=3, minor=9, patch=5>] ``` ## CLI Usage In addition,
-FindPython provides a CLI interface to find python versions: ``` usage:
-findpython [-h] [-V] [-a] [--resolve-symlink] [-v] [--no-same-file] [--no-same-
-python] [version_spec] Find python files in a directory positional arguments:
-version_spec Python version spec or name options: -h, --help show this help
-message and exit -V, --version show program's version number and exit -a, --all
-Show all matching python versions --resolve-symlink Resolve all symlinks -v, --
-verbose Verbose output --no-same-file Eliminate the duplicated results with the
-same file contents --no-same-python Eliminate the duplicated results with the
-same sys.executable ``` ## Integration FindPython finds Python from the
-following places: - `PATH` environment variable - pyenv - asdf - `/Library/
-Frameworks/Python.framework/Versions` (MacOS) - winreg (Windows) ## License
-FindPython is released under MIT License.
+architecture='64bit', major=3, minor=9, patch=5>] ``` ## Rust Usage ```rust use
+findpython::Finder; fn main() { let finder = Finder::default(); // Find by
+major and minor version let py = finder.find(3, 9).unwrap(); println!("{:?}",
+py); // Find all matches let all_pythons = finder.find_all(); println!("{:?}",
+all_pythons); } ``` ## CLI Usage In addition, FindPython provides a CLI
+interface to find python versions: ``` Find python executables on your system
+Usage: findpython [OPTIONS] [VERSION_SPEC] Arguments: [VERSION_SPEC] The
+version spec to find, e.g. 3|3.8|python3 Options: -a, --all Return all matching
+Python versions --resolve-symlinks Resolve symlinks and remove duplicate
+results --no-same-file Remove duplicate results that are the same binary --no-
+same-python Remove duplicate results that wrap the same Python interpreter --
+providers  Select provider names(comma-separated) to use -o, --output  The
+output format [default: default] [possible values: default, json, path] -h, --
+help Print help -V, --version Print version ``` ## Integration FindPython finds
+Python from the following places: - `PATH` environment variable - pyenv - asdf
+- winreg (Windows) (ð§ WIP ð§) - [Rye] project manager backed by [python-
+build-standalone] [rye]: https://rye-up.com [python-build-standalone]: https://
+github.com/indygreg/python-build-standalone ## License FindPython is released
+under MIT License.
```

### Comparing `findpython-0.2.5/PKG-INFO` & `findpython-1.0.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: findpython
-Version: 0.2.5
+Version: 1.0.0a0
+Requires-Dist: pep440-rs >=0.3.11 ; extra == 'types'
+Provides-Extra: types
+License-File: LICENSE
 Summary: A utility to find python versions on your system
-License: MIT
+Author: Frost Ming <me@frostming.com>
 Author-email: Frost Ming <mianghong@gmail.com>
+License: MIT
 Requires-Python: >=3.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Project-URL: Homepage, https://github.com/frostming/findpython
-Description-Content-Type: text/markdown
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/frostming/findpython
 
 # FindPython
 
 _A utility to find python versions on your system._
 
 [![Tests](https://github.com/frostming/findpython/actions/workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/workflows/ci.yml)
 [![PyPI](https://img.shields.io/pypi/v/findpython?logo=python&logoColor=%23cccccc&style=flat-square)](https://pypi.org/project/findpython)
@@ -28,29 +27,43 @@
 It simplifies the whole code structure while preserving most of the original features.
 
 [pythonfinder]: https://github.com/sarugaku/pythonfinder
 [techalchemy]: https://github.com/techalchemy
 
 ## Installation
 
-FindPython is installable via any kind of package manager including `pip`:
+FindPython can be used in both Python and Rust projects.
+
+To install FindPython in Python:
 
 ```bash
 pip install findpython
 ```
 
+To install FindPython in Rust:
+
+```bash
+cargo install findpyhton
+```
+
+Or use FindPython library in a Rust project:
+
+```bash
+cargo add findpython
+```
+
 <details>
 <summary>Expand this section to see findpython's availability in the package ecosystem</summary>
 
 <a href="https://repology.org/project/python:findpython/versions">
     <img src="https://repology.org/badge/vertical-allrepos/python:findpython.svg?header=python%3Afindpython" alt="Packaging status">
 </a>
 </details>
 
-## Usage
+## Python Usage
 
 ```python
 >>> import findpython
 >>> findpython.find(3, 9)  # Find by major and minor version
 <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
 >>> findpython.find("3.9")  # Find by version string
 <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>
@@ -60,43 +73,64 @@
 <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
 >>> findpython.find("python3")  # Find by executable name without keyword argument, same as above
 <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/bin/python3'), version=<Version('3.10.2')>, architecture='64bit', major=3, minor=10, patch=2>
 >>> findpython.find_all(major=3, minor=9)  # Same arguments as `find()`, but return all matches
 [<PythonVersion executable=PosixPath('/opt/homebrew/bin/python3.9'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/opt/homebrew/bin/python3'), version=<Version('3.9.10')>, architecture='64bit', major=3, minor=9, patch=10>, <PythonVersion executable=PosixPath('/Users/fming/Library/PythonUp/cmd/python3.9'), version=<Version('3.9.9')>, architecture='64bit', major=3, minor=9, patch=9>, <PythonVersion executable=PosixPath('/usr/local/bin/python3.9'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>, <PythonVersion executable=PosixPath('/usr/local/bin/python3'), version=<Version('3.9.5')>, architecture='64bit', major=3, minor=9, patch=5>]
 ```
 
+## Rust Usage
+
+```rust
+use findpython::Finder;
+
+fn main() {
+    let finder = Finder::default();
+
+    // Find by major and minor version
+    let py = finder.find(3, 9).unwrap();
+    println!("{:?}", py);
+    // Find all matches
+    let all_pythons = finder.find_all();
+    println!("{:?}", all_pythons);
+}
+```
+
 ## CLI Usage
 
 In addition, FindPython provides a CLI interface to find python versions:
 
 ```
-usage: findpython [-h] [-V] [-a] [--resolve-symlink] [-v] [--no-same-file] [--no-same-python] [version_spec]
+Find python executables on your system
 
-Find python files in a directory
+Usage: findpython [OPTIONS] [VERSION_SPEC]
 
-positional arguments:
-  version_spec       Python version spec or name
+Arguments:
+  [VERSION_SPEC]  The version spec to find, e.g. 3|3.8|python3
 
-options:
-  -h, --help         show this help message and exit
-  -V, --version      show program's version number and exit
-  -a, --all          Show all matching python versions
-  --resolve-symlink  Resolve all symlinks
-  -v, --verbose      Verbose output
-  --no-same-file     Eliminate the duplicated results with the same file contents
-  --no-same-python   Eliminate the duplicated results with the same sys.executable
+Options:
+  -a, --all                    Return all matching Python versions
+      --resolve-symlinks       Resolve symlinks and remove duplicate results
+      --no-same-file           Remove duplicate results that are the same binary
+      --no-same-python         Remove duplicate results that wrap the same Python interpreter
+      --providers <PROVIDERS>  Select provider names(comma-separated) to use
+  -o, --output <OUTPUT>        The output format [default: default] [possible values: default, json, path]
+  -h, --help                   Print help
+  -V, --version                Print version
 ```
 
 ## Integration
 
 FindPython finds Python from the following places:
 
 -   `PATH` environment variable
 -   pyenv
 -   asdf
--   `/Library/Frameworks/Python.framework/Versions` (MacOS)
--   winreg (Windows)
+-   winreg (Windows) (🚧 WIP 🚧)
+-   [Rye] project manager backed by [python-build-standalone]
+
+[rye]: https://rye-up.com
+[python-build-standalone]: https://github.com/indygreg/python-build-standalone
 
 ## License
 
 FindPython is released under MIT License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,49 +1,56 @@
-Metadata-Version: 2.1 Name: findpython Version: 0.2.5 Summary: A utility to
-find python versions on your system License: MIT Author-email: Frost Ming
-gmail.com> Requires-Python: >=3.7 Classifier: Programming Language :: Python ::
-3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage, https:
-//github.com/frostming/findpython Description-Content-Type: text/markdown #
-FindPython _A utility to find python versions on your system._ [![Tests](https:
-//github.com/frostming/findpython/actions/workflows/ci.yml/badge.svg)](https://
-github.com/frostming/findpython/actions/workflows/ci.yml) [![PyPI](https://
-img.shields.io/pypi/v/findpython?logo=python&logoColor=%23cccccc&style=flat-
-square)](https://pypi.org/project/findpython) [![PyPI - Python Version](https:/
-/img.shields.io/pypi/pyversions/
+Metadata-Version: 2.1 Name: findpython Version: 1.0.0a0 Requires-Dist: pep440-
+rs >=0.3.11 ; extra == 'types' Provides-Extra: types License-File: LICENSE
+Summary: A utility to find python versions on your system Author: Frost Ming
+frostming.com> Author-email: Frost Ming
+gmail.com> License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
+markdown; charset=UTF-8; variant=GFM Project-URL: Source Code, https://
+github.com/frostming/findpython # FindPython _A utility to find python versions
+on your system._ [![Tests](https://github.com/frostming/findpython/actions/
+workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/
+workflows/ci.yml) [![PyPI](https://img.shields.io/pypi/v/
 findpython?logo=python&logoColor=%23cccccc&style=flat-square)](https://
-pypi.org/project/findpython) [![pdm-managed](https://img.shields.io/badge/pdm-
-managed-blueviolet?style=flat-square)](https://github.com/frostming/findpython)
-## Description This library is a rewrite of [pythonfinder] project by
-[@techalchemy][techalchemy]. It simplifies the whole code structure while
+pypi.org/project/findpython) [![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/findpython?logo=python&logoColor=%23cccccc&style=flat-square)]
+(https://pypi.org/project/findpython) [![pdm-managed](https://img.shields.io/
+badge/pdm-managed-blueviolet?style=flat-square)](https://github.com/frostming/
+findpython) ## Description This library is a rewrite of [pythonfinder] project
+by [@techalchemy][techalchemy]. It simplifies the whole code structure while
 preserving most of the original features. [pythonfinder]: https://github.com/
 sarugaku/pythonfinder [techalchemy]: https://github.com/techalchemy ##
-Installation FindPython is installable via any kind of package manager
-including `pip`: ```bash pip install findpython ```  Expand this section to see
-findpython's availability in the package ecosystem [Packaging_status]  ## Usage
-```python >>> import findpython >>> findpython.find(3, 9) # Find by major and
-minor version , architecture='64bit', major=3, minor=9, patch=10> >>>
-findpython.find("3.9") # Find by version string , architecture='64bit',
-major=3, minor=9, patch=10> >>> findpython.find("3.9-32") # Find by version
-string and architecture , architecture='32bit', major=3, minor=9, patch=10> >>>
-findpython.find(name="python3") # Find by executable name ,
-architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find
+Installation FindPython can be used in both Python and Rust projects. To
+install FindPython in Python: ```bash pip install findpython ``` To install
+FindPython in Rust: ```bash cargo install findpyhton ``` Or use FindPython
+library in a Rust project: ```bash cargo add findpython ```  Expand this
+section to see findpython's availability in the package ecosystem [Packaging
+status]  ## Python Usage ```python >>> import findpython >>> findpython.find(3,
+9) # Find by major and minor version , architecture='64bit', major=3, minor=9,
+patch=10> >>> findpython.find("3.9") # Find by version string ,
+architecture='64bit', major=3, minor=9, patch=10> >>> findpython.find("3.9-32")
+# Find by version string and architecture , architecture='32bit', major=3,
+minor=9, patch=10> >>> findpython.find(name="python3") # Find by executable
+name , architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find
 ("python3") # Find by executable name without keyword argument, same as above ,
 architecture='64bit', major=3, minor=10, patch=2> >>> findpython.find_all
 (major=3, minor=9) # Same arguments as `find()`, but return all matches [,
 architecture='64bit', major=3, minor=9, patch=10>, , architecture='64bit',
 major=3, minor=9, patch=10>, , architecture='64bit', major=3, minor=9,
 patch=9>, , architecture='64bit', major=3, minor=9, patch=5>, ,
-architecture='64bit', major=3, minor=9, patch=5>] ``` ## CLI Usage In addition,
-FindPython provides a CLI interface to find python versions: ``` usage:
-findpython [-h] [-V] [-a] [--resolve-symlink] [-v] [--no-same-file] [--no-same-
-python] [version_spec] Find python files in a directory positional arguments:
-version_spec Python version spec or name options: -h, --help show this help
-message and exit -V, --version show program's version number and exit -a, --all
-Show all matching python versions --resolve-symlink Resolve all symlinks -v, --
-verbose Verbose output --no-same-file Eliminate the duplicated results with the
-same file contents --no-same-python Eliminate the duplicated results with the
-same sys.executable ``` ## Integration FindPython finds Python from the
-following places: - `PATH` environment variable - pyenv - asdf - `/Library/
-Frameworks/Python.framework/Versions` (MacOS) - winreg (Windows) ## License
-FindPython is released under MIT License.
+architecture='64bit', major=3, minor=9, patch=5>] ``` ## Rust Usage ```rust use
+findpython::Finder; fn main() { let finder = Finder::default(); // Find by
+major and minor version let py = finder.find(3, 9).unwrap(); println!("{:?}",
+py); // Find all matches let all_pythons = finder.find_all(); println!("{:?}",
+all_pythons); } ``` ## CLI Usage In addition, FindPython provides a CLI
+interface to find python versions: ``` Find python executables on your system
+Usage: findpython [OPTIONS] [VERSION_SPEC] Arguments: [VERSION_SPEC] The
+version spec to find, e.g. 3|3.8|python3 Options: -a, --all Return all matching
+Python versions --resolve-symlinks Resolve symlinks and remove duplicate
+results --no-same-file Remove duplicate results that are the same binary --no-
+same-python Remove duplicate results that wrap the same Python interpreter --
+providers  Select provider names(comma-separated) to use -o, --output  The
+output format [default: default] [possible values: default, json, path] -h, --
+help Print help -V, --version Print version ``` ## Integration FindPython finds
+Python from the following places: - `PATH` environment variable - pyenv - asdf
+- winreg (Windows) (ð§ WIP ð§) - [Rye] project manager backed by [python-
+build-standalone] [rye]: https://rye-up.com [python-build-standalone]: https://
+github.com/indygreg/python-build-standalone ## License FindPython is released
+under MIT License.
```

