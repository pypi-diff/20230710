# Comparing `tmp/siman-1.3.2.tar.gz` & `tmp/siman-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.2.tar", last modified: Mon Jun 26 20:19:36 2023, max compression
+gzip compressed data, was "dist/siman-1.3.3.tar", last modified: Mon Jul 10 09:36:03 2023, max compression
```

## Comparing `siman-1.3.2.tar` & `siman-1.3.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.751793 siman-1.3.2/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.2/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.2/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-26 20:19:36.751793 siman-1.3.2/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.2/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-06-26 20:19:36.751793 siman-1.3.2/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-06-26 20:18:50.000000 siman-1.3.2/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.749793 siman-1.3.2/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.2/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.2/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.2/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49648 2023-06-26 19:04:41.000000 siman-1.3.2/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.2/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.749793 siman-1.3.2/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.2/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.2/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.2/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.2/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   126491 2023-06-26 19:03:27.000000 siman-1.3.2/siman/calc_manage.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.2/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.750793 siman-1.3.2/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.2/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.2/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.2/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.2/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.3.2/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.2/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.750793 siman-1.3.2/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.2/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.2/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.2/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.3.2/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.750793 siman-1.3.2/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.2/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.3.2/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.2/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.3.2/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.2/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.2/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118275 2023-06-08 13:38:57.000000 siman-1.3.2/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-06-26 18:28:07.000000 siman-1.3.2/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.2/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.2/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.3.2/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.2/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.3.2/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.3.2/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.3.2/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.2/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.3.2/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.3.2/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.2/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.751793 siman-1.3.2/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.2/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.2/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.3.2/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.2/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.2/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.2/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.2/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.3.2/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.2/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-06-08 13:41:02.000000 siman-1.3.2/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.2/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.2/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.2/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.2/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.2/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.2/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.3.2/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.2/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.2/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.2/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.2/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.2/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.2/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.2/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-26 20:19:36.749793 siman-1.3.2/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-26 20:19:36.000000 siman-1.3.2/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-06-26 20:19:36.000000 siman-1.3.2/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-06-26 20:19:36.000000 siman-1.3.2/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-06-26 20:19:36.000000 siman-1.3.2/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-06-26 20:19:36.000000 siman-1.3.2/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.3/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.3/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-10 09:36:03.473662 siman-1.3.3/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.3/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-10 09:36:03.473662 siman-1.3.3/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-10 09:35:57.000000 siman-1.3.3/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.3/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.3/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.3/siman/__init__.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49648 2023-06-26 19:04:41.000000 siman-1.3.3/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.3/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.3/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.3/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.3/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   126491 2023-06-26 19:03:27.000000 siman-1.3.3/siman/calc_manage.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.3/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.472662 siman-1.3.3/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.3.3/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.472662 siman-1.3.3/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.3.3/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53311 2023-07-10 09:35:43.000000 siman-1.3.3/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.3.3/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118275 2023-06-08 13:38:57.000000 siman-1.3.3/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-06-26 18:28:07.000000 siman-1.3.3/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.3/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.3/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.3.3/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.3/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.3.3/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.3.3/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.3.3/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.3/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.3.3/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80578 2023-07-03 11:35:20.000000 siman-1.3.3/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.3/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.3/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.3.3/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.3/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.3/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.3/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.3/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.3.3/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.3/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-06-08 13:41:02.000000 siman-1.3.3/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.3/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.3/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.3/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.3.3/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.3/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.3/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.3/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.3/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.3/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.3/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.3/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.2/LICENSE` & `siman-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/PKG-INFO` & `siman-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.2
+Version: 1.3.3
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.2/setup.py` & `siman-1.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.2",
+    version="1.3.3",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.2/siman/3d_plot.py` & `siman-1.3.3/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/SSHTools.py` & `siman-1.3.3/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/analysis.py` & `siman-1.3.3/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/analysis_functions.py` & `siman-1.3.3/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/analyze/segregation.py` & `siman-1.3.3/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/approximation.py` & `siman-1.3.3/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/bands.py` & `siman-1.3.3/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calc_manage.py` & `siman-1.3.3/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calcul.py` & `siman-1.3.3/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calculators/aims.py` & `siman-1.3.3/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calculators/gaussian.py` & `siman-1.3.3/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calculators/qe.py` & `siman-1.3.3/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calculators/vasp.py` & `siman-1.3.3/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/calculators/vasp_old.py` & `siman-1.3.3/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/chg/chg_func.py` & `siman-1.3.3/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.3/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/classes.py` & `siman-1.3.3/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/core/calculation.py` & `siman-1.3.3/siman/core/calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -731,15 +731,15 @@
         ylim = pm.get('ylim') or (-6,7)
         xlim = pm.get('xlim') or (-8,6)
         fontsize = pm.get('fontsize') or 13
         ver_lines = pm.get('ver_lines')
         corner_letter = pm.get('corner_letter')
         orbitals = pm.get('orbitals')
         efermi_origin = pm.get('efermi_origin')
