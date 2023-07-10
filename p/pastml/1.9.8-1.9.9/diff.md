# Comparing `tmp/pastml-1.9.8.tar.gz` & `tmp/pastml-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pastml-1.9.8.tar", last modified: Mon Mar  4 15:55:46 2019, max compression
+gzip compressed data, was "dist/pastml-1.9.9.tar", last modified: Tue Mar 12 10:52:30 2019, max compression
```

## Comparing `pastml-1.9.8.tar` & `pastml-1.9.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1636 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/__init__.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)    39332 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/ml.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     2905 2019-03-04 15:10:11.000000 pastml-1.9.8/pastml/file.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml/visualisation/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        0 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/visualisation/__init__.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     8680 2019-02-25 15:03:06.000000 pastml-1.9.8/pastml/visualisation/tree_compressor.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17872 2019-02-25 15:30:45.000000 pastml-1.9.8/pastml/visualisation/cytoscape_manager.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1890 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/visualisation/colour_generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4842 2019-03-04 13:47:10.000000 pastml-1.9.8/pastml/visualisation/generate_geomap.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     7076 2019-03-04 15:34:00.000000 pastml-1.9.8/pastml/visualisation/itol_manager.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)    41003 2019-03-04 15:55:06.000000 pastml-1.9.8/pastml/acr.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml/models/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        0 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/models/__init__.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1737 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/models/generator.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     3844 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/models/jtt.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1501 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/models/hky.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1696 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/models/f81_like.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)    13911 2018-12-07 15:59:24.000000 pastml-1.9.8/pastml/parsimony.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     2035 2018-11-30 14:07:42.000000 pastml-1.9.8/pastml/annotation.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     4408 2019-02-25 15:23:10.000000 pastml-1.9.8/pastml/tree.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml/templates/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      221 2019-02-25 15:27:19.000000 pastml-1.9.8/pastml/templates/time_slider.html
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     7181 2019-02-25 15:46:12.000000 pastml-1.9.8/pastml/templates/pie_tree_simple.js
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     2845 2018-11-28 10:15:50.000000 pastml-1.9.8/pastml/templates/geo_map.html
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4116 2019-02-14 09:24:00.000000 pastml-1.9.8/pastml/templates/index.html
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     9610 2019-02-25 15:46:12.000000 pastml-1.9.8/pastml/templates/pie_tree.js
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5315 2018-11-22 13:57:57.000000 pastml-1.9.8/README.md
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       26 2018-11-15 14:27:59.000000 pastml-1.9.8/MANIFEST.in
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2019-03-04 15:55:46.000000 pastml-1.9.8/setup.cfg
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      840 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/SOURCES.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/dependency_links.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       95 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/entry_points.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       39 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/requires.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        7 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/top_level.txt
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     7356 2019-03-04 15:55:46.000000 pastml-1.9.8/pastml.egg-info/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1291 2019-03-04 15:55:06.000000 pastml-1.9.8/setup.py
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     7356 2019-03-04 15:55:46.000000 pastml-1.9.8/PKG-INFO
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:38.000000 pastml-1.9.9/
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     5315 2019-01-11 13:16:15.000000 pastml-1.9.9/README.md
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml/
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:38.000000 pastml-1.9.9/pastml/visualisation/
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     4842 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/visualisation/generate_geomap.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     7076 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/visualisation/itol_manager.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/visualisation/__init__.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)    17872 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/visualisation/cytoscape_manager.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1890 2019-01-11 13:16:17.000000 pastml-1.9.9/pastml/visualisation/colour_generator.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     8680 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/visualisation/tree_compressor.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     3427 2019-03-12 10:30:06.000000 pastml-1.9.9/pastml/file.py
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:38.000000 pastml-1.9.9/pastml/templates/
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     4116 2019-01-11 13:18:37.000000 pastml-1.9.9/pastml/templates/index.html
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)      221 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/templates/time_slider.html
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     9610 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/templates/pie_tree.js
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     7181 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/templates/pie_tree_simple.js
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     2845 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/templates/geo_map.html
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)    41003 2019-03-12 10:50:45.000000 pastml-1.9.9/pastml/acr.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     4408 2019-03-11 18:37:05.000000 pastml-1.9.9/pastml/tree.py
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml/models/
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1737 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/models/generator.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1501 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/models/hky.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     3844 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/models/jtt.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1696 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/models/f81_like.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/models/__init__.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)    39332 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/ml.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1636 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/__init__.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     2035 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/annotation.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)    13911 2019-01-11 13:16:16.000000 pastml-1.9.9/pastml/parsimony.py
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)       26 2019-01-11 13:16:15.000000 pastml-1.9.9/MANIFEST.in
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)       38 2019-03-12 10:52:38.000000 pastml-1.9.9/setup.cfg
+drwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        0 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)      840 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/SOURCES.txt
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        7 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/top_level.txt
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)        1 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/dependency_links.txt
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     7356 2019-03-12 10:52:36.000000 pastml-1.9.9/pastml.egg-info/PKG-INFO
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)       95 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/entry_points.txt
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)       39 2019-03-12 10:52:37.000000 pastml-1.9.9/pastml.egg-info/requires.txt
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     7356 2019-03-12 10:52:38.000000 pastml-1.9.9/PKG-INFO
+-rwxr-xr-x   0 azhukova  (1000) azhukova  (1000)     1291 2019-03-12 10:50:45.000000 pastml-1.9.9/setup.py
```

### Comparing `pastml-1.9.8/pastml/__init__.py` & `pastml-1.9.9/pastml/__init__.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/ml.py` & `pastml-1.9.9/pastml/ml.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/file.py` & `pastml-1.9.9/pastml/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 import os
 
