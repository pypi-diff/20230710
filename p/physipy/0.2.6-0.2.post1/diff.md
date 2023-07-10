# Comparing `tmp/physipy-0.2.6.tar.gz` & `tmp/physipy-0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physipy-0.2.6.tar", last modified: Sun Jul  9 20:34:22 2023, max compression
+gzip compressed data, was "dist/physipy-0.2.post1.tar", last modified: Mon Apr 20 08:05:28 2020, max compression
```

## Comparing `physipy-0.2.6.tar` & `physipy-0.2.post1.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2023-07-09 20:34:22.851823 physipy-0.2.6/
--rw-r--r--   0 mocquin    (501) staff       (20)     1063 2020-04-17 07:50:09.000000 physipy-0.2.6/LICENSE
--rw-r--r--   0 mocquin    (501) staff       (20)      259 2022-09-13 20:07:22.000000 physipy-0.2.6/MANIFEST.in
--rw-r--r--   0 mocquin    (501) staff       (20)      335 2023-07-09 20:34:22.852015 physipy-0.2.6/PKG-INFO
--rw-r--r--   0 mocquin    (501) staff       (20)        0 2023-07-09 15:09:55.000000 physipy-0.2.6/README.md
-drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2023-07-09 20:34:22.839314 physipy-0.2.6/physipy/
--rw-r--r--   0 mocquin    (501) staff       (20)      660 2023-07-09 17:48:43.000000 physipy-0.2.6/physipy/__init__.py
--rw-r--r--   0 mocquin    (501) staff       (20)     9092 2023-07-09 16:13:27.000000 physipy-0.2.6/physipy/_constants.py
--rw-r--r--   0 mocquin    (501) staff       (20)       70 2023-07-09 20:32:55.000000 physipy-0.2.6/physipy/_version.py
--rw-r--r--   0 mocquin    (501) staff       (20)    10299 2023-07-09 15:45:40.000000 physipy-0.2.6/physipy/calculus.py
--rw-r--r--   0 mocquin    (501) staff       (20)     7919 2023-06-29 19:48:14.000000 physipy-0.2.6/physipy/math.py
-drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2023-07-09 20:34:22.846192 physipy-0.2.6/physipy/quantity/
--rw-r--r--   0 mocquin    (501) staff       (20)      562 2023-07-09 18:09:25.000000 physipy-0.2.6/physipy/quantity/__init__.py
--rw-r--r--   0 mocquin    (501) staff       (20)     3673 2023-07-09 16:18:23.000000 physipy-0.2.6/physipy/quantity/_plot.py
--rw-r--r--   0 mocquin    (501) staff       (20)     8041 2023-07-09 17:37:00.000000 physipy-0.2.6/physipy/quantity/_units.py
--rw-r--r--   0 mocquin    (501) staff       (20)    16543 2023-07-06 19:33:44.000000 physipy-0.2.6/physipy/quantity/dimension.py
--rw-r--r--   0 mocquin    (501) staff       (20)      142 2020-04-17 07:49:04.000000 physipy-0.2.6/physipy/quantity/dimension.txt
--rw-r--r--   0 mocquin    (501) staff       (20)    65867 2023-07-09 17:20:03.000000 physipy-0.2.6/physipy/quantity/quantity.py
--rw-r--r--   0 mocquin    (501) staff       (20)    22369 2023-07-06 19:33:44.000000 physipy-0.2.6/physipy/quantity/utils.py
-drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2023-07-09 20:34:22.851340 physipy-0.2.6/physipy.egg-info/
--rw-r--r--   0 mocquin    (501) staff       (20)      443 2023-07-09 20:34:22.000000 physipy-0.2.6/physipy.egg-info/SOURCES.txt
--rw-r--r--   0 mocquin    (501) staff       (20)       28 2020-11-11 21:50:34.000000 physipy-0.2.6/requirements.txt
--rw-r--r--   0 mocquin    (501) staff       (20)      158 2023-07-09 20:34:22.853071 physipy-0.2.6/setup.cfg
--rw-r--r--   0 mocquin    (501) staff       (20)     1179 2023-06-29 17:34:07.000000 physipy-0.2.6/setup.py
-drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2023-07-09 20:34:22.850139 physipy-0.2.6/test/
--rw-r--r--   0 mocquin    (501) staff       (20)        0 2020-04-17 07:50:09.000000 physipy-0.2.6/test/__init__.py
--rw-r--r--   0 mocquin    (501) staff       (20)     8760 2023-07-09 17:51:56.000000 physipy-0.2.6/test/test_dimension.py
--rw-r--r--   0 mocquin    (501) staff       (20)    84602 2023-07-09 17:52:23.000000 physipy-0.2.6/test/test_quantity.py
--rw-r--r--   0 mocquin    (501) staff       (20)      731 2023-07-09 17:55:20.000000 physipy-0.2.6/test/test_styles.py
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/
+-rw-r--r--   0 mocquin    (501) staff       (20)     1063 2020-04-17 07:50:09.000000 physipy-0.2.post1/LICENSE
+-rw-r--r--   0 mocquin    (501) staff       (20)      178 2020-04-20 08:04:22.000000 physipy-0.2.post1/MANIFEST.in
+-rw-r--r--   0 mocquin    (501) staff       (20)     5816 2020-04-20 08:05:28.000000 physipy-0.2.post1/PKG-INFO
+-rw-r--r--   0 mocquin    (501) staff       (20)     4787 2020-04-17 07:50:09.000000 physipy-0.2.post1/README.md
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy/
+-rw-r--r--   0 mocquin    (501) staff       (20)      791 2020-04-17 07:53:44.000000 physipy-0.2.post1/physipy/__init__.py
+-rw-r--r--   0 mocquin    (501) staff       (20)       73 2020-04-20 08:04:22.000000 physipy-0.2.post1/physipy/_version.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     9119 2020-04-17 07:49:04.000000 physipy-0.2.post1/physipy/constants.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     2617 2020-04-17 07:49:04.000000 physipy-0.2.post1/physipy/custom_units.py
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy/quantity/
+-rw-r--r--   0 mocquin    (501) staff       (20)      678 2020-04-17 07:53:44.000000 physipy-0.2.post1/physipy/quantity/__init__.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     8231 2020-04-17 09:45:51.000000 physipy-0.2.post1/physipy/quantity/calculus.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     9112 2020-04-17 07:50:09.000000 physipy-0.2.post1/physipy/quantity/dimension.py
+-rw-r--r--   0 mocquin    (501) staff       (20)      142 2020-04-17 07:49:04.000000 physipy-0.2.post1/physipy/quantity/dimension.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)     1503 2020-04-17 07:49:04.000000 physipy-0.2.post1/physipy/quantity/plot.py
+-rw-r--r--   0 mocquin    (501) staff       (20)    28159 2020-04-17 07:50:09.000000 physipy-0.2.post1/physipy/quantity/quantity.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     4725 2020-04-17 07:53:44.000000 physipy-0.2.post1/physipy/quantity/units.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     7083 2020-04-17 09:46:03.000000 physipy-0.2.post1/physipy/quantity/utils.py
+-rw-r--r--   0 mocquin    (501) staff       (20)      622 2019-05-19 19:12:31.000000 physipy-0.2.post1/physipy/quickstart.py
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/
+-rw-r--r--   0 mocquin    (501) staff       (20)     5816 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/PKG-INFO
+-rw-r--r--   0 mocquin    (501) staff       (20)      827 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/SOURCES.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)        1 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/dependency_links.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)       29 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/requires.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)        8 2020-04-20 08:05:28.000000 physipy-0.2.post1/physipy.egg-info/top_level.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)       28 2020-04-20 08:04:22.000000 physipy-0.2.post1/requirements.txt
+-rw-r--r--   0 mocquin    (501) staff       (20)       38 2020-04-20 08:05:28.000000 physipy-0.2.post1/setup.cfg
+-rw-r--r--   0 mocquin    (501) staff       (20)     1166 2020-04-20 08:04:22.000000 physipy-0.2.post1/setup.py
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/test/
+drwxr-xr-x   0 mocquin    (501) staff       (20)        0 2020-04-20 08:05:28.000000 physipy-0.2.post1/test/.ipynb_checkpoints/
+-rw-r--r--   0 mocquin    (501) staff       (20)        0 2019-04-05 06:33:34.000000 physipy-0.2.post1/test/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     4432 2020-03-17 09:38:41.000000 physipy-0.2.post1/test/.ipynb_checkpoints/test_dimension-checkpoint.py
+-rw-r--r--   0 mocquin    (501) staff       (20)      115 2019-04-05 17:14:52.000000 physipy-0.2.post1/test/.ipynb_checkpoints/test_physipy-checkpoint.py
+-rw-r--r--   0 mocquin    (501) staff       (20)    36266 2020-04-17 09:48:11.000000 physipy-0.2.post1/test/.ipynb_checkpoints/test_quantity-checkpoint.py
+-rw-r--r--   0 mocquin    (501) staff       (20)        0 2020-04-17 07:50:09.000000 physipy-0.2.post1/test/__init__.py
+-rw-r--r--   0 mocquin    (501) staff       (20)     4432 2020-04-17 07:50:09.000000 physipy-0.2.post1/test/test_dimension.py
+-rw-r--r--   0 mocquin    (501) staff       (20)      115 2020-04-17 07:50:09.000000 physipy-0.2.post1/test/test_physipy.py
+-rw-r--r--   0 mocquin    (501) staff       (20)    35407 2020-04-17 09:55:12.000000 physipy-0.2.post1/test/test_quantity.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `physipy-0.2.6/LICENSE` & `physipy-0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `physipy-0.2.6/physipy/_constants.py` & `physipy-0.2.post1/physipy/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """Define common physical constants.
 
 The constants values are retrieved from scipy.constants, and are separeted in 2 dictionnaries:
  - "scipy_constants" for the most commons constants
  - "scipy_constants_codata" for all the others
 A third "constants" dictionnary merges these two.
 
-TODO :
+TODO : 
  - create a function to wrap dict creation ?
  - should constants and units be in the same module ?
 
 """
 
 import scipy.constants as csts
 
