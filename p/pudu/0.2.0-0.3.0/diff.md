# Comparing `tmp/pudu-0.2.0.tar.gz` & `tmp/pudu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pudu-0.2.0.tar", last modified: Wed Jul  5 21:23:20 2023, max compression
+gzip compressed data, was "pudu-0.3.0.tar", last modified: Mon Jul 10 09:00:19 2023, max compression
```

## Comparing `pudu-0.2.0.tar` & `pudu-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.718939 pudu-0.2.0/
--rw-rw-rw-   0        0        0     1124 2022-11-22 08:22:56.000000 pudu-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4517 2023-07-05 21:23:20.719357 pudu-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3681 2023-05-17 09:45:31.000000 pudu-0.2.0/README.md
--rw-rw-rw-   0        0        0     3721 2023-05-17 09:45:54.000000 pudu-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.667771 pudu-0.2.0/pudu/
--rw-rw-rw-   0        0        0      137 2023-07-05 21:23:10.000000 pudu-0.2.0/pudu/__init__.py
--rw-rw-rw-   0        0        0     4607 2023-06-30 15:11:22.000000 pudu-0.2.0/pudu/error_handler.py
--rw-rw-rw-   0        0        0     2817 2023-06-27 11:07:42.000000 pudu-0.2.0/pudu/masks.py
--rw-rw-rw-   0        0        0     3790 2023-06-29 13:55:14.000000 pudu-0.2.0/pudu/perturbation.py
--rw-rw-rw-   0        0        0    13365 2023-07-04 13:45:49.000000 pudu-0.2.0/pudu/plots.py
--rw-rw-rw-   0        0        0    29322 2023-07-05 21:10:22.000000 pudu-0.2.0/pudu/pudu.py
--rw-rw-rw-   0        0        0     3842 2023-06-30 07:53:45.000000 pudu-0.2.0/pudu/standards.py
-drwxrwxrwx   0        0        0        0 2023-07-05 21:23:20.716988 pudu-0.2.0/pudu.egg-info/
--rw-rw-rw-   0        0        0     4517 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       62 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.2.0/pudu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 21:23:20.000000 pudu-0.2.0/pudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       66 2023-06-28 13:59:09.000000 pudu-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0      449 2023-07-05 21:23:20.723419 pudu-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1844 2023-07-05 21:21:28.000000 pudu-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.942481 pudu-0.3.0/
+-rw-rw-rw-   0        0        0     1124 2023-07-10 07:31:04.000000 pudu-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      129 2022-11-04 23:37:34.000000 pudu-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4517 2023-07-10 09:00:19.943478 pudu-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3681 2023-05-17 09:45:31.000000 pudu-0.3.0/README.md
+-rw-rw-rw-   0        0        0     3721 2023-05-17 09:45:54.000000 pudu-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.918546 pudu-0.3.0/pudu/
+-rw-rw-rw-   0        0        0      137 2023-07-10 07:31:20.000000 pudu-0.3.0/pudu/__init__.py
+-rw-rw-rw-   0        0        0     4461 2023-07-08 13:16:56.000000 pudu-0.3.0/pudu/error_handler.py
+-rw-rw-rw-   0        0        0     2616 2023-07-09 10:38:07.000000 pudu-0.3.0/pudu/masks.py
+-rw-rw-rw-   0        0        0    12316 2023-07-08 15:34:18.000000 pudu-0.3.0/pudu/perturbation.py
+-rw-rw-rw-   0        0        0    13365 2023-07-04 13:45:49.000000 pudu-0.3.0/pudu/plots.py
+-rw-rw-rw-   0        0        0    28362 2023-07-10 07:29:05.000000 pudu-0.3.0/pudu/pudu.py
+-rw-rw-rw-   0        0        0     2941 2023-07-08 14:00:15.000000 pudu-0.3.0/pudu/standards.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:00:19.942481 pudu-0.3.0/pudu.egg-info/
+-rw-rw-rw-   0        0        0     4517 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       62 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-22 10:14:32.000000 pudu-0.3.0/pudu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       62 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-10 09:00:19.000000 pudu-0.3.0/pudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 pudu-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2023-06-28 13:59:09.000000 pudu-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      449 2023-07-10 09:00:19.945473 pudu-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2023-07-10 07:30:25.000000 pudu-0.3.0/setup.py
```

### Comparing `pudu-0.2.0/LICENSE` & `pudu-0.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022, Institut de Recerca en Energia de Catalunya
+Copyright (c) 2023, Institut de Recerca en Energia de Catalunya
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pudu-0.2.0/PKG-INFO` & `pudu-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pudu-0.2.0/README.md` & `pudu-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pudu-0.2.0/README.rst` & `pudu-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pudu-0.2.0/pudu/error_handler.py` & `pudu-0.3.0/pudu/error_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                             "Got `y` with shape: %s" % str(np.array(y).shape))
     else:
         if not isinstance(y, list) or len(y) != x_shape[0]:
             raise ValueError("Expected `x` and `y` to have the same length when `x` has a batch size more than 1."
                             "Got `x` with length (batch size): %s and `y` with length: %s" 
                             % (str(x_shape[0]), str(len(y))))
 
