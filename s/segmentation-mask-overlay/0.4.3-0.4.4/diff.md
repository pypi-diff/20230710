# Comparing `tmp/segmentation-mask-overlay-0.4.3.tar.gz` & `tmp/segmentation-mask-overlay-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation-mask-overlay-0.4.3.tar", last modified: Mon Jun 19 13:54:09 2023, max compression
+gzip compressed data, was "segmentation-mask-overlay-0.4.4.tar", last modified: Mon Jul 10 16:09:15 2023, max compression
```

## Comparing `segmentation-mask-overlay-0.4.3.tar` & `segmentation-mask-overlay-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.357421 segmentation-mask-overlay-0.4.3/
--rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.3/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.3/MANIFEST.in
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:54:09.357523 segmentation-mask-overlay-0.4.3/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     1496 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.3/README.md
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.316789 segmentation-mask-overlay-0.4.3/examples/
--rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat.jpg
--rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat.py
--rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.3/examples/cat_masked.jpg
--rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.3/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)      788 2023-06-19 13:54:09.358407 segmentation-mask-overlay-0.4.3/setup.cfg
--rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.3/setup.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.294938 segmentation-mask-overlay-0.4.3/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.325054 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/
--rw-r--r--   0 artem      (501) staff       (20)      187 2023-06-19 13:53:39.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)     5912 2023-06-18 20:39:45.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/main.py
--rw-r--r--   0 artem      (501) staff       (20)     3322 2023-06-18 20:40:11.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/utils.py
--rw-r--r--   0 artem      (501) staff       (20)     8725 2023-06-19 13:53:04.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/video.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.328664 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     2005 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      564 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)       26 2023-06-19 13:54:09.000000 segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/top_level.txt
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-06-19 13:54:09.356681 segmentation-mask-overlay-0.4.3/tests/
--rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.3/tests/test_overlay.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:15.035770 segmentation-mask-overlay-0.4.4/
+-rw-r--r--   0 artem      (501) staff       (20)     1072 2023-02-16 13:41:43.000000 segmentation-mask-overlay-0.4.4/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)       45 2023-02-16 14:05:23.000000 segmentation-mask-overlay-0.4.4/MANIFEST.in
+-rw-r--r--   0 artem      (501) staff       (20)     2155 2023-07-10 16:09:15.035863 segmentation-mask-overlay-0.4.4/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     1645 2023-07-10 16:08:22.000000 segmentation-mask-overlay-0.4.4/README.md
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:15.028155 segmentation-mask-overlay-0.4.4/examples/
+-rw-r--r--   0 artem      (501) staff       (20)    39331 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.4/examples/cat.jpg
+-rw-r--r--   0 artem      (501) staff       (20)      840 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.4/examples/cat.py
+-rw-r--r--   0 artem      (501) staff       (20)   243410 2022-12-23 11:33:30.000000 segmentation-mask-overlay-0.4.4/examples/cat_masked.jpg
+-rw-r--r--   0 artem      (501) staff       (20)       81 2023-02-16 13:29:52.000000 segmentation-mask-overlay-0.4.4/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)      788 2023-07-10 16:09:15.036664 segmentation-mask-overlay-0.4.4/setup.cfg
+-rwx------   0 artem      (501) staff       (20)       69 2023-02-16 13:38:32.000000 segmentation-mask-overlay-0.4.4/setup.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:14.998859 segmentation-mask-overlay-0.4.4/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:15.031187 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/
+-rw-r--r--   0 artem      (501) staff       (20)      187 2023-07-10 16:03:46.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)     6056 2023-07-10 16:04:44.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/main.py
+-rw-r--r--   0 artem      (501) staff       (20)     3208 2023-07-10 16:05:44.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/utils.py
+-rw-r--r--   0 artem      (501) staff       (20)     8698 2023-07-10 16:04:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/video.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:15.034865 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     2155 2023-07-10 16:09:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      564 2023-07-10 16:09:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2023-07-10 16:09:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2023-07-10 16:09:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)       26 2023-07-10 16:09:14.000000 segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-07-10 16:09:15.035309 segmentation-mask-overlay-0.4.4/tests/
+-rw-r--r--   0 artem      (501) staff       (20)     1778 2023-06-18 20:47:46.000000 segmentation-mask-overlay-0.4.4/tests/test_overlay.py
```

### Comparing `segmentation-mask-overlay-0.4.3/LICENSE` & `segmentation-mask-overlay-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/PKG-INFO` & `segmentation-mask-overlay-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.3
+Version: 0.4.4
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,7 +58,12 @@
 fig = array = overlay_masks(image, np.stack(masks, -1), mask_labels, return_type="mpl")
 
 # Do with that image whatever you want to do.
 fig.savefig("cat_masked.png", bbox_inches="tight", dpi=300)
 ```
 
 ![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/examples/cat_masked.jpg)
+
+## CHANGELOG
+* **v0.4.4**:
+    - Dropped mandatory label arg in `overlay_masks()`
+    - Added one-channel binary masks handling in `overlay_masks()`
```