@@ -26,15 +26,15 @@
 N = units["N"]
 
 # Raw mapping for scipy constants
 scipy_constants_raw = {
     "c"                      : (csts.c                     , m/s),
     "speed_of_light"         : (csts.speed_of_light        , m/s),   	
     "mu_0"                   : (csts.mu_0                  , m * kg * s**-2 * A**-2), 
-    "epsilon_0" 	         : (csts.epsilon_0 	           , A**2 * s**4 * kg**-1 * m**-3), 
+    "epsilon_0" 	         : (csts.epsilon_0 	           , A**2 * s**4 * kg**-2 * m**-3), 
     "h" 	                 : (csts.h 	                   , kg * m**2 * s**-1),    
     "Planck"                 : (csts.Planck                , kg * m**2 * s**-1), 
     "hbar" 	                 : (csts.hbar 	               , kg * m**2 * s**-1),    
     "G" 	                 : (csts.G	                   , m**3 * kg**-1 * s**-2),     
     "gravitational_constant" : (csts.gravitational_constant, m**3 * kg**-1 * s**-2),	
     "g"                      : (csts.g                     , m * s**-2),        
     "e" 	                 : (csts.e                     , A * s),    
@@ -207,30 +207,24 @@
     'kgf'            : (csts.kgf,            N),
     'kilogram_force' : (csts.kilogram_force, N),
 
 }
 
 
 # scipy constants codata