-def for_params(window, scope, padding, absolute, inspect, steps, layer, p):
+def for_params(window, scope, padding, absolute, inspect, layer, p):
     """
     Handles erros for the main parameters of the different functions.
     """
 
     if p is None:
         pass
     elif not (0 <= p <= 1):
@@ -87,12 +87,7 @@
         if inspect[0] <= 0 or inspect[1] <= 0:
             raise ValueError("Value for inspect, or its components, must be greater"
                                 "than 0. Got instead: %s" % str(inspect))
         
     elif (not isinstance(inspect, int)) or inspect < 0:
         raise ValueError("Expected value for inspect is an integer greater than 0." 
                             "Got instead: %s" % str(inspect))
-
-    if not isinstance(steps, list):
-        raise ValueError("Expected value for inspect is a list. Got instead: %s" % str(steps))
-
-
```

### Comparing `pudu-0.2.0/pudu/plots.py` & `pudu-0.3.0/pudu/plots.py`

 * *Files identical despite different names*

### Comparing `pudu-0.2.0/pudu/pudu.py` & `pudu-0.3.0/pudu/pudu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections import defaultdict, Counter
-import matplotlib.pyplot as plt
 from keras.models import Model
 import numpy as np
 import copy
-from . import masks, perturbation, error_handler, plots, standards
+
+from . import error_handler, standards
+from . import masks as msk
+from . import perturbation as ptn
 
 class pudu:
     def __init__(self, x, y, pf, model=None):
         """
         `pudu` constructor.
 
         :type x: list
@@ -47,26 +49,26 @@
         # Activation results
         self.lac = None # layer activation
         self.uac = None # unit activations
         self.fac = None # feature activations
         self.icc = None
 
         # Normalized results are calculated automatically so if the user needs them
-        self.imp_norm = None
-        self.spe_norm = None
-        self.syn_norm = None
-        self.lac_norm = None
-        self.uac_norm = None
+        self.imp_rel = None
+        self.spe_rel = None
+        self.syn_rel = None
+        self.lac_rel = None
+        self.uac_rel = None
         
         # Some error handling        
         error_handler.for_constructor(model, x, y)
         
 
-    def importance(self, window=1, scope=None, evolution=None, padding='center', 
-                    absolute=False, **kwargs):
+    def importance(self, window=1, scope=None, evolution=None, padding='center', bias=0,
+                    absolute=False, perturbation=ptn.Bidirectional(), mask=msk.All()):
         """
         Calculates the importance vector for the input feature.
 
         :type window: int
         :param window: feature width to be changeg each time.
             
         :type scope: tupple(int, int)
