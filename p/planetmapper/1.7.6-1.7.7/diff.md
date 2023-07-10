# Comparing `tmp/planetmapper-1.7.6.tar.gz` & `tmp/planetmapper-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.6.tar", last modified: Fri Jul  7 16:50:54 2023, max compression
+gzip compressed data, was "planetmapper-1.7.7.tar", last modified: Mon Jul 10 15:58:57 2023, max compression
```

## Comparing `planetmapper-1.7.6.tar` & `planetmapper-1.7.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.271321 planetmapper-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 16:50:40.000000 planetmapper-1.7.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-07 16:50:54.271321 planetmapper-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-07 16:50:40.000000 planetmapper-1.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112285 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118974 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46648 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-07 16:50:40.000000 planetmapper-1.7.6/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.267321 planetmapper-1.7.6/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 16:50:54.000000 planetmapper-1.7.6/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-07 16:50:40.000000 planetmapper-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:50:54.271321 planetmapper-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-07 16:50:40.000000 planetmapper-1.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:50:54.271321 planetmapper-1.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 16:50:40.000000 planetmapper-1.7.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 15:58:45.000000 planetmapper-1.7.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-10 15:58:57.960238 planetmapper-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-10 15:58:45.000000 planetmapper-1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.956238 planetmapper-1.7.7/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112443 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119046 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46648 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.956238 planetmapper-1.7.7/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-10 15:58:45.000000 planetmapper-1.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:58:57.960238 planetmapper-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-10 15:58:45.000000 planetmapper-1.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_utils.py
```

### Comparing `planetmapper-1.7.6/LICENSE.txt` & `planetmapper-1.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/PKG-INFO` & `planetmapper-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.6
+Version: 1.7.7
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.6/README.md` & `planetmapper-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/__init__.py` & `planetmapper-1.7.7/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/base.py` & `planetmapper-1.7.7/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/basic_body.py` & `planetmapper-1.7.7/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/body.py` & `planetmapper-1.7.7/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/body_xy.py` & `planetmapper-1.7.7/planetmapper/body_xy.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import pyproj
 import scipy.interpolate
 from matplotlib.axes import Axes
 from matplotlib.collections import QuadMesh
+from matplotlib.figure import Figure
 from spiceypy.utils.exceptions import NotFoundError
 
 from .base import _cache_clearable_result, _cache_stable_result
 from .body import Body, _WireframeComponent, _WireframeKwargs
 from .progress import progress_decorator
 
 
@@ -1318,15 +1319,17 @@
         output_size = output_size or max(nx, ny)
         s = output_size / dpi
         if nx > ny:
             figsize = (s, s * ny / nx)
         else:
             figsize = (s * nx / ny, s)
 
-        fig = plt.figure(figsize=figsize, dpi=dpi, facecolor='w')
+        # Use Figure rather than plt.figure to avoid segmentation fault when running
+        # from tkinter GUI (issue #258)
+        fig = Figure(figsize=figsize, dpi=dpi, facecolor='w')
         ax = fig.add_axes([0, 0, 1, 1], facecolor='w')
         plot_fn(ax)
         ax.axis('off')
         ax.set_xticks([])
         ax.set_yticks([])
 
         with io.BytesIO() as io_buf:
```

### Comparing `planetmapper-1.7.6/planetmapper/data/rings.json` & `planetmapper-1.7.7/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/data_loader.py` & `planetmapper-1.7.7/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/gui.py` & `planetmapper-1.7.7/planetmapper/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import numpy as np
 import spiceypy as spice
 from astropy.io import fits
 from matplotlib.artist import Artist
 from matplotlib.backend_bases import MouseButton, MouseEvent
 from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk  # type: ignore
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
+from matplotlib.figure import Figure
 from matplotlib.text import Text
 
 from . import base, common, data_loader, progress, utils
 from .body import BasicBody, Body, NotFoundError
 from .body_xy import _MapKwargs
 from .observation import Observation
 
