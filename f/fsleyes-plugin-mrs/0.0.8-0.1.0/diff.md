# Comparing `tmp/fsleyes-plugin-mrs-0.0.8.tar.gz` & `tmp/fsleyes-plugin-mrs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsleyes-plugin-mrs-0.0.8.tar", last modified: Thu Mar  2 20:58:33 2023, max compression
+gzip compressed data, was "fsleyes-plugin-mrs-0.1.0.tar", last modified: Mon Jul 10 15:05:23 2023, max compression
```

## Comparing `fsleyes-plugin-mrs-0.0.8.tar` & `fsleyes-plugin-mrs-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-03-02 20:58:33.053342 fsleyes-plugin-mrs-0.0.8/
--rw-r--r--   0 wclarke    (506) staff       (20)     1544 2021-04-19 09:57:16.000000 fsleyes-plugin-mrs-0.0.8/LICENSE
--rw-r--r--   0 wclarke    (506) staff       (20)       15 2021-07-06 19:54:51.000000 fsleyes-plugin-mrs-0.0.8/MANIFEST.in
--rw-r--r--   0 wclarke    (506) staff       (20)     2931 2023-03-02 20:58:33.053553 fsleyes-plugin-mrs-0.0.8/PKG-INFO
--rw-r--r--   0 wclarke    (506) staff       (20)     2359 2021-07-06 18:41:57.000000 fsleyes-plugin-mrs-0.0.8/README.md
-drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-03-02 20:58:33.002627 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/
--rw-r--r--   0 wclarke    (506) staff       (20)        0 2021-02-19 15:23:42.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/__init__.py
-drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-03-02 20:58:33.052053 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/
--rw-r--r--   0 wclarke    (506) staff       (20)    10245 2021-04-09 10:13:29.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon.png
--rw-r--r--   0 wclarke    (506) staff       (20)    24430 2021-04-09 10:13:36.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight.png
--rw-r--r--   0 wclarke    (506) staff       (20)     2076 2021-04-09 10:30:41.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24.png
--rw-r--r--   0 wclarke    (506) staff       (20)     3968 2021-04-19 09:52:03.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24@2x.png
--rw-r--r--   0 wclarke    (506) staff       (20)      969 2021-04-09 10:30:12.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24.png
--rw-r--r--   0 wclarke    (506) staff       (20)     1688 2021-04-19 09:51:12.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png
--rw-r--r--   0 wclarke    (506) staff       (20)     9278 2021-06-03 13:14:11.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/mrsviewprofile.py
--rw-r--r--   0 wclarke    (506) staff       (20)    30313 2023-03-02 20:34:17.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/plugin.py
--rw-r--r--   0 wclarke    (506) staff       (20)    15015 2023-03-02 09:59:15.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/results_load.py
-drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-03-02 20:58:33.035185 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/
--rw-r--r--   0 wclarke    (506) staff       (20)     2931 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/PKG-INFO
--rw-r--r--   0 wclarke    (506) staff       (20)      820 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 wclarke    (506) staff       (20)        1 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 wclarke    (506) staff       (20)      390 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/entry_points.txt
--rw-r--r--   0 wclarke    (506) staff       (20)       16 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/requires.txt
--rw-r--r--   0 wclarke    (506) staff       (20)       19 2023-03-02 20:58:32.000000 fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/top_level.txt
--rw-r--r--   0 wclarke    (506) staff       (20)      248 2023-03-02 20:58:33.056516 fsleyes-plugin-mrs-0.0.8/setup.cfg
--rw-r--r--   0 wclarke    (506) staff       (20)     1480 2023-03-02 20:58:15.000000 fsleyes-plugin-mrs-0.0.8/setup.py
+drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-07-10 15:05:23.587487 fsleyes-plugin-mrs-0.1.0/
+-rw-r--r--   0 wclarke    (506) staff       (20)     1544 2021-04-19 09:57:16.000000 fsleyes-plugin-mrs-0.1.0/LICENSE
+-rw-r--r--   0 wclarke    (506) staff       (20)       15 2021-07-06 19:54:51.000000 fsleyes-plugin-mrs-0.1.0/MANIFEST.in
+-rw-r--r--   0 wclarke    (506) staff       (20)     2931 2023-07-10 15:05:23.587839 fsleyes-plugin-mrs-0.1.0/PKG-INFO
+-rw-r--r--   0 wclarke    (506) staff       (20)     2359 2021-07-06 18:41:57.000000 fsleyes-plugin-mrs-0.1.0/README.md
+drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-07-10 15:05:23.504635 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/
+-rw-r--r--   0 wclarke    (506) staff       (20)        0 2021-02-19 15:23:42.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/__init__.py
+-rw-r--r--   0 wclarke    (506) staff       (20)      545 2023-07-10 13:41:04.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/constants.py
+drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-07-10 15:05:23.579083 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/
+-rw-r--r--   0 wclarke    (506) staff       (20)    10245 2021-04-09 10:13:29.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon.png
+-rw-r--r--   0 wclarke    (506) staff       (20)    24430 2021-04-09 10:13:36.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight.png
+-rw-r--r--   0 wclarke    (506) staff       (20)     2076 2021-04-09 10:30:41.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24.png
+-rw-r--r--   0 wclarke    (506) staff       (20)     3968 2021-04-19 09:52:03.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24@2x.png
+-rw-r--r--   0 wclarke    (506) staff       (20)      969 2021-04-09 10:30:12.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24.png
+-rw-r--r--   0 wclarke    (506) staff       (20)     1688 2021-04-19 09:51:12.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png
+-rw-r--r--   0 wclarke    (506) staff       (20)     9278 2021-06-03 13:14:11.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/mrsviewprofile.py
+-rw-r--r--   0 wclarke    (506) staff       (20)    33985 2023-07-10 13:41:04.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/plugin.py
+-rw-r--r--   0 wclarke    (506) staff       (20)    15015 2023-03-31 09:24:10.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/results_load.py
+drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-07-10 15:05:23.539177 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/
+-rw-r--r--   0 wclarke    (506) staff       (20)     2931 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 wclarke    (506) staff       (20)      878 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 wclarke    (506) staff       (20)        1 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 wclarke    (506) staff       (20)      390 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/entry_points.txt
+-rw-r--r--   0 wclarke    (506) staff       (20)       16 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/requires.txt
+-rw-r--r--   0 wclarke    (506) staff       (20)       19 2023-07-10 15:05:23.000000 fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/top_level.txt
+-rw-r--r--   0 wclarke    (506) staff       (20)      248 2023-07-10 15:05:23.594163 fsleyes-plugin-mrs-0.1.0/setup.cfg
+-rw-r--r--   0 wclarke    (506) staff       (20)     1480 2023-07-10 15:04:15.000000 fsleyes-plugin-mrs-0.1.0/setup.py
+drwxr-xr-x   0 wclarke    (506) staff       (20)        0 2023-07-10 15:05:23.582705 fsleyes-plugin-mrs-0.1.0/tests/
+-rw-r--r--   0 wclarke    (506) staff       (20)      811 2021-05-26 12:29:47.000000 fsleyes-plugin-mrs-0.1.0/tests/test_plugin_load.py
```

### Comparing `fsleyes-plugin-mrs-0.0.8/LICENSE` & `fsleyes-plugin-mrs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/PKG-INFO` & `fsleyes-plugin-mrs-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-plugin-mrs
-Version: 0.0.8
+Version: 0.1.0
 Summary: FSLeyes extension for viewing MRS(I) data formatted as NIfTI-MRS.
 Home-page: https://git.fmrib.ox.ac.uk/wclarke/fsleyes-plugin-mrs
 Author: William Clarke, University of Oxford
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fsleyes-plugin-mrs-0.0.8/README.md` & `fsleyes-plugin-mrs-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24@2x.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24@2x.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/mrsviewprofile.py` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/mrsviewprofile.py`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/plugin.py` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from fsleyes.controls import plottoolbar
 import fsleyes.icons as icons
 import fsleyes.tooltips as tooltips
 
 from fsleyes.views.orthopanel import OrthoPanel
 
 from fsleyes_plugin_mrs.mrsviewprofile import MRSViewProfile
+from fsleyes_plugin_mrs import constants
 
 icon_dir = op.join(op.dirname(__file__), 'icons')
 log = logging.getLogger(__name__)
 
 
 class MRSToolBar(plottoolbar.PlotToolBar):
     """The ``MRSToolBar`` is a toolbar for use with a
@@ -127,15 +128,15 @@
         :class:`.MRSView` views.
         """
         return [MRSView]
 
 
 class MRSDimControl(ctrlpanel.SettingsPanel):
     """Control panel for the MRS view. Controls access to higher dimensions
-    of a NIFTI MRS image.
+    of a NIfTI-MRS image.
     """
 
     @staticmethod
     def title():
         """Overrides :meth:`.ControlMixin.title`. Returns a title to be used
         in FSLeyes menus.
         """
@@ -185,61 +186,104 @@
         """
         self.displayCtx.removeListener('selectedOverlay', self.name)
         self.overlayList.removeListener('overlays', self.name)
         ctrlpanel.SettingsPanel.destroy(self)
 
     def generateDataSeriesWidgets(self, ds, groupName, dims):
         '''Create the required higher dimension spinner widgets in
-        the dimension control pannel.'''
+        the dimension control panel.'''
 
         widgetList = self.getWidgetList()
 
         widgets_out = []
-        if dims > 4:
-            dim5 = props.makeWidget(
-                widgetList,
-                ds,
-                'dim_5',
-                slider=True,
-                showLimits=False)
-            widgetList.AddWidget(
-                dim5,
-                displayName='DIM 5',
-                tooltip="DIM 5 index",
-                groupName=groupName)
-            widgets_out.append(dim5)
-        if dims > 5:
-            dim6 = props.makeWidget(
-                widgetList,
-                ds,
-                'dim_6',
-                slider=True,
-                showLimits=False)
-            widgetList.AddWidget(
-                dim6,
-                displayName='DIM 6',
-                tooltip="DIM 6 index",
-                groupName=groupName)
-            widgets_out.append(dim6)
-        if dims > 6:
-            dim7 = props.makeWidget(
-                widgetList,
-                ds,
-                'dim_7',
-                slider=True,
-                showLimits=False)
-            widgetList.AddWidget(
-                dim7,
-                displayName='DIM 7',
-                tooltip="DIM 7 index",
-                groupName=groupName)
-            widgets_out.append(dim7)
+        for idx in range(5, 8):
+            if dims >= idx:
+                dim = props.makeWidget(
+                    widgetList,
+                    ds,
+                    f'dim_{idx}',
+                    slider=True,
+                    showLimits=False)
+                widgetList.AddWidget(
+                    dim,
+                    displayName=f'DIM {idx}',
+                    tooltip=f"DIM {idx} index",
+                    groupName=groupName)
+                widgets_out.append(dim)
+
+                dim_avg = props.makeWidget(
+                    widgetList,
+                    ds,
+                    f'dim_{idx}_avg')
+                widgetList.AddWidget(
+                    dim_avg,
+                    displayName=f'Average DIM {idx}',
+                    tooltip=f"Show average of {idx}th dimension",
+                    groupName=groupName)
+                widgets_out.append(dim_avg)
+
+                dim_diff = props.makeWidget(
+                    widgetList,
+                    ds,
+                    f'dim_{idx}_diff')
+                widgetList.AddWidget(
+                    dim_diff,
+                    displayName=f'Difference DIM {idx}',
+                    tooltip=f"Show difference of {idx}th dimension",
+                    groupName=groupName)
+                widgets_out.append(dim_diff)
 
         return widgets_out
 
+    def _set_dim_slider_limits(self):
+        """Set the appropriate limits for each dimension index slider.
+        If the dim_N_avg property is True then limit to zero."""
+        overlay = self.displayCtx.getSelectedOverlay()
+
+        if overlay is None:
+            return
+
+        ds = self.__plotPanel.getDataSeries(overlay)
+
+        if ds is None:
+            return
+
+        for dim in range(5, 8):
+            prop = ds.getProp(f'dim_{dim}')
+            is_avg = getattr(ds, f'dim_{dim}_avg')
+            is_diff = getattr(ds, f'dim_{dim}_diff')
+
+            prop.setAttribute(ds, 'minval', 0)
+            if is_avg or is_diff:
+                prop.setAttribute(ds, 'maxval', 0)
+            elif dim <= overlay.ndim:
+                prop.setAttribute(ds, 'maxval', overlay.shape[dim - 1] - 1)
+            else:
+                prop.setAttribute(ds, 'maxval', 0)
+
+    def _set_dim_diff_enabled(self):
+        """Controls whether the difference  checkboxes are enabled or not."""
+        overlay = self.displayCtx.getSelectedOverlay()
+
+        if overlay is None:
+            return
+
+        ds = self.__plotPanel.getDataSeries(overlay)
+
+        if ds is None:
+            return
+
+        for dim in range(5, 8):
+            prop = ds.getProp(f'dim_{dim}_diff')
+            if dim <= overlay.ndim\
+                    and overlay.shape[dim - 1] == 2:
+                prop.enable(ds)
+            else:
+                prop.disable(ds)
+
     def refreshDataSeriesWidgets(self):
         '''Enable/disable and set bounds on the dimensions spinners
         appropriate for the shape of the currently selected overlay.
         '''
         widgetList = self.getWidgetList()
 
         if self.__selectedOverlay is not None:
@@ -258,33 +302,47 @@
         if ds is None:
             return
 
         self.__selectedOverlay = overlay
 
         # Update prop limits now to ensure limits exist before
         # widgets are created
-        # if isinstance(overlay, fslimage.Nifti) and overlay.ndim > 3:
-        for dim in range(5, 8):
-            prop = ds.getProp(f'dim_{dim}')
-            prop.setAttribute(ds, 'minval', 0)
-            if dim <= overlay.ndim:
-                prop.setAttribute(ds, 'maxval', overlay.shape[dim - 1] - 1)
-            else:
-                prop.setAttribute(ds, 'maxval', 0)
+        self._set_dim_slider_limits()
+        self._set_dim_diff_enabled()
 
         # Add listeners to the properties which will cause a
-        # refresh of the Info Pannel.
+        # refresh of the Info Panel and slider limits
         for dim in range(5, 8):
             prop = ds.getProp(f'dim_{dim}')
             prop.addListener(
                 ds,
                 f'dim_{dim}_info_update',
                 self._selectedIndexChanged,
                 overwrite=True)
 
+            prop = ds.getProp(f'dim_{dim}_avg')
+            prop.addListener(
+                ds,
+                f'dim_{dim}_avg_slider_update',
+                self._set_dim_slider_limits,
+                overwrite=True)
+
+            prop.addListener(
+                ds,
+                f'dim_{dim}_avg_info_update',
+                self._selectedIndexChanged,
+                overwrite=True)
+
+            prop = ds.getProp(f'dim_{dim}_diff')
+            prop.addListener(
+                ds,
+                f'dim_{dim}_diff_slider_update',
+                self._set_dim_slider_limits,
+                overwrite=True)
+
         widgetList = self.getWidgetList()
 
         widgetList.AddGroup(
             'niftiMRSDimensions',
             'NIfTI-MRS Dimensions ')
 
         dsWidgets = self.generateDataSeriesWidgets(
@@ -585,22 +643,33 @@
         canvas = self.canvas
         if all_ps_match and canvas.xAutoScale:
             canvas.xAutoScale = False
 
             # Calculate and set x scaling
             canvas.xScale = -1 / spec_freq[0]
 
-            # Calculate x offset
-            if nuclei[0] == '1H':
-                canvas.xOffset = 4.65
+            # Apply x offset
+            known_nuclei = constants.GYRO_MAG_RATIO.keys()
+            if nuclei[0] in known_nuclei:
+                canvas.xOffset = constants.PPM_SHIFT[nuclei[0]]
+            else:
+                print(f'Unknown nucleus {nuclei[0]}.')
+                canvas.xOffset = 0.0
 
             canvas.invertX = True
-            if nuclei[0] == '1H':
-                new_lim = [5, 0, canvas.limits[2], canvas.limits[3]]
-                canvas.limits = new_lim
+            if nuclei[0] in known_nuclei:
+                extra_range = 0.1 * (constants.PPM_RANGE[nuclei[0]][1] - constants.PPM_RANGE[nuclei[0]][0])
+                canvas.limits = [
+                    constants.PPM_RANGE[nuclei[0]][1] + extra_range,
+                    constants.PPM_RANGE[nuclei[0]][0] - extra_range,
+                    canvas.limits[2],
+                    canvas.limits[3]]
+            else:
+                # Force redraw.
+                canvas.limits = canvas.limits
 
     def _add_annotation_listener(self):
         pcanvas = self.canvas
 
         ortho = self.frame.getView(OrthoPanel)
         if len(ortho) == 0:
             log.error('No Ortho panel present')
@@ -666,16 +735,25 @@
 
 
 class MDComplexPowerSpectrumSeries(psseries.ComplexPowerSpectrumSeries):
     '''Sub class of ComplexPowerSpectrumSeries to overload the
        dataAtCurrentVoxel method'''
 
     dim_5 = props.Int(default=0, clamped=True)
+    dim_5_avg = props.Boolean(default=False)
+    dim_5_diff = props.Boolean(default=False)
+
     dim_6 = props.Int(default=0, clamped=True)
+    dim_6_avg = props.Boolean(default=False)
+    dim_6_diff = props.Boolean(default=False)
+
     dim_7 = props.Int(default=0, clamped=True)
+    dim_7_avg = props.Boolean(default=False)
+    dim_7_diff = props.Boolean(default=False)
+
     """Higher order dimension indicies. """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Needs it's own cache or a hack around the name mangling
         self.__cache = cache.Cache(maxsize=1000)
@@ -711,19 +789,27 @@
         """
 
         location = self.currentVoxelLocation(with_time_dim=False)
 
         if location is None:
             return None
 
-        data = self.__cache.get(location, None)
+        try:
+            data = self.__cache.get(location, None)
+        except TypeError:
+            # Handle TypeError: unhashable type: 'slice'
+            data = None
 
         if data is None:
             data = self.currentVoxelData(self.currentVoxelLocation())
-            self.__cache.put(location, data)
+            try:
+                self.__cache.put(location, data)
+            except TypeError:
+                # Handle TypeError: unhashable type: 'slice'
+                pass
 
         return data
 
     def currentVoxelLocation(self, with_time_dim=True):
         """Used by :meth:`dataAtCurrentVoxel`. Returns the current voxel
         location. This is used as a key for the voxel data cache implemented
         within the :meth:`dataAtCurrentVoxel` method, and subsequently passed
@@ -732,35 +818,51 @@
         This implements the higher dimension indexing
 
         If with_time_dim is True (default) then a slice(None) is inserted as
         a fourth dimension.
         """
 
         opts = self.displayCtx.getOpts(self.overlay)
-        vdim = slice(None)
         voxel = opts.getVoxel()
 
         if voxel is None:
             return None
 
-        x, y, z = voxel
+        higher_dim_idx = []
+        for idx in range(5, 8):
+            if getattr(self, f'dim_{idx}_avg'):
+                higher_dim_idx.append(slice(None))
+            elif getattr(self, f'dim_{idx}_diff'):
+                higher_dim_idx.append(slice(0, 2))
+            else:
+                higher_dim_idx.append(getattr(self, f'dim_{idx}'))
 
         if with_time_dim:
-            return (x, y, z, vdim, self.dim_5, self.dim_6, self.dim_7)
+            return tuple(voxel + [slice(None), ] + higher_dim_idx)
         else:
-            return (x, y, z, self.dim_5, self.dim_6, self.dim_7)
+            return tuple(voxel + higher_dim_idx)
 
     def currentVoxelData(self, location):
         """Used by :meth:`dataAtCurrentVoxel`. Returns the data at the
         specified location.
 
         This method may be overridden by sub-classes.
         """
+
         data = self.overlay[location].copy()
-        data = calcSpectrum(data)
+
+        # Take mean of averaged dimensions
+        reduced_loc = [x for x in location[-3:] if isinstance(x, slice)]
+        for idx, loc in enumerate(reduced_loc):
+            if loc == slice(None):
+                data = np.mean(data, axis=idx+1, keepdims=True)
+            elif loc == slice(0, 2):
+                data = np.diff(data, axis=idx+1)
+
+        data = calcSpectrum(data.squeeze())
 
         return data
 
 
 def calcSpectrum(data):
     """Calculates a spectrum for the given one-dimensional data array.
     Includes scaling of first FID point.
```

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs/results_load.py` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs/results_load.py`

 * *Files identical despite different names*

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/PKG-INFO` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsleyes-plugin-mrs
-Version: 0.0.8
+Version: 0.1.0
 Summary: FSLeyes extension for viewing MRS(I) data formatted as NIfTI-MRS.
 Home-page: https://git.fmrib.ox.ac.uk/wclarke/fsleyes-plugin-mrs
 Author: William Clarke, University of Oxford
 Author-email: william.clarke@ndcn.ox.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `fsleyes-plugin-mrs-0.0.8/fsleyes_plugin_mrs.egg-info/SOURCES.txt` & `fsleyes-plugin-mrs-0.1.0/fsleyes_plugin_mrs.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 fsleyes_plugin_mrs/__init__.py
