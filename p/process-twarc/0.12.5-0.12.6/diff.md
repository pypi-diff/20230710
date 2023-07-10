# Comparing `tmp/process-twarc-0.12.5.tar.gz` & `tmp/process-twarc-0.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.12.5.tar", last modified: Mon Jul 10 18:41:50 2023, max compression
+gzip compressed data, was "process-twarc-0.12.6.tar", last modified: Mon Jul 10 19:46:18 2023, max compression
```

## Comparing `process-twarc-0.12.5.tar` & `process-twarc-0.12.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:41:50.775330 process-twarc-0.12.5/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.5/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-07-10 18:41:50.775330 process-twarc-0.12.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:41:50.761095 process-twarc-0.12.5/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.5/process_twarc/__init__.py
--rw-rw-rw-   0        0        0     8173 2023-07-09 15:58:02.000000 process-twarc-0.12.5/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:41:50.774094 process-twarc-0.12.5/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      693 2023-07-10 18:41:50.000000 process-twarc-0.12.5/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-10 18:41:50.000000 process-twarc-0.12.5/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:41:50.000000 process-twarc-0.12.5/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-10 18:41:50.000000 process-twarc-0.12.5/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 18:41:50.000000 process-twarc-0.12.5/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-10 18:41:50.781328 process-twarc-0.12.5/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-10 18:41:43.000000 process-twarc-0.12.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:46:18.518546 process-twarc-0.12.6/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.12.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-07-10 19:46:18.519546 process-twarc-0.12.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.12.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 19:46:18.487546 process-twarc-0.12.6/process_twarc/
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.12.6/process_twarc/__init__.py
+-rw-rw-rw-   0        0        0     8446 2023-07-10 19:42:00.000000 process-twarc-0.12.6/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 19:46:18.518546 process-twarc-0.12.6/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-07-10 19:46:18.000000 process-twarc-0.12.6/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-10 19:46:18.000000 process-twarc-0.12.6/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 19:46:18.000000 process-twarc-0.12.6/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-10 19:46:18.000000 process-twarc-0.12.6/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 19:46:18.000000 process-twarc-0.12.6/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-10 19:46:18.522546 process-twarc-0.12.6/setup.cfg
+-rw-rw-rw-   0        0        0      976 2023-07-10 19:46:07.000000 process-twarc-0.12.6/setup.py
```

### Comparing `process-twarc-0.12.5/LICENSE.txt` & `process-twarc-0.12.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.12.5/PKG-INFO` & `process-twarc-0.12.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.5
+Version: 0.12.6
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.5/process_twarc/util.py` & `process-twarc-0.12.6/process_twarc/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,44 +96,57 @@
             table = pq.read_table(file_path)
         dataset = Dataset(table)
     else:
         raise ValueError("Please input a valid output type. Either 'pd' or 'Dataset'.")
 
     return dataset
 
+def merge_lists(*args):
+    """Helper function for load_dataset"""
+    merged_list = [element for arg in args for element in arg]
+    return list(set(merged_list))
+
+
+
 def load_dataset(file_path: str, output_type: str = "pd", columns=None, masks=None, drop_mask_columns=True):
     """
     Load a data structure of the selected type from a parquet file and apply optional masking.
 
     Args:
         file_path (str): Path to the parquet file.
         output_type (str, defaults to "pd"): Type of the output data structure. Either "pd" for pandas DataFrame or "Dataset" for custom Dataset.
         columns (str or list, optional): Columns to load. If provided, only load the specified columns.
         masks (str or list, optional): Mask column(s) to apply and remove rows where the mask is True.
 
     Returns:
         object: Loaded data structure.
     """
+    if columns and isinstance(columns, str):
+        columns = [columns]
+    
     if masks:
         if isinstance(masks, str):
             masks = [masks]
+        if masks and columns:
+            columns = list(set(columns+masks))
+        
         load_type = "pd"
         dataset = load_parquet(file_path, load_type, columns)
         mask = dataset[masks].any(axis=1)
         dataset = dataset[~mask].reset_index(drop=True)
 
         if drop_mask_columns:
             dataset = dataset.drop(columns=masks)
 
         if output_type == "Dataset":
             dataset = Dataset(pa.Table.from_pandas(dataset))
         return dataset
 
     else:
-        dataset = load_parquet(file_path, load_type, columns)
+        dataset = load_parquet(file_path, output_type, columns)
         return dataset
 
 
 def concat_dataset(file_paths, output_type="pd", columns=None, masks=None, drop_mask_columns=True):
     """
     Concatenate multiple datasets from parquet files and apply optional masking.
 
@@ -143,17 +156,14 @@
         columns (str or list[str], optional): Columns to load. If provided, only load the specified columns.
         masks (str or list[str], optional): Mask column(s) to apply and remove rows where the mask is True.
 
     Returns:
         object: Concatenated and optionally masked data structure.
     """
     datasets = []
-
-    if columns and masks:
-        columns = list(set(columns+masks))
     
     for file_path in tqdm(file_paths, desc = "Loading dataset"):
         dataset = load_dataset(file_path, output_type, columns, masks, drop_mask_columns)
         datasets.append(dataset)
     
     concatenated = pd.concat(datasets) if output_type == "pd" else concatenate_datasets(datasets)
```

### Comparing `process-twarc-0.12.5/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.12.6/process_twarc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.12.5
+Version: 0.12.6
 Summary: Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.12.5/setup.py` & `process-twarc-0.12.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'process-twarc',         
   packages = ['process_twarc'],   
-  version = '0.12.5',
+  version = '0.12.6',
   license='MIT',
   description = 'Tools for tranforming raw data from Twarc2 to structured data for Masked Language Modeling.',   # Give a short description about your library
   author = 'Jordan Wolfgang Klein',
   author_email = 'jordan.klein.21@um.edu.mt',
   url = 'https://github.com/user/Lone-Wolfgang',
   keywords = ['Twitter', 'Deduplication', "Tokenization", "Language Modeling"],
   install_requires=[
```

