# Comparing `tmp/Slpapy-0.4.2.tar.gz` & `tmp/Slpapy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.4.2.tar", last modified: Sat Jun 24 01:55:27 2023, max compression
+gzip compressed data, was "Slpapy-0.4.3.tar", last modified: Mon Jul 10 02:12:52 2023, max compression
```

## Comparing `Slpapy-0.4.2.tar` & `Slpapy-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:27.004376 Slpapy-0.4.2/
--rw-rw-rw-   0        0        0      159 2023-06-24 01:55:27.002384 Slpapy-0.4.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.955508 Slpapy-0.4.2/Slpapy/
--rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.2/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.2/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.999391 Slpapy-0.4.2/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.2/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.2/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6764 2023-06-24 01:54:46.000000 Slpapy-0.4.2/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-06-24 01:55:26.967476 Slpapy-0.4.2/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 01:55:26.000000 Slpapy-0.4.2/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 01:55:27.004376 Slpapy-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-24 01:54:18.000000 Slpapy-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.220468 Slpapy-0.4.3/
+-rw-rw-rw-   0        0        0      159 2023-07-10 02:12:52.219471 Slpapy-0.4.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.150656 Slpapy-0.4.3/Slpapy/
+-rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.3/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.3/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.215482 Slpapy-0.4.3/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.3/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.3/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6880 2023-06-28 10:02:50.000000 Slpapy-0.4.3/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:12:52.167610 Slpapy-0.4.3/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 02:12:51.000000 Slpapy-0.4.3/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 02:12:52.220468 Slpapy-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-07-10 02:12:42.000000 Slpapy-0.4.3/setup.py
```

### Comparing `Slpapy-0.4.2/Slpapy/Data_reconstruction.py` & `Slpapy-0.4.3/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/MZ_ppm_match.py` & `Slpapy-0.4.3/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.4.3/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.4.2/Slpapy/processing_analyze.py` & `Slpapy-0.4.3/Slpapy/processing_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     sc.tl.leiden(adata, resolution=resolution)
     return adata
 
 
 def third_analyze(adata):
     sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
     sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
+    sc.pl.umap(adata, color='leiden', legend_loc='on data', title='', frameon=False, save='_spacial_on_local.png')
     sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
     result = adata.uns['rank_genes_groups']
     groups = result['names'].dtype.names
     res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
                         ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
     res.to_csv("dif.csv")
     sc.pl.rank_genes_groups(adata, n_genes=20, sharey=False, save='_Wilcoxon.png')
```

### Comparing `Slpapy-0.4.2/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.4.3/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

