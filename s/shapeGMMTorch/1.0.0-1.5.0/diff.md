# Comparing `tmp/shapeGMMTorch-1.0.0.tar.gz` & `tmp/shapeGMMTorch-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapeGMMTorch-1.0.0.tar", last modified: Fri Jun  9 16:20:29 2023, max compression
+gzip compressed data, was "shapeGMMTorch-1.5.0.tar", last modified: Mon Jul 10 14:29:09 2023, max compression
```

## Comparing `shapeGMMTorch-1.0.0.tar` & `shapeGMMTorch-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-06-09 16:20:29.523892 shapeGMMTorch-1.0.0/
--rw-r--r--   0 mmccull    (502) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.0.0/LICENSE
--rw-r--r--   0 mmccull    (502) staff       (20)     5048 2023-06-09 16:20:29.523480 shapeGMMTorch-1.0.0/PKG-INFO
--rw-r--r--   0 mmccull    (502) staff       (20)     4441 2022-08-18 21:28:43.000000 shapeGMMTorch-1.0.0/README.md
--rw-r--r--   0 mmccull    (502) staff       (20)       38 2023-06-09 16:20:29.523989 shapeGMMTorch-1.0.0/setup.cfg
--rw-r--r--   0 mmccull    (502) staff       (20)     1006 2023-06-09 16:17:10.000000 shapeGMMTorch-1.0.0/setup.py
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-06-09 16:20:29.471681 shapeGMMTorch-1.0.0/src/
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-06-09 16:20:29.509997 shapeGMMTorch-1.0.0/src/shapeGMMTorch/
--rw-r--r--   0 mmccull    (502) staff       (20)        0 2022-08-10 01:10:39.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/__init__.py
--rw-r--r--   0 mmccull    (502) staff       (20)     4268 2022-08-19 20:33:04.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/scripts.py
--rw-r--r--   0 mmccull    (502) staff       (20)    13593 2023-02-03 20:52:08.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_align.py
--rw-r--r--   0 mmccull    (502) staff       (20)     6368 2023-02-03 20:52:08.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
--rw-r--r--   0 mmccull    (502) staff       (20)    17478 2023-02-03 20:52:08.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_sgmm.py
--rw-r--r--   0 mmccull    (502) staff       (20)     5648 2022-08-18 21:06:31.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
-drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-06-09 16:20:29.523105 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/
--rw-r--r--   0 mmccull    (502) staff       (20)     5048 2023-06-09 16:20:29.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/PKG-INFO
--rw-r--r--   0 mmccull    (502) staff       (20)      444 2023-06-09 16:20:29.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/SOURCES.txt
--rw-r--r--   0 mmccull    (502) staff       (20)        1 2023-06-09 16:20:29.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/dependency_links.txt
--rw-r--r--   0 mmccull    (502) staff       (20)       18 2023-06-09 16:20:29.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/requires.txt
--rw-r--r--   0 mmccull    (502) staff       (20)       14 2023-06-09 16:20:29.000000 shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/top_level.txt
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.962952 shapeGMMTorch-1.5.0/
+-rw-r--r--   0 mmccull    (502) staff       (20)     1070 2022-08-10 01:36:42.000000 shapeGMMTorch-1.5.0/LICENSE
+-rw-r--r--   0 mmccull    (502) staff       (20)     7554 2023-07-10 14:29:09.962504 shapeGMMTorch-1.5.0/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)     6967 2023-07-10 14:27:00.000000 shapeGMMTorch-1.5.0/README.md
+-rw-r--r--   0 mmccull    (502) staff       (20)       38 2023-07-10 14:29:09.963068 shapeGMMTorch-1.5.0/setup.cfg
+-rw-r--r--   0 mmccull    (502) staff       (20)     1006 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/setup.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.942210 shapeGMMTorch-1.5.0/src/
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.960735 shapeGMMTorch-1.5.0/src/shapeGMMTorch/
+-rw-r--r--   0 mmccull    (502) staff       (20)        0 2023-06-28 14:43:45.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/__init__.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     2881 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/plots.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     7292 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/scripts.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    13593 2023-06-28 14:43:45.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_align.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     6529 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py
+-rw-r--r--   0 mmccull    (502) staff       (20)    19790 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_sgmm.py
+-rw-r--r--   0 mmccull    (502) staff       (20)     5781 2023-07-10 14:27:01.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py
+drwxr-xr-x   0 mmccull    (502) staff       (20)        0 2023-07-10 14:29:09.962172 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/
+-rw-r--r--   0 mmccull    (502) staff       (20)     7554 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/PKG-INFO
+-rw-r--r--   0 mmccull    (502) staff       (20)      471 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/SOURCES.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)        1 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/dependency_links.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       18 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/requires.txt
+-rw-r--r--   0 mmccull    (502) staff       (20)       14 2023-07-10 14:29:09.000000 shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/top_level.txt
```

### Comparing `shapeGMMTorch-1.0.0/LICENSE` & `shapeGMMTorch-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.0.0/PKG-INFO` & `shapeGMMTorch-1.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.0.0
+Version: 1.5.0
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,27 +44,33 @@
 
 `pip install shapeGMMTorch`
 
 or by downloading from github and then running
 
 `python setup.py install`
 
+### Installation on a MAC
+
+I have found that PyTorch does not work on a mac using standard `pip install torch` or conda.  Instead, you have to create a special `nomkl` conda environment and install all necessary packages in there.  There are various blogs and/or stack overflow threads on this.
+
+After the `nomkl` conda environment has been created and all dependencies have been added to that environment, shapeGMMTorch can be installed.  Only the `torch.device("cpu")` device will work on a mac, however.
+
 ## Usage 
 
 This package is designed to mimic the usage of the sklearn package.  You first initiliaze the object and then fit.  Predict can be done once the model is fit.  Fit and ppredict functions take particle position trajectories as input in the form of a `(n_frames, n_atoms, 3)` numpy array.
 
 ### Initialize:
 
 `from shapeGMMTorch import torch_sgmm`
 
-Uniform (spherical, uncorrelated) covariance:
+Uniform covariance (spherical, uncorrelated, homogeneous):
 
 `usgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'uniform', verbose=True)`
 
-Weighted (Kronecker product) covariance:
+Kronecker product covariance (formerly call weighted covariance; spherical, correlated, heterogeneous):
 
 `wsgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'kronecker', verbose=True)`
 
 During initialization, the following options are availble:
 
 	- n_clusters (required)   - integer number of clusters must be input
 	- covar_type              - string defining the covariance type.  Options are 'kronecker' and 'uniform'.  Defualt is 'uniform'.