-scipy_constants_codata = {
-    key: make_quantity(
-        value[0] * value[1],
-        symbol=key) for key,
-    value in scipy_constants_codata_raw.items()}
+scipy_constants_codata = {key: make_quantity(value[0]*value[1],
+                                             symbol=key) for key, value in scipy_constants_codata_raw.items()}
 
 # scipy constants
-scipy_constants = {
-    key: make_quantity(
-        value[0] * value[1],
-        symbol=key) for key,
-    value in scipy_constants_raw.items()}
+scipy_constants = {key: make_quantity(value[0]*value[1],
+                                      symbol=key) for key, value in scipy_constants_raw.items()}
 
 # constants : concatenation of the two dicts
 constants = {**scipy_constants, **scipy_constants_codata}
 
 # clean up
 del csts
 del units
 del make_quantity
 del scipy_constants_codata_raw
 del scipy_constants_raw
-del m, s, kg, A, K, rad, mol
+del m, s, kg, A, K, rad, mol
```

### Comparing `physipy-0.2.6/physipy/calculus.py` & `physipy-0.2.post1/physipy/quantity/calculus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,352 +1,250 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Usefull calculus fonctions compatible with Quantity objects.
 
 These are basically numpy function wrapped with dimensions checks.
 """
-from __future__ import annotations
-from typing import Callable
 
 import numbers as nb
 
 import numpy as np
+import scipy
+import scipy.integrate
+import scipy.optimize
 import sympy as sp
 
-from .quantity.dimension import Dimension, DimensionError, SI_UNIT_SYMBOL
-from .quantity.quantity import quantify, Quantity
-from .quantity.utils import decorate_with_various_unit, asqarray
-
-
-def xvectorize(func: Callable) -> Callable:
-    """
-    1-D vectorize func.
-
-    func must have signature 'func(arg)', and vectorization is made along arg.
-    Returned value will be a Quantity object, even if returned values are
-    dimensionless (because of the use of asqarray).
-
-    Just like np.vectorize, this decorator is a utility to wrap a for loop -
-    it does not improve performance in any way.
-
-    Parameter
-    ---------
-    func : callable
-        A function of one parameter.
-
-    Returns
-    -------
-    callable
-        Decorated function.
-    """
-    def vec_func(x):
-        res = asqarray([func(i) for i in x])
-        return res
-    return vec_func
+from .dimension import Dimension, DimensionError, SI_UNIT_SYMBOL
+from .quantity import quantify, Quantity
+from .utils import array_to_Q_array, decorate_with_various_unit
+
+
+# Generiques
+#def linspace(Q_1, Q_2, nb_points=100):
+#    """Generate a lineary-spaced vector of Quantity.
+#    
+#    This function aims to extend numpy.linspace to Quantity objects.
+#    
+#    """
+#    Q_1 = quantify(Q_1)
+#    Q_2 = quantify(Q_2)
+#    if not Q_1.dimension == Q_2.dimension:
+#        raise DimensionError(Q_1.dimension, Q_2.dimension)
+#    val_out = np.linspace(Q_1.value, Q_2.value, nb_points)
+#    dim_out = Q_1.dimension
+#    favunit_out = Q_1.favunit
+#    return Quantity(val_out,
+#                    dim_out,
+#                    favunit=favunit_out)#.rm_dim_if_dimless()
+linspace = decorate_with_various_unit(("A", "A"), "A")(np.linspace)
+
+#def interp(x, tab_x, tab_y):
+#    """Interpolate the value of x in tab_y based on tab_x.
+#    
+#    This function aims to extend numpy.interp to Quantity.
+#    
+#    """
+#    x = quantify(x)
+#    tab_x = quantify(tab_x)
+#    tab_y = quantify(tab_y)
+#    if not x.dimension == tab_x.dimension:
+#        raise DimensionError(x, tab_x)
+#    val_interp = np.interp(x.value, tab_x.value, tab_y.value)
+#    dim_interp = tab_y.dimension
+#    favunit_interp = tab_y.favunit
+#    return Quantity(val_interp,
+#                    dim_interp,
+#                    favunit=favunit_interp)#.rm_dim_if_dimless()
+interp = decorate_with_various_unit(("A", "A", "B"), ("B"))(np.interp)
 
 
-def ndvectorize(func: Callable) -> Callable:
-    """
-    1-D vectorize func and accept input as ndarray.
 
-    func must have signature 'func(arg)', and vectorization is made along arg.
-    Returned value will be a Quantity object, even if returned values are
-    dimensionless (because of the use of asqarray).
-
-    Basically, func is applied to each value in arg input (as a flat list),
-    and output is reshaped to input shape.
-
-    Just like np.vectorize, this decorator is a utility to wrap a for loop -
-    it does not improve performance in any way.
-
-    Parameter
-    ---------
-    func : callable
-        A function of one parameter.
-
-    Returns
-    -------
-    callable
-        Decorated function.
-    """
-    def vec_func(x):
-        res = asqarray([func(i) for i in x.flat])
-        res.value = res.value.reshape(x.shape)
+def vectorize(func):
+    """Allow vectorize a function of Quantity.
+    
+    This function aims to extend numpy.vectorize to Quantity-function.
+    
+    """
+    func_vec = np.vectorize(func)
+    def func_Q_vec(*args, **kwargs):
+        res_brute = func_vec(*args, **kwargs)
+        res = array_to_Q_array(res_brute)
         return res
