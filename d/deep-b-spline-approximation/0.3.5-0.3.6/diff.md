# Comparing `tmp/deep-b-spline-approximation-0.3.5.tar.gz` & `tmp/deep-b-spline-approximation-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-b-spline-approximation-0.3.5.tar", last modified: Mon Jul 10 21:22:52 2023, max compression
+gzip compressed data, was "deep-b-spline-approximation-0.3.6.tar", last modified: Mon Jul 10 21:43:40 2023, max compression
```

## Comparing `deep-b-spline-approximation-0.3.5.tar` & `deep-b-spline-approximation-0.3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 21:22:52.435517 deep-b-spline-approximation-0.3.5/
--rw-rw-rw-   0        0        0     1095 2022-01-23 21:17:54.000000 deep-b-spline-approximation-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     1062 2023-07-10 21:22:52.433504 deep-b-spline-approximation-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      390 2022-07-02 17:04:35.000000 deep-b-spline-approximation-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 21:22:52.401943 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/
--rw-rw-rw-   0        0        0    13779 2022-01-23 20:48:16.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/BSpline.py
--rw-rw-rw-   0        0        0      154 2022-01-23 20:48:16.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-07-10 21:19:50.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/__main__.py
--rw-rw-rw-   0        0        0     6452 2022-07-10 14:44:28.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/deep_b_spline_approximation.py
--rw-rw-rw-   0        0        0     2521 2022-03-06 16:59:01.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/directedHausdorff.py
--rw-rw-rw-   0        0        0     6137 2022-01-23 20:48:17.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/evalmodel.py
--rw-rw-rw-   0        0        0     4150 2022-03-06 16:58:36.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/kpn.py
--rw-rw-rw-   0        0        0      705 2022-01-23 20:48:17.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/loadfromtxt.py
--rw-rw-rw-   0        0        0    32255 2022-03-06 16:58:20.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/ppn.py
--rw-rw-rw-   0        0        0    29741 2022-07-10 15:13:53.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/preprocessing.py
--rw-rw-rw-   0        0        0     3230 2022-01-23 20:48:29.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/resumetraining.py
--rw-rw-rw-   0        0        0     7887 2022-01-23 20:48:29.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/training.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:22:52.428546 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-07-10 21:22:52.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-07-10 21:22:52.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:22:52.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-10 21:22:52.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-10 21:22:52.000000 deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 21:22:52.436497 deep-b-spline-approximation-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-07-10 21:20:00.000000 deep-b-spline-approximation-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:43:40.153778 deep-b-spline-approximation-0.3.6/
+-rw-rw-rw-   0        0        0     1095 2022-01-23 21:17:54.000000 deep-b-spline-approximation-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0     1062 2023-07-10 21:43:40.150492 deep-b-spline-approximation-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2022-07-02 17:04:35.000000 deep-b-spline-approximation-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 21:43:40.115690 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/
+-rw-rw-rw-   0        0        0    13779 2022-01-23 20:48:16.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/BSpline.py
+-rw-rw-rw-   0        0        0      154 2022-01-23 20:48:16.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/__init__.py
+-rw-rw-rw-   0        0        0     2517 2023-07-10 21:37:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/__main__.py
+-rw-rw-rw-   0        0        0     6452 2022-07-10 14:44:28.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/deep_b_spline_approximation.py
+-rw-rw-rw-   0        0        0     2521 2022-03-06 16:59:01.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/directedHausdorff.py
+-rw-rw-rw-   0        0        0     6137 2022-01-23 20:48:17.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/evalmodel.py
+-rw-rw-rw-   0        0        0     4150 2022-03-06 16:58:36.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/kpn.py
+-rw-rw-rw-   0        0        0      705 2022-01-23 20:48:17.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/loadfromtxt.py
+-rw-rw-rw-   0        0        0    32255 2022-03-06 16:58:20.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/ppn.py
+-rw-rw-rw-   0        0        0    29741 2022-07-10 15:13:53.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/preprocessing.py
+-rw-rw-rw-   0        0        0     3230 2022-01-23 20:48:29.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/resumetraining.py
+-rw-rw-rw-   0        0        0     7887 2022-01-23 20:48:29.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/training.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:43:40.145524 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-07-10 21:43:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-07-10 21:43:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:43:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-10 21:43:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-10 21:43:39.000000 deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 21:43:40.153778 deep-b-spline-approximation-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-07-10 21:38:02.000000 deep-b-spline-approximation-0.3.6/setup.py
```

### Comparing `deep-b-spline-approximation-0.3.5/LICENSE` & `deep-b-spline-approximation-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/PKG-INFO` & `deep-b-spline-approximation-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep-b-spline-approximation
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python package for bspline curve approximation using deep learning
 Home-page: https://github.com/t-ceccarini/deep-b-spline-approximation
 Author: Tommaso Ceccarini
 Author-email: <tceccarini93@gmail.com>
 License: UNKNOWN
