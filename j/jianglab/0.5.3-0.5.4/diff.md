# Comparing `tmp/jianglab-0.5.3.tar.gz` & `tmp/jianglab-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.3.tar", last modified: Mon Jul 10 17:01:05 2023, max compression
+gzip compressed data, was "jianglab-0.5.4.tar", last modified: Mon Jul 10 18:16:40 2023, max compression
```

## Comparing `jianglab-0.5.3.tar` & `jianglab-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.023958 jianglab-0.5.3/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 17:01:05.023358 jianglab-0.5.3/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.3/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.014655 jianglab-0.5.3/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.3/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    27430 2023-07-10 16:30:21.000000 jianglab-0.5.3/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.3/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.022463 jianglab-0.5.3/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      103 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 17:01:05.026667 jianglab-0.5.3/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1020 2023-07-10 16:30:28.000000 jianglab-0.5.3/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.453976 jianglab-0.5.4/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:16:40.453521 jianglab-0.5.4/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.4/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.449048 jianglab-0.5.4/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.4/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    29042 2023-07-10 18:16:07.000000 jianglab-0.5.4/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.4/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 18:16:40.452569 jianglab-0.5.4/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      111 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 18:16:40.000000 jianglab-0.5.4/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 18:16:40.454118 jianglab-0.5.4/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1038 2023-07-10 18:16:22.000000 jianglab-0.5.4/setup.py
```

### Comparing `jianglab-0.5.3/PKG-INFO` & `jianglab-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.3/README.md` & `jianglab-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.5.3/jianglab/common_functions.py` & `jianglab-0.5.4/jianglab/common_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import pandas as pd
 from oauth2client.service_account import ServiceAccountCredentials
 import scipy.signal as signal
 from tqdm import tqdm
 import pickle
 import cv2
 import xmltodict
+import matplotlib.animation as animation
+from IPython.display import HTML
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
@@ -624,8 +626,50 @@
 
     # Place the first image onto the canvas
     stitched[:img1.shape[0], :img1.shape[1]] = img1
 
     # Place the second image onto the canvas, shifted by the specified amount
     stitched[shift_y : shift_y + img2.shape[0], shift_x : shift_x + img2.shape[1]] = img2
 
-    return stitched
+    return stitched
+
+
+def array_to_video(np_array, filename, save_to_avi = True, display_inline = True, color_map = 'jet'):
+    """
+    Converts a 3D numpy array to a video file and displays it in the notebook.
+    :param np_array: 3D numpy array
+    :param filename: Name of the video file to be saved
+    :param save_to_avi: If True, saves the video to an AVI file
+    :param color_map: Color map to be used for the video
+    """
+
+    # Ensure the array is 3D
+    if len(np_array.shape) != 3:
+        raise ValueError("Array must be 3-dimensional")
+
+    # Define the codec and create a VideoWriter object
+    fourcc = cv2.VideoWriter_fourcc(*'DIVX')
+    out = cv2.VideoWriter(filename, fourcc, 20.0, (np_array.shape[2], np_array.shape[1]))
+
+    # Create a figure for the plot
+    fig = plt.figure()
+
+    # Function to update figure
+    def update_fig(i):
+        plt.clf()
+        plt.imshow(np_array[i], cmap=color_map, vmin=0, vmax=255)  # Assumes array values are in range 0-255
+
+    # Create an animation
+    ani = animation.FuncAnimation(fig, update_fig, frames=range(np_array.shape[0]), repeat=False)
+
+    if display_inline:
+        # Convert the animation to HTML video tag and display
+        display(HTML(ani.to_html5_video()))
+
+    # Write each frame to video file
+    if save_to_avi:
+        for i in range(np_array.shape[0]):
+            frame = np_array[i].astype('uint8')  # Ensure data type is uint8
+            out.write(cv2.cvtColor(frame, cv2.COLOR_GRAY2BGR))  # OpenCV uses BGR color space
+
+    # Close the video file
+    out.release()
```

### Comparing `jianglab-0.5.3/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.4/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.3/setup.py` & `jianglab-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.3',
+    version='0.5.4',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
         "tqdm",
         "scipy",
         "gspread",
         "oauth2client",
         "xmltodict",
         "opencv-python",
+        "ipython"
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
```