-from pastml import col_name2cat
-from pastml.ml import is_ml, is_marginal
+from parsimony import is_meta_mp, get_default_mp_method
+from pastml import col_name2cat, get_personalized_feature_name
+from pastml.ml import is_ml, is_marginal, is_meta_ml, get_default_ml_method
 
 PASTML_WORK_DIR = '{tree}_pastml'
 
 COMBINED_ANCESTRAL_STATE_TAB = 'combined_ancestral_states.tab'
 NAMED_TREE_NWK = 'named.tree_{tree}'
 
 PASTML_ML_PARAMS_TAB = 'params.character_{state}.method_{method}.model_{model}.tab'
 PASTML_MP_PARAMS_TAB = 'params.character_{state}.method_{method}.tab'
 PASTML_MARGINAL_PROBS_TAB = 'marginal_probabilities.character_{state}.model_{model}.tab'
 
 
+def get_column_method(column, method):
+    column = col_name2cat(column)
+    if is_meta_ml(method):
+        method = get_default_ml_method()
+    elif is_meta_mp(method):
+        method = get_default_mp_method()
+    else:
+        return column, method
+    return get_personalized_feature_name(column, method), method
+
+
 def get_pastml_parameter_file(method, model, column):
     """
     Get the filename where the PastML parameters are saved
     (for non-ML methods and input parameters will be None, as they have no parameters).
     This file is inside the work_dir that can be specified for the pastml_pipeline method.
 
     :param method: str, the ancestral state prediction method used by PASTML.
     :param model: str, the state evolution model used by PASTML.
     :param column: str, the column for which ancestral states are reconstructed with PASTML.
     :return: str, filename or None for non-ML methods
     """
     ml = is_ml(method)
     template = PASTML_ML_PARAMS_TAB if ml else PASTML_MP_PARAMS_TAB
-    return template.format(state=col_name2cat(column), method=method, model=model)
+    column, method = get_column_method(column, method)
+    return template.format(state=column, method=method, model=model)
 
 
 def get_combined_ancestral_state_file():
     """
     Get the filename where the combined ancestral states are saved (for one or several columns).
     This file is inside the work_dir that can be specified for the pastml_pipeline method.
 
@@ -68,8 +81,9 @@
     :param method: str, the ancestral state prediction method used by PASTML.
     :param model: str, the state evolution model used by PASTML.
     :param column: str, the column for which ancestral states are reconstructed with PASTML.
     :return: str, filename or None if the method is not marginal.
     """
     if not is_marginal(method):
         return None