@@ -1013,15 +1014,17 @@
         self.update_coords(print_coords=print_coords)
 
     def update_only_image(self) -> None:
         self.replot_image()
         self.canvas.draw()
 
     def build_plot(self) -> None:
-        self.fig = plt.figure()
+        # Use Figure rather than plt.figure to avoid segmentation fault when running
+        # from tkinter GUI (issue #258)
+        self.fig = Figure()
         self.ax = self.fig.add_axes([0.06, 0.03, 0.93, 0.96])
         self.transform = (
             self.get_observation().matplotlib_radec2xy_transform() + self.ax.transData
         )
 
         self.replot_all()
         self.format_plot()
@@ -2054,15 +2057,15 @@
 
     def click_cancel(self) -> None:
         self.close_window()
 
     def close_window(self, *_) -> None:
         self.window.destroy()
 
-    def try_run_save(self) -> bool:
+    def try_run_save(self) -> None:
         save_nav = bool(self.save_nav.get())
         save_map = bool(self.save_map.get())
         map_kw: _MapKwargs = {}
 
         path_map = self.path_map.get().strip()
         path_nav = self.path_nav.get().strip()
 
@@ -2071,15 +2074,15 @@
         interpolation = 'linear'
 
         if (save_nav and len(path_nav) == 0) or (save_map and len(path_map) == 0):
             tkinter.messagebox.showwarning(
                 title='Error saving file',
                 message='File paths must not be empty',
             )
-            return False
+            return
 
         try:
             if save_map:
                 interpolation = self.map_interpolation.get()
                 map_kw['projection'] = self.map_projection.get()
                 if map_kw['projection'] in {'rectangular'}:
                     map_kw['degree_interval'] = self.get_float(
@@ -2103,15 +2106,15 @@
                     map_kw['lat'] = self.get_float(
                         self.map_lat,
                         name='latitude',
                         positive=False,
                         finite=True,
                     )
         except ValueError:
-            return False
+            return
 
         # If we get to this point, everything should (hopefully) be working
 
         saving_process = SavingProgress(
             self,
             save_nav=save_nav,
             path_nav=path_nav,
@@ -2126,27 +2129,23 @@
         # pylint: disable-next=broad-except
         except Exception as e:
             traceback.print_exc()
             tkinter.messagebox.showwarning(
                 title='Error saving files',
                 message=f'Error: {e}' + '\n\nSee terminal for more details',
             )
-            return False
+            return
         finally:
             self.gui.get_observation()._remove_progress_hook()
 
         self.gui.set_help_hint(
             'File{s} saved successfully'.format(s='s' if save_nav and save_map else ''),
             color='green',
         )
 
-        if keep_open:
-            return False
-        return True
-
 
 class SavingProgress(Popup):
     def __init__(
         self,
         parent: SaveObservation,
         save_nav: bool,
         path_nav: str,
```

### Comparing `planetmapper-1.7.6/planetmapper/kernel_downloader.py` & `planetmapper-1.7.7/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/observation.py` & `planetmapper-1.7.7/planetmapper/observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/progress.py` & `planetmapper-1.7.7/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper/utils.py` & `planetmapper-1.7.7/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.7.7/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.6
+Version: 1.7.7
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.6/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.7.7/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/pyproject.toml` & `planetmapper-1.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/setup.py` & `planetmapper-1.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_base.py` & `planetmapper-1.7.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_basic_body.py` & `planetmapper-1.7.7/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_body.py` & `planetmapper-1.7.7/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_body_xy.py` & `planetmapper-1.7.7/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_common.py` & `planetmapper-1.7.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_data_loader.py` & `planetmapper-1.7.7/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_init.py` & `planetmapper-1.7.7/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_kernel_downloader.py` & `planetmapper-1.7.7/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_observation.py` & `planetmapper-1.7.7/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_progress.py` & `planetmapper-1.7.7/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.6/tests/test_utils.py` & `planetmapper-1.7.7/tests/test_utils.py`

 * *Files identical despite different names*

