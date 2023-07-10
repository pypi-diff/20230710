# Comparing `tmp/jianglab-0.5.4.tar.gz` & `tmp/jianglab-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.4.tar", last modified: Mon Jul 10 18:16:40 2023, max compression
+gzip compressed data, was "jianglab-0.5.5.tar", last modified: Mon Jul 10 18:24:02 2023, max compression
```

## Comparing `jianglab-0.5.4.tar` & `jianglab-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.453976 jianglab-0.5.4/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:16:40.453521 jianglab-0.5.4/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.4/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.449048 jianglab-0.5.4/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.4/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    29042 2023-07-10 18:16:07.000000 jianglab-0.5.4/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.4/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.452569 jianglab-0.5.4/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 18:16:40.454118 jianglab-0.5.4/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-10 18:16:22.000000 jianglab-0.5.4/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.592613 jianglab-0.5.5/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:24:02.592280 jianglab-0.5.5/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.5/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.588593 jianglab-0.5.5/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.5/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    29067 2023-07-10 18:23:12.000000 jianglab-0.5.5/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.5/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:24:02.591627 jianglab-0.5.5/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 18:24:02.000000 jianglab-0.5.5/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 18:24:02.592741 jianglab-0.5.5/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-10 18:23:20.000000 jianglab-0.5.5/setup.py
```

### Comparing `jianglab-0.5.4/PKG-INFO` & `jianglab-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.4/README.md` & `jianglab-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.5.4/jianglab/common_functions.py` & `jianglab-0.5.5/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,30 +629,30 @@
 
     # Place the second image onto the canvas, shifted by the specified amount
     stitched[shift_y : shift_y + img2.shape[0], shift_x : shift_x + img2.shape[1]] = img2
 
     return stitched
 
 
-def array_to_video(np_array, filename, save_to_avi = True, display_inline = True, color_map = 'jet'):
+def array_to_video(np_array, filename, frame_rate = 30.0, save_to_avi = True, display_inline = True, color_map = 'jet'):
     """
     Converts a 3D numpy array to a video file and displays it in the notebook.
     :param np_array: 3D numpy array
     :param filename: Name of the video file to be saved
     :param save_to_avi: If True, saves the video to an AVI file
     :param color_map: Color map to be used for the video
     """
 
     # Ensure the array is 3D
     if len(np_array.shape) != 3:
         raise ValueError("Array must be 3-dimensional")
 
     # Define the codec and create a VideoWriter object
     fourcc = cv2.VideoWriter_fourcc(*'DIVX')
-    out = cv2.VideoWriter(filename, fourcc, 20.0, (np_array.shape[2], np_array.shape[1]))
+    out = cv2.VideoWriter(filename, fourcc, frame_rate, (np_array.shape[2], np_array.shape[1]))
 
     # Create a figure for the plot
     fig = plt.figure()
 
     # Function to update figure
     def update_fig(i):
         plt.clf()
```

### Comparing `jianglab-0.5.4/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.5/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.4
+Version: 0.5.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.4/setup.py` & `jianglab-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.4',
+    version='0.5.5',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

