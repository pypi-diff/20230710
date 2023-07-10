# Comparing `tmp/phylotreeclus-1.0.0.tar.gz` & `tmp/phylotreeclus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylotreeclus-1.0.0.tar", last modified: Fri Jul  7 12:52:41 2023, max compression
+gzip compressed data, was "phylotreeclus-1.0.1.tar", last modified: Mon Jul 10 12:54:30 2023, max compression
```

## Comparing `phylotreeclus-1.0.0.tar` & `phylotreeclus-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-07 12:52:41.785482 phylotreeclus-1.0.0/
--rw-r--r--   0 elisab    (1000) elisab    (1000)     4915 2023-07-07 12:52:41.785482 phylotreeclus-1.0.0/PKG-INFO
-drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-07 12:52:41.775482 phylotreeclus-1.0.0/PhyloTreeClustering/
--rw-r--r--   0 elisab    (1000) elisab    (1000)    31990 2023-07-05 15:06:56.000000 phylotreeclus-1.0.0/PhyloTreeClustering/PhyloTreeClustering.py
--rw-r--r--   0 elisab    (1000) elisab    (1000)        0 2023-07-04 13:33:19.000000 phylotreeclus-1.0.0/PhyloTreeClustering/__init__.py
--rw-r--r--   0 elisab    (1000) elisab    (1000)     1044 2023-07-04 13:26:02.000000 phylotreeclus-1.0.0/PhyloTreeClustering/calculate_pdm.py
--rw-r--r--   0 elisab    (1000) elisab    (1000)     2428 2023-07-06 14:58:00.000000 phylotreeclus-1.0.0/PhyloTreeClustering/calinski_harabasz.py
--rw-r--r--   0 elisab    (1000) elisab    (1000)    22688 2023-07-05 13:40:03.000000 phylotreeclus-1.0.0/PhyloTreeClustering/medicc_functions.py
--rw-r--r--   0 elisab    (1000) elisab    (1000)     4474 2023-07-07 12:48:59.000000 phylotreeclus-1.0.0/README.md
--rwxr-xr-x   0 elisab    (1000) elisab    (1000)     2547 2023-07-05 15:08:55.000000 phylotreeclus-1.0.0/phylotreeclus
-drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-07 12:52:41.785482 phylotreeclus-1.0.0/phylotreeclus.egg-info/
--rw-r--r--   0 elisab    (1000) elisab    (1000)     4915 2023-07-07 12:52:41.000000 phylotreeclus-1.0.0/phylotreeclus.egg-info/PKG-INFO
--rw-r--r--   0 elisab    (1000) elisab    (1000)      424 2023-07-07 12:52:41.000000 phylotreeclus-1.0.0/phylotreeclus.egg-info/SOURCES.txt
--rw-r--r--   0 elisab    (1000) elisab    (1000)        1 2023-07-07 12:52:41.000000 phylotreeclus-1.0.0/phylotreeclus.egg-info/dependency_links.txt
--rw-r--r--   0 elisab    (1000) elisab    (1000)       82 2023-07-07 12:52:41.000000 phylotreeclus-1.0.0/phylotreeclus.egg-info/requires.txt
--rw-r--r--   0 elisab    (1000) elisab    (1000)       20 2023-07-07 12:52:41.000000 phylotreeclus-1.0.0/phylotreeclus.egg-info/top_level.txt
--rw-r--r--   0 elisab    (1000) elisab    (1000)       84 2023-07-07 08:29:56.000000 phylotreeclus-1.0.0/pyproject.toml
--rw-r--r--   0 elisab    (1000) elisab    (1000)       38 2023-07-07 12:52:41.785482 phylotreeclus-1.0.0/setup.cfg
--rw-r--r--   0 elisab    (1000) elisab    (1000)      880 2023-07-07 12:51:56.000000 phylotreeclus-1.0.0/setup.py
+drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-10 12:54:30.216455 phylotreeclus-1.0.1/
+-rw-r--r--   0 elisab    (1000) elisab    (1000)     5197 2023-07-10 12:54:30.206455 phylotreeclus-1.0.1/PKG-INFO
+drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-10 12:54:30.206455 phylotreeclus-1.0.1/PhyloTreeClustering/
+-rw-r--r--   0 elisab    (1000) elisab    (1000)    31962 2023-07-10 12:50:22.000000 phylotreeclus-1.0.1/PhyloTreeClustering/PhyloTreeClustering.py
+-rw-r--r--   0 elisab    (1000) elisab    (1000)        0 2023-07-04 13:33:19.000000 phylotreeclus-1.0.1/PhyloTreeClustering/__init__.py
+-rw-r--r--   0 elisab    (1000) elisab    (1000)     1044 2023-07-04 13:26:02.000000 phylotreeclus-1.0.1/PhyloTreeClustering/calculate_pdm.py
+-rw-r--r--   0 elisab    (1000) elisab    (1000)     2428 2023-07-07 13:42:51.000000 phylotreeclus-1.0.1/PhyloTreeClustering/calinski_harabasz.py
+-rw-r--r--   0 elisab    (1000) elisab    (1000)    22688 2023-07-05 13:40:03.000000 phylotreeclus-1.0.1/PhyloTreeClustering/medicc_functions.py
+-rw-r--r--   0 elisab    (1000) elisab    (1000)     4756 2023-07-10 12:35:06.000000 phylotreeclus-1.0.1/README.md
+-rwxr-xr-x   0 elisab    (1000) elisab    (1000)     2581 2023-07-10 12:41:51.000000 phylotreeclus-1.0.1/phylotreeclus
+drwxr-xr-x   0 elisab    (1000) elisab    (1000)        0 2023-07-10 12:54:30.206455 phylotreeclus-1.0.1/phylotreeclus.egg-info/
+-rw-r--r--   0 elisab    (1000) elisab    (1000)     5197 2023-07-10 12:54:30.000000 phylotreeclus-1.0.1/phylotreeclus.egg-info/PKG-INFO
+-rw-r--r--   0 elisab    (1000) elisab    (1000)      424 2023-07-10 12:54:30.000000 phylotreeclus-1.0.1/phylotreeclus.egg-info/SOURCES.txt
+-rw-r--r--   0 elisab    (1000) elisab    (1000)        1 2023-07-10 12:54:30.000000 phylotreeclus-1.0.1/phylotreeclus.egg-info/dependency_links.txt
+-rw-r--r--   0 elisab    (1000) elisab    (1000)       82 2023-07-10 12:54:30.000000 phylotreeclus-1.0.1/phylotreeclus.egg-info/requires.txt
+-rw-r--r--   0 elisab    (1000) elisab    (1000)       20 2023-07-10 12:54:30.000000 phylotreeclus-1.0.1/phylotreeclus.egg-info/top_level.txt
+-rw-r--r--   0 elisab    (1000) elisab    (1000)       84 2023-07-07 08:29:56.000000 phylotreeclus-1.0.1/pyproject.toml
+-rw-r--r--   0 elisab    (1000) elisab    (1000)       38 2023-07-10 12:54:30.216455 phylotreeclus-1.0.1/setup.cfg
+-rw-r--r--   0 elisab    (1000) elisab    (1000)      880 2023-07-10 12:54:03.000000 phylotreeclus-1.0.1/setup.py
```

### Comparing `phylotreeclus-1.0.0/PKG-INFO` & `phylotreeclus-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,68 @@
-Metadata-Version: 2.1
-Name: phylotreeclus
-Version: 1.0.0
-Summary: Clustering algorithm for phylogenetic cancer evolution trees
-Home-page: https://bitbucket.org/schwarzlab/phylotreeclustering
-Author: Elisa Billard
-Author-email: elisabillard1905@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # PhyloTreeClustering 
-Clustering method for phylogenetic cancer evolution trees.
+Clustering algorithm for phylogenetic cancer evolution trees.
 
 ## Installation
 Install PhyloTreeClustering via pip or from source.
 
 ### Intallation via pip (recommended)
 It is best to use a dedicated conda environment for your PhyloTreeClustering installation with `conda create -n phylo_env`.
 After activating the environment with `conda activate phylo_env` you can install PhyloTreeCLustering via `pip install phylotreeclus`
 
 ### Installation from source
 Clone the PhyloTreeClustering repository using `git clone https://bitbucket.org/schwarzlab/phylotreeclustering`. 
 
 Then, inside the PhyloTreeClustering folder, run `pip install . `to install PhyloTreeClustering to your environment.
 
 ## Usage
