# Comparing `tmp/cnmfsns-1.5.3.tar.gz` & `tmp/cnmfsns-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.5.3.tar", last modified: Fri Jun 23 17:43:42 2023, max compression
+gzip compressed data, was "cnmfsns-1.6.0.tar", last modified: Mon Jul 10 18:03:45 2023, max compression
```

## Comparing `cnmfsns-1.5.3.tar` & `cnmfsns-1.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 17:43:42.356757 cnmfsns-1.5.3/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.5.3/LICENSE
--rw-rw-rw-   0        0        0     4320 2023-06-23 17:43:42.357049 cnmfsns-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3805 2023-06-23 17:42:40.000000 cnmfsns-1.5.3/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.5.3/pyproject.toml
--rw-rw-rw-   0        0        0      980 2023-06-23 17:43:42.359085 cnmfsns-1.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 17:43:42.289749 cnmfsns-1.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 17:43:42.329954 cnmfsns-1.5.3/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.5.3/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    52096 2023-06-23 17:43:01.000000 cnmfsns-1.5.3/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.5.3/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.5.3/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.5.3/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35838 2023-06-23 16:14:21.000000 cnmfsns-1.5.3/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.5.3/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    59406 2023-06-23 17:03:17.000000 cnmfsns-1.5.3/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.5.3/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.5.3/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 17:43:42.354956 cnmfsns-1.5.3/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     4320 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 17:43:42.000000 cnmfsns-1.5.3/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     4320 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2023-07-10 16:56:05.000000 cnmfsns-1.6.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      980 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.447642 cnmfsns-1.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.479030 cnmfsns-1.6.0/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.6.0/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    52096 2023-07-10 16:41:48.000000 cnmfsns-1.6.0/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.6.0/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.6.0/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    36423 2023-07-10 18:02:42.000000 cnmfsns-1.6.0/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.6.0/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    59662 2023-07-10 17:04:09.000000 cnmfsns-1.6.0/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.6.0/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-07-10 02:54:46.000000 cnmfsns-1.6.0/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:03:45.510708 cnmfsns-1.6.0/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     4320 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 18:03:45.000000 cnmfsns-1.6.0/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.5.3/LICENSE` & `cnmfsns-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/PKG-INFO` & `cnmfsns-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.3
+Version: 1.6.0
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.5.3-blue)
+![version badge](https://img.shields.io/badge/version-1.6.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.5.3/README.md` & `cnmfsns-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e35 2e33 2d62 6c75  ersion-1.5.3-blu
+000000b0: 6572 7369 6f6e 2d31 2e36 2e30 2d62 6c75  ersion-1.6.0-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.5.3/setup.cfg` & `cnmfsns-1.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 352e 330d 0a61 7574  ion = 1.5.3..aut
+00000020: 696f 6e20 3d20 312e 362e 300d 0a61 7574  ion = 1.6.0..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.5.3/src/cnmfsns/__init__.py` & `cnmfsns-1.6.0/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/cli.py` & `cnmfsns-1.6.0/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/cnmf.py` & `cnmfsns-1.6.0/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/colors.py` & `cnmfsns-1.6.0/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/config.py` & `cnmfsns-1.6.0/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/dataset.py` & `cnmfsns-1.6.0/src/cnmfsns/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2060,181 +2060,218 @@
 000080b0: 5f63 6f6c 5f73 7472 7d20 6d65 7461 6461  _col_str} metada
 000080c0: 7461 2063 6f6c 756d 6e73 2068 6176 6520  ta columns have 
 000080d0: 756e 7265 636f 676e 697a 6564 2064 7479  unrecognized dty
 000080e0: 7065 732e 2229 0d0a 2020 2020 2020 2020  pes.")..        
 000080f0: 6466 203d 2073 656c 662e 6164 6174 612e  df = self.adata.
 00008100: 6f62 732e 7365 6c65 6374 5f64 7479 7065  obs.select_dtype
 00008110: 7328 696e 636c 7564 653d 6474 7970 6573  s(include=dtypes
-00008120: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00008130: 6e20 6466 0d0a 2020 2020 0d0a 2020 2020  n df..    ..    
-00008140: 6465 6620 6765 745f 6361 7465 676f 7279  def get_category
-00008150: 5f6f 7665 7272 6570 7265 7365 6e74 6174  _overrepresentat
-00008160: 696f 6e28 7365 6c66 2c0d 0a20 2020 2020  ion(self,..     
-00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 206c 6179 6572 3a20 7374 722c 0d0a     layer: str,..
+00008120: 290d 0a20 2020 2020 2020 2064 6620 3d20  )..        df = 
+00008130: 6466 2e64 726f 706e 6128 6178 6973 3d31  df.dropna(axis=1
+00008140: 2c20 686f 773d 2261 6c6c 2229 0d0a 2020  , how="all")..  
+00008150: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
+00008160: 0a20 2020 200d 0a20 2020 2064 6566 2067  .    ..    def g
+00008170: 6574 5f63 6174 6567 6f72 795f 6f76 6572  et_category_over
+00008180: 7265 7072 6573 656e 7461 7469 6f6e 2873  representation(s
+00008190: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
 000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 2020 2020 2020 7472 756e 6361 7465          truncate
-000081d0: 5f6e 6567 6174 6976 653a 2062 6f6f 6c20  _negative: bool 
-000081e0: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
-00008220: 653a 0d0a 2020 2020 2020 2020 2222 2243  e:..        """C
-00008230: 616c 6375 6c61 7465 2050 6561 7273 6f6e  alculate Pearson
-00008240: 2072 6573 6964 7561 6c20 6f66 2063 6869   residual of chi
-00008250: 2d73 7175 6172 6564 2074 6573 742c 2061  -squared test, a
-00008260: 7373 6f63 6961 7469 6e67 2047 4550 7320  ssociating GEPs 
-00008270: 666f 7220 6561 6368 2072 616e 6b20 286b  for each rank (k
-00008280: 2920 746f 2063 6174 6567 6f72 6965 7320  ) to categories 
-00008290: 6f66 2073 616d 706c 6573 2f6f 6273 6572  of samples/obser
-000082a0: 7661 7469 6f6e 732e 2042 7920 6465 6661  vations. By defa
-000082b0: 756c 742c 2074 7275 6e63 6174 6573 206e  ult, truncates n
-000082c0: 6567 6174 6976 6520 7661 6c75 6573 2e0d  egative values..
-000082d0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000082e0: 6d20 6c61 7965 723a 206e 616d 6520 6f66  m layer: name of
-000082f0: 2063 6174 6567 6f72 6963 616c 2064 6174   categorical dat
-00008300: 6120 6c61 7965 720d 0a20 2020 2020 2020  a layer..       
-00008310: 203a 7479 7065 206c 6179 6572 3a20 7374   :type layer: st
-00008320: 720d 0a20 2020 2020 2020 203a 7061 7261  r..        :para
-00008330: 6d20 7472 756e 6361 7465 5f6e 6567 6174  m truncate_negat
-00008340: 6976 653a 2054 7275 6e63 6174 6520 6e65  ive: Truncate ne
-00008350: 6761 7469 7665 2072 6573 6964 7561 6c73  gative residuals
-00008360: 2074 6f20 302c 2064 6566 6175 6c74 7320   to 0, defaults 
-00008370: 746f 2054 7275 650d 0a20 2020 2020 2020  to True..       
-00008380: 203a 7479 7065 2074 7275 6e63 6174 655f   :type truncate_
-00008390: 6e65 6761 7469 7665 3a20 626f 6f6c 2c20  negative: bool, 
-000083a0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000083b0: 2020 3a72 6574 7572 6e3a 2063 6174 6567    :return: categ
-000083c0: 6f72 7920 c397 2047 4550 206d 6174 7269  ory .. GEP matri
-000083d0: 7820 6f66 206f 7665 7272 6570 7265 7365  x of overreprese
-000083e0: 6e74 6174 696f 6e20 7661 6c75 6573 0d0a  ntation values..
-000083f0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00008400: 7064 2e44 6174 6146 7261 6d65 0d0a 2020  pd.DataFrame..  
-00008410: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00008420: 2020 2075 7361 6765 203d 2073 656c 662e     usage = self.
-00008430: 6765 745f 7573 6167 6573 286e 6f72 6d61  get_usages(norma
-00008440: 6c69 7a65 3d54 7275 6529 2e63 6f70 7928  lize=True).copy(
-00008450: 290d 0a20 2020 2020 2020 2073 616d 706c  )..        sampl
-00008460: 655f 746f 5f63 6c61 7373 203d 2073 656c  e_to_class = sel
-00008470: 662e 6765 745f 6d65 7461 6461 7461 5f64  f.get_metadata_d
-00008480: 6628 295b 6c61 7965 725d 0d0a 2020 2020  f()[layer]..    
-00008490: 2020 2020 7573 6167 652e 696e 6465 7820      usage.index 
-000084a0: 3d20 7573 6167 652e 696e 6465 782e 6d61  = usage.index.ma
-000084b0: 7028 7361 6d70 6c65 5f74 6f5f 636c 6173  p(sample_to_clas
-000084c0: 7329 0d0a 2020 2020 2020 2020 6f62 7365  s)..        obse
-000084d0: 7276 6564 203d 2075 7361 6765 2e67 726f  rved = usage.gro
-000084e0: 7570 6279 2861 7869 733d 302c 206c 6576  upby(axis=0, lev
-000084f0: 656c 3d30 292e 7375 6d28 290d 0a20 2020  el=0).sum()..   
-00008500: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
-00008510: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
-00008520: 6b2c 206f 6273 5f6b 2069 6e20 6f62 7365  k, obs_k in obse
-00008530: 7276 6564 2e67 726f 7570 6279 2861 7869  rved.groupby(axi
-00008540: 733d 312c 206c 6576 656c 3d31 293a 0d0a  s=1, level=1):..
-00008550: 2020 2020 2020 2020 2020 2020 6578 705f              exp_
-00008560: 6b20 3d20 7064 2e44 6174 6146 7261 6d65  k = pd.DataFrame
-00008570: 286f 6273 5f6b 2e73 756d 2861 7869 733d  (obs_k.sum(axis=
-00008580: 3129 2920 4020 7064 2e44 6174 6146 7261  1)) @ pd.DataFra
-00008590: 6d65 286f 6273 5f6b 2e73 756d 2861 7869  me(obs_k.sum(axi
-000085a0: 733d 3029 292e 5420 2f20 6f62 735f 6b2e  s=0)).T / obs_k.
-000085b0: 7375 6d28 292e 7375 6d28 290d 0a20 2020  sum().sum()..   
-000085c0: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
-000085d0: 642e 6170 7065 6e64 2865 7870 5f6b 290d  d.append(exp_k).
-000085e0: 0a20 2020 2020 2020 2065 7870 6563 7465  .        expecte
-000085f0: 6420 3d20 7064 2e63 6f6e 6361 7428 6578  d = pd.concat(ex
-00008600: 7065 6374 6564 2c20 6178 6973 3d31 290d  pected, axis=1).
-00008610: 0a20 2020 2020 2020 2063 6869 7371 5f72  .        chisq_r
-00008620: 6573 6964 203d 2028 6f62 7365 7276 6564  esid = (observed
-00008630: 202d 2065 7870 6563 7465 6429 202f 206e   - expected) / n
-00008640: 702e 7371 7274 2865 7870 6563 7465 6429  p.sqrt(expected)
-00008650: 2020 2320 7065 6172 736f 6e20 7265 7369    # pearson resi
-00008660: 6475 616c 206f 6620 6368 692d 7371 7561  dual of chi-squa
-00008670: 7265 6420 7465 7374 206f 6620 636f 6e74  red test of cont
-00008680: 696e 6765 6e63 7920 7461 626c 650d 0a20  ingency table.. 
-00008690: 2020 2020 2020 2069 6620 7472 756e 6361         if trunca
-000086a0: 7465 5f6e 6567 6174 6976 653a 0d0a 2020  te_negative:..  
-000086b0: 2020 2020 2020 2020 2020 6368 6973 715f            chisq_
-000086c0: 7265 7369 6420 3d20 6368 6973 715f 7265  resid = chisq_re
-000086d0: 7369 642e 636c 6970 286c 6f77 6572 3d30  sid.clip(lower=0
-000086e0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000086f0: 6e20 6368 6973 715f 7265 7369 640d 0a20  n chisq_resid.. 
-00008700: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-00008710: 2020 2064 6566 2067 6574 5f6d 6574 6164     def get_metad
-00008720: 6174 615f 636f 7272 656c 6174 696f 6e28  ata_correlation(
-00008730: 7365 6c66 2c20 0d0a 2020 2020 2020 2020  self, ..        
-00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 2020 2020 2020 2020 206c 6179 6572 3a20           layer: 
-00008760: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2020 206d 6574 686f 643a 2073         method: s
-00008790: 7472 203d 2022 7065 6172 736f 6e22 0d0a  tr = "pearson"..
-000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2029 202d 3e20 7064 2e53 6572 6965 733a   ) -> pd.Series:
-000087d0: 0d0a 2020 2020 2020 2020 2222 2243 616c  ..        """Cal
-000087e0: 6375 6c61 7465 2050 6561 7273 6f6e 2063  culate Pearson c
-000087f0: 6f72 7265 6c61 7469 6f6e 206f 6620 4745  orrelation of GE
-00008800: 5020 7573 6167 6520 746f 206e 756d 6572  P usage to numer
-00008810: 6963 616c 206d 6574 6164 6174 6120 6163  ical metadata ac
-00008820: 726f 7373 2073 616d 706c 6573 2f6f 6273  ross samples/obs
-00008830: 6572 7661 7469 6f6e 732e 0d0a 0d0a 2020  ervations.....  
-00008840: 2020 2020 2020 3a70 6172 616d 206c 6179        :param lay
-00008850: 6572 3a20 6e61 6d65 206f 6620 6e75 6d65  er: name of nume
-00008860: 7269 6361 6c20 6461 7461 206c 6179 6572  rical data layer
-00008870: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00008880: 6c61 7965 723a 2073 7472 0d0a 2020 2020  layer: str..    
-00008890: 2020 2020 3a70 6172 616d 206d 6574 686f      :param metho
-000088a0: 643a 2043 6f72 7265 6c61 7469 6f6e 206d  d: Correlation m
-000088b0: 6574 686f 643a 2022 7065 6172 736f 6e22  ethod: "pearson"
-000088c0: 2c20 2273 7065 6172 6d61 6e22 2c20 6f72  , "spearman", or
-000088d0: 2022 6b65 6e64 616c 6c22 2e20 4465 6661   "kendall". Defa
-000088e0: 756c 7473 2074 6f20 2270 6561 7273 6f6e  ults to "pearson
-000088f0: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
-00008900: 206d 6574 686f 643a 2073 7472 2c20 6f70   method: str, op
-00008910: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00008920: 3a72 6574 7572 6e3a 2063 6f72 7265 6c61  :return: correla
-00008930: 7469 6f6e 206f 6620 4745 5020 746f 206d  tion of GEP to m
-00008940: 6574 6164 6174 610d 0a20 2020 2020 2020  etadata..       
-00008950: 203a 7274 7970 653a 2070 642e 5365 7269   :rtype: pd.Seri
-00008960: 6573 0d0a 2020 2020 2020 2020 2222 220d  es..        """.
-00008970: 0a20 2020 2020 2020 2075 7361 6765 203d  .        usage =
-00008980: 2073 656c 662e 6765 745f 7573 6167 6573   self.get_usages
-00008990: 2829 2e63 6f70 7928 290d 0a20 2020 2020  ().copy()..     
-000089a0: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
-000089b0: 6c66 2e67 6574 5f6d 6574 6164 6174 615f  lf.get_metadata_
-000089c0: 6466 2829 5b6c 6179 6572 5d0d 0a20 2020  df()[layer]..   
-000089d0: 2020 2020 206d 645f 636f 7272 203d 2075       md_corr = u
-000089e0: 7361 6765 2e63 6f72 7277 6974 6828 6d65  sage.corrwith(me
-000089f0: 7461 6461 7461 2c20 6d65 7468 6f64 3d6d  tadata, method=m
-00008a00: 6574 686f 6429 0d0a 2020 2020 2020 2020  ethod)..        
-00008a10: 7265 7475 726e 206d 645f 636f 7272 0d0a  return md_corr..
-00008a20: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00008a30: 6620 6170 7065 6e64 5f74 6f5f 6869 7374  f append_to_hist
-00008a40: 6f72 7928 7365 6c66 2c20 656e 7472 7929  ory(self, entry)
-00008a50: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
-00008a60: 6420 656e 7472 7920 746f 2044 6174 6173  d entry to Datas
-00008a70: 6574 2068 6973 746f 7279 2e0d 0a0d 0a20  et history..... 
-00008a80: 2020 2020 2020 203a 7061 7261 6d20 656e         :param en
-00008a90: 7472 793a 2044 6573 6372 6970 7469 6f6e  try: Description
-00008aa0: 206f 6620 6576 656e 7420 746f 2072 6563   of event to rec
-00008ab0: 6f72 6420 696e 2074 6865 2068 6973 746f  ord in the histo
-00008ac0: 7279 2e0d 0a20 2020 2020 2020 203a 7479  ry...        :ty
-00008ad0: 7065 2065 6e74 7279 3a20 7374 720d 0a20  pe entry: str.. 
-00008ae0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00008af0: 2020 2020 7365 6c66 2e61 6461 7461 2e75      self.adata.u
-00008b00: 6e73 5b22 6869 7374 6f72 7922 5d5b 6461  ns["history"][da
-00008b10: 7465 7469 6d65 2e75 7463 6e6f 7728 292e  tetime.utcnow().
-00008b20: 6973 6f66 6f72 6d61 7428 295d 203d 2065  isoformat()] = e
-00008b30: 6e74 7279 0d0a 2020 2020 2020 2020 0d0a  ntry..        ..
-00008b40: 2020 2020 6465 6620 6765 745f 6869 7374      def get_hist
-00008b50: 6f72 7928 7365 6c66 293a 0d0a 2020 2020  ory(self):..    
-00008b60: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
-00008b70: 696d 6573 7461 6d70 6564 2068 6973 746f  imestamped histo
-00008b80: 7279 206f 6620 4461 7461 7365 7420 6f62  ry of Dataset ob
-00008b90: 6a65 6374 2e0d 0a0d 0a20 2020 2020 2020  ject.....       
-00008ba0: 203a 7265 7475 726e 3a20 6869 7374 6f72   :return: histor
-00008bb0: 790d 0a20 2020 2020 2020 203a 7274 7970  y..        :rtyp
-00008bc0: 653a 2064 6963 740d 0a20 2020 2020 2020  e: dict..       
-00008bd0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00008be0: 7475 726e 2073 656c 662e 6164 6174 612e  turn self.adata.
-00008bf0: 756e 735b 2268 6973 746f 7279 225d       uns["history"]
+000081b0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+000081c0: 7965 723a 2073 7472 2c0d 0a20 2020 2020  yer: str,..     
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 2020 2074 7275 6e63 6174 655f 6e65 6761     truncate_nega
+00008200: 7469 7665 3a20 626f 6f6c 203d 2054 7275  tive: bool = Tru
+00008210: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008230: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+00008240: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
+00008250: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
+00008260: 6174 6520 5065 6172 736f 6e20 7265 7369  ate Pearson resi
+00008270: 6475 616c 206f 6620 6368 692d 7371 7561  dual of chi-squa
+00008280: 7265 6420 7465 7374 2c20 6173 736f 6369  red test, associ
+00008290: 6174 696e 6720 4745 5073 2066 6f72 2065  ating GEPs for e
+000082a0: 6163 6820 7261 6e6b 2028 6b29 2074 6f20  ach rank (k) to 
+000082b0: 6361 7465 676f 7269 6573 206f 6620 7361  categories of sa
+000082c0: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
+000082d0: 6e73 2e20 4279 2064 6566 6175 6c74 2c20  ns. By default, 
+000082e0: 7472 756e 6361 7465 7320 6e65 6761 7469  truncates negati
+000082f0: 7665 2076 616c 7565 732e 0d0a 0d0a 2020  ve values.....  
+00008300: 2020 2020 2020 3a70 6172 616d 206c 6179        :param lay
+00008310: 6572 3a20 6e61 6d65 206f 6620 6361 7465  er: name of cate
+00008320: 676f 7269 6361 6c20 6461 7461 206c 6179  gorical data lay
+00008330: 6572 0d0a 2020 2020 2020 2020 3a74 7970  er..        :typ
+00008340: 6520 6c61 7965 723a 2073 7472 0d0a 2020  e layer: str..  
+00008350: 2020 2020 2020 3a70 6172 616d 2074 7275        :param tru
+00008360: 6e63 6174 655f 6e65 6761 7469 7665 3a20  ncate_negative: 
+00008370: 5472 756e 6361 7465 206e 6567 6174 6976  Truncate negativ
+00008380: 6520 7265 7369 6475 616c 7320 746f 2030  e residuals to 0
+00008390: 2c20 6465 6661 756c 7473 2074 6f20 5472  , defaults to Tr
+000083a0: 7565 0d0a 2020 2020 2020 2020 3a74 7970  ue..        :typ
+000083b0: 6520 7472 756e 6361 7465 5f6e 6567 6174  e truncate_negat
+000083c0: 6976 653a 2062 6f6f 6c2c 206f 7074 696f  ive: bool, optio
+000083d0: 6e61 6c0d 0a20 2020 2020 2020 203a 7265  nal..        :re
+000083e0: 7475 726e 3a20 6361 7465 676f 7279 20c3  turn: category .
+000083f0: 9720 4745 5020 6d61 7472 6978 206f 6620  . GEP matrix of 
+00008400: 6f76 6572 7265 7072 6573 656e 7461 7469  overrepresentati
+00008410: 6f6e 2076 616c 7565 730d 0a20 2020 2020  on values..     
+00008420: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
+00008430: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
+00008440: 2022 2222 0d0a 2020 2020 2020 2020 7573   """..        us
+00008450: 6167 6520 3d20 7365 6c66 2e67 6574 5f75  age = self.get_u
+00008460: 7361 6765 7328 6e6f 726d 616c 697a 653d  sages(normalize=
+00008470: 5472 7565 292e 636f 7079 2829 0d0a 2020  True).copy()..  
+00008480: 2020 2020 2020 7361 6d70 6c65 5f74 6f5f        sample_to_
+00008490: 636c 6173 7320 3d20 7365 6c66 2e67 6574  class = self.get
+000084a0: 5f6d 6574 6164 6174 615f 6466 2829 5b6c  _metadata_df()[l
+000084b0: 6179 6572 5d0d 0a20 2020 2020 2020 2075  ayer]..        u
+000084c0: 7361 6765 2e69 6e64 6578 203d 2075 7361  sage.index = usa
+000084d0: 6765 2e69 6e64 6578 2e6d 6170 2873 616d  ge.index.map(sam
+000084e0: 706c 655f 746f 5f63 6c61 7373 290d 0a20  ple_to_class).. 
+000084f0: 2020 2020 2020 206f 6273 6572 7665 6420         observed 
+00008500: 3d20 7573 6167 652e 6772 6f75 7062 7928  = usage.groupby(
+00008510: 6178 6973 3d30 2c20 6c65 7665 6c3d 3029  axis=0, level=0)
+00008520: 2e73 756d 2829 0d0a 0d0a 2020 2020 2020  .sum()....      
+00008530: 2020 6e5f 6361 7465 676f 7269 6573 203d    n_categories =
+00008540: 206f 6273 6572 7665 642e 7368 6170 655b   observed.shape[
+00008550: 305d 0d0a 2020 2020 2020 2020 6966 206e  0]..        if n
+00008560: 5f63 6174 6567 6f72 6965 7320 3c20 323a  _categories < 2:
+00008570: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00008580: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
+00008590: 4f76 6572 7265 7072 6573 656e 7461 7469  Overrepresentati
+000085a0: 6f6e 2063 6f75 6c64 206e 6f74 2062 6520  on could not be 
+000085b0: 6361 6c63 756c 6174 6564 2066 6f72 206c  calculated for l
+000085c0: 6179 6572 2027 7b6c 6179 6572 7d27 2c20  ayer '{layer}', 
+000085d0: 6173 206f 6e6c 7920 7b6e 5f63 6174 6567  as only {n_categ
+000085e0: 6f72 6965 737d 2063 6174 6567 6f72 6965  ories} categorie
+000085f0: 7320 7765 7265 2066 6f75 6e64 2069 6e20  s were found in 
+00008600: 7468 6520 6461 7461 2e20 220d 0a20 2020  the data. "..   
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2020 2020 2020 2066 224e 6f74 6520           f"Note 
+00008630: 7468 6174 2065 6d70 7479 2076 616c 7565  that empty value
+00008640: 7320 696e 2074 6865 206d 6574 6164 6174  s in the metadat
+00008650: 6120 6172 6520 6e6f 7420 636f 6e73 6964  a are not consid
+00008660: 6572 6564 2061 2063 6174 6567 6f72 792e  ered a category.
+00008670: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
+00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008690: 6622 4f76 6572 7265 7072 6573 656e 7461  f"Overrepresenta
+000086a0: 7469 6f6e 2063 616e 6e6f 7420 6265 2063  tion cannot be c
+000086b0: 616c 6375 6c61 7465 6420 7769 7468 2066  alculated with f
+000086c0: 6577 6572 2074 6861 6e20 3220 6361 7465  ewer than 2 cate
+000086d0: 676f 7269 6573 2066 6f72 2065 6163 6820  gories for each 
+000086e0: 6c61 7965 722e 2022 290d 0a20 2020 2020  layer. ")..     
+000086f0: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
+00008700: 2e44 6174 6146 7261 6d65 286e 702e 4e61  .DataFrame(np.Na
+00008710: 4e2c 2069 6e64 6578 203d 206f 6273 6572  N, index = obser
+00008720: 7665 642e 696e 6465 782c 2063 6f6c 756d  ved.index, colum
+00008730: 6e73 3d6f 6273 6572 7665 642e 636f 6c75  ns=observed.colu
+00008740: 6d6e 7329 0d0a 2020 2020 2020 2020 6578  mns)..        ex
+00008750: 7065 6374 6564 203d 205b 5d0d 0a20 2020  pected = []..   
+00008760: 2020 2020 2066 6f72 206b 2c20 6f62 735f       for k, obs_
+00008770: 6b20 696e 206f 6273 6572 7665 642e 6772  k in observed.gr
+00008780: 6f75 7062 7928 6178 6973 3d31 2c20 6c65  oupby(axis=1, le
+00008790: 7665 6c3d 3129 3a0d 0a20 2020 2020 2020  vel=1):..       
+000087a0: 2020 2020 2065 7870 5f6b 203d 2070 642e       exp_k = pd.
+000087b0: 4461 7461 4672 616d 6528 6f62 735f 6b2e  DataFrame(obs_k.
+000087c0: 7375 6d28 6178 6973 3d31 2929 2040 2070  sum(axis=1)) @ p
+000087d0: 642e 4461 7461 4672 616d 6528 6f62 735f  d.DataFrame(obs_
+000087e0: 6b2e 7375 6d28 6178 6973 3d30 2929 2e54  k.sum(axis=0)).T
+000087f0: 202f 206f 6273 5f6b 2e73 756d 2829 2e73   / obs_k.sum().s
+00008800: 756d 2829 0d0a 2020 2020 2020 2020 2020  um()..          
+00008810: 2020 6578 7065 6374 6564 2e61 7070 656e    expected.appen
+00008820: 6428 6578 705f 6b29 0d0a 2020 2020 2020  d(exp_k)..      
+00008830: 2020 6578 7065 6374 6564 203d 2070 642e    expected = pd.
+00008840: 636f 6e63 6174 2865 7870 6563 7465 642c  concat(expected,
+00008850: 2061 7869 733d 3129 0d0a 2020 2020 2020   axis=1)..      
+00008860: 2020 6368 6973 715f 7265 7369 6420 3d20    chisq_resid = 
+00008870: 286f 6273 6572 7665 6420 2d20 6578 7065  (observed - expe
+00008880: 6374 6564 2920 2f20 6e70 2e73 7172 7428  cted) / np.sqrt(
+00008890: 6578 7065 6374 6564 2920 2023 2070 6561  expected)  # pea
+000088a0: 7273 6f6e 2072 6573 6964 7561 6c20 6f66  rson residual of
+000088b0: 2063 6869 2d73 7175 6172 6564 2074 6573   chi-squared tes
+000088c0: 7420 6f66 2063 6f6e 7469 6e67 656e 6379  t of contingency
+000088d0: 2074 6162 6c65 0d0a 2020 2020 2020 2020   table..        
+000088e0: 6966 2074 7275 6e63 6174 655f 6e65 6761  if truncate_nega
+000088f0: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
+00008900: 2020 2063 6869 7371 5f72 6573 6964 203d     chisq_resid =
+00008910: 2063 6869 7371 5f72 6573 6964 2e63 6c69   chisq_resid.cli
+00008920: 7028 6c6f 7765 723d 3029 0d0a 2020 2020  p(lower=0)..    
+00008930: 2020 2020 7265 7475 726e 2063 6869 7371      return chisq
+00008940: 5f72 6573 6964 0d0a 2020 2020 0d0a 2020  _resid..    ..  
+00008950: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
+00008960: 6765 745f 6d65 7461 6461 7461 5f63 6f72  get_metadata_cor
+00008970: 7265 6c61 7469 6f6e 2873 656c 662c 200d  relation(self, .
+00008980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 6c61 7965 723a 2073 7472 2c0d 0a20    layer: str,.. 
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 6d65 7468 6f64 3a20 7374 7220 3d20 2270  method: str = "p
+000089e0: 6561 7273 6f6e 220d 0a20 2020 2020 2020  earson"..       
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
+00008a10: 642e 5365 7269 6573 3a0d 0a20 2020 2020  d.Series:..     
+00008a20: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+00008a30: 5065 6172 736f 6e20 636f 7272 656c 6174  Pearson correlat
+00008a40: 696f 6e20 6f66 2047 4550 2075 7361 6765  ion of GEP usage
+00008a50: 2074 6f20 6e75 6d65 7269 6361 6c20 6d65   to numerical me
+00008a60: 7461 6461 7461 2061 6372 6f73 7320 7361  tadata across sa
+00008a70: 6d70 6c65 732f 6f62 7365 7276 6174 696f  mples/observatio
+00008a80: 6e73 2e0d 0a0d 0a20 2020 2020 2020 203a  ns.....        :
+00008a90: 7061 7261 6d20 6c61 7965 723a 206e 616d  param layer: nam
+00008aa0: 6520 6f66 206e 756d 6572 6963 616c 2064  e of numerical d
+00008ab0: 6174 6120 6c61 7965 720d 0a20 2020 2020  ata layer..     
+00008ac0: 2020 203a 7479 7065 206c 6179 6572 3a20     :type layer: 
+00008ad0: 7374 720d 0a20 2020 2020 2020 203a 7061  str..        :pa
+00008ae0: 7261 6d20 6d65 7468 6f64 3a20 436f 7272  ram method: Corr
+00008af0: 656c 6174 696f 6e20 6d65 7468 6f64 3a20  elation method: 
+00008b00: 2270 6561 7273 6f6e 222c 2022 7370 6561  "pearson", "spea
+00008b10: 726d 616e 222c 206f 7220 226b 656e 6461  rman", or "kenda
+00008b20: 6c6c 222e 2044 6566 6175 6c74 7320 746f  ll". Defaults to
+00008b30: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
+00008b40: 2020 2020 3a74 7970 6520 6d65 7468 6f64      :type method
+00008b50: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
+00008b60: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00008b70: 3a20 636f 7272 656c 6174 696f 6e20 6f66  : correlation of
+00008b80: 2047 4550 2074 6f20 6d65 7461 6461 7461   GEP to metadata
+00008b90: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00008ba0: 3a20 7064 2e53 6572 6965 730d 0a20 2020  : pd.Series..   
+00008bb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00008bc0: 2020 7573 6167 6520 3d20 7365 6c66 2e67    usage = self.g
+00008bd0: 6574 5f75 7361 6765 7328 292e 636f 7079  et_usages().copy
+00008be0: 2829 0d0a 2020 2020 2020 2020 6d65 7461  ()..        meta
+00008bf0: 6461 7461 203d 2073 656c 662e 6765 745f  data = self.get_
+00008c00: 6d65 7461 6461 7461 5f64 6628 295b 6c61  metadata_df()[la
+00008c10: 7965 725d 0d0a 2020 2020 2020 2020 6d64  yer]..        md
+00008c20: 5f63 6f72 7220 3d20 7573 6167 652e 636f  _corr = usage.co
+00008c30: 7272 7769 7468 286d 6574 6164 6174 612c  rrwith(metadata,
+00008c40: 206d 6574 686f 643d 6d65 7468 6f64 290d   method=method).
+00008c50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00008c60: 6d64 5f63 6f72 720d 0a20 2020 2020 2020  md_corr..       
+00008c70: 200d 0a20 2020 2064 6566 2061 7070 656e   ..    def appen
+00008c80: 645f 746f 5f68 6973 746f 7279 2873 656c  d_to_history(sel
+00008c90: 662c 2065 6e74 7279 293a 0d0a 2020 2020  f, entry):..    
+00008ca0: 2020 2020 2222 2241 6464 2065 6e74 7279      """Add entry
+00008cb0: 2074 6f20 4461 7461 7365 7420 6869 7374   to Dataset hist
+00008cc0: 6f72 792e 0d0a 0d0a 2020 2020 2020 2020  ory.....        
+00008cd0: 3a70 6172 616d 2065 6e74 7279 3a20 4465  :param entry: De
+00008ce0: 7363 7269 7074 696f 6e20 6f66 2065 7665  scription of eve
+00008cf0: 6e74 2074 6f20 7265 636f 7264 2069 6e20  nt to record in 
+00008d00: 7468 6520 6869 7374 6f72 792e 0d0a 2020  the history...  
+00008d10: 2020 2020 2020 3a74 7970 6520 656e 7472        :type entr
+00008d20: 793a 2073 7472 0d0a 2020 2020 2020 2020  y: str..        
+00008d30: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00008d40: 662e 6164 6174 612e 756e 735b 2268 6973  f.adata.uns["his
+00008d50: 746f 7279 225d 5b64 6174 6574 696d 652e  tory"][datetime.
+00008d60: 7574 636e 6f77 2829 2e69 736f 666f 726d  utcnow().isoform
+00008d70: 6174 2829 5d20 3d20 656e 7472 790d 0a20  at()] = entry.. 
+00008d80: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00008d90: 2067 6574 5f68 6973 746f 7279 2873 656c   get_history(sel
+00008da0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00008db0: 5265 7475 726e 7320 7469 6d65 7374 616d  Returns timestam
+00008dc0: 7065 6420 6869 7374 6f72 7920 6f66 2044  ped history of D
+00008dd0: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
+00008de0: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00008df0: 6e3a 2068 6973 746f 7279 0d0a 2020 2020  n: history..    
+00008e00: 2020 2020 3a72 7479 7065 3a20 6469 6374      :rtype: dict
+00008e10: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00008e20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00008e30: 6c66 2e61 6461 7461 2e75 6e73 5b22 6869  lf.adata.uns["hi
+00008e40: 7374 6f72 7922 5d                        story"]
```

### Comparing `cnmfsns-1.5.3/src/cnmfsns/integration.py` & `cnmfsns-1.6.0/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/plots.py` & `cnmfsns-1.6.0/src/cnmfsns/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,17 @@
         # data and metadata must have the same index
         metadata = metadata.loc[data.index]
         gs2 = mpl.gridspec.GridSpecFromSubplotSpec(metadata.shape[1], 1, subplot_spec=gs0[2])
         for i, (track, annot) in enumerate(metadata.items()):
             ax = fig.add_subplot(gs2[i], sharex=ax_heatmap)
             ax.set_facecolor(missing_data_color)
             if pd.api.types.is_categorical_dtype(annot) or pd.api.types.is_object_dtype(annot):
-                ordered_rgb = annot.iloc[xind].replace(metadata_colors[track])
+                ordered_rgb = annot.iloc[xind]
+                ordered_rgb[~ordered_rgb.isin(metadata_colors[track])] = np.NaN
+                ordered_rgb = ordered_rgb.replace(metadata_colors[track])
                 if ordered_rgb.isnull().any():
                     if pd.api.types.is_categorical_dtype(annot):
                         ordered_rgb = ordered_rgb.cat.add_categories(missing_data_color)
                     ordered_rgb = ordered_rgb.fillna(missing_data_color)
                 ordered_rgb = ordered_rgb.astype("object").map(mpl.colors.to_rgb)
                 ordered_rgb = np.array([list(rgb) for rgb in ordered_rgb])
                 ax.imshow(np.stack([ordered_rgb, ordered_rgb]), aspect='auto', extent=[xmin,xmax,0,1], interpolation='none')
@@ -437,15 +439,15 @@
     if subset_datasets is not None:
         df = df.loc[subset_datasets]
         
     
     metadata = snsmap.integration.get_metadata_df()
     if subset_metadata is not None:
         metadata = metadata.loc[:, subset_metadata]
-    
+
     metadata_colors = {col: colors.get_metadata_colors(col) for col in metadata.columns}
     if prepend_dataset_colors:
         metadata.insert(0, "dataset", metadata.index.get_level_values(0))
         metadata_colors["dataset"] = colors.dataset_colors
     
     
     fig = annotated_heatmap(data=df, metadata=metadata,
@@ -626,15 +628,20 @@
         width = width / np.max(width)
 
     nx.draw_networkx_edges(snsmap.gep_graph, pos=snsmap.layout, edge_color=edge_color, ax=ax_plot, width=width)
     overrepresentation = snsmap.integration.get_category_overrepresentation(subset_datasets=subset_datasets, layer=layer)
     overrepresentation = overrepresentation.fillna(0)
 
     max_or = np.max(overrepresentation.values.flatten())
-    scale_factor = 1 / max_or
+    if max_or == 0:
+        scale_factor = 1
+    else:
+        scale_factor = 1 / max_or
+    
+    
     for gep, gep_or in overrepresentation.items():
         node = "|".join((str(p) for p in gep))
 
         if node in snsmap.gep_graph and gep_or.any():
             color_list = gep_or.index.map(colors.get_metadata_colors(layer))
             draw_circle_bar_plot(position=snsmap.layout[node],
                                  enrichments=gep_or,
@@ -1044,15 +1051,18 @@
         width = None
 
     nx.draw_networkx_edges(snsmap.comm_graph, pos=snsmap.comm_layout, edge_color=edge_color, ax=ax_plot, width=width)
     overrepresentation = snsmap.get_community_category_overrepresentation(subset_datasets=subset_datasets, layer=layer)
     overrepresentation = overrepresentation.fillna(0)
 
     max_or = np.max(overrepresentation.values.flatten())
-    scale_factor = 1 / max_or
+    if max_or == 0:
+        scale_factor = 1
+    else:
+        scale_factor = 1 / max_or
     for community, comm_or in overrepresentation.items():
         if community in snsmap.comm_graph and comm_or.any():
             color_list = comm_or.index.map(colors.get_metadata_colors(layer))
             draw_circle_bar_plot(position=snsmap.comm_layout[community],
                                  enrichments=comm_or,
                                  scale_factor=scale_factor,
                                  colors=color_list,
@@ -1250,15 +1260,15 @@
                                       ax = None
                                       ) -> Figure:
     
     df = snsmap.get_community_category_overrepresentation(subset_datasets=subset_datasets, layer=layer).fillna(0)
     # if existing axes object is provided, plots with legend on that axes. Otherwise, creates a new figure with a separate plot and legend Axes.
     if ax is None:
         if figsize is None:
-            figsize = [0.1 * df.shape[1] + 3, 3]
+            figsize = [0.1 * df.shape[1] + 4, 4]
         fig, (ax_plot, ax_legend) = plt.subplots(1, 2, figsize=figsize, sharey=True, gridspec_kw={"width_ratios": [4, 1]}, layout="tight")
         ax_legend.set_axis_off()
     else:
         ax_plot = ax
         ax_legend = ax
         
     # Overrepresentation plot
```

### Comparing `cnmfsns-1.5.3/src/cnmfsns/sns.py` & `cnmfsns-1.6.0/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns/utils.py` & `cnmfsns-1.6.0/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.3/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.6.0/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.3
+Version: 1.6.0
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.5.3-blue)
+![version badge](https://img.shields.io/badge/version-1.6.0-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

