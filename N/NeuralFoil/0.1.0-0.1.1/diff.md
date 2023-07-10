# Comparing `tmp/NeuralFoil-0.1.0.tar.gz` & `tmp/NeuralFoil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.0.tar", last modified: Mon Jul 10 19:25:09 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.1.tar", last modified: Mon Jul 10 20:04:38 2023, max compression
```

## Comparing `NeuralFoil-0.1.0.tar` & `NeuralFoil-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:25:09.748929 NeuralFoil-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:25:09.748929 NeuralFoil-0.1.0/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-10 19:25:09.000000 NeuralFoil-0.1.0/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-10 19:25:09.000000 NeuralFoil-0.1.0/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:25:09.000000 NeuralFoil-0.1.0/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 19:25:09.000000 NeuralFoil-0.1.0/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 19:25:09.000000 NeuralFoil-0.1.0/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-10 19:25:09.748929 NeuralFoil-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:25:09.748929 NeuralFoil-0.1.0/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/neuralfoil/neuralfoil.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:25:09.748929 NeuralFoil-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-10 19:24:57.000000 NeuralFoil-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:38.757837 NeuralFoil-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:38.753837 NeuralFoil-0.1.1/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-10 20:04:38.000000 NeuralFoil-0.1.1/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 20:04:38.000000 NeuralFoil-0.1.1/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:04:38.000000 NeuralFoil-0.1.1/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 20:04:38.000000 NeuralFoil-0.1.1/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 20:04:38.000000 NeuralFoil-0.1.1/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-10 20:04:38.757837 NeuralFoil-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:38.753837 NeuralFoil-0.1.1/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:04:38.753837 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:04:38.757837 NeuralFoil-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-10 20:04:29.000000 NeuralFoil-0.1.1/setup.py
```

### Comparing `NeuralFoil-0.1.0/LICENSE.txt` & `NeuralFoil-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.0/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.1/NeuralFoil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.0
+Version: 0.1.1
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.0 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.1 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
```

### Comparing `NeuralFoil-0.1.0/PKG-INFO` & `NeuralFoil-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.0
+Version: 0.1.1
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.0 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.1 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
```

### Comparing `NeuralFoil-0.1.0/README.md` & `NeuralFoil-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.0/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.1/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.0/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.1/neuralfoil/neuralfoil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import aerosandbox as asb
 import aerosandbox.numpy as np
 from typing import Union, Dict, Set, List
 from pathlib import Path
 
-npz_file_directory = Path(__file__).parent.parent / "training"
+npz_file_directory = Path(__file__).parent / "nn_weights_and_biases"
 
 
 def get_aero_from_kulfan_parameters(
-        kulfan_parameters: dict[str, Union[float, np.ndarray]],
+        kulfan_parameters: Dict[str, Union[float, np.ndarray]],
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
         model_size="medium"
 ) -> Dict[str, Union[float, np.ndarray]]:
 
     ### Load the neural network parameters
     filename = npz_file_directory / f"nn-{model_size}.npz"
     if not filename.exists():
-        raise FileNotFoundError(f"Could not find the neural network file {filename}.")
+        raise FileNotFoundError(f"Could not find the neural network file {filename}, which contains the weights and biases.")
 
     data: Dict[str, np.ndarray] = np.load(filename)
 
     ### Prepare the inputs for the neural network
     input_rows: List[Union[float, np.ndarray]] = [
         4 * np.sind(2 * alpha),
         20 * (1 - np.cosd(alpha) ** 2),
         (np.log(Re) - 12.5) / 2,
         *[kulfan_parameters["lower_weights"][i] * 5 for i in range(8)],
         *[kulfan_parameters["upper_weights"][i] * 5 for i in range(8)],
         kulfan_parameters["leading_edge_weight"] * 5,
         kulfan_parameters["TE_thickness"] * 100,
     ]
 
+    ### Handle the vectorization, where here we figure out how many cases the user wants to run
     N_cases = 1  # TODO rework this with np.atleast1d
     for row in input_rows:
         if np.length(row) > 1:
             if N_cases == 1:
                 N_cases = np.length(row)
             else:
                 if np.length(row) != N_cases:
```

### Comparing `NeuralFoil-0.1.0/setup.py` & `NeuralFoil-0.1.1/setup.py`

 * *Files identical despite different names*