-    return vec_func
-
-
-def trapz2(Zs: Quantity, ech_x: Quantity, ech_y: Quantity) -> Quantity:
-    """
-    2D integral based on trapz.
-    ech_x is horizontal sampling, along row
-    ech_y is vertical sampling, along column
-
-
-    Example :
-    ---------
-        #sample a 2 squared meter, in both direction with different spacing
-        nx = 12
-        ny = 30
-        ech_dx = np.linspace(0*m, 2*m, num=nx)
-        ech_dy = np.linspace(0*m, 1*m ,num=ny)
-        X, Y = np.meshgrid(ech_dx, ech_dy)
-        # make a uniform ponderation
-        Zs = np.ones_like(X)
-        print(trapz2(Zs, ech_dx, ech_dy))
-        #prints 2 m**2
-
-    """
-    int_x = np.trapz(Zs, axis=-1, x=ech_x)
-    int_xy = np.trapz(int_x, axis=-1, x=ech_y)
-    return int_xy
+    return func_Q_vec
 
 
-"""
-scipy.integrate wrapped functions
-
-See : https://docs.scipy.org/doc/scipy/reference/integrate.html
-"""
-import numbers as nb
-import numpy as np
-import scipy
-import scipy.integrate
-
-from physipy import quantify, Quantity, Dimension, DimensionError
-from physipy.quantity.utils import check_dimension
+# Integrate
+def trapz(y, x=None, dx=1.0, *args):
+    """Starting from an array of quantity.
+    x and dx are exclusifs """
+    y = quantify(y)
+    if isinstance(x,Quantity):
+        value_trapz = np.trapz(y.value, x=x.value, *args)
+        dim_trapz = y.dimension * x.dimension
+    else:
+        dx = quantify(dx)
+        value_trapz = np.trapz(y.value, x=x, dx=dx.value, *args)
+        dim_trapz = y.dimension * dx.dimension
+    return Quantity(value_trapz, 
+                    dim_trapz).rm_dim_if_dimless()
+
+
+def integrate_trapz(Q_min, Q_max, Q_func):
+    """Integrate Q_func between Q_min and Q_max.
+    
+    We start by creating a np.linspace vector between the min and max values.
+    Then a Quantity vector with this linspace vector and th corresponding 
+    dimension is created.
+    
+    The dimension's are calculted :
+        - the function's output dimension : evaluating the function at Q_min,
+            giving the dimension of the
+        - the integral's output dimension : multipliying the function ouput
+            dimension, by the dimension of the integral's starting point.
+    
+    """
+    Q_min = quantify(Q_min)
+    Q_max = quantify(Q_max)
+    if not Q_min.dimension == Q_max.dimension:
+        raise DimensionError(Q_min.dimension, Q_max.dimension)
+    ech_x_val = np.linspace(Q_min.value, Q_max.value, 100)
+    Q_ech_x = Quantity(ech_x_val, Q_min.dimension)
+    Q_func = vectorize(Q_func)
+    Q_ech_y = quantify(Q_func(Q_ech_x))  # quantify for dimensionless cases
+    dim_in = quantify(Q_func(Q_min)).dimension
+    dim_out = dim_in * Q_min.dimension
+    integral = np.trapz(Q_ech_y.value, x=ech_x_val)
+    return Quantity(integral, dim_out)#.rm_dim_if_dimless()
 
 
-def quad(func, x0, x1, *oargs, args=(), **kwargs):
-    """A wrapper on scipy.integrate.quad :
-         - will check dimensions of x0 and x1 bounds
-         - returned value's dimension is infered by calling func(x0)
-    """
-    # Cast x bounds in Quantity and check dimension
+def quad(func, x0, x1, *args, **kwargs):
     x0 = quantify(x0)
     x1 = quantify(x1)
