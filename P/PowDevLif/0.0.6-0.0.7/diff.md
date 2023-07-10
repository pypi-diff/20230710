# Comparing `tmp/PowDevLif-0.0.6.tar.gz` & `tmp/PowDevLif-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDevLif-0.0.6.tar", last modified: Wed Jul  5 08:15:00 2023, max compression
+gzip compressed data, was "PowDevLif-0.0.7.tar", last modified: Mon Jul 10 09:51:58 2023, max compression
```

## Comparing `PowDevLif-0.0.6.tar` & `PowDevLif-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:15:00.114840 PowDevLif-0.0.6/
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-05 08:15:00.114840 PowDevLif-0.0.6/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.6/README.md
--rw-------   0 runner    (1000) runner    (1000)      451 2023-07-05 08:14:35.000000 PowDevLif-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-05 08:15:00.114840 PowDevLif-0.0.6/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)     1072 2023-07-05 08:14:32.000000 PowDevLif-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:15:00.102840 PowDevLif-0.0.6/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:15:00.106840 PowDevLif-0.0.6/src/PowDevLif.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-05 08:14:59.000000 PowDevLif-0.0.6/src/PowDevLif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-07-05 08:14:59.000000 PowDevLif-0.0.6/src/PowDevLif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-05 08:14:59.000000 PowDevLif-0.0.6/src/PowDevLif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-05 08:14:59.000000 PowDevLif-0.0.6/src/PowDevLif.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-07-05 08:14:59.000000 PowDevLif-0.0.6/src/PowDevLif.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:15:00.106840 PowDevLif-0.0.6/src/powdevlif/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-05 08:15:00.114840 PowDevLif-0.0.6/src/powdevlif/function/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/counters.py
--rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/cumul_endommagement.py
--rw-------   0 runner    (1000) runner    (1000)     3301 2023-07-05 08:05:20.000000 PowDevLif-0.0.6/src/powdevlif/function/graphs.py
--rw-------   0 runner    (1000) runner    (1000)     3175 2023-07-03 13:39:32.000000 PowDevLif-0.0.6/src/powdevlif/function/losses.py
--rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/materials.py
--rw-------   0 runner    (1000) runner    (1000)     2788 2023-07-05 08:14:19.000000 PowDevLif-0.0.6/src/powdevlif/function/matrix.py
--rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/path_reader.py
--rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.6/src/powdevlif/function/poly_somme.py
--rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.6/src/powdevlif/function/temperature.py
--rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.6/src/powdevlif/function/zth_materials.py
--rw-------   0 runner    (1000) runner    (1000)     3216 2023-07-03 13:46:39.000000 PowDevLif-0.0.6/src/powdevlif/lifetime.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 09:51:58.861092 PowDevLif-0.0.7/
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-10 09:51:58.861092 PowDevLif-0.0.7/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3454 2023-06-23 10:37:14.000000 PowDevLif-0.0.7/README.md
+-rw-------   0 runner    (1000) runner    (1000)      451 2023-07-10 09:51:46.000000 PowDevLif-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-10 09:51:58.861092 PowDevLif-0.0.7/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1072 2023-07-10 09:51:34.000000 PowDevLif-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 09:51:58.849092 PowDevLif-0.0.7/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 09:51:58.849092 PowDevLif-0.0.7/src/PowDevLif.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2023-07-10 09:51:58.000000 PowDevLif-0.0.7/src/PowDevLif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      681 2023-07-10 09:51:58.000000 PowDevLif-0.0.7/src/PowDevLif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-10 09:51:58.000000 PowDevLif-0.0.7/src/PowDevLif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-10 09:51:58.000000 PowDevLif-0.0.7/src/PowDevLif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-07-10 09:51:58.000000 PowDevLif-0.0.7/src/PowDevLif.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 09:51:58.853092 PowDevLif-0.0.7/src/powdevlif/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-10 09:51:58.857092 PowDevLif-0.0.7/src/powdevlif/function/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1051 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/counters.py
+-rw-------   0 runner    (1000) runner    (1000)     2297 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/cumul_endommagement.py
+-rw-------   0 runner    (1000) runner    (1000)     3301 2023-07-05 09:02:28.000000 PowDevLif-0.0.7/src/powdevlif/function/graphs.py
+-rw-------   0 runner    (1000) runner    (1000)     3176 2023-07-05 09:03:53.000000 PowDevLif-0.0.7/src/powdevlif/function/losses.py
+-rw-------   0 runner    (1000) runner    (1000)      350 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/materials.py
+-rw-------   0 runner    (1000) runner    (1000)     2788 2023-07-05 08:14:19.000000 PowDevLif-0.0.7/src/powdevlif/function/matrix.py
+-rw-------   0 runner    (1000) runner    (1000)      430 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/path_reader.py
+-rw-------   0 runner    (1000) runner    (1000)     1115 2023-06-23 10:35:27.000000 PowDevLif-0.0.7/src/powdevlif/function/poly_somme.py
+-rw-------   0 runner    (1000) runner    (1000)     2073 2023-06-23 10:54:01.000000 PowDevLif-0.0.7/src/powdevlif/function/temperature.py
+-rw-------   0 runner    (1000) runner    (1000)     3774 2023-06-23 10:54:01.000000 PowDevLif-0.0.7/src/powdevlif/function/zth_materials.py
+-rw-------   0 runner    (1000) runner    (1000)     3216 2023-07-10 09:51:10.000000 PowDevLif-0.0.7/src/powdevlif/lifetime.py
```

### Comparing `PowDevLif-0.0.6/LICENSE` & `PowDevLif-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/PKG-INFO` & `PowDevLif-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.6
+Version: 0.0.7
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.6/README.md` & `PowDevLif-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/setup.py` & `PowDevLif-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='PowDevLif',
-    version='0.0.6',
+    version='0.0.7',
     description ='The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)',
     readme='README.md',
     license='MIT',
     author='Garnier Paul, Baudais Briac',
     author_email='paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
     packages=find_packages('src'),
