# Comparing `tmp/pyrarecomb-0.0.3.tar.gz` & `tmp/pyrarecomb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrarecomb-0.0.3.tar", last modified: Thu Jul  6 17:46:57 2023, max compression
+gzip compressed data, was "pyrarecomb-0.1.0.tar", last modified: Mon Jul 10 17:04:58 2023, max compression
```

## Comparing `pyrarecomb-0.0.3.tar` & `pyrarecomb-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:46:57.584766 pyrarecomb-0.0.3/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     1072 2023-07-05 20:39:51.000000 pyrarecomb-0.0.3/LICENSE
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       18 2023-07-06 16:16:04.000000 pyrarecomb-0.0.3/MANIFEST.in
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3555 2023-07-06 17:46:57.586874 pyrarecomb-0.0.3/PKG-INFO
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3074 2023-07-06 16:28:15.000000 pyrarecomb-0.0.3/README.md
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      107 2023-07-06 16:23:38.000000 pyrarecomb-0.0.3/pyproject.toml
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      651 2023-07-06 17:46:57.594843 pyrarecomb-0.0.3/setup.cfg
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:46:57.429627 pyrarecomb-0.0.3/src/
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:46:57.504588 pyrarecomb-0.0.3/src/pyrarecomb/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-05 21:01:50.000000 pyrarecomb-0.0.3/src/pyrarecomb/__init__.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10398 2023-07-06 17:44:23.000000 pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     9595 2023-07-06 17:44:35.000000 pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment_depletion.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10442 2023-07-06 17:44:30.000000 pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment_modifiers.py
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:46:57.576545 pyrarecomb-0.0.3/src/pyrarecomb/utils/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:28:54.000000 pyrarecomb-0.0.3/src/pyrarecomb/utils/__init__.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     6483 2023-07-03 16:24:22.000000 pyrarecomb-0.0.3/src/pyrarecomb/utils/helpers.py
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     2766 2023-07-05 17:25:55.000000 pyrarecomb-0.0.3/src/pyrarecomb/utils/run_apriori_freqitems.py
-drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-06 17:46:57.550184 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     3555 2023-07-06 17:46:57.000000 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/PKG-INFO
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      512 2023-07-06 17:46:57.000000 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/SOURCES.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        1 2023-07-06 17:46:57.000000 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/dependency_links.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       27 2023-07-06 17:46:57.000000 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/requires.txt
--rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       11 2023-07-06 17:46:57.000000 pyrarecomb-0.0.3/src/pyrarecomb.egg-info/top_level.txt
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:04:58.398153 pyrarecomb-0.1.0/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     1072 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/LICENSE
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       18 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/MANIFEST.in
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     4742 2023-07-10 17:04:58.400545 pyrarecomb-0.1.0/PKG-INFO
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     4261 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/README.md
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      107 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/pyproject.toml
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      651 2023-07-10 17:04:58.409216 pyrarecomb-0.1.0/setup.cfg
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:04:58.226469 pyrarecomb-0.1.0/src/
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:04:58.310279 pyrarecomb-0.1.0/src/pyrarecomb/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/__init__.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10430 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     9608 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment_depletion.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)    10459 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment_modifiers.py
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:04:58.388909 pyrarecomb-0.1.0/src/pyrarecomb/utils/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/utils/__init__.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     6483 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/utils/helpers.py
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     2868 2023-07-10 17:03:48.000000 pyrarecomb-0.1.0/src/pyrarecomb/utils/run_apriori_freqitems.py
+drwxrwxr-x   0 dzb5732   (1178) dzb5732   (1178)        0 2023-07-10 17:04:58.358418 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)     4742 2023-07-10 17:04:58.000000 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/PKG-INFO
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)      512 2023-07-10 17:04:58.000000 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/SOURCES.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)        1 2023-07-10 17:04:58.000000 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/dependency_links.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       27 2023-07-10 17:04:58.000000 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/requires.txt
+-rw-rw-r--   0 dzb5732   (1178) dzb5732   (1178)       11 2023-07-10 17:04:58.000000 pyrarecomb-0.1.0/src/pyrarecomb.egg-info/top_level.txt
```

### Comparing `pyrarecomb-0.0.3/LICENSE` & `pyrarecomb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrarecomb-0.0.3/setup.cfg` & `pyrarecomb-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrarecomb
-version = 0.0.3
+version = 0.1.0
 author = Deepro Banerjee
 author_email = deepro.2.4@gmail.com
 description = A python tool to identify oligogenic combinations of genes with rare variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deeprob/pyrarecomb
 classifiers =
