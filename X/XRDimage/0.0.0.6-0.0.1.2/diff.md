# Comparing `tmp/XRDimage-0.0.0.6.tar.gz` & `tmp/XRDimage-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XRDimage-0.0.0.6.tar", last modified: Mon Jul 10 18:14:33 2023, max compression
+gzip compressed data, was "XRDimage-0.0.1.2.tar", last modified: Mon Jul  3 16:04:52 2023, max compression
```

## Comparing `XRDimage-0.0.0.6.tar` & `XRDimage-0.0.1.2.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 18:14:33.131807 XRDimage-0.0.0.6/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/.keep
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/LICENSE
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)     1761 2023-07-10 18:14:33.128168 XRDimage-0.0.0.6/PKG-INFO
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2019 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/README.md
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 18:14:32.996240 XRDimage-0.0.0.6/XRDimage/
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/XRDimage/__init__.py
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      919 2023-07-10 15:28:37.000000 XRDimage-0.0.0.6/XRDimage/center_of_grav.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1171 2023-07-10 15:28:26.000000 XRDimage-0.0.0.6/XRDimage/dark_correction.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1992 2023-07-10 15:28:21.000000 XRDimage-0.0.0.6/XRDimage/ellipse_fitting.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4433 2023-07-10 15:28:10.000000 XRDimage-0.0.0.6/XRDimage/find_center.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2691 2023-07-10 15:26:50.000000 XRDimage-0.0.0.6/XRDimage/image_processing_function.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1968 2023-07-10 15:26:55.000000 XRDimage-0.0.0.6/XRDimage/image_registration.py
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     5091 2023-07-10 16:12:48.000000 XRDimage-0.0.0.6/XRDimage/image_segmentation.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     1497 2023-07-10 15:25:53.000000 XRDimage-0.0.0.6/XRDimage/mask.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     4395 2023-07-10 15:13:42.000000 XRDimage-0.0.0.6/XRDimage/temperature_independent.py
-drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-10 18:14:33.095325 XRDimage-0.0.0.6/XRDimage.egg-info/
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)     1761 2023-07-10 18:14:32.000000 XRDimage-0.0.0.6/XRDimage.egg-info/PKG-INFO
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)      516 2023-07-10 18:14:32.000000 XRDimage-0.0.0.6/XRDimage.egg-info/SOURCES.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-10 18:14:32.000000 XRDimage-0.0.0.6/XRDimage.egg-info/dependency_links.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)       46 2023-07-10 18:14:32.000000 XRDimage-0.0.0.6/XRDimage.egg-info/requires.txt
--rwxrwx---   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-10 18:14:32.000000 XRDimage-0.0.0.6/XRDimage.egg-info/top_level.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/XRDimageDescription.txt
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      855 2023-07-03 15:14:46.000000 XRDimage-0.0.0.6/pyproject.toml
--rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-10 18:14:33.134447 XRDimage-0.0.0.6/setup.cfg
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)     2144 2023-07-10 18:13:10.000000 XRDimage-0.0.0.6/setup.py
--rw-rw----   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.0.6/test
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.403882 XRDimage-0.0.1.2/
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)        6 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/.keep
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1074 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/LICENSE
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      665 2023-07-03 16:04:52.401608 XRDimage-0.0.1.2/PKG-INFO
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2019 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/README.md
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.363072 XRDimage-0.0.1.2/XRDimage/
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      191 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/__init__.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      819 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/dark_correction.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     3874 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/find_center.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     2040 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/image_processing_function.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1711 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/image_registration.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1138 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/mask.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     3513 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimage/temperature_independent.py
+drwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        0 2023-07-03 16:04:52.394410 XRDimage-0.0.1.2/XRDimage.egg-info/
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      665 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/PKG-INFO
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)      430 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       46 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/requires.txt
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)        1 2023-07-03 16:04:51.000000 XRDimage-0.0.1.2/XRDimage.egg-info/top_level.txt
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)       29 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/XRDimageDescription.txt
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      855 2023-07-03 15:14:46.000000 XRDimage-0.0.1.2/pyproject.toml
+-rwxrwxrwx   0 ewf22    (1167172) rxf131   (10097)       38 2023-07-03 16:04:52.406385 XRDimage-0.0.1.2/setup.cfg
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)     1010 2023-07-03 15:27:28.000000 XRDimage-0.0.1.2/setup.py
+-rw-r--r--   0 ewf22    (1167172) rxf131   (10097)      626 2023-07-03 15:13:51.000000 XRDimage-0.0.1.2/test
```

### Comparing `XRDimage-0.0.0.6/LICENSE` & `XRDimage-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.0.6/README.md` & `XRDimage-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.0.6/XRDimage/image_processing_function.py` & `XRDimage-0.0.1.2/XRDimage/image_processing_function.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,69 +7,45 @@
 # relative imports
 from dark_correction import dark_correction
 from find_center import find_center
 from image_registration import register_image
 from temperature_independent import resize_image
 
 def save_img(img, file_path):