-After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through import PhyloTreeClustering) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run phylotreeclus --help for information on optional arguments.
+After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through `import PhyloTreeClustering`) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run `phylotreeclus --help` for information on optional arguments.
 
 ## Command line Flags
 
--   `tree_file_path`: tree you want to cluster, in Newick format
+-   `tree_file_path`: tree you want to cluster, in Newick format.
 
--   `output_path`: path to save figures and files produced by algorithm
+-   `output_path`: path to save figures and files produced by algorithm.
 
--   `tree`: directly the tree you want to cluster
+-   `tree`: directly the tree you want to cluster.
 
 -   `dist_matrix`: panda dataframe, matrix of the distances between all leaves of the tree, index are the names of the leaves 
                 The default None means the distance matrix will be calculated by the function `calculate_pdm_from_tree`.
 
--   `threshold`: manually choose the cutting threshold (not recommended)
+-   `threshold`: manually choose the cutting threshold (not recommended).
 
--   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score
+-   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score,
+                                True by default.
 
--   `n_diff_th`: number of repetition of scoring, meaning the number of different threshold cuts will be tested.
+-   `n_diff_th`: number of different threshold that will be tested.
                 The default None means this number will be calculated according to the size of the tree in `init_n_diff_th`.
             
--   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score
-                If no matrix is given, the normal dist_matrix will be used
+-   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score,
+                if no matrix is given, the normal `dist_matrix` will be used.
         
 -   `min_size_clus`: minimum size of a cluster. 