+    
     if not x0.dimension == x1.dimension:
         raise DimensionError(x0.dimension, x1.dimension)
-
-    # Get output dimension
+    
     res = func(x0, *args)
     res = quantify(res)
     res_dim = res.dimension
-
-    # define a float-version for inputs and outputs
-    def func_value(x_value, *oargs):
-        # cast back in Quantity
+    
+    def func_value(x_value, *args):
         x = Quantity(x_value, x0.dimension)
-        # compute Quantity result
+        
         res_raw = func(x, *args)
         raw = quantify(res_raw)
-        # return float-value
         return raw.value
-
-    # compute integral with float-value version
+    
     quad_value, prec = scipy.integrate.quad(func_value,
-                                            x0.value, x1.value,
-                                            *oargs, **kwargs)
-    # cast back in Quantity with dimension f(x)dx
+                                      x0.value, x1.value,
+                                      *args, **kwargs)
+    
     return Quantity(quad_value,
-                    res_dim * x0.dimension).rm_dim_if_dimless(), prec
+                   res_dim * x0.dimension).rm_dim_if_dimless(), prec
 
 
-def dblquad(func, x0, x1, y0, y1, *oargs, args=(), **kwargs):
+def dblquad(func, x0, x1, y0, y1, *args):
     x0 = quantify(x0)
     x1 = quantify(x1)
     y0 = quantify(y0)
     y1 = quantify(y1)
