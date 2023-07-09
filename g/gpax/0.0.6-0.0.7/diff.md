# Comparing `tmp/gpax-0.0.6.tar.gz` & `tmp/gpax-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpax-0.0.6.tar", last modified: Mon Jan 16 04:13:00 2023, max compression
+gzip compressed data, was "dist/gpax-0.0.7.tar", last modified: Sun Jul  9 23:51:39 2023, max compression
```

## Comparing `gpax-0.0.6.tar` & `gpax-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-01-16 04:13:00.000000 gpax-0.0.6/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1072 2023-01-16 04:09:14.000000 gpax-0.0.6/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14637 2023-01-16 04:13:00.000000 gpax-0.0.6/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14018 2023-01-16 04:09:14.000000 gpax-0.0.6/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      361 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       18 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/__version__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9478 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/acquisition.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7827 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/dkl.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    17520 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/gp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6008 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/hypo.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3974 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/kernels.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5595 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/spm.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2901 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/utils.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8447 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/vgp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15753 2023-01-16 04:09:14.000000 gpax-0.0.6/gpax/vidkl.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14637 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      499 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/not-zip-safe
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       59 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-01-16 04:13:00.000000 gpax-0.0.6/gpax.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-01-16 04:13:00.000000 gpax-0.0.6/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1442 2023-01-16 04:09:14.000000 gpax-0.0.6/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-01-16 04:13:00.000000 gpax-0.0.6/tests/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1136 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_acq.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4307 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_dkl.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11803 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_gp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1114 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_hypo.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1884 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_spm.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6696 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_vgp.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9727 2023-01-16 04:09:14.000000 gpax-0.0.6/tests/test_vidkl.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-09 23:51:39.000000 gpax-0.0.7/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1072 2023-07-09 23:43:28.000000 gpax-0.0.7/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    16076 2023-07-09 23:51:39.000000 gpax-0.0.7/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15457 2023-07-09 23:43:28.000000 gpax-0.0.7/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      403 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       18 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/__version__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14055 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/acquisition.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7833 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/dkl.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    17308 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/gp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6008 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/hypo.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3974 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/kernels.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6557 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/spm.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3962 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/utils.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8447 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/vgp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15759 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/vidkl.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7621 2023-07-09 23:43:28.000000 gpax-0.0.7/gpax/vigp.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    16076 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      551 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/not-zip-safe
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       59 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2023-07-09 23:51:39.000000 gpax-0.0.7/gpax.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-07-09 23:51:39.000000 gpax-0.0.7/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1442 2023-07-09 23:43:28.000000 gpax-0.0.7/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-07-09 23:51:39.000000 gpax-0.0.7/tests/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2322 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_acq.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4307 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_dkl.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    12537 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_gp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1114 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_hypo.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1884 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_spm.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      793 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_utils.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6696 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_vgp.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9727 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_vidkl.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8699 2023-07-09 23:43:28.000000 gpax-0.0.7/tests/test_vigp.py
```

### Comparing `gpax-0.0.6/LICENSE` & `gpax-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/PKG-INFO` & `gpax-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,81 @@
 Metadata-Version: 2.1
 Name: gpax
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gaussian processes in NumPyro and JAX
 Home-page: https://github.com/ziatdinovmax/gpax/
 Author: Maxim Ziatdinov
 Author-email: maxim.ziatdinov@ai4microcopy.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPax
 [![build](https://github.com/ziatdinovmax/gpax/actions/workflows/actions.yml/badge.svg)](https://github.com/ziatdinovmax/gpax/actions/workflows/actions.yml)
 [![codecov](https://codecov.io/gh/ziatdinovmax/gpax/branch/main/graph/badge.svg?token=FFA8XB0FED)](https://codecov.io/gh/ziatdinovmax/gpax)
 [![PyPI version](https://badge.fury.io/py/gpax.svg)](https://badge.fury.io/py/gpax)
 
 GPax is a small Python package for physics-based Gaussian processes (GPs) built on top of NumPyro and JAX. Its purpose is to take advantage of prior physical knowledge and different data modalities when using GPs for data reconstruction and active learning. It is a work in progress, and more models will be added in the near future.
 
 ## How to use
 ### Simple GP
+#### *1D Example*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb)
 
 The code snippet below shows how to use vanilla GP in a fully Bayesian mode. First, we infer GP model parameters from the available training data
 ```python3
 import gpax
 
 # Get random number generator keys for training and prediction
 rng_key, rng_key_predict = gpax.utils.get_keys()
 # Initialize model
 gp_model = gpax.ExactGP(1, kernel='RBF')
 # Run Hamiltonian Monte Carlo to obtain posterior samples for the GP model parameters
 gp_model.fit(rng_key, X, y)  # X and y are numpy arrays with dimensions (n, d) and (n,)
 ```
-In the [fully Bayesian mode](https://docs.gpytorch.ai/en/v1.5.1/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.html), we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
+In the fully Bayesian mode, we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
 ```python3
 y_pred, y_sampled = gp_model.predict(rng_key_predict, X_test)
 ```
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945293-8cb5b88a-1f64-4f7d-95ab-26863b90d1e5.jpg" height="60%" width="60%">
 
 For 1-dimensional data, we can plot the GP prediction using the standard approach where the uncertainty in predictions - represented by a standard deviation in ```y_sampled``` - is depicted as a shaded area around the mean value. See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb).
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945487-05068084-86cb-4104-a792-d39d2f834151.jpg" height="60%" width="60%">
 
+#### *Sparse Image Reconstruction*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb)
+
+One can also use GP for sparse image reconstruction. The fully Bayesian GP is typically too slow for this purpose and it makes sense to use a stochastic variational inference approximation (viGP) instead. Code-wise, the usage of viGP in GPax is almost the same as that of the fully Bayesian GP. One difference is that instead of ```num_samples``` we have ```num_steps```. We can also control the learning rate by specifying a ```step_size```. 
+```python3
+# Get training inputs/targets and full image indices from sparse image data
+X_train, y_train, X_full = gpax.utils.preprocess_sparse_image(sparse_img) # sparse_img is a 2D numpy array
+
+# Initialize and train a variational inference GP model
+gp_model = gpax.viGP(2, kernel='Matern', guide='delta')
+gp_model.fit(rng_key, X_train, y_train, num_steps=250, step_size=0.05)
+```
+
+When we run the ```.predict()``` method, the output is predictive mean and variance computed from a learned single estimate of the GP model parameters:
+```python3
+y_pred, y_var = gp_model.predict(rng_key_predict, X_full)
+```
+<img src = "https://github.com/ziatdinovmax/gpax/assets/34245227/4c5036ee-4358-420d-b4d8-285b3ee81c09.jpg" height="75%" width="75%">
+
+See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb).
+
 ### Structured GP
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/GP_sGP.ipynb)
 
 The limitation of the standard GP is that it does not usually allow for the incorporation of prior domain knowledge and can be biased toward a trivial interpolative solution. Recently, we [introduced](https://arxiv.org/abs/2108.10280) a structured Gaussian Process (sGP), where a classical GP is augmented by a structured probabilistic model of the expected system’s behavior. This approach allows us to [balance](https://towardsdatascience.com/unknown-knowns-bayesian-inference-and-structured-gaussian-processes-why-domain-scientists-know-4659b7e924a4) the flexibility of the non-parametric GP approach with a rigid structure of prior (physical) knowledge encoded into the parametric model.
 Implementation-wise, we substitute a constant/zero prior mean function in GP with a probabilistic model of the expected system's behavior.
 
 For example, if we have prior knowledge that our objective function has a discontinuous 'phase transition', and a power law-like behavior before and after this transition, we may express it using a simple piecewise function
@@ -105,29 +127,29 @@
 
 ```python3
 # Train a GP model (it can be sGP or vanilla GP)
 gp_model.fit(rng_key, X_measured, y_measured)  # A
 
 # Compute the upper confidence bound (UCB) acquisition function to derive the next measurement point
 acq = gpax.acquisition.UCB(rng_key_predict, gp_model, X_unmeasured, beta=4, maximize=False, noiseless=True)  # B
-next_point_idx = acq.argmin()  # C
+next_point_idx = acq.argmax()  # C
 next_point = X_unmeasured[next_point_idx]  # D
 
 # Perform measurement in next_point, update measured & unmeasured data arrays, and re-run steps A-D.
 ```
 
-In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around x=0.7. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between x=-0.5 and x=0.5, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its minimum corresponds to the next measurement point in the active learning / Bayesian optimization setup. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
+In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around $x=0.7$. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between $x=-0.5$ and $x=0.5$, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its maximum corresponds to the next measurement point in the active learning and Bayesian optimization. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
 
-<img src="https://user-images.githubusercontent.com/34245227/185658311-1106f709-eba8-475e-9d3c-3d9f1c2a30d1.png">
+<img src="https://github.com/ziatdinovmax/gpax/assets/34245227/24f641fb-5959-4780-8d0e-edf62bd0a32b">
 
 
 ### Hypothesis learning
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb)
 
-The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb).
+The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb).
 
 <img src="https://user-images.githubusercontent.com/34245227/167936394-52f5ffd5-a47c-425d-b8a7-0727938dfab2.gif">
 
 
 ### Deep kernel learning
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viDKL_plasmons.ipynb)
```

### Comparing `gpax-0.0.6/README.md` & `gpax-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,38 +3,60 @@
 [![codecov](https://codecov.io/gh/ziatdinovmax/gpax/branch/main/graph/badge.svg?token=FFA8XB0FED)](https://codecov.io/gh/ziatdinovmax/gpax)
 [![PyPI version](https://badge.fury.io/py/gpax.svg)](https://badge.fury.io/py/gpax)
 
 GPax is a small Python package for physics-based Gaussian processes (GPs) built on top of NumPyro and JAX. Its purpose is to take advantage of prior physical knowledge and different data modalities when using GPs for data reconstruction and active learning. It is a work in progress, and more models will be added in the near future.
 
 ## How to use
 ### Simple GP
+#### *1D Example*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb)
 
 The code snippet below shows how to use vanilla GP in a fully Bayesian mode. First, we infer GP model parameters from the available training data
 ```python3
 import gpax
 
 # Get random number generator keys for training and prediction
 rng_key, rng_key_predict = gpax.utils.get_keys()
 # Initialize model
 gp_model = gpax.ExactGP(1, kernel='RBF')
 # Run Hamiltonian Monte Carlo to obtain posterior samples for the GP model parameters
 gp_model.fit(rng_key, X, y)  # X and y are numpy arrays with dimensions (n, d) and (n,)
 ```
-In the [fully Bayesian mode](https://docs.gpytorch.ai/en/v1.5.1/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.html), we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
+In the fully Bayesian mode, we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
 ```python3
 y_pred, y_sampled = gp_model.predict(rng_key_predict, X_test)
 ```
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945293-8cb5b88a-1f64-4f7d-95ab-26863b90d1e5.jpg" height="60%" width="60%">
 
 For 1-dimensional data, we can plot the GP prediction using the standard approach where the uncertainty in predictions - represented by a standard deviation in ```y_sampled``` - is depicted as a shaded area around the mean value. See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb).
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945487-05068084-86cb-4104-a792-d39d2f834151.jpg" height="60%" width="60%">
 
+#### *Sparse Image Reconstruction*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb)
+
+One can also use GP for sparse image reconstruction. The fully Bayesian GP is typically too slow for this purpose and it makes sense to use a stochastic variational inference approximation (viGP) instead. Code-wise, the usage of viGP in GPax is almost the same as that of the fully Bayesian GP. One difference is that instead of ```num_samples``` we have ```num_steps```. We can also control the learning rate by specifying a ```step_size```. 
+```python3
+# Get training inputs/targets and full image indices from sparse image data
+X_train, y_train, X_full = gpax.utils.preprocess_sparse_image(sparse_img) # sparse_img is a 2D numpy array
+
+# Initialize and train a variational inference GP model
+gp_model = gpax.viGP(2, kernel='Matern', guide='delta')
+gp_model.fit(rng_key, X_train, y_train, num_steps=250, step_size=0.05)
+```
+
+When we run the ```.predict()``` method, the output is predictive mean and variance computed from a learned single estimate of the GP model parameters:
+```python3
+y_pred, y_var = gp_model.predict(rng_key_predict, X_full)
+```
+<img src = "https://github.com/ziatdinovmax/gpax/assets/34245227/4c5036ee-4358-420d-b4d8-285b3ee81c09.jpg" height="75%" width="75%">
+
+See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb).
+
 ### Structured GP
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/GP_sGP.ipynb)
 
 The limitation of the standard GP is that it does not usually allow for the incorporation of prior domain knowledge and can be biased toward a trivial interpolative solution. Recently, we [introduced](https://arxiv.org/abs/2108.10280) a structured Gaussian Process (sGP), where a classical GP is augmented by a structured probabilistic model of the expected system’s behavior. This approach allows us to [balance](https://towardsdatascience.com/unknown-knowns-bayesian-inference-and-structured-gaussian-processes-why-domain-scientists-know-4659b7e924a4) the flexibility of the non-parametric GP approach with a rigid structure of prior (physical) knowledge encoded into the parametric model.
 Implementation-wise, we substitute a constant/zero prior mean function in GP with a probabilistic model of the expected system's behavior.
 
 For example, if we have prior knowledge that our objective function has a discontinuous 'phase transition', and a power law-like behavior before and after this transition, we may express it using a simple piecewise function
@@ -86,29 +108,29 @@
 
 ```python3
 # Train a GP model (it can be sGP or vanilla GP)
 gp_model.fit(rng_key, X_measured, y_measured)  # A
 
 # Compute the upper confidence bound (UCB) acquisition function to derive the next measurement point
 acq = gpax.acquisition.UCB(rng_key_predict, gp_model, X_unmeasured, beta=4, maximize=False, noiseless=True)  # B
-next_point_idx = acq.argmin()  # C
+next_point_idx = acq.argmax()  # C
 next_point = X_unmeasured[next_point_idx]  # D
 
 # Perform measurement in next_point, update measured & unmeasured data arrays, and re-run steps A-D.
 ```
 
-In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around x=0.7. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between x=-0.5 and x=0.5, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its minimum corresponds to the next measurement point in the active learning / Bayesian optimization setup. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
+In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around $x=0.7$. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between $x=-0.5$ and $x=0.5$, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its maximum corresponds to the next measurement point in the active learning and Bayesian optimization. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
 
-<img src="https://user-images.githubusercontent.com/34245227/185658311-1106f709-eba8-475e-9d3c-3d9f1c2a30d1.png">
+<img src="https://github.com/ziatdinovmax/gpax/assets/34245227/24f641fb-5959-4780-8d0e-edf62bd0a32b">
 
 
 ### Hypothesis learning
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb)
 
-The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb).
+The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb).
 
 <img src="https://user-images.githubusercontent.com/34245227/167936394-52f5ffd5-a47c-425d-b8a7-0727938dfab2.gif">
 
 
 ### Deep kernel learning
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viDKL_plasmons.ipynb)
```

### Comparing `gpax-0.0.6/gpax/dkl.py` & `gpax-0.0.7/gpax/dkl.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def __init__(self, input_dim: int, z_dim: int = 2, kernel: str = 'RBF',
                  kernel_prior: Optional[Callable[[], Dict[str, jnp.ndarray]]] = None,
                  nn: Optional[Callable[[jnp.ndarray, Dict[str, jnp.ndarray]], jnp.ndarray]] = None,
                  nn_prior: Optional[Callable[[], Dict[str, jnp.ndarray]]] = None,
                  latent_prior: Optional[Callable[[jnp.ndarray], Dict[str, jnp.ndarray]]] = None
                  ) -> None:
-        super(DKL, self).__init__(input_dim, kernel, kernel_prior)
+        super(DKL, self).__init__(input_dim, kernel, None, kernel_prior)
         self.nn = nn if nn else mlp
         self.nn_prior = nn_prior if nn_prior else mlp_prior(input_dim, z_dim)
         self.kernel_dim = z_dim
         self.latent_prior = latent_prior
 
     def model(self,
               X: jnp.ndarray,
```

### Comparing `gpax-0.0.6/gpax/gp.py` & `gpax-0.0.7/gpax/gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,15 @@
 from jax import jit
 from numpyro.infer import MCMC, NUTS, init_to_median, Predictive
 
 from .kernels import get_kernel
 from .utils import split_in_batches
 
 
-if jax.__version__ < '0.2.26':
-    clear_cache = jax.interpreters.xla._xla_callable.cache_clear
-else:
-    from jax._src import dispatch
-    try:
-        clear_cache = dispatch._xla_callable.cache_clear
-    except AttributeError:
-        clear_cache = dispatch.xla_callable.cache_clear
-
+clear_cache = jax._src.dispatch.xla_primitive_callable.cache_clear
 
 
 class ExactGP:
     """
     Gaussian process class
 
     Args:
@@ -224,15 +216,15 @@
                           ) -> Tuple[jnp.ndarray, jnp.ndarray]:
         """
         Returns parameters (mean and cov) of multivariate normal posterior
         for a single sample of GP parameters
         """
         noise = params["noise"]
         noise_p = noise * (1 - jnp.array(noiseless, int))
-        y_residual = self.y_train
+        y_residual = self.y_train.copy()
         if self.mean_fn is not None:
             args = [self.X_train, params] if self.mean_fn_prior else [self.X_train]
             y_residual -= self.mean_fn(*args).squeeze()
         # compute kernel matrices for train and test data
         k_pp = get_kernel(self.kernel)(X_new, X_new, params, noise_p, **kwargs)
         k_pX = get_kernel(self.kernel)(X_new, self.X_train, params, jitter=0.0)
         k_XX = get_kernel(self.kernel)(self.X_train, self.X_train, params, noise, **kwargs)
```

### Comparing `gpax-0.0.6/gpax/hypo.py` & `gpax-0.0.7/gpax/hypo.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/gpax/kernels.py` & `gpax-0.0.7/gpax/kernels.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/gpax/spm.py` & `gpax-0.0.7/gpax/spm.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 over the NumPyro's functions for Bayesian inference on probabilistic models.
 While it has no direct connection to Gaussian processes, this module may come
 in handy for comparisons between predicitons of GP and classical Bayesian models.
 
 Created by Maxim Ziatdinov (email: maxim.ziatdinov@ai4microscopy.com)
 """
 
-from typing import Callable, Dict, Optional, Tuple
+from typing import Callable, Optional, Tuple, Type, Dict
 
+import jax
+import jaxlib
 import jax.numpy as jnp
 import numpyro
 import numpyro.distributions as dist
 from numpyro.infer import MCMC, NUTS, Predictive, init_to_median
 
 model_type = Callable[[jnp.ndarray, Dict[str, jnp.ndarray]], jnp.ndarray]
 prior_type = Callable[[], Dict[str, jnp.ndarray]]
@@ -60,30 +62,36 @@
         sig = self.noise_prior()
         # Score against the observed data points
         numpyro.sample("y", dist.Normal(mu, sig), obs=y)
 
     def fit(self, rng_key: jnp.array, X: jnp.ndarray, y: jnp.ndarray,
             num_warmup: int = 2000, num_samples: int = 2000,
             num_chains: int = 1, chain_method: str = 'sequential',
-            progress_bar: bool = True, print_summary: bool = True) -> None:
+            progress_bar: bool = True, print_summary: bool = True,
+            device: Type[jaxlib.xla_extension.Device] = None) -> None:
         """
         Run HMC to infer parameters of the structured probabilistic model
 
         Args:
             rng_key: random number generator key
             X: 1D or 2D 'feature vector' with :math:`(n,)` or :math:`n x num_features` dimensions
             y: 1D 'target vector' with :math:`(n,)` dimensions
             num_warmup: number of HMC warmup states
             num_samples: number of HMC samples
             num_chains: number of HMC chains
             chain_method: 'sequential', 'parallel' or 'vectorized'
             progress_bar: show progress bar
             print_summary: print summary at the end of sampling
-        """
-
+            device:
+                optionally specify a cpu or gpu device on which to run the inference;
+                e.g., ``device=jax.devices("cpu")[0]`` 
+        """
+        if device:
+            X = jax.device_put(X, device)
+            y = jax.device_put(y, device)
         init_strategy = init_to_median(num_samples=10)
         kernel = NUTS(self.model, init_strategy=init_strategy)
         self.mcmc = MCMC(
             kernel,
             num_warmup=num_warmup,
             num_samples=num_samples,
             num_chains=num_chains,
@@ -116,33 +124,44 @@
         """
         prior_predictive = Predictive(self.model, num_samples=num_samples)
         samples = prior_predictive(rng_key, X)
         return samples['y']
 
     def predict(self, rng_key: jnp.ndarray, X_new: jnp.ndarray,
                 samples: Optional[Dict[str, jnp.ndarray]] = None,
-                filter_nans: bool = False) -> Tuple[jnp.ndarray, jnp.ndarray]:
+                filter_nans: bool = False, take_point_predictions_mean: bool = True,
+                device: Type[jaxlib.xla_extension.Device] = None
+                ) -> Tuple[jnp.ndarray, jnp.ndarray]:
         """
         Make prediction at X_new points using sampled GP hyperparameters
 
         Args:
             rng_key: random number generator key
             X_new: 2D vector with new/'test' data of :math:`n x num_features` dimensionality
             samples: optional posterior samples
             filter_nans: filter out samples containing NaN values (if any)
+            take_point_predictions_mean: take a mean of point predictions (without sampling from the normal distribution)
+            device:
+                optionally specify a cpu or gpu device on which to make a prediction;
+                e.g., ```device=jax.devices("gpu")[0]```
 
         Returns:
-            Center of the mass of sampled means and all the sampled predictions
+            Point predictions (or their mean) and posterior predictive distribution
         """
         if samples is None:
             samples = self.get_samples(chain_dim=False)