@@ -83,39 +85,40 @@
             added and `window`starts from `0`. If `left`, padding to the left
             is applyied and `window` ends at length `x`. If perfet `center` is
             not possible, then ipadding left is added `1`.
         
         :type absolute: bool
         :param absolute: Weather or not the result is in absolute value or not. Default is `False`.
         """
-        error_handler.for_params(window, scope, padding, absolute, 0, [1, 2, 3], None, None)
+        error_handler.for_params(window, scope, padding, absolute, 0, None, None)
 
         # Initial values
         sh = np.array(self.x).shape
-        x_copy = copy.deepcopy(self.x)
         d_temp = np.zeros((sh[0], sh[1], sh[2], sh[3]))
-        
-        scope, window, padding, evolution = standards.params_std(self.y, sh, scope, window, padding, evolution)
-        padd = standards.calc_pad(padding, scope, window)
-        mask_array = masks.function(sh=sh, padd=padd, scope=scope, window=window, **kwargs)
+
+        scope, window, padd, evolution, total = standards.params_std(self.y, sh, scope, window, padding, evolution)
 
         p0 = self.pf(self.x)
+        section = 1
         row = padd[0][0] + scope[0][0]
         while row <= scope[0][1] - padd[0][1] - window[0]:
             col = padd[1][0] + scope[1][0]
             while col <= scope[1][1] - padd[1][1] - window[1]:
+                x_copy = copy.deepcopy(self.x)
+
+                mask_val = mask.apply(section, total)
 
-                if mask_array[0][row][col][0] == 1:
+                if mask_val == 1:
 
                     row_idx, col_idx = np.meshgrid(range(window[0]), range(window[1]), indexing='ij')
                     row_idx, col_idx = row_idx + row, col_idx + col
 
-                    temp, temp2 = perturbation.function(x=x_copy, row=row_idx, col=col_idx, **kwargs)
+                    temp, temp2 = perturbation.apply(x_copy, row, col, window, bias)
 
-                    if temp2 is False:
+                    if temp2 is None:
                         val = self.pf(temp) - p0
                     else:
                         val = (self.pf(temp2) + self.pf(temp) - 2*p0) / 2
 
                     if absolute:
                         val = abs(val)
 
@@ -123,25 +126,28 @@
                         d_temp[0, row:row+window[0], col:col+window[1], 0] = val[evolution]
                     else:
                         d_temp[0, row:row+window[0], col:col+window[1], 0] = val
                 
                 else:
                     pass
 
+                section += 1
+
                 col += window[1]
             row += window[0]
 
         self.imp = d_temp
         
         max_val, min_val = d_temp.max(), d_temp.min()
-        self.imp_norm = (d_temp - min_val) / (max_val - min_val)
+        self.imp_rel = (d_temp - min_val) / (max_val - min_val)
 
 
-    def speed(self, window=1, scope=None, evolution=None, padding='center', 
-                steps=[0,0.1,0.2], absolute=False, **kwargs):
+    def speed(self, window=1, scope=None, evolution=None, padding='center',
+                bias=0, absolute=False, mask=msk.All(), 
+                perturbation=[ptn.Bidirectional(delta=.1), ptn.Bidirectional(delta=.2), ptn.Bidirectional(delta=.3)]):
         """
         Calculates the gradient of the importance. In other words, the slope
             of the curve formed by the importance at different values. This 
             indicates how fast a feature can change the result.
             
         :type window: int
         :param window: feature width to be changeg each time.
@@ -159,50 +165,45 @@
             to each side is applyed. If `right`, then paading to the right is 
             added and `window`starts from `0`. If `left`, padding to the left
             is applyied and `window` ends at length `x`. If perfet `center` is
             not possible, then ipadding left is added `1`.
 
         :type absolute: bool
         :param absolute: Weather or not the result is in absolute value or not. Default is `False`.