-    return PASTML_MARGINAL_PROBS_TAB.format(state=col_name2cat(column), model=model)
+    column, method = get_column_method(column, method)
+    return PASTML_MARGINAL_PROBS_TAB.format(state=column, model=model)
```

### Comparing `pastml-1.9.8/pastml/visualisation/tree_compressor.py` & `pastml-1.9.9/pastml/visualisation/tree_compressor.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/visualisation/cytoscape_manager.py` & `pastml-1.9.9/pastml/visualisation/cytoscape_manager.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/visualisation/colour_generator.py` & `pastml-1.9.9/pastml/visualisation/colour_generator.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/visualisation/generate_geomap.py` & `pastml-1.9.9/pastml/visualisation/generate_geomap.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/visualisation/itol_manager.py` & `pastml-1.9.9/pastml/visualisation/itol_manager.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/acr.py` & `pastml-1.9.9/pastml/acr.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
     out_group.add_argument('-p', '--html_compressed', required=False, default=None, type=str,
                            help="path to the output compressed map visualisation file (html).")
     out_group.add_argument('-l', '--html', required=False, default=None, type=str,
                            help="path to the output full tree visualisation file (html).")
     out_group.add_argument('-v', '--verbose', action='store_true',
                            help="print information on the progress of the analysis (to console)")
 
-    parser.add_argument('--version', action='version', version='%(prog)s 1.9.8')
+    parser.add_argument('--version', action='version', version='%(prog)s 1.9.9')
 
     itol_group = parser.add_argument_group('iTOL-related arguments')
     itol_group.add_argument('--upload_to_itol', action='store_true',
                             help="upload the ACR annotated tree to iTOL (https://itol.embl.de/)")
     itol_group.add_argument('--itol_id', required=False, default=None, type=str,
                             help="iTOL user batch upload ID that enables uploading to your iTOL account "
                                  "(see https://itol.embl.de/help.cgi#batch). "
```

### Comparing `pastml-1.9.8/pastml/models/generator.py` & `pastml-1.9.9/pastml/models/generator.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/models/jtt.py` & `pastml-1.9.9/pastml/models/jtt.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/models/hky.py` & `pastml-1.9.9/pastml/models/hky.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/models/f81_like.py` & `pastml-1.9.9/pastml/models/f81_like.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/parsimony.py` & `pastml-1.9.9/pastml/parsimony.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/annotation.py` & `pastml-1.9.9/pastml/annotation.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/tree.py` & `pastml-1.9.9/pastml/tree.py`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/templates/pie_tree_simple.js` & `pastml-1.9.9/pastml/templates/pie_tree_simple.js`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/templates/geo_map.html` & `pastml-1.9.9/pastml/templates/geo_map.html`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/templates/index.html` & `pastml-1.9.9/pastml/templates/index.html`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml/templates/pie_tree.js` & `pastml-1.9.9/pastml/templates/pie_tree.js`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/README.md` & `pastml-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml.egg-info/SOURCES.txt` & `pastml-1.9.9/pastml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastml-1.9.8/pastml.egg-info/PKG-INFO` & `pastml-1.9.9/pastml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pastml
-Version: 1.9.8
+Version: 1.9.9
 Summary: Ancestral character reconstruction and visualisation for rooted phylogenetic trees.
 Home-page: https://github.com/evolbioinfo/pastml
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 License: UNKNOWN
 Description: # pastml
```

### Comparing `pastml-1.9.8/setup.py` & `pastml-1.9.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    version='1.9.8',
+    version='1.9.9',
     description='Ancestral character reconstruction and visualisation for rooted phylogenetic trees.',
     author='Anna Zhukova',
     author_email='anna.zhukova@pasteur.fr',
     url='https://github.com/evolbioinfo/pastml',
     keywords=['PASTML', 'visualisation', 'phylogeny', 'ancestral character reconstruction'],
     install_requires=['ete3', 'pandas', 'numpy', 'jinja2', 'scipy', 'itolapi'],
     entry_points={
```

### Comparing `pastml-1.9.8/PKG-INFO` & `pastml-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pastml
-Version: 1.9.8
+Version: 1.9.9
 Summary: Ancestral character reconstruction and visualisation for rooted phylogenetic trees.
 Home-page: https://github.com/evolbioinfo/pastml
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 License: UNKNOWN
 Description: # pastml
```