-        nsmooth = pm.get('nsmooth') or 0.0001
+        nsmooth = pm.get('nsmooth') or 1#0.0001
         linewidth = pm.get('linewidth') or 0.8
         efermi_shift = pm.get('efermi_shift') or 0
         labels = pm.get('labels')
         image_name = pm.get('image_name')
         fig_format = pm.get('fig_format') or 'pdf'
         dostype = pm.get('dostype') or 'partial'
         nneighbors = pm.get('nneighbors') or 6
@@ -894,15 +894,15 @@
 
 
                 # print()
                 plot_dos(cl,  iatom = iat+1,  efermi_origin = efermi_origin,
                 dostype = 'partial', orbitals = orbitals, 
                 neighbors = nneighbors,
                 labels = ['', ''], 
-                nsmooth = 1, 
+                nsmooth = nsmooth, 
                 color_dict = color_dicts[i%2],
                 image_name = image_name, 
 
                 # invert_spins = invert_spins,
                 # show_gravity = (1, 'p6', (-10, 10)), 
                 show = 0,  plot_param = {
                 # 'figsize': (6,3),
```

### Comparing `siman-1.3.2/siman/core/calculation_old.py` & `siman-1.3.3/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/core/cluster_batch_script.py` & `siman-1.3.3/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/core/cluster_run_script.py` & `siman-1.3.3/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/core/molecule.py` & `siman-1.3.3/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/core/structure.py` & `siman-1.3.3/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/database.py` & `siman-1.3.3/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/default_project_conf.py` & `siman-1.3.3/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/dev_functions.py` & `siman-1.3.3/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/dos_functions.py` & `siman-1.3.3/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/fit_hex.py` & `siman-1.3.3/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/functions.py` & `siman-1.3.3/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/geo.py` & `siman-1.3.3/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/header.py` & `siman-1.3.3/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/impurity.py` & `siman-1.3.3/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/inout.py` & `siman-1.3.3/siman/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1280,16 +1280,17 @@
 
                     low.append(  float(outcarlines[i_line + kk].split()[4]) )
                     high.append( float(outcarlines[i_line + kk].split()[5]) )
                     kk+=1
 
 
                 if any(v > 1e-3 for v in low+high):
-                    printlog("W(q)/X(q) are too high, check output!\n", 'Y')
+                    printlog("W(q)/X(q) are too high, check output!\n", 'Y') # see here https://www.vasp.at/wiki/index.php/ROPT
                     printlog('Low + high = ', low+high, imp = 'Y' )
+                    printlog('see here https://www.vasp.at/wiki/index.php/ROPT', imp = 'Y' )
                     printlog([v > 1e-3 for v in low+high], imp = 'Y' )
             
             if "direct lattice vectors" in line:
                 if not contcar_read:
                     for v in 0,1,2:
                         line = outcarlines[i_line+1+v]
                         line = line.replace('-', ' -')
```

### Comparing `siman-1.3.2/siman/kpoints_functions.py` & `siman-1.3.3/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/mat_prop/mat_prop.py` & `siman-1.3.3/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/matproj_functions.py` & `siman-1.3.3/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/monte.py` & `siman-1.3.3/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/monte_functions.py` & `siman-1.3.3/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/neb.py` & `siman-1.3.3/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/pairs.py` & `siman-1.3.3/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/picture_functions.py` & `siman-1.3.3/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/plot_functions.py` & `siman-1.3.3/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/polaron.py` & `siman-1.3.3/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/polaron_hop.py` & `siman-1.3.3/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/polaron_mod.py` & `siman-1.3.3/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/project_funcs.py` & `siman-1.3.3/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/properties_2d.py` & `siman-1.3.3/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/properties_energy.py` & `siman-1.3.3/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/properties_lattice.py` & `siman-1.3.3/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/set_functions.py` & `siman-1.3.3/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/simanrc.py` & `siman-1.3.3/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/small_functions.py` & `siman-1.3.3/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/structure_functions.py` & `siman-1.3.3/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/table_functions.py` & `siman-1.3.3/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/thermo.py` & `siman-1.3.3/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman/workflow_utilities.py` & `siman-1.3.3/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.2/siman.egg-info/PKG-INFO` & `siman-1.3.3/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.2
+Version: 1.3.3
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.2/siman.egg-info/SOURCES.txt` & `siman-1.3.3/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