@@ -76,41 +81,64 @@
 	- kabsch_thresh           - float dictating convergence criteria for each iterative alignment (Maximization step).  Default value is 1e-1.
 	- dtype                   - Torch data type to be used.  Default is torch.float32.
 	- device                  - Torch device to be used.  Default is torch.device('cuda:0') device.
 	- verbose                 - boolean dictating whether to print various things at every step. Defualt is False.
 
 ### Fit:
 
-`uniform_aligned_trajectory = usgmm.fit(training_set_positions)`
+A standard fit can be performed in the following manner:
+
+`uniform_aligned_trajectory = usgmm.fit(train_positions)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions)`
+
+where `train_positions` is an array of dimensions `(n_train_frames, n_atoms, 3)`. Notice there is no difference in syntax when fitting the two covariance types.  Two additional options are available during the fit routine which may be necessary under certain situations:
+
+	- cluster_ids   (optional) - (n_train_frames) integer array of initial cluster ids.  This option is necessary if init_cluster_method = 'read'
+	- frame_weights (optional) - (n_train_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
+
+If these options are used the fit call looks like
 
-`kronecker_aligned_trajectory = wsgmm.fit(training_set_positions)`
+`uniform_aligned_trajectory = usgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
 
 ### Predict:
 
+Once the shapeGMM object has been fit, it can be used to precict cluster IDs, aligned trajectory, and log likelihood per frame for a new, or cross validation, trajectory.  The number of atoms must remain the same.  The simple syntax is as follows:
+
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions)`
+
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions)`
+
+where `predict_positions` is an array of dimensions `(n_predict_frames, n_atoms, 3)`. Notice there is no difference in syntax when precicting the two covariance types.  If the predict frames have a non-unifrom frame weight, this can be accounted for  
 
-`clusters, aligned_traj, log_likelihood = usgmm.predict(full_trajectory_positions)`
+	- frame_weights (optional) - (n_predict_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
 
-`clusters, aligned_traj, log_likelihood = wsgmm.predict(full_trajectory_positions)`
+If this option is used the predict call will look like
+
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
+
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
 
 ## Attributes
 
 After being properly fit, a shapeGMM object will have the following attributes:
 
-	- n_clusters		- integer of how many clusters were used in training
-	- n_atoms           	- integer of how many atoms were in the training data
-	- clusters              - integer array of cluster ids for training data
-	- log_likelihood        - float log likelihood of training set
-	- weights               - (n_clusters) float array of cluster weights
-	- centers	      	- (n_clusters, n_atoms, 3) float array of cluster centers/averages
+	- n_clusters	    - integer of how many clusters were used in training
+	- n_atoms           - integer of how many atoms were in the training data
+	- n_train_frames    - integer of how many frames were in the training data
+	- clusters_ids      - integer array of cluster ids for training data
+	- log_likelihood    - float log likelihood of training set
+	- weights           - (n_clusters) float array of cluster weights
+	- centers	        - (n_clusters, n_atoms, 3) float array of cluster centers/averages
 
 Uniform covariance specific attributes
 
 	- vars		       	- (n_clusters) float array of cluster variances
 
 Kronecker covariance specific attributes
 
 	- precisions	   	- (n_clusters, n_atoms, n_atoms) float array of cluster precisions (inverse covariances)
 	- lpdets	    	- (n_clusters) float array of ln(det(covar))
 
 
-
-
```

### Comparing `shapeGMMTorch-1.0.0/README.md` & `shapeGMMTorch-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -28,27 +28,33 @@
 
 `pip install shapeGMMTorch`
 
 or by downloading from github and then running
 
 `python setup.py install`
 
+### Installation on a MAC
+
+I have found that PyTorch does not work on a mac using standard `pip install torch` or conda.  Instead, you have to create a special `nomkl` conda environment and install all necessary packages in there.  There are various blogs and/or stack overflow threads on this.
+
+After the `nomkl` conda environment has been created and all dependencies have been added to that environment, shapeGMMTorch can be installed.  Only the `torch.device("cpu")` device will work on a mac, however.
+
 ## Usage 
 
 This package is designed to mimic the usage of the sklearn package.  You first initiliaze the object and then fit.  Predict can be done once the model is fit.  Fit and ppredict functions take particle position trajectories as input in the form of a `(n_frames, n_atoms, 3)` numpy array.
 
 ### Initialize:
 
 `from shapeGMMTorch import torch_sgmm`
 
-Uniform (spherical, uncorrelated) covariance:
+Uniform covariance (spherical, uncorrelated, homogeneous):
 
 `usgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'uniform', verbose=True)`
 
-Weighted (Kronecker product) covariance:
+Kronecker product covariance (formerly call weighted covariance; spherical, correlated, heterogeneous):
 
 `wsgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'kronecker', verbose=True)`
 
 During initialization, the following options are availble:
 
 	- n_clusters (required)   - integer number of clusters must be input
 	- covar_type              - string defining the covariance type.  Options are 'kronecker' and 'uniform'.  Defualt is 'uniform'.
@@ -59,35 +65,60 @@
 	- kabsch_thresh           - float dictating convergence criteria for each iterative alignment (Maximization step).  Default value is 1e-1.
 	- dtype                   - Torch data type to be used.  Default is torch.float32.
 	- device                  - Torch device to be used.  Default is torch.device('cuda:0') device.
 	- verbose                 - boolean dictating whether to print various things at every step. Defualt is False.
 
 ### Fit:
 
