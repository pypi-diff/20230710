# Comparing `tmp/micomputing-1.1.44.tar.gz` & `tmp/micomputing-1.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.44.tar", last modified: Fri Jul  7 10:16:07 2023, max compression
+gzip compressed data, was "micomputing-1.1.45.tar", last modified: Mon Jul 10 07:53:47 2023, max compression
```

## Comparing `micomputing-1.1.44.tar` & `micomputing-1.1.45.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-07 10:16:07.545988 micomputing-1.1.44/
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-07 10:16:07.000000 micomputing-1.1.44/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-07 10:16:07.545841 micomputing-1.1.44/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-07 10:16:07.000000 micomputing-1.1.44/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-07 10:16:07.543301 micomputing-1.1.44/micomputing/
--rw-r--r--   0 admin      (501) staff       (20)     2397 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/data.py
--rw-r--r--   0 admin      (501) staff       (20)    38302 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/funcs.py
--rw-r--r--   0 admin      (501) staff       (20)    54346 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/metrics.py
--rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/micfunctions.so
--rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/network.py
--rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/plot.py
--rw-r--r--   0 admin      (501) staff       (20)    41826 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/stdio.py
--rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/test.py
--rw-r--r--   0 admin      (501) staff       (20)    98918 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/trans.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-07 10:16:07.544761 micomputing-1.1.44/micomputing/zxhtools/
--rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/TRS.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-07 10:16:07.545606 micomputing-1.1.44/micomputing/zxhtools/__pycache__/
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
--rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/exec.py
--rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/image2.AFF
--rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing/zxhtools/image2.FFD
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-07 10:16:07.544212 micomputing-1.1.44/micomputing.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       83 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-07 10:16:07.000000 micomputing-1.1.44/micomputing.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-07 10:16:07.546038 micomputing-1.1.44/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1496 2023-07-07 10:16:07.000000 micomputing-1.1.44/setup_micomputing.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-10 07:53:47.264627 micomputing-1.1.45/
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-07-10 07:53:47.000000 micomputing-1.1.45/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-10 07:53:47.264454 micomputing-1.1.45/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-10 07:53:47.000000 micomputing-1.1.45/README.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-10 07:53:47.262012 micomputing-1.1.45/micomputing/
+-rw-r--r--   0 admin      (501) staff       (20)     2397 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    29365 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/data.py
+-rw-r--r--   0 admin      (501) staff       (20)    38302 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/funcs.py
+-rw-r--r--   0 admin      (501) staff       (20)    54346 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/metrics.py
+-rwxr-xr-x   0 admin      (501) staff       (20)    33404 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/micfunctions.so
+-rw-r--r--   0 admin      (501) staff       (20)    23556 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/network.py
+-rw-r--r--   0 admin      (501) staff       (20)    23394 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/plot.py
+-rw-r--r--   0 admin      (501) staff       (20)    41820 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/stdio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1215 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/test.py
+-rw-r--r--   0 admin      (501) staff       (20)    99366 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/trans.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-10 07:53:47.263352 micomputing-1.1.45/micomputing/zxhtools/
+-rw-r--r--   0 admin      (501) staff       (20)     7454 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/TRS.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-10 07:53:47.264030 micomputing-1.1.45/micomputing/zxhtools/__pycache__/
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     6173 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     9153 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8988 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc
+-rw-r--r--   0 admin      (501) staff       (20)     8071 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/exec.py
+-rw-r--r--   0 admin      (501) staff       (20)      507 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/image2.AFF
+-rw-r--r--   0 admin      (501) staff       (20)    21032 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing/zxhtools/image2.FFD
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-07-10 07:53:47.262817 micomputing-1.1.45/micomputing.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      766 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       83 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       12 2023-07-10 07:53:47.000000 micomputing-1.1.45/micomputing.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-07-10 07:53:47.264685 micomputing-1.1.45/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1496 2023-07-10 07:53:47.000000 micomputing-1.1.45/setup_micomputing.py
```

### Comparing `micomputing-1.1.44/PKG-INFO` & `micomputing-1.1.45/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.44
+Version: 1.1.45
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.44/README.md` & `micomputing-1.1.45/README.md`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/__init__.py` & `micomputing-1.1.45/micomputing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pycamia import info_manager
 
 __info__ = info_manager(
     project = 'PyCAMIA',
     package = 'micomputing',
     author = 'Yuncheng Zhou',
     create = '2021-12',
-    version = '1.1.43',
+    version = '1.1.44',
     contact = 'bertiezhou@163.com',
     keywords = ['medical image', 'image registration', 'image similarities'],
     description = "'micomputing' is a package for medical image computing. ",
     requires = ['numpy', 'torch>=1.5.1', 'batorch', 'matplotlib', 'pycamia', 'pyoverload', 'nibabel', 'pydicom', 'SimpleITK'],
-    update = '2023-07-07 00:43:40',
+    update = '2023-07-07 18:16:07',
     package_data = True
 ).check()
-__version__ = '1.1.43'
+__version__ = '1.1.44'
 
 from . import plot as plt
 from .stdio import IMG, dcm2nii, nii2dcm #*
 from .data import Info, Subject, ImageObject, Dataset, MedicalDataset #*
 from .network import U_Net, CNN, FCN
 from .funcs import reorient, rescale, reflect, dilate, blur, bending, distance_map, registration, local_prior, center_of_gravity #*
 from .trans import Transformation, SpatialTransformation, ImageTransformation, ComposedTransformation, CompoundTransformation, Identity, Id, Rotation90, Rotation180, Rotation270, Reflect, Reflection, Permutedim, DimPermutation, Rescale, Rescaling, Translate, Translation, Rigid, Rig, Affine, Aff, PolyAffine, logEu, LocallyAffine, LARM, FreeFormDeformation, FFD, DenseDisplacementField, DDF, MultiLayerPerception, MLP, Normalize, resample, interpolation, interpolation_forward, Affine2D2Matrix, Quaterns2Matrix, Matrix2Quaterns #*
```

### Comparing `micomputing-1.1.44/micomputing/data.py` & `micomputing-1.1.45/micomputing/data.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/funcs.py` & `micomputing-1.1.45/micomputing/funcs.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/metrics.py` & `micomputing-1.1.45/micomputing/metrics.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/micfunctions.so` & `micomputing-1.1.45/micomputing/micfunctions.so`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/network.py` & `micomputing-1.1.45/micomputing/network.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/plot.py` & `micomputing-1.1.45/micomputing/plot.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/stdio.py` & `micomputing-1.1.45/micomputing/stdio.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,21 +501,21 @@
         return tuple(self.image.GetSize())
     
     @property
     def orientation(self):
         if self.has_series: raise Error('Property')("No property 'orientation' for micomputing.IMG with series. ")
         affine = self.affine
         dim_ord = np.abs(affine[:-1, :-1]).argmax(0).tolist()
-        try: dx = np.array([affine[d, dim_ord.index(d)] for d in range(len(dim_ord))])
+        try: dx = np.array([affine[dim_ord[d], d] for d in range(len(dim_ord))])
         except ValueError: raise TypeError(f"Invalid affine matrix: {affine}")
         return ''.join([['RL', 'AP', 'SI'][i][j] for i, j in zip(dim_ord, dx > 0)])
 
     def reorient(self, orient='LPI'):
         if self.has_series: raise Error('Property')("Cannot reorient for micomputing.IMG with series. ")
-        axis = {'L':'LR', 'R':'LR', 'A':'AP', 'P':'AP', 'I':'IS', 'S':'IS'}
+        axis = {'L':'LR', 'R':'LR', 'A':'AP', 'P':'AP', 'I':'SI', 'S':'SI'}
         from .funcs import reorient
         from .trans import Translation, Reflection, DimPermutation, ComposedTransformation
         orient_axis = [axis[i] for i in self.orientation]
         permutation = [orient_axis.index(axis[i]) for i in orient]
         new_orient = [self.orientation[i] for i in permutation]
         reflect_dims = [i for i, (a, b) in enumerate(zip(new_orient, orient)) if a != b]
         data = self.to_tensor()
```

### Comparing `micomputing-1.1.44/micomputing/test.py` & `micomputing-1.1.45/micomputing/test.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/trans.py` & `micomputing-1.1.45/micomputing/trans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1100,5084 +1100,5112 @@
 000044b0: 6375 725f 6166 6669 6e65 203d 204e 6f6e  cur_affine = Non
 000044c0: 650a 2020 2020 2020 2020 666f 7220 7420  e.        for t 
 000044d0: 696e 2073 656c 662e 7472 616e 735f 6c69  in self.trans_li
 000044e0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
 000044f0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
 00004500: 6528 742c 2053 7061 7469 616c 5472 616e  e(t, SpatialTran
 00004510: 7366 6f72 6d61 7469 6f6e 293a 206f 7574  sformation): out
-00004520: 5f6c 6973 742e 6170 7065 6e64 2874 290a  _list.append(t).
-00004530: 2020 2020 2020 2020 2020 2020 6166 6620              aff 
-00004540: 3d20 742e 6166 6669 6e65 286e 5f64 696d  = t.affine(n_dim
-00004550: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00004560: 2061 6666 2069 7320 4e6f 6e65 2061 6e64   aff is None and
-00004570: 2063 7572 5f61 6666 696e 6520 6973 206e   cur_affine is n
-00004580: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004590: 2020 2020 2020 2020 206f 7574 5f6c 6973           out_lis
-000045a0: 742e 6578 7465 6e64 285b 4166 6669 6e65  t.extend([Affine
-000045b0: 2863 7572 5f61 6666 696e 6529 2c20 745d  (cur_affine), t]
-000045c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000045d0: 2020 6375 725f 6166 6669 6e65 203d 204e    cur_affine = N
-000045e0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000045f0: 656c 6966 2061 6666 2069 7320 4e6f 6e65  elif aff is None
-00004600: 3a20 6f75 745f 6c69 7374 2e61 7070 656e  : out_list.appen
-00004610: 6428 7429 0a20 2020 2020 2020 2020 2020  d(t).           
-00004620: 2065 6c69 6620 6166 662e 7370 6163 6520   elif aff.space 
-00004630: 213d 2028 6e5f 6469 6d2b 312c 206e 5f64  != (n_dim+1, n_d
-00004640: 696d 2b31 293a 0a20 2020 2020 2020 2020  im+1):.         
-00004650: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00004660: 6545 7272 6f72 2866 2255 6e63 6f6e 7369  eError(f"Unconsi
-00004670: 7374 656e 7420 7472 616e 7366 6f72 6d61  stent transforma
-00004680: 7469 6f6e 2077 6974 6820 6166 6669 6e65  tion with affine
-00004690: 206f 6620 7369 7a65 207b 6166 662e 7370   of size {aff.sp
-000046a0: 6163 657d 2069 6e20 436f 6d70 6f73 6564  ace} in Composed
-000046b0: 5472 616e 7366 6f72 6d61 7469 6f6e 2e20  Transformation. 
-000046c0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-000046d0: 6c69 6620 6375 725f 6166 6669 6e65 2069  lif cur_affine i
-000046e0: 7320 4e6f 6e65 3a20 6375 725f 6166 6669  s None: cur_affi
-000046f0: 6e65 203d 2061 6666 0a20 2020 2020 2020  ne = aff.       
-00004700: 2020 2020 2065 6c73 653a 2063 7572 5f61       else: cur_a
-00004710: 6666 696e 6520 3d20 6375 725f 6166 6669  ffine = cur_affi
-00004720: 6e65 2040 2061 6666 0a20 2020 2020 2020  ne @ aff.       
-00004730: 2069 6620 6375 725f 6166 6669 6e65 2069   if cur_affine i
-00004740: 7320 6e6f 7420 4e6f 6e65 3a20 6f75 745f  s not None: out_
-00004750: 6c69 7374 2e61 7070 656e 6428 4166 6669  list.append(Affi
-00004760: 6e65 2863 7572 5f61 6666 696e 6529 290a  ne(cur_affine)).
-00004770: 2020 2020 2020 2020 7265 7475 726e 2043          return C
-00004780: 6f6d 706f 7365 6454 7261 6e73 666f 726d  omposedTransform
-00004790: 6174 696f 6e28 2a6f 7574 5f6c 6973 742c  ation(*out_list,
-000047a0: 206d 6f64 6520 3d20 7365 6c66 2e6d 6f64   mode = self.mod
-000047b0: 6529 0a0a 2020 2020 6465 6620 746f 5f64  e)..    def to_d
-000047c0: 6963 7428 7365 6c66 293a 0a20 2020 2020  ict(self):.     
-000047d0: 2020 2064 6963 203d 2073 7570 6572 2829     dic = super()
-000047e0: 2e74 6f5f 6469 6374 2829 0a20 2020 2020  .to_dict().     
-000047f0: 2020 2064 6963 5b27 7472 616e 735f 6c69     dic['trans_li
-00004800: 7374 275d 203d 205b 742e 746f 5f64 6963  st'] = [t.to_dic
-00004810: 7428 2920 666f 7220 7420 696e 2073 656c  t() for t in sel
-00004820: 662e 7472 616e 735f 6c69 7374 5d0a 2020  f.trans_list].  
-00004830: 2020 2020 2020 7265 7475 726e 2064 6963        return dic
-00004840: 0a0a 2323 2323 2323 2323 2323 2320 5370  ..########### Sp
-00004850: 6174 6961 6c20 5472 616e 7366 6f72 6d61  atial Transforma
-00004860: 7469 6f6e 7320 2323 2323 2323 2323 2323  tions ##########
-00004870: 230a 0a63 6c61 7373 2053 7061 7469 616c  #..class Spatial
-00004880: 5472 616e 7366 6f72 6d61 7469 6f6e 2854  Transformation(T
-00004890: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
-000048a0: 2020 2020 0a20 2020 2064 6566 205f 5f69      .    def __i
-000048b0: 6e69 745f 5f28 7365 6c66 2c20 2a70 6172  nit__(self, *par
-000048c0: 616d 732c 202a 2a6b 7770 6172 616d 7329  ams, **kwparams)
-000048d0: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
-000048e0: 292e 5f5f 696e 6974 5f5f 282a 7061 7261  ).__init__(*para
-000048f0: 6d73 2c20 2a2a 6b77 7061 7261 6d73 290a  ms, **kwparams).
-00004900: 2020 2020 2020 2020 7365 6c66 2e62 6163          self.bac
-00004910: 6b77 6172 6420 3d20 5472 7565 0a20 2020  kward = True.   
-00004920: 2020 2020 200a 2020 2020 6465 6620 5f5f       .    def __
-00004930: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
-00004940: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004950: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
-00004960: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
-00004970: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
-00004980: 642e 0a20 2020 2020 2020 2020 2020 2073  d..            s
-00004990: 697a 653a 2028 5b6e 5f62 6174 6368 3a20  ize: ([n_batch: 
-000049a0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
-000049b0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-000049c0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-000049d0: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
-000049e0: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
-000049f0: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
-00004a00: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00004a10: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00004a20: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
-00004a30: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
-00004a40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004a50: 6176 6f75 6368 2858 2e68 6173 5f63 6861  avouch(X.has_cha
-00004a60: 6e6e 656c 2c20 6622 506c 6561 7365 2075  nnel, f"Please u
-00004a70: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
-00004a80: 7220 6f66 2073 697a 6520 5c0a 2020 2020  r of size \.    
-00004a90: 2020 2020 2020 2020 285b 6e5f 6261 7463          ([n_batc
-00004aa0: 683a 6f70 7469 6f6e 616c 5d2c 207b 7b6e  h:optional], {{n
-00004ab0: 5f64 696d 7d7d 2c20 6e5f 312c 206e 5f32  _dim}}, n_1, n_2
-00004ac0: 2c20 2e2e 2e2c 206e 5f72 2920 5c0a 2020  , ..., n_r) \.  
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004ae0: 7220 7b73 656c 662e 5f5f 636c 6173 735f  r {self.__class_
-00004af0: 5f2e 5f5f 6e61 6d65 5f5f 2e73 706c 6974  _.__name__.split
-00004b00: 2827 2e27 295b 2d31 5d7d 2054 7261 6e73  ('.')[-1]} Trans
-00004b10: 666f 726d 6174 696f 6e2c 2069 6e73 7465  formation, inste
-00004b20: 6164 206f 6620 7b58 2e73 6861 7065 7d2e  ad of {X.shape}.
-00004b30: 2022 290a 2020 2020 2020 2020 6966 2073   ").        if s
-00004b40: 656c 662e 6e5f 6469 6d20 6973 206e 6f74  elf.n_dim is not
-00004b50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004b60: 2020 2061 766f 7563 6828 582e 6e5f 6368     avouch(X.n_ch
-00004b70: 616e 6e65 6c20 3d3d 2073 656c 662e 6e5f  annel == self.n_
-00004b80: 6469 6d2c 2066 227b 7365 6c66 2e6e 5f64  dim, f"{self.n_d
-00004b90: 696d 7d44 207b 7365 6c66 2e5f 5f63 6c61  im}D {self.__cla
-00004ba0: 7373 5f5f 2e5f 5f6e 616d 655f 5f2e 7370  ss__.__name__.sp
-00004bb0: 6c69 7428 272e 2729 5b2d 315d 7d20 5472  lit('.')[-1]} Tr
-00004bc0: 616e 7366 6f72 6d61 7469 6f6e 205c 0a20  ansformation \. 
-00004bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004be0: 6f65 7320 6e6f 7420 7461 6b65 2063 6f6f  oes not take coo
-00004bf0: 7264 696e 6174 6573 206f 6620 7369 7a65  rdinates of size
-00004c00: 207b 582e 7368 6170 657d 2229 0a20 2020   {X.shape}").   
-00004c10: 2020 2020 2069 6620 582e 6861 735f 6261       if X.has_ba
-00004c20: 7463 683a 2061 766f 7563 6828 7365 6c66  tch: avouch(self
-00004c30: 2e6e 5f62 6174 6368 2069 7320 4e6f 6e65  .n_batch is None
-00004c40: 206f 7220 7365 6c66 2e6e 5f62 6174 6368   or self.n_batch
-00004c50: 203d 3d20 3120 6f72 2058 2e6e 5f62 6174   == 1 or X.n_bat
-00004c60: 6368 203d 3d20 3120 6f72 2058 2e6e 5f62  ch == 1 or X.n_b
-00004c70: 6174 6368 203d 3d20 7365 6c66 2e6e 5f62  atch == self.n_b
-00004c80: 6174 6368 2c20 0a20 2020 2020 2020 2020  atch, .         
-00004c90: 2020 2066 227b 7365 6c66 2e6e 5f64 696d     f"{self.n_dim
-00004ca0: 7d44 207b 7365 6c66 2e5f 5f63 6c61 7373  }D {self.__class
-00004cb0: 5f5f 2e5f 5f6e 616d 655f 5f2e 7370 6c69  __.__name__.spli
-00004cc0: 7428 272e 2729 5b2d 315d 7d20 5472 616e  t('.')[-1]} Tran
-00004cd0: 7366 6f72 6d61 7469 6f6e 2077 6974 6820  sformation with 
-00004ce0: 6261 7463 6820 7369 7a65 207b 7365 6c66  batch size {self
-00004cf0: 2e6e 5f62 6174 6368 7d20 5c0a 2020 2020  .n_batch} \.    
-00004d00: 2020 2020 2020 2020 2020 2020 646f 6573              does
-00004d10: 206e 6f74 2074 616b 6520 636f 6f72 6469   not take coordi
-00004d20: 6e61 7465 7320 7769 7468 2077 726f 6e67  nates with wrong
-00004d30: 2062 6174 6368 2073 697a 652e 2043 7572   batch size. Cur
-00004d40: 7265 6e74 2073 697a 653a 207b 582e 7368  rent size: {X.sh
-00004d50: 6170 657d 2e22 290a 2020 2020 2020 2020  ape}.").        
-00004d60: 5920 3d20 582e 666c 6f61 7428 292e 636c  Y = X.float().cl
-00004d70: 6f6e 6528 290a 2020 2020 2020 2020 6966  one().        if
-00004d80: 206e 6f74 2059 2e68 6173 5f62 6174 6368   not Y.has_batch
-00004d90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00004da0: 2073 656c 662e 6e5f 6261 7463 6820 6973   self.n_batch is
-00004db0: 206e 6f74 204e 6f6e 653a 2059 203d 2059   not None: Y = Y
-00004dc0: 2e6d 756c 7469 706c 7928 7365 6c66 2e6e  .multiply(self.n
-00004dd0: 5f62 6174 6368 2c20 5b5d 290a 2020 2020  _batch, []).    
-00004de0: 2020 2020 2020 2020 656c 7365 3a20 5920          else: Y 
-00004df0: 3d20 592e 756e 7371 7565 657a 6528 5b5d  = Y.unsqueeze([]
-00004e00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00004e10: 2059 0a0a 2020 2020 6465 6620 5f5f 6d61   Y..    def __ma
-00004e20: 746d 756c 5f5f 2878 2c20 7929 3a0a 2020  tmul__(x, y):.  
-00004e30: 2020 2020 2020 6966 2069 735f 7370 6174        if is_spat
-00004e40: 6961 6c5f 7472 616e 7366 6f72 6d61 7469  ial_transformati
-00004e50: 6f6e 2878 2920 616e 6420 6973 5f73 7061  on(x) and is_spa
-00004e60: 7469 616c 5f74 7261 6e73 666f 726d 6174  tial_transformat
-00004e70: 696f 6e28 7929 3a0a 2020 2020 2020 2020  ion(y):.        
-00004e80: 2020 2020 7265 7475 726e 2043 6f6d 706f      return Compo
-00004e90: 7365 6454 7261 6e73 666f 726d 6174 696f  sedTransformatio
-00004ea0: 6e28 782c 2079 2c20 6d6f 6465 3d22 7370  n(x, y, mode="sp
-00004eb0: 6174 6961 6c22 290a 2020 2020 2020 2020  atial").        
-00004ec0: 7265 7475 726e 2043 6f6d 706f 7365 6454  return ComposedT
-00004ed0: 7261 6e73 666f 726d 6174 696f 6e28 782c  ransformation(x,
-00004ee0: 2079 290a 2020 2020 0a20 2020 2064 6566   y).    .    def
-00004ef0: 2061 6666 696e 6528 7365 6c66 2c20 6e5f   affine(self, n_
-00004f00: 6469 6d3d 4e6f 6e65 293a 0a20 2020 2020  dim=None):.     
-00004f10: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00004f20: 2020 200a 2020 2020 4061 6c69 6173 2827     .    @alias('
-00004f30: 746f 4444 4627 290a 2020 2020 6465 6620  toDDF').    def 
-00004f40: 746f 5f44 4446 2873 656c 662c 202a 7368  to_DDF(self, *sh
-00004f50: 6170 6529 3a0a 2020 2020 2020 2020 7368  ape):.        sh
-00004f60: 6170 6520 3d20 6172 675f 7475 706c 6528  ape = arg_tuple(
-00004f70: 7368 6170 6529 0a20 2020 2020 2020 2067  shape).        g
-00004f80: 7269 6420 3d20 6274 2e69 6d61 6765 5f67  rid = bt.image_g
-00004f90: 7269 6428 2a73 6861 7065 292e 756e 7371  rid(*shape).unsq
-00004fa0: 7565 657a 6528 5b5d 292e 666c 6f61 7428  ueeze([]).float(
-00004fb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00004fc0: 2073 656c 6628 6772 6964 2920 2d20 6772   self(grid) - gr
-00004fd0: 6964 0a0a 2020 2020 6465 6620 746f 5f69  id..    def to_i
-00004fe0: 6d61 6765 5f73 7061 6365 2873 656c 662c  mage_space(self,
-00004ff0: 2073 6f75 7263 652c 2074 6172 6765 7429   source, target)
-00005000: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-00005010: 6e73 7461 6e63 6528 736f 7572 6365 2c20  nstance(source, 
-00005020: 7374 7229 3a20 736f 7572 6365 203d 2049  str): source = I
-00005030: 4d47 2873 6f75 7263 6529 0a20 2020 2020  MG(source).     
-00005040: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00005050: 2874 6172 6765 742c 2073 7472 293a 2074  (target, str): t
-00005060: 6172 6765 7420 3d20 494d 4728 7461 7267  arget = IMG(targ
-00005070: 6574 290a 2020 2020 2020 2020 6966 2069  et).        if i
-00005080: 7369 6e73 7461 6e63 6528 736f 7572 6365  sinstance(source
-00005090: 2c20 494d 4729 3a20 736f 7572 6365 203d  , IMG): source =
-000050a0: 2073 6f75 7263 652e 6166 6669 6e65 0a20   source.affine. 
-000050b0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000050c0: 616e 6365 2874 6172 6765 742c 2049 4d47  ance(target, IMG
-000050d0: 293a 2074 6172 6765 7420 3d20 7461 7267  ): target = targ
-000050e0: 6574 2e61 6666 696e 650a 2020 2020 2020  et.affine.      
-000050f0: 2020 7265 7475 726e 2073 656c 662e 746f    return self.to
-00005100: 2827 696d 6167 6527 2c20 736f 7572 6365  ('image', source
-00005110: 5f61 6666 696e 653d 736f 7572 6365 2c20  _affine=source, 
-00005120: 7461 7267 6574 5f61 6666 696e 653d 7461  target_affine=ta
-00005130: 7267 6574 290a 0a20 2020 2064 6566 2074  rget)..    def t
-00005140: 6f5f 776f 726c 645f 7370 6163 6528 7365  o_world_space(se
-00005150: 6c66 2c20 736f 7572 6365 2c20 7461 7267  lf, source, targ
-00005160: 6574 293a 0a20 2020 2020 2020 2069 6620  et):.        if 
-00005170: 6973 696e 7374 616e 6365 2873 6f75 7263  isinstance(sourc
-00005180: 652c 2073 7472 293a 2073 6f75 7263 6520  e, str): source 
-00005190: 3d20 494d 4728 736f 7572 6365 290a 2020  = IMG(source).  
-000051a0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000051b0: 6e63 6528 7461 7267 6574 2c20 7374 7229  nce(target, str)
-000051c0: 3a20 7461 7267 6574 203d 2049 4d47 2874  : target = IMG(t
-000051d0: 6172 6765 7429 0a20 2020 2020 2020 2069  arget).        i
-000051e0: 6620 6973 696e 7374 616e 6365 2873 6f75  f isinstance(sou
-000051f0: 7263 652c 2049 4d47 293a 2073 6f75 7263  rce, IMG): sourc
-00005200: 6520 3d20 736f 7572 6365 2e61 6666 696e  e = source.affin
-00005210: 650a 2020 2020 2020 2020 6966 2069 7369  e.        if isi
-00005220: 6e73 7461 6e63 6528 7461 7267 6574 2c20  nstance(target, 
-00005230: 494d 4729 3a20 7461 7267 6574 203d 2074  IMG): target = t
-00005240: 6172 6765 742e 6166 6669 6e65 0a20 2020  arget.affine.   
-00005250: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00005260: 2e74 6f28 2777 6f72 6c64 272c 2073 6f75  .to('world', sou
-00005270: 7263 655f 6166 6669 6e65 3d73 6f75 7263  rce_affine=sourc
-00005280: 652c 2074 6172 6765 745f 6166 6669 6e65  e, target_affine
-00005290: 3d74 6172 6765 7429 0a0a 2020 2020 6465  =target)..    de
-000052a0: 6620 746f 2873 656c 662c 2073 7061 6365  f to(self, space
-000052b0: 203d 2022 776f 726c 6422 2c20 736f 7572   = "world", sour
-000052c0: 6365 5f61 6666 696e 6520 3d20 6274 2e65  ce_affine = bt.e
-000052d0: 7965 2834 292c 2074 6172 6765 745f 6166  ye(4), target_af
-000052e0: 6669 6e65 203d 2062 742e 6579 6528 3429  fine = bt.eye(4)
-000052f0: 293a 0a20 2020 2020 2020 2074 6172 6765  ):.        targe
-00005300: 745f 6166 6669 6e65 203d 2062 6174 6f72  t_affine = bator
-00005310: 6368 5f74 656e 736f 7228 7461 7267 6574  ch_tensor(target
-00005320: 5f61 6666 696e 6529 2e66 6c6f 6174 2829  _affine).float()
-00005330: 0a20 2020 2020 2020 2073 6f75 7263 655f  .        source_
-00005340: 6166 6669 6e65 203d 2062 6174 6f72 6368  affine = batorch
-00005350: 5f74 656e 736f 7228 736f 7572 6365 5f61  _tensor(source_a
-00005360: 6666 696e 6529 2e66 6c6f 6174 2829 0a20  ffine).float(). 
-00005370: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00005380: 5f61 6666 696e 652e 6e64 696d 203c 3d20  _affine.ndim <= 
-00005390: 323a 2074 6172 6765 745f 6166 6669 6e65  2: target_affine
-000053a0: 203d 2062 742e 756e 7371 7565 657a 6528   = bt.unsqueeze(
-000053b0: 7461 7267 6574 5f61 6666 696e 6529 0a20  target_affine). 
-000053c0: 2020 2020 2020 2069 6620 736f 7572 6365         if source
-000053d0: 5f61 6666 696e 652e 6e64 696d 203c 3d20  _affine.ndim <= 
-000053e0: 323a 2073 6f75 7263 655f 6166 6669 6e65  2: source_affine
-000053f0: 203d 2062 742e 756e 7371 7565 657a 6528   = bt.unsqueeze(
-00005400: 736f 7572 6365 5f61 6666 696e 6529 0a20  source_affine). 
-00005410: 2020 2020 2020 2069 6620 7370 6163 652e         if space.
-00005420: 6c6f 7765 7228 2920 3d3d 2022 776f 726c  lower() == "worl
-00005430: 6422 206f 7220 7370 6163 652e 6c6f 7765  d" or space.lowe
-00005440: 7228 2920 3d3d 2022 7068 7973 6963 616c  r() == "physical
-00005450: 223a 2074 6166 6669 6e65 203d 2062 742e  ": taffine = bt.
-00005460: 696e 7628 7461 7267 6574 5f61 6666 696e  inv(target_affin
-00005470: 6529 3b20 7361 6666 696e 6520 3d20 736f  e); saffine = so
-00005480: 7572 6365 5f61 6666 696e 650a 2020 2020  urce_affine.    
-00005490: 2020 2020 656c 6966 2073 7061 6365 2e6c      elif space.l
-000054a0: 6f77 6572 2829 203d 3d20 2269 6d61 6765  ower() == "image
-000054b0: 2220 6f72 2073 7061 6365 2e6c 6f77 6572  " or space.lower
-000054c0: 2829 203d 3d20 2269 6e64 6578 223a 2074  () == "index": t
-000054d0: 6166 6669 6e65 203d 2074 6172 6765 745f  affine = target_
-000054e0: 6166 6669 6e65 3b20 7361 6666 696e 6520  affine; saffine 
-000054f0: 3d20 6274 2e69 6e76 2873 6f75 7263 655f  = bt.inv(source_
-00005500: 6166 6669 6e65 290a 2020 2020 2020 2020  affine).        
-00005510: 656c 7365 3a20 7261 6973 6520 5479 7065  else: raise Type
-00005520: 4572 726f 7228 2249 6e76 616c 6964 2073  Error("Invalid s
-00005530: 7061 6365 2066 6f72 206d 6574 686f 6420  pace for method 
-00005540: 2774 6f27 2c20 7573 6520 2777 6f72 6c64  'to', use 'world
-00005550: 272f 2770 6879 7369 6361 6c27 206f 7220  '/'physical' or 
-00005560: 2769 6d61 6765 272f 2769 6e64 6578 2720  'image'/'index' 
-00005570: 696e 7374 6561 642e 2229 0a20 2020 2020  instead.").     
-00005580: 2020 2072 6574 7572 6e20 436f 6d70 6f73     return Compos
-00005590: 6564 5472 616e 7366 6f72 6d61 7469 6f6e  edTransformation
-000055a0: 2841 6666 696e 6528 7361 6666 696e 6529  (Affine(saffine)
-000055b0: 2c20 7365 6c66 2c20 4166 6669 6e65 2874  , self, Affine(t
-000055c0: 6166 6669 6e65 292c 206d 6f64 653d 2773  affine), mode='s
-000055d0: 7061 7469 616c 2729 0a20 2020 200a 2020  patial').    .  
-000055e0: 2020 6465 6620 6e75 6d5f 696e 7628 7365    def num_inv(se
-000055f0: 6c66 2c20 2a73 697a 652c 2076 6572 626f  lf, *size, verbo
-00005600: 7365 3d46 616c 7365 293a 0a20 2020 2020  se=False):.     
-00005610: 2020 2066 726f 6d20 2e66 756e 6373 2069     from .funcs i
-00005620: 6d70 6f72 7420 6265 6e64 696e 670a 2020  mport bending.  
-00005630: 2020 2020 2020 7369 7a65 203d 2061 7267        size = arg
-00005640: 5f74 7570 6c65 2873 697a 6529 0a20 2020  _tuple(size).   
-00005650: 2020 2020 2058 203d 2062 742e 696d 6167       X = bt.imag
-00005660: 655f 6772 6964 282a 7369 7a65 292e 756e  e_grid(*size).un
-00005670: 7371 7565 657a 6528 5b5d 292e 666c 6f61  squeeze([]).floa
-00005680: 7428 290a 2020 2020 2020 2020 696e 765f  t().        inv_
-00005690: 6469 7370 203d 202d 2073 656c 662e 746f  disp = - self.to
-000056a0: 5f44 4446 282a 7369 7a65 292e 636c 6f6e  _DDF(*size).clon
-000056b0: 6528 292e 6465 7461 6368 2829 0a20 2020  e().detach().   
-000056c0: 2020 2020 2069 6e76 5f64 6973 702e 7265       inv_disp.re
-000056d0: 7175 6972 6573 5f67 7261 6420 3d20 5472  quires_grad = Tr
-000056e0: 7565 0a20 2020 2020 2020 206f 7074 696d  ue.        optim
-000056f0: 697a 6572 203d 2062 742e 4341 4441 4d28  izer = bt.CADAM(
-00005700: 5b69 6e76 5f64 6973 705d 2c20 6c72 203d  [inv_disp], lr =
-00005710: 2031 652d 3229 0a20 2020 2020 2020 2070   1e-2).        p
-00005720: 7265 765f 6c6f 7373 203d 204e 6f6e 650a  rev_loss = None.
-00005730: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00005740: 2072 616e 6765 2834 3030 293a 0a20 2020   range(400):.   
-00005750: 2020 2020 2020 2020 2069 7472 616e 7320           itrans 
-00005760: 3d20 4465 6e73 6544 6973 706c 6163 656d  = DenseDisplacem
-00005770: 656e 7446 6965 6c64 2869 6e76 5f64 6973  entField(inv_dis
-00005780: 7029 0a20 2020 2020 2020 2020 2020 206c  p).            l
-00005790: 6f73 7320 3d20 2869 7472 616e 7328 7365  oss = (itrans(se
-000057a0: 6c66 2858 2929 202d 2058 292e 6e6f 726d  lf(X)) - X).norm
-000057b0: 3228 292e 6d65 616e 2829 202b 2031 652d  2().mean() + 1e-
-000057c0: 3120 2a20 6265 6e64 696e 6728 696e 765f  1 * bending(inv_
-000057d0: 6469 7370 290a 2020 2020 2020 2020 2020  disp).          
-000057e0: 2020 6f70 7469 6d69 7a65 722e 6d69 6e69    optimizer.mini
-000057f0: 6d69 7a65 286c 6f73 7329 2e73 7465 7028  mize(loss).step(
-00005800: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00005810: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
-00005820: 6622 6974 6572 6174 696f 6e20 7b69 2b31  f"iteration {i+1
-00005830: 7d3a 206c 6f73 7320 3d20 7b6c 6f73 732e  }: loss = {loss.
-00005840: 6974 656d 2829 7d22 290a 2020 2020 2020  item()}").      
-00005850: 2020 2020 2020 6966 2070 7265 765f 6c6f        if prev_lo
-00005860: 7373 2069 7320 6e6f 7420 4e6f 6e65 2061  ss is not None a
-00005870: 6e64 206c 6f73 732e 6974 656d 2829 203e  nd loss.item() >
-00005880: 3d20 7072 6576 5f6c 6f73 733a 206e 6f64  = prev_loss: nod
-00005890: 726f 705f 636f 756e 7420 2b3d 2031 0a20  rop_count += 1. 
-000058a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000058b0: 206e 6f64 726f 705f 636f 756e 7420 3d20   nodrop_count = 
-000058c0: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
-000058d0: 206e 6f64 726f 705f 636f 756e 7420 3e3d   nodrop_count >=
-000058e0: 2036 3a0a 2020 2020 2020 2020 2020 2020   6:.            
-000058f0: 2020 2020 6966 2076 6572 626f 7365 3a20      if verbose: 
-00005900: 7072 696e 7428 6622 5374 6f70 2061 7420  print(f"Stop at 
-00005910: 6974 6572 6174 696f 6e20 7b69 2b31 7d20  iteration {i+1} 
-00005920: 6475 6520 746f 206e 6f20 6472 6f70 7069  due to no droppi
-00005930: 6e67 2e20 2229 0a20 2020 2020 2020 2020  ng. ").         
-00005940: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00005950: 2020 2020 2020 2020 2069 6620 6c6f 7373           if loss
-00005960: 2e69 7465 6d28 2920 3c20 3165 2d33 3a0a  .item() < 1e-3:.
-00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005980: 6966 2076 6572 626f 7365 3a20 7072 696e  if verbose: prin
-00005990: 7428 6622 5374 6f70 2061 7420 6974 6572  t(f"Stop at iter
-000059a0: 6174 696f 6e20 7b69 2b31 7d20 6475 6520  ation {i+1} due 
-000059b0: 746f 2073 6d61 6c6c 206c 6f73 732e 2022  to small loss. "
-000059c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000059d0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-000059e0: 7265 7475 726e 2044 656e 7365 4469 7370  return DenseDisp
-000059f0: 6c61 6365 6d65 6e74 4669 656c 6428 696e  lacementField(in
-00005a00: 765f 6469 7370 290a 2020 2020 0a20 2020  v_disp).    .   
-00005a10: 2064 6566 2066 6f72 6365 5f69 6e76 2873   def force_inv(s
-00005a20: 656c 662c 202a 7369 7a65 293a 0a20 2020  elf, *size):.   
-00005a30: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00005a40: 7365 6c66 2c20 2769 6e76 2729 3a20 7265  self, 'inv'): re
-00005a50: 7475 726e 2073 656c 662e 696e 7628 290a  turn self.inv().
-00005a60: 2020 2020 2020 2020 656c 7365 3a20 7265          else: re
-00005a70: 7475 726e 2073 656c 662e 6e75 6d5f 696e  turn self.num_in
-00005a80: 7628 2a73 697a 6529 0a0a 4061 6c69 6173  v(*size)..@alias
-00005a90: 2822 4964 2229 0a63 6c61 7373 2049 6465  ("Id").class Ide
-00005aa0: 6e74 6974 7928 5370 6174 6961 6c54 7261  ntity(SpatialTra
-00005ab0: 6e73 666f 726d 6174 696f 6e29 3a0a 0a20  nsformation):.. 
-00005ac0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00005ad0: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
-00005ae0: 2727 0a20 2020 2020 2020 2049 6465 6e74  ''.        Ident
-00005af0: 6974 7920 7472 616e 7366 6f72 6d61 7469  ity transformati
-00005b00: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00005b10: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
-00005b20: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
-00005b30: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
-00005b40: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
-00005b50: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
-00005b60: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
-00005b70: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-00005b80: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
-00005b90: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
-00005ba0: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
-00005bb0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00005bc0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
-00005bd0: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
-00005be0: 6f72 6469 6e61 7465 732e 2028 5361 6d65  ordinates. (Same
-00005bf0: 2061 7320 5820 666f 7220 4964 656e 7469   as X for Identi
-00005c00: 7479 290a 2020 2020 2020 2020 2020 2020  ty).            
-00005c10: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00005c20: 7463 685d 2c20 7b6e 5f64 696d 7d2c 206e  tch], {n_dim}, n
-00005c30: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-00005c40: 7229 0a20 2020 2020 2020 2027 2727 0a20  r).        '''. 
-00005c50: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-00005c60: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
-00005c70: 2020 0a20 2020 2064 6566 2061 6666 696e    .    def affin
-00005c80: 6528 7365 6c66 2c20 6e5f 6469 6d3d 4e6f  e(self, n_dim=No
-00005c90: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-00005ca0: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
-00005cb0: 6574 7572 6e0a 2020 2020 2020 2020 7265  eturn.        re
-00005cc0: 7475 726e 2062 742e 6579 6528 6e5f 6469  turn bt.eye(n_di
-00005cd0: 6d20 2b20 3129 2e75 6e73 7175 6565 7a65  m + 1).unsqueeze
-00005ce0: 285b 5d29 0a0a 2020 2020 6465 6620 696e  ([])..    def in
-00005cf0: 7628 7365 6c66 293a 2072 6574 7572 6e20  v(self): return 
-00005d00: 4964 656e 7469 7479 2829 2e62 6163 6b77  Identity().backw
-00005d10: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
-00005d20: 7264 290a 0a63 6c61 7373 2052 6f74 6174  rd)..class Rotat
-00005d30: 696f 6e39 3028 5370 6174 6961 6c54 7261  ion90(SpatialTra
-00005d40: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
-00005d50: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00005d60: 656c 662c 2064 696d 312c 2064 696d 322c  elf, dim1, dim2,
-00005d70: 2069 6d61 6765 5f73 697a 653d 4e6f 6e65   image_size=None
-00005d80: 2c20 7265 7369 7a65 5f69 6d61 6765 3d54  , resize_image=T
-00005d90: 7275 6529 3a0a 2020 2020 2020 2020 2727  rue):.        ''
-00005da0: 270a 2020 2020 2020 2020 5472 616e 7366  '.        Transf
-00005db0: 6f72 6d61 7469 6f6e 2074 6861 7420 726f  ormation that ro
-00005dc0: 7461 7465 7320 616e 2069 6d61 6765 206f  tates an image o
-00005dd0: 6620 6069 6d61 6765 5f73 697a 6560 2062  f `image_size` b
-00005de0: 7920 3930 2064 6567 7265 6573 2e0a 2020  y 90 degrees..  
-00005df0: 2020 2020 2020 0a20 2020 2020 2020 204e        .        N
-00005e00: 6f74 653a 2054 6865 2072 6f74 6174 696f  ote: The rotatio
-00005e10: 6e20 6973 2066 6f72 2063 6f6f 7264 696e  n is for coordin
-00005e20: 6174 6573 2c20 6865 6e63 6520 7468 6520  ates, hence the 
-00005e30: 696d 6167 6520 726f 7461 7465 7320 636c  image rotates cl
-00005e40: 6f63 6b77 6973 652e 200a 2020 2020 2020  ockwise. .      
-00005e50: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00005e60: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-00005e70: 696d 312c 2064 696d 3220 5b69 6e74 5d3a  im1, dim2 [int]:
-00005e80: 2054 6865 2070 6c61 6e65 2077 6520 726f   The plane we ro
-00005e90: 7461 7465 206f 6e2e 2044 6972 6563 7469  tate on. Directi
-00005ea0: 6f6e 206f 6620 7468 6520 726f 7461 7469  on of the rotati
-00005eb0: 6f6e 2069 7320 6672 6f6d 2060 6469 6d31  on is from `dim1
-00005ec0: 6020 746f 2060 6469 6d32 602e 0a20 2020  ` to `dim2`..   
-00005ed0: 2020 2020 2020 2020 2020 2020 2069 2e65               i.e
-00005ee0: 2e20 636f 756e 7465 722d 636c 6f63 6b77  . counter-clockw
-00005ef0: 6973 6520 726f 7461 7469 6f6e 2077 6974  ise rotation wit
-00005f00: 6820 6469 6d31 2061 7320 782d 6178 6973  h dim1 as x-axis
-00005f10: 2061 6e64 2064 696d 3220 6173 2079 2d61   and dim2 as y-a
-00005f20: 7869 733a 205b 6469 6d31 2c20 6469 6d32  xis: [dim1, dim2
-00005f30: 5d20 636f 6f72 6469 6e61 7465 7320 2878  ] coordinates (x
-00005f40: 2c20 7929 2062 6563 6f6d 6573 2028 796d  , y) becomes (ym
-00005f50: 6178 2d79 2c20 7829 2e0a 2020 2020 2020  ax-y, x)..      
-00005f60: 2020 2020 2020 696d 6167 655f 7369 7a65        image_size
-00005f70: 205b 7475 706c 6520 6f72 2062 742e 5465   [tuple or bt.Te
-00005f80: 6e73 6f72 5d3a 2054 6865 2073 697a 6520  nsor]: The size 
-00005f90: 6f66 2074 6865 2069 6d61 6765 2c20 6f72  of the image, or
-00005fa0: 2074 6865 2069 6d61 6765 2069 7473 656c   the image itsel
-00005fb0: 662e 200a 2020 2020 2020 2020 2020 2020  f. .            
-00005fc0: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
-00005fd0: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
-00005fe0: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
-00005ff0: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
-00006000: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
-00006010: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
-00006020: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-00006030: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
-00006040: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
-00006050: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
-00006060: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00006070: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
-00006080: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
-00006090: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
-000060a0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-000060b0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
-000060c0: 6469 6d7d 2c20 6e5f 312c 206e 5f32 2c20  dim}, n_1, n_2, 
-000060d0: 2e2e 2e2c 206e 5f72 290a 2020 2020 2020  ..., n_r).      
-000060e0: 2020 2727 270a 2020 2020 2020 2020 7375    '''.        su
-000060f0: 7065 7228 292e 5f5f 696e 6974 5f5f 2864  per().__init__(d
-00006100: 696d 313d 6469 6d31 2c20 6469 6d32 3d64  im1=dim1, dim2=d
-00006110: 696d 322c 2069 6d61 6765 5f73 697a 653d  im2, image_size=
-00006120: 696d 6167 655f 7369 7a65 2c20 7265 7369  image_size, resi
-00006130: 7a65 5f69 6d61 6765 3d72 6573 697a 655f  ze_image=resize_
-00006140: 696d 6167 6529 0a0a 2020 2020 2020 2020  image)..        
-00006150: 7365 6c66 2e64 696d 312c 2073 656c 662e  self.dim1, self.
-00006160: 6469 6d32 203d 2064 696d 312c 2064 696d  dim2 = dim1, dim
-00006170: 320a 2020 2020 2020 2020 6966 2069 7369  2.        if isi
-00006180: 6e73 7461 6e63 6528 696d 6167 655f 7369  nstance(image_si
-00006190: 7a65 2c20 6274 2e74 6f72 6368 2e54 656e  ze, bt.torch.Ten
-000061a0: 736f 7229 3a20 696d 6167 655f 7369 7a65  sor): image_size
-000061b0: 203d 2069 6d61 6765 5f73 697a 652e 7368   = image_size.sh
-000061c0: 6170 650a 2020 2020 2020 2020 7365 6c66  ape.        self
-000061d0: 2e69 6d61 6765 5f73 697a 6520 3d20 696d  .image_size = im
-000061e0: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
-000061f0: 2069 6620 696d 6167 655f 7369 7a65 2069   if image_size i
-00006200: 7320 6e6f 7420 4e6f 6e65 3a20 7365 6c66  s not None: self
-00006210: 2e6e 5f64 696d 203d 206c 656e 2869 6d61  .n_dim = len(ima
-00006220: 6765 5f73 697a 6529 0a20 2020 2020 2020  ge_size).       
-00006230: 2069 6620 7265 7369 7a65 5f69 6d61 6765   if resize_image
-00006240: 3a20 7365 6c66 2e72 6573 6861 7065 203d  : self.reshape =
-00006250: 205b 2831 2c29 2c20 2864 696d 312c 2064   [(1,), (dim1, d
-00006260: 696d 3229 5d0a 0a20 2020 2064 6566 205f  im2)]..    def _
-00006270: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
-00006280: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
-00006290: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
-000062a0: 290a 2020 2020 2020 2020 6469 6d31 2c20  ).        dim1, 
-000062b0: 6469 6d32 203d 2073 656c 662e 6469 6d31  dim2 = self.dim1
-000062c0: 2c20 7365 6c66 2e64 696d 320a 2020 2020  , self.dim2.    
-000062d0: 2020 2020 7365 6c65 6374 3120 3d20 2873      select1 = (s
-000062e0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
-000062f0: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
-00006300: 6469 6d31 2c29 0a20 2020 2020 2020 2073  dim1,).        s
-00006310: 656c 6563 7432 203d 2028 736c 6963 6528  elect2 = (slice(
-00006320: 4e6f 6e65 292c 2920 2a20 582e 6368 616e  None),) * X.chan
-00006330: 6e65 6c5f 6469 6d20 2b20 2864 696d 322c  nel_dim + (dim2,
-00006340: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00006350: 662e 696d 6167 655f 7369 7a65 2069 7320  f.image_size is 
-00006360: 4e6f 6e65 3a20 6d61 785f 7261 6e67 6520  None: max_range 
-00006370: 3d20 585b 7365 6c65 6374 325d 2e6d 6178  = X[select2].max
-00006380: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-00006390: 206d 6178 5f72 616e 6765 203d 2073 656c   max_range = sel
-000063a0: 662e 696d 6167 655f 7369 7a65 5b64 696d  f.image_size[dim
-000063b0: 325d 0a20 2020 2020 2020 2058 5b73 656c  2].        X[sel
-000063c0: 6563 7431 5d20 3d20 585b 7365 6c65 6374  ect1] = X[select
-000063d0: 315d 202b 206d 6178 5f72 616e 6765 202d  1] + max_range -
-000063e0: 2058 5b73 656c 6563 7432 5d0a 2020 2020   X[select2].    
-000063f0: 2020 2020 585b 7365 6c65 6374 325d 203d      X[select2] =
-00006400: 2058 5b73 656c 6563 7431 5d20 2b20 585b   X[select1] + X[
-00006410: 7365 6c65 6374 325d 202d 206d 6178 5f72  select2] - max_r
-00006420: 616e 6765 0a20 2020 2020 2020 2058 5b73  ange.        X[s
-00006430: 656c 6563 7431 5d20 3d20 585b 7365 6c65  elect1] = X[sele
-00006440: 6374 315d 202d 2058 5b73 656c 6563 7432  ct1] - X[select2
-00006450: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-00006460: 2058 0a20 2020 2020 2020 200a 2020 2020   X.        .    
-00006470: 6465 6620 6166 6669 6e65 2873 656c 662c  def affine(self,
-00006480: 206e 5f64 696d 3d4e 6f6e 6529 3a0a 2020   n_dim=None):.  
-00006490: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
-000064a0: 6167 655f 7369 7a65 2069 7320 4e6f 6e65  age_size is None
-000064b0: 3a20 7265 7475 726e 0a20 2020 2020 2020  : return.       
-000064c0: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
-000064d0: 6520 616e 6420 7365 6c66 2e6e 5f64 696d  e and self.n_dim
-000064e0: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
-000064f0: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
-00006500: 6d20 6973 204e 6f6e 653a 206e 5f64 696d  m is None: n_dim
-00006510: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
-00006520: 2020 2020 2020 6176 6f75 6368 2873 656c        avouch(sel
-00006530: 662e 6e5f 6469 6d20 6973 204e 6f6e 6520  f.n_dim is None 
-00006540: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
-00006550: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
-00006560: 6469 6d31 2c20 6469 6d32 203d 2073 656c  dim1, dim2 = sel
-00006570: 662e 6469 6d31 2c20 7365 6c66 2e64 696d  f.dim1, self.dim
-00006580: 320a 2020 2020 2020 2020 6166 6620 3d20  2.        aff = 
-00006590: 6274 2e65 7965 286e 5f64 696d 202b 2031  bt.eye(n_dim + 1
-000065a0: 290a 2020 2020 2020 2020 6166 665b 6469  ).        aff[di
-000065b0: 6d31 5d5b 6469 6d31 5d20 3d20 302e 0a20  m1][dim1] = 0.. 
-000065c0: 2020 2020 2020 2061 6666 5b64 696d 315d         aff[dim1]
-000065d0: 5b64 696d 325d 203d 202d 312e 0a20 2020  [dim2] = -1..   
-000065e0: 2020 2020 2061 6666 5b64 696d 315d 5b2d       aff[dim1][-
-000065f0: 315d 203d 2066 6c6f 6174 2873 656c 662e  1] = float(self.
-00006600: 696d 6167 655f 7369 7a65 5b64 696d 325d  image_size[dim2]
-00006610: 290a 2020 2020 2020 2020 6166 665b 6469  ).        aff[di
-00006620: 6d32 5d5b 6469 6d32 5d20 3d20 302e 0a20  m2][dim2] = 0.. 
-00006630: 2020 2020 2020 2061 6666 5b64 696d 325d         aff[dim2]
-00006640: 5b64 696d 315d 203d 2031 2e0a 2020 2020  [dim1] = 1..    
-00006650: 2020 2020 7265 7475 726e 2061 6666 2e75      return aff.u
-00006660: 6e73 7175 6565 7a65 285b 5d29 0a20 2020  nsqueeze([]).   
-00006670: 200a 2020 2020 6465 6620 696e 7628 7365   .    def inv(se
-00006680: 6c66 293a 2072 6574 7572 6e20 526f 7461  lf): return Rota
-00006690: 7469 6f6e 3237 3028 7365 6c66 2e64 696d  tion270(self.dim
-000066a0: 312c 2073 656c 662e 6469 6d32 2c20 696d  1, self.dim2, im
-000066b0: 6167 655f 7369 7a65 203d 2073 656c 662e  age_size = self.
-000066c0: 696d 6167 655f 7369 7a65 2c20 7265 7369  image_size, resi
-000066d0: 7a65 5f69 6d61 6765 203d 2073 656c 662e  ze_image = self.
-000066e0: 7265 7369 7a65 5f69 6d61 6765 292e 6261  resize_image).ba
-000066f0: 636b 7761 7264 5f28 7365 6c66 2e62 6163  ckward_(self.bac
-00006700: 6b77 6172 6429 0a0a 636c 6173 7320 526f  kward)..class Ro
-00006710: 7461 7469 6f6e 3237 3028 5370 6174 6961  tation270(Spatia
-00006720: 6c54 7261 6e73 666f 726d 6174 696f 6e29  lTransformation)
-00006730: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00006740: 5f5f 2873 656c 662c 2064 696d 312c 2064  __(self, dim1, d
-00006750: 696d 322c 2069 6d61 6765 5f73 697a 653d  im2, image_size=
-00006760: 4e6f 6e65 2c20 7265 7369 7a65 5f69 6d61  None, resize_ima
-00006770: 6765 3d54 7275 6529 3a0a 2020 2020 2020  ge=True):.      
-00006780: 2020 2727 270a 2020 2020 2020 2020 5472    '''.        Tr
-00006790: 616e 7366 6f72 6d61 7469 6f6e 2074 6861  ansformation tha
-000067a0: 7420 726f 7461 7465 7320 616e 2069 6d61  t rotates an ima
-000067b0: 6765 2062 7920 3237 3020 6465 6772 6565  ge by 270 degree
-000067c0: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-000067d0: 2020 2020 4e6f 7465 3a20 5468 6520 726f      Note: The ro
-000067e0: 7461 7469 6f6e 2069 7320 666f 7220 636f  tation is for co
-000067f0: 6f72 6469 6e61 7465 732c 2068 656e 6365  ordinates, hence
-00006800: 2074 6865 2069 6d61 6765 2072 6f74 6174   the image rotat
-00006810: 6573 2063 6c6f 636b 7769 7365 2e20 0a20  es clockwise. . 
-00006820: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006830: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-00006840: 2020 2020 6469 6d31 2c20 6469 6d32 205b      dim1, dim2 [
-00006850: 696e 745d 3a20 5468 6520 706c 616e 6520  int]: The plane 
-00006860: 7765 2072 6f74 6174 6520 6f6e 2e20 4469  we rotate on. Di
-00006870: 7265 6374 696f 6e20 6f66 2074 6865 2072  rection of the r
-00006880: 6f74 6174 696f 6e20 6973 2066 726f 6d20  otation is from 
-00006890: 6064 696d 3160 2074 6f20 6064 696d 3260  `dim1` to `dim2`
-000068a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000068b0: 2020 692e 652e 2063 6f75 6e74 6572 2d63    i.e. counter-c
-000068c0: 6c6f 636b 7769 7365 2072 6f74 6174 696f  lockwise rotatio
-000068d0: 6e20 7769 7468 2064 696d 3120 6173 2078  n with dim1 as x
-000068e0: 2d61 7869 7320 616e 6420 6469 6d32 2061  -axis and dim2 a
-000068f0: 7320 792d 6178 6973 3a20 5b64 696d 312c  s y-axis: [dim1,
-00006900: 2064 696d 325d 2063 6f6f 7264 696e 6174   dim2] coordinat
-00006910: 6573 2028 782c 2079 2920 6265 636f 6d65  es (x, y) become
-00006920: 7320 2879 2c20 786d 6178 2d78 292e 0a20  s (y, xmax-x).. 
-00006930: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-00006940: 5f73 697a 6520 5b74 7570 6c65 206f 7220  _size [tuple or 
-00006950: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-00006960: 7369 7a65 206f 6620 7468 6520 696d 6167  size of the imag
-00006970: 652c 206f 7220 7468 6520 696d 6167 6520  e, or the image 
-00006980: 6974 7365 6c66 2e20 0a20 2020 2020 2020  itself. .       
-00006990: 2020 2020 200a 2020 2020 2020 2020 5768       .        Wh
-000069a0: 656e 2069 7420 6973 2063 616c 6c65 643a  en it is called:
-000069b0: 0a20 2020 2020 2020 2020 2020 2058 205b  .            X [
-000069c0: 6274 2e54 656e 736f 725d 3a20 436f 6f72  bt.Tensor]: Coor
-000069d0: 6469 6e61 7465 7320 746f 2062 6520 7472  dinates to be tr
-000069e0: 616e 7366 6f72 6d65 642e 0a20 2020 2020  ansformed..     
-000069f0: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00006a00: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00006a10: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
-00006a20: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-00006a30: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
-00006a40: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
-00006a50: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
-00006a60: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-00006a90: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
-00006aa0: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
-00006ab0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00006ac0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00006ad0: 745f 5f28 6469 6d31 3d64 696d 312c 2064  t__(dim1=dim1, d
-00006ae0: 696d 323d 6469 6d32 2c20 696d 6167 655f  im2=dim2, image_
-00006af0: 7369 7a65 3d69 6d61 6765 5f73 697a 652c  size=image_size,
-00006b00: 2072 6573 697a 655f 696d 6167 653d 7265   resize_image=re
-00006b10: 7369 7a65 5f69 6d61 6765 290a 0a20 2020  size_image)..   
-00006b20: 2020 2020 2073 656c 662e 6469 6d31 2c20       self.dim1, 
-00006b30: 7365 6c66 2e64 696d 3220 3d20 6469 6d31  self.dim2 = dim1
-00006b40: 2c20 6469 6d32 0a20 2020 2020 2020 2069  , dim2.        i
-00006b50: 6620 6973 696e 7374 616e 6365 2869 6d61  f isinstance(ima
-00006b60: 6765 5f73 697a 652c 2062 742e 746f 7263  ge_size, bt.torc
-00006b70: 682e 5465 6e73 6f72 293a 2069 6d61 6765  h.Tensor): image
-00006b80: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
-00006b90: 7a65 2e73 6861 7065 0a20 2020 2020 2020  ze.shape.       
-00006ba0: 2073 656c 662e 696d 6167 655f 7369 7a65   self.image_size
-00006bb0: 203d 2069 6d61 6765 5f73 697a 650a 2020   = image_size.  
-00006bc0: 2020 2020 2020 6966 2069 6d61 6765 5f73        if image_s
-00006bd0: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
-00006be0: 2073 656c 662e 6e5f 6469 6d20 3d20 6c65   self.n_dim = le
-00006bf0: 6e28 696d 6167 655f 7369 7a65 290a 2020  n(image_size).  
-00006c00: 2020 2020 2020 6966 2072 6573 697a 655f        if resize_
-00006c10: 696d 6167 653a 2073 656c 662e 7265 7368  image: self.resh
-00006c20: 6170 6520 3d20 5b28 312c 292c 2028 6469  ape = [(1,), (di
-00006c30: 6d31 2c20 6469 6d32 295d 0a0a 2020 2020  m1, dim2)]..    
-00006c40: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00006c50: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
-00006c60: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
-00006c70: 6c5f 5f28 5829 0a20 2020 2020 2020 2064  l__(X).        d
-00006c80: 696d 312c 2064 696d 3220 3d20 7365 6c66  im1, dim2 = self
-00006c90: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
-00006ca0: 0a20 2020 2020 2020 2073 656c 6563 7431  .        select1
-00006cb0: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
-00006cc0: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
-00006cd0: 6d20 2b20 2864 696d 312c 290a 2020 2020  m + (dim1,).    
-00006ce0: 2020 2020 7365 6c65 6374 3220 3d20 2873      select2 = (s
-00006cf0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
-00006d00: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
-00006d10: 6469 6d32 2c29 0a20 2020 2020 2020 2069  dim2,).        i
-00006d20: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
-00006d30: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
-00006d40: 616e 6765 203d 2058 5b73 656c 6563 7431  ange = X[select1
-00006d50: 5d2e 6d61 7828 290a 2020 2020 2020 2020  ].max().        
-00006d60: 656c 7365 3a20 6d61 785f 7261 6e67 6520  else: max_range 
-00006d70: 3d20 7365 6c66 2e69 6d61 6765 5f73 697a  = self.image_siz
-00006d80: 655b 6469 6d31 5d0a 2020 2020 2020 2020  e[dim1].        
-00006d90: 585b 7365 6c65 6374 325d 203d 2058 5b73  X[select2] = X[s
-00006da0: 656c 6563 7432 5d20 2b20 6d61 785f 7261  elect2] + max_ra
-00006db0: 6e67 6520 2d20 585b 7365 6c65 6374 315d  nge - X[select1]
-00006dc0: 0a20 2020 2020 2020 2058 5b73 656c 6563  .        X[selec
-00006dd0: 7431 5d20 3d20 585b 7365 6c65 6374 325d  t1] = X[select2]
-00006de0: 202b 2058 5b73 656c 6563 7431 5d20 2d20   + X[select1] - 
-00006df0: 6d61 785f 7261 6e67 650a 2020 2020 2020  max_range.      
-00006e00: 2020 585b 7365 6c65 6374 325d 203d 2058    X[select2] = X
-00006e10: 5b73 656c 6563 7432 5d20 2d20 585b 7365  [select2] - X[se
-00006e20: 6c65 6374 315d 0a20 2020 2020 2020 2072  lect1].        r
-00006e30: 6574 7572 6e20 580a 2020 2020 2020 2020  eturn X.        
-00006e40: 0a20 2020 2064 6566 2061 6666 696e 6528  .    def affine(
-00006e50: 7365 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65  self, n_dim=None
-00006e60: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00006e70: 6c66 2e69 6d61 6765 5f73 697a 6520 6973  lf.image_size is
-00006e80: 204e 6f6e 653a 2072 6574 7572 6e0a 2020   None: return.  
-00006e90: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
-00006ea0: 7320 4e6f 6e65 2061 6e64 2073 656c 662e  s None and self.
-00006eb0: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
+00004520: 5f6c 6973 742e 6170 7065 6e64 2874 293b  _list.append(t);
+00004530: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00004540: 2020 2020 2020 6166 6620 3d20 742e 6166        aff = t.af
+00004550: 6669 6e65 286e 5f64 696d 290a 2020 2020  fine(n_dim).    
+00004560: 2020 2020 2020 2020 6966 2061 6666 2069          if aff i
+00004570: 7320 4e6f 6e65 2061 6e64 2063 7572 5f61  s None and cur_a
+00004580: 6666 696e 6520 6973 206e 6f74 204e 6f6e  ffine is not Non
+00004590: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000045a0: 2020 206f 7574 5f6c 6973 742e 6578 7465     out_list.exte
+000045b0: 6e64 285b 4166 6669 6e65 2863 7572 5f61  nd([Affine(cur_a
+000045c0: 6666 696e 6529 2c20 745d 290a 2020 2020  ffine), t]).    
+000045d0: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
+000045e0: 6166 6669 6e65 203d 204e 6f6e 650a 2020  affine = None.  
+000045f0: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+00004600: 6666 2069 7320 4e6f 6e65 3a20 6f75 745f  ff is None: out_
+00004610: 6c69 7374 2e61 7070 656e 6428 7429 0a20  list.append(t). 
+00004620: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00004630: 6166 662e 7370 6163 6520 213d 2028 6e5f  aff.space != (n_
+00004640: 6469 6d2b 312c 206e 5f64 696d 2b31 293a  dim+1, n_dim+1):
+00004650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004660: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00004670: 2866 2255 6e63 6f6e 7369 7374 656e 7420  (f"Unconsistent 
+00004680: 7472 616e 7366 6f72 6d61 7469 6f6e 2077  transformation w
+00004690: 6974 6820 6166 6669 6e65 206f 6620 7369  ith affine of si
+000046a0: 7a65 207b 6166 662e 7370 6163 657d 2069  ze {aff.space} i
+000046b0: 6e20 436f 6d70 6f73 6564 5472 616e 7366  n ComposedTransf
+000046c0: 6f72 6d61 7469 6f6e 2e20 2229 0a20 2020  ormation. ").   
+000046d0: 2020 2020 2020 2020 2065 6c69 6620 6375           elif cu
+000046e0: 725f 6166 6669 6e65 2069 7320 4e6f 6e65  r_affine is None
+000046f0: 3a20 6375 725f 6166 6669 6e65 203d 2061  : cur_affine = a
+00004700: 6666 0a20 2020 2020 2020 2020 2020 2065  ff.            e
+00004710: 6c73 653a 2063 7572 5f61 6666 696e 6520  lse: cur_affine 
+00004720: 3d20 6375 725f 6166 6669 6e65 2040 2061  = cur_affine @ a
+00004730: 6666 0a20 2020 2020 2020 2069 6620 6375  ff.        if cu
+00004740: 725f 6166 6669 6e65 2069 7320 6e6f 7420  r_affine is not 
+00004750: 4e6f 6e65 3a20 6f75 745f 6c69 7374 2e61  None: out_list.a
+00004760: 7070 656e 6428 4166 6669 6e65 2863 7572  ppend(Affine(cur
+00004770: 5f61 6666 696e 6529 290a 2020 2020 2020  _affine)).      
+00004780: 2020 7265 7475 726e 2043 6f6d 706f 7365    return Compose
+00004790: 6454 7261 6e73 666f 726d 6174 696f 6e28  dTransformation(
+000047a0: 2a6f 7574 5f6c 6973 742c 206d 6f64 6520  *out_list, mode 
+000047b0: 3d20 7365 6c66 2e6d 6f64 6529 0a0a 2020  = self.mode)..  
+000047c0: 2020 6465 6620 746f 5f64 6963 7428 7365    def to_dict(se
+000047d0: 6c66 293a 0a20 2020 2020 2020 2064 6963  lf):.        dic
+000047e0: 203d 2073 7570 6572 2829 2e74 6f5f 6469   = super().to_di
+000047f0: 6374 2829 0a20 2020 2020 2020 2064 6963  ct().        dic
+00004800: 5b27 7472 616e 735f 6c69 7374 275d 203d  ['trans_list'] =
+00004810: 205b 742e 746f 5f64 6963 7428 2920 666f   [t.to_dict() fo
+00004820: 7220 7420 696e 2073 656c 662e 7472 616e  r t in self.tran
+00004830: 735f 6c69 7374 5d0a 2020 2020 2020 2020  s_list].        
+00004840: 7265 7475 726e 2064 6963 0a0a 2323 2323  return dic..####
+00004850: 2323 2323 2323 2320 5370 6174 6961 6c20  ####### Spatial 
+00004860: 5472 616e 7366 6f72 6d61 7469 6f6e 7320  Transformations 
+00004870: 2323 2323 2323 2323 2323 230a 0a63 6c61  ###########..cla
+00004880: 7373 2053 7061 7469 616c 5472 616e 7366  ss SpatialTransf
+00004890: 6f72 6d61 7469 6f6e 2854 7261 6e73 666f  ormation(Transfo
+000048a0: 726d 6174 696f 6e29 3a0a 2020 2020 0a20  rmation):.    . 
+000048b0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000048c0: 7365 6c66 2c20 2a70 6172 616d 732c 202a  self, *params, *
+000048d0: 2a6b 7770 6172 616d 7329 3a0a 2020 2020  *kwparams):.    
+000048e0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+000048f0: 6974 5f5f 282a 7061 7261 6d73 2c20 2a2a  it__(*params, **
+00004900: 6b77 7061 7261 6d73 290a 2020 2020 2020  kwparams).      
+00004910: 2020 7365 6c66 2e62 6163 6b77 6172 6420    self.backward 
+00004920: 3d20 5472 7565 0a20 2020 2020 2020 200a  = True.        .
+00004930: 2020 2020 6465 6620 5f5f 6361 6c6c 5f5f      def __call__
+00004940: 2873 656c 662c 2058 293a 0a20 2020 2020  (self, X):.     
+00004950: 2020 2022 2222 0a20 2020 2020 2020 2058     """.        X
+00004960: 205b 6274 2e54 656e 736f 725d 3a20 436f   [bt.Tensor]: Co
+00004970: 6f72 6469 6e61 7465 7320 746f 2062 6520  ordinates to be 
+00004980: 7472 616e 7366 6f72 6d65 642e 0a20 2020  transformed..   
+00004990: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+000049a0: 5b6e 5f62 6174 6368 3a20 6f70 7469 6f6e  [n_batch: option
+000049b0: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  al], {n_dim}, n_
+000049c0: 312c 206e 5f32 2c20 2e2e 2e2c 206e 5f72  1, n_2, ..., n_r
+000049d0: 290a 2020 2020 2020 2020 6f75 7470 7574  ).        output
+000049e0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+000049f0: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
+00004a00: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
+00004a10: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00004a20: 5f62 6174 6368 5d2c 207b 6e5f 6469 6d7d  _batch], {n_dim}
+00004a30: 2c20 6e5f 312c 206e 5f32 2c20 2e2e 2e2c  , n_1, n_2, ...,
+00004a40: 206e 5f72 290a 2020 2020 2020 2020 2222   n_r).        ""
+00004a50: 220a 2020 2020 2020 2020 6176 6f75 6368  ".        avouch
+00004a60: 2858 2e68 6173 5f63 6861 6e6e 656c 2c20  (X.has_channel, 
+00004a70: 6622 506c 6561 7365 2075 7365 2062 6174  f"Please use bat
+00004a80: 6f72 6368 2074 656e 736f 7220 6f66 2073  orch tensor of s
+00004a90: 697a 6520 5c0a 2020 2020 2020 2020 2020  ize \.          
+00004aa0: 2020 285b 6e5f 6261 7463 683a 6f70 7469    ([n_batch:opti
+00004ab0: 6f6e 616c 5d2c 207b 7b6e 5f64 696d 7d7d  onal], {{n_dim}}
+00004ac0: 2c20 6e5f 312c 206e 5f32 2c20 2e2e 2e2c  , n_1, n_2, ...,
+00004ad0: 206e 5f72 2920 5c0a 2020 2020 2020 2020   n_r) \.        
+00004ae0: 2020 2020 2020 2020 666f 7220 7b73 656c          for {sel
+00004af0: 662e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  f.__class__.__na
+00004b00: 6d65 5f5f 2e73 706c 6974 2827 2e27 295b  me__.split('.')[
+00004b10: 2d31 5d7d 2054 7261 6e73 666f 726d 6174  -1]} Transformat
+00004b20: 696f 6e2c 2069 6e73 7465 6164 206f 6620  ion, instead of 
+00004b30: 7b58 2e73 6861 7065 7d2e 2022 290a 2020  {X.shape}. ").  
+00004b40: 2020 2020 2020 6966 2073 656c 662e 6e5f        if self.n_
+00004b50: 6469 6d20 6973 206e 6f74 204e 6f6e 653a  dim is not None:
+00004b60: 0a20 2020 2020 2020 2020 2020 2061 766f  .            avo
+00004b70: 7563 6828 582e 6e5f 6368 616e 6e65 6c20  uch(X.n_channel 
+00004b80: 3d3d 2073 656c 662e 6e5f 6469 6d2c 2066  == self.n_dim, f
+00004b90: 227b 7365 6c66 2e6e 5f64 696d 7d44 207b  "{self.n_dim}D {
+00004ba0: 7365 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f  self.__class__._
+00004bb0: 5f6e 616d 655f 5f2e 7370 6c69 7428 272e  _name__.split('.
+00004bc0: 2729 5b2d 315d 7d20 5472 616e 7366 6f72  ')[-1]} Transfor
+00004bd0: 6d61 7469 6f6e 205c 0a20 2020 2020 2020  mation \.       
+00004be0: 2020 2020 2020 2020 2064 6f65 7320 6e6f           does no
+00004bf0: 7420 7461 6b65 2063 6f6f 7264 696e 6174  t take coordinat
+00004c00: 6573 206f 6620 7369 7a65 207b 582e 7368  es of size {X.sh
+00004c10: 6170 657d 2229 0a20 2020 2020 2020 2069  ape}").        i
+00004c20: 6620 582e 6861 735f 6261 7463 683a 2061  f X.has_batch: a
+00004c30: 766f 7563 6828 7365 6c66 2e6e 5f62 6174  vouch(self.n_bat
+00004c40: 6368 2069 7320 4e6f 6e65 206f 7220 7365  ch is None or se
+00004c50: 6c66 2e6e 5f62 6174 6368 203d 3d20 3120  lf.n_batch == 1 
+00004c60: 6f72 2058 2e6e 5f62 6174 6368 203d 3d20  or X.n_batch == 
+00004c70: 3120 6f72 2058 2e6e 5f62 6174 6368 203d  1 or X.n_batch =
+00004c80: 3d20 7365 6c66 2e6e 5f62 6174 6368 2c20  = self.n_batch, 
+00004c90: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
+00004ca0: 7365 6c66 2e6e 5f64 696d 7d44 207b 7365  self.n_dim}D {se
+00004cb0: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+00004cc0: 616d 655f 5f2e 7370 6c69 7428 272e 2729  ame__.split('.')
+00004cd0: 5b2d 315d 7d20 5472 616e 7366 6f72 6d61  [-1]} Transforma
+00004ce0: 7469 6f6e 2077 6974 6820 6261 7463 6820  tion with batch 
+00004cf0: 7369 7a65 207b 7365 6c66 2e6e 5f62 6174  size {self.n_bat
+00004d00: 6368 7d20 5c0a 2020 2020 2020 2020 2020  ch} \.          
+00004d10: 2020 2020 2020 646f 6573 206e 6f74 2074        does not t
+00004d20: 616b 6520 636f 6f72 6469 6e61 7465 7320  ake coordinates 
+00004d30: 7769 7468 2077 726f 6e67 2062 6174 6368  with wrong batch
+00004d40: 2073 697a 652e 2043 7572 7265 6e74 2073   size. Current s
+00004d50: 697a 653a 207b 582e 7368 6170 657d 2e22  ize: {X.shape}."
+00004d60: 290a 2020 2020 2020 2020 5920 3d20 582e  ).        Y = X.
+00004d70: 666c 6f61 7428 292e 636c 6f6e 6528 290a  float().clone().
+00004d80: 2020 2020 2020 2020 6966 206e 6f74 2059          if not Y
+00004d90: 2e68 6173 5f62 6174 6368 3a0a 2020 2020  .has_batch:.    
+00004da0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00004db0: 6e5f 6261 7463 6820 6973 206e 6f74 204e  n_batch is not N
+00004dc0: 6f6e 653a 2059 203d 2059 2e6d 756c 7469  one: Y = Y.multi
+00004dd0: 706c 7928 7365 6c66 2e6e 5f62 6174 6368  ply(self.n_batch
+00004de0: 2c20 5b5d 290a 2020 2020 2020 2020 2020  , []).          
+00004df0: 2020 656c 7365 3a20 5920 3d20 592e 756e    else: Y = Y.un
+00004e00: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
+00004e10: 2020 2020 7265 7475 726e 2059 0a0a 2020      return Y..  
+00004e20: 2020 6465 6620 5f5f 6d61 746d 756c 5f5f    def __matmul__
+00004e30: 2878 2c20 7929 3a0a 2020 2020 2020 2020  (x, y):.        
+00004e40: 6966 2069 735f 7370 6174 6961 6c5f 7472  if is_spatial_tr
+00004e50: 616e 7366 6f72 6d61 7469 6f6e 2878 2920  ansformation(x) 
+00004e60: 616e 6420 6973 5f73 7061 7469 616c 5f74  and is_spatial_t
+00004e70: 7261 6e73 666f 726d 6174 696f 6e28 7929  ransformation(y)
+00004e80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004e90: 7475 726e 2043 6f6d 706f 7365 6454 7261  turn ComposedTra
+00004ea0: 6e73 666f 726d 6174 696f 6e28 782c 2079  nsformation(x, y
+00004eb0: 2c20 6d6f 6465 3d22 7370 6174 6961 6c22  , mode="spatial"
+00004ec0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004ed0: 2043 6f6d 706f 7365 6454 7261 6e73 666f   ComposedTransfo
+00004ee0: 726d 6174 696f 6e28 782c 2079 290a 2020  rmation(x, y).  
+00004ef0: 2020 0a20 2020 2064 6566 2061 6666 696e    .    def affin
+00004f00: 6528 7365 6c66 2c20 6e5f 6469 6d3d 4e6f  e(self, n_dim=No
+00004f10: 6e65 293a 0a20 2020 2020 2020 2072 6574  ne):.        ret
+00004f20: 7572 6e20 4e6f 6e65 0a20 2020 200a 2020  urn None.    .  
+00004f30: 2020 4061 6c69 6173 2827 746f 4444 4627    @alias('toDDF'
+00004f40: 290a 2020 2020 6465 6620 746f 5f44 4446  ).    def to_DDF
+00004f50: 2873 656c 662c 202a 7368 6170 6529 3a0a  (self, *shape):.
+00004f60: 2020 2020 2020 2020 7368 6170 6520 3d20          shape = 
+00004f70: 6172 675f 7475 706c 6528 7368 6170 6529  arg_tuple(shape)
+00004f80: 0a20 2020 2020 2020 2067 7269 6420 3d20  .        grid = 
+00004f90: 6274 2e69 6d61 6765 5f67 7269 6428 2a73  bt.image_grid(*s
+00004fa0: 6861 7065 292e 756e 7371 7565 657a 6528  hape).unsqueeze(
+00004fb0: 5b5d 292e 666c 6f61 7428 290a 2020 2020  []).float().    
+00004fc0: 2020 2020 7265 7475 726e 2073 656c 6628      return self(
+00004fd0: 6772 6964 2920 2d20 6772 6964 0a0a 2020  grid) - grid..  
+00004fe0: 2020 6465 6620 746f 5f69 6d61 6765 5f73    def to_image_s
+00004ff0: 7061 6365 2873 656c 662c 2073 6f75 7263  pace(self, sourc
+00005000: 652c 2074 6172 6765 7429 3a0a 2020 2020  e, target):.    
+00005010: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00005020: 6528 736f 7572 6365 2c20 7374 7229 3a20  e(source, str): 
+00005030: 736f 7572 6365 203d 2049 4d47 2873 6f75  source = IMG(sou
+00005040: 7263 6529 0a20 2020 2020 2020 2069 6620  rce).        if 
+00005050: 6973 696e 7374 616e 6365 2874 6172 6765  isinstance(targe
+00005060: 742c 2073 7472 293a 2074 6172 6765 7420  t, str): target 
+00005070: 3d20 494d 4728 7461 7267 6574 290a 2020  = IMG(target).  
+00005080: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00005090: 6e63 6528 736f 7572 6365 2c20 494d 4729  nce(source, IMG)
+000050a0: 3a20 736f 7572 6365 203d 2073 6f75 7263  : source = sourc
+000050b0: 652e 6166 6669 6e65 0a20 2020 2020 2020  e.affine.       
+000050c0: 2069 6620 6973 696e 7374 616e 6365 2874   if isinstance(t
+000050d0: 6172 6765 742c 2049 4d47 293a 2074 6172  arget, IMG): tar
+000050e0: 6765 7420 3d20 7461 7267 6574 2e61 6666  get = target.aff
+000050f0: 696e 650a 2020 2020 2020 2020 7265 7475  ine.        retu
+00005100: 726e 2073 656c 662e 746f 2827 696d 6167  rn self.to('imag
+00005110: 6527 2c20 736f 7572 6365 5f61 6666 696e  e', source_affin
+00005120: 653d 736f 7572 6365 2c20 7461 7267 6574  e=source, target
+00005130: 5f61 6666 696e 653d 7461 7267 6574 290a  _affine=target).
+00005140: 0a20 2020 2064 6566 2074 6f5f 776f 726c  .    def to_worl
+00005150: 645f 7370 6163 6528 7365 6c66 2c20 736f  d_space(self, so
+00005160: 7572 6365 2c20 7461 7267 6574 293a 0a20  urce, target):. 
+00005170: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00005180: 616e 6365 2873 6f75 7263 652c 2073 7472  ance(source, str
+00005190: 293a 2073 6f75 7263 6520 3d20 494d 4728  ): source = IMG(
+000051a0: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
+000051b0: 6966 2069 7369 6e73 7461 6e63 6528 7461  if isinstance(ta
+000051c0: 7267 6574 2c20 7374 7229 3a20 7461 7267  rget, str): targ
+000051d0: 6574 203d 2049 4d47 2874 6172 6765 7429  et = IMG(target)
+000051e0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+000051f0: 7374 616e 6365 2873 6f75 7263 652c 2049  stance(source, I
+00005200: 4d47 293a 2073 6f75 7263 6520 3d20 736f  MG): source = so
+00005210: 7572 6365 2e61 6666 696e 650a 2020 2020  urce.affine.    
+00005220: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00005230: 6528 7461 7267 6574 2c20 494d 4729 3a20  e(target, IMG): 
+00005240: 7461 7267 6574 203d 2074 6172 6765 742e  target = target.
+00005250: 6166 6669 6e65 0a20 2020 2020 2020 2072  affine.        r
+00005260: 6574 7572 6e20 7365 6c66 2e74 6f28 2777  eturn self.to('w
+00005270: 6f72 6c64 272c 2073 6f75 7263 655f 6166  orld', source_af
+00005280: 6669 6e65 3d73 6f75 7263 652c 2074 6172  fine=source, tar
+00005290: 6765 745f 6166 6669 6e65 3d74 6172 6765  get_affine=targe
+000052a0: 7429 0a0a 2020 2020 6465 6620 746f 2873  t)..    def to(s
+000052b0: 656c 662c 2073 7061 6365 203d 2022 776f  elf, space = "wo
+000052c0: 726c 6422 2c20 736f 7572 6365 5f61 6666  rld", source_aff
+000052d0: 696e 6520 3d20 6274 2e65 7965 2834 292c  ine = bt.eye(4),
+000052e0: 2074 6172 6765 745f 6166 6669 6e65 203d   target_affine =
+000052f0: 2062 742e 6579 6528 3429 293a 0a20 2020   bt.eye(4)):.   
+00005300: 2020 2020 2074 6172 6765 745f 6166 6669       target_affi
+00005310: 6e65 203d 2062 6174 6f72 6368 5f74 656e  ne = batorch_ten
+00005320: 736f 7228 7461 7267 6574 5f61 6666 696e  sor(target_affin
+00005330: 6529 2e66 6c6f 6174 2829 0a20 2020 2020  e).float().     
+00005340: 2020 2073 6f75 7263 655f 6166 6669 6e65     source_affine
+00005350: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+00005360: 7228 736f 7572 6365 5f61 6666 696e 6529  r(source_affine)
+00005370: 2e66 6c6f 6174 2829 0a20 2020 2020 2020  .float().       
+00005380: 2069 6620 7461 7267 6574 5f61 6666 696e   if target_affin
+00005390: 652e 6e64 696d 203c 3d20 323a 2074 6172  e.ndim <= 2: tar
+000053a0: 6765 745f 6166 6669 6e65 203d 2062 742e  get_affine = bt.
+000053b0: 756e 7371 7565 657a 6528 7461 7267 6574  unsqueeze(target
+000053c0: 5f61 6666 696e 6529 0a20 2020 2020 2020  _affine).       
+000053d0: 2069 6620 736f 7572 6365 5f61 6666 696e   if source_affin
+000053e0: 652e 6e64 696d 203c 3d20 323a 2073 6f75  e.ndim <= 2: sou
+000053f0: 7263 655f 6166 6669 6e65 203d 2062 742e  rce_affine = bt.
+00005400: 756e 7371 7565 657a 6528 736f 7572 6365  unsqueeze(source
+00005410: 5f61 6666 696e 6529 0a20 2020 2020 2020  _affine).       
+00005420: 2069 6620 7370 6163 652e 6c6f 7765 7228   if space.lower(
+00005430: 2920 3d3d 2022 776f 726c 6422 206f 7220  ) == "world" or 
+00005440: 7370 6163 652e 6c6f 7765 7228 2920 3d3d  space.lower() ==
+00005450: 2022 7068 7973 6963 616c 223a 2074 6166   "physical": taf
+00005460: 6669 6e65 203d 2062 742e 696e 7628 7461  fine = bt.inv(ta
+00005470: 7267 6574 5f61 6666 696e 6529 3b20 7361  rget_affine); sa
+00005480: 6666 696e 6520 3d20 736f 7572 6365 5f61  ffine = source_a
+00005490: 6666 696e 650a 2020 2020 2020 2020 656c  ffine.        el
+000054a0: 6966 2073 7061 6365 2e6c 6f77 6572 2829  if space.lower()
+000054b0: 203d 3d20 2269 6d61 6765 2220 6f72 2073   == "image" or s
+000054c0: 7061 6365 2e6c 6f77 6572 2829 203d 3d20  pace.lower() == 
+000054d0: 2269 6e64 6578 223a 2074 6166 6669 6e65  "index": taffine
+000054e0: 203d 2074 6172 6765 745f 6166 6669 6e65   = target_affine
+000054f0: 3b20 7361 6666 696e 6520 3d20 6274 2e69  ; saffine = bt.i
+00005500: 6e76 2873 6f75 7263 655f 6166 6669 6e65  nv(source_affine
+00005510: 290a 2020 2020 2020 2020 656c 7365 3a20  ).        else: 
+00005520: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00005530: 2249 6e76 616c 6964 2073 7061 6365 2066  "Invalid space f
+00005540: 6f72 206d 6574 686f 6420 2774 6f27 2c20  or method 'to', 
+00005550: 7573 6520 2777 6f72 6c64 272f 2770 6879  use 'world'/'phy
+00005560: 7369 6361 6c27 206f 7220 2769 6d61 6765  sical' or 'image
+00005570: 272f 2769 6e64 6578 2720 696e 7374 6561  '/'index' instea
+00005580: 642e 2229 0a20 2020 2020 2020 2072 6574  d.").        ret
+00005590: 7572 6e20 436f 6d70 6f73 6564 5472 616e  urn ComposedTran
+000055a0: 7366 6f72 6d61 7469 6f6e 2841 6666 696e  sformation(Affin
+000055b0: 6528 7361 6666 696e 6529 2c20 7365 6c66  e(saffine), self
+000055c0: 2c20 4166 6669 6e65 2874 6166 6669 6e65  , Affine(taffine
+000055d0: 292c 206d 6f64 653d 2773 7061 7469 616c  ), mode='spatial
+000055e0: 2729 0a20 2020 200a 2020 2020 6465 6620  ').    .    def 
+000055f0: 6e75 6d5f 696e 7628 7365 6c66 2c20 2a73  num_inv(self, *s
+00005600: 697a 652c 2076 6572 626f 7365 3d46 616c  ize, verbose=Fal
+00005610: 7365 293a 0a20 2020 2020 2020 2066 726f  se):.        fro
+00005620: 6d20 2e66 756e 6373 2069 6d70 6f72 7420  m .funcs import 
+00005630: 6265 6e64 696e 670a 2020 2020 2020 2020  bending.        
+00005640: 7369 7a65 203d 2061 7267 5f74 7570 6c65  size = arg_tuple
+00005650: 2873 697a 6529 0a20 2020 2020 2020 2058  (size).        X
+00005660: 203d 2062 742e 696d 6167 655f 6772 6964   = bt.image_grid
+00005670: 282a 7369 7a65 292e 756e 7371 7565 657a  (*size).unsqueez
+00005680: 6528 5b5d 292e 666c 6f61 7428 290a 2020  e([]).float().  
+00005690: 2020 2020 2020 696e 765f 6469 7370 203d        inv_disp =
+000056a0: 202d 2073 656c 662e 746f 5f44 4446 282a   - self.to_DDF(*
+000056b0: 7369 7a65 292e 636c 6f6e 6528 292e 6465  size).clone().de
+000056c0: 7461 6368 2829 0a20 2020 2020 2020 2069  tach().        i
+000056d0: 6e76 5f64 6973 702e 7265 7175 6972 6573  nv_disp.requires
+000056e0: 5f67 7261 6420 3d20 5472 7565 0a20 2020  _grad = True.   
+000056f0: 2020 2020 206f 7074 696d 697a 6572 203d       optimizer =
+00005700: 2062 742e 4341 4441 4d28 5b69 6e76 5f64   bt.CADAM([inv_d
+00005710: 6973 705d 2c20 6c72 203d 2031 652d 3229  isp], lr = 1e-2)
+00005720: 0a20 2020 2020 2020 2070 7265 765f 6c6f  .        prev_lo
+00005730: 7373 203d 204e 6f6e 650a 2020 2020 2020  ss = None.      
+00005740: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00005750: 2834 3030 293a 0a20 2020 2020 2020 2020  (400):.         
+00005760: 2020 2069 7472 616e 7320 3d20 4465 6e73     itrans = Dens
+00005770: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
+00005780: 6c64 2869 6e76 5f64 6973 7029 0a20 2020  ld(inv_disp).   
+00005790: 2020 2020 2020 2020 206c 6f73 7320 3d20           loss = 
+000057a0: 2869 7472 616e 7328 7365 6c66 2858 2929  (itrans(self(X))
+000057b0: 202d 2058 292e 6e6f 726d 3228 292e 6d65   - X).norm2().me
+000057c0: 616e 2829 202b 2031 652d 3120 2a20 6265  an() + 1e-1 * be
+000057d0: 6e64 696e 6728 696e 765f 6469 7370 290a  nding(inv_disp).
+000057e0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+000057f0: 6d69 7a65 722e 6d69 6e69 6d69 7a65 286c  mizer.minimize(l
+00005800: 6f73 7329 2e73 7465 7028 290a 2020 2020  oss).step().    
+00005810: 2020 2020 2020 2020 6966 2076 6572 626f          if verbo
+00005820: 7365 3a20 7072 696e 7428 6622 6974 6572  se: print(f"iter
+00005830: 6174 696f 6e20 7b69 2b31 7d3a 206c 6f73  ation {i+1}: los
+00005840: 7320 3d20 7b6c 6f73 732e 6974 656d 2829  s = {loss.item()
+00005850: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00005860: 6966 2070 7265 765f 6c6f 7373 2069 7320  if prev_loss is 
+00005870: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6f73  not None and los
+00005880: 732e 6974 656d 2829 203e 3d20 7072 6576  s.item() >= prev
+00005890: 5f6c 6f73 733a 206e 6f64 726f 705f 636f  _loss: nodrop_co
+000058a0: 756e 7420 2b3d 2031 0a20 2020 2020 2020  unt += 1.       
+000058b0: 2020 2020 2065 6c73 653a 206e 6f64 726f       else: nodro
+000058c0: 705f 636f 756e 7420 3d20 300a 2020 2020  p_count = 0.    
+000058d0: 2020 2020 2020 2020 6966 206e 6f64 726f          if nodro
+000058e0: 705f 636f 756e 7420 3e3d 2036 3a0a 2020  p_count >= 6:.  
+000058f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005900: 2076 6572 626f 7365 3a20 7072 696e 7428   verbose: print(
+00005910: 6622 5374 6f70 2061 7420 6974 6572 6174  f"Stop at iterat
+00005920: 696f 6e20 7b69 2b31 7d20 6475 6520 746f  ion {i+1} due to
+00005930: 206e 6f20 6472 6f70 7069 6e67 2e20 2229   no dropping. ")
+00005940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005950: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+00005960: 2020 2069 6620 6c6f 7373 2e69 7465 6d28     if loss.item(
+00005970: 2920 3c20 3165 2d33 3a0a 2020 2020 2020  ) < 1e-3:.      
+00005980: 2020 2020 2020 2020 2020 6966 2076 6572            if ver
+00005990: 626f 7365 3a20 7072 696e 7428 6622 5374  bose: print(f"St
+000059a0: 6f70 2061 7420 6974 6572 6174 696f 6e20  op at iteration 
+000059b0: 7b69 2b31 7d20 6475 6520 746f 2073 6d61  {i+1} due to sma
+000059c0: 6c6c 206c 6f73 732e 2022 290a 2020 2020  ll loss. ").    
+000059d0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000059e0: 6b0a 2020 2020 2020 2020 7265 7475 726e  k.        return
+000059f0: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
+00005a00: 6e74 4669 656c 6428 696e 765f 6469 7370  ntField(inv_disp
+00005a10: 290a 2020 2020 0a20 2020 2064 6566 2066  ).    .    def f
+00005a20: 6f72 6365 5f69 6e76 2873 656c 662c 202a  orce_inv(self, *
+00005a30: 7369 7a65 293a 0a20 2020 2020 2020 2069  size):.        i
+00005a40: 6620 6861 7361 7474 7228 7365 6c66 2c20  f hasattr(self, 
+00005a50: 2769 6e76 2729 3a20 7265 7475 726e 2073  'inv'): return s
+00005a60: 656c 662e 696e 7628 290a 2020 2020 2020  elf.inv().      
+00005a70: 2020 656c 7365 3a20 7265 7475 726e 2073    else: return s
+00005a80: 656c 662e 6e75 6d5f 696e 7628 2a73 697a  elf.num_inv(*siz
+00005a90: 6529 0a0a 4061 6c69 6173 2822 4964 2229  e)..@alias("Id")
+00005aa0: 0a63 6c61 7373 2049 6465 6e74 6974 7928  .class Identity(
+00005ab0: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
+00005ac0: 6174 696f 6e29 3a0a 0a20 2020 2064 6566  ation):..    def
+00005ad0: 205f 5f69 6e69 745f 5f28 7365 6c66 293a   __init__(self):
+00005ae0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00005af0: 2020 2020 2049 6465 6e74 6974 7920 7472       Identity tr
+00005b00: 616e 7366 6f72 6d61 7469 6f6e 2e0a 2020  ansformation..  
+00005b10: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00005b20: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
+00005b30: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00005b40: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
+00005b50: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
+00005b60: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00005b90: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+00005ba0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
+00005bb0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
+00005bc0: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
+00005bd0: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
+00005be0: 7366 6f72 6d65 6420 636f 6f72 6469 6e61  sformed coordina
+00005bf0: 7465 732e 2028 5361 6d65 2061 7320 5820  tes. (Same as X 
+00005c00: 666f 7220 4964 656e 7469 7479 290a 2020  for Identity).  
+00005c10: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00005c20: 7a65 3a20 285b 6e5f 6261 7463 685d 2c20  ze: ([n_batch], 
+00005c30: 7b6e 5f64 696d 7d2c 206e 5f31 2c20 6e5f  {n_dim}, n_1, n_
+00005c40: 322c 202e 2e2e 2c20 6e5f 7229 0a20 2020  2, ..., n_r).   
+00005c50: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00005c60: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00005c70: 5f28 290a 2020 2020 2020 2020 0a20 2020  _().        .   
+00005c80: 2064 6566 2061 6666 696e 6528 7365 6c66   def affine(self
+00005c90: 2c20 6e5f 6469 6d3d 4e6f 6e65 293a 0a20  , n_dim=None):. 
+00005ca0: 2020 2020 2020 2069 6620 6e5f 6469 6d20         if n_dim 
+00005cb0: 6973 204e 6f6e 653a 2072 6574 7572 6e0a  is None: return.
+00005cc0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00005cd0: 742e 6579 6528 6e5f 6469 6d20 2b20 3129  t.eye(n_dim + 1)
+00005ce0: 2e75 6e73 7175 6565 7a65 285b 5d29 0a0a  .unsqueeze([])..
+00005cf0: 2020 2020 6465 6620 696e 7628 7365 6c66      def inv(self
+00005d00: 293a 2072 6574 7572 6e20 4964 656e 7469  ): return Identi
+00005d10: 7479 2829 2e62 6163 6b77 6172 645f 2873  ty().backward_(s
+00005d20: 656c 662e 6261 636b 7761 7264 290a 0a63  elf.backward)..c
+00005d30: 6c61 7373 2052 6f74 6174 696f 6e39 3028  lass Rotation90(
+00005d40: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
+00005d50: 6174 696f 6e29 3a0a 2020 2020 6465 6620  ation):.    def 
+00005d60: 5f5f 696e 6974 5f5f 2873 656c 662c 2064  __init__(self, d
+00005d70: 696d 312c 2064 696d 322c 2069 6d61 6765  im1, dim2, image
+00005d80: 5f73 697a 653d 4e6f 6e65 2c20 7265 7369  _size=None, resi
+00005d90: 7a65 5f69 6d61 6765 3d54 7275 6529 3a0a  ze_image=True):.
+00005da0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00005db0: 2020 2020 5472 616e 7366 6f72 6d61 7469      Transformati
+00005dc0: 6f6e 2074 6861 7420 726f 7461 7465 7320  on that rotates 
+00005dd0: 616e 2069 6d61 6765 206f 6620 6069 6d61  an image of `ima
+00005de0: 6765 5f73 697a 6560 2062 7920 3930 2064  ge_size` by 90 d
+00005df0: 6567 7265 6573 2e0a 2020 2020 2020 2020  egrees..        
+00005e00: 0a20 2020 2020 2020 204e 6f74 653a 2054  .        Note: T
+00005e10: 6865 2072 6f74 6174 696f 6e20 6973 2066  he rotation is f
+00005e20: 6f72 2063 6f6f 7264 696e 6174 6573 2c20  or coordinates, 
+00005e30: 6865 6e63 6520 7468 6520 696d 6167 6520  hence the image 
+00005e40: 726f 7461 7465 7320 636c 6f63 6b77 6973  rotates clockwis
+00005e50: 652e 200a 2020 2020 2020 2020 0a20 2020  e. .        .   
+00005e60: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
+00005e70: 2020 2020 2020 2020 2064 696d 312c 2064           dim1, d
+00005e80: 696d 3220 5b69 6e74 5d3a 2054 6865 2070  im2 [int]: The p
+00005e90: 6c61 6e65 2077 6520 726f 7461 7465 206f  lane we rotate o
+00005ea0: 6e2e 2044 6972 6563 7469 6f6e 206f 6620  n. Direction of 
+00005eb0: 7468 6520 726f 7461 7469 6f6e 2069 7320  the rotation is 
+00005ec0: 6672 6f6d 2060 6469 6d31 6020 746f 2060  from `dim1` to `
+00005ed0: 6469 6d32 602e 0a20 2020 2020 2020 2020  dim2`..         
+00005ee0: 2020 2020 2020 2069 2e65 2e20 636f 756e         i.e. coun
+00005ef0: 7465 722d 636c 6f63 6b77 6973 6520 726f  ter-clockwise ro
+00005f00: 7461 7469 6f6e 2077 6974 6820 6469 6d31  tation with dim1
+00005f10: 2061 7320 782d 6178 6973 2061 6e64 2064   as x-axis and d
+00005f20: 696d 3220 6173 2079 2d61 7869 733a 205b  im2 as y-axis: [
+00005f30: 6469 6d31 2c20 6469 6d32 5d20 636f 6f72  dim1, dim2] coor
+00005f40: 6469 6e61 7465 7320 2878 2c20 7929 2062  dinates (x, y) b
+00005f50: 6563 6f6d 6573 2028 796d 6178 2d79 2c20  ecomes (ymax-y, 
+00005f60: 7829 2e0a 2020 2020 2020 2020 2020 2020  x)..            
+00005f70: 696d 6167 655f 7369 7a65 205b 7475 706c  image_size [tupl
+00005f80: 6520 6f72 2062 742e 5465 6e73 6f72 5d3a  e or bt.Tensor]:
+00005f90: 2054 6865 2073 697a 6520 6f66 2074 6865   The size of the
+00005fa0: 2069 6d61 6765 2c20 6f72 2074 6865 2069   image, or the i
+00005fb0: 6d61 6765 2069 7473 656c 662e 200a 2020  mage itself. .  
+00005fc0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00005fd0: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
+00005fe0: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00005ff0: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
+00006000: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
+00006010: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00006040: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+00006050: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
+00006060: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
+00006070: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
+00006080: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
+00006090: 7366 6f72 6d65 6420 636f 6f72 6469 6e61  sformed coordina
+000060a0: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
+000060b0: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+000060c0: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
+000060d0: 6e5f 312c 206e 5f32 2c20 2e2e 2e2c 206e  n_1, n_2, ..., n
+000060e0: 5f72 290a 2020 2020 2020 2020 2727 270a  _r).        '''.
+000060f0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00006100: 5f5f 696e 6974 5f5f 2864 696d 313d 6469  __init__(dim1=di
+00006110: 6d31 2c20 6469 6d32 3d64 696d 322c 2069  m1, dim2=dim2, i
+00006120: 6d61 6765 5f73 697a 653d 696d 6167 655f  mage_size=image_
+00006130: 7369 7a65 2c20 7265 7369 7a65 5f69 6d61  size, resize_ima
+00006140: 6765 3d72 6573 697a 655f 696d 6167 6529  ge=resize_image)
+00006150: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00006160: 696d 312c 2073 656c 662e 6469 6d32 203d  im1, self.dim2 =
+00006170: 2064 696d 312c 2064 696d 320a 2020 2020   dim1, dim2.    
+00006180: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00006190: 6528 696d 6167 655f 7369 7a65 2c20 6274  e(image_size, bt
+000061a0: 2e74 6f72 6368 2e54 656e 736f 7229 3a20  .torch.Tensor): 
+000061b0: 696d 6167 655f 7369 7a65 203d 2069 6d61  image_size = ima
+000061c0: 6765 5f73 697a 652e 7368 6170 650a 2020  ge_size.shape.  
+000061d0: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
+000061e0: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
+000061f0: 7a65 0a20 2020 2020 2020 2069 6620 696d  ze.        if im
+00006200: 6167 655f 7369 7a65 2069 7320 6e6f 7420  age_size is not 
+00006210: 4e6f 6e65 3a20 7365 6c66 2e6e 5f64 696d  None: self.n_dim
+00006220: 203d 206c 656e 2869 6d61 6765 5f73 697a   = len(image_siz
+00006230: 6529 0a20 2020 2020 2020 2069 6620 7265  e).        if re
+00006240: 7369 7a65 5f69 6d61 6765 3a20 7365 6c66  size_image: self
+00006250: 2e72 6573 6861 7065 203d 205b 2831 2c29  .reshape = [(1,)
+00006260: 2c20 2864 696d 312c 2064 696d 3229 5d0a  , (dim1, dim2)].
+00006270: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
+00006280: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
+00006290: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
+000062a0: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
+000062b0: 2020 2020 6469 6d31 2c20 6469 6d32 203d      dim1, dim2 =
+000062c0: 2073 656c 662e 6469 6d31 2c20 7365 6c66   self.dim1, self
+000062d0: 2e64 696d 320a 2020 2020 2020 2020 7365  .dim2.        se
+000062e0: 6c65 6374 3120 3d20 2873 6c69 6365 284e  lect1 = (slice(N
+000062f0: 6f6e 6529 2c29 202a 2058 2e63 6861 6e6e  one),) * X.chann
+00006300: 656c 5f64 696d 202b 2028 6469 6d31 2c29  el_dim + (dim1,)
+00006310: 0a20 2020 2020 2020 2073 656c 6563 7432  .        select2
+00006320: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
+00006330: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
+00006340: 6d20 2b20 2864 696d 322c 290a 2020 2020  m + (dim2,).    
+00006350: 2020 2020 6966 2073 656c 662e 696d 6167      if self.imag
+00006360: 655f 7369 7a65 2069 7320 4e6f 6e65 3a20  e_size is None: 
+00006370: 6d61 785f 7261 6e67 6520 3d20 585b 7365  max_range = X[se
+00006380: 6c65 6374 325d 2e6d 6178 2829 0a20 2020  lect2].max().   
+00006390: 2020 2020 2065 6c73 653a 206d 6178 5f72       else: max_r
+000063a0: 616e 6765 203d 2073 656c 662e 696d 6167  ange = self.imag
+000063b0: 655f 7369 7a65 5b64 696d 325d 0a20 2020  e_size[dim2].   
+000063c0: 2020 2020 2058 5b73 656c 6563 7431 5d20       X[select1] 
+000063d0: 3d20 585b 7365 6c65 6374 315d 202b 206d  = X[select1] + m
+000063e0: 6178 5f72 616e 6765 202d 2058 5b73 656c  ax_range - X[sel
+000063f0: 6563 7432 5d0a 2020 2020 2020 2020 585b  ect2].        X[
+00006400: 7365 6c65 6374 325d 203d 2058 5b73 656c  select2] = X[sel
+00006410: 6563 7431 5d20 2b20 585b 7365 6c65 6374  ect1] + X[select
+00006420: 325d 202d 206d 6178 5f72 616e 6765 0a20  2] - max_range. 
+00006430: 2020 2020 2020 2058 5b73 656c 6563 7431         X[select1
+00006440: 5d20 3d20 585b 7365 6c65 6374 315d 202d  ] = X[select1] -
+00006450: 2058 5b73 656c 6563 7432 5d0a 2020 2020   X[select2].    
+00006460: 2020 2020 7265 7475 726e 2058 0a20 2020      return X.   
+00006470: 2020 2020 200a 2020 2020 6465 6620 6166       .    def af
+00006480: 6669 6e65 2873 656c 662c 206e 5f64 696d  fine(self, n_dim
+00006490: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+000064a0: 6966 2073 656c 662e 696d 6167 655f 7369  if self.image_si
+000064b0: 7a65 2069 7320 4e6f 6e65 3a20 7265 7475  ze is None: retu
+000064c0: 726e 0a20 2020 2020 2020 2069 6620 6e5f  rn.        if n_
+000064d0: 6469 6d20 6973 204e 6f6e 6520 616e 6420  dim is None and 
+000064e0: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
+000064f0: 6e65 3a20 7265 7475 726e 0a20 2020 2020  ne: return.     
+00006500: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+00006510: 6f6e 653a 206e 5f64 696d 203d 2073 656c  one: n_dim = sel
+00006520: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
+00006530: 6176 6f75 6368 2873 656c 662e 6e5f 6469  avouch(self.n_di
+00006540: 6d20 6973 204e 6f6e 6520 6f72 2073 656c  m is None or sel
+00006550: 662e 6e5f 6469 6d20 3d3d 206e 5f64 696d  f.n_dim == n_dim
+00006560: 290a 2020 2020 2020 2020 6469 6d31 2c20  ).        dim1, 
+00006570: 6469 6d32 203d 2073 656c 662e 6469 6d31  dim2 = self.dim1
+00006580: 2c20 7365 6c66 2e64 696d 320a 2020 2020  , self.dim2.    
+00006590: 2020 2020 6166 6620 3d20 6274 2e65 7965      aff = bt.eye
+000065a0: 286e 5f64 696d 202b 2031 290a 2020 2020  (n_dim + 1).    
+000065b0: 2020 2020 6166 665b 6469 6d31 5d5b 6469      aff[dim1][di
+000065c0: 6d31 5d20 3d20 302e 0a20 2020 2020 2020  m1] = 0..       
+000065d0: 2061 6666 5b64 696d 315d 5b64 696d 325d   aff[dim1][dim2]
+000065e0: 203d 202d 312e 0a20 2020 2020 2020 2061   = -1..        a
+000065f0: 6666 5b64 696d 315d 5b2d 315d 203d 2066  ff[dim1][-1] = f
+00006600: 6c6f 6174 2873 656c 662e 696d 6167 655f  loat(self.image_
+00006610: 7369 7a65 5b64 696d 325d 290a 2020 2020  size[dim2]).    
+00006620: 2020 2020 6166 665b 6469 6d32 5d5b 6469      aff[dim2][di
+00006630: 6d32 5d20 3d20 302e 0a20 2020 2020 2020  m2] = 0..       
+00006640: 2061 6666 5b64 696d 325d 5b64 696d 315d   aff[dim2][dim1]
+00006650: 203d 2031 2e0a 2020 2020 2020 2020 6966   = 1..        if
+00006660: 206e 6f74 2073 656c 662e 6261 636b 7761   not self.backwa
+00006670: 7264 3a20 6166 6620 3d20 6166 662e 696e  rd: aff = aff.in
+00006680: 7628 290a 2020 2020 2020 2020 7265 7475  v().        retu
+00006690: 726e 2061 6666 2e75 6e73 7175 6565 7a65  rn aff.unsqueeze
+000066a0: 285b 5d29 0a20 2020 200a 2020 2020 6465  ([]).    .    de
+000066b0: 6620 696e 7628 7365 6c66 293a 2072 6574  f inv(self): ret
+000066c0: 7572 6e20 526f 7461 7469 6f6e 3237 3028  urn Rotation270(
+000066d0: 7365 6c66 2e64 696d 312c 2073 656c 662e  self.dim1, self.
+000066e0: 6469 6d32 2c20 696d 6167 655f 7369 7a65  dim2, image_size
+000066f0: 203d 2073 656c 662e 696d 6167 655f 7369   = self.image_si
+00006700: 7a65 2c20 7265 7369 7a65 5f69 6d61 6765  ze, resize_image
+00006710: 203d 2073 656c 662e 7265 7369 7a65 5f69   = self.resize_i
+00006720: 6d61 6765 292e 6261 636b 7761 7264 5f28  mage).backward_(
+00006730: 7365 6c66 2e62 6163 6b77 6172 6429 0a0a  self.backward)..
+00006740: 636c 6173 7320 526f 7461 7469 6f6e 3237  class Rotation27
+00006750: 3028 5370 6174 6961 6c54 7261 6e73 666f  0(SpatialTransfo
+00006760: 726d 6174 696f 6e29 3a0a 2020 2020 6465  rmation):.    de
+00006770: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00006780: 2064 696d 312c 2064 696d 322c 2069 6d61   dim1, dim2, ima
+00006790: 6765 5f73 697a 653d 4e6f 6e65 2c20 7265  ge_size=None, re
+000067a0: 7369 7a65 5f69 6d61 6765 3d54 7275 6529  size_image=True)
+000067b0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+000067c0: 2020 2020 2020 5472 616e 7366 6f72 6d61        Transforma
+000067d0: 7469 6f6e 2074 6861 7420 726f 7461 7465  tion that rotate
+000067e0: 7320 616e 2069 6d61 6765 2062 7920 3237  s an image by 27
+000067f0: 3020 6465 6772 6565 732e 0a20 2020 2020  0 degrees..     
+00006800: 2020 200a 2020 2020 2020 2020 4e6f 7465     .        Note
+00006810: 3a20 5468 6520 726f 7461 7469 6f6e 2069  : The rotation i
+00006820: 7320 666f 7220 636f 6f72 6469 6e61 7465  s for coordinate
+00006830: 732c 2068 656e 6365 2074 6865 2069 6d61  s, hence the ima
+00006840: 6765 2072 6f74 6174 6573 2063 6c6f 636b  ge rotates clock
+00006850: 7769 7365 2e20 0a20 2020 2020 2020 200a  wise. .        .
+00006860: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
+00006870: 2020 2020 2020 2020 2020 2020 6469 6d31              dim1
+00006880: 2c20 6469 6d32 205b 696e 745d 3a20 5468  , dim2 [int]: Th
+00006890: 6520 706c 616e 6520 7765 2072 6f74 6174  e plane we rotat
+000068a0: 6520 6f6e 2e20 4469 7265 6374 696f 6e20  e on. Direction 
+000068b0: 6f66 2074 6865 2072 6f74 6174 696f 6e20  of the rotation 
+000068c0: 6973 2066 726f 6d20 6064 696d 3160 2074  is from `dim1` t
+000068d0: 6f20 6064 696d 3260 2e0a 2020 2020 2020  o `dim2`..      
+000068e0: 2020 2020 2020 2020 2020 692e 652e 2063            i.e. c
+000068f0: 6f75 6e74 6572 2d63 6c6f 636b 7769 7365  ounter-clockwise
+00006900: 2072 6f74 6174 696f 6e20 7769 7468 2064   rotation with d
+00006910: 696d 3120 6173 2078 2d61 7869 7320 616e  im1 as x-axis an
+00006920: 6420 6469 6d32 2061 7320 792d 6178 6973  d dim2 as y-axis
+00006930: 3a20 5b64 696d 312c 2064 696d 325d 2063  : [dim1, dim2] c
+00006940: 6f6f 7264 696e 6174 6573 2028 782c 2079  oordinates (x, y
+00006950: 2920 6265 636f 6d65 7320 2879 2c20 786d  ) becomes (y, xm
+00006960: 6178 2d78 292e 0a20 2020 2020 2020 2020  ax-x)..         
+00006970: 2020 2069 6d61 6765 5f73 697a 6520 5b74     image_size [t
+00006980: 7570 6c65 206f 7220 6274 2e54 656e 736f  uple or bt.Tenso
+00006990: 725d 3a20 5468 6520 7369 7a65 206f 6620  r]: The size of 
+000069a0: 7468 6520 696d 6167 652c 206f 7220 7468  the image, or th
+000069b0: 6520 696d 6167 6520 6974 7365 6c66 2e20  e image itself. 
+000069c0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+000069d0: 2020 2020 2020 5768 656e 2069 7420 6973        When it is
+000069e0: 2063 616c 6c65 643a 0a20 2020 2020 2020   called:.       
+000069f0: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
+00006a00: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
+00006a10: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
+00006a20: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
+00006a30: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+00006a40: 6368 3a6f 7074 696f 6e61 6c5d 2c20 7b6e  ch:optional], {n
+00006a50: 5f64 696d 7d2c 206e 5f31 2c20 6e5f 322c  _dim}, n_1, n_2,
+00006a60: 202e 2e2e 2c20 6e5f 7229 0a20 2020 2020   ..., n_r).     
+00006a70: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
+00006a80: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
+00006a90: 7261 6e73 666f 726d 6564 2063 6f6f 7264  ransformed coord
+00006aa0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
+00006ab0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+00006ac0: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+00006ad0: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
+00006ae0: 2c20 6e5f 7229 0a20 2020 2020 2020 2027  , n_r).        '
+00006af0: 2727 0a20 2020 2020 2020 2073 7570 6572  ''.        super
+00006b00: 2829 2e5f 5f69 6e69 745f 5f28 6469 6d31  ().__init__(dim1
+00006b10: 3d64 696d 312c 2064 696d 323d 6469 6d32  =dim1, dim2=dim2
+00006b20: 2c20 696d 6167 655f 7369 7a65 3d69 6d61  , image_size=ima
+00006b30: 6765 5f73 697a 652c 2072 6573 697a 655f  ge_size, resize_
+00006b40: 696d 6167 653d 7265 7369 7a65 5f69 6d61  image=resize_ima
+00006b50: 6765 290a 0a20 2020 2020 2020 2073 656c  ge)..        sel
+00006b60: 662e 6469 6d31 2c20 7365 6c66 2e64 696d  f.dim1, self.dim
+00006b70: 3220 3d20 6469 6d31 2c20 6469 6d32 0a20  2 = dim1, dim2. 
+00006b80: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00006b90: 616e 6365 2869 6d61 6765 5f73 697a 652c  ance(image_size,
+00006ba0: 2062 742e 746f 7263 682e 5465 6e73 6f72   bt.torch.Tensor
+00006bb0: 293a 2069 6d61 6765 5f73 697a 6520 3d20  ): image_size = 
+00006bc0: 696d 6167 655f 7369 7a65 2e73 6861 7065  image_size.shape
+00006bd0: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
+00006be0: 6167 655f 7369 7a65 203d 2069 6d61 6765  age_size = image
+00006bf0: 5f73 697a 650a 2020 2020 2020 2020 6966  _size.        if
+00006c00: 2069 6d61 6765 5f73 697a 6520 6973 206e   image_size is n
+00006c10: 6f74 204e 6f6e 653a 2073 656c 662e 6e5f  ot None: self.n_
+00006c20: 6469 6d20 3d20 6c65 6e28 696d 6167 655f  dim = len(image_
+00006c30: 7369 7a65 290a 2020 2020 2020 2020 6966  size).        if
+00006c40: 2072 6573 697a 655f 696d 6167 653a 2073   resize_image: s
+00006c50: 656c 662e 7265 7368 6170 6520 3d20 5b28  elf.reshape = [(
+00006c60: 312c 292c 2028 6469 6d31 2c20 6469 6d32  1,), (dim1, dim2
+00006c70: 295d 0a0a 2020 2020 6465 6620 5f5f 6361  )]..    def __ca
+00006c80: 6c6c 5f5f 2873 656c 662c 2058 293a 0a20  ll__(self, X):. 
+00006c90: 2020 2020 2020 2058 203d 2073 7570 6572         X = super
+00006ca0: 2829 2e5f 5f63 616c 6c5f 5f28 5829 0a20  ().__call__(X). 
+00006cb0: 2020 2020 2020 2064 696d 312c 2064 696d         dim1, dim
+00006cc0: 3220 3d20 7365 6c66 2e64 696d 312c 2073  2 = self.dim1, s
+00006cd0: 656c 662e 6469 6d32 0a20 2020 2020 2020  elf.dim2.       
+00006ce0: 2073 656c 6563 7431 203d 2028 736c 6963   select1 = (slic
+00006cf0: 6528 4e6f 6e65 292c 2920 2a20 582e 6368  e(None),) * X.ch
+00006d00: 616e 6e65 6c5f 6469 6d20 2b20 2864 696d  annel_dim + (dim
+00006d10: 312c 290a 2020 2020 2020 2020 7365 6c65  1,).        sele
+00006d20: 6374 3220 3d20 2873 6c69 6365 284e 6f6e  ct2 = (slice(Non
+00006d30: 6529 2c29 202a 2058 2e63 6861 6e6e 656c  e),) * X.channel
+00006d40: 5f64 696d 202b 2028 6469 6d32 2c29 0a20  _dim + (dim2,). 
+00006d50: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00006d60: 6d61 6765 5f73 697a 6520 6973 204e 6f6e  mage_size is Non
+00006d70: 653a 206d 6178 5f72 616e 6765 203d 2058  e: max_range = X
+00006d80: 5b73 656c 6563 7431 5d2e 6d61 7828 290a  [select1].max().
+00006d90: 2020 2020 2020 2020 656c 7365 3a20 6d61          else: ma
+00006da0: 785f 7261 6e67 6520 3d20 7365 6c66 2e69  x_range = self.i
+00006db0: 6d61 6765 5f73 697a 655b 6469 6d31 5d0a  mage_size[dim1].
+00006dc0: 2020 2020 2020 2020 585b 7365 6c65 6374          X[select
+00006dd0: 325d 203d 2058 5b73 656c 6563 7432 5d20  2] = X[select2] 
+00006de0: 2b20 6d61 785f 7261 6e67 6520 2d20 585b  + max_range - X[
+00006df0: 7365 6c65 6374 315d 0a20 2020 2020 2020  select1].       
+00006e00: 2058 5b73 656c 6563 7431 5d20 3d20 585b   X[select1] = X[
+00006e10: 7365 6c65 6374 325d 202b 2058 5b73 656c  select2] + X[sel
+00006e20: 6563 7431 5d20 2d20 6d61 785f 7261 6e67  ect1] - max_rang
+00006e30: 650a 2020 2020 2020 2020 585b 7365 6c65  e.        X[sele
+00006e40: 6374 325d 203d 2058 5b73 656c 6563 7432  ct2] = X[select2
+00006e50: 5d20 2d20 585b 7365 6c65 6374 315d 0a20  ] - X[select1]. 
+00006e60: 2020 2020 2020 2072 6574 7572 6e20 580a         return X.
+00006e70: 2020 2020 2020 2020 0a20 2020 2064 6566          .    def
+00006e80: 2061 6666 696e 6528 7365 6c66 2c20 6e5f   affine(self, n_
+00006e90: 6469 6d3d 4e6f 6e65 293a 0a20 2020 2020  dim=None):.     
+00006ea0: 2020 2069 6620 7365 6c66 2e69 6d61 6765     if self.image
+00006eb0: 5f73 697a 6520 6973 204e 6f6e 653a 2072  _size is None: r
 00006ec0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00006ed0: 206e 5f64 696d 2069 7320 4e6f 6e65 3a20   n_dim is None: 
-00006ee0: 6e5f 6469 6d20 3d20 7365 6c66 2e6e 5f64  n_dim = self.n_d
-00006ef0: 696d 0a20 2020 2020 2020 2061 766f 7563  im.        avouc
-00006f00: 6828 7365 6c66 2e6e 5f64 696d 2069 7320  h(self.n_dim is 
-00006f10: 4e6f 6e65 206f 7220 7365 6c66 2e6e 5f64  None or self.n_d
-00006f20: 696d 203d 3d20 6e5f 6469 6d29 0a20 2020  im == n_dim).   
-00006f30: 2020 2020 2064 696d 312c 2064 696d 3220       dim1, dim2 
-00006f40: 3d20 7365 6c66 2e64 696d 312c 2073 656c  = self.dim1, sel
-00006f50: 662e 6469 6d32 0a20 2020 2020 2020 2061  f.dim2.        a
-00006f60: 6666 203d 2062 742e 6579 6528 6e5f 6469  ff = bt.eye(n_di
-00006f70: 6d20 2b20 3129 0a20 2020 2020 2020 2061  m + 1).        a
-00006f80: 6666 5b64 696d 315d 5b64 696d 315d 203d  ff[dim1][dim1] =
-00006f90: 2030 2e0a 2020 2020 2020 2020 6166 665b   0..        aff[
-00006fa0: 6469 6d31 5d5b 6469 6d32 5d20 3d20 312e  dim1][dim2] = 1.
-00006fb0: 0a20 2020 2020 2020 2061 6666 5b64 696d  .        aff[dim
-00006fc0: 325d 5b64 696d 325d 203d 2030 2e0a 2020  2][dim2] = 0..  
-00006fd0: 2020 2020 2020 6166 665b 6469 6d32 5d5b        aff[dim2][
-00006fe0: 6469 6d31 5d20 3d20 2d31 2e0a 2020 2020  dim1] = -1..    
-00006ff0: 2020 2020 6166 665b 6469 6d32 5d5b 2d31      aff[dim2][-1
-00007000: 5d20 3d20 666c 6f61 7428 7365 6c66 2e69  ] = float(self.i
-00007010: 6d61 6765 5f73 697a 655b 6469 6d31 5d29  mage_size[dim1])
-00007020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007030: 6166 662e 756e 7371 7565 657a 6528 5b5d  aff.unsqueeze([]
-00007040: 290a 2020 2020 0a20 2020 2064 6566 2069  ).    .    def i
-00007050: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
-00007060: 2052 6f74 6174 696f 6e39 3028 7365 6c66   Rotation90(self
-00007070: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
-00007080: 2c20 696d 6167 655f 7369 7a65 203d 2073  , image_size = s
-00007090: 656c 662e 696d 6167 655f 7369 7a65 2c20  elf.image_size, 
-000070a0: 7265 7369 7a65 5f69 6d61 6765 203d 2073  resize_image = s
-000070b0: 656c 662e 7265 7369 7a65 5f69 6d61 6765  elf.resize_image
-000070c0: 292e 6261 636b 7761 7264 5f28 7365 6c66  ).backward_(self
-000070d0: 2e62 6163 6b77 6172 6429 0a0a 636c 6173  .backward)..clas
-000070e0: 7320 526f 7461 7469 6f6e 3138 3028 5370  s Rotation180(Sp
-000070f0: 6174 6961 6c54 7261 6e73 666f 726d 6174  atialTransformat
-00007100: 696f 6e29 3a0a 2020 2020 6465 6620 5f5f  ion):.    def __
-00007110: 696e 6974 5f5f 2873 656c 662c 2064 696d  init__(self, dim
-00007120: 312c 2064 696d 322c 2069 6d61 6765 5f73  1, dim2, image_s
-00007130: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
-00007140: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
-00007150: 7261 6e73 666f 726d 6174 696f 6e20 7468  ransformation th
-00007160: 6174 2072 6f74 6174 6573 2061 6e20 696d  at rotates an im
-00007170: 6167 6520 6279 2031 3830 2064 6567 7265  age by 180 degre
-00007180: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00007190: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
-000071a0: 2020 2020 2020 2020 2064 696d 312c 2064           dim1, d
-000071b0: 696d 3220 5b69 6e74 5d3a 2054 6865 2070  im2 [int]: The p
-000071c0: 6c61 6e65 2077 6520 726f 7461 7465 206f  lane we rotate o
-000071d0: 6e2e 2044 6972 6563 7469 6f6e 206f 6620  n. Direction of 
-000071e0: 7468 6520 726f 7461 7469 6f6e 2069 7320  the rotation is 
-000071f0: 6672 6f6d 2060 6469 6d31 6020 746f 2060  from `dim1` to `
-00007200: 6469 6d32 602e 0a20 2020 2020 2020 2020  dim2`..         
-00007210: 2020 2020 2020 2069 2e65 2e20 726f 7461         i.e. rota
-00007220: 7469 6f6e 2077 6974 6820 6469 6d31 2061  tion with dim1 a
-00007230: 7320 782d 6178 6973 2061 6e64 2064 696d  s x-axis and dim
-00007240: 3220 6173 2079 2d61 7869 733a 205b 6469  2 as y-axis: [di
-00007250: 6d31 2c20 6469 6d32 5d20 636f 6f72 6469  m1, dim2] coordi
-00007260: 6e61 7465 7320 2878 2c20 7929 2062 6563  nates (x, y) bec
-00007270: 6f6d 6573 2028 786d 6178 2d78 2c20 796d  omes (xmax-x, ym
-00007280: 6178 2d79 292e 0a20 2020 2020 2020 2020  ax-y)..         
-00007290: 2020 2069 6d61 6765 5f73 697a 6520 5b74     image_size [t
-000072a0: 7570 6c65 206f 7220 6274 2e54 656e 736f  uple or bt.Tenso
-000072b0: 725d 3a20 5468 6520 7369 7a65 206f 6620  r]: The size of 
-000072c0: 7468 6520 696d 6167 652c 206f 7220 7468  the image, or th
-000072d0: 6520 696d 6167 6520 6974 7365 6c66 2e20  e image itself. 
-000072e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-000072f0: 2020 2020 2020 5768 656e 2069 7420 6973        When it is
-00007300: 2063 616c 6c65 643a 0a20 2020 2020 2020   called:.       
-00007310: 2020 2020 2058 205b 6274 2e54 656e 736f       X [bt.Tenso
-00007320: 725d 3a20 436f 6f72 6469 6e61 7465 7320  r]: Coordinates 
-00007330: 746f 2062 6520 7472 616e 7366 6f72 6d65  to be transforme
-00007340: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-00007350: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-00007360: 6368 3a6f 7074 696f 6e61 6c5d 2c20 7b6e  ch:optional], {n
-00007370: 5f64 696d 7d2c 206e 5f31 2c20 6e5f 322c  _dim}, n_1, n_2,
-00007380: 202e 2e2e 2c20 6e5f 7229 0a20 2020 2020   ..., n_r).     
-00007390: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
-000073a0: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
-000073b0: 7261 6e73 666f 726d 6564 2063 6f6f 7264  ransformed coord
-000073c0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
-000073d0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-000073e0: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
-000073f0: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
-00007400: 2c20 6e5f 7229 0a20 2020 2020 2020 2027  , n_r).        '
-00007410: 2727 0a20 2020 2020 2020 2073 7570 6572  ''.        super
-00007420: 2829 2e5f 5f69 6e69 745f 5f28 6469 6d31  ().__init__(dim1
-00007430: 3d64 696d 312c 2064 696d 323d 6469 6d32  =dim1, dim2=dim2
-00007440: 2c20 696d 6167 655f 7369 7a65 3d69 6d61  , image_size=ima
-00007450: 6765 5f73 697a 6529 0a0a 2020 2020 2020  ge_size)..      
-00007460: 2020 7365 6c66 2e64 696d 312c 2073 656c    self.dim1, sel
-00007470: 662e 6469 6d32 203d 2064 696d 312c 2064  f.dim2 = dim1, d
-00007480: 696d 320a 2020 2020 2020 2020 6966 2069  im2.        if i
-00007490: 7369 6e73 7461 6e63 6528 696d 6167 655f  sinstance(image_
-000074a0: 7369 7a65 2c20 6274 2e74 6f72 6368 2e54  size, bt.torch.T
-000074b0: 656e 736f 7229 3a20 696d 6167 655f 7369  ensor): image_si
-000074c0: 7a65 203d 2069 6d61 6765 5f73 697a 652e  ze = image_size.
-000074d0: 7368 6170 650a 2020 2020 2020 2020 7365  shape.        se
-000074e0: 6c66 2e69 6d61 6765 5f73 697a 6520 3d20  lf.image_size = 
-000074f0: 696d 6167 655f 7369 7a65 0a20 2020 2020  image_size.     
-00007500: 2020 2069 6620 696d 6167 655f 7369 7a65     if image_size
-00007510: 2069 7320 6e6f 7420 4e6f 6e65 3a20 7365   is not None: se
-00007520: 6c66 2e6e 5f64 696d 203d 206c 656e 2869  lf.n_dim = len(i
-00007530: 6d61 6765 5f73 697a 6529 0a0a 2020 2020  mage_size)..    
-00007540: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-00007550: 662c 2058 293a 0a20 2020 2020 2020 2058  f, X):.        X
-00007560: 203d 2073 7570 6572 2829 2e5f 5f63 616c   = super().__cal
-00007570: 6c5f 5f28 5829 0a20 2020 2020 2020 2064  l__(X).        d
-00007580: 696d 312c 2064 696d 3220 3d20 7365 6c66  im1, dim2 = self
-00007590: 2e64 696d 312c 2073 656c 662e 6469 6d32  .dim1, self.dim2
-000075a0: 0a20 2020 2020 2020 2073 656c 6563 7431  .        select1
-000075b0: 203d 2028 736c 6963 6528 4e6f 6e65 292c   = (slice(None),
-000075c0: 2920 2a20 582e 6368 616e 6e65 6c5f 6469  ) * X.channel_di
-000075d0: 6d20 2b20 2864 696d 312c 290a 2020 2020  m + (dim1,).    
-000075e0: 2020 2020 7365 6c65 6374 3220 3d20 2873      select2 = (s
-000075f0: 6c69 6365 284e 6f6e 6529 2c29 202a 2058  lice(None),) * X
-00007600: 2e63 6861 6e6e 656c 5f64 696d 202b 2028  .channel_dim + (
-00007610: 6469 6d32 2c29 0a20 2020 2020 2020 2069  dim2,).        i
-00007620: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
-00007630: 6520 6973 204e 6f6e 653a 206d 6178 5f72  e is None: max_r
-00007640: 616e 6765 312c 206d 6178 5f72 616e 6765  ange1, max_range
-00007650: 3220 3d20 585b 7365 6c65 6374 315d 2e6d  2 = X[select1].m
-00007660: 6178 2829 2c20 585b 7365 6c65 6374 325d  ax(), X[select2]
-00007670: 2e6d 6178 2829 0a20 2020 2020 2020 2065  .max().        e
-00007680: 6c73 653a 206d 6178 5f72 616e 6765 312c  lse: max_range1,
-00007690: 206d 6178 5f72 616e 6765 3220 3d20 7365   max_range2 = se
-000076a0: 6c66 2e69 6d61 6765 5f73 697a 655b 6469  lf.image_size[di
-000076b0: 6d31 5d2c 2073 656c 662e 696d 6167 655f  m1], self.image_
-000076c0: 7369 7a65 5b64 696d 325d 0a20 2020 2020  size[dim2].     
-000076d0: 2020 2058 5b73 656c 6563 7431 5d20 3d20     X[select1] = 
-000076e0: 6d61 785f 7261 6e67 6531 202d 2058 5b73  max_range1 - X[s
-000076f0: 656c 6563 7431 5d0a 2020 2020 2020 2020  elect1].        
-00007700: 585b 7365 6c65 6374 325d 203d 206d 6178  X[select2] = max
-00007710: 5f72 616e 6765 3220 2d20 585b 7365 6c65  _range2 - X[sele
-00007720: 6374 325d 0a20 2020 2020 2020 2072 6574  ct2].        ret
-00007730: 7572 6e20 580a 2020 2020 2020 2020 0a20  urn X.        . 
-00007740: 2020 2064 6566 2061 6666 696e 6528 7365     def affine(se
-00007750: 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65 293a  lf, n_dim=None):
-00007760: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007770: 2e69 6d61 6765 5f73 697a 6520 6973 204e  .image_size is N
-00007780: 6f6e 653a 2072 6574 7572 6e0a 2020 2020  one: return.    
-00007790: 2020 2020 6966 206e 5f64 696d 2069 7320      if n_dim is 
-000077a0: 4e6f 6e65 2061 6e64 2073 656c 662e 6e5f  None and self.n_
-000077b0: 6469 6d20 6973 204e 6f6e 653a 2072 6574  dim is None: ret
-000077c0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
-000077d0: 5f64 696d 2069 7320 4e6f 6e65 3a20 6e5f  _dim is None: n_
-000077e0: 6469 6d20 3d20 7365 6c66 2e6e 5f64 696d  dim = self.n_dim
-000077f0: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
-00007800: 7365 6c66 2e6e 5f64 696d 2069 7320 4e6f  self.n_dim is No
-00007810: 6e65 206f 7220 7365 6c66 2e6e 5f64 696d  ne or self.n_dim
-00007820: 203d 3d20 6e5f 6469 6d29 0a20 2020 2020   == n_dim).     
-00007830: 2020 2064 696d 312c 2064 696d 3220 3d20     dim1, dim2 = 
-00007840: 7365 6c66 2e64 696d 312c 2073 656c 662e  self.dim1, self.
-00007850: 6469 6d32 0a20 2020 2020 2020 2061 6666  dim2.        aff
-00007860: 203d 2062 742e 6579 6528 6e5f 6469 6d20   = bt.eye(n_dim 
-00007870: 2b20 3129 0a20 2020 2020 2020 2061 6666  + 1).        aff
-00007880: 5b64 696d 315d 5b64 696d 315d 203d 202d  [dim1][dim1] = -
-00007890: 312e 0a20 2020 2020 2020 2061 6666 5b64  1..        aff[d
-000078a0: 696d 315d 5b2d 315d 203d 2066 6c6f 6174  im1][-1] = float
-000078b0: 2873 656c 662e 696d 6167 655f 7369 7a65  (self.image_size
-000078c0: 5b64 696d 315d 290a 2020 2020 2020 2020  [dim1]).        
-000078d0: 6166 665b 6469 6d32 5d5b 6469 6d32 5d20  aff[dim2][dim2] 
-000078e0: 3d20 2d31 2e0a 2020 2020 2020 2020 6166  = -1..        af
-000078f0: 665b 6469 6d32 5d5b 2d31 5d20 3d20 666c  f[dim2][-1] = fl
-00007900: 6f61 7428 7365 6c66 2e69 6d61 6765 5f73  oat(self.image_s
-00007910: 697a 655b 6469 6d32 5d29 0a20 2020 2020  ize[dim2]).     
-00007920: 2020 2072 6574 7572 6e20 6166 662e 756e     return aff.un
-00007930: 7371 7565 657a 6528 5b5d 290a 0a20 2020  squeeze([])..   
-00007940: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
-00007950: 7265 7475 726e 2052 6f74 6174 696f 6e31  return Rotation1
-00007960: 3830 2873 656c 662e 6469 6d31 2c20 7365  80(self.dim1, se
-00007970: 6c66 2e64 696d 322c 2069 6d61 6765 5f73  lf.dim2, image_s
-00007980: 697a 6520 3d20 7365 6c66 2e69 6d61 6765  ize = self.image
-00007990: 5f73 697a 6529 2e62 6163 6b77 6172 645f  _size).backward_
-000079a0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
-000079b0: 0a40 616c 6961 7328 2252 6566 6c65 6374  .@alias("Reflect
-000079c0: 2229 0a63 6c61 7373 2052 6566 6c65 6374  ").class Reflect
-000079d0: 696f 6e28 5370 6174 6961 6c54 7261 6e73  ion(SpatialTrans
-000079e0: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
-000079f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00007a00: 662c 202a 6469 6d2c 2069 6d61 6765 5f73  f, *dim, image_s
-00007a10: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
-00007a20: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
-00007a30: 7261 6e73 666f 726d 6174 696f 6e20 7468  ransformation th
-00007a40: 6174 2072 6566 6c65 6374 7320 616e 2069  at reflects an i
-00007a50: 6d61 6765 2061 6c6f 6e67 2064 696d 656e  mage along dimen
-00007a60: 7369 6f6e 2064 696d 2e0a 2020 2020 2020  sion dim..      
-00007a70: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00007a80: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-00007a90: 696d 205b 696e 745d 3a20 5468 6520 6469  im [int]: The di
-00007aa0: 6d65 6e73 696f 6e20 7765 2072 6566 6c65  mension we refle
-00007ab0: 6374 2074 6865 2069 6d61 6765 2061 6c6f  ct the image alo
-00007ac0: 6e67 2e20 0a20 2020 2020 2020 2020 2020  ng. .           
-00007ad0: 2020 2020 2069 2e65 2e20 7265 666c 6563       i.e. reflec
-00007ae0: 7469 6f6e 206f 6e20 6469 6d3a 205b 6469  tion on dim: [di
-00007af0: 6d5d 2063 6f6f 7264 696e 6174 6520 7820  m] coordinate x 
-00007b00: 6265 636f 6d65 7320 786d 6178 2d78 2e0a  becomes xmax-x..
-00007b10: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-00007b20: 655f 7369 7a65 205b 7475 706c 6520 6f72  e_size [tuple or
-00007b30: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
-00007b40: 2073 697a 6520 6f66 2074 6865 2069 6d61   size of the ima
-00007b50: 6765 2c20 6f72 2074 6865 2069 6d61 6765  ge, or the image
-00007b60: 2069 7473 656c 662e 200a 2020 2020 2020   itself. .      
-00007b70: 2020 2020 2020 0a20 2020 2020 2020 2057        .        W
-00007b80: 6865 6e20 6974 2069 7320 6361 6c6c 6564  hen it is called
-00007b90: 3a0a 2020 2020 2020 2020 2020 2020 5820  :.            X 
-00007ba0: 5b62 742e 5465 6e73 6f72 5d3a 2043 6f6f  [bt.Tensor]: Coo
-00007bb0: 7264 696e 6174 6573 2074 6f20 6265 2074  rdinates to be t
-00007bc0: 7261 6e73 666f 726d 6564 2e0a 2020 2020  ransformed..    
-00007bd0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00007be0: 3a20 285b 6e5f 6261 7463 683a 6f70 7469  : ([n_batch:opti
-00007bf0: 6f6e 616c 5d2c 207b 6e5f 6469 6d7d 2c20  onal], {n_dim}, 
-00007c00: 6e5f 312c 206e 5f32 2c20 2e2e 2e2c 206e  n_1, n_2, ..., n
-00007c10: 5f72 290a 2020 2020 2020 2020 2020 2020  _r).            
-00007c20: 6f75 7470 7574 205b 6274 2e54 656e 736f  output [bt.Tenso
-00007c30: 725d 3a20 5468 6520 7472 616e 7366 6f72  r]: The transfor
-00007c40: 6d65 6420 636f 6f72 6469 6e61 7465 732e  med coordinates.
-00007c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c60: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00007c70: 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f 312c  ], {n_dim}, n_1,
-00007c80: 206e 5f32 2c20 2e2e 2e2c 206e 5f72 290a   n_2, ..., n_r).
-00007c90: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00007ca0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00007cb0: 6974 5f5f 2864 696d 733d 6469 6d2c 2069  it__(dims=dim, i
-00007cc0: 6d61 6765 5f73 697a 653d 696d 6167 655f  mage_size=image_
-00007cd0: 7369 7a65 290a 0a20 2020 2020 2020 2069  size)..        i
-00007ce0: 6620 6c65 6e28 6469 6d29 203d 3d20 3120  f len(dim) == 1 
-00007cf0: 616e 6420 6973 696e 7374 616e 6365 2864  and isinstance(d
-00007d00: 696d 5b30 5d2c 2028 6c69 7374 2c20 7475  im[0], (list, tu
-00007d10: 706c 6529 293a 2064 696d 203d 2064 696d  ple)): dim = dim
-00007d20: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
-00007d30: 2e64 696d 7320 3d20 6469 6d0a 2020 2020  .dims = dim.    
-00007d40: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00007d50: 6528 696d 6167 655f 7369 7a65 2c20 6274  e(image_size, bt
-00007d60: 2e74 6f72 6368 2e54 656e 736f 7229 3a20  .torch.Tensor): 
-00007d70: 696d 6167 655f 7369 7a65 203d 2069 6d61  image_size = ima
-00007d80: 6765 5f73 697a 652e 7368 6170 650a 2020  ge_size.shape.  
-00007d90: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
-00007da0: 5f73 697a 6520 3d20 696d 6167 655f 7369  _size = image_si
-00007db0: 7a65 0a20 2020 2020 2020 2069 6620 696d  ze.        if im
-00007dc0: 6167 655f 7369 7a65 2069 7320 6e6f 7420  age_size is not 
-00007dd0: 4e6f 6e65 3a20 7365 6c66 2e6e 5f64 696d  None: self.n_dim
-00007de0: 203d 206c 656e 2869 6d61 6765 5f73 697a   = len(image_siz
-00007df0: 6529 0a0a 2020 2020 6465 6620 5f5f 6361  e)..    def __ca
-00007e00: 6c6c 5f5f 2873 656c 662c 2058 293a 0a20  ll__(self, X):. 
-00007e10: 2020 2020 2020 2058 203d 2073 7570 6572         X = super
-00007e20: 2829 2e5f 5f63 616c 6c5f 5f28 5829 0a20  ().__call__(X). 
-00007e30: 2020 2020 2020 2064 696d 7320 3d20 7365         dims = se
-00007e40: 6c66 2e64 696d 730a 2020 2020 2020 2020  lf.dims.        
-00007e50: 666f 7220 6469 6d20 696e 2064 696d 733a  for dim in dims:
-00007e60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007e70: 6563 7420 3d20 2873 6c69 6365 284e 6f6e  ect = (slice(Non
-00007e80: 6529 2c29 202a 2058 2e63 6861 6e6e 656c  e),) * X.channel
-00007e90: 5f64 696d 202b 2028 6469 6d2c 290a 2020  _dim + (dim,).  
-00007ea0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00007eb0: 662e 696d 6167 655f 7369 7a65 2069 7320  f.image_size is 
-00007ec0: 4e6f 6e65 3a20 6d61 785f 7261 6e67 6520  None: max_range 
-00007ed0: 3d20 585b 7365 6c65 6374 5d2e 6d61 7828  = X[select].max(
-00007ee0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00007ef0: 7365 3a20 6d61 785f 7261 6e67 6520 3d20  se: max_range = 
-00007f00: 7365 6c66 2e69 6d61 6765 5f73 697a 655b  self.image_size[
-00007f10: 6469 6d5d 0a20 2020 2020 2020 2020 2020  dim].           
-00007f20: 2058 5b73 656c 6563 745d 203d 206d 6178   X[select] = max
-00007f30: 5f72 616e 6765 202d 2058 5b73 656c 6563  _range - X[selec
-00007f40: 745d 0a20 2020 2020 2020 2072 6574 7572  t].        retur
-00007f50: 6e20 580a 2020 2020 2020 2020 0a20 2020  n X.        .   
-00007f60: 2064 6566 2061 6666 696e 6528 7365 6c66   def affine(self
-00007f70: 2c20 6e5f 6469 6d3d 4e6f 6e65 293a 0a20  , n_dim=None):. 
-00007f80: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00007f90: 6d61 6765 5f73 697a 6520 6973 204e 6f6e  mage_size is Non
-00007fa0: 653a 2072 6574 7572 6e0a 2020 2020 2020  e: return.      
-00007fb0: 2020 6966 206e 5f64 696d 2069 7320 4e6f    if n_dim is No
-00007fc0: 6e65 2061 6e64 2073 656c 662e 6e5f 6469  ne and self.n_di
-00007fd0: 6d20 6973 204e 6f6e 653a 2072 6574 7572  m is None: retur
-00007fe0: 6e0a 2020 2020 2020 2020 6966 206e 5f64  n.        if n_d
-00007ff0: 696d 2069 7320 4e6f 6e65 3a20 6e5f 6469  im is None: n_di
-00008000: 6d20 3d20 7365 6c66 2e6e 5f64 696d 0a20  m = self.n_dim. 
-00008010: 2020 2020 2020 2061 766f 7563 6828 7365         avouch(se
-00008020: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
-00008030: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
-00008040: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
-00008050: 2061 6666 203d 2062 742e 6579 6528 6e5f   aff = bt.eye(n_
-00008060: 6469 6d20 2b20 3129 0a20 2020 2020 2020  dim + 1).       
-00008070: 2066 6f72 2064 696d 2069 6e20 7365 6c66   for dim in self
-00008080: 2e64 696d 733a 0a20 2020 2020 2020 2020  .dims:.         
-00008090: 2020 2061 6666 5b64 696d 5d5b 6469 6d5d     aff[dim][dim]
-000080a0: 203d 202d 312e 0a20 2020 2020 2020 2020   = -1..         
-000080b0: 2020 2061 6666 5b64 696d 5d5b 2d31 5d20     aff[dim][-1] 
-000080c0: 3d20 666c 6f61 7428 7365 6c66 2e69 6d61  = float(self.ima
-000080d0: 6765 5f73 697a 655b 6469 6d5d 290a 2020  ge_size[dim]).  
-000080e0: 2020 2020 2020 7265 7475 726e 2061 6666        return aff
-000080f0: 2e75 6e73 7175 6565 7a65 285b 5d29 0a0a  .unsqueeze([])..
-00008100: 2020 2020 6465 6620 696e 7628 7365 6c66      def inv(self
-00008110: 293a 2072 6574 7572 6e20 5265 666c 6563  ): return Reflec
-00008120: 7428 2a73 656c 662e 6469 6d73 2c20 696d  t(*self.dims, im
-00008130: 6167 655f 7369 7a65 203d 2073 656c 662e  age_size = self.
-00008140: 696d 6167 655f 7369 7a65 292e 6261 636b  image_size).back
-00008150: 7761 7264 5f28 7365 6c66 2e62 6163 6b77  ward_(self.backw
-00008160: 6172 6429 0a0a 4061 6c69 6173 2822 5065  ard)..@alias("Pe
-00008170: 726d 7574 6564 696d 2229 0a63 6c61 7373  rmutedim").class
-00008180: 2044 696d 5065 726d 7574 6174 696f 6e28   DimPermutation(
-00008190: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
-000081a0: 6174 696f 6e29 3a0a 2020 2020 6465 6620  ation):.    def 
-000081b0: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
-000081c0: 6469 6d73 2c20 7265 7369 7a65 5f69 6d61  dims, resize_ima
-000081d0: 6765 3d54 7275 6529 3a0a 2020 2020 2020  ge=True):.      
-000081e0: 2020 2727 270a 2020 2020 2020 2020 5065    '''.        Pe
-000081f0: 726d 7574 6520 7468 6520 6469 6d65 6e73  rmute the dimens
-00008200: 696f 6e73 2066 6f72 2061 6e20 696d 6167  ions for an imag
-00008210: 652c 2073 696d 696c 6172 2074 6f20 6e70  e, similar to np
-00008220: 2e74 7261 6e73 706f 7365 206f 7220 746f  .transpose or to
-00008230: 7263 682f 6261 746f 7263 682e 7065 726d  rch/batorch.perm
-00008240: 7574 652e 0a20 2020 2020 2020 200a 2020  ute..        .  
-00008250: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
-00008260: 2020 2020 2020 2020 2020 6469 6d73 205b            dims [
-00008270: 6c69 7374 206f 7220 7475 706c 6520 6f72  list or tuple or
-00008280: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
-00008290: 2064 696d 656e 7369 6f6e 2070 6572 6d75   dimension permu
-000082a0: 6174 696f 6e2e 200a 2020 2020 2020 2020  ation. .        
-000082b0: 2020 2020 2020 2020 7369 7a65 3a20 6c65          size: le
-000082c0: 6e67 7468 286e 5f64 696d 2920 6f72 2028  ngth(n_dim) or (
-000082d0: 5b6e 5f62 6174 6368 3a6f 7074 696f 6e61  [n_batch:optiona
-000082e0: 6c5d 2c20 7b6e 5f64 696d 7d29 2e0a 0a20  l], {n_dim})... 
-000082f0: 2020 2020 2020 2057 6865 6e20 6974 2069         When it i
-00008300: 7320 6361 6c6c 6564 3a0a 2020 2020 2020  s called:.      
-00008310: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
-00008320: 6f72 5d3a 2043 6f6f 7264 696e 6174 6573  or]: Coordinates
-00008330: 2074 6f20 6265 2074 7261 6e73 666f 726d   to be transform
-00008340: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00008350: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00008360: 7463 683a 6f70 7469 6f6e 616c 5d2c 207b  tch:optional], {
-00008370: 6e5f 6469 6d7d 2c20 6e5f 312c 206e 5f32  n_dim}, n_1, n_2
-00008380: 2c20 2e2e 2e2c 206e 5f72 290a 2020 2020  , ..., n_r).    
-00008390: 2020 2020 2020 2020 6f75 7470 7574 205b          output [
-000083a0: 6274 2e54 656e 736f 725d 3a20 5468 6520  bt.Tensor]: The 
-000083b0: 7472 616e 7366 6f72 6d65 6420 636f 6f72  transformed coor
-000083c0: 6469 6e61 7465 732e 0a20 2020 2020 2020  dinates..       
-000083d0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-000083e0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-000083f0: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
-00008400: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
-00008410: 2727 270a 2020 2020 2020 2020 6966 206c  '''.        if l
-00008420: 656e 2864 696d 7329 203d 3d20 313a 2064  en(dims) == 1: d
-00008430: 696d 7320 3d20 6469 6d73 5b30 5d0a 2020  ims = dims[0].  
-00008440: 2020 2020 2020 6469 6d73 203d 2062 6174        dims = bat
-00008450: 6f72 6368 5f74 656e 736f 7228 6c69 7374  orch_tensor(list
-00008460: 2864 696d 7329 292e 7371 7565 657a 6528  (dims)).squeeze(
-00008470: 290a 2020 2020 2020 2020 6469 6d73 203d  ).        dims =
-00008480: 2064 696d 732e 6c6f 6e67 2829 0a20 2020   dims.long().   
-00008490: 2020 2020 2069 6620 6469 6d73 2e6e 5f64       if dims.n_d
-000084a0: 696d 203c 3d20 313a 2064 696d 7320 3d20  im <= 1: dims = 
-000084b0: 6469 6d73 2e75 6e73 7175 6565 7a65 285b  dims.unsqueeze([
-000084c0: 5d29 0a20 2020 2020 2020 2069 6620 6469  ]).        if di
-000084d0: 6d73 2e6e 5f64 696d 203d 3d20 323a 0a20  ms.n_dim == 2:. 
-000084e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000084f0: 7420 6469 6d73 2e68 6173 5f62 6174 6368  t dims.has_batch
-00008500: 3a20 6469 6d73 2e62 6174 6368 5f64 696d  : dims.batch_dim
-00008510: 656e 7369 6f6e 203d 2030 0a20 2020 2020  ension = 0.     
-00008520: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
-00008530: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
-00008540: 6469 6d73 2e63 6861 6e6e 656c 5f64 696d  dims.channel_dim
-00008550: 656e 7369 6f6e 203d 2030 2069 6620 6469  ension = 0 if di
-00008560: 6d73 2e62 6174 6368 5f64 696d 656e 7369  ms.batch_dimensi
-00008570: 6f6e 203e 2030 2065 6c73 6520 310a 2020  on > 0 else 1.  
-00008580: 2020 2020 2020 6176 6f75 6368 2864 696d        avouch(dim
-00008590: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
-000085a0: 6469 6d73 2e68 6173 5f63 6861 6e6e 656c  dims.has_channel
-000085b0: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
-000085c0: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-000085d0: 2073 697a 6520 5c0a 2020 2020 2020 2020   size \.        
-000085e0: 2020 2020 285b 6e5f 6261 7463 683a 6f70      ([n_batch:op
-000085f0: 7469 6f6e 616c 5d2c 207b 7b6e 5f64 696d  tional], {{n_dim
-00008600: 7d7d 2920 666f 7220 5472 616e 736c 6174  }}) for Translat
-00008610: 696f 6e20 7061 7261 6d65 7465 7273 2c20  ion parameters, 
-00008620: 696e 7374 6561 6420 6f66 207b 6469 6d73  instead of {dims
-00008630: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-00008640: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00008650: 6974 5f5f 2864 696d 732c 2072 6573 697a  it__(dims, resiz
-00008660: 655f 696d 6167 653d 7265 7369 7a65 5f69  e_image=resize_i
-00008670: 6d61 6765 290a 0a20 2020 2020 2020 2073  mage)..        s
-00008680: 656c 662e 6469 6d73 203d 2064 696d 730a  elf.dims = dims.
-00008690: 2020 2020 2020 2020 7365 6c66 2e6e 5f64          self.n_d
-000086a0: 696d 203d 2064 696d 732e 6e5f 6368 616e  im = dims.n_chan
-000086b0: 6e65 6c0a 2020 2020 2020 2020 7365 6c66  nel.        self
-000086c0: 2e72 6573 697a 655f 696d 6167 6520 3d20  .resize_image = 
-000086d0: 7265 7369 7a65 5f69 6d61 6765 0a20 2020  resize_image.   
-000086e0: 2020 2020 2069 6620 7265 7369 7a65 5f69       if resize_i
-000086f0: 6d61 6765 3a0a 2020 2020 2020 2020 2020  mage:.          
-00008700: 2020 6966 2064 696d 732e 6e5f 6261 7463    if dims.n_batc
-00008710: 6820 3e20 313a 0a20 2020 2020 2020 2020  h > 1:.         
-00008720: 2020 2020 2020 2064 696d 735f 6361 7020         dims_cap 
-00008730: 3d20 6469 6d73 2e73 616d 706c 6528 7261  = dims.sample(ra
-00008740: 6e64 6f6d 3d46 616c 7365 2c20 6469 6d3d  ndom=False, dim=
-00008750: 5b5d 290a 2020 2020 2020 2020 2020 2020  []).            
-00008760: 2020 2020 6176 6f75 6368 2862 742e 6e6f      avouch(bt.no
-00008770: 726d 2864 696d 7320 2d20 6469 6d73 5f63  rm(dims - dims_c
-00008780: 6170 292e 7375 6d28 2920 3c20 3165 2d34  ap).sum() < 1e-4
-00008790: 2c20 2243 616e 6e6f 7420 7265 7369 7a65  , "Cannot resize
-000087a0: 2069 6d61 6765 2077 6865 6e20 6469 6666   image when diff
-000087b0: 6572 656e 7420 7065 726d 7574 6174 696f  erent permutatio
-000087c0: 6e20 646f 6e65 2066 6f72 2064 6966 6665  n done for diffe
-000087d0: 7265 6e74 2062 6174 6368 206d 656d 6265  rent batch membe
-000087e0: 7273 2e20 2229 0a20 2020 2020 2020 2020  rs. ").         
-000087f0: 2020 2064 696d 7320 3d20 6469 6d73 2e70     dims = dims.p
-00008800: 6963 6b28 302c 205b 5d29 2e74 6f6c 6973  ick(0, []).tolis
-00008810: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00008820: 7669 7369 7465 6420 3d20 5b5d 0a20 2020  visited = [].   
-00008830: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00008840: 7368 6170 6520 3d20 5b28 312c 295d 0a20  shape = [(1,)]. 
-00008850: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-00008860: 2069 6e20 7261 6e67 6528 7365 6c66 2e6e   in range(self.n
-00008870: 5f64 696d 293a 0a20 2020 2020 2020 2020  _dim):.         
-00008880: 2020 2020 2020 2069 6620 7020 696e 2076         if p in v
-00008890: 6973 6974 6564 3a20 636f 6e74 696e 7565  isited: continue
-000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088b0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 2076 6973 6974 6564 2e61 7070 656e 6428   visited.append(
-000088e0: 7029 0a20 2020 2020 2020 2020 2020 2020  p).             
-000088f0: 2020 2020 2020 2071 203d 2064 696d 735b         q = dims[
-00008900: 705d 0a20 2020 2020 2020 2020 2020 2020  p].             
-00008910: 2020 2020 2020 2069 6620 7120 696e 2076         if q in v
-00008920: 6973 6974 6564 3a20 6272 6561 6b0a 2020  isited: break.  
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 2020 7365 6c66 2e72 6573 6861 7065 2e61    self.reshape.a
-00008950: 7070 656e 6428 2870 2c20 7129 290a 2020  ppend((p, q)).  
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 2020 7020 3d20 710a 0a20 2020 2064 6566    p = q..    def
-00008980: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-00008990: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
-000089a0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
-000089b0: 2858 290a 2020 2020 2020 2020 7265 7475  (X).        retu
-000089c0: 726e 2058 2e67 6174 6865 7228 582e 6368  rn X.gather(X.ch
-000089d0: 616e 6e65 6c5f 6469 6d65 6e73 696f 6e2c  annel_dimension,
-000089e0: 2073 656c 662e 6469 6d73 2e65 7870 616e   self.dims.expan
-000089f0: 645f 746f 2858 2929 0a20 2020 2020 2020  d_to(X)).       
-00008a00: 200a 2020 2020 6465 6620 6166 6669 6e65   .    def affine
-00008a10: 2873 656c 662c 206e 5f64 696d 3d4e 6f6e  (self, n_dim=Non
-00008a20: 6529 3a0a 2020 2020 2020 2020 6176 6f75  e):.        avou
-00008a30: 6368 286e 5f64 696d 2069 7320 4e6f 6e65  ch(n_dim is None
-00008a40: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
-00008a50: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
-00008a60: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
-00008a70: 653a 206e 5f64 696d 203d 2073 656c 662e  e: n_dim = self.
-00008a80: 6e5f 6469 6d0a 2020 2020 2020 2020 6e5f  n_dim.        n_
-00008a90: 6261 7463 6820 3d20 7365 6c66 2e6e 5f62  batch = self.n_b
-00008aa0: 6174 6368 0a20 2020 2020 2020 2069 6620  atch.        if 
-00008ab0: 6e5f 6261 7463 6820 6973 204e 6f6e 653a  n_batch is None:
-00008ac0: 206e 5f62 6174 6368 203d 2031 0a20 2020   n_batch = 1.   
-00008ad0: 2020 2020 2061 6666 203d 2062 742e 6469       aff = bt.di
-00008ae0: 6167 2862 742e 6f6e 655f 686f 7428 2d31  ag(bt.one_hot(-1
-00008af0: 2c20 6e5f 6469 6d20 2b20 3129 2e66 6c6f  , n_dim + 1).flo
-00008b00: 6174 2829 2e6d 756c 7469 706c 7928 6e5f  at().multiply(n_
-00008b10: 6261 7463 682c 205b 5d29 290a 2020 2020  batch, [])).    
-00008b20: 2020 2020 6220 3d20 6274 2e62 6174 6368      b = bt.batch
-00008b30: 5f74 656e 736f 7228 6274 2e61 7261 6e67  _tensor(bt.arang
-00008b40: 6528 6e5f 6261 7463 6829 292e 6578 7061  e(n_batch)).expa
-00008b50: 6e64 5f74 6f28 7365 6c66 2e64 696d 7329  nd_to(self.dims)
-00008b60: 0a20 2020 2020 2020 2069 203d 2062 742e  .        i = bt.
-00008b70: 6172 616e 6765 286e 5f64 696d 292e 6d75  arange(n_dim).mu
-00008b80: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
-00008b90: 5b5d 290a 2020 2020 2020 2020 6166 665b  []).        aff[
-00008ba0: 622c 2069 2c20 7365 6c66 2e64 696d 735d  b, i, self.dims]
-00008bb0: 203d 2031 2e0a 2020 2020 2020 2020 7265   = 1..        re
-00008bc0: 7475 726e 2061 6666 0a0a 2020 2020 6465  turn aff..    de
-00008bd0: 6620 696e 7628 7365 6c66 293a 0a20 2020  f inv(self):.   
-00008be0: 2020 2020 206e 5f64 696d 203d 2073 656c       n_dim = sel
-00008bf0: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
-00008c00: 6e65 775f 7065 726d 7574 6520 3d20 2873  new_permute = (s
-00008c10: 656c 662e 6469 6d73 203d 3d20 6274 2e61  elf.dims == bt.a
-00008c20: 7261 6e67 6528 6e5f 6469 6d29 2e76 6965  range(n_dim).vie
-00008c30: 7728 5b31 5d2c 206e 5f64 696d 2c20 7b31  w([1], n_dim, {1
-00008c40: 7d29 292e 666c 6f61 7428 292e 6172 676d  })).float().argm
-00008c50: 6178 282d 3129 2e63 6861 6e6e 656c 5f64  ax(-1).channel_d
-00008c60: 696d 656e 7369 6f6e 5f28 2d31 290a 2020  imension_(-1).  
-00008c70: 2020 2020 2020 7265 7475 726e 2050 6572        return Per
-00008c80: 6d75 7465 6469 6d28 6e65 775f 7065 726d  mutedim(new_perm
-00008c90: 7574 652c 2072 6573 697a 655f 696d 6167  ute, resize_imag
-00008ca0: 6520 3d20 7365 6c66 2e72 6573 697a 655f  e = self.resize_
-00008cb0: 696d 6167 6529 2e62 6163 6b77 6172 645f  image).backward_
-00008cc0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
-00008cd0: 0a40 616c 6961 7328 2252 6573 6361 6c65  .@alias("Rescale
-00008ce0: 2229 0a63 6c61 7373 2052 6573 6361 6c69  ").class Rescali
-00008cf0: 6e67 2853 7061 7469 616c 5472 616e 7366  ng(SpatialTransf
-00008d00: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
-00008d10: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00008d20: 2c20 2a73 6361 6c65 2c20 7265 7369 7a65  , *scale, resize
-00008d30: 5f69 6d61 6765 3d54 7275 6529 3a0a 2020  _image=True):.  
-00008d40: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00008d50: 2020 5363 616c 6520 616e 2069 6d61 6765    Scale an image
-00008d60: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00008d70: 2020 204e 6f74 653a 2054 6865 2073 6361     Note: The sca
-00008d80: 6c69 6e67 2069 7320 666f 7220 636f 6f72  ling is for coor
-00008d90: 6469 6e61 7465 732c 2068 656e 6365 2074  dinates, hence t
-00008da0: 6865 2069 6d61 6765 2077 6f75 6c64 2073  he image would s
-00008db0: 6872 696e 6b20 6966 2073 6361 6c65 203e  hrink if scale >
-00008dc0: 2031 2e20 0a20 2020 2020 2020 200a 2020   1. .        .  
-00008dd0: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
-00008de0: 2020 2020 2020 2020 2020 7363 616c 6520            scale 
-00008df0: 5b66 6c6f 6174 206f 7220 7475 706c 6520  [float or tuple 
-00008e00: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
-00008e10: 6865 2073 6361 6c69 6e67 2066 6f72 2061  he scaling for a
-00008e20: 6c6c 2064 696d 656e 7369 6f6e 7320 2866  ll dimensions (f
-00008e30: 6c6f 6174 2920 0a20 2020 2020 2020 2020  loat) .         
-00008e40: 2020 2020 2020 206f 7220 666f 7220 6561         or for ea
-00008e50: 6368 2064 696d 656e 7369 6f6e 2028 7475  ch dimension (tu
-00008e60: 706c 6529 2e20 3e31 206d 6561 6e73 2065  ple). >1 means e
-00008e70: 6e6c 6172 6769 6e67 2074 6865 2063 6f6f  nlarging the coo
-00008e80: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
-00008e90: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00008ea0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
-00008eb0: 616c 5d2c 207b 6e5f 6469 6d7d 2920 666f  al], {n_dim}) fo
-00008ec0: 7220 6274 2e54 656e 736f 722e 0a20 2020  r bt.Tensor..   
-00008ed0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00008ee0: 2020 5768 656e 2069 7420 6973 2063 616c    When it is cal
-00008ef0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00008f00: 2058 205b 6274 2e54 656e 736f 725d 3a20   X [bt.Tensor]: 
-00008f10: 436f 6f72 6469 6e61 7465 7320 746f 2062  Coordinates to b
-00008f20: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
-00008f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008f40: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
-00008f50: 7074 696f 6e61 6c5d 2c20 7b6e 5f64 696d  ptional], {n_dim
-00008f60: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
-00008f70: 2c20 6e5f 7229 0a20 2020 2020 2020 2020  , n_r).         
-00008f80: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
-00008f90: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
-00008fa0: 666f 726d 6564 2063 6f6f 7264 696e 6174  formed coordinat
-00008fb0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-00008fc0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00008fd0: 7463 685d 2c20 7b6e 5f64 696d 7d2c 206e  tch], {n_dim}, n
-00008fe0: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-00008ff0: 7229 0a20 2020 2020 2020 2027 2727 0a20  r).        '''. 
-00009000: 2020 2020 2020 2069 6620 6c65 6e28 7363         if len(sc
-00009010: 616c 6529 203d 3d20 3120 616e 6420 6973  ale) == 1 and is
-00009020: 696e 7374 616e 6365 2873 6361 6c65 5b30  instance(scale[0
-00009030: 5d2c 2028 696e 742c 2066 6c6f 6174 2929  ], (int, float))
-00009040: 3a20 7363 616c 6520 3d20 7363 616c 655b  : scale = scale[
-00009050: 305d 202a 2062 742e 6f6e 6573 285b 315d  0] * bt.ones([1]
-00009060: 2c20 7b31 7d29 0a20 2020 2020 2020 2065  , {1}).        e
-00009070: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009080: 2069 6620 6c65 6e28 7363 616c 6529 203d   if len(scale) =
-00009090: 3d20 313a 2073 6361 6c65 203d 2073 6361  = 1: scale = sca
-000090a0: 6c65 5b30 5d0a 2020 2020 2020 2020 2020  le[0].          
-000090b0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-000090c0: 6e63 6528 7363 616c 652c 2062 742e 5465  nce(scale, bt.Te
-000090d0: 6e73 6f72 293a 2073 6361 6c65 203d 2062  nsor): scale = b
-000090e0: 6174 6f72 6368 5f74 656e 736f 7228 6c69  atorch_tensor(li
-000090f0: 7374 2873 6361 6c65 2929 2e73 7175 6565  st(scale)).squee
-00009100: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
-00009110: 2069 6620 7363 616c 652e 6e5f 6469 6d20   if scale.n_dim 
-00009120: 3c3d 2031 3a20 7363 616c 6520 3d20 7363  <= 1: scale = sc
-00009130: 616c 652e 756e 7371 7565 657a 6528 5b5d  ale.unsqueeze([]
-00009140: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00009150: 2073 6361 6c65 2e6e 5f64 696d 203d 3d20   scale.n_dim == 
-00009160: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-00009170: 2020 2069 6620 6e6f 7420 7363 616c 652e     if not scale.
-00009180: 6861 735f 6261 7463 683a 2073 6361 6c65  has_batch: scale
-00009190: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-000091a0: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
-000091b0: 2020 2020 2069 6620 6e6f 7420 7363 616c       if not scal
-000091c0: 652e 6861 735f 6368 616e 6e65 6c3a 2073  e.has_channel: s
-000091d0: 6361 6c65 2e63 6861 6e6e 656c 5f64 696d  cale.channel_dim
-000091e0: 656e 7369 6f6e 203d 2030 2069 6620 7363  ension = 0 if sc
-000091f0: 616c 652e 6261 7463 685f 6469 6d65 6e73  ale.batch_dimens
-00009200: 696f 6e20 3e20 3020 656c 7365 2031 0a20  ion > 0 else 1. 
-00009210: 2020 2020 2020 2061 766f 7563 6828 7363         avouch(sc
-00009220: 616c 652e 6861 735f 6261 7463 6820 616e  ale.has_batch an
-00009230: 6420 7363 616c 652e 6861 735f 6368 616e  d scale.has_chan
-00009240: 6e65 6c2c 2066 2250 6c65 6173 6520 7573  nel, f"Please us
-00009250: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-00009260: 206f 6620 7369 7a65 205c 0a20 2020 2020   of size \.     
-00009270: 2020 2020 2020 2028 5b6e 5f62 6174 6368         ([n_batch
-00009280: 3a6f 7074 696f 6e61 6c5d 2c20 7b7b 6e5f  :optional], {{n_
-00009290: 6469 6d7d 7d29 2066 6f72 2053 6361 6c69  dim}}) for Scali
-000092a0: 6e67 2070 6172 616d 6574 6572 732c 2069  ng parameters, i
-000092b0: 6e73 7465 6164 206f 6620 7b73 6361 6c65  nstead of {scale
-000092c0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-000092d0: 2020 2020 6274 2e74 6f5f 6465 7669 6365      bt.to_device
-000092e0: 2873 6361 6c65 290a 2020 2020 2020 2020  (scale).        
-000092f0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00009300: 2873 6361 6c65 2c20 7265 7369 7a65 5f69  (scale, resize_i
-00009310: 6d61 6765 3d72 6573 697a 655f 696d 6167  mage=resize_imag
-00009320: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00009330: 2e73 6361 6c65 203d 2073 6361 6c65 0a20  .scale = scale. 
-00009340: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00009350: 6361 6c65 2e6e 5f63 6861 6e6e 656c 203e  cale.n_channel >
-00009360: 2031 3a20 7365 6c66 2e6e 5f64 696d 203d   1: self.n_dim =
-00009370: 2073 656c 662e 7363 616c 652e 6e5f 6368   self.scale.n_ch
-00009380: 616e 6e65 6c0a 2020 2020 2020 2020 6966  annel.        if
-00009390: 2072 6573 697a 655f 696d 6167 653a 0a20   resize_image:. 
-000093a0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-000093b0: 203d 2073 6361 6c65 2e73 7175 6565 7a65   = scale.squeeze
-000093c0: 285b 5d29 0a20 2020 2020 2020 2020 2020  ([]).           
-000093d0: 2061 766f 7563 6828 7363 616c 652e 6e64   avouch(scale.nd
-000093e0: 696d 203d 3d20 3129 0a20 2020 2020 2020  im == 1).       
-000093f0: 2020 2020 2073 656c 662e 7265 7368 6170       self.reshap
-00009400: 6520 3d20 5b74 7570 6c65 2828 312f 7363  e = [tuple((1/sc
-00009410: 616c 6529 2e74 6f6c 6973 7428 2929 5d0a  ale).tolist())].
-00009420: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00009430: 697a 655f 696d 6167 6520 3d20 7265 7369  ize_image = resi
-00009440: 7a65 5f69 6d61 6765 0a20 2020 2020 2020  ze_image.       
-00009450: 2073 656c 662e 6261 7463 685f 7061 7261   self.batch_para
-00009460: 6d2e 6170 7065 6e64 2827 7363 616c 6527  m.append('scale'
-00009470: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
-00009480: 6c5f 5f28 7365 6c66 2c20 5829 3a0a 2020  l__(self, X):.  
-00009490: 2020 2020 2020 5820 3d20 7375 7065 7228        X = super(
-000094a0: 292e 5f5f 6361 6c6c 5f5f 2858 290a 2020  ).__call__(X).  
-000094b0: 2020 2020 2020 7363 616c 6520 3d20 7365        scale = se
-000094c0: 6c66 2e73 6361 6c65 0a20 2020 2020 2020  lf.scale.       
-000094d0: 2072 6574 7572 6e20 5820 2a20 7363 616c   return X * scal
-000094e0: 650a 2020 2020 0a20 2020 2064 6566 2061  e.    .    def a
-000094f0: 6666 696e 6528 7365 6c66 2c20 6e5f 6469  ffine(self, n_di
-00009500: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00009510: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
-00009520: 6520 616e 6420 7365 6c66 2e6e 5f64 696d  e and self.n_dim
-00009530: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
-00009540: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
-00009550: 6d20 6973 204e 6f6e 653a 206e 5f64 696d  m is None: n_dim
-00009560: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
-00009570: 2020 2020 2020 6176 6f75 6368 2873 656c        avouch(sel
-00009580: 662e 6e5f 6469 6d20 6973 204e 6f6e 6520  f.n_dim is None 
-00009590: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
-000095a0: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
-000095b0: 7363 616c 6520 3d20 7365 6c66 2e73 6361  scale = self.sca
-000095c0: 6c65 0a20 2020 2020 2020 2069 6620 6973  le.        if is
-000095d0: 696e 7374 616e 6365 2873 6361 6c65 2c20  instance(scale, 
-000095e0: 2869 6e74 2c20 666c 6f61 7429 293a 2072  (int, float)): r
-000095f0: 6574 7572 6e20 7363 616c 6520 2a20 6274  eturn scale * bt
-00009600: 2e65 7965 286e 5f64 696d 202b 2031 290a  .eye(n_dim + 1).
-00009610: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00009620: 742e 6469 6167 2862 742e 6361 7428 7363  t.diag(bt.cat(sc
-00009630: 616c 652c 2062 742e 6f6e 6573 285b 7363  ale, bt.ones([sc
-00009640: 616c 652e 6e5f 6261 7463 685d 2c20 3129  ale.n_batch], 1)
-00009650: 2c20 3129 290a 0a20 2020 2064 6566 2069  , 1))..    def i
-00009660: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
-00009670: 2052 6573 6361 6c65 2831 2f73 656c 662e   Rescale(1/self.
-00009680: 7363 616c 652c 2072 6573 697a 655f 696d  scale, resize_im
-00009690: 6167 6520 3d20 7365 6c66 2e72 6573 697a  age = self.resiz
-000096a0: 655f 696d 6167 6529 2e62 6163 6b77 6172  e_image).backwar
-000096b0: 645f 2873 656c 662e 6261 636b 7761 7264  d_(self.backward
-000096c0: 290a 0a40 616c 6961 7328 2254 7261 6e73  )..@alias("Trans
-000096d0: 6c61 7465 2229 0a63 6c61 7373 2054 7261  late").class Tra
-000096e0: 6e73 6c61 7469 6f6e 2853 7061 7469 616c  nslation(Spatial
-000096f0: 5472 616e 7366 6f72 6d61 7469 6f6e 293a  Transformation):
-00009700: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00009710: 5f28 7365 6c66 2c20 2a74 7261 6e73 6c61  _(self, *transla
-00009720: 7469 6f6e 293a 0a20 2020 2020 2020 2027  tion):.        '
-00009730: 2727 0a20 2020 2020 2020 2054 7261 6e73  ''.        Trans
-00009740: 6c61 7465 2061 6e20 696d 6167 652e 0a20  late an image.. 
-00009750: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009760: 4e6f 7465 3a20 5468 6520 7472 616e 736c  Note: The transl
-00009770: 6174 696f 6e20 6973 2066 6f72 2063 6f6f  ation is for coo
-00009780: 7264 696e 6174 6573 2c20 6865 6e63 6520  rdinates, hence 
-00009790: 7468 6520 696d 6167 6520 776f 756c 6420  the image would 
-000097a0: 676f 2069 6e20 7468 6520 6f70 706f 7369  go in the opposi
-000097b0: 7465 2064 6972 6563 7469 6f6e 2e20 0a20  te direction. . 
-000097c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000097d0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-000097e0: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
-000097f0: 5b74 7570 6c65 206f 7220 6274 2e54 656e  [tuple or bt.Ten
-00009800: 736f 725d 3a20 5468 6520 7472 616e 736c  sor]: The transl
-00009810: 6174 696f 6e20 6f66 2074 6865 2063 6f6f  ation of the coo
-00009820: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
-00009830: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00009840: 6c65 6e67 7468 286e 5f64 696d 2920 6f72  length(n_dim) or
-00009850: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00009860: 6e61 6c5d 2c20 7b6e 5f64 696d 7d29 0a20  nal], {n_dim}). 
-00009870: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00009880: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
-00009890: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
-000098a0: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
-000098b0: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
-000098c0: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
-000098d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098e0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-000098f0: 3a6f 7074 696f 6e61 6c5d 2c20 7b6e 5f64  :optional], {n_d
-00009900: 696d 7d2c 206e 5f31 2c20 6e5f 322c 202e  im}, n_1, n_2, .
-00009910: 2e2e 2c20 6e5f 7229 0a20 2020 2020 2020  .., n_r).       
-00009920: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
-00009930: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
-00009940: 6e73 666f 726d 6564 2063 6f6f 7264 696e  nsformed coordin
-00009950: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-00009960: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-00009970: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
-00009980: 206e 5f31 2c20 6e5f 322c 202e 2e2e 2c20   n_1, n_2, ..., 
-00009990: 6e5f 7229 0a20 2020 2020 2020 2027 2727  n_r).        '''
-000099a0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-000099b0: 7472 616e 736c 6174 696f 6e29 203d 3d20  translation) == 
-000099c0: 313a 2074 7261 6e73 6c61 7469 6f6e 203d  1: translation =
-000099d0: 2074 7261 6e73 6c61 7469 6f6e 5b30 5d0a   translation[0].
-000099e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000099f0: 7461 6e63 6528 7472 616e 736c 6174 696f  tance(translatio
-00009a00: 6e2c 2074 7570 6c65 293a 2074 7261 6e73  n, tuple): trans
-00009a10: 6c61 7469 6f6e 203d 206c 6973 7428 7472  lation = list(tr
-00009a20: 616e 736c 6174 696f 6e29 0a20 2020 2020  anslation).     
-00009a30: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
-00009a40: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
-00009a50: 7472 616e 736c 6174 696f 6e29 2e73 7175  translation).squ
-00009a60: 6565 7a65 2829 0a20 2020 2020 2020 2069  eeze().        i
-00009a70: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
-00009a80: 6469 6d20 3c3d 2031 3a20 7472 616e 736c  dim <= 1: transl
-00009a90: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
-00009aa0: 696f 6e2e 756e 7371 7565 657a 6528 5b5d  ion.unsqueeze([]
-00009ab0: 290a 2020 2020 2020 2020 6966 2074 7261  ).        if tra
-00009ac0: 6e73 6c61 7469 6f6e 2e6e 5f64 696d 203d  nslation.n_dim =
-00009ad0: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-00009ae0: 2069 6620 6e6f 7420 7472 616e 736c 6174   if not translat
-00009af0: 696f 6e2e 6861 735f 6261 7463 683a 2074  ion.has_batch: t
-00009b00: 7261 6e73 6c61 7469 6f6e 2e62 6174 6368  ranslation.batch
-00009b10: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
-00009b20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00009b30: 7420 7472 616e 736c 6174 696f 6e2e 6861  t translation.ha
-00009b40: 735f 6368 616e 6e65 6c3a 2074 7261 6e73  s_channel: trans
-00009b50: 6c61 7469 6f6e 2e63 6861 6e6e 656c 5f64  lation.channel_d
-00009b60: 696d 656e 7369 6f6e 203d 2030 2069 6620  imension = 0 if 
-00009b70: 7472 616e 736c 6174 696f 6e2e 6261 7463  translation.batc
-00009b80: 685f 6469 6d65 6e73 696f 6e20 3e20 3020  h_dimension > 0 
-00009b90: 656c 7365 2031 0a20 2020 2020 2020 2061  else 1.        a
-00009ba0: 766f 7563 6828 7472 616e 736c 6174 696f  vouch(translatio
-00009bb0: 6e2e 6861 735f 6261 7463 6820 616e 6420  n.has_batch and 
-00009bc0: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
-00009bd0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
-00009be0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
-00009bf0: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
-00009c00: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
-00009c10: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-00009c20: 7b7b 6e5f 6469 6d7d 7d29 2066 6f72 2054  {{n_dim}}) for T
-00009c30: 7261 6e73 6c61 7469 6f6e 2070 6172 616d  ranslation param
-00009c40: 6574 6572 732c 2069 6e73 7465 6164 206f  eters, instead o
-00009c50: 6620 7b74 7261 6e73 6c61 7469 6f6e 2e73  f {translation.s
-00009c60: 6861 7065 7d2e 2022 290a 2020 2020 2020  hape}. ").      
-00009c70: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00009c80: 5f5f 2874 7261 6e73 6c61 7469 6f6e 290a  __(translation).
-00009c90: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
-00009ca0: 616e 736c 6174 696f 6e20 3d20 7472 616e  anslation = tran
-00009cb0: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
-00009cc0: 7365 6c66 2e6e 5f64 696d 203d 2073 656c  self.n_dim = sel
-00009cd0: 662e 7472 616e 736c 6174 696f 6e2e 6e5f  f.translation.n_
-00009ce0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
-00009cf0: 7365 6c66 2e62 6174 6368 5f70 6172 616d  self.batch_param
-00009d00: 2e61 7070 656e 6428 2774 7261 6e73 6c61  .append('transla
-00009d10: 7469 6f6e 2729 0a0a 2020 2020 6465 6620  tion')..    def 
-00009d20: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
-00009d30: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
-00009d40: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-00009d50: 5829 0a20 2020 2020 2020 2072 6574 7572  X).        retur
-00009d60: 6e20 5820 2b20 7365 6c66 2e74 7261 6e73  n X + self.trans
-00009d70: 6c61 7469 6f6e 0a20 2020 200a 2020 2020  lation.    .    
-00009d80: 6465 6620 6166 6669 6e65 2873 656c 662c  def affine(self,
-00009d90: 206e 5f64 696d 3d4e 6f6e 6529 3a0a 2020   n_dim=None):.  
-00009da0: 2020 2020 2020 6176 6f75 6368 286e 5f64        avouch(n_d
-00009db0: 696d 2069 7320 4e6f 6e65 206f 7220 7365  im is None or se
-00009dc0: 6c66 2e6e 5f64 696d 203d 3d20 6e5f 6469  lf.n_dim == n_di
-00009dd0: 6d29 0a20 2020 2020 2020 2069 6620 6e5f  m).        if n_
-00009de0: 6469 6d20 6973 204e 6f6e 653a 206e 5f64  dim is None: n_d
-00009df0: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
-00009e00: 2020 2020 2020 2020 6e5f 6261 7463 6820          n_batch 
-00009e10: 3d20 7365 6c66 2e74 7261 6e73 6c61 7469  = self.translati
-00009e20: 6f6e 2e6e 5f62 6174 6368 0a20 2020 2020  on.n_batch.     
-00009e30: 2020 2072 6574 7572 6e20 6274 2e63 6174     return bt.cat
-00009e40: 2862 742e 6361 7428 6274 2e65 7965 2873  (bt.cat(bt.eye(s
-00009e50: 656c 662e 6e5f 6469 6d29 2e6d 756c 7469  elf.n_dim).multi
-00009e60: 706c 7928 6e5f 6261 7463 682c 205b 5d29  ply(n_batch, [])
-00009e70: 2c20 7365 6c66 2e74 7261 6e73 6c61 7469  , self.translati
-00009e80: 6f6e 2e77 6974 685f 6368 616e 6e65 6c64  on.with_channeld
-00009e90: 696d 284e 6f6e 6529 2e75 6e73 7175 6565  im(None).unsquee
-00009ea0: 7a65 282d 3129 2c20 2d31 292c 2062 742e  ze(-1), -1), bt.
-00009eb0: 6f6e 655f 686f 7428 2d31 2c20 6e5f 6469  one_hot(-1, n_di
-00009ec0: 6d2b 3129 2e75 6e73 7175 6565 7a65 2830  m+1).unsqueeze(0
-00009ed0: 292e 6d75 6c74 6970 6c79 286e 5f62 6174  ).multiply(n_bat
-00009ee0: 6368 2c20 5b5d 292c 2031 290a 0a20 2020  ch, []), 1)..   
-00009ef0: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
-00009f00: 7265 7475 726e 2054 7261 6e73 6c61 7465  return Translate
-00009f10: 282d 7365 6c66 2e74 7261 6e73 6c61 7469  (-self.translati
-00009f20: 6f6e 292e 6261 636b 7761 7264 5f28 7365  on).backward_(se
-00009f30: 6c66 2e62 6163 6b77 6172 6429 0a0a 4061  lf.backward)..@a
-00009f40: 6c69 6173 2822 5269 6722 290a 636c 6173  lias("Rig").clas
-00009f50: 7320 5269 6769 6428 5370 6174 6961 6c54  s Rigid(SpatialT
-00009f60: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
-00009f70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00009f80: 2873 656c 662c 2061 6e67 6c65 2c20 6178  (self, angle, ax
-00009f90: 6973 3d4e 6f6e 652c 2074 7261 6e73 6c61  is=None, transla
-00009fa0: 7469 6f6e 3d4e 6f6e 652c 2063 656e 7465  tion=None, cente
-00009fb0: 723d 4e6f 6e65 2c20 7472 616e 735f 7374  r=None, trans_st
-00009fc0: 7265 7463 683d 4e6f 6e65 2c20 7370 6163  retch=None, spac
-00009fd0: 696e 673d 3129 3a0a 2020 2020 2020 2020  ing=1):.        
-00009fe0: 2727 270a 2020 2020 2020 2020 5269 6769  '''.        Rigi
-00009ff0: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
-0000a000: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
-0000a010: 2070 6172 616d 6574 6572 732e 0a20 2020   parameters..   
-0000a020: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-0000a030: 7261 6d73 2053 6574 2031 3a0a 2020 2020  rams Set 1:.    
-0000a040: 2020 2020 2020 2020 616e 676c 6520 5b62          angle [b
-0000a050: 742e 5465 6e73 6f72 206f 7220 6e70 2e6e  t.Tensor or np.n
-0000a060: 756d 7079 5d3a 2074 6865 205b 636c 6f63  umpy]: the [cloc
-0000a070: 6b77 6973 655d 2072 6f74 6174 696f 6e20  kwise] rotation 
-0000a080: 616e 676c 6573 2061 626f 7574 2074 6865  angles about the
-0000a090: 2061 7869 7365 7320 286f 7220 7a20 6469   axises (or z di
-0000a0a0: 7265 6374 696f 6e20 666f 7220 3244 292e  rection for 2D).
-0000a0b0: 2049 7420 6973 2063 6f75 6e74 6572 2d63   It is counter-c
-0000a0c0: 6c6f 636b 7769 7365 2066 6f72 2069 6d61  lockwise for ima
-0000a0d0: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
-0000a0e0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-0000a0f0: 7463 685d 2c29 0a20 2020 2020 2020 2020  tch],).         
-0000a100: 2020 2061 7869 7320 5b62 742e 5465 6e73     axis [bt.Tens
-0000a110: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
-0000a120: 2074 6865 2072 6f74 6174 696f 6e20 6178   the rotation ax
-0000a130: 6973 6573 2c20 6e6f 726d 616c 697a 6564  ises, normalized
-0000a140: 2076 6563 746f 7273 2c20 4e6f 6e65 2066   vectors, None f
-0000a150: 6f72 2032 442e 200a 2020 2020 2020 2020  or 2D. .        
-0000a160: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-0000a170: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
-0000a180: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
-0000a190: 7261 6e73 6c61 7469 6f6e 205b 6274 2e54  ranslation [bt.T
-0000a1a0: 656e 736f 7220 6f72 206e 702e 6e75 6d70  ensor or np.nump
-0000a1b0: 795d 3a20 7468 6520 7472 616e 736c 6174  y]: the translat
-0000a1c0: 696f 6e73 2061 6674 6572 2074 6865 2072  ions after the r
-0000a1d0: 6f74 6174 696f 6e2c 207a 6572 6f73 2062  otation, zeros b
-0000a1e0: 7920 6465 6661 756c 742e 200a 2020 2020  y default. .    
-0000a1f0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-0000a200: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-0000a210: 5f64 696d 7d29 0a20 2020 2020 2020 2020  _dim}).         
-0000a220: 2020 2063 656e 7465 7220 5b62 742e 5465     center [bt.Te
-0000a230: 6e73 6f72 206f 7220 6e70 2e6e 756d 7079  nsor or np.numpy
-0000a240: 5d3a 2074 6865 2063 656e 7465 7220 666f  ]: the center fo
-0000a250: 7220 7468 6520 726f 7461 7469 6f6e 732c  r the rotations,
-0000a260: 207a 6572 6f73 2062 7920 6465 6661 756c   zeros by defaul
-0000a270: 742e 200a 2020 2020 2020 2020 2020 2020  t. .            
-0000a280: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-0000a290: 7463 685d 2c20 7b6e 5f64 696d 7d29 0a20  tch], {n_dim}). 
-0000a2a0: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-0000a2b0: 5f73 7472 6574 6368 205b 696e 745d 3a20  _stretch [int]: 
-0000a2c0: 6f6e 6c79 2075 7365 6420 666f 7220 6974  only used for it
-0000a2d0: 6572 6174 6976 6520 7061 7261 6d65 7465  erative paramete
-0000a2e0: 7220 7472 6169 6e69 6e67 2c20 3120 6279  r training, 1 by
-0000a2f0: 2064 6566 6175 6c74 2e20 3230 2073 6565   default. 20 see
-0000a300: 6d73 2074 6f20 6265 2061 2067 6f6f 6420  ms to be a good 
-0000a310: 6368 6f69 6365 2e20 0a20 2020 2020 2020  choice. .       
-0000a320: 2020 2020 2073 7061 6369 6e67 205b 7475       spacing [tu
-0000a330: 706c 655d 3a20 7468 6520 7370 6163 696e  ple]: the spacin
-0000a340: 6720 6f66 2074 6865 2074 7261 6e73 666f  g of the transfo
-0000a350: 726d 6564 200a 2020 2020 2020 2020 0a20  rmed .        . 
-0000a360: 2020 2020 2020 2050 6172 616d 7320 5365         Params Se
-0000a370: 7420 323a 0a20 2020 2020 2020 2020 2020  t 2:.           
-0000a380: 206d 6174 7269 7820 5b62 742e 5465 6e73   matrix [bt.Tens
-0000a390: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
-0000a3a0: 2074 6865 2061 6666 696e 6520 6d61 7472   the affine matr
-0000a3b0: 6978 2c20 6974 2073 686f 756c 6420 6265  ix, it should be
-0000a3c0: 206f 7274 686f 676f 6e61 6c20 6f72 2077   orthogonal or w
-0000a3d0: 696c 6c20 6265 2070 726f 6a65 6374 6564  ill be projected
-0000a3e0: 2062 7920 5072 6f63 7275 7374 6573 2050   by Procrustes P
-0000a3f0: 726f 626c 656d 2e20 0a20 2020 2020 2020  roblem. .       
-0000a400: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-0000a410: 5b6e 5f62 6174 6368 5d2c 206e 5f64 696d  [n_batch], n_dim
-0000a420: 202b 2031 2c20 6e5f 6469 6d20 2b20 3129   + 1, n_dim + 1)
-0000a430: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-0000a440: 6e73 5f73 7472 6574 6368 205b 696e 745d  ns_stretch [int]
-0000a450: 3a20 6f6e 6c79 2075 7365 6420 666f 7220  : only used for 
-0000a460: 6974 6572 6174 6976 6520 7061 7261 6d65  iterative parame
-0000a470: 7465 7220 7472 6169 6e69 6e67 2c20 3120  ter training, 1 
-0000a480: 6279 2064 6566 6175 6c74 2e20 3230 2073  by default. 20 s
-0000a490: 6565 6d73 2074 6f20 6265 2061 2067 6f6f  eems to be a goo
-0000a4a0: 6420 6368 6f69 6365 2e20 0a20 2020 2020  d choice. .     
-0000a4b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000a4c0: 5768 656e 2069 7420 6973 2063 616c 6c65  When it is calle
-0000a4d0: 643a 0a20 2020 2020 2020 2020 2020 2058  d:.            X
-0000a4e0: 205b 6274 2e54 656e 736f 725d 3a20 436f   [bt.Tensor]: Co
-0000a4f0: 6f72 6469 6e61 7465 7320 746f 2062 6520  ordinates to be 
-0000a500: 7472 616e 7366 6f72 6d65 642e 0a20 2020  transformed..   
-0000a510: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-0000a520: 653a 2028 5b6e 5f62 6174 6368 3a20 6f70  e: ([n_batch: op
-0000a530: 7469 6f6e 616c 5d2c 207b 6e5f 6469 6d7d  tional], {n_dim}
-0000a540: 2c20 6e5f 312c 206e 5f32 2c20 2e2e 2e2c  , n_1, n_2, ...,
-0000a550: 206e 5f72 290a 2020 2020 2020 2020 2020   n_r).          
-0000a560: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
-0000a570: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
-0000a580: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
-0000a590: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-0000a5a0: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-0000a5b0: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  ch], {n_dim}, n_
-0000a5c0: 312c 206e 5f32 2c20 2e2e 2e2c 206e 5f72  1, n_2, ..., n_r
-0000a5d0: 290a 2020 2020 2020 2020 2727 270a 2020  ).        '''.  
-0000a5e0: 2020 2020 2020 616e 676c 6520 3d20 6261        angle = ba
-0000a5f0: 746f 7263 685f 7465 6e73 6f72 2861 6e67  torch_tensor(ang
-0000a600: 6c65 290a 2020 2020 2020 2020 6966 2061  le).        if a
-0000a610: 6e67 6c65 2e6e 5f64 696d 203c 3d20 3020  ngle.n_dim <= 0 
-0000a620: 616e 6420 6e6f 7420 616e 676c 652e 6861  and not angle.ha
-0000a630: 735f 6261 7463 683a 2061 6e67 6c65 203d  s_batch: angle =
-0000a640: 2061 6e67 6c65 2e75 6e73 7175 6565 7a65   angle.unsqueeze
-0000a650: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
-0000a660: 616e 676c 652e 6e5f 6469 6d20 3d3d 2031  angle.n_dim == 1
-0000a670: 2061 6e64 206e 6f74 2061 6e67 6c65 2e68   and not angle.h
-0000a680: 6173 5f62 6174 6368 3a20 616e 676c 6520  as_batch: angle 
-0000a690: 3d20 616e 676c 652e 7769 7468 5f62 6174  = angle.with_bat
-0000a6a0: 6368 6469 6d28 3029 0a20 2020 2020 2020  chdim(0).       
-0000a6b0: 2069 6620 616e 676c 652e 6e5f 6469 6d20   if angle.n_dim 
-0000a6c0: 3d3d 2032 2061 6e64 206e 6f74 2061 6e67  == 2 and not ang
-0000a6d0: 6c65 2e68 6173 5f62 6174 6368 3a20 616e  le.has_batch: an
-0000a6e0: 676c 6520 3d20 616e 676c 652e 756e 7371  gle = angle.unsq
-0000a6f0: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
-0000a700: 2020 6966 2061 6e67 6c65 2e6e 5f64 696d    if angle.n_dim
-0000a710: 203d 3d20 3320 616e 6420 6e6f 7420 616e   == 3 and not an
-0000a720: 676c 652e 6861 735f 6261 7463 6820 616e  gle.has_batch an
-0000a730: 6420 616e 676c 652e 7368 6170 655b 315d  d angle.shape[1]
-0000a740: 203d 3d20 616e 676c 652e 7368 6170 655b   == angle.shape[
-0000a750: 325d 3a20 616e 676c 652e 6261 7463 685f  2]: angle.batch_
-0000a760: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
-0000a770: 2020 2020 2020 6176 6f75 6368 2861 6e67        avouch(ang
-0000a780: 6c65 2e68 6173 5f62 6174 6368 2c20 6622  le.has_batch, f"
-0000a790: 506c 6561 7365 2075 7365 2062 6174 6f72  Please use bator
-0000a7a0: 6368 2074 656e 736f 7220 6f66 2073 697a  ch tensor of siz
-0000a7b0: 6520 285b 6e5f 6261 7463 685d 2c29 2066  e ([n_batch],) f
-0000a7c0: 6f72 2052 6967 6964 2072 6f74 6174 696f  or Rigid rotatio
-0000a7d0: 6e20 616e 676c 6573 2c20 696e 7374 6561  n angles, instea
-0000a7e0: 6420 6f66 207b 616e 676c 652e 7368 6170  d of {angle.shap
-0000a7f0: 657d 2e20 2229 0a20 2020 2020 2020 206e  e}. ").        n
-0000a800: 5f62 6174 6368 203d 2061 6e67 6c65 2e6e  _batch = angle.n
-0000a810: 5f62 6174 6368 0a20 2020 2020 2020 206e  _batch.        n
-0000a820: 5f64 696d 203d 204e 6f6e 650a 2020 2020  _dim = None.    
-0000a830: 2020 2020 6966 2061 6e67 6c65 2e6e 5f64      if angle.n_d
-0000a840: 696d 203e 3d20 323a 0a20 2020 2020 2020  im >= 2:.       
-0000a850: 2020 2020 206d 6174 7269 7820 3d20 616e       matrix = an
-0000a860: 676c 650a 2020 2020 2020 2020 2020 2020  gle.            
-0000a870: 6e5f 6469 6d20 3d20 6d61 7472 6978 2e73  n_dim = matrix.s
-0000a880: 697a 6528 2d31 2920 2d20 310a 2020 2020  ize(-1) - 1.    
-0000a890: 2020 2020 2020 2020 6365 6e74 6572 203d          center =
-0000a8a0: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
-0000a8b0: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
-0000a8c0: 2020 2020 2020 2020 2020 7472 616e 736c            transl
-0000a8d0: 6174 696f 6e20 3d20 6d61 7472 6978 5b2e  ation = matrix[.
-0000a8e0: 2e2e 2c20 3a2d 312c 202d 315d 2e77 6974  .., :-1, -1].wit
-0000a8f0: 685f 6368 616e 6e65 6c64 696d 2831 290a  h_channeldim(1).
-0000a900: 2020 2020 2020 2020 2020 2020 4120 3d20              A = 
-0000a910: 6d61 7472 6978 5b2e 2e2e 2c20 3a2d 312c  matrix[..., :-1,
-0000a920: 203a 2d31 5d0a 2020 2020 2020 2020 2020   :-1].          
-0000a930: 2020 6176 6f75 6368 2862 742e 6e6f 726d    avouch(bt.norm
-0000a940: 2841 2e54 2040 2041 202d 2062 742e 6579  (A.T @ A - bt.ey
-0000a950: 6528 4129 292e 7375 6d28 2920 3c20 3165  e(A)).sum() < 1e
-0000a960: 2d34 2c20 2250 6c65 6173 6520 6d61 6b65  -4, "Please make
-0000a970: 2073 7572 6520 7468 6174 206d 6174 7269   sure that matri
-0000a980: 7820 696e 7075 7420 666f 7220 5269 6769  x input for Rigi
-0000a990: 6420 6973 206f 7274 686f 676f 6e61 6c2e  d is orthogonal.
-0000a9a0: 2055 7365 2041 6666 696e 6520 696e 7374   Use Affine inst
-0000a9b0: 6561 6420 6966 2069 7420 6973 206e 6f74  ead if it is not
-0000a9c0: 2e20 2229 0a20 2020 2020 2020 2020 2020  . ").           
-0000a9d0: 2023 2049 203d 2062 742e 6579 6528 4129   # I = bt.eye(A)
-0000a9e0: 0a20 2020 2020 2020 2020 2020 2023 205a  .            # Z
-0000a9f0: 5f6c 6566 7420 3d20 2841 202d 2049 295b  _left = (A - I)[
-0000aa00: 2e2e 2e2c 203a 2d31 5d20 2320 285b 6e5f  ..., :-1] # ([n_
-0000aa10: 6261 7463 685d 2c20 6e5f 6469 6d2c 206e  batch], n_dim, n
-0000aa20: 5f64 696d 2d31 290a 2020 2020 2020 2020  _dim-1).        
-0000aa30: 2020 2020 2320 5a5f 7269 6768 7420 3d20      # Z_right = 
-0000aa40: 2841 202d 2049 295b 2e2e 2e2c 202d 315d  (A - I)[..., -1]
-0000aa50: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
-0000aa60: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-0000aa70: 2020 2320 5a54 5a20 3d20 5a5f 6c65 6674    # ZTZ = Z_left
-0000aa80: 2e54 2040 205a 5f6c 6566 740a 2020 2020  .T @ Z_left.    
-0000aa90: 2020 2020 2020 2020 2320 6966 206e 5f64          # if n_d
-0000aaa0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
-0000aab0: 2020 2020 2023 2020 2020 2061 7869 7320       #     axis 
-0000aac0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000aad0: 2020 2023 2020 2020 2061 6e67 6c65 203d     #     angle =
-0000aae0: 2062 742e 7768 6572 6528 6274 2e61 6273   bt.where(bt.abs
-0000aaf0: 2862 742e 6465 7428 5a54 5a29 2920 3c20  (bt.det(ZTZ)) < 
-0000ab00: 3165 2d36 2c20 6274 2e7a 6572 6f73 285b  1e-6, bt.zeros([
-0000ab10: 6e5f 6261 7463 685d 292c 2062 742e 6163  n_batch]), bt.ac
-0000ab20: 6f73 2831 202d 205a 545a 202f 2032 292e  os(1 - ZTZ / 2).
-0000ab30: 7371 7565 657a 6528 2d31 2c20 2d31 2929  squeeze(-1, -1))
-0000ab40: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
-0000ab50: 6c69 6620 6e5f 6469 6d20 3d3d 2033 3a0a  lif n_dim == 3:.
-0000ab60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000ab70: 2020 696e 765a 545a 203d 2062 742e 696e    invZTZ = bt.in
-0000ab80: 7628 6274 2e77 6865 7265 2862 742e 6162  v(bt.where(bt.ab
-0000ab90: 7328 6274 2e64 6574 285a 545a 2929 2e75  s(bt.det(ZTZ)).u
-0000aba0: 6e73 7175 6565 7a65 282d 312c 202d 3129  nsqueeze(-1, -1)
-0000abb0: 203c 2031 652d 362c 2062 742e 6579 6528   < 1e-6, bt.eye(
-0000abc0: 5a54 5a29 2c20 5a54 5a29 290a 2020 2020  ZTZ), ZTZ)).    
-0000abd0: 2020 2020 2020 2020 2320 2020 2020 7665          #     ve
-0000abe0: 6374 6f72 203d 2062 742e 6361 7428 2d20  ctor = bt.cat(- 
-0000abf0: 696e 765a 545a 2040 205a 5f6c 6566 742e  invZTZ @ Z_left.
-0000ac00: 5420 4020 5a5f 7269 6768 742c 2062 742e  T @ Z_right, bt.
-0000ac10: 6f6e 6573 285b 6e5f 6261 7463 685d 2c20  ones([n_batch], 
-0000ac20: 3129 2c20 3129 2e77 6974 685f 6368 616e  1), 1).with_chan
-0000ac30: 6e65 6c64 696d 2831 290a 2020 2020 2020  neldim(1).      
-0000ac40: 2020 2020 2020 2320 2020 2020 616e 676c        #     angl
-0000ac50: 6520 3d20 6274 2e77 6865 7265 2862 742e  e = bt.where(bt.
-0000ac60: 6162 7328 6274 2e64 6574 285a 545a 2929  abs(bt.det(ZTZ))
-0000ac70: 203c 2031 652d 362c 2062 742e 7a65 726f   < 1e-6, bt.zero
-0000ac80: 7328 5b6e 5f62 6174 6368 5d29 2c20 7665  s([n_batch]), ve
-0000ac90: 6374 6f72 2e6e 6f72 6d28 2929 0a20 2020  ctor.norm()).   
-0000aca0: 2020 2020 2020 2020 2023 2020 2020 2061           #     a
-0000acb0: 7869 7320 3d20 6274 2e77 6865 7265 2828  xis = bt.where((
-0000acc0: 6274 2e61 6273 2862 742e 6465 7428 5a54  bt.abs(bt.det(ZT
-0000acd0: 5a29 2920 3c20 3165 2d36 292e 6d75 6c74  Z)) < 1e-6).mult
-0000ace0: 6970 6c79 286e 5f64 696d 2c20 7b7d 292c  iply(n_dim, {}),
-0000acf0: 2062 742e 6368 616e 6e65 6c5f 7465 6e73   bt.channel_tens
-0000ad00: 6f72 2862 742e 6f6e 655f 686f 7428 302c  or(bt.one_hot(0,
-0000ad10: 206e 5f64 696d 2929 2e6d 756c 7469 706c   n_dim)).multipl
-0000ad20: 7928 6e5f 6261 7463 682c 205b 5d29 2c20  y(n_batch, []), 
-0000ad30: 7665 6374 6f72 202f 2061 6e67 6c65 290a  vector / angle).
-0000ad40: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000ad50: 5f64 696d 203d 3d20 323a 2061 7869 7320  _dim == 2: axis 
-0000ad60: 3d20 4e6f 6e65 3b20 616e 676c 6520 3d20  = None; angle = 
-0000ad70: 6274 2e61 636f 7328 415b 2e2e 2e2c 2030  bt.acos(A[..., 0
-0000ad80: 2c20 305d 290a 2020 2020 2020 2020 2020  , 0]).          
-0000ad90: 2020 656c 6966 206e 5f64 696d 203d 3d20    elif n_dim == 
-0000ada0: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
-0000adb0: 2020 2061 6e74 695f 7379 6d20 3d20 2841     anti_sym = (A
-0000adc0: 202d 2041 2e54 2920 2f20 320a 2020 2020   - A.T) / 2.    
-0000add0: 2020 2020 2020 2020 2020 2020 7379 6d20              sym 
-0000ade0: 3d20 2841 202b 2041 2e54 2920 2f20 3220  = (A + A.T) / 2 
-0000adf0: 2d20 6274 2e65 7965 2841 290a 2020 2020  - bt.eye(A).    
-0000ae00: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-0000ae10: 6520 3d20 6274 2e61 636f 7328 2828 616e  e = bt.acos(((an
-0000ae20: 7469 5f73 796d 2040 2061 6e74 695f 7379  ti_sym @ anti_sy
-0000ae30: 6d29 202f 2073 796d 292e 6d65 616e 2829  m) / sym).mean()
-0000ae40: 202d 2031 290a 2020 2020 2020 2020 2020   - 1).          
-0000ae50: 2020 2020 2020 6178 6973 203d 2062 742e        axis = bt.
-0000ae60: 756e 6372 6f73 735f 6d61 7472 6978 2861  uncross_matrix(a
-0000ae70: 6e74 695f 7379 6d29 0a20 2020 2020 2020  nti_sym).       
-0000ae80: 2020 2020 2020 2020 2061 7869 7320 2f3d           axis /=
-0000ae90: 2062 742e 7369 6e28 616e 676c 6529 0a20   bt.sin(angle). 
-0000aea0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000aeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aec0: 2072 6169 7365 2045 7272 6f72 2822 4e6f   raise Error("No
-0000aed0: 7449 6d70 6c65 6d65 6e74 6564 2229 2866  tImplemented")(f
-0000aee0: 2252 6967 6964 2074 7261 6e73 666f 726d  "Rigid transform
-0000aef0: 6174 696f 6e20 696e 206d 6963 6f6d 7075  ation in micompu
-0000af00: 7469 6e67 2064 6f65 7320 6e6f 7420 7375  ting does not su
-0000af10: 7070 6f72 7420 7b6e 5f64 696d 7d20 6469  pport {n_dim} di
-0000af20: 6d65 6e73 696f 6e61 6c20 7472 616e 7366  mensional transf
-0000af30: 6f72 6d73 2028 3220 2620 3344 206f 6e6c  orms (2 & 3D onl
-0000af40: 7929 2e20 2220 2b20 0a20 2020 2020 2020  y). " + .       
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af70: 2020 2020 2022 506c 6561 7365 2063 6f6e       "Please con
-0000af80: 7461 6374 2074 6865 2064 6576 656c 6f70  tact the develop
-0000af90: 6572 7320 6966 2074 6865 7265 2061 7265  ers if there are
-0000afa0: 2066 6561 7369 626c 6520 616c 676f 7269   feasible algori
-0000afb0: 7468 6d73 2028 4572 726f 7220 436f 6465  thms (Error Code
-0000afc0: 3a20 5433 3333 292e 2054 6861 6e6b 2079  : T333). Thank y
-0000afd0: 6f75 2e20 2229 0a0a 2020 2020 2020 2020  ou. ")..        
-0000afe0: 6966 2074 7261 6e73 6c61 7469 6f6e 2069  if translation i
-0000aff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b000: 2020 2020 2020 2020 7472 616e 736c 6174          translat
-0000b010: 696f 6e20 3d20 6261 746f 7263 685f 7465  ion = batorch_te
-0000b020: 6e73 6f72 2874 7261 6e73 6c61 7469 6f6e  nsor(translation
-0000b030: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000b040: 2074 7261 6e73 6c61 7469 6f6e 2e6e 5f64   translation.n_d
-0000b050: 696d 203c 3d20 3120 616e 6420 6e6f 7420  im <= 1 and not 
-0000b060: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
-0000b070: 6261 7463 683a 2074 7261 6e73 6c61 7469  batch: translati
-0000b080: 6f6e 203d 2074 7261 6e73 6c61 7469 6f6e  on = translation
-0000b090: 2e75 6e73 7175 6565 7a65 285b 5d29 0a20  .unsqueeze([]). 
-0000b0a0: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
-0000b0b0: 616e 736c 6174 696f 6e2e 6e5f 6469 6d20  anslation.n_dim 
-0000b0c0: 3d3d 2032 2061 6e64 206e 6f74 2074 7261  == 2 and not tra
-0000b0d0: 6e73 6c61 7469 6f6e 2e68 6173 5f62 6174  nslation.has_bat
-0000b0e0: 6368 3a20 7472 616e 736c 6174 696f 6e20  ch: translation 
-0000b0f0: 3d20 7472 616e 736c 6174 696f 6e2e 7769  = translation.wi
-0000b100: 7468 5f62 6174 6368 6469 6d28 2831 202d  th_batchdim((1 -
-0000b110: 2074 7261 6e73 6c61 7469 6f6e 2e63 6861   translation.cha
-0000b120: 6e6e 656c 5f64 696d 656e 7369 6f6e 2920  nnel_dimension) 
-0000b130: 6966 2074 7261 6e73 6c61 7469 6f6e 2e68  if translation.h
-0000b140: 6173 5f63 6861 6e6e 656c 2065 6c73 6520  as_channel else 
-0000b150: 3029 0a20 2020 2020 2020 2020 2020 2069  0).            i
-0000b160: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
-0000b170: 6469 6d20 3d3d 2032 2061 6e64 206e 6f74  dim == 2 and not
-0000b180: 2074 7261 6e73 6c61 7469 6f6e 2e68 6173   translation.has
-0000b190: 5f63 6861 6e6e 656c 3a20 7472 616e 736c  _channel: transl
-0000b1a0: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
-0000b1b0: 696f 6e2e 7769 7468 5f63 6861 6e6e 656c  ion.with_channel
-0000b1c0: 6469 6d28 3120 2d20 7472 616e 736c 6174  dim(1 - translat
-0000b1d0: 696f 6e2e 6261 7463 685f 6469 6d65 6e73  ion.batch_dimens
-0000b1e0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-0000b1f0: 2061 766f 7563 6828 7472 616e 736c 6174   avouch(translat
-0000b200: 696f 6e2e 6861 735f 6261 7463 6820 616e  ion.has_batch an
-0000b210: 6420 7472 616e 736c 6174 696f 6e2e 6861  d translation.ha
-0000b220: 735f 6368 616e 6e65 6c2c 2066 2250 6c65  s_channel, f"Ple
-0000b230: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
-0000b240: 7465 6e73 6f72 206f 6620 7369 7a65 2028  tensor of size (
-0000b250: 5b6e 5f62 6174 6368 5d2c 207b 7b6e 5f64  [n_batch], {{n_d
-0000b260: 696d 7d7d 2920 666f 7220 5269 6769 6420  im}}) for Rigid 
-0000b270: 7472 616e 736c 6174 696f 6e2c 2069 6e73  translation, ins
-0000b280: 7465 6164 206f 6620 7b74 7261 6e73 6c61  tead of {transla
-0000b290: 7469 6f6e 2e73 6861 7065 7d2e 2022 290a  tion.shape}. ").
-0000b2a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000b2b0: 5f62 6174 6368 203d 3d20 3120 616e 6420  _batch == 1 and 
-0000b2c0: 7472 616e 736c 6174 696f 6e2e 6e5f 6261  translation.n_ba
-0000b2d0: 7463 6820 3e20 313a 206e 5f62 6174 6368  tch > 1: n_batch
-0000b2e0: 203d 2074 7261 6e73 6c61 7469 6f6e 2e6e   = translation.n
-0000b2f0: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
-0000b300: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
-0000b310: 6f6e 653a 206e 5f64 696d 203d 2074 7261  one: n_dim = tra
-0000b320: 6e73 6c61 7469 6f6e 2e6e 5f63 6861 6e6e  nslation.n_chann
-0000b330: 656c 0a20 2020 2020 2020 2020 2020 2065  el.            e
-0000b340: 6c73 653a 2061 766f 7563 6828 6e5f 6469  lse: avouch(n_di
-0000b350: 6d20 3d3d 2074 7261 6e73 6c61 7469 6f6e  m == translation
-0000b360: 2e6e 5f63 6861 6e6e 656c 2c20 2253 7973  .n_channel, "Sys
-0000b370: 7465 6d61 7469 6320 6572 726f 722e 2050  tematic error. P
-0000b380: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
-0000b390: 6520 6465 7665 6c6f 7065 7273 2066 6f72  e developers for
-0000b3a0: 2064 6574 6169 6c73 2028 4572 726f 7220   details (Error 
-0000b3b0: 436f 6465 3a20 5433 3332 292e 2022 290a  Code: T332). ").
-0000b3c0: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
-0000b3d0: 6d20 3d20 7472 616e 736c 6174 696f 6e2e  m = translation.
-0000b3e0: 6e5f 6368 616e 6e65 6c0a 2020 2020 2020  n_channel.      
-0000b3f0: 2020 6966 2063 656e 7465 7220 6973 206e    if center is n
-0000b400: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000b410: 2020 2020 2063 656e 7465 7220 3d20 6261       center = ba
-0000b420: 746f 7263 685f 7465 6e73 6f72 2863 656e  torch_tensor(cen
-0000b430: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
-0000b440: 2069 6620 6365 6e74 6572 2e6e 5f64 696d   if center.n_dim
-0000b450: 203c 3d20 3120 616e 6420 6e6f 7420 6365   <= 1 and not ce
-0000b460: 6e74 6572 2e68 6173 5f62 6174 6368 3a20  nter.has_batch: 
-0000b470: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
-0000b480: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
-0000b490: 2020 2020 2020 2020 2020 6966 2063 656e            if cen
-0000b4a0: 7465 722e 6e5f 6469 6d20 3d3d 2032 2061  ter.n_dim == 2 a
-0000b4b0: 6e64 206e 6f74 2063 656e 7465 722e 6861  nd not center.ha
-0000b4c0: 735f 6261 7463 683a 2063 656e 7465 7220  s_batch: center 
-0000b4d0: 3d20 6365 6e74 6572 2e77 6974 685f 6261  = center.with_ba
-0000b4e0: 7463 6864 696d 2828 3120 2d20 6365 6e74  tchdim((1 - cent
-0000b4f0: 6572 2e63 6861 6e6e 656c 5f64 696d 656e  er.channel_dimen
-0000b500: 7369 6f6e 2920 6966 2063 656e 7465 722e  sion) if center.
-0000b510: 6861 735f 6368 616e 6e65 6c20 656c 7365  has_channel else
-0000b520: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-0000b530: 6966 2063 656e 7465 722e 6e5f 6469 6d20  if center.n_dim 
-0000b540: 3d3d 2032 2061 6e64 206e 6f74 2063 656e  == 2 and not cen
-0000b550: 7465 722e 6861 735f 6368 616e 6e65 6c3a  ter.has_channel:
-0000b560: 2063 656e 7465 7220 3d20 6365 6e74 6572   center = center
-0000b570: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
-0000b580: 2831 202d 2063 656e 7465 722e 6261 7463  (1 - center.batc
-0000b590: 685f 6469 6d65 6e73 696f 6e29 0a20 2020  h_dimension).   
-0000b5a0: 2020 2020 2020 2020 2061 766f 7563 6828           avouch(
-0000b5b0: 6365 6e74 6572 2e68 6173 5f62 6174 6368  center.has_batch
-0000b5c0: 2061 6e64 2063 656e 7465 722e 6861 735f   and center.has_
-0000b5d0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
-0000b5e0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
-0000b5f0: 6e73 6f72 206f 6620 7369 7a65 2028 5b6e  nsor of size ([n
-0000b600: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
-0000b610: 7d7d 2920 666f 7220 5269 6769 6420 6365  }}) for Rigid ce
-0000b620: 6e74 6572 2c20 696e 7374 6561 6420 6f66  nter, instead of
-0000b630: 207b 6365 6e74 6572 2e73 6861 7065 7d2e   {center.shape}.
-0000b640: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
-0000b650: 6966 206e 5f62 6174 6368 203d 3d20 3120  if n_batch == 1 
-0000b660: 616e 6420 6365 6e74 6572 2e6e 5f62 6174  and center.n_bat
-0000b670: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
-0000b680: 3d20 6365 6e74 6572 2e6e 5f62 6174 6368  = center.n_batch
-0000b690: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b6a0: 6e5f 6469 6d20 6973 204e 6f6e 653a 206e  n_dim is None: n
-0000b6b0: 5f64 696d 203d 2063 656e 7465 722e 6e5f  _dim = center.n_
-0000b6c0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
-0000b6d0: 2020 2020 656c 7365 3a20 6176 6f75 6368      else: avouch
-0000b6e0: 286e 5f64 696d 203d 3d20 6365 6e74 6572  (n_dim == center
-0000b6f0: 2e6e 5f63 6861 6e6e 656c 2c20 6622 4365  .n_channel, f"Ce
-0000b700: 6e74 6572 287b 6365 6e74 6572 2e6e 5f63  nter({center.n_c
-0000b710: 6861 6e6e 656c 7d44 2920 616e 6420 7472  hannel}D) and tr
-0000b720: 616e 736c 6174 696f 6e28 7b6e 5f64 696d  anslation({n_dim
-0000b730: 7d44 2920 696e 2074 7261 6e73 2e52 6967  }D) in trans.Rig
-0000b740: 6964 2073 686f 756c 6420 6861 7665 2074  id should have t
-0000b750: 6865 2073 616d 6520 6469 6d65 6e73 696f  he same dimensio
-0000b760: 6e2e 2022 290a 2020 2020 2020 2020 2020  n. ").          
-0000b770: 2020 6e5f 6469 6d20 3d20 6365 6e74 6572    n_dim = center
-0000b780: 2e6e 5f63 6861 6e6e 656c 0a20 2020 2020  .n_channel.     
-0000b790: 2020 2069 6620 6178 6973 2069 7320 6e6f     if axis is no
-0000b7a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000b7b0: 2020 2020 6178 6973 203d 2062 6174 6f72      axis = bator
-0000b7c0: 6368 5f74 656e 736f 7228 6178 6973 290a  ch_tensor(axis).
-0000b7d0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000b7e0: 7869 732e 6e5f 6469 6d20 3c3d 2031 2061  xis.n_dim <= 1 a
-0000b7f0: 6e64 206e 6f74 2061 7869 732e 6861 735f  nd not axis.has_
-0000b800: 6261 7463 683a 2061 7869 7320 3d20 6178  batch: axis = ax
-0000b810: 6973 2e75 6e73 7175 6565 7a65 285b 5d29  is.unsqueeze([])
-0000b820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b830: 6178 6973 2e6e 5f64 696d 203d 3d20 3220  axis.n_dim == 2 
-0000b840: 616e 6420 6e6f 7420 6178 6973 2e68 6173  and not axis.has
-0000b850: 5f62 6174 6368 3a20 6178 6973 203d 2061  _batch: axis = a
-0000b860: 7869 732e 7769 7468 5f62 6174 6368 6469  xis.with_batchdi
-0000b870: 6d28 2831 202d 2061 7869 732e 6368 616e  m((1 - axis.chan
-0000b880: 6e65 6c5f 6469 6d65 6e73 696f 6e29 2069  nel_dimension) i
-0000b890: 6620 6178 6973 2e68 6173 5f63 6861 6e6e  f axis.has_chann
-0000b8a0: 656c 2065 6c73 6520 3029 0a20 2020 2020  el else 0).     
-0000b8b0: 2020 2020 2020 2069 6620 6178 6973 2e6e         if axis.n
-0000b8c0: 5f64 696d 203d 3d20 3220 616e 6420 6e6f  _dim == 2 and no
-0000b8d0: 7420 6178 6973 2e68 6173 5f63 6861 6e6e  t axis.has_chann
-0000b8e0: 656c 3a20 6178 6973 203d 2061 7869 732e  el: axis = axis.
-0000b8f0: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
-0000b900: 3120 2d20 6178 6973 2e62 6174 6368 5f64  1 - axis.batch_d
-0000b910: 696d 656e 7369 6f6e 290a 2020 2020 2020  imension).      
-0000b920: 2020 2020 2020 6176 6f75 6368 2861 7869        avouch(axi
-0000b930: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
-0000b940: 6178 6973 2e68 6173 5f63 6861 6e6e 656c  axis.has_channel
-0000b950: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
-0000b960: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
-0000b970: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
-0000b980: 2c20 7b7b 6e5f 6469 6d7d 7d29 2066 6f72  , {{n_dim}}) for
-0000b990: 2052 6967 6964 2061 7869 7365 732c 2069   Rigid axises, i
-0000b9a0: 6e73 7465 6164 206f 6620 7b61 7869 732e  nstead of {axis.
-0000b9b0: 7368 6170 657d 2e20 2229 0a20 2020 2020  shape}. ").     
-0000b9c0: 2020 2020 2020 2069 6620 2828 6178 6973         if ((axis
-0000b9d0: 2e6e 6f72 6d28 2920 2d20 3129 202a 2a20  .norm() - 1) ** 
-0000b9e0: 3229 2e73 756d 2829 2e73 756d 2829 203e  2).sum().sum() >
-0000b9f0: 3d20 3165 2d34 3a0a 2020 2020 2020 2020  = 1e-4:.        
-0000ba00: 2020 2020 2020 2020 7072 696e 7428 2277          print("w
-0000ba10: 6172 6e69 6e67 3a20 7061 7261 6d2e 2061  arning: param. a
-0000ba20: 7869 7365 7320 666f 7220 2752 6967 6964  xises for 'Rigid
-0000ba30: 2720 7472 616e 7366 6f72 6d61 7469 6f6e  ' transformation
-0000ba40: 2073 686f 756c 6420 6265 206e 6f72 6d2d   should be norm-
-0000ba50: 3120 7665 6374 6f72 732c 2061 7574 6f2d  1 vectors, auto-
-0000ba60: 6e6f 726d 616c 697a 6174 696f 6e20 776f  normalization wo
-0000ba70: 756c 6420 6265 2070 6572 666f 726d 6564  uld be performed
-0000ba80: 2e20 506c 6561 7365 2063 6f6e 7461 6374  . Please contact
-0000ba90: 2074 6865 2064 6576 656c 6f70 6572 7320   the developers 
-0000baa0: 6966 206e 6563 6573 7361 7279 2028 4572  if necessary (Er
-0000bab0: 726f 7220 436f 6465 3a20 5433 3331 292e  ror Code: T331).
-0000bac0: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
-0000bad0: 2020 2020 6178 6973 203d 2061 7869 7320      axis = axis 
-0000bae0: 2f20 6178 6973 2e6e 6f72 6d28 290a 2020  / axis.norm().  
-0000baf0: 2020 2020 2020 2020 2020 6966 206e 5f62            if n_b
-0000bb00: 6174 6368 203d 3d20 3120 616e 6420 6178  atch == 1 and ax
-0000bb10: 6973 2e6e 5f62 6174 6368 203e 2031 3a20  is.n_batch > 1: 
-0000bb20: 6e5f 6261 7463 6820 3d20 6178 6973 2e6e  n_batch = axis.n
-0000bb30: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
-0000bb40: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
-0000bb50: 6f6e 653a 206e 5f64 696d 203d 2061 7869  one: n_dim = axi
-0000bb60: 732e 6e5f 6368 616e 6e65 6c0a 2020 2020  s.n_channel.    
-0000bb70: 2020 2020 2020 2020 656c 7365 3a20 6176          else: av
-0000bb80: 6f75 6368 286e 5f64 696d 203d 3d20 6178  ouch(n_dim == ax
-0000bb90: 6973 2e6e 5f63 6861 6e6e 656c 2c20 6622  is.n_channel, f"
-0000bba0: 5472 616e 736c 6174 696f 6e28 7b6e 5f64  Translation({n_d
-0000bbb0: 696d 7d44 2920 616e 6420 6178 6973 6573  im}D) and axises
-0000bbc0: 287b 6178 6973 2e6e 5f63 6861 6e6e 656c  ({axis.n_channel
-0000bbd0: 7d44 2929 2069 6e20 7472 616e 732e 5269  }D)) in trans.Ri
-0000bbe0: 6769 6420 7368 6f75 6c64 2068 6176 6520  gid should have 
-0000bbf0: 7468 6520 7361 6d65 2064 696d 656e 7369  the same dimensi
-0000bc00: 6f6e 2e20 2229 0a20 2020 2020 2020 2069  on. ").        i
-0000bc10: 6620 6e5f 6469 6d20 6973 204e 6f6e 653a  f n_dim is None:
-0000bc20: 206e 5f64 696d 203d 2032 2069 6620 6178   n_dim = 2 if ax
-0000bc30: 6973 2069 7320 4e6f 6e65 2065 6c73 6520  is is None else 
-0000bc40: 330a 2020 2020 2020 2020 6966 2074 7261  3.        if tra
-0000bc50: 6e73 6c61 7469 6f6e 2069 7320 4e6f 6e65  nslation is None
-0000bc60: 3a20 7472 616e 736c 6174 696f 6e20 3d20  : translation = 
-0000bc70: 6274 2e7a 6572 6f73 285b 6e5f 6261 7463  bt.zeros([n_batc
-0000bc80: 685d 2c20 7b6e 5f64 696d 7d29 0a20 2020  h], {n_dim}).   
-0000bc90: 2020 2020 2069 6620 6365 6e74 6572 2069       if center i
-0000bca0: 7320 4e6f 6e65 3a20 6365 6e74 6572 203d  s None: center =
-0000bcb0: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
-0000bcc0: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
-0000bcd0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000bce0: 204e 6f77 2077 6520 6372 6561 7465 2074   Now we create t
-0000bcf0: 6865 206d 6174 7269 780a 2020 2020 2020  he matrix.      
-0000bd00: 2020 616e 676c 6520 3d20 616e 676c 652e    angle = angle.
-0000bd10: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
-0000bd20: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
-0000bd30: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
-0000bd40: 7472 616e 736c 6174 696f 6e20 3d20 7472  translation = tr
-0000bd50: 616e 736c 6174 696f 6e2e 666c 6f61 7428  anslation.float(
-0000bd60: 290a 2020 2020 2020 2020 6966 206e 5f64  ).        if n_d
-0000bd70: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
-0000bd80: 2020 2020 2041 203d 2062 742e 7374 6163       A = bt.stac
-0000bd90: 6b28 6274 2e63 6f73 2861 6e67 6c65 292c  k(bt.cos(angle),
-0000bda0: 2062 742e 7369 6e28 616e 676c 6529 2c20   bt.sin(angle), 
-0000bdb0: 2d62 742e 7369 6e28 616e 676c 6529 2c20  -bt.sin(angle), 
-0000bdc0: 6274 2e63 6f73 2861 6e67 6c65 292c 202d  bt.cos(angle), -
-0000bdd0: 3129 2e73 706c 6974 6469 6d28 2d31 2c20  1).splitdim(-1, 
-0000bde0: 322c 2032 290a 2020 2020 2020 2020 656c  2, 2).        el
-0000bdf0: 6966 206e 5f64 696d 203d 3d20 333a 0a20  if n_dim == 3:. 
-0000be00: 2020 2020 2020 2020 2020 2061 7869 7320             axis 
-0000be10: 3d20 6178 6973 2e66 6c6f 6174 2829 0a20  = axis.float(). 
-0000be20: 2020 2020 2020 2020 2020 2041 203d 2062             A = b
-0000be30: 742e 6579 6528 5b6e 5f62 6174 6368 5d2c  t.eye([n_batch],
-0000be40: 206e 5f64 696d 2920 2b20 2831 202d 2062   n_dim) + (1 - b
-0000be50: 742e 636f 7328 616e 676c 6529 2920 2a20  t.cos(angle)) * 
-0000be60: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
-0000be70: 6178 6973 2920 4020 6274 2e63 726f 7373  axis) @ bt.cross
-0000be80: 5f6d 6174 7269 7828 6178 6973 2920 2b20  _matrix(axis) + 
-0000be90: 6274 2e73 696e 2861 6e67 6c65 2920 2a20  bt.sin(angle) * 
-0000bea0: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
-0000beb0: 6178 6973 290a 2020 2020 2020 2020 656c  axis).        el
-0000bec0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000bed0: 7261 6973 6520 4572 726f 7228 224e 6f74  raise Error("Not
-0000bee0: 496d 706c 656d 656e 7465 6422 2928 6622  Implemented")(f"
-0000bef0: 5269 6769 6420 7472 616e 7366 6f72 6d61  Rigid transforma
-0000bf00: 7469 6f6e 2069 6e20 6d69 636f 6d70 7574  tion in micomput
-0000bf10: 696e 6720 646f 6573 206e 6f74 2073 7570  ing does not sup
-0000bf20: 706f 7274 207b 6e5f 6469 6d7d 2064 696d  port {n_dim} dim
-0000bf30: 656e 7369 6f6e 616c 2074 7261 6e73 666f  ensional transfo
-0000bf40: 726d 7320 2832 2026 2033 4420 6f6e 6c79  rms (2 & 3D only
-0000bf50: 292e 2022 202b 200a 2020 2020 2020 2020  ). " + .        
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 2250 6c65 6173 6520 636f 6e74 6163 7420  "Please contact 
-0000bf90: 7468 6520 6465 7665 6c6f 7065 7273 2069  the developers i
-0000bfa0: 6620 7468 6572 6520 6172 6520 6665 6173  f there are feas
-0000bfb0: 6962 6c65 2061 6c67 6f72 6974 686d 7320  ible algorithms 
-0000bfc0: 2845 7272 6f72 2043 6f64 653a 2054 3333  (Error Code: T33
-0000bfd0: 3329 2e20 5468 616e 6b20 796f 752e 2022  3). Thank you. "
-0000bfe0: 290a 2020 2020 2020 2020 6d61 7472 6978  ).        matrix
-0000bff0: 203d 2062 742e 6361 7428 6274 2e63 6174   = bt.cat(bt.cat
-0000c000: 2841 2c20 2828 7472 616e 736c 6174 696f  (A, ((translatio
-0000c010: 6e20 2b20 6365 6e74 6572 292e 7769 7468  n + center).with
-0000c020: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
-0000c030: 2920 2d20 4120 4020 6365 6e74 6572 2e77  ) - A @ center.w
-0000c040: 6974 685f 6368 616e 6e65 6c64 696d 284e  ith_channeldim(N
-0000c050: 6f6e 6529 292e 756e 7371 7565 657a 6528  one)).unsqueeze(
-0000c060: 2d31 292c 202d 3129 2c20 0a20 2020 2020  -1), -1), .     
-0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 2020 2062 742e 6361 7428 6274 2e7a 6572     bt.cat(bt.zer
-0000c090: 6f73 286e 5f64 696d 292c 2062 742e 6f6e  os(n_dim), bt.on
-0000c0a0: 6573 2831 2929 2e75 6e73 7175 6565 7a65  es(1)).unsqueeze
-0000c0b0: 285b 5d2c 2031 292c 2031 290a 2020 2020  ([], 1), 1).    
-0000c0c0: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
-0000c0d0: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
-0000c0e0: 3a20 6d61 7472 6978 5b2e 2e2e 2c20 3a6e  : matrix[..., :n
-0000c0f0: 5f64 696d 2c20 2d31 5d20 2a3d 2074 7261  _dim, -1] *= tra
-0000c100: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
-0000c110: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000c120: 616e 6365 2873 7061 6369 6e67 2c20 7475  ance(spacing, tu
-0000c130: 706c 6529 3a20 7370 6163 696e 6720 3d20  ple): spacing = 
-0000c140: 746f 5f74 7570 6c65 2873 7061 6369 6e67  to_tuple(spacing
-0000c150: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-0000c160: 2873 7061 6369 6e67 2920 3d3d 2031 3a20  (spacing) == 1: 
-0000c170: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
-0000c180: 6720 2a20 6e5f 6469 6d0a 2020 2020 2020  g * n_dim.      
-0000c190: 2020 4120 3d20 6274 2e64 6961 6728 6261    A = bt.diag(ba
-0000c1a0: 746f 7263 685f 7465 6e73 6f72 286c 6973  torch_tensor(lis
-0000c1b0: 7428 7370 6163 696e 6729 202b 205b 312e  t(spacing) + [1.
-0000c1c0: 5d29 292e 756e 7371 7565 657a 6528 5b5d  ])).unsqueeze([]
-0000c1d0: 292e 6173 7479 7065 286d 6174 7269 7829  ).astype(matrix)
-0000c1e0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-0000c1f0: 2e5f 5f69 6e69 745f 5f28 616e 676c 652c  .__init__(angle,
-0000c200: 2061 7869 732c 2074 7261 6e73 6c61 7469   axis, translati
-0000c210: 6f6e 2c20 6365 6e74 6572 3d63 656e 7465  on, center=cente
-0000c220: 722c 2074 7261 6e73 5f73 7472 6574 6368  r, trans_stretch
-0000c230: 3d74 7261 6e73 5f73 7472 6574 6368 2c20  =trans_stretch, 
-0000c240: 7370 6163 696e 673d 7370 6163 696e 6729  spacing=spacing)
-0000c250: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-0000c260: 5f64 696d 203d 206e 5f64 696d 0a20 2020  _dim = n_dim.   
-0000c270: 2020 2020 2073 656c 662e 7472 616e 735f       self.trans_
-0000c280: 7374 7265 7463 6820 3d20 7472 616e 735f  stretch = trans_
-0000c290: 7374 7265 7463 680a 2020 2020 2020 2020  stretch.        
-0000c2a0: 7365 6c66 2e73 7061 6369 6e67 203d 2073  self.spacing = s
-0000c2b0: 7061 6369 6e67 0a20 2020 2020 2020 2073  pacing.        s
-0000c2c0: 656c 662e 6d61 7472 6978 203d 2041 2e69  elf.matrix = A.i
-0000c2d0: 6e76 2829 2040 206d 6174 7269 7820 4020  nv() @ matrix @ 
-0000c2e0: 410a 2020 2020 2020 2020 7365 6c66 2e62  A.        self.b
-0000c2f0: 6174 6368 5f70 6172 616d 2e61 7070 656e  atch_param.appen
-0000c300: 6428 276d 6174 7269 7827 290a 0a20 2020  d('matrix')..   
-0000c310: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-0000c320: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
-0000c330: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
-0000c340: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
-0000c350: 6d61 7472 6978 203d 2073 656c 662e 6d61  matrix = self.ma
-0000c360: 7472 6978 0a20 2020 2020 2020 206e 5f64  trix.        n_d
-0000c370: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
-0000c380: 2020 2020 2020 2020 4120 3d20 6d61 7472          A = matr
-0000c390: 6978 5b3a 2c20 3a6e 5f64 696d 2c20 3a6e  ix[:, :n_dim, :n
-0000c3a0: 5f64 696d 5d0a 2020 2020 2020 2020 6220  _dim].        b 
-0000c3b0: 3d20 6d61 7472 6978 5b3a 2c20 3a6e 5f64  = matrix[:, :n_d
-0000c3c0: 696d 2c20 6e5f 6469 6d5d 0a20 2020 2020  im, n_dim].     
-0000c3d0: 2020 2073 6861 7065 203d 2058 2e73 6861     shape = X.sha
-0000c3e0: 7065 0a20 2020 2020 2020 2059 203d 2028  pe.        Y = (
-0000c3f0: 4120 4020 582e 666c 6174 7465 6e28 292e  A @ X.flatten().
-0000c400: 6368 616e 6e65 6c5f 6469 6d5f 284e 6f6e  channel_dim_(Non
-0000c410: 6529 202b 2062 2e75 6e73 7175 6565 7a65  e) + b.unsqueeze
-0000c420: 282d 3129 292e 7669 6577 2873 6861 7065  (-1)).view(shape
-0000c430: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000c440: 2059 0a20 2020 200a 2020 2020 6465 6620   Y.    .    def 
-0000c450: 6166 6669 6e65 2873 656c 662c 206e 5f64  affine(self, n_d
-0000c460: 696d 3d4e 6f6e 6529 3a0a 2020 2020 2020  im=None):.      
-0000c470: 2020 6176 6f75 6368 286e 5f64 696d 2069    avouch(n_dim i
-0000c480: 7320 4e6f 6e65 206f 7220 7365 6c66 2e6e  s None or self.n
-0000c490: 5f64 696d 203d 3d20 6e5f 6469 6d29 0a20  _dim == n_dim). 
-0000c4a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000c4b0: 6c66 2e6d 6174 7269 780a 0a20 2020 2064  lf.matrix..    d
-0000c4c0: 6566 2069 6e76 2873 656c 6629 3a0a 2020  ef inv(self):.  
-0000c4d0: 2020 2020 2020 4120 3d20 6274 2e64 6961        A = bt.dia
-0000c4e0: 6728 6261 746f 7263 685f 7465 6e73 6f72  g(batorch_tensor
-0000c4f0: 286c 6973 7428 7365 6c66 2e73 7061 6369  (list(self.spaci
-0000c500: 6e67 2920 2b20 5b31 2e5d 2929 2e75 6e73  ng) + [1.])).uns
-0000c510: 7175 6565 7a65 285b 5d29 2e61 7374 7970  queeze([]).astyp
-0000c520: 6528 7365 6c66 2e6d 6174 7269 7829 0a20  e(self.matrix). 
-0000c530: 2020 2020 2020 2072 6574 7572 6e20 5269         return Ri
-0000c540: 6769 6428 4120 4020 6274 2e69 6e76 2873  gid(A @ bt.inv(s
-0000c550: 656c 662e 6d61 7472 6978 2920 4020 412e  elf.matrix) @ A.
-0000c560: 696e 7628 292c 2074 7261 6e73 5f73 7472  inv(), trans_str
-0000c570: 6574 6368 203d 2031 2c20 7370 6163 696e  etch = 1, spacin
-0000c580: 673d 7365 6c66 2e73 7061 6369 6e67 292e  g=self.spacing).
-0000c590: 6261 636b 7761 7264 5f28 7365 6c66 2e62  backward_(self.b
-0000c5a0: 6163 6b77 6172 6429 0a0a 4061 6c69 6173  ackward)..@alias
-0000c5b0: 2822 4166 6622 290a 636c 6173 7320 4166  ("Aff").class Af
-0000c5c0: 6669 6e65 2853 7061 7469 616c 5472 616e  fine(SpatialTran
-0000c5d0: 7366 6f72 6d61 7469 6f6e 293a 0a20 2020  sformation):.   
-0000c5e0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0000c5f0: 6c66 2c20 6d61 7472 6978 2c20 7472 616e  lf, matrix, tran
-0000c600: 735f 7374 7265 7463 683d 4e6f 6e65 2c20  s_stretch=None, 
-0000c610: 7370 6163 696e 673d 3129 3a0a 2020 2020  spacing=1):.    
-0000c620: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000c630: 4166 6669 6e65 2074 7261 6e73 666f 726d  Affine transform
-0000c640: 6174 696f 6e20 7769 7468 2072 6573 7065  ation with respe
-0000c650: 6374 2074 6f20 7472 616e 7366 6f72 6d61  ct to transforma
-0000c660: 7469 6f6e 206d 6174 7269 782e 0a20 2020  tion matrix..   
-0000c670: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-0000c680: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
-0000c690: 2020 6d61 7472 6978 205b 6274 2e54 656e    matrix [bt.Ten
-0000c6a0: 736f 7220 6f72 206e 702e 6e75 6d70 795d  sor or np.numpy]
-0000c6b0: 3a20 7468 6520 6166 6669 6e65 206d 6174  : the affine mat
-0000c6c0: 7269 782e 200a 2020 2020 2020 2020 2020  rix. .          
-0000c6d0: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-0000c6e0: 6261 7463 685d 2c20 6e5f 6469 6d20 2b20  batch], n_dim + 
-0000c6f0: 312c 206e 5f64 696d 202b 2031 290a 2020  1, n_dim + 1).  
-0000c700: 2020 2020 2020 2020 2020 7472 616e 735f            trans_
-0000c710: 7374 7265 7463 6820 5b69 6e74 5d3a 206f  stretch [int]: o
-0000c720: 6e6c 7920 7573 6564 2066 6f72 2069 7465  nly used for ite
-0000c730: 7261 7469 7665 2070 6172 616d 6574 6572  rative parameter
-0000c740: 2074 7261 696e 696e 672c 2031 2062 7920   training, 1 by 
-0000c750: 6465 6661 756c 742e 2032 3020 7365 656d  default. 20 seem
-0000c760: 7320 746f 2062 6520 6120 676f 6f64 2063  s to be a good c
-0000c770: 686f 6963 652e 200a 2020 2020 2020 2020  hoice. .        
-0000c780: 2020 2020 0a20 2020 2020 2020 2057 6865      .        Whe
-0000c790: 6e20 6974 2069 7320 6361 6c6c 6564 3a0a  n it is called:.
-0000c7a0: 2020 2020 2020 2020 2020 2020 5820 5b62              X [b
-0000c7b0: 742e 5465 6e73 6f72 5d3a 2043 6f6f 7264  t.Tensor]: Coord
-0000c7c0: 696e 6174 6573 2074 6f20 6265 2074 7261  inates to be tra
-0000c7d0: 6e73 666f 726d 6564 2e0a 2020 2020 2020  nsformed..      
-0000c7e0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-0000c7f0: 285b 6e5f 6261 7463 683a 206f 7074 696f  ([n_batch: optio
-0000c800: 6e61 6c5d 2c20 7b6e 5f64 696d 7d2c 206e  nal], {n_dim}, n
-0000c810: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
-0000c820: 7229 0a20 2020 2020 2020 2020 2020 206f  r).            o
-0000c830: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
-0000c840: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
-0000c850: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
-0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c870: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-0000c880: 2c20 7b6e 5f64 696d 7d2c 206e 5f31 2c20  , {n_dim}, n_1, 
-0000c890: 6e5f 322c 202e 2e2e 2c20 6e5f 7229 0a20  n_2, ..., n_r). 
-0000c8a0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0000c8b0: 2020 206d 6174 7269 7820 3d20 6261 746f     matrix = bato
-0000c8c0: 7263 685f 7465 6e73 6f72 286d 6174 7269  rch_tensor(matri
-0000c8d0: 7829 0a20 2020 2020 2020 206e 5f64 696d  x).        n_dim
-0000c8e0: 203d 206d 6174 7269 782e 7369 7a65 282d   = matrix.size(-
-0000c8f0: 3129 202d 2031 0a20 2020 2020 2020 2069  1) - 1.        i
-0000c900: 6620 6d61 7472 6978 2e6e 5f64 696d 203c  f matrix.n_dim <
-0000c910: 3d20 3220 616e 6420 6e6f 7420 6d61 7472  = 2 and not matr
-0000c920: 6978 2e68 6173 5f62 6174 6368 3a20 6d61  ix.has_batch: ma
-0000c930: 7472 6978 203d 206d 6174 7269 782e 756e  trix = matrix.un
-0000c940: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
-0000c950: 2020 2020 6966 206d 6174 7269 782e 6e5f      if matrix.n_
-0000c960: 6469 6d20 3d3d 2033 2061 6e64 206e 6f74  dim == 3 and not
-0000c970: 206d 6174 7269 782e 6861 735f 6261 7463   matrix.has_batc
-0000c980: 6820 616e 6420 6d61 7472 6978 2e73 6861  h and matrix.sha
-0000c990: 7065 5b31 5d20 3d3d 206d 6174 7269 782e  pe[1] == matrix.
-0000c9a0: 7368 6170 655b 325d 3a20 6d61 7472 6978  shape[2]: matrix
-0000c9b0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-0000c9c0: 203d 2030 0a20 2020 2020 2020 2061 766f   = 0.        avo
-0000c9d0: 7563 6828 6d61 7472 6978 2e68 6173 5f62  uch(matrix.has_b
-0000c9e0: 6174 6368 2c20 6622 506c 6561 7365 2075  atch, f"Please u
-0000c9f0: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
-0000ca00: 7220 6f66 2073 697a 6520 285b 6e5f 6261  r of size ([n_ba
-0000ca10: 7463 685d 2c20 6e5f 6469 6d20 2b20 312c  tch], n_dim + 1,
-0000ca20: 206e 5f64 696d 202b 2031 2920 666f 7220   n_dim + 1) for 
-0000ca30: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
-0000ca40: 732c 2069 6e73 7465 6164 206f 6620 7b6d  s, instead of {m
-0000ca50: 6174 7269 782e 7368 6170 657d 2e20 2229  atrix.shape}. ")
-0000ca60: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
-0000ca70: 735f 7374 7265 7463 6820 6973 206e 6f74  s_stretch is not
-0000ca80: 204e 6f6e 653a 206d 6174 7269 785b 2e2e   None: matrix[..
-0000ca90: 2e2c 203a 6e5f 6469 6d2c 202d 315d 202a  ., :n_dim, -1] *
-0000caa0: 3d20 7472 616e 735f 7374 7265 7463 680a  = trans_stretch.
-0000cab0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0000cac0: 7369 6e73 7461 6e63 6528 7370 6163 696e  sinstance(spacin
-0000cad0: 672c 2074 7570 6c65 293a 2073 7061 6369  g, tuple): spaci
-0000cae0: 6e67 203d 2074 6f5f 7475 706c 6528 7370  ng = to_tuple(sp
-0000caf0: 6163 696e 6729 0a20 2020 2020 2020 2069  acing).        i
-0000cb00: 6620 6c65 6e28 7370 6163 696e 6729 203d  f len(spacing) =
-0000cb10: 3d20 313a 2073 7061 6369 6e67 203d 2073  = 1: spacing = s
-0000cb20: 7061 6369 6e67 202a 206e 5f64 696d 0a20  pacing * n_dim. 
-0000cb30: 2020 2020 2020 2041 203d 2062 742e 6469         A = bt.di
-0000cb40: 6167 2862 6174 6f72 6368 5f74 656e 736f  ag(batorch_tenso
-0000cb50: 7228 6c69 7374 2873 7061 6369 6e67 2920  r(list(spacing) 
-0000cb60: 2b20 5b31 2e5d 2929 2e75 6e73 7175 6565  + [1.])).unsquee
-0000cb70: 7a65 285b 5d29 2e61 7374 7970 6528 6d61  ze([]).astype(ma
-0000cb80: 7472 6978 290a 2020 2020 2020 2020 7375  trix).        su
-0000cb90: 7065 7228 292e 5f5f 696e 6974 5f5f 286d  per().__init__(m
-0000cba0: 6174 7269 782c 2074 7261 6e73 5f73 7472  atrix, trans_str
-0000cbb0: 6574 6368 3d74 7261 6e73 5f73 7472 6574  etch=trans_stret
-0000cbc0: 6368 2c20 7370 6163 696e 673d 7370 6163  ch, spacing=spac
-0000cbd0: 696e 6729 0a0a 2020 2020 2020 2020 7365  ing)..        se
-0000cbe0: 6c66 2e6e 5f64 696d 203d 206d 6174 7269  lf.n_dim = matri
-0000cbf0: 782e 7369 7a65 282d 3129 202d 2031 0a20  x.size(-1) - 1. 
-0000cc00: 2020 2020 2020 2073 656c 662e 7472 616e         self.tran
-0000cc10: 735f 7374 7265 7463 6820 3d20 7472 616e  s_stretch = tran
-0000cc20: 735f 7374 7265 7463 680a 2020 2020 2020  s_stretch.      
-0000cc30: 2020 7365 6c66 2e73 7061 6369 6e67 203d    self.spacing =
-0000cc40: 2073 7061 6369 6e67 0a20 2020 2020 2020   spacing.       
-0000cc50: 2073 656c 662e 6d61 7472 6978 203d 2041   self.matrix = A
-0000cc60: 2e69 6e76 2829 2040 206d 6174 7269 7820  .inv() @ matrix 
-0000cc70: 4020 410a 2020 2020 2020 2020 7365 6c66  @ A.        self
-0000cc80: 2e62 6174 6368 5f70 6172 616d 2e61 7070  .batch_param.app
-0000cc90: 656e 6428 276d 6174 7269 7827 290a 0a20  end('matrix').. 
-0000cca0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-0000ccb0: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
-0000ccc0: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
-0000ccd0: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
-0000cce0: 2020 6d61 7472 6978 203d 2073 656c 662e    matrix = self.
-0000ccf0: 6d61 7472 6978 2e66 6c6f 6174 2829 0a20  matrix.float(). 
-0000cd00: 2020 2020 2020 206e 5f64 696d 203d 2073         n_dim = s
-0000cd10: 656c 662e 6e5f 6469 6d0a 2020 2020 2020  elf.n_dim.      
-0000cd20: 2020 4120 3d20 6d61 7472 6978 5b3a 2c20    A = matrix[:, 
-0000cd30: 3a6e 5f64 696d 2c20 3a6e 5f64 696d 5d0a  :n_dim, :n_dim].
-0000cd40: 2020 2020 2020 2020 6220 3d20 6d61 7472          b = matr
-0000cd50: 6978 5b3a 2c20 3a6e 5f64 696d 2c20 6e5f  ix[:, :n_dim, n_
-0000cd60: 6469 6d5d 0a20 2020 2020 2020 2073 6861  dim].        sha
-0000cd70: 7065 203d 2058 2e73 6861 7065 0a20 2020  pe = X.shape.   
-0000cd80: 2020 2020 2059 203d 2028 4120 4020 582e       Y = (A @ X.
-0000cd90: 666c 6174 7465 6e28 292e 6368 616e 6e65  flatten().channe
-0000cda0: 6c5f 6469 6d5f 284e 6f6e 6529 202b 2062  l_dim_(None) + b
-0000cdb0: 2e75 6e73 7175 6565 7a65 282d 3129 292e  .unsqueeze(-1)).
-0000cdc0: 7669 6577 2873 6861 7065 290a 2020 2020  view(shape).    
-0000cdd0: 2020 2020 7265 7475 726e 2059 0a20 2020      return Y.   
-0000cde0: 200a 2020 2020 6465 6620 6166 6669 6e65   .    def affine
-0000cdf0: 2873 656c 662c 206e 5f64 696d 3d4e 6f6e  (self, n_dim=Non
-0000ce00: 6529 3a0a 2020 2020 2020 2020 6176 6f75  e):.        avou
-0000ce10: 6368 286e 5f64 696d 2069 7320 4e6f 6e65  ch(n_dim is None
-0000ce20: 206f 7220 7365 6c66 2e6e 5f64 696d 203d   or self.n_dim =
-0000ce30: 3d20 6e5f 6469 6d29 0a20 2020 2020 2020  = n_dim).       
-0000ce40: 2072 6574 7572 6e20 7365 6c66 2e6d 6174   return self.mat
-0000ce50: 7269 780a 0a20 2020 2064 6566 2069 6e76  rix..    def inv
-0000ce60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ce70: 4120 3d20 6274 2e64 6961 6728 6261 746f  A = bt.diag(bato
-0000ce80: 7263 685f 7465 6e73 6f72 286c 6973 7428  rch_tensor(list(
-0000ce90: 7365 6c66 2e73 7061 6369 6e67 2920 2b20  self.spacing) + 
-0000cea0: 5b31 2e5d 2929 2e75 6e73 7175 6565 7a65  [1.])).unsqueeze
-0000ceb0: 285b 5d29 2e61 7374 7970 6528 7365 6c66  ([]).astype(self
-0000cec0: 2e6d 6174 7269 7829 0a20 2020 2020 2020  .matrix).       
-0000ced0: 2072 6574 7572 6e20 4166 6669 6e65 2841   return Affine(A
-0000cee0: 2040 2062 742e 696e 7628 7365 6c66 2e6d   @ bt.inv(self.m
-0000cef0: 6174 7269 7829 2040 2041 2e69 6e76 2829  atrix) @ A.inv()
-0000cf00: 2c20 7472 616e 735f 7374 7265 7463 6820  , trans_stretch 
-0000cf10: 3d20 312c 2073 7061 6369 6e67 3d73 656c  = 1, spacing=sel
-0000cf20: 662e 7370 6163 696e 6729 2e62 6163 6b77  f.spacing).backw
-0000cf30: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
-0000cf40: 7264 290a 0a40 616c 6961 7328 226c 6f67  rd)..@alias("log
-0000cf50: 4575 2229 0a63 6c61 7373 2050 6f6c 7941  Eu").class PolyA
-0000cf60: 6666 696e 6528 5370 6174 6961 6c54 7261  ffine(SpatialTra
-0000cf70: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
-0000cf80: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000cf90: 656c 662c 2064 6d61 7472 6963 6573 2c20  elf, dmatrices, 
-0000cfa0: 6d61 736b 732c 206f 7264 6572 3d32 2c20  masks, order=2, 
-0000cfb0: 6973 5f69 6e76 3d46 616c 7365 2c20 7472  is_inv=False, tr
-0000cfc0: 616e 735f 7374 7265 7463 683d 4e6f 6e65  ans_stretch=None
-0000cfd0: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
-0000cfe0: 2020 2020 2020 2050 6f6c 7920 6166 6669         Poly affi
-0000cff0: 6e65 2074 7261 6e73 666f 726d 6174 696f  ne transformatio
-0000d000: 6e20 7769 7468 2072 6573 7065 6374 2074  n with respect t
-0000d010: 6f20 7472 616e 7366 6f72 6d61 7469 6f6e  o transformation
-0000d020: 206d 6174 7269 6365 7320 5b31 5d2e 0a20   matrices [1].. 
-0000d030: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-0000d040: 2064 6d61 7472 6963 6573 2066 6f72 2074   dmatrices for t
-0000d050: 6869 7320 7472 616e 666f 726d 6174 696f  his tranformatio
-0000d060: 6e20 4953 204e 4f54 2074 6865 2061 6374  n IS NOT the act
-0000d070: 7561 6c20 6166 6669 6e65 206d 6174 7269  ual affine matri
-0000d080: 6365 732c 2062 7574 2049 5320 6120 6469  ces, but IS a di
-0000d090: 6666 6572 656e 7469 6174 696f 6e20 696e  fferentiation in
-0000d0a0: 7374 6561 642e 0a20 2020 2020 2020 200a  stead..        .
-0000d0b0: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
-0000d0c0: 2020 2020 2020 2020 2020 2020 646d 6174              dmat
-0000d0d0: 7269 6365 7320 5b62 742e 5465 6e73 6f72  rices [bt.Tensor
-0000d0e0: 206f 7220 6e70 2e6e 756d 7079 5d3a 204f   or np.numpy]: O
-0000d0f0: 6e65 2061 6666 696e 6520 6d61 7472 6978  ne affine matrix
-0000d100: 2066 6f72 2065 6163 6820 7265 6769 6f6e   for each region
-0000d110: 2e20 0a20 2020 2020 2020 2020 2020 2020  . .             
-0000d120: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-0000d130: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
-0000d140: 206e 5f64 696d 202b 2031 2c20 6e5f 6469   n_dim + 1, n_di
-0000d150: 6d20 2b20 3129 0a20 2020 2020 2020 2020  m + 1).         
-0000d160: 2020 206d 6173 6b73 205b 6274 2e54 656e     masks [bt.Ten
-0000d170: 736f 7220 6f72 206e 702e 6e75 6d70 795d  sor or np.numpy]
-0000d180: 3a20 4f6e 6520 302d 3120 6d61 736b 2066  : One 0-1 mask f
-0000d190: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
-0000d1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d1b0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-0000d1c0: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
-0000d1d0: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
-0000d1e0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
-0000d1f0: 2020 206f 7264 6572 205b 696e 745d 3a20     order [int]: 
-0000d200: 7468 6520 6f72 6465 7220 6f66 2069 6e74  the order of int
-0000d210: 6572 706f 6c61 7469 6f6e 2063 6f65 6666  erpolation coeff
-0000d220: 6963 6965 6e74 2e20 5468 6520 696e 666c  icient. The infl
-0000d230: 7565 6e63 6520 6f66 2061 6e20 6166 6669  uence of an affi
-0000d240: 6e65 2064 6563 6179 7320 6174 2061 2072  ne decays at a r
-0000d250: 6174 6520 6f66 2031 202f 2064 6973 7461  ate of 1 / dista
-0000d260: 6e63 655e 6f72 6465 722e 0a20 2020 2020  nce^order..     
-0000d270: 2020 2020 2020 2074 7261 6e73 5f73 7472         trans_str
-0000d280: 6574 6368 205b 696e 745d 3a20 6f6e 6c79  etch [int]: only
-0000d290: 2075 7365 6420 666f 7220 6974 6572 6174   used for iterat
-0000d2a0: 6976 6520 7061 7261 6d65 7465 7220 7472  ive parameter tr
-0000d2b0: 6169 6e69 6e67 2c20 3120 6279 2064 6566  aining, 1 by def
-0000d2c0: 6175 6c74 2e20 3230 2073 6565 6d73 2074  ault. 20 seems t
-0000d2d0: 6f20 6265 2061 2067 6f6f 6420 6368 6f69  o be a good choi
-0000d2e0: 6365 2e20 200a 2020 2020 2020 2020 2020  ce.  .          
-0000d2f0: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
-0000d300: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
-0000d310: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
-0000d320: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
-0000d330: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
-0000d340: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-0000d350: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-0000d360: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
-0000d370: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
-0000d380: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-0000d390: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-0000d3a0: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
-0000d3b0: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
-0000d3c0: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
-0000d3d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d3e0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-0000d3f0: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
-0000d400: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-0000d410: 6469 6d29 0a0a 2020 2020 2020 2020 5b31  dim)..        [1
-0000d420: 5d20 4172 7369 676e 7920 5620 2c20 436f  ] Arsigny V , Co
-0000d430: 6d6d 6f77 6963 6b20 4f20 2c20 4179 6163  mmowick O , Ayac
-0000d440: 6865 204e 202c 2065 7420 616c 2e20 4120  he N , et al. A 
-0000d450: 4661 7374 2061 6e64 204c 6f67 2d45 7563  Fast and Log-Euc
-0000d460: 6c69 6465 616e 2050 6f6c 7961 6666 696e  lidean Polyaffin
-0000d470: 6520 4672 616d 6577 6f72 6b20 666f 7220  e Framework for 
-0000d480: 4c6f 6361 6c6c 7920 0a20 2020 2020 2020  Locally .       
-0000d490: 2020 2020 204c 696e 6561 7220 5265 6769       Linear Regi
-0000d4a0: 7374 7261 7469 6f6e 5b4a 5d2e 204a 6f75  stration[J]. Jou
-0000d4b0: 726e 616c 206f 6620 4d61 7468 656d 6174  rnal of Mathemat
-0000d4c0: 6963 616c 2049 6d61 6769 6e67 2026 2056  ical Imaging & V
-0000d4d0: 6973 696f 6e2c 2032 3030 392c 2033 3328  ision, 2009, 33(
-0000d4e0: 3229 3a32 3232 2d32 3338 2e0a 2020 2020  2):222-238..    
-0000d4f0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-0000d500: 696d 706f 7274 2053 696d 706c 6549 544b  import SimpleITK
-0000d510: 2061 7320 7369 746b 0a20 2020 2020 2020   as sitk.       
-0000d520: 2066 726f 6d20 2e66 756e 6373 2069 6d70   from .funcs imp
-0000d530: 6f72 7420 6469 6c61 7465 2c20 6469 7374  ort dilate, dist
-0000d540: 616e 6365 5f6d 6170 0a20 2020 2020 2020  ance_map.       
-0000d550: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-0000d560: 6365 2864 6d61 7472 6963 6573 2c20 6274  ce(dmatrices, bt
-0000d570: 2e54 656e 736f 7229 3a20 646d 6174 7269  .Tensor): dmatri
-0000d580: 6365 7320 3d20 6274 2e74 656e 736f 7228  ces = bt.tensor(
-0000d590: 646d 6174 7269 6365 7329 0a20 2020 2020  dmatrices).     
-0000d5a0: 2020 2069 6620 646d 6174 7269 6365 732e     if dmatrices.
-0000d5b0: 6e5f 6469 6d20 3c3d 2033 2061 6e64 206e  n_dim <= 3 and n
-0000d5c0: 6f74 2064 6d61 7472 6963 6573 2e68 6173  ot dmatrices.has
-0000d5d0: 5f62 6174 6368 3a20 646d 6174 7269 6365  _batch: dmatrice
-0000d5e0: 7320 3d20 646d 6174 7269 6365 732e 756e  s = dmatrices.un
-0000d5f0: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
-0000d600: 2020 2020 6966 2064 6d61 7472 6963 6573      if dmatrices
-0000d610: 2e6e 5f64 696d 203c 3d20 3320 616e 6420  .n_dim <= 3 and 
-0000d620: 6e6f 7420 646d 6174 7269 6365 732e 6861  not dmatrices.ha
-0000d630: 735f 6368 616e 6e65 6c3a 2064 6d61 7472  s_channel: dmatr
-0000d640: 6963 6573 203d 2064 6d61 7472 6963 6573  ices = dmatrices
-0000d650: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
-0000d660: 2020 2020 2020 2069 6620 646d 6174 7269         if dmatri
-0000d670: 6365 732e 6e5f 6469 6d20 3d3d 2034 2061  ces.n_dim == 4 a
-0000d680: 6e64 2064 6d61 7472 6963 6573 2e73 6861  nd dmatrices.sha
-0000d690: 7065 5b32 5d20 3d3d 2064 6d61 7472 6963  pe[2] == dmatric
-0000d6a0: 6573 2e73 6861 7065 5b33 5d3a 0a20 2020  es.shape[3]:.   
-0000d6b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000d6c0: 646d 6174 7269 6365 732e 6861 735f 6261  dmatrices.has_ba
-0000d6d0: 7463 683a 2064 6d61 7472 6963 6573 2e62  tch: dmatrices.b
-0000d6e0: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
-0000d6f0: 2030 0a20 2020 2020 2020 2020 2020 2069   0.            i
-0000d700: 6620 6e6f 7420 646d 6174 7269 6365 732e  f not dmatrices.
-0000d710: 6861 735f 6368 616e 6e65 6c3a 2064 6d61  has_channel: dma
-0000d720: 7472 6963 6573 2e63 6861 6e6e 656c 5f64  trices.channel_d
-0000d730: 696d 656e 7369 6f6e 203d 2031 0a20 2020  imension = 1.   
-0000d740: 2020 2020 2061 766f 7563 6828 646d 6174       avouch(dmat
-0000d750: 7269 6365 732e 6861 735f 6261 7463 6820  rices.has_batch 
-0000d760: 616e 6420 646d 6174 7269 6365 732e 6861  and dmatrices.ha
-0000d770: 735f 6368 616e 6e65 6c2c 2022 506c 6561  s_channel, "Plea
-0000d780: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
-0000d790: 656e 736f 7220 6f66 2073 697a 6520 285b  ensor of size ([
-0000d7a0: 6e5f 6261 7463 685d 2c20 7b6e 5f72 6567  n_batch], {n_reg
-0000d7b0: 696f 6e7d 2c22 202b 0a20 2020 2020 2020  ion}," +.       
-0000d7c0: 2020 2020 2020 2020 6622 6e5f 6469 6d20          f"n_dim 
-0000d7d0: 2b20 312c 206e 5f64 696d 202b 2031 2920  + 1, n_dim + 1) 
-0000d7e0: 666f 7220 506f 6c79 4166 6669 6e65 2070  for PolyAffine p
-0000d7f0: 6172 616d 6574 6572 732c 2069 6e73 7465  arameters, inste
-0000d800: 6164 206f 6620 7b64 6d61 7472 6963 6573  ad of {dmatrices
-0000d810: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-0000d820: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
-0000d830: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
-0000d840: 3a20 646d 6174 7269 6365 735b 2e2e 2e2c  : dmatrices[...,
-0000d850: 203a 6e5f 6469 6d2c 202d 315d 202a 3d20   :n_dim, -1] *= 
-0000d860: 7472 616e 735f 7374 7265 7463 680a 2020  trans_stretch.  
-0000d870: 2020 2020 2020 6e5f 6469 6d20 3d20 646d        n_dim = dm
-0000d880: 6174 7269 6365 732e 7369 7a65 282d 3129  atrices.size(-1)
-0000d890: 202d 2031 0a20 2020 2020 2020 2069 6620   - 1.        if 
-0000d8a0: 6e6f 7420 6973 696e 7374 616e 6365 286d  not isinstance(m
-0000d8b0: 6173 6b73 2c20 6274 2e54 656e 736f 7229  asks, bt.Tensor)
-0000d8c0: 3a20 6d61 736b 7320 3d20 6274 2e74 656e  : masks = bt.ten
-0000d8d0: 736f 7228 6d61 736b 7329 0a20 2020 2020  sor(masks).     
-0000d8e0: 2020 2069 6620 6d61 736b 732e 6e5f 6469     if masks.n_di
-0000d8f0: 6d20 3c3d 206e 5f64 696d 202b 2031 2061  m <= n_dim + 1 a
-0000d900: 6e64 206e 6f74 206d 6173 6b73 2e68 6173  nd not masks.has
-0000d910: 5f62 6174 6368 3a20 6d61 736b 7320 3d20  _batch: masks = 
-0000d920: 6d61 736b 732e 756e 7371 7565 657a 6528  masks.unsqueeze(
-0000d930: 5b5d 290a 2020 2020 2020 2020 6966 206d  []).        if m
-0000d940: 6173 6b73 2e6e 5f64 696d 203c 3d20 6e5f  asks.n_dim <= n_
-0000d950: 6469 6d20 2b20 3120 616e 6420 6e6f 7420  dim + 1 and not 
-0000d960: 6d61 736b 732e 6861 735f 6368 616e 6e65  masks.has_channe
-0000d970: 6c3a 206d 6173 6b73 203d 206d 6173 6b73  l: masks = masks
-0000d980: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
-0000d990: 2020 2020 2020 2069 6620 6d61 736b 732e         if masks.
-0000d9a0: 6e5f 6469 6d20 3d3d 206e 5f64 696d 202b  n_dim == n_dim +
-0000d9b0: 2032 2061 6e64 206e 6f74 206d 6173 6b73   2 and not masks
-0000d9c0: 2e68 6173 5f62 6174 6368 3a20 6d61 736b  .has_batch: mask
-0000d9d0: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
-0000d9e0: 6e20 3d20 300a 2020 2020 2020 2020 6966  n = 0.        if
-0000d9f0: 206d 6173 6b73 2e6e 5f64 696d 203d 3d20   masks.n_dim == 
-0000da00: 6e5f 6469 6d20 2b20 3220 616e 6420 6e6f  n_dim + 2 and no
-0000da10: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
-0000da20: 6e65 6c3a 206d 6173 6b73 2e63 6861 6e6e  nel: masks.chann
-0000da30: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
-0000da40: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
-0000da50: 6d61 736b 732e 6861 735f 6261 7463 6820  masks.has_batch 
-0000da60: 616e 6420 6d61 736b 732e 6861 735f 6368  and masks.has_ch
-0000da70: 616e 6e65 6c2c 2022 506c 6561 7365 2075  annel, "Please u
-0000da80: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
-0000da90: 7220 6f66 2073 697a 6520 285b 6e5f 6261  r of size ([n_ba
-0000daa0: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
-0000dab0: 2c22 202b 0a20 2020 2020 2020 2020 2020  ," +.           
-0000dac0: 2020 2020 6622 6e40 312c 206e 4032 2c20      f"n@1, n@2, 
-0000dad0: 2e2e 2e2c 206e 406e 5f64 696d 2920 666f  ..., n@n_dim) fo
-0000dae0: 7220 506f 6c79 4166 6669 6e65 2070 6172  r PolyAffine par
-0000daf0: 616d 6574 6572 732c 2069 6e73 7465 6164  ameters, instead
-0000db00: 206f 6620 7b6d 6173 6b73 2e73 6861 7065   of {masks.shape
-0000db10: 7d2e 2022 290a 0a20 2020 2020 2020 2023  }. ")..        #
-0000db20: 2070 7265 7072 6f63 6573 7320 6d61 736b   preprocess mask
-0000db30: 7320 285b 6e5f 6261 7463 685d 2c20 7b6e  s ([n_batch], {n
-0000db40: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
-0000db50: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
-0000db60: 290a 2020 2020 2020 2020 6e5f 6261 7463  ).        n_batc
-0000db70: 6820 3d20 6d61 736b 732e 6e5f 6261 7463  h = masks.n_batc
-0000db80: 680a 2020 2020 2020 2020 6e5f 7265 6769  h.        n_regi
-0000db90: 6f6e 203d 206d 6173 6b73 2e6e 5f63 6861  on = masks.n_cha
-0000dba0: 6e6e 656c 0a20 2020 2020 2020 2064 6973  nnel.        dis
-0000dbb0: 203d 2064 6973 7461 6e63 655f 6d61 7028   = distance_map(
-0000dbc0: 6d61 736b 7329 0a20 2020 2020 2020 2064  masks).        d
-0000dbd0: 6973 203d 2028 6469 7320 2b20 3129 2e63  is = (dis + 1).c
-0000dbe0: 6c61 6d70 2830 290a 2020 2020 2020 2020  lamp(0).        
-0000dbf0: 2320 696d 706f 7274 206d 6963 6f6d 7075  # import micompu
-0000dc00: 7469 6e67 2e70 6c6f 7420 6173 2070 6c74  ting.plot as plt
-0000dc10: 0a20 2020 2020 2020 2023 2070 6c74 2e73  .        # plt.s
-0000dc20: 7562 706c 6f74 7328 3229 0a20 2020 2020  ubplots(2).     
-0000dc30: 2020 2023 2070 6c74 2e69 6d73 7368 6f77     # plt.imsshow
-0000dc40: 2864 6973 5b30 2c20 305d 2c20 6469 735b  (dis[0, 0], dis[
-0000dc50: 302c 2031 5d29 0a20 2020 2020 2020 2023  0, 1]).        #
-0000dc60: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
-0000dc70: 2020 2020 7765 6967 6874 7320 3d20 3120      weights = 1 
-0000dc80: 2f20 2864 6973 202a 2a20 6f72 6465 7220  / (dis ** order 
-0000dc90: 2b20 3165 2d35 290a 2020 2020 2020 2020  + 1e-5).        
-0000dca0: 7765 6967 6874 7320 3d20 7765 6967 6874  weights = weight
-0000dcb0: 7320 2f20 7765 6967 6874 732e 7375 6d28  s / weights.sum(
-0000dcc0: 7b7d 2920 2320 285b 6e5f 6261 7463 685d  {}) # ([n_batch]
-0000dcd0: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
-0000dce0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-0000dcf0: 5f64 696d 290a 2020 2020 2020 2020 0a20  _dim).        . 
-0000dd00: 2020 2020 2020 2023 2023 2064 6570 7265         # # depre
-0000dd10: 6361 7465 6420 7072 6570 726f 6365 7373  cated preprocess
-0000dd20: 206f 6620 6d61 736b 730a 2020 2020 2020   of masks.      
-0000dd30: 2020 2320 6d61 736b 7320 3d20 6d61 736b    # masks = mask
-0000dd40: 732e 6e75 6d70 7928 292e 6173 7479 7065  s.numpy().astype
-0000dd50: 286e 702e 696e 7429 0a20 2020 2020 2020  (np.int).       
-0000dd60: 2023 206e 5f62 6174 6368 2c20 6e5f 7265   # n_batch, n_re
-0000dd70: 6769 6f6e 2c20 2a5f 203d 206d 6173 6b73  gion, *_ = masks
-0000dd80: 2e73 6861 7065 0a20 2020 2020 2020 2023  .shape.        #
-0000dd90: 205f 6469 735f 6d61 7020 3d20 6274 2e7a   _dis_map = bt.z
-0000dda0: 6572 6f73 282a 6d61 736b 732e 7368 6170  eros(*masks.shap
-0000ddb0: 6529 0a20 2020 2020 2020 2023 2066 6f72  e).        # for
-0000ddc0: 2069 2069 6e20 7261 6e67 6528 6e5f 6261   i in range(n_ba
-0000ddd0: 7463 6829 3a0a 2020 2020 2020 2020 2320  tch):.        # 
-0000dde0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-0000ddf0: 6765 286e 5f72 6567 696f 6e29 3a0a 2020  ge(n_region):.  
-0000de00: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0000de10: 6d61 736b 5f69 6d61 6765 203d 2073 6974  mask_image = sit
-0000de20: 6b2e 4765 7449 6d61 6765 4672 6f6d 4172  k.GetImageFromAr
-0000de30: 7261 7928 6d61 736b 735b 692c 206a 5d2c  ray(masks[i, j],
-0000de40: 2069 7356 6563 746f 7220 3d20 4661 6c73   isVector = Fals
-0000de50: 6529 0a20 2020 2020 2020 2023 2020 2020  e).        #    
-0000de60: 2020 2020 2064 6973 5f6d 6170 203d 2073       dis_map = s
-0000de70: 6974 6b2e 4765 7441 7272 6179 5669 6577  itk.GetArrayView
-0000de80: 4672 6f6d 496d 6167 6528 7369 746b 2e53  FromImage(sitk.S
-0000de90: 6967 6e65 644d 6175 7265 7244 6973 7461  ignedMaurerDista
-0000dea0: 6e63 654d 6170 286d 6173 6b5f 696d 6167  nceMap(mask_imag
-0000deb0: 652c 2073 7175 6172 6564 4469 7374 616e  e, squaredDistan
-0000dec0: 6365 203d 2046 616c 7365 2c20 7573 6549  ce = False, useI
-0000ded0: 6d61 6765 5370 6163 696e 6720 3d20 4661  mageSpacing = Fa
-0000dee0: 6c73 6529 290a 2020 2020 2020 2020 2320  lse)).        # 
-0000def0: 2020 2020 2020 2020 6469 735f 6d61 7020          dis_map 
-0000df00: 3d20 6e70 2e61 7272 6179 2864 6973 5f6d  = np.array(dis_m
-0000df10: 6170 292e 6173 7479 7065 286e 702e 666c  ap).astype(np.fl
-0000df20: 6f61 7429 0a20 2020 2020 2020 2023 2020  oat).        #  
-0000df30: 2020 2020 2020 205f 6469 735f 6d61 705b         _dis_map[
-0000df40: 692c 206a 5d20 3d20 6274 2e74 656e 736f  i, j] = bt.tenso
-0000df50: 7228 6469 735f 6d61 7020 2a20 2864 6973  r(dis_map * (dis
-0000df60: 5f6d 6170 203e 2030 292e 6173 7479 7065  _map > 0).astype
-0000df70: 286e 702e 666c 6f61 7429 290a 2020 2020  (np.float)).    
-0000df80: 2020 2020 2320 6b20 3d20 320a 2020 2020      # k = 2.    
-0000df90: 2020 2020 2320 696e 7670 6f77 6b5f 6469      # invpowk_di
-0000dfa0: 735f 6d61 7020 3d20 3120 2f20 285f 6469  s_map = 1 / (_di
-0000dfb0: 735f 6d61 7020 2a2a 206b 202b 2031 652d  s_map ** k + 1e-
-0000dfc0: 3529 0a20 2020 2020 2020 2023 2073 756d  5).        # sum
-0000dfd0: 5f64 6973 5f6d 6170 203d 2069 6e76 706f  _dis_map = invpo
-0000dfe0: 776b 5f64 6973 5f6d 6170 2e73 756d 2831  wk_dis_map.sum(1
-0000dff0: 2c20 6b65 6570 6469 6d20 3d20 5472 7565  , keepdim = True
-0000e000: 290a 2020 2020 2020 2020 2320 7765 6967  ).        # weig
-0000e010: 6874 7320 3d20 696e 7670 6f77 6b5f 6469  hts = invpowk_di
-0000e020: 735f 6d61 7020 2f20 7375 6d5f 6469 735f  s_map / sum_dis_
-0000e030: 6d61 700a 2020 2020 2020 2020 2320 6672  map.        # fr
-0000e040: 6f6d 206d 6174 706c 6f74 6c69 6220 696d  om matplotlib im
-0000e050: 706f 7274 2070 7970 6c6f 7420 6173 2070  port pyplot as p
-0000e060: 6c74 0a20 2020 2020 2020 2023 2070 6c74  lt.        # plt
-0000e070: 2e73 7562 706c 6f74 2831 3231 293b 2070  .subplot(121); p
-0000e080: 6c74 2e69 6d73 686f 7728 7765 6967 6874  lt.imshow(weight
-0000e090: 735b 302c 2030 5d29 0a20 2020 2020 2020  s[0, 0]).       
-0000e0a0: 2023 2070 6c74 2e73 7562 706c 6f74 2831   # plt.subplot(1
-0000e0b0: 3232 293b 2070 6c74 2e69 6d73 686f 7728  22); plt.imshow(
-0000e0c0: 7765 6967 6874 735b 302c 2031 5d29 0a20  weights[0, 1]). 
-0000e0d0: 2020 2020 2020 2023 2070 6c74 2e73 686f         # plt.sho
-0000e0e0: 7728 290a 2020 2020 2020 2020 2320 6966  w().        # if
-0000e0f0: 2074 7261 6e73 5f73 7472 6574 6368 2069   trans_stretch i
-0000e100: 7320 6e6f 7420 4e6f 6e65 3a20 646d 6174  s not None: dmat
-0000e110: 7269 6365 7320 3d20 646d 6174 7269 6365  rices = dmatrice
-0000e120: 7320 2a20 6274 2e74 656e 736f 7228 5b31  s * bt.tensor([1
-0000e130: 2e5d 202a 206e 5f64 696d 202b 205b 7472  .] * n_dim + [tr
-0000e140: 616e 735f 7374 7265 7463 685d 292e 756e  ans_stretch]).un
-0000e150: 7371 7565 657a 6528 302c 2030 2c20 3029  squeeze(0, 0, 0)
-0000e160: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-0000e170: 292e 5f5f 696e 6974 5f5f 2864 6d61 7472  ).__init__(dmatr
-0000e180: 6963 6573 2c20 6d61 736b 733d 6d61 736b  ices, masks=mask
-0000e190: 732c 206f 7264 6572 3d6f 7264 6572 2c20  s, order=order, 
-0000e1a0: 6973 5f69 6e76 3d69 735f 696e 762c 2074  is_inv=is_inv, t
-0000e1b0: 7261 6e73 5f73 7472 6574 6368 3d74 7261  rans_stretch=tra
-0000e1c0: 6e73 5f73 7472 6574 6368 290a 2020 2020  ns_stretch).    
-0000e1d0: 2020 2020 7365 6c66 2e6e 5f62 6174 6368      self.n_batch
-0000e1e0: 203d 206e 5f62 6174 6368 0a20 2020 2020   = n_batch.     
-0000e1f0: 2020 2073 656c 662e 6e5f 6469 6d20 3d20     self.n_dim = 
-0000e200: 6e5f 6469 6d0a 2020 2020 2020 2020 7365  n_dim.        se
-0000e210: 6c66 2e6d 6173 6b73 203d 206d 6173 6b73  lf.masks = masks
-0000e220: 0a20 2020 2020 2020 2073 656c 662e 7765  .        self.we
-0000e230: 6967 6874 7320 3d20 7765 6967 6874 730a  ights = weights.
-0000e240: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000e250: 6e73 5f73 7472 6574 6368 203d 2074 7261  ns_stretch = tra
-0000e260: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
-0000e270: 2020 2073 656c 662e 646d 6174 7269 6365     self.dmatrice
-0000e280: 7320 3d20 646d 6174 7269 6365 730a 2020  s = dmatrices.  
-0000e290: 2020 2020 2020 7365 6c66 2e69 735f 696e        self.is_in
-0000e2a0: 7620 3d20 6973 5f69 6e76 0a20 2020 2020  v = is_inv.     
-0000e2b0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
-0000e2c0: 6f72 6465 720a 0a20 2020 2064 6566 205f  order..    def _
-0000e2d0: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
-0000e2e0: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
-0000e2f0: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
-0000e300: 290a 2020 2020 2020 2020 646d 6174 7269  ).        dmatri
-0000e310: 6365 7320 3d20 7365 6c66 2e64 6d61 7472  ces = self.dmatr
-0000e320: 6963 6573 2023 2028 5b6e 5f62 6174 6368  ices # ([n_batch
-0000e330: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
-0000e340: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
-0000e350: 2b20 3129 0a20 2020 2020 2020 2077 6569  + 1).        wei
-0000e360: 6768 7473 203d 2073 656c 662e 7765 6967  ghts = self.weig
-0000e370: 6874 7320 2320 285b 6e5f 6261 7463 685d  hts # ([n_batch]
-0000e380: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
-0000e390: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-0000e3a0: 5f64 696d 290a 2020 2020 2020 2020 6e5f  _dim).        n_
-0000e3b0: 6469 6d20 3d20 7365 6c66 2e6e 5f64 696d  dim = self.n_dim
-0000e3c0: 0a20 2020 2020 2020 206e 5f72 6567 696f  .        n_regio
-0000e3d0: 6e20 3d20 646d 6174 7269 6365 732e 6e5f  n = dmatrices.n_
-0000e3e0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
-0000e3f0: 5873 203d 2058 2e6d 756c 7469 706c 7928  Xs = X.multiply(
-0000e400: 6e5f 7265 6769 6f6e 2c20 7b7d 2920 2320  n_region, {}) # 
-0000e410: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000e420: 6567 696f 6e7d 2c20 6e5f 6469 6d2c 206e  egion}, n_dim, n
-0000e430: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
-0000e440: 6e5f 6469 6d29 0a20 2020 2020 2020 2041  n_dim).        A
-0000e450: 203d 2064 6d61 7472 6963 6573 5b2e 2e2e   = dmatrices[...
-0000e460: 2c20 3a6e 5f64 696d 2c20 3a6e 5f64 696d  , :n_dim, :n_dim
-0000e470: 5d0a 2020 2020 2020 2020 6220 3d20 646d  ].        b = dm
-0000e480: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
-0000e490: 6469 6d2c 206e 5f64 696d 3a5d 0a20 2020  dim, n_dim:].   
-0000e4a0: 2020 2020 2059 203d 2028 4120 4020 5873       Y = (A @ Xs
-0000e4b0: 2e66 6c61 7474 656e 2833 2920 2b20 6229  .flatten(3) + b)
-0000e4c0: 2e76 6965 775f 6173 2858 7329 0a20 2020  .view_as(Xs).   
-0000e4d0: 2020 2020 2044 203d 2028 5920 2a20 7765       D = (Y * we
-0000e4e0: 6967 6874 732e 756e 7371 7565 657a 6528  ights.unsqueeze(
-0000e4f0: 2929 2e73 756d 287b 7d29 2e77 6974 685f  )).sum({}).with_
-0000e500: 6368 616e 6e65 6c64 696d 2831 2920 2d20  channeldim(1) - 
-0000e510: 580a 2020 2020 2020 2020 6966 2073 656c  X.        if sel
-0000e520: 662e 6973 5f69 6e76 3a20 4420 3d20 2d44  f.is_inv: D = -D
-0000e530: 0a20 2020 2020 2020 2074 7261 6e73 203d  .        trans =
-0000e540: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
-0000e550: 6e74 4669 656c 6428 4429 0a20 2020 2020  ntField(D).     
-0000e560: 2020 2074 7261 6e73 3220 3d20 4465 6e73     trans2 = Dens
-0000e570: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
-0000e580: 6c64 2874 7261 6e73 2874 7261 6e73 2858  ld(trans(trans(X
-0000e590: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
-0000e5a0: 7472 616e 7334 203d 2044 656e 7365 4469  trans4 = DenseDi
-0000e5b0: 7370 6c61 6365 6d65 6e74 4669 656c 6428  splacementField(
-0000e5c0: 7472 616e 7332 2874 7261 6e73 3228 5829  trans2(trans2(X)
-0000e5d0: 2920 2d20 5829 0a20 2020 2020 2020 2074  ) - X).        t
-0000e5e0: 7261 6e73 3820 3d20 4465 6e73 6544 6973  rans8 = DenseDis
-0000e5f0: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
-0000e600: 7261 6e73 3428 7472 616e 7334 2858 2929  rans4(trans4(X))
-0000e610: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
-0000e620: 616e 7331 3620 3d20 4465 6e73 6544 6973  ans16 = DenseDis
-0000e630: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
-0000e640: 7261 6e73 3828 7472 616e 7338 2858 2929  rans8(trans8(X))
-0000e650: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
-0000e660: 616e 7333 3220 3d20 4465 6e73 6544 6973  ans32 = DenseDis
-0000e670: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
-0000e680: 7261 6e73 3136 2874 7261 6e73 3136 2858  rans16(trans16(X
-0000e690: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
-0000e6a0: 7472 616e 7336 3420 3d20 4465 6e73 6544  trans64 = DenseD
-0000e6b0: 6973 706c 6163 656d 656e 7446 6965 6c64  isplacementField
-0000e6c0: 2874 7261 6e73 3332 2874 7261 6e73 3332  (trans32(trans32
-0000e6d0: 2858 2929 202d 2058 290a 2020 2020 2020  (X)) - X).      
-0000e6e0: 2020 7265 7475 726e 2074 7261 6e73 3634    return trans64
-0000e6f0: 2858 290a 0a20 2020 2064 6566 2069 6e76  (X)..    def inv
-0000e700: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e710: 7265 7475 726e 2050 6f6c 7941 6666 696e  return PolyAffin
-0000e720: 6528 7365 6c66 2e64 6d61 7472 6963 6573  e(self.dmatrices
-0000e730: 2c20 7365 6c66 2e6d 6173 6b73 2c20 6f72  , self.masks, or
-0000e740: 6465 723d 7365 6c66 2e6f 7264 6572 2c20  der=self.order, 
-0000e750: 6973 5f69 6e76 3d6e 6f74 2073 656c 662e  is_inv=not self.
-0000e760: 6973 5f69 6e76 2c20 7472 616e 735f 7374  is_inv, trans_st
-0000e770: 7265 7463 6820 3d20 3129 2e62 6163 6b77  retch = 1).backw
-0000e780: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
-0000e790: 7264 290a 2020 2020 2020 2020 2320 6e5f  rd).        # n_
-0000e7a0: 6261 7463 6820 3d20 7365 6c66 2e64 6d61  batch = self.dma
-0000e7b0: 7472 6963 6573 2e6e 5f62 6174 6368 0a20  trices.n_batch. 
-0000e7c0: 2020 2020 2020 2023 2061 6666 7320 3d20         # affs = 
-0000e7d0: 6274 2e69 6e76 2873 656c 662e 646d 6174  bt.inv(self.dmat
-0000e7e0: 7269 6365 7329 0a20 2020 2020 2020 2023  rices).        #
-0000e7f0: 206d 6173 6b73 203d 2069 6e74 6572 706f   masks = interpo
-0000e800: 6c61 7469 6f6e 2873 656c 662e 6d61 736b  lation(self.mask
-0000e810: 732e 6d65 7267 6564 696d 7328 5b5d 2c20  s.mergedims([], 
-0000e820: 7b7d 292c 2041 6666 696e 6528 6274 2e6d  {}), Affine(bt.m
-0000e830: 6174 706f 7728 6166 6673 2e6d 6572 6765  atpow(affs.merge
-0000e840: 6469 6d73 285b 5d2c 207b 7d29 2c20 3634  dims([], {}), 64
-0000e850: 2929 292e 7370 6c69 7464 696d 285b 5d2c  ))).splitdim([],
-0000e860: 205b 6e5f 6261 7463 685d 2c20 7b2d 317d   [n_batch], {-1}
-0000e870: 290a 2020 2020 2020 2020 2320 7265 7475  ).        # retu
-0000e880: 726e 2050 6f6c 7941 6666 696e 6528 6166  rn PolyAffine(af
-0000e890: 6673 2c20 6d61 736b 7320 3d20 6d61 736b  fs, masks = mask
-0000e8a0: 732c 2074 7261 6e73 5f73 7472 6574 6368  s, trans_stretch
-0000e8b0: 203d 2073 656c 662e 7472 616e 735f 7374   = self.trans_st
-0000e8c0: 7265 7463 6829 2e62 6163 6b77 6172 645f  retch).backward_
-0000e8d0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
-0000e8e0: 0a40 616c 6961 7328 224c 4152 4d22 290a  .@alias("LARM").
-0000e8f0: 636c 6173 7320 4c6f 6361 6c6c 7941 6666  class LocallyAff
-0000e900: 696e 6528 5370 6174 6961 6c54 7261 6e73  ine(SpatialTrans
-0000e910: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
-0000e920: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000e930: 662c 206d 6174 7269 6365 732c 206d 6173  f, matrices, mas
-0000e940: 6b73 2c20 6f72 6465 723d 322c 2074 7261  ks, order=2, tra
-0000e950: 6e73 5f73 7472 6574 6368 3d4e 6f6e 652c  ns_stretch=None,
-0000e960: 2061 766f 6964 5f63 6f6e 666c 6963 743d   avoid_conflict=
-0000e970: 5472 7565 293a 0a20 2020 2020 2020 2027  True):.        '
-0000e980: 2727 0a20 2020 2020 2020 204c 6f63 616c  ''.        Local
-0000e990: 6c79 2061 6666 696e 6520 7472 616e 7366  ly affine transf
-0000e9a0: 6f72 6d61 7469 6f6e 2077 6974 6820 7265  ormation with re
-0000e9b0: 7370 6563 7420 746f 2074 7261 6e73 666f  spect to transfo
-0000e9c0: 726d 6174 696f 6e20 6d61 7472 6963 6573  rmation matrices
-0000e9d0: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
-0000e9e0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
-0000e9f0: 2020 2020 2020 2020 2020 206d 6174 7269             matri
-0000ea00: 6365 7320 5b62 742e 5465 6e73 6f72 206f  ces [bt.Tensor o
-0000ea10: 7220 6e70 2e6e 756d 7079 5d3a 204f 6e65  r np.numpy]: One
-0000ea20: 2061 6666 696e 6520 6d61 7472 6978 2066   affine matrix f
-0000ea30: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
-0000ea40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea50: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-0000ea60: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
-0000ea70: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
-0000ea80: 2b20 3129 0a20 2020 2020 2020 2020 2020  + 1).           
-0000ea90: 206d 6173 6b73 205b 6274 2e54 656e 736f   masks [bt.Tenso
-0000eaa0: 7220 6f72 206e 702e 6e75 6d70 795d 3a20  r or np.numpy]: 
-0000eab0: 4f6e 6520 302d 3120 6d61 736b 2066 6f72  One 0-1 mask for
-0000eac0: 2065 6163 6820 7265 6769 6f6e 2e20 0a20   each region. . 
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000eae0: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
-0000eaf0: 207b 6e5f 7265 6769 6f6e 7d2c 206e 4031   {n_region}, n@1
-0000eb00: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-0000eb10: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-0000eb20: 206f 7264 6572 205b 696e 745d 3a20 7468   order [int]: th
-0000eb30: 6520 6f72 6465 7220 6f66 2069 6e74 6572  e order of inter
-0000eb40: 706f 6c61 7469 6f6e 2063 6f65 6666 6963  polation coeffic
-0000eb50: 6965 6e74 2e20 5468 6520 696e 666c 7565  ient. The influe
-0000eb60: 6e63 6520 6f66 2061 6e20 6166 6669 6e65  nce of an affine
-0000eb70: 2064 6563 6179 7320 6174 2061 2072 6174   decays at a rat
-0000eb80: 6520 6f66 2031 202f 2064 6973 7461 6e63  e of 1 / distanc
-0000eb90: 655e 6f72 6465 722e 0a20 2020 2020 2020  e^order..       
-0000eba0: 2020 2020 2074 7261 6e73 5f73 7472 6574       trans_stret
-0000ebb0: 6368 205b 696e 745d 3a20 6f6e 6c79 2075  ch [int]: only u
-0000ebc0: 7365 6420 666f 7220 6974 6572 6174 6976  sed for iterativ
-0000ebd0: 6520 7061 7261 6d65 7465 7220 7472 6169  e parameter trai
-0000ebe0: 6e69 6e67 2c20 3120 6279 2064 6566 6175  ning, 1 by defau
-0000ebf0: 6c74 2e20 3230 2073 6565 6d73 2074 6f20  lt. 20 seems to 
-0000ec00: 6265 2061 2067 6f6f 6420 6368 6f69 6365  be a good choice
-0000ec10: 2e20 200a 2020 2020 2020 2020 2020 2020  .  .            
-0000ec20: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
-0000ec30: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
-0000ec40: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
-0000ec50: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
-0000ec60: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
-0000ec70: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
-0000ec80: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
-0000ec90: 6261 7463 683a 206f 7074 696f 6e61 6c5d  batch: optional]
-0000eca0: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
-0000ecb0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-0000ecc0: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
-0000ecd0: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
-0000ece0: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
-0000ecf0: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed10: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-0000ed20: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
-0000ed30: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-0000ed40: 6d29 0a0a 2020 2020 2020 2020 5b31 5d20  m)..        [1] 
-0000ed50: 5a68 7561 6e67 2058 202c 2052 686f 6465  Zhuang X , Rhode
-0000ed60: 204b 202c 2041 7272 6964 6765 2053 202c   K , Arridge S ,
-0000ed70: 2065 7420 616c 2e20 416e 2041 746c 6173   et al. An Atlas
-0000ed80: 2d42 6173 6564 2053 6567 6d65 6e74 6174  -Based Segmentat
-0000ed90: 696f 6e20 5072 6f70 6167 6174 696f 6e20  ion Propagation 
-0000eda0: 4672 616d 6577 6f72 6b20 5573 696e 6720  Framework Using 
-0000edb0: 4c6f 6361 6c6c 7920 4166 6669 6e65 200a  Locally Affine .
-0000edc0: 2020 2020 2020 2020 2020 2020 5265 6769              Regi
-0000edd0: 7374 7261 7469 6f6e 202d 2041 7070 6c69  stration - Appli
-0000ede0: 6361 7469 6f6e 2074 6f20 4175 746f 6d61  cation to Automa
-0000edf0: 7469 6320 5768 6f6c 6520 4865 6172 7420  tic Whole Heart 
-0000ee00: 5365 676d 656e 7461 7469 6f6e 5b4a 5d2e  Segmentation[J].
-0000ee10: 2053 7072 696e 6765 722c 2042 6572 6c69   Springer, Berli
-0000ee20: 6e2c 2048 6569 6465 6c62 6572 672c 2032  n, Heidelberg, 2
-0000ee30: 3030 382e 0a20 2020 2020 2020 2027 2727  008..        '''
-0000ee40: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-0000ee50: 5369 6d70 6c65 4954 4b20 6173 2073 6974  SimpleITK as sit
-0000ee60: 6b0a 2020 2020 2020 2020 6672 6f6d 202e  k.        from .
-0000ee70: 6675 6e63 7320 696d 706f 7274 2064 696c  funcs import dil
-0000ee80: 6174 652c 2064 6973 7461 6e63 655f 6d61  ate, distance_ma
-0000ee90: 700a 2020 2020 2020 2020 6d61 7472 6963  p.        matric
-0000eea0: 6573 203d 2062 6174 6f72 6368 5f74 656e  es = batorch_ten
-0000eeb0: 736f 7228 6d61 7472 6963 6573 290a 2020  sor(matrices).  
-0000eec0: 2020 2020 2020 6966 206d 6174 7269 6365        if matrice
-0000eed0: 732e 6e5f 6469 6d20 3c3d 2033 2061 6e64  s.n_dim <= 3 and
-0000eee0: 206e 6f74 206d 6174 7269 6365 732e 6861   not matrices.ha
-0000eef0: 735f 6261 7463 683a 206d 6174 7269 6365  s_batch: matrice
-0000ef00: 7320 3d20 6d61 7472 6963 6573 2e75 6e73  s = matrices.uns
-0000ef10: 7175 6565 7a65 285b 5d29 0a20 2020 2020  queeze([]).     
-0000ef20: 2020 2069 6620 6d61 7472 6963 6573 2e6e     if matrices.n
-0000ef30: 5f64 696d 203c 3d20 3320 616e 6420 6e6f  _dim <= 3 and no
-0000ef40: 7420 6d61 7472 6963 6573 2e68 6173 5f63  t matrices.has_c
-0000ef50: 6861 6e6e 656c 3a20 6d61 7472 6963 6573  hannel: matrices
-0000ef60: 203d 206d 6174 7269 6365 732e 756e 7371   = matrices.unsq
-0000ef70: 7565 657a 6528 7b7d 290a 2020 2020 2020  ueeze({}).      
-0000ef80: 2020 6966 206d 6174 7269 6365 732e 6e5f    if matrices.n_
-0000ef90: 6469 6d20 3d3d 2034 2061 6e64 206d 6174  dim == 4 and mat
-0000efa0: 7269 6365 732e 7368 6170 655b 325d 203d  rices.shape[2] =
-0000efb0: 3d20 6d61 7472 6963 6573 2e73 6861 7065  = matrices.shape
-0000efc0: 5b33 5d3a 0a20 2020 2020 2020 2020 2020  [3]:.           
-0000efd0: 2069 6620 6e6f 7420 6d61 7472 6963 6573   if not matrices
-0000efe0: 2e68 6173 5f62 6174 6368 3a20 6d61 7472  .has_batch: matr
-0000eff0: 6963 6573 2e62 6174 6368 5f64 696d 656e  ices.batch_dimen
-0000f000: 7369 6f6e 203d 2030 0a20 2020 2020 2020  sion = 0.       
-0000f010: 2020 2020 2069 6620 6e6f 7420 6d61 7472       if not matr
-0000f020: 6963 6573 2e68 6173 5f63 6861 6e6e 656c  ices.has_channel
-0000f030: 3a20 6d61 7472 6963 6573 2e63 6861 6e6e  : matrices.chann
-0000f040: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
-0000f050: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
-0000f060: 6d61 7472 6963 6573 2e68 6173 5f62 6174  matrices.has_bat
-0000f070: 6368 2061 6e64 206d 6174 7269 6365 732e  ch and matrices.
-0000f080: 6861 735f 6368 616e 6e65 6c2c 2022 506c  has_channel, "Pl
-0000f090: 6561 7365 2075 7365 2062 6174 6f72 6368  ease use batorch
-0000f0a0: 2074 656e 736f 7220 6f66 2073 697a 6520   tensor of size 
-0000f0b0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000f0c0: 6567 696f 6e7d 2c22 202b 0a20 2020 2020  egion}," +.     
-0000f0d0: 2020 2020 2020 2020 2020 6622 6e5f 6469            f"n_di
-0000f0e0: 6d20 2b20 312c 206e 5f64 696d 202b 2031  m + 1, n_dim + 1
-0000f0f0: 2920 666f 7220 4c6f 6361 6c6c 7941 6666  ) for LocallyAff
-0000f100: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
-0000f110: 696e 7374 6561 6420 6f66 207b 6d61 7472  instead of {matr
-0000f120: 6963 6573 2e73 6861 7065 7d2e 2022 290a  ices.shape}. ").
-0000f130: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
-0000f140: 5f73 7472 6574 6368 2069 7320 6e6f 7420  _stretch is not 
-0000f150: 4e6f 6e65 3a20 6d61 7472 6963 6573 5b2e  None: matrices[.
-0000f160: 2e2e 2c20 3a6e 5f64 696d 2c20 2d31 5d20  .., :n_dim, -1] 
-0000f170: 2a3d 2074 7261 6e73 5f73 7472 6574 6368  *= trans_stretch
-0000f180: 0a20 2020 2020 2020 206e 5f64 696d 203d  .        n_dim =
-0000f190: 206d 6174 7269 6365 732e 7369 7a65 282d   matrices.size(-
-0000f1a0: 3129 202d 2031 0a20 2020 2020 2020 206d  1) - 1.        m
-0000f1b0: 6173 6b73 203d 2062 6174 6f72 6368 5f74  asks = batorch_t
-0000f1c0: 656e 736f 7228 6d61 736b 7329 0a20 2020  ensor(masks).   
-0000f1d0: 2020 2020 2069 6620 6d61 736b 732e 6e5f       if masks.n_
-0000f1e0: 6469 6d20 3c3d 206e 5f64 696d 202b 2031  dim <= n_dim + 1
-0000f1f0: 2061 6e64 206e 6f74 206d 6173 6b73 2e68   and not masks.h
-0000f200: 6173 5f62 6174 6368 3a20 6d61 736b 7320  as_batch: masks 
-0000f210: 3d20 6d61 736b 732e 756e 7371 7565 657a  = masks.unsqueez
-0000f220: 6528 5b5d 290a 2020 2020 2020 2020 6966  e([]).        if
-0000f230: 206d 6173 6b73 2e6e 5f64 696d 203c 3d20   masks.n_dim <= 
-0000f240: 6e5f 6469 6d20 2b20 3120 616e 6420 6e6f  n_dim + 1 and no
-0000f250: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
-0000f260: 6e65 6c3a 206d 6173 6b73 203d 206d 6173  nel: masks = mas
-0000f270: 6b73 2e75 6e73 7175 6565 7a65 287b 7d29  ks.unsqueeze({})
-0000f280: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
-0000f290: 732e 6e5f 6469 6d20 3d3d 206e 5f64 696d  s.n_dim == n_dim
-0000f2a0: 202b 2032 2061 6e64 206e 6f74 206d 6173   + 2 and not mas
-0000f2b0: 6b73 2e68 6173 5f62 6174 6368 3a20 6d61  ks.has_batch: ma
-0000f2c0: 736b 732e 6261 7463 685f 6469 6d65 6e73  sks.batch_dimens
-0000f2d0: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
-0000f2e0: 6966 206d 6173 6b73 2e6e 5f64 696d 203d  if masks.n_dim =
-0000f2f0: 3d20 6e5f 6469 6d20 2b20 3220 616e 6420  = n_dim + 2 and 
-0000f300: 6e6f 7420 6d61 736b 732e 6861 735f 6368  not masks.has_ch
-0000f310: 616e 6e65 6c3a 206d 6173 6b73 2e63 6861  annel: masks.cha
-0000f320: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
-0000f330: 2031 0a20 2020 2020 2020 2061 766f 7563   1.        avouc
-0000f340: 6828 6d61 736b 732e 6861 735f 6261 7463  h(masks.has_batc
-0000f350: 6820 616e 6420 6d61 736b 732e 6861 735f  h and masks.has_
-0000f360: 6368 616e 6e65 6c2c 2022 506c 6561 7365  channel, "Please
-0000f370: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
-0000f380: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
-0000f390: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
-0000f3a0: 6e7d 2c22 202b 200a 2020 2020 2020 2020  n}," + .        
-0000f3b0: 2020 2020 2020 2066 226e 4031 2c20 6e40         f"n@1, n@
-0000f3c0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-0000f3d0: 2066 6f72 204c 6f63 616c 6c79 4166 6669   for LocallyAffi
-0000f3e0: 6e65 2070 6172 616d 6574 6572 732c 2069  ne parameters, i
-0000f3f0: 6e73 7465 6164 206f 6620 7b6d 6173 6b73  nstead of {masks
-0000f400: 2e73 6861 7065 7d2e 2022 290a 0a20 2020  .shape}. ")..   
-0000f410: 2020 2020 2023 2070 7265 7072 6f63 6573       # preproces
-0000f420: 7320 6d61 736b 730a 2020 2020 2020 2020  s masks.        
-0000f430: 6e5f 6261 7463 6820 3d20 6d61 7472 6963  n_batch = matric
-0000f440: 6573 2e6e 5f62 6174 6368 0a20 2020 2020  es.n_batch.     
-0000f450: 2020 206e 5f72 6567 696f 6e20 3d20 6d61     n_region = ma
-0000f460: 7472 6963 6573 2e6e 5f63 6861 6e6e 656c  trices.n_channel
-0000f470: 0a20 2020 2020 2020 2069 6620 6176 6f69  .        if avoi
-0000f480: 645f 636f 6e66 6c69 6374 3a0a 2020 2020  d_conflict:.    
-0000f490: 2020 2020 2020 2020 4769 203d 2041 6666          Gi = Aff
-0000f4a0: 696e 6528 6d61 7472 6963 6573 2e6d 6572  ine(matrices.mer
-0000f4b0: 6765 6469 6d73 287b 7d2c 205b 5d29 290a  gedims({}, [])).
-0000f4c0: 2020 2020 2020 2020 2020 2020 4769 5669              GiVi
-0000f4d0: 203d 2069 6e74 6572 706f 6c61 7469 6f6e   = interpolation
-0000f4e0: 286d 6173 6b73 2e6d 6572 6765 6469 6d73  (masks.mergedims
-0000f4f0: 287b 7d2c 205b 5d29 2c20 4769 2e69 6e76  ({}, []), Gi.inv
-0000f500: 2829 2c20 6d65 7468 6f64 3d27 4e65 6172  (), method='Near
-0000f510: 6573 7427 292e 7370 6c69 7464 696d 285b  est').splitdim([
-0000f520: 5d2c 205b 6e5f 6261 7463 685d 2c20 6e5f  ], [n_batch], n_
-0000f530: 7265 6769 6f6e 2920 2320 285b 6e5f 6261  region) # ([n_ba
-0000f540: 7463 685d 2c20 6e5f 7265 6769 6f6e 2c20  tch], n_region, 
-0000f550: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
-0000f560: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
-0000f570: 2020 2020 4769 5669 6a6f 696e 476b 566b      GiVijoinGkVk
-0000f580: 203d 2028 4769 5669 2e75 6e73 7175 6565   = (GiVi.unsquee
-0000f590: 7a65 2831 2920 2a20 4769 5669 2e75 6e73  ze(1) * GiVi.uns
-0000f5a0: 7175 6565 7a65 2832 2929 2e6d 6572 6765  queeze(2)).merge
-0000f5b0: 6469 6d73 2831 2c20 5b5d 292e 7769 7468  dims(1, []).with
-0000f5c0: 5f63 6861 6e6e 656c 6469 6d28 3129 2023  _channeldim(1) #
-0000f5d0: 2028 5b6e 5f62 6174 6368 2078 206e 5f72   ([n_batch x n_r
-0000f5e0: 6567 696f 6e5d 2c20 7b6e 5f72 6567 696f  egion], {n_regio
-0000f5f0: 6e7d 2c20 6e40 312c 206e 4032 2c20 2e2e  n}, n@1, n@2, ..
-0000f600: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-0000f610: 2020 2020 2020 2020 5269 6b20 3d20 696e          Rik = in
-0000f620: 7465 7270 6f6c 6174 696f 6e28 4769 5669  terpolation(GiVi
-0000f630: 6a6f 696e 476b 566b 2c20 4769 2c20 6d65  joinGkVk, Gi, me
-0000f640: 7468 6f64 3d27 4e65 6172 6573 7427 292e  thod='Nearest').
-0000f650: 7370 6c69 7464 696d 285b 5d2c 205b 6e5f  splitdim([], [n_
-0000f660: 6261 7463 685d 2c20 6e5f 7265 6769 6f6e  batch], n_region
-0000f670: 2920 2320 285b 6e5f 6261 7463 685d 2c20  ) # ([n_batch], 
-0000f680: 6e5f 7265 6769 6f6e 2c20 7b6e 5f72 6567  n_region, {n_reg
-0000f690: 696f 6e7d 2c20 6e40 312c 206e 4032 2c20  ion}, n@1, n@2, 
-0000f6a0: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
-0000f6b0: 2020 2020 2020 2020 2020 5552 696b 203d            URik =
-0000f6c0: 2028 5269 6b2e 7375 6d28 7b7d 292e 7769   (Rik.sum({}).wi
-0000f6d0: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
-0000f6e0: 202d 206d 6173 6b73 203e 2030 2e31 292e   - masks > 0.1).
-0000f6f0: 666c 6f61 7428 2920 2320 285b 6e5f 6261  float() # ([n_ba
-0000f700: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
-0000f710: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
-0000f720: 206e 406e 5f64 696d 290a 2020 2020 2020   n@n_dim).      
-0000f730: 2020 2020 2020 5552 696b 5f70 6c75 7320        URik_plus 
-0000f740: 3d20 6469 6c61 7465 2855 5269 6b2e 6d65  = dilate(URik.me
-0000f750: 7267 6564 696d 7328 7b7d 2c20 5b5d 292c  rgedims({}, []),
-0000f760: 2031 292e 7370 6c69 7464 696d 285b 5d2c   1).splitdim([],
-0000f770: 205b 6e5f 6261 7463 685d 2c20 6e5f 7265   [n_batch], n_re
-0000f780: 6769 6f6e 2920 2320 285b 6e5f 6261 7463  gion) # ([n_batc
-0000f790: 685d 2c20 7b6e 5f72 6567 696f 6e7d 2c20  h], {n_region}, 
-0000f7a0: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
-0000f7b0: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
-0000f7c0: 2020 2020 6d61 736b 7320 3d20 286d 6173      masks = (mas
-0000f7d0: 6b73 202d 2055 5269 6b5f 706c 7573 203e  ks - URik_plus >
-0000f7e0: 2030 2e31 292e 666c 6f61 7428 2920 2320   0.1).float() # 
-0000f7f0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
-0000f800: 6567 696f 6e7d 2c20 6e40 312c 206e 4032  egion}, n@1, n@2
-0000f810: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
-0000f820: 0a20 2020 2020 2020 2077 6569 6768 7473  .        weights
-0000f830: 203d 2031 202f 2028 6469 7374 616e 6365   = 1 / (distance
-0000f840: 5f6d 6170 286d 6173 6b73 2920 2a2a 206f  _map(masks) ** o
-0000f850: 7264 6572 202b 2031 652d 3529 0a20 2020  rder + 1e-5).   
-0000f860: 2020 2020 2077 6569 6768 7473 203d 2077       weights = w
-0000f870: 6569 6768 7473 202f 2077 6569 6768 7473  eights / weights
-0000f880: 2e73 756d 287b 7d29 2023 2028 5b6e 5f62  .sum({}) # ([n_b
-0000f890: 6174 6368 5d2c 207b 6e5f 7265 6769 6f6e  atch], {n_region
-0000f8a0: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-0000f8b0: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-0000f8c0: 2020 2023 2069 6620 7472 616e 735f 7374     # if trans_st
-0000f8d0: 7265 7463 6820 6973 206e 6f74 204e 6f6e  retch is not Non
-0000f8e0: 653a 206d 6174 7269 6365 7320 3d20 6d61  e: matrices = ma
-0000f8f0: 7472 6963 6573 202a 2062 6174 6f72 6368  trices * batorch
-0000f900: 5f74 656e 736f 7228 5b31 2e5d 202a 206e  _tensor([1.] * n
-0000f910: 5f64 696d 202b 205b 7472 616e 735f 7374  _dim + [trans_st
-0000f920: 7265 7463 685d 292e 756e 7371 7565 657a  retch]).unsqueez
-0000f930: 6528 302c 2030 2c20 3029 0a0a 2020 2020  e(0, 0, 0)..    
-0000f940: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0000f950: 6974 5f5f 286d 6174 7269 6365 732c 206d  it__(matrices, m
-0000f960: 6173 6b73 3d6d 6173 6b73 2c20 6f72 6465  asks=masks, orde
-0000f970: 723d 6f72 6465 722c 2074 7261 6e73 5f73  r=order, trans_s
-0000f980: 7472 6574 6368 3d74 7261 6e73 5f73 7472  tretch=trans_str
-0000f990: 6574 6368 290a 2020 2020 2020 2020 7365  etch).        se
-0000f9a0: 6c66 2e6e 5f62 6174 6368 203d 206e 5f62  lf.n_batch = n_b
-0000f9b0: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
-0000f9c0: 662e 6e5f 6469 6d20 3d20 6e5f 6469 6d0a  f.n_dim = n_dim.
-0000f9d0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000f9e0: 6b73 203d 206d 6173 6b73 0a20 2020 2020  ks = masks.     
-0000f9f0: 2020 2073 656c 662e 7765 6967 6874 7320     self.weights 
-0000fa00: 3d20 7765 6967 6874 730a 2020 2020 2020  = weights.      
-0000fa10: 2020 7365 6c66 2e74 7261 6e73 5f73 7472    self.trans_str
-0000fa20: 6574 6368 203d 2074 7261 6e73 5f73 7472  etch = trans_str
-0000fa30: 6574 6368 0a20 2020 2020 2020 2073 656c  etch.        sel
-0000fa40: 662e 6d61 7472 6963 6573 203d 206d 6174  f.matrices = mat
-0000fa50: 7269 6365 730a 2020 2020 2020 2020 7365  rices.        se
-0000fa60: 6c66 2e62 6174 6368 5f70 6172 616d 2e65  lf.batch_param.e
-0000fa70: 7874 656e 6428 5b27 6d61 7472 6963 6573  xtend(['matrices
-0000fa80: 272c 2027 7765 6967 6874 7327 2c20 276d  ', 'weights', 'm
-0000fa90: 6173 6b73 275d 290a 0a20 2020 2064 6566  asks'])..    def
-0000faa0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-0000fab0: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
-0000fac0: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
-0000fad0: 2858 290a 2020 2020 2020 2020 6d61 7472  (X).        matr
-0000fae0: 6963 6573 203d 2073 656c 662e 6d61 7472  ices = self.matr
-0000faf0: 6963 6573 0a20 2020 2020 2020 206d 6173  ices.        mas
-0000fb00: 6b73 203d 2073 656c 662e 6d61 736b 7320  ks = self.masks 
-0000fb10: 2320 285b 6e5f 6261 7463 685d 2c20 7b6e  # ([n_batch], {n
-0000fb20: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
-0000fb30: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
-0000fb40: 290a 2020 2020 2020 2020 7765 6967 6874  ).        weight
-0000fb50: 7320 3d20 7365 6c66 2e77 6569 6768 7473  s = self.weights
-0000fb60: 2023 2028 5b6e 5f62 6174 6368 5d2c 207b   # ([n_batch], {
-0000fb70: 6e5f 7265 6769 6f6e 7d2c 206e 4031 2c20  n_region}, n@1, 
-0000fb80: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-0000fb90: 6d29 0a20 2020 2020 2020 206e 5f64 696d  m).        n_dim
-0000fba0: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
-0000fbb0: 2020 2020 2020 6e5f 7265 6769 6f6e 203d        n_region =
-0000fbc0: 206d 6174 7269 6365 732e 6e5f 6368 616e   matrices.n_chan
-0000fbd0: 6e65 6c0a 2020 2020 2020 2020 5873 203d  nel.        Xs =
-0000fbe0: 2058 2e6d 756c 7469 706c 7928 6e5f 7265   X.multiply(n_re
-0000fbf0: 6769 6f6e 2c20 7b7d 2920 2320 285b 6e5f  gion, {}) # ([n_
-0000fc00: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
-0000fc10: 6e7d 2c20 6e5f 6469 6d2c 206e 4031 2c20  n}, n_dim, n@1, 
-0000fc20: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-0000fc30: 6d29 0a20 2020 2020 2020 2041 203d 206d  m).        A = m
-0000fc40: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
-0000fc50: 6469 6d2c 203a 6e5f 6469 6d5d 0a20 2020  dim, :n_dim].   
-0000fc60: 2020 2020 2062 203d 206d 6174 7269 6365       b = matrice
-0000fc70: 735b 2e2e 2e2c 203a 6e5f 6469 6d2c 206e  s[..., :n_dim, n
-0000fc80: 5f64 696d 3a5d 0a20 2020 2020 2020 2059  _dim:].        Y
-0000fc90: 203d 2028 4120 4020 5873 2e66 6c61 7474   = (A @ Xs.flatt
-0000fca0: 656e 2833 2920 2b20 6229 2e76 6965 775f  en(3) + b).view_
-0000fcb0: 6173 2858 7329 0a20 2020 2020 2020 2072  as(Xs).        r
-0000fcc0: 6574 7572 6e20 2877 6569 6768 7473 2e75  eturn (weights.u
-0000fcd0: 6e73 7175 6565 7a65 2829 202a 2059 292e  nsqueeze() * Y).
-0000fce0: 7375 6d28 7b7d 292e 7769 7468 5f63 6861  sum({}).with_cha
-0000fcf0: 6e6e 656c 6469 6d28 3129 202a 2028 3120  nneldim(1) * (1 
-0000fd00: 2d20 6d61 736b 732e 7375 6d28 7b7d 292e  - masks.sum({}).
-0000fd10: 756e 7371 7565 657a 6528 7b7d 2929 202b  unsqueeze({})) +
-0000fd20: 2028 5920 2a20 6d61 736b 732e 756e 7371   (Y * masks.unsq
-0000fd30: 7565 657a 6528 2929 2e73 756d 287b 7d29  ueeze()).sum({})
-0000fd40: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
-0000fd50: 2831 290a 0a20 2020 2064 6566 2069 6e76  (1)..    def inv
-0000fd60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000fd70: 6e5f 6261 7463 6820 3d20 7365 6c66 2e6d  n_batch = self.m
-0000fd80: 6174 7269 6365 732e 6e5f 6261 7463 680a  atrices.n_batch.
-0000fd90: 2020 2020 2020 2020 6166 6673 203d 2062          affs = b
-0000fda0: 742e 696e 7628 7365 6c66 2e6d 6174 7269  t.inv(self.matri
-0000fdb0: 6365 7329 0a20 2020 2020 2020 206d 6173  ces).        mas
-0000fdc0: 6b73 203d 2069 6e74 6572 706f 6c61 7469  ks = interpolati
-0000fdd0: 6f6e 2873 656c 662e 6d61 736b 732e 6d65  on(self.masks.me
-0000fde0: 7267 6564 696d 7328 5b5d 2c20 7b7d 292c  rgedims([], {}),
-0000fdf0: 2041 6666 696e 6528 6166 6673 2e6d 6572   Affine(affs.mer
-0000fe00: 6765 6469 6d73 285b 5d2c 207b 7d29 2929  gedims([], {})))
-0000fe10: 2e73 706c 6974 6469 6d28 5b5d 2c20 5b6e  .splitdim([], [n
-0000fe20: 5f62 6174 6368 5d2c 207b 2d31 7d29 0a20  _batch], {-1}). 
-0000fe30: 2020 2020 2020 2072 6574 7572 6e20 506f         return Po
-0000fe40: 6c79 4166 6669 6e65 2861 6666 732c 206d  lyAffine(affs, m
-0000fe50: 6173 6b73 203d 206d 6173 6b73 2c20 7472  asks = masks, tr
-0000fe60: 616e 735f 7374 7265 7463 6820 3d20 3129  ans_stretch = 1)
-0000fe70: 2e62 6163 6b77 6172 645f 2873 656c 662e  .backward_(self.
-0000fe80: 6261 636b 7761 7264 290a 0a40 616c 6961  backward)..@alia
-0000fe90: 7328 2246 4644 2229 0a63 6c61 7373 2046  s("FFD").class F
-0000fea0: 7265 6546 6f72 6d44 6566 6f72 6d61 7469  reeFormDeformati
-0000feb0: 6f6e 2853 7061 7469 616c 5472 616e 7366  on(SpatialTransf
-0000fec0: 6f72 6d61 7469 6f6e 293a 0a0a 2020 2020  ormation):..    
-0000fed0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000fee0: 662c 206f 6666 7365 7473 2c20 7370 6163  f, offsets, spac
-0000fef0: 696e 673d 312c 206f 7269 6769 6e3d 3029  ing=1, origin=0)
-0000ff00: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-0000ff10: 2020 2020 2020 4672 6565 2046 6f72 6d20        Free Form 
-0000ff20: 4465 666f 726d 6174 696f 6e20 2846 4644  Deformation (FFD
-0000ff30: 2920 7472 616e 7366 6f72 6d61 7469 6f6e  ) transformation
-0000ff40: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
-0000ff50: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
-0000ff60: 2020 2020 2020 2020 2020 206f 6666 7365             offse
-0000ff70: 7473 205b 6274 2e54 656e 736f 725d 3a20  ts [bt.Tensor]: 
-0000ff80: 7468 6520 4646 4420 6f66 6673 6574 732e  the FFD offsets.
-0000ff90: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000ffa0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-0000ffb0: 685d 2c20 7b6e 5f64 696d 7d2c 206d 4031  h], {n_dim}, m@1
-0000ffc0: 2c20 6d40 322c 202e 2e2e 2c20 6d40 6e5f  , m@2, ..., m@n_
-0000ffd0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-0000ffe0: 2020 2020 2066 6f72 206d 4031 2078 206d       for m@1 x m
-0000fff0: 4032 2078 202e 2e2e 2078 206d 406e 5f64  @2 x ... x m@n_d
-00010000: 696d 2067 7269 6420 6f66 20ce 9463 6f6e  im grid of ..con
-00010010: 7472 6f6c 2070 6f69 6e74 730a 2020 2020  trol points.    
-00010020: 2020 2020 2020 2020 7370 6163 696e 6720          spacing 
-00010030: 5b69 6e74 206f 7220 7475 706c 655d 3a20  [int or tuple]: 
-00010040: 4646 4420 7370 6163 696e 673b 2073 7061  FFD spacing; spa
-00010050: 6369 6e67 2062 6574 7765 656e 2046 4644  cing between FFD
-00010060: 2063 6f6e 7472 6f6c 2070 6f69 6e74 732e   control points.
-00010070: 200a 2020 2020 2020 2020 2020 2020 6f72   .            or
-00010080: 6967 696e 205b 696e 7420 6f72 2074 7570  igin [int or tup
-00010090: 6c65 5d3a 2046 4644 206f 7269 6769 6e3b  le]: FFD origin;
-000100a0: 2063 6f6f 7264 696e 6174 6520 666f 7220   coordinate for 
-000100b0: 7468 6520 2830 2c20 302c 2030 2920 636f  the (0, 0, 0) co
-000100c0: 6e74 726f 6c20 706f 696e 742e 200a 2020  ntrol point. .  
-000100d0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000100e0: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
-000100f0: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
-00010100: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
-00010110: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
-00010120: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
-00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010140: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
-00010150: 206f 7074 696f 6e61 6c5d 2c20 7b6e 5f64   optional], {n_d
-00010160: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
-00010170: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
-00010180: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-00010190: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
-000101a0: 2074 7261 6e73 666f 726d 6564 2063 6f6f   transformed coo
-000101b0: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
-000101c0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-000101d0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
-000101e0: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
-000101f0: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
-00010200: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00010210: 2020 2020 2020 5b31 5d20 5275 6563 6b65        [1] Ruecke
-00010220: 7274 2044 202c 2053 6f6e 6f64 6120 4c20  rt D , Sonoda L 
-00010230: 4920 2c20 4861 7965 7320 4320 2c20 6574  I , Hayes C , et
-00010240: 2061 6c2e 204e 6f6e 7269 6769 6420 7265   al. Nonrigid re
-00010250: 6769 7374 7261 7469 6f6e 2075 7369 6e67  gistration using
-00010260: 2066 7265 652d 666f 726d 2064 6566 6f72   free-form defor
-00010270: 6d61 7469 6f6e 733a 200a 2020 2020 2020  mations: .      
-00010280: 2020 2020 2020 6170 706c 6963 6174 696f        applicatio
-00010290: 6e20 746f 2062 7265 6173 7420 4d52 2069  n to breast MR i
-000102a0: 6d61 6765 735b 4a5d 2e20 4945 4545 2054  mages[J]. IEEE T
-000102b0: 7261 6e73 6163 7469 6f6e 7320 6f6e 204d  ransactions on M
-000102c0: 6564 6963 616c 2049 6d61 6769 6e67 2c20  edical Imaging, 
-000102d0: 3139 3939 2838 292e 0a20 2020 2020 2020  1999(8)..       
-000102e0: 2027 2727 0a20 2020 2020 2020 206f 6666   '''.        off
-000102f0: 7365 7473 203d 2062 6174 6f72 6368 5f74  sets = batorch_t
-00010300: 656e 736f 7228 6f66 6673 6574 7329 0a20  ensor(offsets). 
-00010310: 2020 2020 2020 2069 6620 6e6f 7420 6f66         if not of
-00010320: 6673 6574 732e 6861 735f 6368 616e 6e65  fsets.has_channe
-00010330: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
-00010340: 6620 6f66 6673 6574 732e 7369 7a65 2830  f offsets.size(0
-00010350: 2920 3d3d 206f 6666 7365 7473 2e6e 5f64  ) == offsets.n_d
-00010360: 696d 202d 2031 3a0a 2020 2020 2020 2020  im - 1:.        
-00010370: 2020 2020 2020 2020 6e5f 6469 6d20 3d20          n_dim = 
-00010380: 6f66 6673 6574 732e 7369 7a65 2830 290a  offsets.size(0).
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 6f66 6673 6574 732e 6368 616e 6e65 6c5f  offsets.channel_
-000103b0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
-000103c0: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-000103d0: 6673 6574 7320 3d20 6f66 6673 6574 732e  fsets = offsets.
-000103e0: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
-000103f0: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
-00010400: 6666 7365 7473 2e73 697a 6528 3129 203d  ffsets.size(1) =
-00010410: 3d20 6f66 6673 6574 732e 6e5f 6469 6d20  = offsets.n_dim 
-00010420: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
-00010430: 2020 2020 206e 5f64 696d 203d 206f 6666       n_dim = off
-00010440: 7365 7473 2e73 697a 6528 3129 0a20 2020  sets.size(1).   
-00010450: 2020 2020 2020 2020 2020 2020 206f 6666               off
-00010460: 7365 7473 2e63 6861 6e6e 656c 5f64 696d  sets.channel_dim
-00010470: 656e 7369 6f6e 203d 2031 0a20 2020 2020  ension = 1.     
-00010480: 2020 2020 2020 2065 6c73 653a 2072 6169         else: rai
-00010490: 7365 2054 7970 6545 7272 6f72 2866 2246  se TypeError(f"F
-000104a0: 4644 2070 6172 616d 6574 6572 7320 7769  FD parameters wi
-000104b0: 7468 2073 697a 6520 7b6f 6666 7365 7473  th size {offsets
-000104c0: 2e73 6861 7065 7d20 646f 6e6f 7420 6d61  .shape} donot ma
-000104d0: 7463 6820 285b 6e5f 6261 7463 685d 2c20  tch ([n_batch], 
-000104e0: 7b7b 6e5f 6469 6d7d 7d2c 206d 5f31 2c20  {{n_dim}}, m_1, 
-000104f0: 6d5f 322c 202e 2e2e 2c20 6d5f 7229 205b  m_2, ..., m_r) [
-00010500: 723d 6e5f 6469 6d5d 2e20 2229 0a20 2020  r=n_dim]. ").   
-00010510: 2020 2020 2069 6620 6e6f 7420 6f66 6673       if not offs
-00010520: 6574 732e 6861 735f 6261 7463 683a 0a20  ets.has_batch:. 
-00010530: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
-00010540: 203d 206f 6666 7365 7473 2e6e 5f63 6861   = offsets.n_cha
-00010550: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
-00010560: 2069 6620 6f66 6673 6574 732e 6e5f 6469   if offsets.n_di
-00010570: 6d20 3c3d 206e 5f64 696d 202b 2031 3a20  m <= n_dim + 1: 
-00010580: 6f66 6673 6574 7320 3d20 6f66 6673 6574  offsets = offset
-00010590: 732e 756e 7371 7565 657a 6528 5b5d 290a  s.unsqueeze([]).
-000105a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000105b0: 3a20 6f66 6673 6574 732e 6261 7463 685f  : offsets.batch_
-000105c0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
-000105d0: 2020 2020 2020 6176 6f75 6368 286f 6666        avouch(off
-000105e0: 7365 7473 2e68 6173 5f62 6174 6368 2061  sets.has_batch a
-000105f0: 6e64 206f 6666 7365 7473 2e68 6173 5f63  nd offsets.has_c
-00010600: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
-00010610: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
-00010620: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
-00010630: 2020 2020 2020 2020 2020 285b 6e5f 6261            ([n_ba
-00010640: 7463 685d 2c20 7b7b 6e5f 6469 6d7d 7d2c  tch], {{n_dim}},
-00010650: 206d 5f31 2c20 6d5f 322c 202e 2e2e 2c20   m_1, m_2, ..., 
-00010660: 6d5f 7229 205b 723d 6e5f 6469 6d5d 2066  m_r) [r=n_dim] f
-00010670: 6f72 2046 4644 2070 6172 616d 6574 6572  or FFD parameter
-00010680: 732c 2069 6e73 7465 6164 206f 6620 7b6f  s, instead of {o
-00010690: 6666 7365 7473 2e73 6861 7065 7d2e 2022  ffsets.shape}. "
-000106a0: 290a 2020 2020 2020 2020 6e5f 6469 6d20  ).        n_dim 
-000106b0: 3d20 6f66 6673 6574 732e 6e5f 6368 616e  = offsets.n_chan
-000106c0: 6e65 6c0a 2020 2020 2020 2020 7370 6163  nel.        spac
-000106d0: 696e 6720 3d20 746f 5f74 7570 6c65 2873  ing = to_tuple(s
-000106e0: 7061 6369 6e67 290a 2020 2020 2020 2020  pacing).        
-000106f0: 6f72 6967 696e 203d 2074 6f5f 7475 706c  origin = to_tupl
-00010700: 6528 6f72 6967 696e 290a 2020 2020 2020  e(origin).      
-00010710: 2020 6966 206c 656e 2873 7061 6369 6e67    if len(spacing
-00010720: 2920 3d3d 2031 3a20 7370 6163 696e 6720  ) == 1: spacing 
-00010730: 2a3d 206e 5f64 696d 0a20 2020 2020 2020  *= n_dim.       
-00010740: 2069 6620 6c65 6e28 6f72 6967 696e 2920   if len(origin) 
-00010750: 3d3d 2031 3a20 6f72 6967 696e 202a 3d20  == 1: origin *= 
-00010760: 6e5f 6469 6d0a 2020 2020 2020 2020 7375  n_dim.        su
-00010770: 7065 7228 292e 5f5f 696e 6974 5f5f 286f  per().__init__(o
-00010780: 6666 7365 7473 2c20 7370 6163 696e 673d  ffsets, spacing=
-00010790: 7370 6163 696e 672c 206f 7269 6769 6e3d  spacing, origin=
-000107a0: 6f72 6967 696e 290a 0a20 2020 2020 2020  origin)..       
-000107b0: 2073 656c 662e 6e5f 6469 6d20 3d20 6e5f   self.n_dim = n_
-000107c0: 6469 6d0a 2020 2020 2020 2020 7365 6c66  dim.        self
-000107d0: 2e6f 6666 7365 7473 203d 206f 6666 7365  .offsets = offse
-000107e0: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
-000107f0: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
-00010800: 670a 2020 2020 2020 2020 7365 6c66 2e6f  g.        self.o
-00010810: 7269 6769 6e20 3d20 6f72 6967 696e 0a20  rigin = origin. 
-00010820: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
-00010830: 685f 7061 7261 6d2e 6170 7065 6e64 2827  h_param.append('
-00010840: 6f66 6673 6574 7327 290a 2020 2020 0a20  offsets').    . 
-00010850: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
-00010860: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
-00010870: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
-00010880: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
-00010890: 2020 7368 6170 6520 3d20 582e 7368 6170    shape = X.shap
-000108a0: 650a 2020 2020 2020 2020 6e5f 6469 6d20  e.        n_dim 
-000108b0: 3d20 7365 6c66 2e6e 5f64 696d 0a20 2020  = self.n_dim.   
-000108c0: 2020 2020 206f 6666 7365 7473 203d 2073       offsets = s
-000108d0: 656c 662e 6f66 6673 6574 732e 666c 6f61  elf.offsets.floa
-000108e0: 7428 290a 2020 2020 2020 2020 7370 6163  t().        spac
-000108f0: 696e 6720 3d20 7365 6c66 2e73 7061 6369  ing = self.spaci
-00010900: 6e67 0a20 2020 2020 2020 206e 5f62 6174  ng.        n_bat
-00010910: 6368 203d 206f 6666 7365 7473 2e6e 5f62  ch = offsets.n_b
-00010920: 6174 6368 0a20 2020 2020 2020 2023 2058  atch.        # X
-00010930: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-00010940: 5f64 696d 7d2c 206e 5f64 6174 6120 3d20  _dim}, n_data = 
-00010950: 6e5f 3120 7820 6e5f 3220 7820 2e2e 2e20  n_1 x n_2 x ... 
-00010960: 7820 6e5f 7229 0a20 2020 2020 2020 2058  x n_r).        X
-00010970: 203d 2058 2e66 6c61 7474 656e 2829 0a20   = X.flatten(). 
-00010980: 2020 2020 2020 2058 202d 3d20 6274 2e63         X -= bt.c
-00010990: 6861 6e6e 656c 5f74 656e 736f 7228 7365  hannel_tensor(se
-000109a0: 6c66 2e6f 7269 6769 6e29 0a20 2020 2020  lf.origin).     
-000109b0: 2020 206e 5f64 6174 6120 3d20 582e 7369     n_data = X.si
-000109c0: 7a65 282d 3129 0a20 2020 2020 2020 2073  ze(-1).        s
-000109d0: 697a 6520 3d20 6274 2e63 6861 6e6e 656c  ize = bt.channel
-000109e0: 5f74 656e 736f 7228 6f66 6673 6574 732e  _tensor(offsets.
-000109f0: 7370 6163 6529 0a20 2020 2020 2020 2023  space).        #
-00010a00: 204e 6f72 6d61 6c69 7a65 2058 2069 6e20   Normalize X in 
-00010a10: 7468 6520 646f 6d61 696e 2028 6d5f 312c  the domain (m_1,
-00010a20: 206d 5f32 2c20 2e2e 2e2c 206d 5f7b 6e5f   m_2, ..., m_{n_
-00010a30: 6469 6d7d 292e 0a20 2020 2020 2020 2046  dim})..        F
-00010a40: 4644 5820 3d20 5820 2f20 6274 2e63 6861  FDX = X / bt.cha
-00010a50: 6e6e 656c 5f74 656e 736f 7228 7370 6163  nnel_tensor(spac
-00010a60: 696e 6729 2e66 6c6f 6174 2829 0a20 2020  ing).float().   
-00010a70: 2020 2020 2069 5820 3d20 6274 2e66 6c6f       iX = bt.flo
-00010a80: 6f72 2846 4644 5829 2e66 6c6f 6174 2829  or(FFDX).float()
-00010a90: 3b20 7558 203d 2046 4644 5820 2d20 6958  ; uX = FFDX - iX
-00010aa0: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
-00010ab0: 7465 2074 6865 2077 6569 6768 7473 2e20  te the weights. 
-00010ac0: 573a 2028 342c 205b 6e5f 6261 7463 685d  W: (4, [n_batch]
-00010ad0: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
-00010ae0: 6120 3d20 6e5f 3120 7820 6e5f 3220 7820  a = n_1 x n_2 x 
-00010af0: 2e2e 2e20 7820 6e5f 7229 0a20 2020 2020  ... x n_r).     
-00010b00: 2020 2069 203d 2062 742e 6172 616e 6765     i = bt.arange
-00010b10: 282d 312c 2033 292e 6578 7061 6e64 5f74  (-1, 3).expand_t
-00010b20: 6f28 342c 205b 6e5f 6261 7463 685d 2c20  o(4, [n_batch], 
-00010b30: 7b6e 5f64 696d 7d2c 206e 5f64 6174 612c  {n_dim}, n_data,
-00010b40: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-00010b50: 2057 203d 2042 7370 6c69 6e65 2869 2c20   W = Bspline(i, 
-00010b60: 7558 2e6d 756c 7469 706c 7928 342c 2030  uX.multiply(4, 0
-00010b70: 2929 0a20 2020 2020 2020 2022 436f 6d70  )).        "Comp
-00010b80: 7574 6520 4646 4420 5472 616e 7366 6f72  ute FFD Transfor
-00010b90: 6d61 7469 6f6e 220a 2020 2020 2020 2020  mation".        
-00010ba0: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
-00010bb0: 735f 6c69 6b65 2858 290a 2020 2020 2020  s_like(X).      
-00010bc0: 2020 2320 4c6f 6f70 2069 6e20 7468 6520    # Loop in the 
-00010bd0: 7370 6163 6520 7b2d 312c 2030 2c20 312c  space {-1, 0, 1,
-00010be0: 2032 7d20 5e20 6e5f 6469 6d3b 2047 2069   2} ^ n_dim; G i
-00010bf0: 7320 696e 2028 302c 2031 2c20 322c 2033  s in (0, 1, 2, 3
-00010c00: 290a 2020 2020 2020 2020 666f 7220 4720  ).        for G 
-00010c10: 696e 2062 742e 696d 6167 655f 6772 6964  in bt.image_grid
-00010c20: 285b 345d 2a6e 5f64 696d 292e 666c 6174  ([4]*n_dim).flat
-00010c30: 7465 6e28 292e 7472 616e 7370 6f73 6528  ten().transpose(
-00010c40: 302c 2031 293a 0a20 2020 2020 2020 2020  0, 1):.         
-00010c50: 2020 2047 203d 2062 742e 6368 616e 6e65     G = bt.channe
-00010c60: 6c5f 7465 6e73 6f72 2847 290a 2020 2020  l_tensor(G).    
-00010c70: 2020 2020 2020 2020 2320 5765 6967 6874          # Weight
-00010c80: 7320 666f 7220 6561 6368 2070 6f69 6e74  s for each point
-00010c90: 3a20 5b70 726f 6475 6374 206f 6620 575b  : [product of W[
-00010ca0: 475b 445d 2c20 742c 2044 2c20 785d 2066  G[D], t, D, x] f
-00010cb0: 6f72 2044 2069 6e20 7261 6e67 6528 6e5f  or D in range(n_
-00010cc0: 6469 6d29 5d20 666f 7220 706f 696e 7420  dim)] for point 
-00010cd0: 7820 616e 6420 6261 7463 6820 742e 0a20  x and batch t.. 
-00010ce0: 2020 2020 2020 2020 2020 2023 2057 673a             # Wg:
-00010cf0: 2028 5b6e 5f62 6174 6368 5d2c 207b 317d   ([n_batch], {1}
-00010d00: 2c20 6e5f 6461 7461 203d 206e 5f31 2078  , n_data = n_1 x
-00010d10: 206e 5f32 2078 202e 2e2e 2078 206e 5f72   n_2 x ... x n_r
-00010d20: 290a 2020 2020 2020 2020 2020 2020 5767  ).            Wg
-00010d30: 203d 2057 2e67 6174 6865 7228 302c 2047   = W.gather(0, G
-00010d40: 2e65 7870 616e 645f 746f 2828 312c 2920  .expand_to((1,) 
-00010d50: 2b20 572e 7368 6170 655b 313a 5d29 292e  + W.shape[1:])).
-00010d60: 7371 7565 657a 6528 3029 2e70 726f 6428  squeeze(0).prod(
-00010d70: 7b7d 2c20 6b65 6570 6469 6d3d 5472 7565  {}, keepdim=True
-00010d80: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00010d90: 436f 6d70 7574 6520 7468 6520 696e 6469  Compute the indi
-00010da0: 6365 7320 6f66 2072 656c 6174 6564 2063  ces of related c
-00010db0: 6f6e 7472 6f6c 2070 6f69 6e74 732e 2049  ontrol points. I
-00010dc0: 6e64 3a20 285b 6e5f 6261 7463 685d 2c20  nd: ([n_batch], 
-00010dd0: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
-00010de0: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
-00010df0: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
-00010e00: 2020 2020 2049 6e64 203d 2062 742e 636c       Ind = bt.cl
-00010e10: 616d 7028 6958 2e6c 6f6e 6728 2920 2b20  amp(iX.long() + 
-00010e20: 4720 2d20 312c 206d 696e 3d30 290a 2020  G - 1, min=0).  
-00010e30: 2020 2020 2020 2020 2020 496e 6420 3d20            Ind = 
-00010e40: 6274 2e6d 696e 2849 6e64 2c20 2873 697a  bt.min(Ind, (siz
-00010e50: 6520 2d20 3129 2e65 7870 616e 645f 746f  e - 1).expand_to
-00010e60: 2849 6e64 2929 0a20 2020 2020 2020 2020  (Ind)).         
-00010e70: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
-00010e80: 2069 6e64 6963 6573 2074 6f20 3120 6469   indices to 1 di
-00010e90: 6d65 6e73 696f 6e61 6c2e 2044 6f74 3a20  mensional. Dot: 
-00010ea0: 285b 6e5f 6261 7463 685d 2c20 6e5f 6461  ([n_batch], n_da
-00010eb0: 7461 203d 206e 5f31 2078 206e 5f32 2078  ta = n_1 x n_2 x
-00010ec0: 202e 2e2e 2078 206e 5f72 290a 2020 2020   ... x n_r).    
-00010ed0: 2020 2020 2020 2020 446f 7420 3d20 496e          Dot = In
-00010ee0: 645b 3a2c 2030 5d0a 2020 2020 2020 2020  d[:, 0].        
-00010ef0: 2020 2020 666f 7220 7220 696e 2072 616e      for r in ran
-00010f00: 6765 2831 2c20 6e5f 6469 6d29 3a20 446f  ge(1, n_dim): Do
-00010f10: 7420 2a3d 2073 697a 655b 725d 3b20 446f  t *= size[r]; Do
-00010f20: 7420 2b3d 2049 6e64 5b3a 2c20 725d 0a20  t += Ind[:, r]. 
-00010f30: 2020 2020 2020 2020 2020 2023 204f 6274             # Obt
-00010f40: 6169 6e20 7468 6520 636f 6f72 6469 6e61  ain the coordina
-00010f50: 7465 7320 6f66 2074 6865 2063 6f6e 7472  tes of the contr
-00010f60: 6f6c 2070 6f69 6e74 732e 2043 506f 696e  ol points. CPoin
-00010f70: 7473 3a20 285b 6e5f 6261 7463 685d 2c20  ts: ([n_batch], 
-00010f80: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
-00010f90: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
-00010fa0: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
-00010fb0: 2020 2020 2043 506f 696e 7473 203d 206f       CPoints = o
-00010fc0: 6666 7365 7473 2e66 6c61 7474 656e 2829  ffsets.flatten()
-00010fd0: 2e67 6174 6865 7228 2d31 2c20 446f 742e  .gather(-1, Dot.
-00010fe0: 6c6f 6e67 2829 2e65 7870 616e 645f 746f  long().expand_to
-00010ff0: 2849 6e64 2929 2e66 6c6f 6174 2829 0a20  (Ind)).float(). 
-00011000: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
-00011010: 2074 6865 2077 6569 6768 7465 6420 636f   the weighted co
-00011020: 6e74 726f 6c20 636f 6f72 6469 6e61 7465  ntrol coordinate
-00011030: 7320 746f 2074 6865 206f 7574 7075 7420  s to the output 
-00011040: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
-00011050: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-00011060: 2b3d 2028 5767 202a 2043 506f 696e 7473  += (Wg * CPoints
-00011070: 292e 7669 6577 5f61 7328 5829 0a20 2020  ).view_as(X).   
-00011080: 2020 2020 2023 2044 656e 6f72 6d61 6c69       # Denormali
-00011090: 7a65 2074 6865 206f 7574 7075 7473 2e0a  ze the outputs..
-000110a0: 2020 2020 2020 2020 6f75 7470 7574 202b          output +
-000110b0: 3d20 580a 2020 2020 2020 2020 6f75 7470  = X.        outp
-000110c0: 7574 202b 3d20 6274 2e63 6861 6e6e 656c  ut += bt.channel
-000110d0: 5f74 656e 736f 7228 7365 6c66 2e6f 7269  _tensor(self.ori
-000110e0: 6769 6e29 0a20 2020 2020 2020 2072 6574  gin).        ret
-000110f0: 7572 6e20 6f75 7470 7574 2e76 6965 7728  urn output.view(
-00011100: 7368 6170 6529 0a0a 4061 6c69 6173 2822  shape)..@alias("
-00011110: 4444 4622 290a 636c 6173 7320 4465 6e73  DDF").class Dens
-00011120: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
-00011130: 6c64 2853 7061 7469 616c 5472 616e 7366  ld(SpatialTransf
-00011140: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
-00011150: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00011160: 2c20 6469 7370 6c61 6365 6d65 6e74 732c  , displacements,
-00011170: 2073 6861 7065 3d4e 6f6e 652c 2069 6e74   shape=None, int
-00011180: 6572 706f 6c61 7465 3d46 616c 7365 293a  erpolate=False):
-00011190: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000111a0: 2020 2020 2044 656e 7365 2044 6973 706c       Dense Displ
-000111b0: 6163 656d 656e 7420 4669 656c 6420 2844  acement Field (D
-000111c0: 4446 2920 7472 616e 7366 6f72 6d61 7469  DF) transformati
-000111d0: 6f6e 2e0a 2020 2020 2020 2020 0a20 2020  on..        .   
-000111e0: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
-000111f0: 2020 2020 2020 2020 2064 6973 706c 6163           displac
-00011200: 656d 656e 7473 205b 6274 2e54 656e 736f  ements [bt.Tenso
-00011210: 725d 3a20 7468 6520 6469 7370 6c61 6365  r]: the displace
-00011220: 6d65 6e74 206f 6620 6561 6368 2076 6f78  ment of each vox
-00011230: 656c 2e20 0a20 2020 2020 2020 2020 2020  el. .           
-00011240: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-00011250: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
-00011260: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
-00011270: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
-00011280: 2020 2020 7368 6170 6520 5b62 742e 5369      shape [bt.Si
-00011290: 7a65 206f 7220 7475 706c 655d 3a20 7468  ze or tuple]: th
-000112a0: 6520 7368 6170 6520 6f66 2064 6973 706c  e shape of displ
-000112b0: 6163 656d 656e 7420 286e 6565 6465 6420  acement (needed 
-000112c0: 6966 2069 6e70 7574 2064 6973 706c 6163  if input displac
-000112d0: 656d 656e 7420 6973 2061 2074 7261 6e73  ement is a trans
-000112e0: 666f 726d 6174 696f 6e29 2e20 0a20 2020  formation). .   
-000112f0: 2020 2020 2020 2020 2069 6e74 6572 706f           interpo
-00011300: 6c61 7465 205b 626f 6f6c 5d3a 2057 6865  late [bool]: Whe
-00011310: 7468 6572 2074 6f20 666f 7263 6520 696e  ther to force in
-00011320: 7465 7270 6f6c 6174 696f 6e20 696e 2061  terpolation in a
-00011330: 7070 6c79 2e20 0a20 2020 2020 2020 2020  pply. .         
-00011340: 2020 200a 2020 2020 2020 2020 5768 656e     .        When
-00011350: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
-00011360: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
-00011370: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
-00011380: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
-00011390: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
-000113a0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
-000113b0: 5b6e 5f62 6174 6368 3a20 6f70 7469 6f6e  [n_batch: option
-000113c0: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  al], {n_dim}, n@
-000113d0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-000113e0: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-000113f0: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
-00011400: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
-00011410: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
-00011420: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00011430: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
-00011440: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  ch], {n_dim}, n@
-00011450: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
-00011460: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
-00011470: 270a 2020 2020 2020 2020 6966 2069 7369  '.        if isi
-00011480: 6e73 7461 6e63 6528 6469 7370 6c61 6365  nstance(displace
-00011490: 6d65 6e74 732c 2053 7061 7469 616c 5472  ments, SpatialTr
-000114a0: 616e 7366 6f72 6d61 7469 6f6e 293a 2064  ansformation): d
-000114b0: 6973 706c 6163 656d 656e 7473 203d 2064  isplacements = d
-000114c0: 6973 706c 6163 656d 656e 7473 2e74 6f44  isplacements.toD
-000114d0: 4446 2873 6861 7065 290a 2020 2020 2020  DF(shape).      
-000114e0: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
-000114f0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
-00011500: 2864 6973 706c 6163 656d 656e 7473 290a  (displacements).
-00011510: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00011520: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
-00011530: 5f63 6861 6e6e 656c 3a0a 2020 2020 2020  _channel:.      
-00011540: 2020 2020 2020 6966 2064 6973 706c 6163        if displac
-00011550: 656d 656e 7473 2e73 697a 6528 3029 203d  ements.size(0) =
-00011560: 3d20 6469 7370 6c61 6365 6d65 6e74 732e  = displacements.
-00011570: 6e5f 6469 6d20 2d20 313a 0a20 2020 2020  n_dim - 1:.     
-00011580: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
-00011590: 203d 2064 6973 706c 6163 656d 656e 7473   = displacements
-000115a0: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
-000115b0: 2020 2020 2020 2020 2064 6973 706c 6163           displac
-000115c0: 656d 656e 7473 2e63 6861 6e6e 656c 5f64  ements.channel_d
-000115d0: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
-000115e0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000115f0: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
-00011600: 706c 6163 656d 656e 7473 2e75 6e73 7175  placements.unsqu
-00011610: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
-00011620: 2020 2020 2065 6c69 6620 6469 7370 6c61       elif displa
-00011630: 6365 6d65 6e74 732e 7369 7a65 2831 2920  cements.size(1) 
-00011640: 3d3d 2064 6973 706c 6163 656d 656e 7473  == displacements
-00011650: 2e6e 5f64 696d 202d 2032 3a0a 2020 2020  .n_dim - 2:.    
-00011660: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
-00011670: 6d20 3d20 6469 7370 6c61 6365 6d65 6e74  m = displacement
-00011680: 732e 7369 7a65 2831 290a 2020 2020 2020  s.size(1).      
-00011690: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-000116a0: 6365 6d65 6e74 732e 6368 616e 6e65 6c5f  cements.channel_
-000116b0: 6469 6d65 6e73 696f 6e20 3d20 310a 2020  dimension = 1.  
-000116c0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-000116d0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000116e0: 6622 4444 4620 7061 7261 6d65 7465 7273  f"DDF parameters
-000116f0: 2077 6974 6820 7369 7a65 207b 6469 7370   with size {disp
-00011700: 6c61 6365 6d65 6e74 732e 7368 6170 657d  lacements.shape}
-00011710: 2064 6f6e 6f74 206d 6174 6368 2028 5b6e   donot match ([n
-00011720: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
-00011730: 7d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  }}, n@1, n@2, ..
-00011740: 2e2c 206e 406e 5f64 696d 292e 2022 290a  ., n@n_dim). ").
-00011750: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00011760: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
-00011770: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
-00011780: 2020 2020 6e5f 6469 6d20 3d20 6469 7370      n_dim = disp
-00011790: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
-000117a0: 6e65 6c0a 2020 2020 2020 2020 2020 2020  nel.            
-000117b0: 6966 2064 6973 706c 6163 656d 656e 7473  if displacements
-000117c0: 2e6e 5f64 696d 203c 3d20 6e5f 6469 6d20  .n_dim <= n_dim 
-000117d0: 2b20 313a 2064 6973 706c 6163 656d 656e  + 1: displacemen
-000117e0: 7473 203d 2064 6973 706c 6163 656d 656e  ts = displacemen
-000117f0: 7473 2e75 6e73 7175 6565 7a65 285b 5d29  ts.unsqueeze([])
-00011800: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00011810: 653a 2064 6973 706c 6163 656d 656e 7473  e: displacements
-00011820: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-00011830: 203d 2030 0a20 2020 2020 2020 2064 6973   = 0.        dis
-00011840: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
-00011850: 706c 6163 656d 656e 7473 2e66 6c6f 6174  placements.float
-00011860: 2829 0a20 2020 2020 2020 2061 766f 7563  ().        avouc
-00011870: 6828 6469 7370 6c61 6365 6d65 6e74 732e  h(displacements.
-00011880: 6861 735f 6261 7463 6820 616e 6420 6469  has_batch and di
-00011890: 7370 6c61 6365 6d65 6e74 732e 6861 735f  splacements.has_
-000118a0: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
-000118b0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
-000118c0: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
-000118d0: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
-000118e0: 6174 6368 5d2c 207b 7b6e 5f64 696d 7d7d  atch], {{n_dim}}
-000118f0: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
-00011900: 206e 406e 5f64 696d 2920 666f 7220 4444   n@n_dim) for DD
-00011910: 4620 7061 7261 6d65 7465 7273 2c20 696e  F parameters, in
-00011920: 7374 6561 6420 6f66 207b 6469 7370 6c61  stead of {displa
-00011930: 6365 6d65 6e74 732e 7368 6170 657d 2e20  cements.shape}. 
-00011940: 2229 0a20 2020 2020 2020 2073 7570 6572  ").        super
-00011950: 2829 2e5f 5f69 6e69 745f 5f28 6469 7370  ().__init__(disp
-00011960: 6c61 6365 6d65 6e74 732c 2073 6861 7065  lacements, shape
-00011970: 3d73 6861 7065 2c20 696e 7465 7270 6f6c  =shape, interpol
-00011980: 6174 653d 696e 7465 7270 6f6c 6174 6529  ate=interpolate)
-00011990: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
-000119a0: 6469 6d20 3d20 6469 7370 6c61 6365 6d65  dim = displaceme
-000119b0: 6e74 732e 6e5f 6368 616e 6e65 6c0a 2020  nts.n_channel.  
-000119c0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
-000119d0: 6163 656d 656e 7473 203d 2064 6973 706c  acements = displ
-000119e0: 6163 656d 656e 7473 0a20 2020 2020 2020  acements.       
-000119f0: 2073 656c 662e 696e 7465 7270 6f6c 6174   self.interpolat
-00011a00: 6520 3d20 696e 7465 7270 6f6c 6174 650a  e = interpolate.
-00011a10: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
-00011a20: 6368 5f70 6172 616d 2e61 7070 656e 6428  ch_param.append(
-00011a30: 2764 6973 706c 6163 656d 656e 7473 2729  'displacements')
-00011a40: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
-00011a50: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
-00011a60: 0a20 2020 2020 2020 2058 203d 2073 7570  .        X = sup
-00011a70: 6572 2829 2e5f 5f63 616c 6c5f 5f28 5829  er().__call__(X)
-00011a80: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-00011a90: 656d 656e 7473 203d 2073 656c 662e 6469  ements = self.di
-00011aa0: 7370 6c61 6365 6d65 6e74 730a 2020 2020  splacements.    
-00011ab0: 2020 2020 6e5f 6469 6d20 3d20 7365 6c66      n_dim = self
-00011ac0: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
-00011ad0: 6620 582e 6e5f 7370 6163 6520 3d3d 2030  f X.n_space == 0
-00011ae0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
-00011af0: 6528 2d31 290a 2020 2020 2020 2020 6966  e(-1).        if
-00011b00: 206e 6f74 2073 656c 662e 696e 7465 7270   not self.interp
-00011b10: 6f6c 6174 6520 616e 6420 582e 7370 6163  olate and X.spac
-00011b20: 6520 3d3d 2064 6973 706c 6163 656d 656e  e == displacemen
-00011b30: 7473 2e73 7061 6365 2061 6e64 2058 2e6e  ts.space and X.n
-00011b40: 5f63 6861 6e6e 656c 203d 3d20 6469 7370  _channel == disp
-00011b50: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
-00011b60: 6e65 6c3a 2072 6574 7572 6e20 5820 2b20  nel: return X + 
-00011b70: 6469 7370 6c61 6365 6d65 6e74 730a 2020  displacements.  
-00011b80: 2020 2020 2020 656c 7365 3a20 7265 7475        else: retu
-00011b90: 726e 2058 202b 2069 6e74 6572 706f 6c61  rn X + interpola
-00011ba0: 7469 6f6e 2864 6973 706c 6163 656d 656e  tion(displacemen
-00011bb0: 7473 2c20 7461 7267 6574 5f73 7061 6365  ts, target_space
-00011bc0: 3d58 292e 6368 616e 6e65 6c5f 6469 6d65  =X).channel_dime
-00011bd0: 6e73 696f 6e5f 2831 290a 0a40 616c 6961  nsion_(1)..@alia
-00011be0: 7328 224d 4c50 2229 0a63 6c61 7373 204d  s("MLP").class M
-00011bf0: 756c 7469 4c61 7965 7250 6572 6365 7074  ultiLayerPercept
-00011c00: 696f 6e28 5370 6174 6961 6c54 7261 6e73  ion(SpatialTrans
-00011c10: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
-00011c20: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00011c30: 662c 2077 6569 6768 7473 2c20 6869 6464  f, weights, hidd
-00011c40: 656e 5f6c 6179 6572 733d 5b5d 2c20 6163  en_layers=[], ac
-00011c50: 7469 7665 5f66 756e 6374 696f 6e3d 4e6f  tive_function=No
-00011c60: 6e65 2c20 7472 616e 735f 7374 7265 7463  ne, trans_stretc
-00011c70: 683d 3129 3a0a 2020 2020 2020 2020 2727  h=1):.        ''
-00011c80: 270a 2020 2020 2020 2020 4120 7472 616e  '.        A tran
-00011c90: 7366 6f72 6d61 7469 6f6e 2064 6566 696e  sformation defin
-00011ca0: 6564 2062 7920 6120 4d4c 502e 200a 2020  ed by a MLP. .  
-00011cb0: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
-00011cc0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
-00011cd0: 2020 2077 6569 6768 7473 205b 6274 2e54     weights [bt.T
-00011ce0: 656e 736f 725d 3a20 7468 6520 7765 6967  ensor]: the weig
-00011cf0: 6874 7320 666f 7220 7468 6520 7065 7263  hts for the perc
-00011d00: 6570 7469 6f6e 206e 6574 776f 726b 2e20  eption network. 
-00011d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d20: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00011d30: 5d2c 206e 5f64 696d 202a 206e 5f68 6c5f  ], n_dim * n_hl_
-00011d40: 3120 2b20 6e5f 686c 5f31 202b 2073 756d  1 + n_hl_1 + sum
-00011d50: 2869 3d31 2e2e 6b2d 3129 7b6e 5f68 6c5f  (i=1..k-1){n_hl_
-00011d60: 6920 2a20 6e5f 686c 5f7b 692b 317d 202b  i * n_hl_{i+1} +
-00011d70: 206e 5f68 6c5f 7b69 2b31 7d7d 202b 206e   n_hl_{i+1}} + n
-00011d80: 5f68 6c5f 6b20 2a20 6e5f 6469 6d20 2b20  _hl_k * n_dim + 
-00011d90: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
-00011da0: 2020 2020 2020 2077 6865 7265 206b 2069         where k i
-00011db0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-00011dc0: 6869 6464 656e 206c 6179 6572 7320 616e  hidden layers an
-00011dd0: 6420 6e5f 686c 5f69 2069 7320 7468 6520  d n_hl_i is the 
-00011de0: 6c65 6e67 7468 206f 6620 7468 6520 692d  length of the i-
-00011df0: 7468 2068 6964 6465 6e20 6c61 7965 722e  th hidden layer.
-00011e00: 200a 2020 2020 2020 2020 2020 2020 6869   .            hi
-00011e10: 6464 656e 5f6c 6179 6572 7320 5b6c 6973  dden_layers [lis
-00011e20: 7420 6f66 2069 6e74 5d3a 2074 6865 206c  t of int]: the l
-00011e30: 656e 6774 6873 2066 6f72 2074 6865 2068  engths for the h
-00011e40: 6964 6465 6e20 6c61 7965 7273 2c20 692e  idden layers, i.
-00011e50: 652e 205b 6e5f 686c 5f31 2c20 6e5f 686c  e. [n_hl_1, n_hl
-00011e60: 5f32 2c20 2e2e 2e2c 206e 5f68 6c5f 6b5d  _2, ..., n_hl_k]
-00011e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e80: 2049 7420 6973 2062 7920 6465 6661 756c   It is by defaul
-00011e90: 7420 275b 5d27 2073 6f20 7468 6174 2074  t '[]' so that t
-00011ea0: 6865 2064 6566 6175 6c74 204d 4c50 2069  he default MLP i
-00011eb0: 7320 616e 2061 6666 696e 6520 7472 616e  s an affine tran
-00011ec0: 7366 6f72 6d61 7469 6f6e 2e20 0a20 2020  sformation. .   
-00011ed0: 2020 2020 2020 2020 2061 6374 6976 655f           active_
-00011ee0: 6675 6e63 7469 6f6e 205b 636c 6173 735d  function [class]
-00011ef0: 3a20 7468 6520 6163 7469 7665 5f66 756e  : the active_fun
-00011f00: 6374 696f 6e2e 200a 2020 2020 2020 2020  ction. .        
-00011f10: 2020 2020 7472 616e 735f 7374 7265 7463      trans_stretc
-00011f20: 6820 5b69 6e74 5d3a 2031 2062 7920 6465  h [int]: 1 by de
-00011f30: 6661 756c 742e 2032 3020 7365 656d 7320  fault. 20 seems 
-00011f40: 746f 2062 6520 6120 676f 6f64 2063 686f  to be a good cho
-00011f50: 6963 652e 200a 2020 2020 2020 2020 2020  ice. .          
-00011f60: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
-00011f70: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
-00011f80: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
-00011f90: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
-00011fa0: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
-00011fb0: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
-00011fc0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
-00011fd0: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
-00011fe0: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
-00011ff0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-00012000: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
-00012010: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
-00012020: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
-00012030: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
-00012040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012050: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-00012060: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
-00012070: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
-00012080: 6469 6d29 0a20 2020 2020 2020 2027 2727  dim).        '''
-00012090: 0a20 2020 2020 2020 2073 656c 662e 6869  .        self.hi
-000120a0: 6464 656e 5f6c 6179 6572 7320 3d20 6869  dden_layers = hi
-000120b0: 6464 656e 5f6c 6179 6572 730a 2020 2020  dden_layers.    
-000120c0: 2020 2020 6966 206e 6f74 2077 6569 6768      if not weigh
-000120d0: 7473 2e68 6173 5f62 6174 6368 3a0a 2020  ts.has_batch:.  
-000120e0: 2020 2020 2020 2020 2020 6966 2077 6569            if wei
-000120f0: 6768 7473 2e6e 5f64 696d 203d 3d20 323a  ghts.n_dim == 2:
-00012100: 2077 6569 6768 7473 2e62 6174 6368 5f64   weights.batch_d
-00012110: 696d 203d 2030 0a20 2020 2020 2020 2020  im = 0.         
-00012120: 2020 2065 6c73 653a 2077 6569 6768 7473     else: weights
-00012130: 203d 2077 6569 6768 7473 2e75 6e73 7175   = weights.unsqu
-00012140: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
-00012150: 2073 656c 662e 7765 6967 6874 7320 3d20   self.weights = 
-00012160: 7765 6967 6874 730a 2020 2020 2020 2020  weights.        
-00012170: 7365 6c66 2e74 7261 6e73 5f73 7472 6574  self.trans_stret
-00012180: 6368 203d 2074 7261 6e73 5f73 7472 6574  ch = trans_stret
-00012190: 6368 0a20 2020 2020 2020 2073 7570 6572  ch.        super
-000121a0: 2829 2e5f 5f69 6e69 745f 5f28 7765 6967  ().__init__(weig
-000121b0: 6874 732c 2068 6964 6465 6e5f 6c61 7965  hts, hidden_laye
-000121c0: 7273 203d 2068 6964 6465 6e5f 6c61 7965  rs = hidden_laye
-000121d0: 7273 2c20 7472 616e 735f 7374 7265 7463  rs, trans_stretc
-000121e0: 6820 3d20 7472 616e 735f 7374 7265 7463  h = trans_stretc
-000121f0: 6829 0a20 2020 2020 2020 2064 696d 5f63  h).        dim_c
-00012200: 6f6e 7374 203d 2077 6569 6768 7473 2e73  onst = weights.s
-00012210: 697a 6528 2d31 2920 2d20 7375 6d28 6869  ize(-1) - sum(hi
-00012220: 6464 656e 5f6c 6179 6572 7329 202d 2073  dden_layers) - s
-00012230: 756d 2878 202a 2079 2066 6f72 2078 2c20  um(x * y for x, 
-00012240: 7920 696e 207a 6970 2868 6964 6465 6e5f  y in zip(hidden_
-00012250: 6c61 7965 7273 5b3a 2d31 5d2c 2068 6964  layers[:-1], hid
-00012260: 6465 6e5f 6c61 7965 7273 5b31 3a5d 2929  den_layers[1:]))
-00012270: 0a20 2020 2020 2020 2064 696d 5f63 6f65  .        dim_coe
-00012280: 6666 203d 2068 6964 6465 6e5f 6c61 7965  ff = hidden_laye
-00012290: 7273 5b30 5d20 2b20 6869 6464 656e 5f6c  rs[0] + hidden_l
-000122a0: 6179 6572 735b 2d31 5d20 2b20 310a 2020  ayers[-1] + 1.  
-000122b0: 2020 2020 2020 6176 6f75 6368 2864 696d        avouch(dim
-000122c0: 5f63 6f6e 7374 2025 2064 696d 5f63 6f65  _const % dim_coe
-000122d0: 6666 203d 3d20 302c 2066 2257 726f 6e67  ff == 0, f"Wrong
-000122e0: 2077 6569 6768 7420 6c65 6e67 7468 2066   weight length f
-000122f0: 6f72 2068 6964 6465 6e20 6c61 7965 7273  or hidden layers
-00012300: 206f 6620 7369 7a65 7320 7b68 6964 6465   of sizes {hidde
-00012310: 6e5f 6c61 7965 7273 7d2c 207b 6469 6d5f  n_layers}, {dim_
-00012320: 636f 6566 667d 2078 206e 5f64 696d 202b  coeff} x n_dim +
-00012330: 207b 6469 6d5f 636f 6e73 747d 2065 7870   {dim_const} exp
-00012340: 6563 7465 642c 2062 7574 2067 6f74 207b  ected, but got {
-00012350: 7765 6967 6874 732e 7369 7a65 282d 3129  weights.size(-1)
-00012360: 7d2e 2229 0a20 2020 2020 2020 2073 656c  }.").        sel
-00012370: 662e 6e5f 6469 6d20 3d20 6469 6d5f 636f  f.n_dim = dim_co
-00012380: 6e73 7420 2f2f 2064 696d 5f63 6f65 6666  nst // dim_coeff
-00012390: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
-000123a0: 6261 7463 6820 3d20 7765 6967 6874 732e  batch = weights.
-000123b0: 6e5f 6261 7463 680a 2020 2020 2020 2020  n_batch.        
-000123c0: 7365 6c66 2e6c 6179 6572 7320 3d20 5b5d  self.layers = []
-000123d0: 0a20 2020 2020 2020 2070 203d 2030 0a20  .        p = 0. 
-000123e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000123f0: 7261 6e67 6528 6c65 6e28 6869 6464 656e  range(len(hidden
-00012400: 5f6c 6179 6572 7329 202b 2031 293a 0a20  _layers) + 1):. 
-00012410: 2020 2020 2020 2020 2020 2069 6e5f 6665             in_fe
-00012420: 6174 7572 6573 203d 2073 656c 662e 6e5f  atures = self.n_
-00012430: 6469 6d20 6966 2069 203d 3d20 3020 656c  dim if i == 0 el
-00012440: 7365 2068 6964 6465 6e5f 6c61 7965 7273  se hidden_layers
-00012450: 5b69 202d 2031 5d0a 2020 2020 2020 2020  [i - 1].        
-00012460: 2020 2020 6f75 745f 6665 6174 7572 6573      out_features
-00012470: 203d 2073 656c 662e 6e5f 6469 6d20 6966   = self.n_dim if
-00012480: 2069 203d 3d20 6c65 6e28 6869 6464 656e   i == len(hidden
-00012490: 5f6c 6179 6572 7329 2065 6c73 6520 6869  _layers) else hi
-000124a0: 6464 656e 5f6c 6179 6572 735b 695d 0a20  dden_layers[i]. 
-000124b0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-000124c0: 5f77 6569 6768 7473 203d 2077 6569 6768  _weights = weigh
-000124d0: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
-000124e0: 6665 6174 7572 6573 2a69 6e5f 6665 6174  features*in_feat
-000124f0: 7572 6573 5d2e 7669 6577 285b 7365 6c66  ures].view([self
-00012500: 2e6e 5f62 6174 6368 5d2c 206f 7574 5f66  .n_batch], out_f
-00012510: 6561 7475 7265 732c 2069 6e5f 6665 6174  eatures, in_feat
-00012520: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
-00012530: 2020 7020 2b3d 206f 7574 5f66 6561 7475    p += out_featu
-00012540: 7265 7320 2a20 696e 5f66 6561 7475 7265  res * in_feature
-00012550: 730a 2020 2020 2020 2020 2020 2020 6c61  s.            la
-00012560: 7965 725f 6269 6173 203d 2077 6569 6768  yer_bias = weigh
-00012570: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
-00012580: 6665 6174 7572 6573 5d2e 7669 6577 285b  features].view([
-00012590: 7365 6c66 2e6e 5f62 6174 6368 5d2c 206f  self.n_batch], o
-000125a0: 7574 5f66 6561 7475 7265 7329 0a20 2020  ut_features).   
-000125b0: 2020 2020 2020 2020 2070 202b 3d20 6f75           p += ou
-000125c0: 745f 6665 6174 7572 6573 0a20 2020 2020  t_features.     
-000125d0: 2020 2020 2020 2073 656c 662e 6c61 7965         self.laye
-000125e0: 7273 2e61 7070 656e 6428 286c 6179 6572  rs.append((layer
-000125f0: 5f77 6569 6768 7473 2c20 6c61 7965 725f  _weights, layer_
-00012600: 6269 6173 2929 0a20 2020 2020 2020 2073  bias)).        s
-00012610: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
-00012620: 696f 6e20 3d20 6163 7469 7665 5f66 756e  ion = active_fun
-00012630: 6374 696f 6e0a 2020 2020 2020 2020 6966  ction.        if
-00012640: 2073 656c 662e 6163 7469 7665 5f66 756e   self.active_fun
-00012650: 6374 696f 6e20 6973 204e 6f6e 653a 2073  ction is None: s
-00012660: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
-00012670: 696f 6e20 3d20 6274 2e6e 6e2e 5265 4c55  ion = bt.nn.ReLU
-00012680: 0a20 2020 200a 2020 2020 4070 726f 7065  .    .    @prope
-00012690: 7274 790a 2020 2020 6465 6620 6e5f 7765  rty.    def n_we
-000126a0: 6967 6874 5f6c 656e 6774 6828 7365 6c66  ight_length(self
-000126b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-000126c0: 6e20 7365 6c66 2e6e 5f64 696d 202a 2028  n self.n_dim * (
-000126d0: 7365 6c66 2e68 6964 6465 6e5f 6c61 7965  self.hidden_laye
-000126e0: 7273 5b30 5d20 2b20 7365 6c66 2e68 6964  rs[0] + self.hid
-000126f0: 6465 6e5f 6c61 7965 7273 5b2d 315d 202b  den_layers[-1] +
-00012700: 2031 2920 2b20 7375 6d28 7365 6c66 2e68   1) + sum(self.h
-00012710: 6964 6465 6e5f 6c61 7965 7273 2920 2b20  idden_layers) + 
-00012720: 7375 6d28 7820 2a20 7920 666f 7220 782c  sum(x * y for x,
-00012730: 2079 2069 6e20 7a69 7028 7365 6c66 2e68   y in zip(self.h
-00012740: 6964 6465 6e5f 6c61 7965 7273 5b3a 2d31  idden_layers[:-1
-00012750: 5d2c 2073 656c 662e 6869 6464 656e 5f6c  ], self.hidden_l
-00012760: 6179 6572 735b 313a 5d29 290a 2020 2020  ayers[1:])).    
-00012770: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
-00012780: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
-00012790: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
-000127a0: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
-000127b0: 2020 2020 6966 2058 2e6e 5f73 7061 6365      if X.n_space
-000127c0: 203d 3d20 303a 2058 203d 2058 2e75 6e73   == 0: X = X.uns
-000127d0: 7175 6565 7a65 282d 3129 0a20 2020 2020  queeze(-1).     
-000127e0: 2020 2059 203d 2058 2e66 6c61 7474 656e     Y = X.flatten
-000127f0: 2829 2e63 6861 6e6e 656c 5f64 696d 5f28  ().channel_dim_(
-00012800: 4e6f 6e65 290a 2020 2020 2020 2020 666f  None).        fo
-00012810: 7220 692c 2028 7765 6967 6874 732c 2062  r i, (weights, b
-00012820: 6961 7329 2069 6e20 656e 756d 6572 6174  ias) in enumerat
-00012830: 6528 7365 6c66 2e6c 6179 6572 7329 3a0a  e(self.layers):.
-00012840: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
-00012850: 7765 6967 6874 7320 4020 590a 2020 2020  weights @ Y.    
-00012860: 2020 2020 2020 2020 6966 2069 203c 206c          if i < l
-00012870: 656e 2873 656c 662e 6c61 7965 7273 2920  en(self.layers) 
-00012880: 2d20 313a 2059 203d 2073 656c 662e 6163  - 1: Y = self.ac
-00012890: 7469 7665 5f66 756e 6374 696f 6e28 2928  tive_function()(
-000128a0: 5920 2b20 6269 6173 2e75 6e73 7175 6565  Y + bias.unsquee
-000128b0: 7a65 282d 3129 290a 2020 2020 2020 2020  ze(-1)).        
-000128c0: 2020 2020 656c 7365 3a20 5920 2b3d 2073      else: Y += s
-000128d0: 656c 662e 7472 616e 735f 7374 7265 7463  elf.trans_stretc
-000128e0: 6820 2a20 6269 6173 2e75 6e73 7175 6565  h * bias.unsquee
-000128f0: 7a65 282d 3129 0a20 2020 2020 2020 2072  ze(-1).        r
-00012900: 6574 7572 6e20 5820 2b20 592e 7669 6577  eturn X + Y.view
-00012910: 5f61 7328 5829 2e63 6861 6e6e 656c 5f64  _as(X).channel_d
-00012920: 696d 656e 7369 6f6e 5f28 3129 0a0a 4061  imension_(1)..@a
-00012930: 6c69 6173 2822 7265 7361 6d70 6c65 2229  lias("resample")
-00012940: 0a64 6566 2069 6e74 6572 706f 6c61 7469  .def interpolati
-00012950: 6f6e 280a 2020 2020 2020 2020 696d 6167  on(.        imag
-00012960: 653a 2062 742e 5465 6e73 6f72 2c20 0a20  e: bt.Tensor, . 
-00012970: 2020 2020 2020 2074 7261 6e73 3a20 4361         trans: Ca
-00012980: 6c6c 6162 6c65 203d 204e 6f6e 652c 200a  llable = None, .
-00012990: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
-000129a0: 7374 7220 3d20 274c 696e 6561 7227 2c20  str = 'Linear', 
-000129b0: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
-000129c0: 7370 6163 653a 2074 7570 6c65 203d 204e  space: tuple = N
-000129d0: 6f6e 652c 0a20 2020 2020 2020 2066 696c  one,.        fil
-000129e0: 6c3a 2028 7374 722c 2069 6e74 2c20 666c  l: (str, int, fl
-000129f0: 6f61 7429 203d 2030 2c0a 2020 2020 2020  oat) = 0,.      
-00012a00: 2020 6465 7269 7661 7469 7665 3a20 626f    derivative: bo
-00012a10: 6f6c 203d 2046 616c 7365 0a20 2020 2029  ol = False.    )
-00012a20: 3a0a 2020 2020 2727 270a 2020 2020 496e  :.    '''.    In
-00012a30: 7465 7270 6f6c 6174 6520 7573 696e 6720  terpolate using 
-00012a40: 6261 636b 7761 7264 2074 7261 6e73 666f  backward transfo
-00012a50: 726d 6174 696f 6e2e 0a20 2020 2069 2e65  rmation..    i.e
-00012a60: 2e20 436f 6d70 7574 6520 7468 6520 696d  . Compute the im
-00012a70: 6167 6520 4920 732e 742e 2074 7261 6e73  age I s.t. trans
-00012a80: 2878 2920 3d20 7920 666f 7220 7820 696e  (x) = y for x in
-00012a90: 2049 2061 6e64 2079 2069 6e20 696e 7075   I and y in inpu
-00012aa0: 7420 696d 6167 6520 7573 696e 6720 696e  t image using in
-00012ab0: 7465 7270 6f6c 6174 696f 6e20 6d65 7468  terpolation meth
-00012ac0: 6f64 3a0a 2020 2020 2020 2020 6d65 7468  od:.        meth
-00012ad0: 6f64 203d 204c 696e 6561 723a 2042 696c  od = Linear: Bil
-00012ae0: 696e 6561 7220 696e 7465 7270 6f6c 6174  inear interpolat
-00012af0: 696f 6e0a 2020 2020 2020 2020 6d65 7468  ion.        meth
-00012b00: 6f64 203d 204e 6561 7265 7374 205b 4e4f  od = Nearest [NO
-00012b10: 2047 5241 4449 454e 5421 2121 5d3a 204e   GRADIENT!!!]: N
-00012b20: 6561 7265 7374 2069 6e74 6572 706f 6c61  earest interpola
-00012b30: 7469 6f6e 0a0a 2020 2020 5061 7261 6d73  tion..    Params
-00012b40: 3a0a 2020 2020 2020 2020 696d 6167 6520  :.        image 
-00012b50: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
-00012b60: 2074 6172 6765 7420 696d 6167 652e 0a20   target image.. 
-00012b70: 2020 2020 2020 2020 2020 2073 697a 653a             size:
-00012b80: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
-00012b90: 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e 656c  nal], {n_channel
-00012ba0: 3a6f 7074 696f 6e61 6c7d 2c20 6d40 312c  :optional}, m@1,
-00012bb0: 206d 4032 2c20 2e2e 2e2c 206d 406e 5f64   m@2, ..., m@n_d
-00012bc0: 696d 290a 2020 2020 2020 2020 7472 616e  im).        tran
-00012bd0: 7320 5b46 756e 6374 696f 6e20 6f72 206d  s [Function or m
-00012be0: 6963 6f6d 7075 7469 6e67 2e53 7061 7469  icomputing.Spati
-00012bf0: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
-00012c00: 5d3a 2054 7261 6e73 666f 726d 6174 696f  ]: Transformatio
-00012c10: 6e20 6675 6e63 7469 6f6e 2c20 6d61 7070  n function, mapp
-00012c20: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00012c30: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
-00012c40: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
-00012c50: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-00012c60: 2e2c 206e 406e 5f64 696d 2920 746f 2028  ., n@n_dim) to (
-00012c70: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00012c80: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
-00012c90: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
-00012ca0: 2020 2020 6d65 7468 6f64 205b 7374 723a      method [str:
-00012cb0: 206c 696e 6561 727c 6e65 6172 6573 745d   linear|nearest]
-00012cc0: 3a20 5468 6520 696e 7465 7270 6f6c 6174  : The interpolat
-00012cd0: 696f 6e20 6d65 7468 6f64 2e20 0a20 2020  ion method. .   
-00012ce0: 2020 2020 2074 6172 6765 745f 7370 6163       target_spac
-00012cf0: 6520 5b74 7570 6c65 206f 7220 6274 2e54  e [tuple or bt.T
-00012d00: 656e 736f 725d 3a0a 2020 2020 2020 2020  ensor]:.        
-00012d10: 2020 2020 5369 7a65 2028 7475 706c 6529      Size (tuple)
-00012d20: 206f 6620 6120 7461 7267 6574 2052 4f49   of a target ROI
-00012d30: 2061 7420 7468 6520 6365 6e74 6572 206f   at the center o
-00012d40: 6620 696d 6167 652e 200a 2020 2020 2020  f image. .      
-00012d50: 2020 2020 2020 4f52 2054 7261 6e73 666f        OR Transfo
-00012d60: 726d 6564 2063 6f6f 7264 696e 6174 6520  rmed coordinate 
-00012d70: 7370 6163 6520 2862 742e 5465 6e73 6f72  space (bt.Tensor
-00012d80: 2920 6f66 2074 6865 206f 7574 7075 7420  ) of the output 
-00012d90: 696d 6167 652e 200a 2020 2020 2020 2020  image. .        
-00012da0: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
-00012db0: 286e 5f64 696d 2920 6f72 2028 5b6e 5f62  (n_dim) or ([n_b
-00012dc0: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-00012dd0: 7b6e 5f64 696d 3a6f 7074 696f 6e61 6c7d  {n_dim:optional}
-00012de0: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
-00012df0: 2c20 2e2e 2e2c 2073 697a 6540 7229 0a20  , ..., size@r). 
-00012e00: 2020 2020 2020 2066 696c 6c20 5b73 7472         fill [str
-00012e10: 3a20 6e65 6172 6573 747c 6261 636b 6772  : nearest|backgr
-00012e20: 6f75 6e64 206f 7220 696e 7420 6f72 2066  ound or int or f
-00012e30: 6c6f 6174 286e 756d 6265 7229 5d3a 2049  loat(number)]: I
-00012e40: 6e64 6963 6174 6520 7468 6520 7761 7920  ndicate the way 
-00012e50: 746f 2066 696c 6c20 6261 636b 6772 6f75  to fill backgrou
-00012e60: 6e64 206f 7574 7369 6465 2060 5375 7272  nd outside `Surr
-00012e70: 6f75 6e64 696e 6760 2e20 0a20 2020 2020  ounding`. .     
-00012e80: 2020 2064 6572 6976 6174 6976 6520 5b62     derivative [b
-00012e90: 6f6f 6c5d 3a20 5768 6574 6865 7220 746f  ool]: Whether to
-00012ea0: 2072 6574 7572 6e20 7468 6520 6772 6164   return the grad
-00012eb0: 6965 6e74 2e20 4f6e 6520 6361 6e20 6f6d  ient. One can om
-00012ec0: 6974 2069 7420 7768 656e 2075 7369 6e67  it it when using
-00012ed0: 2074 6f72 6368 2e61 7574 6f67 7261 642e   torch.autograd.
-00012ee0: 0a0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
-00012ef0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
-00012f00: 6520 7472 616e 7366 6f72 6d65 6420 696d  e transformed im
-00012f10: 6167 652e 0a20 2020 2020 2020 2020 2020  age..           
-00012f20: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
-00012f30: 5d2c 207b 6e5f 6368 616e 6e65 6c3a 6f70  ], {n_channel:op
-00012f40: 7469 6f6e 616c 7d2c 206d 4031 2c20 6d40  tional}, m@1, m@
-00012f50: 322c 202e 2e2e 2c20 6d40 6e5f 6469 6d29  2, ..., m@n_dim)
-00012f60: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
-00012f70: 7768 656e 2060 7461 7267 6574 5f73 7061  when `target_spa
-00012f80: 6365 6020 6973 2064 6566 696e 6564 2062  ce` is defined b
-00012f90: 7920 7465 6e73 6f72 2e20 0a20 2020 2020  y tensor. .     
-00012fa0: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
-00012fb0: 5f62 6174 6368 5d2c 2073 697a 6540 312c  _batch], size@1,
-00012fc0: 2073 697a 6540 322c 202e 2e2e 2c20 7369   size@2, ..., si
-00012fd0: 7a65 406e 5f64 696d 290a 2020 2020 2020  ze@n_dim).      
-00012fe0: 2020 2020 2020 6f72 2074 6865 2064 6572        or the der
-00012ff0: 6976 6174 6976 6520 666f 7220 7468 6520  ivative for the 
-00013000: 696e 7465 7270 6f6c 6174 696f 6e2e 2028  interpolation. (
-00013010: 6966 2060 6465 7269 7661 7469 7665 203d  if `derivative =
-00013020: 2054 7275 6560 290a 2020 2020 2020 2020   True`).        
-00013030: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
-00013040: 7463 685d 2c20 7b6e 5f64 696d 7d2c 2073  tch], {n_dim}, s
-00013050: 697a 6540 312c 2073 697a 6540 322c 202e  ize@1, size@2, .
-00013060: 2e2e 2c20 7369 7a65 406e 5f64 696d 290a  .., size@n_dim).
-00013070: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-00013080: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00013090: 2020 3e3e 3e20 496d 6167 6520 3d20 6274    >>> Image = bt
-000130a0: 2e72 616e 6428 332c 2031 3030 2c20 3132  .rand(3, 100, 12
-000130b0: 302c 2038 3029 0a20 2020 203e 3e3e 2041  0, 80).    >>> A
-000130c0: 4d20 3d20 6274 2e72 616e 6428 342c 2034  M = bt.rand(4, 4
-000130d0: 290a 2020 2020 3e3e 3e20 414d 5b33 2c20  ).    >>> AM[3, 
-000130e0: 3a5d 203d 2062 742e 6f6e 655f 686f 7428  :] = bt.one_hot(
-000130f0: 2d31 2c20 3429 0a20 2020 203e 3e3e 2069  -1, 4).    >>> i
-00013100: 6e74 6572 706f 6c61 7469 6f6e 2849 6d61  nterpolation(Ima
-00013110: 6765 2c20 4166 6669 6e65 2841 4d29 2c20  ge, Affine(AM), 
-00013120: 6d65 7468 6f64 3d27 4c69 6e65 6172 2729  method='Linear')
-00013130: 0a20 2020 2027 2727 0a20 2020 2069 6620  .    '''.    if 
-00013140: 7472 616e 7320 6973 206e 6f74 204e 6f6e  trans is not Non
-00013150: 6520 616e 6420 6e6f 7420 7472 616e 732e  e and not trans.
-00013160: 6261 636b 7761 7264 3a0a 2020 2020 2020  backward:.      
-00013170: 2020 6966 2068 6173 6174 7472 2874 7261    if hasattr(tra
-00013180: 6e73 2c20 2769 6e76 2729 3a20 7472 616e  ns, 'inv'): tran
-00013190: 7320 3d20 7472 616e 732e 696e 7628 292e  s = trans.inv().
-000131a0: 6661 6b65 5f69 6e76 2829 0a20 2020 2020  fake_inv().     
-000131b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000131c0: 2020 2020 2070 7269 6e74 2822 5761 726e       print("Warn
-000131d0: 696e 673a 2046 6f72 7761 7264 2074 7261  ing: Forward tra
-000131e0: 6e73 666f 726d 6174 696f 6e20 666f 756e  nsformation foun
-000131f0: 6420 696e 206d 6574 686f 6420 6069 6e74  d in method `int
-00013200: 6572 706f 6c61 7469 6f6e 602e 2055 7369  erpolation`. Usi
-00013210: 6e67 2060 696e 7465 7270 6f6c 6174 696f  ng `interpolatio
-00013220: 6e5f 666f 7277 6172 6460 2069 6e73 7465  n_forward` inste
-00013230: 6164 2e20 2229 0a20 2020 2020 2020 2020  ad. ").         
-00013240: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
-00013250: 6f6c 6174 696f 6e5f 666f 7277 6172 6428  olation_forward(
-00013260: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
-00013270: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
-00013280: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
-00013290: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
-000132a0: 203d 2066 696c 6c29 0a20 2020 2069 6d61   = fill).    ima
-000132b0: 6765 203d 2062 742e 746f 5f64 6576 6963  ge = bt.to_devic
-000132c0: 6528 6261 746f 7263 685f 7465 6e73 6f72  e(batorch_tensor
-000132d0: 2869 6d61 6765 2929 0a20 2020 2073 6861  (image)).    sha
-000132e0: 7065 5f6f 7574 203d 2069 6d61 6765 2e73  pe_out = image.s
-000132f0: 6861 7065 0a20 2020 2069 6620 7472 616e  hape.    if tran
-00013300: 7320 6973 204e 6f6e 6520 6f72 2074 7261  s is None or tra
-00013310: 6e73 2e6e 5f64 696d 2069 7320 4e6f 6e65  ns.n_dim is None
-00013320: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00013330: 2069 6d61 6765 2e68 6173 5f62 6174 6368   image.has_batch
-00013340: 3a20 696d 6167 652e 756e 7371 7565 657a  : image.unsqueez
-00013350: 655f 285b 5d29 0a20 2020 2020 2020 2069  e_([]).        i
-00013360: 6620 6e6f 7420 696d 6167 652e 6861 735f  f not image.has_
-00013370: 6368 616e 6e65 6c3a 2069 6d61 6765 2e73  channel: image.s
-00013380: 7461 6e64 6172 645f 2829 2e75 6e73 7175  tandard_().unsqu
-00013390: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
-000133a0: 2020 206e 5f64 696d 203d 2069 6d61 6765     n_dim = image
-000133b0: 2e6e 5f73 7061 6365 2023 2047 6574 2074  .n_space # Get t
-000133c0: 6865 2073 7061 7469 616c 2072 616e 6b2e  he spatial rank.
-000133d0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000133e0: 2020 206e 5f64 696d 203d 2074 7261 6e73     n_dim = trans
-000133f0: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
-00013400: 6620 696d 6167 652e 6e5f 6469 6d20 3d3d  f image.n_dim ==
-00013410: 206e 5f64 696d 3a0a 2020 2020 2020 2020   n_dim:.        
-00013420: 2020 2020 6966 2069 6d61 6765 2e68 6173      if image.has
-00013430: 5f73 7065 6369 616c 3a0a 2020 2020 2020  _special:.      
-00013440: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00013450: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
-00013460: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
-00013470: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
-00013480: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
-00013490: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
-000134a0: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
-000134b0: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
-000134c0: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
-000134d0: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
-000134e0: 2d72 656d 6f76 696e 6720 7370 6563 6961  -removing specia
-000134f0: 6c20 6469 6d65 6e73 696f 6e73 2e22 290a  l dimensions.").
-00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013510: 696d 6167 652e 7265 6d6f 7665 5f73 7065  image.remove_spe
-00013520: 6369 616c 5f28 290a 2020 2020 2020 2020  cial_().        
-00013530: 2020 2020 696d 6167 652e 756e 7371 7565      image.unsque
-00013540: 657a 655f 285b 5d29 2e75 6e73 7175 6565  eze_([]).unsquee
-00013550: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
-00013560: 656c 6966 2069 6d61 6765 2e6e 5f64 696d  elif image.n_dim
-00013570: 203d 3d20 6e5f 6469 6d20 2b20 313a 0a20   == n_dim + 1:. 
-00013580: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00013590: 7420 696d 6167 652e 6861 735f 6261 7463  t image.has_batc
-000135a0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-000135b0: 2020 2069 6620 696d 6167 652e 6861 735f     if image.has_
-000135c0: 6368 616e 6e65 6c3a 2069 6d61 6765 2e75  channel: image.u
-000135d0: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
-000135e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000135f0: 7365 3a20 696d 6167 652e 7769 7468 5f62  se: image.with_b
-00013600: 6174 6368 6469 6d28 3029 2e75 6e73 7175  atchdim(0).unsqu
-00013610: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
-00013620: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-00013630: 696d 6167 652e 6861 735f 6368 616e 6e65  image.has_channe
-00013640: 6c3a 2069 6d61 6765 2e75 6e73 7175 6565  l: image.unsquee
-00013650: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
-00013660: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013670: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00013680: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
-00013690: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
-000136a0: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
-000136b0: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
-000136c0: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
-000136d0: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
-000136e0: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
-000136f0: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
-00013700: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
-00013710: 2d72 656d 6f76 696e 6720 7468 6520 6368  -removing the ch
-00013720: 616e 6e65 6c20 6469 6d65 6e73 696f 6e73  annel dimensions
-00013730: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00013740: 2020 2020 696d 6167 652e 7769 7468 5f63      image.with_c
-00013750: 6861 6e6e 656c 6469 6d28 4e6f 6e65 292e  hanneldim(None).
-00013760: 756e 7371 7565 657a 655f 287b 7d29 0a20  unsqueeze_({}). 
-00013770: 2020 2020 2020 2065 6c69 6620 696d 6167         elif imag
-00013780: 652e 6e5f 6469 6d20 3d3d 206e 5f64 696d  e.n_dim == n_dim
-00013790: 202b 2032 3a0a 2020 2020 2020 2020 2020   + 2:.          
-000137a0: 2020 2320 5f63 6861 6e6e 616c 2f62 6174    # _channal/bat
-000137b0: 6368 2064 696d 656e 7369 6f6e 7320 7573  ch dimensions us
-000137c0: 6564 2068 6572 6520 6173 2074 6865 7920  ed here as they 
-000137d0: 6172 6520 6e5f 6469 6d20 7768 656e 206e  are n_dim when n
-000137e0: 6f74 2065 7869 7374 6564 2e20 0a20 2020  ot existed. .   
-000137f0: 2020 2020 2020 2020 2069 6620 696d 6167           if imag
-00013800: 652e 6e5f 7370 6563 6961 6c20 3d3d 2031  e.n_special == 1
-00013810: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013820: 2020 7072 696e 7428 6622 5761 726e 696e    print(f"Warnin
-00013830: 673a 2027 696e 7465 7270 6f6c 6174 696f  g: 'interpolatio
-00013840: 6e27 2074 7279 696e 6720 746f 2074 7261  n' trying to tra
-00013850: 6e73 666f 726d 207b 696d 6167 652e 6e5f  nsform {image.n_
-00013860: 7370 6163 657d 2b31 4420 696d 6167 6520  space}+1D image 
-00013870: 2877 6974 6820 6261 7463 6820 6f72 2063  (with batch or c
-00013880: 6861 6e6e 656c 2920 6279 207b 6e5f 6469  hannel) by {n_di
-00013890: 6d7d 4420 7472 616e 7366 6f72 6d61 7469  m}D transformati
-000138a0: 6f6e 2c20 6175 746f 2d69 6e73 6572 7469  on, auto-inserti
-000138b0: 6e67 206e 6577 2073 7065 6369 616c 2064  ng new special d
-000138c0: 696d 656e 7369 6f6e 2e22 290a 2020 2020  imension.").    
-000138d0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-000138e0: 6d61 6765 2e68 6173 5f62 6174 6368 3a20  mage.has_batch: 
-000138f0: 696d 6167 652e 6261 7463 685f 6469 6d65  image.batch_dime
-00013900: 6e73 696f 6e20 3d20 3020 6966 2069 6d61  nsion = 0 if ima
-00013910: 6765 2e5f 6368 616e 6e65 6c5f 6469 6d65  ge._channel_dime
-00013920: 6e73 696f 6e20 3e20 3020 656c 7365 2031  nsion > 0 else 1
-00013930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013940: 6e6f 7420 696d 6167 652e 6861 735f 6368  not image.has_ch
-00013950: 616e 6e65 6c3a 2069 6d61 6765 2e63 6861  annel: image.cha
-00013960: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
-00013970: 2030 2069 6620 696d 6167 652e 5f62 6174   0 if image._bat
-00013980: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
-00013990: 2065 6c73 6520 310a 2020 2020 6176 6f75   else 1.    avou
-000139a0: 6368 2869 6d61 6765 2e68 6173 5f62 6174  ch(image.has_bat
-000139b0: 6368 2061 6e64 2069 6d61 6765 2e68 6173  ch and image.has
-000139c0: 5f63 6861 6e6e 656c 2c20 2250 6c65 6173  _channel, "Pleas
-000139d0: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
-000139e0: 6e73 6f72 206f 6620 7369 7a65 2022 202b  nsor of size " +
-000139f0: 0a20 2020 2020 2020 2020 2020 2022 285b  .            "([
-00013a00: 6e5f 6261 7463 685d 2c20 7b6e 5f63 6861  n_batch], {n_cha
-00013a10: 6e6e 656c 2f6e 5f66 6561 7475 7265 3a6f  nnel/n_feature:o
-00013a20: 7074 696f 6e61 6c7d 2c20 6d5f 312c 206d  ptional}, m_1, m
-00013a30: 5f32 2c20 2e2e 2e2c 206d 5f72 2920 5b72  _2, ..., m_r) [r
-00013a40: 3d6e 5f64 696d 5d20 666f 7220 2220 2b20  =n_dim] for " + 
-00013a50: 0a20 2020 2020 2020 2020 2020 2066 2264  .            f"d
-00013a60: 6174 6120 746f 2062 6520 7370 6174 6961  ata to be spatia
-00013a70: 6c6c 7920 696e 7465 7270 6f6c 6174 6564  lly interpolated
-00013a80: 2c20 696e 7374 6561 6420 6f66 207b 696d  , instead of {im
-00013a90: 6167 652e 7368 6170 657d 2e20 2229 0a20  age.shape}. "). 
-00013aa0: 2020 2069 6620 7472 616e 7320 6973 206e     if trans is n
-00013ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013ac0: 2061 766f 7563 6828 696d 6167 652e 6e5f   avouch(image.n_
-00013ad0: 6261 7463 6820 3d3d 2031 206f 7220 7472  batch == 1 or tr
-00013ae0: 616e 732e 6e5f 6261 7463 6820 696e 2028  ans.n_batch in (
-00013af0: 4e6f 6e65 2c20 696d 6167 652e 6e5f 6261  None, image.n_ba
-00013b00: 7463 682c 2031 292c 2022 506c 6561 7365  tch, 1), "Please
-00013b10: 2075 7365 2074 7261 6e73 666f 726d 6174   use transformat
-00013b20: 696f 6e20 6f66 2061 2022 202b 0a20 2020  ion of a " +.   
-00013b30: 2020 2020 2020 2020 2066 2273 7569 7461           f"suita
-00013b40: 626c 6520 6e5f 6261 7463 6820 746f 2074  ble n_batch to t
-00013b50: 7261 6e73 666f 726d 2069 6d61 6765 2077  ransform image w
-00013b60: 6974 6820 6261 7463 6873 697a 6520 7b69  ith batchsize {i
-00013b70: 6d61 6765 2e6e 5f62 6174 6368 7d2c 2063  mage.n_batch}, c
-00013b80: 7572 7265 6e74 6c79 207b 7472 616e 732e  urrently {trans.
-00013b90: 6e5f 6261 7463 687d 2e22 290a 0a20 2020  n_batch}.")..   
-00013ba0: 206e 5f62 6174 6368 203d 2069 6d61 6765   n_batch = image
-00013bb0: 2e6e 5f62 6174 6368 0a20 2020 2069 6620  .n_batch.    if 
-00013bc0: 6e5f 6261 7463 6820 3d3d 2031 2061 6e64  n_batch == 1 and
-00013bd0: 2074 7261 6e73 2069 7320 6e6f 7420 4e6f   trans is not No
-00013be0: 6e65 2061 6e64 2074 7261 6e73 2e6e 5f62  ne and trans.n_b
-00013bf0: 6174 6368 2069 7320 6e6f 7420 4e6f 6e65  atch is not None
-00013c00: 2061 6e64 2074 7261 6e73 2e6e 5f62 6174   and trans.n_bat
-00013c10: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
-00013c20: 3d20 7472 616e 732e 6e5f 6261 7463 680a  = trans.n_batch.
-00013c30: 2020 2020 6966 206e 5f62 6174 6368 203d      if n_batch =
-00013c40: 3d20 3120 616e 6420 6973 696e 7374 616e  = 1 and isinstan
-00013c50: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
-00013c60: 2062 742e 5465 6e73 6f72 2920 616e 6420   bt.Tensor) and 
-00013c70: 7461 7267 6574 5f73 7061 6365 2e68 6173  target_space.has
-00013c80: 5f62 6174 6368 2061 6e64 2074 6172 6765  _batch and targe
-00013c90: 745f 7370 6163 652e 6e5f 6261 7463 6820  t_space.n_batch 
-00013ca0: 3e20 313a 206e 5f62 6174 6368 203d 2074  > 1: n_batch = t
-00013cb0: 6172 6765 745f 7370 6163 652e 6e5f 6261  arget_space.n_ba
-00013cc0: 7463 680a 2020 2020 6966 2069 6d61 6765  tch.    if image
-00013cd0: 2e6e 5f62 6174 6368 203d 3d20 313a 2069  .n_batch == 1: i
-00013ce0: 6d61 6765 203d 2069 6d61 6765 2e72 6570  mage = image.rep
-00013cf0: 6561 7465 6428 6e5f 6261 7463 682c 205b  eated(n_batch, [
-00013d00: 5d29 0a20 2020 206e 5f66 6561 7475 7265  ]).    n_feature
-00013d10: 203d 2069 6d61 6765 2e6e 5f63 6861 6e6e   = image.n_chann
-00013d20: 656c 0a20 2020 2073 697a 6520 3d20 6274  el.    size = bt
-00013d30: 2e63 6861 6e6e 656c 5f74 656e 736f 7228  .channel_tensor(
-00013d40: 696d 6167 652e 7370 6163 6529 2e69 6e74  image.space).int
-00013d50: 2829 0a20 2020 2069 6620 6e5f 6261 7463  ().    if n_batc
-00013d60: 6820 3e20 3120 616e 6420 6e6f 7420 7368  h > 1 and not sh
-00013d70: 6170 655f 6f75 742e 6861 735f 6261 7463  ape_out.has_batc
-00013d80: 683a 2073 6861 7065 5f6f 7574 203d 2062  h: shape_out = b
-00013d90: 742e 5369 7a65 285b 6e5f 6261 7463 685d  t.Size([n_batch]
-00013da0: 2920 2b20 7368 6170 655f 6f75 740a 2020  ) + shape_out.  
-00013db0: 2020 6966 2074 6172 6765 745f 7370 6163    if target_spac
-00013dc0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00013dd0: 2020 2073 6361 6c65 2c20 2a70 6169 7273     scale, *pairs
-00013de0: 203d 2074 7261 6e73 2e72 6573 6861 7065   = trans.reshape
-00013df0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00013e00: 7363 616c 6529 203d 3d20 313a 2073 6361  scale) == 1: sca
-00013e10: 6c65 202a 3d20 6e5f 6469 6d0a 2020 2020  le *= n_dim.    
-00013e20: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
-00013e30: 203d 205b 696e 7428 7820 2a20 7929 2066   = [int(x * y) f
-00013e40: 6f72 2078 2c20 7920 696e 207a 6970 2869  or x, y in zip(i
-00013e50: 6d61 6765 2e73 7061 6365 2c20 7363 616c  mage.space, scal
-00013e60: 6529 5d0a 2020 2020 2020 2020 666f 7220  e)].        for 
-00013e70: 702c 2071 2069 6e20 7061 6972 733a 2074  p, q in pairs: t
-00013e80: 6172 6765 745f 7370 6163 655b 705d 2c20  arget_space[p], 
-00013e90: 7461 7267 6574 5f73 7061 6365 5b71 5d20  target_space[q] 
-00013ea0: 3d20 7461 7267 6574 5f73 7061 6365 5b71  = target_space[q
-00013eb0: 5d2c 2074 6172 6765 745f 7370 6163 655b  ], target_space[
-00013ec0: 705d 0a20 2020 2020 2020 2074 6172 6765  p].        targe
-00013ed0: 745f 7370 6163 6520 3d20 7475 706c 6528  t_space = tuple(
-00013ee0: 7461 7267 6574 5f73 7061 6365 290a 2020  target_space).  
-00013ef0: 2020 2020 2020 7368 6170 655f 6f75 7420        shape_out 
-00013f00: 3d20 7368 6170 655f 6f75 742e 7265 7365  = shape_out.rese
-00013f10: 745f 7370 6163 6528 7461 7267 6574 5f73  t_space(target_s
-00013f20: 7061 6365 290a 2020 2020 6966 2069 7369  pace).    if isi
-00013f30: 6e73 7461 6e63 6528 7461 7267 6574 5f73  nstance(target_s
-00013f40: 7061 6365 2c20 7475 706c 6529 2061 6e64  pace, tuple) and
-00013f50: 206c 656e 2874 6172 6765 745f 7370 6163   len(target_spac
-00013f60: 6529 203d 3d20 6e5f 6469 6d3a 2070 6173  e) == n_dim: pas
-00013f70: 730a 2020 2020 656c 6966 2069 7369 6e73  s.    elif isins
-00013f80: 7461 6e63 6528 7461 7267 6574 5f73 7061  tance(target_spa
-00013f90: 6365 2c20 6274 2e74 6f72 6368 2e54 656e  ce, bt.torch.Ten
-00013fa0: 736f 7229 3a20 7061 7373 0a20 2020 2065  sor): pass.    e
-00013fb0: 6c73 653a 2072 6169 7365 2054 7970 6545  lse: raise TypeE
-00013fc0: 7272 6f72 2866 2257 726f 6e67 2074 6172  rror(f"Wrong tar
-00013fd0: 6765 7420 7370 6163 6520 666f 7220 696e  get space for in
-00013fe0: 7465 7270 6f6c 6174 696f 6e3a 207b 7461  terpolation: {ta
-00013ff0: 7267 6574 5f73 7061 6365 7d2e 2022 290a  rget_space}. ").
-00014000: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00014010: 6528 7461 7267 6574 5f73 7061 6365 2c20  e(target_space, 
-00014020: 7475 706c 6529 3a20 0a20 2020 2020 2020  tuple): .       
-00014030: 2023 2043 7265 6174 6520 6120 6772 6964   # Create a grid
-00014040: 2058 2077 6974 6820 7369 7a65 2028 7b6e   X with size ({n
-00014050: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
-00014060: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
-00014070: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
-00014080: 2020 2020 2020 2058 203d 2062 742e 696d         X = bt.im
-00014090: 6167 655f 6772 6964 2874 6172 6765 745f  age_grid(target_
-000140a0: 7370 6163 6529 2e66 6c6f 6174 2829 2023  space).float() #
-000140b0: 202b 2062 742e 6368 616e 6e65 6c5f 7465   + bt.channel_te
-000140c0: 6e73 6f72 285b 666c 6f61 7428 612d 6229  nsor([float(a-b)
-000140d0: 2f32 2066 6f72 2061 2c20 6220 696e 207a  /2 for a, b in z
-000140e0: 6970 2869 6d61 6765 2e73 7061 6365 2c20  ip(image.space, 
-000140f0: 7461 7267 6574 5f73 7061 6365 295d 290a  target_space)]).
-00014100: 2020 2020 2020 2020 2320 436f 6d70 7574          # Comput
-00014110: 6520 7468 6520 7472 616e 7366 6f72 6d65  e the transforme
-00014120: 6420 636f 6f72 6469 6e61 7465 732e 2059  d coordinates. Y
-00014130: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
-00014140: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
-00014150: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
-00014160: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
-00014170: 2020 2020 2020 2069 6620 7472 616e 7320         if trans 
-00014180: 6973 204e 6f6e 653a 2074 7261 6e73 203d  is None: trans =
-00014190: 2049 6465 6e74 6974 7928 290a 2020 2020   Identity().    
-000141a0: 2020 2020 5920 3d20 7472 616e 7328 5829      Y = trans(X)
-000141b0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000141c0: 592e 6861 735f 6261 7463 683a 2059 203d  Y.has_batch: Y =
-000141d0: 2059 2e6d 756c 7469 706c 7928 6e5f 6261   Y.multiply(n_ba
-000141e0: 7463 682c 205b 5d29 0a20 2020 2020 2020  tch, []).       
-000141f0: 2069 6620 592e 6e5f 6261 7463 6820 3d3d   if Y.n_batch ==
-00014200: 2031 3a20 5920 3d20 592e 7265 7065 6174   1: Y = Y.repeat
-00014210: 6564 286e 5f62 6174 6368 2c20 5b5d 290a  ed(n_batch, []).
-00014220: 2020 2020 2020 2020 5920 3d20 592e 616d          Y = Y.am
-00014230: 706c 6966 7928 6e5f 6665 6174 7572 652c  plify(n_feature,
-00014240: 205b 5d29 0a20 2020 2020 2020 2073 6861   []).        sha
-00014250: 7065 5f6f 7574 203d 2073 6861 7065 5f6f  pe_out = shape_o
-00014260: 7574 2e72 6573 6574 5f73 7061 6365 2874  ut.reset_space(t
-00014270: 6172 6765 745f 7370 6163 6529 0a20 2020  arget_space).   
-00014280: 2065 6c73 653a 0a20 2020 2020 2020 2074   else:.        t
-00014290: 6172 6765 745f 7370 6163 6520 3d20 6261  arget_space = ba
-000142a0: 746f 7263 685f 7465 6e73 6f72 2874 6172  torch_tensor(tar
-000142b0: 6765 745f 7370 6163 6529 0a20 2020 2020  get_space).     
-000142c0: 2020 2069 6620 6e6f 7420 7461 7267 6574     if not target
-000142d0: 5f73 7061 6365 2e68 6173 5f62 6174 6368  _space.has_batch
-000142e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000142f0: 2074 6172 6765 745f 7370 6163 652e 7369   target_space.si
-00014300: 7a65 2830 2920 3d3d 206e 5f62 6174 6368  ze(0) == n_batch
-00014310: 2061 6e64 206e 5f62 6174 6368 2021 3d20   and n_batch != 
-00014320: 6e5f 6469 6d20 6f72 206c 656e 285b 7820  n_dim or len([x 
-00014330: 666f 7220 7820 696e 2074 6172 6765 745f  for x in target_
-00014340: 7370 6163 652e 7368 6170 6520 6966 2078  space.shape if x
-00014350: 203d 3d20 6e5f 6469 6d5d 2920 3e3d 2032   == n_dim]) >= 2
-00014360: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014370: 2020 7461 7267 6574 5f73 7061 6365 2e77    target_space.w
-00014380: 6974 685f 6261 7463 6864 696d 2830 290a  ith_batchdim(0).
-00014390: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000143a0: 3a20 7461 7267 6574 5f73 7061 6365 2e75  : target_space.u
-000143b0: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
-000143c0: 2020 2020 2020 6966 206e 6f74 2074 6172        if not tar
-000143d0: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
-000143e0: 616e 6e65 6c3a 0a20 2020 2020 2020 2020  annel:.         
-000143f0: 2020 2069 6620 7461 7267 6574 5f73 7061     if target_spa
-00014400: 6365 2e62 6174 6368 5f64 696d 656e 7369  ce.batch_dimensi
-00014410: 6f6e 2021 3d20 3020 616e 6420 7461 7267  on != 0 and targ
-00014420: 6574 5f73 7061 6365 2e73 697a 6528 3029  et_space.size(0)
-00014430: 203d 3d20 6e5f 6469 6d3a 2074 6172 6765   == n_dim: targe
-00014440: 745f 7370 6163 652e 7769 7468 5f63 6861  t_space.with_cha
-00014450: 6e6e 656c 6469 6d28 3029 0a20 2020 2020  nneldim(0).     
-00014460: 2020 2020 2020 2065 6c69 6620 7461 7267         elif targ
-00014470: 6574 5f73 7061 6365 2e62 6174 6368 5f64  et_space.batch_d
-00014480: 696d 656e 7369 6f6e 2021 3d20 3120 616e  imension != 1 an
-00014490: 6420 7461 7267 6574 5f73 7061 6365 2e73  d target_space.s
-000144a0: 697a 6528 3129 203d 3d20 6e5f 6469 6d3a  ize(1) == n_dim:
-000144b0: 2074 6172 6765 745f 7370 6163 652e 7769   target_space.wi
-000144c0: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
-000144d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-000144e0: 6620 7461 7267 6574 5f73 7061 6365 2e62  f target_space.b
-000144f0: 6174 6368 5f64 696d 656e 7369 6f6e 2021  atch_dimension !
-00014500: 3d20 7461 7267 6574 5f73 7061 6365 2e6e  = target_space.n
-00014510: 5f64 696d 202d 2031 2061 6e64 2074 6172  _dim - 1 and tar
-00014520: 6765 745f 7370 6163 652e 7369 7a65 282d  get_space.size(-
-00014530: 3129 203d 3d20 6e5f 6469 6d3a 2074 6172  1) == n_dim: tar
-00014540: 6765 745f 7370 6163 652e 7769 7468 5f63  get_space.with_c
-00014550: 6861 6e6e 656c 6469 6d28 2d31 290a 2020  hanneldim(-1).  
-00014560: 2020 2020 2020 6176 6f75 6368 2874 6172        avouch(tar
-00014570: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
-00014580: 616e 6e65 6c20 616e 6420 7461 7267 6574  annel and target
-00014590: 5f73 7061 6365 2e6e 5f63 6861 6e6e 656c  _space.n_channel
-000145a0: 203d 3d20 6e5f 6469 6d2c 2022 2774 6172   == n_dim, "'tar
-000145b0: 6765 745f 7370 6163 6527 2066 6f72 2069  get_space' for i
-000145c0: 6e74 6572 706f 6c61 7469 6f6e 2073 686f  nterpolation sho
-000145d0: 756c 6420 6861 7665 2061 2063 6861 6e6e  uld have a chann
-000145e0: 656c 2064 696d 656e 7369 6f6e 2066 6f72  el dimension for
-000145f0: 2063 6f6f 7264 696e 6174 6573 2e20 2229   coordinates. ")
-00014600: 0a20 2020 2020 2020 2059 203d 2074 6172  .        Y = tar
-00014610: 6765 745f 7370 6163 652e 7265 7065 6174  get_space.repeat
-00014620: 6564 286e 5f62 6174 6368 202f 2f20 7461  ed(n_batch // ta
-00014630: 7267 6574 5f73 7061 6365 2e6e 5f62 6174  rget_space.n_bat
-00014640: 6368 2c20 5b5d 292e 616d 706c 6966 7928  ch, []).amplify(
-00014650: 6e5f 6665 6174 7572 652c 205b 5d29 0a20  n_feature, []). 
-00014660: 2020 2020 2020 2073 6861 7065 5f6f 7574         shape_out
-00014670: 203d 2073 6861 7065 5f6f 7574 2e72 6573   = shape_out.res
-00014680: 6574 5f73 7061 6365 2874 6172 6765 745f  et_space(target_
-00014690: 7370 6163 652e 7370 6163 6529 0a20 2020  space.space).   
-000146a0: 2020 2020 200a 2020 2020 696d 6167 6520       .    image 
-000146b0: 3d20 696d 6167 652e 6d65 7267 6564 696d  = image.mergedim
-000146c0: 7328 7b7d 2c20 5b5d 290a 2020 2020 6e5f  s({}, []).    n_
-000146d0: 6261 7463 6820 3d20 696d 6167 652e 6e5f  batch = image.n_
-000146e0: 6261 7463 680a 0a20 2020 2069 6620 6d65  batch..    if me
-000146f0: 7468 6f64 2e6c 6f77 6572 2829 203d 3d20  thod.lower() == 
-00014700: 2762 7370 6c69 6e65 273a 0a20 2020 2020  'bspline':.     
-00014710: 2020 2069 6620 6465 7269 7661 7469 7665     if derivative
-00014720: 3a20 7261 6973 6520 5479 7065 4572 726f  : raise TypeErro
-00014730: 7228 224e 6f20 6465 7269 7661 7469 7665  r("No derivative
-00014740: 7320 666f 7220 6273 706c 696e 6520 696e  s for bspline in
-00014750: 7465 7270 6f6c 6174 696f 6e73 2061 7265  terpolations are
-00014760: 2061 7661 696c 6162 6c65 2073 6f20 6661   available so fa
-00014770: 722e 2050 6c65 6173 6520 7772 6974 6520  r. Please write 
-00014780: 6974 2062 7920 796f 7572 7365 6c66 2e20  it by yourself. 
-00014790: 2229 0a20 2020 2020 2020 2023 2054 4f44  ").        # TOD
-000147a0: 4f3a 2046 4644 0a20 2020 2020 2020 2072  O: FFD.        r
-000147b0: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
-000147c0: 4273 706c 696e 6520 696e 7465 7270 6f6c  Bspline interpol
-000147d0: 6174 696f 6e20 6973 206e 6f74 2061 7661  ation is not ava
-000147e0: 696c 6162 6c65 2073 6f20 6661 722e 2050  ilable so far. P
-000147f0: 6c65 6173 6520 7772 6974 6520 6974 2062  lease write it b
-00014800: 7920 796f 7572 7365 6c66 2e20 2229 0a0a  y yourself. ")..
-00014810: 2020 2020 6959 203d 2062 742e 666c 6f6f      iY = bt.floo
-00014820: 7228 5929 2e6c 6f6e 6728 2920 2320 4765  r(Y).long() # Ge
-00014830: 6e65 7261 7465 2074 6865 2069 6e74 6567  nerate the integ
-00014840: 6572 2070 6172 7420 6f66 2059 0a20 2020  er part of Y.   
-00014850: 206a 5920 3d20 6959 202b 2031 2023 2061   jY = iY + 1 # a
-00014860: 6e64 2074 6865 2069 6e74 6567 6572 2070  nd the integer p
-00014870: 6172 7420 706c 7573 206f 6e65 2e0a 2020  art plus one..  
-00014880: 2020 6966 206d 6574 686f 642e 6c6f 7765    if method.lowe
-00014890: 7228 2920 3d3d 2027 6c69 6e65 6172 273a  r() == 'linear':
-000148a0: 2066 5920 3d20 5920 2d20 6959 2e66 6c6f   fY = Y - iY.flo
-000148b0: 6174 2829 2023 2054 6865 2064 6563 696d  at() # The decim
-000148c0: 616c 2070 6172 7420 6f66 2059 2e0a 2020  al part of Y..  
-000148d0: 2020 656c 6966 206d 6574 686f 642e 6c6f    elif method.lo
-000148e0: 7765 7228 2920 3d3d 2027 6e65 6172 6573  wer() == 'neares
-000148f0: 7427 3a20 6659 203d 2062 742e 666c 6f6f  t': fY = bt.floo
-00014900: 7228 5920 2d20 6959 2e66 6c6f 6174 2829  r(Y - iY.float()
-00014910: 202b 2030 2e35 2920 2320 5468 6520 6465   + 0.5) # The de
-00014920: 6369 6d61 6c20 7061 7274 206f 6620 592e  cimal part of Y.
-00014930: 0a20 2020 2065 6c73 653a 2072 6169 7365  .    else: raise
-00014940: 2054 7970 6545 7272 6f72 2822 556e 7265   TypeError("Unre
-00014950: 636f 676e 697a 6564 2061 7267 756d 656e  cognized argumen
-00014960: 7420 276d 6574 686f 6427 2e20 2229 0a20  t 'method'. "). 
-00014970: 2020 2062 5920 3d20 6274 2e73 7461 636b     bY = bt.stack
-00014980: 2828 6959 2c20 6a59 292c 2031 292e 7669  ((iY, jY), 1).vi
-00014990: 6577 285b 6e5f 6261 7463 685d 2c20 322c  ew([n_batch], 2,
-000149a0: 207b 6e5f 6469 6d7d 2c20 2d31 2920 2320   {n_dim}, -1) # 
-000149b0: 285b 6e5f 6261 7463 685d 2c20 322c 207b  ([n_batch], 2, {
-000149c0: 6e5f 6469 6d7d 2c20 6e5f 6461 7461 292e  n_dim}, n_data).
-000149d0: 0a20 2020 2057 203d 2062 742e 7374 6163  .    W = bt.stac
-000149e0: 6b28 2831 202d 2066 592c 2066 5929 2c20  k((1 - fY, fY), 
-000149f0: 3129 2e76 6965 7728 5b6e 5f62 6174 6368  1).view([n_batch
-00014a00: 5d2c 2032 2c20 7b6e 5f64 696d 7d2c 202d  ], 2, {n_dim}, -
-00014a10: 3129 2023 2028 5b6e 5f62 6174 6368 5d2c  1) # ([n_batch],
-00014a20: 2032 2c20 7b6e 5f64 696d 7d2c 206e 5f64   2, {n_dim}, n_d
-00014a30: 6174 6129 2e0a 2020 2020 6e5f 6461 7461  ata)..    n_data
-00014a40: 203d 2062 592e 7369 7a65 282d 3129 0a0a   = bY.size(-1)..
-00014a50: 2020 2020 2320 5072 6570 6172 6520 666f      # Prepare fo
-00014a60: 7220 7468 6520 6f75 7470 7574 2073 7061  r the output spa
-00014a70: 6365 3a20 6e5f 6261 7463 682c 206d 5f31  ce: n_batch, m_1
-00014a80: 2c20 2e2e 2e2c 206d 5f73 0a20 2020 2069  , ..., m_s.    i
-00014a90: 6620 6465 7269 7661 7469 7665 3a20 6f75  f derivative: ou
-00014aa0: 7470 7574 203d 2062 742e 7a65 726f 7328  tput = bt.zeros(
-00014ab0: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
-00014ac0: 6d7d 2c20 2a73 6861 7065 5f6f 7574 2e73  m}, *shape_out.s
-00014ad0: 7061 6365 290a 2020 2020 656c 7365 3a20  pace).    else: 
-00014ae0: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
-00014af0: 7328 7368 6170 655f 6f75 7429 0a20 2020  s(shape_out).   
-00014b00: 2066 6f72 2047 2069 6e20 6274 2e69 6d61   for G in bt.ima
-00014b10: 6765 5f67 7269 6428 5b32 5d2a 6e5f 6469  ge_grid([2]*n_di
-00014b20: 6d29 2e66 6c61 7474 656e 2829 2e74 7261  m).flatten().tra
-00014b30: 6e73 706f 7365 2830 2c20 3129 3a0a 2020  nspose(0, 1):.  
-00014b40: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-00014b50: 696e 6469 6365 7320 666f 7220 7468 6520  indices for the 
-00014b60: 7465 726d 3a20 6259 5b3a 2c20 475b 445d  term: bY[:, G[D]
-00014b70: 2c20 442c 203a 5d2c 2073 697a 653d 285b  , D, :], size=([
-00014b80: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
-00014b90: 7d2c 206e 5f64 6174 6129 0a20 2020 2020  }, n_data).     
-00014ba0: 2020 2049 6e64 203d 2062 592e 6761 7468     Ind = bY.gath
-00014bb0: 6572 2831 2c20 472e 6578 7061 6e64 5f74  er(1, G.expand_t
-00014bc0: 6f28 5b6e 5f62 6174 6368 5d2c 2031 2c20  o([n_batch], 1, 
-00014bd0: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6129  {n_dim}, n_data)
-00014be0: 292e 7371 7565 657a 6528 3129 0a20 2020  ).squeeze(1).   
-00014bf0: 2020 2020 2023 2043 6c61 6d70 2074 6865       # Clamp the
-00014c00: 2069 6e64 6963 6573 2069 6e20 7468 6520   indices in the 
-00014c10: 636f 7272 6563 7420 7261 6e67 6520 2620  correct range & 
-00014c20: 436f 6d70 7574 6520 7468 6520 626f 7264  Compute the bord
-00014c30: 6572 2063 6f6e 6469 7469 6f6e 0a20 2020  er condition.   
-00014c40: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
-00014c50: 2062 742e 7375 6d28 2849 6e64 203c 2030   bt.sum((Ind < 0
-00014c60: 2920 2b20 2849 6e64 203e 2073 697a 6520  ) + (Ind > size 
-00014c70: 2d20 3129 2c20 3129 0a20 2020 2020 2020  - 1), 1).       
-00014c80: 2049 6e64 203d 2062 742e 6d69 6e28 6274   Ind = bt.min(bt
-00014c90: 2e63 6c61 6d70 2849 6e64 2c20 6d69 6e3d  .clamp(Ind, min=
-00014ca0: 3029 2c20 2873 697a 6520 2d20 3129 2e65  0), (size - 1).e
-00014cb0: 7870 616e 645f 746f 2849 6e64 2929 0a20  xpand_to(Ind)). 
-00014cc0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
-00014cd0: 2074 6865 2069 6e64 6963 6573 2074 6f20   the indices to 
-00014ce0: 3120 6469 6d65 6e73 696f 6e61 6c2e 2044  1 dimensional. D
-00014cf0: 6f74 3a20 285b 6e5f 6261 7463 685d 2c20  ot: ([n_batch], 
-00014d00: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
-00014d10: 446f 7420 3d20 496e 645b 3a2c 2030 5d0a  Dot = Ind[:, 0].
-00014d20: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
-00014d30: 2072 616e 6765 2831 2c20 6e5f 6469 6d29   range(1, n_dim)
-00014d40: 3a20 446f 7420 2a3d 2073 697a 655b 725d  : Dot *= size[r]
-00014d50: 3b20 446f 7420 2b3d 2049 6e64 5b3a 2c20  ; Dot += Ind[:, 
-00014d60: 725d 0a20 2020 2020 2020 2023 2047 6574  r].        # Get
-00014d70: 2074 6865 2069 6d61 6765 2076 616c 7565   the image value
-00014d80: 7320 4956 3a20 285b 6e5f 6261 7463 685d  s IV: ([n_batch]
-00014d90: 2c20 6e5f 6461 7461 290a 2020 2020 2020  , n_data).      
-00014da0: 2020 4956 203d 204e 6f6e 650a 2020 2020    IV = None.    
-00014db0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00014dc0: 6528 6669 6c6c 2c20 7374 7229 3a0a 2020  e(fill, str):.  
-00014dd0: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
-00014de0: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6e65  l.lower() == 'ne
-00014df0: 6172 6573 7427 3a0a 2020 2020 2020 2020  arest':.        
-00014e00: 2020 2020 2020 2020 4956 203d 2069 6d61          IV = ima
-00014e10: 6765 2e66 6c61 7474 656e 2829 2e67 6174  ge.flatten().gat
-00014e20: 6865 7228 312c 2044 6f74 290a 2020 2020  her(1, Dot).    
-00014e30: 2020 2020 2020 2020 656c 6966 2066 696c          elif fil
-00014e40: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6261  l.lower() == 'ba
-00014e50: 636b 6772 6f75 6e64 273a 0a20 2020 2020  ckground':.     
-00014e60: 2020 2020 2020 2020 2020 2062 6b5f 7661             bk_va
-00014e70: 6c75 6520 3d20 6274 2e73 7461 636b 285b  lue = bt.stack([
-00014e80: 696d 6167 655b 2873 6c69 6365 284e 6f6e  image[(slice(Non
-00014e90: 6529 2c29 202b 2074 7570 6c65 2867 295d  e),) + tuple(g)]
-00014ea0: 2066 6f72 2067 2069 6e20 2862 742e 696d   for g in (bt.im
-00014eb0: 6167 655f 6772 6964 285b 325d 2a6e 5f64  age_grid([2]*n_d
-00014ec0: 696d 2920 2a20 6274 2e63 6861 6e6e 656c  im) * bt.channel
-00014ed0: 5f74 656e 736f 7228 7369 7a65 2d31 2929  _tensor(size-1))
-00014ee0: 2e66 6c61 7474 656e 2829 2e74 7261 6e73  .flatten().trans
-00014ef0: 706f 7365 2830 2c31 295d 2c20 3129 2e6d  pose(0,1)], 1).m
-00014f00: 6564 6961 6e28 3129 2e76 616c 7565 730a  edian(1).values.
-00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f20: 6261 636b 6772 6f75 6e64 203d 2062 6b5f  background = bk_
-00014f30: 7661 6c75 6520 2a20 6274 2e6f 6e65 735f  value * bt.ones_
-00014f40: 6c69 6b65 2844 6f74 290a 2020 2020 2020  like(Dot).      
-00014f50: 2020 2020 2020 656c 6966 2066 696c 6c2e        elif fill.
-00014f60: 6c6f 7765 7228 2920 3d3d 2027 7a65 726f  lower() == 'zero
-00014f70: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00014f80: 2020 2062 6163 6b67 726f 756e 6420 3d20     background = 
-00014f90: 6274 2e7a 6572 6f73 5f6c 696b 6528 446f  bt.zeros_like(Do
-00014fa0: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
-00014fb0: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
-00014fc0: 6b67 726f 756e 6420 3d20 6669 6c6c 202a  kground = fill *
-00014fd0: 2062 742e 6f6e 6573 5f6c 696b 6528 446f   bt.ones_like(Do
-00014fe0: 7429 0a20 2020 2020 2020 2069 6620 4956  t).        if IV
-00014ff0: 2069 7320 4e6f 6e65 3a20 4956 203d 2062   is None: IV = b
-00015000: 742e 7768 6572 6528 636f 6e64 6974 696f  t.where(conditio
-00015010: 6e20 3e3d 2031 2c20 6261 636b 6772 6f75  n >= 1, backgrou
-00015020: 6e64 2e66 6c6f 6174 2829 2c20 696d 6167  nd.float(), imag
-00015030: 652e 666c 6174 7465 6e28 292e 6761 7468  e.flatten().gath
-00015040: 6572 2831 2c20 446f 7429 2e66 6c6f 6174  er(1, Dot).float
-00015050: 2829 290a 2020 2020 2020 2020 2320 5765  ()).        # We
-00015060: 6967 6874 7320 666f 7220 6561 6368 2070  ights for each p
-00015070: 6f69 6e74 3a20 5b70 726f 6475 6374 206f  oint: [product o
-00015080: 6620 575b 3a2c 2047 5b44 5d2c 2044 2c20  f W[:, G[D], D, 
-00015090: 785d 2066 6f72 2044 2069 6e20 7261 6e67  x] for D in rang
-000150a0: 6528 6e5f 6469 6d29 5d20 666f 7220 706f  e(n_dim)] for po
-000150b0: 696e 7420 782e 0a20 2020 2020 2020 2023  int x..        #
-000150c0: 2057 673a 2028 5b6e 5f62 6174 6368 5d2c   Wg: ([n_batch],
-000150d0: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
-000150e0: 290a 2020 2020 2020 2020 5767 203d 2057  ).        Wg = W
-000150f0: 2e67 6174 6865 7228 312c 2047 2e65 7870  .gather(1, G.exp
-00015100: 616e 645f 746f 285b 6e5f 6261 7463 685d  and_to([n_batch]
-00015110: 2c20 312c 207b 6e5f 6469 6d7d 2c20 6e5f  , 1, {n_dim}, n_
-00015120: 6461 7461 2929 2e73 7175 6565 7a65 2831  data)).squeeze(1
-00015130: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00015140: 2064 6572 6976 6174 6976 653a 0a20 2020   derivative:.   
-00015150: 2020 2020 2020 2020 206f 7574 7075 7420           output 
-00015160: 2b3d 2028 5767 2e70 726f 6428 3129 202a  += (Wg.prod(1) *
-00015170: 2049 5629 2e76 6965 775f 6173 286f 7574   IV).view_as(out
-00015180: 7075 7429 0a20 2020 2020 2020 2065 6c73  put).        els
-00015190: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000151a0: 656d 7057 674d 6174 203d 2057 672e 6d75  empWgMat = Wg.mu
-000151b0: 6c74 6970 6c79 286e 5f64 696d 2c20 3129  ltiply(n_dim, 1)
-000151c0: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
-000151d0: 5f64 696d 2c20 7b6e 5f64 696d 7d2c 206e  _dim, {n_dim}, n
-000151e0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
-000151f0: 2020 2074 656d 7057 674d 6174 5b3a 2c20     tempWgMat[:, 
-00015200: 6274 2e61 7261 6e67 6528 6e5f 6469 6d29  bt.arange(n_dim)
-00015210: 2c20 6274 2e61 7261 6e67 6528 6e5f 6469  , bt.arange(n_di
-00015220: 6d29 5d20 3d20 310a 2020 2020 2020 2020  m)] = 1.        
-00015230: 2020 2020 6457 6720 3d20 7465 6d70 5767      dWg = tempWg
-00015240: 4d61 742e 7072 6f64 2831 2920 2a20 2847  Mat.prod(1) * (G
-00015250: 202a 2032 202d 2031 292e 666c 6f61 7428   * 2 - 1).float(
-00015260: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
-00015270: 7470 7574 202b 3d20 2864 5767 202a 2049  tput += (dWg * I
-00015280: 562e 756e 7371 7565 657a 6528 3129 292e  V.unsqueeze(1)).
-00015290: 7669 6577 5f61 7328 6f75 7470 7574 290a  view_as(output).
-000152a0: 2020 2020 6274 2e74 6f72 6368 2e63 7564      bt.torch.cud
-000152b0: 612e 656d 7074 795f 6361 6368 6528 290a  a.empty_cache().
-000152c0: 2020 2020 6570 7320 3d20 3165 2d36 0a20      eps = 1e-6. 
-000152d0: 2020 206d 203d 2030 2069 6620 696d 6167     m = 0 if imag
-000152e0: 652e 6d69 6e28 2920 3e20 2d65 7073 2065  e.min() > -eps e
-000152f0: 6c73 6520 696d 6167 652e 6d69 6e28 292e  lse image.min().
-00015300: 6974 656d 2829 0a20 2020 204d 203d 2031  item().    M = 1
-00015310: 2069 6620 696d 6167 652e 6d61 7828 2920   if image.max() 
-00015320: 3c20 3120 2b20 6570 7320 656c 7365 2069  < 1 + eps else i
-00015330: 6d61 6765 2e6d 6178 2829 2e69 7465 6d28  mage.max().item(
-00015340: 290a 2020 2020 7265 7475 726e 206f 7574  ).    return out
-00015350: 7075 742e 636c 616d 7028 6d2c 204d 290a  put.clamp(m, M).
-00015360: 0a40 616c 6961 7328 2272 6573 616d 706c  .@alias("resampl
-00015370: 655f 666f 7277 6172 6422 290a 6465 6620  e_forward").def 
-00015380: 696e 7465 7270 6f6c 6174 696f 6e5f 666f  interpolation_fo
-00015390: 7277 6172 6428 0a20 2020 2020 2020 2069  rward(.        i
-000153a0: 6d61 6765 2c20 0a20 2020 2020 2020 2074  mage, .        t
-000153b0: 7261 6e73 203d 204e 6f6e 652c 200a 2020  rans = None, .  
-000153c0: 2020 2020 2020 6d65 7468 6f64 203d 2027        method = '
-000153d0: 4c69 6e65 6172 272c 200a 2020 2020 2020  Linear', .      
-000153e0: 2020 7461 7267 6574 5f73 7061 6365 203d    target_space =
-000153f0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
-00015400: 696c 6c20 3d20 277a 6572 6f27 2c0a 2020  ill = 'zero',.  
-00015410: 2020 2020 2020 6465 7269 7661 7469 7665        derivative
-00015420: 203d 2046 616c 7365 0a20 2020 2029 3a0a   = False.    ):.
-00015430: 2020 2020 2727 270a 2020 2020 496e 7465      '''.    Inte
-00015440: 7270 6f6c 6174 6520 7573 696e 6720 666f  rpolate using fo
-00015450: 7277 6172 6420 7472 616e 7366 6f72 6d61  rward transforma
-00015460: 7469 6f6e 2e20 4974 2069 7320 6e6f 7420  tion. It is not 
-00015470: 7965 7420 696d 706c 656d 656e 7465 642e  yet implemented.
-00015480: 200a 2020 2020 692e 652e 2043 6f6d 7075   .    i.e. Compu
-00015490: 7465 2074 6865 2069 6d61 6765 2049 2073  te the image I s
-000154a0: 2e74 2e20 7472 616e 7328 7829 203d 2079  .t. trans(x) = y
-000154b0: 2066 6f72 2078 2069 6e20 696e 7075 7420   for x in input 
-000154c0: 696d 6167 6520 616e 6420 7920 696e 2074  image and y in t
-000154d0: 6865 206f 7574 7075 7420 4920 7573 696e  he output I usin
-000154e0: 6720 696e 7465 7270 6f6c 6174 696f 6e20  g interpolation 
-000154f0: 6d65 7468 6f64 3a0a 2020 2020 2020 2020  method:.        
-00015500: 6d65 7468 6f64 203d 204c 696e 6561 7220  method = Linear 
-00015510: 5b4e 4f20 4752 4144 4945 4e54 2121 215d  [NO GRADIENT!!!]
-00015520: 3a20 4269 6c69 6e65 6172 2069 6e74 6572  : Bilinear inter
-00015530: 706f 6c61 7469 6f6e 0a20 2020 2020 2020  polation.       
-00015540: 206d 6574 686f 6420 3d20 4e65 6172 6573   method = Neares
-00015550: 7420 5b4e 4f20 4752 4144 4945 4e54 2121  t [NO GRADIENT!!
-00015560: 215d 3a20 4e65 6172 6573 7420 696e 7465  !]: Nearest inte
-00015570: 7270 6f6c 6174 696f 6e0a 0a20 2020 2050  rpolation..    P
-00015580: 6172 616d 733a 0a20 2020 2020 2020 2069  arams:.        i
-00015590: 6d61 6765 205b 6274 2e54 656e 736f 725d  mage [bt.Tensor]
-000155a0: 3a20 5468 6520 7461 7267 6574 2069 6d61  : The target ima
-000155b0: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
-000155c0: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
-000155d0: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6368  optional], {n_ch
-000155e0: 616e 6e65 6c3a 6f70 7469 6f6e 616c 7d2c  annel:optional},
-000155f0: 206d 4031 2c20 6d40 322c 202e 2e2e 2c20   m@1, m@2, ..., 
-00015600: 6d40 6e5f 6469 6d29 0a20 2020 2020 2020  m@n_dim).       
-00015610: 2074 7261 6e73 205b 4675 6e63 7469 6f6e   trans [Function
-00015620: 206f 7220 6d69 636f 6d70 7574 696e 672e   or micomputing.
-00015630: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
-00015640: 6174 696f 6e5d 3a20 5472 616e 7366 6f72  ation]: Transfor
-00015650: 6d61 7469 6f6e 2066 756e 6374 696f 6e2c  mation function,
-00015660: 206d 6170 7069 6e67 0a20 2020 2020 2020   mapping.       
-00015670: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
-00015680: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
-00015690: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
-000156a0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-000156b0: 2074 6f20 285b 6e5f 6261 7463 685d 2c20   to ([n_batch], 
-000156c0: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
-000156d0: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
-000156e0: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
-000156f0: 5b73 7472 3a20 6c69 6e65 6172 7c6e 6561  [str: linear|nea
-00015700: 7265 7374 5d3a 2054 6865 2069 6e74 6572  rest]: The inter
-00015710: 706f 6c61 7469 6f6e 206d 6574 686f 642e  polation method.
-00015720: 200a 2020 2020 2020 2020 7461 7267 6574   .        target
-00015730: 5f73 7061 6365 205b 7475 706c 6520 6f72  _space [tuple or
-00015740: 2062 742e 5465 6e73 6f72 5d3a 0a20 2020   bt.Tensor]:.   
-00015750: 2020 2020 2020 2020 2053 697a 6520 2874           Size (t
-00015760: 7570 6c65 2920 6f66 2061 2074 6172 6765  uple) of a targe
-00015770: 7420 524f 4920 6174 2074 6865 2063 656e  t ROI at the cen
-00015780: 7465 7220 6f66 2069 6d61 6765 2e20 0a20  ter of image. . 
-00015790: 2020 2020 2020 2020 2020 204f 5220 5472             OR Tr
-000157a0: 616e 7366 6f72 6d65 6420 636f 6f72 6469  ansformed coordi
-000157b0: 6e61 7465 2073 7061 6365 2028 6274 2e54  nate space (bt.T
-000157c0: 656e 736f 7229 206f 6620 7468 6520 6f75  ensor) of the ou
-000157d0: 7470 7574 2069 6d61 6765 2e20 0a20 2020  tput image. .   
-000157e0: 2020 2020 2020 2020 2073 697a 653a 206c           size: l
-000157f0: 656e 6774 6828 6e5f 6469 6d29 206f 7220  ength(n_dim) or 
-00015800: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
-00015810: 616c 5d2c 207b 6e5f 6469 6d3a 6f70 7469  al], {n_dim:opti
-00015820: 6f6e 616c 7d2c 2073 697a 6540 312c 2073  onal}, size@1, s
-00015830: 697a 6540 322c 202e 2e2e 2c20 7369 7a65  ize@2, ..., size
-00015840: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
-00015850: 6669 6c6c 205b 7374 723a 206e 6561 7265  fill [str: neare
-00015860: 7374 7c62 6163 6b67 726f 756e 6420 6f72  st|background or
-00015870: 2069 6e74 206f 7220 666c 6f61 7428 6e75   int or float(nu
-00015880: 6d62 6572 295d 3a20 496e 6469 6361 7465  mber)]: Indicate
-00015890: 2074 6865 2077 6179 2074 6f20 6669 6c6c   the way to fill
-000158a0: 2062 6163 6b67 726f 756e 6420 6f75 7473   background outs
-000158b0: 6964 6520 6053 7572 726f 756e 6469 6e67  ide `Surrounding
-000158c0: 602e 200a 2020 2020 2020 2020 6465 7269  `. .        deri
-000158d0: 7661 7469 7665 205b 626f 6f6c 5d3a 2057  vative [bool]: W
-000158e0: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
-000158f0: 2074 6865 2067 7261 6469 656e 742e 204f   the gradient. O
-00015900: 6e65 2063 616e 206f 6d69 7420 6974 2077  ne can omit it w
-00015910: 6865 6e20 7573 696e 6720 746f 7263 682e  hen using torch.
-00015920: 6175 746f 6772 6164 2e0a 0a20 2020 2020  autograd...     
-00015930: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
-00015940: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
-00015950: 666f 726d 6564 2069 6d61 6765 2e0a 2020  formed image..  
-00015960: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00015970: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
-00015980: 6861 6e6e 656c 3a6f 7074 696f 6e61 6c7d  hannel:optional}
-00015990: 2c20 6d40 312c 206d 4032 2c20 2e2e 2e2c  , m@1, m@2, ...,
-000159a0: 206d 406e 5f64 696d 290a 2020 2020 2020   m@n_dim).      
-000159b0: 2020 2020 2020 6f72 2077 6865 6e20 6074        or when `t
-000159c0: 6172 6765 745f 7370 6163 6560 2069 7320  arget_space` is 
-000159d0: 6465 6669 6e65 6420 6279 2074 656e 736f  defined by tenso
-000159e0: 722e 200a 2020 2020 2020 2020 2020 2020  r. .            
-000159f0: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
-00015a00: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
-00015a10: 2c20 2e2e 2e2c 2073 697a 6540 6e5f 6469  , ..., size@n_di
-00015a20: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
-00015a30: 7220 7468 6520 6465 7269 7661 7469 7665  r the derivative
-00015a40: 2066 6f72 2074 6865 2069 6e74 6572 706f   for the interpo
-00015a50: 6c61 7469 6f6e 2e20 2869 6620 6064 6572  lation. (if `der
-00015a60: 6976 6174 6976 6520 3d20 5472 7565 6029  ivative = True`)
-00015a70: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00015a80: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00015a90: 6e5f 6469 6d7d 2c20 7369 7a65 4031 2c20  n_dim}, size@1, 
-00015aa0: 7369 7a65 4032 2c20 2e2e 2e2c 2073 697a  size@2, ..., siz
-00015ab0: 6540 6e5f 6469 6d29 0a0a 2020 2020 4578  e@n_dim)..    Ex
-00015ac0: 616d 706c 6573 3a0a 2020 2020 2d2d 2d2d  amples:.    ----
-00015ad0: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2049  ------.    >>> I
-00015ae0: 6d61 6765 203d 2062 742e 7261 6e64 2833  mage = bt.rand(3
-00015af0: 2c20 3130 302c 2031 3230 2c20 3830 290a  , 100, 120, 80).
-00015b00: 2020 2020 3e3e 3e20 414d 203d 2062 742e      >>> AM = bt.
-00015b10: 7261 6e64 2834 2c20 3429 0a20 2020 203e  rand(4, 4).    >
-00015b20: 3e3e 2041 4d5b 332c 203a 5d20 3d20 6274  >> AM[3, :] = bt
-00015b30: 2e6f 6e65 5f68 6f74 282d 312c 2034 290a  .one_hot(-1, 4).
-00015b40: 2020 2020 3e3e 3e20 696e 7465 7270 6f6c      >>> interpol
-00015b50: 6174 696f 6e28 496d 6167 652c 2041 6666  ation(Image, Aff
-00015b60: 696e 6528 414d 292c 206d 6574 686f 643d  ine(AM), method=
-00015b70: 274c 696e 6561 7227 290a 2020 2020 2727  'Linear').    ''
-00015b80: 270a 2020 2020 6966 2074 7261 6e73 2069  '.    if trans i
-00015b90: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2074  s not None and t
-00015ba0: 7261 6e73 2e62 6163 6b77 6172 643a 0a20  rans.backward:. 
-00015bb0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00015bc0: 7228 7472 616e 732c 2027 696e 7627 293a  r(trans, 'inv'):
-00015bd0: 2074 7261 6e73 203d 2074 7261 6e73 2e69   trans = trans.i
-00015be0: 6e76 2829 2e66 616b 655f 696e 7628 290a  nv().fake_inv().
-00015bf0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00015c00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00015c10: 2257 6172 6e69 6e67 3a20 4261 636b 7761  "Warning: Backwa
-00015c20: 7264 2074 7261 6e73 666f 726d 6174 696f  rd transformatio
-00015c30: 6e20 666f 756e 6420 696e 206d 6574 686f  n found in metho
-00015c40: 6420 6069 6e74 6572 706f 6c61 7469 6f6e  d `interpolation
-00015c50: 5f66 6f72 7761 7264 602e 2055 7369 6e67  _forward`. Using
-00015c60: 2060 696e 7465 7270 6f6c 6174 696f 6e60   `interpolation`
-00015c70: 2069 6e73 7465 6164 2e20 2229 0a20 2020   instead. ").   
-00015c80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00015c90: 696e 7465 7270 6f6c 6174 696f 6e28 696d  interpolation(im
-00015ca0: 6167 652c 2074 7261 6e73 2c20 6d65 7468  age, trans, meth
-00015cb0: 6f64 203d 206d 6574 686f 642c 2074 6172  od = method, tar
-00015cc0: 6765 745f 7370 6163 6520 3d20 7461 7267  get_space = targ
-00015cd0: 6574 5f73 7061 6365 2c20 6669 6c6c 203d  et_space, fill =
-00015ce0: 2066 696c 6c29 0a20 2020 2072 6574 7572   fill).    retur
-00015cf0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
-00015d00: 0a0a 2323 2323 2323 2323 2323 2323 2049  ..############ I
-00015d10: 6d61 6765 2054 7261 6e73 666f 726d 6174  mage Transformat
-00015d20: 696f 6e73 2023 2323 2323 2323 2323 2323  ions ###########
-00015d30: 230a 0a63 6c61 7373 2049 6d61 6765 5472  #..class ImageTr
-00015d40: 616e 7366 6f72 6d61 7469 6f6e 2854 7261  ansformation(Tra
-00015d50: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
-00015d60: 2020 2020 2020 0a20 2020 2064 6566 205f        .    def _
-00015d70: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
-00015d80: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-00015d90: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
-00015da0: 6f72 5d3a 2049 6d61 6765 2074 6f20 6265  or]: Image to be
-00015db0: 2074 7261 6e73 666f 726d 6564 2e0a 2020   transformed..  
-00015dc0: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00015dd0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
-00015de0: 616c 5d2c 207b 6e5f 6368 616e 6e65 6c3a  al], {n_channel:
-00015df0: 6f70 7469 6f6e 616c 7d2c 206e 4031 2c20  optional}, n@1, 
-00015e00: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
-00015e10: 6d29 0a20 2020 2020 2020 206f 7574 7075  m).        outpu
-00015e20: 7420 5b62 742e 5465 6e73 6f72 5d3a 2054  t [bt.Tensor]: T
-00015e30: 6865 2074 7261 6e73 666f 726d 6564 2069  he transformed i
-00015e40: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
-00015e50: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-00015e60: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
-00015e70: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
-00015e80: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
-00015e90: 2027 2727 0a20 2020 2020 2020 2058 203d   '''.        X =
-00015ea0: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
-00015eb0: 5829 0a20 2020 2020 2020 2069 6620 7365  X).        if se
-00015ec0: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
-00015ed0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00015ee0: 206e 6f74 2058 2e68 6173 5f62 6174 6368   not X.has_batch
-00015ef0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
-00015f00: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
-00015f10: 2020 6966 206e 6f74 2058 2e68 6173 5f63    if not X.has_c
-00015f20: 6861 6e6e 656c 3a20 5820 3d20 582e 7374  hannel: X = X.st
-00015f30: 616e 6461 7264 2829 2e75 6e73 7175 6565  andard().unsquee
-00015f40: 7a65 287b 317d 290a 2020 2020 2020 2020  ze({1}).        
-00015f50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015f60: 2020 6966 2058 2e6e 5f64 696d 203d 3d20    if X.n_dim == 
-00015f70: 7365 6c66 2e6e 5f64 696d 3a20 5820 3d20  self.n_dim: X = 
-00015f80: 582e 7265 6d6f 7665 5f73 7065 6369 616c  X.remove_special
-00015f90: 5f28 292e 756e 7371 7565 657a 6528 5b5d  _().unsqueeze([]
-00015fa0: 292e 756e 7371 7565 657a 6528 7b31 7d29  ).unsqueeze({1})
-00015fb0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00015fc0: 6620 582e 6e5f 6469 6d20 3d3d 2073 656c  f X.n_dim == sel
-00015fd0: 662e 6e5f 6469 6d20 2b20 313a 0a20 2020  f.n_dim + 1:.   
-00015fe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015ff0: 582e 6861 735f 6261 7463 683a 2058 2e63  X.has_batch: X.c
-00016000: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
-00016010: 203d 204e 6f6e 653b 2058 203d 2058 2e75   = None; X = X.u
-00016020: 6e73 7175 6565 7a65 287b 3020 6966 2058  nsqueeze({0 if X
-00016030: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
-00016040: 203e 2030 2065 6c73 6520 317d 290a 2020   > 0 else 1}).  
-00016050: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00016060: 6966 2058 2e68 6173 5f63 6861 6e6e 656c  if X.has_channel
-00016070: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
-00016080: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
-00016090: 2020 2020 2020 656c 7365 3a20 5820 3d20        else: X = 
-000160a0: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
-000160b0: 6e5f 2830 292e 756e 7371 7565 657a 6528  n_(0).unsqueeze(
-000160c0: 7b31 7d29 0a20 2020 2020 2020 2020 2020  {1}).           
-000160d0: 2065 6c69 6620 582e 6e5f 6469 6d20 3d3d   elif X.n_dim ==
-000160e0: 2073 656c 662e 6e5f 6469 6d20 2b20 323a   self.n_dim + 2:
-000160f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016100: 2023 205f 6368 616e 6e61 6c2f 6261 7463   # _channal/batc
-00016110: 6820 6469 6d65 6e73 696f 6e73 2075 7365  h dimensions use
-00016120: 6420 6865 7265 2061 7320 7468 6579 2061  d here as they a
-00016130: 7265 206e 5f64 696d 2077 6865 6e20 6e6f  re n_dim when no
-00016140: 7420 6578 6973 7465 642e 200a 2020 2020  t existed. .    
-00016150: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00016160: 6f74 2058 2e68 6173 5f62 6174 6368 3a20  ot X.has_batch: 
-00016170: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
-00016180: 6e20 3d20 3020 6966 2058 2e5f 6368 616e  n = 0 if X._chan
-00016190: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3e20  nel_dimension > 
-000161a0: 3020 656c 7365 2031 0a20 2020 2020 2020  0 else 1.       
-000161b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000161c0: 582e 6861 735f 6368 616e 6e65 6c3a 2058  X.has_channel: X
-000161d0: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
-000161e0: 6f6e 203d 2030 2069 6620 582e 5f62 6174  on = 0 if X._bat
-000161f0: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
-00016200: 2065 6c73 6520 310a 2020 2020 2020 2020   else 1.        
-00016210: 6176 6f75 6368 2858 2e68 6173 5f62 6174  avouch(X.has_bat
-00016220: 6368 2061 6e64 2058 2e68 6173 5f63 6861  ch and X.has_cha
-00016230: 6e6e 656c 2c20 6622 506c 6561 7365 2075  nnel, f"Please u
-00016240: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
-00016250: 7220 6f66 2073 697a 6520 5c0a 2020 2020  r of size \.    
-00016260: 2020 2020 2020 2020 285b 6e5f 6261 7463          ([n_batc
-00016270: 685d 2c20 7b7b 6e5f 6368 616e 6e65 6c2f  h], {{n_channel/
-00016280: 6e5f 6665 6174 7572 653a 6f70 7469 6f6e  n_feature:option
-00016290: 616c 7d7d 2c20 6d5f 312c 206d 5f32 2c20  al}}, m_1, m_2, 
-000162a0: 2e2e 2e2c 206d 5f72 2920 5b72 3d6e 5f64  ..., m_r) [r=n_d
-000162b0: 696d 5d20 666f 7220 5c0a 2020 2020 2020  im] for \.      
-000162c0: 2020 2020 2020 2020 2020 7b73 656c 662e            {self.
-000162d0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-000162e0: 5f5f 2e73 706c 6974 2827 2e27 295b 2d31  __.split('.')[-1
-000162f0: 5d7d 2054 7261 6e73 666f 726d 6174 696f  ]} Transformatio
-00016300: 6e2c 2069 6e73 7465 6164 206f 6620 7b58  n, instead of {X
-00016310: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
-00016320: 2020 2020 7265 7475 726e 2058 2e63 6c6f      return X.clo
-00016330: 6e65 2829 0a0a 636c 6173 7320 4e6f 726d  ne()..class Norm
-00016340: 616c 697a 6528 496d 6167 6554 7261 6e73  alize(ImageTrans
-00016350: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
-00016360: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00016370: 662c 202a 5f72 616e 6765 293a 0a20 2020  f, *_range):.   
-00016380: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00016390: 204e 6f72 6d61 6c69 7a65 2074 6865 2069   Normalize the i
-000163a0: 6e74 656e 7369 7479 206f 6620 616e 2069  ntensity of an i
-000163b0: 6d61 6765 2e0a 2020 2020 2020 2020 0a20  mage..        . 
-000163c0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
-000163d0: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
-000163e0: 6520 3d20 286c 6f77 2c20 6869 6768 2920  e = (low, high) 
-000163f0: 5b69 6e74 206f 7220 666c 6f61 7420 6f72  [int or float or
-00016400: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
-00016410: 206c 6f77 6573 7420 2861 6e64 2068 6967   lowest (and hig
-00016420: 6865 7374 2920 696e 7465 6e73 6974 792e  hest) intensity.
-00016430: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00016440: 2020 7369 7a65 3a20 6c65 6e67 7468 2832    size: length(2
-00016450: 2920 6f72 2028 5b6e 5f62 6174 6368 5d2c  ) or ([n_batch],
-00016460: 207b 327d 290a 2020 2020 2020 2020 2020   {2}).          
-00016470: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
-00016480: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
-00016490: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
-000164a0: 5465 6e73 6f72 5d3a 2049 6d61 6765 2074  Tensor]: Image t
-000164b0: 6f20 6265 2074 7261 6e73 666f 726d 6564  o be transformed
-000164c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000164d0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-000164e0: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
-000164f0: 6368 616e 6e65 6c3a 6f70 7469 6f6e 616c  channel:optional
-00016500: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
-00016510: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
-00016520: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
-00016530: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
-00016540: 7261 6e73 666f 726d 6564 2069 6d61 6765  ransformed image
-00016550: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016560: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
-00016570: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
-00016580: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
-00016590: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
-000165a0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
-000165b0: 6c65 6e28 5f72 616e 6765 2920 3d3d 2030  len(_range) == 0
-000165c0: 3a20 5f72 616e 6765 203d 204e 6f6e 650a  : _range = None.
-000165d0: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
-000165e0: 285f 7261 6e67 6529 203d 3d20 3120 616e  (_range) == 1 an
-000165f0: 6420 6973 696e 7374 616e 6365 285f 7261  d isinstance(_ra
-00016600: 6e67 655b 305d 2c20 286c 6973 742c 2074  nge[0], (list, t
-00016610: 7570 6c65 2929 3a20 5f72 616e 6765 203d  uple)): _range =
-00016620: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
-00016630: 6c69 7374 285f 7261 6e67 655b 305d 2929  list(_range[0]))
-00016640: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
-00016650: 6e28 5f72 616e 6765 2920 3d3d 2031 2061  n(_range) == 1 a
-00016660: 6e64 2069 7369 6e73 7461 6e63 6528 5f72  nd isinstance(_r
-00016670: 616e 6765 5b30 5d2c 2062 742e 5465 6e73  ange[0], bt.Tens
-00016680: 6f72 293a 205f 7261 6e67 6520 3d20 5f72  or): _range = _r
-00016690: 616e 6765 5b30 5d0a 2020 2020 2020 2020  ange[0].        
-000166a0: 656c 6966 206c 656e 285f 7261 6e67 6529  elif len(_range)
-000166b0: 203d 3d20 313a 205f 7261 6e67 6520 3d20   == 1: _range = 
-000166c0: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
-000166d0: 7228 2830 2c20 5f72 616e 6765 2929 0a20  r((0, _range)). 
-000166e0: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
-000166f0: 5f72 616e 6765 2920 3d3d 2032 3a20 5f72  _range) == 2: _r
-00016700: 616e 6765 203d 2062 742e 6368 616e 6e65  ange = bt.channe
-00016710: 6c5f 7465 6e73 6f72 285f 7261 6e67 6529  l_tensor(_range)
-00016720: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
-00016730: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
-00016740: 2249 6e76 616c 6964 2072 616e 6765 2066  "Invalid range f
-00016750: 6f72 204e 6f72 6d61 6c69 7a65 3a20 7b5f  or Normalize: {_
-00016760: 7261 6e67 657d 2e20 2229 0a20 2020 2020  range}. ").     
-00016770: 2020 2069 6620 5f72 616e 6765 2069 7320     if _range is 
-00016780: 4e6f 6e65 3a20 7061 7373 0a20 2020 2020  None: pass.     
-00016790: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000167a0: 2020 2020 2069 6620 5f72 616e 6765 2e6e       if _range.n
-000167b0: 5f64 696d 203c 2032 3a20 5f72 616e 6765  _dim < 2: _range
-000167c0: 203d 205f 7261 6e67 652e 756e 7371 7565   = _range.unsque
-000167d0: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
-000167e0: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
-000167f0: 652e 6861 735f 6261 7463 683a 205f 7261  e.has_batch: _ra
-00016800: 6e67 652e 6261 7463 685f 6469 6d65 6e73  nge.batch_dimens
-00016810: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
-00016820: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
-00016830: 652e 6861 735f 6368 616e 6e65 6c3a 205f  e.has_channel: _
-00016840: 7261 6e67 652e 6368 616e 6e65 6c5f 6469  range.channel_di
-00016850: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
-00016860: 2020 2020 2020 2020 6176 6f75 6368 285f          avouch(_
-00016870: 7261 6e67 652e 6861 735f 6261 7463 6820  range.has_batch 
-00016880: 616e 6420 5f72 616e 6765 2e68 6173 5f63  and _range.has_c
-00016890: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
-000168a0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
-000168b0: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
-000168c0: 2020 2020 2020 2020 2020 2020 2020 285b                ([
-000168d0: 6e5f 6261 7463 683a 6f70 7469 6f6e 616c  n_batch:optional
-000168e0: 5d2c 207b 7b32 7d7d 2920 666f 7220 4e6f  ], {{2}}) for No
-000168f0: 726d 616c 697a 696e 6720 7061 7261 6d65  rmalizing parame
-00016900: 7465 7273 2c20 696e 7374 6561 6420 6f66  ters, instead of
-00016910: 207b 5f72 616e 6765 2e73 6861 7065 7d2e   {_range.shape}.
-00016920: 2022 290a 2020 2020 2020 2020 7375 7065   ").        supe
-00016930: 7228 292e 5f5f 696e 6974 5f5f 285f 7261  r().__init__(_ra
-00016940: 6e67 6529 0a20 2020 2020 2020 2073 656c  nge).        sel
-00016950: 662e 7261 6e67 6520 3d20 5f72 616e 6765  f.range = _range
-00016960: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
-00016970: 616e 6765 203d 204e 6f6e 650a 0a20 2020  ange = None..   
-00016980: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
-00016990: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
-000169a0: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
-000169b0: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
-000169c0: 5f72 616e 6765 203d 2073 656c 662e 7261  _range = self.ra
-000169d0: 6e67 650a 2020 2020 2020 2020 6966 205f  nge.        if _
-000169e0: 7261 6e67 6520 6973 204e 6f6e 653a 0a20  range is None:. 
-000169f0: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
-00016a00: 6520 3d20 6274 2e71 7561 6e74 696c 6528  e = bt.quantile(
-00016a10: 582e 666c 6174 7465 6e28 292e 666c 6f61  X.flatten().floa
-00016a20: 7428 292c 2062 6174 6f72 6368 5f74 656e  t(), batorch_ten
-00016a30: 736f 7228 5b30 2e30 3235 2c20 302e 3937  sor([0.025, 0.97
-00016a40: 355d 292c 2061 7869 733d 2d31 292e 6d6f  5]), axis=-1).mo
-00016a50: 7665 6469 6d28 302c 202d 3129 2e73 7065  vedim(0, -1).spe
-00016a60: 6369 616c 5f66 726f 6d5f 2858 290a 2020  cial_from_(X).  
-00016a70: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00016a80: 7261 6e67 6520 3d20 5f72 616e 6765 0a20  range = _range. 
-00016a90: 2020 2020 2020 2072 6574 7572 6e20 2828         return ((
-00016aa0: 5820 2d20 5f72 616e 6765 5b2e 2e2e 2c20  X - _range[..., 
-00016ab0: 305d 2920 2f20 285f 7261 6e67 655b 2e2e  0]) / (_range[..
-00016ac0: 2e2c 2031 5d20 2d20 5f72 616e 6765 5b2e  ., 1] - _range[.
-00016ad0: 2e2e 2c20 305d 2929 2e63 6c61 6d70 2830  .., 0])).clamp(0
-00016ae0: 2e2c 2031 2e29 0a20 2020 200a 2020 2020  ., 1.).    .    
-00016af0: 6465 6620 696e 7628 7365 6c66 293a 0a20  def inv(self):. 
-00016b00: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00016b10: 616e 6765 2069 7320 6e6f 7420 4e6f 6e65  ange is not None
-00016b20: 3a20 5f72 616e 6765 203d 2073 656c 662e  : _range = self.
-00016b30: 7261 6e67 650a 2020 2020 2020 2020 656c  range.        el
-00016b40: 6966 2073 656c 662e 5f72 616e 6765 2069  if self._range i
-00016b50: 7320 6e6f 7420 4e6f 6e65 3a20 5f72 616e  s not None: _ran
-00016b60: 6765 203d 2073 656c 662e 5f72 616e 6765  ge = self._range
-00016b70: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
-00016b80: 6574 7572 6e20 4e6f 726d 616c 697a 6528  eturn Normalize(
-00016b90: 4e6f 6e65 290a 2020 2020 2020 2020 6465  None).        de
-00016ba0: 6e20 3d20 5f72 616e 6765 5b2e 2e2e 2c20  n = _range[..., 
-00016bb0: 315d 202d 205f 7261 6e67 655b 2e2e 2e2c  1] - _range[...,
-00016bc0: 2030 5d0a 2020 2020 2020 2020 5f72 616e   0].        _ran
-00016bd0: 6765 203d 2062 742e 7374 6163 6b28 2d5f  ge = bt.stack(-_
-00016be0: 7261 6e67 655b 2e2e 2e2c 2030 5d2c 2031  range[..., 0], 1
-00016bf0: 2d5f 7261 6e67 655b 2e2e 2e2c 2030 5d2c  -_range[..., 0],
-00016c00: 202d 3129 202f 2064 656e 0a20 2020 2020   -1) / den.     
-00016c10: 2020 2072 6574 7572 6e20 4e6f 726d 616c     return Normal
-00016c20: 697a 6528 5f72 616e 6765 290a 0a23 2323  ize(_range)..###
-00016c30: 2323 2323 2323 2323 2323 2053 7570 706f  ########## Suppo
-00016c40: 7274 696e 6720 4675 6e63 7469 6f6e 7320  rting Functions 
-00016c50: 2323 2323 2323 2323 2323 2323 0a0a 6465  ############..de
-00016c60: 6620 4273 706c 696e 6528 692c 2055 293a  f Bspline(i, U):
-00016c70: 0a20 2020 2022 2222 0a20 2020 2043 7562  .    """.    Cub
-00016c80: 6963 2042 2d73 706c 696e 6520 6675 6e63  ic B-spline func
-00016c90: 7469 6f6e 2e20 0a20 2020 204e 6f74 653a  tion. .    Note:
-00016ca0: 2041 7320 6c6f 6e67 2061 7320 6920 616e   As long as i an
-00016cb0: 6420 5520 6861 7665 2074 6865 2073 616d  d U have the sam
-00016cc0: 6520 7369 7a65 2c20 616e 7920 7368 6170  e size, any shap
-00016cd0: 6520 6f66 2074 656e 736f 7273 2077 6f75  e of tensors wou
-00016ce0: 6c64 2064 6f2e 0a20 2020 200a 2020 2020  ld do..    .    
-00016cf0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
-00016d00: 6920 5b62 742e 5465 6e73 6f72 5d3a 2074  i [bt.Tensor]: t
-00016d10: 6865 2069 6e64 6578 206f 6620 7365 676d  he index of segm
-00016d20: 656e 7420 6675 6e63 7469 6f6e 206f 6620  ent function of 
-00016d30: 422d 7370 6c69 6e65 2e0a 2020 2020 2020  B-spline..      
-00016d40: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
-00016d50: 6f66 2065 6163 6820 656c 656d 656e 7420  of each element 
-00016d60: 6361 6e20 6265 2063 686f 7365 6e20 696e  can be chosen in
-00016d70: 2028 2d31 2c20 302c 2031 2c20 3229 2e20   (-1, 0, 1, 2). 
-00016d80: 0a20 2020 2020 2020 2055 205b 6274 2e54  .        U [bt.T
-00016d90: 656e 736f 725d 3a20 7468 6520 6465 6369  ensor]: the deci
-00016da0: 6d61 6c20 6172 6775 6d65 6e74 206f 6620  mal argument of 
-00016db0: 422d 7370 6c69 6e65 2066 756e 6374 696f  B-spline functio
-00016dc0: 6e2e 2049 7420 7368 6f75 6c64 2062 6520  n. It should be 
-00016dd0: 7769 7468 696e 2072 616e 6765 205b 302c  within range [0,
-00016de0: 2031 292e 0a20 2020 2022 2222 0a20 2020   1)..    """.   
-00016df0: 2069 203d 2062 6174 6f72 6368 5f74 656e   i = batorch_ten
-00016e00: 736f 7228 6929 3b20 5520 3d20 6261 746f  sor(i); U = bato
-00016e10: 7263 685f 7465 6e73 6f72 2855 290a 2020  rch_tensor(U).  
-00016e20: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-00016e30: 2020 2062 742e 7768 6572 6528 6920 3d3d     bt.where(i ==
-00016e40: 202d 312c 2028 3120 2d20 5529 202a 2a20   -1, (1 - U) ** 
-00016e50: 3320 2f20 362c 0a20 2020 2020 2020 2062  3 / 6,.        b
-00016e60: 742e 7768 6572 6528 6920 3d3d 2030 2c20  t.where(i == 0, 
-00016e70: 5520 2a2a 2033 202f 2032 202d 2055 202a  U ** 3 / 2 - U *
-00016e80: 2055 202b 2032 202f 2033 2c0a 2020 2020   U + 2 / 3,.    
-00016e90: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
-00016ea0: 3d20 312c 2028 2d20 3320 2a20 5520 2a2a  = 1, (- 3 * U **
-00016eb0: 2033 202b 2033 202a 2055 202a 2055 202b   3 + 3 * U * U +
-00016ec0: 2033 202a 2055 202b 2031 2920 2f20 362c   3 * U + 1) / 6,
-00016ed0: 0a20 2020 2020 2020 2062 742e 7768 6572  .        bt.wher
-00016ee0: 6528 6920 3d3d 2032 2c20 5520 2a2a 2033  e(i == 2, U ** 3
-00016ef0: 202f 2036 2c0a 2020 2020 2020 2020 6274   / 6,.        bt
-00016f00: 2e7a 6572 6f73 5f6c 696b 6528 5529 2929  .zeros_like(U)))
-00016f10: 2929 0a20 2020 2029 0a0a 6465 6620 6442  )).    )..def dB
-00016f20: 7370 6c69 6e65 2869 2c20 5529 3a0a 2020  spline(i, U):.  
-00016f30: 2020 2222 220a 2020 2020 5468 6520 6465    """.    The de
-00016f40: 7269 7661 7469 7665 206f 6620 422d 7370  rivative of B-sp
-00016f50: 6c69 6e65 2066 756e 6374 696f 6e2c 2077  line function, w
-00016f60: 6974 6820 7265 7370 6563 7420 746f 2055  ith respect to U
-00016f70: 2e20 0a20 2020 204e 6f74 653a 2041 7320  . .    Note: As 
-00016f80: 6c6f 6e67 2061 7320 6920 616e 6420 5520  long as i and U 
-00016f90: 6861 7665 2074 6865 2073 616d 6520 7369  have the same si
-00016fa0: 7a65 2c20 616e 7920 7368 6170 6520 6f66  ze, any shape of
-00016fb0: 2074 656e 736f 7273 2077 6f75 6c64 2064   tensors would d
-00016fc0: 6f2e 0a20 2020 200a 2020 2020 5061 7261  o..    .    Para
-00016fd0: 6d73 3a0a 2020 2020 2020 2020 6920 5b62  ms:.        i [b
-00016fe0: 742e 5465 6e73 6f72 5d3a 2074 6865 2069  t.Tensor]: the i
-00016ff0: 6e64 6578 206f 6620 7365 676d 656e 7420  ndex of segment 
-00017000: 6675 6e63 7469 6f6e 206f 6620 422d 7370  function of B-sp
-00017010: 6c69 6e65 2e0a 2020 2020 2020 2020 2020  line..          
-00017020: 2020 5468 6520 7661 6c75 6520 6f66 2065    The value of e
-00017030: 6163 6820 656c 656d 656e 7420 6361 6e20  ach element can 
-00017040: 6265 2063 686f 7365 6e20 696e 2028 2d31  be chosen in (-1
-00017050: 2c20 302c 2031 2c20 3229 2e20 0a20 2020  , 0, 1, 2). .   
-00017060: 2020 2020 2055 205b 6274 2e54 656e 736f       U [bt.Tenso
-00017070: 725d 3a20 7468 6520 6465 6369 6d61 6c20  r]: the decimal 
-00017080: 6172 6775 6d65 6e74 206f 6620 422d 7370  argument of B-sp
-00017090: 6c69 6e65 2066 756e 6374 696f 6e2e 2049  line function. I
-000170a0: 7420 7368 6f75 6c64 2062 6520 7769 7468  t should be with
-000170b0: 696e 2072 616e 6765 205b 302c 2031 292e  in range [0, 1).
-000170c0: 0a20 2020 2022 2222 0a20 2020 2069 203d  .    """.    i =
-000170d0: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
-000170e0: 6929 3b20 5520 3d20 6261 746f 7263 685f  i); U = batorch_
-000170f0: 7465 6e73 6f72 2855 290a 2020 2020 7265  tensor(U).    re
-00017100: 7475 726e 2028 0a20 2020 2020 2020 2062  turn (.        b
-00017110: 742e 7768 6572 6528 6920 3d3d 202d 312c  t.where(i == -1,
-00017120: 202d 2033 202a 2028 3120 2d20 5529 202a   - 3 * (1 - U) *
-00017130: 2a20 3220 2f20 362c 0a20 2020 2020 2020  * 2 / 6,.       
-00017140: 2062 742e 7768 6572 6528 6920 3d3d 2030   bt.where(i == 0
-00017150: 2c20 3320 2a20 5520 2a2a 2032 202f 2032  , 3 * U ** 2 / 2
-00017160: 202d 2032 202a 2055 2c0a 2020 2020 2020   - 2 * U,.      
-00017170: 2020 6274 2e77 6865 7265 2869 203d 3d20    bt.where(i == 
-00017180: 312c 2028 2d20 3320 2a20 5520 2a2a 2032  1, (- 3 * U ** 2
-00017190: 202b 2032 202a 2055 202b 2031 2920 2f20   + 2 * U + 1) / 
-000171a0: 322c 0a20 2020 2020 2020 2062 742e 7768  2,.        bt.wh
-000171b0: 6572 6528 6920 3d3d 2032 2c20 3320 2a20  ere(i == 2, 3 * 
-000171c0: 5520 2a2a 2032 202f 2036 2c0a 2020 2020  U ** 2 / 6,.    
-000171d0: 2020 2020 6274 2e7a 6572 6f73 5f6c 696b      bt.zeros_lik
-000171e0: 6528 5529 2929 2929 0a20 2020 2029 0a0a  e(U))))).    )..
-000171f0: 6465 6620 6642 7370 6c69 6e65 2863 2c20  def fBspline(c, 
-00017200: 7829 3a0a 2020 2020 6320 3d20 6261 746f  x):.    c = bato
-00017210: 7263 685f 7465 6e73 6f72 2863 293b 2078  rch_tensor(c); x
-00017220: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-00017230: 7228 7829 0a20 2020 2064 203d 2078 202d  r(x).    d = x -
-00017240: 2063 0a20 2020 2072 6574 7572 6e20 280a   c.    return (.
-00017250: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
-00017260: 2828 2d32 203c 3d20 6429 202a 2028 6420  ((-2 <= d) * (d 
-00017270: 3c20 2d31 292c 2064 202a 2a20 3320 2b20  < -1), d ** 3 + 
-00017280: 3620 2a20 6420 2a2a 2032 202b 2031 3220  6 * d ** 2 + 12 
-00017290: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
-000172a0: 2062 742e 7768 6572 6528 282d 3120 3c3d   bt.where((-1 <=
-000172b0: 2064 2920 2a20 2864 203c 2030 292c 202d   d) * (d < 0), -
-000172c0: 2033 202a 2064 202a 2a20 3320 2d20 3620   3 * d ** 3 - 6 
-000172d0: 2a20 6420 2a2a 2032 202b 2034 2c0a 2020  * d ** 2 + 4,.  
-000172e0: 2020 2020 2020 6274 2e77 6865 7265 2828        bt.where((
-000172f0: 3020 3c3d 2064 2920 2a20 2864 203c 2031  0 <= d) * (d < 1
-00017300: 292c 2033 202a 2064 202a 2a20 3320 2d20  ), 3 * d ** 3 - 
-00017310: 3620 2a20 6420 2a2a 2032 202b 2034 2c0a  6 * d ** 2 + 4,.
-00017320: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
-00017330: 2828 3120 3c3d 2064 2920 2a20 2864 203c  ((1 <= d) * (d <
-00017340: 2032 292c 202d 2064 202a 2a20 3320 2b20   2), - d ** 3 + 
-00017350: 3620 2a20 6420 2a2a 2032 202d 2031 3220  6 * d ** 2 - 12 
-00017360: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
-00017370: 2062 742e 7a65 726f 735f 6c69 6b65 2864   bt.zeros_like(d
-00017380: 2929 2929 2920 2f20 360a 2020 2020 290a  ))))) / 6.    ).
-00017390: 0a64 6566 2041 6666 696e 6532 4432 4d61  .def Affine2D2Ma
-000173a0: 7472 6978 2870 6172 616d 7329 3a0a 2020  trix(params):.  
-000173b0: 2020 2222 220a 2020 2020 7431 2c20 7432    """.    t1, t2
-000173c0: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
-000173d0: 312c 20cf 8132 2069 6e20 7369 7a65 3a20  1, ..2 in size: 
-000173e0: 285b 6e5f 6261 7463 685d 2c20 7b37 7d29  ([n_batch], {7})
-000173f0: 0a20 2020 2074 312c 2074 322c 2063 312c  .    t1, t2, c1,
-00017400: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
-00017410: 20cf 8131 2c20 cf81 3220 696e 2073 697a   ..1, ..2 in siz
-00017420: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
-00017430: 397d 290a 2020 2020 6f75 7470 7574 2069  9}).    output i
-00017440: 6e20 7369 7a65 3a20 285b 6e5f 6261 7463  n size: ([n_batc
-00017450: 685d 2c20 332c 2033 290a 2020 2020 2222  h], 3, 3).    ""
-00017460: 220a 2020 2020 7061 7261 6d73 203d 2062  ".    params = b
-00017470: 6174 6f72 6368 5f74 656e 736f 7228 7061  atorch_tensor(pa
-00017480: 7261 6d73 290a 2020 2020 6966 2070 6172  rams).    if par
-00017490: 616d 732e 6e5f 6469 6d20 3c3d 2031 2061  ams.n_dim <= 1 a
-000174a0: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
-000174b0: 735f 6261 7463 683a 2070 6172 616d 7320  s_batch: params 
-000174c0: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
-000174d0: 7a65 285b 5d29 0a20 2020 2069 6620 7061  ze([]).    if pa
-000174e0: 7261 6d73 2e6e 5f64 696d 203c 3d20 3120  rams.n_dim <= 1 
-000174f0: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
-00017500: 6173 5f63 6861 6e6e 656c 3a20 7061 7261  as_channel: para
-00017510: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
-00017520: 7565 657a 6528 7b31 7d29 0a20 2020 2069  ueeze({1}).    i
-00017530: 6620 7061 7261 6d73 2e6e 5f64 696d 203d  f params.n_dim =
-00017540: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
-00017550: 6d73 2e68 6173 5f62 6174 6368 3a20 7061  ms.has_batch: pa
-00017560: 7261 6d73 2e62 6174 6368 5f64 696d 656e  rams.batch_dimen
-00017570: 7369 6f6e 203d 2030 0a20 2020 2069 6620  sion = 0.    if 
-00017580: 7061 7261 6d73 2e6e 5f64 696d 203d 3d20  params.n_dim == 
-00017590: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
-000175a0: 2e68 6173 5f63 6861 6e6e 656c 3a20 7061  .has_channel: pa
-000175b0: 7261 6d73 2e63 6861 6e6e 656c 5f64 696d  rams.channel_dim
-000175c0: 656e 7369 6f6e 203d 2031 0a20 2020 2061  ension = 1.    a
-000175d0: 766f 7563 6828 7061 7261 6d73 2e68 6173  vouch(params.has
-000175e0: 5f62 6174 6368 2c20 6622 506c 6561 7365  _batch, f"Please
-000175f0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
-00017600: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
-00017610: 6261 7463 685d 2c20 7b37 206f 7220 397d  batch], {7 or 9}
-00017620: 2920 5c0a 2020 2020 2020 2020 666f 7220  ) \.        for 
-00017630: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
-00017640: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
-00017650: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
-00017660: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
-00017670: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
-00017680: 2020 6966 2070 6172 616d 732e 7369 7a65    if params.size
-00017690: 2831 2920 3d3d 2037 3a0a 2020 2020 2020  (1) == 7:.      
-000176a0: 2020 7431 2c20 7432 2c20 ceb8 2c20 7331    t1, t2, .., s1
-000176b0: 2c20 7332 2c20 cf81 312c 20cf 8132 203d  , s2, ..1, ..2 =
-000176c0: 2070 6172 616d 732e 7370 6c69 7428 290a   params.split().
-000176d0: 2020 2020 2020 2020 6331 203d 2062 742e          c1 = bt.
-000176e0: 7a65 726f 7328 5b6e 5f62 6174 6368 5d2c  zeros([n_batch],
-000176f0: 2031 293b 2063 3220 3d20 6274 2e7a 6572   1); c2 = bt.zer
-00017700: 6f73 285b 6e5f 6261 7463 685d 2c20 3129  os([n_batch], 1)
-00017710: 0a20 2020 2069 6620 7061 7261 6d73 2e73  .    if params.s
-00017720: 697a 6528 3129 203d 3d20 393a 0a20 2020  ize(1) == 9:.   
-00017730: 2020 2020 2074 312c 2074 322c 2063 312c       t1, t2, c1,
-00017740: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
-00017750: 20cf 8131 2c20 cf81 3220 3d20 7061 7261   ..1, ..2 = para
-00017760: 6d73 2e73 706c 6974 2829 0a20 2020 2061  ms.split().    a
-00017770: 203d 2028 cf81 3120 2a20 cf81 3220 2b20   = (..1 * ..2 + 
-00017780: 3129 202a 2073 3120 2a20 6274 2e63 6f73  1) * s1 * bt.cos
-00017790: 28ce b829 202b 20cf 8131 202a 2073 3220  (..) + ..1 * s2 
-000177a0: 2a20 6274 2e73 696e 28ce b829 0a20 2020  * bt.sin(..).   
-000177b0: 2062 203d 202d 2028 cf81 3120 2a20 cf81   b = - (..1 * ..
-000177c0: 3220 2b20 3129 202a 2073 3120 2a20 6274  2 + 1) * s1 * bt
-000177d0: 2e73 696e 28ce b829 202b 20cf 8131 202a  .sin(..) + ..1 *
-000177e0: 2073 3220 2a20 6274 2e63 6f73 28ce b829   s2 * bt.cos(..)
-000177f0: 0a20 2020 2063 203d 20cf 8132 202a 2073  .    c = ..2 * s
-00017800: 3120 2a20 6274 2e63 6f73 28ce b829 202b  1 * bt.cos(..) +
-00017810: 2073 3220 2a20 6274 2e73 696e 28ce b829   s2 * bt.sin(..)
-00017820: 0a20 2020 2064 203d 202d 20cf 8132 202a  .    d = - ..2 *
-00017830: 2073 3120 2a20 6274 2e73 696e 28ce b829   s1 * bt.sin(..)
-00017840: 202b 2073 3220 2a20 6274 2e63 6f73 28ce   + s2 * bt.cos(.
-00017850: b829 0a20 2020 2072 6574 7572 6e20 6274  .).    return bt
-00017860: 2e63 6174 280a 2020 2020 2020 2020 6274  .cat(.        bt
-00017870: 2e63 6174 2828 612c 2062 2c20 7431 202d  .cat((a, b, t1 -
-00017880: 2061 202a 2063 3120 2d20 6220 2a20 6332   a * c1 - b * c2
-00017890: 202b 2063 312c 2063 2c20 642c 2074 3220   + c1, c, d, t2 
-000178a0: 2d20 6320 2a20 6331 202d 2064 202a 2063  - c * c1 - d * c
-000178b0: 3220 2b20 6332 292c 207b 7d29 2e76 6965  2 + c2), {}).vie
-000178c0: 7728 5b6e 5f62 6174 6368 5d2c 2032 2c20  w([n_batch], 2, 
-000178d0: 3329 2c20 0a20 2020 2020 2020 2062 742e  3), .        bt.
-000178e0: 6f6e 655f 686f 7428 2d31 2c20 3329 2e6d  one_hot(-1, 3).m
-000178f0: 756c 7469 706c 7928 6e5f 6261 7463 682c  ultiply(n_batch,
-00017900: 205b 5d29 2e76 6965 7728 5b6e 5f62 6174   []).view([n_bat
-00017910: 6368 5d2c 2031 2c20 3329 2c20 310a 2020  ch], 1, 3), 1.  
-00017920: 2020 290a 0a64 6566 2051 7561 7465 726e    )..def Quatern
-00017930: 7332 4d61 7472 6978 2870 6172 616d 7329  s2Matrix(params)
-00017940: 3a0a 2020 2020 2222 220a 2020 2020 2020  :.    """.      
-00017950: 2020 5175 6174 6572 6e3a 2071 622c 2071    Quatern: qb, q
-00017960: 632c 2071 642c 2070 782c 2070 792c 2070  c, qd, px, py, p
-00017970: 7a20 696e 2073 697a 653a 2028 5b6e 5f62  z in size: ([n_b
-00017980: 6174 6368 5d2c 207b 367d 290a 2020 2020  atch], {6}).    
-00017990: 2020 2020 4d61 7472 6978 3a20 285b 6e5f      Matrix: ([n_
-000179a0: 6261 7463 685d 2c20 342c 2034 290a 2020  batch], 4, 4).  
-000179b0: 2020 2222 220a 2020 2020 7061 7261 6d73    """.    params
-000179c0: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
-000179d0: 7228 7061 7261 6d73 290a 2020 2020 6966  r(params).    if
-000179e0: 2070 6172 616d 732e 6e5f 6469 6d20 3c3d   params.n_dim <=
-000179f0: 2031 2061 6e64 206e 6f74 2070 6172 616d   1 and not param
-00017a00: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
-00017a10: 616d 7320 3d20 7061 7261 6d73 2e75 6e73  ams = params.uns
-00017a20: 7175 6565 7a65 285b 5d29 0a20 2020 2069  queeze([]).    i
-00017a30: 6620 7061 7261 6d73 2e6e 5f64 696d 203c  f params.n_dim <
-00017a40: 3d20 3120 616e 6420 6e6f 7420 7061 7261  = 1 and not para
-00017a50: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
-00017a60: 7061 7261 6d73 203d 2070 6172 616d 732e  params = params.
-00017a70: 756e 7371 7565 657a 6528 7b31 7d29 0a20  unsqueeze({1}). 
-00017a80: 2020 2069 6620 7061 7261 6d73 2e6e 5f64     if params.n_d
-00017a90: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
-00017aa0: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
-00017ab0: 3a20 7061 7261 6d73 2e62 6174 6368 5f64  : params.batch_d
-00017ac0: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
-00017ad0: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
-00017ae0: 203d 3d20 3220 616e 6420 6e6f 7420 7061   == 2 and not pa
-00017af0: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
-00017b00: 3a20 7061 7261 6d73 2e63 6861 6e6e 656c  : params.channel
-00017b10: 5f64 696d 656e 7369 6f6e 203d 2031 0a20  _dimension = 1. 
-00017b20: 2020 2061 766f 7563 6828 7061 7261 6d73     avouch(params
-00017b30: 2e6e 5f64 696d 203d 3d20 3220 616e 6420  .n_dim == 2 and 
-00017b40: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
-00017b50: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
-00017b60: 6368 616e 6e65 6c2c 200a 2020 2020 2020  channel, .      
-00017b70: 2020 2020 2066 2250 6c65 6173 6520 7573       f"Please us
-00017b80: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
-00017b90: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
-00017ba0: 6368 5d2c 207b 7b36 7d7d 2920 666f 7220  ch], {{6}}) for 
-00017bb0: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
-00017bc0: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
-00017bd0: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
-00017be0: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
-00017bf0: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
-00017c00: 2020 622c 2063 2c20 642c 2078 2c20 792c    b, c, d, x, y,
-00017c10: 207a 203d 2070 6172 616d 732e 7370 6c69   z = params.spli
-00017c20: 7428 290a 2020 2020 6120 3d20 6274 2e73  t().    a = bt.s
-00017c30: 7172 7428 2831 2d62 2a62 2d63 2a63 2d64  qrt((1-b*b-c*c-d
-00017c40: 2a64 292e 636c 616d 7028 3029 290a 2020  *d).clamp(0)).  
-00017c50: 2020 5231 3120 3d20 612a 612b 622a 622d    R11 = a*a+b*b-
-00017c60: 632a 632d 642a 640a 2020 2020 5231 3220  c*c-d*d.    R12 
-00017c70: 3d20 322a 622a 632d 322a 612a 640a 2020  = 2*b*c-2*a*d.  
-00017c80: 2020 5231 3320 3d20 322a 622a 642b 322a    R13 = 2*b*d+2*
-00017c90: 612a 630a 2020 2020 5232 3120 3d20 322a  a*c.    R21 = 2*
-00017ca0: 622a 632b 322a 612a 640a 2020 2020 5232  b*c+2*a*d.    R2
-00017cb0: 3220 3d20 612a 612b 632a 632d 622a 622d  2 = a*a+c*c-b*b-
-00017cc0: 642a 640a 2020 2020 5232 3320 3d20 322a  d*d.    R23 = 2*
-00017cd0: 632a 642d 322a 612a 620a 2020 2020 5233  c*d-2*a*b.    R3
-00017ce0: 3120 3d20 322a 622a 642d 322a 612a 630a  1 = 2*b*d-2*a*c.
-00017cf0: 2020 2020 5233 3220 3d20 322a 632a 642b      R32 = 2*c*d+
-00017d00: 322a 612a 620a 2020 2020 5233 3320 3d20  2*a*b.    R33 = 
-00017d10: 612a 612b 642a 642d 632a 632d 622a 620a  a*a+d*d-c*c-b*b.
-00017d20: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
-00017d30: 7428 0a20 2020 2020 2020 2062 742e 6361  t(.        bt.ca
-00017d40: 7428 2852 3131 2c20 5231 322c 2052 3133  t((R11, R12, R13
-00017d50: 2c20 782c 2052 3231 2c20 5232 322c 2052  , x, R21, R22, R
-00017d60: 3233 2c20 792c 2052 3331 2c20 5233 322c  23, y, R31, R32,
-00017d70: 2052 3333 2c20 7a29 2c20 3129 2e76 6965   R33, z), 1).vie
-00017d80: 7728 5b6e 5f62 6174 6368 5d2c 2033 2c20  w([n_batch], 3, 
-00017d90: 3429 2c0a 2020 2020 2020 2020 6274 2e6f  4),.        bt.o
-00017da0: 6e65 5f68 6f74 282d 312c 2034 292e 6d75  ne_hot(-1, 4).mu
-00017db0: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
-00017dc0: 5b5d 292e 7669 6577 285b 6e5f 6261 7463  []).view([n_batc
-00017dd0: 685d 2c20 312c 2034 292c 2031 0a20 2020  h], 1, 4), 1.   
-00017de0: 2029 0a0a 6465 6620 4d61 7472 6978 3251   )..def Matrix2Q
-00017df0: 7561 7465 726e 7328 7061 7261 6d73 293a  uaterns(params):
-00017e00: 0a20 2020 2022 2222 0a20 2020 2020 2020  .    """.       
-00017e10: 204d 6174 7269 783a 2028 5b6e 5f62 6174   Matrix: ([n_bat
-00017e20: 6368 5d2c 2034 2c20 3429 0a20 2020 2020  ch], 4, 4).     
-00017e30: 2020 2051 7561 7465 726e 3a20 7162 2c20     Quatern: qb, 
-00017e40: 7163 2c20 7164 2c20 7078 2c20 7079 2c20  qc, qd, px, py, 
-00017e50: 707a 2069 6e20 7369 7a65 3a20 285b 6e5f  pz in size: ([n_
-00017e60: 6261 7463 685d 2c20 7b36 7d29 0a20 2020  batch], {6}).   
-00017e70: 2022 2222 0a20 2020 2070 6172 616d 7320   """.    params 
-00017e80: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
-00017e90: 2870 6172 616d 7329 0a20 2020 2069 6620  (params).    if 
-00017ea0: 7061 7261 6d73 2e6e 5f64 696d 203c 3d20  params.n_dim <= 
-00017eb0: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
-00017ec0: 2e68 6173 5f62 6174 6368 3a20 7061 7261  .has_batch: para
-00017ed0: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
-00017ee0: 7565 657a 6528 5b5d 290a 2020 2020 6966  ueeze([]).    if
-00017ef0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
-00017f00: 2033 2061 6e64 206e 6f74 2070 6172 616d   3 and not param
-00017f10: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
-00017f20: 616d 732e 6261 7463 685f 6469 6d65 6e73  ams.batch_dimens
-00017f30: 696f 6e20 3d20 300a 2020 2020 6966 2070  ion = 0.    if p
-00017f40: 6172 616d 732e 6e5f 6469 6d20 3d3d 2033  arams.n_dim == 3
-00017f50: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
-00017f60: 6368 616e 6e65 6c3a 2070 6172 616d 732e  channel: params.
-00017f70: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
-00017f80: 6e20 3d20 4e6f 6e65 0a20 2020 2061 766f  n = None.    avo
-00017f90: 7563 6828 7061 7261 6d73 2e6e 5f64 696d  uch(params.n_dim
-00017fa0: 203d 3d20 3320 616e 6420 7061 7261 6d73   == 3 and params
-00017fb0: 2e68 6173 5f62 6174 6368 2061 6e64 206e  .has_batch and n
-00017fc0: 6f74 2070 6172 616d 732e 6861 735f 6368  ot params.has_ch
-00017fd0: 616e 6e65 6c2c 200a 2020 2020 2020 2020  annel, .        
-00017fe0: 2020 2066 2250 6c65 6173 6520 7573 6520     f"Please use 
-00017ff0: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
-00018000: 6620 7369 7a65 2028 5b6e 5f62 6174 6368  f size ([n_batch
-00018010: 5d2c 2034 2c20 3429 2066 6f72 2041 6666  ], 4, 4) for Aff
-00018020: 696e 6520 6d61 7472 6978 2c20 696e 7374  ine matrix, inst
-00018030: 6561 6420 6f66 207b 7061 7261 6d73 2e73  ead of {params.s
-00018040: 6861 7065 7d2e 2022 290a 2020 2020 6e5f  hape}. ").    n_
-00018050: 6261 7463 6820 3d20 7061 7261 6d73 2e6e  batch = params.n
-00018060: 5f62 6174 6368 0a20 2020 2078 2c20 792c  _batch.    x, y,
-00018070: 207a 203d 2070 6172 616d 735b 2e2e 2e2c   z = params[...,
-00018080: 203a 332c 202d 315d 2e63 6861 6e6e 656c   :3, -1].channel
-00018090: 5f64 696d 5f28 3129 2e73 706c 6974 2831  _dim_(1).split(1
-000180a0: 2c20 3129 0a20 2020 2061 3220 3d20 2862  , 1).    a2 = (b
-000180b0: 742e 6469 6167 2870 6172 616d 7329 2e73  t.diag(params).s
-000180c0: 756d 2829 2e75 6e73 7175 6565 7a65 287b  um().unsqueeze({
-000180d0: 7d29 202b 2031 2920 2f20 340a 2020 2020  }) + 1) / 4.    
-000180e0: 6120 3d20 6274 2e73 7172 7428 6132 290a  a = bt.sqrt(a2).
-000180f0: 2020 2020 6232 203d 2061 3220 2d20 2870      b2 = a2 - (p
-00018100: 6172 616d 735b 2e2e 2e2c 2031 2c20 315d  arams[..., 1, 1]
-00018110: 202b 2070 6172 616d 735b 2e2e 2e2c 2032   + params[..., 2
-00018120: 2c20 325d 2920 2f20 320a 2020 2020 6332  , 2]) / 2.    c2
-00018130: 203d 2061 3220 2d20 2870 6172 616d 735b   = a2 - (params[
-00018140: 2e2e 2e2c 2032 2c20 325d 202b 2070 6172  ..., 2, 2] + par
-00018150: 616d 735b 2e2e 2e2c 2030 2c20 305d 2920  ams[..., 0, 0]) 
-00018160: 2f20 320a 2020 2020 6432 203d 2061 3220  / 2.    d2 = a2 
-00018170: 2d20 2870 6172 616d 735b 2e2e 2e2c 2030  - (params[..., 0
-00018180: 2c20 305d 202b 2070 6172 616d 735b 2e2e  , 0] + params[..
-00018190: 2e2c 2031 2c20 315d 2920 2f20 320a 2020  ., 1, 1]) / 2.  
-000181a0: 2020 4420 3d20 7061 7261 6d73 202d 2070    D = params - p
-000181b0: 6172 616d 732e 540a 2020 2020 6220 3d20  arams.T.    b = 
-000181c0: 6274 2e73 6967 6e28 445b 2e2e 2e2c 2032  bt.sign(D[..., 2
-000181d0: 2c20 315d 2920 2a20 6274 2e73 7172 7428  , 1]) * bt.sqrt(
-000181e0: 6232 290a 2020 2020 6320 3d20 2d20 6274  b2).    c = - bt
-000181f0: 2e73 6967 6e28 445b 2e2e 2e2c 2032 2c20  .sign(D[..., 2, 
-00018200: 305d 2920 2a20 6274 2e73 7172 7428 6332  0]) * bt.sqrt(c2
-00018210: 290a 2020 2020 6420 3d20 6274 2e73 6967  ).    d = bt.sig
-00018220: 6e28 445b 2e2e 2e2c 2031 2c20 305d 2920  n(D[..., 1, 0]) 
-00018230: 2a20 6274 2e73 7172 7428 6432 290a 2020  * bt.sqrt(d2).  
-00018240: 2020 7265 7475 726e 2062 742e 6361 7428    return bt.cat(
-00018250: 622c 2063 2c20 642c 2078 2c20 792c 207a  b, c, d, x, y, z
-00018260: 2c20 7b7d 290a                           , {}).
+00006ed0: 206e 5f64 696d 2069 7320 4e6f 6e65 2061   n_dim is None a
+00006ee0: 6e64 2073 656c 662e 6e5f 6469 6d20 6973  nd self.n_dim is
+00006ef0: 204e 6f6e 653a 2072 6574 7572 6e0a 2020   None: return.  
+00006f00: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
+00006f10: 7320 4e6f 6e65 3a20 6e5f 6469 6d20 3d20  s None: n_dim = 
+00006f20: 7365 6c66 2e6e 5f64 696d 0a20 2020 2020  self.n_dim.     
+00006f30: 2020 2061 766f 7563 6828 7365 6c66 2e6e     avouch(self.n
+00006f40: 5f64 696d 2069 7320 4e6f 6e65 206f 7220  _dim is None or 
+00006f50: 7365 6c66 2e6e 5f64 696d 203d 3d20 6e5f  self.n_dim == n_
+00006f60: 6469 6d29 0a20 2020 2020 2020 2064 696d  dim).        dim
+00006f70: 312c 2064 696d 3220 3d20 7365 6c66 2e64  1, dim2 = self.d
+00006f80: 696d 312c 2073 656c 662e 6469 6d32 0a20  im1, self.dim2. 
+00006f90: 2020 2020 2020 2061 6666 203d 2062 742e         aff = bt.
+00006fa0: 6579 6528 6e5f 6469 6d20 2b20 3129 0a20  eye(n_dim + 1). 
+00006fb0: 2020 2020 2020 2061 6666 5b64 696d 315d         aff[dim1]
+00006fc0: 5b64 696d 315d 203d 2030 2e0a 2020 2020  [dim1] = 0..    
+00006fd0: 2020 2020 6166 665b 6469 6d31 5d5b 6469      aff[dim1][di
+00006fe0: 6d32 5d20 3d20 312e 0a20 2020 2020 2020  m2] = 1..       
+00006ff0: 2061 6666 5b64 696d 325d 5b64 696d 325d   aff[dim2][dim2]
+00007000: 203d 2030 2e0a 2020 2020 2020 2020 6166   = 0..        af
+00007010: 665b 6469 6d32 5d5b 6469 6d31 5d20 3d20  f[dim2][dim1] = 
+00007020: 2d31 2e0a 2020 2020 2020 2020 6166 665b  -1..        aff[
+00007030: 6469 6d32 5d5b 2d31 5d20 3d20 666c 6f61  dim2][-1] = floa
+00007040: 7428 7365 6c66 2e69 6d61 6765 5f73 697a  t(self.image_siz
+00007050: 655b 6469 6d31 5d29 0a20 2020 2020 2020  e[dim1]).       
+00007060: 2069 6620 6e6f 7420 7365 6c66 2e62 6163   if not self.bac
+00007070: 6b77 6172 643a 2061 6666 203d 2061 6666  kward: aff = aff
+00007080: 2e69 6e76 2829 0a20 2020 2020 2020 2072  .inv().        r
+00007090: 6574 7572 6e20 6166 662e 756e 7371 7565  eturn aff.unsque
+000070a0: 657a 6528 5b5d 290a 2020 2020 0a20 2020  eze([]).    .   
+000070b0: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
+000070c0: 7265 7475 726e 2052 6f74 6174 696f 6e39  return Rotation9
+000070d0: 3028 7365 6c66 2e64 696d 312c 2073 656c  0(self.dim1, sel
+000070e0: 662e 6469 6d32 2c20 696d 6167 655f 7369  f.dim2, image_si
+000070f0: 7a65 203d 2073 656c 662e 696d 6167 655f  ze = self.image_
+00007100: 7369 7a65 2c20 7265 7369 7a65 5f69 6d61  size, resize_ima
+00007110: 6765 203d 2073 656c 662e 7265 7369 7a65  ge = self.resize
+00007120: 5f69 6d61 6765 292e 6261 636b 7761 7264  _image).backward
+00007130: 5f28 7365 6c66 2e62 6163 6b77 6172 6429  _(self.backward)
+00007140: 0a0a 636c 6173 7320 526f 7461 7469 6f6e  ..class Rotation
+00007150: 3138 3028 5370 6174 6961 6c54 7261 6e73  180(SpatialTrans
+00007160: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+00007170: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007180: 662c 2064 696d 312c 2064 696d 322c 2069  f, dim1, dim2, i
+00007190: 6d61 6765 5f73 697a 653d 4e6f 6e65 293a  mage_size=None):
+000071a0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000071b0: 2020 2020 2054 7261 6e73 666f 726d 6174       Transformat
+000071c0: 696f 6e20 7468 6174 2072 6f74 6174 6573  ion that rotates
+000071d0: 2061 6e20 696d 6167 6520 6279 2031 3830   an image by 180
+000071e0: 2064 6567 7265 6573 2e0a 2020 2020 2020   degrees..      
+000071f0: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
+00007200: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00007210: 696d 312c 2064 696d 3220 5b69 6e74 5d3a  im1, dim2 [int]:
+00007220: 2054 6865 2070 6c61 6e65 2077 6520 726f   The plane we ro
+00007230: 7461 7465 206f 6e2e 2044 6972 6563 7469  tate on. Directi
+00007240: 6f6e 206f 6620 7468 6520 726f 7461 7469  on of the rotati
+00007250: 6f6e 2069 7320 6672 6f6d 2060 6469 6d31  on is from `dim1
+00007260: 6020 746f 2060 6469 6d32 602e 0a20 2020  ` to `dim2`..   
+00007270: 2020 2020 2020 2020 2020 2020 2069 2e65               i.e
+00007280: 2e20 726f 7461 7469 6f6e 2077 6974 6820  . rotation with 
+00007290: 6469 6d31 2061 7320 782d 6178 6973 2061  dim1 as x-axis a
+000072a0: 6e64 2064 696d 3220 6173 2079 2d61 7869  nd dim2 as y-axi
+000072b0: 733a 205b 6469 6d31 2c20 6469 6d32 5d20  s: [dim1, dim2] 
+000072c0: 636f 6f72 6469 6e61 7465 7320 2878 2c20  coordinates (x, 
+000072d0: 7929 2062 6563 6f6d 6573 2028 786d 6178  y) becomes (xmax
+000072e0: 2d78 2c20 796d 6178 2d79 292e 0a20 2020  -x, ymax-y)..   
+000072f0: 2020 2020 2020 2020 2069 6d61 6765 5f73           image_s
+00007300: 697a 6520 5b74 7570 6c65 206f 7220 6274  ize [tuple or bt
+00007310: 2e54 656e 736f 725d 3a20 5468 6520 7369  .Tensor]: The si
+00007320: 7a65 206f 6620 7468 6520 696d 6167 652c  ze of the image,
+00007330: 206f 7220 7468 6520 696d 6167 6520 6974   or the image it
+00007340: 7365 6c66 2e20 0a20 2020 2020 2020 2020  self. .         
+00007350: 2020 200a 2020 2020 2020 2020 5768 656e     .        When
+00007360: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
+00007370: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
+00007380: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
+00007390: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
+000073a0: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
+000073b0: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+000073c0: 5b6e 5f62 6174 6368 3a6f 7074 696f 6e61  [n_batch:optiona
+000073d0: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 5f31  l], {n_dim}, n_1
+000073e0: 2c20 6e5f 322c 202e 2e2e 2c20 6e5f 7229  , n_2, ..., n_r)
+000073f0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00007400: 7075 7420 5b62 742e 5465 6e73 6f72 5d3a  put [bt.Tensor]:
+00007410: 2054 6865 2074 7261 6e73 666f 726d 6564   The transformed
+00007420: 2063 6f6f 7264 696e 6174 6573 2e0a 2020   coordinates..  
+00007430: 2020 2020 2020 2020 2020 2020 2020 7369                si
+00007440: 7a65 3a20 285b 6e5f 6261 7463 685d 2c20  ze: ([n_batch], 
+00007450: 7b6e 5f64 696d 7d2c 206e 5f31 2c20 6e5f  {n_dim}, n_1, n_
+00007460: 322c 202e 2e2e 2c20 6e5f 7229 0a20 2020  2, ..., n_r).   
+00007470: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00007480: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+00007490: 5f28 6469 6d31 3d64 696d 312c 2064 696d  _(dim1=dim1, dim
+000074a0: 323d 6469 6d32 2c20 696d 6167 655f 7369  2=dim2, image_si
+000074b0: 7a65 3d69 6d61 6765 5f73 697a 6529 0a0a  ze=image_size)..
+000074c0: 2020 2020 2020 2020 7365 6c66 2e64 696d          self.dim
+000074d0: 312c 2073 656c 662e 6469 6d32 203d 2064  1, self.dim2 = d
+000074e0: 696d 312c 2064 696d 320a 2020 2020 2020  im1, dim2.      
+000074f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00007500: 696d 6167 655f 7369 7a65 2c20 6274 2e74  image_size, bt.t
+00007510: 6f72 6368 2e54 656e 736f 7229 3a20 696d  orch.Tensor): im
+00007520: 6167 655f 7369 7a65 203d 2069 6d61 6765  age_size = image
+00007530: 5f73 697a 652e 7368 6170 650a 2020 2020  _size.shape.    
+00007540: 2020 2020 7365 6c66 2e69 6d61 6765 5f73      self.image_s
+00007550: 697a 6520 3d20 696d 6167 655f 7369 7a65  ize = image_size
+00007560: 0a20 2020 2020 2020 2069 6620 696d 6167  .        if imag
+00007570: 655f 7369 7a65 2069 7320 6e6f 7420 4e6f  e_size is not No
+00007580: 6e65 3a20 7365 6c66 2e6e 5f64 696d 203d  ne: self.n_dim =
+00007590: 206c 656e 2869 6d61 6765 5f73 697a 6529   len(image_size)
+000075a0: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+000075b0: 5f5f 2873 656c 662c 2058 293a 0a20 2020  __(self, X):.   
+000075c0: 2020 2020 2058 203d 2073 7570 6572 2829       X = super()
+000075d0: 2e5f 5f63 616c 6c5f 5f28 5829 0a20 2020  .__call__(X).   
+000075e0: 2020 2020 2064 696d 312c 2064 696d 3220       dim1, dim2 
+000075f0: 3d20 7365 6c66 2e64 696d 312c 2073 656c  = self.dim1, sel
+00007600: 662e 6469 6d32 0a20 2020 2020 2020 2073  f.dim2.        s
+00007610: 656c 6563 7431 203d 2028 736c 6963 6528  elect1 = (slice(
+00007620: 4e6f 6e65 292c 2920 2a20 582e 6368 616e  None),) * X.chan
+00007630: 6e65 6c5f 6469 6d20 2b20 2864 696d 312c  nel_dim + (dim1,
+00007640: 290a 2020 2020 2020 2020 7365 6c65 6374  ).        select
+00007650: 3220 3d20 2873 6c69 6365 284e 6f6e 6529  2 = (slice(None)
+00007660: 2c29 202a 2058 2e63 6861 6e6e 656c 5f64  ,) * X.channel_d
+00007670: 696d 202b 2028 6469 6d32 2c29 0a20 2020  im + (dim2,).   
+00007680: 2020 2020 2069 6620 7365 6c66 2e69 6d61       if self.ima
+00007690: 6765 5f73 697a 6520 6973 204e 6f6e 653a  ge_size is None:
+000076a0: 206d 6178 5f72 616e 6765 312c 206d 6178   max_range1, max
+000076b0: 5f72 616e 6765 3220 3d20 585b 7365 6c65  _range2 = X[sele
+000076c0: 6374 315d 2e6d 6178 2829 2c20 585b 7365  ct1].max(), X[se
+000076d0: 6c65 6374 325d 2e6d 6178 2829 0a20 2020  lect2].max().   
+000076e0: 2020 2020 2065 6c73 653a 206d 6178 5f72       else: max_r
+000076f0: 616e 6765 312c 206d 6178 5f72 616e 6765  ange1, max_range
+00007700: 3220 3d20 7365 6c66 2e69 6d61 6765 5f73  2 = self.image_s
+00007710: 697a 655b 6469 6d31 5d2c 2073 656c 662e  ize[dim1], self.
+00007720: 696d 6167 655f 7369 7a65 5b64 696d 325d  image_size[dim2]
+00007730: 0a20 2020 2020 2020 2058 5b73 656c 6563  .        X[selec
+00007740: 7431 5d20 3d20 6d61 785f 7261 6e67 6531  t1] = max_range1
+00007750: 202d 2058 5b73 656c 6563 7431 5d0a 2020   - X[select1].  
+00007760: 2020 2020 2020 585b 7365 6c65 6374 325d        X[select2]
+00007770: 203d 206d 6178 5f72 616e 6765 3220 2d20   = max_range2 - 
+00007780: 585b 7365 6c65 6374 325d 0a20 2020 2020  X[select2].     
+00007790: 2020 2072 6574 7572 6e20 580a 2020 2020     return X.    
+000077a0: 2020 2020 0a20 2020 2064 6566 2061 6666      .    def aff
+000077b0: 696e 6528 7365 6c66 2c20 6e5f 6469 6d3d  ine(self, n_dim=
+000077c0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+000077d0: 6620 7365 6c66 2e69 6d61 6765 5f73 697a  f self.image_siz
+000077e0: 6520 6973 204e 6f6e 653a 2072 6574 7572  e is None: retur
+000077f0: 6e0a 2020 2020 2020 2020 6966 206e 5f64  n.        if n_d
+00007800: 696d 2069 7320 4e6f 6e65 2061 6e64 2073  im is None and s
+00007810: 656c 662e 6e5f 6469 6d20 6973 204e 6f6e  elf.n_dim is Non
+00007820: 653a 2072 6574 7572 6e0a 2020 2020 2020  e: return.      
+00007830: 2020 6966 206e 5f64 696d 2069 7320 4e6f    if n_dim is No
+00007840: 6e65 3a20 6e5f 6469 6d20 3d20 7365 6c66  ne: n_dim = self
+00007850: 2e6e 5f64 696d 0a20 2020 2020 2020 2061  .n_dim.        a
+00007860: 766f 7563 6828 7365 6c66 2e6e 5f64 696d  vouch(self.n_dim
+00007870: 2069 7320 4e6f 6e65 206f 7220 7365 6c66   is None or self
+00007880: 2e6e 5f64 696d 203d 3d20 6e5f 6469 6d29  .n_dim == n_dim)
+00007890: 0a20 2020 2020 2020 2064 696d 312c 2064  .        dim1, d
+000078a0: 696d 3220 3d20 7365 6c66 2e64 696d 312c  im2 = self.dim1,
+000078b0: 2073 656c 662e 6469 6d32 0a20 2020 2020   self.dim2.     
+000078c0: 2020 2061 6666 203d 2062 742e 6579 6528     aff = bt.eye(
+000078d0: 6e5f 6469 6d20 2b20 3129 0a20 2020 2020  n_dim + 1).     
+000078e0: 2020 2061 6666 5b64 696d 315d 5b64 696d     aff[dim1][dim
+000078f0: 315d 203d 202d 312e 0a20 2020 2020 2020  1] = -1..       
+00007900: 2061 6666 5b64 696d 315d 5b2d 315d 203d   aff[dim1][-1] =
+00007910: 2066 6c6f 6174 2873 656c 662e 696d 6167   float(self.imag
+00007920: 655f 7369 7a65 5b64 696d 315d 290a 2020  e_size[dim1]).  
+00007930: 2020 2020 2020 6166 665b 6469 6d32 5d5b        aff[dim2][
+00007940: 6469 6d32 5d20 3d20 2d31 2e0a 2020 2020  dim2] = -1..    
+00007950: 2020 2020 6166 665b 6469 6d32 5d5b 2d31      aff[dim2][-1
+00007960: 5d20 3d20 666c 6f61 7428 7365 6c66 2e69  ] = float(self.i
+00007970: 6d61 6765 5f73 697a 655b 6469 6d32 5d29  mage_size[dim2])
+00007980: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007990: 7365 6c66 2e62 6163 6b77 6172 643a 2061  self.backward: a
+000079a0: 6666 203d 2061 6666 2e69 6e76 2829 0a20  ff = aff.inv(). 
+000079b0: 2020 2020 2020 2072 6574 7572 6e20 6166         return af
+000079c0: 662e 756e 7371 7565 657a 6528 5b5d 290a  f.unsqueeze([]).
+000079d0: 0a20 2020 2064 6566 2069 6e76 2873 656c  .    def inv(sel
+000079e0: 6629 3a20 7265 7475 726e 2052 6f74 6174  f): return Rotat
+000079f0: 696f 6e31 3830 2873 656c 662e 6469 6d31  ion180(self.dim1
+00007a00: 2c20 7365 6c66 2e64 696d 322c 2069 6d61  , self.dim2, ima
+00007a10: 6765 5f73 697a 6520 3d20 7365 6c66 2e69  ge_size = self.i
+00007a20: 6d61 6765 5f73 697a 6529 2e62 6163 6b77  mage_size).backw
+00007a30: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+00007a40: 7264 290a 0a40 616c 6961 7328 2252 6566  rd)..@alias("Ref
+00007a50: 6c65 6374 2229 0a63 6c61 7373 2052 6566  lect").class Ref
+00007a60: 6c65 6374 696f 6e28 5370 6174 6961 6c54  lection(SpatialT
+00007a70: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
+00007a80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00007a90: 2873 656c 662c 202a 6469 6d2c 2069 6d61  (self, *dim, ima
+00007aa0: 6765 5f73 697a 653d 4e6f 6e65 293a 0a20  ge_size=None):. 
+00007ab0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00007ac0: 2020 2054 7261 6e73 666f 726d 6174 696f     Transformatio
+00007ad0: 6e20 7468 6174 2072 6566 6c65 6374 7320  n that reflects 
+00007ae0: 616e 2069 6d61 6765 2061 6c6f 6e67 2064  an image along d
+00007af0: 696d 656e 7369 6f6e 2064 696d 2e0a 2020  imension dim..  
+00007b00: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00007b10: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
+00007b20: 2020 2064 696d 205b 696e 745d 3a20 5468     dim [int]: Th
+00007b30: 6520 6469 6d65 6e73 696f 6e20 7765 2072  e dimension we r
+00007b40: 6566 6c65 6374 2074 6865 2069 6d61 6765  eflect the image
+00007b50: 2061 6c6f 6e67 2e20 0a20 2020 2020 2020   along. .       
+00007b60: 2020 2020 2020 2020 2069 2e65 2e20 7265           i.e. re
+00007b70: 666c 6563 7469 6f6e 206f 6e20 6469 6d3a  flection on dim:
+00007b80: 205b 6469 6d5d 2063 6f6f 7264 696e 6174   [dim] coordinat
+00007b90: 6520 7820 6265 636f 6d65 7320 786d 6178  e x becomes xmax
+00007ba0: 2d78 2e0a 2020 2020 2020 2020 2020 2020  -x..            
+00007bb0: 696d 6167 655f 7369 7a65 205b 7475 706c  image_size [tupl
+00007bc0: 6520 6f72 2062 742e 5465 6e73 6f72 5d3a  e or bt.Tensor]:
+00007bd0: 2054 6865 2073 697a 6520 6f66 2074 6865   The size of the
+00007be0: 2069 6d61 6765 2c20 6f72 2074 6865 2069   image, or the i
+00007bf0: 6d61 6765 2069 7473 656c 662e 200a 2020  mage itself. .  
+00007c00: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00007c10: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
+00007c20: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00007c30: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
+00007c40: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
+00007c50: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c70: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00007c80: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+00007c90: 6d7d 2c20 6e5f 312c 206e 5f32 2c20 2e2e  m}, n_1, n_2, ..
+00007ca0: 2e2c 206e 5f72 290a 2020 2020 2020 2020  ., n_r).        
+00007cb0: 2020 2020 6f75 7470 7574 205b 6274 2e54      output [bt.T
+00007cc0: 656e 736f 725d 3a20 5468 6520 7472 616e  ensor]: The tran
+00007cd0: 7366 6f72 6d65 6420 636f 6f72 6469 6e61  sformed coordina
+00007ce0: 7465 732e 0a20 2020 2020 2020 2020 2020  tes..           
+00007cf0: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+00007d00: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
+00007d10: 6e5f 312c 206e 5f32 2c20 2e2e 2e2c 206e  n_1, n_2, ..., n
+00007d20: 5f72 290a 2020 2020 2020 2020 2727 270a  _r).        '''.
+00007d30: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00007d40: 5f5f 696e 6974 5f5f 2864 696d 733d 6469  __init__(dims=di
+00007d50: 6d2c 2069 6d61 6765 5f73 697a 653d 696d  m, image_size=im
+00007d60: 6167 655f 7369 7a65 290a 0a20 2020 2020  age_size)..     
+00007d70: 2020 2069 6620 6c65 6e28 6469 6d29 203d     if len(dim) =
+00007d80: 3d20 3120 616e 6420 6973 696e 7374 616e  = 1 and isinstan
+00007d90: 6365 2864 696d 5b30 5d2c 2028 6c69 7374  ce(dim[0], (list
+00007da0: 2c20 7475 706c 6529 293a 2064 696d 203d  , tuple)): dim =
+00007db0: 2064 696d 5b30 5d0a 2020 2020 2020 2020   dim[0].        
+00007dc0: 7365 6c66 2e64 696d 7320 3d20 6469 6d0a  self.dims = dim.
+00007dd0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00007de0: 7461 6e63 6528 696d 6167 655f 7369 7a65  tance(image_size
+00007df0: 2c20 6274 2e74 6f72 6368 2e54 656e 736f  , bt.torch.Tenso
+00007e00: 7229 3a20 696d 6167 655f 7369 7a65 203d  r): image_size =
+00007e10: 2069 6d61 6765 5f73 697a 652e 7368 6170   image_size.shap
+00007e20: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+00007e30: 6d61 6765 5f73 697a 6520 3d20 696d 6167  mage_size = imag
+00007e40: 655f 7369 7a65 0a20 2020 2020 2020 2069  e_size.        i
+00007e50: 6620 696d 6167 655f 7369 7a65 2069 7320  f image_size is 
+00007e60: 6e6f 7420 4e6f 6e65 3a20 7365 6c66 2e6e  not None: self.n
+00007e70: 5f64 696d 203d 206c 656e 2869 6d61 6765  _dim = len(image
+00007e80: 5f73 697a 6529 0a0a 2020 2020 6465 6620  _size)..    def 
+00007e90: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
+00007ea0: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
+00007eb0: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
+00007ec0: 5829 0a20 2020 2020 2020 2064 696d 7320  X).        dims 
+00007ed0: 3d20 7365 6c66 2e64 696d 730a 2020 2020  = self.dims.    
+00007ee0: 2020 2020 666f 7220 6469 6d20 696e 2064      for dim in d
+00007ef0: 696d 733a 0a20 2020 2020 2020 2020 2020  ims:.           
+00007f00: 2073 656c 6563 7420 3d20 2873 6c69 6365   select = (slice
+00007f10: 284e 6f6e 6529 2c29 202a 2058 2e63 6861  (None),) * X.cha
+00007f20: 6e6e 656c 5f64 696d 202b 2028 6469 6d2c  nnel_dim + (dim,
+00007f30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00007f40: 2073 656c 662e 696d 6167 655f 7369 7a65   self.image_size
+00007f50: 2069 7320 4e6f 6e65 3a20 6d61 785f 7261   is None: max_ra
+00007f60: 6e67 6520 3d20 585b 7365 6c65 6374 5d2e  nge = X[select].
+00007f70: 6d61 7828 290a 2020 2020 2020 2020 2020  max().          
+00007f80: 2020 656c 7365 3a20 6d61 785f 7261 6e67    else: max_rang
+00007f90: 6520 3d20 7365 6c66 2e69 6d61 6765 5f73  e = self.image_s
+00007fa0: 697a 655b 6469 6d5d 0a20 2020 2020 2020  ize[dim].       
+00007fb0: 2020 2020 2058 5b73 656c 6563 745d 203d       X[select] =
+00007fc0: 206d 6178 5f72 616e 6765 202d 2058 5b73   max_range - X[s
+00007fd0: 656c 6563 745d 0a20 2020 2020 2020 2072  elect].        r
+00007fe0: 6574 7572 6e20 580a 2020 2020 2020 2020  eturn X.        
+00007ff0: 0a20 2020 2064 6566 2061 6666 696e 6528  .    def affine(
+00008000: 7365 6c66 2c20 6e5f 6469 6d3d 4e6f 6e65  self, n_dim=None
+00008010: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00008020: 6c66 2e69 6d61 6765 5f73 697a 6520 6973  lf.image_size is
+00008030: 204e 6f6e 653a 2072 6574 7572 6e0a 2020   None: return.  
+00008040: 2020 2020 2020 6966 206e 5f64 696d 2069        if n_dim i
+00008050: 7320 4e6f 6e65 2061 6e64 2073 656c 662e  s None and self.
+00008060: 6e5f 6469 6d20 6973 204e 6f6e 653a 2072  n_dim is None: r
+00008070: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00008080: 206e 5f64 696d 2069 7320 4e6f 6e65 3a20   n_dim is None: 
+00008090: 6e5f 6469 6d20 3d20 7365 6c66 2e6e 5f64  n_dim = self.n_d
+000080a0: 696d 0a20 2020 2020 2020 2061 766f 7563  im.        avouc
+000080b0: 6828 7365 6c66 2e6e 5f64 696d 2069 7320  h(self.n_dim is 
+000080c0: 4e6f 6e65 206f 7220 7365 6c66 2e6e 5f64  None or self.n_d
+000080d0: 696d 203d 3d20 6e5f 6469 6d29 0a20 2020  im == n_dim).   
+000080e0: 2020 2020 2061 6666 203d 2062 742e 6579       aff = bt.ey
+000080f0: 6528 6e5f 6469 6d20 2b20 3129 0a20 2020  e(n_dim + 1).   
+00008100: 2020 2020 2066 6f72 2064 696d 2069 6e20       for dim in 
+00008110: 7365 6c66 2e64 696d 733a 0a20 2020 2020  self.dims:.     
+00008120: 2020 2020 2020 2061 6666 5b64 696d 5d5b         aff[dim][
+00008130: 6469 6d5d 203d 202d 312e 0a20 2020 2020  dim] = -1..     
+00008140: 2020 2020 2020 2061 6666 5b64 696d 5d5b         aff[dim][
+00008150: 2d31 5d20 3d20 666c 6f61 7428 7365 6c66  -1] = float(self
+00008160: 2e69 6d61 6765 5f73 697a 655b 6469 6d5d  .image_size[dim]
+00008170: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00008180: 2073 656c 662e 6261 636b 7761 7264 3a20   self.backward: 
+00008190: 6166 6620 3d20 6166 662e 696e 7628 290a  aff = aff.inv().
+000081a0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+000081b0: 6666 2e75 6e73 7175 6565 7a65 285b 5d29  ff.unsqueeze([])
+000081c0: 0a0a 2020 2020 6465 6620 696e 7628 7365  ..    def inv(se
+000081d0: 6c66 293a 2072 6574 7572 6e20 5265 666c  lf): return Refl
+000081e0: 6563 7428 2a73 656c 662e 6469 6d73 2c20  ect(*self.dims, 
+000081f0: 696d 6167 655f 7369 7a65 203d 2073 656c  image_size = sel
+00008200: 662e 696d 6167 655f 7369 7a65 292e 6261  f.image_size).ba
+00008210: 636b 7761 7264 5f28 7365 6c66 2e62 6163  ckward_(self.bac
+00008220: 6b77 6172 6429 0a0a 4061 6c69 6173 2822  kward)..@alias("
+00008230: 5065 726d 7574 6564 696d 2229 0a63 6c61  Permutedim").cla
+00008240: 7373 2044 696d 5065 726d 7574 6174 696f  ss DimPermutatio
+00008250: 6e28 5370 6174 6961 6c54 7261 6e73 666f  n(SpatialTransfo
+00008260: 726d 6174 696f 6e29 3a0a 2020 2020 6465  rmation):.    de
+00008270: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00008280: 202a 6469 6d73 2c20 7265 7369 7a65 5f69   *dims, resize_i
+00008290: 6d61 6765 3d54 7275 6529 3a0a 2020 2020  mage=True):.    
+000082a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000082b0: 5065 726d 7574 6520 7468 6520 6469 6d65  Permute the dime
+000082c0: 6e73 696f 6e73 2066 6f72 2061 6e20 696d  nsions for an im
+000082d0: 6167 652c 2073 696d 696c 6172 2074 6f20  age, similar to 
+000082e0: 6e70 2e74 7261 6e73 706f 7365 206f 7220  np.transpose or 
+000082f0: 746f 7263 682f 6261 746f 7263 682e 7065  torch/batorch.pe
+00008300: 726d 7574 652e 0a20 2020 2020 2020 200a  rmute..        .
+00008310: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
+00008320: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
+00008330: 205b 6c69 7374 206f 7220 7475 706c 6520   [list or tuple 
+00008340: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
+00008350: 6865 2064 696d 656e 7369 6f6e 2070 6572  he dimension per
+00008360: 6d75 6174 696f 6e2e 200a 2020 2020 2020  muation. .      
+00008370: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00008380: 6c65 6e67 7468 286e 5f64 696d 2920 6f72  length(n_dim) or
+00008390: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+000083a0: 6e61 6c5d 2c20 7b6e 5f64 696d 7d29 2e0a  nal], {n_dim})..
+000083b0: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
+000083c0: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
+000083d0: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+000083e0: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
+000083f0: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
+00008400: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
+00008410: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+00008420: 6261 7463 683a 6f70 7469 6f6e 616c 5d2c  batch:optional],
+00008430: 207b 6e5f 6469 6d7d 2c20 6e5f 312c 206e   {n_dim}, n_1, n
+00008440: 5f32 2c20 2e2e 2e2c 206e 5f72 290a 2020  _2, ..., n_r).  
+00008450: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00008460: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+00008470: 6520 7472 616e 7366 6f72 6d65 6420 636f  e transformed co
+00008480: 6f72 6469 6e61 7465 732e 0a20 2020 2020  ordinates..     
+00008490: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+000084a0: 2028 5b6e 5f62 6174 6368 5d2c 207b 6e5f   ([n_batch], {n_
+000084b0: 6469 6d7d 2c20 6e5f 312c 206e 5f32 2c20  dim}, n_1, n_2, 
+000084c0: 2e2e 2e2c 206e 5f72 290a 2020 2020 2020  ..., n_r).      
+000084d0: 2020 2727 270a 2020 2020 2020 2020 6966    '''.        if
+000084e0: 206c 656e 2864 696d 7329 203d 3d20 313a   len(dims) == 1:
+000084f0: 2064 696d 7320 3d20 6469 6d73 5b30 5d0a   dims = dims[0].
+00008500: 2020 2020 2020 2020 6469 6d73 203d 2062          dims = b
+00008510: 6174 6f72 6368 5f74 656e 736f 7228 6c69  atorch_tensor(li
+00008520: 7374 2864 696d 7329 292e 7371 7565 657a  st(dims)).squeez
+00008530: 6528 290a 2020 2020 2020 2020 6469 6d73  e().        dims
+00008540: 203d 2064 696d 732e 6c6f 6e67 2829 0a20   = dims.long(). 
+00008550: 2020 2020 2020 2069 6620 6469 6d73 2e6e         if dims.n
+00008560: 5f64 696d 203c 3d20 313a 2064 696d 7320  _dim <= 1: dims 
+00008570: 3d20 6469 6d73 2e75 6e73 7175 6565 7a65  = dims.unsqueeze
+00008580: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
+00008590: 6469 6d73 2e6e 5f64 696d 203d 3d20 323a  dims.n_dim == 2:
+000085a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000085b0: 6e6f 7420 6469 6d73 2e68 6173 5f62 6174  not dims.has_bat
+000085c0: 6368 3a20 6469 6d73 2e62 6174 6368 5f64  ch: dims.batch_d
+000085d0: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+000085e0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000085f0: 6469 6d73 2e68 6173 5f63 6861 6e6e 656c  dims.has_channel
+00008600: 3a20 6469 6d73 2e63 6861 6e6e 656c 5f64  : dims.channel_d
+00008610: 696d 656e 7369 6f6e 203d 2030 2069 6620  imension = 0 if 
+00008620: 6469 6d73 2e62 6174 6368 5f64 696d 656e  dims.batch_dimen
+00008630: 7369 6f6e 203e 2030 2065 6c73 6520 310a  sion > 0 else 1.
+00008640: 2020 2020 2020 2020 6176 6f75 6368 2864          avouch(d
+00008650: 696d 732e 6861 735f 6261 7463 6820 616e  ims.has_batch an
+00008660: 6420 6469 6d73 2e68 6173 5f63 6861 6e6e  d dims.has_chann
+00008670: 656c 2c20 6622 506c 6561 7365 2075 7365  el, f"Please use
+00008680: 2062 6174 6f72 6368 2074 656e 736f 7220   batorch tensor 
+00008690: 6f66 2073 697a 6520 5c0a 2020 2020 2020  of size \.      
+000086a0: 2020 2020 2020 285b 6e5f 6261 7463 683a        ([n_batch:
+000086b0: 6f70 7469 6f6e 616c 5d2c 207b 7b6e 5f64  optional], {{n_d
+000086c0: 696d 7d7d 2920 666f 7220 5472 616e 736c  im}}) for Transl
+000086d0: 6174 696f 6e20 7061 7261 6d65 7465 7273  ation parameters
+000086e0: 2c20 696e 7374 6561 6420 6f66 207b 6469  , instead of {di
+000086f0: 6d73 2e73 6861 7065 7d2e 2022 290a 2020  ms.shape}. ").  
+00008700: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00008710: 696e 6974 5f5f 2864 696d 732c 2072 6573  init__(dims, res
+00008720: 697a 655f 696d 6167 653d 7265 7369 7a65  ize_image=resize
+00008730: 5f69 6d61 6765 290a 0a20 2020 2020 2020  _image)..       
+00008740: 2073 656c 662e 6469 6d73 203d 2064 696d   self.dims = dim
+00008750: 730a 2020 2020 2020 2020 7365 6c66 2e6e  s.        self.n
+00008760: 5f64 696d 203d 2064 696d 732e 6e5f 6368  _dim = dims.n_ch
+00008770: 616e 6e65 6c0a 2020 2020 2020 2020 7365  annel.        se
+00008780: 6c66 2e72 6573 697a 655f 696d 6167 6520  lf.resize_image 
+00008790: 3d20 7265 7369 7a65 5f69 6d61 6765 0a20  = resize_image. 
+000087a0: 2020 2020 2020 2069 6620 7265 7369 7a65         if resize
+000087b0: 5f69 6d61 6765 3a0a 2020 2020 2020 2020  _image:.        
+000087c0: 2020 2020 6966 2064 696d 732e 6e5f 6261      if dims.n_ba
+000087d0: 7463 6820 3e20 313a 0a20 2020 2020 2020  tch > 1:.       
+000087e0: 2020 2020 2020 2020 2064 696d 735f 6361           dims_ca
+000087f0: 7020 3d20 6469 6d73 2e73 616d 706c 6528  p = dims.sample(
+00008800: 7261 6e64 6f6d 3d46 616c 7365 2c20 6469  random=False, di
+00008810: 6d3d 5b5d 290a 2020 2020 2020 2020 2020  m=[]).          
+00008820: 2020 2020 2020 6176 6f75 6368 2862 742e        avouch(bt.
+00008830: 6e6f 726d 2864 696d 7320 2d20 6469 6d73  norm(dims - dims
+00008840: 5f63 6170 292e 7375 6d28 2920 3c20 3165  _cap).sum() < 1e
+00008850: 2d34 2c20 2243 616e 6e6f 7420 7265 7369  -4, "Cannot resi
+00008860: 7a65 2069 6d61 6765 2077 6865 6e20 6469  ze image when di
+00008870: 6666 6572 656e 7420 7065 726d 7574 6174  fferent permutat
+00008880: 696f 6e20 646f 6e65 2066 6f72 2064 6966  ion done for dif
+00008890: 6665 7265 6e74 2062 6174 6368 206d 656d  ferent batch mem
+000088a0: 6265 7273 2e20 2229 0a20 2020 2020 2020  bers. ").       
+000088b0: 2020 2020 2064 696d 7320 3d20 6469 6d73       dims = dims
+000088c0: 2e70 6963 6b28 302c 205b 5d29 2e74 6f6c  .pick(0, []).tol
+000088d0: 6973 7428 290a 2020 2020 2020 2020 2020  ist().          
+000088e0: 2020 7669 7369 7465 6420 3d20 5b5d 0a20    visited = []. 
+000088f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008900: 7265 7368 6170 6520 3d20 5b28 312c 295d  reshape = [(1,)]
+00008910: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00008920: 2070 2069 6e20 7261 6e67 6528 7365 6c66   p in range(self
+00008930: 2e6e 5f64 696d 293a 0a20 2020 2020 2020  .n_dim):.       
+00008940: 2020 2020 2020 2020 2069 6620 7020 696e           if p in
+00008950: 2076 6973 6974 6564 3a20 636f 6e74 696e   visited: contin
+00008960: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00008970: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2076 6973 6974 6564 2e61 7070 656e     visited.appen
+000089a0: 6428 7029 0a20 2020 2020 2020 2020 2020  d(p).           
+000089b0: 2020 2020 2020 2020 2071 203d 2064 696d           q = dim
+000089c0: 735b 705d 0a20 2020 2020 2020 2020 2020  s[p].           
+000089d0: 2020 2020 2020 2020 2069 6620 7120 696e           if q in
+000089e0: 2076 6973 6974 6564 3a20 6272 6561 6b0a   visited: break.
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2020 7365 6c66 2e72 6573 6861 7065      self.reshape
+00008a10: 2e61 7070 656e 6428 2870 2c20 7129 290a  .append((p, q)).
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 2020 2020 7020 3d20 710a 0a20 2020 2064      p = q..    d
+00008a40: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
+00008a50: 2c20 5829 3a0a 2020 2020 2020 2020 5820  , X):.        X 
+00008a60: 3d20 7375 7065 7228 292e 5f5f 6361 6c6c  = super().__call
+00008a70: 5f5f 2858 290a 2020 2020 2020 2020 7265  __(X).        re
+00008a80: 7475 726e 2058 2e67 6174 6865 7228 582e  turn X.gather(X.
+00008a90: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
+00008aa0: 6e2c 2073 656c 662e 6469 6d73 2e65 7870  n, self.dims.exp
+00008ab0: 616e 645f 746f 2858 2929 0a20 2020 2020  and_to(X)).     
+00008ac0: 2020 200a 2020 2020 6465 6620 6166 6669     .    def affi
+00008ad0: 6e65 2873 656c 662c 206e 5f64 696d 3d4e  ne(self, n_dim=N
+00008ae0: 6f6e 6529 3a0a 2020 2020 2020 2020 6176  one):.        av
+00008af0: 6f75 6368 286e 5f64 696d 2069 7320 4e6f  ouch(n_dim is No
+00008b00: 6e65 206f 7220 7365 6c66 2e6e 5f64 696d  ne or self.n_dim
+00008b10: 203d 3d20 6e5f 6469 6d29 0a20 2020 2020   == n_dim).     
+00008b20: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+00008b30: 6f6e 653a 206e 5f64 696d 203d 2073 656c  one: n_dim = sel
+00008b40: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
+00008b50: 6e5f 6261 7463 6820 3d20 7365 6c66 2e6e  n_batch = self.n
+00008b60: 5f62 6174 6368 0a20 2020 2020 2020 2069  _batch.        i
+00008b70: 6620 6e5f 6261 7463 6820 6973 204e 6f6e  f n_batch is Non
+00008b80: 653a 206e 5f62 6174 6368 203d 2031 0a20  e: n_batch = 1. 
+00008b90: 2020 2020 2020 2061 6666 203d 2062 742e         aff = bt.
+00008ba0: 6469 6167 2862 742e 6f6e 655f 686f 7428  diag(bt.one_hot(
+00008bb0: 2d31 2c20 6e5f 6469 6d20 2b20 3129 2e66  -1, n_dim + 1).f
+00008bc0: 6c6f 6174 2829 2e6d 756c 7469 706c 7928  loat().multiply(
+00008bd0: 6e5f 6261 7463 682c 205b 5d29 290a 2020  n_batch, [])).  
+00008be0: 2020 2020 2020 6220 3d20 6274 2e62 6174        b = bt.bat
+00008bf0: 6368 5f74 656e 736f 7228 6274 2e61 7261  ch_tensor(bt.ara
+00008c00: 6e67 6528 6e5f 6261 7463 6829 292e 6578  nge(n_batch)).ex
+00008c10: 7061 6e64 5f74 6f28 7365 6c66 2e64 696d  pand_to(self.dim
+00008c20: 7329 0a20 2020 2020 2020 2069 203d 2062  s).        i = b
+00008c30: 742e 6172 616e 6765 286e 5f64 696d 292e  t.arange(n_dim).
+00008c40: 6d75 6c74 6970 6c79 286e 5f62 6174 6368  multiply(n_batch
+00008c50: 2c20 5b5d 290a 2020 2020 2020 2020 6166  , []).        af
+00008c60: 665b 622c 2069 2c20 7365 6c66 2e64 696d  f[b, i, self.dim
+00008c70: 735d 203d 2031 2e0a 2020 2020 2020 2020  s] = 1..        
+00008c80: 6966 206e 6f74 2073 656c 662e 6261 636b  if not self.back
+00008c90: 7761 7264 3a20 6166 6620 3d20 6166 662e  ward: aff = aff.
+00008ca0: 696e 7628 290a 2020 2020 2020 2020 7265  inv().        re
+00008cb0: 7475 726e 2061 6666 0a0a 2020 2020 6465  turn aff..    de
+00008cc0: 6620 696e 7628 7365 6c66 293a 0a20 2020  f inv(self):.   
+00008cd0: 2020 2020 206e 5f64 696d 203d 2073 656c       n_dim = sel
+00008ce0: 662e 6e5f 6469 6d0a 2020 2020 2020 2020  f.n_dim.        
+00008cf0: 6e65 775f 7065 726d 7574 6520 3d20 2873  new_permute = (s
+00008d00: 656c 662e 6469 6d73 203d 3d20 6274 2e61  elf.dims == bt.a
+00008d10: 7261 6e67 6528 6e5f 6469 6d29 2e76 6965  range(n_dim).vie
+00008d20: 7728 5b31 5d2c 206e 5f64 696d 2c20 7b31  w([1], n_dim, {1
+00008d30: 7d29 292e 666c 6f61 7428 292e 6172 676d  })).float().argm
+00008d40: 6178 282d 3129 2e63 6861 6e6e 656c 5f64  ax(-1).channel_d
+00008d50: 696d 656e 7369 6f6e 5f28 2d31 290a 2020  imension_(-1).  
+00008d60: 2020 2020 2020 7265 7475 726e 2050 6572        return Per
+00008d70: 6d75 7465 6469 6d28 6e65 775f 7065 726d  mutedim(new_perm
+00008d80: 7574 652c 2072 6573 697a 655f 696d 6167  ute, resize_imag
+00008d90: 6520 3d20 7365 6c66 2e72 6573 697a 655f  e = self.resize_
+00008da0: 696d 6167 6529 2e62 6163 6b77 6172 645f  image).backward_
+00008db0: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
+00008dc0: 0a40 616c 6961 7328 2252 6573 6361 6c65  .@alias("Rescale
+00008dd0: 2229 0a63 6c61 7373 2052 6573 6361 6c69  ").class Rescali
+00008de0: 6e67 2853 7061 7469 616c 5472 616e 7366  ng(SpatialTransf
+00008df0: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
+00008e00: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00008e10: 2c20 2a73 6361 6c65 2c20 7265 7369 7a65  , *scale, resize
+00008e20: 5f69 6d61 6765 3d54 7275 6529 3a0a 2020  _image=True):.  
+00008e30: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00008e40: 2020 5363 616c 6520 616e 2069 6d61 6765    Scale an image
+00008e50: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008e60: 2020 204e 6f74 653a 2054 6865 2073 6361     Note: The sca
+00008e70: 6c69 6e67 2069 7320 666f 7220 636f 6f72  ling is for coor
+00008e80: 6469 6e61 7465 732c 2068 656e 6365 2074  dinates, hence t
+00008e90: 6865 2069 6d61 6765 2077 6f75 6c64 2073  he image would s
+00008ea0: 6872 696e 6b20 6966 2073 6361 6c65 203e  hrink if scale >
+00008eb0: 2031 2e20 0a20 2020 2020 2020 200a 2020   1. .        .  
+00008ec0: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
+00008ed0: 2020 2020 2020 2020 2020 7363 616c 6520            scale 
+00008ee0: 5b66 6c6f 6174 206f 7220 7475 706c 6520  [float or tuple 
+00008ef0: 6f72 2062 742e 5465 6e73 6f72 5d3a 2054  or bt.Tensor]: T
+00008f00: 6865 2073 6361 6c69 6e67 2066 6f72 2061  he scaling for a
+00008f10: 6c6c 2064 696d 656e 7369 6f6e 7320 2866  ll dimensions (f
+00008f20: 6c6f 6174 2920 0a20 2020 2020 2020 2020  loat) .         
+00008f30: 2020 2020 2020 206f 7220 666f 7220 6561         or for ea
+00008f40: 6368 2064 696d 656e 7369 6f6e 2028 7475  ch dimension (tu
+00008f50: 706c 6529 2e20 3e31 206d 6561 6e73 2065  ple). >1 means e
+00008f60: 6e6c 6172 6769 6e67 2074 6865 2063 6f6f  nlarging the coo
+00008f70: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00008f80: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00008f90: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+00008fa0: 616c 5d2c 207b 6e5f 6469 6d7d 2920 666f  al], {n_dim}) fo
+00008fb0: 7220 6274 2e54 656e 736f 722e 0a20 2020  r bt.Tensor..   
+00008fc0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00008fd0: 2020 5768 656e 2069 7420 6973 2063 616c    When it is cal
+00008fe0: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+00008ff0: 2058 205b 6274 2e54 656e 736f 725d 3a20   X [bt.Tensor]: 
+00009000: 436f 6f72 6469 6e61 7465 7320 746f 2062  Coordinates to b
+00009010: 6520 7472 616e 7366 6f72 6d65 642e 0a20  e transformed.. 
+00009020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009030: 697a 653a 2028 5b6e 5f62 6174 6368 3a6f  ize: ([n_batch:o
+00009040: 7074 696f 6e61 6c5d 2c20 7b6e 5f64 696d  ptional], {n_dim
+00009050: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
+00009060: 2c20 6e5f 7229 0a20 2020 2020 2020 2020  , n_r).         
+00009070: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
+00009080: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
+00009090: 666f 726d 6564 2063 6f6f 7264 696e 6174  formed coordinat
+000090a0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+000090b0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+000090c0: 7463 685d 2c20 7b6e 5f64 696d 7d2c 206e  tch], {n_dim}, n
+000090d0: 5f31 2c20 6e5f 322c 202e 2e2e 2c20 6e5f  _1, n_2, ..., n_
+000090e0: 7229 0a20 2020 2020 2020 2027 2727 0a20  r).        '''. 
+000090f0: 2020 2020 2020 2069 6620 6c65 6e28 7363         if len(sc
+00009100: 616c 6529 203d 3d20 3120 616e 6420 6973  ale) == 1 and is
+00009110: 696e 7374 616e 6365 2873 6361 6c65 5b30  instance(scale[0
+00009120: 5d2c 2028 696e 742c 2066 6c6f 6174 2929  ], (int, float))
+00009130: 3a20 7363 616c 6520 3d20 7363 616c 655b  : scale = scale[
+00009140: 305d 202a 2062 742e 6f6e 6573 285b 315d  0] * bt.ones([1]
+00009150: 2c20 7b31 7d29 0a20 2020 2020 2020 2065  , {1}).        e
+00009160: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00009170: 2069 6620 6c65 6e28 7363 616c 6529 203d   if len(scale) =
+00009180: 3d20 313a 2073 6361 6c65 203d 2073 6361  = 1: scale = sca
+00009190: 6c65 5b30 5d0a 2020 2020 2020 2020 2020  le[0].          
+000091a0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+000091b0: 6e63 6528 7363 616c 652c 2062 742e 5465  nce(scale, bt.Te
+000091c0: 6e73 6f72 293a 2073 6361 6c65 203d 2062  nsor): scale = b
+000091d0: 6174 6f72 6368 5f74 656e 736f 7228 6c69  atorch_tensor(li
+000091e0: 7374 2873 6361 6c65 2929 2e73 7175 6565  st(scale)).squee
+000091f0: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
+00009200: 2069 6620 7363 616c 652e 6e5f 6469 6d20   if scale.n_dim 
+00009210: 3c3d 2031 3a20 7363 616c 6520 3d20 7363  <= 1: scale = sc
+00009220: 616c 652e 756e 7371 7565 657a 6528 5b5d  ale.unsqueeze([]
+00009230: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00009240: 2073 6361 6c65 2e6e 5f64 696d 203d 3d20   scale.n_dim == 
+00009250: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00009260: 2020 2069 6620 6e6f 7420 7363 616c 652e     if not scale.
+00009270: 6861 735f 6261 7463 683a 2073 6361 6c65  has_batch: scale
+00009280: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00009290: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+000092a0: 2020 2020 2069 6620 6e6f 7420 7363 616c       if not scal
+000092b0: 652e 6861 735f 6368 616e 6e65 6c3a 2073  e.has_channel: s
+000092c0: 6361 6c65 2e63 6861 6e6e 656c 5f64 696d  cale.channel_dim
+000092d0: 656e 7369 6f6e 203d 2030 2069 6620 7363  ension = 0 if sc
+000092e0: 616c 652e 6261 7463 685f 6469 6d65 6e73  ale.batch_dimens
+000092f0: 696f 6e20 3e20 3020 656c 7365 2031 0a20  ion > 0 else 1. 
+00009300: 2020 2020 2020 2061 766f 7563 6828 7363         avouch(sc
+00009310: 616c 652e 6861 735f 6261 7463 6820 616e  ale.has_batch an
+00009320: 6420 7363 616c 652e 6861 735f 6368 616e  d scale.has_chan
+00009330: 6e65 6c2c 2066 2250 6c65 6173 6520 7573  nel, f"Please us
+00009340: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00009350: 206f 6620 7369 7a65 205c 0a20 2020 2020   of size \.     
+00009360: 2020 2020 2020 2028 5b6e 5f62 6174 6368         ([n_batch
+00009370: 3a6f 7074 696f 6e61 6c5d 2c20 7b7b 6e5f  :optional], {{n_
+00009380: 6469 6d7d 7d29 2066 6f72 2053 6361 6c69  dim}}) for Scali
+00009390: 6e67 2070 6172 616d 6574 6572 732c 2069  ng parameters, i
+000093a0: 6e73 7465 6164 206f 6620 7b73 6361 6c65  nstead of {scale
+000093b0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+000093c0: 2020 2020 6274 2e74 6f5f 6465 7669 6365      bt.to_device
+000093d0: 2873 6361 6c65 290a 2020 2020 2020 2020  (scale).        
+000093e0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+000093f0: 2873 6361 6c65 2c20 7265 7369 7a65 5f69  (scale, resize_i
+00009400: 6d61 6765 3d72 6573 697a 655f 696d 6167  mage=resize_imag
+00009410: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00009420: 2e73 6361 6c65 203d 2073 6361 6c65 0a20  .scale = scale. 
+00009430: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00009440: 6361 6c65 2e6e 5f63 6861 6e6e 656c 203e  cale.n_channel >
+00009450: 2031 3a20 7365 6c66 2e6e 5f64 696d 203d   1: self.n_dim =
+00009460: 2073 656c 662e 7363 616c 652e 6e5f 6368   self.scale.n_ch
+00009470: 616e 6e65 6c0a 2020 2020 2020 2020 6966  annel.        if
+00009480: 2072 6573 697a 655f 696d 6167 653a 0a20   resize_image:. 
+00009490: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000094a0: 203d 2073 6361 6c65 2e73 7175 6565 7a65   = scale.squeeze
+000094b0: 285b 5d29 0a20 2020 2020 2020 2020 2020  ([]).           
+000094c0: 2061 766f 7563 6828 7363 616c 652e 6e64   avouch(scale.nd
+000094d0: 696d 203d 3d20 3129 0a20 2020 2020 2020  im == 1).       
+000094e0: 2020 2020 2073 656c 662e 7265 7368 6170       self.reshap
+000094f0: 6520 3d20 5b74 7570 6c65 2828 312f 7363  e = [tuple((1/sc
+00009500: 616c 6529 2e74 6f6c 6973 7428 2929 5d0a  ale).tolist())].
+00009510: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00009520: 697a 655f 696d 6167 6520 3d20 7265 7369  ize_image = resi
+00009530: 7a65 5f69 6d61 6765 0a20 2020 2020 2020  ze_image.       
+00009540: 2073 656c 662e 6261 7463 685f 7061 7261   self.batch_para
+00009550: 6d2e 6170 7065 6e64 2827 7363 616c 6527  m.append('scale'
+00009560: 290a 0a20 2020 2064 6566 205f 5f63 616c  )..    def __cal
+00009570: 6c5f 5f28 7365 6c66 2c20 5829 3a0a 2020  l__(self, X):.  
+00009580: 2020 2020 2020 5820 3d20 7375 7065 7228        X = super(
+00009590: 292e 5f5f 6361 6c6c 5f5f 2858 290a 2020  ).__call__(X).  
+000095a0: 2020 2020 2020 7363 616c 6520 3d20 7365        scale = se
+000095b0: 6c66 2e73 6361 6c65 0a20 2020 2020 2020  lf.scale.       
+000095c0: 2072 6574 7572 6e20 5820 2a20 7363 616c   return X * scal
+000095d0: 650a 2020 2020 0a20 2020 2064 6566 2061  e.    .    def a
+000095e0: 6666 696e 6528 7365 6c66 2c20 6e5f 6469  ffine(self, n_di
+000095f0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00009600: 2069 6620 6e5f 6469 6d20 6973 204e 6f6e   if n_dim is Non
+00009610: 6520 616e 6420 7365 6c66 2e6e 5f64 696d  e and self.n_dim
+00009620: 2069 7320 4e6f 6e65 3a20 7265 7475 726e   is None: return
+00009630: 0a20 2020 2020 2020 2069 6620 6e5f 6469  .        if n_di
+00009640: 6d20 6973 204e 6f6e 653a 206e 5f64 696d  m is None: n_dim
+00009650: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
+00009660: 2020 2020 2020 6176 6f75 6368 2873 656c        avouch(sel
+00009670: 662e 6e5f 6469 6d20 6973 204e 6f6e 6520  f.n_dim is None 
+00009680: 6f72 2073 656c 662e 6e5f 6469 6d20 3d3d  or self.n_dim ==
+00009690: 206e 5f64 696d 290a 2020 2020 2020 2020   n_dim).        
+000096a0: 7363 616c 6520 3d20 7365 6c66 2e73 6361  scale = self.sca
+000096b0: 6c65 0a20 2020 2020 2020 2069 6620 6973  le.        if is
+000096c0: 696e 7374 616e 6365 2873 6361 6c65 2c20  instance(scale, 
+000096d0: 2869 6e74 2c20 666c 6f61 7429 293a 2072  (int, float)): r
+000096e0: 6574 7572 6e20 7363 616c 6520 2a20 6274  eturn scale * bt
+000096f0: 2e65 7965 286e 5f64 696d 202b 2031 290a  .eye(n_dim + 1).
+00009700: 2020 2020 2020 2020 6166 6620 3d20 6274          aff = bt
+00009710: 2e64 6961 6728 6274 2e63 6174 2873 6361  .diag(bt.cat(sca
+00009720: 6c65 2c20 6274 2e6f 6e65 7328 5b73 6361  le, bt.ones([sca
+00009730: 6c65 2e6e 5f62 6174 6368 5d2c 2031 292c  le.n_batch], 1),
+00009740: 2031 2929 0a20 2020 2020 2020 2069 6620   1)).        if 
+00009750: 6e6f 7420 7365 6c66 2e62 6163 6b77 6172  not self.backwar
+00009760: 643a 2061 6666 203d 2061 6666 2e69 6e76  d: aff = aff.inv
+00009770: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00009780: 6e20 6166 660a 0a20 2020 2064 6566 2069  n aff..    def i
+00009790: 6e76 2873 656c 6629 3a20 7265 7475 726e  nv(self): return
+000097a0: 2052 6573 6361 6c65 2831 2f73 656c 662e   Rescale(1/self.
+000097b0: 7363 616c 652c 2072 6573 697a 655f 696d  scale, resize_im
+000097c0: 6167 6520 3d20 7365 6c66 2e72 6573 697a  age = self.resiz
+000097d0: 655f 696d 6167 6529 2e62 6163 6b77 6172  e_image).backwar
+000097e0: 645f 2873 656c 662e 6261 636b 7761 7264  d_(self.backward
+000097f0: 290a 0a40 616c 6961 7328 2254 7261 6e73  )..@alias("Trans
+00009800: 6c61 7465 2229 0a63 6c61 7373 2054 7261  late").class Tra
+00009810: 6e73 6c61 7469 6f6e 2853 7061 7469 616c  nslation(Spatial
+00009820: 5472 616e 7366 6f72 6d61 7469 6f6e 293a  Transformation):
+00009830: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00009840: 5f28 7365 6c66 2c20 2a74 7261 6e73 6c61  _(self, *transla
+00009850: 7469 6f6e 293a 0a20 2020 2020 2020 2027  tion):.        '
+00009860: 2727 0a20 2020 2020 2020 2054 7261 6e73  ''.        Trans
+00009870: 6c61 7465 2061 6e20 696d 6167 652e 0a20  late an image.. 
+00009880: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009890: 4e6f 7465 3a20 5468 6520 7472 616e 736c  Note: The transl
+000098a0: 6174 696f 6e20 6973 2066 6f72 2063 6f6f  ation is for coo
+000098b0: 7264 696e 6174 6573 2c20 6865 6e63 6520  rdinates, hence 
+000098c0: 7468 6520 696d 6167 6520 776f 756c 6420  the image would 
+000098d0: 676f 2069 6e20 7468 6520 6f70 706f 7369  go in the opposi
+000098e0: 7465 2064 6972 6563 7469 6f6e 2e20 0a20  te direction. . 
+000098f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009900: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
+00009910: 2020 2020 7472 616e 736c 6174 696f 6e20      translation 
+00009920: 5b74 7570 6c65 206f 7220 6274 2e54 656e  [tuple or bt.Ten
+00009930: 736f 725d 3a20 5468 6520 7472 616e 736c  sor]: The transl
+00009940: 6174 696f 6e20 6f66 2074 6865 2063 6f6f  ation of the coo
+00009950: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00009960: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00009970: 6c65 6e67 7468 286e 5f64 696d 2920 6f72  length(n_dim) or
+00009980: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+00009990: 6e61 6c5d 2c20 7b6e 5f64 696d 7d29 0a20  nal], {n_dim}). 
+000099a0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+000099b0: 2020 2020 5768 656e 2069 7420 6973 2063      When it is c
+000099c0: 616c 6c65 643a 0a20 2020 2020 2020 2020  alled:.         
+000099d0: 2020 2058 205b 6274 2e54 656e 736f 725d     X [bt.Tensor]
+000099e0: 3a20 436f 6f72 6469 6e61 7465 7320 746f  : Coordinates to
+000099f0: 2062 6520 7472 616e 7366 6f72 6d65 642e   be transformed.
+00009a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a10: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+00009a20: 3a6f 7074 696f 6e61 6c5d 2c20 7b6e 5f64  :optional], {n_d
+00009a30: 696d 7d2c 206e 5f31 2c20 6e5f 322c 202e  im}, n_1, n_2, .
+00009a40: 2e2e 2c20 6e5f 7229 0a20 2020 2020 2020  .., n_r).       
+00009a50: 2020 2020 206f 7574 7075 7420 5b62 742e       output [bt.
+00009a60: 5465 6e73 6f72 5d3a 2054 6865 2074 7261  Tensor]: The tra
+00009a70: 6e73 666f 726d 6564 2063 6f6f 7264 696e  nsformed coordin
+00009a80: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
+00009a90: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+00009aa0: 6261 7463 685d 2c20 7b6e 5f64 696d 7d2c  batch], {n_dim},
+00009ab0: 206e 5f31 2c20 6e5f 322c 202e 2e2e 2c20   n_1, n_2, ..., 
+00009ac0: 6e5f 7229 0a20 2020 2020 2020 2027 2727  n_r).        '''
+00009ad0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00009ae0: 7472 616e 736c 6174 696f 6e29 203d 3d20  translation) == 
+00009af0: 313a 2074 7261 6e73 6c61 7469 6f6e 203d  1: translation =
+00009b00: 2074 7261 6e73 6c61 7469 6f6e 5b30 5d0a   translation[0].
+00009b10: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00009b20: 7461 6e63 6528 7472 616e 736c 6174 696f  tance(translatio
+00009b30: 6e2c 2074 7570 6c65 293a 2074 7261 6e73  n, tuple): trans
+00009b40: 6c61 7469 6f6e 203d 206c 6973 7428 7472  lation = list(tr
+00009b50: 616e 736c 6174 696f 6e29 0a20 2020 2020  anslation).     
+00009b60: 2020 2074 7261 6e73 6c61 7469 6f6e 203d     translation =
+00009b70: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00009b80: 7472 616e 736c 6174 696f 6e29 2e73 7175  translation).squ
+00009b90: 6565 7a65 2829 0a20 2020 2020 2020 2069  eeze().        i
+00009ba0: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
+00009bb0: 6469 6d20 3c3d 2031 3a20 7472 616e 736c  dim <= 1: transl
+00009bc0: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+00009bd0: 696f 6e2e 756e 7371 7565 657a 6528 5b5d  ion.unsqueeze([]
+00009be0: 290a 2020 2020 2020 2020 6966 2074 7261  ).        if tra
+00009bf0: 6e73 6c61 7469 6f6e 2e6e 5f64 696d 203d  nslation.n_dim =
+00009c00: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
+00009c10: 2069 6620 6e6f 7420 7472 616e 736c 6174   if not translat
+00009c20: 696f 6e2e 6861 735f 6261 7463 683a 2074  ion.has_batch: t
+00009c30: 7261 6e73 6c61 7469 6f6e 2e62 6174 6368  ranslation.batch
+00009c40: 5f64 696d 656e 7369 6f6e 203d 2030 0a20  _dimension = 0. 
+00009c50: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00009c60: 7420 7472 616e 736c 6174 696f 6e2e 6861  t translation.ha
+00009c70: 735f 6368 616e 6e65 6c3a 2074 7261 6e73  s_channel: trans
+00009c80: 6c61 7469 6f6e 2e63 6861 6e6e 656c 5f64  lation.channel_d
+00009c90: 696d 656e 7369 6f6e 203d 2030 2069 6620  imension = 0 if 
+00009ca0: 7472 616e 736c 6174 696f 6e2e 6261 7463  translation.batc
+00009cb0: 685f 6469 6d65 6e73 696f 6e20 3e20 3020  h_dimension > 0 
+00009cc0: 656c 7365 2031 0a20 2020 2020 2020 2061  else 1.        a
+00009cd0: 766f 7563 6828 7472 616e 736c 6174 696f  vouch(translatio
+00009ce0: 6e2e 6861 735f 6261 7463 6820 616e 6420  n.has_batch and 
+00009cf0: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
+00009d00: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+00009d10: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+00009d20: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
+00009d30: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
+00009d40: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00009d50: 7b7b 6e5f 6469 6d7d 7d29 2066 6f72 2054  {{n_dim}}) for T
+00009d60: 7261 6e73 6c61 7469 6f6e 2070 6172 616d  ranslation param
+00009d70: 6574 6572 732c 2069 6e73 7465 6164 206f  eters, instead o
+00009d80: 6620 7b74 7261 6e73 6c61 7469 6f6e 2e73  f {translation.s
+00009d90: 6861 7065 7d2e 2022 290a 2020 2020 2020  hape}. ").      
+00009da0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00009db0: 5f5f 2874 7261 6e73 6c61 7469 6f6e 290a  __(translation).
+00009dc0: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
+00009dd0: 616e 736c 6174 696f 6e20 3d20 7472 616e  anslation = tran
+00009de0: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
+00009df0: 7365 6c66 2e6e 5f64 696d 203d 2073 656c  self.n_dim = sel
+00009e00: 662e 7472 616e 736c 6174 696f 6e2e 6e5f  f.translation.n_
+00009e10: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+00009e20: 7365 6c66 2e62 6174 6368 5f70 6172 616d  self.batch_param
+00009e30: 2e61 7070 656e 6428 2774 7261 6e73 6c61  .append('transla
+00009e40: 7469 6f6e 2729 0a0a 2020 2020 6465 6620  tion')..    def 
+00009e50: 5f5f 6361 6c6c 5f5f 2873 656c 662c 2058  __call__(self, X
+00009e60: 293a 0a20 2020 2020 2020 2058 203d 2073  ):.        X = s
+00009e70: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
+00009e80: 5829 0a20 2020 2020 2020 2072 6574 7572  X).        retur
+00009e90: 6e20 5820 2b20 7365 6c66 2e74 7261 6e73  n X + self.trans
+00009ea0: 6c61 7469 6f6e 0a20 2020 200a 2020 2020  lation.    .    
+00009eb0: 6465 6620 6166 6669 6e65 2873 656c 662c  def affine(self,
+00009ec0: 206e 5f64 696d 3d4e 6f6e 6529 3a0a 2020   n_dim=None):.  
+00009ed0: 2020 2020 2020 6176 6f75 6368 286e 5f64        avouch(n_d
+00009ee0: 696d 2069 7320 4e6f 6e65 206f 7220 7365  im is None or se
+00009ef0: 6c66 2e6e 5f64 696d 203d 3d20 6e5f 6469  lf.n_dim == n_di
+00009f00: 6d29 0a20 2020 2020 2020 2069 6620 6e5f  m).        if n_
+00009f10: 6469 6d20 6973 204e 6f6e 653a 206e 5f64  dim is None: n_d
+00009f20: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
+00009f30: 2020 2020 2020 2020 6e5f 6261 7463 6820          n_batch 
+00009f40: 3d20 7365 6c66 2e74 7261 6e73 6c61 7469  = self.translati
+00009f50: 6f6e 2e6e 5f62 6174 6368 0a20 2020 2020  on.n_batch.     
+00009f60: 2020 2061 6666 203d 2062 742e 6361 7428     aff = bt.cat(
+00009f70: 6274 2e63 6174 2862 742e 6579 6528 7365  bt.cat(bt.eye(se
+00009f80: 6c66 2e6e 5f64 696d 292e 6d75 6c74 6970  lf.n_dim).multip
+00009f90: 6c79 286e 5f62 6174 6368 2c20 5b5d 292c  ly(n_batch, []),
+00009fa0: 2073 656c 662e 7472 616e 736c 6174 696f   self.translatio
+00009fb0: 6e2e 7769 7468 5f63 6861 6e6e 656c 6469  n.with_channeldi
+00009fc0: 6d28 4e6f 6e65 292e 756e 7371 7565 657a  m(None).unsqueez
+00009fd0: 6528 2d31 292c 202d 3129 2c20 6274 2e6f  e(-1), -1), bt.o
+00009fe0: 6e65 5f68 6f74 282d 312c 206e 5f64 696d  ne_hot(-1, n_dim
+00009ff0: 2b31 292e 756e 7371 7565 657a 6528 3029  +1).unsqueeze(0)
+0000a000: 2e6d 756c 7469 706c 7928 6e5f 6261 7463  .multiply(n_batc
+0000a010: 682c 205b 5d29 2c20 3129 0a20 2020 2020  h, []), 1).     
+0000a020: 2020 2069 6620 6e6f 7420 7365 6c66 2e62     if not self.b
+0000a030: 6163 6b77 6172 643a 2061 6666 203d 2061  ackward: aff = a
+0000a040: 6666 2e69 6e76 2829 0a20 2020 2020 2020  ff.inv().       
+0000a050: 2072 6574 7572 6e20 6166 660a 0a20 2020   return aff..   
+0000a060: 2064 6566 2069 6e76 2873 656c 6629 3a20   def inv(self): 
+0000a070: 7265 7475 726e 2054 7261 6e73 6c61 7465  return Translate
+0000a080: 282d 7365 6c66 2e74 7261 6e73 6c61 7469  (-self.translati
+0000a090: 6f6e 292e 6261 636b 7761 7264 5f28 7365  on).backward_(se
+0000a0a0: 6c66 2e62 6163 6b77 6172 6429 0a0a 4061  lf.backward)..@a
+0000a0b0: 6c69 6173 2822 5269 6722 290a 636c 6173  lias("Rig").clas
+0000a0c0: 7320 5269 6769 6428 5370 6174 6961 6c54  s Rigid(SpatialT
+0000a0d0: 7261 6e73 666f 726d 6174 696f 6e29 3a0a  ransformation):.
+0000a0e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000a0f0: 2873 656c 662c 2061 6e67 6c65 2c20 6178  (self, angle, ax
+0000a100: 6973 3d4e 6f6e 652c 2074 7261 6e73 6c61  is=None, transla
+0000a110: 7469 6f6e 3d4e 6f6e 652c 2063 656e 7465  tion=None, cente
+0000a120: 723d 4e6f 6e65 2c20 7472 616e 735f 7374  r=None, trans_st
+0000a130: 7265 7463 683d 4e6f 6e65 2c20 7370 6163  retch=None, spac
+0000a140: 696e 673d 3129 3a0a 2020 2020 2020 2020  ing=1):.        
+0000a150: 2727 270a 2020 2020 2020 2020 5269 6769  '''.        Rigi
+0000a160: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
+0000a170: 2077 6974 6820 7265 7370 6563 7420 746f   with respect to
+0000a180: 2070 6172 616d 6574 6572 732e 0a20 2020   parameters..   
+0000a190: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+0000a1a0: 7261 6d73 2053 6574 2031 3a0a 2020 2020  rams Set 1:.    
+0000a1b0: 2020 2020 2020 2020 616e 676c 6520 5b62          angle [b
+0000a1c0: 742e 5465 6e73 6f72 206f 7220 6e70 2e6e  t.Tensor or np.n
+0000a1d0: 756d 7079 5d3a 2074 6865 205b 636c 6f63  umpy]: the [cloc
+0000a1e0: 6b77 6973 655d 2072 6f74 6174 696f 6e20  kwise] rotation 
+0000a1f0: 616e 676c 6573 2061 626f 7574 2074 6865  angles about the
+0000a200: 2061 7869 7365 7320 286f 7220 7a20 6469   axises (or z di
+0000a210: 7265 6374 696f 6e20 666f 7220 3244 292e  rection for 2D).
+0000a220: 2049 7420 6973 2063 6f75 6e74 6572 2d63   It is counter-c
+0000a230: 6c6f 636b 7769 7365 2066 6f72 2069 6d61  lockwise for ima
+0000a240: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+0000a250: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+0000a260: 7463 685d 2c29 0a20 2020 2020 2020 2020  tch],).         
+0000a270: 2020 2061 7869 7320 5b62 742e 5465 6e73     axis [bt.Tens
+0000a280: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
+0000a290: 2074 6865 2072 6f74 6174 696f 6e20 6178   the rotation ax
+0000a2a0: 6973 6573 2c20 6e6f 726d 616c 697a 6564  ises, normalized
+0000a2b0: 2076 6563 746f 7273 2c20 4e6f 6e65 2066   vectors, None f
+0000a2c0: 6f72 2032 442e 200a 2020 2020 2020 2020  or 2D. .        
+0000a2d0: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+0000a2e0: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+0000a2f0: 7d29 0a20 2020 2020 2020 2020 2020 2074  }).            t
+0000a300: 7261 6e73 6c61 7469 6f6e 205b 6274 2e54  ranslation [bt.T
+0000a310: 656e 736f 7220 6f72 206e 702e 6e75 6d70  ensor or np.nump
+0000a320: 795d 3a20 7468 6520 7472 616e 736c 6174  y]: the translat
+0000a330: 696f 6e73 2061 6674 6572 2074 6865 2072  ions after the r
+0000a340: 6f74 6174 696f 6e2c 207a 6572 6f73 2062  otation, zeros b
+0000a350: 7920 6465 6661 756c 742e 200a 2020 2020  y default. .    
+0000a360: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+0000a370: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+0000a380: 5f64 696d 7d29 0a20 2020 2020 2020 2020  _dim}).         
+0000a390: 2020 2063 656e 7465 7220 5b62 742e 5465     center [bt.Te
+0000a3a0: 6e73 6f72 206f 7220 6e70 2e6e 756d 7079  nsor or np.numpy
+0000a3b0: 5d3a 2074 6865 2063 656e 7465 7220 666f  ]: the center fo
+0000a3c0: 7220 7468 6520 726f 7461 7469 6f6e 732c  r the rotations,
+0000a3d0: 207a 6572 6f73 2062 7920 6465 6661 756c   zeros by defaul
+0000a3e0: 742e 200a 2020 2020 2020 2020 2020 2020  t. .            
+0000a3f0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+0000a400: 7463 685d 2c20 7b6e 5f64 696d 7d29 0a20  tch], {n_dim}). 
+0000a410: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+0000a420: 5f73 7472 6574 6368 205b 696e 745d 3a20  _stretch [int]: 
+0000a430: 6f6e 6c79 2075 7365 6420 666f 7220 6974  only used for it
+0000a440: 6572 6174 6976 6520 7061 7261 6d65 7465  erative paramete
+0000a450: 7220 7472 6169 6e69 6e67 2c20 3120 6279  r training, 1 by
+0000a460: 2064 6566 6175 6c74 2e20 3230 2073 6565   default. 20 see
+0000a470: 6d73 2074 6f20 6265 2061 2067 6f6f 6420  ms to be a good 
+0000a480: 6368 6f69 6365 2e20 0a20 2020 2020 2020  choice. .       
+0000a490: 2020 2020 2073 7061 6369 6e67 205b 7475       spacing [tu
+0000a4a0: 706c 655d 3a20 7468 6520 7370 6163 696e  ple]: the spacin
+0000a4b0: 6720 6f66 2074 6865 2074 7261 6e73 666f  g of the transfo
+0000a4c0: 726d 6564 200a 2020 2020 2020 2020 0a20  rmed .        . 
+0000a4d0: 2020 2020 2020 2050 6172 616d 7320 5365         Params Se
+0000a4e0: 7420 323a 0a20 2020 2020 2020 2020 2020  t 2:.           
+0000a4f0: 206d 6174 7269 7820 5b62 742e 5465 6e73   matrix [bt.Tens
+0000a500: 6f72 206f 7220 6e70 2e6e 756d 7079 5d3a  or or np.numpy]:
+0000a510: 2074 6865 2061 6666 696e 6520 6d61 7472   the affine matr
+0000a520: 6978 2c20 6974 2073 686f 756c 6420 6265  ix, it should be
+0000a530: 206f 7274 686f 676f 6e61 6c20 6f72 2077   orthogonal or w
+0000a540: 696c 6c20 6265 2070 726f 6a65 6374 6564  ill be projected
+0000a550: 2062 7920 5072 6f63 7275 7374 6573 2050   by Procrustes P
+0000a560: 726f 626c 656d 2e20 0a20 2020 2020 2020  roblem. .       
+0000a570: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+0000a580: 5b6e 5f62 6174 6368 5d2c 206e 5f64 696d  [n_batch], n_dim
+0000a590: 202b 2031 2c20 6e5f 6469 6d20 2b20 3129   + 1, n_dim + 1)
+0000a5a0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+0000a5b0: 6e73 5f73 7472 6574 6368 205b 696e 745d  ns_stretch [int]
+0000a5c0: 3a20 6f6e 6c79 2075 7365 6420 666f 7220  : only used for 
+0000a5d0: 6974 6572 6174 6976 6520 7061 7261 6d65  iterative parame
+0000a5e0: 7465 7220 7472 6169 6e69 6e67 2c20 3120  ter training, 1 
+0000a5f0: 6279 2064 6566 6175 6c74 2e20 3230 2073  by default. 20 s
+0000a600: 6565 6d73 2074 6f20 6265 2061 2067 6f6f  eems to be a goo
+0000a610: 6420 6368 6f69 6365 2e20 0a20 2020 2020  d choice. .     
+0000a620: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a630: 5768 656e 2069 7420 6973 2063 616c 6c65  When it is calle
+0000a640: 643a 0a20 2020 2020 2020 2020 2020 2058  d:.            X
+0000a650: 205b 6274 2e54 656e 736f 725d 3a20 436f   [bt.Tensor]: Co
+0000a660: 6f72 6469 6e61 7465 7320 746f 2062 6520  ordinates to be 
+0000a670: 7472 616e 7366 6f72 6d65 642e 0a20 2020  transformed..   
+0000a680: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+0000a690: 653a 2028 5b6e 5f62 6174 6368 3a20 6f70  e: ([n_batch: op
+0000a6a0: 7469 6f6e 616c 5d2c 207b 6e5f 6469 6d7d  tional], {n_dim}
+0000a6b0: 2c20 6e5f 312c 206e 5f32 2c20 2e2e 2e2c  , n_1, n_2, ...,
+0000a6c0: 206e 5f72 290a 2020 2020 2020 2020 2020   n_r).          
+0000a6d0: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
+0000a6e0: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
+0000a6f0: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
+0000a700: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000a710: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+0000a720: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e5f  ch], {n_dim}, n_
+0000a730: 312c 206e 5f32 2c20 2e2e 2e2c 206e 5f72  1, n_2, ..., n_r
+0000a740: 290a 2020 2020 2020 2020 2727 270a 2020  ).        '''.  
+0000a750: 2020 2020 2020 616e 676c 6520 3d20 6261        angle = ba
+0000a760: 746f 7263 685f 7465 6e73 6f72 2861 6e67  torch_tensor(ang
+0000a770: 6c65 290a 2020 2020 2020 2020 6966 2061  le).        if a
+0000a780: 6e67 6c65 2e6e 5f64 696d 203c 3d20 3020  ngle.n_dim <= 0 
+0000a790: 616e 6420 6e6f 7420 616e 676c 652e 6861  and not angle.ha
+0000a7a0: 735f 6261 7463 683a 2061 6e67 6c65 203d  s_batch: angle =
+0000a7b0: 2061 6e67 6c65 2e75 6e73 7175 6565 7a65   angle.unsqueeze
+0000a7c0: 285b 5d29 0a20 2020 2020 2020 2069 6620  ([]).        if 
+0000a7d0: 616e 676c 652e 6e5f 6469 6d20 3d3d 2031  angle.n_dim == 1
+0000a7e0: 2061 6e64 206e 6f74 2061 6e67 6c65 2e68   and not angle.h
+0000a7f0: 6173 5f62 6174 6368 3a20 616e 676c 6520  as_batch: angle 
+0000a800: 3d20 616e 676c 652e 7769 7468 5f62 6174  = angle.with_bat
+0000a810: 6368 6469 6d28 3029 0a20 2020 2020 2020  chdim(0).       
+0000a820: 2069 6620 616e 676c 652e 6e5f 6469 6d20   if angle.n_dim 
+0000a830: 3d3d 2032 2061 6e64 206e 6f74 2061 6e67  == 2 and not ang
+0000a840: 6c65 2e68 6173 5f62 6174 6368 3a20 616e  le.has_batch: an
+0000a850: 676c 6520 3d20 616e 676c 652e 756e 7371  gle = angle.unsq
+0000a860: 7565 657a 6528 5b5d 290a 2020 2020 2020  ueeze([]).      
+0000a870: 2020 6966 2061 6e67 6c65 2e6e 5f64 696d    if angle.n_dim
+0000a880: 203d 3d20 3320 616e 6420 6e6f 7420 616e   == 3 and not an
+0000a890: 676c 652e 6861 735f 6261 7463 6820 616e  gle.has_batch an
+0000a8a0: 6420 616e 676c 652e 7368 6170 655b 315d  d angle.shape[1]
+0000a8b0: 203d 3d20 616e 676c 652e 7368 6170 655b   == angle.shape[
+0000a8c0: 325d 3a20 616e 676c 652e 6261 7463 685f  2]: angle.batch_
+0000a8d0: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+0000a8e0: 2020 2020 2020 6176 6f75 6368 2861 6e67        avouch(ang
+0000a8f0: 6c65 2e68 6173 5f62 6174 6368 2c20 6622  le.has_batch, f"
+0000a900: 506c 6561 7365 2075 7365 2062 6174 6f72  Please use bator
+0000a910: 6368 2074 656e 736f 7220 6f66 2073 697a  ch tensor of siz
+0000a920: 6520 285b 6e5f 6261 7463 685d 2c29 2066  e ([n_batch],) f
+0000a930: 6f72 2052 6967 6964 2072 6f74 6174 696f  or Rigid rotatio
+0000a940: 6e20 616e 676c 6573 2c20 696e 7374 6561  n angles, instea
+0000a950: 6420 6f66 207b 616e 676c 652e 7368 6170  d of {angle.shap
+0000a960: 657d 2e20 2229 0a20 2020 2020 2020 206e  e}. ").        n
+0000a970: 5f62 6174 6368 203d 2061 6e67 6c65 2e6e  _batch = angle.n
+0000a980: 5f62 6174 6368 0a20 2020 2020 2020 206e  _batch.        n
+0000a990: 5f64 696d 203d 204e 6f6e 650a 2020 2020  _dim = None.    
+0000a9a0: 2020 2020 6966 2061 6e67 6c65 2e6e 5f64      if angle.n_d
+0000a9b0: 696d 203e 3d20 323a 0a20 2020 2020 2020  im >= 2:.       
+0000a9c0: 2020 2020 206d 6174 7269 7820 3d20 616e       matrix = an
+0000a9d0: 676c 650a 2020 2020 2020 2020 2020 2020  gle.            
+0000a9e0: 6e5f 6469 6d20 3d20 6d61 7472 6978 2e73  n_dim = matrix.s
+0000a9f0: 697a 6528 2d31 2920 2d20 310a 2020 2020  ize(-1) - 1.    
+0000aa00: 2020 2020 2020 2020 6365 6e74 6572 203d          center =
+0000aa10: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
+0000aa20: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
+0000aa30: 2020 2020 2020 2020 2020 7472 616e 736c            transl
+0000aa40: 6174 696f 6e20 3d20 6d61 7472 6978 5b2e  ation = matrix[.
+0000aa50: 2e2e 2c20 3a2d 312c 202d 315d 2e77 6974  .., :-1, -1].wit
+0000aa60: 685f 6368 616e 6e65 6c64 696d 2831 290a  h_channeldim(1).
+0000aa70: 2020 2020 2020 2020 2020 2020 4120 3d20              A = 
+0000aa80: 6d61 7472 6978 5b2e 2e2e 2c20 3a2d 312c  matrix[..., :-1,
+0000aa90: 203a 2d31 5d0a 2020 2020 2020 2020 2020   :-1].          
+0000aaa0: 2020 6176 6f75 6368 2862 742e 6e6f 726d    avouch(bt.norm
+0000aab0: 2841 2e54 2040 2041 202d 2062 742e 6579  (A.T @ A - bt.ey
+0000aac0: 6528 4129 292e 7375 6d28 2920 3c20 3165  e(A)).sum() < 1e
+0000aad0: 2d34 2c20 2250 6c65 6173 6520 6d61 6b65  -4, "Please make
+0000aae0: 2073 7572 6520 7468 6174 206d 6174 7269   sure that matri
+0000aaf0: 7820 696e 7075 7420 666f 7220 5269 6769  x input for Rigi
+0000ab00: 6420 6973 206f 7274 686f 676f 6e61 6c2e  d is orthogonal.
+0000ab10: 2055 7365 2041 6666 696e 6520 696e 7374   Use Affine inst
+0000ab20: 6561 6420 6966 2069 7420 6973 206e 6f74  ead if it is not
+0000ab30: 2e20 2229 0a20 2020 2020 2020 2020 2020  . ").           
+0000ab40: 2023 2049 203d 2062 742e 6579 6528 4129   # I = bt.eye(A)
+0000ab50: 0a20 2020 2020 2020 2020 2020 2023 205a  .            # Z
+0000ab60: 5f6c 6566 7420 3d20 2841 202d 2049 295b  _left = (A - I)[
+0000ab70: 2e2e 2e2c 203a 2d31 5d20 2320 285b 6e5f  ..., :-1] # ([n_
+0000ab80: 6261 7463 685d 2c20 6e5f 6469 6d2c 206e  batch], n_dim, n
+0000ab90: 5f64 696d 2d31 290a 2020 2020 2020 2020  _dim-1).        
+0000aba0: 2020 2020 2320 5a5f 7269 6768 7420 3d20      # Z_right = 
+0000abb0: 2841 202d 2049 295b 2e2e 2e2c 202d 315d  (A - I)[..., -1]
+0000abc0: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
+0000abd0: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
+0000abe0: 2020 2320 5a54 5a20 3d20 5a5f 6c65 6674    # ZTZ = Z_left
+0000abf0: 2e54 2040 205a 5f6c 6566 740a 2020 2020  .T @ Z_left.    
+0000ac00: 2020 2020 2020 2020 2320 6966 206e 5f64          # if n_d
+0000ac10: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+0000ac20: 2020 2020 2023 2020 2020 2061 7869 7320       #     axis 
+0000ac30: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000ac40: 2020 2023 2020 2020 2061 6e67 6c65 203d     #     angle =
+0000ac50: 2062 742e 7768 6572 6528 6274 2e61 6273   bt.where(bt.abs
+0000ac60: 2862 742e 6465 7428 5a54 5a29 2920 3c20  (bt.det(ZTZ)) < 
+0000ac70: 3165 2d36 2c20 6274 2e7a 6572 6f73 285b  1e-6, bt.zeros([
+0000ac80: 6e5f 6261 7463 685d 292c 2062 742e 6163  n_batch]), bt.ac
+0000ac90: 6f73 2831 202d 205a 545a 202f 2032 292e  os(1 - ZTZ / 2).
+0000aca0: 7371 7565 657a 6528 2d31 2c20 2d31 2929  squeeze(-1, -1))
+0000acb0: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
+0000acc0: 6c69 6620 6e5f 6469 6d20 3d3d 2033 3a0a  lif n_dim == 3:.
+0000acd0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000ace0: 2020 696e 765a 545a 203d 2062 742e 696e    invZTZ = bt.in
+0000acf0: 7628 6274 2e77 6865 7265 2862 742e 6162  v(bt.where(bt.ab
+0000ad00: 7328 6274 2e64 6574 285a 545a 2929 2e75  s(bt.det(ZTZ)).u
+0000ad10: 6e73 7175 6565 7a65 282d 312c 202d 3129  nsqueeze(-1, -1)
+0000ad20: 203c 2031 652d 362c 2062 742e 6579 6528   < 1e-6, bt.eye(
+0000ad30: 5a54 5a29 2c20 5a54 5a29 290a 2020 2020  ZTZ), ZTZ)).    
+0000ad40: 2020 2020 2020 2020 2320 2020 2020 7665          #     ve
+0000ad50: 6374 6f72 203d 2062 742e 6361 7428 2d20  ctor = bt.cat(- 
+0000ad60: 696e 765a 545a 2040 205a 5f6c 6566 742e  invZTZ @ Z_left.
+0000ad70: 5420 4020 5a5f 7269 6768 742c 2062 742e  T @ Z_right, bt.
+0000ad80: 6f6e 6573 285b 6e5f 6261 7463 685d 2c20  ones([n_batch], 
+0000ad90: 3129 2c20 3129 2e77 6974 685f 6368 616e  1), 1).with_chan
+0000ada0: 6e65 6c64 696d 2831 290a 2020 2020 2020  neldim(1).      
+0000adb0: 2020 2020 2020 2320 2020 2020 616e 676c        #     angl
+0000adc0: 6520 3d20 6274 2e77 6865 7265 2862 742e  e = bt.where(bt.
+0000add0: 6162 7328 6274 2e64 6574 285a 545a 2929  abs(bt.det(ZTZ))
+0000ade0: 203c 2031 652d 362c 2062 742e 7a65 726f   < 1e-6, bt.zero
+0000adf0: 7328 5b6e 5f62 6174 6368 5d29 2c20 7665  s([n_batch]), ve
+0000ae00: 6374 6f72 2e6e 6f72 6d28 2929 0a20 2020  ctor.norm()).   
+0000ae10: 2020 2020 2020 2020 2023 2020 2020 2061           #     a
+0000ae20: 7869 7320 3d20 6274 2e77 6865 7265 2828  xis = bt.where((
+0000ae30: 6274 2e61 6273 2862 742e 6465 7428 5a54  bt.abs(bt.det(ZT
+0000ae40: 5a29 2920 3c20 3165 2d36 292e 6d75 6c74  Z)) < 1e-6).mult
+0000ae50: 6970 6c79 286e 5f64 696d 2c20 7b7d 292c  iply(n_dim, {}),
+0000ae60: 2062 742e 6368 616e 6e65 6c5f 7465 6e73   bt.channel_tens
+0000ae70: 6f72 2862 742e 6f6e 655f 686f 7428 302c  or(bt.one_hot(0,
+0000ae80: 206e 5f64 696d 2929 2e6d 756c 7469 706c   n_dim)).multipl
+0000ae90: 7928 6e5f 6261 7463 682c 205b 5d29 2c20  y(n_batch, []), 
+0000aea0: 7665 6374 6f72 202f 2061 6e67 6c65 290a  vector / angle).
+0000aeb0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000aec0: 5f64 696d 203d 3d20 323a 2061 7869 7320  _dim == 2: axis 
+0000aed0: 3d20 4e6f 6e65 3b20 616e 676c 6520 3d20  = None; angle = 
+0000aee0: 6274 2e61 636f 7328 415b 2e2e 2e2c 2030  bt.acos(A[..., 0
+0000aef0: 2c20 305d 290a 2020 2020 2020 2020 2020  , 0]).          
+0000af00: 2020 656c 6966 206e 5f64 696d 203d 3d20    elif n_dim == 
+0000af10: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
+0000af20: 2020 2061 6e74 695f 7379 6d20 3d20 2841     anti_sym = (A
+0000af30: 202d 2041 2e54 2920 2f20 320a 2020 2020   - A.T) / 2.    
+0000af40: 2020 2020 2020 2020 2020 2020 7379 6d20              sym 
+0000af50: 3d20 2841 202b 2041 2e54 2920 2f20 3220  = (A + A.T) / 2 
+0000af60: 2d20 6274 2e65 7965 2841 290a 2020 2020  - bt.eye(A).    
+0000af70: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+0000af80: 6520 3d20 6274 2e61 636f 7328 2828 616e  e = bt.acos(((an
+0000af90: 7469 5f73 796d 2040 2061 6e74 695f 7379  ti_sym @ anti_sy
+0000afa0: 6d29 202f 2073 796d 292e 6d65 616e 2829  m) / sym).mean()
+0000afb0: 202d 2031 290a 2020 2020 2020 2020 2020   - 1).          
+0000afc0: 2020 2020 2020 6178 6973 203d 2062 742e        axis = bt.
+0000afd0: 756e 6372 6f73 735f 6d61 7472 6978 2861  uncross_matrix(a
+0000afe0: 6e74 695f 7379 6d29 0a20 2020 2020 2020  nti_sym).       
+0000aff0: 2020 2020 2020 2020 2061 7869 7320 2f3d           axis /=
+0000b000: 2062 742e 7369 6e28 616e 676c 6529 0a20   bt.sin(angle). 
+0000b010: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000b020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b030: 2072 6169 7365 2045 7272 6f72 2822 4e6f   raise Error("No
+0000b040: 7449 6d70 6c65 6d65 6e74 6564 2229 2866  tImplemented")(f
+0000b050: 2252 6967 6964 2074 7261 6e73 666f 726d  "Rigid transform
+0000b060: 6174 696f 6e20 696e 206d 6963 6f6d 7075  ation in micompu
+0000b070: 7469 6e67 2064 6f65 7320 6e6f 7420 7375  ting does not su
+0000b080: 7070 6f72 7420 7b6e 5f64 696d 7d20 6469  pport {n_dim} di
+0000b090: 6d65 6e73 696f 6e61 6c20 7472 616e 7366  mensional transf
+0000b0a0: 6f72 6d73 2028 3220 2620 3344 206f 6e6c  orms (2 & 3D onl
+0000b0b0: 7929 2e20 2220 2b20 0a20 2020 2020 2020  y). " + .       
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0e0: 2020 2020 2022 506c 6561 7365 2063 6f6e       "Please con
+0000b0f0: 7461 6374 2074 6865 2064 6576 656c 6f70  tact the develop
+0000b100: 6572 7320 6966 2074 6865 7265 2061 7265  ers if there are
+0000b110: 2066 6561 7369 626c 6520 616c 676f 7269   feasible algori
+0000b120: 7468 6d73 2028 4572 726f 7220 436f 6465  thms (Error Code
+0000b130: 3a20 5433 3333 292e 2054 6861 6e6b 2079  : T333). Thank y
+0000b140: 6f75 2e20 2229 0a0a 2020 2020 2020 2020  ou. ")..        
+0000b150: 6966 2074 7261 6e73 6c61 7469 6f6e 2069  if translation i
+0000b160: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b170: 2020 2020 2020 2020 7472 616e 736c 6174          translat
+0000b180: 696f 6e20 3d20 6261 746f 7263 685f 7465  ion = batorch_te
+0000b190: 6e73 6f72 2874 7261 6e73 6c61 7469 6f6e  nsor(translation
+0000b1a0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b1b0: 2074 7261 6e73 6c61 7469 6f6e 2e6e 5f64   translation.n_d
+0000b1c0: 696d 203c 3d20 3120 616e 6420 6e6f 7420  im <= 1 and not 
+0000b1d0: 7472 616e 736c 6174 696f 6e2e 6861 735f  translation.has_
+0000b1e0: 6261 7463 683a 2074 7261 6e73 6c61 7469  batch: translati
+0000b1f0: 6f6e 203d 2074 7261 6e73 6c61 7469 6f6e  on = translation
+0000b200: 2e75 6e73 7175 6565 7a65 285b 5d29 0a20  .unsqueeze([]). 
+0000b210: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+0000b220: 616e 736c 6174 696f 6e2e 6e5f 6469 6d20  anslation.n_dim 
+0000b230: 3d3d 2032 2061 6e64 206e 6f74 2074 7261  == 2 and not tra
+0000b240: 6e73 6c61 7469 6f6e 2e68 6173 5f62 6174  nslation.has_bat
+0000b250: 6368 3a20 7472 616e 736c 6174 696f 6e20  ch: translation 
+0000b260: 3d20 7472 616e 736c 6174 696f 6e2e 7769  = translation.wi
+0000b270: 7468 5f62 6174 6368 6469 6d28 2831 202d  th_batchdim((1 -
+0000b280: 2074 7261 6e73 6c61 7469 6f6e 2e63 6861   translation.cha
+0000b290: 6e6e 656c 5f64 696d 656e 7369 6f6e 2920  nnel_dimension) 
+0000b2a0: 6966 2074 7261 6e73 6c61 7469 6f6e 2e68  if translation.h
+0000b2b0: 6173 5f63 6861 6e6e 656c 2065 6c73 6520  as_channel else 
+0000b2c0: 3029 0a20 2020 2020 2020 2020 2020 2069  0).            i
+0000b2d0: 6620 7472 616e 736c 6174 696f 6e2e 6e5f  f translation.n_
+0000b2e0: 6469 6d20 3d3d 2032 2061 6e64 206e 6f74  dim == 2 and not
+0000b2f0: 2074 7261 6e73 6c61 7469 6f6e 2e68 6173   translation.has
+0000b300: 5f63 6861 6e6e 656c 3a20 7472 616e 736c  _channel: transl
+0000b310: 6174 696f 6e20 3d20 7472 616e 736c 6174  ation = translat
+0000b320: 696f 6e2e 7769 7468 5f63 6861 6e6e 656c  ion.with_channel
+0000b330: 6469 6d28 3120 2d20 7472 616e 736c 6174  dim(1 - translat
+0000b340: 696f 6e2e 6261 7463 685f 6469 6d65 6e73  ion.batch_dimens
+0000b350: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000b360: 2061 766f 7563 6828 7472 616e 736c 6174   avouch(translat
+0000b370: 696f 6e2e 6861 735f 6261 7463 6820 616e  ion.has_batch an
+0000b380: 6420 7472 616e 736c 6174 696f 6e2e 6861  d translation.ha
+0000b390: 735f 6368 616e 6e65 6c2c 2066 2250 6c65  s_channel, f"Ple
+0000b3a0: 6173 6520 7573 6520 6261 746f 7263 6820  ase use batorch 
+0000b3b0: 7465 6e73 6f72 206f 6620 7369 7a65 2028  tensor of size (
+0000b3c0: 5b6e 5f62 6174 6368 5d2c 207b 7b6e 5f64  [n_batch], {{n_d
+0000b3d0: 696d 7d7d 2920 666f 7220 5269 6769 6420  im}}) for Rigid 
+0000b3e0: 7472 616e 736c 6174 696f 6e2c 2069 6e73  translation, ins
+0000b3f0: 7465 6164 206f 6620 7b74 7261 6e73 6c61  tead of {transla
+0000b400: 7469 6f6e 2e73 6861 7065 7d2e 2022 290a  tion.shape}. ").
+0000b410: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0000b420: 5f62 6174 6368 203d 3d20 3120 616e 6420  _batch == 1 and 
+0000b430: 7472 616e 736c 6174 696f 6e2e 6e5f 6261  translation.n_ba
+0000b440: 7463 6820 3e20 313a 206e 5f62 6174 6368  tch > 1: n_batch
+0000b450: 203d 2074 7261 6e73 6c61 7469 6f6e 2e6e   = translation.n
+0000b460: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
+0000b470: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+0000b480: 6f6e 653a 206e 5f64 696d 203d 2074 7261  one: n_dim = tra
+0000b490: 6e73 6c61 7469 6f6e 2e6e 5f63 6861 6e6e  nslation.n_chann
+0000b4a0: 656c 0a20 2020 2020 2020 2020 2020 2065  el.            e
+0000b4b0: 6c73 653a 2061 766f 7563 6828 6e5f 6469  lse: avouch(n_di
+0000b4c0: 6d20 3d3d 2074 7261 6e73 6c61 7469 6f6e  m == translation
+0000b4d0: 2e6e 5f63 6861 6e6e 656c 2c20 2253 7973  .n_channel, "Sys
+0000b4e0: 7465 6d61 7469 6320 6572 726f 722e 2050  tematic error. P
+0000b4f0: 6c65 6173 6520 636f 6e74 6163 7420 7468  lease contact th
+0000b500: 6520 6465 7665 6c6f 7065 7273 2066 6f72  e developers for
+0000b510: 2064 6574 6169 6c73 2028 4572 726f 7220   details (Error 
+0000b520: 436f 6465 3a20 5433 3332 292e 2022 290a  Code: T332). ").
+0000b530: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
+0000b540: 6d20 3d20 7472 616e 736c 6174 696f 6e2e  m = translation.
+0000b550: 6e5f 6368 616e 6e65 6c0a 2020 2020 2020  n_channel.      
+0000b560: 2020 6966 2063 656e 7465 7220 6973 206e    if center is n
+0000b570: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000b580: 2020 2020 2063 656e 7465 7220 3d20 6261       center = ba
+0000b590: 746f 7263 685f 7465 6e73 6f72 2863 656e  torch_tensor(cen
+0000b5a0: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
+0000b5b0: 2069 6620 6365 6e74 6572 2e6e 5f64 696d   if center.n_dim
+0000b5c0: 203c 3d20 3120 616e 6420 6e6f 7420 6365   <= 1 and not ce
+0000b5d0: 6e74 6572 2e68 6173 5f62 6174 6368 3a20  nter.has_batch: 
+0000b5e0: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
+0000b5f0: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
+0000b600: 2020 2020 2020 2020 2020 6966 2063 656e            if cen
+0000b610: 7465 722e 6e5f 6469 6d20 3d3d 2032 2061  ter.n_dim == 2 a
+0000b620: 6e64 206e 6f74 2063 656e 7465 722e 6861  nd not center.ha
+0000b630: 735f 6261 7463 683a 2063 656e 7465 7220  s_batch: center 
+0000b640: 3d20 6365 6e74 6572 2e77 6974 685f 6261  = center.with_ba
+0000b650: 7463 6864 696d 2828 3120 2d20 6365 6e74  tchdim((1 - cent
+0000b660: 6572 2e63 6861 6e6e 656c 5f64 696d 656e  er.channel_dimen
+0000b670: 7369 6f6e 2920 6966 2063 656e 7465 722e  sion) if center.
+0000b680: 6861 735f 6368 616e 6e65 6c20 656c 7365  has_channel else
+0000b690: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+0000b6a0: 6966 2063 656e 7465 722e 6e5f 6469 6d20  if center.n_dim 
+0000b6b0: 3d3d 2032 2061 6e64 206e 6f74 2063 656e  == 2 and not cen
+0000b6c0: 7465 722e 6861 735f 6368 616e 6e65 6c3a  ter.has_channel:
+0000b6d0: 2063 656e 7465 7220 3d20 6365 6e74 6572   center = center
+0000b6e0: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
+0000b6f0: 2831 202d 2063 656e 7465 722e 6261 7463  (1 - center.batc
+0000b700: 685f 6469 6d65 6e73 696f 6e29 0a20 2020  h_dimension).   
+0000b710: 2020 2020 2020 2020 2061 766f 7563 6828           avouch(
+0000b720: 6365 6e74 6572 2e68 6173 5f62 6174 6368  center.has_batch
+0000b730: 2061 6e64 2063 656e 7465 722e 6861 735f   and center.has_
+0000b740: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+0000b750: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+0000b760: 6e73 6f72 206f 6620 7369 7a65 2028 5b6e  nsor of size ([n
+0000b770: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
+0000b780: 7d7d 2920 666f 7220 5269 6769 6420 6365  }}) for Rigid ce
+0000b790: 6e74 6572 2c20 696e 7374 6561 6420 6f66  nter, instead of
+0000b7a0: 207b 6365 6e74 6572 2e73 6861 7065 7d2e   {center.shape}.
+0000b7b0: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+0000b7c0: 6966 206e 5f62 6174 6368 203d 3d20 3120  if n_batch == 1 
+0000b7d0: 616e 6420 6365 6e74 6572 2e6e 5f62 6174  and center.n_bat
+0000b7e0: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
+0000b7f0: 3d20 6365 6e74 6572 2e6e 5f62 6174 6368  = center.n_batch
+0000b800: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b810: 6e5f 6469 6d20 6973 204e 6f6e 653a 206e  n_dim is None: n
+0000b820: 5f64 696d 203d 2063 656e 7465 722e 6e5f  _dim = center.n_
+0000b830: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+0000b840: 2020 2020 656c 7365 3a20 6176 6f75 6368      else: avouch
+0000b850: 286e 5f64 696d 203d 3d20 6365 6e74 6572  (n_dim == center
+0000b860: 2e6e 5f63 6861 6e6e 656c 2c20 6622 4365  .n_channel, f"Ce
+0000b870: 6e74 6572 287b 6365 6e74 6572 2e6e 5f63  nter({center.n_c
+0000b880: 6861 6e6e 656c 7d44 2920 616e 6420 7472  hannel}D) and tr
+0000b890: 616e 736c 6174 696f 6e28 7b6e 5f64 696d  anslation({n_dim
+0000b8a0: 7d44 2920 696e 2074 7261 6e73 2e52 6967  }D) in trans.Rig
+0000b8b0: 6964 2073 686f 756c 6420 6861 7665 2074  id should have t
+0000b8c0: 6865 2073 616d 6520 6469 6d65 6e73 696f  he same dimensio
+0000b8d0: 6e2e 2022 290a 2020 2020 2020 2020 2020  n. ").          
+0000b8e0: 2020 6e5f 6469 6d20 3d20 6365 6e74 6572    n_dim = center
+0000b8f0: 2e6e 5f63 6861 6e6e 656c 0a20 2020 2020  .n_channel.     
+0000b900: 2020 2069 6620 6178 6973 2069 7320 6e6f     if axis is no
+0000b910: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b920: 2020 2020 6178 6973 203d 2062 6174 6f72      axis = bator
+0000b930: 6368 5f74 656e 736f 7228 6178 6973 290a  ch_tensor(axis).
+0000b940: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0000b950: 7869 732e 6e5f 6469 6d20 3c3d 2031 2061  xis.n_dim <= 1 a
+0000b960: 6e64 206e 6f74 2061 7869 732e 6861 735f  nd not axis.has_
+0000b970: 6261 7463 683a 2061 7869 7320 3d20 6178  batch: axis = ax
+0000b980: 6973 2e75 6e73 7175 6565 7a65 285b 5d29  is.unsqueeze([])
+0000b990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b9a0: 6178 6973 2e6e 5f64 696d 203d 3d20 3220  axis.n_dim == 2 
+0000b9b0: 616e 6420 6e6f 7420 6178 6973 2e68 6173  and not axis.has
+0000b9c0: 5f62 6174 6368 3a20 6178 6973 203d 2061  _batch: axis = a
+0000b9d0: 7869 732e 7769 7468 5f62 6174 6368 6469  xis.with_batchdi
+0000b9e0: 6d28 2831 202d 2061 7869 732e 6368 616e  m((1 - axis.chan
+0000b9f0: 6e65 6c5f 6469 6d65 6e73 696f 6e29 2069  nel_dimension) i
+0000ba00: 6620 6178 6973 2e68 6173 5f63 6861 6e6e  f axis.has_chann
+0000ba10: 656c 2065 6c73 6520 3029 0a20 2020 2020  el else 0).     
+0000ba20: 2020 2020 2020 2069 6620 6178 6973 2e6e         if axis.n
+0000ba30: 5f64 696d 203d 3d20 3220 616e 6420 6e6f  _dim == 2 and no
+0000ba40: 7420 6178 6973 2e68 6173 5f63 6861 6e6e  t axis.has_chann
+0000ba50: 656c 3a20 6178 6973 203d 2061 7869 732e  el: axis = axis.
+0000ba60: 7769 7468 5f63 6861 6e6e 656c 6469 6d28  with_channeldim(
+0000ba70: 3120 2d20 6178 6973 2e62 6174 6368 5f64  1 - axis.batch_d
+0000ba80: 696d 656e 7369 6f6e 290a 2020 2020 2020  imension).      
+0000ba90: 2020 2020 2020 6176 6f75 6368 2861 7869        avouch(axi
+0000baa0: 732e 6861 735f 6261 7463 6820 616e 6420  s.has_batch and 
+0000bab0: 6178 6973 2e68 6173 5f63 6861 6e6e 656c  axis.has_channel
+0000bac0: 2c20 6622 506c 6561 7365 2075 7365 2062  , f"Please use b
+0000bad0: 6174 6f72 6368 2074 656e 736f 7220 6f66  atorch tensor of
+0000bae0: 2073 697a 6520 285b 6e5f 6261 7463 685d   size ([n_batch]
+0000baf0: 2c20 7b7b 6e5f 6469 6d7d 7d29 2066 6f72  , {{n_dim}}) for
+0000bb00: 2052 6967 6964 2061 7869 7365 732c 2069   Rigid axises, i
+0000bb10: 6e73 7465 6164 206f 6620 7b61 7869 732e  nstead of {axis.
+0000bb20: 7368 6170 657d 2e20 2229 0a20 2020 2020  shape}. ").     
+0000bb30: 2020 2020 2020 2069 6620 2828 6178 6973         if ((axis
+0000bb40: 2e6e 6f72 6d28 2920 2d20 3129 202a 2a20  .norm() - 1) ** 
+0000bb50: 3229 2e73 756d 2829 2e73 756d 2829 203e  2).sum().sum() >
+0000bb60: 3d20 3165 2d34 3a0a 2020 2020 2020 2020  = 1e-4:.        
+0000bb70: 2020 2020 2020 2020 7072 696e 7428 2277          print("w
+0000bb80: 6172 6e69 6e67 3a20 7061 7261 6d2e 2061  arning: param. a
+0000bb90: 7869 7365 7320 666f 7220 2752 6967 6964  xises for 'Rigid
+0000bba0: 2720 7472 616e 7366 6f72 6d61 7469 6f6e  ' transformation
+0000bbb0: 2073 686f 756c 6420 6265 206e 6f72 6d2d   should be norm-
+0000bbc0: 3120 7665 6374 6f72 732c 2061 7574 6f2d  1 vectors, auto-
+0000bbd0: 6e6f 726d 616c 697a 6174 696f 6e20 776f  normalization wo
+0000bbe0: 756c 6420 6265 2070 6572 666f 726d 6564  uld be performed
+0000bbf0: 2e20 506c 6561 7365 2063 6f6e 7461 6374  . Please contact
+0000bc00: 2074 6865 2064 6576 656c 6f70 6572 7320   the developers 
+0000bc10: 6966 206e 6563 6573 7361 7279 2028 4572  if necessary (Er
+0000bc20: 726f 7220 436f 6465 3a20 5433 3331 292e  ror Code: T331).
+0000bc30: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+0000bc40: 2020 2020 6178 6973 203d 2061 7869 7320      axis = axis 
+0000bc50: 2f20 6178 6973 2e6e 6f72 6d28 290a 2020  / axis.norm().  
+0000bc60: 2020 2020 2020 2020 2020 6966 206e 5f62            if n_b
+0000bc70: 6174 6368 203d 3d20 3120 616e 6420 6178  atch == 1 and ax
+0000bc80: 6973 2e6e 5f62 6174 6368 203e 2031 3a20  is.n_batch > 1: 
+0000bc90: 6e5f 6261 7463 6820 3d20 6178 6973 2e6e  n_batch = axis.n
+0000bca0: 5f62 6174 6368 0a20 2020 2020 2020 2020  _batch.         
+0000bcb0: 2020 2069 6620 6e5f 6469 6d20 6973 204e     if n_dim is N
+0000bcc0: 6f6e 653a 206e 5f64 696d 203d 2061 7869  one: n_dim = axi
+0000bcd0: 732e 6e5f 6368 616e 6e65 6c0a 2020 2020  s.n_channel.    
+0000bce0: 2020 2020 2020 2020 656c 7365 3a20 6176          else: av
+0000bcf0: 6f75 6368 286e 5f64 696d 203d 3d20 6178  ouch(n_dim == ax
+0000bd00: 6973 2e6e 5f63 6861 6e6e 656c 2c20 6622  is.n_channel, f"
+0000bd10: 5472 616e 736c 6174 696f 6e28 7b6e 5f64  Translation({n_d
+0000bd20: 696d 7d44 2920 616e 6420 6178 6973 6573  im}D) and axises
+0000bd30: 287b 6178 6973 2e6e 5f63 6861 6e6e 656c  ({axis.n_channel
+0000bd40: 7d44 2929 2069 6e20 7472 616e 732e 5269  }D)) in trans.Ri
+0000bd50: 6769 6420 7368 6f75 6c64 2068 6176 6520  gid should have 
+0000bd60: 7468 6520 7361 6d65 2064 696d 656e 7369  the same dimensi
+0000bd70: 6f6e 2e20 2229 0a20 2020 2020 2020 2069  on. ").        i
+0000bd80: 6620 6e5f 6469 6d20 6973 204e 6f6e 653a  f n_dim is None:
+0000bd90: 206e 5f64 696d 203d 2032 2069 6620 6178   n_dim = 2 if ax
+0000bda0: 6973 2069 7320 4e6f 6e65 2065 6c73 6520  is is None else 
+0000bdb0: 330a 2020 2020 2020 2020 6966 2074 7261  3.        if tra
+0000bdc0: 6e73 6c61 7469 6f6e 2069 7320 4e6f 6e65  nslation is None
+0000bdd0: 3a20 7472 616e 736c 6174 696f 6e20 3d20  : translation = 
+0000bde0: 6274 2e7a 6572 6f73 285b 6e5f 6261 7463  bt.zeros([n_batc
+0000bdf0: 685d 2c20 7b6e 5f64 696d 7d29 0a20 2020  h], {n_dim}).   
+0000be00: 2020 2020 2069 6620 6365 6e74 6572 2069       if center i
+0000be10: 7320 4e6f 6e65 3a20 6365 6e74 6572 203d  s None: center =
+0000be20: 2062 742e 7a65 726f 7328 5b6e 5f62 6174   bt.zeros([n_bat
+0000be30: 6368 5d2c 207b 6e5f 6469 6d7d 290a 2020  ch], {n_dim}).  
+0000be40: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000be50: 204e 6f77 2077 6520 6372 6561 7465 2074   Now we create t
+0000be60: 6865 206d 6174 7269 780a 2020 2020 2020  he matrix.      
+0000be70: 2020 616e 676c 6520 3d20 616e 676c 652e    angle = angle.
+0000be80: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
+0000be90: 6365 6e74 6572 203d 2063 656e 7465 722e  center = center.
+0000bea0: 666c 6f61 7428 290a 2020 2020 2020 2020  float().        
+0000beb0: 7472 616e 736c 6174 696f 6e20 3d20 7472  translation = tr
+0000bec0: 616e 736c 6174 696f 6e2e 666c 6f61 7428  anslation.float(
+0000bed0: 290a 2020 2020 2020 2020 6966 206e 5f64  ).        if n_d
+0000bee0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
+0000bef0: 2020 2020 2041 203d 2062 742e 7374 6163       A = bt.stac
+0000bf00: 6b28 6274 2e63 6f73 2861 6e67 6c65 292c  k(bt.cos(angle),
+0000bf10: 2062 742e 7369 6e28 616e 676c 6529 2c20   bt.sin(angle), 
+0000bf20: 2d62 742e 7369 6e28 616e 676c 6529 2c20  -bt.sin(angle), 
+0000bf30: 6274 2e63 6f73 2861 6e67 6c65 292c 202d  bt.cos(angle), -
+0000bf40: 3129 2e73 706c 6974 6469 6d28 2d31 2c20  1).splitdim(-1, 
+0000bf50: 322c 2032 290a 2020 2020 2020 2020 656c  2, 2).        el
+0000bf60: 6966 206e 5f64 696d 203d 3d20 333a 0a20  if n_dim == 3:. 
+0000bf70: 2020 2020 2020 2020 2020 2061 7869 7320             axis 
+0000bf80: 3d20 6178 6973 2e66 6c6f 6174 2829 0a20  = axis.float(). 
+0000bf90: 2020 2020 2020 2020 2020 2041 203d 2062             A = b
+0000bfa0: 742e 6579 6528 5b6e 5f62 6174 6368 5d2c  t.eye([n_batch],
+0000bfb0: 206e 5f64 696d 2920 2b20 2831 202d 2062   n_dim) + (1 - b
+0000bfc0: 742e 636f 7328 616e 676c 6529 2920 2a20  t.cos(angle)) * 
+0000bfd0: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
+0000bfe0: 6178 6973 2920 4020 6274 2e63 726f 7373  axis) @ bt.cross
+0000bff0: 5f6d 6174 7269 7828 6178 6973 2920 2b20  _matrix(axis) + 
+0000c000: 6274 2e73 696e 2861 6e67 6c65 2920 2a20  bt.sin(angle) * 
+0000c010: 6274 2e63 726f 7373 5f6d 6174 7269 7828  bt.cross_matrix(
+0000c020: 6178 6973 290a 2020 2020 2020 2020 656c  axis).        el
+0000c030: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c040: 7261 6973 6520 4572 726f 7228 224e 6f74  raise Error("Not
+0000c050: 496d 706c 656d 656e 7465 6422 2928 6622  Implemented")(f"
+0000c060: 5269 6769 6420 7472 616e 7366 6f72 6d61  Rigid transforma
+0000c070: 7469 6f6e 2069 6e20 6d69 636f 6d70 7574  tion in micomput
+0000c080: 696e 6720 646f 6573 206e 6f74 2073 7570  ing does not sup
+0000c090: 706f 7274 207b 6e5f 6469 6d7d 2064 696d  port {n_dim} dim
+0000c0a0: 656e 7369 6f6e 616c 2074 7261 6e73 666f  ensional transfo
+0000c0b0: 726d 7320 2832 2026 2033 4420 6f6e 6c79  rms (2 & 3D only
+0000c0c0: 292e 2022 202b 200a 2020 2020 2020 2020  ). " + .        
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2250 6c65 6173 6520 636f 6e74 6163 7420  "Please contact 
+0000c100: 7468 6520 6465 7665 6c6f 7065 7273 2069  the developers i
+0000c110: 6620 7468 6572 6520 6172 6520 6665 6173  f there are feas
+0000c120: 6962 6c65 2061 6c67 6f72 6974 686d 7320  ible algorithms 
+0000c130: 2845 7272 6f72 2043 6f64 653a 2054 3333  (Error Code: T33
+0000c140: 3329 2e20 5468 616e 6b20 796f 752e 2022  3). Thank you. "
+0000c150: 290a 2020 2020 2020 2020 6d61 7472 6978  ).        matrix
+0000c160: 203d 2062 742e 6361 7428 6274 2e63 6174   = bt.cat(bt.cat
+0000c170: 2841 2c20 2828 7472 616e 736c 6174 696f  (A, ((translatio
+0000c180: 6e20 2b20 6365 6e74 6572 292e 7769 7468  n + center).with
+0000c190: 5f63 6861 6e6e 656c 6469 6d28 4e6f 6e65  _channeldim(None
+0000c1a0: 2920 2d20 4120 4020 6365 6e74 6572 2e77  ) - A @ center.w
+0000c1b0: 6974 685f 6368 616e 6e65 6c64 696d 284e  ith_channeldim(N
+0000c1c0: 6f6e 6529 292e 756e 7371 7565 657a 6528  one)).unsqueeze(
+0000c1d0: 2d31 292c 202d 3129 2c20 0a20 2020 2020  -1), -1), .     
+0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1f0: 2020 2062 742e 6361 7428 6274 2e7a 6572     bt.cat(bt.zer
+0000c200: 6f73 286e 5f64 696d 292c 2062 742e 6f6e  os(n_dim), bt.on
+0000c210: 6573 2831 2929 2e75 6e73 7175 6565 7a65  es(1)).unsqueeze
+0000c220: 285b 5d2c 2031 292c 2031 290a 2020 2020  ([], 1), 1).    
+0000c230: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
+0000c240: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
+0000c250: 3a20 6d61 7472 6978 5b2e 2e2e 2c20 3a6e  : matrix[..., :n
+0000c260: 5f64 696d 2c20 2d31 5d20 2a3d 2074 7261  _dim, -1] *= tra
+0000c270: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
+0000c280: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+0000c290: 616e 6365 2873 7061 6369 6e67 2c20 7475  ance(spacing, tu
+0000c2a0: 706c 6529 3a20 7370 6163 696e 6720 3d20  ple): spacing = 
+0000c2b0: 746f 5f74 7570 6c65 2873 7061 6369 6e67  to_tuple(spacing
+0000c2c0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+0000c2d0: 2873 7061 6369 6e67 2920 3d3d 2031 3a20  (spacing) == 1: 
+0000c2e0: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
+0000c2f0: 6720 2a20 6e5f 6469 6d0a 2020 2020 2020  g * n_dim.      
+0000c300: 2020 4120 3d20 6274 2e64 6961 6728 6261    A = bt.diag(ba
+0000c310: 746f 7263 685f 7465 6e73 6f72 286c 6973  torch_tensor(lis
+0000c320: 7428 7370 6163 696e 6729 202b 205b 312e  t(spacing) + [1.
+0000c330: 5d29 292e 756e 7371 7565 657a 6528 5b5d  ])).unsqueeze([]
+0000c340: 292e 6173 7479 7065 286d 6174 7269 7829  ).astype(matrix)
+0000c350: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000c360: 2e5f 5f69 6e69 745f 5f28 616e 676c 652c  .__init__(angle,
+0000c370: 2061 7869 732c 2074 7261 6e73 6c61 7469   axis, translati
+0000c380: 6f6e 2c20 6365 6e74 6572 3d63 656e 7465  on, center=cente
+0000c390: 722c 2074 7261 6e73 5f73 7472 6574 6368  r, trans_stretch
+0000c3a0: 3d74 7261 6e73 5f73 7472 6574 6368 2c20  =trans_stretch, 
+0000c3b0: 7370 6163 696e 673d 7370 6163 696e 6729  spacing=spacing)
+0000c3c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+0000c3d0: 5f64 696d 203d 206e 5f64 696d 0a20 2020  _dim = n_dim.   
+0000c3e0: 2020 2020 2073 656c 662e 7472 616e 735f       self.trans_
+0000c3f0: 7374 7265 7463 6820 3d20 7472 616e 735f  stretch = trans_
+0000c400: 7374 7265 7463 680a 2020 2020 2020 2020  stretch.        
+0000c410: 7365 6c66 2e73 7061 6369 6e67 203d 2073  self.spacing = s
+0000c420: 7061 6369 6e67 0a20 2020 2020 2020 2073  pacing.        s
+0000c430: 656c 662e 6d61 7472 6978 203d 2041 2e69  elf.matrix = A.i
+0000c440: 6e76 2829 2040 206d 6174 7269 7820 4020  nv() @ matrix @ 
+0000c450: 410a 2020 2020 2020 2020 7365 6c66 2e62  A.        self.b
+0000c460: 6174 6368 5f70 6172 616d 2e61 7070 656e  atch_param.appen
+0000c470: 6428 276d 6174 7269 7827 290a 0a20 2020  d('matrix')..   
+0000c480: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+0000c490: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
+0000c4a0: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
+0000c4b0: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
+0000c4c0: 6d61 7472 6978 203d 2073 656c 662e 6d61  matrix = self.ma
+0000c4d0: 7472 6978 0a20 2020 2020 2020 206e 5f64  trix.        n_d
+0000c4e0: 696d 203d 2073 656c 662e 6e5f 6469 6d0a  im = self.n_dim.
+0000c4f0: 2020 2020 2020 2020 4120 3d20 6d61 7472          A = matr
+0000c500: 6978 5b3a 2c20 3a6e 5f64 696d 2c20 3a6e  ix[:, :n_dim, :n
+0000c510: 5f64 696d 5d0a 2020 2020 2020 2020 6220  _dim].        b 
+0000c520: 3d20 6d61 7472 6978 5b3a 2c20 3a6e 5f64  = matrix[:, :n_d
+0000c530: 696d 2c20 6e5f 6469 6d5d 0a20 2020 2020  im, n_dim].     
+0000c540: 2020 2073 6861 7065 203d 2058 2e73 6861     shape = X.sha
+0000c550: 7065 0a20 2020 2020 2020 2059 203d 2028  pe.        Y = (
+0000c560: 4120 4020 582e 666c 6174 7465 6e28 292e  A @ X.flatten().
+0000c570: 6368 616e 6e65 6c5f 6469 6d5f 284e 6f6e  channel_dim_(Non
+0000c580: 6529 202b 2062 2e75 6e73 7175 6565 7a65  e) + b.unsqueeze
+0000c590: 282d 3129 292e 7669 6577 2873 6861 7065  (-1)).view(shape
+0000c5a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000c5b0: 2059 0a20 2020 200a 2020 2020 6465 6620   Y.    .    def 
+0000c5c0: 6166 6669 6e65 2873 656c 662c 206e 5f64  affine(self, n_d
+0000c5d0: 696d 3d4e 6f6e 6529 3a0a 2020 2020 2020  im=None):.      
+0000c5e0: 2020 6176 6f75 6368 286e 5f64 696d 2069    avouch(n_dim i
+0000c5f0: 7320 4e6f 6e65 206f 7220 7365 6c66 2e6e  s None or self.n
+0000c600: 5f64 696d 203d 3d20 6e5f 6469 6d29 0a20  _dim == n_dim). 
+0000c610: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c620: 6c66 2e6d 6174 7269 7820 6966 2073 656c  lf.matrix if sel
+0000c630: 662e 6261 636b 7761 7264 2065 6c73 6520  f.backward else 
+0000c640: 7365 6c66 2e6d 6174 7269 782e 696e 7628  self.matrix.inv(
+0000c650: 290a 0a20 2020 2064 6566 2069 6e76 2873  )..    def inv(s
+0000c660: 656c 6629 3a0a 2020 2020 2020 2020 4120  elf):.        A 
+0000c670: 3d20 6274 2e64 6961 6728 6261 746f 7263  = bt.diag(batorc
+0000c680: 685f 7465 6e73 6f72 286c 6973 7428 7365  h_tensor(list(se
+0000c690: 6c66 2e73 7061 6369 6e67 2920 2b20 5b31  lf.spacing) + [1
+0000c6a0: 2e5d 2929 2e75 6e73 7175 6565 7a65 285b  .])).unsqueeze([
+0000c6b0: 5d29 2e61 7374 7970 6528 7365 6c66 2e6d  ]).astype(self.m
+0000c6c0: 6174 7269 7829 0a20 2020 2020 2020 2072  atrix).        r
+0000c6d0: 6574 7572 6e20 5269 6769 6428 4120 4020  eturn Rigid(A @ 
+0000c6e0: 6274 2e69 6e76 2873 656c 662e 6d61 7472  bt.inv(self.matr
+0000c6f0: 6978 2920 4020 412e 696e 7628 292c 2074  ix) @ A.inv(), t
+0000c700: 7261 6e73 5f73 7472 6574 6368 203d 2031  rans_stretch = 1
+0000c710: 2c20 7370 6163 696e 673d 7365 6c66 2e73  , spacing=self.s
+0000c720: 7061 6369 6e67 292e 6261 636b 7761 7264  pacing).backward
+0000c730: 5f28 7365 6c66 2e62 6163 6b77 6172 6429  _(self.backward)
+0000c740: 0a0a 4061 6c69 6173 2822 4166 6622 290a  ..@alias("Aff").
+0000c750: 636c 6173 7320 4166 6669 6e65 2853 7061  class Affine(Spa
+0000c760: 7469 616c 5472 616e 7366 6f72 6d61 7469  tialTransformati
+0000c770: 6f6e 293a 0a20 2020 2064 6566 205f 5f69  on):.    def __i
+0000c780: 6e69 745f 5f28 7365 6c66 2c20 6d61 7472  nit__(self, matr
+0000c790: 6978 2c20 7472 616e 735f 7374 7265 7463  ix, trans_stretc
+0000c7a0: 683d 4e6f 6e65 2c20 7370 6163 696e 673d  h=None, spacing=
+0000c7b0: 3129 3a0a 2020 2020 2020 2020 2727 270a  1):.        '''.
+0000c7c0: 2020 2020 2020 2020 4166 6669 6e65 2074          Affine t
+0000c7d0: 7261 6e73 666f 726d 6174 696f 6e20 7769  ransformation wi
+0000c7e0: 7468 2072 6573 7065 6374 2074 6f20 7472  th respect to tr
+0000c7f0: 616e 7366 6f72 6d61 7469 6f6e 206d 6174  ansformation mat
+0000c800: 7269 782e 0a20 2020 2020 2020 200a 2020  rix..        .  
+0000c810: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
+0000c820: 2020 2020 2020 2020 2020 6d61 7472 6978            matrix
+0000c830: 205b 6274 2e54 656e 736f 7220 6f72 206e   [bt.Tensor or n
+0000c840: 702e 6e75 6d70 795d 3a20 7468 6520 6166  p.numpy]: the af
+0000c850: 6669 6e65 206d 6174 7269 782e 200a 2020  fine matrix. .  
+0000c860: 2020 2020 2020 2020 2020 2020 2020 7369                si
+0000c870: 7a65 3a20 285b 6e5f 6261 7463 685d 2c20  ze: ([n_batch], 
+0000c880: 6e5f 6469 6d20 2b20 312c 206e 5f64 696d  n_dim + 1, n_dim
+0000c890: 202b 2031 290a 2020 2020 2020 2020 2020   + 1).          
+0000c8a0: 2020 7472 616e 735f 7374 7265 7463 6820    trans_stretch 
+0000c8b0: 5b69 6e74 5d3a 206f 6e6c 7920 7573 6564  [int]: only used
+0000c8c0: 2066 6f72 2069 7465 7261 7469 7665 2070   for iterative p
+0000c8d0: 6172 616d 6574 6572 2074 7261 696e 696e  arameter trainin
+0000c8e0: 672c 2031 2062 7920 6465 6661 756c 742e  g, 1 by default.
+0000c8f0: 2032 3020 7365 656d 7320 746f 2062 6520   20 seems to be 
+0000c900: 6120 676f 6f64 2063 686f 6963 652e 200a  a good choice. .
+0000c910: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000c920: 2020 2020 2057 6865 6e20 6974 2069 7320       When it is 
+0000c930: 6361 6c6c 6564 3a0a 2020 2020 2020 2020  called:.        
+0000c940: 2020 2020 5820 5b62 742e 5465 6e73 6f72      X [bt.Tensor
+0000c950: 5d3a 2043 6f6f 7264 696e 6174 6573 2074  ]: Coordinates t
+0000c960: 6f20 6265 2074 7261 6e73 666f 726d 6564  o be transformed
+0000c970: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c980: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+0000c990: 683a 206f 7074 696f 6e61 6c5d 2c20 7b6e  h: optional], {n
+0000c9a0: 5f64 696d 7d2c 206e 5f31 2c20 6e5f 322c  _dim}, n_1, n_2,
+0000c9b0: 202e 2e2e 2c20 6e5f 7229 0a20 2020 2020   ..., n_r).     
+0000c9c0: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
+0000c9d0: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
+0000c9e0: 7261 6e73 666f 726d 6564 2063 6f6f 7264  ransformed coord
+0000c9f0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
+0000ca00: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+0000ca10: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+0000ca20: 7d2c 206e 5f31 2c20 6e5f 322c 202e 2e2e  }, n_1, n_2, ...
+0000ca30: 2c20 6e5f 7229 0a20 2020 2020 2020 2027  , n_r).        '
+0000ca40: 2727 0a20 2020 2020 2020 206d 6174 7269  ''.        matri
+0000ca50: 7820 3d20 6261 746f 7263 685f 7465 6e73  x = batorch_tens
+0000ca60: 6f72 286d 6174 7269 7829 0a20 2020 2020  or(matrix).     
+0000ca70: 2020 206e 5f64 696d 203d 206d 6174 7269     n_dim = matri
+0000ca80: 782e 7369 7a65 282d 3129 202d 2031 0a20  x.size(-1) - 1. 
+0000ca90: 2020 2020 2020 2069 6620 6d61 7472 6978         if matrix
+0000caa0: 2e6e 5f64 696d 203c 3d20 3220 616e 6420  .n_dim <= 2 and 
+0000cab0: 6e6f 7420 6d61 7472 6978 2e68 6173 5f62  not matrix.has_b
+0000cac0: 6174 6368 3a20 6d61 7472 6978 203d 206d  atch: matrix = m
+0000cad0: 6174 7269 782e 756e 7371 7565 657a 6528  atrix.unsqueeze(
+0000cae0: 5b5d 290a 2020 2020 2020 2020 6966 206d  []).        if m
+0000caf0: 6174 7269 782e 6e5f 6469 6d20 3d3d 2033  atrix.n_dim == 3
+0000cb00: 2061 6e64 206e 6f74 206d 6174 7269 782e   and not matrix.
+0000cb10: 6861 735f 6261 7463 6820 616e 6420 6d61  has_batch and ma
+0000cb20: 7472 6978 2e73 6861 7065 5b31 5d20 3d3d  trix.shape[1] ==
+0000cb30: 206d 6174 7269 782e 7368 6170 655b 325d   matrix.shape[2]
+0000cb40: 3a20 6d61 7472 6978 2e62 6174 6368 5f64  : matrix.batch_d
+0000cb50: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+0000cb60: 2020 2020 2061 766f 7563 6828 6d61 7472       avouch(matr
+0000cb70: 6978 2e68 6173 5f62 6174 6368 2c20 6622  ix.has_batch, f"
+0000cb80: 506c 6561 7365 2075 7365 2062 6174 6f72  Please use bator
+0000cb90: 6368 2074 656e 736f 7220 6f66 2073 697a  ch tensor of siz
+0000cba0: 6520 285b 6e5f 6261 7463 685d 2c20 6e5f  e ([n_batch], n_
+0000cbb0: 6469 6d20 2b20 312c 206e 5f64 696d 202b  dim + 1, n_dim +
+0000cbc0: 2031 2920 666f 7220 4166 6669 6e65 2070   1) for Affine p
+0000cbd0: 6172 616d 6574 6572 732c 2069 6e73 7465  arameters, inste
+0000cbe0: 6164 206f 6620 7b6d 6174 7269 782e 7368  ad of {matrix.sh
+0000cbf0: 6170 657d 2e20 2229 0a20 2020 2020 2020  ape}. ").       
+0000cc00: 2069 6620 7472 616e 735f 7374 7265 7463   if trans_stretc
+0000cc10: 6820 6973 206e 6f74 204e 6f6e 653a 206d  h is not None: m
+0000cc20: 6174 7269 785b 2e2e 2e2c 203a 6e5f 6469  atrix[..., :n_di
+0000cc30: 6d2c 202d 315d 202a 3d20 7472 616e 735f  m, -1] *= trans_
+0000cc40: 7374 7265 7463 680a 2020 2020 2020 2020  stretch.        
+0000cc50: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000cc60: 6528 7370 6163 696e 672c 2074 7570 6c65  e(spacing, tuple
+0000cc70: 293a 2073 7061 6369 6e67 203d 2074 6f5f  ): spacing = to_
+0000cc80: 7475 706c 6528 7370 6163 696e 6729 0a20  tuple(spacing). 
+0000cc90: 2020 2020 2020 2069 6620 6c65 6e28 7370         if len(sp
+0000cca0: 6163 696e 6729 203d 3d20 313a 2073 7061  acing) == 1: spa
+0000ccb0: 6369 6e67 203d 2073 7061 6369 6e67 202a  cing = spacing *
+0000ccc0: 206e 5f64 696d 0a20 2020 2020 2020 2041   n_dim.        A
+0000ccd0: 203d 2062 742e 6469 6167 2862 6174 6f72   = bt.diag(bator
+0000cce0: 6368 5f74 656e 736f 7228 6c69 7374 2873  ch_tensor(list(s
+0000ccf0: 7061 6369 6e67 2920 2b20 5b31 2e5d 2929  pacing) + [1.]))
+0000cd00: 2e75 6e73 7175 6565 7a65 285b 5d29 2e61  .unsqueeze([]).a
+0000cd10: 7374 7970 6528 6d61 7472 6978 290a 2020  stype(matrix).  
+0000cd20: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+0000cd30: 696e 6974 5f5f 286d 6174 7269 782c 2074  init__(matrix, t
+0000cd40: 7261 6e73 5f73 7472 6574 6368 3d74 7261  rans_stretch=tra
+0000cd50: 6e73 5f73 7472 6574 6368 2c20 7370 6163  ns_stretch, spac
+0000cd60: 696e 673d 7370 6163 696e 6729 0a0a 2020  ing=spacing)..  
+0000cd70: 2020 2020 2020 7365 6c66 2e6e 5f64 696d        self.n_dim
+0000cd80: 203d 206d 6174 7269 782e 7369 7a65 282d   = matrix.size(-
+0000cd90: 3129 202d 2031 0a20 2020 2020 2020 2073  1) - 1.        s
+0000cda0: 656c 662e 7472 616e 735f 7374 7265 7463  elf.trans_stretc
+0000cdb0: 6820 3d20 7472 616e 735f 7374 7265 7463  h = trans_stretc
+0000cdc0: 680a 2020 2020 2020 2020 7365 6c66 2e73  h.        self.s
+0000cdd0: 7061 6369 6e67 203d 2073 7061 6369 6e67  pacing = spacing
+0000cde0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+0000cdf0: 7472 6978 203d 2041 2e69 6e76 2829 2040  trix = A.inv() @
+0000ce00: 206d 6174 7269 7820 4020 410a 2020 2020   matrix @ A.    
+0000ce10: 2020 2020 7365 6c66 2e62 6174 6368 5f70      self.batch_p
+0000ce20: 6172 616d 2e61 7070 656e 6428 276d 6174  aram.append('mat
+0000ce30: 7269 7827 290a 0a20 2020 2064 6566 205f  rix')..    def _
+0000ce40: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+0000ce50: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
+0000ce60: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
+0000ce70: 290a 2020 2020 2020 2020 6d61 7472 6978  ).        matrix
+0000ce80: 203d 2073 656c 662e 6d61 7472 6978 2e66   = self.matrix.f
+0000ce90: 6c6f 6174 2829 0a20 2020 2020 2020 206e  loat().        n
+0000cea0: 5f64 696d 203d 2073 656c 662e 6e5f 6469  _dim = self.n_di
+0000ceb0: 6d0a 2020 2020 2020 2020 4120 3d20 6d61  m.        A = ma
+0000cec0: 7472 6978 5b3a 2c20 3a6e 5f64 696d 2c20  trix[:, :n_dim, 
+0000ced0: 3a6e 5f64 696d 5d0a 2020 2020 2020 2020  :n_dim].        
+0000cee0: 6220 3d20 6d61 7472 6978 5b3a 2c20 3a6e  b = matrix[:, :n
+0000cef0: 5f64 696d 2c20 6e5f 6469 6d5d 0a20 2020  _dim, n_dim].   
+0000cf00: 2020 2020 2073 6861 7065 203d 2058 2e73       shape = X.s
+0000cf10: 6861 7065 0a20 2020 2020 2020 2059 203d  hape.        Y =
+0000cf20: 2028 4120 4020 582e 666c 6174 7465 6e28   (A @ X.flatten(
+0000cf30: 292e 6368 616e 6e65 6c5f 6469 6d5f 284e  ).channel_dim_(N
+0000cf40: 6f6e 6529 202b 2062 2e75 6e73 7175 6565  one) + b.unsquee
+0000cf50: 7a65 282d 3129 292e 7669 6577 2873 6861  ze(-1)).view(sha
+0000cf60: 7065 290a 2020 2020 2020 2020 7265 7475  pe).        retu
+0000cf70: 726e 2059 0a20 2020 200a 2020 2020 6465  rn Y.    .    de
+0000cf80: 6620 6166 6669 6e65 2873 656c 662c 206e  f affine(self, n
+0000cf90: 5f64 696d 3d4e 6f6e 6529 3a0a 2020 2020  _dim=None):.    
+0000cfa0: 2020 2020 6176 6f75 6368 286e 5f64 696d      avouch(n_dim
+0000cfb0: 2069 7320 4e6f 6e65 206f 7220 7365 6c66   is None or self
+0000cfc0: 2e6e 5f64 696d 203d 3d20 6e5f 6469 6d29  .n_dim == n_dim)
+0000cfd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cfe0: 7365 6c66 2e6d 6174 7269 7820 6966 2073  self.matrix if s
+0000cff0: 656c 662e 6261 636b 7761 7264 2065 6c73  elf.backward els
+0000d000: 6520 7365 6c66 2e6d 6174 7269 782e 696e  e self.matrix.in
+0000d010: 7628 290a 0a20 2020 2064 6566 2069 6e76  v()..    def inv
+0000d020: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d030: 4120 3d20 6274 2e64 6961 6728 6261 746f  A = bt.diag(bato
+0000d040: 7263 685f 7465 6e73 6f72 286c 6973 7428  rch_tensor(list(
+0000d050: 7365 6c66 2e73 7061 6369 6e67 2920 2b20  self.spacing) + 
+0000d060: 5b31 2e5d 2929 2e75 6e73 7175 6565 7a65  [1.])).unsqueeze
+0000d070: 285b 5d29 2e61 7374 7970 6528 7365 6c66  ([]).astype(self
+0000d080: 2e6d 6174 7269 7829 0a20 2020 2020 2020  .matrix).       
+0000d090: 2072 6574 7572 6e20 4166 6669 6e65 2841   return Affine(A
+0000d0a0: 2040 2062 742e 696e 7628 7365 6c66 2e6d   @ bt.inv(self.m
+0000d0b0: 6174 7269 7829 2040 2041 2e69 6e76 2829  atrix) @ A.inv()
+0000d0c0: 2c20 7472 616e 735f 7374 7265 7463 6820  , trans_stretch 
+0000d0d0: 3d20 312c 2073 7061 6369 6e67 3d73 656c  = 1, spacing=sel
+0000d0e0: 662e 7370 6163 696e 6729 2e62 6163 6b77  f.spacing).backw
+0000d0f0: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+0000d100: 7264 290a 0a40 616c 6961 7328 226c 6f67  rd)..@alias("log
+0000d110: 4575 2229 0a63 6c61 7373 2050 6f6c 7941  Eu").class PolyA
+0000d120: 6666 696e 6528 5370 6174 6961 6c54 7261  ffine(SpatialTra
+0000d130: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+0000d140: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000d150: 656c 662c 2064 6d61 7472 6963 6573 2c20  elf, dmatrices, 
+0000d160: 6d61 736b 732c 206f 7264 6572 3d32 2c20  masks, order=2, 
+0000d170: 6973 5f69 6e76 3d46 616c 7365 2c20 7472  is_inv=False, tr
+0000d180: 616e 735f 7374 7265 7463 683d 4e6f 6e65  ans_stretch=None
+0000d190: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
+0000d1a0: 2020 2020 2020 2050 6f6c 7920 6166 6669         Poly affi
+0000d1b0: 6e65 2074 7261 6e73 666f 726d 6174 696f  ne transformatio
+0000d1c0: 6e20 7769 7468 2072 6573 7065 6374 2074  n with respect t
+0000d1d0: 6f20 7472 616e 7366 6f72 6d61 7469 6f6e  o transformation
+0000d1e0: 206d 6174 7269 6365 7320 5b31 5d2e 0a20   matrices [1].. 
+0000d1f0: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+0000d200: 2064 6d61 7472 6963 6573 2066 6f72 2074   dmatrices for t
+0000d210: 6869 7320 7472 616e 666f 726d 6174 696f  his tranformatio
+0000d220: 6e20 4953 204e 4f54 2074 6865 2061 6374  n IS NOT the act
+0000d230: 7561 6c20 6166 6669 6e65 206d 6174 7269  ual affine matri
+0000d240: 6365 732c 2062 7574 2049 5320 6120 6469  ces, but IS a di
+0000d250: 6666 6572 656e 7469 6174 696f 6e20 696e  fferentiation in
+0000d260: 7374 6561 642e 0a20 2020 2020 2020 200a  stead..        .
+0000d270: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
+0000d280: 2020 2020 2020 2020 2020 2020 646d 6174              dmat
+0000d290: 7269 6365 7320 5b62 742e 5465 6e73 6f72  rices [bt.Tensor
+0000d2a0: 206f 7220 6e70 2e6e 756d 7079 5d3a 204f   or np.numpy]: O
+0000d2b0: 6e65 2061 6666 696e 6520 6d61 7472 6978  ne affine matrix
+0000d2c0: 2066 6f72 2065 6163 6820 7265 6769 6f6e   for each region
+0000d2d0: 2e20 0a20 2020 2020 2020 2020 2020 2020  . .             
+0000d2e0: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+0000d2f0: 6368 5d2c 207b 6e5f 7265 6769 6f6e 7d2c  ch], {n_region},
+0000d300: 206e 5f64 696d 202b 2031 2c20 6e5f 6469   n_dim + 1, n_di
+0000d310: 6d20 2b20 3129 0a20 2020 2020 2020 2020  m + 1).         
+0000d320: 2020 206d 6173 6b73 205b 6274 2e54 656e     masks [bt.Ten
+0000d330: 736f 7220 6f72 206e 702e 6e75 6d70 795d  sor or np.numpy]
+0000d340: 3a20 4f6e 6520 302d 3120 6d61 736b 2066  : One 0-1 mask f
+0000d350: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
+0000d360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d370: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+0000d380: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000d390: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
+0000d3a0: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
+0000d3b0: 2020 206f 7264 6572 205b 696e 745d 3a20     order [int]: 
+0000d3c0: 7468 6520 6f72 6465 7220 6f66 2069 6e74  the order of int
+0000d3d0: 6572 706f 6c61 7469 6f6e 2063 6f65 6666  erpolation coeff
+0000d3e0: 6963 6965 6e74 2e20 5468 6520 696e 666c  icient. The infl
+0000d3f0: 7565 6e63 6520 6f66 2061 6e20 6166 6669  uence of an affi
+0000d400: 6e65 2064 6563 6179 7320 6174 2061 2072  ne decays at a r
+0000d410: 6174 6520 6f66 2031 202f 2064 6973 7461  ate of 1 / dista
+0000d420: 6e63 655e 6f72 6465 722e 0a20 2020 2020  nce^order..     
+0000d430: 2020 2020 2020 2074 7261 6e73 5f73 7472         trans_str
+0000d440: 6574 6368 205b 696e 745d 3a20 6f6e 6c79  etch [int]: only
+0000d450: 2075 7365 6420 666f 7220 6974 6572 6174   used for iterat
+0000d460: 6976 6520 7061 7261 6d65 7465 7220 7472  ive parameter tr
+0000d470: 6169 6e69 6e67 2c20 3120 6279 2064 6566  aining, 1 by def
+0000d480: 6175 6c74 2e20 3230 2073 6565 6d73 2074  ault. 20 seems t
+0000d490: 6f20 6265 2061 2067 6f6f 6420 6368 6f69  o be a good choi
+0000d4a0: 6365 2e20 200a 2020 2020 2020 2020 2020  ce.  .          
+0000d4b0: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+0000d4c0: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+0000d4d0: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+0000d4e0: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
+0000d4f0: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
+0000d500: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+0000d510: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+0000d520: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
+0000d530: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
+0000d540: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000d550: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0000d560: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
+0000d570: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
+0000d580: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
+0000d590: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d5a0: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+0000d5b0: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
+0000d5c0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000d5d0: 6469 6d29 0a0a 2020 2020 2020 2020 5b31  dim)..        [1
+0000d5e0: 5d20 4172 7369 676e 7920 5620 2c20 436f  ] Arsigny V , Co
+0000d5f0: 6d6d 6f77 6963 6b20 4f20 2c20 4179 6163  mmowick O , Ayac
+0000d600: 6865 204e 202c 2065 7420 616c 2e20 4120  he N , et al. A 
+0000d610: 4661 7374 2061 6e64 204c 6f67 2d45 7563  Fast and Log-Euc
+0000d620: 6c69 6465 616e 2050 6f6c 7961 6666 696e  lidean Polyaffin
+0000d630: 6520 4672 616d 6577 6f72 6b20 666f 7220  e Framework for 
+0000d640: 4c6f 6361 6c6c 7920 0a20 2020 2020 2020  Locally .       
+0000d650: 2020 2020 204c 696e 6561 7220 5265 6769       Linear Regi
+0000d660: 7374 7261 7469 6f6e 5b4a 5d2e 204a 6f75  stration[J]. Jou
+0000d670: 726e 616c 206f 6620 4d61 7468 656d 6174  rnal of Mathemat
+0000d680: 6963 616c 2049 6d61 6769 6e67 2026 2056  ical Imaging & V
+0000d690: 6973 696f 6e2c 2032 3030 392c 2033 3328  ision, 2009, 33(
+0000d6a0: 3229 3a32 3232 2d32 3338 2e0a 2020 2020  2):222-238..    
+0000d6b0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0000d6c0: 696d 706f 7274 2053 696d 706c 6549 544b  import SimpleITK
+0000d6d0: 2061 7320 7369 746b 0a20 2020 2020 2020   as sitk.       
+0000d6e0: 2066 726f 6d20 2e66 756e 6373 2069 6d70   from .funcs imp
+0000d6f0: 6f72 7420 6469 6c61 7465 2c20 6469 7374  ort dilate, dist
+0000d700: 616e 6365 5f6d 6170 0a20 2020 2020 2020  ance_map.       
+0000d710: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000d720: 6365 2864 6d61 7472 6963 6573 2c20 6274  ce(dmatrices, bt
+0000d730: 2e54 656e 736f 7229 3a20 646d 6174 7269  .Tensor): dmatri
+0000d740: 6365 7320 3d20 6274 2e74 656e 736f 7228  ces = bt.tensor(
+0000d750: 646d 6174 7269 6365 7329 0a20 2020 2020  dmatrices).     
+0000d760: 2020 2069 6620 646d 6174 7269 6365 732e     if dmatrices.
+0000d770: 6e5f 6469 6d20 3c3d 2033 2061 6e64 206e  n_dim <= 3 and n
+0000d780: 6f74 2064 6d61 7472 6963 6573 2e68 6173  ot dmatrices.has
+0000d790: 5f62 6174 6368 3a20 646d 6174 7269 6365  _batch: dmatrice
+0000d7a0: 7320 3d20 646d 6174 7269 6365 732e 756e  s = dmatrices.un
+0000d7b0: 7371 7565 657a 6528 5b5d 290a 2020 2020  squeeze([]).    
+0000d7c0: 2020 2020 6966 2064 6d61 7472 6963 6573      if dmatrices
+0000d7d0: 2e6e 5f64 696d 203c 3d20 3320 616e 6420  .n_dim <= 3 and 
+0000d7e0: 6e6f 7420 646d 6174 7269 6365 732e 6861  not dmatrices.ha
+0000d7f0: 735f 6368 616e 6e65 6c3a 2064 6d61 7472  s_channel: dmatr
+0000d800: 6963 6573 203d 2064 6d61 7472 6963 6573  ices = dmatrices
+0000d810: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
+0000d820: 2020 2020 2020 2069 6620 646d 6174 7269         if dmatri
+0000d830: 6365 732e 6e5f 6469 6d20 3d3d 2034 2061  ces.n_dim == 4 a
+0000d840: 6e64 2064 6d61 7472 6963 6573 2e73 6861  nd dmatrices.sha
+0000d850: 7065 5b32 5d20 3d3d 2064 6d61 7472 6963  pe[2] == dmatric
+0000d860: 6573 2e73 6861 7065 5b33 5d3a 0a20 2020  es.shape[3]:.   
+0000d870: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000d880: 646d 6174 7269 6365 732e 6861 735f 6261  dmatrices.has_ba
+0000d890: 7463 683a 2064 6d61 7472 6963 6573 2e62  tch: dmatrices.b
+0000d8a0: 6174 6368 5f64 696d 656e 7369 6f6e 203d  atch_dimension =
+0000d8b0: 2030 0a20 2020 2020 2020 2020 2020 2069   0.            i
+0000d8c0: 6620 6e6f 7420 646d 6174 7269 6365 732e  f not dmatrices.
+0000d8d0: 6861 735f 6368 616e 6e65 6c3a 2064 6d61  has_channel: dma
+0000d8e0: 7472 6963 6573 2e63 6861 6e6e 656c 5f64  trices.channel_d
+0000d8f0: 696d 656e 7369 6f6e 203d 2031 0a20 2020  imension = 1.   
+0000d900: 2020 2020 2061 766f 7563 6828 646d 6174       avouch(dmat
+0000d910: 7269 6365 732e 6861 735f 6261 7463 6820  rices.has_batch 
+0000d920: 616e 6420 646d 6174 7269 6365 732e 6861  and dmatrices.ha
+0000d930: 735f 6368 616e 6e65 6c2c 2022 506c 6561  s_channel, "Plea
+0000d940: 7365 2075 7365 2062 6174 6f72 6368 2074  se use batorch t
+0000d950: 656e 736f 7220 6f66 2073 697a 6520 285b  ensor of size ([
+0000d960: 6e5f 6261 7463 685d 2c20 7b6e 5f72 6567  n_batch], {n_reg
+0000d970: 696f 6e7d 2c22 202b 0a20 2020 2020 2020  ion}," +.       
+0000d980: 2020 2020 2020 2020 6622 6e5f 6469 6d20          f"n_dim 
+0000d990: 2b20 312c 206e 5f64 696d 202b 2031 2920  + 1, n_dim + 1) 
+0000d9a0: 666f 7220 506f 6c79 4166 6669 6e65 2070  for PolyAffine p
+0000d9b0: 6172 616d 6574 6572 732c 2069 6e73 7465  arameters, inste
+0000d9c0: 6164 206f 6620 7b64 6d61 7472 6963 6573  ad of {dmatrices
+0000d9d0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+0000d9e0: 2020 2020 6966 2074 7261 6e73 5f73 7472      if trans_str
+0000d9f0: 6574 6368 2069 7320 6e6f 7420 4e6f 6e65  etch is not None
+0000da00: 3a20 646d 6174 7269 6365 735b 2e2e 2e2c  : dmatrices[...,
+0000da10: 203a 6e5f 6469 6d2c 202d 315d 202a 3d20   :n_dim, -1] *= 
+0000da20: 7472 616e 735f 7374 7265 7463 680a 2020  trans_stretch.  
+0000da30: 2020 2020 2020 6e5f 6469 6d20 3d20 646d        n_dim = dm
+0000da40: 6174 7269 6365 732e 7369 7a65 282d 3129  atrices.size(-1)
+0000da50: 202d 2031 0a20 2020 2020 2020 2069 6620   - 1.        if 
+0000da60: 6e6f 7420 6973 696e 7374 616e 6365 286d  not isinstance(m
+0000da70: 6173 6b73 2c20 6274 2e54 656e 736f 7229  asks, bt.Tensor)
+0000da80: 3a20 6d61 736b 7320 3d20 6274 2e74 656e  : masks = bt.ten
+0000da90: 736f 7228 6d61 736b 7329 0a20 2020 2020  sor(masks).     
+0000daa0: 2020 2069 6620 6d61 736b 732e 6e5f 6469     if masks.n_di
+0000dab0: 6d20 3c3d 206e 5f64 696d 202b 2031 2061  m <= n_dim + 1 a
+0000dac0: 6e64 206e 6f74 206d 6173 6b73 2e68 6173  nd not masks.has
+0000dad0: 5f62 6174 6368 3a20 6d61 736b 7320 3d20  _batch: masks = 
+0000dae0: 6d61 736b 732e 756e 7371 7565 657a 6528  masks.unsqueeze(
+0000daf0: 5b5d 290a 2020 2020 2020 2020 6966 206d  []).        if m
+0000db00: 6173 6b73 2e6e 5f64 696d 203c 3d20 6e5f  asks.n_dim <= n_
+0000db10: 6469 6d20 2b20 3120 616e 6420 6e6f 7420  dim + 1 and not 
+0000db20: 6d61 736b 732e 6861 735f 6368 616e 6e65  masks.has_channe
+0000db30: 6c3a 206d 6173 6b73 203d 206d 6173 6b73  l: masks = masks
+0000db40: 2e75 6e73 7175 6565 7a65 287b 7d29 0a20  .unsqueeze({}). 
+0000db50: 2020 2020 2020 2069 6620 6d61 736b 732e         if masks.
+0000db60: 6e5f 6469 6d20 3d3d 206e 5f64 696d 202b  n_dim == n_dim +
+0000db70: 2032 2061 6e64 206e 6f74 206d 6173 6b73   2 and not masks
+0000db80: 2e68 6173 5f62 6174 6368 3a20 6d61 736b  .has_batch: mask
+0000db90: 732e 6261 7463 685f 6469 6d65 6e73 696f  s.batch_dimensio
+0000dba0: 6e20 3d20 300a 2020 2020 2020 2020 6966  n = 0.        if
+0000dbb0: 206d 6173 6b73 2e6e 5f64 696d 203d 3d20   masks.n_dim == 
+0000dbc0: 6e5f 6469 6d20 2b20 3220 616e 6420 6e6f  n_dim + 2 and no
+0000dbd0: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
+0000dbe0: 6e65 6c3a 206d 6173 6b73 2e63 6861 6e6e  nel: masks.chann
+0000dbf0: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
+0000dc00: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
+0000dc10: 6d61 736b 732e 6861 735f 6261 7463 6820  masks.has_batch 
+0000dc20: 616e 6420 6d61 736b 732e 6861 735f 6368  and masks.has_ch
+0000dc30: 616e 6e65 6c2c 2022 506c 6561 7365 2075  annel, "Please u
+0000dc40: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+0000dc50: 7220 6f66 2073 697a 6520 285b 6e5f 6261  r of size ([n_ba
+0000dc60: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
+0000dc70: 2c22 202b 0a20 2020 2020 2020 2020 2020  ," +.           
+0000dc80: 2020 2020 6622 6e40 312c 206e 4032 2c20      f"n@1, n@2, 
+0000dc90: 2e2e 2e2c 206e 406e 5f64 696d 2920 666f  ..., n@n_dim) fo
+0000dca0: 7220 506f 6c79 4166 6669 6e65 2070 6172  r PolyAffine par
+0000dcb0: 616d 6574 6572 732c 2069 6e73 7465 6164  ameters, instead
+0000dcc0: 206f 6620 7b6d 6173 6b73 2e73 6861 7065   of {masks.shape
+0000dcd0: 7d2e 2022 290a 0a20 2020 2020 2020 2023  }. ")..        #
+0000dce0: 2070 7265 7072 6f63 6573 7320 6d61 736b   preprocess mask
+0000dcf0: 7320 285b 6e5f 6261 7463 685d 2c20 7b6e  s ([n_batch], {n
+0000dd00: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
+0000dd10: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
+0000dd20: 290a 2020 2020 2020 2020 6e5f 6261 7463  ).        n_batc
+0000dd30: 6820 3d20 6d61 736b 732e 6e5f 6261 7463  h = masks.n_batc
+0000dd40: 680a 2020 2020 2020 2020 6e5f 7265 6769  h.        n_regi
+0000dd50: 6f6e 203d 206d 6173 6b73 2e6e 5f63 6861  on = masks.n_cha
+0000dd60: 6e6e 656c 0a20 2020 2020 2020 2064 6973  nnel.        dis
+0000dd70: 203d 2064 6973 7461 6e63 655f 6d61 7028   = distance_map(
+0000dd80: 6d61 736b 7329 0a20 2020 2020 2020 2064  masks).        d
+0000dd90: 6973 203d 2028 6469 7320 2b20 3129 2e63  is = (dis + 1).c
+0000dda0: 6c61 6d70 2830 290a 2020 2020 2020 2020  lamp(0).        
+0000ddb0: 2320 696d 706f 7274 206d 6963 6f6d 7075  # import micompu
+0000ddc0: 7469 6e67 2e70 6c6f 7420 6173 2070 6c74  ting.plot as plt
+0000ddd0: 0a20 2020 2020 2020 2023 2070 6c74 2e73  .        # plt.s
+0000dde0: 7562 706c 6f74 7328 3229 0a20 2020 2020  ubplots(2).     
+0000ddf0: 2020 2023 2070 6c74 2e69 6d73 7368 6f77     # plt.imsshow
+0000de00: 2864 6973 5b30 2c20 305d 2c20 6469 735b  (dis[0, 0], dis[
+0000de10: 302c 2031 5d29 0a20 2020 2020 2020 2023  0, 1]).        #
+0000de20: 2070 6c74 2e73 686f 7728 290a 2020 2020   plt.show().    
+0000de30: 2020 2020 7765 6967 6874 7320 3d20 3120      weights = 1 
+0000de40: 2f20 2864 6973 202a 2a20 6f72 6465 7220  / (dis ** order 
+0000de50: 2b20 3165 2d35 290a 2020 2020 2020 2020  + 1e-5).        
+0000de60: 7765 6967 6874 7320 3d20 7765 6967 6874  weights = weight
+0000de70: 7320 2f20 7765 6967 6874 732e 7375 6d28  s / weights.sum(
+0000de80: 7b7d 2920 2320 285b 6e5f 6261 7463 685d  {}) # ([n_batch]
+0000de90: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
+0000dea0: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+0000deb0: 5f64 696d 290a 2020 2020 2020 2020 0a20  _dim).        . 
+0000dec0: 2020 2020 2020 2023 2023 2064 6570 7265         # # depre
+0000ded0: 6361 7465 6420 7072 6570 726f 6365 7373  cated preprocess
+0000dee0: 206f 6620 6d61 736b 730a 2020 2020 2020   of masks.      
+0000def0: 2020 2320 6d61 736b 7320 3d20 6d61 736b    # masks = mask
+0000df00: 732e 6e75 6d70 7928 292e 6173 7479 7065  s.numpy().astype
+0000df10: 286e 702e 696e 7429 0a20 2020 2020 2020  (np.int).       
+0000df20: 2023 206e 5f62 6174 6368 2c20 6e5f 7265   # n_batch, n_re
+0000df30: 6769 6f6e 2c20 2a5f 203d 206d 6173 6b73  gion, *_ = masks
+0000df40: 2e73 6861 7065 0a20 2020 2020 2020 2023  .shape.        #
+0000df50: 205f 6469 735f 6d61 7020 3d20 6274 2e7a   _dis_map = bt.z
+0000df60: 6572 6f73 282a 6d61 736b 732e 7368 6170  eros(*masks.shap
+0000df70: 6529 0a20 2020 2020 2020 2023 2066 6f72  e).        # for
+0000df80: 2069 2069 6e20 7261 6e67 6528 6e5f 6261   i in range(n_ba
+0000df90: 7463 6829 3a0a 2020 2020 2020 2020 2320  tch):.        # 
+0000dfa0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0000dfb0: 6765 286e 5f72 6567 696f 6e29 3a0a 2020  ge(n_region):.  
+0000dfc0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0000dfd0: 6d61 736b 5f69 6d61 6765 203d 2073 6974  mask_image = sit
+0000dfe0: 6b2e 4765 7449 6d61 6765 4672 6f6d 4172  k.GetImageFromAr
+0000dff0: 7261 7928 6d61 736b 735b 692c 206a 5d2c  ray(masks[i, j],
+0000e000: 2069 7356 6563 746f 7220 3d20 4661 6c73   isVector = Fals
+0000e010: 6529 0a20 2020 2020 2020 2023 2020 2020  e).        #    
+0000e020: 2020 2020 2064 6973 5f6d 6170 203d 2073       dis_map = s
+0000e030: 6974 6b2e 4765 7441 7272 6179 5669 6577  itk.GetArrayView
+0000e040: 4672 6f6d 496d 6167 6528 7369 746b 2e53  FromImage(sitk.S
+0000e050: 6967 6e65 644d 6175 7265 7244 6973 7461  ignedMaurerDista
+0000e060: 6e63 654d 6170 286d 6173 6b5f 696d 6167  nceMap(mask_imag
+0000e070: 652c 2073 7175 6172 6564 4469 7374 616e  e, squaredDistan
+0000e080: 6365 203d 2046 616c 7365 2c20 7573 6549  ce = False, useI
+0000e090: 6d61 6765 5370 6163 696e 6720 3d20 4661  mageSpacing = Fa
+0000e0a0: 6c73 6529 290a 2020 2020 2020 2020 2320  lse)).        # 
+0000e0b0: 2020 2020 2020 2020 6469 735f 6d61 7020          dis_map 
+0000e0c0: 3d20 6e70 2e61 7272 6179 2864 6973 5f6d  = np.array(dis_m
+0000e0d0: 6170 292e 6173 7479 7065 286e 702e 666c  ap).astype(np.fl
+0000e0e0: 6f61 7429 0a20 2020 2020 2020 2023 2020  oat).        #  
+0000e0f0: 2020 2020 2020 205f 6469 735f 6d61 705b         _dis_map[
+0000e100: 692c 206a 5d20 3d20 6274 2e74 656e 736f  i, j] = bt.tenso
+0000e110: 7228 6469 735f 6d61 7020 2a20 2864 6973  r(dis_map * (dis
+0000e120: 5f6d 6170 203e 2030 292e 6173 7479 7065  _map > 0).astype
+0000e130: 286e 702e 666c 6f61 7429 290a 2020 2020  (np.float)).    
+0000e140: 2020 2020 2320 6b20 3d20 320a 2020 2020      # k = 2.    
+0000e150: 2020 2020 2320 696e 7670 6f77 6b5f 6469      # invpowk_di
+0000e160: 735f 6d61 7020 3d20 3120 2f20 285f 6469  s_map = 1 / (_di
+0000e170: 735f 6d61 7020 2a2a 206b 202b 2031 652d  s_map ** k + 1e-
+0000e180: 3529 0a20 2020 2020 2020 2023 2073 756d  5).        # sum
+0000e190: 5f64 6973 5f6d 6170 203d 2069 6e76 706f  _dis_map = invpo
+0000e1a0: 776b 5f64 6973 5f6d 6170 2e73 756d 2831  wk_dis_map.sum(1
+0000e1b0: 2c20 6b65 6570 6469 6d20 3d20 5472 7565  , keepdim = True
+0000e1c0: 290a 2020 2020 2020 2020 2320 7765 6967  ).        # weig
+0000e1d0: 6874 7320 3d20 696e 7670 6f77 6b5f 6469  hts = invpowk_di
+0000e1e0: 735f 6d61 7020 2f20 7375 6d5f 6469 735f  s_map / sum_dis_
+0000e1f0: 6d61 700a 2020 2020 2020 2020 2320 6672  map.        # fr
+0000e200: 6f6d 206d 6174 706c 6f74 6c69 6220 696d  om matplotlib im
+0000e210: 706f 7274 2070 7970 6c6f 7420 6173 2070  port pyplot as p
+0000e220: 6c74 0a20 2020 2020 2020 2023 2070 6c74  lt.        # plt
+0000e230: 2e73 7562 706c 6f74 2831 3231 293b 2070  .subplot(121); p
+0000e240: 6c74 2e69 6d73 686f 7728 7765 6967 6874  lt.imshow(weight
+0000e250: 735b 302c 2030 5d29 0a20 2020 2020 2020  s[0, 0]).       
+0000e260: 2023 2070 6c74 2e73 7562 706c 6f74 2831   # plt.subplot(1
+0000e270: 3232 293b 2070 6c74 2e69 6d73 686f 7728  22); plt.imshow(
+0000e280: 7765 6967 6874 735b 302c 2031 5d29 0a20  weights[0, 1]). 
+0000e290: 2020 2020 2020 2023 2070 6c74 2e73 686f         # plt.sho
+0000e2a0: 7728 290a 2020 2020 2020 2020 2320 6966  w().        # if
+0000e2b0: 2074 7261 6e73 5f73 7472 6574 6368 2069   trans_stretch i
+0000e2c0: 7320 6e6f 7420 4e6f 6e65 3a20 646d 6174  s not None: dmat
+0000e2d0: 7269 6365 7320 3d20 646d 6174 7269 6365  rices = dmatrice
+0000e2e0: 7320 2a20 6274 2e74 656e 736f 7228 5b31  s * bt.tensor([1
+0000e2f0: 2e5d 202a 206e 5f64 696d 202b 205b 7472  .] * n_dim + [tr
+0000e300: 616e 735f 7374 7265 7463 685d 292e 756e  ans_stretch]).un
+0000e310: 7371 7565 657a 6528 302c 2030 2c20 3029  squeeze(0, 0, 0)
+0000e320: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+0000e330: 292e 5f5f 696e 6974 5f5f 2864 6d61 7472  ).__init__(dmatr
+0000e340: 6963 6573 2c20 6d61 736b 733d 6d61 736b  ices, masks=mask
+0000e350: 732c 206f 7264 6572 3d6f 7264 6572 2c20  s, order=order, 
+0000e360: 6973 5f69 6e76 3d69 735f 696e 762c 2074  is_inv=is_inv, t
+0000e370: 7261 6e73 5f73 7472 6574 6368 3d74 7261  rans_stretch=tra
+0000e380: 6e73 5f73 7472 6574 6368 290a 2020 2020  ns_stretch).    
+0000e390: 2020 2020 7365 6c66 2e6e 5f62 6174 6368      self.n_batch
+0000e3a0: 203d 206e 5f62 6174 6368 0a20 2020 2020   = n_batch.     
+0000e3b0: 2020 2073 656c 662e 6e5f 6469 6d20 3d20     self.n_dim = 
+0000e3c0: 6e5f 6469 6d0a 2020 2020 2020 2020 7365  n_dim.        se
+0000e3d0: 6c66 2e6d 6173 6b73 203d 206d 6173 6b73  lf.masks = masks
+0000e3e0: 0a20 2020 2020 2020 2073 656c 662e 7765  .        self.we
+0000e3f0: 6967 6874 7320 3d20 7765 6967 6874 730a  ights = weights.
+0000e400: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000e410: 6e73 5f73 7472 6574 6368 203d 2074 7261  ns_stretch = tra
+0000e420: 6e73 5f73 7472 6574 6368 0a20 2020 2020  ns_stretch.     
+0000e430: 2020 2073 656c 662e 646d 6174 7269 6365     self.dmatrice
+0000e440: 7320 3d20 646d 6174 7269 6365 730a 2020  s = dmatrices.  
+0000e450: 2020 2020 2020 7365 6c66 2e69 735f 696e        self.is_in
+0000e460: 7620 3d20 6973 5f69 6e76 0a20 2020 2020  v = is_inv.     
+0000e470: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0000e480: 6f72 6465 720a 0a20 2020 2064 6566 205f  order..    def _
+0000e490: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+0000e4a0: 3a0a 2020 2020 2020 2020 5820 3d20 7375  :.        X = su
+0000e4b0: 7065 7228 292e 5f5f 6361 6c6c 5f5f 2858  per().__call__(X
+0000e4c0: 290a 2020 2020 2020 2020 646d 6174 7269  ).        dmatri
+0000e4d0: 6365 7320 3d20 7365 6c66 2e64 6d61 7472  ces = self.dmatr
+0000e4e0: 6963 6573 2023 2028 5b6e 5f62 6174 6368  ices # ([n_batch
+0000e4f0: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000e500: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
+0000e510: 2b20 3129 0a20 2020 2020 2020 2077 6569  + 1).        wei
+0000e520: 6768 7473 203d 2073 656c 662e 7765 6967  ghts = self.weig
+0000e530: 6874 7320 2320 285b 6e5f 6261 7463 685d  hts # ([n_batch]
+0000e540: 2c20 7b6e 5f72 6567 696f 6e7d 2c20 6e40  , {n_region}, n@
+0000e550: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+0000e560: 5f64 696d 290a 2020 2020 2020 2020 6e5f  _dim).        n_
+0000e570: 6469 6d20 3d20 7365 6c66 2e6e 5f64 696d  dim = self.n_dim
+0000e580: 0a20 2020 2020 2020 206e 5f72 6567 696f  .        n_regio
+0000e590: 6e20 3d20 646d 6174 7269 6365 732e 6e5f  n = dmatrices.n_
+0000e5a0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
+0000e5b0: 5873 203d 2058 2e6d 756c 7469 706c 7928  Xs = X.multiply(
+0000e5c0: 6e5f 7265 6769 6f6e 2c20 7b7d 2920 2320  n_region, {}) # 
+0000e5d0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000e5e0: 6567 696f 6e7d 2c20 6e5f 6469 6d2c 206e  egion}, n_dim, n
+0000e5f0: 4031 2c20 6e40 322c 202e 2e2e 2c20 6e40  @1, n@2, ..., n@
+0000e600: 6e5f 6469 6d29 0a20 2020 2020 2020 2041  n_dim).        A
+0000e610: 203d 2064 6d61 7472 6963 6573 5b2e 2e2e   = dmatrices[...
+0000e620: 2c20 3a6e 5f64 696d 2c20 3a6e 5f64 696d  , :n_dim, :n_dim
+0000e630: 5d0a 2020 2020 2020 2020 6220 3d20 646d  ].        b = dm
+0000e640: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
+0000e650: 6469 6d2c 206e 5f64 696d 3a5d 0a20 2020  dim, n_dim:].   
+0000e660: 2020 2020 2059 203d 2028 4120 4020 5873       Y = (A @ Xs
+0000e670: 2e66 6c61 7474 656e 2833 2920 2b20 6229  .flatten(3) + b)
+0000e680: 2e76 6965 775f 6173 2858 7329 0a20 2020  .view_as(Xs).   
+0000e690: 2020 2020 2044 203d 2028 5920 2a20 7765       D = (Y * we
+0000e6a0: 6967 6874 732e 756e 7371 7565 657a 6528  ights.unsqueeze(
+0000e6b0: 2929 2e73 756d 287b 7d29 2e77 6974 685f  )).sum({}).with_
+0000e6c0: 6368 616e 6e65 6c64 696d 2831 2920 2d20  channeldim(1) - 
+0000e6d0: 580a 2020 2020 2020 2020 6966 2073 656c  X.        if sel
+0000e6e0: 662e 6973 5f69 6e76 3a20 4420 3d20 2d44  f.is_inv: D = -D
+0000e6f0: 0a20 2020 2020 2020 2074 7261 6e73 203d  .        trans =
+0000e700: 2044 656e 7365 4469 7370 6c61 6365 6d65   DenseDisplaceme
+0000e710: 6e74 4669 656c 6428 4429 0a20 2020 2020  ntField(D).     
+0000e720: 2020 2074 7261 6e73 3220 3d20 4465 6e73     trans2 = Dens
+0000e730: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
+0000e740: 6c64 2874 7261 6e73 2874 7261 6e73 2858  ld(trans(trans(X
+0000e750: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
+0000e760: 7472 616e 7334 203d 2044 656e 7365 4469  trans4 = DenseDi
+0000e770: 7370 6c61 6365 6d65 6e74 4669 656c 6428  splacementField(
+0000e780: 7472 616e 7332 2874 7261 6e73 3228 5829  trans2(trans2(X)
+0000e790: 2920 2d20 5829 0a20 2020 2020 2020 2074  ) - X).        t
+0000e7a0: 7261 6e73 3820 3d20 4465 6e73 6544 6973  rans8 = DenseDis
+0000e7b0: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e7c0: 7261 6e73 3428 7472 616e 7334 2858 2929  rans4(trans4(X))
+0000e7d0: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
+0000e7e0: 616e 7331 3620 3d20 4465 6e73 6544 6973  ans16 = DenseDis
+0000e7f0: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e800: 7261 6e73 3828 7472 616e 7338 2858 2929  rans8(trans8(X))
+0000e810: 202d 2058 290a 2020 2020 2020 2020 7472   - X).        tr
+0000e820: 616e 7333 3220 3d20 4465 6e73 6544 6973  ans32 = DenseDis
+0000e830: 706c 6163 656d 656e 7446 6965 6c64 2874  placementField(t
+0000e840: 7261 6e73 3136 2874 7261 6e73 3136 2858  rans16(trans16(X
+0000e850: 2929 202d 2058 290a 2020 2020 2020 2020  )) - X).        
+0000e860: 7472 616e 7336 3420 3d20 4465 6e73 6544  trans64 = DenseD
+0000e870: 6973 706c 6163 656d 656e 7446 6965 6c64  isplacementField
+0000e880: 2874 7261 6e73 3332 2874 7261 6e73 3332  (trans32(trans32
+0000e890: 2858 2929 202d 2058 290a 2020 2020 2020  (X)) - X).      
+0000e8a0: 2020 7265 7475 726e 2074 7261 6e73 3634    return trans64
+0000e8b0: 2858 290a 0a20 2020 2064 6566 2069 6e76  (X)..    def inv
+0000e8c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e8d0: 7265 7475 726e 2050 6f6c 7941 6666 696e  return PolyAffin
+0000e8e0: 6528 7365 6c66 2e64 6d61 7472 6963 6573  e(self.dmatrices
+0000e8f0: 2c20 7365 6c66 2e6d 6173 6b73 2c20 6f72  , self.masks, or
+0000e900: 6465 723d 7365 6c66 2e6f 7264 6572 2c20  der=self.order, 
+0000e910: 6973 5f69 6e76 3d6e 6f74 2073 656c 662e  is_inv=not self.
+0000e920: 6973 5f69 6e76 2c20 7472 616e 735f 7374  is_inv, trans_st
+0000e930: 7265 7463 6820 3d20 3129 2e62 6163 6b77  retch = 1).backw
+0000e940: 6172 645f 2873 656c 662e 6261 636b 7761  ard_(self.backwa
+0000e950: 7264 290a 2020 2020 2020 2020 2320 6e5f  rd).        # n_
+0000e960: 6261 7463 6820 3d20 7365 6c66 2e64 6d61  batch = self.dma
+0000e970: 7472 6963 6573 2e6e 5f62 6174 6368 0a20  trices.n_batch. 
+0000e980: 2020 2020 2020 2023 2061 6666 7320 3d20         # affs = 
+0000e990: 6274 2e69 6e76 2873 656c 662e 646d 6174  bt.inv(self.dmat
+0000e9a0: 7269 6365 7329 0a20 2020 2020 2020 2023  rices).        #
+0000e9b0: 206d 6173 6b73 203d 2069 6e74 6572 706f   masks = interpo
+0000e9c0: 6c61 7469 6f6e 2873 656c 662e 6d61 736b  lation(self.mask
+0000e9d0: 732e 6d65 7267 6564 696d 7328 5b5d 2c20  s.mergedims([], 
+0000e9e0: 7b7d 292c 2041 6666 696e 6528 6274 2e6d  {}), Affine(bt.m
+0000e9f0: 6174 706f 7728 6166 6673 2e6d 6572 6765  atpow(affs.merge
+0000ea00: 6469 6d73 285b 5d2c 207b 7d29 2c20 3634  dims([], {}), 64
+0000ea10: 2929 292e 7370 6c69 7464 696d 285b 5d2c  ))).splitdim([],
+0000ea20: 205b 6e5f 6261 7463 685d 2c20 7b2d 317d   [n_batch], {-1}
+0000ea30: 290a 2020 2020 2020 2020 2320 7265 7475  ).        # retu
+0000ea40: 726e 2050 6f6c 7941 6666 696e 6528 6166  rn PolyAffine(af
+0000ea50: 6673 2c20 6d61 736b 7320 3d20 6d61 736b  fs, masks = mask
+0000ea60: 732c 2074 7261 6e73 5f73 7472 6574 6368  s, trans_stretch
+0000ea70: 203d 2073 656c 662e 7472 616e 735f 7374   = self.trans_st
+0000ea80: 7265 7463 6829 2e62 6163 6b77 6172 645f  retch).backward_
+0000ea90: 2873 656c 662e 6261 636b 7761 7264 290a  (self.backward).
+0000eaa0: 0a40 616c 6961 7328 224c 4152 4d22 290a  .@alias("LARM").
+0000eab0: 636c 6173 7320 4c6f 6361 6c6c 7941 6666  class LocallyAff
+0000eac0: 696e 6528 5370 6174 6961 6c54 7261 6e73  ine(SpatialTrans
+0000ead0: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+0000eae0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000eaf0: 662c 206d 6174 7269 6365 732c 206d 6173  f, matrices, mas
+0000eb00: 6b73 2c20 6f72 6465 723d 322c 2074 7261  ks, order=2, tra
+0000eb10: 6e73 5f73 7472 6574 6368 3d4e 6f6e 652c  ns_stretch=None,
+0000eb20: 2061 766f 6964 5f63 6f6e 666c 6963 743d   avoid_conflict=
+0000eb30: 5472 7565 293a 0a20 2020 2020 2020 2027  True):.        '
+0000eb40: 2727 0a20 2020 2020 2020 204c 6f63 616c  ''.        Local
+0000eb50: 6c79 2061 6666 696e 6520 7472 616e 7366  ly affine transf
+0000eb60: 6f72 6d61 7469 6f6e 2077 6974 6820 7265  ormation with re
+0000eb70: 7370 6563 7420 746f 2074 7261 6e73 666f  spect to transfo
+0000eb80: 726d 6174 696f 6e20 6d61 7472 6963 6573  rmation matrices
+0000eb90: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
+0000eba0: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+0000ebb0: 2020 2020 2020 2020 2020 206d 6174 7269             matri
+0000ebc0: 6365 7320 5b62 742e 5465 6e73 6f72 206f  ces [bt.Tensor o
+0000ebd0: 7220 6e70 2e6e 756d 7079 5d3a 204f 6e65  r np.numpy]: One
+0000ebe0: 2061 6666 696e 6520 6d61 7472 6978 2066   affine matrix f
+0000ebf0: 6f72 2065 6163 6820 7265 6769 6f6e 2e20  or each region. 
+0000ec00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec10: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+0000ec20: 5d2c 207b 6e5f 7265 6769 6f6e 7d2c 206e  ], {n_region}, n
+0000ec30: 5f64 696d 202b 2031 2c20 6e5f 6469 6d20  _dim + 1, n_dim 
+0000ec40: 2b20 3129 0a20 2020 2020 2020 2020 2020  + 1).           
+0000ec50: 206d 6173 6b73 205b 6274 2e54 656e 736f   masks [bt.Tenso
+0000ec60: 7220 6f72 206e 702e 6e75 6d70 795d 3a20  r or np.numpy]: 
+0000ec70: 4f6e 6520 302d 3120 6d61 736b 2066 6f72  One 0-1 mask for
+0000ec80: 2065 6163 6820 7265 6769 6f6e 2e20 0a20   each region. . 
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eca0: 697a 653a 2028 5b6e 5f62 6174 6368 5d2c  ize: ([n_batch],
+0000ecb0: 207b 6e5f 7265 6769 6f6e 7d2c 206e 4031   {n_region}, n@1
+0000ecc0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+0000ecd0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+0000ece0: 206f 7264 6572 205b 696e 745d 3a20 7468   order [int]: th
+0000ecf0: 6520 6f72 6465 7220 6f66 2069 6e74 6572  e order of inter
+0000ed00: 706f 6c61 7469 6f6e 2063 6f65 6666 6963  polation coeffic
+0000ed10: 6965 6e74 2e20 5468 6520 696e 666c 7565  ient. The influe
+0000ed20: 6e63 6520 6f66 2061 6e20 6166 6669 6e65  nce of an affine
+0000ed30: 2064 6563 6179 7320 6174 2061 2072 6174   decays at a rat
+0000ed40: 6520 6f66 2031 202f 2064 6973 7461 6e63  e of 1 / distanc
+0000ed50: 655e 6f72 6465 722e 0a20 2020 2020 2020  e^order..       
+0000ed60: 2020 2020 2074 7261 6e73 5f73 7472 6574       trans_stret
+0000ed70: 6368 205b 696e 745d 3a20 6f6e 6c79 2075  ch [int]: only u
+0000ed80: 7365 6420 666f 7220 6974 6572 6174 6976  sed for iterativ
+0000ed90: 6520 7061 7261 6d65 7465 7220 7472 6169  e parameter trai
+0000eda0: 6e69 6e67 2c20 3120 6279 2064 6566 6175  ning, 1 by defau
+0000edb0: 6c74 2e20 3230 2073 6565 6d73 2074 6f20  lt. 20 seems to 
+0000edc0: 6265 2061 2067 6f6f 6420 6368 6f69 6365  be a good choice
+0000edd0: 2e20 200a 2020 2020 2020 2020 2020 2020  .  .            
+0000ede0: 0a20 2020 2020 2020 2057 6865 6e20 6974  .        When it
+0000edf0: 2069 7320 6361 6c6c 6564 3a0a 2020 2020   is called:.    
+0000ee00: 2020 2020 2020 2020 5820 5b62 742e 5465          X [bt.Te
+0000ee10: 6e73 6f72 5d3a 2043 6f6f 7264 696e 6174  nsor]: Coordinat
+0000ee20: 6573 2074 6f20 6265 2074 7261 6e73 666f  es to be transfo
+0000ee30: 726d 6564 2e0a 2020 2020 2020 2020 2020  rmed..          
+0000ee40: 2020 2020 2020 7369 7a65 3a20 285b 6e5f        size: ([n_
+0000ee50: 6261 7463 683a 206f 7074 696f 6e61 6c5d  batch: optional]
+0000ee60: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+0000ee70: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000ee80: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
+0000ee90: 7574 7075 7420 5b62 742e 5465 6e73 6f72  utput [bt.Tensor
+0000eea0: 5d3a 2054 6865 2074 7261 6e73 666f 726d  ]: The transform
+0000eeb0: 6564 2063 6f6f 7264 696e 6174 6573 2e0a  ed coordinates..
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eed0: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+0000eee0: 2c20 7b6e 5f64 696d 7d2c 206e 4031 2c20  , {n_dim}, n@1, 
+0000eef0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000ef00: 6d29 0a0a 2020 2020 2020 2020 5b31 5d20  m)..        [1] 
+0000ef10: 5a68 7561 6e67 2058 202c 2052 686f 6465  Zhuang X , Rhode
+0000ef20: 204b 202c 2041 7272 6964 6765 2053 202c   K , Arridge S ,
+0000ef30: 2065 7420 616c 2e20 416e 2041 746c 6173   et al. An Atlas
+0000ef40: 2d42 6173 6564 2053 6567 6d65 6e74 6174  -Based Segmentat
+0000ef50: 696f 6e20 5072 6f70 6167 6174 696f 6e20  ion Propagation 
+0000ef60: 4672 616d 6577 6f72 6b20 5573 696e 6720  Framework Using 
+0000ef70: 4c6f 6361 6c6c 7920 4166 6669 6e65 200a  Locally Affine .
+0000ef80: 2020 2020 2020 2020 2020 2020 5265 6769              Regi
+0000ef90: 7374 7261 7469 6f6e 202d 2041 7070 6c69  stration - Appli
+0000efa0: 6361 7469 6f6e 2074 6f20 4175 746f 6d61  cation to Automa
+0000efb0: 7469 6320 5768 6f6c 6520 4865 6172 7420  tic Whole Heart 
+0000efc0: 5365 676d 656e 7461 7469 6f6e 5b4a 5d2e  Segmentation[J].
+0000efd0: 2053 7072 696e 6765 722c 2042 6572 6c69   Springer, Berli
+0000efe0: 6e2c 2048 6569 6465 6c62 6572 672c 2032  n, Heidelberg, 2
+0000eff0: 3030 382e 0a20 2020 2020 2020 2027 2727  008..        '''
+0000f000: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+0000f010: 5369 6d70 6c65 4954 4b20 6173 2073 6974  SimpleITK as sit
+0000f020: 6b0a 2020 2020 2020 2020 6672 6f6d 202e  k.        from .
+0000f030: 6675 6e63 7320 696d 706f 7274 2064 696c  funcs import dil
+0000f040: 6174 652c 2064 6973 7461 6e63 655f 6d61  ate, distance_ma
+0000f050: 700a 2020 2020 2020 2020 6d61 7472 6963  p.        matric
+0000f060: 6573 203d 2062 6174 6f72 6368 5f74 656e  es = batorch_ten
+0000f070: 736f 7228 6d61 7472 6963 6573 290a 2020  sor(matrices).  
+0000f080: 2020 2020 2020 6966 206d 6174 7269 6365        if matrice
+0000f090: 732e 6e5f 6469 6d20 3c3d 2033 2061 6e64  s.n_dim <= 3 and
+0000f0a0: 206e 6f74 206d 6174 7269 6365 732e 6861   not matrices.ha
+0000f0b0: 735f 6261 7463 683a 206d 6174 7269 6365  s_batch: matrice
+0000f0c0: 7320 3d20 6d61 7472 6963 6573 2e75 6e73  s = matrices.uns
+0000f0d0: 7175 6565 7a65 285b 5d29 0a20 2020 2020  queeze([]).     
+0000f0e0: 2020 2069 6620 6d61 7472 6963 6573 2e6e     if matrices.n
+0000f0f0: 5f64 696d 203c 3d20 3320 616e 6420 6e6f  _dim <= 3 and no
+0000f100: 7420 6d61 7472 6963 6573 2e68 6173 5f63  t matrices.has_c
+0000f110: 6861 6e6e 656c 3a20 6d61 7472 6963 6573  hannel: matrices
+0000f120: 203d 206d 6174 7269 6365 732e 756e 7371   = matrices.unsq
+0000f130: 7565 657a 6528 7b7d 290a 2020 2020 2020  ueeze({}).      
+0000f140: 2020 6966 206d 6174 7269 6365 732e 6e5f    if matrices.n_
+0000f150: 6469 6d20 3d3d 2034 2061 6e64 206d 6174  dim == 4 and mat
+0000f160: 7269 6365 732e 7368 6170 655b 325d 203d  rices.shape[2] =
+0000f170: 3d20 6d61 7472 6963 6573 2e73 6861 7065  = matrices.shape
+0000f180: 5b33 5d3a 0a20 2020 2020 2020 2020 2020  [3]:.           
+0000f190: 2069 6620 6e6f 7420 6d61 7472 6963 6573   if not matrices
+0000f1a0: 2e68 6173 5f62 6174 6368 3a20 6d61 7472  .has_batch: matr
+0000f1b0: 6963 6573 2e62 6174 6368 5f64 696d 656e  ices.batch_dimen
+0000f1c0: 7369 6f6e 203d 2030 0a20 2020 2020 2020  sion = 0.       
+0000f1d0: 2020 2020 2069 6620 6e6f 7420 6d61 7472       if not matr
+0000f1e0: 6963 6573 2e68 6173 5f63 6861 6e6e 656c  ices.has_channel
+0000f1f0: 3a20 6d61 7472 6963 6573 2e63 6861 6e6e  : matrices.chann
+0000f200: 656c 5f64 696d 656e 7369 6f6e 203d 2031  el_dimension = 1
+0000f210: 0a20 2020 2020 2020 2061 766f 7563 6828  .        avouch(
+0000f220: 6d61 7472 6963 6573 2e68 6173 5f62 6174  matrices.has_bat
+0000f230: 6368 2061 6e64 206d 6174 7269 6365 732e  ch and matrices.
+0000f240: 6861 735f 6368 616e 6e65 6c2c 2022 506c  has_channel, "Pl
+0000f250: 6561 7365 2075 7365 2062 6174 6f72 6368  ease use batorch
+0000f260: 2074 656e 736f 7220 6f66 2073 697a 6520   tensor of size 
+0000f270: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000f280: 6567 696f 6e7d 2c22 202b 0a20 2020 2020  egion}," +.     
+0000f290: 2020 2020 2020 2020 2020 6622 6e5f 6469            f"n_di
+0000f2a0: 6d20 2b20 312c 206e 5f64 696d 202b 2031  m + 1, n_dim + 1
+0000f2b0: 2920 666f 7220 4c6f 6361 6c6c 7941 6666  ) for LocallyAff
+0000f2c0: 696e 6520 7061 7261 6d65 7465 7273 2c20  ine parameters, 
+0000f2d0: 696e 7374 6561 6420 6f66 207b 6d61 7472  instead of {matr
+0000f2e0: 6963 6573 2e73 6861 7065 7d2e 2022 290a  ices.shape}. ").
+0000f2f0: 2020 2020 2020 2020 6966 2074 7261 6e73          if trans
+0000f300: 5f73 7472 6574 6368 2069 7320 6e6f 7420  _stretch is not 
+0000f310: 4e6f 6e65 3a20 6d61 7472 6963 6573 5b2e  None: matrices[.
+0000f320: 2e2e 2c20 3a6e 5f64 696d 2c20 2d31 5d20  .., :n_dim, -1] 
+0000f330: 2a3d 2074 7261 6e73 5f73 7472 6574 6368  *= trans_stretch
+0000f340: 0a20 2020 2020 2020 206e 5f64 696d 203d  .        n_dim =
+0000f350: 206d 6174 7269 6365 732e 7369 7a65 282d   matrices.size(-
+0000f360: 3129 202d 2031 0a20 2020 2020 2020 206d  1) - 1.        m
+0000f370: 6173 6b73 203d 2062 6174 6f72 6368 5f74  asks = batorch_t
+0000f380: 656e 736f 7228 6d61 736b 7329 0a20 2020  ensor(masks).   
+0000f390: 2020 2020 2069 6620 6d61 736b 732e 6e5f       if masks.n_
+0000f3a0: 6469 6d20 3c3d 206e 5f64 696d 202b 2031  dim <= n_dim + 1
+0000f3b0: 2061 6e64 206e 6f74 206d 6173 6b73 2e68   and not masks.h
+0000f3c0: 6173 5f62 6174 6368 3a20 6d61 736b 7320  as_batch: masks 
+0000f3d0: 3d20 6d61 736b 732e 756e 7371 7565 657a  = masks.unsqueez
+0000f3e0: 6528 5b5d 290a 2020 2020 2020 2020 6966  e([]).        if
+0000f3f0: 206d 6173 6b73 2e6e 5f64 696d 203c 3d20   masks.n_dim <= 
+0000f400: 6e5f 6469 6d20 2b20 3120 616e 6420 6e6f  n_dim + 1 and no
+0000f410: 7420 6d61 736b 732e 6861 735f 6368 616e  t masks.has_chan
+0000f420: 6e65 6c3a 206d 6173 6b73 203d 206d 6173  nel: masks = mas
+0000f430: 6b73 2e75 6e73 7175 6565 7a65 287b 7d29  ks.unsqueeze({})
+0000f440: 0a20 2020 2020 2020 2069 6620 6d61 736b  .        if mask
+0000f450: 732e 6e5f 6469 6d20 3d3d 206e 5f64 696d  s.n_dim == n_dim
+0000f460: 202b 2032 2061 6e64 206e 6f74 206d 6173   + 2 and not mas
+0000f470: 6b73 2e68 6173 5f62 6174 6368 3a20 6d61  ks.has_batch: ma
+0000f480: 736b 732e 6261 7463 685f 6469 6d65 6e73  sks.batch_dimens
+0000f490: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
+0000f4a0: 6966 206d 6173 6b73 2e6e 5f64 696d 203d  if masks.n_dim =
+0000f4b0: 3d20 6e5f 6469 6d20 2b20 3220 616e 6420  = n_dim + 2 and 
+0000f4c0: 6e6f 7420 6d61 736b 732e 6861 735f 6368  not masks.has_ch
+0000f4d0: 616e 6e65 6c3a 206d 6173 6b73 2e63 6861  annel: masks.cha
+0000f4e0: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
+0000f4f0: 2031 0a20 2020 2020 2020 2061 766f 7563   1.        avouc
+0000f500: 6828 6d61 736b 732e 6861 735f 6261 7463  h(masks.has_batc
+0000f510: 6820 616e 6420 6d61 736b 732e 6861 735f  h and masks.has_
+0000f520: 6368 616e 6e65 6c2c 2022 506c 6561 7365  channel, "Please
+0000f530: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+0000f540: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
+0000f550: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
+0000f560: 6e7d 2c22 202b 200a 2020 2020 2020 2020  n}," + .        
+0000f570: 2020 2020 2020 2066 226e 4031 2c20 6e40         f"n@1, n@
+0000f580: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+0000f590: 2066 6f72 204c 6f63 616c 6c79 4166 6669   for LocallyAffi
+0000f5a0: 6e65 2070 6172 616d 6574 6572 732c 2069  ne parameters, i
+0000f5b0: 6e73 7465 6164 206f 6620 7b6d 6173 6b73  nstead of {masks
+0000f5c0: 2e73 6861 7065 7d2e 2022 290a 0a20 2020  .shape}. ")..   
+0000f5d0: 2020 2020 2023 2070 7265 7072 6f63 6573       # preproces
+0000f5e0: 7320 6d61 736b 730a 2020 2020 2020 2020  s masks.        
+0000f5f0: 6e5f 6261 7463 6820 3d20 6d61 7472 6963  n_batch = matric
+0000f600: 6573 2e6e 5f62 6174 6368 0a20 2020 2020  es.n_batch.     
+0000f610: 2020 206e 5f72 6567 696f 6e20 3d20 6d61     n_region = ma
+0000f620: 7472 6963 6573 2e6e 5f63 6861 6e6e 656c  trices.n_channel
+0000f630: 0a20 2020 2020 2020 2069 6620 6176 6f69  .        if avoi
+0000f640: 645f 636f 6e66 6c69 6374 3a0a 2020 2020  d_conflict:.    
+0000f650: 2020 2020 2020 2020 4769 203d 2041 6666          Gi = Aff
+0000f660: 696e 6528 6d61 7472 6963 6573 2e6d 6572  ine(matrices.mer
+0000f670: 6765 6469 6d73 287b 7d2c 205b 5d29 290a  gedims({}, [])).
+0000f680: 2020 2020 2020 2020 2020 2020 4769 5669              GiVi
+0000f690: 203d 2069 6e74 6572 706f 6c61 7469 6f6e   = interpolation
+0000f6a0: 286d 6173 6b73 2e6d 6572 6765 6469 6d73  (masks.mergedims
+0000f6b0: 287b 7d2c 205b 5d29 2c20 4769 2e69 6e76  ({}, []), Gi.inv
+0000f6c0: 2829 2c20 6d65 7468 6f64 3d27 4e65 6172  (), method='Near
+0000f6d0: 6573 7427 292e 7370 6c69 7464 696d 285b  est').splitdim([
+0000f6e0: 5d2c 205b 6e5f 6261 7463 685d 2c20 6e5f  ], [n_batch], n_
+0000f6f0: 7265 6769 6f6e 2920 2320 285b 6e5f 6261  region) # ([n_ba
+0000f700: 7463 685d 2c20 6e5f 7265 6769 6f6e 2c20  tch], n_region, 
+0000f710: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+0000f720: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+0000f730: 2020 2020 4769 5669 6a6f 696e 476b 566b      GiVijoinGkVk
+0000f740: 203d 2028 4769 5669 2e75 6e73 7175 6565   = (GiVi.unsquee
+0000f750: 7a65 2831 2920 2a20 4769 5669 2e75 6e73  ze(1) * GiVi.uns
+0000f760: 7175 6565 7a65 2832 2929 2e6d 6572 6765  queeze(2)).merge
+0000f770: 6469 6d73 2831 2c20 5b5d 292e 7769 7468  dims(1, []).with
+0000f780: 5f63 6861 6e6e 656c 6469 6d28 3129 2023  _channeldim(1) #
+0000f790: 2028 5b6e 5f62 6174 6368 2078 206e 5f72   ([n_batch x n_r
+0000f7a0: 6567 696f 6e5d 2c20 7b6e 5f72 6567 696f  egion], {n_regio
+0000f7b0: 6e7d 2c20 6e40 312c 206e 4032 2c20 2e2e  n}, n@1, n@2, ..
+0000f7c0: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
+0000f7d0: 2020 2020 2020 2020 5269 6b20 3d20 696e          Rik = in
+0000f7e0: 7465 7270 6f6c 6174 696f 6e28 4769 5669  terpolation(GiVi
+0000f7f0: 6a6f 696e 476b 566b 2c20 4769 2c20 6d65  joinGkVk, Gi, me
+0000f800: 7468 6f64 3d27 4e65 6172 6573 7427 292e  thod='Nearest').
+0000f810: 7370 6c69 7464 696d 285b 5d2c 205b 6e5f  splitdim([], [n_
+0000f820: 6261 7463 685d 2c20 6e5f 7265 6769 6f6e  batch], n_region
+0000f830: 2920 2320 285b 6e5f 6261 7463 685d 2c20  ) # ([n_batch], 
+0000f840: 6e5f 7265 6769 6f6e 2c20 7b6e 5f72 6567  n_region, {n_reg
+0000f850: 696f 6e7d 2c20 6e40 312c 206e 4032 2c20  ion}, n@1, n@2, 
+0000f860: 2e2e 2e2c 206e 406e 5f64 696d 290a 2020  ..., n@n_dim).  
+0000f870: 2020 2020 2020 2020 2020 5552 696b 203d            URik =
+0000f880: 2028 5269 6b2e 7375 6d28 7b7d 292e 7769   (Rik.sum({}).wi
+0000f890: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
+0000f8a0: 202d 206d 6173 6b73 203e 2030 2e31 292e   - masks > 0.1).
+0000f8b0: 666c 6f61 7428 2920 2320 285b 6e5f 6261  float() # ([n_ba
+0000f8c0: 7463 685d 2c20 7b6e 5f72 6567 696f 6e7d  tch], {n_region}
+0000f8d0: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
+0000f8e0: 206e 406e 5f64 696d 290a 2020 2020 2020   n@n_dim).      
+0000f8f0: 2020 2020 2020 5552 696b 5f70 6c75 7320        URik_plus 
+0000f900: 3d20 6469 6c61 7465 2855 5269 6b2e 6d65  = dilate(URik.me
+0000f910: 7267 6564 696d 7328 7b7d 2c20 5b5d 292c  rgedims({}, []),
+0000f920: 2031 292e 7370 6c69 7464 696d 285b 5d2c   1).splitdim([],
+0000f930: 205b 6e5f 6261 7463 685d 2c20 6e5f 7265   [n_batch], n_re
+0000f940: 6769 6f6e 2920 2320 285b 6e5f 6261 7463  gion) # ([n_batc
+0000f950: 685d 2c20 7b6e 5f72 6567 696f 6e7d 2c20  h], {n_region}, 
+0000f960: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+0000f970: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+0000f980: 2020 2020 6d61 736b 7320 3d20 286d 6173      masks = (mas
+0000f990: 6b73 202d 2055 5269 6b5f 706c 7573 203e  ks - URik_plus >
+0000f9a0: 2030 2e31 292e 666c 6f61 7428 2920 2320   0.1).float() # 
+0000f9b0: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f72  ([n_batch], {n_r
+0000f9c0: 6567 696f 6e7d 2c20 6e40 312c 206e 4032  egion}, n@1, n@2
+0000f9d0: 2c20 2e2e 2e2c 206e 406e 5f64 696d 290a  , ..., n@n_dim).
+0000f9e0: 0a20 2020 2020 2020 2077 6569 6768 7473  .        weights
+0000f9f0: 203d 2031 202f 2028 6469 7374 616e 6365   = 1 / (distance
+0000fa00: 5f6d 6170 286d 6173 6b73 2920 2a2a 206f  _map(masks) ** o
+0000fa10: 7264 6572 202b 2031 652d 3529 0a20 2020  rder + 1e-5).   
+0000fa20: 2020 2020 2077 6569 6768 7473 203d 2077       weights = w
+0000fa30: 6569 6768 7473 202f 2077 6569 6768 7473  eights / weights
+0000fa40: 2e73 756d 287b 7d29 2023 2028 5b6e 5f62  .sum({}) # ([n_b
+0000fa50: 6174 6368 5d2c 207b 6e5f 7265 6769 6f6e  atch], {n_region
+0000fa60: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+0000fa70: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+0000fa80: 2020 2023 2069 6620 7472 616e 735f 7374     # if trans_st
+0000fa90: 7265 7463 6820 6973 206e 6f74 204e 6f6e  retch is not Non
+0000faa0: 653a 206d 6174 7269 6365 7320 3d20 6d61  e: matrices = ma
+0000fab0: 7472 6963 6573 202a 2062 6174 6f72 6368  trices * batorch
+0000fac0: 5f74 656e 736f 7228 5b31 2e5d 202a 206e  _tensor([1.] * n
+0000fad0: 5f64 696d 202b 205b 7472 616e 735f 7374  _dim + [trans_st
+0000fae0: 7265 7463 685d 292e 756e 7371 7565 657a  retch]).unsqueez
+0000faf0: 6528 302c 2030 2c20 3029 0a0a 2020 2020  e(0, 0, 0)..    
+0000fb00: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0000fb10: 6974 5f5f 286d 6174 7269 6365 732c 206d  it__(matrices, m
+0000fb20: 6173 6b73 3d6d 6173 6b73 2c20 6f72 6465  asks=masks, orde
+0000fb30: 723d 6f72 6465 722c 2074 7261 6e73 5f73  r=order, trans_s
+0000fb40: 7472 6574 6368 3d74 7261 6e73 5f73 7472  tretch=trans_str
+0000fb50: 6574 6368 290a 2020 2020 2020 2020 7365  etch).        se
+0000fb60: 6c66 2e6e 5f62 6174 6368 203d 206e 5f62  lf.n_batch = n_b
+0000fb70: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
+0000fb80: 662e 6e5f 6469 6d20 3d20 6e5f 6469 6d0a  f.n_dim = n_dim.
+0000fb90: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000fba0: 6b73 203d 206d 6173 6b73 0a20 2020 2020  ks = masks.     
+0000fbb0: 2020 2073 656c 662e 7765 6967 6874 7320     self.weights 
+0000fbc0: 3d20 7765 6967 6874 730a 2020 2020 2020  = weights.      
+0000fbd0: 2020 7365 6c66 2e74 7261 6e73 5f73 7472    self.trans_str
+0000fbe0: 6574 6368 203d 2074 7261 6e73 5f73 7472  etch = trans_str
+0000fbf0: 6574 6368 0a20 2020 2020 2020 2073 656c  etch.        sel
+0000fc00: 662e 6d61 7472 6963 6573 203d 206d 6174  f.matrices = mat
+0000fc10: 7269 6365 730a 2020 2020 2020 2020 7365  rices.        se
+0000fc20: 6c66 2e62 6174 6368 5f70 6172 616d 2e65  lf.batch_param.e
+0000fc30: 7874 656e 6428 5b27 6d61 7472 6963 6573  xtend(['matrices
+0000fc40: 272c 2027 7765 6967 6874 7327 2c20 276d  ', 'weights', 'm
+0000fc50: 6173 6b73 275d 290a 0a20 2020 2064 6566  asks'])..    def
+0000fc60: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
+0000fc70: 5829 3a0a 2020 2020 2020 2020 5820 3d20  X):.        X = 
+0000fc80: 7375 7065 7228 292e 5f5f 6361 6c6c 5f5f  super().__call__
+0000fc90: 2858 290a 2020 2020 2020 2020 6d61 7472  (X).        matr
+0000fca0: 6963 6573 203d 2073 656c 662e 6d61 7472  ices = self.matr
+0000fcb0: 6963 6573 0a20 2020 2020 2020 206d 6173  ices.        mas
+0000fcc0: 6b73 203d 2073 656c 662e 6d61 736b 7320  ks = self.masks 
+0000fcd0: 2320 285b 6e5f 6261 7463 685d 2c20 7b6e  # ([n_batch], {n
+0000fce0: 5f72 6567 696f 6e7d 2c20 6e40 312c 206e  _region}, n@1, n
+0000fcf0: 4032 2c20 2e2e 2e2c 206e 406e 5f64 696d  @2, ..., n@n_dim
+0000fd00: 290a 2020 2020 2020 2020 7765 6967 6874  ).        weight
+0000fd10: 7320 3d20 7365 6c66 2e77 6569 6768 7473  s = self.weights
+0000fd20: 2023 2028 5b6e 5f62 6174 6368 5d2c 207b   # ([n_batch], {
+0000fd30: 6e5f 7265 6769 6f6e 7d2c 206e 4031 2c20  n_region}, n@1, 
+0000fd40: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000fd50: 6d29 0a20 2020 2020 2020 206e 5f64 696d  m).        n_dim
+0000fd60: 203d 2073 656c 662e 6e5f 6469 6d0a 2020   = self.n_dim.  
+0000fd70: 2020 2020 2020 6e5f 7265 6769 6f6e 203d        n_region =
+0000fd80: 206d 6174 7269 6365 732e 6e5f 6368 616e   matrices.n_chan
+0000fd90: 6e65 6c0a 2020 2020 2020 2020 5873 203d  nel.        Xs =
+0000fda0: 2058 2e6d 756c 7469 706c 7928 6e5f 7265   X.multiply(n_re
+0000fdb0: 6769 6f6e 2c20 7b7d 2920 2320 285b 6e5f  gion, {}) # ([n_
+0000fdc0: 6261 7463 685d 2c20 7b6e 5f72 6567 696f  batch], {n_regio
+0000fdd0: 6e7d 2c20 6e5f 6469 6d2c 206e 4031 2c20  n}, n_dim, n@1, 
+0000fde0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+0000fdf0: 6d29 0a20 2020 2020 2020 2041 203d 206d  m).        A = m
+0000fe00: 6174 7269 6365 735b 2e2e 2e2c 203a 6e5f  atrices[..., :n_
+0000fe10: 6469 6d2c 203a 6e5f 6469 6d5d 0a20 2020  dim, :n_dim].   
+0000fe20: 2020 2020 2062 203d 206d 6174 7269 6365       b = matrice
+0000fe30: 735b 2e2e 2e2c 203a 6e5f 6469 6d2c 206e  s[..., :n_dim, n
+0000fe40: 5f64 696d 3a5d 0a20 2020 2020 2020 2059  _dim:].        Y
+0000fe50: 203d 2028 4120 4020 5873 2e66 6c61 7474   = (A @ Xs.flatt
+0000fe60: 656e 2833 2920 2b20 6229 2e76 6965 775f  en(3) + b).view_
+0000fe70: 6173 2858 7329 0a20 2020 2020 2020 2072  as(Xs).        r
+0000fe80: 6574 7572 6e20 2877 6569 6768 7473 2e75  eturn (weights.u
+0000fe90: 6e73 7175 6565 7a65 2829 202a 2059 292e  nsqueeze() * Y).
+0000fea0: 7375 6d28 7b7d 292e 7769 7468 5f63 6861  sum({}).with_cha
+0000feb0: 6e6e 656c 6469 6d28 3129 202a 2028 3120  nneldim(1) * (1 
+0000fec0: 2d20 6d61 736b 732e 7375 6d28 7b7d 292e  - masks.sum({}).
+0000fed0: 756e 7371 7565 657a 6528 7b7d 2929 202b  unsqueeze({})) +
+0000fee0: 2028 5920 2a20 6d61 736b 732e 756e 7371   (Y * masks.unsq
+0000fef0: 7565 657a 6528 2929 2e73 756d 287b 7d29  ueeze()).sum({})
+0000ff00: 2e77 6974 685f 6368 616e 6e65 6c64 696d  .with_channeldim
+0000ff10: 2831 290a 0a20 2020 2064 6566 2069 6e76  (1)..    def inv
+0000ff20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ff30: 6e5f 6261 7463 6820 3d20 7365 6c66 2e6d  n_batch = self.m
+0000ff40: 6174 7269 6365 732e 6e5f 6261 7463 680a  atrices.n_batch.
+0000ff50: 2020 2020 2020 2020 6166 6673 203d 2062          affs = b
+0000ff60: 742e 696e 7628 7365 6c66 2e6d 6174 7269  t.inv(self.matri
+0000ff70: 6365 7329 0a20 2020 2020 2020 206d 6173  ces).        mas
+0000ff80: 6b73 203d 2069 6e74 6572 706f 6c61 7469  ks = interpolati
+0000ff90: 6f6e 2873 656c 662e 6d61 736b 732e 6d65  on(self.masks.me
+0000ffa0: 7267 6564 696d 7328 5b5d 2c20 7b7d 292c  rgedims([], {}),
+0000ffb0: 2041 6666 696e 6528 6166 6673 2e6d 6572   Affine(affs.mer
+0000ffc0: 6765 6469 6d73 285b 5d2c 207b 7d29 2929  gedims([], {})))
+0000ffd0: 2e73 706c 6974 6469 6d28 5b5d 2c20 5b6e  .splitdim([], [n
+0000ffe0: 5f62 6174 6368 5d2c 207b 2d31 7d29 0a20  _batch], {-1}). 
+0000fff0: 2020 2020 2020 2072 6574 7572 6e20 506f         return Po
+00010000: 6c79 4166 6669 6e65 2861 6666 732c 206d  lyAffine(affs, m
+00010010: 6173 6b73 203d 206d 6173 6b73 2c20 7472  asks = masks, tr
+00010020: 616e 735f 7374 7265 7463 6820 3d20 3129  ans_stretch = 1)
+00010030: 2e62 6163 6b77 6172 645f 2873 656c 662e  .backward_(self.
+00010040: 6261 636b 7761 7264 290a 0a40 616c 6961  backward)..@alia
+00010050: 7328 2246 4644 2229 0a63 6c61 7373 2046  s("FFD").class F
+00010060: 7265 6546 6f72 6d44 6566 6f72 6d61 7469  reeFormDeformati
+00010070: 6f6e 2853 7061 7469 616c 5472 616e 7366  on(SpatialTransf
+00010080: 6f72 6d61 7469 6f6e 293a 0a0a 2020 2020  ormation):..    
+00010090: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000100a0: 662c 206f 6666 7365 7473 2c20 7370 6163  f, offsets, spac
+000100b0: 696e 673d 312c 206f 7269 6769 6e3d 3029  ing=1, origin=0)
+000100c0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+000100d0: 2020 2020 2020 4672 6565 2046 6f72 6d20        Free Form 
+000100e0: 4465 666f 726d 6174 696f 6e20 2846 4644  Deformation (FFD
+000100f0: 2920 7472 616e 7366 6f72 6d61 7469 6f6e  ) transformation
+00010100: 205b 315d 2e0a 2020 2020 2020 2020 0a20   [1]..        . 
+00010110: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+00010120: 2020 2020 2020 2020 2020 206f 6666 7365             offse
+00010130: 7473 205b 6274 2e54 656e 736f 725d 3a20  ts [bt.Tensor]: 
+00010140: 7468 6520 4646 4420 6f66 6673 6574 732e  the FFD offsets.
+00010150: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00010160: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00010170: 685d 2c20 7b6e 5f64 696d 7d2c 206d 4031  h], {n_dim}, m@1
+00010180: 2c20 6d40 322c 202e 2e2e 2c20 6d40 6e5f  , m@2, ..., m@n_
+00010190: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+000101a0: 2020 2020 2066 6f72 206d 4031 2078 206d       for m@1 x m
+000101b0: 4032 2078 202e 2e2e 2078 206d 406e 5f64  @2 x ... x m@n_d
+000101c0: 696d 2067 7269 6420 6f66 20ce 9463 6f6e  im grid of ..con
+000101d0: 7472 6f6c 2070 6f69 6e74 730a 2020 2020  trol points.    
+000101e0: 2020 2020 2020 2020 7370 6163 696e 6720          spacing 
+000101f0: 5b69 6e74 206f 7220 7475 706c 655d 3a20  [int or tuple]: 
+00010200: 4646 4420 7370 6163 696e 673b 2073 7061  FFD spacing; spa
+00010210: 6369 6e67 2062 6574 7765 656e 2046 4644  cing between FFD
+00010220: 2063 6f6e 7472 6f6c 2070 6f69 6e74 732e   control points.
+00010230: 200a 2020 2020 2020 2020 2020 2020 6f72   .            or
+00010240: 6967 696e 205b 696e 7420 6f72 2074 7570  igin [int or tup
+00010250: 6c65 5d3a 2046 4644 206f 7269 6769 6e3b  le]: FFD origin;
+00010260: 2063 6f6f 7264 696e 6174 6520 666f 7220   coordinate for 
+00010270: 7468 6520 2830 2c20 302c 2030 2920 636f  the (0, 0, 0) co
+00010280: 6e74 726f 6c20 706f 696e 742e 200a 2020  ntrol point. .  
+00010290: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+000102a0: 2020 2057 6865 6e20 6974 2069 7320 6361     When it is ca
+000102b0: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+000102c0: 2020 5820 5b62 742e 5465 6e73 6f72 5d3a    X [bt.Tensor]:
+000102d0: 2043 6f6f 7264 696e 6174 6573 2074 6f20   Coordinates to 
+000102e0: 6265 2074 7261 6e73 666f 726d 6564 2e0a  be transformed..
+000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010300: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00010310: 206f 7074 696f 6e61 6c5d 2c20 7b6e 5f64   optional], {n_d
+00010320: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
+00010330: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
+00010340: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00010350: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
+00010360: 2074 7261 6e73 666f 726d 6564 2063 6f6f   transformed coo
+00010370: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00010380: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00010390: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f64  ([n_batch], {n_d
+000103a0: 696d 7d2c 206e 4031 2c20 6e40 322c 202e  im}, n@1, n@2, .
+000103b0: 2e2e 2c20 6e40 6e5f 6469 6d29 0a20 2020  .., n@n_dim).   
+000103c0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000103d0: 2020 2020 2020 5b31 5d20 5275 6563 6b65        [1] Ruecke
+000103e0: 7274 2044 202c 2053 6f6e 6f64 6120 4c20  rt D , Sonoda L 
+000103f0: 4920 2c20 4861 7965 7320 4320 2c20 6574  I , Hayes C , et
+00010400: 2061 6c2e 204e 6f6e 7269 6769 6420 7265   al. Nonrigid re
+00010410: 6769 7374 7261 7469 6f6e 2075 7369 6e67  gistration using
+00010420: 2066 7265 652d 666f 726d 2064 6566 6f72   free-form defor
+00010430: 6d61 7469 6f6e 733a 200a 2020 2020 2020  mations: .      
+00010440: 2020 2020 2020 6170 706c 6963 6174 696f        applicatio
+00010450: 6e20 746f 2062 7265 6173 7420 4d52 2069  n to breast MR i
+00010460: 6d61 6765 735b 4a5d 2e20 4945 4545 2054  mages[J]. IEEE T
+00010470: 7261 6e73 6163 7469 6f6e 7320 6f6e 204d  ransactions on M
+00010480: 6564 6963 616c 2049 6d61 6769 6e67 2c20  edical Imaging, 
+00010490: 3139 3939 2838 292e 0a20 2020 2020 2020  1999(8)..       
+000104a0: 2027 2727 0a20 2020 2020 2020 206f 6666   '''.        off
+000104b0: 7365 7473 203d 2062 6174 6f72 6368 5f74  sets = batorch_t
+000104c0: 656e 736f 7228 6f66 6673 6574 7329 0a20  ensor(offsets). 
+000104d0: 2020 2020 2020 2069 6620 6e6f 7420 6f66         if not of
+000104e0: 6673 6574 732e 6861 735f 6368 616e 6e65  fsets.has_channe
+000104f0: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
+00010500: 6620 6f66 6673 6574 732e 7369 7a65 2830  f offsets.size(0
+00010510: 2920 3d3d 206f 6666 7365 7473 2e6e 5f64  ) == offsets.n_d
+00010520: 696d 202d 2031 3a0a 2020 2020 2020 2020  im - 1:.        
+00010530: 2020 2020 2020 2020 6e5f 6469 6d20 3d20          n_dim = 
+00010540: 6f66 6673 6574 732e 7369 7a65 2830 290a  offsets.size(0).
+00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010560: 6f66 6673 6574 732e 6368 616e 6e65 6c5f  offsets.channel_
+00010570: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+00010580: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00010590: 6673 6574 7320 3d20 6f66 6673 6574 732e  fsets = offsets.
+000105a0: 756e 7371 7565 657a 6528 5b5d 290a 2020  unsqueeze([]).  
+000105b0: 2020 2020 2020 2020 2020 656c 6966 206f            elif o
+000105c0: 6666 7365 7473 2e73 697a 6528 3129 203d  ffsets.size(1) =
+000105d0: 3d20 6f66 6673 6574 732e 6e5f 6469 6d20  = offsets.n_dim 
+000105e0: 2d20 323a 0a20 2020 2020 2020 2020 2020  - 2:.           
+000105f0: 2020 2020 206e 5f64 696d 203d 206f 6666       n_dim = off
+00010600: 7365 7473 2e73 697a 6528 3129 0a20 2020  sets.size(1).   
+00010610: 2020 2020 2020 2020 2020 2020 206f 6666               off
+00010620: 7365 7473 2e63 6861 6e6e 656c 5f64 696d  sets.channel_dim
+00010630: 656e 7369 6f6e 203d 2031 0a20 2020 2020  ension = 1.     
+00010640: 2020 2020 2020 2065 6c73 653a 2072 6169         else: rai
+00010650: 7365 2054 7970 6545 7272 6f72 2866 2246  se TypeError(f"F
+00010660: 4644 2070 6172 616d 6574 6572 7320 7769  FD parameters wi
+00010670: 7468 2073 697a 6520 7b6f 6666 7365 7473  th size {offsets
+00010680: 2e73 6861 7065 7d20 646f 6e6f 7420 6d61  .shape} donot ma
+00010690: 7463 6820 285b 6e5f 6261 7463 685d 2c20  tch ([n_batch], 
+000106a0: 7b7b 6e5f 6469 6d7d 7d2c 206d 5f31 2c20  {{n_dim}}, m_1, 
+000106b0: 6d5f 322c 202e 2e2e 2c20 6d5f 7229 205b  m_2, ..., m_r) [
+000106c0: 723d 6e5f 6469 6d5d 2e20 2229 0a20 2020  r=n_dim]. ").   
+000106d0: 2020 2020 2069 6620 6e6f 7420 6f66 6673       if not offs
+000106e0: 6574 732e 6861 735f 6261 7463 683a 0a20  ets.has_batch:. 
+000106f0: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
+00010700: 203d 206f 6666 7365 7473 2e6e 5f63 6861   = offsets.n_cha
+00010710: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
+00010720: 2069 6620 6f66 6673 6574 732e 6e5f 6469   if offsets.n_di
+00010730: 6d20 3c3d 206e 5f64 696d 202b 2031 3a20  m <= n_dim + 1: 
+00010740: 6f66 6673 6574 7320 3d20 6f66 6673 6574  offsets = offset
+00010750: 732e 756e 7371 7565 657a 6528 5b5d 290a  s.unsqueeze([]).
+00010760: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00010770: 3a20 6f66 6673 6574 732e 6261 7463 685f  : offsets.batch_
+00010780: 6469 6d65 6e73 696f 6e20 3d20 300a 2020  dimension = 0.  
+00010790: 2020 2020 2020 6176 6f75 6368 286f 6666        avouch(off
+000107a0: 7365 7473 2e68 6173 5f62 6174 6368 2061  sets.has_batch a
+000107b0: 6e64 206f 6666 7365 7473 2e68 6173 5f63  nd offsets.has_c
+000107c0: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
+000107d0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+000107e0: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
+000107f0: 2020 2020 2020 2020 2020 285b 6e5f 6261            ([n_ba
+00010800: 7463 685d 2c20 7b7b 6e5f 6469 6d7d 7d2c  tch], {{n_dim}},
+00010810: 206d 5f31 2c20 6d5f 322c 202e 2e2e 2c20   m_1, m_2, ..., 
+00010820: 6d5f 7229 205b 723d 6e5f 6469 6d5d 2066  m_r) [r=n_dim] f
+00010830: 6f72 2046 4644 2070 6172 616d 6574 6572  or FFD parameter
+00010840: 732c 2069 6e73 7465 6164 206f 6620 7b6f  s, instead of {o
+00010850: 6666 7365 7473 2e73 6861 7065 7d2e 2022  ffsets.shape}. "
+00010860: 290a 2020 2020 2020 2020 6e5f 6469 6d20  ).        n_dim 
+00010870: 3d20 6f66 6673 6574 732e 6e5f 6368 616e  = offsets.n_chan
+00010880: 6e65 6c0a 2020 2020 2020 2020 7370 6163  nel.        spac
+00010890: 696e 6720 3d20 746f 5f74 7570 6c65 2873  ing = to_tuple(s
+000108a0: 7061 6369 6e67 290a 2020 2020 2020 2020  pacing).        
+000108b0: 6f72 6967 696e 203d 2074 6f5f 7475 706c  origin = to_tupl
+000108c0: 6528 6f72 6967 696e 290a 2020 2020 2020  e(origin).      
+000108d0: 2020 6966 206c 656e 2873 7061 6369 6e67    if len(spacing
+000108e0: 2920 3d3d 2031 3a20 7370 6163 696e 6720  ) == 1: spacing 
+000108f0: 2a3d 206e 5f64 696d 0a20 2020 2020 2020  *= n_dim.       
+00010900: 2069 6620 6c65 6e28 6f72 6967 696e 2920   if len(origin) 
+00010910: 3d3d 2031 3a20 6f72 6967 696e 202a 3d20  == 1: origin *= 
+00010920: 6e5f 6469 6d0a 2020 2020 2020 2020 7375  n_dim.        su
+00010930: 7065 7228 292e 5f5f 696e 6974 5f5f 286f  per().__init__(o
+00010940: 6666 7365 7473 2c20 7370 6163 696e 673d  ffsets, spacing=
+00010950: 7370 6163 696e 672c 206f 7269 6769 6e3d  spacing, origin=
+00010960: 6f72 6967 696e 290a 0a20 2020 2020 2020  origin)..       
+00010970: 2073 656c 662e 6e5f 6469 6d20 3d20 6e5f   self.n_dim = n_
+00010980: 6469 6d0a 2020 2020 2020 2020 7365 6c66  dim.        self
+00010990: 2e6f 6666 7365 7473 203d 206f 6666 7365  .offsets = offse
+000109a0: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
+000109b0: 7370 6163 696e 6720 3d20 7370 6163 696e  spacing = spacin
+000109c0: 670a 2020 2020 2020 2020 7365 6c66 2e6f  g.        self.o
+000109d0: 7269 6769 6e20 3d20 6f72 6967 696e 0a20  rigin = origin. 
+000109e0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+000109f0: 685f 7061 7261 6d2e 6170 7065 6e64 2827  h_param.append('
+00010a00: 6f66 6673 6574 7327 290a 2020 2020 0a20  offsets').    . 
+00010a10: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+00010a20: 7365 6c66 2c20 5829 3a0a 2020 2020 2020  self, X):.      
+00010a30: 2020 5820 3d20 7375 7065 7228 292e 5f5f    X = super().__
+00010a40: 6361 6c6c 5f5f 2858 290a 2020 2020 2020  call__(X).      
+00010a50: 2020 7368 6170 6520 3d20 582e 7368 6170    shape = X.shap
+00010a60: 650a 2020 2020 2020 2020 6e5f 6469 6d20  e.        n_dim 
+00010a70: 3d20 7365 6c66 2e6e 5f64 696d 0a20 2020  = self.n_dim.   
+00010a80: 2020 2020 206f 6666 7365 7473 203d 2073       offsets = s
+00010a90: 656c 662e 6f66 6673 6574 732e 666c 6f61  elf.offsets.floa
+00010aa0: 7428 290a 2020 2020 2020 2020 7370 6163  t().        spac
+00010ab0: 696e 6720 3d20 7365 6c66 2e73 7061 6369  ing = self.spaci
+00010ac0: 6e67 0a20 2020 2020 2020 206e 5f62 6174  ng.        n_bat
+00010ad0: 6368 203d 206f 6666 7365 7473 2e6e 5f62  ch = offsets.n_b
+00010ae0: 6174 6368 0a20 2020 2020 2020 2023 2058  atch.        # X
+00010af0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+00010b00: 5f64 696d 7d2c 206e 5f64 6174 6120 3d20  _dim}, n_data = 
+00010b10: 6e5f 3120 7820 6e5f 3220 7820 2e2e 2e20  n_1 x n_2 x ... 
+00010b20: 7820 6e5f 7229 0a20 2020 2020 2020 2058  x n_r).        X
+00010b30: 203d 2058 2e66 6c61 7474 656e 2829 0a20   = X.flatten(). 
+00010b40: 2020 2020 2020 2058 202d 3d20 6274 2e63         X -= bt.c
+00010b50: 6861 6e6e 656c 5f74 656e 736f 7228 7365  hannel_tensor(se
+00010b60: 6c66 2e6f 7269 6769 6e29 0a20 2020 2020  lf.origin).     
+00010b70: 2020 206e 5f64 6174 6120 3d20 582e 7369     n_data = X.si
+00010b80: 7a65 282d 3129 0a20 2020 2020 2020 2073  ze(-1).        s
+00010b90: 697a 6520 3d20 6274 2e63 6861 6e6e 656c  ize = bt.channel
+00010ba0: 5f74 656e 736f 7228 6f66 6673 6574 732e  _tensor(offsets.
+00010bb0: 7370 6163 6529 0a20 2020 2020 2020 2023  space).        #
+00010bc0: 204e 6f72 6d61 6c69 7a65 2058 2069 6e20   Normalize X in 
+00010bd0: 7468 6520 646f 6d61 696e 2028 6d5f 312c  the domain (m_1,
+00010be0: 206d 5f32 2c20 2e2e 2e2c 206d 5f7b 6e5f   m_2, ..., m_{n_
+00010bf0: 6469 6d7d 292e 0a20 2020 2020 2020 2046  dim})..        F
+00010c00: 4644 5820 3d20 5820 2f20 6274 2e63 6861  FDX = X / bt.cha
+00010c10: 6e6e 656c 5f74 656e 736f 7228 7370 6163  nnel_tensor(spac
+00010c20: 696e 6729 2e66 6c6f 6174 2829 0a20 2020  ing).float().   
+00010c30: 2020 2020 2069 5820 3d20 6274 2e66 6c6f       iX = bt.flo
+00010c40: 6f72 2846 4644 5829 2e66 6c6f 6174 2829  or(FFDX).float()
+00010c50: 3b20 7558 203d 2046 4644 5820 2d20 6958  ; uX = FFDX - iX
+00010c60: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
+00010c70: 7465 2074 6865 2077 6569 6768 7473 2e20  te the weights. 
+00010c80: 573a 2028 342c 205b 6e5f 6261 7463 685d  W: (4, [n_batch]
+00010c90: 2c20 7b6e 5f64 696d 7d2c 206e 5f64 6174  , {n_dim}, n_dat
+00010ca0: 6120 3d20 6e5f 3120 7820 6e5f 3220 7820  a = n_1 x n_2 x 
+00010cb0: 2e2e 2e20 7820 6e5f 7229 0a20 2020 2020  ... x n_r).     
+00010cc0: 2020 2069 203d 2062 742e 6172 616e 6765     i = bt.arange
+00010cd0: 282d 312c 2033 292e 6578 7061 6e64 5f74  (-1, 3).expand_t
+00010ce0: 6f28 342c 205b 6e5f 6261 7463 685d 2c20  o(4, [n_batch], 
+00010cf0: 7b6e 5f64 696d 7d2c 206e 5f64 6174 612c  {n_dim}, n_data,
+00010d00: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+00010d10: 2057 203d 2042 7370 6c69 6e65 2869 2c20   W = Bspline(i, 
+00010d20: 7558 2e6d 756c 7469 706c 7928 342c 2030  uX.multiply(4, 0
+00010d30: 2929 0a20 2020 2020 2020 2022 436f 6d70  )).        "Comp
+00010d40: 7574 6520 4646 4420 5472 616e 7366 6f72  ute FFD Transfor
+00010d50: 6d61 7469 6f6e 220a 2020 2020 2020 2020  mation".        
+00010d60: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
+00010d70: 735f 6c69 6b65 2858 290a 2020 2020 2020  s_like(X).      
+00010d80: 2020 2320 4c6f 6f70 2069 6e20 7468 6520    # Loop in the 
+00010d90: 7370 6163 6520 7b2d 312c 2030 2c20 312c  space {-1, 0, 1,
+00010da0: 2032 7d20 5e20 6e5f 6469 6d3b 2047 2069   2} ^ n_dim; G i
+00010db0: 7320 696e 2028 302c 2031 2c20 322c 2033  s in (0, 1, 2, 3
+00010dc0: 290a 2020 2020 2020 2020 666f 7220 4720  ).        for G 
+00010dd0: 696e 2062 742e 696d 6167 655f 6772 6964  in bt.image_grid
+00010de0: 285b 345d 2a6e 5f64 696d 292e 666c 6174  ([4]*n_dim).flat
+00010df0: 7465 6e28 292e 7472 616e 7370 6f73 6528  ten().transpose(
+00010e00: 302c 2031 293a 0a20 2020 2020 2020 2020  0, 1):.         
+00010e10: 2020 2047 203d 2062 742e 6368 616e 6e65     G = bt.channe
+00010e20: 6c5f 7465 6e73 6f72 2847 290a 2020 2020  l_tensor(G).    
+00010e30: 2020 2020 2020 2020 2320 5765 6967 6874          # Weight
+00010e40: 7320 666f 7220 6561 6368 2070 6f69 6e74  s for each point
+00010e50: 3a20 5b70 726f 6475 6374 206f 6620 575b  : [product of W[
+00010e60: 475b 445d 2c20 742c 2044 2c20 785d 2066  G[D], t, D, x] f
+00010e70: 6f72 2044 2069 6e20 7261 6e67 6528 6e5f  or D in range(n_
+00010e80: 6469 6d29 5d20 666f 7220 706f 696e 7420  dim)] for point 
+00010e90: 7820 616e 6420 6261 7463 6820 742e 0a20  x and batch t.. 
+00010ea0: 2020 2020 2020 2020 2020 2023 2057 673a             # Wg:
+00010eb0: 2028 5b6e 5f62 6174 6368 5d2c 207b 317d   ([n_batch], {1}
+00010ec0: 2c20 6e5f 6461 7461 203d 206e 5f31 2078  , n_data = n_1 x
+00010ed0: 206e 5f32 2078 202e 2e2e 2078 206e 5f72   n_2 x ... x n_r
+00010ee0: 290a 2020 2020 2020 2020 2020 2020 5767  ).            Wg
+00010ef0: 203d 2057 2e67 6174 6865 7228 302c 2047   = W.gather(0, G
+00010f00: 2e65 7870 616e 645f 746f 2828 312c 2920  .expand_to((1,) 
+00010f10: 2b20 572e 7368 6170 655b 313a 5d29 292e  + W.shape[1:])).
+00010f20: 7371 7565 657a 6528 3029 2e70 726f 6428  squeeze(0).prod(
+00010f30: 7b7d 2c20 6b65 6570 6469 6d3d 5472 7565  {}, keepdim=True
+00010f40: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00010f50: 436f 6d70 7574 6520 7468 6520 696e 6469  Compute the indi
+00010f60: 6365 7320 6f66 2072 656c 6174 6564 2063  ces of related c
+00010f70: 6f6e 7472 6f6c 2070 6f69 6e74 732e 2049  ontrol points. I
+00010f80: 6e64 3a20 285b 6e5f 6261 7463 685d 2c20  nd: ([n_batch], 
+00010f90: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
+00010fa0: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
+00010fb0: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
+00010fc0: 2020 2020 2049 6e64 203d 2062 742e 636c       Ind = bt.cl
+00010fd0: 616d 7028 6958 2e6c 6f6e 6728 2920 2b20  amp(iX.long() + 
+00010fe0: 4720 2d20 312c 206d 696e 3d30 290a 2020  G - 1, min=0).  
+00010ff0: 2020 2020 2020 2020 2020 496e 6420 3d20            Ind = 
+00011000: 6274 2e6d 696e 2849 6e64 2c20 2873 697a  bt.min(Ind, (siz
+00011010: 6520 2d20 3129 2e65 7870 616e 645f 746f  e - 1).expand_to
+00011020: 2849 6e64 2929 0a20 2020 2020 2020 2020  (Ind)).         
+00011030: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
+00011040: 2069 6e64 6963 6573 2074 6f20 3120 6469   indices to 1 di
+00011050: 6d65 6e73 696f 6e61 6c2e 2044 6f74 3a20  mensional. Dot: 
+00011060: 285b 6e5f 6261 7463 685d 2c20 6e5f 6461  ([n_batch], n_da
+00011070: 7461 203d 206e 5f31 2078 206e 5f32 2078  ta = n_1 x n_2 x
+00011080: 202e 2e2e 2078 206e 5f72 290a 2020 2020   ... x n_r).    
+00011090: 2020 2020 2020 2020 446f 7420 3d20 496e          Dot = In
+000110a0: 645b 3a2c 2030 5d0a 2020 2020 2020 2020  d[:, 0].        
+000110b0: 2020 2020 666f 7220 7220 696e 2072 616e      for r in ran
+000110c0: 6765 2831 2c20 6e5f 6469 6d29 3a20 446f  ge(1, n_dim): Do
+000110d0: 7420 2a3d 2073 697a 655b 725d 3b20 446f  t *= size[r]; Do
+000110e0: 7420 2b3d 2049 6e64 5b3a 2c20 725d 0a20  t += Ind[:, r]. 
+000110f0: 2020 2020 2020 2020 2020 2023 204f 6274             # Obt
+00011100: 6169 6e20 7468 6520 636f 6f72 6469 6e61  ain the coordina
+00011110: 7465 7320 6f66 2074 6865 2063 6f6e 7472  tes of the contr
+00011120: 6f6c 2070 6f69 6e74 732e 2043 506f 696e  ol points. CPoin
+00011130: 7473 3a20 285b 6e5f 6261 7463 685d 2c20  ts: ([n_batch], 
+00011140: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6120  {n_dim}, n_data 
+00011150: 3d20 6e5f 3120 7820 6e5f 3220 7820 2e2e  = n_1 x n_2 x ..
+00011160: 2e20 7820 6e5f 7229 0a20 2020 2020 2020  . x n_r).       
+00011170: 2020 2020 2043 506f 696e 7473 203d 206f       CPoints = o
+00011180: 6666 7365 7473 2e66 6c61 7474 656e 2829  ffsets.flatten()
+00011190: 2e67 6174 6865 7228 2d31 2c20 446f 742e  .gather(-1, Dot.
+000111a0: 6c6f 6e67 2829 2e65 7870 616e 645f 746f  long().expand_to
+000111b0: 2849 6e64 2929 2e66 6c6f 6174 2829 0a20  (Ind)).float(). 
+000111c0: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
+000111d0: 2074 6865 2077 6569 6768 7465 6420 636f   the weighted co
+000111e0: 6e74 726f 6c20 636f 6f72 6469 6e61 7465  ntrol coordinate
+000111f0: 7320 746f 2074 6865 206f 7574 7075 7420  s to the output 
+00011200: 636f 6f72 6469 6e61 7465 732e 0a20 2020  coordinates..   
+00011210: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00011220: 2b3d 2028 5767 202a 2043 506f 696e 7473  += (Wg * CPoints
+00011230: 292e 7669 6577 5f61 7328 5829 0a20 2020  ).view_as(X).   
+00011240: 2020 2020 2023 2044 656e 6f72 6d61 6c69       # Denormali
+00011250: 7a65 2074 6865 206f 7574 7075 7473 2e0a  ze the outputs..
+00011260: 2020 2020 2020 2020 6f75 7470 7574 202b          output +
+00011270: 3d20 580a 2020 2020 2020 2020 6f75 7470  = X.        outp
+00011280: 7574 202b 3d20 6274 2e63 6861 6e6e 656c  ut += bt.channel
+00011290: 5f74 656e 736f 7228 7365 6c66 2e6f 7269  _tensor(self.ori
+000112a0: 6769 6e29 0a20 2020 2020 2020 2072 6574  gin).        ret
+000112b0: 7572 6e20 6f75 7470 7574 2e76 6965 7728  urn output.view(
+000112c0: 7368 6170 6529 0a0a 4061 6c69 6173 2822  shape)..@alias("
+000112d0: 4444 4622 290a 636c 6173 7320 4465 6e73  DDF").class Dens
+000112e0: 6544 6973 706c 6163 656d 656e 7446 6965  eDisplacementFie
+000112f0: 6c64 2853 7061 7469 616c 5472 616e 7366  ld(SpatialTransf
+00011300: 6f72 6d61 7469 6f6e 293a 0a20 2020 2064  ormation):.    d
+00011310: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00011320: 2c20 6469 7370 6c61 6365 6d65 6e74 732c  , displacements,
+00011330: 2073 6861 7065 3d4e 6f6e 652c 2069 6e74   shape=None, int
+00011340: 6572 706f 6c61 7465 3d46 616c 7365 293a  erpolate=False):
+00011350: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00011360: 2020 2020 2044 656e 7365 2044 6973 706c       Dense Displ
+00011370: 6163 656d 656e 7420 4669 656c 6420 2844  acement Field (D
+00011380: 4446 2920 7472 616e 7366 6f72 6d61 7469  DF) transformati
+00011390: 6f6e 2e0a 2020 2020 2020 2020 0a20 2020  on..        .   
+000113a0: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
+000113b0: 2020 2020 2020 2020 2064 6973 706c 6163           displac
+000113c0: 656d 656e 7473 205b 6274 2e54 656e 736f  ements [bt.Tenso
+000113d0: 725d 3a20 7468 6520 6469 7370 6c61 6365  r]: the displace
+000113e0: 6d65 6e74 206f 6620 6561 6368 2076 6f78  ment of each vox
+000113f0: 656c 2e20 0a20 2020 2020 2020 2020 2020  el. .           
+00011400: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+00011410: 6174 6368 5d2c 207b 6e5f 6469 6d7d 2c20  atch], {n_dim}, 
+00011420: 6e40 312c 206e 4032 2c20 2e2e 2e2c 206e  n@1, n@2, ..., n
+00011430: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+00011440: 2020 2020 7368 6170 6520 5b62 742e 5369      shape [bt.Si
+00011450: 7a65 206f 7220 7475 706c 655d 3a20 7468  ze or tuple]: th
+00011460: 6520 7368 6170 6520 6f66 2064 6973 706c  e shape of displ
+00011470: 6163 656d 656e 7420 286e 6565 6465 6420  acement (needed 
+00011480: 6966 2069 6e70 7574 2064 6973 706c 6163  if input displac
+00011490: 656d 656e 7420 6973 2061 2074 7261 6e73  ement is a trans
+000114a0: 666f 726d 6174 696f 6e29 2e20 0a20 2020  formation). .   
+000114b0: 2020 2020 2020 2020 2069 6e74 6572 706f           interpo
+000114c0: 6c61 7465 205b 626f 6f6c 5d3a 2057 6865  late [bool]: Whe
+000114d0: 7468 6572 2074 6f20 666f 7263 6520 696e  ther to force in
+000114e0: 7465 7270 6f6c 6174 696f 6e20 696e 2061  terpolation in a
+000114f0: 7070 6c79 2e20 0a20 2020 2020 2020 2020  pply. .         
+00011500: 2020 200a 2020 2020 2020 2020 5768 656e     .        When
+00011510: 2069 7420 6973 2063 616c 6c65 643a 0a20   it is called:. 
+00011520: 2020 2020 2020 2020 2020 2058 205b 6274             X [bt
+00011530: 2e54 656e 736f 725d 3a20 436f 6f72 6469  .Tensor]: Coordi
+00011540: 6e61 7465 7320 746f 2062 6520 7472 616e  nates to be tran
+00011550: 7366 6f72 6d65 642e 0a20 2020 2020 2020  sformed..       
+00011560: 2020 2020 2020 2020 2073 697a 653a 2028           size: (
+00011570: 5b6e 5f62 6174 6368 3a20 6f70 7469 6f6e  [n_batch: option
+00011580: 616c 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  al], {n_dim}, n@
+00011590: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+000115a0: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
+000115b0: 2020 6f75 7470 7574 205b 6274 2e54 656e    output [bt.Ten
+000115c0: 736f 725d 3a20 5468 6520 7472 616e 7366  sor]: The transf
+000115d0: 6f72 6d65 6420 636f 6f72 6469 6e61 7465  ormed coordinate
+000115e0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+000115f0: 2020 2073 697a 653a 2028 5b6e 5f62 6174     size: ([n_bat
+00011600: 6368 5d2c 207b 6e5f 6469 6d7d 2c20 6e40  ch], {n_dim}, n@
+00011610: 312c 206e 4032 2c20 2e2e 2e2c 206e 406e  1, n@2, ..., n@n
+00011620: 5f64 696d 290a 2020 2020 2020 2020 2727  _dim).        ''
+00011630: 270a 2020 2020 2020 2020 6966 2069 7369  '.        if isi
+00011640: 6e73 7461 6e63 6528 6469 7370 6c61 6365  nstance(displace
+00011650: 6d65 6e74 732c 2053 7061 7469 616c 5472  ments, SpatialTr
+00011660: 616e 7366 6f72 6d61 7469 6f6e 293a 2064  ansformation): d
+00011670: 6973 706c 6163 656d 656e 7473 203d 2064  isplacements = d
+00011680: 6973 706c 6163 656d 656e 7473 2e74 6f44  isplacements.toD
+00011690: 4446 2873 6861 7065 290a 2020 2020 2020  DF(shape).      
+000116a0: 2020 6469 7370 6c61 6365 6d65 6e74 7320    displacements 
+000116b0: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
+000116c0: 2864 6973 706c 6163 656d 656e 7473 290a  (displacements).
+000116d0: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+000116e0: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
+000116f0: 5f63 6861 6e6e 656c 3a0a 2020 2020 2020  _channel:.      
+00011700: 2020 2020 2020 6966 2064 6973 706c 6163        if displac
+00011710: 656d 656e 7473 2e73 697a 6528 3029 203d  ements.size(0) =
+00011720: 3d20 6469 7370 6c61 6365 6d65 6e74 732e  = displacements.
+00011730: 6e5f 6469 6d20 2d20 313a 0a20 2020 2020  n_dim - 1:.     
+00011740: 2020 2020 2020 2020 2020 206e 5f64 696d             n_dim
+00011750: 203d 2064 6973 706c 6163 656d 656e 7473   = displacements
+00011760: 2e73 697a 6528 3029 0a20 2020 2020 2020  .size(0).       
+00011770: 2020 2020 2020 2020 2064 6973 706c 6163           displac
+00011780: 656d 656e 7473 2e63 6861 6e6e 656c 5f64  ements.channel_d
+00011790: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+000117a0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000117b0: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
+000117c0: 706c 6163 656d 656e 7473 2e75 6e73 7175  placements.unsqu
+000117d0: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
+000117e0: 2020 2020 2065 6c69 6620 6469 7370 6c61       elif displa
+000117f0: 6365 6d65 6e74 732e 7369 7a65 2831 2920  cements.size(1) 
+00011800: 3d3d 2064 6973 706c 6163 656d 656e 7473  == displacements
+00011810: 2e6e 5f64 696d 202d 2032 3a0a 2020 2020  .n_dim - 2:.    
+00011820: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
+00011830: 6d20 3d20 6469 7370 6c61 6365 6d65 6e74  m = displacement
+00011840: 732e 7369 7a65 2831 290a 2020 2020 2020  s.size(1).      
+00011850: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00011860: 6365 6d65 6e74 732e 6368 616e 6e65 6c5f  cements.channel_
+00011870: 6469 6d65 6e73 696f 6e20 3d20 310a 2020  dimension = 1.  
+00011880: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+00011890: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+000118a0: 6622 4444 4620 7061 7261 6d65 7465 7273  f"DDF parameters
+000118b0: 2077 6974 6820 7369 7a65 207b 6469 7370   with size {disp
+000118c0: 6c61 6365 6d65 6e74 732e 7368 6170 657d  lacements.shape}
+000118d0: 2064 6f6e 6f74 206d 6174 6368 2028 5b6e   donot match ([n
+000118e0: 5f62 6174 6368 5d2c 207b 7b6e 5f64 696d  _batch], {{n_dim
+000118f0: 7d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  }}, n@1, n@2, ..
+00011900: 2e2c 206e 406e 5f64 696d 292e 2022 290a  ., n@n_dim). ").
+00011910: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
+00011920: 6973 706c 6163 656d 656e 7473 2e68 6173  isplacements.has
+00011930: 5f62 6174 6368 3a0a 2020 2020 2020 2020  _batch:.        
+00011940: 2020 2020 6e5f 6469 6d20 3d20 6469 7370      n_dim = disp
+00011950: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
+00011960: 6e65 6c0a 2020 2020 2020 2020 2020 2020  nel.            
+00011970: 6966 2064 6973 706c 6163 656d 656e 7473  if displacements
+00011980: 2e6e 5f64 696d 203c 3d20 6e5f 6469 6d20  .n_dim <= n_dim 
+00011990: 2b20 313a 2064 6973 706c 6163 656d 656e  + 1: displacemen
+000119a0: 7473 203d 2064 6973 706c 6163 656d 656e  ts = displacemen
+000119b0: 7473 2e75 6e73 7175 6565 7a65 285b 5d29  ts.unsqueeze([])
+000119c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000119d0: 653a 2064 6973 706c 6163 656d 656e 7473  e: displacements
+000119e0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+000119f0: 203d 2030 0a20 2020 2020 2020 2064 6973   = 0.        dis
+00011a00: 706c 6163 656d 656e 7473 203d 2064 6973  placements = dis
+00011a10: 706c 6163 656d 656e 7473 2e66 6c6f 6174  placements.float
+00011a20: 2829 0a20 2020 2020 2020 2061 766f 7563  ().        avouc
+00011a30: 6828 6469 7370 6c61 6365 6d65 6e74 732e  h(displacements.
+00011a40: 6861 735f 6261 7463 6820 616e 6420 6469  has_batch and di
+00011a50: 7370 6c61 6365 6d65 6e74 732e 6861 735f  splacements.has_
+00011a60: 6368 616e 6e65 6c2c 2066 2250 6c65 6173  channel, f"Pleas
+00011a70: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+00011a80: 6e73 6f72 206f 6620 7369 7a65 205c 0a20  nsor of size \. 
+00011a90: 2020 2020 2020 2020 2020 2028 5b6e 5f62             ([n_b
+00011aa0: 6174 6368 5d2c 207b 7b6e 5f64 696d 7d7d  atch], {{n_dim}}
+00011ab0: 2c20 6e40 312c 206e 4032 2c20 2e2e 2e2c  , n@1, n@2, ...,
+00011ac0: 206e 406e 5f64 696d 2920 666f 7220 4444   n@n_dim) for DD
+00011ad0: 4620 7061 7261 6d65 7465 7273 2c20 696e  F parameters, in
+00011ae0: 7374 6561 6420 6f66 207b 6469 7370 6c61  stead of {displa
+00011af0: 6365 6d65 6e74 732e 7368 6170 657d 2e20  cements.shape}. 
+00011b00: 2229 0a20 2020 2020 2020 2073 7570 6572  ").        super
+00011b10: 2829 2e5f 5f69 6e69 745f 5f28 6469 7370  ().__init__(disp
+00011b20: 6c61 6365 6d65 6e74 732c 2073 6861 7065  lacements, shape
+00011b30: 3d73 6861 7065 2c20 696e 7465 7270 6f6c  =shape, interpol
+00011b40: 6174 653d 696e 7465 7270 6f6c 6174 6529  ate=interpolate)
+00011b50: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+00011b60: 6469 6d20 3d20 6469 7370 6c61 6365 6d65  dim = displaceme
+00011b70: 6e74 732e 6e5f 6368 616e 6e65 6c0a 2020  nts.n_channel.  
+00011b80: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
+00011b90: 6163 656d 656e 7473 203d 2064 6973 706c  acements = displ
+00011ba0: 6163 656d 656e 7473 0a20 2020 2020 2020  acements.       
+00011bb0: 2073 656c 662e 696e 7465 7270 6f6c 6174   self.interpolat
+00011bc0: 6520 3d20 696e 7465 7270 6f6c 6174 650a  e = interpolate.
+00011bd0: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
+00011be0: 6368 5f70 6172 616d 2e61 7070 656e 6428  ch_param.append(
+00011bf0: 2764 6973 706c 6163 656d 656e 7473 2729  'displacements')
+00011c00: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
+00011c10: 6361 6c6c 5f5f 2873 656c 662c 2058 293a  call__(self, X):
+00011c20: 0a20 2020 2020 2020 2058 203d 2073 7570  .        X = sup
+00011c30: 6572 2829 2e5f 5f63 616c 6c5f 5f28 5829  er().__call__(X)
+00011c40: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
+00011c50: 656d 656e 7473 203d 2073 656c 662e 6469  ements = self.di
+00011c60: 7370 6c61 6365 6d65 6e74 730a 2020 2020  splacements.    
+00011c70: 2020 2020 6e5f 6469 6d20 3d20 7365 6c66      n_dim = self
+00011c80: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
+00011c90: 6620 582e 6e5f 7370 6163 6520 3d3d 2030  f X.n_space == 0
+00011ca0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+00011cb0: 6528 2d31 290a 2020 2020 2020 2020 6966  e(-1).        if
+00011cc0: 206e 6f74 2073 656c 662e 696e 7465 7270   not self.interp
+00011cd0: 6f6c 6174 6520 616e 6420 582e 7370 6163  olate and X.spac
+00011ce0: 6520 3d3d 2064 6973 706c 6163 656d 656e  e == displacemen
+00011cf0: 7473 2e73 7061 6365 2061 6e64 2058 2e6e  ts.space and X.n
+00011d00: 5f63 6861 6e6e 656c 203d 3d20 6469 7370  _channel == disp
+00011d10: 6c61 6365 6d65 6e74 732e 6e5f 6368 616e  lacements.n_chan
+00011d20: 6e65 6c3a 2072 6574 7572 6e20 5820 2b20  nel: return X + 
+00011d30: 6469 7370 6c61 6365 6d65 6e74 730a 2020  displacements.  
+00011d40: 2020 2020 2020 656c 7365 3a20 7265 7475        else: retu
+00011d50: 726e 2058 202b 2069 6e74 6572 706f 6c61  rn X + interpola
+00011d60: 7469 6f6e 2864 6973 706c 6163 656d 656e  tion(displacemen
+00011d70: 7473 2c20 7461 7267 6574 5f73 7061 6365  ts, target_space
+00011d80: 3d58 292e 6368 616e 6e65 6c5f 6469 6d65  =X).channel_dime
+00011d90: 6e73 696f 6e5f 2831 290a 0a40 616c 6961  nsion_(1)..@alia
+00011da0: 7328 224d 4c50 2229 0a63 6c61 7373 204d  s("MLP").class M
+00011db0: 756c 7469 4c61 7965 7250 6572 6365 7074  ultiLayerPercept
+00011dc0: 696f 6e28 5370 6174 6961 6c54 7261 6e73  ion(SpatialTrans
+00011dd0: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+00011de0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00011df0: 662c 2077 6569 6768 7473 2c20 6869 6464  f, weights, hidd
+00011e00: 656e 5f6c 6179 6572 733d 5b5d 2c20 6163  en_layers=[], ac
+00011e10: 7469 7665 5f66 756e 6374 696f 6e3d 4e6f  tive_function=No
+00011e20: 6e65 2c20 7472 616e 735f 7374 7265 7463  ne, trans_stretc
+00011e30: 683d 3129 3a0a 2020 2020 2020 2020 2727  h=1):.        ''
+00011e40: 270a 2020 2020 2020 2020 4120 7472 616e  '.        A tran
+00011e50: 7366 6f72 6d61 7469 6f6e 2064 6566 696e  sformation defin
+00011e60: 6564 2062 7920 6120 4d4c 502e 200a 2020  ed by a MLP. .  
+00011e70: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00011e80: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
+00011e90: 2020 2077 6569 6768 7473 205b 6274 2e54     weights [bt.T
+00011ea0: 656e 736f 725d 3a20 7468 6520 7765 6967  ensor]: the weig
+00011eb0: 6874 7320 666f 7220 7468 6520 7065 7263  hts for the perc
+00011ec0: 6570 7469 6f6e 206e 6574 776f 726b 2e20  eption network. 
+00011ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ee0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+00011ef0: 5d2c 206e 5f64 696d 202a 206e 5f68 6c5f  ], n_dim * n_hl_
+00011f00: 3120 2b20 6e5f 686c 5f31 202b 2073 756d  1 + n_hl_1 + sum
+00011f10: 2869 3d31 2e2e 6b2d 3129 7b6e 5f68 6c5f  (i=1..k-1){n_hl_
+00011f20: 6920 2a20 6e5f 686c 5f7b 692b 317d 202b  i * n_hl_{i+1} +
+00011f30: 206e 5f68 6c5f 7b69 2b31 7d7d 202b 206e   n_hl_{i+1}} + n
+00011f40: 5f68 6c5f 6b20 2a20 6e5f 6469 6d20 2b20  _hl_k * n_dim + 
+00011f50: 6e5f 6469 6d29 0a20 2020 2020 2020 2020  n_dim).         
+00011f60: 2020 2020 2020 2077 6865 7265 206b 2069         where k i
+00011f70: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00011f80: 6869 6464 656e 206c 6179 6572 7320 616e  hidden layers an
+00011f90: 6420 6e5f 686c 5f69 2069 7320 7468 6520  d n_hl_i is the 
+00011fa0: 6c65 6e67 7468 206f 6620 7468 6520 692d  length of the i-
+00011fb0: 7468 2068 6964 6465 6e20 6c61 7965 722e  th hidden layer.
+00011fc0: 200a 2020 2020 2020 2020 2020 2020 6869   .            hi
+00011fd0: 6464 656e 5f6c 6179 6572 7320 5b6c 6973  dden_layers [lis
+00011fe0: 7420 6f66 2069 6e74 5d3a 2074 6865 206c  t of int]: the l
+00011ff0: 656e 6774 6873 2066 6f72 2074 6865 2068  engths for the h
+00012000: 6964 6465 6e20 6c61 7965 7273 2c20 692e  idden layers, i.
+00012010: 652e 205b 6e5f 686c 5f31 2c20 6e5f 686c  e. [n_hl_1, n_hl
+00012020: 5f32 2c20 2e2e 2e2c 206e 5f68 6c5f 6b5d  _2, ..., n_hl_k]
+00012030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012040: 2049 7420 6973 2062 7920 6465 6661 756c   It is by defaul
+00012050: 7420 275b 5d27 2073 6f20 7468 6174 2074  t '[]' so that t
+00012060: 6865 2064 6566 6175 6c74 204d 4c50 2069  he default MLP i
+00012070: 7320 616e 2061 6666 696e 6520 7472 616e  s an affine tran
+00012080: 7366 6f72 6d61 7469 6f6e 2e20 0a20 2020  sformation. .   
+00012090: 2020 2020 2020 2020 2061 6374 6976 655f           active_
+000120a0: 6675 6e63 7469 6f6e 205b 636c 6173 735d  function [class]
+000120b0: 3a20 7468 6520 6163 7469 7665 5f66 756e  : the active_fun
+000120c0: 6374 696f 6e2e 200a 2020 2020 2020 2020  ction. .        
+000120d0: 2020 2020 7472 616e 735f 7374 7265 7463      trans_stretc
+000120e0: 6820 5b69 6e74 5d3a 2031 2062 7920 6465  h [int]: 1 by de
+000120f0: 6661 756c 742e 2032 3020 7365 656d 7320  fault. 20 seems 
+00012100: 746f 2062 6520 6120 676f 6f64 2063 686f  to be a good cho
+00012110: 6963 652e 200a 2020 2020 2020 2020 2020  ice. .          
+00012120: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+00012130: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+00012140: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+00012150: 5465 6e73 6f72 5d3a 2043 6f6f 7264 696e  Tensor]: Coordin
+00012160: 6174 6573 2074 6f20 6265 2074 7261 6e73  ates to be trans
+00012170: 666f 726d 6564 2e0a 2020 2020 2020 2020  formed..        
+00012180: 2020 2020 2020 2020 7369 7a65 3a20 285b          size: ([
+00012190: 6e5f 6261 7463 683a 206f 7074 696f 6e61  n_batch: optiona
+000121a0: 6c5d 2c20 7b6e 5f64 696d 7d2c 206e 4031  l], {n_dim}, n@1
+000121b0: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+000121c0: 6469 6d29 0a20 2020 2020 2020 2020 2020  dim).           
+000121d0: 206f 7574 7075 7420 5b62 742e 5465 6e73   output [bt.Tens
+000121e0: 6f72 5d3a 2054 6865 2074 7261 6e73 666f  or]: The transfo
+000121f0: 726d 6564 2063 6f6f 7264 696e 6174 6573  rmed coordinates
+00012200: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012210: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00012220: 685d 2c20 7b6e 5f64 696d 7d2c 206e 4031  h], {n_dim}, n@1
+00012230: 2c20 6e40 322c 202e 2e2e 2c20 6e40 6e5f  , n@2, ..., n@n_
+00012240: 6469 6d29 0a20 2020 2020 2020 2027 2727  dim).        '''
+00012250: 0a20 2020 2020 2020 2073 656c 662e 6869  .        self.hi
+00012260: 6464 656e 5f6c 6179 6572 7320 3d20 6869  dden_layers = hi
+00012270: 6464 656e 5f6c 6179 6572 730a 2020 2020  dden_layers.    
+00012280: 2020 2020 6966 206e 6f74 2077 6569 6768      if not weigh
+00012290: 7473 2e68 6173 5f62 6174 6368 3a0a 2020  ts.has_batch:.  
+000122a0: 2020 2020 2020 2020 2020 6966 2077 6569            if wei
+000122b0: 6768 7473 2e6e 5f64 696d 203d 3d20 323a  ghts.n_dim == 2:
+000122c0: 2077 6569 6768 7473 2e62 6174 6368 5f64   weights.batch_d
+000122d0: 696d 203d 2030 0a20 2020 2020 2020 2020  im = 0.         
+000122e0: 2020 2065 6c73 653a 2077 6569 6768 7473     else: weights
+000122f0: 203d 2077 6569 6768 7473 2e75 6e73 7175   = weights.unsqu
+00012300: 6565 7a65 285b 5d29 0a20 2020 2020 2020  eeze([]).       
+00012310: 2073 656c 662e 7765 6967 6874 7320 3d20   self.weights = 
+00012320: 7765 6967 6874 730a 2020 2020 2020 2020  weights.        
+00012330: 7365 6c66 2e74 7261 6e73 5f73 7472 6574  self.trans_stret
+00012340: 6368 203d 2074 7261 6e73 5f73 7472 6574  ch = trans_stret
+00012350: 6368 0a20 2020 2020 2020 2073 7570 6572  ch.        super
+00012360: 2829 2e5f 5f69 6e69 745f 5f28 7765 6967  ().__init__(weig
+00012370: 6874 732c 2068 6964 6465 6e5f 6c61 7965  hts, hidden_laye
+00012380: 7273 203d 2068 6964 6465 6e5f 6c61 7965  rs = hidden_laye
+00012390: 7273 2c20 7472 616e 735f 7374 7265 7463  rs, trans_stretc
+000123a0: 6820 3d20 7472 616e 735f 7374 7265 7463  h = trans_stretc
+000123b0: 6829 0a20 2020 2020 2020 2064 696d 5f63  h).        dim_c
+000123c0: 6f6e 7374 203d 2077 6569 6768 7473 2e73  onst = weights.s
+000123d0: 697a 6528 2d31 2920 2d20 7375 6d28 6869  ize(-1) - sum(hi
+000123e0: 6464 656e 5f6c 6179 6572 7329 202d 2073  dden_layers) - s
+000123f0: 756d 2878 202a 2079 2066 6f72 2078 2c20  um(x * y for x, 
+00012400: 7920 696e 207a 6970 2868 6964 6465 6e5f  y in zip(hidden_
+00012410: 6c61 7965 7273 5b3a 2d31 5d2c 2068 6964  layers[:-1], hid
+00012420: 6465 6e5f 6c61 7965 7273 5b31 3a5d 2929  den_layers[1:]))
+00012430: 0a20 2020 2020 2020 2064 696d 5f63 6f65  .        dim_coe
+00012440: 6666 203d 2068 6964 6465 6e5f 6c61 7965  ff = hidden_laye
+00012450: 7273 5b30 5d20 2b20 6869 6464 656e 5f6c  rs[0] + hidden_l
+00012460: 6179 6572 735b 2d31 5d20 2b20 310a 2020  ayers[-1] + 1.  
+00012470: 2020 2020 2020 6176 6f75 6368 2864 696d        avouch(dim
+00012480: 5f63 6f6e 7374 2025 2064 696d 5f63 6f65  _const % dim_coe
+00012490: 6666 203d 3d20 302c 2066 2257 726f 6e67  ff == 0, f"Wrong
+000124a0: 2077 6569 6768 7420 6c65 6e67 7468 2066   weight length f
+000124b0: 6f72 2068 6964 6465 6e20 6c61 7965 7273  or hidden layers
+000124c0: 206f 6620 7369 7a65 7320 7b68 6964 6465   of sizes {hidde
+000124d0: 6e5f 6c61 7965 7273 7d2c 207b 6469 6d5f  n_layers}, {dim_
+000124e0: 636f 6566 667d 2078 206e 5f64 696d 202b  coeff} x n_dim +
+000124f0: 207b 6469 6d5f 636f 6e73 747d 2065 7870   {dim_const} exp
+00012500: 6563 7465 642c 2062 7574 2067 6f74 207b  ected, but got {
+00012510: 7765 6967 6874 732e 7369 7a65 282d 3129  weights.size(-1)
+00012520: 7d2e 2229 0a20 2020 2020 2020 2073 656c  }.").        sel
+00012530: 662e 6e5f 6469 6d20 3d20 6469 6d5f 636f  f.n_dim = dim_co
+00012540: 6e73 7420 2f2f 2064 696d 5f63 6f65 6666  nst // dim_coeff
+00012550: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+00012560: 6261 7463 6820 3d20 7765 6967 6874 732e  batch = weights.
+00012570: 6e5f 6261 7463 680a 2020 2020 2020 2020  n_batch.        
+00012580: 7365 6c66 2e6c 6179 6572 7320 3d20 5b5d  self.layers = []
+00012590: 0a20 2020 2020 2020 2070 203d 2030 0a20  .        p = 0. 
+000125a0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000125b0: 7261 6e67 6528 6c65 6e28 6869 6464 656e  range(len(hidden
+000125c0: 5f6c 6179 6572 7329 202b 2031 293a 0a20  _layers) + 1):. 
+000125d0: 2020 2020 2020 2020 2020 2069 6e5f 6665             in_fe
+000125e0: 6174 7572 6573 203d 2073 656c 662e 6e5f  atures = self.n_
+000125f0: 6469 6d20 6966 2069 203d 3d20 3020 656c  dim if i == 0 el
+00012600: 7365 2068 6964 6465 6e5f 6c61 7965 7273  se hidden_layers
+00012610: 5b69 202d 2031 5d0a 2020 2020 2020 2020  [i - 1].        
+00012620: 2020 2020 6f75 745f 6665 6174 7572 6573      out_features
+00012630: 203d 2073 656c 662e 6e5f 6469 6d20 6966   = self.n_dim if
+00012640: 2069 203d 3d20 6c65 6e28 6869 6464 656e   i == len(hidden
+00012650: 5f6c 6179 6572 7329 2065 6c73 6520 6869  _layers) else hi
+00012660: 6464 656e 5f6c 6179 6572 735b 695d 0a20  dden_layers[i]. 
+00012670: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+00012680: 5f77 6569 6768 7473 203d 2077 6569 6768  _weights = weigh
+00012690: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
+000126a0: 6665 6174 7572 6573 2a69 6e5f 6665 6174  features*in_feat
+000126b0: 7572 6573 5d2e 7669 6577 285b 7365 6c66  ures].view([self
+000126c0: 2e6e 5f62 6174 6368 5d2c 206f 7574 5f66  .n_batch], out_f
+000126d0: 6561 7475 7265 732c 2069 6e5f 6665 6174  eatures, in_feat
+000126e0: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
+000126f0: 2020 7020 2b3d 206f 7574 5f66 6561 7475    p += out_featu
+00012700: 7265 7320 2a20 696e 5f66 6561 7475 7265  res * in_feature
+00012710: 730a 2020 2020 2020 2020 2020 2020 6c61  s.            la
+00012720: 7965 725f 6269 6173 203d 2077 6569 6768  yer_bias = weigh
+00012730: 7473 5b2e 2e2e 2c20 703a 702b 6f75 745f  ts[..., p:p+out_
+00012740: 6665 6174 7572 6573 5d2e 7669 6577 285b  features].view([
+00012750: 7365 6c66 2e6e 5f62 6174 6368 5d2c 206f  self.n_batch], o
+00012760: 7574 5f66 6561 7475 7265 7329 0a20 2020  ut_features).   
+00012770: 2020 2020 2020 2020 2070 202b 3d20 6f75           p += ou
+00012780: 745f 6665 6174 7572 6573 0a20 2020 2020  t_features.     
+00012790: 2020 2020 2020 2073 656c 662e 6c61 7965         self.laye
+000127a0: 7273 2e61 7070 656e 6428 286c 6179 6572  rs.append((layer
+000127b0: 5f77 6569 6768 7473 2c20 6c61 7965 725f  _weights, layer_
+000127c0: 6269 6173 2929 0a20 2020 2020 2020 2073  bias)).        s
+000127d0: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
+000127e0: 696f 6e20 3d20 6163 7469 7665 5f66 756e  ion = active_fun
+000127f0: 6374 696f 6e0a 2020 2020 2020 2020 6966  ction.        if
+00012800: 2073 656c 662e 6163 7469 7665 5f66 756e   self.active_fun
+00012810: 6374 696f 6e20 6973 204e 6f6e 653a 2073  ction is None: s
+00012820: 656c 662e 6163 7469 7665 5f66 756e 6374  elf.active_funct
+00012830: 696f 6e20 3d20 6274 2e6e 6e2e 5265 4c55  ion = bt.nn.ReLU
+00012840: 0a20 2020 200a 2020 2020 4070 726f 7065  .    .    @prope
+00012850: 7274 790a 2020 2020 6465 6620 6e5f 7765  rty.    def n_we
+00012860: 6967 6874 5f6c 656e 6774 6828 7365 6c66  ight_length(self
+00012870: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00012880: 6e20 7365 6c66 2e6e 5f64 696d 202a 2028  n self.n_dim * (
+00012890: 7365 6c66 2e68 6964 6465 6e5f 6c61 7965  self.hidden_laye
+000128a0: 7273 5b30 5d20 2b20 7365 6c66 2e68 6964  rs[0] + self.hid
+000128b0: 6465 6e5f 6c61 7965 7273 5b2d 315d 202b  den_layers[-1] +
+000128c0: 2031 2920 2b20 7375 6d28 7365 6c66 2e68   1) + sum(self.h
+000128d0: 6964 6465 6e5f 6c61 7965 7273 2920 2b20  idden_layers) + 
+000128e0: 7375 6d28 7820 2a20 7920 666f 7220 782c  sum(x * y for x,
+000128f0: 2079 2069 6e20 7a69 7028 7365 6c66 2e68   y in zip(self.h
+00012900: 6964 6465 6e5f 6c61 7965 7273 5b3a 2d31  idden_layers[:-1
+00012910: 5d2c 2073 656c 662e 6869 6464 656e 5f6c  ], self.hidden_l
+00012920: 6179 6572 735b 313a 5d29 290a 2020 2020  ayers[1:])).    
+00012930: 0a20 2020 2064 6566 205f 5f63 616c 6c5f  .    def __call_
+00012940: 5f28 7365 6c66 2c20 5829 3a0a 2020 2020  _(self, X):.    
+00012950: 2020 2020 5820 3d20 7375 7065 7228 292e      X = super().
+00012960: 5f5f 6361 6c6c 5f5f 2858 290a 2020 2020  __call__(X).    
+00012970: 2020 2020 6966 2058 2e6e 5f73 7061 6365      if X.n_space
+00012980: 203d 3d20 303a 2058 203d 2058 2e75 6e73   == 0: X = X.uns
+00012990: 7175 6565 7a65 282d 3129 0a20 2020 2020  queeze(-1).     
+000129a0: 2020 2059 203d 2058 2e66 6c61 7474 656e     Y = X.flatten
+000129b0: 2829 2e63 6861 6e6e 656c 5f64 696d 5f28  ().channel_dim_(
+000129c0: 4e6f 6e65 290a 2020 2020 2020 2020 666f  None).        fo
+000129d0: 7220 692c 2028 7765 6967 6874 732c 2062  r i, (weights, b
+000129e0: 6961 7329 2069 6e20 656e 756d 6572 6174  ias) in enumerat
+000129f0: 6528 7365 6c66 2e6c 6179 6572 7329 3a0a  e(self.layers):.
+00012a00: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
+00012a10: 7765 6967 6874 7320 4020 590a 2020 2020  weights @ Y.    
+00012a20: 2020 2020 2020 2020 6966 2069 203c 206c          if i < l
+00012a30: 656e 2873 656c 662e 6c61 7965 7273 2920  en(self.layers) 
+00012a40: 2d20 313a 2059 203d 2073 656c 662e 6163  - 1: Y = self.ac
+00012a50: 7469 7665 5f66 756e 6374 696f 6e28 2928  tive_function()(
+00012a60: 5920 2b20 6269 6173 2e75 6e73 7175 6565  Y + bias.unsquee
+00012a70: 7a65 282d 3129 290a 2020 2020 2020 2020  ze(-1)).        
+00012a80: 2020 2020 656c 7365 3a20 5920 2b3d 2073      else: Y += s
+00012a90: 656c 662e 7472 616e 735f 7374 7265 7463  elf.trans_stretc
+00012aa0: 6820 2a20 6269 6173 2e75 6e73 7175 6565  h * bias.unsquee
+00012ab0: 7a65 282d 3129 0a20 2020 2020 2020 2072  ze(-1).        r
+00012ac0: 6574 7572 6e20 5820 2b20 592e 7669 6577  eturn X + Y.view
+00012ad0: 5f61 7328 5829 2e63 6861 6e6e 656c 5f64  _as(X).channel_d
+00012ae0: 696d 656e 7369 6f6e 5f28 3129 0a0a 4061  imension_(1)..@a
+00012af0: 6c69 6173 2822 7265 7361 6d70 6c65 2229  lias("resample")
+00012b00: 0a64 6566 2069 6e74 6572 706f 6c61 7469  .def interpolati
+00012b10: 6f6e 280a 2020 2020 2020 2020 696d 6167  on(.        imag
+00012b20: 653a 2062 742e 5465 6e73 6f72 2c20 0a20  e: bt.Tensor, . 
+00012b30: 2020 2020 2020 2074 7261 6e73 3a20 4361         trans: Ca
+00012b40: 6c6c 6162 6c65 203d 204e 6f6e 652c 200a  llable = None, .
+00012b50: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+00012b60: 7374 7220 3d20 274c 696e 6561 7227 2c20  str = 'Linear', 
+00012b70: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+00012b80: 7370 6163 653a 2074 7570 6c65 203d 204e  space: tuple = N
+00012b90: 6f6e 652c 0a20 2020 2020 2020 2066 696c  one,.        fil
+00012ba0: 6c3a 2028 7374 722c 2069 6e74 2c20 666c  l: (str, int, fl
+00012bb0: 6f61 7429 203d 2030 2c0a 2020 2020 2020  oat) = 0,.      
+00012bc0: 2020 6465 7269 7661 7469 7665 3a20 626f    derivative: bo
+00012bd0: 6f6c 203d 2046 616c 7365 0a20 2020 2029  ol = False.    )
+00012be0: 3a0a 2020 2020 2727 270a 2020 2020 496e  :.    '''.    In
+00012bf0: 7465 7270 6f6c 6174 6520 7573 696e 6720  terpolate using 
+00012c00: 6261 636b 7761 7264 2074 7261 6e73 666f  backward transfo
+00012c10: 726d 6174 696f 6e2e 0a20 2020 2069 2e65  rmation..    i.e
+00012c20: 2e20 436f 6d70 7574 6520 7468 6520 696d  . Compute the im
+00012c30: 6167 6520 4920 732e 742e 2074 7261 6e73  age I s.t. trans
+00012c40: 2878 2920 3d20 7920 666f 7220 7820 696e  (x) = y for x in
+00012c50: 2049 2061 6e64 2079 2069 6e20 696e 7075   I and y in inpu
+00012c60: 7420 696d 6167 6520 7573 696e 6720 696e  t image using in
+00012c70: 7465 7270 6f6c 6174 696f 6e20 6d65 7468  terpolation meth
+00012c80: 6f64 3a0a 2020 2020 2020 2020 6d65 7468  od:.        meth
+00012c90: 6f64 203d 204c 696e 6561 723a 2042 696c  od = Linear: Bil
+00012ca0: 696e 6561 7220 696e 7465 7270 6f6c 6174  inear interpolat
+00012cb0: 696f 6e0a 2020 2020 2020 2020 6d65 7468  ion.        meth
+00012cc0: 6f64 203d 204e 6561 7265 7374 205b 4e4f  od = Nearest [NO
+00012cd0: 2047 5241 4449 454e 5421 2121 5d3a 204e   GRADIENT!!!]: N
+00012ce0: 6561 7265 7374 2069 6e74 6572 706f 6c61  earest interpola
+00012cf0: 7469 6f6e 0a0a 2020 2020 5061 7261 6d73  tion..    Params
+00012d00: 3a0a 2020 2020 2020 2020 696d 6167 6520  :.        image 
+00012d10: 5b62 742e 5465 6e73 6f72 5d3a 2054 6865  [bt.Tensor]: The
+00012d20: 2074 6172 6765 7420 696d 6167 652e 0a20   target image.. 
+00012d30: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+00012d40: 2028 5b6e 5f62 6174 6368 3a6f 7074 696f   ([n_batch:optio
+00012d50: 6e61 6c5d 2c20 7b6e 5f63 6861 6e6e 656c  nal], {n_channel
+00012d60: 3a6f 7074 696f 6e61 6c7d 2c20 6d40 312c  :optional}, m@1,
+00012d70: 206d 4032 2c20 2e2e 2e2c 206d 406e 5f64   m@2, ..., m@n_d
+00012d80: 696d 290a 2020 2020 2020 2020 7472 616e  im).        tran
+00012d90: 7320 5b46 756e 6374 696f 6e20 6f72 206d  s [Function or m
+00012da0: 6963 6f6d 7075 7469 6e67 2e53 7061 7469  icomputing.Spati
+00012db0: 616c 5472 616e 7366 6f72 6d61 7469 6f6e  alTransformation
+00012dc0: 5d3a 2054 7261 6e73 666f 726d 6174 696f  ]: Transformatio
+00012dd0: 6e20 6675 6e63 7469 6f6e 2c20 6d61 7070  n function, mapp
+00012de0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00012df0: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00012e00: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6469  optional], {n_di
+00012e10: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
+00012e20: 2e2c 206e 406e 5f64 696d 2920 746f 2028  ., n@n_dim) to (
+00012e30: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+00012e40: 6d7d 2c20 6e40 312c 206e 4032 2c20 2e2e  m}, n@1, n@2, ..
+00012e50: 2e2c 206e 406e 5f64 696d 290a 2020 2020  ., n@n_dim).    
+00012e60: 2020 2020 6d65 7468 6f64 205b 7374 723a      method [str:
+00012e70: 206c 696e 6561 727c 6e65 6172 6573 745d   linear|nearest]
+00012e80: 3a20 5468 6520 696e 7465 7270 6f6c 6174  : The interpolat
+00012e90: 696f 6e20 6d65 7468 6f64 2e20 0a20 2020  ion method. .   
+00012ea0: 2020 2020 2074 6172 6765 745f 7370 6163       target_spac
+00012eb0: 6520 5b74 7570 6c65 206f 7220 6274 2e54  e [tuple or bt.T
+00012ec0: 656e 736f 725d 3a0a 2020 2020 2020 2020  ensor]:.        
+00012ed0: 2020 2020 5369 7a65 2028 7475 706c 6529      Size (tuple)
+00012ee0: 206f 6620 6120 7461 7267 6574 2052 4f49   of a target ROI
+00012ef0: 2061 7420 7468 6520 6365 6e74 6572 206f   at the center o
+00012f00: 6620 696d 6167 652e 200a 2020 2020 2020  f image. .      
+00012f10: 2020 2020 2020 4f52 2054 7261 6e73 666f        OR Transfo
+00012f20: 726d 6564 2063 6f6f 7264 696e 6174 6520  rmed coordinate 
+00012f30: 7370 6163 6520 2862 742e 5465 6e73 6f72  space (bt.Tensor
+00012f40: 2920 6f66 2074 6865 206f 7574 7075 7420  ) of the output 
+00012f50: 696d 6167 652e 200a 2020 2020 2020 2020  image. .        
+00012f60: 2020 2020 7369 7a65 3a20 6c65 6e67 7468      size: length
+00012f70: 286e 5f64 696d 2920 6f72 2028 5b6e 5f62  (n_dim) or ([n_b
+00012f80: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00012f90: 7b6e 5f64 696d 3a6f 7074 696f 6e61 6c7d  {n_dim:optional}
+00012fa0: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
+00012fb0: 2c20 2e2e 2e2c 2073 697a 6540 7229 0a20  , ..., size@r). 
+00012fc0: 2020 2020 2020 2066 696c 6c20 5b73 7472         fill [str
+00012fd0: 3a20 6e65 6172 6573 747c 6261 636b 6772  : nearest|backgr
+00012fe0: 6f75 6e64 206f 7220 696e 7420 6f72 2066  ound or int or f
+00012ff0: 6c6f 6174 286e 756d 6265 7229 5d3a 2049  loat(number)]: I
+00013000: 6e64 6963 6174 6520 7468 6520 7761 7920  ndicate the way 
+00013010: 746f 2066 696c 6c20 6261 636b 6772 6f75  to fill backgrou
+00013020: 6e64 206f 7574 7369 6465 2060 5375 7272  nd outside `Surr
+00013030: 6f75 6e64 696e 6760 2e20 0a20 2020 2020  ounding`. .     
+00013040: 2020 2064 6572 6976 6174 6976 6520 5b62     derivative [b
+00013050: 6f6f 6c5d 3a20 5768 6574 6865 7220 746f  ool]: Whether to
+00013060: 2072 6574 7572 6e20 7468 6520 6772 6164   return the grad
+00013070: 6965 6e74 2e20 4f6e 6520 6361 6e20 6f6d  ient. One can om
+00013080: 6974 2069 7420 7768 656e 2075 7369 6e67  it it when using
+00013090: 2074 6f72 6368 2e61 7574 6f67 7261 642e   torch.autograd.
+000130a0: 0a0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
+000130b0: 205b 6274 2e54 656e 736f 725d 3a20 5468   [bt.Tensor]: Th
+000130c0: 6520 7472 616e 7366 6f72 6d65 6420 696d  e transformed im
+000130d0: 6167 652e 0a20 2020 2020 2020 2020 2020  age..           
+000130e0: 2073 697a 653a 2028 5b6e 5f62 6174 6368   size: ([n_batch
+000130f0: 5d2c 207b 6e5f 6368 616e 6e65 6c3a 6f70  ], {n_channel:op
+00013100: 7469 6f6e 616c 7d2c 206d 4031 2c20 6d40  tional}, m@1, m@
+00013110: 322c 202e 2e2e 2c20 6d40 6e5f 6469 6d29  2, ..., m@n_dim)
+00013120: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+00013130: 7768 656e 2060 7461 7267 6574 5f73 7061  when `target_spa
+00013140: 6365 6020 6973 2064 6566 696e 6564 2062  ce` is defined b
+00013150: 7920 7465 6e73 6f72 2e20 0a20 2020 2020  y tensor. .     
+00013160: 2020 2020 2020 2073 697a 653a 2028 5b6e         size: ([n
+00013170: 5f62 6174 6368 5d2c 2073 697a 6540 312c  _batch], size@1,
+00013180: 2073 697a 6540 322c 202e 2e2e 2c20 7369   size@2, ..., si
+00013190: 7a65 406e 5f64 696d 290a 2020 2020 2020  ze@n_dim).      
+000131a0: 2020 2020 2020 6f72 2074 6865 2064 6572        or the der
+000131b0: 6976 6174 6976 6520 666f 7220 7468 6520  ivative for the 
+000131c0: 696e 7465 7270 6f6c 6174 696f 6e2e 2028  interpolation. (
+000131d0: 6966 2060 6465 7269 7661 7469 7665 203d  if `derivative =
+000131e0: 2054 7275 6560 290a 2020 2020 2020 2020   True`).        
+000131f0: 2020 2020 7369 7a65 3a20 285b 6e5f 6261      size: ([n_ba
+00013200: 7463 685d 2c20 7b6e 5f64 696d 7d2c 2073  tch], {n_dim}, s
+00013210: 697a 6540 312c 2073 697a 6540 322c 202e  ize@1, size@2, .
+00013220: 2e2e 2c20 7369 7a65 406e 5f64 696d 290a  .., size@n_dim).
+00013230: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
+00013240: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00013250: 2020 3e3e 3e20 496d 6167 6520 3d20 6274    >>> Image = bt
+00013260: 2e72 616e 6428 332c 2031 3030 2c20 3132  .rand(3, 100, 12
+00013270: 302c 2038 3029 0a20 2020 203e 3e3e 2041  0, 80).    >>> A
+00013280: 4d20 3d20 6274 2e72 616e 6428 342c 2034  M = bt.rand(4, 4
+00013290: 290a 2020 2020 3e3e 3e20 414d 5b33 2c20  ).    >>> AM[3, 
+000132a0: 3a5d 203d 2062 742e 6f6e 655f 686f 7428  :] = bt.one_hot(
+000132b0: 2d31 2c20 3429 0a20 2020 203e 3e3e 2069  -1, 4).    >>> i
+000132c0: 6e74 6572 706f 6c61 7469 6f6e 2849 6d61  nterpolation(Ima
+000132d0: 6765 2c20 4166 6669 6e65 2841 4d29 2c20  ge, Affine(AM), 
+000132e0: 6d65 7468 6f64 3d27 4c69 6e65 6172 2729  method='Linear')
+000132f0: 0a20 2020 2027 2727 0a20 2020 2069 6620  .    '''.    if 
+00013300: 7472 616e 7320 6973 206e 6f74 204e 6f6e  trans is not Non
+00013310: 6520 616e 6420 6e6f 7420 7472 616e 732e  e and not trans.
+00013320: 6261 636b 7761 7264 3a0a 2020 2020 2020  backward:.      
+00013330: 2020 6966 2068 6173 6174 7472 2874 7261    if hasattr(tra
+00013340: 6e73 2c20 2769 6e76 2729 3a20 7472 616e  ns, 'inv'): tran
+00013350: 7320 3d20 7472 616e 732e 696e 7628 292e  s = trans.inv().
+00013360: 6661 6b65 5f69 6e76 2829 0a20 2020 2020  fake_inv().     
+00013370: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013380: 2020 2020 2070 7269 6e74 2822 5761 726e       print("Warn
+00013390: 696e 673a 2046 6f72 7761 7264 2074 7261  ing: Forward tra
+000133a0: 6e73 666f 726d 6174 696f 6e20 666f 756e  nsformation foun
+000133b0: 6420 696e 206d 6574 686f 6420 6069 6e74  d in method `int
+000133c0: 6572 706f 6c61 7469 6f6e 602e 2055 7369  erpolation`. Usi
+000133d0: 6e67 2060 696e 7465 7270 6f6c 6174 696f  ng `interpolatio
+000133e0: 6e5f 666f 7277 6172 6460 2069 6e73 7465  n_forward` inste
+000133f0: 6164 2e20 2229 0a20 2020 2020 2020 2020  ad. ").         
+00013400: 2020 2072 6574 7572 6e20 696e 7465 7270     return interp
+00013410: 6f6c 6174 696f 6e5f 666f 7277 6172 6428  olation_forward(
+00013420: 696d 6167 652c 2074 7261 6e73 2c20 6d65  image, trans, me
+00013430: 7468 6f64 203d 206d 6574 686f 642c 2074  thod = method, t
+00013440: 6172 6765 745f 7370 6163 6520 3d20 7461  arget_space = ta
+00013450: 7267 6574 5f73 7061 6365 2c20 6669 6c6c  rget_space, fill
+00013460: 203d 2066 696c 6c29 0a20 2020 2069 6d61   = fill).    ima
+00013470: 6765 203d 2062 742e 746f 5f64 6576 6963  ge = bt.to_devic
+00013480: 6528 6261 746f 7263 685f 7465 6e73 6f72  e(batorch_tensor
+00013490: 2869 6d61 6765 2929 0a20 2020 2073 6861  (image)).    sha
+000134a0: 7065 5f6f 7574 203d 2069 6d61 6765 2e73  pe_out = image.s
+000134b0: 6861 7065 0a20 2020 2069 6620 7472 616e  hape.    if tran
+000134c0: 7320 6973 204e 6f6e 6520 6f72 2074 7261  s is None or tra
+000134d0: 6e73 2e6e 5f64 696d 2069 7320 4e6f 6e65  ns.n_dim is None
+000134e0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+000134f0: 2069 6d61 6765 2e68 6173 5f62 6174 6368   image.has_batch
+00013500: 3a20 696d 6167 652e 756e 7371 7565 657a  : image.unsqueez
+00013510: 655f 285b 5d29 0a20 2020 2020 2020 2069  e_([]).        i
+00013520: 6620 6e6f 7420 696d 6167 652e 6861 735f  f not image.has_
+00013530: 6368 616e 6e65 6c3a 2069 6d61 6765 2e73  channel: image.s
+00013540: 7461 6e64 6172 645f 2829 2e75 6e73 7175  tandard_().unsqu
+00013550: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
+00013560: 2020 206e 5f64 696d 203d 2069 6d61 6765     n_dim = image
+00013570: 2e6e 5f73 7061 6365 2023 2047 6574 2074  .n_space # Get t
+00013580: 6865 2073 7061 7469 616c 2072 616e 6b2e  he spatial rank.
+00013590: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000135a0: 2020 206e 5f64 696d 203d 2074 7261 6e73     n_dim = trans
+000135b0: 2e6e 5f64 696d 0a20 2020 2020 2020 2069  .n_dim.        i
+000135c0: 6620 696d 6167 652e 6e5f 6469 6d20 3d3d  f image.n_dim ==
+000135d0: 206e 5f64 696d 3a0a 2020 2020 2020 2020   n_dim:.        
+000135e0: 2020 2020 6966 2069 6d61 6765 2e68 6173      if image.has
+000135f0: 5f73 7065 6369 616c 3a0a 2020 2020 2020  _special:.      
+00013600: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00013610: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
+00013620: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
+00013630: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
+00013640: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
+00013650: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
+00013660: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
+00013670: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
+00013680: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
+00013690: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
+000136a0: 2d72 656d 6f76 696e 6720 7370 6563 6961  -removing specia
+000136b0: 6c20 6469 6d65 6e73 696f 6e73 2e22 290a  l dimensions.").
+000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136d0: 696d 6167 652e 7265 6d6f 7665 5f73 7065  image.remove_spe
+000136e0: 6369 616c 5f28 290a 2020 2020 2020 2020  cial_().        
+000136f0: 2020 2020 696d 6167 652e 756e 7371 7565      image.unsque
+00013700: 657a 655f 285b 5d29 2e75 6e73 7175 6565  eze_([]).unsquee
+00013710: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
+00013720: 656c 6966 2069 6d61 6765 2e6e 5f64 696d  elif image.n_dim
+00013730: 203d 3d20 6e5f 6469 6d20 2b20 313a 0a20   == n_dim + 1:. 
+00013740: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00013750: 7420 696d 6167 652e 6861 735f 6261 7463  t image.has_batc
+00013760: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00013770: 2020 2069 6620 696d 6167 652e 6861 735f     if image.has_
+00013780: 6368 616e 6e65 6c3a 2069 6d61 6765 2e75  channel: image.u
+00013790: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
+000137a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000137b0: 7365 3a20 696d 6167 652e 7769 7468 5f62  se: image.with_b
+000137c0: 6174 6368 6469 6d28 3029 2e75 6e73 7175  atchdim(0).unsqu
+000137d0: 6565 7a65 5f28 7b31 7d29 0a20 2020 2020  eeze_({1}).     
+000137e0: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
+000137f0: 696d 6167 652e 6861 735f 6368 616e 6e65  image.has_channe
+00013800: 6c3a 2069 6d61 6765 2e75 6e73 7175 6565  l: image.unsquee
+00013810: 7a65 5f28 7b7d 290a 2020 2020 2020 2020  ze_({}).        
+00013820: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00013830: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00013840: 6622 5761 726e 696e 673a 2027 696e 7465  f"Warning: 'inte
+00013850: 7270 6f6c 6174 696f 6e27 2074 7279 696e  rpolation' tryin
+00013860: 6720 746f 2074 7261 6e73 666f 726d 207b  g to transform {
+00013870: 696d 6167 652e 6e5f 7370 6163 657d 2b7b  image.n_space}+{
+00013880: 696d 6167 652e 6e5f 7370 6563 6961 6c7d  image.n_special}
+00013890: 4420 696d 6167 6520 2877 6974 6820 6261  D image (with ba
+000138a0: 7463 6820 6f72 2063 6861 6e6e 656c 2920  tch or channel) 
+000138b0: 6279 207b 6e5f 6469 6d7d 4420 7472 616e  by {n_dim}D tran
+000138c0: 7366 6f72 6d61 7469 6f6e 2c20 6175 746f  sformation, auto
+000138d0: 2d72 656d 6f76 696e 6720 7468 6520 6368  -removing the ch
+000138e0: 616e 6e65 6c20 6469 6d65 6e73 696f 6e73  annel dimensions
+000138f0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00013900: 2020 2020 696d 6167 652e 7769 7468 5f63      image.with_c
+00013910: 6861 6e6e 656c 6469 6d28 4e6f 6e65 292e  hanneldim(None).
+00013920: 756e 7371 7565 657a 655f 287b 7d29 0a20  unsqueeze_({}). 
+00013930: 2020 2020 2020 2065 6c69 6620 696d 6167         elif imag
+00013940: 652e 6e5f 6469 6d20 3d3d 206e 5f64 696d  e.n_dim == n_dim
+00013950: 202b 2032 3a0a 2020 2020 2020 2020 2020   + 2:.          
+00013960: 2020 2320 5f63 6861 6e6e 616c 2f62 6174    # _channal/bat
+00013970: 6368 2064 696d 656e 7369 6f6e 7320 7573  ch dimensions us
+00013980: 6564 2068 6572 6520 6173 2074 6865 7920  ed here as they 
+00013990: 6172 6520 6e5f 6469 6d20 7768 656e 206e  are n_dim when n
+000139a0: 6f74 2065 7869 7374 6564 2e20 0a20 2020  ot existed. .   
+000139b0: 2020 2020 2020 2020 2069 6620 696d 6167           if imag
+000139c0: 652e 6e5f 7370 6563 6961 6c20 3d3d 2031  e.n_special == 1
+000139d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000139e0: 2020 7072 696e 7428 6622 5761 726e 696e    print(f"Warnin
+000139f0: 673a 2027 696e 7465 7270 6f6c 6174 696f  g: 'interpolatio
+00013a00: 6e27 2074 7279 696e 6720 746f 2074 7261  n' trying to tra
+00013a10: 6e73 666f 726d 207b 696d 6167 652e 6e5f  nsform {image.n_
+00013a20: 7370 6163 657d 2b31 4420 696d 6167 6520  space}+1D image 
+00013a30: 2877 6974 6820 6261 7463 6820 6f72 2063  (with batch or c
+00013a40: 6861 6e6e 656c 2920 6279 207b 6e5f 6469  hannel) by {n_di
+00013a50: 6d7d 4420 7472 616e 7366 6f72 6d61 7469  m}D transformati
+00013a60: 6f6e 2c20 6175 746f 2d69 6e73 6572 7469  on, auto-inserti
+00013a70: 6e67 206e 6577 2073 7065 6369 616c 2064  ng new special d
+00013a80: 696d 656e 7369 6f6e 2e22 290a 2020 2020  imension.").    
+00013a90: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00013aa0: 6d61 6765 2e68 6173 5f62 6174 6368 3a20  mage.has_batch: 
+00013ab0: 696d 6167 652e 6261 7463 685f 6469 6d65  image.batch_dime
+00013ac0: 6e73 696f 6e20 3d20 3020 6966 2069 6d61  nsion = 0 if ima
+00013ad0: 6765 2e5f 6368 616e 6e65 6c5f 6469 6d65  ge._channel_dime
+00013ae0: 6e73 696f 6e20 3e20 3020 656c 7365 2031  nsion > 0 else 1
+00013af0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013b00: 6e6f 7420 696d 6167 652e 6861 735f 6368  not image.has_ch
+00013b10: 616e 6e65 6c3a 2069 6d61 6765 2e63 6861  annel: image.cha
+00013b20: 6e6e 656c 5f64 696d 656e 7369 6f6e 203d  nnel_dimension =
+00013b30: 2030 2069 6620 696d 6167 652e 5f62 6174   0 if image._bat
+00013b40: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
+00013b50: 2065 6c73 6520 310a 2020 2020 6176 6f75   else 1.    avou
+00013b60: 6368 2869 6d61 6765 2e68 6173 5f62 6174  ch(image.has_bat
+00013b70: 6368 2061 6e64 2069 6d61 6765 2e68 6173  ch and image.has
+00013b80: 5f63 6861 6e6e 656c 2c20 2250 6c65 6173  _channel, "Pleas
+00013b90: 6520 7573 6520 6261 746f 7263 6820 7465  e use batorch te
+00013ba0: 6e73 6f72 206f 6620 7369 7a65 2022 202b  nsor of size " +
+00013bb0: 0a20 2020 2020 2020 2020 2020 2022 285b  .            "([
+00013bc0: 6e5f 6261 7463 685d 2c20 7b6e 5f63 6861  n_batch], {n_cha
+00013bd0: 6e6e 656c 2f6e 5f66 6561 7475 7265 3a6f  nnel/n_feature:o
+00013be0: 7074 696f 6e61 6c7d 2c20 6d5f 312c 206d  ptional}, m_1, m
+00013bf0: 5f32 2c20 2e2e 2e2c 206d 5f72 2920 5b72  _2, ..., m_r) [r
+00013c00: 3d6e 5f64 696d 5d20 666f 7220 2220 2b20  =n_dim] for " + 
+00013c10: 0a20 2020 2020 2020 2020 2020 2066 2264  .            f"d
+00013c20: 6174 6120 746f 2062 6520 7370 6174 6961  ata to be spatia
+00013c30: 6c6c 7920 696e 7465 7270 6f6c 6174 6564  lly interpolated
+00013c40: 2c20 696e 7374 6561 6420 6f66 207b 696d  , instead of {im
+00013c50: 6167 652e 7368 6170 657d 2e20 2229 0a20  age.shape}. "). 
+00013c60: 2020 2069 6620 7472 616e 7320 6973 206e     if trans is n
+00013c70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00013c80: 2061 766f 7563 6828 696d 6167 652e 6e5f   avouch(image.n_
+00013c90: 6261 7463 6820 3d3d 2031 206f 7220 7472  batch == 1 or tr
+00013ca0: 616e 732e 6e5f 6261 7463 6820 696e 2028  ans.n_batch in (
+00013cb0: 4e6f 6e65 2c20 696d 6167 652e 6e5f 6261  None, image.n_ba
+00013cc0: 7463 682c 2031 292c 2022 506c 6561 7365  tch, 1), "Please
+00013cd0: 2075 7365 2074 7261 6e73 666f 726d 6174   use transformat
+00013ce0: 696f 6e20 6f66 2061 2022 202b 0a20 2020  ion of a " +.   
+00013cf0: 2020 2020 2020 2020 2066 2273 7569 7461           f"suita
+00013d00: 626c 6520 6e5f 6261 7463 6820 746f 2074  ble n_batch to t
+00013d10: 7261 6e73 666f 726d 2069 6d61 6765 2077  ransform image w
+00013d20: 6974 6820 6261 7463 6873 697a 6520 7b69  ith batchsize {i
+00013d30: 6d61 6765 2e6e 5f62 6174 6368 7d2c 2063  mage.n_batch}, c
+00013d40: 7572 7265 6e74 6c79 207b 7472 616e 732e  urrently {trans.
+00013d50: 6e5f 6261 7463 687d 2e22 290a 0a20 2020  n_batch}.")..   
+00013d60: 206e 5f62 6174 6368 203d 2069 6d61 6765   n_batch = image
+00013d70: 2e6e 5f62 6174 6368 0a20 2020 2069 6620  .n_batch.    if 
+00013d80: 6e5f 6261 7463 6820 3d3d 2031 2061 6e64  n_batch == 1 and
+00013d90: 2074 7261 6e73 2069 7320 6e6f 7420 4e6f   trans is not No
+00013da0: 6e65 2061 6e64 2074 7261 6e73 2e6e 5f62  ne and trans.n_b
+00013db0: 6174 6368 2069 7320 6e6f 7420 4e6f 6e65  atch is not None
+00013dc0: 2061 6e64 2074 7261 6e73 2e6e 5f62 6174   and trans.n_bat
+00013dd0: 6368 203e 2031 3a20 6e5f 6261 7463 6820  ch > 1: n_batch 
+00013de0: 3d20 7472 616e 732e 6e5f 6261 7463 680a  = trans.n_batch.
+00013df0: 2020 2020 6966 206e 5f62 6174 6368 203d      if n_batch =
+00013e00: 3d20 3120 616e 6420 6973 696e 7374 616e  = 1 and isinstan
+00013e10: 6365 2874 6172 6765 745f 7370 6163 652c  ce(target_space,
+00013e20: 2062 742e 5465 6e73 6f72 2920 616e 6420   bt.Tensor) and 
+00013e30: 7461 7267 6574 5f73 7061 6365 2e68 6173  target_space.has
+00013e40: 5f62 6174 6368 2061 6e64 2074 6172 6765  _batch and targe
+00013e50: 745f 7370 6163 652e 6e5f 6261 7463 6820  t_space.n_batch 
+00013e60: 3e20 313a 206e 5f62 6174 6368 203d 2074  > 1: n_batch = t
+00013e70: 6172 6765 745f 7370 6163 652e 6e5f 6261  arget_space.n_ba
+00013e80: 7463 680a 2020 2020 6966 2069 6d61 6765  tch.    if image
+00013e90: 2e6e 5f62 6174 6368 203d 3d20 313a 2069  .n_batch == 1: i
+00013ea0: 6d61 6765 203d 2069 6d61 6765 2e72 6570  mage = image.rep
+00013eb0: 6561 7465 6428 6e5f 6261 7463 682c 205b  eated(n_batch, [
+00013ec0: 5d29 0a20 2020 206e 5f66 6561 7475 7265  ]).    n_feature
+00013ed0: 203d 2069 6d61 6765 2e6e 5f63 6861 6e6e   = image.n_chann
+00013ee0: 656c 0a20 2020 2073 697a 6520 3d20 6274  el.    size = bt
+00013ef0: 2e63 6861 6e6e 656c 5f74 656e 736f 7228  .channel_tensor(
+00013f00: 696d 6167 652e 7370 6163 6529 2e69 6e74  image.space).int
+00013f10: 2829 0a20 2020 2069 6620 6e5f 6261 7463  ().    if n_batc
+00013f20: 6820 3e20 3120 616e 6420 6e6f 7420 7368  h > 1 and not sh
+00013f30: 6170 655f 6f75 742e 6861 735f 6261 7463  ape_out.has_batc
+00013f40: 683a 2073 6861 7065 5f6f 7574 203d 2062  h: shape_out = b
+00013f50: 742e 5369 7a65 285b 6e5f 6261 7463 685d  t.Size([n_batch]
+00013f60: 2920 2b20 7368 6170 655f 6f75 740a 2020  ) + shape_out.  
+00013f70: 2020 6966 2074 6172 6765 745f 7370 6163    if target_spac
+00013f80: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00013f90: 2020 2073 6361 6c65 2c20 2a70 6169 7273     scale, *pairs
+00013fa0: 203d 2074 7261 6e73 2e72 6573 6861 7065   = trans.reshape
+00013fb0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00013fc0: 7363 616c 6529 203d 3d20 313a 2073 6361  scale) == 1: sca
+00013fd0: 6c65 202a 3d20 6e5f 6469 6d0a 2020 2020  le *= n_dim.    
+00013fe0: 2020 2020 7461 7267 6574 5f73 7061 6365      target_space
+00013ff0: 203d 205b 696e 7428 7820 2a20 7929 2066   = [int(x * y) f
+00014000: 6f72 2078 2c20 7920 696e 207a 6970 2869  or x, y in zip(i
+00014010: 6d61 6765 2e73 7061 6365 2c20 7363 616c  mage.space, scal
+00014020: 6529 5d0a 2020 2020 2020 2020 666f 7220  e)].        for 
+00014030: 702c 2071 2069 6e20 7061 6972 733a 2074  p, q in pairs: t
+00014040: 6172 6765 745f 7370 6163 655b 705d 2c20  arget_space[p], 
+00014050: 7461 7267 6574 5f73 7061 6365 5b71 5d20  target_space[q] 
+00014060: 3d20 7461 7267 6574 5f73 7061 6365 5b71  = target_space[q
+00014070: 5d2c 2074 6172 6765 745f 7370 6163 655b  ], target_space[
+00014080: 705d 0a20 2020 2020 2020 2074 6172 6765  p].        targe
+00014090: 745f 7370 6163 6520 3d20 7475 706c 6528  t_space = tuple(
+000140a0: 7461 7267 6574 5f73 7061 6365 290a 2020  target_space).  
+000140b0: 2020 2020 2020 7368 6170 655f 6f75 7420        shape_out 
+000140c0: 3d20 7368 6170 655f 6f75 742e 7265 7365  = shape_out.rese
+000140d0: 745f 7370 6163 6528 7461 7267 6574 5f73  t_space(target_s
+000140e0: 7061 6365 290a 2020 2020 6966 2069 7369  pace).    if isi
+000140f0: 6e73 7461 6e63 6528 7461 7267 6574 5f73  nstance(target_s
+00014100: 7061 6365 2c20 7475 706c 6529 2061 6e64  pace, tuple) and
+00014110: 206c 656e 2874 6172 6765 745f 7370 6163   len(target_spac
+00014120: 6529 203d 3d20 6e5f 6469 6d3a 2070 6173  e) == n_dim: pas
+00014130: 730a 2020 2020 656c 6966 2069 7369 6e73  s.    elif isins
+00014140: 7461 6e63 6528 7461 7267 6574 5f73 7061  tance(target_spa
+00014150: 6365 2c20 6274 2e74 6f72 6368 2e54 656e  ce, bt.torch.Ten
+00014160: 736f 7229 3a20 7061 7373 0a20 2020 2065  sor): pass.    e
+00014170: 6c73 653a 2072 6169 7365 2054 7970 6545  lse: raise TypeE
+00014180: 7272 6f72 2866 2257 726f 6e67 2074 6172  rror(f"Wrong tar
+00014190: 6765 7420 7370 6163 6520 666f 7220 696e  get space for in
+000141a0: 7465 7270 6f6c 6174 696f 6e3a 207b 7461  terpolation: {ta
+000141b0: 7267 6574 5f73 7061 6365 7d2e 2022 290a  rget_space}. ").
+000141c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000141d0: 6528 7461 7267 6574 5f73 7061 6365 2c20  e(target_space, 
+000141e0: 7475 706c 6529 3a20 0a20 2020 2020 2020  tuple): .       
+000141f0: 2023 2043 7265 6174 6520 6120 6772 6964   # Create a grid
+00014200: 2058 2077 6974 6820 7369 7a65 2028 7b6e   X with size ({n
+00014210: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
+00014220: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
+00014230: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
+00014240: 2020 2020 2020 2058 203d 2062 742e 696d         X = bt.im
+00014250: 6167 655f 6772 6964 2874 6172 6765 745f  age_grid(target_
+00014260: 7370 6163 6529 2e66 6c6f 6174 2829 2023  space).float() #
+00014270: 202b 2062 742e 6368 616e 6e65 6c5f 7465   + bt.channel_te
+00014280: 6e73 6f72 285b 666c 6f61 7428 612d 6229  nsor([float(a-b)
+00014290: 2f32 2066 6f72 2061 2c20 6220 696e 207a  /2 for a, b in z
+000142a0: 6970 2869 6d61 6765 2e73 7061 6365 2c20  ip(image.space, 
+000142b0: 7461 7267 6574 5f73 7061 6365 295d 290a  target_space)]).
+000142c0: 2020 2020 2020 2020 2320 436f 6d70 7574          # Comput
+000142d0: 6520 7468 6520 7472 616e 7366 6f72 6d65  e the transforme
+000142e0: 6420 636f 6f72 6469 6e61 7465 732e 2059  d coordinates. Y
+000142f0: 3a20 285b 6e5f 6261 7463 685d 2c20 7b6e  : ([n_batch], {n
+00014300: 5f64 696d 7d2c 2073 697a 655f 312c 2073  _dim}, size_1, s
+00014310: 697a 655f 322c 202e 2e2e 2c20 7369 7a65  ize_2, ..., size
+00014320: 5f72 2920 5b72 3d6e 5f64 696d 5d2e 0a20  _r) [r=n_dim].. 
+00014330: 2020 2020 2020 2069 6620 7472 616e 7320         if trans 
+00014340: 6973 204e 6f6e 653a 2074 7261 6e73 203d  is None: trans =
+00014350: 2049 6465 6e74 6974 7928 290a 2020 2020   Identity().    
+00014360: 2020 2020 5920 3d20 7472 616e 7328 5829      Y = trans(X)
+00014370: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00014380: 592e 6861 735f 6261 7463 683a 2059 203d  Y.has_batch: Y =
+00014390: 2059 2e6d 756c 7469 706c 7928 6e5f 6261   Y.multiply(n_ba
+000143a0: 7463 682c 205b 5d29 0a20 2020 2020 2020  tch, []).       
+000143b0: 2069 6620 592e 6e5f 6261 7463 6820 3d3d   if Y.n_batch ==
+000143c0: 2031 3a20 5920 3d20 592e 7265 7065 6174   1: Y = Y.repeat
+000143d0: 6564 286e 5f62 6174 6368 2c20 5b5d 290a  ed(n_batch, []).
+000143e0: 2020 2020 2020 2020 5920 3d20 592e 616d          Y = Y.am
+000143f0: 706c 6966 7928 6e5f 6665 6174 7572 652c  plify(n_feature,
+00014400: 205b 5d29 0a20 2020 2020 2020 2073 6861   []).        sha
+00014410: 7065 5f6f 7574 203d 2073 6861 7065 5f6f  pe_out = shape_o
+00014420: 7574 2e72 6573 6574 5f73 7061 6365 2874  ut.reset_space(t
+00014430: 6172 6765 745f 7370 6163 6529 0a20 2020  arget_space).   
+00014440: 2065 6c73 653a 0a20 2020 2020 2020 2074   else:.        t
+00014450: 6172 6765 745f 7370 6163 6520 3d20 6261  arget_space = ba
+00014460: 746f 7263 685f 7465 6e73 6f72 2874 6172  torch_tensor(tar
+00014470: 6765 745f 7370 6163 6529 0a20 2020 2020  get_space).     
+00014480: 2020 2069 6620 6e6f 7420 7461 7267 6574     if not target
+00014490: 5f73 7061 6365 2e68 6173 5f62 6174 6368  _space.has_batch
+000144a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000144b0: 2074 6172 6765 745f 7370 6163 652e 7369   target_space.si
+000144c0: 7a65 2830 2920 3d3d 206e 5f62 6174 6368  ze(0) == n_batch
+000144d0: 2061 6e64 206e 5f62 6174 6368 2021 3d20   and n_batch != 
+000144e0: 6e5f 6469 6d20 6f72 206c 656e 285b 7820  n_dim or len([x 
+000144f0: 666f 7220 7820 696e 2074 6172 6765 745f  for x in target_
+00014500: 7370 6163 652e 7368 6170 6520 6966 2078  space.shape if x
+00014510: 203d 3d20 6e5f 6469 6d5d 2920 3e3d 2032   == n_dim]) >= 2
+00014520: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014530: 2020 7461 7267 6574 5f73 7061 6365 2e77    target_space.w
+00014540: 6974 685f 6261 7463 6864 696d 2830 290a  ith_batchdim(0).
+00014550: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00014560: 3a20 7461 7267 6574 5f73 7061 6365 2e75  : target_space.u
+00014570: 6e73 7175 6565 7a65 5f28 5b5d 290a 2020  nsqueeze_([]).  
+00014580: 2020 2020 2020 6966 206e 6f74 2074 6172        if not tar
+00014590: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
+000145a0: 616e 6e65 6c3a 0a20 2020 2020 2020 2020  annel:.         
+000145b0: 2020 2069 6620 7461 7267 6574 5f73 7061     if target_spa
+000145c0: 6365 2e62 6174 6368 5f64 696d 656e 7369  ce.batch_dimensi
+000145d0: 6f6e 2021 3d20 3020 616e 6420 7461 7267  on != 0 and targ
+000145e0: 6574 5f73 7061 6365 2e73 697a 6528 3029  et_space.size(0)
+000145f0: 203d 3d20 6e5f 6469 6d3a 2074 6172 6765   == n_dim: targe
+00014600: 745f 7370 6163 652e 7769 7468 5f63 6861  t_space.with_cha
+00014610: 6e6e 656c 6469 6d28 3029 0a20 2020 2020  nneldim(0).     
+00014620: 2020 2020 2020 2065 6c69 6620 7461 7267         elif targ
+00014630: 6574 5f73 7061 6365 2e62 6174 6368 5f64  et_space.batch_d
+00014640: 696d 656e 7369 6f6e 2021 3d20 3120 616e  imension != 1 an
+00014650: 6420 7461 7267 6574 5f73 7061 6365 2e73  d target_space.s
+00014660: 697a 6528 3129 203d 3d20 6e5f 6469 6d3a  ize(1) == n_dim:
+00014670: 2074 6172 6765 745f 7370 6163 652e 7769   target_space.wi
+00014680: 7468 5f63 6861 6e6e 656c 6469 6d28 3129  th_channeldim(1)
+00014690: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000146a0: 6620 7461 7267 6574 5f73 7061 6365 2e62  f target_space.b
+000146b0: 6174 6368 5f64 696d 656e 7369 6f6e 2021  atch_dimension !
+000146c0: 3d20 7461 7267 6574 5f73 7061 6365 2e6e  = target_space.n
+000146d0: 5f64 696d 202d 2031 2061 6e64 2074 6172  _dim - 1 and tar
+000146e0: 6765 745f 7370 6163 652e 7369 7a65 282d  get_space.size(-
+000146f0: 3129 203d 3d20 6e5f 6469 6d3a 2074 6172  1) == n_dim: tar
+00014700: 6765 745f 7370 6163 652e 7769 7468 5f63  get_space.with_c
+00014710: 6861 6e6e 656c 6469 6d28 2d31 290a 2020  hanneldim(-1).  
+00014720: 2020 2020 2020 6176 6f75 6368 2874 6172        avouch(tar
+00014730: 6765 745f 7370 6163 652e 6861 735f 6368  get_space.has_ch
+00014740: 616e 6e65 6c20 616e 6420 7461 7267 6574  annel and target
+00014750: 5f73 7061 6365 2e6e 5f63 6861 6e6e 656c  _space.n_channel
+00014760: 203d 3d20 6e5f 6469 6d2c 2022 2774 6172   == n_dim, "'tar
+00014770: 6765 745f 7370 6163 6527 2066 6f72 2069  get_space' for i
+00014780: 6e74 6572 706f 6c61 7469 6f6e 2073 686f  nterpolation sho
+00014790: 756c 6420 6861 7665 2061 2063 6861 6e6e  uld have a chann
+000147a0: 656c 2064 696d 656e 7369 6f6e 2066 6f72  el dimension for
+000147b0: 2063 6f6f 7264 696e 6174 6573 2e20 2229   coordinates. ")
+000147c0: 0a20 2020 2020 2020 2059 203d 2074 6172  .        Y = tar
+000147d0: 6765 745f 7370 6163 652e 7265 7065 6174  get_space.repeat
+000147e0: 6564 286e 5f62 6174 6368 202f 2f20 7461  ed(n_batch // ta
+000147f0: 7267 6574 5f73 7061 6365 2e6e 5f62 6174  rget_space.n_bat
+00014800: 6368 2c20 5b5d 292e 616d 706c 6966 7928  ch, []).amplify(
+00014810: 6e5f 6665 6174 7572 652c 205b 5d29 0a20  n_feature, []). 
+00014820: 2020 2020 2020 2073 6861 7065 5f6f 7574         shape_out
+00014830: 203d 2073 6861 7065 5f6f 7574 2e72 6573   = shape_out.res
+00014840: 6574 5f73 7061 6365 2874 6172 6765 745f  et_space(target_
+00014850: 7370 6163 652e 7370 6163 6529 0a20 2020  space.space).   
+00014860: 2020 2020 200a 2020 2020 696d 6167 6520       .    image 
+00014870: 3d20 696d 6167 652e 6d65 7267 6564 696d  = image.mergedim
+00014880: 7328 7b7d 2c20 5b5d 290a 2020 2020 6e5f  s({}, []).    n_
+00014890: 6261 7463 6820 3d20 696d 6167 652e 6e5f  batch = image.n_
+000148a0: 6261 7463 680a 0a20 2020 2069 6620 6d65  batch..    if me
+000148b0: 7468 6f64 2e6c 6f77 6572 2829 203d 3d20  thod.lower() == 
+000148c0: 2762 7370 6c69 6e65 273a 0a20 2020 2020  'bspline':.     
+000148d0: 2020 2069 6620 6465 7269 7661 7469 7665     if derivative
+000148e0: 3a20 7261 6973 6520 5479 7065 4572 726f  : raise TypeErro
+000148f0: 7228 224e 6f20 6465 7269 7661 7469 7665  r("No derivative
+00014900: 7320 666f 7220 6273 706c 696e 6520 696e  s for bspline in
+00014910: 7465 7270 6f6c 6174 696f 6e73 2061 7265  terpolations are
+00014920: 2061 7661 696c 6162 6c65 2073 6f20 6661   available so fa
+00014930: 722e 2050 6c65 6173 6520 7772 6974 6520  r. Please write 
+00014940: 6974 2062 7920 796f 7572 7365 6c66 2e20  it by yourself. 
+00014950: 2229 0a20 2020 2020 2020 2023 2054 4f44  ").        # TOD
+00014960: 4f3a 2046 4644 0a20 2020 2020 2020 2072  O: FFD.        r
+00014970: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+00014980: 4273 706c 696e 6520 696e 7465 7270 6f6c  Bspline interpol
+00014990: 6174 696f 6e20 6973 206e 6f74 2061 7661  ation is not ava
+000149a0: 696c 6162 6c65 2073 6f20 6661 722e 2050  ilable so far. P
+000149b0: 6c65 6173 6520 7772 6974 6520 6974 2062  lease write it b
+000149c0: 7920 796f 7572 7365 6c66 2e20 2229 0a0a  y yourself. ")..
+000149d0: 2020 2020 6959 203d 2062 742e 666c 6f6f      iY = bt.floo
+000149e0: 7228 5929 2e6c 6f6e 6728 2920 2320 4765  r(Y).long() # Ge
+000149f0: 6e65 7261 7465 2074 6865 2069 6e74 6567  nerate the integ
+00014a00: 6572 2070 6172 7420 6f66 2059 0a20 2020  er part of Y.   
+00014a10: 206a 5920 3d20 6959 202b 2031 2023 2061   jY = iY + 1 # a
+00014a20: 6e64 2074 6865 2069 6e74 6567 6572 2070  nd the integer p
+00014a30: 6172 7420 706c 7573 206f 6e65 2e0a 2020  art plus one..  
+00014a40: 2020 6966 206d 6574 686f 642e 6c6f 7765    if method.lowe
+00014a50: 7228 2920 3d3d 2027 6c69 6e65 6172 273a  r() == 'linear':
+00014a60: 2066 5920 3d20 5920 2d20 6959 2e66 6c6f   fY = Y - iY.flo
+00014a70: 6174 2829 2023 2054 6865 2064 6563 696d  at() # The decim
+00014a80: 616c 2070 6172 7420 6f66 2059 2e0a 2020  al part of Y..  
+00014a90: 2020 656c 6966 206d 6574 686f 642e 6c6f    elif method.lo
+00014aa0: 7765 7228 2920 3d3d 2027 6e65 6172 6573  wer() == 'neares
+00014ab0: 7427 3a20 6659 203d 2062 742e 666c 6f6f  t': fY = bt.floo
+00014ac0: 7228 5920 2d20 6959 2e66 6c6f 6174 2829  r(Y - iY.float()
+00014ad0: 202b 2030 2e35 2920 2320 5468 6520 6465   + 0.5) # The de
+00014ae0: 6369 6d61 6c20 7061 7274 206f 6620 592e  cimal part of Y.
+00014af0: 0a20 2020 2065 6c73 653a 2072 6169 7365  .    else: raise
+00014b00: 2054 7970 6545 7272 6f72 2822 556e 7265   TypeError("Unre
+00014b10: 636f 676e 697a 6564 2061 7267 756d 656e  cognized argumen
+00014b20: 7420 276d 6574 686f 6427 2e20 2229 0a20  t 'method'. "). 
+00014b30: 2020 2062 5920 3d20 6274 2e73 7461 636b     bY = bt.stack
+00014b40: 2828 6959 2c20 6a59 292c 2031 292e 7669  ((iY, jY), 1).vi
+00014b50: 6577 285b 6e5f 6261 7463 685d 2c20 322c  ew([n_batch], 2,
+00014b60: 207b 6e5f 6469 6d7d 2c20 2d31 2920 2320   {n_dim}, -1) # 
+00014b70: 285b 6e5f 6261 7463 685d 2c20 322c 207b  ([n_batch], 2, {
+00014b80: 6e5f 6469 6d7d 2c20 6e5f 6461 7461 292e  n_dim}, n_data).
+00014b90: 0a20 2020 2057 203d 2062 742e 7374 6163  .    W = bt.stac
+00014ba0: 6b28 2831 202d 2066 592c 2066 5929 2c20  k((1 - fY, fY), 
+00014bb0: 3129 2e76 6965 7728 5b6e 5f62 6174 6368  1).view([n_batch
+00014bc0: 5d2c 2032 2c20 7b6e 5f64 696d 7d2c 202d  ], 2, {n_dim}, -
+00014bd0: 3129 2023 2028 5b6e 5f62 6174 6368 5d2c  1) # ([n_batch],
+00014be0: 2032 2c20 7b6e 5f64 696d 7d2c 206e 5f64   2, {n_dim}, n_d
+00014bf0: 6174 6129 2e0a 2020 2020 6e5f 6461 7461  ata)..    n_data
+00014c00: 203d 2062 592e 7369 7a65 282d 3129 0a0a   = bY.size(-1)..
+00014c10: 2020 2020 2320 5072 6570 6172 6520 666f      # Prepare fo
+00014c20: 7220 7468 6520 6f75 7470 7574 2073 7061  r the output spa
+00014c30: 6365 3a20 6e5f 6261 7463 682c 206d 5f31  ce: n_batch, m_1
+00014c40: 2c20 2e2e 2e2c 206d 5f73 0a20 2020 2069  , ..., m_s.    i
+00014c50: 6620 6465 7269 7661 7469 7665 3a20 6f75  f derivative: ou
+00014c60: 7470 7574 203d 2062 742e 7a65 726f 7328  tput = bt.zeros(
+00014c70: 5b6e 5f62 6174 6368 5d2c 207b 6e5f 6469  [n_batch], {n_di
+00014c80: 6d7d 2c20 2a73 6861 7065 5f6f 7574 2e73  m}, *shape_out.s
+00014c90: 7061 6365 290a 2020 2020 656c 7365 3a20  pace).    else: 
+00014ca0: 6f75 7470 7574 203d 2062 742e 7a65 726f  output = bt.zero
+00014cb0: 7328 7368 6170 655f 6f75 7429 0a20 2020  s(shape_out).   
+00014cc0: 2066 6f72 2047 2069 6e20 6274 2e69 6d61   for G in bt.ima
+00014cd0: 6765 5f67 7269 6428 5b32 5d2a 6e5f 6469  ge_grid([2]*n_di
+00014ce0: 6d29 2e66 6c61 7474 656e 2829 2e74 7261  m).flatten().tra
+00014cf0: 6e73 706f 7365 2830 2c20 3129 3a0a 2020  nspose(0, 1):.  
+00014d00: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00014d10: 696e 6469 6365 7320 666f 7220 7468 6520  indices for the 
+00014d20: 7465 726d 3a20 6259 5b3a 2c20 475b 445d  term: bY[:, G[D]
+00014d30: 2c20 442c 203a 5d2c 2073 697a 653d 285b  , D, :], size=([
+00014d40: 6e5f 6261 7463 685d 2c20 7b6e 5f64 696d  n_batch], {n_dim
+00014d50: 7d2c 206e 5f64 6174 6129 0a20 2020 2020  }, n_data).     
+00014d60: 2020 2049 6e64 203d 2062 592e 6761 7468     Ind = bY.gath
+00014d70: 6572 2831 2c20 472e 6578 7061 6e64 5f74  er(1, G.expand_t
+00014d80: 6f28 5b6e 5f62 6174 6368 5d2c 2031 2c20  o([n_batch], 1, 
+00014d90: 7b6e 5f64 696d 7d2c 206e 5f64 6174 6129  {n_dim}, n_data)
+00014da0: 292e 7371 7565 657a 6528 3129 0a20 2020  ).squeeze(1).   
+00014db0: 2020 2020 2023 2043 6c61 6d70 2074 6865       # Clamp the
+00014dc0: 2069 6e64 6963 6573 2069 6e20 7468 6520   indices in the 
+00014dd0: 636f 7272 6563 7420 7261 6e67 6520 2620  correct range & 
+00014de0: 436f 6d70 7574 6520 7468 6520 626f 7264  Compute the bord
+00014df0: 6572 2063 6f6e 6469 7469 6f6e 0a20 2020  er condition.   
+00014e00: 2020 2020 2063 6f6e 6469 7469 6f6e 203d       condition =
+00014e10: 2062 742e 7375 6d28 2849 6e64 203c 2030   bt.sum((Ind < 0
+00014e20: 2920 2b20 2849 6e64 203e 2073 697a 6520  ) + (Ind > size 
+00014e30: 2d20 3129 2c20 3129 0a20 2020 2020 2020  - 1), 1).       
+00014e40: 2049 6e64 203d 2062 742e 6d69 6e28 6274   Ind = bt.min(bt
+00014e50: 2e63 6c61 6d70 2849 6e64 2c20 6d69 6e3d  .clamp(Ind, min=
+00014e60: 3029 2c20 2873 697a 6520 2d20 3129 2e65  0), (size - 1).e
+00014e70: 7870 616e 645f 746f 2849 6e64 2929 0a20  xpand_to(Ind)). 
+00014e80: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+00014e90: 2074 6865 2069 6e64 6963 6573 2074 6f20   the indices to 
+00014ea0: 3120 6469 6d65 6e73 696f 6e61 6c2e 2044  1 dimensional. D
+00014eb0: 6f74 3a20 285b 6e5f 6261 7463 685d 2c20  ot: ([n_batch], 
+00014ec0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00014ed0: 446f 7420 3d20 496e 645b 3a2c 2030 5d0a  Dot = Ind[:, 0].
+00014ee0: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+00014ef0: 2072 616e 6765 2831 2c20 6e5f 6469 6d29   range(1, n_dim)
+00014f00: 3a20 446f 7420 2a3d 2073 697a 655b 725d  : Dot *= size[r]
+00014f10: 3b20 446f 7420 2b3d 2049 6e64 5b3a 2c20  ; Dot += Ind[:, 
+00014f20: 725d 0a20 2020 2020 2020 2023 2047 6574  r].        # Get
+00014f30: 2074 6865 2069 6d61 6765 2076 616c 7565   the image value
+00014f40: 7320 4956 3a20 285b 6e5f 6261 7463 685d  s IV: ([n_batch]
+00014f50: 2c20 6e5f 6461 7461 290a 2020 2020 2020  , n_data).      
+00014f60: 2020 4956 203d 204e 6f6e 650a 2020 2020    IV = None.    
+00014f70: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00014f80: 6528 6669 6c6c 2c20 7374 7229 3a0a 2020  e(fill, str):.  
+00014f90: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+00014fa0: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6e65  l.lower() == 'ne
+00014fb0: 6172 6573 7427 3a0a 2020 2020 2020 2020  arest':.        
+00014fc0: 2020 2020 2020 2020 4956 203d 2069 6d61          IV = ima
+00014fd0: 6765 2e66 6c61 7474 656e 2829 2e67 6174  ge.flatten().gat
+00014fe0: 6865 7228 312c 2044 6f74 290a 2020 2020  her(1, Dot).    
+00014ff0: 2020 2020 2020 2020 656c 6966 2066 696c          elif fil
+00015000: 6c2e 6c6f 7765 7228 2920 3d3d 2027 6261  l.lower() == 'ba
+00015010: 636b 6772 6f75 6e64 273a 0a20 2020 2020  ckground':.     
+00015020: 2020 2020 2020 2020 2020 2062 6b5f 7661             bk_va
+00015030: 6c75 6520 3d20 6274 2e73 7461 636b 285b  lue = bt.stack([
+00015040: 696d 6167 655b 2873 6c69 6365 284e 6f6e  image[(slice(Non
+00015050: 6529 2c29 202b 2074 7570 6c65 2867 295d  e),) + tuple(g)]
+00015060: 2066 6f72 2067 2069 6e20 2862 742e 696d   for g in (bt.im
+00015070: 6167 655f 6772 6964 285b 325d 2a6e 5f64  age_grid([2]*n_d
+00015080: 696d 2920 2a20 6274 2e63 6861 6e6e 656c  im) * bt.channel
+00015090: 5f74 656e 736f 7228 7369 7a65 2d31 2929  _tensor(size-1))
+000150a0: 2e66 6c61 7474 656e 2829 2e74 7261 6e73  .flatten().trans
+000150b0: 706f 7365 2830 2c31 295d 2c20 3129 2e6d  pose(0,1)], 1).m
+000150c0: 6564 6961 6e28 3129 2e76 616c 7565 730a  edian(1).values.
+000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150e0: 6261 636b 6772 6f75 6e64 203d 2062 6b5f  background = bk_
+000150f0: 7661 6c75 6520 2a20 6274 2e6f 6e65 735f  value * bt.ones_
+00015100: 6c69 6b65 2844 6f74 290a 2020 2020 2020  like(Dot).      
+00015110: 2020 2020 2020 656c 6966 2066 696c 6c2e        elif fill.
+00015120: 6c6f 7765 7228 2920 3d3d 2027 7a65 726f  lower() == 'zero
+00015130: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00015140: 2020 2062 6163 6b67 726f 756e 6420 3d20     background = 
+00015150: 6274 2e7a 6572 6f73 5f6c 696b 6528 446f  bt.zeros_like(Do
+00015160: 7429 0a20 2020 2020 2020 2065 6c73 653a  t).        else:
+00015170: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
+00015180: 6b67 726f 756e 6420 3d20 6669 6c6c 202a  kground = fill *
+00015190: 2062 742e 6f6e 6573 5f6c 696b 6528 446f   bt.ones_like(Do
+000151a0: 7429 0a20 2020 2020 2020 2069 6620 4956  t).        if IV
+000151b0: 2069 7320 4e6f 6e65 3a20 4956 203d 2062   is None: IV = b
+000151c0: 742e 7768 6572 6528 636f 6e64 6974 696f  t.where(conditio
+000151d0: 6e20 3e3d 2031 2c20 6261 636b 6772 6f75  n >= 1, backgrou
+000151e0: 6e64 2e66 6c6f 6174 2829 2c20 696d 6167  nd.float(), imag
+000151f0: 652e 666c 6174 7465 6e28 292e 6761 7468  e.flatten().gath
+00015200: 6572 2831 2c20 446f 7429 2e66 6c6f 6174  er(1, Dot).float
+00015210: 2829 290a 2020 2020 2020 2020 2320 5765  ()).        # We
+00015220: 6967 6874 7320 666f 7220 6561 6368 2070  ights for each p
+00015230: 6f69 6e74 3a20 5b70 726f 6475 6374 206f  oint: [product o
+00015240: 6620 575b 3a2c 2047 5b44 5d2c 2044 2c20  f W[:, G[D], D, 
+00015250: 785d 2066 6f72 2044 2069 6e20 7261 6e67  x] for D in rang
+00015260: 6528 6e5f 6469 6d29 5d20 666f 7220 706f  e(n_dim)] for po
+00015270: 696e 7420 782e 0a20 2020 2020 2020 2023  int x..        #
+00015280: 2057 673a 2028 5b6e 5f62 6174 6368 5d2c   Wg: ([n_batch],
+00015290: 207b 6e5f 6469 6d7d 2c20 6e5f 6461 7461   {n_dim}, n_data
+000152a0: 290a 2020 2020 2020 2020 5767 203d 2057  ).        Wg = W
+000152b0: 2e67 6174 6865 7228 312c 2047 2e65 7870  .gather(1, G.exp
+000152c0: 616e 645f 746f 285b 6e5f 6261 7463 685d  and_to([n_batch]
+000152d0: 2c20 312c 207b 6e5f 6469 6d7d 2c20 6e5f  , 1, {n_dim}, n_
+000152e0: 6461 7461 2929 2e73 7175 6565 7a65 2831  data)).squeeze(1
+000152f0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00015300: 2064 6572 6976 6174 6976 653a 0a20 2020   derivative:.   
+00015310: 2020 2020 2020 2020 206f 7574 7075 7420           output 
+00015320: 2b3d 2028 5767 2e70 726f 6428 3129 202a  += (Wg.prod(1) *
+00015330: 2049 5629 2e76 6965 775f 6173 286f 7574   IV).view_as(out
+00015340: 7075 7429 0a20 2020 2020 2020 2065 6c73  put).        els
+00015350: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00015360: 656d 7057 674d 6174 203d 2057 672e 6d75  empWgMat = Wg.mu
+00015370: 6c74 6970 6c79 286e 5f64 696d 2c20 3129  ltiply(n_dim, 1)
+00015380: 2023 2028 5b6e 5f62 6174 6368 5d2c 206e   # ([n_batch], n
+00015390: 5f64 696d 2c20 7b6e 5f64 696d 7d2c 206e  _dim, {n_dim}, n
+000153a0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+000153b0: 2020 2074 656d 7057 674d 6174 5b3a 2c20     tempWgMat[:, 
+000153c0: 6274 2e61 7261 6e67 6528 6e5f 6469 6d29  bt.arange(n_dim)
+000153d0: 2c20 6274 2e61 7261 6e67 6528 6e5f 6469  , bt.arange(n_di
+000153e0: 6d29 5d20 3d20 310a 2020 2020 2020 2020  m)] = 1.        
+000153f0: 2020 2020 6457 6720 3d20 7465 6d70 5767      dWg = tempWg
+00015400: 4d61 742e 7072 6f64 2831 2920 2a20 2847  Mat.prod(1) * (G
+00015410: 202a 2032 202d 2031 292e 666c 6f61 7428   * 2 - 1).float(
+00015420: 290a 2020 2020 2020 2020 2020 2020 6f75  ).            ou
+00015430: 7470 7574 202b 3d20 2864 5767 202a 2049  tput += (dWg * I
+00015440: 562e 756e 7371 7565 657a 6528 3129 292e  V.unsqueeze(1)).
+00015450: 7669 6577 5f61 7328 6f75 7470 7574 290a  view_as(output).
+00015460: 2020 2020 6274 2e74 6f72 6368 2e63 7564      bt.torch.cud
+00015470: 612e 656d 7074 795f 6361 6368 6528 290a  a.empty_cache().
+00015480: 2020 2020 6570 7320 3d20 3165 2d36 0a20      eps = 1e-6. 
+00015490: 2020 206d 203d 2030 2069 6620 696d 6167     m = 0 if imag
+000154a0: 652e 6d69 6e28 2920 3e20 2d65 7073 2065  e.min() > -eps e
+000154b0: 6c73 6520 696d 6167 652e 6d69 6e28 292e  lse image.min().
+000154c0: 6974 656d 2829 0a20 2020 204d 203d 2031  item().    M = 1
+000154d0: 2069 6620 696d 6167 652e 6d61 7828 2920   if image.max() 
+000154e0: 3c20 3120 2b20 6570 7320 656c 7365 2069  < 1 + eps else i
+000154f0: 6d61 6765 2e6d 6178 2829 2e69 7465 6d28  mage.max().item(
+00015500: 290a 2020 2020 7265 7475 726e 206f 7574  ).    return out
+00015510: 7075 742e 636c 616d 7028 6d2c 204d 290a  put.clamp(m, M).
+00015520: 0a40 616c 6961 7328 2272 6573 616d 706c  .@alias("resampl
+00015530: 655f 666f 7277 6172 6422 290a 6465 6620  e_forward").def 
+00015540: 696e 7465 7270 6f6c 6174 696f 6e5f 666f  interpolation_fo
+00015550: 7277 6172 6428 0a20 2020 2020 2020 2069  rward(.        i
+00015560: 6d61 6765 2c20 0a20 2020 2020 2020 2074  mage, .        t
+00015570: 7261 6e73 203d 204e 6f6e 652c 200a 2020  rans = None, .  
+00015580: 2020 2020 2020 6d65 7468 6f64 203d 2027        method = '
+00015590: 4c69 6e65 6172 272c 200a 2020 2020 2020  Linear', .      
+000155a0: 2020 7461 7267 6574 5f73 7061 6365 203d    target_space =
+000155b0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+000155c0: 696c 6c20 3d20 277a 6572 6f27 2c0a 2020  ill = 'zero',.  
+000155d0: 2020 2020 2020 6465 7269 7661 7469 7665        derivative
+000155e0: 203d 2046 616c 7365 0a20 2020 2029 3a0a   = False.    ):.
+000155f0: 2020 2020 2727 270a 2020 2020 496e 7465      '''.    Inte
+00015600: 7270 6f6c 6174 6520 7573 696e 6720 666f  rpolate using fo
+00015610: 7277 6172 6420 7472 616e 7366 6f72 6d61  rward transforma
+00015620: 7469 6f6e 2e20 4974 2069 7320 6e6f 7420  tion. It is not 
+00015630: 7965 7420 696d 706c 656d 656e 7465 642e  yet implemented.
+00015640: 200a 2020 2020 692e 652e 2043 6f6d 7075   .    i.e. Compu
+00015650: 7465 2074 6865 2069 6d61 6765 2049 2073  te the image I s
+00015660: 2e74 2e20 7472 616e 7328 7829 203d 2079  .t. trans(x) = y
+00015670: 2066 6f72 2078 2069 6e20 696e 7075 7420   for x in input 
+00015680: 696d 6167 6520 616e 6420 7920 696e 2074  image and y in t
+00015690: 6865 206f 7574 7075 7420 4920 7573 696e  he output I usin
+000156a0: 6720 696e 7465 7270 6f6c 6174 696f 6e20  g interpolation 
+000156b0: 6d65 7468 6f64 3a0a 2020 2020 2020 2020  method:.        
+000156c0: 6d65 7468 6f64 203d 204c 696e 6561 7220  method = Linear 
+000156d0: 5b4e 4f20 4752 4144 4945 4e54 2121 215d  [NO GRADIENT!!!]
+000156e0: 3a20 4269 6c69 6e65 6172 2069 6e74 6572  : Bilinear inter
+000156f0: 706f 6c61 7469 6f6e 0a20 2020 2020 2020  polation.       
+00015700: 206d 6574 686f 6420 3d20 4e65 6172 6573   method = Neares
+00015710: 7420 5b4e 4f20 4752 4144 4945 4e54 2121  t [NO GRADIENT!!
+00015720: 215d 3a20 4e65 6172 6573 7420 696e 7465  !]: Nearest inte
+00015730: 7270 6f6c 6174 696f 6e0a 0a20 2020 2050  rpolation..    P
+00015740: 6172 616d 733a 0a20 2020 2020 2020 2069  arams:.        i
+00015750: 6d61 6765 205b 6274 2e54 656e 736f 725d  mage [bt.Tensor]
+00015760: 3a20 5468 6520 7461 7267 6574 2069 6d61  : The target ima
+00015770: 6765 2e0a 2020 2020 2020 2020 2020 2020  ge..            
+00015780: 7369 7a65 3a20 285b 6e5f 6261 7463 683a  size: ([n_batch:
+00015790: 6f70 7469 6f6e 616c 5d2c 207b 6e5f 6368  optional], {n_ch
+000157a0: 616e 6e65 6c3a 6f70 7469 6f6e 616c 7d2c  annel:optional},
+000157b0: 206d 4031 2c20 6d40 322c 202e 2e2e 2c20   m@1, m@2, ..., 
+000157c0: 6d40 6e5f 6469 6d29 0a20 2020 2020 2020  m@n_dim).       
+000157d0: 2074 7261 6e73 205b 4675 6e63 7469 6f6e   trans [Function
+000157e0: 206f 7220 6d69 636f 6d70 7574 696e 672e   or micomputing.
+000157f0: 5370 6174 6961 6c54 7261 6e73 666f 726d  SpatialTransform
+00015800: 6174 696f 6e5d 3a20 5472 616e 7366 6f72  ation]: Transfor
+00015810: 6d61 7469 6f6e 2066 756e 6374 696f 6e2c  mation function,
+00015820: 206d 6170 7069 6e67 0a20 2020 2020 2020   mapping.       
+00015830: 2020 2020 2073 697a 653a 2028 5b6e 5f62       size: ([n_b
+00015840: 6174 6368 3a6f 7074 696f 6e61 6c5d 2c20  atch:optional], 
+00015850: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
+00015860: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+00015870: 2074 6f20 285b 6e5f 6261 7463 685d 2c20   to ([n_batch], 
+00015880: 7b6e 5f64 696d 7d2c 206e 4031 2c20 6e40  {n_dim}, n@1, n@
+00015890: 322c 202e 2e2e 2c20 6e40 6e5f 6469 6d29  2, ..., n@n_dim)
+000158a0: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
+000158b0: 5b73 7472 3a20 6c69 6e65 6172 7c6e 6561  [str: linear|nea
+000158c0: 7265 7374 5d3a 2054 6865 2069 6e74 6572  rest]: The inter
+000158d0: 706f 6c61 7469 6f6e 206d 6574 686f 642e  polation method.
+000158e0: 200a 2020 2020 2020 2020 7461 7267 6574   .        target
+000158f0: 5f73 7061 6365 205b 7475 706c 6520 6f72  _space [tuple or
+00015900: 2062 742e 5465 6e73 6f72 5d3a 0a20 2020   bt.Tensor]:.   
+00015910: 2020 2020 2020 2020 2053 697a 6520 2874           Size (t
+00015920: 7570 6c65 2920 6f66 2061 2074 6172 6765  uple) of a targe
+00015930: 7420 524f 4920 6174 2074 6865 2063 656e  t ROI at the cen
+00015940: 7465 7220 6f66 2069 6d61 6765 2e20 0a20  ter of image. . 
+00015950: 2020 2020 2020 2020 2020 204f 5220 5472             OR Tr
+00015960: 616e 7366 6f72 6d65 6420 636f 6f72 6469  ansformed coordi
+00015970: 6e61 7465 2073 7061 6365 2028 6274 2e54  nate space (bt.T
+00015980: 656e 736f 7229 206f 6620 7468 6520 6f75  ensor) of the ou
+00015990: 7470 7574 2069 6d61 6765 2e20 0a20 2020  tput image. .   
+000159a0: 2020 2020 2020 2020 2073 697a 653a 206c           size: l
+000159b0: 656e 6774 6828 6e5f 6469 6d29 206f 7220  ength(n_dim) or 
+000159c0: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+000159d0: 616c 5d2c 207b 6e5f 6469 6d3a 6f70 7469  al], {n_dim:opti
+000159e0: 6f6e 616c 7d2c 2073 697a 6540 312c 2073  onal}, size@1, s
+000159f0: 697a 6540 322c 202e 2e2e 2c20 7369 7a65  ize@2, ..., size
+00015a00: 406e 5f64 696d 290a 2020 2020 2020 2020  @n_dim).        
+00015a10: 6669 6c6c 205b 7374 723a 206e 6561 7265  fill [str: neare
+00015a20: 7374 7c62 6163 6b67 726f 756e 6420 6f72  st|background or
+00015a30: 2069 6e74 206f 7220 666c 6f61 7428 6e75   int or float(nu
+00015a40: 6d62 6572 295d 3a20 496e 6469 6361 7465  mber)]: Indicate
+00015a50: 2074 6865 2077 6179 2074 6f20 6669 6c6c   the way to fill
+00015a60: 2062 6163 6b67 726f 756e 6420 6f75 7473   background outs
+00015a70: 6964 6520 6053 7572 726f 756e 6469 6e67  ide `Surrounding
+00015a80: 602e 200a 2020 2020 2020 2020 6465 7269  `. .        deri
+00015a90: 7661 7469 7665 205b 626f 6f6c 5d3a 2057  vative [bool]: W
+00015aa0: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
+00015ab0: 2074 6865 2067 7261 6469 656e 742e 204f   the gradient. O
+00015ac0: 6e65 2063 616e 206f 6d69 7420 6974 2077  ne can omit it w
+00015ad0: 6865 6e20 7573 696e 6720 746f 7263 682e  hen using torch.
+00015ae0: 6175 746f 6772 6164 2e0a 0a20 2020 2020  autograd...     
+00015af0: 2020 206f 7574 7075 7420 5b62 742e 5465     output [bt.Te
+00015b00: 6e73 6f72 5d3a 2054 6865 2074 7261 6e73  nsor]: The trans
+00015b10: 666f 726d 6564 2069 6d61 6765 2e0a 2020  formed image..  
+00015b20: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00015b30: 285b 6e5f 6261 7463 685d 2c20 7b6e 5f63  ([n_batch], {n_c
+00015b40: 6861 6e6e 656c 3a6f 7074 696f 6e61 6c7d  hannel:optional}
+00015b50: 2c20 6d40 312c 206d 4032 2c20 2e2e 2e2c  , m@1, m@2, ...,
+00015b60: 206d 406e 5f64 696d 290a 2020 2020 2020   m@n_dim).      
+00015b70: 2020 2020 2020 6f72 2077 6865 6e20 6074        or when `t
+00015b80: 6172 6765 745f 7370 6163 6560 2069 7320  arget_space` is 
+00015b90: 6465 6669 6e65 6420 6279 2074 656e 736f  defined by tenso
+00015ba0: 722e 200a 2020 2020 2020 2020 2020 2020  r. .            
+00015bb0: 7369 7a65 3a20 285b 6e5f 6261 7463 685d  size: ([n_batch]
+00015bc0: 2c20 7369 7a65 4031 2c20 7369 7a65 4032  , size@1, size@2
+00015bd0: 2c20 2e2e 2e2c 2073 697a 6540 6e5f 6469  , ..., size@n_di
+00015be0: 6d29 0a20 2020 2020 2020 2020 2020 206f  m).            o
+00015bf0: 7220 7468 6520 6465 7269 7661 7469 7665  r the derivative
+00015c00: 2066 6f72 2074 6865 2069 6e74 6572 706f   for the interpo
+00015c10: 6c61 7469 6f6e 2e20 2869 6620 6064 6572  lation. (if `der
+00015c20: 6976 6174 6976 6520 3d20 5472 7565 6029  ivative = True`)
+00015c30: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00015c40: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
+00015c50: 6e5f 6469 6d7d 2c20 7369 7a65 4031 2c20  n_dim}, size@1, 
+00015c60: 7369 7a65 4032 2c20 2e2e 2e2c 2073 697a  size@2, ..., siz
+00015c70: 6540 6e5f 6469 6d29 0a0a 2020 2020 4578  e@n_dim)..    Ex
+00015c80: 616d 706c 6573 3a0a 2020 2020 2d2d 2d2d  amples:.    ----
+00015c90: 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e 2049  ------.    >>> I
+00015ca0: 6d61 6765 203d 2062 742e 7261 6e64 2833  mage = bt.rand(3
+00015cb0: 2c20 3130 302c 2031 3230 2c20 3830 290a  , 100, 120, 80).
+00015cc0: 2020 2020 3e3e 3e20 414d 203d 2062 742e      >>> AM = bt.
+00015cd0: 7261 6e64 2834 2c20 3429 0a20 2020 203e  rand(4, 4).    >
+00015ce0: 3e3e 2041 4d5b 332c 203a 5d20 3d20 6274  >> AM[3, :] = bt
+00015cf0: 2e6f 6e65 5f68 6f74 282d 312c 2034 290a  .one_hot(-1, 4).
+00015d00: 2020 2020 3e3e 3e20 696e 7465 7270 6f6c      >>> interpol
+00015d10: 6174 696f 6e28 496d 6167 652c 2041 6666  ation(Image, Aff
+00015d20: 696e 6528 414d 292c 206d 6574 686f 643d  ine(AM), method=
+00015d30: 274c 696e 6561 7227 290a 2020 2020 2727  'Linear').    ''
+00015d40: 270a 2020 2020 6966 2074 7261 6e73 2069  '.    if trans i
+00015d50: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2074  s not None and t
+00015d60: 7261 6e73 2e62 6163 6b77 6172 643a 0a20  rans.backward:. 
+00015d70: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+00015d80: 7228 7472 616e 732c 2027 696e 7627 293a  r(trans, 'inv'):
+00015d90: 2074 7261 6e73 203d 2074 7261 6e73 2e69   trans = trans.i
+00015da0: 6e76 2829 2e66 616b 655f 696e 7628 290a  nv().fake_inv().
+00015db0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015dc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00015dd0: 2257 6172 6e69 6e67 3a20 4261 636b 7761  "Warning: Backwa
+00015de0: 7264 2074 7261 6e73 666f 726d 6174 696f  rd transformatio
+00015df0: 6e20 666f 756e 6420 696e 206d 6574 686f  n found in metho
+00015e00: 6420 6069 6e74 6572 706f 6c61 7469 6f6e  d `interpolation
+00015e10: 5f66 6f72 7761 7264 602e 2055 7369 6e67  _forward`. Using
+00015e20: 2060 696e 7465 7270 6f6c 6174 696f 6e60   `interpolation`
+00015e30: 2069 6e73 7465 6164 2e20 2229 0a20 2020   instead. ").   
+00015e40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015e50: 696e 7465 7270 6f6c 6174 696f 6e28 696d  interpolation(im
+00015e60: 6167 652c 2074 7261 6e73 2c20 6d65 7468  age, trans, meth
+00015e70: 6f64 203d 206d 6574 686f 642c 2074 6172  od = method, tar
+00015e80: 6765 745f 7370 6163 6520 3d20 7461 7267  get_space = targ
+00015e90: 6574 5f73 7061 6365 2c20 6669 6c6c 203d  et_space, fill =
+00015ea0: 2066 696c 6c29 0a20 2020 2072 6574 7572   fill).    retur
+00015eb0: 6e20 4e6f 7449 6d70 6c65 6d65 6e74 6564  n NotImplemented
+00015ec0: 0a0a 2323 2323 2323 2323 2323 2323 2049  ..############ I
+00015ed0: 6d61 6765 2054 7261 6e73 666f 726d 6174  mage Transformat
+00015ee0: 696f 6e73 2023 2323 2323 2323 2323 2323  ions ###########
+00015ef0: 230a 0a63 6c61 7373 2049 6d61 6765 5472  #..class ImageTr
+00015f00: 616e 7366 6f72 6d61 7469 6f6e 2854 7261  ansformation(Tra
+00015f10: 6e73 666f 726d 6174 696f 6e29 3a0a 2020  nsformation):.  
+00015f20: 2020 2020 2020 0a20 2020 2064 6566 205f        .    def _
+00015f30: 5f63 616c 6c5f 5f28 7365 6c66 2c20 5829  _call__(self, X)
+00015f40: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00015f50: 2020 2020 2020 5820 5b62 742e 5465 6e73        X [bt.Tens
+00015f60: 6f72 5d3a 2049 6d61 6765 2074 6f20 6265  or]: Image to be
+00015f70: 2074 7261 6e73 666f 726d 6564 2e0a 2020   transformed..  
+00015f80: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
+00015f90: 285b 6e5f 6261 7463 683a 6f70 7469 6f6e  ([n_batch:option
+00015fa0: 616c 5d2c 207b 6e5f 6368 616e 6e65 6c3a  al], {n_channel:
+00015fb0: 6f70 7469 6f6e 616c 7d2c 206e 4031 2c20  optional}, n@1, 
+00015fc0: 6e40 322c 202e 2e2e 2c20 6e40 6e5f 6469  n@2, ..., n@n_di
+00015fd0: 6d29 0a20 2020 2020 2020 206f 7574 7075  m).        outpu
+00015fe0: 7420 5b62 742e 5465 6e73 6f72 5d3a 2054  t [bt.Tensor]: T
+00015ff0: 6865 2074 7261 6e73 666f 726d 6564 2069  he transformed i
+00016000: 6d61 6765 2e0a 2020 2020 2020 2020 2020  mage..          
+00016010: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00016020: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
+00016030: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
+00016040: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
+00016050: 2027 2727 0a20 2020 2020 2020 2058 203d   '''.        X =
+00016060: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+00016070: 5829 0a20 2020 2020 2020 2069 6620 7365  X).        if se
+00016080: 6c66 2e6e 5f64 696d 2069 7320 4e6f 6e65  lf.n_dim is None
+00016090: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000160a0: 206e 6f74 2058 2e68 6173 5f62 6174 6368   not X.has_batch
+000160b0: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+000160c0: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
+000160d0: 2020 6966 206e 6f74 2058 2e68 6173 5f63    if not X.has_c
+000160e0: 6861 6e6e 656c 3a20 5820 3d20 582e 7374  hannel: X = X.st
+000160f0: 616e 6461 7264 2829 2e75 6e73 7175 6565  andard().unsquee
+00016100: 7a65 287b 317d 290a 2020 2020 2020 2020  ze({1}).        
+00016110: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00016120: 2020 6966 2058 2e6e 5f64 696d 203d 3d20    if X.n_dim == 
+00016130: 7365 6c66 2e6e 5f64 696d 3a20 5820 3d20  self.n_dim: X = 
+00016140: 582e 7265 6d6f 7665 5f73 7065 6369 616c  X.remove_special
+00016150: 5f28 292e 756e 7371 7565 657a 6528 5b5d  _().unsqueeze([]
+00016160: 292e 756e 7371 7565 657a 6528 7b31 7d29  ).unsqueeze({1})
+00016170: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00016180: 6620 582e 6e5f 6469 6d20 3d3d 2073 656c  f X.n_dim == sel
+00016190: 662e 6e5f 6469 6d20 2b20 313a 0a20 2020  f.n_dim + 1:.   
+000161a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000161b0: 582e 6861 735f 6261 7463 683a 2058 2e63  X.has_batch: X.c
+000161c0: 6861 6e6e 656c 5f64 696d 656e 7369 6f6e  hannel_dimension
+000161d0: 203d 204e 6f6e 653b 2058 203d 2058 2e75   = None; X = X.u
+000161e0: 6e73 7175 6565 7a65 287b 3020 6966 2058  nsqueeze({0 if X
+000161f0: 2e62 6174 6368 5f64 696d 656e 7369 6f6e  .batch_dimension
+00016200: 203e 2030 2065 6c73 6520 317d 290a 2020   > 0 else 1}).  
+00016210: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00016220: 6966 2058 2e68 6173 5f63 6861 6e6e 656c  if X.has_channel
+00016230: 3a20 5820 3d20 582e 756e 7371 7565 657a  : X = X.unsqueez
+00016240: 6528 5b5d 290a 2020 2020 2020 2020 2020  e([]).          
+00016250: 2020 2020 2020 656c 7365 3a20 5820 3d20        else: X = 
+00016260: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
+00016270: 6e5f 2830 292e 756e 7371 7565 657a 6528  n_(0).unsqueeze(
+00016280: 7b31 7d29 0a20 2020 2020 2020 2020 2020  {1}).           
+00016290: 2065 6c69 6620 582e 6e5f 6469 6d20 3d3d   elif X.n_dim ==
+000162a0: 2073 656c 662e 6e5f 6469 6d20 2b20 323a   self.n_dim + 2:
+000162b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000162c0: 2023 205f 6368 616e 6e61 6c2f 6261 7463   # _channal/batc
+000162d0: 6820 6469 6d65 6e73 696f 6e73 2075 7365  h dimensions use
+000162e0: 6420 6865 7265 2061 7320 7468 6579 2061  d here as they a
+000162f0: 7265 206e 5f64 696d 2077 6865 6e20 6e6f  re n_dim when no
+00016300: 7420 6578 6973 7465 642e 200a 2020 2020  t existed. .    
+00016310: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00016320: 6f74 2058 2e68 6173 5f62 6174 6368 3a20  ot X.has_batch: 
+00016330: 582e 6261 7463 685f 6469 6d65 6e73 696f  X.batch_dimensio
+00016340: 6e20 3d20 3020 6966 2058 2e5f 6368 616e  n = 0 if X._chan
+00016350: 6e65 6c5f 6469 6d65 6e73 696f 6e20 3e20  nel_dimension > 
+00016360: 3020 656c 7365 2031 0a20 2020 2020 2020  0 else 1.       
+00016370: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00016380: 582e 6861 735f 6368 616e 6e65 6c3a 2058  X.has_channel: X
+00016390: 2e63 6861 6e6e 656c 5f64 696d 656e 7369  .channel_dimensi
+000163a0: 6f6e 203d 2030 2069 6620 582e 5f62 6174  on = 0 if X._bat
+000163b0: 6368 5f64 696d 656e 7369 6f6e 203e 2030  ch_dimension > 0
+000163c0: 2065 6c73 6520 310a 2020 2020 2020 2020   else 1.        
+000163d0: 6176 6f75 6368 2858 2e68 6173 5f62 6174  avouch(X.has_bat
+000163e0: 6368 2061 6e64 2058 2e68 6173 5f63 6861  ch and X.has_cha
+000163f0: 6e6e 656c 2c20 6622 506c 6561 7365 2075  nnel, f"Please u
+00016400: 7365 2062 6174 6f72 6368 2074 656e 736f  se batorch tenso
+00016410: 7220 6f66 2073 697a 6520 5c0a 2020 2020  r of size \.    
+00016420: 2020 2020 2020 2020 285b 6e5f 6261 7463          ([n_batc
+00016430: 685d 2c20 7b7b 6e5f 6368 616e 6e65 6c2f  h], {{n_channel/
+00016440: 6e5f 6665 6174 7572 653a 6f70 7469 6f6e  n_feature:option
+00016450: 616c 7d7d 2c20 6d5f 312c 206d 5f32 2c20  al}}, m_1, m_2, 
+00016460: 2e2e 2e2c 206d 5f72 2920 5b72 3d6e 5f64  ..., m_r) [r=n_d
+00016470: 696d 5d20 666f 7220 5c0a 2020 2020 2020  im] for \.      
+00016480: 2020 2020 2020 2020 2020 7b73 656c 662e            {self.
+00016490: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+000164a0: 5f5f 2e73 706c 6974 2827 2e27 295b 2d31  __.split('.')[-1
+000164b0: 5d7d 2054 7261 6e73 666f 726d 6174 696f  ]} Transformatio
+000164c0: 6e2c 2069 6e73 7465 6164 206f 6620 7b58  n, instead of {X
+000164d0: 2e73 6861 7065 7d2e 2022 290a 2020 2020  .shape}. ").    
+000164e0: 2020 2020 7265 7475 726e 2058 2e63 6c6f      return X.clo
+000164f0: 6e65 2829 0a0a 636c 6173 7320 4e6f 726d  ne()..class Norm
+00016500: 616c 697a 6528 496d 6167 6554 7261 6e73  alize(ImageTrans
+00016510: 666f 726d 6174 696f 6e29 3a0a 2020 2020  formation):.    
+00016520: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00016530: 662c 202a 5f72 616e 6765 293a 0a20 2020  f, *_range):.   
+00016540: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00016550: 204e 6f72 6d61 6c69 7a65 2074 6865 2069   Normalize the i
+00016560: 6e74 656e 7369 7479 206f 6620 616e 2069  ntensity of an i
+00016570: 6d61 6765 2e0a 2020 2020 2020 2020 0a20  mage..        . 
+00016580: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
+00016590: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
+000165a0: 6520 3d20 286c 6f77 2c20 6869 6768 2920  e = (low, high) 
+000165b0: 5b69 6e74 206f 7220 666c 6f61 7420 6f72  [int or float or
+000165c0: 2062 742e 5465 6e73 6f72 5d3a 2054 6865   bt.Tensor]: The
+000165d0: 206c 6f77 6573 7420 2861 6e64 2068 6967   lowest (and hig
+000165e0: 6865 7374 2920 696e 7465 6e73 6974 792e  hest) intensity.
+000165f0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00016600: 2020 7369 7a65 3a20 6c65 6e67 7468 2832    size: length(2
+00016610: 2920 6f72 2028 5b6e 5f62 6174 6368 5d2c  ) or ([n_batch],
+00016620: 207b 327d 290a 2020 2020 2020 2020 2020   {2}).          
+00016630: 2020 0a20 2020 2020 2020 2057 6865 6e20    .        When 
+00016640: 6974 2069 7320 6361 6c6c 6564 3a0a 2020  it is called:.  
+00016650: 2020 2020 2020 2020 2020 5820 5b62 742e            X [bt.
+00016660: 5465 6e73 6f72 5d3a 2049 6d61 6765 2074  Tensor]: Image t
+00016670: 6f20 6265 2074 7261 6e73 666f 726d 6564  o be transformed
+00016680: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016690: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+000166a0: 683a 6f70 7469 6f6e 616c 5d2c 207b 6e5f  h:optional], {n_
+000166b0: 6368 616e 6e65 6c3a 6f70 7469 6f6e 616c  channel:optional
+000166c0: 7d2c 206e 4031 2c20 6e40 322c 202e 2e2e  }, n@1, n@2, ...
+000166d0: 2c20 6e40 6e5f 6469 6d29 0a20 2020 2020  , n@n_dim).     
+000166e0: 2020 2020 2020 206f 7574 7075 7420 5b62         output [b
+000166f0: 742e 5465 6e73 6f72 5d3a 2054 6865 2074  t.Tensor]: The t
+00016700: 7261 6e73 666f 726d 6564 2069 6d61 6765  ransformed image
+00016710: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016720: 2020 7369 7a65 3a20 285b 6e5f 6261 7463    size: ([n_batc
+00016730: 685d 2c20 7b6e 5f63 6861 6e6e 656c 7d2c  h], {n_channel},
+00016740: 206e 4031 2c20 6e40 322c 202e 2e2e 2c20   n@1, n@2, ..., 
+00016750: 6e40 6e5f 6469 6d29 0a20 2020 2020 2020  n@n_dim).       
+00016760: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
+00016770: 6c65 6e28 5f72 616e 6765 2920 3d3d 2030  len(_range) == 0
+00016780: 3a20 5f72 616e 6765 203d 204e 6f6e 650a  : _range = None.
+00016790: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
+000167a0: 285f 7261 6e67 6529 203d 3d20 3120 616e  (_range) == 1 an
+000167b0: 6420 6973 696e 7374 616e 6365 285f 7261  d isinstance(_ra
+000167c0: 6e67 655b 305d 2c20 286c 6973 742c 2074  nge[0], (list, t
+000167d0: 7570 6c65 2929 3a20 5f72 616e 6765 203d  uple)): _range =
+000167e0: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+000167f0: 6c69 7374 285f 7261 6e67 655b 305d 2929  list(_range[0]))
+00016800: 0a20 2020 2020 2020 2065 6c69 6620 6c65  .        elif le
+00016810: 6e28 5f72 616e 6765 2920 3d3d 2031 2061  n(_range) == 1 a
+00016820: 6e64 2069 7369 6e73 7461 6e63 6528 5f72  nd isinstance(_r
+00016830: 616e 6765 5b30 5d2c 2062 742e 5465 6e73  ange[0], bt.Tens
+00016840: 6f72 293a 205f 7261 6e67 6520 3d20 5f72  or): _range = _r
+00016850: 616e 6765 5b30 5d0a 2020 2020 2020 2020  ange[0].        
+00016860: 656c 6966 206c 656e 285f 7261 6e67 6529  elif len(_range)
+00016870: 203d 3d20 313a 205f 7261 6e67 6520 3d20   == 1: _range = 
+00016880: 6274 2e63 6861 6e6e 656c 5f74 656e 736f  bt.channel_tenso
+00016890: 7228 2830 2c20 5f72 616e 6765 2929 0a20  r((0, _range)). 
+000168a0: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
+000168b0: 5f72 616e 6765 2920 3d3d 2032 3a20 5f72  _range) == 2: _r
+000168c0: 616e 6765 203d 2062 742e 6368 616e 6e65  ange = bt.channe
+000168d0: 6c5f 7465 6e73 6f72 285f 7261 6e67 6529  l_tensor(_range)
+000168e0: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
+000168f0: 6169 7365 2054 7970 6545 7272 6f72 2866  aise TypeError(f
+00016900: 2249 6e76 616c 6964 2072 616e 6765 2066  "Invalid range f
+00016910: 6f72 204e 6f72 6d61 6c69 7a65 3a20 7b5f  or Normalize: {_
+00016920: 7261 6e67 657d 2e20 2229 0a20 2020 2020  range}. ").     
+00016930: 2020 2069 6620 5f72 616e 6765 2069 7320     if _range is 
+00016940: 4e6f 6e65 3a20 7061 7373 0a20 2020 2020  None: pass.     
+00016950: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016960: 2020 2020 2069 6620 5f72 616e 6765 2e6e       if _range.n
+00016970: 5f64 696d 203c 2032 3a20 5f72 616e 6765  _dim < 2: _range
+00016980: 203d 205f 7261 6e67 652e 756e 7371 7565   = _range.unsque
+00016990: 657a 6528 5b5d 290a 2020 2020 2020 2020  eze([]).        
+000169a0: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
+000169b0: 652e 6861 735f 6261 7463 683a 205f 7261  e.has_batch: _ra
+000169c0: 6e67 652e 6261 7463 685f 6469 6d65 6e73  nge.batch_dimens
+000169d0: 696f 6e20 3d20 300a 2020 2020 2020 2020  ion = 0.        
+000169e0: 2020 2020 6966 206e 6f74 205f 7261 6e67      if not _rang
+000169f0: 652e 6861 735f 6368 616e 6e65 6c3a 205f  e.has_channel: _
+00016a00: 7261 6e67 652e 6368 616e 6e65 6c5f 6469  range.channel_di
+00016a10: 6d65 6e73 696f 6e20 3d20 310a 2020 2020  mension = 1.    
+00016a20: 2020 2020 2020 2020 6176 6f75 6368 285f          avouch(_
+00016a30: 7261 6e67 652e 6861 735f 6261 7463 6820  range.has_batch 
+00016a40: 616e 6420 5f72 616e 6765 2e68 6173 5f63  and _range.has_c
+00016a50: 6861 6e6e 656c 2c20 6622 506c 6561 7365  hannel, f"Please
+00016a60: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+00016a70: 736f 7220 6f66 2073 697a 6520 5c0a 2020  sor of size \.  
+00016a80: 2020 2020 2020 2020 2020 2020 2020 285b                ([
+00016a90: 6e5f 6261 7463 683a 6f70 7469 6f6e 616c  n_batch:optional
+00016aa0: 5d2c 207b 7b32 7d7d 2920 666f 7220 4e6f  ], {{2}}) for No
+00016ab0: 726d 616c 697a 696e 6720 7061 7261 6d65  rmalizing parame
+00016ac0: 7465 7273 2c20 696e 7374 6561 6420 6f66  ters, instead of
+00016ad0: 207b 5f72 616e 6765 2e73 6861 7065 7d2e   {_range.shape}.
+00016ae0: 2022 290a 2020 2020 2020 2020 7375 7065   ").        supe
+00016af0: 7228 292e 5f5f 696e 6974 5f5f 285f 7261  r().__init__(_ra
+00016b00: 6e67 6529 0a20 2020 2020 2020 2073 656c  nge).        sel
+00016b10: 662e 7261 6e67 6520 3d20 5f72 616e 6765  f.range = _range
+00016b20: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00016b30: 616e 6765 203d 204e 6f6e 650a 0a20 2020  ange = None..   
+00016b40: 2064 6566 205f 5f63 616c 6c5f 5f28 7365   def __call__(se
+00016b50: 6c66 2c20 5829 3a0a 2020 2020 2020 2020  lf, X):.        
+00016b60: 5820 3d20 7375 7065 7228 292e 5f5f 6361  X = super().__ca
+00016b70: 6c6c 5f5f 2858 290a 2020 2020 2020 2020  ll__(X).        
+00016b80: 5f72 616e 6765 203d 2073 656c 662e 7261  _range = self.ra
+00016b90: 6e67 650a 2020 2020 2020 2020 6966 205f  nge.        if _
+00016ba0: 7261 6e67 6520 6973 204e 6f6e 653a 0a20  range is None:. 
+00016bb0: 2020 2020 2020 2020 2020 205f 7261 6e67             _rang
+00016bc0: 6520 3d20 6274 2e71 7561 6e74 696c 6528  e = bt.quantile(
+00016bd0: 582e 666c 6174 7465 6e28 292e 666c 6f61  X.flatten().floa
+00016be0: 7428 292c 2062 6174 6f72 6368 5f74 656e  t(), batorch_ten
+00016bf0: 736f 7228 5b30 2e30 3235 2c20 302e 3937  sor([0.025, 0.97
+00016c00: 355d 292c 2061 7869 733d 2d31 292e 6d6f  5]), axis=-1).mo
+00016c10: 7665 6469 6d28 302c 202d 3129 2e73 7065  vedim(0, -1).spe
+00016c20: 6369 616c 5f66 726f 6d5f 2858 290a 2020  cial_from_(X).  
+00016c30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00016c40: 7261 6e67 6520 3d20 5f72 616e 6765 0a20  range = _range. 
+00016c50: 2020 2020 2020 2072 6574 7572 6e20 2828         return ((
+00016c60: 5820 2d20 5f72 616e 6765 5b2e 2e2e 2c20  X - _range[..., 
+00016c70: 305d 2920 2f20 285f 7261 6e67 655b 2e2e  0]) / (_range[..
+00016c80: 2e2c 2031 5d20 2d20 5f72 616e 6765 5b2e  ., 1] - _range[.
+00016c90: 2e2e 2c20 305d 2929 2e63 6c61 6d70 2830  .., 0])).clamp(0
+00016ca0: 2e2c 2031 2e29 0a20 2020 200a 2020 2020  ., 1.).    .    
+00016cb0: 6465 6620 696e 7628 7365 6c66 293a 0a20  def inv(self):. 
+00016cc0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00016cd0: 616e 6765 2069 7320 6e6f 7420 4e6f 6e65  ange is not None
+00016ce0: 3a20 5f72 616e 6765 203d 2073 656c 662e  : _range = self.
+00016cf0: 7261 6e67 650a 2020 2020 2020 2020 656c  range.        el
+00016d00: 6966 2073 656c 662e 5f72 616e 6765 2069  if self._range i
+00016d10: 7320 6e6f 7420 4e6f 6e65 3a20 5f72 616e  s not None: _ran
+00016d20: 6765 203d 2073 656c 662e 5f72 616e 6765  ge = self._range
+00016d30: 0a20 2020 2020 2020 2065 6c73 653a 2072  .        else: r
+00016d40: 6574 7572 6e20 4e6f 726d 616c 697a 6528  eturn Normalize(
+00016d50: 4e6f 6e65 290a 2020 2020 2020 2020 6465  None).        de
+00016d60: 6e20 3d20 5f72 616e 6765 5b2e 2e2e 2c20  n = _range[..., 
+00016d70: 315d 202d 205f 7261 6e67 655b 2e2e 2e2c  1] - _range[...,
+00016d80: 2030 5d0a 2020 2020 2020 2020 5f72 616e   0].        _ran
+00016d90: 6765 203d 2062 742e 7374 6163 6b28 2d5f  ge = bt.stack(-_
+00016da0: 7261 6e67 655b 2e2e 2e2c 2030 5d2c 2031  range[..., 0], 1
+00016db0: 2d5f 7261 6e67 655b 2e2e 2e2c 2030 5d2c  -_range[..., 0],
+00016dc0: 202d 3129 202f 2064 656e 0a20 2020 2020   -1) / den.     
+00016dd0: 2020 2072 6574 7572 6e20 4e6f 726d 616c     return Normal
+00016de0: 697a 6528 5f72 616e 6765 290a 0a23 2323  ize(_range)..###
+00016df0: 2323 2323 2323 2323 2323 2053 7570 706f  ########## Suppo
+00016e00: 7274 696e 6720 4675 6e63 7469 6f6e 7320  rting Functions 
+00016e10: 2323 2323 2323 2323 2323 2323 0a0a 6465  ############..de
+00016e20: 6620 4273 706c 696e 6528 692c 2055 293a  f Bspline(i, U):
+00016e30: 0a20 2020 2022 2222 0a20 2020 2043 7562  .    """.    Cub
+00016e40: 6963 2042 2d73 706c 696e 6520 6675 6e63  ic B-spline func
+00016e50: 7469 6f6e 2e20 0a20 2020 204e 6f74 653a  tion. .    Note:
+00016e60: 2041 7320 6c6f 6e67 2061 7320 6920 616e   As long as i an
+00016e70: 6420 5520 6861 7665 2074 6865 2073 616d  d U have the sam
+00016e80: 6520 7369 7a65 2c20 616e 7920 7368 6170  e size, any shap
+00016e90: 6520 6f66 2074 656e 736f 7273 2077 6f75  e of tensors wou
+00016ea0: 6c64 2064 6f2e 0a20 2020 200a 2020 2020  ld do..    .    
+00016eb0: 5061 7261 6d73 3a0a 2020 2020 2020 2020  Params:.        
+00016ec0: 6920 5b62 742e 5465 6e73 6f72 5d3a 2074  i [bt.Tensor]: t
+00016ed0: 6865 2069 6e64 6578 206f 6620 7365 676d  he index of segm
+00016ee0: 656e 7420 6675 6e63 7469 6f6e 206f 6620  ent function of 
+00016ef0: 422d 7370 6c69 6e65 2e0a 2020 2020 2020  B-spline..      
+00016f00: 2020 2020 2020 5468 6520 7661 6c75 6520        The value 
+00016f10: 6f66 2065 6163 6820 656c 656d 656e 7420  of each element 
+00016f20: 6361 6e20 6265 2063 686f 7365 6e20 696e  can be chosen in
+00016f30: 2028 2d31 2c20 302c 2031 2c20 3229 2e20   (-1, 0, 1, 2). 
+00016f40: 0a20 2020 2020 2020 2055 205b 6274 2e54  .        U [bt.T
+00016f50: 656e 736f 725d 3a20 7468 6520 6465 6369  ensor]: the deci
+00016f60: 6d61 6c20 6172 6775 6d65 6e74 206f 6620  mal argument of 
+00016f70: 422d 7370 6c69 6e65 2066 756e 6374 696f  B-spline functio
+00016f80: 6e2e 2049 7420 7368 6f75 6c64 2062 6520  n. It should be 
+00016f90: 7769 7468 696e 2072 616e 6765 205b 302c  within range [0,
+00016fa0: 2031 292e 0a20 2020 2022 2222 0a20 2020   1)..    """.   
+00016fb0: 2069 203d 2062 6174 6f72 6368 5f74 656e   i = batorch_ten
+00016fc0: 736f 7228 6929 3b20 5520 3d20 6261 746f  sor(i); U = bato
+00016fd0: 7263 685f 7465 6e73 6f72 2855 290a 2020  rch_tensor(U).  
+00016fe0: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
+00016ff0: 2020 2062 742e 7768 6572 6528 6920 3d3d     bt.where(i ==
+00017000: 202d 312c 2028 3120 2d20 5529 202a 2a20   -1, (1 - U) ** 
+00017010: 3320 2f20 362c 0a20 2020 2020 2020 2062  3 / 6,.        b
+00017020: 742e 7768 6572 6528 6920 3d3d 2030 2c20  t.where(i == 0, 
+00017030: 5520 2a2a 2033 202f 2032 202d 2055 202a  U ** 3 / 2 - U *
+00017040: 2055 202b 2032 202f 2033 2c0a 2020 2020   U + 2 / 3,.    
+00017050: 2020 2020 6274 2e77 6865 7265 2869 203d      bt.where(i =
+00017060: 3d20 312c 2028 2d20 3320 2a20 5520 2a2a  = 1, (- 3 * U **
+00017070: 2033 202b 2033 202a 2055 202a 2055 202b   3 + 3 * U * U +
+00017080: 2033 202a 2055 202b 2031 2920 2f20 362c   3 * U + 1) / 6,
+00017090: 0a20 2020 2020 2020 2062 742e 7768 6572  .        bt.wher
+000170a0: 6528 6920 3d3d 2032 2c20 5520 2a2a 2033  e(i == 2, U ** 3
+000170b0: 202f 2036 2c0a 2020 2020 2020 2020 6274   / 6,.        bt
+000170c0: 2e7a 6572 6f73 5f6c 696b 6528 5529 2929  .zeros_like(U)))
+000170d0: 2929 0a20 2020 2029 0a0a 6465 6620 6442  )).    )..def dB
+000170e0: 7370 6c69 6e65 2869 2c20 5529 3a0a 2020  spline(i, U):.  
+000170f0: 2020 2222 220a 2020 2020 5468 6520 6465    """.    The de
+00017100: 7269 7661 7469 7665 206f 6620 422d 7370  rivative of B-sp
+00017110: 6c69 6e65 2066 756e 6374 696f 6e2c 2077  line function, w
+00017120: 6974 6820 7265 7370 6563 7420 746f 2055  ith respect to U
+00017130: 2e20 0a20 2020 204e 6f74 653a 2041 7320  . .    Note: As 
+00017140: 6c6f 6e67 2061 7320 6920 616e 6420 5520  long as i and U 
+00017150: 6861 7665 2074 6865 2073 616d 6520 7369  have the same si
+00017160: 7a65 2c20 616e 7920 7368 6170 6520 6f66  ze, any shape of
+00017170: 2074 656e 736f 7273 2077 6f75 6c64 2064   tensors would d
+00017180: 6f2e 0a20 2020 200a 2020 2020 5061 7261  o..    .    Para
+00017190: 6d73 3a0a 2020 2020 2020 2020 6920 5b62  ms:.        i [b
+000171a0: 742e 5465 6e73 6f72 5d3a 2074 6865 2069  t.Tensor]: the i
+000171b0: 6e64 6578 206f 6620 7365 676d 656e 7420  ndex of segment 
+000171c0: 6675 6e63 7469 6f6e 206f 6620 422d 7370  function of B-sp
+000171d0: 6c69 6e65 2e0a 2020 2020 2020 2020 2020  line..          
+000171e0: 2020 5468 6520 7661 6c75 6520 6f66 2065    The value of e
+000171f0: 6163 6820 656c 656d 656e 7420 6361 6e20  ach element can 
+00017200: 6265 2063 686f 7365 6e20 696e 2028 2d31  be chosen in (-1
+00017210: 2c20 302c 2031 2c20 3229 2e20 0a20 2020  , 0, 1, 2). .   
+00017220: 2020 2020 2055 205b 6274 2e54 656e 736f       U [bt.Tenso
+00017230: 725d 3a20 7468 6520 6465 6369 6d61 6c20  r]: the decimal 
+00017240: 6172 6775 6d65 6e74 206f 6620 422d 7370  argument of B-sp
+00017250: 6c69 6e65 2066 756e 6374 696f 6e2e 2049  line function. I
+00017260: 7420 7368 6f75 6c64 2062 6520 7769 7468  t should be with
+00017270: 696e 2072 616e 6765 205b 302c 2031 292e  in range [0, 1).
+00017280: 0a20 2020 2022 2222 0a20 2020 2069 203d  .    """.    i =
+00017290: 2062 6174 6f72 6368 5f74 656e 736f 7228   batorch_tensor(
+000172a0: 6929 3b20 5520 3d20 6261 746f 7263 685f  i); U = batorch_
+000172b0: 7465 6e73 6f72 2855 290a 2020 2020 7265  tensor(U).    re
+000172c0: 7475 726e 2028 0a20 2020 2020 2020 2062  turn (.        b
+000172d0: 742e 7768 6572 6528 6920 3d3d 202d 312c  t.where(i == -1,
+000172e0: 202d 2033 202a 2028 3120 2d20 5529 202a   - 3 * (1 - U) *
+000172f0: 2a20 3220 2f20 362c 0a20 2020 2020 2020  * 2 / 6,.       
+00017300: 2062 742e 7768 6572 6528 6920 3d3d 2030   bt.where(i == 0
+00017310: 2c20 3320 2a20 5520 2a2a 2032 202f 2032  , 3 * U ** 2 / 2
+00017320: 202d 2032 202a 2055 2c0a 2020 2020 2020   - 2 * U,.      
+00017330: 2020 6274 2e77 6865 7265 2869 203d 3d20    bt.where(i == 
+00017340: 312c 2028 2d20 3320 2a20 5520 2a2a 2032  1, (- 3 * U ** 2
+00017350: 202b 2032 202a 2055 202b 2031 2920 2f20   + 2 * U + 1) / 
+00017360: 322c 0a20 2020 2020 2020 2062 742e 7768  2,.        bt.wh
+00017370: 6572 6528 6920 3d3d 2032 2c20 3320 2a20  ere(i == 2, 3 * 
+00017380: 5520 2a2a 2032 202f 2036 2c0a 2020 2020  U ** 2 / 6,.    
+00017390: 2020 2020 6274 2e7a 6572 6f73 5f6c 696b      bt.zeros_lik
+000173a0: 6528 5529 2929 2929 0a20 2020 2029 0a0a  e(U))))).    )..
+000173b0: 6465 6620 6642 7370 6c69 6e65 2863 2c20  def fBspline(c, 
+000173c0: 7829 3a0a 2020 2020 6320 3d20 6261 746f  x):.    c = bato
+000173d0: 7263 685f 7465 6e73 6f72 2863 293b 2078  rch_tensor(c); x
+000173e0: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+000173f0: 7228 7829 0a20 2020 2064 203d 2078 202d  r(x).    d = x -
+00017400: 2063 0a20 2020 2072 6574 7572 6e20 280a   c.    return (.
+00017410: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+00017420: 2828 2d32 203c 3d20 6429 202a 2028 6420  ((-2 <= d) * (d 
+00017430: 3c20 2d31 292c 2064 202a 2a20 3320 2b20  < -1), d ** 3 + 
+00017440: 3620 2a20 6420 2a2a 2032 202b 2031 3220  6 * d ** 2 + 12 
+00017450: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
+00017460: 2062 742e 7768 6572 6528 282d 3120 3c3d   bt.where((-1 <=
+00017470: 2064 2920 2a20 2864 203c 2030 292c 202d   d) * (d < 0), -
+00017480: 2033 202a 2064 202a 2a20 3320 2d20 3620   3 * d ** 3 - 6 
+00017490: 2a20 6420 2a2a 2032 202b 2034 2c0a 2020  * d ** 2 + 4,.  
+000174a0: 2020 2020 2020 6274 2e77 6865 7265 2828        bt.where((
+000174b0: 3020 3c3d 2064 2920 2a20 2864 203c 2031  0 <= d) * (d < 1
+000174c0: 292c 2033 202a 2064 202a 2a20 3320 2d20  ), 3 * d ** 3 - 
+000174d0: 3620 2a20 6420 2a2a 2032 202b 2034 2c0a  6 * d ** 2 + 4,.
+000174e0: 2020 2020 2020 2020 6274 2e77 6865 7265          bt.where
+000174f0: 2828 3120 3c3d 2064 2920 2a20 2864 203c  ((1 <= d) * (d <
+00017500: 2032 292c 202d 2064 202a 2a20 3320 2b20   2), - d ** 3 + 
+00017510: 3620 2a20 6420 2a2a 2032 202d 2031 3220  6 * d ** 2 - 12 
+00017520: 2a20 6420 2b20 382c 0a20 2020 2020 2020  * d + 8,.       
+00017530: 2062 742e 7a65 726f 735f 6c69 6b65 2864   bt.zeros_like(d
+00017540: 2929 2929 2920 2f20 360a 2020 2020 290a  ))))) / 6.    ).
+00017550: 0a64 6566 2041 6666 696e 6532 4432 4d61  .def Affine2D2Ma
+00017560: 7472 6978 2870 6172 616d 7329 3a0a 2020  trix(params):.  
+00017570: 2020 2222 220a 2020 2020 7431 2c20 7432    """.    t1, t2
+00017580: 2c20 ceb8 2c20 7331 2c20 7332 2c20 cf81  , .., s1, s2, ..
+00017590: 312c 20cf 8132 2069 6e20 7369 7a65 3a20  1, ..2 in size: 
+000175a0: 285b 6e5f 6261 7463 685d 2c20 7b37 7d29  ([n_batch], {7})
+000175b0: 0a20 2020 2074 312c 2074 322c 2063 312c  .    t1, t2, c1,
+000175c0: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
+000175d0: 20cf 8131 2c20 cf81 3220 696e 2073 697a   ..1, ..2 in siz
+000175e0: 653a 2028 5b6e 5f62 6174 6368 5d2c 207b  e: ([n_batch], {
+000175f0: 397d 290a 2020 2020 6f75 7470 7574 2069  9}).    output i
+00017600: 6e20 7369 7a65 3a20 285b 6e5f 6261 7463  n size: ([n_batc
+00017610: 685d 2c20 332c 2033 290a 2020 2020 2222  h], 3, 3).    ""
+00017620: 220a 2020 2020 7061 7261 6d73 203d 2062  ".    params = b
+00017630: 6174 6f72 6368 5f74 656e 736f 7228 7061  atorch_tensor(pa
+00017640: 7261 6d73 290a 2020 2020 6966 2070 6172  rams).    if par
+00017650: 616d 732e 6e5f 6469 6d20 3c3d 2031 2061  ams.n_dim <= 1 a
+00017660: 6e64 206e 6f74 2070 6172 616d 732e 6861  nd not params.ha
+00017670: 735f 6261 7463 683a 2070 6172 616d 7320  s_batch: params 
+00017680: 3d20 7061 7261 6d73 2e75 6e73 7175 6565  = params.unsquee
+00017690: 7a65 285b 5d29 0a20 2020 2069 6620 7061  ze([]).    if pa
+000176a0: 7261 6d73 2e6e 5f64 696d 203c 3d20 3120  rams.n_dim <= 1 
+000176b0: 616e 6420 6e6f 7420 7061 7261 6d73 2e68  and not params.h
+000176c0: 6173 5f63 6861 6e6e 656c 3a20 7061 7261  as_channel: para
+000176d0: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
+000176e0: 7565 657a 6528 7b31 7d29 0a20 2020 2069  ueeze({1}).    i
+000176f0: 6620 7061 7261 6d73 2e6e 5f64 696d 203d  f params.n_dim =
+00017700: 3d20 3220 616e 6420 6e6f 7420 7061 7261  = 2 and not para
+00017710: 6d73 2e68 6173 5f62 6174 6368 3a20 7061  ms.has_batch: pa
+00017720: 7261 6d73 2e62 6174 6368 5f64 696d 656e  rams.batch_dimen
+00017730: 7369 6f6e 203d 2030 0a20 2020 2069 6620  sion = 0.    if 
+00017740: 7061 7261 6d73 2e6e 5f64 696d 203d 3d20  params.n_dim == 
+00017750: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
+00017760: 2e68 6173 5f63 6861 6e6e 656c 3a20 7061  .has_channel: pa
+00017770: 7261 6d73 2e63 6861 6e6e 656c 5f64 696d  rams.channel_dim
+00017780: 656e 7369 6f6e 203d 2031 0a20 2020 2061  ension = 1.    a
+00017790: 766f 7563 6828 7061 7261 6d73 2e68 6173  vouch(params.has
+000177a0: 5f62 6174 6368 2c20 6622 506c 6561 7365  _batch, f"Please
+000177b0: 2075 7365 2062 6174 6f72 6368 2074 656e   use batorch ten
+000177c0: 736f 7220 6f66 2073 697a 6520 285b 6e5f  sor of size ([n_
+000177d0: 6261 7463 685d 2c20 7b37 206f 7220 397d  batch], {7 or 9}
+000177e0: 2920 5c0a 2020 2020 2020 2020 666f 7220  ) \.        for 
+000177f0: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
+00017800: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
+00017810: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
+00017820: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
+00017830: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
+00017840: 2020 6966 2070 6172 616d 732e 7369 7a65    if params.size
+00017850: 2831 2920 3d3d 2037 3a0a 2020 2020 2020  (1) == 7:.      
+00017860: 2020 7431 2c20 7432 2c20 ceb8 2c20 7331    t1, t2, .., s1
+00017870: 2c20 7332 2c20 cf81 312c 20cf 8132 203d  , s2, ..1, ..2 =
+00017880: 2070 6172 616d 732e 7370 6c69 7428 290a   params.split().
+00017890: 2020 2020 2020 2020 6331 203d 2062 742e          c1 = bt.
+000178a0: 7a65 726f 7328 5b6e 5f62 6174 6368 5d2c  zeros([n_batch],
+000178b0: 2031 293b 2063 3220 3d20 6274 2e7a 6572   1); c2 = bt.zer
+000178c0: 6f73 285b 6e5f 6261 7463 685d 2c20 3129  os([n_batch], 1)
+000178d0: 0a20 2020 2069 6620 7061 7261 6d73 2e73  .    if params.s
+000178e0: 697a 6528 3129 203d 3d20 393a 0a20 2020  ize(1) == 9:.   
+000178f0: 2020 2020 2074 312c 2074 322c 2063 312c       t1, t2, c1,
+00017900: 2063 322c 20ce b82c 2073 312c 2073 322c   c2, .., s1, s2,
+00017910: 20cf 8131 2c20 cf81 3220 3d20 7061 7261   ..1, ..2 = para
+00017920: 6d73 2e73 706c 6974 2829 0a20 2020 2061  ms.split().    a
+00017930: 203d 2028 cf81 3120 2a20 cf81 3220 2b20   = (..1 * ..2 + 
+00017940: 3129 202a 2073 3120 2a20 6274 2e63 6f73  1) * s1 * bt.cos
+00017950: 28ce b829 202b 20cf 8131 202a 2073 3220  (..) + ..1 * s2 
+00017960: 2a20 6274 2e73 696e 28ce b829 0a20 2020  * bt.sin(..).   
+00017970: 2062 203d 202d 2028 cf81 3120 2a20 cf81   b = - (..1 * ..
+00017980: 3220 2b20 3129 202a 2073 3120 2a20 6274  2 + 1) * s1 * bt
+00017990: 2e73 696e 28ce b829 202b 20cf 8131 202a  .sin(..) + ..1 *
+000179a0: 2073 3220 2a20 6274 2e63 6f73 28ce b829   s2 * bt.cos(..)
+000179b0: 0a20 2020 2063 203d 20cf 8132 202a 2073  .    c = ..2 * s
+000179c0: 3120 2a20 6274 2e63 6f73 28ce b829 202b  1 * bt.cos(..) +
+000179d0: 2073 3220 2a20 6274 2e73 696e 28ce b829   s2 * bt.sin(..)
+000179e0: 0a20 2020 2064 203d 202d 20cf 8132 202a  .    d = - ..2 *
+000179f0: 2073 3120 2a20 6274 2e73 696e 28ce b829   s1 * bt.sin(..)
+00017a00: 202b 2073 3220 2a20 6274 2e63 6f73 28ce   + s2 * bt.cos(.
+00017a10: b829 0a20 2020 2072 6574 7572 6e20 6274  .).    return bt
+00017a20: 2e63 6174 280a 2020 2020 2020 2020 6274  .cat(.        bt
+00017a30: 2e63 6174 2828 612c 2062 2c20 7431 202d  .cat((a, b, t1 -
+00017a40: 2061 202a 2063 3120 2d20 6220 2a20 6332   a * c1 - b * c2
+00017a50: 202b 2063 312c 2063 2c20 642c 2074 3220   + c1, c, d, t2 
+00017a60: 2d20 6320 2a20 6331 202d 2064 202a 2063  - c * c1 - d * c
+00017a70: 3220 2b20 6332 292c 207b 7d29 2e76 6965  2 + c2), {}).vie
+00017a80: 7728 5b6e 5f62 6174 6368 5d2c 2032 2c20  w([n_batch], 2, 
+00017a90: 3329 2c20 0a20 2020 2020 2020 2062 742e  3), .        bt.
+00017aa0: 6f6e 655f 686f 7428 2d31 2c20 3329 2e6d  one_hot(-1, 3).m
+00017ab0: 756c 7469 706c 7928 6e5f 6261 7463 682c  ultiply(n_batch,
+00017ac0: 205b 5d29 2e76 6965 7728 5b6e 5f62 6174   []).view([n_bat
+00017ad0: 6368 5d2c 2031 2c20 3329 2c20 310a 2020  ch], 1, 3), 1.  
+00017ae0: 2020 290a 0a64 6566 2051 7561 7465 726e    )..def Quatern
+00017af0: 7332 4d61 7472 6978 2870 6172 616d 7329  s2Matrix(params)
+00017b00: 3a0a 2020 2020 2222 220a 2020 2020 2020  :.    """.      
+00017b10: 2020 5175 6174 6572 6e3a 2071 622c 2071    Quatern: qb, q
+00017b20: 632c 2071 642c 2070 782c 2070 792c 2070  c, qd, px, py, p
+00017b30: 7a20 696e 2073 697a 653a 2028 5b6e 5f62  z in size: ([n_b
+00017b40: 6174 6368 5d2c 207b 367d 290a 2020 2020  atch], {6}).    
+00017b50: 2020 2020 4d61 7472 6978 3a20 285b 6e5f      Matrix: ([n_
+00017b60: 6261 7463 685d 2c20 342c 2034 290a 2020  batch], 4, 4).  
+00017b70: 2020 2222 220a 2020 2020 7061 7261 6d73    """.    params
+00017b80: 203d 2062 6174 6f72 6368 5f74 656e 736f   = batorch_tenso
+00017b90: 7228 7061 7261 6d73 290a 2020 2020 6966  r(params).    if
+00017ba0: 2070 6172 616d 732e 6e5f 6469 6d20 3c3d   params.n_dim <=
+00017bb0: 2031 2061 6e64 206e 6f74 2070 6172 616d   1 and not param
+00017bc0: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
+00017bd0: 616d 7320 3d20 7061 7261 6d73 2e75 6e73  ams = params.uns
+00017be0: 7175 6565 7a65 285b 5d29 0a20 2020 2069  queeze([]).    i
+00017bf0: 6620 7061 7261 6d73 2e6e 5f64 696d 203c  f params.n_dim <
+00017c00: 3d20 3120 616e 6420 6e6f 7420 7061 7261  = 1 and not para
+00017c10: 6d73 2e68 6173 5f63 6861 6e6e 656c 3a20  ms.has_channel: 
+00017c20: 7061 7261 6d73 203d 2070 6172 616d 732e  params = params.
+00017c30: 756e 7371 7565 657a 6528 7b31 7d29 0a20  unsqueeze({1}). 
+00017c40: 2020 2069 6620 7061 7261 6d73 2e6e 5f64     if params.n_d
+00017c50: 696d 203d 3d20 3220 616e 6420 6e6f 7420  im == 2 and not 
+00017c60: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
+00017c70: 3a20 7061 7261 6d73 2e62 6174 6368 5f64  : params.batch_d
+00017c80: 696d 656e 7369 6f6e 203d 2030 0a20 2020  imension = 0.   
+00017c90: 2069 6620 7061 7261 6d73 2e6e 5f64 696d   if params.n_dim
+00017ca0: 203d 3d20 3220 616e 6420 6e6f 7420 7061   == 2 and not pa
+00017cb0: 7261 6d73 2e68 6173 5f63 6861 6e6e 656c  rams.has_channel
+00017cc0: 3a20 7061 7261 6d73 2e63 6861 6e6e 656c  : params.channel
+00017cd0: 5f64 696d 656e 7369 6f6e 203d 2031 0a20  _dimension = 1. 
+00017ce0: 2020 2061 766f 7563 6828 7061 7261 6d73     avouch(params
+00017cf0: 2e6e 5f64 696d 203d 3d20 3220 616e 6420  .n_dim == 2 and 
+00017d00: 7061 7261 6d73 2e68 6173 5f62 6174 6368  params.has_batch
+00017d10: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
+00017d20: 6368 616e 6e65 6c2c 200a 2020 2020 2020  channel, .      
+00017d30: 2020 2020 2066 2250 6c65 6173 6520 7573       f"Please us
+00017d40: 6520 6261 746f 7263 6820 7465 6e73 6f72  e batorch tensor
+00017d50: 206f 6620 7369 7a65 2028 5b6e 5f62 6174   of size ([n_bat
+00017d60: 6368 5d2c 207b 7b36 7d7d 2920 666f 7220  ch], {{6}}) for 
+00017d70: 4166 6669 6e65 2070 6172 616d 6574 6572  Affine parameter
+00017d80: 732c 2069 6e73 7465 6164 206f 6620 7b70  s, instead of {p
+00017d90: 6172 616d 732e 7368 6170 657d 2e20 2229  arams.shape}. ")
+00017da0: 0a20 2020 206e 5f62 6174 6368 203d 2070  .    n_batch = p
+00017db0: 6172 616d 732e 6e5f 6261 7463 680a 2020  arams.n_batch.  
+00017dc0: 2020 622c 2063 2c20 642c 2078 2c20 792c    b, c, d, x, y,
+00017dd0: 207a 203d 2070 6172 616d 732e 7370 6c69   z = params.spli
+00017de0: 7428 290a 2020 2020 6120 3d20 6274 2e73  t().    a = bt.s
+00017df0: 7172 7428 2831 2d62 2a62 2d63 2a63 2d64  qrt((1-b*b-c*c-d
+00017e00: 2a64 292e 636c 616d 7028 3029 290a 2020  *d).clamp(0)).  
+00017e10: 2020 5231 3120 3d20 612a 612b 622a 622d    R11 = a*a+b*b-
+00017e20: 632a 632d 642a 640a 2020 2020 5231 3220  c*c-d*d.    R12 
+00017e30: 3d20 322a 622a 632d 322a 612a 640a 2020  = 2*b*c-2*a*d.  
+00017e40: 2020 5231 3320 3d20 322a 622a 642b 322a    R13 = 2*b*d+2*
+00017e50: 612a 630a 2020 2020 5232 3120 3d20 322a  a*c.    R21 = 2*
+00017e60: 622a 632b 322a 612a 640a 2020 2020 5232  b*c+2*a*d.    R2
+00017e70: 3220 3d20 612a 612b 632a 632d 622a 622d  2 = a*a+c*c-b*b-
+00017e80: 642a 640a 2020 2020 5232 3320 3d20 322a  d*d.    R23 = 2*
+00017e90: 632a 642d 322a 612a 620a 2020 2020 5233  c*d-2*a*b.    R3
+00017ea0: 3120 3d20 322a 622a 642d 322a 612a 630a  1 = 2*b*d-2*a*c.
+00017eb0: 2020 2020 5233 3220 3d20 322a 632a 642b      R32 = 2*c*d+
+00017ec0: 322a 612a 620a 2020 2020 5233 3320 3d20  2*a*b.    R33 = 
+00017ed0: 612a 612b 642a 642d 632a 632d 622a 620a  a*a+d*d-c*c-b*b.
+00017ee0: 2020 2020 7265 7475 726e 2062 742e 6361      return bt.ca
+00017ef0: 7428 0a20 2020 2020 2020 2062 742e 6361  t(.        bt.ca
+00017f00: 7428 2852 3131 2c20 5231 322c 2052 3133  t((R11, R12, R13
+00017f10: 2c20 782c 2052 3231 2c20 5232 322c 2052  , x, R21, R22, R
+00017f20: 3233 2c20 792c 2052 3331 2c20 5233 322c  23, y, R31, R32,
+00017f30: 2052 3333 2c20 7a29 2c20 3129 2e76 6965   R33, z), 1).vie
+00017f40: 7728 5b6e 5f62 6174 6368 5d2c 2033 2c20  w([n_batch], 3, 
+00017f50: 3429 2c0a 2020 2020 2020 2020 6274 2e6f  4),.        bt.o
+00017f60: 6e65 5f68 6f74 282d 312c 2034 292e 6d75  ne_hot(-1, 4).mu
+00017f70: 6c74 6970 6c79 286e 5f62 6174 6368 2c20  ltiply(n_batch, 
+00017f80: 5b5d 292e 7669 6577 285b 6e5f 6261 7463  []).view([n_batc
+00017f90: 685d 2c20 312c 2034 292c 2031 0a20 2020  h], 1, 4), 1.   
+00017fa0: 2029 0a0a 6465 6620 4d61 7472 6978 3251   )..def Matrix2Q
+00017fb0: 7561 7465 726e 7328 7061 7261 6d73 293a  uaterns(params):
+00017fc0: 0a20 2020 2022 2222 0a20 2020 2020 2020  .    """.       
+00017fd0: 204d 6174 7269 783a 2028 5b6e 5f62 6174   Matrix: ([n_bat
+00017fe0: 6368 5d2c 2034 2c20 3429 0a20 2020 2020  ch], 4, 4).     
+00017ff0: 2020 2051 7561 7465 726e 3a20 7162 2c20     Quatern: qb, 
+00018000: 7163 2c20 7164 2c20 7078 2c20 7079 2c20  qc, qd, px, py, 
+00018010: 707a 2069 6e20 7369 7a65 3a20 285b 6e5f  pz in size: ([n_
+00018020: 6261 7463 685d 2c20 7b36 7d29 0a20 2020  batch], {6}).   
+00018030: 2022 2222 0a20 2020 2070 6172 616d 7320   """.    params 
+00018040: 3d20 6261 746f 7263 685f 7465 6e73 6f72  = batorch_tensor
+00018050: 2870 6172 616d 7329 0a20 2020 2069 6620  (params).    if 
+00018060: 7061 7261 6d73 2e6e 5f64 696d 203c 3d20  params.n_dim <= 
+00018070: 3220 616e 6420 6e6f 7420 7061 7261 6d73  2 and not params
+00018080: 2e68 6173 5f62 6174 6368 3a20 7061 7261  .has_batch: para
+00018090: 6d73 203d 2070 6172 616d 732e 756e 7371  ms = params.unsq
+000180a0: 7565 657a 6528 5b5d 290a 2020 2020 6966  ueeze([]).    if
+000180b0: 2070 6172 616d 732e 6e5f 6469 6d20 3d3d   params.n_dim ==
+000180c0: 2033 2061 6e64 206e 6f74 2070 6172 616d   3 and not param
+000180d0: 732e 6861 735f 6261 7463 683a 2070 6172  s.has_batch: par
+000180e0: 616d 732e 6261 7463 685f 6469 6d65 6e73  ams.batch_dimens
+000180f0: 696f 6e20 3d20 300a 2020 2020 6966 2070  ion = 0.    if p
+00018100: 6172 616d 732e 6e5f 6469 6d20 3d3d 2033  arams.n_dim == 3
+00018110: 2061 6e64 2070 6172 616d 732e 6861 735f   and params.has_
+00018120: 6368 616e 6e65 6c3a 2070 6172 616d 732e  channel: params.
+00018130: 6368 616e 6e65 6c5f 6469 6d65 6e73 696f  channel_dimensio
+00018140: 6e20 3d20 4e6f 6e65 0a20 2020 2061 766f  n = None.    avo
+00018150: 7563 6828 7061 7261 6d73 2e6e 5f64 696d  uch(params.n_dim
+00018160: 203d 3d20 3320 616e 6420 7061 7261 6d73   == 3 and params
+00018170: 2e68 6173 5f62 6174 6368 2061 6e64 206e  .has_batch and n
+00018180: 6f74 2070 6172 616d 732e 6861 735f 6368  ot params.has_ch
+00018190: 616e 6e65 6c2c 200a 2020 2020 2020 2020  annel, .        
+000181a0: 2020 2066 2250 6c65 6173 6520 7573 6520     f"Please use 
+000181b0: 6261 746f 7263 6820 7465 6e73 6f72 206f  batorch tensor o
+000181c0: 6620 7369 7a65 2028 5b6e 5f62 6174 6368  f size ([n_batch
+000181d0: 5d2c 2034 2c20 3429 2066 6f72 2041 6666  ], 4, 4) for Aff
+000181e0: 696e 6520 6d61 7472 6978 2c20 696e 7374  ine matrix, inst
+000181f0: 6561 6420 6f66 207b 7061 7261 6d73 2e73  ead of {params.s
+00018200: 6861 7065 7d2e 2022 290a 2020 2020 6e5f  hape}. ").    n_
+00018210: 6261 7463 6820 3d20 7061 7261 6d73 2e6e  batch = params.n
+00018220: 5f62 6174 6368 0a20 2020 2078 2c20 792c  _batch.    x, y,
+00018230: 207a 203d 2070 6172 616d 735b 2e2e 2e2c   z = params[...,
+00018240: 203a 332c 202d 315d 2e63 6861 6e6e 656c   :3, -1].channel
+00018250: 5f64 696d 5f28 3129 2e73 706c 6974 2831  _dim_(1).split(1
+00018260: 2c20 3129 0a20 2020 2061 3220 3d20 2862  , 1).    a2 = (b
+00018270: 742e 6469 6167 2870 6172 616d 7329 2e73  t.diag(params).s
+00018280: 756d 2829 2e75 6e73 7175 6565 7a65 287b  um().unsqueeze({
+00018290: 7d29 202b 2031 2920 2f20 340a 2020 2020  }) + 1) / 4.    
+000182a0: 6120 3d20 6274 2e73 7172 7428 6132 290a  a = bt.sqrt(a2).
+000182b0: 2020 2020 6232 203d 2061 3220 2d20 2870      b2 = a2 - (p
+000182c0: 6172 616d 735b 2e2e 2e2c 2031 2c20 315d  arams[..., 1, 1]
+000182d0: 202b 2070 6172 616d 735b 2e2e 2e2c 2032   + params[..., 2
+000182e0: 2c20 325d 2920 2f20 320a 2020 2020 6332  , 2]) / 2.    c2
+000182f0: 203d 2061 3220 2d20 2870 6172 616d 735b   = a2 - (params[
+00018300: 2e2e 2e2c 2032 2c20 325d 202b 2070 6172  ..., 2, 2] + par
+00018310: 616d 735b 2e2e 2e2c 2030 2c20 305d 2920  ams[..., 0, 0]) 
+00018320: 2f20 320a 2020 2020 6432 203d 2061 3220  / 2.    d2 = a2 
+00018330: 2d20 2870 6172 616d 735b 2e2e 2e2c 2030  - (params[..., 0
+00018340: 2c20 305d 202b 2070 6172 616d 735b 2e2e  , 0] + params[..
+00018350: 2e2c 2031 2c20 315d 2920 2f20 320a 2020  ., 1, 1]) / 2.  
+00018360: 2020 4420 3d20 7061 7261 6d73 202d 2070    D = params - p
+00018370: 6172 616d 732e 540a 2020 2020 6220 3d20  arams.T.    b = 
+00018380: 6274 2e73 6967 6e28 445b 2e2e 2e2c 2032  bt.sign(D[..., 2
+00018390: 2c20 315d 2920 2a20 6274 2e73 7172 7428  , 1]) * bt.sqrt(
+000183a0: 6232 290a 2020 2020 6320 3d20 2d20 6274  b2).    c = - bt
+000183b0: 2e73 6967 6e28 445b 2e2e 2e2c 2032 2c20  .sign(D[..., 2, 
+000183c0: 305d 2920 2a20 6274 2e73 7172 7428 6332  0]) * bt.sqrt(c2
+000183d0: 290a 2020 2020 6420 3d20 6274 2e73 6967  ).    d = bt.sig
+000183e0: 6e28 445b 2e2e 2e2c 2031 2c20 305d 2920  n(D[..., 1, 0]) 
+000183f0: 2a20 6274 2e73 7172 7428 6432 290a 2020  * bt.sqrt(d2).  
+00018400: 2020 7265 7475 726e 2062 742e 6361 7428    return bt.cat(
+00018410: 622c 2063 2c20 642c 2078 2c20 792c 207a  b, c, d, x, y, z
+00018420: 2c20 7b7d 290a                           , {}).
```

### Comparing `micomputing-1.1.44/micomputing/zxhtools/TRS.py` & `micomputing-1.1.45/micomputing/zxhtools/TRS.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc` & `micomputing-1.1.45/micomputing/zxhtools/__pycache__/AFF.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc` & `micomputing-1.1.45/micomputing/zxhtools/__pycache__/FFD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc` & `micomputing-1.1.45/micomputing/zxhtools/__pycache__/TRS.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc` & `micomputing-1.1.45/micomputing/zxhtools/__pycache__/TRS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/exec.py` & `micomputing-1.1.45/micomputing/zxhtools/exec.py`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing/zxhtools/image2.FFD` & `micomputing-1.1.45/micomputing/zxhtools/image2.FFD`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/micomputing.egg-info/PKG-INFO` & `micomputing-1.1.45/micomputing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micomputing
-Version: 1.1.44
+Version: 1.1.45
 Summary: 'micomputing' is a package for medical image computing. 
 Home-page: https://github.com/Bertie97/PyZMyc/micomputing
 Author: Yuncheng Zhou
 Author-email: bertiezhou@163.com
 License: MIT Licence
 Description: # MIComputing
```

### Comparing `micomputing-1.1.44/micomputing.egg-info/SOURCES.txt` & `micomputing-1.1.45/micomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micomputing-1.1.44/setup_micomputing.py` & `micomputing-1.1.45/setup_micomputing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'micomputing',
-	version = '1.1.44',
+	version = '1.1.45',
 	keywords = ['pip', 'pymyc', 'micomputing', 'medical image', 'image registration', 'image similarities'],
 	description = "'micomputing' is a package for medical image computing. ",
 	long_description = '# MIComputing\n\n## Introduction\n\nPackage [`micomputing`](https://github.com/Bertie97/pycamia/tree/main/micomputing) is the medical image processing package under project [`PyCAMIA`](https://github.com/Bertie97/pycamia). It handles medical image read write, image interpolation, transformation, registration and so on. This package works under `PyCAMIA` and use `batorch.Tensor` as its basic data format. \n\n## Installation\n\nThis package can be installed by `pip install micomputing` or moving the source code to the directory of python libraries (the source code can be downloaded on [github](https://github.com/Bertie97/pycamia) or [PyPI](https://pypi.org/project/micomputing/)). \n\n```shell\npip install micomputing\n```\n\n\n\n## Acknowledgment\n\n@Yuncheng Zhou: Developer\n',
 	long_description_content_type = 'text/markdown',
 	license = 'MIT Licence',
 	url = 'https://github.com/Bertie97/PyZMyc/micomputing',
 	author = 'Yuncheng Zhou',
```