+fsleyes_plugin_mrs/constants.py
 fsleyes_plugin_mrs/mrsviewprofile.py
 fsleyes_plugin_mrs/plugin.py
 fsleyes_plugin_mrs/results_load.py
 fsleyes_plugin_mrs.egg-info/PKG-INFO
 fsleyes_plugin_mrs.egg-info/SOURCES.txt
 fsleyes_plugin_mrs.egg-info/dependency_links.txt
 fsleyes_plugin_mrs.egg-info/entry_points.txt
 fsleyes_plugin_mrs.egg-info/requires.txt
 fsleyes_plugin_mrs.egg-info/top_level.txt
 fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon.png
 fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight.png
 fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24.png
 fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_highlight_thumb24@2x.png
 fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24.png
-fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png
+fsleyes_plugin_mrs/icons/nifti_mrs_icon-mrs_icon_thumb24@2x.png
+tests/test_plugin_load.py
```

### Comparing `fsleyes-plugin-mrs-0.0.8/setup.py` & `fsleyes-plugin-mrs-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fsleyes-plugin-mrs',
 
-    version='0.0.8',
+    version='0.1.0',
 
     description='FSLeyes extension for viewing MRS(I) data formatted as NIfTI-MRS.',
     author='William Clarke, University of Oxford',
     author_email='william.clarke@ndcn.ox.ac.uk',
     url='https://git.fmrib.ox.ac.uk/wclarke/fsleyes-plugin-mrs',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