-`uniform_aligned_trajectory = usgmm.fit(training_set_positions)`
+A standard fit can be performed in the following manner:
+
+`uniform_aligned_trajectory = usgmm.fit(train_positions)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions)`
+
+where `train_positions` is an array of dimensions `(n_train_frames, n_atoms, 3)`. Notice there is no difference in syntax when fitting the two covariance types.  Two additional options are available during the fit routine which may be necessary under certain situations:
+
+	- cluster_ids   (optional) - (n_train_frames) integer array of initial cluster ids.  This option is necessary if init_cluster_method = 'read'
+	- frame_weights (optional) - (n_train_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
 
-`kronecker_aligned_trajectory = wsgmm.fit(training_set_positions)`
+If these options are used the fit call looks like
+
+`uniform_aligned_trajectory = usgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
 
 ### Predict:
 
+Once the shapeGMM object has been fit, it can be used to precict cluster IDs, aligned trajectory, and log likelihood per frame for a new, or cross validation, trajectory.  The number of atoms must remain the same.  The simple syntax is as follows:
+
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions)`
+
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions)`
+
+where `predict_positions` is an array of dimensions `(n_predict_frames, n_atoms, 3)`. Notice there is no difference in syntax when precicting the two covariance types.  If the predict frames have a non-unifrom frame weight, this can be accounted for  
+
+	- frame_weights (optional) - (n_predict_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
+
+If this option is used the predict call will look like
 
-`clusters, aligned_traj, log_likelihood = usgmm.predict(full_trajectory_positions)`
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
 
-`clusters, aligned_traj, log_likelihood = wsgmm.predict(full_trajectory_positions)`
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
 
 ## Attributes
 
 After being properly fit, a shapeGMM object will have the following attributes:
 
-	- n_clusters		- integer of how many clusters were used in training
-	- n_atoms           	- integer of how many atoms were in the training data
-	- clusters              - integer array of cluster ids for training data
-	- log_likelihood        - float log likelihood of training set
-	- weights               - (n_clusters) float array of cluster weights
-	- centers	      	- (n_clusters, n_atoms, 3) float array of cluster centers/averages
+	- n_clusters	    - integer of how many clusters were used in training
+	- n_atoms           - integer of how many atoms were in the training data
+	- n_train_frames    - integer of how many frames were in the training data
+	- clusters_ids      - integer array of cluster ids for training data
+	- log_likelihood    - float log likelihood of training set
+	- weights           - (n_clusters) float array of cluster weights
+	- centers	        - (n_clusters, n_atoms, 3) float array of cluster centers/averages
 
 Uniform covariance specific attributes
 
 	- vars		       	- (n_clusters) float array of cluster variances
 
 Kronecker covariance specific attributes
```