-Download-URL: https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.5.tar.gz
+Download-URL: https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.6.tar.gz
 Keywords: python,deep learning,mlp,cnn,cagd,bspline,bezier
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/BSpline.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/BSpline.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/__main__.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     
     print("Downloaded models")
     
 def download_evalsets(output_dir):
     print("Downloading evalsets")
     
     download_file('https://github.com/t-ceccarini/deep-b-spline-approximation/blob/master/evalsets/evalset1.txt?raw=true',
-                  os.path.join(output_dir,'ppn_mlp1.pt'))
+                  os.path.join(output_dir,'evalset1.txt'))
     download_file('https://github.com/t-ceccarini/deep-b-spline-approximation/blob/master/evalsets/evalset2.txt?raw=true',
-                  os.path.join(output_dir,'kpn_mlp4.pt'))
+                  os.path.join(output_dir,'evalset2.txt'))
     
     download_file('https://github.com/t-ceccarini/deep-b-spline-approximation/blob/master/evalsets/evalset3.txt?raw=true',
-                  os.path.join(output_dir,'ppn_cnn1.pt'))
+                  os.path.join(output_dir,'evalset3.txt'))
     
     download_file('https://github.com/t-ceccarini/deep-b-spline-approximation/blob/master/evalsets/evalset4.txt?raw=true',
-                  os.path.join(output_dir,'ppn_cnn1.pt'))
+                  os.path.join(output_dir,'evalset4.txt'))
     
     print("Downloaded evalsets")
 
 def main():
     
     if sys.argv[1] == 'download-models':
         os.makedirs(os.path.join(os.path.dirname(os.path.realpath(__file__)),'models'))
```

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/deep_b_spline_approximation.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/deep_b_spline_approximation.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/directedHausdorff.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/directedHausdorff.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/evalmodel.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/evalmodel.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/kpn.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/kpn.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/loadfromtxt.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/loadfromtxt.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/ppn.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/ppn.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/preprocessing.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/resumetraining.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/resumetraining.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation/training.py` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation/training.py`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/PKG-INFO` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deep-b-spline-approximation
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python package for bspline curve approximation using deep learning
 Home-page: https://github.com/t-ceccarini/deep-b-spline-approximation
 Author: Tommaso Ceccarini
 Author-email: <tceccarini93@gmail.com>
 License: UNKNOWN
-Download-URL: https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.5.tar.gz
+Download-URL: https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.6.tar.gz
 Keywords: python,deep learning,mlp,cnn,cagd,bspline,bezier
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deep-b-spline-approximation-0.3.5/deep_b_spline_approximation.egg-info/SOURCES.txt` & `deep-b-spline-approximation-0.3.6/deep_b_spline_approximation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep-b-spline-approximation-0.3.5/setup.py` & `deep-b-spline-approximation-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 """
 Created on Thu Jan 13 23:29:22 2022
 
 @author: Tommaso
 """
 from setuptools import setup
 
-VERSION = '0.3.5'
+VERSION = '0.3.6'
 DESCRIPTION = 'A python package for bspline curve approximation using deep learning'
 
 # Setting up
 setup(
     name='deep-b-spline-approximation',
     packages=['deep_b_spline_approximation'],
     version=VERSION,
     author="Tommaso Ceccarini",
     author_email="<tceccarini93@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/t-ceccarini/deep-b-spline-approximation',
-    download_url='https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.5.tar.gz',
+    download_url='https://github.com/t-ceccarini/deep-b-spline-approximation/archive/refs/tags/v_0.3.6.tar.gz',
     install_requires=['torch','prettytable','numpy','scipy','matplotlib'],
     keywords=['python', 'deep learning', 'mlp', 'cnn', 'cagd', 'bspline', 'bezier'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
```