```

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment.py` & `pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 from statsmodels.stats.multitest import multipletests
 
 from .utils.run_apriori_freqitems import run_apriori_freqitems
 from .utils import helpers as hp
 
 
 def compare_enrichment(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold, 
+        input_format="Input_", output_format="Output_", pval_filter_threshold=0.05, 
+        adj_pval_type="BH", min_power_threshold=0.7, sample_names_ind="Y", method="fpgrowth"
         ):
     ##########
     # Filter #
     ##########
     apriori_input_cases_df, apriori_input_controls_df, sel_input_colname_list, output_column, number_of_cases = hp.preprocess_boolean(
         boolean_input_df, input_format, output_format, min_indv_threshold, max_freq_threshold
     )
+    num_cases, num_controls, num_genes = len(apriori_input_cases_df), len(apriori_input_controls_df), len(sel_input_colname_list)
     # debugging
-    print(f"Number of cases remaining after filtration: {len(apriori_input_cases_df)}")
-    print(f"Number of controls remaining after filtration: {len(apriori_input_controls_df)}")
-    print(f"Number of items remaining after filtration: {len(sel_input_colname_list)}")
+    print(f"Number of cases remaining after filtration: {num_cases}")
+    print(f"Number of controls remaining after filtration: {num_controls}")
+    print(f"Number of items remaining after filtration: {num_genes}")
+
+    if min(num_cases, num_controls, num_genes)==0:
+        raise ValueError("No samples/items detected: Relax your thresholds")
 
     ############################
     # CASES / SEVERE Phenotype #
     ############################
     # Introduce a support threshold
     support_threshold = min_indv_threshold / apriori_input_cases_df.shape[0]
-    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold)
+    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold, method=method)
     # set the number of frequent items column name 
     case_freqitems_df = case_freqitems_df.rename(columns={"Obs_Count_Combo": "Case_Obs_Count_Combo"})
     # get the number of unique items forming combinations
     uniq_combo_items = set(case_freqitems_df.loc[:, [f"Item_{i}" for i in range(1, combo_length+1)]].values.flatten())
     # Store the counts as a dictionary for each item
     case_freqitems_countdict = dict(zip(case_freqitems_size1_df.Item_1, case_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Get the observed count for each item
@@ -52,15 +57,15 @@
     #############################
     # Get the control profile of the combo items
     apriori_input_controls_df = apriori_input_controls_df.loc[:, list(uniq_combo_items)]
     number_of_controls = apriori_input_controls_df.shape[0]
     # define support threshold for controls
     support_threshold = 2 / number_of_controls
     # get the frequently mutated genes in controls using apriori
-    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold)
+    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold, method=method)
     # set the number of frequent items column name 
     cont_freqitems_df = cont_freqitems_df.rename(columns={"Obs_Count_Combo": "Cont_Obs_Count_Combo"})
     # Store the counts as a dictionary for each item
     cont_freqitems_countdict = dict(zip(cont_freqitems_size1_df.Item_1, cont_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Keep combos found in case only
     case_cont_freqitems_df = case_freqitems_df.merge(cont_freqitems_df, left_on="uniq_items", right_on="uniq_items", how="left", suffixes=('', '_cont')).drop(columns=[f"Item_{i}_cont" for i in range(1, combo_length + 1)]).fillna(0.)
     # Get the observed count in controls for each item
@@ -155,19 +160,11 @@
 if __name__ == "__main__":
     # load the input df
     boolean_input_df = pd.read_csv("/data6/deepro/computational_pipelines/pyrarecomb/test/input/test_input.csv")
     # define all other params
     combo_length = 2
     min_indv_threshold = 5
     max_freq_threshold = 0.25
-    input_format = 'Input_'
-    output_format = 'Output_'
-    pval_filter_threshold = 0.05
-    adj_pval_type = 'BH'
-    min_power_threshold = 0.7
-    sample_names_ind = 'Y'
 
     compare_enrichment(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold, method="fpgrowth"
         )
-
```

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment_depletion.py` & `pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment_depletion.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,34 +5,39 @@
 from statsmodels.stats.multitest import multipletests
 
 from .utils.run_apriori_freqitems import run_apriori_freqitems
 from .utils import helpers as hp
 
 
 def compare_enrichment_depletion(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold, 
+        input_format="Input_", output_format="Output_", pval_filter_threshold=0.05, 
+        adj_pval_type="BH", min_power_threshold=0.7, sample_names_ind="Y", method="fpgrowth"
         ):
     ##########
     # Filter #
     ##########
     apriori_input_cases_df, apriori_input_controls_df, sel_input_colname_list, output_column, number_of_cases = hp.preprocess_boolean(
         boolean_input_df, input_format, output_format, min_indv_threshold, max_freq_threshold
     )
