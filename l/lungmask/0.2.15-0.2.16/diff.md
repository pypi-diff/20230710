# Comparing `tmp/lungmask-0.2.15.tar.gz` & `tmp/lungmask-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungmask-0.2.15.tar", last modified: Thu Jun 15 06:09:22 2023, max compression
+gzip compressed data, was "lungmask-0.2.16.tar", last modified: Mon Jul 10 19:31:54 2023, max compression
```

## Comparing `lungmask-0.2.15.tar` & `lungmask-0.2.16.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 06:09:11.000000 lungmask-0.2.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-15 06:09:22.337246 lungmask-0.2.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-15 06:09:11.000000 lungmask-0.2.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.333246 lungmask-0.2.15/lungmask/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/resunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-06-15 06:09:11.000000 lungmask-0.2.15/lungmask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/lungmask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 06:09:22.000000 lungmask-0.2.15/lungmask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 06:09:11.000000 lungmask-0.2.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:09:22.337246 lungmask-0.2.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-15 06:09:11.000000 lungmask-0.2.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:09:22.337246 lungmask-0.2.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-15 06:09:11.000000 lungmask-0.2.15/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:54.381039 lungmask-0.2.16/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:31:43.000000 lungmask-0.2.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-10 19:31:54.381039 lungmask-0.2.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-10 19:31:43.000000 lungmask-0.2.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:54.377039 lungmask-0.2.16/lungmask/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/resunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-10 19:31:43.000000 lungmask-0.2.16/lungmask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:54.381039 lungmask-0.2.16/lungmask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 19:31:54.000000 lungmask-0.2.16/lungmask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-10 19:31:43.000000 lungmask-0.2.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:31:54.381039 lungmask-0.2.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-10 19:31:43.000000 lungmask-0.2.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:54.381039 lungmask-0.2.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-10 19:31:43.000000 lungmask-0.2.16/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-10 19:31:43.000000 lungmask-0.2.16/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-10 19:31:43.000000 lungmask-0.2.16/tests/test_utils.py
```

### Comparing `lungmask-0.2.15/LICENSE` & `lungmask-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.15/PKG-INFO` & `lungmask-0.2.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.15
+Version: 0.2.16
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
 Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lungmask-0.2.15/README.md` & `lungmask-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.15/lungmask/__main__.py` & `lungmask-0.2.16/lungmask/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
-import logging
 import os
 import sys
 
 import numpy as np
 import pkg_resources  # type: ignore
 import SimpleITK as sitk
 
 from lungmask import LMInferer, utils
+from lungmask.logger import logger
 
 
 def path(string):
     if os.path.exists(string):
         return string
     else:
         sys.exit(f"File not found: {string}")
@@ -82,26 +82,26 @@
         version=version,
     )
 
     argsin = sys.argv[1:]
     args = parser.parse_args(argsin)
 
     if args.classes is not None:
-        logging.warn(
+        logger.warn(
             "!!! Warning: The `classes` parameter is deprecated and will be removed in the next version !!!"
         )
 
     batchsize = args.batchsize
     if args.cpu:
         batchsize = 1
 
-    logging.info("Load model")
+    logger.info("Load model")
 
     input_image = utils.load_input_image(args.input, disable_tqdm=args.noprogress)
-    logging.info("Infer lungmask")
+    logger.info("Infer lungmask")
     if args.modelname == "LTRCLobes_R231":
         assert (
             args.modelpath is None
         ), "Modelpath can not be specified for LTRCLobes_R231 mode"
         inferer = LMInferer(
             modelname="LTRCLobes",
             force_cpu=args.cpu,
@@ -128,14 +128,14 @@
         file_ending = args.output.split(".")[-1]
         if file_ending in ["jpg", "jpeg", "png"]:
             result = (result / (result.max()) * 255).astype(np.uint8)
         result = result[0]
 
     result_out = sitk.GetImageFromArray(result)
     result_out.CopyInformation(input_image)
-    logging.info(f"Save result to: {args.output}")
+    logger.info(f"Save result to: {args.output}")
     sitk.WriteImage(result_out, args.output)
 
 
 if __name__ == "__main__":
     print("called as script")
     main()
```

### Comparing `lungmask-0.2.15/lungmask/mask.py` & `lungmask-0.2.16/lungmask/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import logging
 import os
 import sys
 import warnings
 from typing import Optional, Union
 
 import numpy as np
 import SimpleITK as sitk
 import skimage
 import torch
 from more_itertools import chunked
 from tqdm import tqdm
 
 from lungmask import utils
+from lungmask.logger import logger
 
 from .resunet import UNet
 
-logging.basicConfig(
-    stream=sys.stdout,
-    format="lungmask %(asctime)s %(message)s",
-    datefmt="%Y-%m-%d %H:%M:%S",
-    level=logging.INFO,
-)
-
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 # stores urls and number of classes of the models
 MODEL_URLS = {
     "R231": (
         "https://github.com/JoHof/lungmask/releases/download/v0.0/unet_r231-d5d2fc3d.pth",
@@ -126,15 +119,15 @@
         self.model = get_model(self.modelname, modelpath)
 
         self.device = torch.device("cpu")
         if not self.force_cpu:
             if torch.cuda.is_available():
                 self.device = torch.device("cuda")
             else:
-                logging.info("No GPU found, using CPU instead")
+                logger.info("No GPU found, using CPU instead")
         self.model.to(self.device)
 
         self.fillmodelm = None
         if self.fillmodel is not None:
             self.fillmodelm = get_model(self.fillmodel, fillmodel_path)
             self.fillmodelm.to(self.device)
 
@@ -237,22 +230,22 @@
 
         Returns:
             np.ndarray: Lung segmentation
         """
         if self.fillmodel is None:
             return self._inference(image, self.model)
         else:
-            logging.info(f"Apply: {self.modelname}")
+            logger.info(f"Apply: {self.modelname}")
             res_l = self._inference(image, self.model)
-            logging.info(f"Apply: {self.fillmodel}")
+            logger.info(f"Apply: {self.fillmodel}")
             res_r = self._inference(image, self.fillmodelm)
             spare_value = res_l.max() + 1
             res_l[np.logical_and(res_l == 0, res_r > 0)] = spare_value
             res_l[res_r == 0] = 0
-            logging.info("Fusing results... this may take up to several minutes!")
+            logger.info("Fusing results... this may take up to several minutes!")
             return utils.postprocessing(res_l, spare=[spare_value])
 
 
 def apply(
     image: Union[sitk.Image, np.ndarray],
     model=None,
     force_cpu=False,
```

### Comparing `lungmask-0.2.15/lungmask/resunet.py` & `lungmask-0.2.16/lungmask/resunet.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.15/lungmask/utils.py` & `lungmask-0.2.16/lungmask/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import logging
 import os
 import sys
 from typing import Tuple
 
 import fill_voids
 import numpy as np
 import pydicom as pyd
 import SimpleITK as sitk
 import skimage.measure
 import skimage.morphology
 from scipy import ndimage
 from torch.utils.data import Dataset
 from tqdm import tqdm
 
+from lungmask.logger import logger
+
 
 def preprocess(
     img: np.ndarray, resolution: list = [192, 192]
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Preprocesses the image by clipping, cropping and resizing. Clipping at -1024 and 600 HU, cropping to the body
 
     Args:
@@ -165,27 +166,27 @@
                                 dicom_header.ImagePositionPatient,
                             ]
                             if h_info_wo_name not in unique_set:
                                 unique_set.append(h_info_wo_name)
                                 dcm_header_info.append(h_info)
 
             except Exception as e:
-                logging.error("Unexpected error:", e)
-                logging.warning("Doesn't seem to be DICOM, will be skipped: ", fname)
+                logger.error("Unexpected error:", e)
+                logger.warning("Doesn't seem to be DICOM, will be skipped: ", fname)
 
     conc = [x[1] for x in dcm_header_info]
     sidx = np.argsort(conc)
     conc = np.asarray(conc)[sidx]
     dcm_header_info = np.asarray(dcm_header_info, dtype=object)[sidx]
     vol_unique = np.unique(conc, return_index=1, return_inverse=1)  # unique volumes
     n_vol = len(vol_unique[1])
     if n_vol == 1:
-        logging.info("There is " + str(n_vol) + " volume in the study")
+        logger.info("There is " + str(n_vol) + " volume in the study")
     else:
-        logging.info("There are " + str(n_vol) + " volumes in the study")
+        logger.info("There are " + str(n_vol) + " volumes in the study")
 
     relevant_series = []
     relevant_volumes = []
 
     for i in range(len(vol_unique[1])):
         curr_vol = i
         info_idxs = np.where(vol_unique[2] == curr_vol)[0]
@@ -211,25 +212,25 @@
         path (str): File or folderpath to be loaded. If folder, DICOM series is expected
         disable_tqdm (bool, optional): Disable tqdm progress bar. Defaults to False.
 
     Returns:
         sitk.Image: Loaded image
     """
     if os.path.isfile(path):
-        logging.info(f"Read input: {path}")
+        logger.info(f"Read input: {path}")
         input_image = sitk.ReadImage(path)
     else:
-        logging.info(f"Looking for dicoms in {path}")
+        logger.info(f"Looking for dicoms in {path}")
         dicom_vols = read_dicoms(
             path, original=False, primary=False, disable_tqdm=disable_tqdm
         )
         if len(dicom_vols) < 1:
             sys.exit("No dicoms found!")
         if len(dicom_vols) > 1:
-            logging.warning(
+            logger.warning(
                 "There are more than one volume in the path, will take the largest one"
             )
         input_image = dicom_vols[
             np.argmax([np.prod(v.GetSize()) for v in dicom_vols], axis=0)
         ]
     return input_image
 
@@ -248,15 +249,15 @@
         spare (list, optional): Labels that are used for mapping to neighbors but not considered for final labelling. This is used for label fusion with a filling model. Defaults to [].
         disable_tqdm (bool, optional): If true, tqdm will be diabled. Defaults to False.
         skip_below (int, optional): If a CC is smaller than this value. It will not be merged but removed. This is for performance optimization.
 
     Returns:
         np.ndarray: Postprocessed volume
     """
-    logging.info("Postprocessing")
+    logger.info("Postprocessing")
 
     # CC analysis
     regionmask = skimage.measure.label(label_image)
     origlabels = np.unique(label_image)
     origlabels_maxsub = np.zeros(
         (max(origlabels) + 1,), dtype=np.uint32
     )  # will hold the largest component for a label
```

### Comparing `lungmask-0.2.15/lungmask.egg-info/PKG-INFO` & `lungmask-0.2.16/lungmask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.15
+Version: 0.2.16
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
 Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lungmask-0.2.15/setup.py` & `lungmask-0.2.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lungmask",
-    version="0.2.15",
+    version="0.2.16",
     author="Johannes Hofmanninger",
     author_email="johannes.hofmanninger@gmail.com",
     description="Package for automated lung segmentation in CT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JoHof/lungmask",
     packages=setuptools.find_packages(),
```

### Comparing `lungmask-0.2.15/tests/test_cli.py` & `lungmask-0.2.16/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.15/tests/test_mask.py` & `lungmask-0.2.16/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.15/tests/test_utils.py` & `lungmask-0.2.16/tests/test_utils.py`

 * *Files identical despite different names*