-                If no value is given, it is calculated in init_min_size_clus according to the size of the tree
+                If no value is given, it is calculated in `init_min_size_clus` according to the size of the tree.
         
--   `multi_level_clus`: if True, make a second level of clusters.
-                The default is False, so only one level of clustering will be performed
+-   `multi_level_clus`: if True, a second level of clustering will be performed for the bigger clusters.
+                The default is False, so only one level of clustering will be performed.
         
 -   `dist_type`: distance calculation used to compute the new dendrogram distances.
-                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`
+                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`.
 
 ## Output plot
 
 PhyloTreeClustering creates the following output files:
--   summary_plot.png : dendrogram and medicc tree next to each other, with the clustering
--   sample_labels.txt : list of all the samples and the cluster they were assigned to 
--   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen
+-   summary_plot.png : dendrogram and tree next to each other, with the clustering shown with colors (outliers in black), the red dotted lines are the min and max threshold     tested, the yellow line is the chosen threshold.
+-   sample_labels.txt : list of all the samples and the cluster they were assigned to.
+-   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen.
 
 ## Usage example
 
-For first time users we recommend to have a look at the trees (Newick format) in /examples to get an idea of how input data should look like. Then run phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder as an example of a standard PhyloTreeClustering run. Finally, the notebook notebooks/simple_example.py shows how the individual functions in the workflow are used.
+For first time users we recommend to have a look at the trees (Newick format) in /examples on Bitbucket to get an idea of how input data should look like. Then run `phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder` as an example of a standard PhyloTreeClustering run. Finally, the notebook `notebooks/simple_example.py` shows how the individual functions in the workflow are used.
 
