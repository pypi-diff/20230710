# Comparing `tmp/ipyvasp-0.6.0.tar.gz` & `tmp/ipyvasp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.6.0.tar", last modified: Wed Jul  5 00:37:19 2023, max compression
+gzip compressed data, was "ipyvasp-0.6.1.tar", last modified: Mon Jul 10 18:46:45 2023, max compression
```

## Comparing `ipyvasp-0.6.0.tar` & `ipyvasp-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     1862 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.721723 ipyvasp-0.6.0/ipyvasp/
--rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.6.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.0/ipyvasp/__main__.py
--rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.0/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    92969 2023-07-04 23:43:08.000000 ipyvasp-0.6.0/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0       23 2023-07-05 00:36:32.000000 ipyvasp-0.6.0/ipyvasp/_version.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.0/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     1590 2023-07-05 00:32:00.000000 ipyvasp-0.6.0/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.761724 ipyvasp-0.6.0/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.0/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.0/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.6.0/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.6.0/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.0/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.0/ipyvasp/evals_dataframe.py
--rw-rw-rw-   0        0        0    22397 2023-07-04 23:42:24.000000 ipyvasp-0.6.0/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.0/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.0/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.6.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:37:19.761724 ipyvasp-0.6.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      203 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 00:37:19.000000 ipyvasp-0.6.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 00:37:19.769721 ipyvasp-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.455264 ipyvasp-0.6.1/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-07-10 18:46:45.454265 ipyvasp-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.425717 ipyvasp-0.6.1/ipyvasp/
+-rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.6.1/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-04 22:54:12.000000 ipyvasp-0.6.1/ipyvasp/__main__.py
+-rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.6.1/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    93200 2023-07-05 18:49:40.000000 ipyvasp-0.6.1/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-07-10 18:46:22.000000 ipyvasp-0.6.1/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.6.1/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     3335 2023-07-10 18:45:22.000000 ipyvasp-0.6.1/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.453265 ipyvasp-0.6.1/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.6.1/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.6.1/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.6.1/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.6.1/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.6.1/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.6.1/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    22397 2023-07-04 23:42:24.000000 ipyvasp-0.6.1/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.6.1/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.6.1/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15225 2023-07-10 18:26:17.000000 ipyvasp-0.6.1/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.6.1/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-10 18:46:45.448205 ipyvasp-0.6.1/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      203 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 18:46:45.000000 ipyvasp-0.6.1/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 18:46:45.455264 ipyvasp-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     3840 2023-07-04 22:57:57.000000 ipyvasp-0.6.1/setup.py
```

### Comparing `ipyvasp-0.6.0/LICENSE` & `ipyvasp-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/PKG-INFO` & `ipyvasp-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.0
+Version: 0.6.1
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.0/README.md` & `ipyvasp-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/__init__.py` & `ipyvasp-0.6.1/ipyvasp/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/_enplots.py` & `ipyvasp-0.6.1/ipyvasp/_enplots.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/_lattice.py` & `ipyvasp-0.6.1/ipyvasp/_lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,14 +547,20 @@
             structures.append(Structure(res))
 
         self.success = True  # set success flag
         return structures
 
 
 def _str2kpoints(kpts_str):
+    try:
+        with open(kpts_str, "r", encoding="utf-8") as f:
+            kpts_str = f.read()
+    except:
+        pass
+
     hsk_list = []
     for j, line in enumerate(kpts_str.splitlines()):
         if line.strip():  # Make sure line is not empty
             data = line.split()
             if len(data) < 3:
                 raise ValueError(f"Line {j + 1} has less than 3 values.")
 
@@ -588,14 +594,15 @@
 
     Parameters
     ----------
     kpoints : list or str
         Any number points as [(x,y,z,[label],[N]), ...]. N adds as many points in current interval.
         To disconnect path at a point, provide it as (x,y,z,[label], 0), next point will be start of other patch.
         If `kpoints` is a multiline string, it is converted to list of points. Each line should be in format "x y z [label] [N]".
+        A file path can be provided to read kpoints from file with same format as multiline string.
     n : int
         Number of point per averge length of `rec_basis`, this makes uniform steps based on distance between points.
         If (x,y,z,[label], N) is provided, this is ignored for that specific interval. If `rec_basis` is not provided, each interval has exactly `n` points.
         Number of points in each interval is at least 2 even if `n` is less than 2 to keep end points anyway.
     weight : float
         None by default to auto generates weights.
     ibzkpt : PathLike
```

### Comparing `ipyvasp-0.6.0/ipyvasp/bsdos.py` & `ipyvasp-0.6.1/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/core/parser.py` & `ipyvasp-0.6.1/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.6.1/ipyvasp/core/plot_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/core/serializer.py` & `ipyvasp-0.6.1/ipyvasp/core/serializer.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.6.1/ipyvasp/core/spatial_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/evals_dataframe.py` & `ipyvasp-0.6.1/ipyvasp/evals_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/lattice.py` & `ipyvasp-0.6.1/ipyvasp/lattice.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/misc.py` & `ipyvasp-0.6.1/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/potential.py` & `ipyvasp-0.6.1/ipyvasp/potential.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp/utils.py` & `ipyvasp-0.6.1/ipyvasp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,23 +94,24 @@
 
     return wrapper
 
 
 @contextmanager
 def set_dir(path: str):
     """Context manager to work in some directory and come back.
-    
+
     >>> with set_dir('some_folder'):
     >>>    do_something()
     >>> # Now you are back in starting directory
     """
     current = os.getcwd()  # not available in pathlib yet
+    abspath = Path(path).resolve(strict=True).absolute()
     try:
-        os.chdir(path)
-        yield
+        os.chdir(abspath)
+        yield abspath
     finally:
         os.chdir(current)
 
 
 def interpolate_data(x: np.ndarray, y: np.ndarray, n: int = 10, k: int = 3) -> tuple:
     """
     Returns interpolated xnew,ynew. If two points are same, it will add 0.1*min(dx>0) to compensate it.
```

### Comparing `ipyvasp-0.6.0/ipyvasp/widgets.py` & `ipyvasp-0.6.1/ipyvasp/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/ipyvasp.egg-info/PKG-INFO` & `ipyvasp-0.6.1/ipyvasp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.6.0
+Version: 0.6.1
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.6.0/ipyvasp.egg-info/SOURCES.txt` & `ipyvasp-0.6.1/ipyvasp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.6.0/setup.py` & `ipyvasp-0.6.1/setup.py`

 * *Files identical despite different names*