+        if device:
+            X_new = jax.device_put(X_new, device)
+            samples = jax.device_put(samples, device)
         predictive = Predictive(
             self.model, posterior_samples=samples, parallel=True)
         y_pred = predictive(rng_key, X_new)
         y_pred, y_sampled = y_pred["mu"], y_pred["y"]
         if filter_nans:
             y_sampled_ = [y_i for y_i in y_sampled if not jnp.isnan(y_i).any()]
             y_sampled = jnp.array(y_sampled_)
-        return y_pred.mean(0), y_sampled
+        if take_point_predictions_mean:
+            y_pred = y_pred.mean(0)
+        return y_pred, y_sampled
 
     def _print_summary(self):
         self.mcmc.print_summary()
```

### Comparing `gpax-0.0.6/gpax/utils.py` & `gpax-0.0.7/gpax/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -90,7 +90,27 @@
     import matplotlib.pyplot as plt
 
     with numpyro.handlers.seed(rng_seed=0):
         samples = d.sample(jax.random.PRNGKey(0), sample_shape=(samples,))
     plt.figure(dpi=100)
     sns.histplot(samples, kde=True, fill=False)
     plt.show()
+
+
+def preprocess_sparse_image(sparse_image):
+    """
+    Creates GP inputs from sparse image data where missing values are represented by zeros.
+    If your actual data contains zeros, you will need to (re-)normalize it.
+    Otherwise, those elements will be interpreted as missng values. The function returns
+    two arrays of the shapes (N, D) and (N,) that are used as training inputs and targets in GP
+    and an array of full indices of the shape (N_full, D) for reconstructing the full image. D is
+    the image dimensionality (D=2 for a 2D image)
+    """
+    # Find non-zero element indices
+    non_zero_indices = onp.nonzero(sparse_image)
+    # Create the GP input using the indices
+    gp_input = onp.column_stack(non_zero_indices)
+    # Extract non-zero values (targets) from the sparse image
+    targets = sparse_image[non_zero_indices]
+    # Generate indices for the entire image
+    full_indices = onp.array(onp.meshgrid(*[onp.arange(dim) for dim in sparse_image.shape])).T.reshape(-1, sparse_image.ndim)
+    return gp_input, targets, full_indices
```

### Comparing `gpax-0.0.6/gpax/vgp.py` & `gpax-0.0.7/gpax/vgp.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/gpax/vidkl.py` & `gpax-0.0.7/gpax/vidkl.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def __init__(self, input_dim: int, z_dim: int = 2, kernel: str = 'RBF',
                  kernel_prior: Optional[Callable[[], Dict[str, jnp.ndarray]]] = None,
                  nn: Optional[Callable[[jnp.ndarray], jnp.ndarray]] = None,
                  latent_prior: Optional[Callable[[jnp.ndarray], Dict[str, jnp.ndarray]]] = None,
                  guide: str = 'delta'
                  ) -> None:
