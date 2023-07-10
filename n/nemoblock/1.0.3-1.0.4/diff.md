# Comparing `tmp/nemoblock-1.0.3.tar.gz` & `tmp/nemoblock-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemoblock-1.0.3.tar", last modified: Wed Jan  4 14:55:12 2023, max compression
+gzip compressed data, was "nemoblock-1.0.4.tar", last modified: Mon Jul 10 09:51:30 2023, max compression
```

## Comparing `nemoblock-1.0.3.tar` & `nemoblock-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 14:55:12.095881 nemoblock-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-04 14:54:58.000000 nemoblock-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-01-04 14:55:12.095881 nemoblock-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-01-04 14:54:58.000000 nemoblock-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 14:55:12.099881 nemoblock-1.0.3/nemoblock/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-04 14:54:58.000000 nemoblock-1.0.3/nemoblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-01-04 14:55:12.099881 nemoblock-1.0.3/nemoblock/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-01-04 14:54:58.000000 nemoblock-1.0.3/nemoblock/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-01-04 14:54:58.000000 nemoblock-1.0.3/nemoblock/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-01-04 14:54:58.000000 nemoblock-1.0.3/nemoblock/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 14:55:12.095881 nemoblock-1.0.3/nemoblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-01-04 14:55:12.000000 nemoblock-1.0.3/nemoblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-01-04 14:55:12.000000 nemoblock-1.0.3/nemoblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 14:55:12.000000 nemoblock-1.0.3/nemoblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 14:55:12.000000 nemoblock-1.0.3/nemoblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-04 14:55:12.000000 nemoblock-1.0.3/nemoblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-04 14:55:12.099881 nemoblock-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-04 14:54:58.000000 nemoblock-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:51:30.438514 nemoblock-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 09:51:19.000000 nemoblock-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-10 09:51:30.438514 nemoblock-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-10 09:51:19.000000 nemoblock-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:51:30.438514 nemoblock-1.0.4/nemoblock/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-10 09:51:19.000000 nemoblock-1.0.4/nemoblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 09:51:30.438514 nemoblock-1.0.4/nemoblock/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25494 2023-07-10 09:51:19.000000 nemoblock-1.0.4/nemoblock/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-07-10 09:51:19.000000 nemoblock-1.0.4/nemoblock/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-10 09:51:19.000000 nemoblock-1.0.4/nemoblock/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:51:30.438514 nemoblock-1.0.4/nemoblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-10 09:51:30.000000 nemoblock-1.0.4/nemoblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-10 09:51:30.000000 nemoblock-1.0.4/nemoblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:51:30.000000 nemoblock-1.0.4/nemoblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 09:51:30.000000 nemoblock-1.0.4/nemoblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:51:30.000000 nemoblock-1.0.4/nemoblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-10 09:51:30.438514 nemoblock-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-10 09:51:19.000000 nemoblock-1.0.4/setup.py
```

### Comparing `nemoblock-1.0.3/LICENSE` & `nemoblock-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nemoblock-1.0.3/PKG-INFO` & `nemoblock-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nemoblock
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities to generate blockMeshDicts for OpenFOAM.
 Home-page: https://github.com/nemocrys/nemoblock
 Author: Arved Enders-Seidlitz
 Author-email: arved.enders-seidlitz@ikz-berlin.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nemoblock
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7503822.svg)](https://doi.org/10.5281/zenodo.7503822)
 
 ## Project description
 
 nemoblock provides utilities to generate blockMeshDicts for structured mesh generation in OpenFOAM. It manages the numbering of the points, the orientation of the surfaces and the connections between the blocks. In this way it helps the user to focus on the most important point: generating high quality meshes.
 
 The project is developed and maintained by the [**Model experiments group**](https://www.ikz-berlin.de/en/research/materials-science/section-fundamental-description#c486) at the Leibniz Institute for Crystal Growth (IKZ).
 
@@ -147,14 +148,14 @@
 
 ## License
 
 nemoblock is published under the [GPLv3 license](https://www.gnu.org/licenses/gpl-3.0.html).
 
 ## Acknowledgements
 
-[This project](https://www.researchgate.net/project/NEMOCRYS-Next-Generation-Multiphysical-Models-for-Crystal-Growth-Processes) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
+[This project](https://nemocrys.github.io/) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
 
 <img src="https://raw.githubusercontent.com/nemocrys/nemoblock/master/EU-ERC.png">
 
 ## Contribution
 
 Any help to improve this package is very welcome!
```

### Comparing `nemoblock-1.0.3/README.md` & `nemoblock-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # nemoblock
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7503822.svg)](https://doi.org/10.5281/zenodo.7503822)
 
 ## Project description
 
 nemoblock provides utilities to generate blockMeshDicts for structured mesh generation in OpenFOAM. It manages the numbering of the points, the orientation of the surfaces and the connections between the blocks. In this way it helps the user to focus on the most important point: generating high quality meshes.
 
 The project is developed and maintained by the [**Model experiments group**](https://www.ikz-berlin.de/en/research/materials-science/section-fundamental-description#c486) at the Leibniz Institute for Crystal Growth (IKZ).
 
@@ -133,14 +134,14 @@
 
 ## License
 
 nemoblock is published under the [GPLv3 license](https://www.gnu.org/licenses/gpl-3.0.html).
 
 ## Acknowledgements
 
-[This project](https://www.researchgate.net/project/NEMOCRYS-Next-Generation-Multiphysical-Models-for-Crystal-Growth-Processes) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
+[This project](https://nemocrys.github.io/) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
 
 <img src="https://raw.githubusercontent.com/nemocrys/nemoblock/master/EU-ERC.png">
 
 ## Contribution
 
 Any help to improve this package is very welcome!
```

### Comparing `nemoblock-1.0.3/nemoblock/blocks.py` & `nemoblock-1.0.4/nemoblock/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         return e
 
     def _add_block(self, block):
         block.id = self.block_count
         self.block_count += 1
         self.blocks.append(block)
 
-    def write(self):
-        if not os.path.exists("./system"):
-            os.makedirs("./system")
-        with open("./system/blockMeshDict", "w") as f:
+    def write(self, directory="./system"):
+        if not os.path.exists(directory):
+            os.makedirs(directory)
+        with open(f"{directory}/blockMeshDict", "w") as f:
             # header
             f.writelines(
                 [
                     "FoamFile\n",
                     "{\n",
                     "    version     2.0;\n",
                     "    format      ascii;\n",
```

### Comparing `nemoblock-1.0.3/nemoblock/cylinder.py` & `nemoblock-1.0.4/nemoblock/cylinder.py`

 * *Files identical despite different names*

### Comparing `nemoblock-1.0.3/nemoblock/experimental.py` & `nemoblock-1.0.4/nemoblock/experimental.py`

 * *Files identical despite different names*

### Comparing `nemoblock-1.0.3/nemoblock.egg-info/PKG-INFO` & `nemoblock-1.0.4/nemoblock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nemoblock
-Version: 1.0.3
+Version: 1.0.4
 Summary: Utilities to generate blockMeshDicts for OpenFOAM.
 Home-page: https://github.com/nemocrys/nemoblock
 Author: Arved Enders-Seidlitz
 Author-email: arved.enders-seidlitz@ikz-berlin.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nemoblock
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7503822.svg)](https://doi.org/10.5281/zenodo.7503822)
 
 ## Project description
 
 nemoblock provides utilities to generate blockMeshDicts for structured mesh generation in OpenFOAM. It manages the numbering of the points, the orientation of the surfaces and the connections between the blocks. In this way it helps the user to focus on the most important point: generating high quality meshes.
 
 The project is developed and maintained by the [**Model experiments group**](https://www.ikz-berlin.de/en/research/materials-science/section-fundamental-description#c486) at the Leibniz Institute for Crystal Growth (IKZ).
 
@@ -147,14 +148,14 @@
 
 ## License
 
 nemoblock is published under the [GPLv3 license](https://www.gnu.org/licenses/gpl-3.0.html).
 
 ## Acknowledgements
 
-[This project](https://www.researchgate.net/project/NEMOCRYS-Next-Generation-Multiphysical-Models-for-Crystal-Growth-Processes) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
+[This project](https://nemocrys.github.io/) has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation programme (grant agreement No 851768).
 
 <img src="https://raw.githubusercontent.com/nemocrys/nemoblock/master/EU-ERC.png">
 
 ## Contribution
 
 Any help to improve this package is very welcome!
```

### Comparing `nemoblock-1.0.3/setup.py` & `nemoblock-1.0.4/setup.py`

 * *Files identical despite different names*