### Comparing `shapeGMMTorch-1.0.0/setup.py` & `shapeGMMTorch-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='shapeGMMTorch',
-    version='1.0.0',
+    version='1.5.0',
     author='Martin McCullagh',
     author_email='martin.mccullagh@okstate.edu',
     description='Gaussian Mixture Model clustering in size-and-shape space using PyTorch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mccullaghlab/shapeGMMTorch',
     project_urls = {
```

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch/scripts.py` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch/scripts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import numpy as np
 import time
 import sys
 import torch
+#import torch_sgmm
 from . import torch_sgmm
 
-def cross_validate_cluster_scan(traj_data, n_train_frames, covar_type="kronecker", cluster_array = np.arange(2,9,1).astype(int), n_training_sets=10, n_attempts = 5, dtype=torch.float32, device=torch.device("cuda:0")):
+def cross_validate_cluster_scan(traj_data, n_train_frames, frame_weights = [], covar_type="kronecker", cluster_array = np.arange(2,9,1).astype(int), n_training_sets=10, n_attempts = 5, dtype=torch.float32, device=torch.device("cuda:0")):
     """
-    perform cross validation weighted shape-GMM for range of cluster sizes
+    perform cross validation weighted shape-GMM for range of cluster sizes. Return train and CV log likelihoods as a function of number of clusters for each training set.
     Inputs:
         traj_data                    (required)  : float64 array with dimensions (n_frames, n_atoms,3) of molecular configurations
         n_train_frames               (required)  : int     scalar dictating number of frames to use as training (rest is used for CV)
+        frame_weights               (default []) : float   array defining frame weights.  Default is empty/uniform
         covar_type         (default "kronecker") : string defining the covariance type.  Options are 'kronecker' and 'uniform'.  Defualt is 'uniform'.
         cluster_array         (default: [2..8])  : int     array of cluster sizes - can be of any number but must be ints. Default is [2, 3, 4, 5, 6, 7, 8]
         n_training_sets           (default: 10)  : int     scalar dictating how many training sets to choose. Default is 10
         n_attempts                 (default: 5)  : int     scalar dictating how many attempts to perform shape-GMM on same set.  Default is 5
         dtype          (default: torch.float32)  : torch data type for trajectory and centers
         device (default: torch.device("cuda:0")  : torch data type for trajectory and centers
     Returns:
@@ -33,38 +35,89 @@
     # open data files
     weighted_train_log_lik = np.empty((cluster_array.size,n_training_sets),dtype=np.float64)
     weighted_predict_log_lik = np.empty((cluster_array.size,n_training_sets),dtype=np.float64)
     # print log info
     print("%15s %15s %15s %19s %15s" % ("Training Set", "N Clusters", "Attempt", "Log Like per Frame","CPU Time (s)"))
     print("%84s" % ("------------------------------------------------------------------------------------"))
     # loop over training sets
+    index_array = np.arange(n_frames).astype(int)
     for training_set in range(n_training_sets):
         # shuffle trajectory data
-        np.random.shuffle(traj_data)
+        np.random.shuffle(index_array)
         # create training and predict data
-        train_data = traj_data[:n_train_frames]
-        predict_data = traj_data[n_train_frames:]
+        train_data = traj_data[index_array[:n_train_frames]]
+        predict_data = traj_data[index_array[n_train_frames:]]
+        if len(frame_weights) == 0:
+            train_frame_weights = []
+            predict_frame_weights = []
+        else:
+            train_frame_weights = frame_weights[index_array[:n_train_frames]]
+            predict_frame_weights = frame_weights[index_array[n_train_frames:]]
         # loop over all number of clusters
         for cluster_index, cluster_size in enumerate(cluster_array):
             w_log_lik = []
             w_objs = []
             # for each n_clusters and training set, perform shape-GMM n_attempts times and take object with largest log likelihood
-            for attempt in range(n_attempts):
+            # if cluster size is 1 there is no need to do multiple attempts
+            if cluster_size == 1:
+                current_attempts = 1
+            else:
+                current_attempts = n_attempts
+            for attempt in range(current_attempts):
                 start_time = time.process_time()
                 wsgmm = torch_sgmm.ShapeGMMTorch(cluster_size, covar_type=covar_type, dtype=dtype, device=device)
-                wsgmm.fit(train_data)
+                wsgmm.fit(train_data, frame_weights=train_frame_weights)
                 w_log_lik.append(wsgmm.log_likelihood)
                 w_objs.append(wsgmm)
                 elapsed_time = time.process_time()-start_time
                 print("%15d %15d %15d %19.3f %15.3f" % (training_set+1, cluster_size, attempt+1, np.round(wsgmm.log_likelihood,3), np.round(elapsed_time,3)))
                 sys.stdout.flush()
             # determine maximum
             w_arg = np.argmax(w_log_lik)
             # save training log likes
             weighted_train_log_lik[cluster_index,training_set] = w_log_lik[w_arg]
             # save prediction log likes
-            weighted_predict_log_lik[cluster_index,training_set] = w_objs[w_arg].predict(predict_data)[2]
+            weighted_predict_log_lik[cluster_index,training_set] = w_objs[w_arg].predict(predict_data,predict_frame_weights)[2]
 
     #return
     return weighted_train_log_lik, weighted_predict_log_lik
 
+def sgmm_fit_with_attempts(train_data, n_clusters, n_attempts, frame_weights = [], covar_type='kronecker', dtype=torch.float32, device=torch.device("cuda:0")):
+    """
+    Initialize and fit shapeGMM object with training data but do so a number of times and return the max log likelihood object
+
+    Arguments:
+        train_data (required)   - (n_train_frames,n_atoms,3) float array containing training data
+        n_clusters (required)   - integer number of clusters must be input
+        n_attempts (required)   - integer dictating the number of random intializations to attempt
+        frame_weights (optional)- (n_train_frames) float array containing relative frame weights.  Defaults to empty (uniform weights)
+        covar_type              - string defining the covariance type.  Options are 'kronecker' and 'uniform'.  Defualt is 'kronecker'.
+        dtype                   - Data type to be used.  Default is torch.float32.
+        device                  - device to be used.  Default is torch.device('cuda:0') device.
+
+    Returns:
+        shapeGMM object with max log likelhood from attempts
+    """
+    # meta data from input array
+    n_frames = train_data.shape[0]
+    # set parameters
+    print("Number of training frames:", n_frames)
+    print("Number of clusters:", n_clusters)
+    print("Number of attempts:", n_attempts)
+    sys.stdout.flush()
+    objs = []
+    log_likes = []
+    # print log info
+    print("%8s %19s %15s" % ("Attempt", "Log Like per Frame","CPU Time (s)"))
+    print("%50s" % ("--------------------------------------------------"))
+    #
+    for i in range(n_attempts):
+        start_time = time.process_time()
+        wsgmm = torch_sgmm.ShapeGMMTorch(n_clusters,covar_type=covar_type, dtype=dtype, device=device)
+        wsgmm.fit(train_data, frame_weights = frame_weights)
+        elapsed_time = time.process_time()-start_time
+        print("%8d %19.3f %15.3f" % (i+1, np.round(wsgmm.log_likelihood,3), np.round(elapsed_time,3)))
+        objs.append(wsgmm)
+        log_likes.append(wsgmm.log_likelihood)
+    # return obj with max log likelihood per frame
+    return objs[np.argmax(log_likes)]
```

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_align.py` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_align.py`

 * *Files identical despite different names*

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_kronecker_sgmm_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 import warnings
 warnings.filterwarnings('ignore')
 import random
+#import torch_align
 from . import torch_align
 import torch
 
 GAMMA_THRESH = 1e-15
 
 ##
 def kronecker_sgmm_log_likelihood(traj_tensor, clusters, thresh=1e-3, dtype=torch.float32, device=torch.device("cuda:0")):
     # meta data from inputs
     n_frames = traj_tensor.shape[0]
-    n_clusters = np.amax(clusters) + 1
+    n_clusters = np.unique(clusters).shape[0] 
     n_atoms = traj_tensor.shape[1]
     n_dim = traj_tensor.shape[2]
     n_features = n_atoms*n_dim
     # declare arrays 
     cluster_frame_ln_likelihoods = torch.empty((n_frames, n_clusters),dtype=torch.float64, device=device)
     # compute likelihood of each frame at each Gaussian
     for k in range(n_clusters):
@@ -47,15 +48,15 @@
     del precision_tensor
     del lpdet_tensor
     torch.cuda.empty_cache()
     return log_likelihood.cpu().numpy()
 
 
 ## Expectation Maximization for GMM with Kronecker covariance model
-def torch_sgmm_kronecker_em(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, dtype=torch.float32, device=torch.device("cuda:0"), thresh=1e-1):
+def torch_sgmm_kronecker_em(traj_tensor, frame_weights_tensor, centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, dtype=torch.float32, device=torch.device("cuda:0"), thresh=1e-1):
     
     # get metadata from trajectory data
     n_frames = traj_tensor.shape[0]
     n_atoms = traj_tensor.shape[1]
     n_dim = traj_tensor.shape[2]
     n_clusters = ln_weights_tensor.shape[0]
 
@@ -64,21 +65,23 @@
     # Expectation step:
     cluster_frame_ln_likelihoods_tensor = torch_sgmm_expectation_kronecker(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, dtype=dtype, device=device)
     
     # compute log likelihood and gamma normalization
     for k in range(n_clusters):
         cluster_frame_ln_likelihoods_tensor[:,k] += ln_weights_tensor[k]
     log_norm = torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)
-    log_likelihood = torch.mean(log_norm)
+    log_likelihood = torch.sum(frame_weights_tensor*log_norm,0)
     # determine gamma values
     # use the current values for the parameters to evaluate the posterior
     # probabilities of the data to have been generanted by each gaussian
     gamma_tensor = torch.exp(cluster_frame_ln_likelihoods_tensor - log_norm.view(-1,1))
+    # multiply gamma by frame weights
+    gamma_tensor *= frame_weights_tensor.view(-1,1)
     # update the weights
-    ln_weights_tensor = torch.log(torch.mean(gamma_tensor,0))
+    ln_weights_tensor = torch.log(torch.sum(gamma_tensor,0))
     # update averages and variances of each cluster
     for k in range(n_clusters):
         gamma_indeces = torch.argwhere(gamma_tensor[:,k] > gamma_thresh_tensor).flatten()
         if gamma_indeces.shape[0] > n_atoms:
             # update mean and variance
             centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[gamma_indeces], gamma_tensor[gamma_indeces,k].to(dtype), ref_tensor=centers_tensor[k], ref_precision_tensor=precisions_tensor[k], dtype=dtype, thresh=thresh, device=device)[1:]
     return centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, log_likelihood
```

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_sgmm.py` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_sgmm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 import torch
 import warnings
 warnings.filterwarnings('ignore')
 import random
 # the following are local libraries
+#import torch_align
+#import torch_uniform_sgmm_lib
+#import torch_kronecker_sgmm_lib
 from . import torch_align
-from . import torch_uniform_sgmm_lib
-from . import torch_kronecker_sgmm_lib
+from . import torch_uniform_sgmm_lib                            
+from . import torch_kronecker_sgmm_lib  
 
 # class
 class ShapeGMMTorch:
     """
     ShapeGMMTorch is a class that can be used to perform Gaussian Mixture Model clustering in size-and-shape space.
     The class is designed to mimic similar clustering methods implemented in sklearn.  The model is first initialized
     and then fit with supplied data.  Fit parameters for the model include average structures and (co)variances.
@@ -44,28 +47,41 @@
         self.dtype = dtype                                      # torch dtype
         self.device = device                                    # torch device
         self.verbose = verbose                                  # boolean
         self._init_clusters_flag = False                        # boolean tracking if clusters have been initialized or not.
         self._gmm_fit_flag = False                              # boolean tracking if GMM has been fit.
 
     # fit the model
-    def fit(self, traj_data, clusters = []):
+    def fit(self, traj_data, cluster_ids = [], frame_weights = []):
         """
         Fit size-and-shape GMM using traj_data as the training data.
-        traj_data (required)   - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
-        clusters               - (n_frames) integer numpy array of initial cluster assignments.  
+        traj_data     (required) - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
+        cluster_ids   (optional) - (n_frames) integer numpy array of initial cluster assignments.  
+        frame_weights (optional) - (n_frames) float numpy array of frame weights
 
         Returns an aligned trajectory, if requested.  Each cluster aligned to respective average.
         """
 
         # pass trajectory data to device
         traj_tensor = torch.tensor(traj_data,dtype=self.dtype,device=self.device)
         # Initialize clusters if they have not been already
         if (self._init_clusters_flag == False):
-            self._init_clusters(traj_tensor, clusters)
+            self._init_clusters(traj_tensor, cluster_ids)
+        # frame weights
+        if len(frame_weights) == 0:
+            if (self.verbose==True):
+                print("Setting uniform frame weights")
+            self.frame_weights = np.ones(self.n_train_frames,dtype=np.float64)/self.n_train_frames
+        else:
+            if (self.verbose==True):
+                print("Using user provided frame weights")
+            # use provided frame weights but make sure they are normalized
+            self.frame_weights = frame_weights/np.sum(frame_weights)   
+        # pass the frame weights to the device (enforce double precision for accuracy)
+        frame_weights_tensor = torch.tensor(self.frame_weights,dtype=torch.float64,device=self.device)
             
         # declare some important arrays for the model
         centers_tensor = torch.empty((self.n_clusters,self.n_atoms,self.n_dim),dtype=self.dtype,device=self.device)
         self.weights = np.empty(self.n_clusters,dtype=np.float64)
         # uniform/weighted specific variables
         if self.covar_type == 'uniform': 
             vars_tensor = torch.empty(self.n_clusters,dtype=torch.float64,device=self.device)
@@ -73,36 +89,36 @@
             # declare precision matrices (inverse covariances)
             precisions_tensor = torch.empty((self.n_clusters,self.n_atoms,self.n_atoms),dtype=torch.float64,device=self.device)
             # declare array for log determinants for each clusters
             lpdets_tensor = torch.empty(self.n_clusters, dtype=torch.float64,device=self.device)
 
         # compute average and covariance of initial clustering
         for k in range(self.n_clusters):
-            indeces = np.argwhere(self.clusters == k).flatten()
+            indeces = np.argwhere(self.cluster_ids == k).flatten()
             # initialize weights as populations of clusters
-            self.weights[k] = indeces.size/self.n_frames
+            self.weights[k] = indeces.size/self.n_train_frames
             if self.covar_type == 'uniform':
-                centers_tensor[k], vars_tensor[k] = torch_align.torch_iterative_align_uniform(traj_tensor[indeces],thresh=self.kabsch_thresh,device=self.device,dtype=self.dtype)[1:]
+                centers_tensor[k], vars_tensor[k] = torch_align.torch_iterative_align_uniform_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,device=self.device,dtype=self.dtype)[1:]
             else:
-                centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker(traj_tensor[indeces],thresh=self.kabsch_thresh,device=self.device,dtype=self.dtype)[1:]        
+                centers_tensor[k], precisions_tensor[k], lpdets_tensor[k] = torch_align.torch_iterative_align_kronecker_weighted(traj_tensor[indeces],frame_weights_tensor[indeces],thresh=self.kabsch_thresh,device=self.device,dtype=self.dtype)[1:]        
         if (self.verbose == True):
             print("Weights from initial clusters in fit:", self.weights)
     
         # pass remaining data to device
         ln_weights_tensor = torch.tensor(np.log(self.weights),dtype=torch.float64,device=self.device)
         
         # perform Expectation Maximization
         delta_log_lik = 100.0 + self.log_thresh
         step = 0
         while step < self.max_steps and delta_log_lik > self.log_thresh:
             # Expectation maximization
             if self.covar_type == 'uniform':
-                centers_tensor, vars_tensor, ln_weights_tensor, log_likelihood = torch_uniform_sgmm_lib.torch_sgmm_uniform_em(traj_tensor, centers_tensor, vars_tensor, ln_weights_tensor, thresh=self.kabsch_thresh, dtype=self.dtype, device=self.device)
+                centers_tensor, vars_tensor, ln_weights_tensor, log_likelihood = torch_uniform_sgmm_lib.torch_sgmm_uniform_em(traj_tensor, frame_weights_tensor, centers_tensor, vars_tensor, ln_weights_tensor, thresh=self.kabsch_thresh, dtype=self.dtype, device=self.device)
             else:
-                centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, log_likelihood = torch_kronecker_sgmm_lib.torch_sgmm_kronecker_em(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, thresh=self.kabsch_thresh, dtype=self.dtype, device=self.device)
+                centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, log_likelihood = torch_kronecker_sgmm_lib.torch_sgmm_kronecker_em(traj_tensor, frame_weights_tensor, centers_tensor, precisions_tensor, lpdets_tensor, ln_weights_tensor, thresh=self.kabsch_thresh, dtype=self.dtype, device=self.device)
             if (self.verbose == True):
                 print(step+1, np.round(torch.exp(ln_weights_tensor).cpu().numpy(),3), np.round(log_likelihood.cpu().numpy(),3))
             # compute convergence criteria
             if step>0:
                 delta_log_lik = torch.abs(old_log_likelihood - log_likelihood)
             old_log_likelihood = log_likelihood
             step += 1
@@ -112,76 +128,93 @@
         # pass data back to cpu and delete from gpu
         self.weights = torch.exp(ln_weights_tensor).cpu().numpy()
         self.log_likelihood = log_likelihood.cpu().numpy()
         # uniform/weighted specific variables
         if self.covar_type == 'uniform': 
             cluster_frame_ln_likelihoods_tensor =  torch_uniform_sgmm_lib.torch_sgmm_expectation_uniform(traj_tensor, centers_tensor, vars_tensor, device=self.device)
             # assign clusters based on largest likelihood 
-            self.clusters = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
+            self.cluster_ids = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
             traj_data, self.centers = self._align_clusters_uniform(traj_tensor,centers_tensor)
             self.vars = vars_tensor.cpu().numpy()
             del vars_tensor
         else: # assume Kronecker product covariance
             cluster_frame_ln_likelihoods_tensor =  torch_kronecker_sgmm_lib.torch_sgmm_expectation_kronecker(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, dtype=self.dtype, device=self.device)
             # assign clusters based on largest likelihood 
