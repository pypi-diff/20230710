# Comparing `tmp/ansys_tools_path-0.2.6.tar.gz` & `tmp/ansys_tools_path-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_path-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_path-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_path-0.2.6.tar` & `ansys_tools_path-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1089 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/LICENSE
--rw-r--r--   0        0        0     4691 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/README.rst
--rw-r--r--   0        0        0     1843 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      919 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    26251 2023-06-21 15:10:34.732927 ansys_tools_path-0.2.6/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 ansys_tools_path-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4692 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/README.rst
+-rw-r--r--   0        0        0     1914 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      905 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      677 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    30449 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:42:41.894488 ansys_tools_path-0.3.0/src/ansys/tools/path/py.typed
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 ansys_tools_path-0.3.0/PKG-INFO
```

### Comparing `ansys_tools_path-0.2.6/LICENSE` & `ansys_tools_path-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_path-0.2.6/README.rst` & `ansys_tools_path-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
       # Activate it in Windows Powershell
       .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest required build system and doc, testing, and CI tools:
 
    .. code:: bash
 
-      python -m pip install .[test]
+      python -m pip install .[tests]
       python -m pip install .[doc]
       python -m pip install .[build]
 
 
 #. Install the project in editable mode:
 
    .. code:: bash
```

### Comparing `ansys_tools_path-0.2.6/pyproject.toml` & `ansys_tools_path-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.6"
+version = "0.3.0"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "importlib-metadata >=4.0",
-    "appdirs>=1.4.0",
+    "platformdirs>=3.6.0",
 ]
 
 
 [project.optional-dependencies]