-![Clustering example](example_data/example_summary_plot_readme.png)
+![Clustering example](https://bitbucket.org/schwarzlab/phylotreeclustering/raw/master/example_data/example_summary_plot_readme.png)
 
 ## References
 
 **For the examples :**
 
 - Original data from Gao et al. 2016 
 Gao, R., Davis, A., McDonald, T. et al.
```

### Comparing `phylotreeclus-1.0.0/PhyloTreeClustering/PhyloTreeClustering.py` & `phylotreeclus-1.0.1/PhyloTreeClustering/PhyloTreeClustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import sys
 from copy import deepcopy, copy
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-#from tqdm.auto import tqdm
 
 from PhyloTreeClustering.calculate_pdm import calculate_pdm_from_tree
 from PhyloTreeClustering.calinski_harabasz import calinski_harabasz_score
 from PhyloTreeClustering.medicc_functions import plot_tree, import_tree
 
 plt.rcParams["axes.prop_cycle"] = plt.cycler("color", plt.cm.tab20.colors)
```

### Comparing `phylotreeclus-1.0.0/PhyloTreeClustering/calculate_pdm.py` & `phylotreeclus-1.0.1/PhyloTreeClustering/calculate_pdm.py`

 * *Files identical despite different names*

### Comparing `phylotreeclus-1.0.0/PhyloTreeClustering/calinski_harabasz.py` & `phylotreeclus-1.0.1/PhyloTreeClustering/calinski_harabasz.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     X, labels = check_X_y(X, labels)
     le = LabelEncoder()
     labels = le.fit_transform(labels)
 
     n_samples, _ = X.shape
     n_labels = len(le.classes_)
     matrix_mean = np.mean(np.mean(X))
-    outliers_penalty = matrix_mean**2 * 8
+    outliers_penalty = matrix_mean**2 * 9
 
     check_number_of_labels(n_labels, n_samples)
     extra_disp, intra_disp = 0.0, 0.0
     mean = np.mean(X, axis=0)
     for k in range(n_labels):
         
         cluster_k = X[labels == k]
```

### Comparing `phylotreeclus-1.0.0/PhyloTreeClustering/medicc_functions.py` & `phylotreeclus-1.0.1/PhyloTreeClustering/medicc_functions.py`

 * *Files identical despite different names*

### Comparing `phylotreeclus-1.0.0/README.md` & `phylotreeclus-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,80 @@
+Metadata-Version: 2.1
+Name: phylotreeclus
+Version: 1.0.1
+Summary: Clustering algorithm for phylogenetic cancer evolution trees
+Home-page: https://bitbucket.org/schwarzlab/phylotreeclustering
+Author: Elisa Billard
+Author-email: elisabillard1905@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # PhyloTreeClustering 
-Clustering method for phylogenetic cancer evolution trees.
+Clustering algorithm for phylogenetic cancer evolution trees.
 
 ## Installation
 Install PhyloTreeClustering via pip or from source.
 
 ### Intallation via pip (recommended)
 It is best to use a dedicated conda environment for your PhyloTreeClustering installation with `conda create -n phylo_env`.
 After activating the environment with `conda activate phylo_env` you can install PhyloTreeCLustering via `pip install phylotreeclus`
 
 ### Installation from source
 Clone the PhyloTreeClustering repository using `git clone https://bitbucket.org/schwarzlab/phylotreeclustering`. 
 
 Then, inside the PhyloTreeClustering folder, run `pip install . `to install PhyloTreeClustering to your environment.
 
 ## Usage
-After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through import PhyloTreeClustering) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run phylotreeclus --help for information on optional arguments.
+After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through `import PhyloTreeClustering`) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run `phylotreeclus --help` for information on optional arguments.
 
 ## Command line Flags
 
--   `tree_file_path`: tree you want to cluster, in Newick format
+-   `tree_file_path`: tree you want to cluster, in Newick format.
 
--   `output_path`: path to save figures and files produced by algorithm
+-   `output_path`: path to save figures and files produced by algorithm.
 
--   `tree`: directly the tree you want to cluster
+-   `tree`: directly the tree you want to cluster.
 
 -   `dist_matrix`: panda dataframe, matrix of the distances between all leaves of the tree, index are the names of the leaves 
                 The default None means the distance matrix will be calculated by the function `calculate_pdm_from_tree`.
 
--   `threshold`: manually choose the cutting threshold (not recommended)
+-   `threshold`: manually choose the cutting threshold (not recommended).
 
--   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score
+-   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score,
+                                True by default.
 
--   `n_diff_th`: number of repetition of scoring, meaning the number of different threshold cuts will be tested.
+-   `n_diff_th`: number of different threshold that will be tested.
                 The default None means this number will be calculated according to the size of the tree in `init_n_diff_th`.
             
--   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score
-                If no matrix is given, the normal dist_matrix will be used
+-   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score,
+                if no matrix is given, the normal `dist_matrix` will be used.
         
 -   `min_size_clus`: minimum size of a cluster. 
-                If no value is given, it is calculated in init_min_size_clus according to the size of the tree
+                If no value is given, it is calculated in `init_min_size_clus` according to the size of the tree.
         
--   `multi_level_clus`: if True, make a second level of clusters.
-                The default is False, so only one level of clustering will be performed
+-   `multi_level_clus`: if True, a second level of clustering will be performed for the bigger clusters.
+                The default is False, so only one level of clustering will be performed.
         
 -   `dist_type`: distance calculation used to compute the new dendrogram distances.
-                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`
+                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`.
 
 ## Output plot
 
 PhyloTreeClustering creates the following output files:
--   summary_plot.png : dendrogram and medicc tree next to each other, with the clustering
--   sample_labels.txt : list of all the samples and the cluster they were assigned to 
--   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen
+-   summary_plot.png : dendrogram and tree next to each other, with the clustering shown with colors (outliers in black), the red dotted lines are the min and max threshold     tested, the yellow line is the chosen threshold.
+-   sample_labels.txt : list of all the samples and the cluster they were assigned to.
+-   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen.
 
 ## Usage example
 
-For first time users we recommend to have a look at the trees (Newick format) in /examples to get an idea of how input data should look like. Then run phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder as an example of a standard PhyloTreeClustering run. Finally, the notebook notebooks/simple_example.py shows how the individual functions in the workflow are used.
+For first time users we recommend to have a look at the trees (Newick format) in /examples on Bitbucket to get an idea of how input data should look like. Then run `phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder` as an example of a standard PhyloTreeClustering run. Finally, the notebook `notebooks/simple_example.py` shows how the individual functions in the workflow are used.
 
-![Clustering example](example_data/example_summary_plot_readme.png)
+![Clustering example](https://bitbucket.org/schwarzlab/phylotreeclustering/raw/master/example_data/example_summary_plot_readme.png)
 
 ## References
 
 **For the examples :**
 
 - Original data from Gao et al. 2016 
 Gao, R., Davis, A., McDonald, T. et al.
```

### Comparing `phylotreeclus-1.0.0/phylotreeclus` & `phylotreeclus-1.0.1/phylotreeclus`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,25 @@
         description="Takes a phylogeny tree, transforms it in a dendrogram, and clusters the leaves on the dendrogram",
         # bottom text
         epilog="By Elisa Billard"
     )
     # positional arguments  
     parser.add_argument(
         dest= "tree_file_path",
-        help="The input file : the copy number data"
+        help="The input file : Newick tree"
     )
     parser.add_argument(
         dest= "output_path",
         help="The output path to save the figure"
     )
 
     # optional arguments
     parser.add_argument(
         "--th", dest= "threshold",
-        help="The threshold where to cut the dendrogram"
+        help="Manually choose the threshlod where you want to cut the dendrogram (not recommended)"
     )
     parser.add_argument(
         "-c", "--calinski_h", action="store_false", dest = "calinski_harabasz_score",
         help="Whether to test different threshold and choose the final one based on CH score"
     )
     parser.add_argument(
         "-n", "--n_diff_th", dest = "n_diff_th",
@@ -43,15 +43,15 @@
     parser.add_argument(
         "--dist_type", dest = "dist_type",
         help="The distance type used to calculate the dendrogram distances"
     )
     parser.add_argument(
         "-m", "--multi_level_clus", action= "store_true", # flag, meaning it is False by default
         dest = "multi_level_clus",
-        help="Whether to to a 2nd level of clustering on the big clusters"
+        help="Whether to do a 2nd level of clustering on the big clusters"
     )
     
     
     args = parser.parse_args()
 
     clus = PhyloTreeClustering(**vars(args))
     clus.run()
```

### Comparing `phylotreeclus-1.0.0/phylotreeclus.egg-info/PKG-INFO` & `phylotreeclus-1.0.1/phylotreeclus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 Metadata-Version: 2.1
 Name: phylotreeclus
-Version: 1.0.0
+Version: 1.0.1
 Summary: Clustering algorithm for phylogenetic cancer evolution trees
 Home-page: https://bitbucket.org/schwarzlab/phylotreeclustering
 Author: Elisa Billard
 Author-email: elisabillard1905@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # PhyloTreeClustering 
-Clustering method for phylogenetic cancer evolution trees.
+Clustering algorithm for phylogenetic cancer evolution trees.
 
 ## Installation
 Install PhyloTreeClustering via pip or from source.
 
 ### Intallation via pip (recommended)
 It is best to use a dedicated conda environment for your PhyloTreeClustering installation with `conda create -n phylo_env`.
 After activating the environment with `conda activate phylo_env` you can install PhyloTreeCLustering via `pip install phylotreeclus`
 
 ### Installation from source
 Clone the PhyloTreeClustering repository using `git clone https://bitbucket.org/schwarzlab/phylotreeclustering`. 
 
 Then, inside the PhyloTreeClustering folder, run `pip install . `to install PhyloTreeClustering to your environment.
 
 ## Usage
-After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through import PhyloTreeClustering) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run phylotreeclus --help for information on optional arguments.
+After installing PhyloTreeClustering, you can use PhyloTreeClustering functions in python scripts (through `import PhyloTreeClustering`) and from the command line. General usage from the command line is `phylotreeclus path/to/input/file path/to/output/folder`. Run `phylotreeclus --help` for information on optional arguments.
 
 ## Command line Flags
 