-            self.clusters = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
+            self.cluster_ids = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
             traj_data, self.centers = self._align_clusters_kronecker(traj_tensor,centers_tensor, precisions_tensor)
             self.precisions = precisions_tensor.cpu().numpy()
             self.lpdets = lpdets_tensor.cpu().numpy()
             del precisions_tensor
             del lpdets_tensor
+        self.train_frame_log_likelihood = (frame_weights_tensor*torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)).cpu().numpy()
         del traj_tensor
         del ln_weights_tensor
         del cluster_frame_ln_likelihoods_tensor
         del centers_tensor
         torch.cuda.empty_cache()
         
         # sort object
         if self.sort == True:
             self._sort_object()
         # return aligned trajectory
         return traj_data
 
     # predict clustering of provided data based on prefit parameters from fit_weighted
-    def predict(self,traj_data):
+    def predict(self,traj_data, frame_weights = []):
         """
         Predict size-and-shape GMM using traj_data as prediction set and already fit object parameters.
-        traj_data (required)   - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
+        traj_data (required)     - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
+        frame_weights (optional) - (n_frames) float numpy array of frame weights
 
         Returns:
         cluster ids             - (n_frames) int array
         aligned trajectory      - (n_frames, n_atoms, 3) float32 or float64 numpy array of particle positions. 
         log likelihood          - float64 scalar of the log likelihood of the data given the fit model
         """
 
         if self._gmm_fit_flag == True:
+            # metadata
+            n_predict_frames = traj_data.shape[0]
             # send data to device
             traj_tensor = torch.tensor(traj_data,dtype=self.dtype,device=self.device)
             centers_tensor = torch.tensor(self.centers,dtype=self.dtype,device=self.device)
             ln_weights_tensor = torch.tensor(np.log(self.weights),dtype=torch.float64,device=self.device)
-            # uniform/weighted specific variables
+            # uniform/kronecker covariance specific variables
             if self.covar_type == 'uniform': 
                 vars_tensor = torch.tensor(self.vars,dtype=torch.float64,device=self.device)
             else: # assume weighted
                 # declare precision matrices (inverse covariances)
                 precisions_tensor = torch.tensor(self.precisions,dtype=torch.float64,device=self.device)
                 # declare array for log determinants for each clusters
                 lpdets_tensor = torch.tensor(self.lpdets, dtype=torch.float64,device=self.device)
+            # frame weights
+            if len(frame_weights) == 0:
+                if (self.verbose==True):
+                    print("Assuming uniform frame weights")
+                frame_weights = np.ones(n_predict_frames,dtype=np.float64)/n_predict_frames
+            else:
+                if (self.verbose==True):
+                    print("Using user provided frame weights")
+                # use provided frame weights but make sure they are normalized
+                frame_weights = frame_weights.astype(np.float64)
+                frame_weights /= np.sum(frame_weights)   
+            # pass the frame weights to the device (enforce double precision for accuracy)
+            frame_weights_tensor = torch.tensor(frame_weights,dtype=torch.float64,device=self.device)
             
             # make sure trajectory is centered
             torch_align.torch_remove_center_of_geometry(traj_tensor,dtype=self.dtype,device=self.device)
             # Expectation step
             if self.covar_type == 'uniform': 
                 cluster_frame_ln_likelihoods_tensor =  torch_uniform_sgmm_lib.torch_sgmm_expectation_uniform(traj_tensor, centers_tensor, vars_tensor, device=self.device)
             else: # assume weighted
                 cluster_frame_ln_likelihoods_tensor = torch_kronecker_sgmm_lib.torch_sgmm_expectation_kronecker(traj_tensor, centers_tensor, precisions_tensor, lpdets_tensor, dtype=self.dtype, device=self.device)
             for k in range(self.n_clusters):
                 cluster_frame_ln_likelihoods_tensor[:,k] += ln_weights_tensor[k]
-            log_norm = torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)
-            log_likelihood = torch.mean(log_norm).cpu().numpy()
+            self.predict_frame_log_likelihood = (frame_weights_tensor*torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)).cpu().numpy()
+            log_likelihood = np.sum(self.predict_frame_log_likelihood)
             # assign clusters based on largest likelihood (probability density)
             clusters = torch.argmax(cluster_frame_ln_likelihoods_tensor, dim = 1).cpu().numpy()
             # align each cluster to its average
             for k in range(self.n_clusters):
                 indeces = np.argwhere(clusters == k).flatten()
                 if self.covar_type == 'uniform':
                     traj_tensor[indeces] = torch_align.torch_align_uniform(traj_tensor[indeces], centers_tensor[k])
@@ -201,89 +234,89 @@
             torch.cuda.empty_cache()
             # return values
             return clusters, traj_data, log_likelihood
         else:
             print("shapeGMM must be fit before it can predict.")
 
     # initialize clusters
-    def _init_clusters(self, traj_tensor, clusters=[]):
+    def _init_clusters(self, traj_tensor, cluster_ids=[]):
         
         # get metadata
-        self.n_frames = int(traj_tensor.shape[0])
+        self.n_train_frames = int(traj_tensor.shape[0])
         self.n_atoms = traj_tensor.shape[1]
         self.n_dim = traj_tensor.shape[2]
         self.n_features = self.n_dim*self.n_atoms
         if (self.verbose == True):
             # print metadata to stdout
-            print("Number of frames being analyzed:", self.n_frames)
+            print("Number of frames being analyzed:", self.n_train_frames)
             print("Number of particles being analyzed:", self.n_atoms)
             print("Number of dimensions (must be 3):", self.n_dim)
             print("Initializing clustering using method:", self.init_cluster_method)
         # declare clusters
-        self.clusters = np.zeros(self.n_frames,dtype=np.int)
+        self.cluster_ids = np.zeros(self.n_train_frames,dtype=np.int32)
 
         # Remove the center-of-geometry from entire trajectory
         torch_align.torch_remove_center_of_geometry(traj_tensor)
 
         # make initial clustering based on input user choice (default is random)
         if (self.init_cluster_method == "chunk"):
-            for i in range(self.n_frames):
-                self.clusters[i] = i*self.n_clusters // self.n_frames
+            for i in range(self.n_train_frames):
+                self.cluster_ids[i] = i*self.n_clusters // self.n_train_frames
         elif (self.init_cluster_method == "read"):