-
+    
     if not x0.dimension == x1.dimension:
         raise DimensionError(x0.dimension, x1.dimension)
     if not y0.dimension == y1.dimension:
         raise DimensionError(y0.dimension, y1.dimension)
-
-    res = func(y0, x0, *args)
+    
+    res = func(y0,x0, *args)
     res = quantify(res)
     res_dim = res.dimension
-
-    def func_value(y_value, x_value, *args):
+    
+    def func_value(y_value,x_value, *args):
         x = Quantity(x_value, x0.dimension)
         y = Quantity(y_value, y0.dimension)
-        res_raw = func(y, x, *args)
+        res_raw = func(y,x, *args)
         raw = quantify(res_raw)
         return raw.value
-
+    
     dblquad_value, prec = scipy.integrate.dblquad(func_value,
-                                                  x0.value, x1.value,
-                                                  y0.value, y1.value,
-                                                  *oargs, **kwargs)
-    return Quantity(dblquad_value, res_dim * x0.dimension *
-                    y0.dimension).rm_dim_if_dimless(), prec
+                                           x0.value, x1.value,
+                                           y0.value, y1.value,
+                                           args=args)
+    return Quantity(dblquad_value,
+                   res_dim * x0.dimension * y0.dimension).rm_dim_if_dimless(), prec
 
 
 def tplquad(func, x0, x1, y0, y1, z0, z1, *args):
     x0 = quantify(x0)
     x1 = quantify(x1)
     y0 = quantify(y0)
     y1 = quantify(y1)
     z0 = quantify(z0)
     z1 = quantify(z1)
-
+    
     if not x0.dimension == x1.dimension:
         raise DimensionError(x0.dimension, x1.dimension)
     if not y0.dimension == y1.dimension:
         raise DimensionError(y0.dimension, y1.dimension)
     if not z0.dimension == z1.dimension:
         raise DimensionError(z0.dimension, z1.dimension)
-
+    
     res = func(z0, y0, x0, *args)
     res = quantify(res)
     res_dim = res.dimension
-
-    def func_value(z_value, y_value, x_value, *args):
+    
+    def func_value(z_value, y_value,x_value, *args):
         x = Quantity(x_value, x0.dimension)
         y = Quantity(y_value, y0.dimension)
         z = Quantity(z_value, z0.dimension)
         res_raw = func(z, y, x, *args)
         raw = quantify(res_raw)
         return raw.value
