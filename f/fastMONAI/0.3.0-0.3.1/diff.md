# Comparing `tmp/fastMONAI-0.3.0.tar.gz` & `tmp/fastMONAI-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastMONAI-0.3.0.tar", last modified: Wed Feb  1 09:15:20 2023, max compression
+gzip compressed data, was "fastMONAI-0.3.1.tar", last modified: Mon Jul 10 11:23:35 2023, max compression
```

## Comparing `fastMONAI-0.3.0.tar` & `fastMONAI-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-02-01 09:15:20.634648 fastMONAI-0.3.0/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      138 2022-09-05 07:20:58.000000 fastMONAI-0.3.0/CONTRIBUTING.md
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.0/LICENSE
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.0/MANIFEST.in
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-02-01 09:15:20.634648 fastMONAI-0.3.0/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2022-12-23 10:52:36.000000 fastMONAI-0.3.0/README.md
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-02-01 09:15:20.634648 fastMONAI-0.3.0/fastMONAI/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/__init__.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    29222 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/_modidx.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4781 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/dataset_info.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     8357 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/external_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.0/fastMONAI/research_utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1431 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.0/fastMONAI/vision_all.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9887 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_augmentation.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4892 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_core.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9193 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2582 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_inference.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3674 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_loss.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3035 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_metrics.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2107 2023-02-01 09:13:23.000000 fastMONAI-0.3.0/fastMONAI/vision_plot.py
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-02-01 09:15:20.634648 fastMONAI-0.3.0/fastMONAI.egg-info/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/SOURCES.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/dependency_links.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/entry_points.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.0/fastMONAI.egg-info/not-zip-safe
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/requires.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-02-01 09:15:20.000000 fastMONAI-0.3.0/fastMONAI.egg-info/top_level.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-02-01 09:12:50.000000 fastMONAI-0.3.0/settings.ini
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-02-01 09:15:20.634648 fastMONAI-0.3.0/setup.cfg
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.0/setup.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      138 2022-09-05 07:20:58.000000 fastMONAI-0.3.1/CONTRIBUTING.md
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/LICENSE
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/MANIFEST.in
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.1/README.md
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/fastMONAI/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/__init__.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    29361 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/_modidx.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4795 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/dataset_info.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     8357 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/external_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.1/fastMONAI/research_utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1431 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.1/fastMONAI/vision_all.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9887 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_augmentation.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     6553 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_core.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9193 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3352 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_inference.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3674 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_loss.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3035 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_metrics.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2997 2023-07-10 11:05:25.000000 fastMONAI-0.3.1/fastMONAI/vision_plot.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/fastMONAI.egg-info/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/entry_points.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.1/fastMONAI.egg-info/not-zip-safe
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/requires.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-10 11:23:35.000000 fastMONAI-0.3.1/fastMONAI.egg-info/top_level.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-10 11:19:23.000000 fastMONAI-0.3.1/settings.ini
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-10 11:23:35.385545 fastMONAI-0.3.1/setup.cfg
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.1/setup.py
```

### Comparing `fastMONAI-0.3.0/LICENSE` & `fastMONAI-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/PKG-INFO` & `fastMONAI-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.0
+Version: 0.3.1
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.0/README.md` & `fastMONAI-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/_modidx.py` & `fastMONAI-0.3.1/fastMONAI/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,16 @@
                                                                                  'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedBase.item_preprocessing': ( 'vision_core.html#medbase.item_preprocessing',
                                                                                              'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedBase.show': ('vision_core.html#medbase.show', 'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedImage': ('vision_core.html#medimage', 'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MedMask': ('vision_core.html#medmask', 'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.MetaResolver': ('vision_core.html#metaresolver', 'fastMONAI/vision_core.py'),
-                                       'fastMONAI.vision_core._load': ('vision_core.html#_load', 'fastMONAI/vision_core.py'),
+                                       'fastMONAI.vision_core._load_and_preprocess': ( 'vision_core.html#_load_and_preprocess',
+                                                                                       'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core._multi_channel': ( 'vision_core.html#_multi_channel',
                                                                                  'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core._preprocess': ('vision_core.html#_preprocess', 'fastMONAI/vision_core.py'),
                                        'fastMONAI.vision_core.med_img_reader': ( 'vision_core.html#med_img_reader',
                                                                                  'fastMONAI/vision_core.py')},
             'fastMONAI.vision_data': { 'fastMONAI.vision_data.MedDataBlock': ('vision_data.html#meddatablock', 'fastMONAI/vision_data.py'),
                                        'fastMONAI.vision_data.MedDataBlock.__init__': ( 'vision_data.html#meddatablock.__init__',
@@ -186,16 +187,16 @@
                                        'fastMONAI.vision_data.show_results': ('vision_data.html#show_results', 'fastMONAI/vision_data.py')},
             'fastMONAI.vision_inference': { 'fastMONAI.vision_inference._do_resize': ( 'vision_inference.html#_do_resize',
                                                                                        'fastMONAI/vision_inference.py'),
                                             'fastMONAI.vision_inference._to_original_orientation': ( 'vision_inference.html#_to_original_orientation',
                                                                                                      'fastMONAI/vision_inference.py'),
                                             'fastMONAI.vision_inference.inference': ( 'vision_inference.html#inference',
                                                                                       'fastMONAI/vision_inference.py'),
-                                            'fastMONAI.vision_inference.pred_postprocess': ( 'vision_inference.html#pred_postprocess',
-                                                                                             'fastMONAI/vision_inference.py')},
+                                            'fastMONAI.vision_inference.refine_binary_pred_mask': ( 'vision_inference.html#refine_binary_pred_mask',
+                                                                                                    'fastMONAI/vision_inference.py')},
             'fastMONAI.vision_loss': { 'fastMONAI.vision_loss.CustomLoss': ( 'vision_loss_functions.html#customloss',
                                                                              'fastMONAI/vision_loss.py'),
                                        'fastMONAI.vision_loss.CustomLoss.__call__': ( 'vision_loss_functions.html#customloss.__call__',
                                                                                       'fastMONAI/vision_loss.py'),
                                        'fastMONAI.vision_loss.CustomLoss.__init__': ( 'vision_loss_functions.html#customloss.__init__',
                                                                                       'fastMONAI/vision_loss.py'),
                                        'fastMONAI.vision_loss.CustomLoss.activation': ( 'vision_loss_functions.html#customloss.activation',
```

### Comparing `fastMONAI-0.3.0/fastMONAI/dataset_info.py` & `fastMONAI-0.3.1/fastMONAI/dataset_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% auto 0
 __all__ = ['MedDataset', 'get_class_weights']
 
 # %% ../nbs/08_dataset_info.ipynb 2
 from .vision_core import *
 
 from sklearn.utils.class_weight import compute_class_weight
-import multiprocessing as mp
+from concurrent.futures import ThreadPoolExecutor
 import pandas as pd
 import numpy as np
 import torch
 import glob
 
 # %% ../nbs/08_dataset_info.ipynb 4
 class MedDataset():
@@ -40,18 +40,17 @@
         Returns:
             DataFrame: A DataFrame with information about the dataset.
         '''
 
         if self.path:
             self.img_list = glob.glob(f'{self.path}/*{self.postfix}*')
             if not self.img_list: print('Could not find images. Check the image path')
-
-        #pool = mp.Pool(self.max_workers)
-        with mp.Pool(processes=self.max_workers) as pool:
-            data_info_dict = pool.map(self._get_data_info, self.img_list)
+        
+        with ThreadPoolExecutor(max_workers=self.max_workers) as executor:
+            data_info_dict = list(executor.map(self._get_data_info, self.img_list))
         
         df = pd.DataFrame(data_info_dict)
         if df.orientation.nunique() > 1: print('The volumes in this dataset have different orientations. Recommended to pass in the argument reorder=True when creating a MedDataset object for this dataset')
         return df
 
     def summary(self):
         '''Summary DataFrame of the dataset with example path for similar data.'''
```

### Comparing `fastMONAI-0.3.0/fastMONAI/external_data.py` & `fastMONAI-0.3.1/fastMONAI/external_data.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/research_utils.py` & `fastMONAI-0.3.1/fastMONAI/research_utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/utils.py` & `fastMONAI-0.3.1/fastMONAI/utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/vision_augmentation.py` & `fastMONAI-0.3.1/fastMONAI/vision_augmentation.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/vision_data.py` & `fastMONAI-0.3.1/fastMONAI/vision_data.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/vision_inference.py` & `fastMONAI-0.3.1/fastMONAI/vision_inference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_vision_inference.ipynb.
 
 # %% auto 0
-__all__ = ['inference', 'pred_postprocess']
+__all__ = ['inference', 'refine_binary_pred_mask']
 
 # %% ../nbs/06_vision_inference.ipynb 1
 import numpy as np
 from pathlib import Path
 from torchio import Resize
 from scipy.ndimage import label
 from .vision_core import *
@@ -52,14 +52,40 @@
         save_fn = Path(save_path)/('pred_' + Path(fn).parts[-1])
         org_img.save(save_fn)
         return save_fn
     
     return org_img
 
 # %% ../nbs/06_vision_inference.ipynb 7
-def pred_postprocess(pred_mask, remove_size=10437, percentage=0.2): 
-    '''Remove small objects from predicted mask.'''
-    small_objects = remove_size*percentage    
-    labeled_mask, ncomponents = label(pred_mask)
-    labeled_mask = remove_small_objects(labeled_mask, min_size=small_objects)
-    
-    return np.where(labeled_mask>0, 1., 0.)
+def refine_binary_pred_mask(
+        pred_mask,
+        remove_size: (int, float) = None,
+        percentage: float = 0.2,
+        verbose: bool = False
+):
+    """Removes small objects from the predicted binary mask.
+
+    Args:
+        pred_mask: The predicted mask from which small objects are to be removed.
+        remove_size: The size under which objects are considered 'small'.
+        percentage: The percentage of the remove_size to be used as threshold. 
+            Defaults to 0.2.
+        verbose: If True, print the number of components. Defaults to False.
+
+    Returns:
+        The processed mask with small objects removed.
+    """
+    labeled_mask, n_components = label(pred_mask)
+
+    if verbose:
+        print(n_components)
+
+    if remove_size is None:
+        sizes = np.bincount(labeled_mask.ravel())
+        max_label = sizes[1:].argmax() + 1
+        remove_size = sizes[max_label]
+
+    small_objects_threshold = remove_size * percentage
+    processed_mask = remove_small_objects(
+        labeled_mask, min_size=small_objects_threshold)
+
+    return np.where(processed_mask > 0, 1., 0.)
```

### Comparing `fastMONAI-0.3.0/fastMONAI/vision_loss.py` & `fastMONAI-0.3.1/fastMONAI/vision_loss.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI/vision_metrics.py` & `fastMONAI-0.3.1/fastMONAI/vision_metrics.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/fastMONAI.egg-info/PKG-INFO` & `fastMONAI-0.3.1/fastMONAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.0
+Version: 0.3.1
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.0/fastMONAI.egg-info/SOURCES.txt` & `fastMONAI-0.3.1/fastMONAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.0/settings.ini` & `fastMONAI-0.3.1/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = fastMONAI
 min_python = 3.7
-version = 0.3.0
+version = 0.3.1
 ### OPTIONAL ###
 
-requirements = fastai==2.7.10 monai==1.1.0 torchio==0.18.86 xlrd>=1.2.0 scikit-image==0.19.3 huggingface-hub gdown
+requirements = fastai==2.7.12 monai==1.2.0 torchio==0.18.91 xlrd>=1.2.0 scikit-image==0.19.3 huggingface-hub gdown
 dev_requirements = ipywidgets nbdev tabulate
 
 ### nbdev ###
 nbs_path = nbs
 doc_path = _docs
 recursive = False
 tst_flags = notest
```

### Comparing `fastMONAI-0.3.0/setup.py` & `fastMONAI-0.3.1/setup.py`

 * *Files identical despite different names*