-            # should affirm that there are n_frames clusters
-            self.clusters = clusters
+            # should affirm that there are n_train_frames clusters
+            self.cluster_ids = cluster_ids
         else: # default is random
-            self.clusters = torch_uniform_sgmm_lib.init_random(traj_tensor,self.n_clusters,dtype=self.dtype, device=self.device)
-            #log_lik = torch_uniform_sgmm_lib.uniform_sgmm_log_likelihood(traj_tensor,self.clusters,device=self.device).cpu().numpy()
+            self.cluster_ids = torch_uniform_sgmm_lib.init_random(traj_tensor,self.n_clusters,dtype=self.dtype, device=self.device)
+            #log_lik = torch_uniform_sgmm_lib.uniform_sgmm_log_likelihood(traj_tensor,self.cluster_ids,device=self.device).cpu().numpy()
         # clusters have been initialized
         self._init_clusters_flag = True
 
     # align the trajectory and averages
     def _align_clusters_uniform(self, traj_tensor, centers_tensor):
         if self._gmm_fit_flag == True:
             # determine a global average 
             global_center_tensor, global_var_tensor = torch_align.torch_iterative_align_uniform(traj_tensor, dtype=self.dtype, device=self.device)[1:]
             # align centers to global average
             centers_tensor = torch_align.torch_align_uniform(centers_tensor, global_center_tensor)
             # align each cluster to its average
             for k in range(self.n_clusters):
-                indeces = np.argwhere(self.clusters == k).flatten()
+                indeces = np.argwhere(self.cluster_ids == k).flatten()
                 traj_tensor[indeces] = torch_align.torch_align_uniform(traj_tensor[indeces], centers_tensor[k])
             return traj_tensor.cpu().numpy(), centers_tensor.cpu().numpy()
         else:
             print("shapeGMM must be fit before it can be aligned.")
 
     def _align_clusters_kronecker(self, traj_tensor, centers_tensor, precisions_tensor):
         if self._gmm_fit_flag == True:
             # determine a global average 
             global_center_tensor, global_precision_tensor = torch_align.torch_iterative_align_kronecker(traj_tensor, dtype=self.dtype, device=self.device)[1:3]
             # align centers to global average (NxN covars/precisions are rotationally invariant so don't need to rotate them)
             centers_tensor = torch_align.torch_align_kronecker(centers_tensor, global_center_tensor, global_precision_tensor, dtype=self.dtype, device=self.device)
             # align each cluster to its average
             for k in range(self.n_clusters):
-                indeces = np.argwhere(self.clusters == k).flatten()
+                indeces = np.argwhere(self.cluster_ids == k).flatten()
                 traj_tensor[indeces] = torch_align.torch_align_kronecker(traj_tensor[indeces], centers_tensor[k], precisions_tensor[k], dtype=self.dtype, device=self.device)
             return traj_tensor.cpu().numpy(), centers_tensor.cpu().numpy()
         else:
             print("shapeGMM must be fit before it can be aligned.")
 
     # sort the object based on cluster weights
     def _sort_object(self):
         if self._gmm_fit_flag == True:
             # determine sort key
             sort_key = np.argsort(self.weights)[::-1]
             cluster_ids = np.arange(self.n_clusters).astype(int)
             sorted_cluster_ids = cluster_ids[sort_key]
-            new_clusters = np.empty(self.n_frames,dtype=int)
-            for frame in range(self.n_frames):
-                new_clusters[frame] = np.argwhere(sorted_cluster_ids == self.clusters[frame])
+            new_clusters = np.empty(self.n_train_frames,dtype=int)
+            for frame in range(self.n_train_frames):
+                new_clusters[frame] = np.argwhere(sorted_cluster_ids == self.cluster_ids[frame])
             # repopulate object
             self.centers    = self.centers[sort_key]
             self.weights    = self.weights[sort_key]
-            self.clusters   = new_clusters
+            self.cluster_ids   = new_clusters
             if self.covar_type == "uniform":
                 self.vars = self.vars[sort_key]
             else:
                 self.precisions = self.precisions[sort_key]
                 self.lpdets     = self.lpdets[sort_key]
         else:
             print("shapeGMM must be fit before it can be sorted.")
```

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch/torch_uniform_sgmm_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import warnings
 warnings.filterwarnings('ignore')
 import random
-from . import torch_align
 #import torch_align
+from . import torch_align
 import torch
 
 GAMMA_THRESH = 1e-15
 
 ##
 
 def uniform_sgmm_log_likelihood(traj_tensor, clusters, thresh=1e-3, dtype=torch.float32, device=torch.device("cuda:0")):
@@ -65,15 +65,15 @@
             if indeces.size < n_atoms:
                 clustersPass = False
                 break
     return clusters
 
 
 ## Expectation Maximization for GMM with uniform covariance model
-def torch_sgmm_uniform_em(traj_tensor, centers_tensor, vars_tensor, ln_weights_tensor, dtype=torch.float32, device=torch.device("cuda:0"), thresh=1e-3):
+def torch_sgmm_uniform_em(traj_tensor, frame_weights_tensor, centers_tensor, vars_tensor, ln_weights_tensor, dtype=torch.float32, device=torch.device("cuda:0"), thresh=1e-3):
     
     # get metadata from trajectory data
     n_frames = traj_tensor.shape[0]
     n_atoms = traj_tensor.shape[1]
     n_dim = traj_tensor.shape[2]
     n_clusters = ln_weights_tensor.shape[0]
     gamma_thresh_tensor = torch.tensor(GAMMA_THRESH,dtype=torch.float64,device=device)
@@ -81,21 +81,23 @@
     # Expectation step:
     cluster_frame_ln_likelihoods_tensor = torch_sgmm_expectation_uniform(traj_tensor, centers_tensor, vars_tensor, device=device)
     
     # compute log likelihood and gamma normalization
     for k in range(n_clusters):
         cluster_frame_ln_likelihoods_tensor[:,k] += ln_weights_tensor[k]
     log_norm = torch.logsumexp(cluster_frame_ln_likelihoods_tensor,1)
-    log_likelihood = torch.mean(log_norm)
+    log_likelihood = torch.sum(frame_weights_tensor*log_norm,0)
     # determine gamma values
     # use the current values for the parameters to evaluate the posterior
     # probabilities of the data to have been generanted by each gaussian
     gamma_tensor = torch.exp(cluster_frame_ln_likelihoods_tensor - log_norm.view(-1,1))
+    # multiply gamma by frame weights
+    gamma_tensor *= frame_weights_tensor.view(-1,1)
     # update the weights
-    ln_weights_tensor = torch.log(torch.mean(gamma_tensor,0))
+    ln_weights_tensor = torch.log(torch.sum(gamma_tensor,0))
     # update averages and variances of each cluster
     for k in range(n_clusters):
         gamma_indeces = torch.argwhere(gamma_tensor[:,k] > gamma_thresh_tensor).flatten()
         # update mean and variance
         centers_tensor[k], vars_tensor[k] = torch_align.torch_iterative_align_uniform_weighted(traj_tensor[gamma_indeces], gamma_tensor[gamma_indeces,k].to(dtype), ref_tensor=centers_tensor[k], dtype=dtype, thresh=thresh, device=device)[1:]
     return centers_tensor, vars_tensor, ln_weights_tensor, log_likelihood    
     del gamma_tensor
```

