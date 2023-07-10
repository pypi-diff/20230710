# Comparing `tmp/confluentfucci-0.0.16.tar.gz` & `tmp/confluentfucci-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluentfucci-0.0.16.tar", max compression
+gzip compressed data, was "confluentfucci-0.0.17.tar", max compression
```

## Comparing `confluentfucci-0.0.16.tar` & `confluentfucci-0.0.17.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/LICENSE.txt
--rw-r--r--   0        0        0     1617 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/README.md
--rw-r--r--   0        0        0      313 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/confluentfucci/__init__.py
--rw-r--r--   0        0        0    22419 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/confluentfucci/gui.py
--rw-r--r--   0        0        0    22441 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/confluentfucci/math.py
--rw-r--r--   0        0        0     3909 2023-07-08 20:03:54.220098 confluentfucci-0.0.16/confluentfucci/utils.py
--rw-r--r--   0        0        0     4892 2023-07-08 20:07:40.038032 confluentfucci-0.0.16/pyproject.toml
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 confluentfucci-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/LICENSE.txt
+-rw-r--r--   0        0        0     1617 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/README.md
+-rw-r--r--   0        0        0      351 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/__init__.py
+-rw-r--r--   0        0        0    22573 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/gui.py
+-rw-r--r--   0        0        0    22441 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/math.py
+-rw-r--r--   0        0        0     3909 2023-07-10 21:28:11.234752 confluentfucci-0.0.17/confluentfucci/utils.py
+-rw-r--r--   0        0        0     4793 2023-07-10 21:31:42.521841 confluentfucci-0.0.17/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 confluentfucci-0.0.17/PKG-INFO
```

### Comparing `confluentfucci-0.0.16/LICENSE.txt` & `confluentfucci-0.0.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.16/README.md` & `confluentfucci-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.16/confluentfucci/gui.py` & `confluentfucci-0.0.17/confluentfucci/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 import numpy as np
 import pandas as pd
 import panel as pn
 import param
 from dask_image.imread import imread
 from shapely import Polygon
 from skimage.exposure import equalize_adapthist
-from utils import (
-    get_docker_client,
-    read_stack,
-    run_trackmate,
-    segment_stack,
-)
 
 from confluentfucci.math import (
     CartesianSimilarity,
     CartesianSimilarityFromFile,
     TrackmateXML,
     compute_voronoi,
     compute_voronoi_stats,
     filter_voronoi_tiling,
 )
+from confluentfucci.utils import (
+    get_docker_client,
+    read_stack,
+    run_trackmate,
+    segment_stack,
+)
 
 pn.extension("terminal")
 
 
 class CollectiveStats:
     def __init__(self, metric: CartesianSimilarity, phase_stack_path: Path):
         self.stack = read_stack(phase_stack_path)
@@ -211,15 +211,15 @@
         return fig
 
 
 def select_files_model():
     root = Tk()
     root.withdraw()
     root.call("wm", "attributes", ".", "-topmost", True)
-    files = filedialog.askopenfilename(initialdir=Path().cwd().parent / "models/cellpose")
+    files = filedialog.askopenfilename(initialdir=Path("__file__").cwd().parent / "models/cellpose")
     print(files)
     return Path(files)
 
 
 def view_segmented(data_dir_path):
     base_data_path = Path(data_dir_path)
     viewer = napari.Viewer(title="PyFucciTrack Viewer")
@@ -251,15 +251,15 @@
     viewer.layers[:] = viewer.layers[::-1]
 
     napari.run(force=True, gui_exceptions=True)
 
 
 def trackmate_available():
     try:
-        get_docker_client().images.pull('leogold/trackmate:v1')
+        get_docker_client().images.pull("leogold/trackmate:v1")
         return True
     except Exception as e:
         print(traceback.format_exc())
         return False
 
 
 def check_cellpose_gpu():
@@ -350,15 +350,17 @@
             self.validate_btn.button_type = "danger"
         self.validate_btn.disabled = False
 
     def select_data_folder(self, *b):
         root = Tk()
         root.withdraw()
         root.call("wm", "attributes", ".", "-topmost", True)
-        files = filedialog.askdirectory(initialdir=Path().cwd().parent / "data")
+        initial_dir = Path("__file__").cwd().parent.parent / "data"
+        print(initial_dir.absolute(), initial_dir.exists())
+        files = filedialog.askdirectory(initialdir=initial_dir)
         # files = filedialog.askdirectory(
         #     initialdir=r"D:\Data\full_pipeline_tests\left_60_frames"
         # )
 
         print(files)
         self.data_dir_path = Path(files)
 
@@ -387,19 +389,19 @@
 
     def track(self, event):
         self.run_tracking_btn.disabled = True
         sys.stdout = self.tracking_terminal
 
         (Path(self.data_dir_path) / "metric.h5").unlink(missing_ok=True)
         run_trackmate(
-            Path().cwd().parent / "models/trackmate/basic_settings.xml",
+            Path("__file__").cwd().parent / "models/trackmate/basic_settings.xml",
             Path(self.data_dir_path) / "red_segmented.tiff",
         )
         run_trackmate(
-            Path().cwd().parent / "models/trackmate/basic_settings.xml",
+            Path("__file__").cwd().parent / "models/trackmate/basic_settings.xml",
             Path(self.data_dir_path) / "green_segmented.tiff",
         )
 
         sys.stdout = sys.__stdout__
         self.run_tracking_btn.disabled = False
 
     def segment_one(self):