-        super(viDKL, self).__init__(input_dim, kernel, kernel_prior)
+        super(viDKL, self).__init__(input_dim, kernel, None, kernel_prior)
         if guide not in ['delta', 'normal']:
             raise NotImplementedError("Select guide between 'delta' and 'normal'")
         nn_module = nn if nn else MLP
         self.nn_module = hk.transform(lambda x: nn_module(z_dim)(x))
         self.kernel_dim = z_dim
         self.data_dim = (input_dim,) if isinstance(input_dim, int) else input_dim
         self.latent_prior = latent_prior
```

### Comparing `gpax-0.0.6/gpax.egg-info/PKG-INFO` & `gpax-0.0.7/gpax.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,81 @@
 Metadata-Version: 2.1
 Name: gpax
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gaussian processes in NumPyro and JAX
 Home-page: https://github.com/ziatdinovmax/gpax/
 Author: Maxim Ziatdinov
 Author-email: maxim.ziatdinov@ai4microcopy.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPax
 [![build](https://github.com/ziatdinovmax/gpax/actions/workflows/actions.yml/badge.svg)](https://github.com/ziatdinovmax/gpax/actions/workflows/actions.yml)
 [![codecov](https://codecov.io/gh/ziatdinovmax/gpax/branch/main/graph/badge.svg?token=FFA8XB0FED)](https://codecov.io/gh/ziatdinovmax/gpax)
 [![PyPI version](https://badge.fury.io/py/gpax.svg)](https://badge.fury.io/py/gpax)
 
 GPax is a small Python package for physics-based Gaussian processes (GPs) built on top of NumPyro and JAX. Its purpose is to take advantage of prior physical knowledge and different data modalities when using GPs for data reconstruction and active learning. It is a work in progress, and more models will be added in the near future.
 
 ## How to use
 ### Simple GP
+#### *1D Example*
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb)
 
 The code snippet below shows how to use vanilla GP in a fully Bayesian mode. First, we infer GP model parameters from the available training data
 ```python3
 import gpax
 
 # Get random number generator keys for training and prediction
 rng_key, rng_key_predict = gpax.utils.get_keys()
 # Initialize model
 gp_model = gpax.ExactGP(1, kernel='RBF')
 # Run Hamiltonian Monte Carlo to obtain posterior samples for the GP model parameters
 gp_model.fit(rng_key, X, y)  # X and y are numpy arrays with dimensions (n, d) and (n,)
 ```
-In the [fully Bayesian mode](https://docs.gpytorch.ai/en/v1.5.1/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.html), we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
+In the fully Bayesian mode, we get a pair of predictive mean and covariance for each Hamiltonian Monte Carlo sample containing the GP parameters (in this case, the RBF kernel hyperparameters and model noise). Hence, a prediction on new inputs with a trained GP model returns the center of the mass of all the predictive means (```y_pred```) and samples from multivariate normal distributions for all the pairs of predictive means and covariances (```y_sampled```).
 ```python3
 y_pred, y_sampled = gp_model.predict(rng_key_predict, X_test)
 ```
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945293-8cb5b88a-1f64-4f7d-95ab-26863b90d1e5.jpg" height="60%" width="60%">
 
 For 1-dimensional data, we can plot the GP prediction using the standard approach where the uncertainty in predictions - represented by a standard deviation in ```y_sampled``` - is depicted as a shaded area around the mean value. See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/simpleGP.ipynb).
 
 <img src = "https://user-images.githubusercontent.com/34245227/167945487-05068084-86cb-4104-a792-d39d2f834151.jpg" height="60%" width="60%">
 
+#### *Sparse Image Reconstruction*
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb)
+
+One can also use GP for sparse image reconstruction. The fully Bayesian GP is typically too slow for this purpose and it makes sense to use a stochastic variational inference approximation (viGP) instead. Code-wise, the usage of viGP in GPax is almost the same as that of the fully Bayesian GP. One difference is that instead of ```num_samples``` we have ```num_steps```. We can also control the learning rate by specifying a ```step_size```. 
+```python3
+# Get training inputs/targets and full image indices from sparse image data
+X_train, y_train, X_full = gpax.utils.preprocess_sparse_image(sparse_img) # sparse_img is a 2D numpy array
+
+# Initialize and train a variational inference GP model
+gp_model = gpax.viGP(2, kernel='Matern', guide='delta')
+gp_model.fit(rng_key, X_train, y_train, num_steps=250, step_size=0.05)
+```
+
+When we run the ```.predict()``` method, the output is predictive mean and variance computed from a learned single estimate of the GP model parameters:
+```python3
+y_pred, y_var = gp_model.predict(rng_key_predict, X_full)
+```
+<img src = "https://github.com/ziatdinovmax/gpax/assets/34245227/4c5036ee-4358-420d-b4d8-285b3ee81c09.jpg" height="75%" width="75%">
+
+See the full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viGP.ipynb).
+
 ### Structured GP
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/GP_sGP.ipynb)
 
 The limitation of the standard GP is that it does not usually allow for the incorporation of prior domain knowledge and can be biased toward a trivial interpolative solution. Recently, we [introduced](https://arxiv.org/abs/2108.10280) a structured Gaussian Process (sGP), where a classical GP is augmented by a structured probabilistic model of the expected system’s behavior. This approach allows us to [balance](https://towardsdatascience.com/unknown-knowns-bayesian-inference-and-structured-gaussian-processes-why-domain-scientists-know-4659b7e924a4) the flexibility of the non-parametric GP approach with a rigid structure of prior (physical) knowledge encoded into the parametric model.
 Implementation-wise, we substitute a constant/zero prior mean function in GP with a probabilistic model of the expected system's behavior.
 
 For example, if we have prior knowledge that our objective function has a discontinuous 'phase transition', and a power law-like behavior before and after this transition, we may express it using a simple piecewise function
@@ -105,29 +127,29 @@
 
 ```python3
 # Train a GP model (it can be sGP or vanilla GP)
 gp_model.fit(rng_key, X_measured, y_measured)  # A
 
 # Compute the upper confidence bound (UCB) acquisition function to derive the next measurement point
 acq = gpax.acquisition.UCB(rng_key_predict, gp_model, X_unmeasured, beta=4, maximize=False, noiseless=True)  # B
-next_point_idx = acq.argmin()  # C
+next_point_idx = acq.argmax()  # C
 next_point = X_unmeasured[next_point_idx]  # D
 
 # Perform measurement in next_point, update measured & unmeasured data arrays, and re-run steps A-D.
 ```
 
-In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around x=0.7. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between x=-0.5 and x=0.5, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its minimum corresponds to the next measurement point in the active learning / Bayesian optimization setup. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
+In the figure below we illustrate the connection between the (s)GP posterior predictive distribution and the acquisiton function used to derive the next measurement points. Here, the posterior mean values indicate that the minimum of a "black box" function describing a behaviour of interest is around $x=0.7$. At the same time, there is a large dispersion in the samples from the posterior predictive distribution between $x=-0.5$ and $x=0.5$, resulting in a high uncertainty in that region. The acquisition function is computed as a function of both predictive mean and uncertainty and its maximum corresponds to the next measurement point in the active learning and Bayesian optimization. Here, after taking into account the uncertainty in the prediction, the UCB acquisition function suggests exploring a point at x≈0 where potentially a true minimum is located. See full example [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_GPBO.ipynb).
 
-<img src="https://user-images.githubusercontent.com/34245227/185658311-1106f709-eba8-475e-9d3c-3d9f1c2a30d1.png">
+<img src="https://github.com/ziatdinovmax/gpax/assets/34245227/24f641fb-5959-4780-8d0e-edf62bd0a32b">
 
 
 ### Hypothesis learning
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb)
 
-The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/hypoAL.ipynb).
+The structured GP can be also used for hypothesis learning in automated experiments. The [hypothesis learning](https://arxiv.org/abs/2112.06649) is based on the idea that in active learning, the correct model of the system’s behavior leads to a faster decrease in the overall Bayesian uncertainty about the system under study. In the hypothesis learning setup, probabilistic models of the possible system’s behaviors (hypotheses) are wrapped into structured GPs, and a basic reinforcement learning policy is used to select a correct model from several competing hypotheses. The example of hypothesis learning on toy data is available [here](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_hypo.ipynb).
 
 <img src="https://user-images.githubusercontent.com/34245227/167936394-52f5ffd5-a47c-425d-b8a7-0727938dfab2.gif">
 
 
 ### Deep kernel learning
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ziatdinovmax/gpax/blob/main/examples/gpax_viDKL_plasmons.ipynb)
```

### Comparing `gpax-0.0.6/setup.py` & `gpax-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 with open(os.path.join(module_dir, 'gpax/__version__.py')) as f:
     __version__ = f.read().split("'")[1]
 
 if __name__ == "__main__":
     setup(
         name='gpax',
-        python_requires='>=3.7',
+        python_requires='>=3.9',
         version=__version__,
         description='Gaussian processes in NumPyro and JAX',
         long_description=open(os.path.join(module_dir, 'README.md')).read(),
         long_description_content_type='text/markdown',
         url='https://github.com/ziatdinovmax/gpax/',
         author='Maxim Ziatdinov',
         author_email='maxim.ziatdinov@ai4microcopy.com',
         license='MIT license',
         packages=find_packages(),
         zip_safe=False,
         install_requires=[
-            'jax>=0.2.21',
-            'numpyro>=0.8.0',
+            'jax>=0.4.8',
+            'numpyro>=0.11.0',
             'dm-haiku>=0.0.5',
             'matplotlib>=3.1'
         ],
         classifiers=['Programming Language :: Python',
                      'Development Status :: 3 - Alpha',
                      'Intended Audience :: Science/Research',
                      'Operating System :: POSIX :: Linux',
```

### Comparing `gpax-0.0.6/tests/test_acq.py` & `gpax-0.0.7/tests/test_acq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import pytest
 import numpy as onp
 import jax.numpy as jnp
-from numpy.testing import assert_equal
+from numpy.testing import assert_equal, assert_
 
 sys.path.insert(0, "../gpax/")
 
 from gpax.gp import ExactGP
 from gpax.dkl import DKL
 from gpax.vidkl import viDKL
 from gpax.utils import get_keys
@@ -18,22 +18,54 @@
     rng_keys = get_keys()
     X = onp.random.randn(8,)
     X_new = onp.random.randn(12,)
     y = 10 * X**2
     m = ExactGP(1, 'RBF')
     m.fit(rng_keys[0], X, y, num_warmup=100, num_samples=100)
     obj = acq(rng_keys[1], m, X_new)
-    assert isinstance(obj, jnp.ndarray)
+    assert_(isinstance(obj, jnp.ndarray))
     assert_equal(obj.squeeze().shape, (len(X_new),))
 
 
 @pytest.mark.parametrize("acq", [EI, UCB, UE, Thompson])
 def test_acq_dkl(acq):
     rng_keys = get_keys()
     X = onp.random.randn(32, 36)
     y = onp.random.randn(32,)
     X_new = onp.random.randn(10, 36)
     m = viDKL(X.shape[-1])
     m.fit(rng_keys[0], X, y, num_steps=20, step_size=0.05)
     obj = acq(rng_keys[1], m, X_new)
-    assert isinstance(obj, jnp.ndarray)
+    assert_(isinstance(obj, jnp.ndarray))
     assert_equal(obj.squeeze().shape, (len(X_new),))
+
+
+@pytest.mark.parametrize("acq", [EI, UCB, UE])
+def test_acq_penalty(acq):
+    rng_keys = get_keys()
+    X = onp.random.randn(8,)
+    X_new = onp.random.randn(12,)
+    y = 10 * X**2
+    m = ExactGP(1, 'RBF')
+    m.fit(rng_keys[0], X, y, num_warmup=100, num_samples=100)
+    obj1 = acq(rng_keys[1], m, X_new)
+    recent_points = onp.array(X_new[2:4] - 0.02)
+    obj2 = acq(rng_keys[1], m, X_new, distance_penalty=0.1, recent_points=recent_points)
+    assert_(onp.count_nonzero(obj1 - obj2) > 0)
+
+
+@pytest.mark.parametrize("acq", [EI, UCB, UE])
+def test_acq_penalty_indices(acq):
+    rng_keys = get_keys()
+    h = w = 5
+    X = onp.random.randn(h*w, 16)
+    y = onp.random.randn(len(X))
+    indices = onp.array([(i, j) for i in range(h) for j in range(w)])
+    X_new = onp.random.randn(h*w, 16)
+    m = viDKL(input_dim=16)
+    m.fit(rng_keys[0], X, y, num_steps=50)
+    obj1 = acq(rng_keys[1], m, X_new, grid_indices=indices,
+               distance_penalty=0.1, recent_points=indices[5:7])
+    obj2 = acq(rng_keys[1], m, X_new)
+    assert_(isinstance(obj1, jnp.ndarray))
+    assert_equal(obj1.squeeze().shape, (len(X_new),))
+    assert_(onp.count_nonzero(obj1 - obj2) > 0)
```

### Comparing `gpax-0.0.6/tests/test_dkl.py` & `gpax-0.0.7/tests/test_dkl.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/tests/test_gp.py` & `gpax-0.0.7/tests/test_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,41 +189,58 @@
     m.y_train = y
     y_mean1, y_sampled1 = m.predict(rng_keys[1], X_test, samples, n=1, noiseless=True)
     y_mean2, y_sampled2 = m.predict(rng_keys[1], X_test, samples, n=1, noiseless=False)
     assert_array_equal(y_mean1, y_mean2)
     assert onp.count_nonzero(y_sampled1 - y_sampled2) > 0
 
 
+@pytest.mark.parametrize("batch_size", [2, 3, 8])
+@pytest.mark.parametrize("n", [1, 10])
+def test_prediction_in_batches(batch_size, n):
+    rng_keys = get_keys()
+    X, y = get_dummy_data(unsqueeze=True)
+    X_test, _ = get_dummy_data()
+    samples = {"k_length": jax.random.normal(rng_keys[0], shape=(100, 1)),
+               "k_scale": jax.random.normal(rng_keys[0], shape=(100,)),
+               "noise": jax.random.normal(rng_keys[0], shape=(100,))}
+    m = ExactGP(1, 'RBF')
+    m.X_train = X
+    m.y_train = y
+    y_pred, y_sampled = m.predict_in_batches(rng_keys[1], X_test, batch_size, samples, n=n)
+    assert isinstance(y_pred, jnp.ndarray)
+    assert isinstance(y_sampled, jnp.ndarray)
+    assert_equal(y_pred.shape, X_test.squeeze().shape)
+    assert_equal(y_sampled.shape, (100, n, X_test.shape[0]))
+
+
 @pytest.mark.parametrize("kernel", ['RBF', 'Matern', 'Periodic'])
 def test_fit_predict(kernel):
     rng_keys = get_keys()
     X, y = get_dummy_data()
     X_test, _ = get_dummy_data()
     m = ExactGP(1, kernel)
     m.fit(rng_keys[0], X, y, num_warmup=100, num_samples=100)
     y_pred, y_sampled = m.predict(rng_keys[1], X_test)
     assert isinstance(y_pred, jnp.ndarray)
     assert isinstance(y_sampled, jnp.ndarray)
     assert_equal(y_pred.shape, X_test.squeeze().shape)
-    print(y_sampled.shape)
     assert_equal(y_sampled.shape, (100, 1, X_test.shape[0]))
 
 
 @pytest.mark.parametrize("n", [1, 10])
 def test_fit_predict_in_batches(n):
     rng_keys = get_keys()
     X, y = get_dummy_data()
     X_test, _ = get_dummy_data()
     m = ExactGP(1, 'RBF')
     m.fit(rng_keys[0], X, y, num_warmup=100, num_samples=100)
     y_pred, y_sampled = m.predict_in_batches(rng_keys[1], X_test, batch_size=4, n=n)
     assert isinstance(y_pred, jnp.ndarray)
     assert isinstance(y_sampled, jnp.ndarray)
     assert_equal(y_pred.shape, X_test.squeeze().shape)
-    print(y_sampled.shape)
     assert_equal(y_sampled.shape, (100, n, X_test.shape[0]))
 
 
 @pytest.mark.parametrize("n", [1, 10])
 def test_fit_noiseless_predict_in_batches(n):
     rng_keys = get_keys()
     X, y = get_dummy_data()
@@ -260,15 +277,14 @@
     X_test, _ = get_dummy_data()
     m = ExactGP(1, 'RBF', mean_fn = lambda x: 8*x**2)
     m.fit(rng_keys[0], X, y, num_warmup=100, num_samples=100)
     y_pred, y_sampled = m.predict(rng_keys[1], X_test)
     assert isinstance(y_pred, jnp.ndarray)
     assert isinstance(y_sampled, jnp.ndarray)
     assert_equal(y_pred.shape, X_test.squeeze().shape)
-    print(y_sampled.shape)
     assert_equal(y_sampled.shape, (100, 1, X_test.shape[0]))
 
 
 def test_fit_predict_with_prob_mean_fn():
     rng_keys = get_keys()
     X, y = get_dummy_data()
     X_test, _ = get_dummy_data()
```

### Comparing `gpax-0.0.6/tests/test_hypo.py` & `gpax-0.0.7/tests/test_hypo.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/tests/test_spm.py` & `gpax-0.0.7/tests/test_spm.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/tests/test_vgp.py` & `gpax-0.0.7/tests/test_vgp.py`

 * *Files identical despite different names*

### Comparing `gpax-0.0.6/tests/test_vidkl.py` & `gpax-0.0.7/tests/test_vidkl.py`

 * *Files identical despite different names*