-
-        :type steps: list
-        :param steps: Contains the different values at which the importance will be measured.
-            In other words, the values at which the feature will be changed (feature*steps)
-            before applyin the perturbation function (perturbation(feature*steps)). This means
-            it orks somewhat differently than `importnace` and `synergy`.
         """
-        error_handler.for_params(window, scope, padding, absolute, 0, steps, None, None)
+        error_handler.for_params(window, scope, padding, absolute, 0, None, None)
 
         # Initial values
         sh = np.array(self.x).shape
-        x_copy = copy.deepcopy(self.x)
         d_temp = np.zeros((sh[0], sh[1], sh[2], sh[3]))
         
-        scope, window, padding, evolution = standards.params_std(self.y, sh, scope, window, padding, evolution)
-        padd = standards.calc_pad(padding, scope, window)
-        mask_array = masks.function(sh=sh, padd=padd, scope=scope, window=window, **kwargs)
+        scope, window, padd, evolution, total = standards.params_std(self.y, sh, scope, window, padding, evolution)
 
-        p0 = self.pf(self.x) 
+        p0 = self.pf(self.x)
+        section = 1
         row = padd[0][0] + scope[0][0]
         while row <= scope[0][1] - padd[0][1] - window[0]:
             col = padd[1][0] + scope[1][0]
             while col <= scope[1][1] - padd[1][1] - window[1]:
+                x_copy = copy.deepcopy(self.x)
+
+                mask_val = mask.apply(section, total)
 
-                if mask_array[0][row][col][0] == 1:
+                if mask_val == 1:
 
                     p = []
 
                     row_idx, col_idx = np.meshgrid(range(window[0]), range(window[1]), indexing='ij')
                     row_idx, col_idx = row_idx + row, col_idx + col
                     
-                    for j in steps:
+                    for j in perturbation:
                         temp = self.x.copy()
-                        temp[0, row, col, 0] = (x_copy[0, row, col, 0]) * j
-                        temp, temp2 = perturbation.function(x=temp, row=row_idx, col=col_idx, **kwargs)
-                        
+                       
+                        temp, temp2 = j.apply(x_copy, row, col, window, bias)
+
                         if temp2 is False:
                             val = self.pf(temp) - p0
                         else:
                             val = (self.pf(temp2) + self.pf(temp)) / 2
 
                         if absolute:
                             val = abs(val)
@@ -215,26 +216,28 @@
                     var_x = [i for i in range(len(p))]
                     var_y = [i for i in p]
                             
                     d_temp[0, row:row+window[0], col:col+window[1], 0] = np.polyfit(var_x, var_y, 1)[0]
 
                 else:
                     pass    
+                
+                section += 1
 
                 col += window[1]
             row += window[0]
 
         self.spe = d_temp
         
         max_val, min_val = d_temp.max(), d_temp.min()
-        self.spe_norm = (d_temp - min_val) / (max_val - min_val)
+        self.spe_rel = (d_temp - min_val) / (max_val - min_val)
 
     
-    def synergy(self, delta=0.1, window=1, inspect=0, scope=None, absolute=False,
-                    evolution=None, padding='center', **kwargs):
+    def synergy(self, window=1, inspect=0, scope=None, absolute=False, bias=0,
+                    evolution=None, padding='center', perturbation=ptn.Bidirectional(), mask=msk.All()):
         """
         Calculates the synergy between features.
         
         :type delta: float
         :param delta: maximum variation to apply to each feature.
             
         :type window: int
