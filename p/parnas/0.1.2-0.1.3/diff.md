# Comparing `tmp/parnas-0.1.2.tar.gz` & `tmp/parnas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/parnas-0.1.2.tar", last modified: Thu Dec 22 18:12:23 2022, max compression
+gzip compressed data, was "dist/parnas-0.1.3.tar", last modified: Sun Jul  9 22:17:21 2023, max compression
```

## Comparing `parnas-0.1.2.tar` & `parnas-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2022-12-22 18:12:23.795814 parnas-0.1.2/
--rwxr-xr-x   0 alexey.markin (1295527787) 1161554559     1124 2022-07-03 20:26:04.000000 parnas-0.1.2/LICENSE
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    12434 2022-12-22 18:12:23.795005 parnas-0.1.2/PKG-INFO
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    10609 2022-12-22 17:41:58.000000 parnas-0.1.2/README.md
-drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2022-12-22 18:12:23.781568 parnas-0.1.2/parnas/
--rw-r--r--   0 alexey.markin (1295527787) 1161554559       59 2022-05-04 18:28:10.000000 parnas-0.1.2/parnas/__init__.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     9496 2022-07-04 20:18:19.000000 parnas-0.1.2/parnas/cli.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     1347 2022-05-04 18:28:10.000000 parnas-0.1.2/parnas/logging.py
-drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2022-12-22 18:12:23.794149 parnas-0.1.2/parnas/medoids/
--rw-r--r--   0 alexey.markin (1295527787) 1161554559      220 2022-05-02 15:58:42.000000 parnas-0.1.2/parnas/medoids/__init__.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    28484 2022-12-22 17:41:58.000000 parnas-0.1.2/parnas/medoids/fast_pmedian_finder.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     1021 2022-02-10 18:39:40.000000 parnas-0.1.2/parnas/medoids/input.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     6769 2022-12-22 17:41:58.000000 parnas-0.1.2/parnas/medoids/medoid_utils.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    15239 2022-02-10 18:39:40.000000 parnas-0.1.2/parnas/medoids/pmedian_finder.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     3745 2022-02-10 18:39:40.000000 parnas-0.1.2/parnas/medoids/pmedian_utils.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    13742 2022-02-10 18:39:40.000000 parnas-0.1.2/parnas/medoids/tree_coverage.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     1455 2022-02-10 18:39:40.000000 parnas-0.1.2/parnas/medoids/tree_indexer.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     4023 2022-07-04 20:18:19.000000 parnas-0.1.2/parnas/medoids/tree_medoids.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    16534 2022-12-22 17:41:58.000000 parnas-0.1.2/parnas/options.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559       22 2022-12-22 18:03:06.000000 parnas-0.1.2/parnas/version.py
-drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2022-12-22 18:12:23.786727 parnas-0.1.2/parnas.egg-info/
--rw-r--r--   0 alexey.markin (1295527787) 1161554559    12434 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/PKG-INFO
--rw-r--r--   0 alexey.markin (1295527787) 1161554559      584 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/SOURCES.txt
--rw-r--r--   0 alexey.markin (1295527787) 1161554559        1 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/dependency_links.txt
--rw-r--r--   0 alexey.markin (1295527787) 1161554559       54 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/entry_points.txt
--rw-r--r--   0 alexey.markin (1295527787) 1161554559       86 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/requires.txt
--rw-r--r--   0 alexey.markin (1295527787) 1161554559        7 2022-12-22 18:12:23.000000 parnas-0.1.2/parnas.egg-info/top_level.txt
--rwxr-xr-x   0 alexey.markin (1295527787) 1161554559      134 2022-05-04 18:28:10.000000 parnas-0.1.2/parnas.py
--rw-r--r--   0 alexey.markin (1295527787) 1161554559       38 2022-12-22 18:12:23.795999 parnas-0.1.2/setup.cfg
--rw-r--r--   0 alexey.markin (1295527787) 1161554559     1266 2022-10-03 12:57:38.000000 parnas-0.1.2/setup.py
+drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2023-07-09 22:17:21.228000 parnas-0.1.3/
+-rwxr-xr-x   0 alexey.markin (1295527787) 1161554559     1124 2022-07-03 20:26:04.000000 parnas-0.1.3/LICENSE
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    14594 2023-07-09 22:17:21.227378 parnas-0.1.3/PKG-INFO
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    12454 2023-07-09 22:05:35.000000 parnas-0.1.3/README.md
+drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2023-07-09 22:17:21.208296 parnas-0.1.3/parnas/
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559       59 2022-05-04 18:28:10.000000 parnas-0.1.3/parnas/__init__.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     9496 2022-07-04 20:18:19.000000 parnas-0.1.3/parnas/cli.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     1347 2022-05-04 18:28:10.000000 parnas-0.1.3/parnas/logging.py
+drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2023-07-09 22:17:21.225938 parnas-0.1.3/parnas/medoids/
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559      220 2022-05-02 15:58:42.000000 parnas-0.1.3/parnas/medoids/__init__.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    28484 2022-12-22 17:41:58.000000 parnas-0.1.3/parnas/medoids/fast_pmedian_finder.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     1021 2022-02-10 18:39:40.000000 parnas-0.1.3/parnas/medoids/input.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     6769 2022-12-22 17:41:58.000000 parnas-0.1.3/parnas/medoids/medoid_utils.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    15239 2022-02-10 18:39:40.000000 parnas-0.1.3/parnas/medoids/pmedian_finder.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     3745 2022-02-10 18:39:40.000000 parnas-0.1.3/parnas/medoids/pmedian_utils.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    13742 2022-02-10 18:39:40.000000 parnas-0.1.3/parnas/medoids/tree_coverage.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     1455 2022-02-10 18:39:40.000000 parnas-0.1.3/parnas/medoids/tree_indexer.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     4023 2022-07-04 20:18:19.000000 parnas-0.1.3/parnas/medoids/tree_medoids.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    16697 2023-07-09 22:02:50.000000 parnas-0.1.3/parnas/options.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559       22 2023-07-09 22:02:50.000000 parnas-0.1.3/parnas/version.py
+drwxr-xr-x   0 alexey.markin (1295527787) 1161554559        0 2023-07-09 22:17:21.213037 parnas-0.1.3/parnas.egg-info/
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559    14594 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/PKG-INFO
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559      584 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559        1 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559       54 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/entry_points.txt
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559       87 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/requires.txt
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559        7 2023-07-09 22:17:21.000000 parnas-0.1.3/parnas.egg-info/top_level.txt
+-rwxr-xr-x   0 alexey.markin (1295527787) 1161554559      134 2022-05-04 18:28:10.000000 parnas-0.1.3/parnas.py
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559       38 2023-07-09 22:17:21.228225 parnas-0.1.3/setup.cfg
+-rw-r--r--   0 alexey.markin (1295527787) 1161554559     1317 2023-07-09 22:02:50.000000 parnas-0.1.3/setup.py
```

### Comparing `parnas-0.1.2/LICENSE` & `parnas-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/PKG-INFO` & `parnas-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,86 @@
 Metadata-Version: 2.1
 Name: parnas
-Version: 0.1.2
+Version: 0.1.3
 Summary: Representative taxon sampling from phylogenetic trees
 Home-page: https://github.com/flu-crew/parnas
 Author: Alexey Markin, Sanket Wagle, Siddhant Grover
 Author-email: alex.markin57@gmail.com
 License: MIT
 Description: ## PARNAS ##