### Comparing `segmentation-mask-overlay-0.4.3/README.md` & `segmentation-mask-overlay-0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,7 +43,12 @@
 fig = array = overlay_masks(image, np.stack(masks, -1), mask_labels, return_type="mpl")
 
 # Do with that image whatever you want to do.
 fig.savefig("cat_masked.png", bbox_inches="tight", dpi=300)
 ```
 
 ![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/examples/cat_masked.jpg)
+
+## CHANGELOG
+* **v0.4.4**:
+    - Dropped mandatory label arg in `overlay_masks()`
+    - Added one-channel binary masks handling in `overlay_masks()`
```

### Comparing `segmentation-mask-overlay-0.4.3/examples/cat.jpg` & `segmentation-mask-overlay-0.4.4/examples/cat.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/examples/cat.py` & `segmentation-mask-overlay-0.4.4/examples/cat.py`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/examples/cat_masked.jpg` & `segmentation-mask-overlay-0.4.4/examples/cat_masked.jpg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/setup.cfg` & `segmentation-mask-overlay-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/main.py` & `segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from PIL import Image as PILImage
 from segmentation_mask_overlay.utils import check_convert_image, check_convert_mask
 
 
 def overlay_masks(
     image: np.ndarray,
     masks: np.ndarray,
-    labels: List[str],
+    labels: Optional[List[str]] = None,
     colors: Optional[Union[np.ndarray, List[Union[str, List[float]]]]] = None,
     alpha: float = 1.0,
     beta: float = 0.5,
     return_type: str = "numpy",
     mpl_figsize: Tuple[int, int] = (8, 8),
     mpl_dpi: int = 90,
     concat_original: Optional[str] = None,
@@ -32,15 +32,15 @@
         if you want to control this.
     mask : np.ndarray[bool | int]
         Mask should be a numpy array of shape of the image in one of the following forms:
         - H W C, with bool mask per channel, where each channel represents a class.
         - H W, with an pixel integer value representing a class.
     labels : Optional[List[str]], optional
         Names of expected labels. Provide in the same order as the channels in the masks.
-        If provided, defines 
+        If provided, defines
         If not provided, will be set as range(mask.shape[-1] | max(mask) + 1), by default None
     colors : Union[np.ndarray, List[Union[str, List[float]]]], optional
         Array of shape (n_labels x 3) or list of matplotlib acceptable colornames.
         Example to get persistent colormap: `plt.cm.tab20(np.arange(NUM_LABELS))[..., :-1]`
     alpha : float, optional
         Image alpha, by default 1.0
     beta : float, optional
@@ -63,14 +63,20 @@
     -------
     plt.Figure | PIL.Image | np.ndarray
         Output mpl figure or pillow image with masks.
     """
 
     assert image.shape[:2] == masks.shape[:2], "Image and mask should be of the same size"
 
+    if masks.ndim == 2:
+        masks = masks[..., None]
+
+    if labels is None:
+        labels = list(range(masks.shape[-1]))
+
     num_classes = len(labels)
 
     image = check_convert_image(image)
     masks = check_convert_mask(masks, num_classes)
 
     if colors is None:
         if num_classes <= 10:
```

### Comparing `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/utils.py` & `segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,18 @@
         array = array / (array.max() + 1e-6) * 255
     else:
         array = (array - array.min()) / (array.max() - array.min() + 1e-6) * 255
     return array.round().astype(np.uint8)
 
 
 def check_convert_image(image: np.ndarray, input_dims: str = "HWC") -> np.ndarray:
-    if input_dims == "HWC":
-        ch_dim = -1
-    elif input_dims == "CHW":
-        ch_dim = -3
-    else:
+    if input_dims not in ["HWC", "CHW"]:
         raise AssertionError("input_dims should be HWC | CHW")
 
-    if (
-        image.dtype == np.uint8
-        and image.max() <= 255
-        and image.min() >= 0
-    ):
+    if image.dtype == np.uint8 and image.max() <= 255 and image.min() >= 0:
         pass
     else:
         image = normalize_to_uint8(image)
 
     if image.ndim == 2:
         return cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
 
@@ -46,28 +38,26 @@
         if image.shape[-1] == 4:
             return cv2.cvtColor(image, cv2.COLOR_RGBA2RGB)
 
     else:
         raise AssertionError("Expected numpy array of shape HW, HW1, HW3, HW4.")
 
 
-def check_convert_mask(
-    mask: np.ndarray, num_classes: Optional[int] = None, input_dims: str = "HWC"
-) -> np.ndarray:
+def check_convert_mask(mask: np.ndarray, num_classes: Optional[int] = None, input_dims: str = "HWC") -> np.ndarray:
     """Checks and converts mask to HWC format if needed.
 
     Parameters
     ----------
     mask : np.ndarray
         Segmenttaion mask HWC, with binary channel per class
     num_classes : Optional[int], optional
-        You may provide this to infer correct number of channels if mask 
+        You may provide this to infer correct number of channels if mask
         is provided in HW format. By default number of channels inferred
         as max(mask) + 1, by default None
-    
+
     Returns
     -------
     np.ndarray (bool)
         CHW boolean mask array
     """
 
     assert_message = "The mask is expected to be an HW array with integer per class or HWC with bool mask per channel"
@@ -97,14 +87,14 @@
 
     Example
     ------
     >>> with catchtime() as t:
     >>>     time.sleep(1)
     >>> print(f"Execution time: {t():.4f} secs")
     """
-    
+
     start = time.perf_counter()
     yield
     if logger is not None:
         logger.info(f"{arg} exec time: {time.perf_counter() - start:.4f} secs")
     else:
         print(f"{arg} exec time: {time.perf_counter() - start:.4f} secs")
```

### Comparing `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay/video.py` & `segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,26 @@
     im_sequence: np.ndarray,
     *mask_sequences: np.ndarray,
     output: Union[str, Path] = "numpy",
     array_dims: str = "THWC",
     fps: int = 15,
     image_weight: float = 1.0,
     mask_weight: float = 0.5,
-
 ):
     """Create videos out of sequences of images and masks.
 
     Parameters
     ----------
     savepath: str "path/to/video.mp4"
     im_sequence : np.ndarray of shape THW or THWC
     mask_sequences : numpy arrays of shape THWC of dtype bool
     output: str | Path
         if output == 'numpy' output is a numpy array. If Path, an mp4 file
         will be saved there, default: 'numpy'
-    array_dims: str, 
+    array_dims: str,
         THWC | TCHW, default: THWC
     fps: int
         default: 15
 
     Returns
     -------
     Depends on output.
@@ -65,15 +64,14 @@
             mask_cmaps.append(plt.cm.tab10(range(10), bytes=True)[:num_classes, :-1][:, ::-1])
         else:
             mask_cmaps.append(plt.cm.rainbow_r(np.linspace(0, 1, num_classes), bytes=True)[:, :-1][:, ::-1])
 
     # Iterate through: frame, (frame_mask0, frame_mask1, ...)
     video_frames = []
     for im, *masks in zip(im_sequence, *mask_sequences):
-
         # Normalize, cast to uint8, convert to RGB
         im = check_convert_image(im, input_dims=array_dims[1:])
 
         masks_im = []
         if len(masks) > 0:
             # Prepare image for each mask
             masks_im = [np.copy(im) for _ in range(len(masks))]
@@ -145,15 +143,15 @@
     ----------
     savepath: str "path/to/video.mp4"
     im_sequence : np.ndarray of shape THW or THWC
     pts_sequences : numpy arrays of shape TN2 of dtype int
     output: str | Path
         if output == 'numpy' output is a numpy array. If Path, an mp4 file
         will be saved there, default: 'numpy'
-    array_dims: str, 
+    array_dims: str,
         THWC | TCHW, default: THWC
     fps: int
         default: 15
 
     Returns
     -------
     Depends on output.
@@ -162,30 +160,27 @@
     """
 
     if array_dims not in ["TCHW", "THWC"]:
         raise AssertionError("array_dims should be THWC | TCHW")
 
     # Check array length consistency between image and masks.
     if len(pts_sequences) > 0:
-        assert all(
-            [im_sequence.shape[0] == len(p) for p in pts_sequences]
-        ), "Sequence and masks have different size T"
+        assert all([im_sequence.shape[0] == len(p) for p in pts_sequences]), "Sequence and masks have different size T"
 
     # Set colormaps: 'tab10' if n_classes <=10, 'rainbow' otherwise
     pts_cmaps = []
     num_classes = len(pts_sequences)
     if num_classes <= 10:
         pts_cmaps = plt.cm.tab10(range(10), bytes=True)[:num_classes, :-1][:, ::-1]
     else:
         pts_cmaps = plt.cm.rainbow_r(np.linspace(0, 1, num_classes), bytes=True)[:, :-1][:, ::-1]
 
     # Iterate through: frame, (frame_mask0, frame_mask1, ...)
     video_frames = []
     for im, *pts in zip(im_sequence, *pts_sequences):
-
         if isinstance(sizes, list):
             assert len(pts) == len(sizes), "Provide the sizes for all the point arrays"
 
         # Normalize, cast to uint8, convert to RGB
         im = check_convert_image(im, input_dims=array_dims[1:])
 
         pts_im = []
```

### Comparing `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/PKG-INFO` & `segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation-mask-overlay
-Version: 0.4.3
+Version: 0.4.4
 Summary: Plotting the segmentation masks has never been so exciting!
 Home-page: https://github.com/lobantseff/segmentation-mask-overlay
 Author: Artem Lobantsev
 Author-email: lobantseff@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,7 +58,12 @@
 fig = array = overlay_masks(image, np.stack(masks, -1), mask_labels, return_type="mpl")
 
 # Do with that image whatever you want to do.
 fig.savefig("cat_masked.png", bbox_inches="tight", dpi=300)
 ```
 
 ![Segmented cat](https://raw.githubusercontent.com/lobantseff/segmentation-mask-overlay/master/examples/cat_masked.jpg)
+
+## CHANGELOG
+* **v0.4.4**:
+    - Dropped mandatory label arg in `overlay_masks()`
+    - Added one-channel binary masks handling in `overlay_masks()`
```

### Comparing `segmentation-mask-overlay-0.4.3/src/segmentation_mask_overlay.egg-info/SOURCES.txt` & `segmentation-mask-overlay-0.4.4/src/segmentation_mask_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segmentation-mask-overlay-0.4.3/tests/test_overlay.py` & `segmentation-mask-overlay-0.4.4/tests/test_overlay.py`

 * *Files identical despite different names*