### Comparing `shapeGMMTorch-1.0.0/src/shapeGMMTorch.egg-info/PKG-INFO` & `shapeGMMTorch-1.5.0/src/shapeGMMTorch.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: shapeGMMTorch
-Version: 1.0.0
+Version: 1.5.0
 Summary: Gaussian Mixture Model clustering in size-and-shape space using PyTorch
 Home-page: https://github.com/mccullaghlab/shapeGMMTorch
 Author: Martin McCullagh
 Author-email: martin.mccullagh@okstate.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mccullaghlab/shapeGMMTorch/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,27 +44,33 @@
 
 `pip install shapeGMMTorch`
 
 or by downloading from github and then running
 
 `python setup.py install`
 
+### Installation on a MAC
+
+I have found that PyTorch does not work on a mac using standard `pip install torch` or conda.  Instead, you have to create a special `nomkl` conda environment and install all necessary packages in there.  There are various blogs and/or stack overflow threads on this.
+
+After the `nomkl` conda environment has been created and all dependencies have been added to that environment, shapeGMMTorch can be installed.  Only the `torch.device("cpu")` device will work on a mac, however.
+
 ## Usage 
 
 This package is designed to mimic the usage of the sklearn package.  You first initiliaze the object and then fit.  Predict can be done once the model is fit.  Fit and ppredict functions take particle position trajectories as input in the form of a `(n_frames, n_atoms, 3)` numpy array.
 
 ### Initialize:
 
 `from shapeGMMTorch import torch_sgmm`
 
-Uniform (spherical, uncorrelated) covariance:
+Uniform covariance (spherical, uncorrelated, homogeneous):
 
 `usgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'uniform', verbose=True)`
 
-Weighted (Kronecker product) covariance:
+Kronecker product covariance (formerly call weighted covariance; spherical, correlated, heterogeneous):
 
 `wsgmm = torch_sgmm.ShapeGMMTorch(n_clusters, covar_type = 'kronecker', verbose=True)`
 
 During initialization, the following options are availble:
 
 	- n_clusters (required)   - integer number of clusters must be input
 	- covar_type              - string defining the covariance type.  Options are 'kronecker' and 'uniform'.  Defualt is 'uniform'.
@@ -76,41 +81,64 @@
 	- kabsch_thresh           - float dictating convergence criteria for each iterative alignment (Maximization step).  Default value is 1e-1.
 	- dtype                   - Torch data type to be used.  Default is torch.float32.
 	- device                  - Torch device to be used.  Default is torch.device('cuda:0') device.
 	- verbose                 - boolean dictating whether to print various things at every step. Defualt is False.
 
 ### Fit:
 
-`uniform_aligned_trajectory = usgmm.fit(training_set_positions)`
+A standard fit can be performed in the following manner:
+
+`uniform_aligned_trajectory = usgmm.fit(train_positions)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions)`
+
+where `train_positions` is an array of dimensions `(n_train_frames, n_atoms, 3)`. Notice there is no difference in syntax when fitting the two covariance types.  Two additional options are available during the fit routine which may be necessary under certain situations:
+
+	- cluster_ids   (optional) - (n_train_frames) integer array of initial cluster ids.  This option is necessary if init_cluster_method = 'read'
+	- frame_weights (optional) - (n_train_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
+
+If these options are used the fit call looks like
 
-`kronecker_aligned_trajectory = wsgmm.fit(training_set_positions)`
+`uniform_aligned_trajectory = usgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
+
+`kronecker_aligned_trajectory = wsgmm.fit(train_positions, cluster_ids = initial_cluster_ids, frame_weights = train_frame_weights)`
 
 ### Predict:
 
+Once the shapeGMM object has been fit, it can be used to precict cluster IDs, aligned trajectory, and log likelihood per frame for a new, or cross validation, trajectory.  The number of atoms must remain the same.  The simple syntax is as follows:
+
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions)`
+
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions)`
+
+where `predict_positions` is an array of dimensions `(n_predict_frames, n_atoms, 3)`. Notice there is no difference in syntax when precicting the two covariance types.  If the predict frames have a non-unifrom frame weight, this can be accounted for  
 
-`clusters, aligned_traj, log_likelihood = usgmm.predict(full_trajectory_positions)`
+	- frame_weights (optional) - (n_predict_frames) float array of relative frame weights.  If none are provided the code assumes equal weights for all frames.
 
-`clusters, aligned_traj, log_likelihood = wsgmm.predict(full_trajectory_positions)`
+If this option is used the predict call will look like
+
+`cluster_ids, aligned_traj, log_likelihood = usgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
+
+`clusters_ids, aligned_traj, log_likelihood = wsgmm.predict(predict_positions, frame_weights = predict_frame_weights)`
 
 ## Attributes
 
 After being properly fit, a shapeGMM object will have the following attributes:
 
-	- n_clusters		- integer of how many clusters were used in training
-	- n_atoms           	- integer of how many atoms were in the training data
-	- clusters              - integer array of cluster ids for training data
-	- log_likelihood        - float log likelihood of training set
-	- weights               - (n_clusters) float array of cluster weights
-	- centers	      	- (n_clusters, n_atoms, 3) float array of cluster centers/averages
+	- n_clusters	    - integer of how many clusters were used in training
+	- n_atoms           - integer of how many atoms were in the training data
+	- n_train_frames    - integer of how many frames were in the training data
+	- clusters_ids      - integer array of cluster ids for training data
+	- log_likelihood    - float log likelihood of training set
+	- weights           - (n_clusters) float array of cluster weights
+	- centers	        - (n_clusters, n_atoms, 3) float array of cluster centers/averages
 
 Uniform covariance specific attributes
 
 	- vars		       	- (n_clusters) float array of cluster variances
 
 Kronecker covariance specific attributes
 
 	- precisions	   	- (n_clusters, n_atoms, n_atoms) float array of cluster precisions (inverse covariances)
 	- lpdets	    	- (n_clusters) float array of ln(det(covar))
 
 
-
-
```