@@ -254,82 +257,84 @@
             added and `window`starts from `0`. If `left`, padding to the left
             is applyied and `window` ends at length `x`. If perfet `center` is
             not possible, then ipadding left is added `1`.
         
         :type absolute: bool
         :param absolute: Weather or not the result is in absolute value or not. Default is `False`.
         """
-        error_handler.for_params(window, scope, padding, absolute, inspect, [1, 2, 3], None, None)
+        error_handler.for_params(window, scope, padding, absolute, inspect, None, None)
 
         # Initial values
         sh = np.array(self.x).shape
-        x_copy = copy.deepcopy(self.x)
         d_temp = np.zeros((sh[0], sh[1], sh[2], sh[3]))
         
-        scope, window, padding, evolution = standards.params_std(self.y, sh, scope, window, padding, evolution)
-        padd = standards.calc_pad(padding, scope, window)
-        mask_array = masks.function(sh=sh, padd=padd, scope=scope, window=window, **kwargs)
+        scope, window, padd, evolution, total = standards.params_std(self.y, sh, scope, window, padding, evolution)
 
         # Position to range of the desired area to calculate synergy from
         if len(np.array(inspect).shape) == 0:
             if sh[1] == 1:
                 inspect = (0, int(window[1]*inspect + padd[1][0] + scope[1][0]))
             else:
                 inspect = (window[0]*inspect + padd[0][0] + scope[0][0], 
                            window[1]*inspect + padd[1][0] + scope[1][0])
-        
-        base = copy.deepcopy(x_copy)
-        for i in range(inspect[0], inspect[0]+window[0]):
-            for j in range(inspect[1], inspect[1]+window[1]):
-                base[0][i][j][0] = x_copy[0][i][j][0]*(1+delta)
-        
-        p0 = self.pf(self.x)
+                
+        x_copy = copy.deepcopy(self.x)
+        base, base2 = perturbation.apply(x_copy, inspect[0], inspect[1], window, bias)
+
+        pb0 = self.pf(base)
+        pb2 = self.pf(base2)
+
+        section = 1
         row = padd[0][0] + scope[0][0]
         while row <= scope[0][1] - padd[0][1] - window[0]:
             col = padd[1][0] + scope[1][0]
             while col <= scope[1][1] - padd[1][1] - window[1]:
-                if mask_array[0][row][col][0] == 1:
+                x_copy = copy.deepcopy(self.x)
+
+                mask_val = mask.apply(section, total)
+
+                if mask_val == 1:
 
                     if inspect[0] == row and inspect[1] == col:
                         pass
                     else:
                         row_idx, col_idx = np.meshgrid(range(window[0]), range(window[1]), indexing='ij')
                         row_idx, col_idx = row_idx + row, col_idx + col
 
-                        temp, temp2 = perturbation.function(x=x_copy, row=row_idx, col=col_idx, **kwargs)
+                        temp, temp2 = perturbation.apply(x_copy, row, col, window, bias)
 
                         if temp2 is False:
-                            val = self.pf(temp) - p0
+                            val = self.pf(temp) - pb0
                         else:
-                            val = (self.pf(temp2) + self.pf(temp)) / 2
+                            val = (self.pf(temp2) + self.pf(temp) - pb0 - pb2) / 2
 
                         if absolute:
                             val = abs(val)
 
                         if np.shape(val):
                             d_temp[0, row:row+window[0], col:col+window[1], 0] = val[evolution]
                         else:
                             d_temp[0, row:row+window[0], col:col+window[1], 0] = val
                 else:
                     pass
 
+                section += 1
+
                 col += window[1]
             row += window[0]
 
         self.syn = d_temp
         
         max_val, min_val = d_temp.max(), d_temp.min()
-        self.syn_norm = (d_temp - min_val) / (max_val - min_val)
+        self.syn_rel = (d_temp - min_val) / (max_val - min_val)
 
 
-    def activations(self, layer=0, slope=0, p=0.005, window=1, scope=None, 
-                        padding='center', **kwargs):
+    def reactivations(self, layer=0, slope=0, p=0.005, window=1, scope=None, bias=0,
+                        padding='center', perturbation=ptn.Bidirectional(), mask=msk.All()):
         """
-        a_q_a
-        a_q_k
         Counts the unit activations in the selected `layer` of a `Keras` model according 
             to change in the feature.
         
         :type layer: int
         :param layer: Position number within the keras model to be analyzed. Use `model.summary()`
             to see exactly the position of the desired layer.
 
