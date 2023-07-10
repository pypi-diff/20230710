# Comparing `tmp/plakakia-0.1.0.tar.gz` & `tmp/plakakia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plakakia-0.1.0.tar", last modified: Sun May 28 06:40:07 2023, max compression
+gzip compressed data, was "plakakia-0.2.0.tar", last modified: Mon Jul 10 15:08:50 2023, max compression
```

## Comparing `plakakia-0.1.0.tar` & `plakakia-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-05-28 06:40:07.392085 plakakia-0.1.0/
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)    35149 2023-04-07 18:56:29.000000 plakakia-0.1.0/LICENSE
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      212 2023-05-28 06:40:07.392085 plakakia-0.1.0/PKG-INFO
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     5928 2023-05-28 06:14:20.000000 plakakia-0.1.0/README.md
-drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-05-28 06:40:07.392085 plakakia-0.1.0/plakakia/
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      118 2023-05-27 20:31:32.000000 plakakia-0.1.0/plakakia/__init__.py
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     1158 2023-05-27 20:49:00.000000 plakakia-0.1.0/plakakia/config.yaml
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     2264 2023-05-27 20:33:13.000000 plakakia-0.1.0/plakakia/make_some_tiles.py
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     7895 2023-05-27 19:59:28.000000 plakakia-0.1.0/plakakia/settings.py
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     9870 2023-05-24 17:41:11.000000 plakakia-0.1.0/plakakia/utils_annotations.py
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)    13298 2023-05-27 19:59:18.000000 plakakia-0.1.0/plakakia/utils_tiling.py
-drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-05-28 06:40:07.392085 plakakia-0.1.0/plakakia.egg-info/
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      212 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/PKG-INFO
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      393 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/SOURCES.txt
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)        1 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/dependency_links.txt
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)       66 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/entry_points.txt
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      206 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/requires.txt
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)        9 2023-05-28 06:40:07.000000 plakakia-0.1.0/plakakia.egg-info/top_level.txt
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)       38 2023-05-28 06:40:07.392085 plakakia-0.1.0/setup.cfg
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      835 2023-05-27 20:28:54.000000 plakakia-0.1.0/setup.py
-drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-05-28 06:40:07.392085 plakakia-0.1.0/tests/
--rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     7528 2023-05-27 17:18:34.000000 plakakia-0.1.0/tests/test_utils_tiling.py
+drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-07-10 15:08:50.574118 plakakia-0.2.0/
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)    35149 2023-03-27 11:58:54.000000 plakakia-0.2.0/LICENSE
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      212 2023-07-10 15:08:50.574118 plakakia-0.2.0/PKG-INFO
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     7458 2023-05-30 13:27:34.000000 plakakia-0.2.0/README.md
+drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-07-10 15:08:50.574118 plakakia-0.2.0/plakakia/
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      118 2023-05-30 13:27:34.000000 plakakia-0.2.0/plakakia/__init__.py
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     1248 2023-07-10 14:33:52.000000 plakakia-0.2.0/plakakia/config.yaml
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     2268 2023-07-10 13:58:58.000000 plakakia-0.2.0/plakakia/make_some_tiles.py
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     7931 2023-05-31 10:45:31.000000 plakakia-0.2.0/plakakia/settings.py
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)    10842 2023-07-10 14:32:00.000000 plakakia-0.2.0/plakakia/utils_annotations.py
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)     1538 2023-07-10 14:29:35.000000 plakakia-0.2.0/plakakia/utils_images.py
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)    13620 2023-07-10 14:31:41.000000 plakakia-0.2.0/plakakia/utils_tiling.py
+drwxr-xr-x   0 kalfasyan  (1000) kalfasyan  (1000)        0 2023-07-10 15:08:50.574118 plakakia-0.2.0/plakakia.egg-info/
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      212 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/PKG-INFO
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      391 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/SOURCES.txt
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)        1 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/dependency_links.txt
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)       66 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/entry_points.txt
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      206 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/requires.txt
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)        9 2023-07-10 15:08:50.000000 plakakia-0.2.0/plakakia.egg-info/top_level.txt
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)       38 2023-07-10 15:08:50.574118 plakakia-0.2.0/setup.cfg
+-rw-r--r--   0 kalfasyan  (1000) kalfasyan  (1000)      835 2023-07-10 15:02:36.000000 plakakia-0.2.0/setup.py
```

### Comparing `plakakia-0.1.0/LICENSE` & `plakakia-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plakakia-0.1.0/README.md` & `plakakia-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,58 @@
-# plakakia
+# plakakia 
+### /πλακάκια  
 *Python image tiling library for image processing, object detection, etc.*
 
 **DISCLAIMER**: This is a work in progress.  
   
 ![Alt text](logo/logo.png?raw=true "This is a \"plakaki\", meaning tile in Greek.")  
 