+    num_cases, num_controls, num_genes = len(apriori_input_cases_df), len(apriori_input_controls_df), len(sel_input_colname_list)
     # debugging
-    print(f"Number of cases remaining after filtration: {len(apriori_input_cases_df)}")
-    print(f"Number of controls remaining after filtration: {len(apriori_input_controls_df)}")
-    print(f"Number of items remaining after filtration: {len(sel_input_colname_list)}")
+    print(f"Number of cases remaining after filtration: {num_cases}")
+    print(f"Number of controls remaining after filtration: {num_controls}")
+    print(f"Number of items remaining after filtration: {num_genes}")
+
+    if min(num_cases, num_controls, num_genes)==0:
+        raise ValueError("No samples/items detected: Relax your thresholds")
 
     ############################
     # CASES / SEVERE Phenotype #
     ############################
     # Introduce a support threshold
     support_threshold = min_indv_threshold / apriori_input_cases_df.shape[0]
-    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold)
+    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold, method=method)
     # set the number of frequent items column name 
     case_freqitems_df = case_freqitems_df.rename(columns={"Obs_Count_Combo": "Case_Obs_Count_Combo"})
     # get the number of unique items forming combinations
     uniq_combo_items = set(case_freqitems_df.loc[:, [f"Item_{i}" for i in range(1, combo_length+1)]].values.flatten())
     # Store the counts as a dictionary for each item
     case_freqitems_countdict = dict(zip(case_freqitems_size1_df.Item_1, case_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Get the observed count for each item
@@ -53,15 +58,15 @@
     #############################
     # Get the control profile of the combo items
     apriori_input_controls_df = apriori_input_controls_df.loc[:, list(uniq_combo_items)]
     number_of_controls = apriori_input_controls_df.shape[0]
     # define support threshold for controls
     support_threshold = 2 / number_of_controls
     # get the frequently mutated genes in controls using apriori
-    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold)
+    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold, method=method)
     # set the number of frequent items column name 
     cont_freqitems_df = cont_freqitems_df.rename(columns={"Obs_Count_Combo": "Cont_Obs_Count_Combo"})
     # Store the counts as a dictionary for each item
     cont_freqitems_countdict = dict(zip(cont_freqitems_size1_df.Item_1, cont_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Keep combos found in case only
     case_cont_freqitems_df = case_freqitems_df.merge(cont_freqitems_df, left_on="uniq_items", right_on="uniq_items", how="left", suffixes=('', '_cont')).drop(columns=[f"Item_{i}_cont" for i in range(1, combo_length + 1)]).fillna(0.)
     # Get the observed count in controls for each item
@@ -149,19 +154,11 @@
 if __name__ == "__main__":
     # load the input df
     boolean_input_df = pd.read_csv("/data6/deepro/computational_pipelines/pyrarecomb/test/input/test_input.csv")
     # define all other params
     combo_length = 2
     min_indv_threshold = 5
     max_freq_threshold = 0.25
-    input_format = 'Input_'
-    output_format = 'Output_'
-    pval_filter_threshold = 0.05
-    adj_pval_type = 'BH'
-    min_power_threshold = 0.7
-    sample_names_ind = 'Y'
 
     compare_enrichment_depletion(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold
         )
-
```

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb/compare_enrichment_modifiers.py` & `pyrarecomb-0.1.0/src/pyrarecomb/compare_enrichment_modifiers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,38 +4,44 @@
 from statsmodels.stats.multitest import multipletests
 
 from .utils.run_apriori_freqitems import run_apriori_freqitems
 from .utils import helpers as hp
 
 
 def compare_enrichment_modifiers(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        primary_input_entities, pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold, primary_input_entities,
+        input_format="Input_", output_format="Output_", pval_filter_threshold=0.05, 
+        adj_pval_type="BH", min_power_threshold=0.7, sample_names_ind="Y", method="fpgrowth"
         ):
     ##########
     # Filter #
     ##########
     apriori_input_cases_df, apriori_input_controls_df, sel_input_colname_list, output_column, number_of_cases = hp.preprocess_boolean(
         boolean_input_df, input_format, output_format, min_indv_threshold, max_freq_threshold
     )
     input_colname_only_list = list(set(sel_input_colname_list).difference(set(primary_input_entities)))
     primary_input_list = list(set(sel_input_colname_list).intersection(set(primary_input_entities)))
+    num_cases, num_controls, num_genes = len(apriori_input_cases_df), len(apriori_input_controls_df), len(sel_input_colname_list)
     # debugging
-    print(f"Number of cases remaining after filtration: {len(apriori_input_cases_df)}")
-    print(f"Number of controls remaining after filtration: {len(apriori_input_controls_df)}")
-    print(f"Number of items remaining after filtration: {len(sel_input_colname_list)}")
+    print(f"Number of cases remaining after filtration: {num_cases}")
+    print(f"Number of controls remaining after filtration: {num_controls}")
+    print(f"Number of items remaining after filtration: {num_genes}")
+
+    if min(num_cases, num_controls, num_genes)==0:
+        raise ValueError("No samples/items detected: Relax your thresholds")
+    
     print(f"Number of secondary items remaining after filtration: {len(input_colname_only_list)}")
     print(f"Number of primary items remaining after filtration: {len(primary_input_list)}")
 
     ############################
     # CASES / SEVERE Phenotype #
     ############################
     # Introduce a support threshold
     support_threshold = min_indv_threshold / apriori_input_cases_df.shape[0]
-    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold, primary_entities=primary_input_list)
+    case_freqitems_df, case_freqitems_size1_df = run_apriori_freqitems(apriori_input_cases_df, combo_length, support_threshold, primary_entities=primary_input_list, method=method)
     # set the number of frequent items column name 
     case_freqitems_df = case_freqitems_df.rename(columns={"Obs_Count_Combo": "Case_Obs_Count_Combo"})
     # get the number of unique items forming combinations
     uniq_combo_items = set(case_freqitems_df.loc[:, [f"Item_{i}" for i in range(1, combo_length+1)]].values.flatten())
     # Store the counts as a dictionary for each item
     case_freqitems_countdict = dict(zip(case_freqitems_size1_df.Item_1, case_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Get the observed count for each item
@@ -57,15 +63,15 @@
     # Get the control profile of the combo items
     apriori_input_controls_df = apriori_input_controls_df.loc[:, list(uniq_combo_items)]
     number_of_controls = apriori_input_controls_df.shape[0]
     # define support threshold for controls
     support_threshold = 2 / number_of_controls
     # get the frequently mutated genes in controls using apriori
     sel_primary_input_list = uniq_combo_items.intersection(primary_input_list)
-    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold, primary_entities=sel_primary_input_list)
+    cont_freqitems_df, cont_freqitems_size1_df = run_apriori_freqitems(apriori_input_controls_df, combo_length, support_threshold, primary_entities=sel_primary_input_list, method=method)
     # set the number of frequent items column name 
     cont_freqitems_df = cont_freqitems_df.rename(columns={"Obs_Count_Combo": "Cont_Obs_Count_Combo"})
     # Store the counts as a dictionary for each item
     cont_freqitems_countdict = dict(zip(cont_freqitems_size1_df.Item_1, cont_freqitems_size1_df.Obs_Count_Combo.astype(int)))
     # Keep combos found in case only
     case_cont_freqitems_df = case_freqitems_df.merge(cont_freqitems_df, left_on="uniq_items", right_on="uniq_items", how="left", suffixes=('', '_cont')).drop(columns=[f"Item_{i}_cont" for i in range(1, combo_length + 1)]).fillna(0.)
     # Get the observed count in controls for each item
@@ -155,20 +161,12 @@
     # load the input df
     boolean_input_df = pd.read_csv("/data6/deepro/computational_pipelines/pyrarecomb/test/input/test_input.csv")
     primary_inputs = pd.read_csv("/data6/deepro/computational_pipelines/pyrarecomb/test/input/primary.txt", header=None).iloc[:, 0].values
     # define all other params
     combo_length = 2
     min_indv_threshold = 5
     max_freq_threshold = 0.25
-    input_format = 'Input_'
-    output_format = 'Output_'
-    pval_filter_threshold = 0.05
-    adj_pval_type = 'BH'
-    min_power_threshold = 0.7
-    sample_names_ind = 'Y'
     primary_input_entities= primary_inputs
 
     compare_enrichment_modifiers(
-        boolean_input_df, combo_length, input_format, output_format, min_indv_threshold, max_freq_threshold,
-        primary_input_entities, pval_filter_threshold, adj_pval_type, min_power_threshold, sample_names_ind
+        boolean_input_df, combo_length, min_indv_threshold, max_freq_threshold, primary_input_entities
         )
-
```

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb/utils/helpers.py` & `pyrarecomb-0.1.0/src/pyrarecomb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb/utils/run_apriori_freqitems.py` & `pyrarecomb-0.1.0/src/pyrarecomb/utils/run_apriori_freqitems.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import reduce
 import pandas as pd
-from mlxtend.frequent_patterns import apriori, association_rules
+from mlxtend.frequent_patterns import apriori, fpgrowth, association_rules
 
 
 def get_freq_items_combo(frequent_itemsets, combo_length):
     # get items of specific combo size
     frequent_itemsets = frequent_itemsets.loc[frequent_itemsets.length==combo_length].drop(columns=["length"])
     # Split itemsets into separate columns
     frequent_itemsets = frequent_itemsets.merge(frequent_itemsets['itemsets'].apply(lambda x: pd.Series(list(x))), left_index=True, right_index=True).drop(columns=["support", "itemsets"])
@@ -13,16 +13,17 @@
     new_colnames = [f"Item_{i}" for i in range(1, combo_length+1)]
     frequent_itemsets = frequent_itemsets.rename(columns=dict(zip(old_colnames, new_colnames)))
     return frequent_itemsets.loc[:, new_colnames + ["uniq_items", "Obs_Count_Combo"]].reset_index(drop=True)
 
 def add_frozensets(a, b):
     return a.union(b)  
 
-def run_apriori_freqitems(apriori_input_df, combo_length, support_threshold, primary_entities=None):
-    frequent_itemsets = apriori(
+def run_apriori_freqitems(apriori_input_df, combo_length, support_threshold, primary_entities=None, method="fpgrowth"):
+    method_dict = {"apriori": apriori, "fpgrowth": fpgrowth}
+    frequent_itemsets = method_dict[method](
         apriori_input_df.astype(bool), min_support=support_threshold, 
         use_colnames=True, max_len=combo_length
         )
     if primary_entities is not None:
         # run association rules
         assoc_df = association_rules(frequent_itemsets, metric="confidence", min_threshold=0.0)
         # the primary entities must be in the consequents only
```

### Comparing `pyrarecomb-0.0.3/src/pyrarecomb.egg-info/SOURCES.txt` & `pyrarecomb-0.1.0/src/pyrarecomb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