+        **If you use PARNAS, please cite it as**</br>
+        *Markin, A., Wagle, S., Grover, S., Baker, A.L.V., Eulenstein, O. and Anderson, T.K. PARNAS: Objectively Selecting the Most Representative Taxa on a Phylogeny. Systematic Biology, 2023; syad028 [doi: 10.1093/sysbio/syad028](https://doi.org/10.1093/sysbio/syad028).*
+        
         PARNAS identifies taxa that best represent diversity on a phylogenetic tree
         and can be used to
         - Select most representative taxa
         - Downsample a large phylogeny while optimally preserving the underlying diversity
         - Reduce redundancy among genetic/genomic sequences
         - Identify key diversity groups on a phylogeny
         
-        PARNAS solves urgent needs in virology/microbiology, such as
+        PARNAS solves needs in virology/microbiology, such as
         - Objectively finding representative strains for in-depth analyses (phenotypic characterization, Bayesian inference, etc.)
         - Objective and flexible vaccine strain selection
         
         PARNAS can take into account previously used representatives and a wide range of user's constraints.
         Additionally, PARNAS is flexible in allowing
-        arbitrary weighing of taxa, e.g., based on predicted fitness/antigenic drift. Finally, PARNAS allows you to fine-tune 
+        arbitrary weighing of taxa, e.g., based on predicted fitness/antigenic drift. Finally, PARNAS allows you to fine-tune
         representation definition with a user-defined coverage radius.
         
         
         Alternative methods currently exist to select taxa on phylogenetic trees (ADCL), or to reduce the number of taxa in a phylogeny (Treemer).
-        PARNAS is faster and more versatile than [ADCL](https://matsen.github.io/pplacer/generated_rst/rppr_min_adcl_tree.html#rppr-min-adcl-tree) by Matsen et al. (Systematic Biology 2013). 
-        Similarly, PARNAS is faster than [Treemmer](https://github.com/fmenardo/Treemmer) (Menardo et al., BMC Bioinformatics 2018), 
+        PARNAS is faster and more versatile than [ADCL](https://matsen.github.io/pplacer/generated_rst/rppr_min_adcl_tree.html#rppr-min-adcl-tree) by Matsen et al. (Systematic Biology 2013).
+        Similarly, PARNAS is faster than [Treemmer](https://github.com/fmenardo/Treemmer) (Menardo et al., BMC Bioinformatics 2018),
         and our objective allows for reproducible and interpretable selections that are optimally representative.
         
-        **If you use PARNAS, please cite it as**</br>
-        *Markin, A., Wagle, S., Grover, S., Baker, A.L.V., Eulenstein, O. and Anderson, T.K., 2022. PARNAS: Objectively Selecting the Most Representative Taxa on a Phylogeny. bioRxiv.*
+        
         
         ### Installation ###
         PARNAS is available in PyPi and can be installed as
         `pip install parnas`. Note that PARNAS requires Python 3.7 or higher.
         
         PARNAS depends on dendropy and Biopython for phylogenetic and MSA manipulations, numpy and numba for just-in-time compilation of the critical algorithms into machine code, and (optionally) phylo-treetime to infer ancestral substitutions along tree edges. These dependencies will be installed automatically.
         
         
         Alternatively, to install PARNAS, clone or download this project and run
         `python setup.py install`.
         ## Tutorial ##
         
-        We use a human H1N1 (pdm09) dataset with HA sequences collected in 2020, downloaded from [IRD](fludb.org), for this tutorial.
+        PARNAS has the following two main use-cases.
+        1. [Optimal downsampling](#optimal-downsampling-of-large-trees)
+        2. [Selecting best representatives](#selecting-best-representatives)
+        
+        ### Optimal downsampling of large trees ###
+        PARNAS lets you downsample a large phylogeny, while preserving all the diversity up to a user-specified threshold.
+        
+        In particular, if you have a threshold parameter (e.g., 1% sequence divergence on a tree) PARNAS selects **the smallest** subset of taxa so that all other taxa are within that threshold distance to a representative.
+        
+        
+        The typical application of this feature is downscaling large densely-sampled trees.
+        In this example we will use a (human) H1N1pdm influenza A dataset with 12,000 taxa.
+        We optimally downsample it while preserving all diversity up to 99.5% sequence similarity, as follows:
+        
+        `parnas -t genbank_H1N1pdm_USA.rooted.tre --cover --radius 0.005 --subtree H1N1pdm.r005.tre`
+        
+        This results in a tree with only 443 taxa! Note that 0.005 distance on a maximum likelihood phylogeny serves here as a proxy for the 0.5% sequence divergence. A downsampled tree will be saved to a new `H1N1pdm.r005.tre` file.
+        The initial 12,000 taxa tree (`genbank_H1N1pdm_USA.rooted.tre`) can be found in the tutorial [folder](tutorial/H1N1pdm_2020.zip).
+        
+        <center>
+        <img src="tutorial/figures/H1N1pdm-downsampling-300.png">
+        <!-- <object data="tutorial/figures/H1N1pdm-downsampling.pdf" type="application/pdf">
+            <embed src="tutorial/figures/H1N1pdm-downsampling.pdf">
+                <p>This browser does not support PDFs. You can view the trees <a href="tutorial/figures/H1N1pdm-downsampling.pdf">here</a>.</p>
+            </embed>
+        </object> -->
+        </center>
+        
+        Below we discuss how PARNAS selects most representative taxa.
+        
+        ### Selecting best representatives ###
+        We use a human H1N1pdm dataset with HA sequences collected in 2020, downloaded from [IRD](fludb.org), for this tutorial.
         The alignment and an inferred rooted tree can be found in the tutorial [folder](tutorial/H1N1pdm_2020.zip).
         
         The basic usage of PARNAS is to find a fixed number of representative taxa, as follows:<br>
         `parnas -t H1N1_human_2020_IRD.rooted.tre -n 3 --color "H1N1_parnas_n3.tre"`<br>
         PARNAS will identify 3 best representative strains and save a colored tree to H1N1_parnas_n3.tre.
         Opening this tree in FigTree, will show the representatives and their respective clusters of strains with different colors. Below is the `H1N1_parnas_n3.tre` output tree, when opened in FigTree. Each color corresponds to one PARNAS-selected representative and the area of the tree it represents.
         
@@ -144,11 +177,12 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `parnas-0.1.2/README.md` & `parnas-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,664 +1,779 @@
-00000000: 2323 2050 4152 4e41 5320 2323 0a50 4152  ## PARNAS ##.PAR
-00000010: 4e41 5320 6964 656e 7469 6669 6573 2074  NAS identifies t
-00000020: 6178 6120 7468 6174 2062 6573 7420 7265  axa that best re
-00000030: 7072 6573 656e 7420 6469 7665 7273 6974  present diversit
-00000040: 7920 6f6e 2061 2070 6879 6c6f 6765 6e65  y on a phylogene
-00000050: 7469 6320 7472 6565 0a61 6e64 2063 616e  tic tree.and can
-00000060: 2062 6520 7573 6564 2074 6f0a 2d20 5365   be used to.- Se
-00000070: 6c65 6374 206d 6f73 7420 7265 7072 6573  lect most repres
-00000080: 656e 7461 7469 7665 2074 6178 610a 2d20  entative taxa.- 
-00000090: 446f 776e 7361 6d70 6c65 2061 206c 6172  Downsample a lar
-000000a0: 6765 2070 6879 6c6f 6765 6e79 2077 6869  ge phylogeny whi
-000000b0: 6c65 206f 7074 696d 616c 6c79 2070 7265  le optimally pre
-000000c0: 7365 7276 696e 6720 7468 6520 756e 6465  serving the unde
-000000d0: 726c 7969 6e67 2064 6976 6572 7369 7479  rlying diversity
-000000e0: 0a2d 2052 6564 7563 6520 7265 6475 6e64  .- Reduce redund
-000000f0: 616e 6379 2061 6d6f 6e67 2067 656e 6574  ancy among genet
-00000100: 6963 2f67 656e 6f6d 6963 2073 6571 7565  ic/genomic seque
-00000110: 6e63 6573 0a2d 2049 6465 6e74 6966 7920  nces.- Identify 
-00000120: 6b65 7920 6469 7665 7273 6974 7920 6772  key diversity gr
-00000130: 6f75 7073 206f 6e20 6120 7068 796c 6f67  oups on a phylog
-00000140: 656e 790a 0a50 4152 4e41 5320 736f 6c76  eny..PARNAS solv
-00000150: 6573 2075 7267 656e 7420 6e65 6564 7320  es urgent needs 
-00000160: 696e 2076 6972 6f6c 6f67 792f 6d69 6372  in virology/micr
-00000170: 6f62 696f 6c6f 6779 2c20 7375 6368 2061  obiology, such a
-00000180: 730a 2d20 4f62 6a65 6374 6976 656c 7920  s.- Objectively 
-00000190: 6669 6e64 696e 6720 7265 7072 6573 656e  finding represen
-000001a0: 7461 7469 7665 2073 7472 6169 6e73 2066  tative strains f
-000001b0: 6f72 2069 6e2d 6465 7074 6820 616e 616c  or in-depth anal
-000001c0: 7973 6573 2028 7068 656e 6f74 7970 6963  yses (phenotypic
-000001d0: 2063 6861 7261 6374 6572 697a 6174 696f   characterizatio
-000001e0: 6e2c 2042 6179 6573 6961 6e20 696e 6665  n, Bayesian infe
-000001f0: 7265 6e63 652c 2065 7463 2e29 0a2d 204f  rence, etc.).- O
-00000200: 626a 6563 7469 7665 2061 6e64 2066 6c65  bjective and fle
-00000210: 7869 626c 6520 7661 6363 696e 6520 7374  xible vaccine st
-00000220: 7261 696e 2073 656c 6563 7469 6f6e 0a0a  rain selection..
-00000230: 5041 524e 4153 2063 616e 2074 616b 6520  PARNAS can take 
-00000240: 696e 746f 2061 6363 6f75 6e74 2070 7265  into account pre
-00000250: 7669 6f75 736c 7920 7573 6564 2072 6570  viously used rep
-00000260: 7265 7365 6e74 6174 6976 6573 2061 6e64  resentatives and
-00000270: 2061 2077 6964 6520 7261 6e67 6520 6f66   a wide range of
-00000280: 2075 7365 7227 7320 636f 6e73 7472 6169   user's constrai
-00000290: 6e74 732e 0a41 6464 6974 696f 6e61 6c6c  nts..Additionall
-000002a0: 792c 2050 4152 4e41 5320 6973 2066 6c65  y, PARNAS is fle
-000002b0: 7869 626c 6520 696e 2061 6c6c 6f77 696e  xible in allowin
-000002c0: 670a 6172 6269 7472 6172 7920 7765 6967  g.arbitrary weig
-000002d0: 6869 6e67 206f 6620 7461 7861 2c20 652e  hing of taxa, e.
-000002e0: 672e 2c20 6261 7365 6420 6f6e 2070 7265  g., based on pre
-000002f0: 6469 6374 6564 2066 6974 6e65 7373 2f61  dicted fitness/a
-00000300: 6e74 6967 656e 6963 2064 7269 6674 2e20  ntigenic drift. 
-00000310: 4669 6e61 6c6c 792c 2050 4152 4e41 5320  Finally, PARNAS 
-00000320: 616c 6c6f 7773 2079 6f75 2074 6f20 6669  allows you to fi
-00000330: 6e65 2d74 756e 6520 0a72 6570 7265 7365  ne-tune .represe
-00000340: 6e74 6174 696f 6e20 6465 6669 6e69 7469  ntation definiti
-00000350: 6f6e 2077 6974 6820 6120 7573 6572 2d64  on with a user-d
-00000360: 6566 696e 6564 2063 6f76 6572 6167 6520  efined coverage 
-00000370: 7261 6469 7573 2e0a 0a0a 416c 7465 726e  radius....Altern
-00000380: 6174 6976 6520 6d65 7468 6f64 7320 6375  ative methods cu
-00000390: 7272 656e 746c 7920 6578 6973 7420 746f  rrently exist to
-000003a0: 2073 656c 6563 7420 7461 7861 206f 6e20   select taxa on 
-000003b0: 7068 796c 6f67 656e 6574 6963 2074 7265  phylogenetic tre
-000003c0: 6573 2028 4144 434c 292c 206f 7220 746f  es (ADCL), or to
-000003d0: 2072 6564 7563 6520 7468 6520 6e75 6d62   reduce the numb
-000003e0: 6572 206f 6620 7461 7861 2069 6e20 6120  er of taxa in a 
-000003f0: 7068 796c 6f67 656e 7920 2854 7265 656d  phylogeny (Treem
-00000400: 6572 292e 0a50 4152 4e41 5320 6973 2066  er)..PARNAS is f
-00000410: 6173 7465 7220 616e 6420 6d6f 7265 2076  aster and more v
-00000420: 6572 7361 7469 6c65 2074 6861 6e20 5b41  ersatile than [A
-00000430: 4443 4c5d 2868 7474 7073 3a2f 2f6d 6174  DCL](https://mat
-00000440: 7365 6e2e 6769 7468 7562 2e69 6f2f 7070  sen.github.io/pp
-00000450: 6c61 6365 722f 6765 6e65 7261 7465 645f  lacer/generated_
-00000460: 7273 742f 7270 7072 5f6d 696e 5f61 6463  rst/rppr_min_adc
-00000470: 6c5f 7472 6565 2e68 746d 6c23 7270 7072  l_tree.html#rppr
-00000480: 2d6d 696e 2d61 6463 6c2d 7472 6565 2920  -min-adcl-tree) 
-00000490: 6279 204d 6174 7365 6e20 6574 2061 6c2e  by Matsen et al.
-000004a0: 2028 5379 7374 656d 6174 6963 2042 696f   (Systematic Bio
-000004b0: 6c6f 6779 2032 3031 3329 2e20 0a53 696d  logy 2013). .Sim
-000004c0: 696c 6172 6c79 2c20 5041 524e 4153 2069  ilarly, PARNAS i
-000004d0: 7320 6661 7374 6572 2074 6861 6e20 5b54  s faster than [T
-000004e0: 7265 656d 6d65 725d 2868 7474 7073 3a2f  reemmer](https:/
-000004f0: 2f67 6974 6875 622e 636f 6d2f 666d 656e  /github.com/fmen
-00000500: 6172 646f 2f54 7265 656d 6d65 7229 2028  ardo/Treemmer) (
-00000510: 4d65 6e61 7264 6f20 6574 2061 6c2e 2c20  Menardo et al., 
-00000520: 424d 4320 4269 6f69 6e66 6f72 6d61 7469  BMC Bioinformati
-00000530: 6373 2032 3031 3829 2c20 0a61 6e64 206f  cs 2018), .and o
-00000540: 7572 206f 626a 6563 7469 7665 2061 6c6c  ur objective all
-00000550: 6f77 7320 666f 7220 7265 7072 6f64 7563  ows for reproduc
-00000560: 6962 6c65 2061 6e64 2069 6e74 6572 7072  ible and interpr
-00000570: 6574 6162 6c65 2073 656c 6563 7469 6f6e  etable selection
-00000580: 7320 7468 6174 2061 7265 206f 7074 696d  s that are optim
-00000590: 616c 6c79 2072 6570 7265 7365 6e74 6174  ally representat
-000005a0: 6976 652e 0a0a 2a2a 4966 2079 6f75 2075  ive...**If you u
-000005b0: 7365 2050 4152 4e41 532c 2070 6c65 6173  se PARNAS, pleas
-000005c0: 6520 6369 7465 2069 7420 6173 2a2a 3c2f  e cite it as**</
-000005d0: 6272 3e0a 2a4d 6172 6b69 6e2c 2041 2e2c  br>.*Markin, A.,
-000005e0: 2057 6167 6c65 2c20 532e 2c20 4772 6f76   Wagle, S., Grov
-000005f0: 6572 2c20 532e 2c20 4261 6b65 722c 2041  er, S., Baker, A
-00000600: 2e4c 2e56 2e2c 2045 756c 656e 7374 6569  .L.V., Eulenstei
-00000610: 6e2c 204f 2e20 616e 6420 416e 6465 7273  n, O. and Anders
-00000620: 6f6e 2c20 542e 4b2e 2c20 3230 3232 2e20  on, T.K., 2022. 
-00000630: 5041 524e 4153 3a20 4f62 6a65 6374 6976  PARNAS: Objectiv
-00000640: 656c 7920 5365 6c65 6374 696e 6720 7468  ely Selecting th
-00000650: 6520 4d6f 7374 2052 6570 7265 7365 6e74  e Most Represent
-00000660: 6174 6976 6520 5461 7861 206f 6e20 6120  ative Taxa on a 
-00000670: 5068 796c 6f67 656e 792e 2062 696f 5278  Phylogeny. bioRx
-00000680: 6976 2e2a 0a0a 2323 2320 496e 7374 616c  iv.*..### Instal
-00000690: 6c61 7469 6f6e 2023 2323 0a50 4152 4e41  lation ###.PARNA
-000006a0: 5320 6973 2061 7661 696c 6162 6c65 2069  S is available i
-000006b0: 6e20 5079 5069 2061 6e64 2063 616e 2062  n PyPi and can b
-000006c0: 6520 696e 7374 616c 6c65 6420 6173 0a60  e installed as.`
-000006d0: 7069 7020 696e 7374 616c 6c20 7061 726e  pip install parn
-000006e0: 6173 602e 204e 6f74 6520 7468 6174 2050  as`. Note that P
-000006f0: 4152 4e41 5320 7265 7175 6972 6573 2050  ARNAS requires P
-00000700: 7974 686f 6e20 332e 3720 6f72 2068 6967  ython 3.7 or hig
-00000710: 6865 722e 0a0a 5041 524e 4153 2064 6570  her...PARNAS dep
-00000720: 656e 6473 206f 6e20 6465 6e64 726f 7079  ends on dendropy
-00000730: 2061 6e64 2042 696f 7079 7468 6f6e 2066   and Biopython f
-00000740: 6f72 2070 6879 6c6f 6765 6e65 7469 6320  or phylogenetic 
-00000750: 616e 6420 4d53 4120 6d61 6e69 7075 6c61  and MSA manipula
-00000760: 7469 6f6e 732c 206e 756d 7079 2061 6e64  tions, numpy and
-00000770: 206e 756d 6261 2066 6f72 206a 7573 742d   numba for just-
-00000780: 696e 2d74 696d 6520 636f 6d70 696c 6174  in-time compilat
-00000790: 696f 6e20 6f66 2074 6865 2063 7269 7469  ion of the criti
-000007a0: 6361 6c20 616c 676f 7269 7468 6d73 2069  cal algorithms i
-000007b0: 6e74 6f20 6d61 6368 696e 6520 636f 6465  nto machine code
-000007c0: 2c20 616e 6420 286f 7074 696f 6e61 6c6c  , and (optionall
-000007d0: 7929 2070 6879 6c6f 2d74 7265 6574 696d  y) phylo-treetim
-000007e0: 6520 746f 2069 6e66 6572 2061 6e63 6573  e to infer ances
-000007f0: 7472 616c 2073 7562 7374 6974 7574 696f  tral substitutio
-00000800: 6e73 2061 6c6f 6e67 2074 7265 6520 6564  ns along tree ed
-00000810: 6765 732e 2054 6865 7365 2064 6570 656e  ges. These depen
-00000820: 6465 6e63 6965 7320 7769 6c6c 2062 6520  dencies will be 
-00000830: 696e 7374 616c 6c65 6420 6175 746f 6d61  installed automa
-00000840: 7469 6361 6c6c 792e 0a0a 0a41 6c74 6572  tically....Alter
-00000850: 6e61 7469 7665 6c79 2c20 746f 2069 6e73  natively, to ins
-00000860: 7461 6c6c 2050 4152 4e41 532c 2063 6c6f  tall PARNAS, clo
-00000870: 6e65 206f 7220 646f 776e 6c6f 6164 2074  ne or download t
-00000880: 6869 7320 7072 6f6a 6563 7420 616e 6420  his project and 
-00000890: 7275 6e0a 6070 7974 686f 6e20 7365 7475  run.`python setu
-000008a0: 702e 7079 2069 6e73 7461 6c6c 602e 0a23  p.py install`..#
-000008b0: 2320 5475 746f 7269 616c 2023 230a 0a57  # Tutorial ##..W
-000008c0: 6520 7573 6520 6120 6875 6d61 6e20 4831  e use a human H1
-000008d0: 4e31 2028 7064 6d30 3929 2064 6174 6173  N1 (pdm09) datas
-000008e0: 6574 2077 6974 6820 4841 2073 6571 7565  et with HA seque
-000008f0: 6e63 6573 2063 6f6c 6c65 6374 6564 2069  nces collected i
-00000900: 6e20 3230 3230 2c20 646f 776e 6c6f 6164  n 2020, download
-00000910: 6564 2066 726f 6d20 5b49 5244 5d28 666c  ed from [IRD](fl
-00000920: 7564 622e 6f72 6729 2c20 666f 7220 7468  udb.org), for th
-00000930: 6973 2074 7574 6f72 6961 6c2e 0a54 6865  is tutorial..The
-00000940: 2061 6c69 676e 6d65 6e74 2061 6e64 2061   alignment and a
-00000950: 6e20 696e 6665 7272 6564 2072 6f6f 7465  n inferred roote
-00000960: 6420 7472 6565 2063 616e 2062 6520 666f  d tree can be fo
-00000970: 756e 6420 696e 2074 6865 2074 7574 6f72  und in the tutor
-00000980: 6961 6c20 5b66 6f6c 6465 725d 2874 7574  ial [folder](tut
-00000990: 6f72 6961 6c2f 4831 4e31 7064 6d5f 3230  orial/H1N1pdm_20
-000009a0: 3230 2e7a 6970 292e 0a0a 5468 6520 6261  20.zip)...The ba
-000009b0: 7369 6320 7573 6167 6520 6f66 2050 4152  sic usage of PAR
-000009c0: 4e41 5320 6973 2074 6f20 6669 6e64 2061  NAS is to find a
-000009d0: 2066 6978 6564 206e 756d 6265 7220 6f66   fixed number of
-000009e0: 2072 6570 7265 7365 6e74 6174 6976 6520   representative 
-000009f0: 7461 7861 2c20 6173 2066 6f6c 6c6f 7773  taxa, as follows
-00000a00: 3a3c 6272 3e0a 6070 6172 6e61 7320 2d74  :<br>.`parnas -t
-00000a10: 2048 314e 315f 6875 6d61 6e5f 3230 3230   H1N1_human_2020
-00000a20: 5f49 5244 2e72 6f6f 7465 642e 7472 6520  _IRD.rooted.tre 
-00000a30: 2d6e 2033 202d 2d63 6f6c 6f72 2022 4831  -n 3 --color "H1
-00000a40: 4e31 5f70 6172 6e61 735f 6e33 2e74 7265  N1_parnas_n3.tre
-00000a50: 2260 3c62 723e 0a50 4152 4e41 5320 7769  "`<br>.PARNAS wi
-00000a60: 6c6c 2069 6465 6e74 6966 7920 3320 6265  ll identify 3 be
-00000a70: 7374 2072 6570 7265 7365 6e74 6174 6976  st representativ
-00000a80: 6520 7374 7261 696e 7320 616e 6420 7361  e strains and sa
-00000a90: 7665 2061 2063 6f6c 6f72 6564 2074 7265  ve a colored tre
-00000aa0: 6520 746f 2048 314e 315f 7061 726e 6173  e to H1N1_parnas
-00000ab0: 5f6e 332e 7472 652e 0a4f 7065 6e69 6e67  _n3.tre..Opening
-00000ac0: 2074 6869 7320 7472 6565 2069 6e20 4669   this tree in Fi
-00000ad0: 6754 7265 652c 2077 696c 6c20 7368 6f77  gTree, will show
-00000ae0: 2074 6865 2072 6570 7265 7365 6e74 6174   the representat
-00000af0: 6976 6573 2061 6e64 2074 6865 6972 2072  ives and their r
-00000b00: 6573 7065 6374 6976 6520 636c 7573 7465  espective cluste
-00000b10: 7273 206f 6620 7374 7261 696e 7320 7769  rs of strains wi
-00000b20: 7468 2064 6966 6665 7265 6e74 2063 6f6c  th different col
-00000b30: 6f72 732e 2042 656c 6f77 2069 7320 7468  ors. Below is th
-00000b40: 6520 6048 314e 315f 7061 726e 6173 5f6e  e `H1N1_parnas_n
-00000b50: 332e 7472 6560 206f 7574 7075 7420 7472  3.tre` output tr
-00000b60: 6565 2c20 7768 656e 206f 7065 6e65 6420  ee, when opened 
-00000b70: 696e 2046 6967 5472 6565 2e20 4561 6368  in FigTree. Each
-00000b80: 2063 6f6c 6f72 2063 6f72 7265 7370 6f6e   color correspon
-00000b90: 6473 2074 6f20 6f6e 6520 5041 524e 4153  ds to one PARNAS
-00000ba0: 2d73 656c 6563 7465 6420 7265 7072 6573  -selected repres
-00000bb0: 656e 7461 7469 7665 2061 6e64 2074 6865  entative and the
-00000bc0: 2061 7265 6120 6f66 2074 6865 2074 7265   area of the tre
-00000bd0: 6520 6974 2072 6570 7265 7365 6e74 732e  e it represents.
-00000be0: 0a0a 3c63 656e 7465 723e 0a3c 696d 6720  ..<center>.<img 
-00000bf0: 7372 633d 2274 7574 6f72 6961 6c2f 6669  src="tutorial/fi
-00000c00: 6775 7265 732f 4831 4e31 5f70 6172 6e61  gures/H1N1_parna
-00000c10: 735f 6e33 2e70 6e67 223e 0a3c 2f63 656e  s_n3.png">.</cen
-00000c20: 7465 723e 0a0a 4164 6469 7469 6f6e 616c  ter>..Additional
-00000c30: 6c79 2c20 696e 2074 6865 206f 7574 7075  ly, in the outpu
-00000c40: 7420 5041 524e 4153 2073 7065 6369 6669  t PARNAS specifi
-00000c50: 6573 2074 6865 2061 6d6f 756e 7420 6f66  es the amount of
-00000c60: 206f 7665 7261 6c6c 2064 6976 6572 7369   overall diversi
-00000c70: 7479 2063 6f76 6572 6564 2062 7920 7468  ty covered by th
-00000c80: 6520 6368 6f73 656e 2072 6570 7265 7365  e chosen represe
-00000c90: 6e74 6174 6976 6573 2c20 7768 6963 6820  ntatives, which 
-00000ca0: 6973 2034 3325 2066 6f72 206f 7572 2064  is 43% for our d
-00000cb0: 6174 6173 6574 2e0a 0a23 2323 2320 4465  ataset...#### De
-00000cc0: 7465 726d 696e 696e 6720 7468 6520 7269  termining the ri
-00000cd0: 6768 7420 6e75 6d62 6572 206f 6620 7265  ght number of re
-00000ce0: 7072 6573 656e 7461 7469 7665 7320 2323  presentatives ##
-00000cf0: 2323 0a54 6865 2022 6469 7665 7273 6974  ##.The "diversit
-00000d00: 7920 636f 7665 7265 6422 206d 6574 7269  y covered" metri
-00000d10: 6320 6361 6c63 756c 6174 6564 2062 7920  c calculated by 
-00000d20: 5041 524e 4153 2069 7320 6120 7573 6566  PARNAS is a usef
-00000d30: 756c 2074 6f6f 6c20 746f 2064 6574 6572  ul tool to deter
-00000d40: 6d69 6e65 2068 6f77 206d 616e 7920 7265  mine how many re
-00000d50: 7072 6573 656e 7461 7469 7665 7320 6973  presentatives is
-00000d60: 2073 7566 6669 6369 656e 742e 0a54 6f20   sufficient..To 
-00000d70: 6669 6e64 2074 6865 2061 6d6f 756e 7420  find the amount 
-00000d80: 6f66 2064 6976 6572 7369 7479 2063 6f76  of diversity cov
-00000d90: 6572 6564 2062 7920 6469 6666 6572 656e  ered by differen
-00000da0: 7420 6e75 6d62 6572 7320 6f66 2072 6570  t numbers of rep
-00000db0: 7265 7365 6e74 6174 6976 6573 2c20 796f  resentatives, yo
-00000dc0: 7520 6361 6e20 6368 6f6f 7365 2061 206c  u can choose a l
-00000dd0: 6172 6765 2065 6e6f 7567 6820 6e2c 2065  arge enough n, e
-00000de0: 2e67 2e2c 206e 3d32 302c 2061 6e64 2072  .g., n=20, and r
-00000df0: 756e 3c62 723e 0a60 7061 726e 6173 202d  un<br>.`parnas -
-00000e00: 7420 4831 4e31 5f68 756d 616e 5f32 3032  t H1N1_human_202
-00000e10: 305f 4952 442e 726f 6f74 6564 2e74 7265  0_IRD.rooted.tre
-00000e20: 202d 6e20 3230 202d 2d64 6976 6572 7369   -n 20 --diversi
-00000e30: 7479 2022 6469 7665 7273 6974 795f 7363  ty "diversity_sc
-00000e40: 6f72 6573 2e63 7376 2260 3c62 723e 0a54  ores.csv"`<br>.T
-00000e50: 6869 7320 636f 6d6d 616e 6420 7769 6c6c  his command will
-00000e60: 2073 6176 6520 6120 4353 5620 6669 6c65   save a CSV file
-00000e70: 2077 6974 6820 6f70 7469 6d61 6c20 6469   with optimal di
-00000e80: 7665 7273 6974 7920 7363 6f72 6573 2066  versity scores f
-00000e90: 6f72 206e 2062 6574 7765 656e 2032 2061  or n between 2 a
-00000ea0: 6e64 2032 302e 2046 6f72 206f 7572 2064  nd 20. For our d
-00000eb0: 6174 6173 6574 2c20 6974 2073 686f 7773  ataset, it shows
-00000ec0: 2074 6861 7420 6f6e 6c79 2036 2072 6570   that only 6 rep
-00000ed0: 7265 7365 6e74 6174 6976 6520 7374 7261  resentative stra
-00000ee0: 696e 7320 6172 6520 6e65 6564 6564 2074  ins are needed t
-00000ef0: 6f20 636f 7665 7220 6f76 6572 2036 3025  o cover over 60%
-00000f00: 206f 6620 7468 6520 6f76 6572 616c 6c20   of the overall 
-00000f10: 6469 7665 7273 6974 792e 204f 7065 6e69  diversity. Openi
-00000f20: 6e67 2074 6865 2043 5356 2066 696c 6520  ng the CSV file 
-00000f30: 696e 2045 7863 656c 2f4e 756d 6265 7273  in Excel/Numbers
-00000f40: 2c20 6f6e 6520 6361 6e20 7468 656e 2063  , one can then c
-00000f50: 6f6e 7374 7275 6374 2074 6865 2066 6f6c  onstruct the fol
-00000f60: 6c6f 7769 6e67 2067 7261 7068 2074 6f20  lowing graph to 
-00000f70: 6265 7474 6572 2076 6973 7561 6c69 7a65  better visualize
-00000f80: 2074 6865 2064 6174 612e 0a0a 3c63 656e   the data...<cen
-00000f90: 7465 723e 0a3c 696d 6720 7372 633d 2274  ter>.<img src="t
-00000fa0: 7574 6f72 6961 6c2f 6669 6775 7265 732f  utorial/figures/
-00000fb0: 6469 7665 7273 6974 795f 636f 7665 7265  diversity_covere
-00000fc0: 642e 706e 6722 2077 6964 7468 3d22 3435  d.png" width="45
-00000fd0: 3070 7822 3e0a 3c2f 6365 6e74 6572 3e0a  0px">.</center>.
-00000fe0: 0a23 2323 2320 5573 696e 6720 7072 696f  .#### Using prio
-00000ff0: 7220 7265 7072 6573 656e 7461 7469 7665  r representative
-00001000: 7320 2323 2323 0a49 7420 6f66 7465 6e20  s ####.It often 
-00001010: 6d61 7920 6265 2075 7365 6675 6c20 746f  may be useful to
-00001020: 2066 696e 6420 6e65 7720 7265 7072 6573   find new repres
-00001030: 656e 7461 7469 7665 732c 2077 6869 6c65  entatives, while
-00001040: 2073 7065 6369 6679 696e 6720 7468 6520   specifying the 
-00001050: 7072 6576 696f 7573 2074 6178 612f 7374  previous taxa/st
-00001060: 7261 696e 7320 7468 6174 2077 6572 6520  rains that were 
-00001070: 7472 6561 7465 6420 6173 2072 6570 7265  treated as repre
-00001080: 7365 6e74 6174 6976 6573 2e20 496e 206f  sentatives. In o
-00001090: 7572 2048 314e 3120 6461 7461 7365 742c  ur H1N1 dataset,
-000010a0: 2077 6520 696e 636c 7564 6564 2074 776f   we included two
-000010b0: 206c 6174 6573 7420 4831 4e31 2076 6163   latest H1N1 vac
-000010c0: 6369 6e65 2073 7472 6169 6e73 2c20 412f  cine strains, A/
-000010d0: 5769 7363 6f6e 7369 6e2f 3538 382f 3230  Wisconsin/588/20
-000010e0: 3139 2061 6e64 2041 2f48 6177 6169 692f  19 and A/Hawaii/
-000010f0: 3730 2f32 3031 392e 2055 7369 6e67 2050  70/2019. Using P
-00001100: 4152 4e41 5320 7765 2063 616e 2066 6978  ARNAS we can fix
-00001110: 2074 6865 7365 2074 776f 2073 7472 6169   these two strai
-00001120: 6e73 2061 7320 2770 7269 6f72 2720 7265  ns as 'prior' re
-00001130: 7072 6573 656e 7461 7469 7665 7320 616e  presentatives an
-00001140: 6420 6669 6e64 206e 6577 2072 6570 7265  d find new repre
-00001150: 7365 6e74 6174 6976 6573 2c20 736f 2074  sentatives, so t
-00001160: 6861 7420 6f6c 6420 616e 6420 6e65 7720  hat old and new 
-00001170: 7265 7072 6573 656e 7461 7469 7665 7320  representatives 
-00001180: 776f 726b 206f 7074 696d 616c 6c79 2074  work optimally t
-00001190: 6f67 6574 6865 722e 2057 6520 7573 6520  ogether. We use 
-000011a0: 602d 2d70 7269 6f72 6020 6f70 7469 6f6e  `--prior` option
-000011b0: 2074 6f20 6e6f 7469 6679 2050 4152 4e41   to notify PARNA
-000011c0: 5320 6f66 2074 6865 2074 776f 2076 6163  S of the two vac
-000011d0: 6369 6e65 2073 7472 6169 6e73 2062 7920  cine strains by 
-000011e0: 7370 6563 6966 7969 6e67 2061 2072 6567  specifying a reg
-000011f0: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-00001200: 6d61 7463 6869 6e67 2074 6865 6972 206e  matching their n
-00001210: 616d 6573 2069 6e20 6f75 7220 6461 7461  ames in our data
-00001220: 7365 7420 2877 6869 6368 2073 7461 7274  set (which start
-00001230: 2077 6974 6820 2256 6163 6369 6e65 7c22   with "Vaccine|"
-00001240: 293a 3c62 723e 0a60 7061 726e 6173 202d  ):<br>.`parnas -
-00001250: 7420 4831 4e31 5f68 756d 616e 5f32 3032  t H1N1_human_202
-00001260: 305f 4952 442e 726f 6f74 6564 2e74 7265  0_IRD.rooted.tre
-00001270: 202d 6e20 3320 2d2d 7072 696f 7220 2256   -n 3 --prior "V
-00001280: 6163 6369 6e65 2e2a 2220 2d2d 636f 6c6f  accine.*" --colo
-00001290: 7220 2248 314e 315f 7061 726e 6173 5f6e  r "H1N1_parnas_n
-000012a0: 335f 7661 6363 696e 6573 2e74 7265 2260  3_vaccines.tre"`
-000012b0: 3c62 723e 0a54 6865 2072 6573 756c 7420  <br>.The result 
-000012c0: 6973 2073 686f 776e 2069 6e20 6120 7472  is shown in a tr
-000012d0: 6565 2062 656c 6f77 2e20 5041 524e 4153  ee below. PARNAS
-000012e0: 2063 6f6c 6f72 7320 7468 6520 7072 696f   colors the prio
-000012f0: 7220 7265 7072 6573 656e 7461 7469 7665  r representative
-00001300: 7320 616e 6420 7468 6520 7265 7370 6563  s and the respec
-00001310: 7469 7665 2070 6172 7473 206f 6620 7468  tive parts of th
-00001320: 6520 7472 6565 2069 6e20 7265 642e 0a0a  e tree in red...
-00001330: 3c63 656e 7465 723e 0a3c 696d 6720 7372  <center>.<img sr
-00001340: 633d 2274 7574 6f72 6961 6c2f 6669 6775  c="tutorial/figu
-00001350: 7265 732f 4831 4e31 5f70 6172 6e61 735f  res/H1N1_parnas_
-00001360: 6e33 5f76 6163 6369 6e65 732e 706e 6722  n3_vaccines.png"
-00001370: 3e0a 3c2f 6365 6e74 6572 3e0a 0a23 2323  >.</center>..###
-00001380: 2320 5370 6563 6966 7969 6e67 2061 2063  # Specifying a c
-00001390: 6f76 6572 6167 6520 7261 6469 7573 2023  overage radius #
-000013a0: 2323 230a 596f 7520 6361 6e20 6e6f 7469  ###.You can noti
-000013b0: 6679 2050 4152 4e41 5320 7468 6174 2061  fy PARNAS that a
-000013c0: 2073 696e 676c 6520 7461 786f 6e20 2763   single taxon 'c
-000013d0: 6f76 6572 7327 206f 7468 6572 2074 6178  overs' other tax
-000013e0: 6120 7769 7468 696e 2061 2066 6978 6564  a within a fixed
-000013f0: 2072 6164 6975 7320 2875 7369 6e67 2060   radius (using `
-00001400: 2d2d 7261 6469 7573 6020 6f70 7469 6f6e  --radius` option
-00001410: 292e 2050 4152 4e41 5320 7769 6c6c 2074  ). PARNAS will t
-00001420: 6865 6e20 6669 6e64 2072 6570 7265 7365  hen find represe
-00001430: 6e74 6174 6976 6573 2c20 7768 6963 6820  ntatives, which 
-00001440: 746f 6765 7468 6572 2063 6f76 6572 2061  together cover a
-00001450: 7320 6d75 6368 2064 6976 6572 7369 7479  s much diversity
-00001460: 2061 7320 706f 7373 6962 6c65 2e20 416c   as possible. Al
-00001470: 7465 726e 6174 6976 656c 792c 2050 4152  ternatively, PAR
-00001480: 4e41 5320 6361 6e20 6669 6e64 2074 6865  NAS can find the
-00001490: 206d 696e 696d 756d 206e 756d 6265 7220   minimum number 
-000014a0: 6f66 2072 6570 7265 7365 6e74 6174 6976  of representativ
-000014b0: 6573 2074 6861 7420 6a6f 696e 746c 7920  es that jointly 
-000014c0: 636f 7665 7220 2a61 6c6c 2a20 6469 7665  cover *all* dive
-000014d0: 7273 6974 7920 6f6e 2074 6865 2074 7265  rsity on the tre
-000014e0: 6520 2860 2d2d 636f 7665 7260 206f 7074  e (`--cover` opt
-000014f0: 696f 6e29 2e20 5468 6973 2066 6561 7475  ion). This featu
-00001500: 7265 2063 616e 2062 6520 7573 6564 2074  re can be used t
-00001510: 6f20 6f70 7469 6d61 6c6c 7920 7265 6475  o optimally redu
-00001520: 6365 2074 6865 2072 6564 756e 6461 6e63  ce the redundanc
-00001530: 7920 696e 2079 6f75 7220 6461 7461 7365  y in your datase
-00001540: 742e 204d 6f72 656f 7665 722c 2074 6869  t. Moreover, thi
-00001550: 7320 6665 6174 7572 6520 7761 7320 6d6f  s feature was mo
-00001560: 7469 7661 7465 6420 6279 2061 7070 6c69  tivated by appli
-00001570: 6361 7469 6f6e 7320 696e 2076 6972 6f6c  cations in virol
-00001580: 6f67 792c 2077 6865 7265 2065 766f 6c75  ogy, where evolu
-00001590: 7469 6f6e 6172 7920 6469 7374 616e 6365  tionary distance
-000015a0: 206f 6674 656e 2063 6f72 7265 6c61 7465   often correlate
-000015b0: 7320 7769 7468 2061 6e74 6967 656e 6963  s with antigenic
-000015c0: 2064 7269 6674 2e20 466f 7220 6578 616d   drift. For exam
-000015d0: 706c 652c 2069 6e20 7377 696e 6520 696e  ple, in swine in
-000015e0: 666c 7565 6e7a 6120 4120 7669 7275 7320  fluenza A virus 
-000015f0: 7265 7365 6172 6368 2c20 3525 2028 616d  research, 5% (am
-00001600: 696e 6f20 6163 6964 2920 6469 7665 7267  ino acid) diverg
-00001610: 656e 6365 2062 6574 7765 656e 2048 4120  ence between HA 
-00001620: 7365 7175 656e 6365 7320 6973 2063 6f6e  sequences is con
-00001630: 7369 6465 7265 6420 6120 636f 7272 656c  sidered a correl
-00001640: 6174 6520 6f66 206c 6f73 7320 696e 2063  ate of loss in c
-00001650: 726f 7373 2d72 6561 6374 6976 6974 7920  ross-reactivity 
-00001660: 6265 7477 6565 6e20 7374 7261 696e 732e  between strains.
-00001670: 2054 6865 7265 666f 7265 2c20 7370 6563   Therefore, spec
-00001680: 6966 7969 6e67 2061 2072 6164 6975 7320  ifying a radius 
-00001690: 6f6e 2061 2074 7265 6520 636f 7272 6573  on a tree corres
-000016a0: 706f 6e64 696e 6720 746f 207e 3425 2073  ponding to ~4% s
-000016b0: 6571 7565 6e63 6520 6469 7665 7267 656e  equence divergen
-000016c0: 6365 2c20 6361 6e20 6865 6c70 2069 6465  ce, can help ide
-000016d0: 6e74 6966 7920 676f 6f64 2076 6163 6369  ntify good vacci
-000016e0: 6e65 2063 616e 6469 6461 7465 732e 0a0a  ne candidates...
-000016f0: 546f 2066 7572 7468 6572 2066 6163 696c  To further facil
-00001700: 6974 6174 6520 7468 6973 2070 726f 6365  itate this proce
-00001710: 7373 2c20 5041 524e 4153 2063 616e 2074  ss, PARNAS can t
-00001720: 616b 6520 616d 696e 6f20 6163 6964 2073  ake amino acid s
-00001730: 6571 7565 6e63 6520 616c 6967 6e6d 656e  equence alignmen
-00001740: 7420 616e 6420 7061 7373 2069 7420 746f  t and pass it to
-00001750: 205b 5472 6565 5469 6d65 5d28 6874 7470   [TreeTime](http
-00001760: 733a 2f2f 7472 6565 7469 6d65 2e72 6561  s://treetime.rea
-00001770: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001780: 6174 6573 742f 2920 746f 2066 696e 6420  atest/) to find 
-00001790: 616e 6365 7374 7261 6c20 4141 2073 7562  ancestral AA sub
-000017a0: 7374 6974 7574 696f 6e73 2061 6c6f 6e67  stitutions along
-000017b0: 2074 6865 2074 7265 6520 6564 6765 732e   the tree edges.
-000017c0: 2049 7420 7769 6c6c 2074 6865 6e20 7265   It will then re
-000017d0: 2d73 6361 6c65 2074 6865 2074 7265 652c  -scale the tree,
-000017e0: 2073 6f20 7468 6174 2065 6467 6520 6c65   so that edge le
-000017f0: 6e67 7468 7320 7769 6c6c 2072 6566 6c65  ngths will refle
-00001800: 6374 2074 6865 206e 756d 6265 7220 6f66  ct the number of
-00001810: 2073 7562 7374 6974 7574 696f 6e73 2061   substitutions a
-00001820: 6c6f 6e67 2074 6861 7420 6564 6765 2c20  long that edge, 
-00001830: 7768 6963 6820 7769 6c6c 2068 656c 7020  which will help 
-00001840: 7370 6563 6966 7920 6120 3425 2064 6976  specify a 4% div
-00001850: 6572 6765 6e63 6520 7261 6469 7573 2069  ergence radius i
-00001860: 6e20 7465 726d 7320 6f66 2074 6865 2023  n terms of the #
-00001870: 206f 6620 616d 696e 6f20 6163 6964 2073   of amino acid s
-00001880: 7562 7374 6974 7574 696f 6e73 2e0a 0a60  ubstitutions...`
-00001890: 7061 726e 6173 202d 7420 4831 4e31 5f68  parnas -t H1N1_h
-000018a0: 756d 616e 5f32 3032 305f 4952 442e 726f  uman_2020_IRD.ro
-000018b0: 6f74 6564 2e74 7265 202d 2d63 6f76 6572  oted.tre --cover
-000018c0: 202d 2d74 6872 6573 686f 6c64 2039 3620   --threshold 96 
-000018d0: 2d2d 6161 2048 314e 315f 6875 6d61 6e5f  --aa H1N1_human_
-000018e0: 3230 3230 5f49 5244 2e68 6131 2e61 6c6e  2020_IRD.ha1.aln
-000018f0: 202d 2d63 6f6c 6f72 2022 7061 726e 6173   --color "parnas
-00001900: 5f39 3663 6f76 6572 6167 652e 7472 6522  _96coverage.tre"
-00001910: 600a 0a49 6e20 7468 6520 6162 6f76 6520  `..In the above 
-00001920: 636f 6d6d 616e 6420 7765 2070 6173 7320  command we pass 
-00001930: 7468 6520 4141 2061 6c69 676e 6d65 6e74  the AA alignment
-00001940: 206f 6620 4841 3120 7365 7175 656e 6365   of HA1 sequence
-00001950: 7320 6672 6f6d 206f 7572 2064 6174 6173  s from our datas
-00001960: 6574 2077 6974 6820 7468 6520 602d 2d61  et with the `--a
-00001970: 6160 206f 7074 696f 6e2c 2061 6e64 2073  a` option, and s
-00001980: 7065 6369 6679 2074 6865 2039 3625 2074  pecify the 96% t
-00001990: 6872 6573 686f 6c64 2028 692e 652e 2c20  hreshold (i.e., 
-000019a0: 3425 2073 6571 7565 6e63 6520 6469 7665  4% sequence dive
-000019b0: 7267 656e 6365 292e 204e 6f74 6520 7468  rgence). Note th
-000019c0: 6174 2060 2d2d 7468 7265 7368 6f6c 6460  at `--threshold`
-000019d0: 2077 6f72 6b73 2061 7320 6120 7375 6273   works as a subs
-000019e0: 7469 7475 7465 2066 6f72 2060 2d2d 7261  titute for `--ra
-000019f0: 6469 7573 602c 2077 6865 6e20 796f 7520  dius`, when you 
-00001a00: 776f 756c 6420 6c69 6b65 2050 4152 4e41  would like PARNA
-00001a10: 5320 746f 2075 7365 2074 6865 2061 6c69  S to use the ali
-00001a20: 676e 6d65 6e74 2069 6e66 6f72 6d61 7469  gnment informati
-00001a30: 6f6e 2061 6e64 2072 652d 7363 616c 6520  on and re-scale 
-00001a40: 7468 6520 7472 6565 2e20 5275 6e6e 696e  the tree. Runnin
-00001a50: 6720 7468 6973 2063 6f6d 6d61 6e64 2077  g this command w
-00001a60: 696c 6c20 7368 6f77 2074 6861 7420 6120  ill show that a 
-00001a70: 7369 6e67 6c65 2073 7472 6169 6e20 2841  single strain (A
-00001a80: 2f57 6973 636f 6e73 696e 2f33 322f 3230  /Wisconsin/32/20
-00001a90: 3230 2920 6973 2073 7566 6669 6369 656e  20) is sufficien
-00001aa0: 7420 746f 2063 6f76 6572 2061 6c6c 2064  t to cover all d
-00001ab0: 6976 6572 7369 7479 206f 6e20 6f75 7220  iversity on our 
-00001ac0: 7472 6565 2e0a 0a4e 6578 742c 2077 6520  tree...Next, we 
-00001ad0: 7573 6520 6120 6d6f 7265 2072 6573 7472  use a more restr
-00001ae0: 6963 7469 7665 2074 6872 6573 686f 6c64  ictive threshold
-00001af0: 206f 6620 3937 2520 616e 6420 616c 736f   of 97% and also
-00001b00: 2061 6464 2074 6865 2076 6163 6369 6e65   add the vaccine
-00001b10: 2073 7472 6169 6e73 2061 7320 7468 6520   strains as the 
-00001b20: 7072 696f 7220 7265 7072 6573 656e 7461  prior representa
-00001b30: 7469 7665 732e 2054 6869 7320 7761 7920  tives. This way 
-00001b40: 5041 524e 4153 2063 616e 2069 6e64 6963  PARNAS can indic
-00001b50: 6174 6520 7468 6520 6172 6561 7320 6f66  ate the areas of
-00001b60: 2074 6865 2074 7265 652c 2077 6869 6368   the tree, which
-00001b70: 2061 7265 206e 6f74 2063 6f76 6572 6564   are not covered
-00001b80: 2062 7920 7468 6520 7661 6363 696e 6520   by the vaccine 
-00001b90: 7374 7261 696e 7320 616e 6420 7375 6767  strains and sugg
-00001ba0: 6573 7420 6e65 7720 7265 7072 6573 656e  est new represen
-00001bb0: 7461 7469 7665 7320 746f 2063 6f6d 706c  tatives to compl
-00001bc0: 656d 656e 7420 7468 6520 7661 6363 696e  ement the vaccin
-00001bd0: 6520 7374 7261 696e 732e 0a0a 6070 6172  e strains...`par
-00001be0: 6e61 7320 2d74 2048 314e 315f 6875 6d61  nas -t H1N1_huma
-00001bf0: 6e5f 3230 3230 5f49 5244 2e72 6f6f 7465  n_2020_IRD.roote
-00001c00: 642e 7472 6520 2d2d 636f 7665 7220 2d2d  d.tre --cover --
-00001c10: 7468 7265 7368 6f6c 6420 3937 202d 2d61  threshold 97 --a
-00001c20: 6120 4831 4e31 5f68 756d 616e 5f32 3032  a H1N1_human_202
-00001c30: 305f 4952 442e 6861 312e 616c 6e20 2d2d  0_IRD.ha1.aln --
-00001c40: 636f 6c6f 7220 2270 6172 6e61 735f 3937  color "parnas_97
-00001c50: 636f 7665 7261 6765 5f76 6163 6369 6e65  coverage_vaccine
-00001c60: 732e 7472 6522 202d 2d70 7269 6f72 2022  s.tre" --prior "
-00001c70: 5661 6363 696e 652e 2a22 600a 0a4f 7065  Vaccine.*"`..Ope
-00001c80: 6e69 6e67 2060 7061 726e 6173 5f39 3763  ning `parnas_97c
-00001c90: 6f76 6572 6167 655f 7661 6363 696e 6573  overage_vaccines
-00001ca0: 2e74 7265 6020 696e 2046 6967 5472 6565  .tre` in FigTree
-00001cb0: 2077 696c 6c20 7368 6f77 2075 7320 7468   will show us th
-00001cc0: 6174 2074 6865 7265 2061 7265 2074 776f  at there are two
-00001cd0: 2063 6c61 6465 7320 696e 2074 6865 2074   clades in the t
-00001ce0: 7265 652c 2077 6869 6368 2061 7265 206e  ree, which are n
-00001cf0: 6f74 2063 6f76 6572 6564 2062 7920 7661  ot covered by va
-00001d00: 6363 696e 6520 7374 7261 696e 7320 2874  ccine strains (t
-00001d10: 6865 2067 7265 656e 2061 6e64 2062 6c75  he green and blu
-00001d20: 6520 636c 6164 6573 292e 204e 6f74 6520  e clades). Note 
-00001d30: 7468 6174 2074 6865 2074 7265 6520 7761  that the tree wa
-00001d40: 7320 7265 2d73 6361 6c65 6420 6279 2050  s re-scaled by P
-00001d50: 4152 4e41 532e 0a0a 3c63 656e 7465 723e  ARNAS...<center>
-00001d60: 0a3c 696d 6720 7372 633d 2274 7574 6f72  .<img src="tutor
-00001d70: 6961 6c2f 6669 6775 7265 732f 4831 4e31  ial/figures/H1N1
-00001d80: 5f70 6172 6e61 735f 3937 636f 7665 7261  _parnas_97covera
-00001d90: 6765 5f76 6163 6369 6e65 732e 706e 6722  ge_vaccines.png"
-00001da0: 3e0a 3c2f 6365 6e74 6572 3e0a 0a23 2323  >.</center>..###
-00001db0: 2320 4f74 6865 7220 6675 6e63 7469 6f6e  # Other function
-00001dc0: 616c 6974 7920 2323 2323 0a2d 2053 7065  ality ####.- Spe
-00001dd0: 6369 6679 2077 6569 6768 7473 2066 6f72  cify weights for
-00001de0: 2074 6178 612c 2073 6f20 7468 6174 2074   taxa, so that t
-00001df0: 6178 612f 7374 7261 696e 7320 7769 7468  axa/strains with
-00001e00: 206c 6172 6765 7220 7765 6967 6874 7320   larger weights 
-00001e10: 6172 6520 6265 7474 6572 2072 6570 7265  are better repre
-00001e20: 7365 6e74 6564 2e0a 2d20 466c 6578 6962  sented..- Flexib
-00001e30: 6c79 2065 7863 6c75 6465 2074 6178 6120  ly exclude taxa 
-00001e40: 746f 2065 6974 6865 7220 6675 6c6c 7920  to either fully 
-00001e50: 6967 6e6f 7265 2074 6865 6d20 6f72 2074  ignore them or t
-00001e60: 6f20 6e6f 7420 636f 6e73 6964 6572 2074  o not consider t
-00001e70: 6865 6d20 6173 2070 6f74 656e 7469 616c  hem as potential
-00001e80: 2072 6570 7265 7365 6e74 6174 6976 6573   representatives
-00001e90: 2e0a 0a23 2320 5041 524e 4153 2075 7361  ...## PARNAS usa
-00001ea0: 6765 2023 230a 0a60 7061 726e 6173 202d  ge ##..`parnas -
-00001eb0: 7420 5452 4545 205b 2d6e 2053 414d 504c  t TREE [-n SAMPL
-00001ec0: 4553 5d20 5b6f 7468 6572 206f 7074 696f  ES] [other optio
-00001ed0: 6e73 5d60 0a0a 5468 6520 696e 7075 7420  ns]`..The input 
-00001ee0: 7472 6565 2073 686f 756c 6420 6265 2069  tree should be i
-00001ef0: 6e20 6e65 7875 7320 6f72 206e 6577 6963  n nexus or newic
-00001f00: 6b20 666f 726d 6174 2e0a 0a46 6f72 2061  k format...For a
-00001f10: 2064 6574 6169 6c65 6420 7265 6665 7265   detailed refere
-00001f20: 6e63 6520 6f6e 2050 4152 4e41 5320 6f70  nce on PARNAS op
-00001f30: 7469 6f6e 7320 7275 6e20 6070 6172 6e61  tions run `parna
-00001f40: 7320 2d68 6020 6f72 2073 6565 2062 656c  s -h` or see bel
-00001f50: 6f77 2e0a 0a2a 4765 6e65 7261 6c20 6f70  ow...*General op
-00001f60: 7469 6f6e 732a 0a0a 7c20 4f70 7469 6f6e  tions*..| Option
-00001f70: 207c 2044 6573 6372 6970 7469 6f6e 207c   | Description |
-00001f80: 0a7c 202d 2d2d 207c 202d 2d2d 207c 0a7c  .| --- | --- |.|
-00001f90: 2d2d 7261 6469 7573 207c 2053 7065 6369  --radius | Speci
-00001fa0: 6679 2061 2072 6164 6975 7320 2864 6973  fy a radius (dis
-00001fb0: 7461 6e63 6520 6f6e 2061 2074 7265 6529  tance on a tree)
-00001fc0: 2073 6f20 7468 6174 2065 7665 7279 2072   so that every r
-00001fd0: 6570 7265 7365 6e74 6174 6976 6520 636f  epresentative co
-00001fe0: 7665 7273 2061 6c6c 2064 6976 6572 7369  vers all diversi
-00001ff0: 7479 2077 6974 6869 6e20 7468 6174 2072  ty within that r
-00002000: 6164 6975 732e 2050 4152 4e41 5320 7769  adius. PARNAS wi
-00002010: 6c6c 2074 6865 6e20 6368 6f6f 7365 2072  ll then choose r
-00002020: 6570 7265 7365 6e74 6174 6976 6573 2074  epresentatives t
-00002030: 6861 7420 6f70 7469 6d61 6c6c 7920 636f  hat optimally co
-00002040: 7665 7220 6173 206d 7563 6820 6469 7665  ver as much dive
-00002050: 7273 6974 7920 6173 2070 6f73 7369 626c  rsity as possibl
-00002060: 6520 7c0a 7c20 2d2d 7072 696f 7220 7c20  e |.| --prior | 
-00002070: 5370 6563 6966 7920 7072 696f 7220 7265  Specify prior re
-00002080: 7072 6573 656e 7461 7469 7665 7320 7769  presentatives wi
-00002090: 7468 2061 2072 6567 6578 2e20 5041 524e  th a regex. PARN
-000020a0: 4153 2077 696c 6c20 7468 656e 2069 6465  AS will then ide
-000020b0: 6e74 6966 7920 7265 7072 6573 656e 7461  ntify representa
-000020c0: 7469 7665 7320 6f66 2027 6e65 7727 2064  tives of 'new' d
-000020d0: 6976 6572 7369 7479 207c 0a7c 202d 2d77  iversity |.| --w
-000020e0: 6569 6768 7473 207c 2041 6464 2061 2043  eights | Add a C
-000020f0: 5356 2066 696c 6520 7370 6563 6966 7969  SV file specifyi
-00002100: 6e67 2077 6569 6768 7473 2066 6f72 2073  ng weights for s
-00002110: 6f6d 6520 6f72 2061 6c6c 2074 6178 612f  ome or all taxa/
-00002120: 7374 7261 696e 7320 7c0a 7c20 2d2d 636f  strains |.| --co
-00002130: 7665 7220 7c20 496e 7374 6561 6420 6f66  ver | Instead of
-00002140: 2073 7065 6369 6679 696e 6720 7468 6520   specifying the 
-00002150: 6e75 6d62 6572 206f 6620 7265 7072 6573  number of repres
-00002160: 656e 7461 7469 7665 732c 2073 7065 6369  entatives, speci
-00002170: 6679 2074 6865 2072 6164 6975 7320 616e  fy the radius an
-00002180: 6420 5041 524e 4153 2077 696c 6c20 6669  d PARNAS will fi
-00002190: 6e64 2072 6570 7265 7365 6e74 6174 6976  nd representativ
-000021a0: 6520 7468 6174 2063 6f76 6572 2061 6c6c  e that cover all
-000021b0: 2064 6976 6572 7369 7479 206f 6e20 7468   diversity on th
-000021c0: 6520 7472 6565 207c 0a0a 2a4f 7574 7075  e tree |..*Outpu
-000021d0: 7420 6f70 7469 6f6e 7320 2863 6f6d 6269  t options (combi
-000021e0: 6e69 6e67 206f 7574 7075 7420 6f70 7469  ning output opti
-000021f0: 6f6e 7320 6973 2061 6c6c 6f77 6564 292a  ons is allowed)*
-00002200: 0a0a 7c20 4f70 7469 6f6e 207c 2044 6573  ..| Option | Des
-00002210: 6372 6970 7469 6f6e 207c 0a7c 202d 2d2d  cription |.| ---
-00002220: 207c 202d 2d2d 207c 0a7c 202d 2d63 6f6c   | --- |.| --col
-00002230: 6f72 207c 2053 7065 6369 6679 2061 6e20  or | Specify an 
-00002240: 6f75 7470 7574 2070 6174 682c 2077 6865  output path, whe
-00002250: 7265 2061 2063 6f6c 6f72 6564 2074 7265  re a colored tre
-00002260: 6520 7769 6c6c 2062 6520 7361 7665 642e  e will be saved.
-00002270: 2050 4152 4e41 5320 7769 6c6c 2068 6967   PARNAS will hig
-00002280: 686c 6967 6874 2074 6865 2063 686f 7365  hlight the chose
-00002290: 6e20 7265 7072 6573 656e 7461 7469 7665  n representative
-000022a0: 7320 616e 6420 636f 6c6f 722d 7061 7274  s and color-part
-000022b0: 6974 696f 6e20 7468 6520 7472 6565 2072  ition the tree r
-000022c0: 6573 7065 6374 6976 6520 746f 2074 6865  espective to the
-000022d0: 2072 6570 7265 7365 6e74 6174 6976 6573   representatives
-000022e0: 2e20 4966 2070 7269 6f72 2072 6570 7265  . If prior repre
-000022f0: 7365 6e74 6174 6976 6573 2061 7265 2073  sentatives are s
-00002300: 7065 6369 6669 6564 2c20 7468 6579 2028  pecified, they (
-00002310: 616e 6420 7468 6520 7375 6274 7265 6573  and the subtrees
-00002320: 2074 6865 7920 7265 7072 6573 656e 7429   they represent)
-00002330: 2077 696c 6c20 6265 2063 6f6c 6f72 6564   will be colored
-00002340: 2072 6564 2e7c 0a7c 202d 2d64 6976 6572   red.|.| --diver
-00002350: 7369 7479 207c 2053 7065 6369 6679 2061  sity | Specify a
-00002360: 6e20 6f75 7470 7574 2070 6174 682c 2077  n output path, w
-00002370: 6865 7265 2061 2043 5356 2077 696c 6c20  here a CSV will 
-00002380: 6265 2073 6176 6564 2077 6974 6820 6469  be saved with di
-00002390: 7665 7273 6974 7920 7363 6f72 6573 2066  versity scores f
-000023a0: 6f72 2061 6c6c 206b 2028 6e75 6d62 6572  or all k (number
-000023b0: 206f 6620 7265 7072 6573 656e 7461 7469   of representati
-000023c0: 7665 7329 2066 726f 6d20 3220 746f 206e  ves) from 2 to n
-000023d0: 2e20 4361 6e20 6265 2075 7365 6420 746f  . Can be used to
-000023e0: 2063 686f 6f73 6520 7468 6520 7269 6768   choose the righ
-000023f0: 7420 6e75 6d62 6572 206f 6620 7265 7072  t number of repr
-00002400: 6573 656e 7461 7469 7665 7320 666f 7220  esentatives for 
-00002410: 6120 6461 7461 7365 7420 7c0a 7c20 2d2d  a dataset |.| --
-00002420: 7375 6274 7265 6520 7c20 5370 6563 6966  subtree | Specif
-00002430: 7920 6120 7061 7468 2c20 7768 6572 6520  y a path, where 
-00002440: 6120 7375 6274 7265 6520 7769 7468 2074  a subtree with t
-00002450: 6865 2073 616d 706c 6564 2072 6570 7265  he sampled repre
-00002460: 7365 6e74 6174 6976 6573 2077 696c 6c20  sentatives will 
-00002470: 6265 2073 6176 6564 2028 696e 204e 4558  be saved (in NEX
-00002480: 5553 2066 6f72 6d61 7429 207c 0a0a 0a2a  US format) |...*
-00002490: 4f70 7469 6f6e 7320 746f 2065 7863 6c75  Options to exclu
-000024a0: 6465 2f63 6f6e 7374 7261 696e 2074 6178  de/constrain tax
-000024b0: 612a 0a0a 7c20 4f70 7469 6f6e 207c 2044  a*..| Option | D
-000024c0: 6573 6372 6970 7469 6f6e 207c 0a7c 202d  escription |.| -
-000024d0: 2d2d 207c 202d 2d2d 207c 0a7c 202d 2d65  -- | --- |.| --e
-000024e0: 7863 6c75 6465 2d72 6570 207c 2052 4547  xclude-rep | REG
-000024f0: 4558 2e20 4d61 7463 6869 6e67 2074 6178  EX. Matching tax
-00002500: 6120 7769 6c6c 206e 6f74 2062 6520 6368  a will not be ch
-00002510: 6f73 656e 2061 7320 7265 7072 6573 656e  osen as represen
-00002520: 7461 7469 7665 732c 2062 7574 2074 6865  tatives, but the
-00002530: 7920 7769 6c6c 2063 6f6e 7472 6962 7574  y will contribut
-00002540: 6520 746f 2074 6865 206f 626a 6563 7469  e to the objecti
-00002550: 7665 2066 756e 6374 696f 6e20 7c0a 7c20  ve function |.| 
-00002560: 2d2d 6578 636c 7564 652d 6f62 6a20 7c20  --exclude-obj | 
-00002570: 5245 4745 582e 204d 6174 6368 696e 6720  REGEX. Matching 
-00002580: 7461 7861 2063 616e 2062 6520 7365 6c65  taxa can be sele
-00002590: 6374 6564 2c20 6275 7420 7769 6c6c 206e  cted, but will n
-000025a0: 6f74 2063 6f6e 7472 6962 7574 6520 746f  ot contribute to
-000025b0: 2074 6865 206f 626a 6563 7469 7665 2066   the objective f
-000025c0: 756e 6374 696f 6e20 2874 6865 206f 7070  unction (the opp
-000025d0: 6f73 6974 6520 6f66 202d 2d65 7863 6c75  osite of --exclu
-000025e0: 6465 2d72 6570 2920 7c0a 7c20 2d2d 6578  de-rep) |.| --ex
-000025f0: 636c 7564 652d 6675 6c6c 7920 7c20 5245  clude-fully | RE
-00002600: 4745 582e 204d 6174 6368 696e 6720 7461  GEX. Matching ta
-00002610: 7861 2077 696c 6c20 6265 2063 6f6d 706c  xa will be compl
-00002620: 6574 656c 7920 6967 6e6f 7265 6420 6279  etely ignored by
-00002630: 2050 4152 4e41 5320 7c0a 7c20 2d2d 636f   PARNAS |.| --co
-00002640: 6e73 7472 6169 6e2d 6675 6c6c 7920 7c20  nstrain-fully | 
-00002650: 5245 4745 582e 204f 7070 6f73 6974 6520  REGEX. Opposite 
-00002660: 746f 2027 2d2d 6578 636c 7564 652d 6675  to '--exclude-fu
-00002670: 6c6c 7927 2c20 692e 652e 2c20 6f6e 6c79  lly', i.e., only
-00002680: 2074 6865 206d 6174 6368 696e 6720 7461   the matching ta
-00002690: 7861 2077 696c 6c20 6265 2063 6f6e 7369  xa will be consi
-000026a0: 6465 7265 6420 6279 2050 4152 4e41 5320  dered by PARNAS 
-000026b0: 7c0a 0a2a 4f70 7469 6f6e 7320 746f 2063  |..*Options to c
-000026c0: 6f6e 7472 6f6c 2073 6571 7565 6e63 6520  ontrol sequence 
-000026d0: 6469 7665 7267 656e 6365 2a0a 0a7c 204f  divergence*..| O
-000026e0: 7074 696f 6e20 7c20 4465 7363 7269 7074  ption | Descript
-000026f0: 696f 6e20 7c0a 7c20 2d2d 2d20 7c20 2d2d  ion |.| --- | --
-00002700: 2d20 7c0a 7c20 2d2d 7468 7265 7368 6f6c  - |.| --threshol
-00002710: 6420 7c20 4e75 6d62 6572 2062 6574 7765  d | Number betwe
-00002720: 656e 2030 2061 6e64 2031 3030 2e20 5468  en 0 and 100. Th
-00002730: 6520 7365 7175 656e 6365 2073 696d 696c  e sequence simil
-00002740: 6172 6974 7920 7468 7265 7368 6f6c 6420  arity threshold 
-00002750: 7468 6174 2077 6f72 6b73 2061 7320 2d2d  that works as --
-00002760: 7261 6469 7573 2e20 466f 7220 6578 616d  radius. For exam
-00002770: 706c 652c 2022 3935 2220 7769 6c6c 2069  ple, "95" will i
-00002780: 6d70 6c79 2074 6861 7420 6561 6368 2072  mply that each r
-00002790: 6570 7265 7365 6e74 6174 6976 6520 636f  epresentative co
-000027a0: 7665 7273 2061 6c6c 206c 6561 7665 7320  vers all leaves 
-000027b0: 7769 7468 696e 2035 2520 6469 7665 7267  within 5% diverg
-000027c0: 656e 6365 206f 6e20 7468 6520 7472 6565  ence on the tree
-000027d0: 2e20 546f 2061 6363 6f75 6e74 2066 6f72  . To account for
-000027e0: 2073 6571 7565 6e63 6520 6469 7665 7267   sequence diverg
-000027f0: 656e 6365 2c20 5041 524e 4153 2077 696c  ence, PARNAS wil
-00002800: 6c20 7275 6e20 5472 6565 5469 6d65 2074  l run TreeTime t
-00002810: 6f20 696e 6665 7220 616e 6365 7374 7261  o infer ancestra
-00002820: 6c20 7375 6273 7469 7475 7469 6f6e 7320  l substitutions 
-00002830: 616c 6f6e 6720 7468 6520 7472 6565 2065  along the tree e
-00002840: 6467 6573 2061 6e64 2072 652d 7765 6967  dges and re-weig
-00002850: 6820 7468 6520 6564 6765 7320 6261 7365  h the edges base
-00002860: 6420 6f6e 2074 6865 206e 756d 6265 7220  d on the number 
-00002870: 6f66 2073 7562 7374 6974 7574 696f 6e73  of substitutions
-00002880: 206f 6e20 7468 656d 2e20 4120 7365 7175   on them. A sequ
-00002890: 656e 6365 2061 6c69 676e 6d65 6e74 2028  ence alignment (
-000028a0: 2d2d 6e74 206f 7220 2d2d 6161 2920 6d75  --nt or --aa) mu
-000028b0: 7374 2062 6520 7370 6563 6966 6965 6420  st be specified 
-000028c0: 7769 7468 2074 6869 7320 6f70 7469 6f6e  with this option
-000028d0: 207c 0a7c 202d 2d6e 7420 7c20 5061 7468   |.| --nt | Path
-000028e0: 2074 6f20 6e75 636c 656f 7469 6465 2073   to nucleotide s
-000028f0: 6571 7565 6e63 6520 616c 6967 6e6d 656e  equence alignmen
-00002900: 7420 6173 736f 6369 6174 6564 2077 6974  t associated wit
-00002910: 6820 7468 6520 7472 6565 2074 6970 7320  h the tree tips 
-00002920: 7c0a 7c20 2d2d 6161 207c 2050 6174 6820  |.| --aa | Path 
-00002930: 746f 2061 6d69 6e6f 2061 6369 6420 7365  to amino acid se
-00002940: 7175 656e 6365 2061 6c69 676e 6d65 6e74  quence alignment
-00002950: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00002960: 2074 6865 2074 7265 6520 7469 7073 207c   the tree tips |
-00002970: 0a                                       .
+00000000: 2323 2050 4152 4e41 5320 2323 0a2a 2a49  ## PARNAS ##.**I
+00000010: 6620 796f 7520 7573 6520 5041 524e 4153  f you use PARNAS
+00000020: 2c20 706c 6561 7365 2063 6974 6520 6974  , please cite it
+00000030: 2061 732a 2a3c 2f62 723e 0a2a 4d61 726b   as**</br>.*Mark
+00000040: 696e 2c20 412e 2c20 5761 676c 652c 2053  in, A., Wagle, S
+00000050: 2e2c 2047 726f 7665 722c 2053 2e2c 2042  ., Grover, S., B
+00000060: 616b 6572 2c20 412e 4c2e 562e 2c20 4575  aker, A.L.V., Eu
+00000070: 6c65 6e73 7465 696e 2c20 4f2e 2061 6e64  lenstein, O. and
+00000080: 2041 6e64 6572 736f 6e2c 2054 2e4b 2e20   Anderson, T.K. 
+00000090: 5041 524e 4153 3a20 4f62 6a65 6374 6976  PARNAS: Objectiv
+000000a0: 656c 7920 5365 6c65 6374 696e 6720 7468  ely Selecting th
+000000b0: 6520 4d6f 7374 2052 6570 7265 7365 6e74  e Most Represent
+000000c0: 6174 6976 6520 5461 7861 206f 6e20 6120  ative Taxa on a 
+000000d0: 5068 796c 6f67 656e 792e 2053 7973 7465  Phylogeny. Syste
+000000e0: 6d61 7469 6320 4269 6f6c 6f67 792c 2032  matic Biology, 2
+000000f0: 3032 333b 2073 7961 6430 3238 205b 646f  023; syad028 [do
+00000100: 693a 2031 302e 3130 3933 2f73 7973 6269  i: 10.1093/sysbi
+00000110: 6f2f 7379 6164 3032 385d 2868 7474 7073  o/syad028](https
+00000120: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
+00000130: 3933 2f73 7973 6269 6f2f 7379 6164 3032  93/sysbio/syad02
+00000140: 3829 2e2a 0a0a 5041 524e 4153 2069 6465  8).*..PARNAS ide
+00000150: 6e74 6966 6965 7320 7461 7861 2074 6861  ntifies taxa tha
+00000160: 7420 6265 7374 2072 6570 7265 7365 6e74  t best represent
+00000170: 2064 6976 6572 7369 7479 206f 6e20 6120   diversity on a 
+00000180: 7068 796c 6f67 656e 6574 6963 2074 7265  phylogenetic tre
+00000190: 650a 616e 6420 6361 6e20 6265 2075 7365  e.and can be use
+000001a0: 6420 746f 0a2d 2053 656c 6563 7420 6d6f  d to.- Select mo
+000001b0: 7374 2072 6570 7265 7365 6e74 6174 6976  st representativ
+000001c0: 6520 7461 7861 0a2d 2044 6f77 6e73 616d  e taxa.- Downsam
+000001d0: 706c 6520 6120 6c61 7267 6520 7068 796c  ple a large phyl
+000001e0: 6f67 656e 7920 7768 696c 6520 6f70 7469  ogeny while opti
+000001f0: 6d61 6c6c 7920 7072 6573 6572 7669 6e67  mally preserving
+00000200: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+00000210: 6469 7665 7273 6974 790a 2d20 5265 6475  diversity.- Redu
+00000220: 6365 2072 6564 756e 6461 6e63 7920 616d  ce redundancy am
+00000230: 6f6e 6720 6765 6e65 7469 632f 6765 6e6f  ong genetic/geno
+00000240: 6d69 6320 7365 7175 656e 6365 730a 2d20  mic sequences.- 
+00000250: 4964 656e 7469 6679 206b 6579 2064 6976  Identify key div
+00000260: 6572 7369 7479 2067 726f 7570 7320 6f6e  ersity groups on
+00000270: 2061 2070 6879 6c6f 6765 6e79 0a0a 5041   a phylogeny..PA
+00000280: 524e 4153 2073 6f6c 7665 7320 6e65 6564  RNAS solves need
+00000290: 7320 696e 2076 6972 6f6c 6f67 792f 6d69  s in virology/mi
+000002a0: 6372 6f62 696f 6c6f 6779 2c20 7375 6368  crobiology, such
+000002b0: 2061 730a 2d20 4f62 6a65 6374 6976 656c   as.- Objectivel
+000002c0: 7920 6669 6e64 696e 6720 7265 7072 6573  y finding repres
+000002d0: 656e 7461 7469 7665 2073 7472 6169 6e73  entative strains
+000002e0: 2066 6f72 2069 6e2d 6465 7074 6820 616e   for in-depth an
+000002f0: 616c 7973 6573 2028 7068 656e 6f74 7970  alyses (phenotyp
+00000300: 6963 2063 6861 7261 6374 6572 697a 6174  ic characterizat
+00000310: 696f 6e2c 2042 6179 6573 6961 6e20 696e  ion, Bayesian in
+00000320: 6665 7265 6e63 652c 2065 7463 2e29 0a2d  ference, etc.).-
+00000330: 204f 626a 6563 7469 7665 2061 6e64 2066   Objective and f
+00000340: 6c65 7869 626c 6520 7661 6363 696e 6520  lexible vaccine 
+00000350: 7374 7261 696e 2073 656c 6563 7469 6f6e  strain selection
+00000360: 0a0a 5041 524e 4153 2063 616e 2074 616b  ..PARNAS can tak
+00000370: 6520 696e 746f 2061 6363 6f75 6e74 2070  e into account p
+00000380: 7265 7669 6f75 736c 7920 7573 6564 2072  reviously used r
+00000390: 6570 7265 7365 6e74 6174 6976 6573 2061  epresentatives a
+000003a0: 6e64 2061 2077 6964 6520 7261 6e67 6520  nd a wide range 
+000003b0: 6f66 2075 7365 7227 7320 636f 6e73 7472  of user's constr
+000003c0: 6169 6e74 732e 0a41 6464 6974 696f 6e61  aints..Additiona
+000003d0: 6c6c 792c 2050 4152 4e41 5320 6973 2066  lly, PARNAS is f
+000003e0: 6c65 7869 626c 6520 696e 2061 6c6c 6f77  lexible in allow
+000003f0: 696e 670a 6172 6269 7472 6172 7920 7765  ing.arbitrary we
+00000400: 6967 6869 6e67 206f 6620 7461 7861 2c20  ighing of taxa, 
+00000410: 652e 672e 2c20 6261 7365 6420 6f6e 2070  e.g., based on p
+00000420: 7265 6469 6374 6564 2066 6974 6e65 7373  redicted fitness
+00000430: 2f61 6e74 6967 656e 6963 2064 7269 6674  /antigenic drift
+00000440: 2e20 4669 6e61 6c6c 792c 2050 4152 4e41  . Finally, PARNA
+00000450: 5320 616c 6c6f 7773 2079 6f75 2074 6f20  S allows you to 
+00000460: 6669 6e65 2d74 756e 650a 7265 7072 6573  fine-tune.repres
+00000470: 656e 7461 7469 6f6e 2064 6566 696e 6974  entation definit
+00000480: 696f 6e20 7769 7468 2061 2075 7365 722d  ion with a user-
+00000490: 6465 6669 6e65 6420 636f 7665 7261 6765  defined coverage
+000004a0: 2072 6164 6975 732e 0a0a 0a41 6c74 6572   radius....Alter
+000004b0: 6e61 7469 7665 206d 6574 686f 6473 2063  native methods c
+000004c0: 7572 7265 6e74 6c79 2065 7869 7374 2074  urrently exist t
+000004d0: 6f20 7365 6c65 6374 2074 6178 6120 6f6e  o select taxa on
+000004e0: 2070 6879 6c6f 6765 6e65 7469 6320 7472   phylogenetic tr
+000004f0: 6565 7320 2841 4443 4c29 2c20 6f72 2074  ees (ADCL), or t
+00000500: 6f20 7265 6475 6365 2074 6865 206e 756d  o reduce the num
+00000510: 6265 7220 6f66 2074 6178 6120 696e 2061  ber of taxa in a
+00000520: 2070 6879 6c6f 6765 6e79 2028 5472 6565   phylogeny (Tree
+00000530: 6d65 7229 2e0a 5041 524e 4153 2069 7320  mer)..PARNAS is 
+00000540: 6661 7374 6572 2061 6e64 206d 6f72 6520  faster and more 
+00000550: 7665 7273 6174 696c 6520 7468 616e 205b  versatile than [
+00000560: 4144 434c 5d28 6874 7470 733a 2f2f 6d61  ADCL](https://ma
+00000570: 7473 656e 2e67 6974 6875 622e 696f 2f70  tsen.github.io/p
+00000580: 706c 6163 6572 2f67 656e 6572 6174 6564  placer/generated
+00000590: 5f72 7374 2f72 7070 725f 6d69 6e5f 6164  _rst/rppr_min_ad
+000005a0: 636c 5f74 7265 652e 6874 6d6c 2372 7070  cl_tree.html#rpp
+000005b0: 722d 6d69 6e2d 6164 636c 2d74 7265 6529  r-min-adcl-tree)
+000005c0: 2062 7920 4d61 7473 656e 2065 7420 616c   by Matsen et al
+000005d0: 2e20 2853 7973 7465 6d61 7469 6320 4269  . (Systematic Bi
+000005e0: 6f6c 6f67 7920 3230 3133 292e 0a53 696d  ology 2013)..Sim
+000005f0: 696c 6172 6c79 2c20 5041 524e 4153 2069  ilarly, PARNAS i
+00000600: 7320 6661 7374 6572 2074 6861 6e20 5b54  s faster than [T
+00000610: 7265 656d 6d65 725d 2868 7474 7073 3a2f  reemmer](https:/
+00000620: 2f67 6974 6875 622e 636f 6d2f 666d 656e  /github.com/fmen
+00000630: 6172 646f 2f54 7265 656d 6d65 7229 2028  ardo/Treemmer) (
+00000640: 4d65 6e61 7264 6f20 6574 2061 6c2e 2c20  Menardo et al., 
+00000650: 424d 4320 4269 6f69 6e66 6f72 6d61 7469  BMC Bioinformati
+00000660: 6373 2032 3031 3829 2c0a 616e 6420 6f75  cs 2018),.and ou
+00000670: 7220 6f62 6a65 6374 6976 6520 616c 6c6f  r objective allo
+00000680: 7773 2066 6f72 2072 6570 726f 6475 6369  ws for reproduci
+00000690: 626c 6520 616e 6420 696e 7465 7270 7265  ble and interpre
+000006a0: 7461 626c 6520 7365 6c65 6374 696f 6e73  table selections
+000006b0: 2074 6861 7420 6172 6520 6f70 7469 6d61   that are optima
+000006c0: 6c6c 7920 7265 7072 6573 656e 7461 7469  lly representati
+000006d0: 7665 2e0a 0a0a 0a23 2323 2049 6e73 7461  ve.....### Insta
+000006e0: 6c6c 6174 696f 6e20 2323 230a 5041 524e  llation ###.PARN
+000006f0: 4153 2069 7320 6176 6169 6c61 626c 6520  AS is available 
+00000700: 696e 2050 7950 6920 616e 6420 6361 6e20  in PyPi and can 
+00000710: 6265 2069 6e73 7461 6c6c 6564 2061 730a  be installed as.
+00000720: 6070 6970 2069 6e73 7461 6c6c 2070 6172  `pip install par
+00000730: 6e61 7360 2e20 4e6f 7465 2074 6861 7420  nas`. Note that 
+00000740: 5041 524e 4153 2072 6571 7569 7265 7320  PARNAS requires 
+00000750: 5079 7468 6f6e 2033 2e37 206f 7220 6869  Python 3.7 or hi
+00000760: 6768 6572 2e0a 0a50 4152 4e41 5320 6465  gher...PARNAS de
+00000770: 7065 6e64 7320 6f6e 2064 656e 6472 6f70  pends on dendrop
+00000780: 7920 616e 6420 4269 6f70 7974 686f 6e20  y and Biopython 
+00000790: 666f 7220 7068 796c 6f67 656e 6574 6963  for phylogenetic
+000007a0: 2061 6e64 204d 5341 206d 616e 6970 756c   and MSA manipul
+000007b0: 6174 696f 6e73 2c20 6e75 6d70 7920 616e  ations, numpy an
+000007c0: 6420 6e75 6d62 6120 666f 7220 6a75 7374  d numba for just
+000007d0: 2d69 6e2d 7469 6d65 2063 6f6d 7069 6c61  -in-time compila
+000007e0: 7469 6f6e 206f 6620 7468 6520 6372 6974  tion of the crit
+000007f0: 6963 616c 2061 6c67 6f72 6974 686d 7320  ical algorithms 
+00000800: 696e 746f 206d 6163 6869 6e65 2063 6f64  into machine cod
+00000810: 652c 2061 6e64 2028 6f70 7469 6f6e 616c  e, and (optional
+00000820: 6c79 2920 7068 796c 6f2d 7472 6565 7469  ly) phylo-treeti
+00000830: 6d65 2074 6f20 696e 6665 7220 616e 6365  me to infer ance
+00000840: 7374 7261 6c20 7375 6273 7469 7475 7469  stral substituti
+00000850: 6f6e 7320 616c 6f6e 6720 7472 6565 2065  ons along tree e
+00000860: 6467 6573 2e20 5468 6573 6520 6465 7065  dges. These depe
+00000870: 6e64 656e 6369 6573 2077 696c 6c20 6265  ndencies will be
+00000880: 2069 6e73 7461 6c6c 6564 2061 7574 6f6d   installed autom
+00000890: 6174 6963 616c 6c79 2e0a 0a0a 416c 7465  atically....Alte
+000008a0: 726e 6174 6976 656c 792c 2074 6f20 696e  rnatively, to in
+000008b0: 7374 616c 6c20 5041 524e 4153 2c20 636c  stall PARNAS, cl
+000008c0: 6f6e 6520 6f72 2064 6f77 6e6c 6f61 6420  one or download 
+000008d0: 7468 6973 2070 726f 6a65 6374 2061 6e64  this project and
+000008e0: 2072 756e 0a60 7079 7468 6f6e 2073 6574   run.`python set
+000008f0: 7570 2e70 7920 696e 7374 616c 6c60 2e0a  up.py install`..
+00000900: 2323 2054 7574 6f72 6961 6c20 2323 0a0a  ## Tutorial ##..
+00000910: 5041 524e 4153 2068 6173 2074 6865 2066  PARNAS has the f
+00000920: 6f6c 6c6f 7769 6e67 2074 776f 206d 6169  ollowing two mai
+00000930: 6e20 7573 652d 6361 7365 732e 0a31 2e20  n use-cases..1. 
+00000940: 5b4f 7074 696d 616c 2064 6f77 6e73 616d  [Optimal downsam
+00000950: 706c 696e 675d 2823 6f70 7469 6d61 6c2d  pling](#optimal-
+00000960: 646f 776e 7361 6d70 6c69 6e67 2d6f 662d  downsampling-of-
+00000970: 6c61 7267 652d 7472 6565 7329 0a32 2e20  large-trees).2. 
+00000980: 5b53 656c 6563 7469 6e67 2062 6573 7420  [Selecting best 
+00000990: 7265 7072 6573 656e 7461 7469 7665 735d  representatives]
+000009a0: 2823 7365 6c65 6374 696e 672d 6265 7374  (#selecting-best
+000009b0: 2d72 6570 7265 7365 6e74 6174 6976 6573  -representatives
+000009c0: 290a 0a23 2323 204f 7074 696d 616c 2064  )..### Optimal d
+000009d0: 6f77 6e73 616d 706c 696e 6720 6f66 206c  ownsampling of l
+000009e0: 6172 6765 2074 7265 6573 2023 2323 0a50  arge trees ###.P
+000009f0: 4152 4e41 5320 6c65 7473 2079 6f75 2064  ARNAS lets you d
+00000a00: 6f77 6e73 616d 706c 6520 6120 6c61 7267  ownsample a larg
+00000a10: 6520 7068 796c 6f67 656e 792c 2077 6869  e phylogeny, whi
+00000a20: 6c65 2070 7265 7365 7276 696e 6720 616c  le preserving al
+00000a30: 6c20 7468 6520 6469 7665 7273 6974 7920  l the diversity 
+00000a40: 7570 2074 6f20 6120 7573 6572 2d73 7065  up to a user-spe
+00000a50: 6369 6669 6564 2074 6872 6573 686f 6c64  cified threshold
+00000a60: 2e0a 0a49 6e20 7061 7274 6963 756c 6172  ...In particular
+00000a70: 2c20 6966 2079 6f75 2068 6176 6520 6120  , if you have a 
+00000a80: 7468 7265 7368 6f6c 6420 7061 7261 6d65  threshold parame
+00000a90: 7465 7220 2865 2e67 2e2c 2031 2520 7365  ter (e.g., 1% se
+00000aa0: 7175 656e 6365 2064 6976 6572 6765 6e63  quence divergenc
+00000ab0: 6520 6f6e 2061 2074 7265 6529 2050 4152  e on a tree) PAR
+00000ac0: 4e41 5320 7365 6c65 6374 7320 2a2a 7468  NAS selects **th
+00000ad0: 6520 736d 616c 6c65 7374 2a2a 2073 7562  e smallest** sub
+00000ae0: 7365 7420 6f66 2074 6178 6120 736f 2074  set of taxa so t
+00000af0: 6861 7420 616c 6c20 6f74 6865 7220 7461  hat all other ta
+00000b00: 7861 2061 7265 2077 6974 6869 6e20 7468  xa are within th
+00000b10: 6174 2074 6872 6573 686f 6c64 2064 6973  at threshold dis
+00000b20: 7461 6e63 6520 746f 2061 2072 6570 7265  tance to a repre
+00000b30: 7365 6e74 6174 6976 652e 0a0a 0a54 6865  sentative....The
+00000b40: 2074 7970 6963 616c 2061 7070 6c69 6361   typical applica
+00000b50: 7469 6f6e 206f 6620 7468 6973 2066 6561  tion of this fea
+00000b60: 7475 7265 2069 7320 646f 776e 7363 616c  ture is downscal
+00000b70: 696e 6720 6c61 7267 6520 6465 6e73 656c  ing large densel
+00000b80: 792d 7361 6d70 6c65 6420 7472 6565 732e  y-sampled trees.
+00000b90: 0a49 6e20 7468 6973 2065 7861 6d70 6c65  .In this example
+00000ba0: 2077 6520 7769 6c6c 2075 7365 2061 2028   we will use a (
+00000bb0: 6875 6d61 6e29 2048 314e 3170 646d 2069  human) H1N1pdm i
+00000bc0: 6e66 6c75 656e 7a61 2041 2064 6174 6173  nfluenza A datas
+00000bd0: 6574 2077 6974 6820 3132 2c30 3030 2074  et with 12,000 t
+00000be0: 6178 612e 0a57 6520 6f70 7469 6d61 6c6c  axa..We optimall
+00000bf0: 7920 646f 776e 7361 6d70 6c65 2069 7420  y downsample it 
+00000c00: 7768 696c 6520 7072 6573 6572 7669 6e67  while preserving
+00000c10: 2061 6c6c 2064 6976 6572 7369 7479 2075   all diversity u
+00000c20: 7020 746f 2039 392e 3525 2073 6571 7565  p to 99.5% seque
+00000c30: 6e63 6520 7369 6d69 6c61 7269 7479 2c20  nce similarity, 
+00000c40: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 7061  as follows:..`pa
+00000c50: 726e 6173 202d 7420 6765 6e62 616e 6b5f  rnas -t genbank_
+00000c60: 4831 4e31 7064 6d5f 5553 412e 726f 6f74  H1N1pdm_USA.root
+00000c70: 6564 2e74 7265 202d 2d63 6f76 6572 202d  ed.tre --cover -
+00000c80: 2d72 6164 6975 7320 302e 3030 3520 2d2d  -radius 0.005 --
+00000c90: 7375 6274 7265 6520 4831 4e31 7064 6d2e  subtree H1N1pdm.
+00000ca0: 7230 3035 2e74 7265 600a 0a54 6869 7320  r005.tre`..This 
+00000cb0: 7265 7375 6c74 7320 696e 2061 2074 7265  results in a tre
+00000cc0: 6520 7769 7468 206f 6e6c 7920 3434 3320  e with only 443 
+00000cd0: 7461 7861 2120 4e6f 7465 2074 6861 7420  taxa! Note that 
+00000ce0: 302e 3030 3520 6469 7374 616e 6365 206f  0.005 distance o
+00000cf0: 6e20 6120 6d61 7869 6d75 6d20 6c69 6b65  n a maximum like
+00000d00: 6c69 686f 6f64 2070 6879 6c6f 6765 6e79  lihood phylogeny
+00000d10: 2073 6572 7665 7320 6865 7265 2061 7320   serves here as 
+00000d20: 6120 7072 6f78 7920 666f 7220 7468 6520  a proxy for the 
+00000d30: 302e 3525 2073 6571 7565 6e63 6520 6469  0.5% sequence di
+00000d40: 7665 7267 656e 6365 2e20 4120 646f 776e  vergence. A down
+00000d50: 7361 6d70 6c65 6420 7472 6565 2077 696c  sampled tree wil
+00000d60: 6c20 6265 2073 6176 6564 2074 6f20 6120  l be saved to a 
+00000d70: 6e65 7720 6048 314e 3170 646d 2e72 3030  new `H1N1pdm.r00
+00000d80: 352e 7472 6560 2066 696c 652e 0a54 6865  5.tre` file..The
+00000d90: 2069 6e69 7469 616c 2031 322c 3030 3020   initial 12,000 
+00000da0: 7461 7861 2074 7265 6520 2860 6765 6e62  taxa tree (`genb
+00000db0: 616e 6b5f 4831 4e31 7064 6d5f 5553 412e  ank_H1N1pdm_USA.
+00000dc0: 726f 6f74 6564 2e74 7265 6029 2063 616e  rooted.tre`) can
+00000dd0: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
+00000de0: 2074 7574 6f72 6961 6c20 5b66 6f6c 6465   tutorial [folde
+00000df0: 725d 2874 7574 6f72 6961 6c2f 4831 4e31  r](tutorial/H1N1
+00000e00: 7064 6d5f 3230 3230 2e7a 6970 292e 0a0a  pdm_2020.zip)...
+00000e10: 3c63 656e 7465 723e 0a3c 696d 6720 7372  <center>.<img sr
+00000e20: 633d 2274 7574 6f72 6961 6c2f 6669 6775  c="tutorial/figu
+00000e30: 7265 732f 4831 4e31 7064 6d2d 646f 776e  res/H1N1pdm-down
+00000e40: 7361 6d70 6c69 6e67 2d33 3030 2e70 6e67  sampling-300.png
+00000e50: 223e 0a3c 212d 2d20 3c6f 626a 6563 7420  ">.<!-- <object 
+00000e60: 6461 7461 3d22 7475 746f 7269 616c 2f66  data="tutorial/f
+00000e70: 6967 7572 6573 2f48 314e 3170 646d 2d64  igures/H1N1pdm-d
+00000e80: 6f77 6e73 616d 706c 696e 672e 7064 6622  ownsampling.pdf"
+00000e90: 2074 7970 653d 2261 7070 6c69 6361 7469   type="applicati
+00000ea0: 6f6e 2f70 6466 223e 0a20 2020 203c 656d  on/pdf">.    <em
+00000eb0: 6265 6420 7372 633d 2274 7574 6f72 6961  bed src="tutoria
+00000ec0: 6c2f 6669 6775 7265 732f 4831 4e31 7064  l/figures/H1N1pd
+00000ed0: 6d2d 646f 776e 7361 6d70 6c69 6e67 2e70  m-downsampling.p
+00000ee0: 6466 223e 0a20 2020 2020 2020 203c 703e  df">.        <p>
+00000ef0: 5468 6973 2062 726f 7773 6572 2064 6f65  This browser doe
+00000f00: 7320 6e6f 7420 7375 7070 6f72 7420 5044  s not support PD
+00000f10: 4673 2e20 596f 7520 6361 6e20 7669 6577  Fs. You can view
+00000f20: 2074 6865 2074 7265 6573 203c 6120 6872   the trees <a hr
+00000f30: 6566 3d22 7475 746f 7269 616c 2f66 6967  ef="tutorial/fig
+00000f40: 7572 6573 2f48 314e 3170 646d 2d64 6f77  ures/H1N1pdm-dow
+00000f50: 6e73 616d 706c 696e 672e 7064 6622 3e68  nsampling.pdf">h
+00000f60: 6572 653c 2f61 3e2e 3c2f 703e 0a20 2020  ere</a>.</p>.   
+00000f70: 203c 2f65 6d62 6564 3e0a 3c2f 6f62 6a65   </embed>.</obje
+00000f80: 6374 3e20 2d2d 3e0a 3c2f 6365 6e74 6572  ct> -->.</center
+00000f90: 3e0a 0a42 656c 6f77 2077 6520 6469 7363  >..Below we disc
+00000fa0: 7573 7320 686f 7720 5041 524e 4153 2073  uss how PARNAS s
+00000fb0: 656c 6563 7473 206d 6f73 7420 7265 7072  elects most repr
+00000fc0: 6573 656e 7461 7469 7665 2074 6178 612e  esentative taxa.
+00000fd0: 0a0a 2323 2320 5365 6c65 6374 696e 6720  ..### Selecting 
+00000fe0: 6265 7374 2072 6570 7265 7365 6e74 6174  best representat
+00000ff0: 6976 6573 2023 2323 0a57 6520 7573 6520  ives ###.We use 
+00001000: 6120 6875 6d61 6e20 4831 4e31 7064 6d20  a human H1N1pdm 
+00001010: 6461 7461 7365 7420 7769 7468 2048 4120  dataset with HA 
+00001020: 7365 7175 656e 6365 7320 636f 6c6c 6563  sequences collec
+00001030: 7465 6420 696e 2032 3032 302c 2064 6f77  ted in 2020, dow
+00001040: 6e6c 6f61 6465 6420 6672 6f6d 205b 4952  nloaded from [IR
+00001050: 445d 2866 6c75 6462 2e6f 7267 292c 2066  D](fludb.org), f
+00001060: 6f72 2074 6869 7320 7475 746f 7269 616c  or this tutorial
+00001070: 2e0a 5468 6520 616c 6967 6e6d 656e 7420  ..The alignment 
+00001080: 616e 6420 616e 2069 6e66 6572 7265 6420  and an inferred 
+00001090: 726f 6f74 6564 2074 7265 6520 6361 6e20  rooted tree can 
+000010a0: 6265 2066 6f75 6e64 2069 6e20 7468 6520  be found in the 
+000010b0: 7475 746f 7269 616c 205b 666f 6c64 6572  tutorial [folder
+000010c0: 5d28 7475 746f 7269 616c 2f48 314e 3170  ](tutorial/H1N1p
+000010d0: 646d 5f32 3032 302e 7a69 7029 2e0a 0a54  dm_2020.zip)...T
+000010e0: 6865 2062 6173 6963 2075 7361 6765 206f  he basic usage o
+000010f0: 6620 5041 524e 4153 2069 7320 746f 2066  f PARNAS is to f
+00001100: 696e 6420 6120 6669 7865 6420 6e75 6d62  ind a fixed numb
+00001110: 6572 206f 6620 7265 7072 6573 656e 7461  er of representa
+00001120: 7469 7665 2074 6178 612c 2061 7320 666f  tive taxa, as fo
+00001130: 6c6c 6f77 733a 3c62 723e 0a60 7061 726e  llows:<br>.`parn
+00001140: 6173 202d 7420 4831 4e31 5f68 756d 616e  as -t H1N1_human
+00001150: 5f32 3032 305f 4952 442e 726f 6f74 6564  _2020_IRD.rooted
+00001160: 2e74 7265 202d 6e20 3320 2d2d 636f 6c6f  .tre -n 3 --colo
+00001170: 7220 2248 314e 315f 7061 726e 6173 5f6e  r "H1N1_parnas_n
+00001180: 332e 7472 6522 603c 6272 3e0a 5041 524e  3.tre"`<br>.PARN
+00001190: 4153 2077 696c 6c20 6964 656e 7469 6679  AS will identify
+000011a0: 2033 2062 6573 7420 7265 7072 6573 656e   3 best represen
+000011b0: 7461 7469 7665 2073 7472 6169 6e73 2061  tative strains a
+000011c0: 6e64 2073 6176 6520 6120 636f 6c6f 7265  nd save a colore
+000011d0: 6420 7472 6565 2074 6f20 4831 4e31 5f70  d tree to H1N1_p
+000011e0: 6172 6e61 735f 6e33 2e74 7265 2e0a 4f70  arnas_n3.tre..Op
+000011f0: 656e 696e 6720 7468 6973 2074 7265 6520  ening this tree 
+00001200: 696e 2046 6967 5472 6565 2c20 7769 6c6c  in FigTree, will
+00001210: 2073 686f 7720 7468 6520 7265 7072 6573   show the repres
+00001220: 656e 7461 7469 7665 7320 616e 6420 7468  entatives and th
+00001230: 6569 7220 7265 7370 6563 7469 7665 2063  eir respective c
+00001240: 6c75 7374 6572 7320 6f66 2073 7472 6169  lusters of strai
+00001250: 6e73 2077 6974 6820 6469 6666 6572 656e  ns with differen
+00001260: 7420 636f 6c6f 7273 2e20 4265 6c6f 7720  t colors. Below 
+00001270: 6973 2074 6865 2060 4831 4e31 5f70 6172  is the `H1N1_par
+00001280: 6e61 735f 6e33 2e74 7265 6020 6f75 7470  nas_n3.tre` outp
+00001290: 7574 2074 7265 652c 2077 6865 6e20 6f70  ut tree, when op
+000012a0: 656e 6564 2069 6e20 4669 6754 7265 652e  ened in FigTree.
+000012b0: 2045 6163 6820 636f 6c6f 7220 636f 7272   Each color corr
+000012c0: 6573 706f 6e64 7320 746f 206f 6e65 2050  esponds to one P
+000012d0: 4152 4e41 532d 7365 6c65 6374 6564 2072  ARNAS-selected r
+000012e0: 6570 7265 7365 6e74 6174 6976 6520 616e  epresentative an
+000012f0: 6420 7468 6520 6172 6561 206f 6620 7468  d the area of th
+00001300: 6520 7472 6565 2069 7420 7265 7072 6573  e tree it repres
+00001310: 656e 7473 2e0a 0a3c 6365 6e74 6572 3e0a  ents...<center>.
+00001320: 3c69 6d67 2073 7263 3d22 7475 746f 7269  <img src="tutori
+00001330: 616c 2f66 6967 7572 6573 2f48 314e 315f  al/figures/H1N1_
+00001340: 7061 726e 6173 5f6e 332e 706e 6722 3e0a  parnas_n3.png">.
+00001350: 3c2f 6365 6e74 6572 3e0a 0a41 6464 6974  </center>..Addit
+00001360: 696f 6e61 6c6c 792c 2069 6e20 7468 6520  ionally, in the 
+00001370: 6f75 7470 7574 2050 4152 4e41 5320 7370  output PARNAS sp
+00001380: 6563 6966 6965 7320 7468 6520 616d 6f75  ecifies the amou
+00001390: 6e74 206f 6620 6f76 6572 616c 6c20 6469  nt of overall di
+000013a0: 7665 7273 6974 7920 636f 7665 7265 6420  versity covered 
+000013b0: 6279 2074 6865 2063 686f 7365 6e20 7265  by the chosen re
+000013c0: 7072 6573 656e 7461 7469 7665 732c 2077  presentatives, w
+000013d0: 6869 6368 2069 7320 3433 2520 666f 7220  hich is 43% for 
+000013e0: 6f75 7220 6461 7461 7365 742e 0a0a 2323  our dataset...##
+000013f0: 2323 2044 6574 6572 6d69 6e69 6e67 2074  ## Determining t
+00001400: 6865 2072 6967 6874 206e 756d 6265 7220  he right number 
+00001410: 6f66 2072 6570 7265 7365 6e74 6174 6976  of representativ
+00001420: 6573 2023 2323 230a 5468 6520 2264 6976  es ####.The "div
+00001430: 6572 7369 7479 2063 6f76 6572 6564 2220  ersity covered" 
+00001440: 6d65 7472 6963 2063 616c 6375 6c61 7465  metric calculate
+00001450: 6420 6279 2050 4152 4e41 5320 6973 2061  d by PARNAS is a
+00001460: 2075 7365 6675 6c20 746f 6f6c 2074 6f20   useful tool to 
+00001470: 6465 7465 726d 696e 6520 686f 7720 6d61  determine how ma
+00001480: 6e79 2072 6570 7265 7365 6e74 6174 6976  ny representativ
+00001490: 6573 2069 7320 7375 6666 6963 6965 6e74  es is sufficient
+000014a0: 2e0a 546f 2066 696e 6420 7468 6520 616d  ..To find the am
+000014b0: 6f75 6e74 206f 6620 6469 7665 7273 6974  ount of diversit
+000014c0: 7920 636f 7665 7265 6420 6279 2064 6966  y covered by dif
+000014d0: 6665 7265 6e74 206e 756d 6265 7273 206f  ferent numbers o
+000014e0: 6620 7265 7072 6573 656e 7461 7469 7665  f representative
+000014f0: 732c 2079 6f75 2063 616e 2063 686f 6f73  s, you can choos
+00001500: 6520 6120 6c61 7267 6520 656e 6f75 6768  e a large enough
+00001510: 206e 2c20 652e 672e 2c20 6e3d 3230 2c20   n, e.g., n=20, 
+00001520: 616e 6420 7275 6e3c 6272 3e0a 6070 6172  and run<br>.`par
+00001530: 6e61 7320 2d74 2048 314e 315f 6875 6d61  nas -t H1N1_huma
+00001540: 6e5f 3230 3230 5f49 5244 2e72 6f6f 7465  n_2020_IRD.roote
+00001550: 642e 7472 6520 2d6e 2032 3020 2d2d 6469  d.tre -n 20 --di
+00001560: 7665 7273 6974 7920 2264 6976 6572 7369  versity "diversi
+00001570: 7479 5f73 636f 7265 732e 6373 7622 603c  ty_scores.csv"`<
+00001580: 6272 3e0a 5468 6973 2063 6f6d 6d61 6e64  br>.This command
+00001590: 2077 696c 6c20 7361 7665 2061 2043 5356   will save a CSV
+000015a0: 2066 696c 6520 7769 7468 206f 7074 696d   file with optim
+000015b0: 616c 2064 6976 6572 7369 7479 2073 636f  al diversity sco
+000015c0: 7265 7320 666f 7220 6e20 6265 7477 6565  res for n betwee
+000015d0: 6e20 3220 616e 6420 3230 2e20 466f 7220  n 2 and 20. For 
+000015e0: 6f75 7220 6461 7461 7365 742c 2069 7420  our dataset, it 
+000015f0: 7368 6f77 7320 7468 6174 206f 6e6c 7920  shows that only 
+00001600: 3620 7265 7072 6573 656e 7461 7469 7665  6 representative
+00001610: 2073 7472 6169 6e73 2061 7265 206e 6565   strains are nee
+00001620: 6465 6420 746f 2063 6f76 6572 206f 7665  ded to cover ove
+00001630: 7220 3630 2520 6f66 2074 6865 206f 7665  r 60% of the ove
+00001640: 7261 6c6c 2064 6976 6572 7369 7479 2e20  rall diversity. 
+00001650: 4f70 656e 696e 6720 7468 6520 4353 5620  Opening the CSV 
+00001660: 6669 6c65 2069 6e20 4578 6365 6c2f 4e75  file in Excel/Nu
+00001670: 6d62 6572 732c 206f 6e65 2063 616e 2074  mbers, one can t
+00001680: 6865 6e20 636f 6e73 7472 7563 7420 7468  hen construct th
+00001690: 6520 666f 6c6c 6f77 696e 6720 6772 6170  e following grap
+000016a0: 6820 746f 2062 6574 7465 7220 7669 7375  h to better visu
+000016b0: 616c 697a 6520 7468 6520 6461 7461 2e0a  alize the data..
+000016c0: 0a3c 6365 6e74 6572 3e0a 3c69 6d67 2073  .<center>.<img s
+000016d0: 7263 3d22 7475 746f 7269 616c 2f66 6967  rc="tutorial/fig
+000016e0: 7572 6573 2f64 6976 6572 7369 7479 5f63  ures/diversity_c
+000016f0: 6f76 6572 6564 2e70 6e67 2220 7769 6474  overed.png" widt
+00001700: 683d 2234 3530 7078 223e 0a3c 2f63 656e  h="450px">.</cen
+00001710: 7465 723e 0a0a 2323 2323 2055 7369 6e67  ter>..#### Using
+00001720: 2070 7269 6f72 2072 6570 7265 7365 6e74   prior represent
+00001730: 6174 6976 6573 2023 2323 230a 4974 206f  atives ####.It o
+00001740: 6674 656e 206d 6179 2062 6520 7573 6566  ften may be usef
+00001750: 756c 2074 6f20 6669 6e64 206e 6577 2072  ul to find new r
+00001760: 6570 7265 7365 6e74 6174 6976 6573 2c20  epresentatives, 
+00001770: 7768 696c 6520 7370 6563 6966 7969 6e67  while specifying
+00001780: 2074 6865 2070 7265 7669 6f75 7320 7461   the previous ta
+00001790: 7861 2f73 7472 6169 6e73 2074 6861 7420  xa/strains that 
+000017a0: 7765 7265 2074 7265 6174 6564 2061 7320  were treated as 
+000017b0: 7265 7072 6573 656e 7461 7469 7665 732e  representatives.
+000017c0: 2049 6e20 6f75 7220 4831 4e31 2064 6174   In our H1N1 dat
+000017d0: 6173 6574 2c20 7765 2069 6e63 6c75 6465  aset, we include
+000017e0: 6420 7477 6f20 6c61 7465 7374 2048 314e  d two latest H1N
+000017f0: 3120 7661 6363 696e 6520 7374 7261 696e  1 vaccine strain
+00001800: 732c 2041 2f57 6973 636f 6e73 696e 2f35  s, A/Wisconsin/5
+00001810: 3838 2f32 3031 3920 616e 6420 412f 4861  88/2019 and A/Ha
+00001820: 7761 6969 2f37 302f 3230 3139 2e20 5573  waii/70/2019. Us
+00001830: 696e 6720 5041 524e 4153 2077 6520 6361  ing PARNAS we ca
+00001840: 6e20 6669 7820 7468 6573 6520 7477 6f20  n fix these two 
+00001850: 7374 7261 696e 7320 6173 2027 7072 696f  strains as 'prio
+00001860: 7227 2072 6570 7265 7365 6e74 6174 6976  r' representativ
+00001870: 6573 2061 6e64 2066 696e 6420 6e65 7720  es and find new 
+00001880: 7265 7072 6573 656e 7461 7469 7665 732c  representatives,
+00001890: 2073 6f20 7468 6174 206f 6c64 2061 6e64   so that old and
+000018a0: 206e 6577 2072 6570 7265 7365 6e74 6174   new representat
+000018b0: 6976 6573 2077 6f72 6b20 6f70 7469 6d61  ives work optima
+000018c0: 6c6c 7920 746f 6765 7468 6572 2e20 5765  lly together. We
+000018d0: 2075 7365 2060 2d2d 7072 696f 7260 206f   use `--prior` o
+000018e0: 7074 696f 6e20 746f 206e 6f74 6966 7920  ption to notify 
+000018f0: 5041 524e 4153 206f 6620 7468 6520 7477  PARNAS of the tw
+00001900: 6f20 7661 6363 696e 6520 7374 7261 696e  o vaccine strain
+00001910: 7320 6279 2073 7065 6369 6679 696e 6720  s by specifying 
+00001920: 6120 7265 6775 6c61 7220 6578 7072 6573  a regular expres
+00001930: 7369 6f6e 206d 6174 6368 696e 6720 7468  sion matching th
+00001940: 6569 7220 6e61 6d65 7320 696e 206f 7572  eir names in our
+00001950: 2064 6174 6173 6574 2028 7768 6963 6820   dataset (which 
+00001960: 7374 6172 7420 7769 7468 2022 5661 6363  start with "Vacc
+00001970: 696e 657c 2229 3a3c 6272 3e0a 6070 6172  ine|"):<br>.`par
+00001980: 6e61 7320 2d74 2048 314e 315f 6875 6d61  nas -t H1N1_huma
+00001990: 6e5f 3230 3230 5f49 5244 2e72 6f6f 7465  n_2020_IRD.roote
+000019a0: 642e 7472 6520 2d6e 2033 202d 2d70 7269  d.tre -n 3 --pri
+000019b0: 6f72 2022 5661 6363 696e 652e 2a22 202d  or "Vaccine.*" -
+000019c0: 2d63 6f6c 6f72 2022 4831 4e31 5f70 6172  -color "H1N1_par
+000019d0: 6e61 735f 6e33 5f76 6163 6369 6e65 732e  nas_n3_vaccines.
+000019e0: 7472 6522 603c 6272 3e0a 5468 6520 7265  tre"`<br>.The re
+000019f0: 7375 6c74 2069 7320 7368 6f77 6e20 696e  sult is shown in
+00001a00: 2061 2074 7265 6520 6265 6c6f 772e 2050   a tree below. P
+00001a10: 4152 4e41 5320 636f 6c6f 7273 2074 6865  ARNAS colors the
+00001a20: 2070 7269 6f72 2072 6570 7265 7365 6e74   prior represent
+00001a30: 6174 6976 6573 2061 6e64 2074 6865 2072  atives and the r
+00001a40: 6573 7065 6374 6976 6520 7061 7274 7320  espective parts 
+00001a50: 6f66 2074 6865 2074 7265 6520 696e 2072  of the tree in r
+00001a60: 6564 2e0a 0a3c 6365 6e74 6572 3e0a 3c69  ed...<center>.<i
+00001a70: 6d67 2073 7263 3d22 7475 746f 7269 616c  mg src="tutorial
+00001a80: 2f66 6967 7572 6573 2f48 314e 315f 7061  /figures/H1N1_pa
+00001a90: 726e 6173 5f6e 335f 7661 6363 696e 6573  rnas_n3_vaccines
+00001aa0: 2e70 6e67 223e 0a3c 2f63 656e 7465 723e  .png">.</center>
+00001ab0: 0a0a 2323 2323 2053 7065 6369 6679 696e  ..#### Specifyin
+00001ac0: 6720 6120 636f 7665 7261 6765 2072 6164  g a coverage rad
+00001ad0: 6975 7320 2323 2323 0a59 6f75 2063 616e  ius ####.You can
+00001ae0: 206e 6f74 6966 7920 5041 524e 4153 2074   notify PARNAS t
+00001af0: 6861 7420 6120 7369 6e67 6c65 2074 6178  hat a single tax
+00001b00: 6f6e 2027 636f 7665 7273 2720 6f74 6865  on 'covers' othe
+00001b10: 7220 7461 7861 2077 6974 6869 6e20 6120  r taxa within a 
+00001b20: 6669 7865 6420 7261 6469 7573 2028 7573  fixed radius (us
+00001b30: 696e 6720 602d 2d72 6164 6975 7360 206f  ing `--radius` o
+00001b40: 7074 696f 6e29 2e20 5041 524e 4153 2077  ption). PARNAS w
+00001b50: 696c 6c20 7468 656e 2066 696e 6420 7265  ill then find re
+00001b60: 7072 6573 656e 7461 7469 7665 732c 2077  presentatives, w
+00001b70: 6869 6368 2074 6f67 6574 6865 7220 636f  hich together co
+00001b80: 7665 7220 6173 206d 7563 6820 6469 7665  ver as much dive
+00001b90: 7273 6974 7920 6173 2070 6f73 7369 626c  rsity as possibl
+00001ba0: 652e 2041 6c74 6572 6e61 7469 7665 6c79  e. Alternatively
+00001bb0: 2c20 5041 524e 4153 2063 616e 2066 696e  , PARNAS can fin
+00001bc0: 6420 7468 6520 6d69 6e69 6d75 6d20 6e75  d the minimum nu
+00001bd0: 6d62 6572 206f 6620 7265 7072 6573 656e  mber of represen
+00001be0: 7461 7469 7665 7320 7468 6174 206a 6f69  tatives that joi
+00001bf0: 6e74 6c79 2063 6f76 6572 202a 616c 6c2a  ntly cover *all*
+00001c00: 2064 6976 6572 7369 7479 206f 6e20 7468   diversity on th
+00001c10: 6520 7472 6565 2028 602d 2d63 6f76 6572  e tree (`--cover
+00001c20: 6020 6f70 7469 6f6e 292e 2054 6869 7320  ` option). This 
+00001c30: 6665 6174 7572 6520 6361 6e20 6265 2075  feature can be u
+00001c40: 7365 6420 746f 206f 7074 696d 616c 6c79  sed to optimally
+00001c50: 2072 6564 7563 6520 7468 6520 7265 6475   reduce the redu
+00001c60: 6e64 616e 6379 2069 6e20 796f 7572 2064  ndancy in your d
+00001c70: 6174 6173 6574 2e20 4d6f 7265 6f76 6572  ataset. Moreover
+00001c80: 2c20 7468 6973 2066 6561 7475 7265 2077  , this feature w
+00001c90: 6173 206d 6f74 6976 6174 6564 2062 7920  as motivated by 
+00001ca0: 6170 706c 6963 6174 696f 6e73 2069 6e20  applications in 
+00001cb0: 7669 726f 6c6f 6779 2c20 7768 6572 6520  virology, where 
+00001cc0: 6576 6f6c 7574 696f 6e61 7279 2064 6973  evolutionary dis
+00001cd0: 7461 6e63 6520 6f66 7465 6e20 636f 7272  tance often corr
+00001ce0: 656c 6174 6573 2077 6974 6820 616e 7469  elates with anti
+00001cf0: 6765 6e69 6320 6472 6966 742e 2046 6f72  genic drift. For
+00001d00: 2065 7861 6d70 6c65 2c20 696e 2073 7769   example, in swi
+00001d10: 6e65 2069 6e66 6c75 656e 7a61 2041 2076  ne influenza A v
+00001d20: 6972 7573 2072 6573 6561 7263 682c 2035  irus research, 5
+00001d30: 2520 2861 6d69 6e6f 2061 6369 6429 2064  % (amino acid) d
+00001d40: 6976 6572 6765 6e63 6520 6265 7477 6565  ivergence betwee
+00001d50: 6e20 4841 2073 6571 7565 6e63 6573 2069  n HA sequences i
+00001d60: 7320 636f 6e73 6964 6572 6564 2061 2063  s considered a c
+00001d70: 6f72 7265 6c61 7465 206f 6620 6c6f 7373  orrelate of loss
+00001d80: 2069 6e20 6372 6f73 732d 7265 6163 7469   in cross-reacti
+00001d90: 7669 7479 2062 6574 7765 656e 2073 7472  vity between str
+00001da0: 6169 6e73 2e20 5468 6572 6566 6f72 652c  ains. Therefore,
+00001db0: 2073 7065 6369 6679 696e 6720 6120 7261   specifying a ra
+00001dc0: 6469 7573 206f 6e20 6120 7472 6565 2063  dius on a tree c
+00001dd0: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
+00001de0: 7e34 2520 7365 7175 656e 6365 2064 6976  ~4% sequence div
+00001df0: 6572 6765 6e63 652c 2063 616e 2068 656c  ergence, can hel
+00001e00: 7020 6964 656e 7469 6679 2067 6f6f 6420  p identify good 
+00001e10: 7661 6363 696e 6520 6361 6e64 6964 6174  vaccine candidat
+00001e20: 6573 2e0a 0a54 6f20 6675 7274 6865 7220  es...To further 
+00001e30: 6661 6369 6c69 7461 7465 2074 6869 7320  facilitate this 
+00001e40: 7072 6f63 6573 732c 2050 4152 4e41 5320  process, PARNAS 
+00001e50: 6361 6e20 7461 6b65 2061 6d69 6e6f 2061  can take amino a
+00001e60: 6369 6420 7365 7175 656e 6365 2061 6c69  cid sequence ali
+00001e70: 676e 6d65 6e74 2061 6e64 2070 6173 7320  gnment and pass 
+00001e80: 6974 2074 6f20 5b54 7265 6554 696d 655d  it to [TreeTime]
+00001e90: 2868 7474 7073 3a2f 2f74 7265 6574 696d  (https://treetim
+00001ea0: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00001eb0: 2f65 6e2f 6c61 7465 7374 2f29 2074 6f20  /en/latest/) to 
+00001ec0: 6669 6e64 2061 6e63 6573 7472 616c 2041  find ancestral A
+00001ed0: 4120 7375 6273 7469 7475 7469 6f6e 7320  A substitutions 
+00001ee0: 616c 6f6e 6720 7468 6520 7472 6565 2065  along the tree e
+00001ef0: 6467 6573 2e20 4974 2077 696c 6c20 7468  dges. It will th
+00001f00: 656e 2072 652d 7363 616c 6520 7468 6520  en re-scale the 
+00001f10: 7472 6565 2c20 736f 2074 6861 7420 6564  tree, so that ed
+00001f20: 6765 206c 656e 6774 6873 2077 696c 6c20  ge lengths will 
+00001f30: 7265 666c 6563 7420 7468 6520 6e75 6d62  reflect the numb
+00001f40: 6572 206f 6620 7375 6273 7469 7475 7469  er of substituti
+00001f50: 6f6e 7320 616c 6f6e 6720 7468 6174 2065  ons along that e
+00001f60: 6467 652c 2077 6869 6368 2077 696c 6c20  dge, which will 
+00001f70: 6865 6c70 2073 7065 6369 6679 2061 2034  help specify a 4
+00001f80: 2520 6469 7665 7267 656e 6365 2072 6164  % divergence rad
+00001f90: 6975 7320 696e 2074 6572 6d73 206f 6620  ius in terms of 
+00001fa0: 7468 6520 2320 6f66 2061 6d69 6e6f 2061  the # of amino a
+00001fb0: 6369 6420 7375 6273 7469 7475 7469 6f6e  cid substitution
+00001fc0: 732e 0a0a 6070 6172 6e61 7320 2d74 2048  s...`parnas -t H
+00001fd0: 314e 315f 6875 6d61 6e5f 3230 3230 5f49  1N1_human_2020_I
+00001fe0: 5244 2e72 6f6f 7465 642e 7472 6520 2d2d  RD.rooted.tre --
+00001ff0: 636f 7665 7220 2d2d 7468 7265 7368 6f6c  cover --threshol
+00002000: 6420 3936 202d 2d61 6120 4831 4e31 5f68  d 96 --aa H1N1_h
+00002010: 756d 616e 5f32 3032 305f 4952 442e 6861  uman_2020_IRD.ha
+00002020: 312e 616c 6e20 2d2d 636f 6c6f 7220 2270  1.aln --color "p
+00002030: 6172 6e61 735f 3936 636f 7665 7261 6765  arnas_96coverage
+00002040: 2e74 7265 2260 0a0a 496e 2074 6865 2061  .tre"`..In the a
+00002050: 626f 7665 2063 6f6d 6d61 6e64 2077 6520  bove command we 
+00002060: 7061 7373 2074 6865 2041 4120 616c 6967  pass the AA alig
+00002070: 6e6d 656e 7420 6f66 2048 4131 2073 6571  nment of HA1 seq
+00002080: 7565 6e63 6573 2066 726f 6d20 6f75 7220  uences from our 
+00002090: 6461 7461 7365 7420 7769 7468 2074 6865  dataset with the
+000020a0: 2060 2d2d 6161 6020 6f70 7469 6f6e 2c20   `--aa` option, 
+000020b0: 616e 6420 7370 6563 6966 7920 7468 6520  and specify the 
+000020c0: 3936 2520 7468 7265 7368 6f6c 6420 2869  96% threshold (i
+000020d0: 2e65 2e2c 2034 2520 7365 7175 656e 6365  .e., 4% sequence
+000020e0: 2064 6976 6572 6765 6e63 6529 2e20 4e6f   divergence). No
+000020f0: 7465 2074 6861 7420 602d 2d74 6872 6573  te that `--thres
+00002100: 686f 6c64 6020 776f 726b 7320 6173 2061  hold` works as a
+00002110: 2073 7562 7374 6974 7574 6520 666f 7220   substitute for 
+00002120: 602d 2d72 6164 6975 7360 2c20 7768 656e  `--radius`, when
+00002130: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
+00002140: 5041 524e 4153 2074 6f20 7573 6520 7468  PARNAS to use th
+00002150: 6520 616c 6967 6e6d 656e 7420 696e 666f  e alignment info
+00002160: 726d 6174 696f 6e20 616e 6420 7265 2d73  rmation and re-s
+00002170: 6361 6c65 2074 6865 2074 7265 652e 2052  cale the tree. R
+00002180: 756e 6e69 6e67 2074 6869 7320 636f 6d6d  unning this comm
+00002190: 616e 6420 7769 6c6c 2073 686f 7720 7468  and will show th
+000021a0: 6174 2061 2073 696e 676c 6520 7374 7261  at a single stra
+000021b0: 696e 2028 412f 5769 7363 6f6e 7369 6e2f  in (A/Wisconsin/
+000021c0: 3332 2f32 3032 3029 2069 7320 7375 6666  32/2020) is suff
+000021d0: 6963 6965 6e74 2074 6f20 636f 7665 7220  icient to cover 
+000021e0: 616c 6c20 6469 7665 7273 6974 7920 6f6e  all diversity on
+000021f0: 206f 7572 2074 7265 652e 0a0a 4e65 7874   our tree...Next
+00002200: 2c20 7765 2075 7365 2061 206d 6f72 6520  , we use a more 
+00002210: 7265 7374 7269 6374 6976 6520 7468 7265  restrictive thre
+00002220: 7368 6f6c 6420 6f66 2039 3725 2061 6e64  shold of 97% and
+00002230: 2061 6c73 6f20 6164 6420 7468 6520 7661   also add the va
+00002240: 6363 696e 6520 7374 7261 696e 7320 6173  ccine strains as
+00002250: 2074 6865 2070 7269 6f72 2072 6570 7265   the prior repre
+00002260: 7365 6e74 6174 6976 6573 2e20 5468 6973  sentatives. This
+00002270: 2077 6179 2050 4152 4e41 5320 6361 6e20   way PARNAS can 
+00002280: 696e 6469 6361 7465 2074 6865 2061 7265  indicate the are
+00002290: 6173 206f 6620 7468 6520 7472 6565 2c20  as of the tree, 
+000022a0: 7768 6963 6820 6172 6520 6e6f 7420 636f  which are not co
+000022b0: 7665 7265 6420 6279 2074 6865 2076 6163  vered by the vac
+000022c0: 6369 6e65 2073 7472 6169 6e73 2061 6e64  cine strains and
+000022d0: 2073 7567 6765 7374 206e 6577 2072 6570   suggest new rep
+000022e0: 7265 7365 6e74 6174 6976 6573 2074 6f20  resentatives to 
+000022f0: 636f 6d70 6c65 6d65 6e74 2074 6865 2076  complement the v
+00002300: 6163 6369 6e65 2073 7472 6169 6e73 2e0a  accine strains..
+00002310: 0a60 7061 726e 6173 202d 7420 4831 4e31  .`parnas -t H1N1
+00002320: 5f68 756d 616e 5f32 3032 305f 4952 442e  _human_2020_IRD.
+00002330: 726f 6f74 6564 2e74 7265 202d 2d63 6f76  rooted.tre --cov
+00002340: 6572 202d 2d74 6872 6573 686f 6c64 2039  er --threshold 9
+00002350: 3720 2d2d 6161 2048 314e 315f 6875 6d61  7 --aa H1N1_huma
+00002360: 6e5f 3230 3230 5f49 5244 2e68 6131 2e61  n_2020_IRD.ha1.a
+00002370: 6c6e 202d 2d63 6f6c 6f72 2022 7061 726e  ln --color "parn
+00002380: 6173 5f39 3763 6f76 6572 6167 655f 7661  as_97coverage_va
+00002390: 6363 696e 6573 2e74 7265 2220 2d2d 7072  ccines.tre" --pr
+000023a0: 696f 7220 2256 6163 6369 6e65 2e2a 2260  ior "Vaccine.*"`
+000023b0: 0a0a 4f70 656e 696e 6720 6070 6172 6e61  ..Opening `parna
+000023c0: 735f 3937 636f 7665 7261 6765 5f76 6163  s_97coverage_vac
+000023d0: 6369 6e65 732e 7472 6560 2069 6e20 4669  cines.tre` in Fi
+000023e0: 6754 7265 6520 7769 6c6c 2073 686f 7720  gTree will show 
+000023f0: 7573 2074 6861 7420 7468 6572 6520 6172  us that there ar
+00002400: 6520 7477 6f20 636c 6164 6573 2069 6e20  e two clades in 
+00002410: 7468 6520 7472 6565 2c20 7768 6963 6820  the tree, which 
+00002420: 6172 6520 6e6f 7420 636f 7665 7265 6420  are not covered 
+00002430: 6279 2076 6163 6369 6e65 2073 7472 6169  by vaccine strai
+00002440: 6e73 2028 7468 6520 6772 6565 6e20 616e  ns (the green an
+00002450: 6420 626c 7565 2063 6c61 6465 7329 2e20  d blue clades). 
+00002460: 4e6f 7465 2074 6861 7420 7468 6520 7472  Note that the tr
+00002470: 6565 2077 6173 2072 652d 7363 616c 6564  ee was re-scaled
+00002480: 2062 7920 5041 524e 4153 2e0a 0a3c 6365   by PARNAS...<ce
+00002490: 6e74 6572 3e0a 3c69 6d67 2073 7263 3d22  nter>.<img src="
+000024a0: 7475 746f 7269 616c 2f66 6967 7572 6573  tutorial/figures
+000024b0: 2f48 314e 315f 7061 726e 6173 5f39 3763  /H1N1_parnas_97c
+000024c0: 6f76 6572 6167 655f 7661 6363 696e 6573  overage_vaccines
+000024d0: 2e70 6e67 223e 0a3c 2f63 656e 7465 723e  .png">.</center>
+000024e0: 0a0a 2323 2323 204f 7468 6572 2066 756e  ..#### Other fun
+000024f0: 6374 696f 6e61 6c69 7479 2023 2323 230a  ctionality ####.
+00002500: 2d20 5370 6563 6966 7920 7765 6967 6874  - Specify weight
+00002510: 7320 666f 7220 7461 7861 2c20 736f 2074  s for taxa, so t
+00002520: 6861 7420 7461 7861 2f73 7472 6169 6e73  hat taxa/strains
+00002530: 2077 6974 6820 6c61 7267 6572 2077 6569   with larger wei
+00002540: 6768 7473 2061 7265 2062 6574 7465 7220  ghts are better 
+00002550: 7265 7072 6573 656e 7465 642e 0a2d 2046  represented..- F
+00002560: 6c65 7869 626c 7920 6578 636c 7564 6520  lexibly exclude 
+00002570: 7461 7861 2074 6f20 6569 7468 6572 2066  taxa to either f
+00002580: 756c 6c79 2069 676e 6f72 6520 7468 656d  ully ignore them
+00002590: 206f 7220 746f 206e 6f74 2063 6f6e 7369   or to not consi
+000025a0: 6465 7220 7468 656d 2061 7320 706f 7465  der them as pote
+000025b0: 6e74 6961 6c20 7265 7072 6573 656e 7461  ntial representa
+000025c0: 7469 7665 732e 0a0a 2323 2050 4152 4e41  tives...## PARNA
+000025d0: 5320 7573 6167 6520 2323 0a0a 6070 6172  S usage ##..`par
+000025e0: 6e61 7320 2d74 2054 5245 4520 5b2d 6e20  nas -t TREE [-n 
+000025f0: 5341 4d50 4c45 535d 205b 6f74 6865 7220  SAMPLES] [other 
+00002600: 6f70 7469 6f6e 735d 600a 0a54 6865 2069  options]`..The i
+00002610: 6e70 7574 2074 7265 6520 7368 6f75 6c64  nput tree should
+00002620: 2062 6520 696e 206e 6578 7573 206f 7220   be in nexus or 
+00002630: 6e65 7769 636b 2066 6f72 6d61 742e 0a0a  newick format...
+00002640: 466f 7220 6120 6465 7461 696c 6564 2072  For a detailed r
+00002650: 6566 6572 656e 6365 206f 6e20 5041 524e  eference on PARN
+00002660: 4153 206f 7074 696f 6e73 2072 756e 2060  AS options run `
+00002670: 7061 726e 6173 202d 6860 206f 7220 7365  parnas -h` or se
+00002680: 6520 6265 6c6f 772e 0a0a 2a47 656e 6572  e below...*Gener
+00002690: 616c 206f 7074 696f 6e73 2a0a 0a7c 204f  al options*..| O
+000026a0: 7074 696f 6e20 7c20 4465 7363 7269 7074  ption | Descript
+000026b0: 696f 6e20 7c0a 7c20 2d2d 2d20 7c20 2d2d  ion |.| --- | --
+000026c0: 2d20 7c0a 7c2d 2d72 6164 6975 7320 7c20  - |.|--radius | 
+000026d0: 5370 6563 6966 7920 6120 7261 6469 7573  Specify a radius
+000026e0: 2028 6469 7374 616e 6365 206f 6e20 6120   (distance on a 
+000026f0: 7472 6565 2920 736f 2074 6861 7420 6576  tree) so that ev
+00002700: 6572 7920 7265 7072 6573 656e 7461 7469  ery representati
+00002710: 7665 2063 6f76 6572 7320 616c 6c20 6469  ve covers all di
+00002720: 7665 7273 6974 7920 7769 7468 696e 2074  versity within t
+00002730: 6861 7420 7261 6469 7573 2e20 5041 524e  hat radius. PARN
+00002740: 4153 2077 696c 6c20 7468 656e 2063 686f  AS will then cho
+00002750: 6f73 6520 7265 7072 6573 656e 7461 7469  ose representati
+00002760: 7665 7320 7468 6174 206f 7074 696d 616c  ves that optimal
+00002770: 6c79 2063 6f76 6572 2061 7320 6d75 6368  ly cover as much
+00002780: 2064 6976 6572 7369 7479 2061 7320 706f   diversity as po
+00002790: 7373 6962 6c65 207c 0a7c 202d 2d70 7269  ssible |.| --pri
+000027a0: 6f72 207c 2053 7065 6369 6679 2070 7269  or | Specify pri
+000027b0: 6f72 2072 6570 7265 7365 6e74 6174 6976  or representativ
+000027c0: 6573 2077 6974 6820 6120 7265 6765 782e  es with a regex.
+000027d0: 2050 4152 4e41 5320 7769 6c6c 2074 6865   PARNAS will the
+000027e0: 6e20 6964 656e 7469 6679 2072 6570 7265  n identify repre
+000027f0: 7365 6e74 6174 6976 6573 206f 6620 276e  sentatives of 'n
+00002800: 6577 2720 6469 7665 7273 6974 7920 7c0a  ew' diversity |.
+00002810: 7c20 2d2d 7765 6967 6874 7320 7c20 4164  | --weights | Ad
+00002820: 6420 6120 4353 5620 6669 6c65 2073 7065  d a CSV file spe
+00002830: 6369 6679 696e 6720 7765 6967 6874 7320  cifying weights 
+00002840: 666f 7220 736f 6d65 206f 7220 616c 6c20  for some or all 
+00002850: 7461 7861 2f73 7472 6169 6e73 207c 0a7c  taxa/strains |.|
+00002860: 202d 2d63 6f76 6572 207c 2049 6e73 7465   --cover | Inste
+00002870: 6164 206f 6620 7370 6563 6966 7969 6e67  ad of specifying
+00002880: 2074 6865 206e 756d 6265 7220 6f66 2072   the number of r
+00002890: 6570 7265 7365 6e74 6174 6976 6573 2c20  epresentatives, 
+000028a0: 7370 6563 6966 7920 7468 6520 7261 6469  specify the radi
+000028b0: 7573 2061 6e64 2050 4152 4e41 5320 7769  us and PARNAS wi
+000028c0: 6c6c 2066 696e 6420 7265 7072 6573 656e  ll find represen
+000028d0: 7461 7469 7665 2074 6861 7420 636f 7665  tative that cove
+000028e0: 7220 616c 6c20 6469 7665 7273 6974 7920  r all diversity 
+000028f0: 6f6e 2074 6865 2074 7265 6520 7c0a 0a2a  on the tree |..*
+00002900: 4f75 7470 7574 206f 7074 696f 6e73 2028  Output options (
+00002910: 636f 6d62 696e 696e 6720 6f75 7470 7574  combining output
+00002920: 206f 7074 696f 6e73 2069 7320 616c 6c6f   options is allo
+00002930: 7765 6429 2a0a 0a7c 204f 7074 696f 6e20  wed)*..| Option 
+00002940: 7c20 4465 7363 7269 7074 696f 6e20 7c0a  | Description |.
+00002950: 7c20 2d2d 2d20 7c20 2d2d 2d20 7c0a 7c20  | --- | --- |.| 
+00002960: 2d2d 636f 6c6f 7220 7c20 5370 6563 6966  --color | Specif
+00002970: 7920 616e 206f 7574 7075 7420 7061 7468  y an output path
+00002980: 2c20 7768 6572 6520 6120 636f 6c6f 7265  , where a colore
+00002990: 6420 7472 6565 2077 696c 6c20 6265 2073  d tree will be s
+000029a0: 6176 6564 2e20 5041 524e 4153 2077 696c  aved. PARNAS wil
+000029b0: 6c20 6869 6768 6c69 6768 7420 7468 6520  l highlight the 
+000029c0: 6368 6f73 656e 2072 6570 7265 7365 6e74  chosen represent
+000029d0: 6174 6976 6573 2061 6e64 2063 6f6c 6f72  atives and color
+000029e0: 2d70 6172 7469 7469 6f6e 2074 6865 2074  -partition the t
+000029f0: 7265 6520 7265 7370 6563 7469 7665 2074  ree respective t
+00002a00: 6f20 7468 6520 7265 7072 6573 656e 7461  o the representa
+00002a10: 7469 7665 732e 2049 6620 7072 696f 7220  tives. If prior 
+00002a20: 7265 7072 6573 656e 7461 7469 7665 7320  representatives 
+00002a30: 6172 6520 7370 6563 6966 6965 642c 2074  are specified, t
+00002a40: 6865 7920 2861 6e64 2074 6865 2073 7562  hey (and the sub
+00002a50: 7472 6565 7320 7468 6579 2072 6570 7265  trees they repre
+00002a60: 7365 6e74 2920 7769 6c6c 2062 6520 636f  sent) will be co
+00002a70: 6c6f 7265 6420 7265 642e 7c0a 7c20 2d2d  lored red.|.| --
+00002a80: 6469 7665 7273 6974 7920 7c20 5370 6563  diversity | Spec
+00002a90: 6966 7920 616e 206f 7574 7075 7420 7061  ify an output pa
+00002aa0: 7468 2c20 7768 6572 6520 6120 4353 5620  th, where a CSV 
+00002ab0: 7769 6c6c 2062 6520 7361 7665 6420 7769  will be saved wi
+00002ac0: 7468 2064 6976 6572 7369 7479 2073 636f  th diversity sco
+00002ad0: 7265 7320 666f 7220 616c 6c20 6b20 286e  res for all k (n
+00002ae0: 756d 6265 7220 6f66 2072 6570 7265 7365  umber of represe
+00002af0: 6e74 6174 6976 6573 2920 6672 6f6d 2032  ntatives) from 2
+00002b00: 2074 6f20 6e2e 2043 616e 2062 6520 7573   to n. Can be us
+00002b10: 6564 2074 6f20 6368 6f6f 7365 2074 6865  ed to choose the
+00002b20: 2072 6967 6874 206e 756d 6265 7220 6f66   right number of
+00002b30: 2072 6570 7265 7365 6e74 6174 6976 6573   representatives
+00002b40: 2066 6f72 2061 2064 6174 6173 6574 207c   for a dataset |
+00002b50: 0a7c 202d 2d73 7562 7472 6565 207c 2053  .| --subtree | S
+00002b60: 7065 6369 6679 2061 2070 6174 682c 2077  pecify a path, w
+00002b70: 6865 7265 2061 2073 7562 7472 6565 2077  here a subtree w
+00002b80: 6974 6820 7468 6520 7361 6d70 6c65 6420  ith the sampled 
+00002b90: 7265 7072 6573 656e 7461 7469 7665 7320  representatives 
+00002ba0: 7769 6c6c 2062 6520 7361 7665 6420 2869  will be saved (i
+00002bb0: 6e20 4e45 5855 5320 666f 726d 6174 2920  n NEXUS format) 
+00002bc0: 7c0a 0a0a 2a4f 7074 696f 6e73 2074 6f20  |...*Options to 
+00002bd0: 6578 636c 7564 652f 636f 6e73 7472 6169  exclude/constrai
+00002be0: 6e20 7461 7861 2a0a 0a7c 204f 7074 696f  n taxa*..| Optio
+00002bf0: 6e20 7c20 4465 7363 7269 7074 696f 6e20  n | Description 
+00002c00: 7c0a 7c20 2d2d 2d20 7c20 2d2d 2d20 7c0a  |.| --- | --- |.
+00002c10: 7c20 2d2d 6578 636c 7564 652d 7265 7020  | --exclude-rep 
+00002c20: 7c20 5245 4745 582e 204d 6174 6368 696e  | REGEX. Matchin
+00002c30: 6720 7461 7861 2077 696c 6c20 6e6f 7420  g taxa will not 
+00002c40: 6265 2063 686f 7365 6e20 6173 2072 6570  be chosen as rep
+00002c50: 7265 7365 6e74 6174 6976 6573 2c20 6275  resentatives, bu
+00002c60: 7420 7468 6579 2077 696c 6c20 636f 6e74  t they will cont
+00002c70: 7269 6275 7465 2074 6f20 7468 6520 6f62  ribute to the ob
+00002c80: 6a65 6374 6976 6520 6675 6e63 7469 6f6e  jective function
+00002c90: 207c 0a7c 202d 2d65 7863 6c75 6465 2d6f   |.| --exclude-o
+00002ca0: 626a 207c 2052 4547 4558 2e20 4d61 7463  bj | REGEX. Matc
+00002cb0: 6869 6e67 2074 6178 6120 6361 6e20 6265  hing taxa can be
+00002cc0: 2073 656c 6563 7465 642c 2062 7574 2077   selected, but w
+00002cd0: 696c 6c20 6e6f 7420 636f 6e74 7269 6275  ill not contribu
+00002ce0: 7465 2074 6f20 7468 6520 6f62 6a65 6374  te to the object
+00002cf0: 6976 6520 6675 6e63 7469 6f6e 2028 7468  ive function (th
+00002d00: 6520 6f70 706f 7369 7465 206f 6620 2d2d  e opposite of --
+00002d10: 6578 636c 7564 652d 7265 7029 207c 0a7c  exclude-rep) |.|
+00002d20: 202d 2d65 7863 6c75 6465 2d66 756c 6c79   --exclude-fully
+00002d30: 207c 2052 4547 4558 2e20 4d61 7463 6869   | REGEX. Matchi
+00002d40: 6e67 2074 6178 6120 7769 6c6c 2062 6520  ng taxa will be 
+00002d50: 636f 6d70 6c65 7465 6c79 2069 676e 6f72  completely ignor
+00002d60: 6564 2062 7920 5041 524e 4153 207c 0a7c  ed by PARNAS |.|
+00002d70: 202d 2d63 6f6e 7374 7261 696e 2d66 756c   --constrain-ful
+00002d80: 6c79 207c 2052 4547 4558 2e20 4f70 706f  ly | REGEX. Oppo
+00002d90: 7369 7465 2074 6f20 272d 2d65 7863 6c75  site to '--exclu
+00002da0: 6465 2d66 756c 6c79 272c 2069 2e65 2e2c  de-fully', i.e.,
+00002db0: 206f 6e6c 7920 7468 6520 6d61 7463 6869   only the matchi
+00002dc0: 6e67 2074 6178 6120 7769 6c6c 2062 6520  ng taxa will be 
+00002dd0: 636f 6e73 6964 6572 6564 2062 7920 5041  considered by PA
+00002de0: 524e 4153 207c 0a0a 2a4f 7074 696f 6e73  RNAS |..*Options
+00002df0: 2074 6f20 636f 6e74 726f 6c20 7365 7175   to control sequ
+00002e00: 656e 6365 2064 6976 6572 6765 6e63 652a  ence divergence*
+00002e10: 0a0a 7c20 4f70 7469 6f6e 207c 2044 6573  ..| Option | Des
+00002e20: 6372 6970 7469 6f6e 207c 0a7c 202d 2d2d  cription |.| ---
+00002e30: 207c 202d 2d2d 207c 0a7c 202d 2d74 6872   | --- |.| --thr
+00002e40: 6573 686f 6c64 207c 204e 756d 6265 7220  eshold | Number 
+00002e50: 6265 7477 6565 6e20 3020 616e 6420 3130  between 0 and 10
+00002e60: 302e 2054 6865 2073 6571 7565 6e63 6520  0. The sequence 
+00002e70: 7369 6d69 6c61 7269 7479 2074 6872 6573  similarity thres
+00002e80: 686f 6c64 2074 6861 7420 776f 726b 7320  hold that works 
+00002e90: 6173 202d 2d72 6164 6975 732e 2046 6f72  as --radius. For
+00002ea0: 2065 7861 6d70 6c65 2c20 2239 3522 2077   example, "95" w
+00002eb0: 696c 6c20 696d 706c 7920 7468 6174 2065  ill imply that e
+00002ec0: 6163 6820 7265 7072 6573 656e 7461 7469  ach representati
+00002ed0: 7665 2063 6f76 6572 7320 616c 6c20 6c65  ve covers all le
+00002ee0: 6176 6573 2077 6974 6869 6e20 3525 2064  aves within 5% d
+00002ef0: 6976 6572 6765 6e63 6520 6f6e 2074 6865  ivergence on the
+00002f00: 2074 7265 652e 2054 6f20 6163 636f 756e   tree. To accoun
+00002f10: 7420 666f 7220 7365 7175 656e 6365 2064  t for sequence d
+00002f20: 6976 6572 6765 6e63 652c 2050 4152 4e41  ivergence, PARNA
+00002f30: 5320 7769 6c6c 2072 756e 2054 7265 6554  S will run TreeT
+00002f40: 696d 6520 746f 2069 6e66 6572 2061 6e63  ime to infer anc
+00002f50: 6573 7472 616c 2073 7562 7374 6974 7574  estral substitut
+00002f60: 696f 6e73 2061 6c6f 6e67 2074 6865 2074  ions along the t
+00002f70: 7265 6520 6564 6765 7320 616e 6420 7265  ree edges and re
+00002f80: 2d77 6569 6768 2074 6865 2065 6467 6573  -weigh the edges
+00002f90: 2062 6173 6564 206f 6e20 7468 6520 6e75   based on the nu
+00002fa0: 6d62 6572 206f 6620 7375 6273 7469 7475  mber of substitu
+00002fb0: 7469 6f6e 7320 6f6e 2074 6865 6d2e 2041  tions on them. A
+00002fc0: 2073 6571 7565 6e63 6520 616c 6967 6e6d   sequence alignm
+00002fd0: 656e 7420 282d 2d6e 7420 6f72 202d 2d61  ent (--nt or --a
+00002fe0: 6129 206d 7573 7420 6265 2073 7065 6369  a) must be speci
+00002ff0: 6669 6564 2077 6974 6820 7468 6973 206f  fied with this o
+00003000: 7074 696f 6e20 7c0a 7c20 2d2d 6e74 207c  ption |.| --nt |
+00003010: 2050 6174 6820 746f 206e 7563 6c65 6f74   Path to nucleot
+00003020: 6964 6520 7365 7175 656e 6365 2061 6c69  ide sequence ali
+00003030: 676e 6d65 6e74 2061 7373 6f63 6961 7465  gnment associate
+00003040: 6420 7769 7468 2074 6865 2074 7265 6520  d with the tree 
+00003050: 7469 7073 207c 0a7c 202d 2d61 6120 7c20  tips |.| --aa | 
+00003060: 5061 7468 2074 6f20 616d 696e 6f20 6163  Path to amino ac
+00003070: 6964 2073 6571 7565 6e63 6520 616c 6967  id sequence alig
+00003080: 6e6d 656e 7420 6173 736f 6369 6174 6564  nment associated
+00003090: 2077 6974 6820 7468 6520 7472 6565 2074   with the tree t
+000030a0: 6970 7320 7c0a                           ips |.
```

### Comparing `parnas-0.1.2/parnas/cli.py` & `parnas-0.1.3/parnas/cli.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/logging.py` & `parnas-0.1.3/parnas/logging.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/fast_pmedian_finder.py` & `parnas-0.1.3/parnas/medoids/fast_pmedian_finder.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/input.py` & `parnas-0.1.3/parnas/medoids/input.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/medoid_utils.py` & `parnas-0.1.3/parnas/medoids/medoid_utils.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/pmedian_finder.py` & `parnas-0.1.3/parnas/medoids/pmedian_finder.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/pmedian_utils.py` & `parnas-0.1.3/parnas/medoids/pmedian_utils.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/tree_coverage.py` & `parnas-0.1.3/parnas/medoids/tree_coverage.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/tree_indexer.py` & `parnas-0.1.3/parnas/medoids/tree_indexer.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/medoids/tree_medoids.py` & `parnas-0.1.3/parnas/medoids/tree_medoids.py`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/parnas/options.py` & `parnas-0.1.3/parnas/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,20 +193,22 @@
 def parse_and_validate():
     args = parser.parse_args()
 
     # Validate the tree.
     tree = None
     try:
         tree = Tree.get(path=args.tree, schema='newick', preserve_underscores=True)
-    except Exception:
+    except Exception as newick_exception:
         try:
             tree = Tree.get(path=args.tree, schema='nexus', preserve_underscores=True)
-        except Exception:
+        except Exception as nexus_exception:
             parser.error('Cannot read the specified tree file "%s". ' % args.tree +
-                         'Make sure the tree is in the newick or nexus format.')
+                         'Make sure the tree is in the newick or nexus format.\n'
+                         f'Nexus error: {nexus_exception}\n'
+                         f'Newick error: {newick_exception}')
 
     # Validate n.
     n = -1
     if not args.samples and not args.cover:
         parser.error('Please either specify the number of representatives with "-n" or use the --cover option.')
     if args.samples:
         n = args.samples
```

### Comparing `parnas-0.1.2/parnas.egg-info/PKG-INFO` & `parnas-0.1.3/parnas.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,86 @@
 Metadata-Version: 2.1
 Name: parnas
-Version: 0.1.2
+Version: 0.1.3
 Summary: Representative taxon sampling from phylogenetic trees
 Home-page: https://github.com/flu-crew/parnas
 Author: Alexey Markin, Sanket Wagle, Siddhant Grover
 Author-email: alex.markin57@gmail.com
 License: MIT
 Description: ## PARNAS ##
+        **If you use PARNAS, please cite it as**</br>
+        *Markin, A., Wagle, S., Grover, S., Baker, A.L.V., Eulenstein, O. and Anderson, T.K. PARNAS: Objectively Selecting the Most Representative Taxa on a Phylogeny. Systematic Biology, 2023; syad028 [doi: 10.1093/sysbio/syad028](https://doi.org/10.1093/sysbio/syad028).*
+        
         PARNAS identifies taxa that best represent diversity on a phylogenetic tree
         and can be used to
         - Select most representative taxa
         - Downsample a large phylogeny while optimally preserving the underlying diversity
         - Reduce redundancy among genetic/genomic sequences
         - Identify key diversity groups on a phylogeny
         
-        PARNAS solves urgent needs in virology/microbiology, such as
+        PARNAS solves needs in virology/microbiology, such as
         - Objectively finding representative strains for in-depth analyses (phenotypic characterization, Bayesian inference, etc.)
         - Objective and flexible vaccine strain selection
         
         PARNAS can take into account previously used representatives and a wide range of user's constraints.
         Additionally, PARNAS is flexible in allowing
-        arbitrary weighing of taxa, e.g., based on predicted fitness/antigenic drift. Finally, PARNAS allows you to fine-tune 
+        arbitrary weighing of taxa, e.g., based on predicted fitness/antigenic drift. Finally, PARNAS allows you to fine-tune
         representation definition with a user-defined coverage radius.
         
         
         Alternative methods currently exist to select taxa on phylogenetic trees (ADCL), or to reduce the number of taxa in a phylogeny (Treemer).
-        PARNAS is faster and more versatile than [ADCL](https://matsen.github.io/pplacer/generated_rst/rppr_min_adcl_tree.html#rppr-min-adcl-tree) by Matsen et al. (Systematic Biology 2013). 
-        Similarly, PARNAS is faster than [Treemmer](https://github.com/fmenardo/Treemmer) (Menardo et al., BMC Bioinformatics 2018), 
+        PARNAS is faster and more versatile than [ADCL](https://matsen.github.io/pplacer/generated_rst/rppr_min_adcl_tree.html#rppr-min-adcl-tree) by Matsen et al. (Systematic Biology 2013).
+        Similarly, PARNAS is faster than [Treemmer](https://github.com/fmenardo/Treemmer) (Menardo et al., BMC Bioinformatics 2018),
         and our objective allows for reproducible and interpretable selections that are optimally representative.
         
-        **If you use PARNAS, please cite it as**</br>
-        *Markin, A., Wagle, S., Grover, S., Baker, A.L.V., Eulenstein, O. and Anderson, T.K., 2022. PARNAS: Objectively Selecting the Most Representative Taxa on a Phylogeny. bioRxiv.*
+        
         
         ### Installation ###
         PARNAS is available in PyPi and can be installed as
         `pip install parnas`. Note that PARNAS requires Python 3.7 or higher.
         
         PARNAS depends on dendropy and Biopython for phylogenetic and MSA manipulations, numpy and numba for just-in-time compilation of the critical algorithms into machine code, and (optionally) phylo-treetime to infer ancestral substitutions along tree edges. These dependencies will be installed automatically.
         
         
         Alternatively, to install PARNAS, clone or download this project and run
         `python setup.py install`.
         ## Tutorial ##
         
-        We use a human H1N1 (pdm09) dataset with HA sequences collected in 2020, downloaded from [IRD](fludb.org), for this tutorial.
+        PARNAS has the following two main use-cases.
+        1. [Optimal downsampling](#optimal-downsampling-of-large-trees)
+        2. [Selecting best representatives](#selecting-best-representatives)
+        
+        ### Optimal downsampling of large trees ###
+        PARNAS lets you downsample a large phylogeny, while preserving all the diversity up to a user-specified threshold.
+        
+        In particular, if you have a threshold parameter (e.g., 1% sequence divergence on a tree) PARNAS selects **the smallest** subset of taxa so that all other taxa are within that threshold distance to a representative.
+        
+        
+        The typical application of this feature is downscaling large densely-sampled trees.
+        In this example we will use a (human) H1N1pdm influenza A dataset with 12,000 taxa.
+        We optimally downsample it while preserving all diversity up to 99.5% sequence similarity, as follows:
+        
+        `parnas -t genbank_H1N1pdm_USA.rooted.tre --cover --radius 0.005 --subtree H1N1pdm.r005.tre`
+        
+        This results in a tree with only 443 taxa! Note that 0.005 distance on a maximum likelihood phylogeny serves here as a proxy for the 0.5% sequence divergence. A downsampled tree will be saved to a new `H1N1pdm.r005.tre` file.
+        The initial 12,000 taxa tree (`genbank_H1N1pdm_USA.rooted.tre`) can be found in the tutorial [folder](tutorial/H1N1pdm_2020.zip).
+        
+        <center>
+        <img src="tutorial/figures/H1N1pdm-downsampling-300.png">
+        <!-- <object data="tutorial/figures/H1N1pdm-downsampling.pdf" type="application/pdf">
+            <embed src="tutorial/figures/H1N1pdm-downsampling.pdf">
+                <p>This browser does not support PDFs. You can view the trees <a href="tutorial/figures/H1N1pdm-downsampling.pdf">here</a>.</p>
+            </embed>
+        </object> -->
+        </center>
+        
+        Below we discuss how PARNAS selects most representative taxa.
+        
+        ### Selecting best representatives ###
+        We use a human H1N1pdm dataset with HA sequences collected in 2020, downloaded from [IRD](fludb.org), for this tutorial.
         The alignment and an inferred rooted tree can be found in the tutorial [folder](tutorial/H1N1pdm_2020.zip).
         
         The basic usage of PARNAS is to find a fixed number of representative taxa, as follows:<br>
         `parnas -t H1N1_human_2020_IRD.rooted.tre -n 3 --color "H1N1_parnas_n3.tre"`<br>
         PARNAS will identify 3 best representative strains and save a colored tree to H1N1_parnas_n3.tre.
         Opening this tree in FigTree, will show the representatives and their respective clusters of strains with different colors. Below is the `H1N1_parnas_n3.tre` output tree, when opened in FigTree. Each color corresponds to one PARNAS-selected representative and the area of the tree it represents.
         
@@ -144,11 +177,12 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `parnas-0.1.2/parnas.egg-info/SOURCES.txt` & `parnas-0.1.3/parnas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parnas-0.1.2/setup.py` & `parnas-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from parnas.version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     install_requires=[
-        'numpy<1.23,>=1.17',
-        'numba==0.55.2',
+        'numpy<=1.24,>=1.17',
+        'numba>=0.57.0',
         'biopython>=1.67',
         'dendropy>=4.5.0',
         'phylo-treetime>=0.9.4'
     ],
     name="parnas",
     version=__version__,
     author="Alexey Markin, Sanket Wagle, Siddhant Grover",
@@ -25,14 +25,15 @@
     packages=["parnas", "parnas.medoids"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["parnas=parnas.cli:run_parnas_cli"]},
     py_modules=["parnas"],
 )
```