```

### Comparing `PowDevLif-0.0.6/src/PowDevLif.egg-info/PKG-INFO` & `PowDevLif-0.0.7/src/PowDevLif.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PowDevLif
-Version: 0.0.6
+Version: 0.0.7
 Summary: The project aims to assess the lifetime and efficiency of electronic components by using thermal and electrical calculations based on data from an Excel file. Authors: Paul Garnier (paul.garnier@ens-rennes.fr), Briac Baudais (briac.baudais@ens-rennes.fr)
 Home-page: https://github.com/PGarn/LifeTime
 Author: Garnier Paul, Baudais Briac
 Author-email: paul.garnier@ens-rennes.fr, briac.baudais@ens-rennes.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PowDevLif-0.0.6/src/PowDevLif.egg-info/SOURCES.txt` & `PowDevLif-0.0.7/src/PowDevLif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/counters.py` & `PowDevLif-0.0.7/src/powdevlif/function/counters.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/cumul_endommagement.py` & `PowDevLif-0.0.7/src/powdevlif/function/cumul_endommagement.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/graphs.py` & `PowDevLif-0.0.7/src/powdevlif/function/graphs.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/losses.py` & `PowDevLif-0.0.7/src/powdevlif/function/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         dic (dict): Dictionary of constants and file parameters
         file (pandas DataFrame): A pandas DataFrame representation of the Excel file
         """
         # Extract relevant data and constants from the provided file and dictionary
         self.i_ref = file.iloc[(dic["excel_starting_row"]-1):(dic["excel_ending_row"]-1), (dic["excel_column_current"]-1)].values
         self.cosphi = file.iloc[(dic["excel_starting_row"]-1):(dic["excel_ending_row"]-1), (dic["excel_column_cosphi"]-1)].values
         self.m = file.iloc[(dic["excel_starting_row"]-1):(dic["excel_ending_row"]-1), (dic["excel_column_m"]-1)].values
+
       
         # Additional constants are also initialized here
         self.Vce0 = dic["Vce0"]
         self.Rce = dic["Rce"]
         self.f_sw = dic["f_sw"]
         self.E_sw = dic["E_sw"]
         self.Iref_sw = dic["Iref_sw"]
```

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/matrix.py` & `PowDevLif-0.0.7/src/powdevlif/function/matrix.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/poly_somme.py` & `PowDevLif-0.0.7/src/powdevlif/function/poly_somme.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/temperature.py` & `PowDevLif-0.0.7/src/powdevlif/function/temperature.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/function/zth_materials.py` & `PowDevLif-0.0.7/src/powdevlif/function/zth_materials.py`

 * *Files identical despite different names*

### Comparing `PowDevLif-0.0.6/src/powdevlif/lifetime.py` & `PowDevLif-0.0.7/src/powdevlif/lifetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   # Display Torque, Speed, Current, Loss through a graph
   # Uncomment this line if you want to show the graphs
   # graph(file,dic,losses,Temp_IGBT,Temp_diode,Temp_case, counter_IGBT, counter_diode)
   
   # Calculate the cumulative damage law
   lifetime_IGBT, lifetime_diode, e_kwh_byhours, efficiency = calculate_damage_cumulation(counter_IGBT, counter_Nf_IGBT, counter_diode, counter_Nf_diode, losses, dic, file)
 
-  results=[["IGBT Cycles",round(lifetime_IGBT,1)],["Diode Cycles",round(lifetime_diode,1)],["Efficiency",round(efficiency,1)]]
+  results=[["IGBT Cycles",round(lifetime_IGBT,1)],["Diode Cycles",round(lifetime_diode,1)],["Efficiency",round(efficiency,2)]]
   
   # Return the calculated lifetimes and other datas
   return (results[0:3]) #add  e_kwh_byhours if you want
 
 def pdl_graphs(variables_file_path):
   """
   This function executes a sequence of calculations related to thermal
```

