# Comparing `tmp/jianglab-0.5.2.tar.gz` & `tmp/jianglab-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.5.2.tar", last modified: Wed Jun 21 16:21:07 2023, max compression
+gzip compressed data, was "jianglab-0.5.3.tar", last modified: Mon Jul 10 17:01:05 2023, max compression
```

## Comparing `jianglab-0.5.2.tar` & `jianglab-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:21:07.328499 jianglab-0.5.2/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 16:21:07.328153 jianglab-0.5.2/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.2/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:21:07.325364 jianglab-0.5.2/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.2/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    22950 2023-06-21 16:20:53.000000 jianglab-0.5.2/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.2/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-21 16:21:07.327542 jianglab-0.5.2/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-21 16:21:07.000000 jianglab-0.5.2/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-21 16:21:07.000000 jianglab-0.5.2/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-21 16:21:07.000000 jianglab-0.5.2/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-21 16:21:07.000000 jianglab-0.5.2/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-21 16:21:07.000000 jianglab-0.5.2/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-21 16:21:07.328654 jianglab-0.5.2/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-21 16:20:58.000000 jianglab-0.5.2/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.023958 jianglab-0.5.3/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 17:01:05.023358 jianglab-0.5.3/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.5.3/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.014655 jianglab-0.5.3/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.5.3/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    27430 2023-07-10 16:30:21.000000 jianglab-0.5.3/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.5.3/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-10 17:01:05.022463 jianglab-0.5.3/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      103 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-10 17:01:04.000000 jianglab-0.5.3/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-10 17:01:05.026667 jianglab-0.5.3/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1020 2023-07-10 16:30:28.000000 jianglab-0.5.3/setup.py
```

### Comparing `jianglab-0.5.2/PKG-INFO` & `jianglab-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.2/README.md` & `jianglab-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.5.2/jianglab/common_functions.py` & `jianglab-0.5.3/jianglab/common_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import matplotlib.pyplot as plt
 import gspread
 import pandas as pd
 from oauth2client.service_account import ServiceAccountCredentials
 import scipy.signal as signal
 from tqdm import tqdm
 import pickle
+import cv2
+import xmltodict
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
@@ -494,7 +496,136 @@
         else:
             waveform_list = [x["waveform"] for x in candidate_list]
             closest_vector_index = find_closest_vector_index(assign_data["waveform"], waveform_list)
             unit_to_assign["units_data"][key]["globalID"] = candidate_list[closest_vector_index]["unitID"]
             used_IDs.append(unit_to_assign["units_data"][key]["globalID"])
     print(used_IDs)
     return unit_to_assign
