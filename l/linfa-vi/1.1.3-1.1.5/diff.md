# Comparing `tmp/linfa_vi-1.1.3.tar.gz` & `tmp/linfa_vi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.1.3.tar", last modified: Mon Jul  3 19:13:43 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.5.tar", last modified: Mon Jul 10 15:27:59 2023, max compression
```

## Comparing `linfa_vi-1.1.3.tar` & `linfa_vi-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.548683 linfa_vi-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:13:43.544683 linfa_vi-1.1.3/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 19:13:43.000000 linfa_vi-1.1.3/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:13:43.548683 linfa_vi-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:13:32.000000 linfa_vi-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 15:27:59.000000 linfa_vi-1.1.5/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:27:59.438466 linfa_vi-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:27:49.000000 linfa_vi-1.1.5/setup.py
```

### Comparing `linfa_vi-1.1.3/LICENSE` & `linfa_vi-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/PKG-INFO` & `linfa_vi-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.1.3
+Version: 1.1.5
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -65,22 +65,23 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
+python -m unittest linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
+* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -90,32 +91,32 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT
+python linfa.plot_res -n NAME -i IT -f FOLDER
 ```
-where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
+where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
 
 * A computational model.
 * A surrogate model.
 * A log-likelihood model.
 * An optional transformation. 
 
 In addition you need to specify a list of options as discussed in the [documentation](https://linfa-vi.readthedocs.io/en/latest/content/linfa_options.html).
 
 ### Tutorial
 
-A (tutorial)[] is also available which will guide you through the definition of each of the quantities and function required by LINFA. 
+A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
 @misc{TO BE FINALIZED!!!,
       title={LINFA: a Python library for variational inference with normalizing flow and annealing},
```

### Comparing `linfa_vi-1.1.3/README.md` & `linfa_vi-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,22 +43,23 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
+python -m unittest linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
+* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -68,32 +69,32 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT
+python linfa.plot_res -n NAME -i IT -f FOLDER
 ```
-where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
+where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
 
 * A computational model.
 * A surrogate model.
 * A log-likelihood model.
 * An optional transformation. 
 
 In addition you need to specify a list of options as discussed in the [documentation](https://linfa-vi.readthedocs.io/en/latest/content/linfa_options.html).
 
 ### Tutorial
 
-A (tutorial)[] is also available which will guide you through the definition of each of the quantities and function required by LINFA. 
+A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
 @misc{TO BE FINALIZED!!!,
       title={LINFA: a Python library for variational inference with normalizing flow and annealing},
```

### Comparing `linfa_vi-1.1.3/linfa/maf.py` & `linfa_vi-1.1.5/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/linfa/nofas.py` & `linfa_vi-1.1.5/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/linfa/plot_res.py` & `linfa_vi-1.1.5/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/linfa/run_experiment.py` & `linfa_vi-1.1.5/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/linfa/transform.py` & `linfa_vi-1.1.5/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.1.3/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.5/linfa_vi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.1.3
+Version: 1.1.5
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -65,22 +65,23 @@
 * Three-element Windkessel model (a.k.a. RCR model).
 * Friedman 1 dataset example.
 
 The implementation of the lumped parameter network models (RC and RCR models) follows closely from the code developed by [the Schiavazzi Lab at the University of Notre Dame](https://github.com/desResLab/supplMatHarrod20).
 
 To run the tests type
 ```sh
-python -m unittest linfa.tests.test_linfa.linfa_test_suite.NAME_example
+python -m unittest linfa.linfa_test_suite.NAME_example
 ```
 where `NAME` need to be replaced by
 * `trivial` for the trivial example (Ex 1).
 * `highdim` for the high-dimensional example (Ex 2).
 * `rc` for the RC model (Ex 3).
 * `rcr` for the RCR model (Ex 4).
 * `adaann` for the Friedman model example (Ex 5).
+* `rcr_nofas_adaann_example` for the RCR model, combining NoFAS with adaptive annealing (AdaAnn)
 
 At regular intervals set by the parameter `experiment.save_interval` LINFA writes a few results files. The sub-string `NAME` refers to the experiment name specified in the `experiment.name` variable, and `IT` indicates the iteration at which the file is written. The results files are
 
 * `log.txt` contains the log profile information, i.e.
   * Iteration number.
   * Annealing temperature at each iteration.
   * Loss function at each iteration.
@@ -90,32 +91,32 @@
 * `NAME_logdensity_IT` contains the value of the log posterior density corresponding to each parameter realization. 
 * `NAME_outputs_IT` contains the true model (or surrogate model) outputs for each batch sample at iteration `IT`.
 * `NAME_IT.nf` contains a backup of the normalizing flow parameters at iteration `IT`.
 
 A post processing script is also available to plot all results. To run it type
 
 ```sh
-python linfa.plot_res -n NAME -i IT
+python linfa.plot_res -n NAME -i IT -f FOLDER
 ```
-where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest. 
+where `NAME` and `IT` are again the experiment name and iteration number corresponding to the result file of interest, while `FOLDER` is the name of the folder with the results of the inference task are kept.
 
 ### Usage
 
 To use LINFA with your model you need to specify the following components:
 
 * A computational model.
 * A surrogate model.
 * A log-likelihood model.
 * An optional transformation. 
 
 In addition you need to specify a list of options as discussed in the [documentation](https://linfa-vi.readthedocs.io/en/latest/content/linfa_options.html).
 
 ### Tutorial
 
-A (tutorial)[] is also available which will guide you through the definition of each of the quantities and function required by LINFA. 
+A step by step [tutorial](tutorial/TutorialwithPhys.ipynb) is also available which will guide you through the an inference problem for a ballistic simulation. 
 
 ### Citation
 
 Did you use LINFA? Please cite our paper using:
 ```
 @misc{TO BE FINALIZED!!!,
       title={LINFA: a Python library for variational inference with normalizing flow and annealing},
```

### Comparing `linfa_vi-1.1.3/pyproject.toml` & `linfa_vi-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.1.3"
+version = "1.1.5"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