-The reason for making this tool is to handle image tiling that takes into account bounding boxes that exist inside the image. For now, I've only considered rectangular tiles. An image is divided into tiles based on a given `tile_size` and `step_size`. Overlapping tiles are handled fine, too. Bounding boxes belong to a tile only if they are *fully* inside it, but I'm planning to support partial overlap as well. Note that such methods create duplicate bounding boxes (i.e. a bounding box can appear in more than one tiles). There is an option for avoiding duplicates. Note that depending on the selection of `tile_size` and `step_size`, there is a potential cost of missing some bounding boxes altogether sincce the duplicate deletion method is strictly applied. Might consider adding more flexible methods in the future.  
-  
-In this package, I employ `multiprocessing` and `numpy` extensively to make this as fast as possible so that one can use it with thousands of images. For benchmarks on some public datasets, see below.  
+## What is this?
+**`plakakia`** was initially developed to address the need for efficient image tiling while considering bounding boxes within the image. It offers a solution for dividing an image into rectangular tiles based on specified tile_size and step_size parameters. Overlapping tiles are handled seamlessly. Currently, the tool assigns bounding boxes to tiles only if they are fully contained within them. However, future updates will include support for partial overlap.
+
+It is worth noting that the tool may generate duplicate bounding boxes as a result of tiling. To mitigate this, `plakakia` offers an option to eliminate duplicates. However, it is important to be aware that, depending on the chosen `tile_size` and `step_size`, there is a potential risk of missing some bounding boxes entirely due to the strict duplicate deletion method. To address this limitation, I am considering the implementation of more flexible methods in the future.  
+
+## What is it going to be?
+Currently, `plakakia` primarily focuses on RGB images in object detection tasks, where the goal is to have tiles that encompass the corresponding bounding boxes. However, I have plans to expand its capabilities to support segmentation tasks as well. This entails tiling both the input images and the associated masks, where each pixel represents a specific category.
+
+In addition, I aim to enhance the tool by providing support for images with more than 3 channels, such as multispectral images. It is important to **note** that `plakakia` already allows online generation of tiles for images with any number of channels (see [examples](examples/) folder). However, offline batch processing is not currently supported.  
+
+So, `plakakia` will hopefully become a versatile tool for tiling images in a variety of tasks using a variety of image formats with the ultimate goal of fast and efficient processing.
 