@@ -455,15 +457,15 @@
 
         self.analysis_ui = CollectiveStats(self.metric, Path(self.data_dir_path) / "phase.tif")
 
         self.analysis_available = True
         self.run_analysis_btn.disabled = False
 
     def get_sidebar(self):
-        sidebar = pn.Accordion(toggle=True, sizing_mode='stretch_width')
+        sidebar = pn.Accordion(toggle=True, sizing_mode="stretch_width")
 
         sidebar.append(
             (
                 "Welcome",
                 pn.Column(self.validate_btn),
             )
         )
@@ -513,15 +515,15 @@
             theme_toggle=False,
             sidebar=[self.sidebar],
             main=self.main,
         )
 
         return template
 
-    @param.depends("docker_check", "trackmate_check", 'gpu_check')
+    @param.depends("docker_check", "trackmate_check", "gpu_check")
     def get_welcome_message(self):
         # Docker: {🕑 if self.docker_check is None or (✅ if self.docker_check else ❌)}
 
         text = pn.pane.Markdown(
             f"""# Welcome
 See you soon
                 
@@ -622,25 +624,25 @@
 
 # magnification_towards_camera = 1
 # # pixel_size_in_microns = 0.345 * magnification_towards_camera
 # pixel_size_in_microns = 0.67 * magnification_towards_camera
 # calibration_squared_microns_to_squared_pixel = pixel_size_in_microns**2
 
 # AppUI().template.servable()
-AppUI().template.show()
+# AppUI().template.show()
 
 # pn.Row(
 #     pn.widgets.Button(
 #         icon="alert-triangle-filled", button_type="warning", name="WARNING"
 #     ),
 #     pn.widgets.Button(icon="bug", button_type="danger", name="Error"),
 # ).servable()
 
 if __name__ == "__main__":
-    AppUI().get_template().servable()
+    AppUI().get_template().show()
     # magnification_towards_camera = 1
     # # pixel_size_in_microns = 0.345 * magnification_towards_camera
     # pixel_size_in_microns = 0.67 * magnification_towards_camera
     # calibration_squared_microns_to_squared_pixel = pixel_size_in_microns**2
     #
     # # base_data_path = Path("data/fucci_60_frames")
     # base_data_path = Path(r"D:\Data\full_pipeline_tests\left_60_frames")
```

### Comparing `confluentfucci-0.0.16/confluentfucci/math.py` & `confluentfucci-0.0.17/confluentfucci/math.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.16/confluentfucci/utils.py` & `confluentfucci-0.0.17/confluentfucci/utils.py`

 * *Files identical despite different names*

### Comparing `confluentfucci-0.0.16/pyproject.toml` & `confluentfucci-0.0.17/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 [tool.poetry]
 name = "ConfluentFUCCI"
-version = "0.0.16"
+version = "0.0.17"
 description = ""
 authors = ["Leo Goldstien <leogoldstien@gmail.com>"]
 readme = "README.md"
 packages = [{include = "confluentfucci"}]
 
 [tool.poetry.dependencies]
-beartype = "^0.14.1"
-icontract = "^2.6.2"
 loguru = "^0.7.0"
-pydantic = "^1.10.9"
 python = "^3.9"
-python-semantic-release = "^7.32.1"
-mkdocs-jupyter = "^0.24.1"
 h5py = "^3.9.0"
 panel = "0.13.1"
 shapely = "^2.0.1"
 pandas = "1.4.3"
 napari = {extras = ["all"], version = "^0.4.18"}
 holoviews = "^1.16.2"
 hvplot = "^0.8.4"
@@ -39,14 +34,15 @@
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.32.1"
+mkdocs-jupyter = "^0.24.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
```

### Comparing `confluentfucci-0.0.16/PKG-INFO` & `confluentfucci-0.0.17/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.1
 Name: confluentfucci
-Version: 0.0.16
+Version: 0.0.17
 Summary: 
 Author: Leo Goldstien
 Author-email: leogoldstien@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beartype (>=0.14.1,<0.15.0)
 Requires-Dist: cellpose (==2.1.0)
 Requires-Dist: dask-image (>=2023.3.0,<2024.0.0)
 Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: holoviews (>=1.16.2,<2.0.0)
 Requires-Dist: hvplot (>=0.8.4,<0.9.0)
-Requires-Dist: icontract (>=2.6.2,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: mkdocs-jupyter (>=0.24.1,<0.25.0)
 Requires-Dist: napari[all] (>=0.4.18,<0.5.0)
 Requires-Dist: pandas (==1.4.3)
 Requires-Dist: panel (==0.13.1)
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: python-semantic-release (>=7.32.1,<8.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: tables (>=3.8.0,<4.0.0)
 Requires-Dist: tifffile (==2022.5.4)
 Requires-Dist: torch (==1.12.0) ; sys_platform == "darwin"
 Requires-Dist: torch (==1.12.0) ; sys_platform == "linux"
 Requires-Dist: torch (==1.12.0) ; sys_platform == "win32"
 Description-Content-Type: text/markdown
```