-test = [
-    "pytest==7.3.1",
-    "pytest-cov==4.0.0",
+tests = [
+    "pytest==7.4.0",
+    "pytest-cov==4.1.0",
+    "pyfakefs==5.2.2",
 ]
 
 doc = [
-    "Sphinx==6.2.1",
+    "Sphinx==7.0.1",
     "numpydoc==1.5.0",
     "ansys-sphinx-theme==0.9.9",
     "sphinx-copybutton==0.5.2",
 ]
 
 build = [
     "build==0.10.0",
@@ -75,7 +74,13 @@
 max-line-length = 100
 
 [tool.coverage.run]
 source = ["ansys.tools"]
 
 [tool.coverage.report]
 show_missing = true
+
+[tool.pytest.ini_options]
+markers = [
+    "win32: Mark a test windows only",
+    "linux: Mark a test linux only"
+]
```

### Comparing `ansys_tools_path-0.2.6/src/ansys/tools/path/__init__.py` & `ansys_tools_path-0.3.0/src/ansys/tools/path/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 tools to find/cache installed Ansys products.
 
 WARNING: This is not concurrent-safe (multiple python processes might race on this data.)
 """
 
-try:
-    import importlib.metadata as importlib_metadata
-except ModuleNotFoundError:
-    import importlib_metadata
+import importlib.metadata as importlib_metadata
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 from ansys.tools.path.path import (
+    SETTINGS_DIR,
     SUPPORTED_ANSYS_VERSIONS,
     change_default_mapdl_path,
     change_default_mechanical_path,
     find_mapdl,
     find_mechanical,
     get_available_ansys_installations,
+    get_latest_ansys_installation,
     get_mapdl_path,
     get_mechanical_path,
     save_mapdl_path,
     save_mechanical_path,
     version_from_path,
 )
 from ansys.tools.path.path import change_default_ansys_path  # deprecated
```

### Comparing `ansys_tools_path-0.2.6/src/ansys/tools/path/path.py` & `ansys_tools_path-0.3.0/src/ansys/tools/path/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from dataclasses import dataclass
 from glob import glob
 import json
 import logging as LOG  # Temporal hack
 import os
 import re
-import typing
+from typing import Callable, Dict, Literal, Optional, Tuple, Union
 import warnings
 
-import appdirs
+import platformdirs
 
 from ansys.tools.path.misc import is_float, is_linux, is_windows
 
+PRODUCT_TYPE = Literal["mapdl", "mechanical"]
+SUPPORTED_VERSIONS_TYPE = Dict[int, str]
+
 LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"], ["/", "install", "ansys_inc"]]
 LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 CONFIG_FILE_NAME = "config.txt"
 
-SUPPORTED_ANSYS_VERSIONS = {
+SUPPORTED_ANSYS_VERSIONS: SUPPORTED_VERSIONS_TYPE = {
     241: "2024R1",
     232: "2023R2",
     231: "2023R1",
     222: "2022R2",
     221: "2022R1",
     212: "2021R2",
     211: "2021R1",
@@ -47,103 +51,111 @@
     PRODUCT_EXE_INFO["mechanical"]["patternpath"] = "vXXX/aisol/bin/winx64/AnsysWBU.exe"
     PRODUCT_EXE_INFO["mechanical"]["pattern"] = "AnsysWBU.exe"
 else:
     PRODUCT_EXE_INFO["mechanical"]["patternpath"] = "vXXX/aisol/.workbench"
     PRODUCT_EXE_INFO["mechanical"]["pattern"] = ".workbench"
 
 # settings directory
-SETTINGS_DIR = appdirs.user_data_dir("ansys_tools_path")
+SETTINGS_DIR = platformdirs.user_data_dir(appname="ansys_tools_path", appauthor="Ansys")
 if not os.path.isdir(SETTINGS_DIR):  # pragma: no cover
     try:
         LOG.debug(f"Created settings directory: {SETTINGS_DIR}")
         os.makedirs(SETTINGS_DIR)
     except:
         warnings.warn(
             "Unable to create settings directory.\n"
             "Will be unable to cache product executable locations"
         )
 
 CONFIG_FILE = os.path.join(SETTINGS_DIR, CONFIG_FILE_NAME)
 
 
 def _get_installed_windows_versions(
-    supported_versions=SUPPORTED_ANSYS_VERSIONS,
-):  # pragma: no cover
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Dict[int, str]:  # pragma: no cover
     """Get the AWP_ROOT environment variable values for supported versions."""
 
     # The student version overwrites the AWP_ROOT env var
     # (if it is installed later)
     # However the priority should be given to the non-student version.
-    awp_roots = []
-    awp_roots_student = []
-
+    awp_roots: list[Tuple[int, str]] = []
+    awp_roots_student: list[Tuple[int, str]] = []
     for ver in supported_versions:
         path_ = os.environ.get(f"AWP_ROOT{ver}", "")
-        path_non_student = path_.replace("\\ANSYS Student", "")
+        if path_ == "":
+            continue
 
-        if "student" in path_.lower() and os.path.exists(path_non_student):
+        if "student" in path_.lower():
+            awp_roots_student.insert(0, (-1 * ver, path_))
             # Check if also exist a non-student version
-            awp_roots.append([ver, path_non_student])
-            awp_roots_student.insert(0, [-1 * ver, path_])
+            path_non_student = path_.replace("\\ANSYS Student", "")
+            if os.path.exists(path_non_student):
+                awp_roots.append((ver, path_non_student))
 
         else:
-            awp_roots.append([ver, path_])
+            awp_roots.append((ver, path_))
 
     awp_roots.extend(awp_roots_student)
     installed_versions = {ver: path for ver, path in awp_roots if path and os.path.isdir(path)}
     if installed_versions:
         LOG.debug(f"Found the following unified Ansys installation versions: {installed_versions}")
     else:
         LOG.debug("No unified Ansys installations found using 'AWP_ROOT' environments.")
     return installed_versions
 
 
-def _get_default_linux_base_path():
+def _get_default_linux_base_path() -> Optional[str]:
     """Get the default base path of the Ansys unified install on linux."""
 
     for path in LINUX_DEFAULT_DIRS:
         if os.path.isdir(path):
             return path
-    return None  # pragma: no cover
+    return None
 
 
-def _get_default_windows_base_path():  # pragma: no cover
+def _get_default_windows_base_path() -> Optional[str]:  # pragma: no cover
     """Get the default base path of the Ansys unified install on windows."""
 
-    base_path = os.path.join(os.environ["PROGRAMFILES"], "ANSYS INC")
+    base_path = os.path.join(os.environ["PROGRAMFILES"], "ANSYS Inc")
     if not os.path.exists(base_path):
         LOG.debug(f"The supposed 'base_path'{base_path} does not exist. No available ansys found.")
         return None
     return base_path
 
 
-def _expand_base_path(base_path: str) -> dict:
+def _expand_base_path(base_path: Optional[str]) -> Dict[int, str]:
     """Expand the base path to all possible ansys Unified installations contained within."""
     if base_path is None:
         return {}
 
     paths = glob(os.path.join(base_path, "v*"))
 
-    # Testing for ANSYS STUDENT version
-    if not paths:  # pragma: no cover
-        paths = glob(os.path.join(base_path, "ANSYS*"))
+    ansys_paths: Dict[int, str] = {}
 
+    for path in paths:
+        ver_str = path[-3:]
+        if is_float(ver_str):
+            ansys_paths[int(ver_str)] = path
+
+    # Testing for ANSYS STUDENT version
+    paths = glob(os.path.join(base_path, "ANSYS*", "v*"))
     if not paths:
         return {}
 
-    ansys_paths = {}
     for path in paths:
         ver_str = path[-3:]
         if is_float(ver_str):
-            ansys_paths[int(ver_str)] = path
+            ansys_paths[-int(ver_str)] = path
 
     return ansys_paths
 
 
-def _get_available_base_unified(supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def _get_available_base_unified(
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Dict[int, str]:
     r"""Get a dictionary of available Ansys Unified Installation versions with
     their base paths.
 
     Returns
     -------
         Paths for Unified Installation versions installed.
 
@@ -166,19 +178,20 @@
             return installed_versions
         else:  # pragma: no cover
             base_path = _get_default_windows_base_path()
     elif is_linux():
         base_path = _get_default_linux_base_path()
     else:  # pragma: no cover
         raise OSError(f"Unsupported OS {os.name}")
-
     return _expand_base_path(base_path)
 
 
-def get_available_ansys_installations(supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def get_available_ansys_installations(
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Dict[int, str]:
     """Return a dictionary of available Ansys unified installation versions with their base paths.
 
     Returns
     -------
     dict[int: str]
         Return all Ansys unified installations paths in Windows.
 
@@ -206,25 +219,26 @@
      202: '/usr/ansys_inc/v202',
      211: '/usr/ansys_inc/v211'}
     """
     return _get_available_base_unified(supported_versions)
 
 
 def _get_unified_install_base_for_version(
-    version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS
-) -> typing.Tuple[str, str]:
+    version: Optional[Union[int, float]] = None,
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Tuple[str, str]:
     """Search for the unified install of a given version from the supported versions.
 
     Returns
     -------
     Tuple[str, str]
         The base unified install path and version
     """
     versions = _get_available_base_unified(supported_versions)
-    if not versions:  # pragma: no cover
+    if not versions:
         return "", ""
 
     if not version:
         version = max(versions.keys())
 
     elif isinstance(version, float):
         # Using floats, converting to int.
@@ -234,27 +248,31 @@
         ans_path = versions[version]
     except KeyError as e:
         raise ValueError(
             f"Version {version} not found. Available versions are {list(versions.keys())}"
         ) from e
 
     version = abs(version)
-    return ans_path, version
+    return ans_path, str(version)
 
 
-def find_mechanical(version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def find_mechanical(
+    version: Optional[float] = None,
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Union[Tuple[str, float], Tuple[Literal[""], Literal[""]]]:
     """
     Search for the Mechanical path in the standard installation location.
 
     Returns
     -------
     mechanical_path : str
         Full path to the executable file for the latest Mechanical version.
-    version : float
+    version : float | str
         Version in the float format. For example, ``23.1`` for 2023 R1.
+        If no version has be found, version is set to ""
 
     Examples
     --------
     On Windows:
 
     >>> from ansys.mechanical.core.mechanical import find_mechanical
     >>> find_mechanical()
@@ -271,15 +289,18 @@
     if is_windows():  # pragma: no cover
         mechanical_bin = os.path.join(ans_path, "aisol", "bin", "winx64", f"AnsysWBU.exe")
     else:
         mechanical_bin = os.path.join(ans_path, "aisol", ".workbench")
     return mechanical_bin, int(version) / 10
 
 
-def find_mapdl(version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def find_mapdl(
+    version: Optional[Union[int, float]] = None,
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Union[Tuple[str, float], Tuple[Literal[""], Literal[""]]]:
     """Searches for Ansys MAPDL path within the standard install location
     and returns the path of the latest version.
 
     Parameters
     ----------
     version : int, float, optional
         Version of Ansys MAPDL to search for.
@@ -319,53 +340,62 @@
     if is_windows():
         ansys_bin = os.path.join(ans_path, "ansys", "bin", "winx64", f"ansys{version}.exe")
     else:
         ansys_bin = os.path.join(ans_path, "ansys", "bin", f"ansys{version}")
     return ansys_bin, int(version) / 10
 
 
-def _find_installation(product: str, version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def _find_installation(
+    product: PRODUCT_TYPE,
+    version: Optional[float] = None,
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Union[Tuple[str, float], Tuple[Literal[""], Literal[""]]]:
     if product == "mapdl":
         return find_mapdl(version, supported_versions)
     elif product == "mechanical":
         return find_mechanical(version, supported_versions)
     raise Exception("unexpected product")
 
 
-def find_ansys(version=None, supported_versions=SUPPORTED_ANSYS_VERSIONS):
+def find_ansys(
+    version: Optional[float] = None,
+    supported_versions: SUPPORTED_VERSIONS_TYPE = SUPPORTED_ANSYS_VERSIONS,
+) -> Union[Tuple[str, float], Tuple[Literal[""], Literal[""]]]:
     """Obsolete method, use find_mapdl."""
     warnings.warn(
         "This method is going to be deprecated in future versions. Please use 'find_mapdl'.",
         category=DeprecationWarning,
     )
 
     return _find_installation("mapdl", version, supported_versions)
 
 
-def is_valid_executable_path(product: str, exe_loc: str):
+def is_valid_executable_path(product: PRODUCT_TYPE, exe_loc: str) -> bool:
     if product == "mapdl":
         return (
             os.path.isfile(exe_loc)
             and re.search(r"ansys\d\d\d", os.path.basename(os.path.normpath(exe_loc))) is not None
         )
     elif product == "mechanical":
         if is_windows():  # pragma: no cover
             return (
                 os.path.isfile(exe_loc)
-                and re.search("AnsysWBU.exe", os.path.basename(os.path.normpath(exe_loc)))
+                and re.search(
+                    "AnsysWBU.exe", os.path.basename(os.path.normpath(exe_loc)), re.IGNORECASE
+                )
                 is not None
             )
         return (
             os.path.isfile(exe_loc)
             and re.search(".workbench", os.path.basename(os.path.normpath(exe_loc))) is not None
         )
     raise Exception("unexpected application")
 
 
-def _is_common_executable_path(product: str, exe_loc: str) -> bool:
+def _is_common_executable_path(product: PRODUCT_TYPE, exe_loc: str) -> bool:
     if product == "mapdl":
         path = os.path.normpath(exe_loc)
         path = path.split(os.sep)
         # Look for all v(\d\d\d) to catch the last one
         # in case the user has placed the installation folder inside a folder called for example (/ansys/v211)
         v_version = re.findall(r"v(\d\d\d)", exe_loc)
         ansys_version = re.findall(r"ansys(\d\d\d)", exe_loc, re.IGNORECASE)
@@ -381,43 +411,44 @@
     elif product == "mechanical":
         path = os.path.normpath(exe_loc)
         path = path.split(os.sep)
 
         is_valid_path = is_valid_executable_path("mechanical", exe_loc)
 
         if is_windows():  # pragma: no cover
+            lower_case_path = map(str.lower, path)
             return (
                 is_valid_path
                 and re.search(r"v\d\d\d", exe_loc) is not None
-                and "aisol" in path
-                and ("bin" in path or "Bin" in path)
-                and "winx64" in path
-                and ("AnsysWBU.exe" in path or "ANSYSWBU.exe" in path)
+                and "aisol" in lower_case_path
+                and "bin" in lower_case_path
+                and "winx64" in lower_case_path
+                and "ansyswbu.exe" in lower_case_path
             )
 
         return (
             is_valid_path
             and re.search(r"v\d\d\d", exe_loc) is not None
             and "aisol" in path
             and ".workbench" in path
         )
     else:
         raise Exception("unexpected application")
 
 
-def _change_default_path(product: str, exe_loc: str):
+def _change_default_path(product: PRODUCT_TYPE, exe_loc: str) -> None:
     if os.path.isfile(exe_loc):
         config_data = _read_config_file(product)
         config_data[product] = exe_loc
         _write_config_file(config_data)
     else:
         raise FileNotFoundError("File %s is invalid or does not exist" % exe_loc)
 
 
-def change_default_mapdl_path(exe_loc) -> None:
+def change_default_mapdl_path(exe_loc: str) -> None:
     """Change your default Ansys MAPDL path.
 
     Parameters
     ----------
     exe_loc : str
         Ansys MAPDL executable path.  Must be a full path.
 
@@ -435,15 +466,15 @@
     >>> mapdl_path = 'C:/Program Files/ANSYS Inc/v193/ansys/bin/winx64/ANSYS193.exe'
     >>> change_default_mapdl_path(mapdl_path)
 
     """
     _change_default_path("mapdl", exe_loc)
 
 
-def change_default_mechanical_path(exe_loc) -> None:
+def change_default_mechanical_path(exe_loc: str) -> None:
     """Change your default Mechanical path.
 
     Parameters
     ----------
     exe_loc : str
         Full path for the Mechanical executable file to use.
 
@@ -463,43 +494,45 @@
     >>> get_mechanical_path()
     '/ansys_inc/v231/aisol/.workbench'
 
     """
     _change_default_path("mechanical", exe_loc)
 
 
-def change_default_ansys_path(exe_loc) -> None:
+def change_default_ansys_path(exe_loc: str) -> None:
     """Deprecated, use `change_default_mapdl_path` instead"""
 
     warnings.warn(
         "This method is going to be deprecated in future versions. Please use 'change_default_mapdl_path'.",
         category=DeprecationWarning,
     )
 
     _change_default_path("mapdl", exe_loc)
 
 
-def _save_path(product: str, exe_loc: str = None, allow_prompt=True) -> str:
+def _save_path(
+    product: PRODUCT_TYPE, exe_loc: Optional[str] = None, allow_prompt: bool = True
+) -> str:
     if exe_loc is None:
         exe_loc, _ = _find_installation(product)
 
     if is_valid_executable_path(product, exe_loc):
         _check_uncommon_executable_path(product, exe_loc)
 
         _change_default_path(product, exe_loc)
         return exe_loc
 
-    if is_valid_executable_path(product, exe_loc):
-        return exe_loc
     if allow_prompt:
-        exe_loc = _prompt_path(product)
+        exe_loc = _prompt_path(product)  # pragma: no cover
     return exe_loc
 
 
-def save_mechanical_path(exe_loc=None, allow_prompt=True):  # pragma: no cover
+def save_mechanical_path(
+    exe_loc: Optional[str] = None, allow_prompt: bool = True
+) -> str:  # pragma: no cover
     """Find the Mechanical path or query user.
 
     Parameters
     ----------
     exe_loc : string, optional
         Path for the Mechanical executable file (``AnsysWBU.exe``).
         The default is ``None``, in which case an attempt is made to
@@ -507,47 +540,47 @@
 
         - The default Mechanical paths (for example,
           ``C:/Program Files/Ansys Inc/vXXX/aiso/bin/AnsysWBU.exe``)
         - The configuration file
         - User input
 
         If a path is supplied, this method performs some checks. If the
-        checks are aresuccessful, it writes this path to the configuration
+        checks are successful, it writes this path to the configuration
         file.
 
     Returns
     -------
     str
         Path for the Mechanical executable file.
 
     Notes
     -----
-    The location of the configuration file (``config.txt``) can be found in
-    ``appdirs.user_data_dir("ansys_tools_path")``. For example:
+    The location of the configuration file ``config.txt`` can be found in
+    ``ansys.tools.path.SETTINGS_DIR``. For example:
 
     .. code:: pycon
 
-        >>> import appdirs
+        >>> from ansys.tools.path import SETTINGS_DIR
         >>> import os
-        >>> print(os.path.join(appdirs.user_data_dir("ansys_tools_path"), "config.txt"))
-        C:/Users/[username]]/AppData/Local/ansys_tools_path/ansys_tools_path/config.txt
+        >>> print(os.path.join(SETTINGS_DIR, "config.txt"))
+        C:/Users/[username]]/AppData/Local/Ansys/ansys_tools_path/config.txt
 
     You can change the default for the ``exe_loc`` parameter either by modifying the
     ``config.txt`` file or by running this code:
 
     .. code:: pycon
 
        >>> from ansys.tools.path import save_mechanical_path
        >>> save_mechanical_path("/new/path/to/executable")
 
     """
     return _save_path("mechanical", exe_loc, allow_prompt)
 
 
-def save_mapdl_path(exe_loc=None, allow_prompt=True) -> str:
+def save_mapdl_path(exe_loc: Optional[str] = None, allow_prompt: bool = True) -> str:
     """Find Ansys MAPDL's path or query user.
 
     If no ``exe_loc`` argument is supplied, this function attempt
     to obtain the Ansys MAPDL executable from (and in order):
 
     - The default ansys paths (i.e. ``'C:/Program Files/Ansys Inc/vXXX/ansys/bin/ansysXXX'``)
     - The configuration file
@@ -564,157 +597,210 @@
     Returns
     -------
     str
         Path of the MAPDL executable.
 
     Notes
     -----
-    The configuration file location (``config.txt``) can be found in
-    ``appdirs.user_data_dir("ansys_tools_path")``. For example:
+    The location of the configuration file ``config.txt`` can be found in
+    ``ansys.tools.path.SETTINGS_DIR``. For example:
 
     .. code:: pycon
 
-        >>> import appdirs
+        >>> from ansys.tools.path import SETTINGS_DIR
         >>> import os
-        >>> print(os.path.join(appdirs.user_data_dir("ansys_tools_path"), "config.txt"))
-        C:/Users/user/AppData/Local/ansys_tools_path/ansys_tools_path/config.txt
+        >>> print(os.path.join(SETTINGS_DIR, "config.txt"))
+        C:/Users/[username]/AppData/Local/Ansys/ansys_tools_path/config.txt
 
     Examples
     --------
     You can change the default ``exe_loc`` either by modifying the mentioned
     ``config.txt`` file or by executing:
 
     >>> from ansys.tools.path import save_mapdl_path
     >>> save_mapdl_path('/new/path/to/executable')
 
     """
     return _save_path("mapdl", exe_loc, allow_prompt)
 
 
-def save_ansys_path(exe_loc=None, allow_prompt=True) -> str:
+def save_ansys_path(exe_loc: Optional[str] = None, allow_prompt: bool = True) -> str:
     """Deprecated, use `save_mapdl_path` instead"""
 
     warnings.warn(
         "This method is going to be deprecated in future versions. Please use 'save_ansys_path'.",
         category=DeprecationWarning,
     )
     return _save_path("mapdl", exe_loc, allow_prompt)
 
 
-def _check_uncommon_executable_path(product: str, exe_loc: str):
+def _check_uncommon_executable_path(product: PRODUCT_TYPE, exe_loc: str):
     product_pattern_path = PRODUCT_EXE_INFO[product]["patternpath"]
     product_name = PRODUCT_EXE_INFO[product]["name"]
     if not _is_common_executable_path(product, exe_loc):
         warnings.warn(
             f"The supplied path ('{exe_loc}') does not match the usual {product_name} executable path style"
             f"('directory/{product_pattern_path}'). "
             "You might have problems at later use."
         )
 
 
-def _prompt_path(product: str) -> str:  # pragma: no cover
+def _prompt_path(product: PRODUCT_TYPE) -> str:  # pragma: no cover
     product_name = PRODUCT_EXE_INFO[product]["name"]
     product_pattern = PRODUCT_EXE_INFO[product]["pattern"]
     product_pattern_path = PRODUCT_EXE_INFO[product]["patternpath"]
     print(f"Cached {product} executable not found")
     print(
         f"You are about to enter manually the path of the {product_name} executable\n"
         f"({product_pattern}, where XXX is the version\n"
         f"This file is very likely to contained in path ending in '{product_pattern_path}'.\n"
         "\nIf you experience problems with the input path you can overwrite the configuration\n"
         "file by typing:\n"
         f">>> from ansys.tools.path import save_{product}_path\n"
         f">>> save_{product}_path('/new/path/to/executable/')\n"
     )
-    while True:  # pragma: no cover
+    while True:
         exe_loc = input(f"Enter the location of an {product_name} ({product_pattern}):")
 
         if is_valid_executable_path(product, exe_loc):
             _check_uncommon_executable_path(product, exe_loc)
             config_data = _read_config_file(product)
             config_data[product] = exe_loc
             _write_config_file(config_data)
             break
         else:
             print(
-                "The supplied path is either: not a valid file path, or does not match '{product_pattern}' name."
+                f"The supplied path is either: not a valid file path, or does not match '{product_pattern}' name."
             )
     return exe_loc
 
 
 def _clear_config_file() -> None:
     """Used by tests. We can consider supporting it on the library"""
     if os.path.isfile(CONFIG_FILE):
         os.remove(CONFIG_FILE)
 
 
-def _read_config_file(product_name: str) -> dict:
+def _read_config_file(product_name: str) -> Dict[str, str]:
     """Read config file for a given product, migrating if needed"""
 
     if not os.path.isfile(CONFIG_FILE):
         _migrate_config_file(product_name)
     if os.path.isfile(CONFIG_FILE):
         with open(CONFIG_FILE, "r") as f:
-            return json.load(f)
-    else:
-        return {}
+            content = f.read()
+
+        if content:
+            return json.loads(content)
+
+    return {}
 
 
-def _write_config_file(config_data: dict):
+def _write_config_file(config_data: Dict[str, str]):
     """Warning - this isn't threadsafe"""
     with open(CONFIG_FILE, "w") as f:
         json.dump(config_data, f)
 
 
 def _migrate_config_file(product_name: str) -> None:
     """Migrate configuration if needed"""
-    if product_name not in ["mechanical", "mapdl"]:
-        return
-
-    old_config_file_name = "config.txt"
-    old_settings_dir = appdirs.user_data_dir(f"ansys_{product_name}_core")
-    old_config_file = os.path.join(old_settings_dir, old_config_file_name)
-    if os.path.isfile(old_config_file):
-        with open(old_config_file) as f:
-            exe_loc = f.read()
 
+    def _migrate_txt_config_file(old_config_file_path: str) -> None:
+        with open(old_config_file_path) as old_config_file:
+            mapdl_exe_localisation: str = old_config_file.read()
         if os.path.isfile(CONFIG_FILE):
             new_config_data = _read_config_file(product_name)
         else:
-            new_config_data = {}
-        new_config_data[product_name] = exe_loc
+            new_config_data: Dict[str, str] = {}
+        new_config_data[product_name] = mapdl_exe_localisation
         _write_config_file(new_config_data)
-        os.remove(old_config_file)
+
+    def _migrate_json_config_file(old_config_file_path: str) -> None:  # pragma: no cover
+        with open(old_config_file_path) as old_config_file:
+            old_config_data = old_config_file.read()
+        try:
+            old_config_data_json = json.loads(old_config_data)
+            _write_config_file(old_config_data_json)
+        except ValueError:
+            # if the config file cannot be parsed we simply throw it away
+            pass
+
+    @dataclass
+    class FileMigrationStrategy:
+        path: str
+        migration_function: Callable[[str], None]
+
+        def __call__(self):
+            self.migration_function(self.path)
+
+    if product_name not in ["mechanical", "mapdl"]:
+        return
+
+    file_migration_strategy_list: list[FileMigrationStrategy] = [
+        FileMigrationStrategy(
+            os.path.join(platformdirs.user_data_dir(f"ansys_{product_name}_core"), "config.txt"),
+            _migrate_txt_config_file,
+        ),
+        FileMigrationStrategy(
+            os.path.join(platformdirs.user_data_dir("ansys_tools_path"), "config.txt"),
+            _migrate_json_config_file,
+        ),
+    ]
+
+    # Filter to only keep config files that exists
+    file_migration_strategy_list = [
+        file_migration_strategy
+        for file_migration_strategy in file_migration_strategy_list
+        if os.path.exists(file_migration_strategy.path)
+    ]
+
+    if len(file_migration_strategy_list) == 0:
+        return
+
+    # we use the migration strategy of the last file
+    latest_file_migration_strategy = file_migration_strategy_list[-1]
+    latest_file_migration_strategy()
+
+    # remove all old config files
+    for file_migration_strategy in file_migration_strategy_list:
+        os.remove(file_migration_strategy.path)
 
 
-def _read_executable_path_from_config_file(product_name: str):
+def _read_executable_path_from_config_file(product_name: str) -> Optional[str]:
     """Read the executable path for the product given by `product_name` from config file"""
     config_data = _read_config_file(product_name)
     return config_data.get(product_name, None)
 
 
-def _get_application_path(product: str, allow_input=True, version=None):
-    exe_loc = None
-    if not version:
+def _get_application_path(
+    product: PRODUCT_TYPE, allow_input: bool = True, version: Optional[float] = None
+) -> Optional[str]:
+    if version is None:
         exe_loc = _read_executable_path_from_config_file(product)
-        if exe_loc != None:  # verify
-            if not os.path.isfile(exe_loc) and allow_input:
-                exe_loc = _save_path(product)
-        elif allow_input:  # create configuration file
-            exe_loc = _save_path(product)
+        if exe_loc is not None:
+            return exe_loc
 
-    if exe_loc is None:
-        exe_loc = _find_installation(product, version=version)[0]
-        if not exe_loc:
-            exe_loc = None
+    try:
+        exe_loc, exe_version = _find_installation(product, version)
+        if (exe_loc, exe_version) != ("", ""):  # executable not found
+            if os.path.isfile(exe_loc):
+                return exe_loc
+    except ValueError:
+        # Skip to go out of the if statement
+        pass
 
-    return exe_loc
+    if allow_input:
+        exe_loc = _prompt_path(product)
+        _change_default_path(product, exe_loc)
+        return exe_loc
+
+    return None
 
 
-def get_mapdl_path(allow_input=True, version=None) -> str:
+def get_mapdl_path(allow_input: bool = True, version: Optional[float] = None) -> Optional[str]:
     """Acquires Ansys MAPDL Path from a cached file or user input
 
     Parameters
     ----------
     allow_input : bool, optional
         Allow user input to find Ansys MAPDL path.  The default is ``True``.
 
@@ -722,25 +808,25 @@
         Version of Ansys MAPDL to search for. For example ``version=22.2``.
         If ``None``, use latest.
 
     """
     return _get_application_path("mapdl", allow_input, version)
 
 
-def get_ansys_path(allow_input: bool = True, version=None) -> str:
+def get_ansys_path(allow_input: bool = True, version: Optional[float] = None) -> Optional[str]:
     """Deprecated, use `get_mapdl_path` instead"""
 
     warnings.warn(
-        "This method is going to be deprecated in future versions. Please use 'get_ansys_path'.",
+        "This method is going to be deprecated in future versions. Please use 'get_mapdl_path'.",
         category=DeprecationWarning,
     )
     return _get_application_path("mapdl", allow_input, version)
 
 
-def get_mechanical_path(allow_input=True, version=None) -> str:
+def get_mechanical_path(allow_input: bool = True, version: Optional[float] = None) -> Optional[str]:
     """Acquires Ansys Mechanical Path from a cached file or user input
 
     Parameters
     ----------
     allow_input : bool, optional
         Allow user input to find Ansys Mechanical path.  The default is ``True``.
 
@@ -748,15 +834,15 @@
         Version of Ansys Mechanical to search for. For example ``version=22.2``.
         If ``None``, use latest.
 
     """
     return _get_application_path("mechanical", allow_input, version)
 
 
-def _mechanical_version_from_path(path):
+def _mechanical_version_from_path(path: str) -> int:
     """Extract the Ansys Mechanical version from a path.
 
     Generally, the version of Mechanical is contained in the path:
 
     - On Windows, for example: ``C:/Program Files/ANSYS Inc/v231/aisol/bin/winx64/AnsysWBU.exe``
     - On Linux, for example: ``/usr/ansys_inc/v231/aisol/.workbench``
 
@@ -775,15 +861,15 @@
     # replace \\ with / to account for possible windows path
     matches = re.findall(r"v(\d\d\d)", path.replace("\\", "/"), re.IGNORECASE)
     if not matches:
         raise RuntimeError(f"Unable to extract Mechanical version from {path}.")
     return int(matches[-1])
 
 
-def _mapdl_version_from_path(path):
+def _mapdl_version_from_path(path: str) -> int:
     """Extract ansys version from a path.  Generally, the version of
     Ansys MAPDL is contained in the path:
     C:/Program Files/ANSYS Inc/v202/ansys/bin/winx64/ANSYS202.exe
     /usr/ansys_inc/v211/ansys/bin/mapdl
     Note that if the Ansys MAPDL executable, you have to rely on the version
     in the path.
     Parameters
@@ -801,15 +887,15 @@
     # replace \\ with / to account for possible windows path
     matches = re.findall(r"v(\d\d\d).ansys", path.replace("\\", "/"), re.IGNORECASE)
     if not matches:
         raise RuntimeError(f"Unable to extract Ansys version from {path}")
     return int(matches[-1])
 
 
-def version_from_path(product, path):
+def version_from_path(product: PRODUCT_TYPE, path: str) -> int:
     """Extract the product version from a path.
 
     Parameters
     ----------
     path : str
         Path to the executable file.
 
@@ -820,7 +906,35 @@
 
     """
     if product == "mechanical":
         return _mechanical_version_from_path(path)
     elif product == "mapdl":
         return _mapdl_version_from_path(path)
     raise Exception("Unexpected product")
+
+
+def get_latest_ansys_installation() -> Tuple[int, str]:
+    """Return a tuple with the latest ansys installation version and its path
+
+    If there is a student version and a regular installation for the latest release, the regular one is returned
+
+    Returns
+    -------
+    Tuple[int, str]
+        Tuple with the latest version and path of the installation
+
+    Raise
+    -----
+    ValueError
+        No Ansys installation found
+    """
+    installations = get_available_ansys_installations()
+    if not installations:
+        raise ValueError("No Ansys installation found")
+
+    def sort_key(version: int) -> float:
+        if version < 0:
+            return abs(version) - 0.5
+        return float(version)
+
+    max_version = max(installations, key=sort_key)
+    return (max_version, installations[max_version])
```

### Comparing `ansys_tools_path-0.2.6/PKG-INFO` & `ansys_tools_path-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.6
+Version: 0.3.0
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: importlib-metadata >=4.0
-Requires-Dist: appdirs>=1.4.0
+Requires-Dist: platformdirs>=3.6.0
 Requires-Dist: build==0.10.0 ; extra == "build"
 Requires-Dist: twine==4.0.2 ; extra == "build"
-Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: pytest==7.3.1 ; extra == "test"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: pyfakefs==5.2.2 ; extra == "tests"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/ansys-tools-path
 Project-URL: Source, https://github.com/ansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/ansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
-Provides-Extra: test
+Provides-Extra: tests
 
 ansys-tools-path
 ================
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
@@ -126,15 +125,15 @@
       # Activate it in Windows Powershell
       .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest required build system and doc, testing, and CI tools:
 
    .. code:: bash
 
-      python -m pip install .[test]
+      python -m pip install .[tests]
       python -m pip install .[doc]
       python -m pip install .[build]
 
 
 #. Install the project in editable mode:
 
    .. code:: bash
```

