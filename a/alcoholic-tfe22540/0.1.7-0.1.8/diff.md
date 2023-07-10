# Comparing `tmp/alcoholic_tfe22540-0.1.7.tar.gz` & `tmp/alcoholic_tfe22540-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcoholic_tfe22540-0.1.7.tar", last modified: Mon Dec 19 16:33:38 2022, max compression
+gzip compressed data, was "alcoholic_tfe22540-0.1.8.tar", last modified: Mon Jul 10 08:16:05 2023, max compression
```

## Comparing `alcoholic_tfe22540-0.1.7.tar` & `alcoholic_tfe22540-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 16:33:38.867428 alcoholic_tfe22540-0.1.7/
--rw-rw-rw-   0        0        0     8469 2022-12-19 16:33:38.866002 alcoholic_tfe22540-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     7946 2022-12-13 15:38:42.000000 alcoholic_tfe22540-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2022-12-19 16:33:38.814529 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/
--rw-rw-rw-   0        0        0     8469 2022-12-19 16:33:38.000000 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2022-12-19 16:33:38.000000 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 16:33:38.000000 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2022-12-19 16:33:38.000000 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-19 16:33:38.000000 alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-19 16:33:38.868541 alcoholic_tfe22540-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1331 2022-12-19 16:32:44.000000 alcoholic_tfe22540-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-19 16:33:38.862902 alcoholic_tfe22540-0.1.7/tfe22540/
--rw-rw-rw-   0        0        0     4578 2022-12-16 10:35:07.000000 alcoholic_tfe22540-0.1.7/tfe22540/CN2.py
--rw-rw-rw-   0        0        0     5893 2022-12-19 15:24:23.000000 alcoholic_tfe22540-0.1.7/tfe22540/Corpus_callosum_division.py
--rw-rw-rw-   0        0        0     3875 2022-12-19 15:25:58.000000 alcoholic_tfe22540-0.1.7/tfe22540/Corpus_callosum_reg.py
--rw-rw-rw-   0        0        0     4821 2022-12-19 15:26:10.000000 alcoholic_tfe22540-0.1.7/tfe22540/DMD_before_reg.py
--rw-rw-rw-   0        0        0     6185 2022-12-19 15:27:01.000000 alcoholic_tfe22540-0.1.7/tfe22540/DTI_kmeans_clustering.py
--rw-rw-rw-   0        0        0    15376 2022-12-19 15:27:08.000000 alcoholic_tfe22540-0.1.7/tfe22540/DTI_tissue_classification.py
--rw-rw-rw-   0        0        0     5911 2022-12-19 15:27:19.000000 alcoholic_tfe22540-0.1.7/tfe22540/FA_DMD.py
--rw-rw-rw-   0        0        0     1854 2022-11-17 08:44:52.000000 alcoholic_tfe22540-0.1.7/tfe22540/Stat_test.py
--rw-rw-rw-   0        0        0        0 2022-12-19 15:20:53.000000 alcoholic_tfe22540-0.1.7/tfe22540/__init__.py
--rw-rw-rw-   0        0        0    53993 2022-12-19 15:22:56.000000 alcoholic_tfe22540-0.1.7/tfe22540/analyse_ttest.py
--rw-rw-rw-   0        0        0     7194 2022-12-19 15:23:03.000000 alcoholic_tfe22540-0.1.7/tfe22540/atlas_modif_name.py
--rw-rw-rw-   0        0        0     2784 2022-12-19 15:23:11.000000 alcoholic_tfe22540-0.1.7/tfe22540/atlas_registration.py
--rw-rw-rw-   0        0        0    34689 2022-12-19 15:23:21.000000 alcoholic_tfe22540-0.1.7/tfe22540/clustering.py
--rw-rw-rw-   0        0        0    37380 2022-12-19 15:23:30.000000 alcoholic_tfe22540-0.1.7/tfe22540/clustering_v2.py
--rw-rw-rw-   0        0        0    10073 2022-12-19 15:24:16.000000 alcoholic_tfe22540-0.1.7/tfe22540/comportement.py
--rw-rw-rw-   0        0        0     9779 2022-12-19 15:26:15.000000 alcoholic_tfe22540-0.1.7/tfe22540/dMRI_metric_reg.py
--rw-rw-rw-   0        0        0     1925 2022-12-19 15:26:05.000000 alcoholic_tfe22540-0.1.7/tfe22540/diamond_fractions.py
--rw-rw-rw-   0        0        0     2510 2022-12-19 15:27:14.000000 alcoholic_tfe22540-0.1.7/tfe22540/f0_f1_to_ftot.py
--rw-rw-rw-   0        0        0     5939 2022-12-19 15:27:34.000000 alcoholic_tfe22540-0.1.7/tfe22540/job_submission.py
--rw-rw-rw-   0        0        0    10455 2022-12-19 15:28:00.000000 alcoholic_tfe22540-0.1.7/tfe22540/moyenne_ROI_v2.py
--rw-rw-rw-   0        0        0    25142 2022-12-19 15:01:39.000000 alcoholic_tfe22540-0.1.7/tfe22540/moyenne_par_ROI.py
--rw-rw-rw-   0        0        0     1494 2022-12-19 15:28:10.000000 alcoholic_tfe22540-0.1.7/tfe22540/opening_closing.py
--rw-rw-rw-   0        0        0     2165 2022-11-17 07:33:16.000000 alcoholic_tfe22540-0.1.7/tfe22540/perso_path.py
--rw-rw-rw-   0        0        0     8477 2022-12-19 15:28:22.000000 alcoholic_tfe22540-0.1.7/tfe22540/plot_functions.py
--rw-rw-rw-   0        0        0     2861 2022-12-13 13:03:23.000000 alcoholic_tfe22540-0.1.7/tfe22540/preprocessing.py
--rw-rw-rw-   0        0        0     6130 2022-11-16 21:19:54.000000 alcoholic_tfe22540-0.1.7/tfe22540/registration.py
--rw-rw-rw-   0        0        0    55481 2022-12-19 15:29:16.000000 alcoholic_tfe22540-0.1.7/tfe22540/ttest.py
--rw-rw-rw-   0        0        0     2684 2022-12-19 15:29:22.000000 alcoholic_tfe22540-0.1.7/tfe22540/useful_fct.py
--rw-rw-rw-   0        0        0     6060 2022-12-19 15:29:38.000000 alcoholic_tfe22540-0.1.7/tfe22540/volumes_zones.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/
+-rw-rw-rw-   0        0        0     8446 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7946 2022-12-13 15:38:44.000000 alcoholic_tfe22540-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.637513 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/
+-rw-rw-rw-   0        0        0     8446 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2023-07-10 08:14:00.000000 alcoholic_tfe22540-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/tfe22540/
+-rw-rw-rw-   0        0        0     4578 2022-12-16 10:35:08.000000 alcoholic_tfe22540-0.1.8/tfe22540/CN2.py
+-rw-rw-rw-   0        0        0     5893 2022-12-19 15:24:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_division.py
+-rw-rw-rw-   0        0        0     3875 2022-12-19 15:26:00.000000 alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_reg.py
+-rw-rw-rw-   0        0        0     4821 2022-12-19 15:26:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/DMD_before_reg.py
+-rw-rw-rw-   0        0        0     6185 2022-12-19 15:27:02.000000 alcoholic_tfe22540-0.1.8/tfe22540/DTI_kmeans_clustering.py
+-rw-rw-rw-   0        0        0    15376 2022-12-19 15:27:10.000000 alcoholic_tfe22540-0.1.8/tfe22540/DTI_tissue_classification.py
+-rw-rw-rw-   0        0        0     6009 2023-07-10 08:10:19.000000 alcoholic_tfe22540-0.1.8/tfe22540/FA_DMD.py
+-rw-rw-rw-   0        0        0     1854 2022-11-17 08:44:54.000000 alcoholic_tfe22540-0.1.8/tfe22540/Stat_test.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 15:20:54.000000 alcoholic_tfe22540-0.1.8/tfe22540/__init__.py
+-rw-rw-rw-   0        0        0    53993 2022-12-19 15:22:58.000000 alcoholic_tfe22540-0.1.8/tfe22540/analyse_ttest.py
+-rw-rw-rw-   0        0        0     7194 2022-12-19 15:23:04.000000 alcoholic_tfe22540-0.1.8/tfe22540/atlas_modif_name.py
+-rw-rw-rw-   0        0        0     2784 2022-12-19 15:23:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/atlas_registration.py
+-rw-rw-rw-   0        0        0    34689 2022-12-19 15:23:22.000000 alcoholic_tfe22540-0.1.8/tfe22540/clustering.py
+-rw-rw-rw-   0        0        0    37380 2022-12-19 15:23:32.000000 alcoholic_tfe22540-0.1.8/tfe22540/clustering_v2.py
+-rw-rw-rw-   0        0        0    10073 2022-12-19 15:24:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/comportement.py
+-rw-rw-rw-   0        0        0     9779 2022-12-19 15:26:16.000000 alcoholic_tfe22540-0.1.8/tfe22540/dMRI_metric_reg.py
+-rw-rw-rw-   0        0        0     1925 2022-12-19 15:26:06.000000 alcoholic_tfe22540-0.1.8/tfe22540/diamond_fractions.py
+-rw-rw-rw-   0        0        0     2510 2022-12-19 15:27:16.000000 alcoholic_tfe22540-0.1.8/tfe22540/f0_f1_to_ftot.py
+-rw-rw-rw-   0        0        0     5939 2022-12-19 15:27:36.000000 alcoholic_tfe22540-0.1.8/tfe22540/job_submission.py
+-rw-rw-rw-   0        0        0    10455 2022-12-19 15:28:02.000000 alcoholic_tfe22540-0.1.8/tfe22540/moyenne_ROI_v2.py
+-rw-rw-rw-   0        0        0    25142 2022-12-19 15:01:40.000000 alcoholic_tfe22540-0.1.8/tfe22540/moyenne_par_ROI.py
+-rw-rw-rw-   0        0        0     1494 2022-12-19 15:28:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/opening_closing.py
+-rw-rw-rw-   0        0        0     2165 2022-11-17 07:33:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/perso_path.py
+-rw-rw-rw-   0        0        0     8477 2022-12-19 15:28:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/plot_functions.py
+-rw-rw-rw-   0        0        0     2861 2022-12-13 13:03:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/preprocessing.py
+-rw-rw-rw-   0        0        0     6130 2022-11-16 21:19:56.000000 alcoholic_tfe22540-0.1.8/tfe22540/registration.py
+-rw-rw-rw-   0        0        0    55481 2022-12-19 15:29:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/ttest.py
+-rw-rw-rw-   0        0        0     2684 2022-12-19 15:29:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/useful_fct.py
+-rw-rw-rw-   0        0        0     6060 2022-12-19 15:29:40.000000 alcoholic_tfe22540-0.1.8/tfe22540/volumes_zones.py
```

### Comparing `alcoholic_tfe22540-0.1.7/PKG-INFO` & `alcoholic_tfe22540-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: alcoholic_tfe22540
-Version: 0.1.7
+Version: 0.1.8
 Summary: Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.
 Home-page: https://github.com/mdausort/TFE22-540
 Author: Manon Dausort
 Author-email: manon.dausort@uclouvain.be
 License: BSD 2-clause
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 
 # Install in local 
 If you want to download the lastest version directly from GitHub, you can close this repository
 