+
+def fit_ellipse(points):
+    # OpenCV's fitEllipse function expects float32 type
+    points = points.astype(np.float32)
+    # Fit ellipse to points
+    ellipse = cv2.fitEllipse(points)
+    # Return ellipse parameters
+    # Note: the center coordinates are returned as a tuple (x, y)
+    # The axes lengths are returned as a tuple (major_axis, minor_axis)
+    # The rotation angle is in degrees
+    return ellipse
+
+def xml_to_dict(file_path):
+    with open(file_path, 'r') as file:
+        xml_string = file.read()
+    dict_data = xmltodict.parse(xml_string)
+    return dict_data
+
+def rotate_point(point, center, angle):
+    """
+    Rotate a point counterclockwise by a given angle around a given center.
+
+    Args:
+        point (tuple): The original point as (x, y).
+        center (tuple): The rotation center as (x, y).
+        angle (float): The rotation angle in degrees.
+
+    Returns:
+        (new_x, new_y): The rotated point's coordinates.
+    """
+    angle = angle
+    angle = np.deg2rad(angle)  # Convert to radians
+
+    original_x, original_y = point
+    center_x, center_y = center
+
+    # Shift the point so that the center of rotation is at the origin
+    shifted_x = original_x - center_x
+    shifted_y = original_y - center_y
+
+    # Perform the rotation
+    new_x = shifted_x * np.cos(angle) - shifted_y * np.sin(angle)
+    new_y = shifted_x * np.sin(angle) + shifted_y * np.cos(angle)
+
+    # Shift the point back
+    new_x += center_x
+    new_y += center_y
+
+    return new_x, new_y
+
+
+def is_point_in_ellipse(point, center, axes, angle):
+    """
+    Check if a point is within an ellipse.
+
+    Args:
+        point (tuple): The point as (x, y).
+        center (tuple): The center of the ellipse as (x, y).
+        axes (tuple): The lengths of the major and minor axes as (minor, major).
+        angle (float): The rotation angle of the ellipse in degrees.
+
+    Returns:
+        bool: True if the point is in the ellipse, False otherwise.
+    """
+    angle = angle
+    angle = np.deg2rad(angle)  # Convert to radians
+    #swap major and minor axes
+    #axes = (axes[1], axes[0]) # to fit the function requirment of major and minor axes order
+    # Shift the point to the origin
+    shifted_x = point[0] - center[0]
+    shifted_y = point[1] - center[1]
+
+    # Rotate the point to align with the coordinate axes
+    rotated_x = shifted_x * np.cos(angle) + shifted_y * np.sin(angle)
+    rotated_y = -shifted_x * np.sin(angle) + shifted_y * np.cos(angle)
+
+    # Check if the point is in the ellipse
+    return (rotated_x / axes[0]) ** 2 + (rotated_y / axes[1]) ** 2 <= 1
+
+
+def get_cmap(n, name='hsv'):
+    '''Returns a function that maps each index in 0, 1, ..., n-1 to a distinct 
+    RGB color; the keyword argument name must be a standard mpl colormap name.'''
+    return plt.cm.get_cmap(name, n)
+
+def calculate_shift(image1, image2):
+    # Initialize ORB detector
+    orb = cv2.ORB_create()
+
+    # Find keypoints and descriptors with ORB
+    kp1, des1 = orb.detectAndCompute(image1, None)
+    kp2, des2 = orb.detectAndCompute(image2, None)
+
+    # Initialize Brute-Force matcher and exclude outliers using RANSAC
+    bf = cv2.BFMatcher(cv2.NORM_HAMMING, crossCheck=True)
+    matches = bf.match(des1,des2)
+
+    # Sort matches based on their distance
+    matches = sorted(matches, key = lambda x:x.distance)
+
+    # Choose top good matches - this number could be varied
+    good = matches[:10]
+
+    src_pts = np.float32([kp1[m.queryIdx].pt for m in good]).reshape(-1, 1, 2)
+    dst_pts = np.float32([kp2[m.trainIdx].pt for m in good]).reshape(-1, 1, 2)
+
+    # Obtain the homography matrix
+    M, _ = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC,1.0)
+
+    # Translation is at the position (2, 0) and (2, 1) in the Homography matrix
+    dx, dy = M[0, 2], M[1, 2]
+    return dx, dy
+
+def stitch_images_with_shift(img1, img2, shift_x, shift_y):
+    # Calculate dimensions of the output image
+    rows = max(img1.shape[0], img2.shape[0] + abs(shift_y))
+    cols = max(img1.shape[1], img2.shape[1] + abs(shift_x))
+
+    # Create an empty canvas for the output image
+    stitched = np.zeros((rows, cols, img1.shape[2]), dtype=np.uint8)
+    print(stitched.shape)
+
+    # Place the first image onto the canvas
+    stitched[:img1.shape[0], :img1.shape[1]] = img1
+
+    # Place the second image onto the canvas, shifted by the specified amount
+    stitched[shift_y : shift_y + img2.shape[0], shift_x : shift_x + img2.shape[1]] = img2
+
+    return stitched
```

### Comparing `jianglab-0.5.2/jianglab.egg-info/PKG-INFO` & `jianglab-0.5.3/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.5.2/setup.py` & `jianglab-0.5.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.5.2',
+    version='0.5.3',
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
+        "xmltodict",
+        "opencv-python",
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
```