-    ''' 
-    Save image as tiff file to specified file path.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param img: PIL image to save.
-    :type img: PIL.Image
-    :param file_path: Complete file path for where to save the file.
-    :type file_path: str
-    :param is_dry_run: Specify whether to perform a dry-run operation (default: False).
-    :type is_dry_run: bool
-    '''
-    # save the file on different directory and filename with categorical suffix
-    final_file_path = file_path.replace('darkCor_', '').replace('.tiff', '_v00_0.tiff')  # TODO: change to regex
-    print('saving result to path --> {}'.format(final_file_path))
-    img.save(final_file_path)
-
-    '''
-    CHANGELOG:
-
-    v0_1 (Jul 23 2022) 
-    '''
+  ''' Save image as tiff file to specified file path.
+  
+  Keyword arguments:
+  
+  img -- PIL image to save
+  file_path -- complete file path for where to save the file
+  is_dry_run -- specify whether to perform a dry-run operation (default: False)
+  '''
+  # save the file on different directory and filename with categorical suffix
+  final_file_path = file_path.replace('darkCor_', '').replace('.tiff', '_v00_0.tiff') # TODO: change to regex
+  print('saving result to path --> {}'.format(final_file_path))
+  img.save(final_file_path)
 
 def image_operations(file_path, output_folder, dark_file_path, ref_img_path):