@@ -77,9 +76,7 @@
   14) [`analyse_ttest.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/analyse_ttest.py): Creation of all the plots concerning the analysis of each model separately (they are saved in the file **Plots** in [Analyse](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/tree/main/Analyse)). Then, creation of excel called **Cluster_ROI** used to do the coherence analysis.
   
   15) [`DTI_tissue_classification.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/DTI_tissue_classification.py): To analyse change in volume for WM, GM and CSF. 
   
   16) [`volume_zones.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/volumes_zones.py): To analyse change in volume for certain areas of the brain. 
   
   17) [`comportement.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/comportement.py): To analyse the data coming from behavioral information. 
-
-
```

### Comparing `alcoholic_tfe22540-0.1.7/README.md` & `alcoholic_tfe22540-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/PKG-INFO` & `alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: alcoholic-tfe22540
-Version: 0.1.7
+Version: 0.1.8
 Summary: Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.
 Home-page: https://github.com/mdausort/TFE22-540
 Author: Manon Dausort
 Author-email: manon.dausort@uclouvain.be
 License: BSD 2-clause
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 
 # Install in local 
 If you want to download the lastest version directly from GitHub, you can close this repository
 
@@ -77,9 +76,7 @@
   14) [`analyse_ttest.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/analyse_ttest.py): Creation of all the plots concerning the analysis of each model separately (they are saved in the file **Plots** in [Analyse](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/tree/main/Analyse)). Then, creation of excel called **Cluster_ROI** used to do the coherence analysis.
   
   15) [`DTI_tissue_classification.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/DTI_tissue_classification.py): To analyse change in volume for WM, GM and CSF. 
   
   16) [`volume_zones.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/volumes_zones.py): To analyse change in volume for certain areas of the brain. 
   
   17) [`comportement.py`](https://github.com/PiLAB-Medical-Imaging/TFE22-540_Alcohol/blob/main/Codes/comportement.py): To analyse the data coming from behavioral information. 
-
-
```

### Comparing `alcoholic_tfe22540-0.1.7/alcoholic_tfe22540.egg-info/SOURCES.txt` & `alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/setup.py` & `alcoholic_tfe22540-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='alcoholic_tfe22540',
-    version='0.1.7',    
+    version='0.1.8',
     description='Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdausort/TFE22-540',
     author='Manon Dausort',
     author_email='manon.dausort@uclouvain.be',
     license='BSD 2-clause',
     packages=['tfe22540'],
     install_requires=['numpy',
-                      'nibabel',     
+                      'nibabel',
                       'xlsxwriter',
                       'pandas',
                       'matplotlib',
                       'sklearn',
                       'seaborn',
                       'dipy',
                       'scikit-image',
                       'scipy',
                       'openpyxl'
                       ],
 
     classifiers=[
-        'Intended Audience :: Science/Research',    
+        'Intended Audience :: Science/Research',
         'Programming Language :: Python',
     ],
-)
+)
```

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/CN2.py` & `alcoholic_tfe22540-0.1.8/tfe22540/CN2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/Corpus_callosum_division.py` & `alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_division.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/Corpus_callosum_reg.py` & `alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/DMD_before_reg.py` & `alcoholic_tfe22540-0.1.8/tfe22540/DMD_before_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/DTI_kmeans_clustering.py` & `alcoholic_tfe22540-0.1.8/tfe22540/DTI_kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/DTI_tissue_classification.py` & `alcoholic_tfe22540-0.1.8/tfe22540/DTI_tissue_classification.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/FA_DMD.py` & `alcoholic_tfe22540-0.1.8/tfe22540/FA_DMD.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,27 @@
                     RD[i,j,k] = (copy_valeurs_propres[0]+copy_valeurs_propres[1])/2
                     
                     if((valeurs_propres[0]**2 + valeurs_propres[1]**2 + valeurs_propres[2]**2) == 0):
                         FA[i,j,k] = 0
                     else:
                         FA[i,j,k] = np.sqrt(3/2)*np.sqrt(((valeurs_propres[0] - MD[i,j,k])**2 + (valeurs_propres[1] - MD[i,j,k])**2 + (valeurs_propres[2] - MD[i,j,k])**2)/(valeurs_propres[0]**2 + valeurs_propres[1]**2 + valeurs_propres[2]**2))
                     
+        MD[np.isnan(MD)] = 0
         out = nib.Nifti1Image(MD, affine = nib.load(path).affine, header = nib.load(path).header)
         out.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_MD_DMD_" + tenseur + ".nii.gz")
-        
+
+        AD[np.isnan(AD)] = 0
         out1 = nib.Nifti1Image(AD, affine = nib.load(path).affine, header = nib.load(path).header)
         out1.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_AD_DMD_" + tenseur + ".nii.gz")
-        
+
+        RD[np.isnan(RD)] = 0
         out2 = nib.Nifti1Image(RD, affine = nib.load(path).affine, header = nib.load(path).header)
         out2.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_RD_DMD_" + tenseur + ".nii.gz")
-        
+
+        FA[np.isnan(FA)] = 0
         out3 = nib.Nifti1Image(FA, affine = nib.load(path).affine, header = nib.load(path).header)
         out3.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_FA_DMD_" + tenseur + ".nii.gz")
         
        
 
 def get_cMetrics(folder_path, patient_path):
 
@@ -109,8 +113,8 @@
         
         fraction_t1 = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_diamond_fractions_f1.nii.gz"
         
         
         cMetric = (nib.load(metric_t0).get_fdata() * nib.load(fraction_t0).get_fdata() + nib.load(metric_t1).get_fdata() * nib.load(fraction_t1).get_fdata())/(nib.load(fraction_t1).get_fdata() + nib.load(fraction_t0).get_fdata())
         
         out = nib.Nifti1Image(cMetric, affine = nib.load(metric_t0).affine, header = nib.load(metric_t0).header)
-        out.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_w" + metric + ".nii.gz")
+        out.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_w" + metric + ".nii.gz")
```

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/Stat_test.py` & `alcoholic_tfe22540-0.1.8/tfe22540/Stat_test.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/analyse_ttest.py` & `alcoholic_tfe22540-0.1.8/tfe22540/analyse_ttest.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/atlas_modif_name.py` & `alcoholic_tfe22540-0.1.8/tfe22540/atlas_modif_name.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/atlas_registration.py` & `alcoholic_tfe22540-0.1.8/tfe22540/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/clustering.py` & `alcoholic_tfe22540-0.1.8/tfe22540/clustering.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/clustering_v2.py` & `alcoholic_tfe22540-0.1.8/tfe22540/clustering_v2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/comportement.py` & `alcoholic_tfe22540-0.1.8/tfe22540/comportement.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/dMRI_metric_reg.py` & `alcoholic_tfe22540-0.1.8/tfe22540/dMRI_metric_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/diamond_fractions.py` & `alcoholic_tfe22540-0.1.8/tfe22540/diamond_fractions.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/f0_f1_to_ftot.py` & `alcoholic_tfe22540-0.1.8/tfe22540/f0_f1_to_ftot.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/job_submission.py` & `alcoholic_tfe22540-0.1.8/tfe22540/job_submission.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/moyenne_ROI_v2.py` & `alcoholic_tfe22540-0.1.8/tfe22540/moyenne_ROI_v2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/moyenne_par_ROI.py` & `alcoholic_tfe22540-0.1.8/tfe22540/moyenne_par_ROI.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/opening_closing.py` & `alcoholic_tfe22540-0.1.8/tfe22540/opening_closing.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/perso_path.py` & `alcoholic_tfe22540-0.1.8/tfe22540/perso_path.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/plot_functions.py` & `alcoholic_tfe22540-0.1.8/tfe22540/plot_functions.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/preprocessing.py` & `alcoholic_tfe22540-0.1.8/tfe22540/preprocessing.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/registration.py` & `alcoholic_tfe22540-0.1.8/tfe22540/registration.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/ttest.py` & `alcoholic_tfe22540-0.1.8/tfe22540/ttest.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/useful_fct.py` & `alcoholic_tfe22540-0.1.8/tfe22540/useful_fct.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.7/tfe22540/volumes_zones.py` & `alcoholic_tfe22540-0.1.8/tfe22540/volumes_zones.py`

 * *Files identical despite different names*

