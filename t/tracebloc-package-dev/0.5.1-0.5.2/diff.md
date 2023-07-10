# Comparing `tmp/tracebloc_package-dev-0.5.1.tar.gz` & `tmp/tracebloc_package-dev-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.1.tar", last modified: Mon Jun 26 09:32:28 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.2.tar", last modified: Mon Jul 10 04:43:01 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.1.tar` & `tracebloc_package-dev-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.833543 tracebloc_package-dev-0.5.1/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.1/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-26 09:32:28.833623 tracebloc_package-dev-0.5.1/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.1/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-26 09:32:28.833845 tracebloc_package-dev-0.5.1/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-23 11:35:27.000000 tracebloc_package-dev-0.5.1/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.832588 tracebloc_package-dev-0.5.1/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.1/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.1/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    24334 2023-06-23 11:37:55.000000 tracebloc_package-dev-0.5.1/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    61330 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-06-23 10:56:15.000000 tracebloc_package-dev-0.5.1/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.1/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.1/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-26 09:32:28.833420 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-26 09:32:28.000000 tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.396218 tracebloc_package-dev-0.5.2/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.2/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-10 04:43:01.396308 tracebloc_package-dev-0.5.2/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.2/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-07-10 04:43:01.396578 tracebloc_package-dev-0.5.2/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-07-10 04:41:35.000000 tracebloc_package-dev-0.5.2/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.395278 tracebloc_package-dev-0.5.2/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.2/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.2/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    24334 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    59315 2023-07-10 04:42:36.000000 tracebloc_package-dev-0.5.2/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.2/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.2/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.2/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.396103 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.1/LICENSE.txt` & `tracebloc_package-dev-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/PKG-INFO` & `tracebloc_package-dev-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.5.1/setup.py` & `tracebloc_package-dev-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.1",
+    version="0.5.2",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/linkModelDataSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -867,241 +867,202 @@
 
     def rotation_range(self, rotation_range: int):
         """
         Int. Degree range for random rotations.
         example: trainingObject.rotation_range(2)
         default: 0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(rotation_range) == int:
-                self.__rotation_range = rotation_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for rotation_range\n"
-                self.__print_error(error_msg)
+        if type(rotation_range) == int:
+            self.__rotation_range = rotation_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("rotation_range")
+            error_msg = "Invalid input type given for rotation_range\n"
+            self.__print_error(error_msg)
 
     def width_shift_range(self, width_shift_range):
         """
         Float or int
         float: fraction of total width, if < 1, or pixels if >= 1.
         int: integer number of pixels from interval (-width_shift_range, +width_shift_range)
         With width_shift_range=2 possible values are integers [-1, 0, +1], same as with width_shift_range=[-1, 0, +1],
         while with width_shift_range=1.0 possible values are floats in the interval [-1.0, +1.0).
         example: trainingObject.width_shift_range(0.1)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(width_shift_range) == float or type(width_shift_range) == int:
-                self.__width_shift_range = width_shift_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for width_shift_range\n"
-                self.__print_error(error_msg)
+        if type(width_shift_range) == float or type(width_shift_range) == int:
+            self.__width_shift_range = width_shift_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("width_shift_range")
+            error_msg = "Invalid input type given for width_shift_range\n"
+            self.__print_error(error_msg)
 
     def height_shift_range(self, height_shift_range):
         """
         Float or int
         float: fraction of total height, if < 1, or pixels if >= 1.
         int: integer number of pixels from interval (-height_shift_range, +height_shift_range)
         With height_shift_range=2 possible values are integers [-1, 0, +1], same as with height_shift_range=[-1, 0, +1],
         while with height_shift_range=1.0 possible values are floats in the interval [-1.0, +1.0).
         example: trainingObject.height_shift_range(0.1)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(height_shift_range) == float or type(height_shift_range) == int:
-                self.__height_shift_range = height_shift_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for height_shift_range\n"
-                self.__print_error(error_msg)
+        if type(height_shift_range) == float or type(height_shift_range) == int:
+            self.__height_shift_range = height_shift_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("height_shift_range")
+            error_msg = "Invalid input type given for height_shift_range\n"
+            self.__print_error(error_msg)
 
     def brightness_range(self, brightness_range):
         """
         Tuple or list of two floats. Range for picking a brightness shift value from.
         example: trainingObject.brightness_range((0.1,0.4))
         default: None
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if (type(brightness_range) == tuple and len(brightness_range) == 2) or (
-                type(brightness_range) == list and len(brightness_range)
-            ) == 2:
-                if (
-                    type(brightness_range[0]) == float
-                    and type(brightness_range[1]) == float
-                ):
-                    brightness_range = str(brightness_range)
-                    self.__brightness_range = brightness_range
-                    self.__remove_error_method()
-                else:
-                    error_msg = "provide float values for brightness_range\n"
-                    self.__print_error(error_msg)
+        if (type(brightness_range) == tuple and len(brightness_range) == 2) or (
+            type(brightness_range) == list and len(brightness_range)
+        ) == 2:
+            if (
+                type(brightness_range[0]) == float
+                and type(brightness_range[1]) == float
+            ):
+                brightness_range = str(brightness_range)
+                self.__brightness_range = brightness_range
+                self.__remove_error_method()
             else:
-                error_msg = "Please provide tuple of two floats for brightness_range\n"
+                error_msg = "provide float values for brightness_range\n"
                 self.__print_error(error_msg)
         else:
-            self.__not_supported_parameters("brightness_range")
+            error_msg = "Please provide tuple of two floats for brightness_range\n"
+            self.__print_error(error_msg)
 
     def shear_range(self, shear_range: float):
         """
         Float. Shear Intensity (Shear angle in counter-clockwise direction in degrees)
         example: trainingObject.shear_range(0.2)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(shear_range) == float:
-                self.__shear_range = shear_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for shear_range\n"
-                self.__print_error(error_msg)
+        if type(shear_range) == float:
+            self.__shear_range = shear_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("shear_range")
+            error_msg = "Invalid input type given for shear_range\n"
+            self.__print_error(error_msg)
 
     def zoom_range(self, zoom_range):
         """
         Float or [lower, upper]. Range for random zoom. If a float, [lower, upper] = [1-zoom_range, 1+zoom_range].
         example: trainingObject.zoom_range(0.2)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(zoom_range) == float or type(zoom_range) == list:
-                self.__zoom_range = zoom_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for zoom_range\n"
-                self.__print_error(error_msg)
+        if type(zoom_range) == float or type(zoom_range) == list:
+            self.__zoom_range = zoom_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("zoom_range")
+            error_msg = "Invalid input type given for zoom_range\n"
+            self.__print_error(error_msg)
 
     def channel_shift_range(self, channel_shift_range: float):
         """
         Float. Range for random channel shifts.
         example: trainingObject.channel_shift_range(0.4)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(channel_shift_range) == float:
-                self.__channel_shift_range = channel_shift_range
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for channel_shift_range\n"
-                self.__print_error(error_msg)
+        if type(channel_shift_range) == float:
+            self.__channel_shift_range = channel_shift_range
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("channel_shift_range")
+            error_msg = "Invalid input type given for channel_shift_range\n"
+            self.__print_error(error_msg)
 
     def fill_mode(self, fill_mode: str):
         """
         One of {"constant", "nearest", "reflect" or "wrap"}. Default is 'nearest'.
         Points outside the boundaries of the input are filled according to the given mode:
         'constant': kkkkkkkk|abcd|kkkkkkkk (cval=k)
         'nearest': aaaaaaaa|abcd|dddddddd
         'reflect': abcddcba|abcd|dcbaabcd
         'wrap': abcdabcd|abcd|abcdabcd
         example: trainingObject.fill_mode("nearest")
         default: "nearest"
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            f = ["constant", "nearest", "reflect", "wrap"]
-            try:
-                f.index(fill_mode.lower())
-                self.__fill_mode = fill_mode.lower()
-                self.__remove_error_method()
-            except:
-                error_msg = f"Please provide supported fill modes: {f}\n"
-                self.__print_error(error_msg)
-        else:
-            self.__not_supported_parameters("fill_mode")
+        f = ["constant", "nearest", "reflect", "wrap"]
+        try:
+            f.index(fill_mode.lower())
+            self.__fill_mode = fill_mode.lower()
+            self.__remove_error_method()
+        except:
+            error_msg = f"Please provide supported fill modes: {f}\n"
+            self.__print_error(error_msg)
 
     def cval(self, cval: float):
         """
         Float or Int. Value used for points outside the boundaries when fill_mode = "constant".
         example: trainingObject.cval(0.3)
         default: 0.0
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(cval) == float:
-                self.__cval = cval
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for cval\n"
-                self.__print_error(error_msg)
+        if type(cval) == float:
+            self.__cval = cval
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("cval")
+            error_msg = "Invalid input type given for cval\n"
+            self.__print_error(error_msg)
 
     def horizontal_flip(self, horizontal_flip: bool):
         """
         Boolean. Randomly flip inputs horizontally.
         example: trainingObject.horizontal_flip(True)
         default: False
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(horizontal_flip) == bool:
-                self.__horizontal_flip = horizontal_flip
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for horizontal_flip\n"
-                self.__print_error(error_msg)
+        if type(horizontal_flip) == bool:
+            self.__horizontal_flip = horizontal_flip
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("horizontal_flip")
+            error_msg = "Invalid input type given for horizontal_flip\n"
+            self.__print_error(error_msg)
 
     def vertical_flip(self, vertical_flip: bool):
         """
         Boolean. Randomly flip inputs vertically.
         example: trainingObject.vertical_flip(True)
         default: False
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(vertical_flip) == bool:
-                self.__vertical_flip = vertical_flip
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for vertical_flip\n"
-                self.__print_error(error_msg)
+        if type(vertical_flip) == bool:
+            self.__vertical_flip = vertical_flip
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("vertical_flip")
+            error_msg = "Invalid input type given for vertical_flip\n"
+            self.__print_error(error_msg)
 
     def rescale(self, rescale: float):
         """
         rescaling factor. Defaults to None. If None, no rescaling is applied,
         otherwise we multiply the data by the value provided (after applying all other transformations).
         example: trainingObject.rescale(0.003921568627)
         default: None
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(rescale) == float:
-                self.__rescale = rescale
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for rescale\n"
-                self.__print_error(error_msg)
+        if type(rescale) == float:
+            self.__rescale = rescale
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("rescale")
+            error_msg = "Invalid input type given for rescale\n"
+            self.__print_error(error_msg)
 
     def shuffle(self, shuffle: bool):
         """
         whether to shuffle the data (default: True)
         example: trainingObject.shuffle(False)
         default: True
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            if type(shuffle) == bool:
-                self.__shuffle = shuffle
-                self.__remove_error_method()
-            else:
-                error_msg = "Invalid input type given for shuffle\n"
-                self.__print_error(error_msg)
+        if type(shuffle) == bool:
+            self.__shuffle = shuffle
+            self.__remove_error_method()
         else:
-            self.__not_supported_parameters("shuffle")
+            error_msg = "Invalid input type given for shuffle\n"
+            self.__print_error(error_msg)
 
     # def category(self, category: str):
     #     """
     #     String.
     #     Category of experiment, like classification
     #     example:trainingObject.category('classification')
     #     default_value: 'Classification'
```

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.2/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.1
+Version: 0.5.2
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.5.1/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