--   `tree_file_path`: tree you want to cluster, in Newick format
+-   `tree_file_path`: tree you want to cluster, in Newick format.
 
--   `output_path`: path to save figures and files produced by algorithm
+-   `output_path`: path to save figures and files produced by algorithm.
 
--   `tree`: directly the tree you want to cluster
+-   `tree`: directly the tree you want to cluster.
 
 -   `dist_matrix`: panda dataframe, matrix of the distances between all leaves of the tree, index are the names of the leaves 
                 The default None means the distance matrix will be calculated by the function `calculate_pdm_from_tree`.
 
--   `threshold`: manually choose the cutting threshold (not recommended)
+-   `threshold`: manually choose the cutting threshold (not recommended).
 
--   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score
+-   `calinski_harabasz_score`: if True, the algorithm chooses the best threshold based on the clustering with the highest score,
+                                True by default.
 
--   `n_diff_th`: number of repetition of scoring, meaning the number of different threshold cuts will be tested.
+-   `n_diff_th`: number of different threshold that will be tested.
                 The default None means this number will be calculated according to the size of the tree in `init_n_diff_th`.
             
--   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score
-                If no matrix is given, the normal dist_matrix will be used
+-   `CH_matrix`: distance matrix that will be used to evaluate the clusering with the CH score,
+                if no matrix is given, the normal `dist_matrix` will be used.
         
 -   `min_size_clus`: minimum size of a cluster. 
-                If no value is given, it is calculated in init_min_size_clus according to the size of the tree
+                If no value is given, it is calculated in `init_min_size_clus` according to the size of the tree.
         
--   `multi_level_clus`: if True, make a second level of clusters.
-                The default is False, so only one level of clustering will be performed
+-   `multi_level_clus`: if True, a second level of clustering will be performed for the bigger clusters.
+                The default is False, so only one level of clustering will be performed.
         
 -   `dist_type`: distance calculation used to compute the new dendrogram distances.
-                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`
+                The default and recommended distance is `half_max`. The others are `mean`, `median` and `max`.
 
 ## Output plot
 
 PhyloTreeClustering creates the following output files:
--   summary_plot.png : dendrogram and medicc tree next to each other, with the clustering
--   sample_labels.txt : list of all the samples and the cluster they were assigned to 
--   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen
+-   summary_plot.png : dendrogram and tree next to each other, with the clustering shown with colors (outliers in black), the red dotted lines are the min and max threshold     tested, the yellow line is the chosen threshold.
+-   sample_labels.txt : list of all the samples and the cluster they were assigned to.
+-   sample_labels_2nd_layer.txt : list of all the samples and the cluster they were assigned to if the option multi_layer_clustering is chosen.
 
 ## Usage example
 
-For first time users we recommend to have a look at the trees (Newick format) in /examples to get an idea of how input data should look like. Then run phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder as an example of a standard PhyloTreeClustering run. Finally, the notebook notebooks/simple_example.py shows how the individual functions in the workflow are used.
+For first time users we recommend to have a look at the trees (Newick format) in /examples on Bitbucket to get an idea of how input data should look like. Then run `phylotreeclus examples/Gao_2016_12_final_tree.new path/to/output/folder` as an example of a standard PhyloTreeClustering run. Finally, the notebook `notebooks/simple_example.py` shows how the individual functions in the workflow are used.
 
-![Clustering example](example_data/example_summary_plot_readme.png)
+![Clustering example](https://bitbucket.org/schwarzlab/phylotreeclustering/raw/master/example_data/example_summary_plot_readme.png)
 
 ## References
 
 **For the examples :**
 
 - Original data from Gao et al. 2016 
 Gao, R., Davis, A., McDonald, T. et al.
```

### Comparing `phylotreeclus-1.0.0/setup.py` & `phylotreeclus-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name='phylotreeclus',
-    version='1.0.0',
+    version='1.0.1',
     author='Elisa Billard',
     author_email='elisabillard1905@gmail.com',
     description='Clustering algorithm for phylogenetic cancer evolution trees',
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/schwarzlab/phylotreeclustering',
     classifiers=[
```