-
+    
     tplquad_value, prec = scipy.integrate.tplquad(func_value,
-                                                  x0.value, x1.value,
-                                                  y0.value, y1.value,
-                                                  z0.value, z1.value,
-                                                  args=args)
-    return Quantity(tplquad_value, res_dim * x0.dimension *
-                    y0.dimension * z0.dimension).rm_dim_if_dimless(), prec
-
-
-def solve_ivp(
-        fun,
-        t_span,
-        Y0,
-        method='RK45',
-        t_eval=None,
-        dense_output=False,
-        events=None,
-        vectorized=False,
-        args=None,
-        **options):
-
-    not_scalar = len(Y0) > 1
-
-    # first, quantify everything that could be quantity
-    tstart, tstop = t_span
-    t_span = quantify(tstart), quantify(tstop)
-    if not t_span[0].dimension == t_span[1].dimension:
-        print("error of dimension")
-
-    if not_scalar:
-        Y0 = np.array([quantify(y) for y in Y0], dtype=object)
-    else:
-        Y0 = [quantify(y) for y in Y0]
-
-    if t_eval is not None:
-        t_eval = quantify(t_eval)
-
-    t_span_value = t_span[0].value, t_span[1].value
-    Y0_value = [y.value for y in Y0]
-    if t_eval is not None:
-        t_eval_value = t_eval.value
-    else:
-        t_eval_value = None
-
-    # second : rewrite everything without units
-
-    def func_value(t_value, Y_value):
-        # add back the units
-        t = Quantity(t_value, t_span[0].dimension)
-        if not_scalar:
-            Y = np.array([Quantity(y_value, y0.dimension)
-                         for y_value, y0 in zip(Y_value, Y0)], dtype=object)
-        else:
-            Y = Quantity(Y_value, Y0[0].dimension)
-        # compute with units
-        res_raw = fun(t, Y)
-        # extract the numerical value
-        if not_scalar:
-            raw = np.array([quantify(r) for r in res_raw], dtype=object)
-            raw_value = np.array([r.value for r in raw])
-        else:
-            raw_value = quantify(res_raw).value
-        return raw_value
-
-    # compute numerical solution
-
-    sol = scipy.integrate.solve_ivp(
-        func_value,
-        t_span_value,
-        Y0_value,
-        method=method,
-        t_eval=t_eval_value,
-        dense_output=dense_output,
-        events=events,
-        vectorized=vectorized,
-        args=args,
-        **options
-    )
-
-    # "decorate" the solution with units
-    sol.t = Quantity(sol.t, t_span[0].dimension)
-
-    if not_scalar:
-        # soly_q =
-        # arr_q = soly_q  # np.array(soly_q, dtype=object)
-        sol.y = [Quantity(y_value, y0.dimension)
-                 for y_value, y0 in zip(sol.y, Y0)]
-    else:
-        sol.y = Quantity(sol.y, Y0[0].dimension)
-
-    func_sol = sol.sol
-
-    # for some reason the solution accepts 0*s as well as 0
-    @check_dimension(t_span[0].dimension)
-    def sol_q(t):
-        return Quantity(func_sol(t), Y0[0].dimension)  # /t_span[0].dimension)
-    sol.sol = sol_q
-    return sol
-
+                                           x0.value, x1.value,
+                                           y0.value, y1.value,
+                                           z0.value, z1.value,
+                                           args=args)
+    return Quantity(tplquad_value,
+                   res_dim * x0.dimension * y0.dimension * z0.dimension).rm_dim_if_dimless(), prec    
 
 
-from typing import Callable
-
-
-import numbers as nb
-import numpy as np
-import scipy.optimize
-
-from physipy import quantify, Quantity, Dimension, DimensionError
-
-
-# Generique
-def root(func_cal: Callable, start, args=(), **kwargs) -> Quantity:
-    start = quantify(start)
+# Generique 
+def qroot(func_cal, start):
     start_val = start.value
     start_dim = start.dimension