+## Performance
+To ensure optimal performance, `plakakia` extensively utilizes the `multiprocessing` and `numpy` libraries. This enables efficient processing of thousands of images without the use of nested for-loops which is often applied in tiling tasks. For detailed benchmarks on various public datasets, please refer to the information provided below.
+  
 # Installation
 
 It is **highly** recommended that you create a new virtual environment for the installation:    
  1. Download and install [Mamba](https://mamba.readthedocs.io/en/latest/installation.html) (or [Anaconda](https://www.anaconda.com/products/distribution)). 
  2. Create a virtual environment:  
  `mamba create -n plakakia jupyterlab nb_conda_kernels ipykernel ipywidgets pip -y`  
  3. Activate the environment:  
  `mamba activate plakakia`
 4. Run the following command to install the library:  
-`pip install git+https://github.com/kalfasyan/plakakia.git`  
-**OR** Clone the repository --> `cd plakakia/` --> `pip install .` (don't omit the dot)  
-This will use the setup.py file in the current directory to install the plakakia library along with its dependencies.
+`pip install plakakia`  
 
 # Usage
 
 In this section we cover two main use cases for this library.
 ## A. Offline tile generation with a config file
 This scenario covers the case in which you already have a folder with images and annotations.
  - Make sure you have the plakakia library installed in your Python environment. You can refer to the installation instructions mentioned earlier.
  - Open a terminal or command prompt and activate your Python environment (e.g. `mamba activate plakakia`).
  - Run the following command to execute the make_some_tiles script:  
   > `make_some_tiles --config path/to/config.yaml`  
-
+  ⚠️ When executed, the `make_some_tiles` script removes the following folders from the current location: ['tiles/', 'output/', 'annotations/', 'images/', 'logs/']
 -    Replace *path/to/config.yaml* with the actual path to your configuration file. This file specifies the settings and parameters for the tiling process. Check an example [`config.yaml`](plakakia/config.yaml).  
  - The script will read your `config.yaml` and generate tiles accordingly.  
 
  Check the output directory you specified in the yaml file for results.  
   
 ## B. Online tile generation
-In this scenario you want to apply tiling on images that you have loaded in memory (e.g. during model inference).  
+In this scenario you want to apply tiling on images - *with any number of channels* - that you have loaded in memory (e.g. during model inference).  
 ```
 from plakakia.utils_tiling import tile_image
 import cv2
 import matplotlib.pyplot as plt
 
 # Read image
 img = cv2.imread('../logo/logo.png')
@@ -69,19 +79,21 @@
 Shape of original image: (500, 500, 3)  
 Shape of tiles array: (25, 100, 100, 3)  
 Some coordinates in x1,y1,x2,y2 format:  
 [[  0   0 100 100]  
  [100   0 200 100]  
  [200   0 300 100]]
 ![Alt text](logo/tiles.png?raw=true "The result of the tiling process.")  
+  
 
-
+> ⚠️ For more examples, check the [examples](examples/) folder.   
+    
 # Benchmarks
 
-**Benchmarked on**: AMD Ryzen 5 PRO 6650U; 6 cores; 12 threads; 2.9 GHz
+**Benchmarked on HP Laptop with specs**: AMD Ryzen 5 PRO 6650U; 6 cores; 12 threads; 2.9 GHz
 
 | Dataset | Source | Formats (images/labels) | Number of images | tile_size | step_size | tiles generated | plakakia performance |
 | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
 | Solar Panels v2  | [RoboFlow](https://universe.roboflow.com/roboflow-100/solar-panels-taxvb/dataset/2) | jpg/COCO | 112  | 150 | 50 | 3.075 | 1,11 sec | 
 | Traffic Signs  | [Kaggle](https://www.kaggle.com/datasets/valentynsichkar/traffic-signs-dataset-in-yolo-format) | jpg/YOLO | 741  | 300 | 200 | 1.695 | 2,8 sec | 
 | Hard Hat Workers v2  | [RoboFlow](https://public.roboflow.com/object-detection/hard-hat-workers/2) | jpg/YOLO | 5.269 | 100 | 50 | 21.678 | 6,94 sec| 
 | Microsoft COCO dataset  | [RoboFlow](https://public.roboflow.com/object-detection/microsoft-coco-subset) | jpg/YOLO | 121.408 | 200 | 150 | 177.039 | 3 min 4 sec| 
@@ -92,9 +104,12 @@
  ☑️ ~~Read settings from a file (e.g. json).~~  
  ☑️ ~~Removing all tiles with duplicate bounding boxes (that appear in other tiles).~~  
  ☑️ ~~Support other annotation formats (e.g. coco).~~ (only input for now)  
  ☑️ ~~Provide tiling functionality without any labels needed.~~  
  ⬜️ Add less strict (flexible) duplicate removal methods to avoid missing bounding boxes.  
  ⬜️ Consider bounding boxes in tiles if they *partially* belong to one.  
  ⬜️ Support reading annotations from a dataframe/csv file.  
- ⬜️ Make tiles with multidimensional data (e.g. hdf5 hyperspectral images).  
+ ⬜️ Make tiles with multidimensional data offline with config file (e.g. hdf5 hyperspectral images).  
+ ⬜️ Add support for segmentation tasks (tile both input images and masks).  
   
+# Want to contribute?
+If you want to contribute to this project, please check the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `plakakia-0.1.0/plakakia/config.yaml` & `plakakia-0.2.0/plakakia/config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {
-    "input_extension_images": "png",
-    "output_extension_images": "png",
-    "tile_size": 250, # tile size in pixels
-    "step_size": 100, # step size in pixels for sliding window
-    "input_dir_images": "/home/kalfasyan/data/insect-tiles/images",
-    "input_dir_annotations": "/home/kalfasyan/data/insect-tiles/labels",
-    "input_format_annotations": "yolo", # yolo, pascal_voc or coco
+    "input_extension_images": "jpg",
+    "output_extension_images": "jpg",
+    "tile_size": 70, # tile size in pixels
+    "step_size": 70, # step size in pixels for sliding window
+    "input_dir_images": "/home/kalfasyan/data/Object_Detection/Garbage_plastic/Warp-S/JPEGImages",
+    "input_dir_annotations": "/home/kalfasyan/data/Object_Detection/Garbage_plastic/Warp-S/SegmentationClass",
+    "input_format_annotations": "segmentation", # yolo, pascal_voc, coco or segmentation
     "output_dir_images": "output/images",
     "output_dir_annotations": "output/annotations",
     "output_format_annotations": "yolo", # yolo or pascal_voc
     "annotation_mapping": { # mapping of annotation classes to integers
         "kernel": 0,
         "person": 1,
         "bottle": 2,
@@ -19,10 +19,10 @@
         "crosswalk": 6,
         "stop": 7
     },
     "validate_settings": true, # validate settings before running
     "log": false, # log to file
     "log_folder": "logs", # folder to save logs
     "num_workers": -1, # number of workers for multiprocessing
-    "clear_duplicates": true, # clear duplicate images in the output folder
+    "clear_duplicates": false, # clear duplicate images in the output folder
     "draw_boxes": true, # draw bounding boxes on the output images
 }
```

### Comparing `plakakia-0.1.0/plakakia/make_some_tiles.py` & `plakakia-0.2.0/plakakia/make_some_tiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from pathlib import Path
 from time import perf_counter
 
 import yaml
 from tqdm import tqdm
 
 from .settings import Settings
-from .utils_tiling import clear_duplicates, process_tile
+from .utils_tiling import clear_duplicates, process_tiles
 
 random.seed(3)
 
 
-def process_tile_wrapper(args):
+def process_tiles_wrapper(args):
     """Wrapper function for the process_tile function."""
     t, input_image, input_annotation, settings = args
-    return process_tile(t, input_image, input_annotation, settings)
+    return process_tiles(t, input_image, input_annotation, settings)
 
 
 def main(config_path=None):
     # Delete the tiles and annotations folders if they exist
     [shutil.rmtree(x) if Path(x).exists() else None for x in [
                 'tiles/', 'output/', 'annotations/', 'images/', 'logs/']]
 
@@ -50,15 +50,15 @@
     with mp.Pool(processes=settings.num_workers) as pool:
         # Prepare the arguments for each task
         args = [(t, input_image, input_annotation, settings) \
             for t, (input_image, input_annotation) in \
                 enumerate(zip(settings.input_images, settings.input_annotations))]
 
         # Submit the tasks to the pool
-        results = pool.map(process_tile_wrapper, args)
+        results = pool.map(process_tiles_wrapper, args)
 
     end_time = perf_counter() - start_time
 
     print(f"Finished making tiles! Elapsed time: {end_time:.2f} seconds")
 
     if settings.clear_duplicates:
         clear_duplicates(settings)
```

### Comparing `plakakia-0.1.0/plakakia/settings.py` & `plakakia-0.2.0/plakakia/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     format_to_extension: dict = field(default_factory=dict)
 
     # Define the initialization method of this dataclass
     def __post_init__(self):
         self.format_to_extension = {
             'yolo': 'txt',
             'pascal_voc': 'xml',
-            'coco': 'json'
+            'coco': 'json',
+            'segmentation': 'png',
         }
         assert Path(self.input_dir_images).exists(), \
             f"{self.input_dir_images} image input directory does not exist."
         assert Path(self.input_dir_annotations).exists(), \
             f"{self.input_dir_annotations} annotations directory does not exist."
         # Create the output directories for the images and annotations
         Path(self.output_dir_images).mkdir(parents=True, exist_ok=True)
```

### Comparing `plakakia-0.1.0/plakakia/utils_annotations.py` & `plakakia-0.2.0/plakakia/utils_annotations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import xml.etree.ElementTree as ET
 import os
 import numpy as np
 from tqdm import tqdm
 from pathlib import Path
 import json
+import cv2
 
 def read_pascalvoc_coordinates_from_xml(filename=str, settings=None):
     ''' Read coordinates from PascalVOC xml file. '''
     tree = ET.parse(filename) # type: ignore
     root = tree.getroot()
 
     boxes, classes = [], []
@@ -61,40 +62,40 @@
 
 def read_coco_coordinates_from_json(filename, dir_images) -> pd.DataFrame:
     """Read coordinates from COCO format json file."""
     with open(filename, 'r', encoding='utf-8') as f:
         data = json.load(f)
 
     df_anns = pd.DataFrame(data['annotations'])
-    df_imgs = pd.DataFrame(data['images'])
+    df_ims = pd.DataFrame(data['images'])
     boxes = []
     for annotation in data['annotations']:
         x, y, w, h = annotation['bbox']
         x_1, y_1 = int(x), int(y)
         x_2, y_2 = int(x+w), int(y+h)
         boxes.append([x_1, y_1, x_2, y_2])
 
-    df_merged = pd.merge(df_anns, df_imgs, left_on='image_id', right_on='id')
+    df_merged = pd.merge(df_anns, df_ims, left_on='image_id', right_on='id')
     df_merged['boxes'] = boxes
     df_merged['file_name'] = df_merged['file_name'].apply(lambda x: (Path(dir_images) / x).as_posix())
 
     return df_merged
 
-def read_coordinates_from_annotations(img_path=None, 
+def read_coordinates_from_annotations(im_path=None, 
                                       ant_path=None,
                                       image_shape=None, 
                                       settings=None) -> tuple:
     """ Read coordinates from annotations. """
     if settings.input_format_annotations == 'yolo':
         boxes, classes = read_yolo_coordinates_from_txt(ant_path, image_shape)
     elif settings.input_format_annotations == 'pascal_voc':
         boxes, classes = read_pascalvoc_coordinates_from_xml(ant_path, settings)
     elif settings.input_format_annotations == 'coco':
-        boxes = settings.df_coco.query("file_name == @img_path").boxes.tolist()
-        classes = settings.df_coco.query("file_name == @img_path").category_id.tolist()
+        boxes = settings.df_coco.query("file_name == @im_path").boxes.tolist()
+        classes = settings.df_coco.query("file_name == @im_path").category_id.tolist()
     else:
         raise ValueError(f"Annotation format {settings.input_format_annotations} not supported")
 
     box_classes = [int(i) for i in classes]
 
     return np.array(boxes), box_classes
 
@@ -222,7 +223,28 @@
                          image_height):
     """ Convert YOLO format to XYXY format. """
     x_1 = int((yolo_x - yolo_w/2) * image_width)
     y_1 = int((yolo_y - yolo_h/2) * image_height)
     x_2 = int((yolo_x + yolo_w/2) * image_width)
     y_2 = int((yolo_y + yolo_h/2) * image_height)
     return x_1, y_1, x_2, y_2
+
+def save_image_tiles(filename=None, tiles=None, coordinates=None, settings=None, prefix=None):
+    """ Save the mask tiles. """
+
+    if prefix == 'mask':
+        output_dir = settings.output_dir_annotations
+        extension = settings.output_extension_images
+    elif prefix in ['tile', 'image']:
+        output_dir = settings.output_dir_images
+        extension = settings.output_extension_images
+    else:
+        raise ValueError(f"The prefix is not valid. The only accepted values are 'mask', 'tile' and 'image'.")
+
+    for i, (tile, tile_coord) in tqdm(enumerate(zip(tiles, coordinates)),
+                                       desc="Saving mask tiles",
+                                       total=len(tiles)):
+        # Save the tile
+        file_path = f"{prefix}_{filename}_{tile_coord[0]}_{tile_coord[1]}_{tile_coord[2]}_{tile_coord[3]}.{extension}"
+        save_path = Path(output_dir) / Path(file_path)
+
+        cv2.imwrite(save_path.as_posix(), tile)
```

### Comparing `plakakia-0.1.0/plakakia/utils_tiling.py` & `plakakia-0.2.0/plakakia/utils_tiling.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,36 +4,19 @@
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from .utils_annotations import (convert_yolo_to_xyxy,
-                               read_coordinates_from_annotations,
-                               save_annotations)
+from .utils_annotations import *
+from .utils_images import *
 
 logger = logging.getLogger(__name__)
 
-def add_border(image, settings, color=[0, 0, 0]):
-    """ Add border to an image. """
-
-    top=settings.pad_size
-    bottom=settings.pad_size
-    left=settings.pad_size
-    right=settings.pad_size
-
-    if isinstance(image, str):
-        image = cv2.imread(image)
-
-    # Create border
-    border = cv2.copyMakeBorder(image, top, bottom, left, right, cv2.BORDER_CONSTANT, value=color)
-
-    return border
-
 def tile_image(image, tile_size=250, step_size=50):
     """ Tile an image into overlapping tiles. """
 
     # Compute the number of rows and columns of tiles
     rows = (image.shape[0] - tile_size) // step_size + 1
     cols = (image.shape[1] - tile_size) // step_size + 1
 
@@ -56,66 +39,66 @@
     y_2 = y_1 + tile_size
 
     # Stack the tile indices and coordinates into a single array
     coordinates = np.stack((x_1, y_1, x_2, y_2), axis=-1)
 
     return tiles, coordinates
 
-def get_boxes_inside_tiles(bounding_boxes,
+def get_boxes_inside_tiles(bboxes,
                            tile_coordinates,
                            settings):
     """ Get the bounding boxes that are inside the tiles. """
 
     partial_boxes=settings.check_partial
     overlap_threshold=settings.partial_overlap_threshold
 
     boxes_inside_tiles = [[] for _ in range(len(tile_coordinates))]
 
     for i, tile_coord in enumerate(tile_coordinates):
         if partial_boxes:
             # Create a boolean mask indicating which boxes partially overlap with the tile
-            mask = is_partial_square_inside_array(bounding_boxes,
+            mask = is_partial_square_inside_array(bboxes,
                                                   tile_coord,
                                                   overlap_threshold=overlap_threshold)
         else:
             # Create a boolean mask indicating which boxes are completely inside the tile
-            mask = is_square_inside_array(bounding_boxes, tile_coord)
+            mask = is_square_inside_array(bboxes, tile_coord)
 
         # Add the boxes that satisfy the condition to the corresponding tile
-        boxes_inside_tiles[i] = bounding_boxes[mask].tolist()
+        boxes_inside_tiles[i] = bboxes[mask].tolist()
 
     return boxes_inside_tiles
 
-def is_partial_square_inside_array(bounding_boxes, tile_coord, overlap_threshold=None):
+def is_partial_square_inside_array(bboxes, tile_coord, overlap_threshold=None):
     """ Check if a square is partially inside an array. """
     # Compute the coordinates of the intersection between the box and the tile
-    x_1 = np.maximum(bounding_boxes[:, 0], tile_coord[0])
-    y_1 = np.maximum(bounding_boxes[:, 1], tile_coord[1])
-    x_2 = np.minimum(bounding_boxes[:, 2], tile_coord[2])
-    y_2 = np.minimum(bounding_boxes[:, 3], tile_coord[3])
+    x_1 = np.maximum(bboxes[:, 0], tile_coord[0])
+    y_1 = np.maximum(bboxes[:, 1], tile_coord[1])
+    x_2 = np.minimum(bboxes[:, 2], tile_coord[2])
+    y_2 = np.minimum(bboxes[:, 3], tile_coord[3])
 
     # Compute the areas of the intersection and the box
     intersection_area = (x_2 - x_1) * (y_2 - y_1)
-    box_area = (bounding_boxes[:, 2] - bounding_boxes[:, 0]) * \
-        (bounding_boxes[:, 3] - bounding_boxes[:, 1])
+    box_area = (bboxes[:, 2] - bboxes[:, 0]) * \
+        (bboxes[:, 3] - bboxes[:, 1])
 
     # Compute the overlap between the box and the tile
     overlap = intersection_area / box_area
 
     # Return a boolean mask indicating which boxes have overlap above the threshold
     return overlap > overlap_threshold
 
-def is_square_inside_array(bounding_boxes, tile_coord):
+def is_square_inside_array(bboxes, tile_coord):
     """ Check if a square is completely inside an array. """
     # Return a boolean mask indicating which boxes are inside the tile
     return np.logical_and.reduce((
-        bounding_boxes[:, 0] >= tile_coord[0],
-        bounding_boxes[:, 1] >= tile_coord[1],
-        bounding_boxes[:, 2] <= tile_coord[2],
-        bounding_boxes[:, 3] <= tile_coord[3]
+        bboxes[:, 0] >= tile_coord[0],
+        bboxes[:, 1] >= tile_coord[1],
+        bboxes[:, 2] <= tile_coord[2],
+        bboxes[:, 3] <= tile_coord[3]
     ))
 
 def save_boxes(tiles=np.array([]),
                filename=None,
                coordinates=np.array([]),
                boxes_in_tiles=[],
                box_classes=[],
@@ -184,21 +167,21 @@
 def plot_example_tile_with_yolo_annotation(settings=None):
     """ Plot an example tile with the corresponding YOLO annotation. """
 
     # Get all image files from the tiles folder
     tile_imagepaths = list(Path(settings.output_dir_images).glob('*.{settings.output_extension_images}'))
 
     # Randomly select a tile from tile_imagepaths list
-    img_selection  = random.choice(tile_imagepaths)
-    logger.info(img_selection)
-    assert Path(img_selection).exists(), "does not exist"
-    tile = cv2.imread(str(img_selection))
+    im_selection  = random.choice(tile_imagepaths)
+    logger.info(im_selection)
+    assert Path(im_selection).exists(), "does not exist"
+    tile = cv2.imread(str(im_selection))
 
     # Read the corresponding annotation file
-    annotation_selection = Path(settings.output_dir_annotations) / f"{img_selection.stem}.txt"
+    annotation_selection = Path(settings.output_dir_annotations) / f"{im_selection.stem}.txt"
     logger.info(annotation_selection)
     assert Path(annotation_selection).exists(), "does not exist"
     with open(annotation_selection, mode='r', encoding="utf-8") as file:
         lines = file.readlines()
         for line in lines:
             line = line.strip().split()
             yolo_x = float(line[1])
@@ -214,61 +197,78 @@
             cv2.rectangle(tile, (x_1, y_1), (x_2, y_2), (0, 255, 0), 2)
 
     # Plot the tile in RGB
     tile_rgb = cv2.cvtColor(tile, cv2.COLOR_BGR2RGB)
     plt.imshow(tile_rgb)
     plt.show()
 
-def process_tile(t, input_image, input_annotation, settings=None):
+def process_tiles(t, input_im, input_annotation, settings=None):
     """ The main function to process a tile. """
     # Get the file name
-    file_name = Path(input_image).stem
+    file_name = Path(input_im).stem
 
     # Read the image
-    extension = settings.input_extension_images
-    image_filename = str(Path(settings.input_dir_images).joinpath(f"{file_name}.{extension}"))
-    image = cv2.imread(image_filename)
-
-    # Pad the image if needed
-    if settings.pad_image:
-        image = add_border(image, settings=settings, color=[0, 0, 0])
-    image_shape = image.shape
-
-    # Read the coordinates of the bounding boxes from the annotation files
-    bounding_boxes, box_classes = read_coordinates_from_annotations(img_path=input_image,
-                                                                    ant_path=input_annotation,
-                                                                    image_shape=image_shape,
-                                                                    settings=settings)
+    im = read_input_image(im_fname=file_name, settings=settings)
+
     # Split the image into tiles and get the coordinates of the tiles
-    tiles, coordinates = tile_image(image.copy(),
-                                    tile_size=settings.tile_size,
-                                    step_size=settings.step_size)
-
-    # Get the bounding boxes inside the tiles
-    if bounding_boxes.shape[0] > 0:
-        boxes_in_tiles = get_boxes_inside_tiles(bounding_boxes=bounding_boxes,
-                                                tile_coordinates=coordinates,
-                                                settings=settings)
-    else:
+    tiles, coordinates = tile_image(im.copy(), tile_size=settings.tile_size, step_size=settings.step_size)
+
+    if settings.input_format_annotations == "segmentation":
+        # raise NotImplementedError("Segmentation annotations are not supported yet.")
+        settings.output_format_annotations = "segmentation"
+        # assert spatial dimensions of image and mask are the same
+        mask = read_input_mask(im_fname=file_name, settings=settings)
+        assert (im.shape[0]==mask.shape[0]) and (im.shape[1]==mask.shape[1]), "spatial dimensions of image and mask are not the same"
+        # Split the mask into tiles
+        mask_tiles, mask_coordinates = tile_image(mask.copy(), tile_size=settings.tile_size, step_size=settings.step_size)
+        print(f"mask_tiles.shape: {mask_tiles.shape}")
+        # Save the mask tiles in the output directory for masks
+        save_image_tiles(filename=file_name,
+                        tiles=mask_tiles,
+                        coordinates=mask_coordinates,
+                        settings=settings,
+                        prefix="mask")
+
+        # Save the image tiles in the output directory for images
+        save_image_tiles(filename=file_name,
+                         tiles=tiles,
+                         coordinates=coordinates,
+                         settings=settings,
+                         prefix="tile")        
         return t
 
-    # Generate the tiles with the bounding boxes
-    df_results = save_boxes(filename=file_name,
-                            tiles=tiles,
-                            coordinates=coordinates,
-                            boxes_in_tiles=boxes_in_tiles,
-                            box_classes=box_classes,
-                            settings=settings)
-
-    # Save the annotations in Pascal VOC format or YOLO format
-    save_annotations(df_results,
-                     filename=file_name,
-                     settings=settings,
-                     disable_progress_bar=True)
-    return t
+    else:
+        # Read the coordinates of the bounding boxes from the annotation files
+        bboxes, box_classes = read_coordinates_from_annotations(im_path=input_im, 
+                                                                ant_path=input_annotation, 
+                                                                image_shape=im.shape, 
+                                                                settings=settings)
+
+        # Get the bounding boxes inside the tiles
+        if bboxes.shape[0] > 0:
+            boxes_in_tiles = get_boxes_inside_tiles(bboxes=bboxes,
+                                                    tile_coordinates=coordinates,
+                                                    settings=settings)
+        else:
+            return t
+
+        # Generate the tiles with the bounding boxes
+        df_results = save_boxes(filename=file_name,
+                                tiles=tiles,
+                                coordinates=coordinates,
+                                boxes_in_tiles=boxes_in_tiles,
+                                box_classes=box_classes,
+                                settings=settings)
+
+        # Save the annotations in Pascal VOC format or YOLO format
+        save_annotations(df_results,
+                        filename=file_name,
+                        settings=settings,
+                        disable_progress_bar=True)
+        return t
 
 def clear_duplicates(settings):
     """ Clear the duplicate tiles. """
 
     # Gather all the results from the different processes
     # since settings.duplicates is set to True
     # the results are saved in parquet files
```

### Comparing `plakakia-0.1.0/setup.py` & `plakakia-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup
 
 setup(
     name='plakakia',
-    version='0.1.0',
+    version='0.2.0',
     author='Yannis Kalfas',
     author_email='kalfasyan@gmail.com',
     description='Python image tiling library for image processing, object detection, etc.',
     packages=['plakakia'],
     install_requires=[
         'numpy>=1.24.2',
         'pandas>=1.5.3',
```