-    '''
-    Apply preprocessing transformations to image and save to disk.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param file_path: The full file path to the image input.
-    :type file_path: str
-    :param output_folder: The folder for which to save the outputs.
-    :type output_folder: str
-    :param dark_file_path: The full path to the dark file to be used for correction.
-    :type dark_file_path: str
-    :param ref_img_path: Full path to reference image to be used for resizing.
-    :type ref_img_path: str
-    '''
-    try:
-        curr_img = Image.open(file_path)  # open image as numpy array
-        curr_img = dark_correction(curr_img, dark_file_path)  # TODO: add dark file path as required
-        img_center_x, img_center_y = find_center(curr_img)  # find the ring center
-        curr_img = register_image(curr_img, img_center_x, img_center_y)  # register image given center
-        curr_img, ratio_value = resize_image(curr_img, ref_path=ref_img_path)  # resize the image and get the rescale ratio
-
-        print(f'file path: {file_path}')
-        print(f'image center: ({img_center_x}, {img_center_y})')
-        print(f'ratio: {ratio_value}')
-
-        file_name = re.findall('\w+.tiff$', file_path)[0]  # get the file name of the image
-        save_path = join(output_folder, file_name)
-        save_img(curr_img, save_path)  # save the image
-    except Exception as e:
-        print(e)
-
-    '''
-    CHANGELOG:
-
-    v0_1 (Jul 23 2022) 
-    '''
+  '''Apply preprocessing transformations to image and save to disk.
+  
+  Keyword arguments:
+  
+  file_path -- the full file path to the image input
+  output_folder -- the folder for which to save the outputs
+  ref_img_path -- full path to reference image to be used for resize
+  '''
+  try:
+    curr_img = Image.open(file_path) # open image as numpy array
+    curr_img = dark_correction(curr_img, dark_file_path) # TODO: add dark file path as required
+    img_center_x, img_center_y = find_center(curr_img) # find the ring center
+    curr_img = register_image(curr_img, img_center_x, img_center_y) # register image given center
+    curr_img, ratio_value = resize_image(curr_img, ref_path=ref_img_path) # resize the image and get the rescale ratio
+
+    print(f'file path: {file_path}')
+    print(f'image center: ({img_center_x}, {img_center_y})')
+    print(f'ratio: {ratio_value}')
+    
+    file_name = re.findall('\w+.tiff$', file_path)[0] # get the file name of the image
+    save_path = join(output_folder, file_name)
+    save_img(curr_img, save_path) # save the image
+  except Exception as e:
+    print(e)
```

### Comparing `XRDimage-0.0.0.6/XRDimage/image_registration.py` & `XRDimage-0.0.1.2/XRDimage/image_registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from PIL import Image as im
 import numpy as np
 
 def register_image(img, input_center_x, input_center_y):
   '''
-    Outputs a PIL image shifted so that the specified 'true' center
-    coordinates can be found in the geometric center of the image frame.
-    The image is cropped to remove trailing regions and resized to the 
-    original image size.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param img: The input PIL image to center and register.
-    :type img: PIL.Image
-    :param input_center_x: The 'true' center x-coordinate identified for the image.
-    :type input_center_x: float
-    :param input_center_y: The 'true' center y-coordinate identified for the image.
-    :type input_center_y: float
-'''
-
+  Outputs a PIL image shifted so that the specified 'true' center
+  coordinates can be found in the geometric center of the image frame.
+  The image is cropped to remove trailing regions and resized to the 
+  original image size.
+  
+  Keyword arguments:
+  img -- input PIL image to center and register
+  input_center_x -- 'true' center x-coordinate identified for image
+  input_center_t -- 'true' center y-coordinate identified for image
+  '''
   
   ## Define the center of the image and the offset between it and the center of the ring
   dim_x = img.size[0]
   dim_y = img.size[1]
   true_center_x = dim_x/2
   true_center_y = dim_y/2
   offset_x = int(round(true_center_x - input_center_x))
@@ -45,14 +39,8 @@
     new_img = offset_img[0:dim_y + offset_y, offset_x: dim_x]
 
   # convert pixel value array into image
   new_img = im.fromarray(new_img)
 
   # resize the image
   new_img = new_img.resize((dim_x, dim_y))
-  return new_img
-
-  '''
-  CHANGELOG:
-
-  v0_1 (Jul 23 2022) 
-  '''
+  return new_img
```

### Comparing `XRDimage-0.0.0.6/XRDimage/mask.py` & `XRDimage-0.0.1.2/XRDimage/mask.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,31 @@
 import numpy as np
 from PIL import Image as im
 from PIL import ImageOps, ImageChops
 
 from .find_center import create_circular_mask
 
 def define_mask(h=2048, w=2048, inner_radius=40, white_width=8, black_width=10):
-    '''
-    Returns a multiring mask of the given dimensions that can be multiplied to filter an XRD image.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param h: Height of the image.
-    :type h: int
-    :param w: Width of the image.
-    :type w: int
-    :param inner_radius: Inner radius of the first ring.
-    :type inner_radius: int
-    :param white_width: Width of the transparent ring portions for the filter.
-    :type white_width: int
-    :param black_width: Width of the opaque ring portions for the filter.
-    :type black_width: int
-    :return: The resulting multiring mask.
-    :rtype: numpy.ndarray
-    '''
-    # get image mask dimensions
-    # define center mask value
-    center = (int(w/2), int(h/2))
-    # set ring mask parameters
-    result_mask = np.zeros((h,w))
-    # iterate over entire mask to set appropriate values
-    for i in range(0,50):
-        start = inner_radius + (white_width + black_width) * i
-        end = start + white_width
-        raw_mask = create_circular_mask(w,h, outer_radius = end, inner_radius = start)
-        one_array = np.ones((w,h))
-        mask = raw_mask * one_array
-        result_mask = np.add(result_mask, mask)
-    return result_mask
-
-'''
-CHANGELOG:
-
-v0_1 (Jul 23 2022) 
-'''
+  '''Returns a multiring mask of the given dimensions that can be multiplied to filter an XRD image.
+  
+    Keyword arguments:
+    
+    h -- height of image
+    w -- width of the image
+    inner_radius -- inner radius of the first ring
+    white_width -- width of the transparent ring portions for the filter
+    black_width -- width of the opaque ring portions for the filter
+  '''
+  # get image mask dimensions
+  # define center mask value
+  center = (int(w/2), int(h/2))
+  # set ring mask parameters
+  result_mask = np.zeros((h,w))
+  # iterate over entire mask to set appropriate values
+  for i in range(0,50):
+      start = inner_radius + (white_width + black_width) * i
+      end = start + white_width
+      raw_mask = create_circular_mask(w,h, outer_radius = end, inner_radius = start)
+      one_array = np.ones((w,h))
+      mask = raw_mask * one_array
+      result_mask = np.add(result_mask, mask)
+  return result_mask
```

### Comparing `XRDimage-0.0.0.6/XRDimage/temperature_independent.py` & `XRDimage-0.0.1.2/XRDimage/temperature_independent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,110 @@
 from PIL import Image as im
 import numpy as np
 from PIL import ImageOps, ImageChops
 
 
 def add_margin(pil_img, top, right, bottom, left, color):
-    '''
-    Image padding script, to add 300 pixels around the border of an XRD image
-    so the images become 2048 plus 600 square matrices.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param pil_img: Input PIL image to which margins are added.
-    :type pil_img: PIL.Image.Image
-    :param top: Size of the top margin.
-    :type top: int
-    :param right: Size of the right margin.
-    :type right: int
-    :param bottom: Size of the bottom margin.
-    :type bottom: int
-    :param left: Size of the left margin.
-    :type left: int
-    :param color: Color to overlay for margins.
-    :type color: int or tuple
-    :return: Resulting image with added margins.
-    :rtype: PIL.Image.Image
-    '''
-    width, height = pil_img.size
-    new_width = width + right + left
-    new_height = height + top + bottom
-    result = im.new(pil_img.mode, (new_width, new_height), color)
-    result.paste(pil_img, (left, top))
-    return result
+  '''
+  Image padding script, to add 300 pixels around the border of an XRD image
+  so the images become 2048 plus 600 square matrices.
+  
+  Keyword arguments:
+  
+  pil_img -- input PIL image whom to add margins
+  top -- size of the top margin
+  right -- size of the right margin
+  bottom -- size of the bottom margin
+  left -- size of the left margin
+  color -- color to overlay for margins
+  '''
+  width, height = pil_img.size
+  new_width = width + right + left
+  new_height = height + top + bottom
+  result = im.new(pil_img.mode, (new_width, new_height), color)
+  result.paste(pil_img, (left, top))
+  return result
 
 
 def reshape(input_img):
-    '''
-    Change image array shape to fit resize operation.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param input_img: The input PIL image to reshape.
-    :type input_img: PIL.Image.Image
-    :return: Reshaped image array.
-    :rtype: numpy.ndarray
-    '''
-    result_img = input_img.resize((4194304,1))
-    result_img = np.array(result_img)
-    result_img = result_img[0]
-    return result_img
-
+  '''Change image array shape to fit resize operation.
+  
+  Keyword arguments:
+  input_img -- the input PIL image to reshape
+  '''
+  result_img = input_img.resize((4194304,1))
+  result_img = np.array(result_img)
+  result_img = result_img[0]
+  return result_img
 
 def resize_image(img, ref_path, r_only=False, img_only=False, fixed_ratio=None):
-    '''
-    Resize image to desired 2048 x 2048 size by finding optimum ratio.
-    The optimum is determined by minimizing a correlation coefficient between
-    the input image and a reference image.
-
-    Authors:
-        Weiqi Yue, Gabriel Ponon, Zhuldyz Ualikhankyzy, Nathaniel K. Tomczak
-
-    :param img: Input PIL image to resize.
-    :type img: PIL.Image.Image
-    :param ref_path: Full path to the reference image.
-    :type ref_path: str
-    :param r_only: True when the output is the ratio number only. (default: False)
-    :type r_only: bool
-    :param img_only: True when the output is the PIL image only. (default: False)
-    :type img_only: bool
-    :param fixed_ratio: The value to fix the ratio for computation. Set to None to retrieve the ratio value automatically. (default: None)
-    :type fixed_ratio: float or None
-    :return: Resized image or ratio value, depending on the parameters.
-    :rtype: PIL.Image.Image or float
-    '''
-    # add padding to PIL image input
-    im_padding = add_margin(img, 300, 300, 300, 300, 0)
-    ref = im.open(ref_path)
-    C2 = reshape(ref)
-
-    old_size = im_padding.size
-    desired_size = 2048
-
-    # ratio of diameter
-    if fixed_ratio is not None:
-        ratio = np.asarray([fixed_ratio])  # fixed ratio
+  '''
+  Resize image to desired 2048 x 2048 size by finding optimum ratio. 
+  The optimum is determined by minimizing a correlation coefficent between
+  the input image and a reference image.
+  
+  Keyword arguments:
+  img --> input PIL image to resize
+  ref_path --> the full path to the reference image (default: /mnt/rstor/CSE_MSE_RXF131/cradle-members/mdle/wxy215/ti64/ref.tiff)
+  r_only --> true when output is the ratio number only (default: False)
+  img_only --> true when output is the PIL image output only (default: False)
+  fixed_ratio --> the value to fix the ratio value for computation. Set to None to retrieve ratio value automatically (default: None)
+  '''
+  # add padding to PIL image input
+  im_padding = add_margin(img, 300, 300, 300, 300, 0)
+  ref = im.open(ref_path)
+  C2 = reshape(ref)
+
+  old_size = im_padding.size
+  desired_size = 2048
+
+  ### ratio of diameter
+  if fixed_ratio != None:
+    ratio = np.asarray([fixed_ratio]) # fixed ratio
+  else:
+    ratio = np.arange(0.9, 1.1, 0.005)     # create a series of ratios, change parameters here
+
+  max_cor = -99999
+  max_img = np.nan
+
+  # iterate over ratios to find configuration with the lowest correlation
+  for i in ratio:
+    new_size = tuple([int(x * i) for x in old_size]) # set reference size
+
+    ### resize padding image
+    im_re = im_padding.resize(new_size)
+
+    # create a new image and paste the resized on it
+    new_im = im.new(im_padding.mode, (desired_size, desired_size))
+    new_im.paste(im_re, ((desired_size-new_size[0])//2,
+                        (desired_size-new_size[1])//2))
+    max_img = new_im # set max to current since there is only one
+
+    # skip correlation if fixed ratio is no defined
+    
+    if fixed_ratio == None:
+      # with correlation
+      C1 = reshape(new_im)
+      cor = np.corrcoef(C1, C2) # find correlation value between image and reference
+
+      aa = cor[0,1] # FIXME: max_cor might not be in range
+      if max_cor < aa: # set image with min correlation as the new image
+        max_cor = aa
+        max_img = new_im
+        r = i # set min correlation ratio value as output ratio
     else:
-        ratio = np.arange(0.9, 1.1, 0.005)  # create a series of ratios, change parameters here
-
-    max_cor = -99999
-    max_img = np.nan
-
-    # iterate over ratios to find configuration with the lowest correlation
-    for i in ratio:
-        new_size = tuple([int(x * i) for x in old_size])  # set reference size
-
-        # resize padding image
-        im_re = im_padding.resize(new_size)
-
-        # create a new image and paste the resized one onto it
-        new_im = im.new(im_padding.mode, (desired_size, desired_size))
-        new_im.paste(im_re, ((desired_size - new_size[0]) // 2, (desired_size - new_size[1]) // 2))
-        max_img = new_im  # set max to current since there is only one
-
-        # skip correlation if fixed ratio is not defined
-        if fixed_ratio is None:
-            # calculate correlation
-            C1 = reshape(new_im)
-            cor = np.corrcoef(C1, C2)  # find correlation value between image and reference
-            aa = cor[0, 1]
-            if max_cor < aa:
-                max_cor = aa
-                max_img = new_im
-                r = i  # set min correlation ratio value as output ratio
-        else:
-            r = i
-
-    if r_only:
-        return r
-    elif img_only:
-        return max_img
-    else:
-        return max_img, r
+      r = i
+    
+  if r_only:
+      return r
+  elif img_only:
+      return max_img
+  else:
+      return max_img, r
 
 
 '''
 CHANGELOG:
 
 v0_1 (Jul 23 2022) - changed ratio range from 0.95 to 1.05 to 0.9 to 1.1
                    - fixed bad condition for fixed ratio
-'''
+'''
```

### Comparing `XRDimage-0.0.0.6/pyproject.toml` & `XRDimage-0.0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `XRDimage-0.0.0.6/test` & `XRDimage-0.0.1.2/test`

 * *Files identical despite different names*