-
     def func_cal_float(x_float):
-        q = Quantity(x_float, start_dim)
-        return func_cal(q, *args)
-    res = scipy.optimize.root(func_cal_float, start_val, **kwargs).x[0]
-    return Quantity(res, start_dim)
+        return func_cal(Quantity(x_float,start_dim))
+    return Quantity(scipy.optimize.root(func_cal_float, start_val).x[0], start_dim) #♦Quantity(fsolve(func_cal_float, start_val), start_dim)
 
 
-def brentq(func_cal: Callable, start, stop, *
-           oargs, args=(), **kwargs) -> Quantity:
+#def qbrentq(func_cal, start, stop):
+#    start_val = start.value
+#    stop_val = stop.value
+#    start_dim = start.dimension
+#    def func_cal_float(x_float):
+#        return func_cal(Quantity(x_float,start_dim))
+#    return Quantity(scipy.optimize.brentq(func_cal_float, start_val, stop_val), start_dim) #♦Quantity(fsolve(func_cal_float, start_val), start_dim)
+
+def qbrentq(func_cal, target, start, stop):
     start = quantify(start)
     stop = quantify(stop)
     if not start.dimension == stop.dimension:
         raise DimensionError(start.dimension, stop.dimension)
-
+        
     start_val = start.value
     start_dim = start.dimension
     stop_val = stop.value
-
+    
     def func_float(x):
-        res = func_cal(Quantity(x, start_dim), *args)
-        return quantify(res).value
+        return quantify(func_cal(Quantity(x, start_dim))).value - target.value
+    res = scipy.optimize.brentq(func_float, start_val, stop.value)
+    return Quantity(res, start_dim) # Quantity(fsolve(func_cal_float, 
+
+
+def main():
+    pass
 
-    res = scipy.optimize.brentq(func_float, start_val, stop.value, *oargs)
 
-    return Quantity(res, start_dim)
+if __name__ == "__main__":
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `physipy-0.2.6/physipy/quantity/__init__.py` & `physipy-0.2.post1/physipy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .quantity import Dimension, Quantity
-from .quantity import DimensionError, SI_UNIT_SYMBOL
-from .quantity import quantify, make_quantity, dimensionify
-from .utils import (check_dimension, set_favunit,
-                    dimension_and_favunit, drop_dimension,
-                    add_back_unit_param,
-                    decorate_with_various_unit, asqarray)
+from numpy import pi
 
-from ._plot import setup_matplotlib, plotting_context
+from ._version import __version__
+from . import quantity
+from .quantity import Quantity, Dimension, make_quantity, quantify, DimensionError, dimensionify
+from .quantity import check_dimension, set_favunit, dimension_and_favunit, drop_dimension, decorate_with_various_unit, add_back_unit_param, array_to_Q_array
+from .quantity import trapz, quad, dblquad, tplquad, qroot, qbrentq
+from .quantity import linspace, interp, vectorize
+from .quantity import m, kg, s, A, K, cd, mol, rad, sr, SI_units, SI_units_prefixed, SI_derived_units, other_units, units
 
-from ._units import m, s, kg, A, cd, K, mol, rad, sr
-from ._units import units, imperial_units
+from .quantity import setup_matplotlib
+
+from .constants import constants, scipy_constants, scipy_constants_codata
+from .custom_units import custom_units, imperial_units
```

### Comparing `physipy-0.2.6/setup.py` & `physipy-0.2.post1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSIONFILE = "physipy/_version.py"
+VERSIONFILE="physipy/_version.py"
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
@@ -27,16 +27,16 @@
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mocquin/physipy",
     author="mocquin",
     author_email="mocquin@me.com",
     license="MIT",
     keywords='physics physical unit units dimension quantity quantities',
-    packages=find_packages(exclude=("test", "benchmarks")),
+    packages=find_packages(exclude=("test", )),
     # add content of MANIFEST
     include_package_data=True,
-    install_requires=["numpy",
-                      "scipy",
+    install_requires=["numpy", 
+                      "scipy", 
                       "sympy",
                       "matplotlib",
-                      ]
+                     ]
 )
```