@@ -347,51 +352,52 @@
         :param padding: Type of padding. If the legnth of `x` is not divisible 
             by `window` then padding is applyed. If `center`, then equal padding 
             to each side is applyed. If `right`, then paading to the right is 
             added and `window`starts from `0`. If `left`, padding to the left
             is applyied and `window` ends at length `x`. If perfet `center` is
             not possible, then ipadding left is added `1`.
         """
-        error_handler.for_params(window, scope, padding, False, 0, [1, 2, 3], layer, p)
+        error_handler.for_params(window, scope, padding, False, 0, layer, p)
         
         # Initial values
         sh = np.array(self.x).shape
-        x_copy = copy.deepcopy(self.x)
         d_temp = np.zeros((sh[0], sh[1], sh[2], sh[3]))
         o_b, o_h, o_w, o_d = sh[0], sh[1], sh[2], sh[3]
         
-        scope, window, padding, _ = standards.params_std(self.y, sh, scope, window, padding, None)
-        padd = standards.calc_pad(padding, scope, window)
-        mask_array = masks.function(sh=sh, padd=padd, scope=scope, window=window, **kwargs)
+        scope, window, padd, evolution, total = standards.params_std(self.y, sh, scope, window, padding, None)
 
         # Keras
         layer_outputs = [layer.output for layer in self.model.layers]
         activation_model = Model(inputs=self.model.input, outputs=layer_outputs)
 
         x = np.squeeze(self.x, axis=0) if self.x.shape[1] == 1 else self.x
         activations = activation_model.predict(x, verbose=0)
         p0 = activations[layer] # raw activation values for the image
 
-        index_array = [[] for _ in range(len(p0.flatten()))] # to store unit idx and coordinates
-        # act_count = np.zeros_like(p0) # this one counts activations per unit
-        act_count = [] # new
-        
+        # index_array = [[] for _ in range(len(p0.flatten()))] # to store unit idx and coordinates
+
+        act_count = []
         act_idx_count = 1
+        section = 1
         row = padd[0][0] + scope[0][0]
         while row <= scope[0][1] - padd[0][1] - window[0]:
             col = padd[1][0] + scope[1][0]
             while col <= scope[1][1] - padd[1][1] - window[1]:
-                if mask_array[0][row][col][0] == 1:
+                x_copy = copy.deepcopy(self.x)
+                
+                mask_val = mask.apply(section, total)
+
+                if mask_val == 1:
 
                     row_idx, col_idx = np.meshgrid(range(window[0]), range(window[1]), indexing='ij')
                     row_idx, col_idx = row_idx + row, col_idx + col
 
-                    temp, temp2 = perturbation.function(x=x_copy, row=row_idx, col=col_idx, **kwargs)
+                    temp, temp2 = perturbation.apply(x_copy, row, col, window, bias)
 
-                    if temp2 is False:
+                    if temp2 is None:
                         temp = np.squeeze(temp, axis=0) if temp.shape[1] == 1 else temp
 
                         activations = activation_model.predict(temp, verbose=0)
                         activations = activations[layer]
                         activations = activations-p0
 
                     else:
@@ -402,24 +408,24 @@
                         p1 = activations[layer]
 
                         activations = activation_model.predict(temp2, verbose=0)
                         p2 = activations[layer]
 
                         activations = (p1 + p2 - 2*p0) / 2
 
-                    # act_flat = activations.flatten()
-                    # act_count.append(act_flat)
                     act_count.append(activations.flatten())
 
                     d_temp[0, row:row+window[0], col:col+window[1], 0] = act_idx_count
                     act_idx_count += 1
 
                 else:
                     pass
 
+                section += 1
+
                 col += window[1]
             row += window[0]
 
         """
         At this point 'act_count' has dims. (n, k), where n is the number
         of times the kernel fits in the input and 'k' is the number of of units.
         So now we calculate the quantiles and store the values above the quantile
@@ -468,19 +474,19 @@
         mask = d_temp[0, :, :, 0] != 0
         d_temp[0, :, :, 0][mask] = vfunc(d_temp[0, :, :, 0][mask])
 
         self.fac = counts_feats
 
         self.lac = d_temp # this shows the activation mapping, or activations per feature
         max_val, min_val = d_temp.max(), d_temp.min()
-        self.lac_norm = (d_temp - min_val) / (1 if (max_val - min_val) == 0 else (max_val - min_val))
+        self.lac_rel = (d_temp - min_val) / (1 if (max_val - min_val) == 0 else (max_val - min_val))
         
         self.uac = counts_units # new
         max_val, min_val = counts_units.max(), counts_units.min()
-        self.uac_norm = (counts_units - min_val) / (1 if (max_val - min_val) == 0 else (max_val - min_val))
+        self.uac_rel = (counts_units - min_val) / (1 if (max_val - min_val) == 0 else (max_val - min_val))
 
         un_fe = defaultdict(list)
         for u, f in zip(units, feats):
             un_fe[u].append(f)
         un_fe = [un_fe[i] for i in range(max(units) + 1)]
 
         result = []
@@ -489,16 +495,16 @@
                 counts = Counter(sublist) # reps. of each number
                 most_common_num, num_repetitions = counts.most_common(1)[0] # most reps.
                 result.append([i, most_common_num, num_repetitions])
         
         return feats, units
 
 
-    def relatable(self, layer=0, slope=0, p=0.005, window=1, scope=None, 
-                    padding='center', **kwargs):
+    def relatable(self, layer=0, slope=0, p=0.005, window=1, scope=None, bias=0,
+                    padding='center', perturbation=ptn.Bidirectional(), mask=msk.All()):
         """
         This function generates an activation report for each set of coordinates in `x` and `y`. 
 
         :type layer: int
         :param layer: Specifies the layer of the model for which the activation report is to be generated. 
                     Default is 0.
 
@@ -523,40 +529,35 @@
         """
         # hay que cambiar self.x e .y para iterar. Se guarda y luego
         # se cambia por cada integrante. Al final se vuelve a la forma
         # original si se desea usar denuevo
         s_x, s_y = self.x, self.y
 
         master = []
-        # master = np.array()
         for x, y in zip(s_x, s_y):
             x = np.expand_dims(x, 0)
-            self.x, self.y = x, y 
-            feats, units = self.activations(layer, slope, p, window, scope, padding, **kwargs)
+            self.x, self.y = x, y
 
-            master.extend((i, j) for i, j in zip(feats, units))
+            feats, units = self.reactivations(layer, slope, p, window, scope, bias, padding,
+                                                perturbation, mask)
 
-            feats = np.array(feats)
-            units = np.array(units)
-            master = np.column_stack((feats, units))
-                        
-            master = master.tolist()
+            master.extend((i, j) for i, j in zip(feats, units))
 
-        master = [tuple(arr) for arr in master]
         counts = Counter(master)
         result = [[j, count, i] for (i, j), count in counts.items()]
         result = np.transpose(result)
 
         self.x, self.y = s_x, s_y
         self.icc = result
 
 
     def preview(self, window=1, scope=None, padding='center', axis=None, show_data=True,
                     title='Preview', xlabel='Feature', ylabel='Intensity', xticks=None, 
-                    yticks=[], cmap='Greens', font_size=15, figsize=(14, 4), bold=False, **kwargs):
+                    yticks=[], cmap='Greens', font_size=15, figsize=(14, 4), bold=False,
+                    mask = msk.All()):
         """
         Plots an approximate preview of the sections, areas, or mask to be analyzed over the data
             before executing. It is particularly useful to check if the parameters are
             correct, especially if the user expects long runtimes.
         
         :type feature: list
         :param feature: feature analyzed or any that the user whant to plot against.
@@ -610,43 +611,44 @@
 
         :type figsize: tuple
         :param figsize: Figure size for the plot.
 
         :type bold: Boolean
         :param bold: To make the limit lines bolder. Default is 'False'.
         """
-        error_handler.for_params(window, scope, padding, False, 0, [1, 2, 3], None, None)
+        error_handler.for_params(window, scope, padding, False, 0, None, None)
 
         # Initial values
         image = [] # this will be the preview image
         sh = np.array(self.x).shape
         d_temp = np.zeros((sh[0], sh[1], sh[2], sh[3]))
         countour = np.zeros((sh[0], sh[1], sh[2], sh[3]))
                 
-        scope, window, padding, _ = standards.params_std(self.y, sh, scope, window, padding, evolution=None)
-        padd = standards.calc_pad(padding, scope, window)
-        mask_array = masks.function(sh=sh, padd=padd, scope=scope, window=window, **kwargs)
+        scope, window, padd, evolution, total = standards.params_std(self.y, sh, scope, window, padding, None)
 
+        section = 1
         row = padd[0][0] + scope[0][0]
         while row <= scope[0][1] - padd[0][1] - window[0]:
             col = padd[1][0] + scope[1][0]
             while col <= scope[1][1] - padd[1][1] - window[1]:
+                mask_val = mask.apply(section, total)
 
-                if mask_array[0][row][col][0] == 1:
+                if mask_val == 1:
                     countour[0, row, col, 0] = 1
                     d_temp[0, row:row+window[0], col:col+window[1], 0] = 1
 
                     if sh[1] > 1:
                         for i in range(sh[1]):
                             countour[0, i, col, 0] = 1
                         for i in range(sh[2]):
                             countour[0, row, i, 0] = 1
                 else:
                     pass
-
+                
+                section += 1
                 col += window[1]
             row += window[0]
 
         dims = np.array(d_temp).shape
         image = d_temp[0,:,:,0]
         countour = countour[0,:,:,0]
```

### Comparing `pudu-0.2.0/pudu.egg-info/PKG-INFO` & `pudu-0.3.0/pudu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pudu
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for explainability of machine learinng algorithms in an agnostic, deterministic, and simple way.
 Home-page: https://github.com/pudu-py/pudu
 Author: pudu
 Author-email: puduhola@gmail.com
 License: MIT license
 Keywords: pudu
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pudu-0.2.0/setup.py` & `pudu-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pudu',
     name='pudu',
     packages=find_packages(include=['pudu', 'pudu.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pudu-py/pudu',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

