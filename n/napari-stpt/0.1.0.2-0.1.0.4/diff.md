# Comparing `tmp/napari-stpt-0.1.0.2.tar.gz` & `tmp/napari-stpt-0.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.1.0.2.tar", last modified: Fri May 12 15:41:10 2023, max compression
+gzip compressed data, was "napari-stpt-0.1.0.4.tar", last modified: Mon Jul 10 03:39:33 2023, max compression
```

## Comparing `napari-stpt-0.1.0.2.tar` & `napari-stpt-0.1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.124565 napari-stpt-0.1.0.2/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.2/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-12 15:41:10.123565 napari-stpt-0.1.0.2/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.2/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.051564 napari-stpt-0.1.0.2/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.2/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.2/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)   139569 2023-05-12 14:48:30.000000 napari-stpt-0.1.0.2/napari_stpt/napari_stpt.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.121565 napari-stpt-0.1.0.2/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)      108 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-05-12 15:41:10.124565 napari-stpt-0.1.0.2/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1335 2023-05-12 15:40:33.000000 napari-stpt-0.1.0.2/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.946569 napari-stpt-0.1.0.4/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.4/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 03:39:33.945569 napari-stpt-0.1.0.4/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.4/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.870568 napari-stpt-0.1.0.4/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.4/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.4/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)   147416 2023-07-08 14:57:22.000000 napari-stpt-0.1.0.4/napari_stpt/napari_stpt.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-07-10 03:39:33.942569 napari-stpt-0.1.0.4/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      116 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-07-10 03:39:33.000000 napari-stpt-0.1.0.4/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-07-10 03:39:33.946569 napari-stpt-0.1.0.4/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1343 2023-07-10 03:38:36.000000 napari-stpt-0.1.0.4/setup.py
```

### Comparing `napari-stpt-0.1.0.2/LICENSE` & `napari-stpt-0.1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.2/PKG-INFO` & `napari-stpt-0.1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.2
+Version: 0.1.0.4
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.2/README.md` & `napari-stpt-0.1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.2/napari_stpt/napari_stpt.py` & `napari-stpt-0.1.0.4/napari_stpt/napari_stpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import os
 import sys
 import napari
 import numpy as np
 import xarray as xr
-
+import vispy.color
 
 if 'PyQt5' in sys.modules:
     from qtpy import QtCore, QtWidgets
     from qtpy.QtWidgets import QComboBox, QApplication, QCompleter, QMessageBox
     from qtpy.QtCore import QSortFilterProxyModel, Qt
 else:
     from PySide2 import QtCore, QtWidgets, QtGui
@@ -266,49 +266,63 @@
         output_resolution = float(self.pixel_size.text())
         scale_x = float(self.slice_spacing)/float(self.optical_slices) / output_resolution
         self.viewer.add_shapes(np.asarray(line_locations), name = 'bounding box',shape_type='line', scale=(scale_x, 1, 1), edge_color = "white", edge_width = width)
 
     def Load(self, text):
         
 
-        def AlignAXIO(axio_volume, sample_name, slice_names, resolution):
+        def AlignAXIO(axio_volume, sample_name, slice_names, resolution, channel):
             
             sample_name = sample_name[:-5]
             
             new_volume = np.zeros(axio_volume.shape)
 
-            df = pd.read_parquet(f"/home/tristan/Shared/imaxt_reg/{sample_name}/{sample_name}_EXT_AXIO_STPT_all_reg.parquet", engine='pyarrow')
+            # df = pd.read_parquet(f"/home/tristan/Shared/imaxt_reg/{sample_name}/{sample_name}_EXT_AXIO_STPT_all_reg.parquet", engine='pyarrow')
+            df = pd.read_parquet(f"/storage/imaxt/imaxt_reg/{sample_name}/{sample_name}_EXT_AXIO_STPT_all_reg.parquet", engine='pyarrow')
+            
 
             filtered_df = df[(df['ranking'] == 1) & ((df['FLAG'] == 1) | (df['FLAG'] == 0))]
             #filtered_df = df[(df['ranking'] == 1)]
             
-            for index, element in enumerate(slice_names):
-                
-                row = filtered_df[filtered_df['D_S'] == element]
-                
+            print(slice_names)
+            
+            axio_zoom = xr.open_zarr(f"/storage/processed.2022/axio/{sample_name}_Axio/mos", group='l.{0:d}'.format(resolution))
+            
+            for index, slice_name in enumerate(slice_names):
+
+                row = filtered_df[filtered_df['D_S'] == slice_name]
+
                 if not row.empty:
 
                     axio_location = int(row.iloc[0, 4][1:]) - 1
+                    # print(row.iloc[0, 4])
+                    # print(axio_location)
+                    # print(row)
+                    # print(" ")
 
-                    axio_image = axio_volume[index,:,:]
+                    axio_image = axio_zoom[slice_name].sel(channel=channel).data
+                    axio_image = axio_image.squeeze()
+
+                    #axio_image = axio_volume[index,:,:]
 
                     #flip image
                     if row.iloc[0, 8] == 0.0:
                         axio_image = axio_image[::-1,:]
-                    if row.iloc[0, 8] == 1.0:
-                        axio_image = axio_image[:,::-1]
 
                     axio_image = np.asarray(axio_image)
 
                     M = np.array([[row.iloc[0, 24], row.iloc[0, 25], row.iloc[0, 26]/resolution], [row.iloc[0, 27], row.iloc[0, 28], row.iloc[0, 29]/resolution]])
+                    # Expand the dimensions of M so that it can be multiplied by T.
+                    M = np.append(M, [[0, 0, 0]], axis=0)
 
                     rows, cols = axio_image.shape
                     affine_np_img = cv2.warpAffine(axio_image, M[:2,:], (cols, rows))
-
-                    new_volume[axio_location,:,:] = affine_np_img
+                    if (axio_location < new_volume.shape[0]):
+                        new_volume[axio_location,:,:] = affine_np_img
+                    
 
             return new_volume
 
         verbose = True
 
         load_in_reference = False
         
@@ -471,17 +485,18 @@
             self.number_of_sections = len(list(self.ds1))
             self.optical_slices_available = 1
         else:
             if self.old_method:
                 self.number_of_sections = len(set(self.ds1.attrs['cube_reg']['slice']))
             else:
                 try:
-                    self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
-                except:
                     self.number_of_sections = int(json.loads(self.ds1.attrs['multiscale'])['metadata']['number_of_sections'])
+                except:
+                    self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
+
         
         if verbose:
             print(f"Number of sections: {self.number_of_sections}")
             
             
         #print("")
         #print(self.ds1.attrs)
@@ -562,17 +577,18 @@
 
         # Get the optical slice spacing
         if self.old_method or self.axio:
             # assume that the optical slices do not overlap
             optical_section_spacing = self.slice_spacing / self.optical_slices_available
         else:
             try:
-                optical_section_spacing = float(json.loads(self.ds1['S001'].attrs['raw_meta'])['zres'])
-            except:
                 optical_section_spacing = float(json.loads(self.ds1.attrs['multiscale'])['metadata']['optical_section_spacing'])
+            except:
+                optical_section_spacing = float(json.loads(self.ds1['S001'].attrs['raw_meta'])['zres'])
+
 
         if verbose:
             print(f"optical_slices zres: {optical_section_spacing}")
 
 
         # Calculate how many optical slices to use
         if self.optical_slices_available > 1:
@@ -646,362 +662,477 @@
         # Define number of slices
         number_of_slices = end_slice_number - start_slice_number + 1
         if verbose:
             print(f"number_of_slices {number_of_slices}")
 
         
         # Load the volume for each channel seperately
-        if self.cb_C1.isChecked():
-            print("loading C1")
-            
-            if self.axio:
-                try:
-                    volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic').to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_1_temp = (ds.sel(channel=self.channels_start).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-            else:
-                try:
-                    volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_1_temp = (ds.sel(channel=self.channels_start, z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-            
-            if self.crop:
-                spacing_x = resolution*0.1*self.spacing[0]
-                spacing_y = resolution*0.1*self.spacing[1]
-
-                size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
-                size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
-                start_y = int(math.floor(self.crop_start_x / spacing_x))
-                start_z = int(math.floor(self.crop_start_y / spacing_y))
-            else:
+        if False:
+            if self.cb_C1.isChecked():
+                print("loading C1")
+
                 if self.axio:
-                    size_y = int(math.floor(volume_1_temp.shape[2]))
-                    size_z = int(math.floor(volume_1_temp.shape[3]))
+                    try:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic').to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=self.channels_start).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
                 else:
-                    size_y = int(math.floor(volume_1_temp.shape[1]))
-                    size_z = int(math.floor(volume_1_temp.shape[2]))
-                start_y = 0
-                start_z = 0
-                
-            volume_1 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
-            
-            if number_of_slices != volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Critical)
-                msg.setText("One or more slices appear to be missing")
-                msg.setInformativeText("Find the missing slice(s) by using the Load slice function and scrolling through the slices until an error message is displayed. Then set a Slices range to avoid this slice.")
-                msg.setWindowTitle("Error")
-                msg.setStandardButtons(QMessageBox.Ok)
-                retval = msg.exec_()
-                return
-            
-            if self.axio:
-                volume_1_temp = volume_1_temp[:,0,:,:]
-                volume_1_temp = AlignAXIO(volume_1_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
-            
-            volume_1[0::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-            
-            for optical_slice in range(1, self.optical_slices):
-                # volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
-                # ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                # volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-                
-                try:
-                    volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_1_temp = (ds.sel(channel=self.channels_start, z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                    
-                volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+                    try:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                if self.crop:
+                    spacing_x = resolution*0.1*self.spacing[0]
+                    spacing_y = resolution*0.1*self.spacing[1]
+
+                    size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
+                    size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
+                    start_y = int(math.floor(self.crop_start_x / spacing_x))
+                    start_z = int(math.floor(self.crop_start_y / spacing_y))
+                else:
+                    if self.axio:
+                        size_y = int(math.floor(volume_1_temp.shape[2]))
+                        size_z = int(math.floor(volume_1_temp.shape[3]))
+                    else:
+                        size_y = int(math.floor(volume_1_temp.shape[1]))
+                        size_z = int(math.floor(volume_1_temp.shape[2]))
+                    start_y = 0
+                    start_z = 0
+
+                volume_1 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
+
+                if number_of_slices != volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
+                    msg = QMessageBox()
+                    msg.setIcon(QMessageBox.Critical)
+                    msg.setText("One or more slices appear to be missing")
+                    msg.setInformativeText("Find the missing slice(s) by using the Load slice function and scrolling through the slices until an error message is displayed. Then set a Slices range to avoid this slice.")
+                    msg.setWindowTitle("Error")
+                    msg.setStandardButtons(QMessageBox.Ok)
+                    retval = msg.exec_()
+                    return
 
-            # Normalize the brightness changes between optical sections
-            if self.cb_correct_brightness_optical_section.isChecked():
-                print("correcting brightness of optical sections C1")
-                self.Normalize_slices(volume_1, self.optical_slices)
+                if self.axio:
+                    volume_1_temp = volume_1_temp[:,0,:,:]
+                    volume_1_temp = AlignAXIO(volume_1_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution, 0)
 
-            print("aligning C1")
-            self.aligned_1 = self.AlignNew(volume_1, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
-            
-            if load_in_reference:
-                self.aligned_1 = self.aligned_1[:,0:reference_size[1],0:reference_size[2]]
-                
-            self.aligned_1 = self.aligned_1[chop_bottom:self.aligned_1.shape[0]-chop_top,:,:]
-            self.shape = self.aligned_1.shape
-            
-            if verbose:
-                print(f"self.shape {self.shape}")
-            
-            self.viewer.add_image([self.aligned_1], name='C1', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
-                                  blending='additive', colormap='bop purple', contrast_limits=self.default_contrast_limits)
+                volume_1[0::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
-        if self.cb_C2.isChecked():
-            print("loading C2")
-            
-            if self.axio:
-                try:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic').to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-            else:
-                try:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1, z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                for optical_slice in range(1, self.optical_slices):
+                    # volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
+                    # ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    # volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
+                    try:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                    volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                # Normalize the brightness changes between optical sections
+                if self.cb_correct_brightness_optical_section.isChecked():
+                    print("correcting brightness of optical sections C1")
+                    self.Normalize_slices(volume_1, self.optical_slices)
+
+                print("aligning C1")
+                self.aligned_1 = self.AlignNew(volume_1, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+
+                if load_in_reference:
+                    self.aligned_1 = self.aligned_1[:,0:reference_size[1],0:reference_size[2]]
+
+                self.aligned_1 = self.aligned_1[chop_bottom:self.aligned_1.shape[0]-chop_top,:,:]
+                self.shape = self.aligned_1.shape
+
+                if verbose:
+                    print(f"self.shape {self.shape}")
+
+                self.viewer.add_image([self.aligned_1], name='C1', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
+                                      blending='additive', colormap='bop purple', contrast_limits=self.default_contrast_limits)
+
+            if self.cb_C2.isChecked():
+                print("loading C2")
 
-            if self.crop:
-                spacing_x = resolution*0.1*self.spacing[0]
-                spacing_y = resolution*0.1*self.spacing[1]
-
-                size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
-                size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
-                start_y = int(math.floor(self.crop_start_x / spacing_x))
-                start_z = int(math.floor(self.crop_start_y / spacing_y))
-            else:
                 if self.axio:
-                    size_y = int(math.floor(volume_2_temp.shape[2]))
-                    size_z = int(math.floor(volume_2_temp.shape[3]))
+                    try:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic').to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
                 else:
-                    size_y = int(math.floor(volume_2_temp.shape[1]))
-                    size_z = int(math.floor(volume_2_temp.shape[2]))
-                start_y = 0
-                start_z = 0
+                    try:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1, z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+
+                if self.crop:
+                    spacing_x = resolution*0.1*self.spacing[0]
+                    spacing_y = resolution*0.1*self.spacing[1]
+
+                    size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
+                    size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
+                    start_y = int(math.floor(self.crop_start_x / spacing_x))
+                    start_z = int(math.floor(self.crop_start_y / spacing_y))
+                else:
+                    if self.axio:
+                        size_y = int(math.floor(volume_2_temp.shape[2]))
+                        size_z = int(math.floor(volume_2_temp.shape[3]))
+                    else:
+                        size_y = int(math.floor(volume_2_temp.shape[1]))
+                        size_z = int(math.floor(volume_2_temp.shape[2]))
+                    start_y = 0
+                    start_z = 0
+
+                volume_2 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
+
+                if number_of_slices != volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
+                    msg = QMessageBox()
+                    msg.setIcon(QMessageBox.Critical)
+                    msg.setText("One or more slices appear to be missing")
+                    msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
+                    msg.setWindowTitle("Error")
+                    msg.setStandardButtons(QMessageBox.Ok)
+                    retval = msg.exec_()
+                    return
 
-            volume_2 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
-            
-            if number_of_slices != volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Critical)
-                msg.setText("One or more slices appear to be missing")
-                msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
-                msg.setWindowTitle("Error")
-                msg.setStandardButtons(QMessageBox.Ok)
-                retval = msg.exec_()
-                return
-            
-            if self.axio:
-                volume_2_temp = volume_2_temp[:,0,:,:]
-                volume_2_temp = AlignAXIO(volume_2_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
-            
-            volume_2[0::self.optical_slices, :, :] = volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+                if self.axio:
+                    volume_2_temp = volume_2_temp[:,0,:,:]
+                    volume_2_temp = AlignAXIO(volume_2_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution, 1)
 
-            for optical_slice in range(1, self.optical_slices):
-                
-                try:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_2_temp = (ds.sel(channel=self.channels_start + 1, z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                    
-                # volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=optical_slice).to_array(
-                # ).data * self.bscale + self.bzero).astype(dtype=np.float16)
-                volume_2[optical_slice::self.optical_slices, :, :] = volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-
-            # Normalize the brightness changes between optical sections
-            if self.cb_correct_brightness_optical_section.isChecked():
-                print("correcting brightness of optical sections C2")
-                self.Normalize_slices(volume_2, self.optical_slices)
+                volume_2[0::self.optical_slices, :, :] = volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
-            print("aligning C2")
-            self.aligned_2 = self.AlignNew(volume_2, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
-            
-            if load_in_reference:
-                self.aligned_2 = self.aligned_2[:,0:reference_size[1],0:reference_size[2]]
-                
-            self.aligned_2 = self.aligned_2[chop_bottom:self.aligned_2.shape[0]-chop_top,:,:]
-            self.shape = self.aligned_2.shape
-            self.viewer.add_image([self.aligned_2], name='C2', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
-                                  blending='additive', colormap='red', contrast_limits=self.default_contrast_limits)
+                for optical_slice in range(1, self.optical_slices):
 
-        if self.cb_C3.isChecked():
-            print("loading C3")
-            
-            if self.axio:
-                try:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic').to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-            else:
-                try:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2, z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    try:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_2_temp = (ds.sel(channel=self.channels_start + 1, z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                    # volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=optical_slice).to_array(
+                    # ).data * self.bscale + self.bzero).astype(dtype=np.float16)
+                    volume_2[optical_slice::self.optical_slices, :, :] = volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                # Normalize the brightness changes between optical sections
+                if self.cb_correct_brightness_optical_section.isChecked():
+                    print("correcting brightness of optical sections C2")
+                    self.Normalize_slices(volume_2, self.optical_slices)
+
+                print("aligning C2")
+                self.aligned_2 = self.AlignNew(volume_2, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+
+                if load_in_reference:
+                    self.aligned_2 = self.aligned_2[:,0:reference_size[1],0:reference_size[2]]
+
+                self.aligned_2 = self.aligned_2[chop_bottom:self.aligned_2.shape[0]-chop_top,:,:]
+                self.shape = self.aligned_2.shape
+                self.viewer.add_image([self.aligned_2], name='C2', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
+                                      blending='additive', colormap='red', contrast_limits=self.default_contrast_limits)
+
+            if self.cb_C3.isChecked():
+                print("loading C3")
 
-            
-            if self.crop:
-                spacing_x = resolution*0.1*self.spacing[0]
-                spacing_y = resolution*0.1*self.spacing[1]
-
-                size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
-                size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
-                start_y = int(math.floor(self.crop_start_x / spacing_x))
-                start_z = int(math.floor(self.crop_start_y / spacing_y))
-            else:
                 if self.axio:
-                    size_y = int(math.floor(volume_3_temp.shape[2]))
-                    size_z = int(math.floor(volume_3_temp.shape[3]))
+                    try:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic').to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
                 else:
-                    size_y = int(math.floor(volume_3_temp.shape[1]))
-                    size_z = int(math.floor(volume_3_temp.shape[2]))
-                start_y = 0
-                start_z = 0
-
-
-            #print(f"start_y {start_y}, start_z {start_z}, size_y {size_y}, size_z {size_z}")
-
-            volume_3 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
-
-            # print(f"volume_3.shape {volume_3.shape}")
-            # print(f"self.optical_slices {self.optical_slices}")
-            # print(f"start_slice_number {start_slice_number}")
-            # print(f"end_slice_number {end_slice_number}")
-           
-            if number_of_slices != volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Critical)
-                msg.setText("One or more slices appear to be missing")
-                msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
-                msg.setWindowTitle("Error")
-                msg.setStandardButtons(QMessageBox.Ok)
-                retval = msg.exec_()
-                return
-            
-            if self.axio:
-                volume_3_temp = volume_3_temp[:,0,:,:]
-                volume_3_temp = AlignAXIO(volume_3_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
-            
-            volume_3[0::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-            
-            for optical_slice in range(1, self.optical_slices):
-#                 volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=optical_slice).to_array(
-#                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-#                 volume_3[optical_slice::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-                
-                try:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_3_temp = (ds.sel(channel=self.channels_start + 2, z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                    
-                volume_3[optical_slice::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+                    try:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2, z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+
+                if self.crop:
+                    spacing_x = resolution*0.1*self.spacing[0]
+                    spacing_y = resolution*0.1*self.spacing[1]
+
+                    size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
+                    size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
+                    start_y = int(math.floor(self.crop_start_x / spacing_x))
+                    start_z = int(math.floor(self.crop_start_y / spacing_y))
+                else:
+                    if self.axio:
+                        size_y = int(math.floor(volume_3_temp.shape[2]))
+                        size_z = int(math.floor(volume_3_temp.shape[3]))
+                    else:
+                        size_y = int(math.floor(volume_3_temp.shape[1]))
+                        size_z = int(math.floor(volume_3_temp.shape[2]))
+                    start_y = 0
+                    start_z = 0
+
+
+                #print(f"start_y {start_y}, start_z {start_z}, size_y {size_y}, size_z {size_z}")
+
+                volume_3 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
+
+                # print(f"volume_3.shape {volume_3.shape}")
+                # print(f"self.optical_slices {self.optical_slices}")
+                # print(f"start_slice_number {start_slice_number}")
+                # print(f"end_slice_number {end_slice_number}")
+
+                if number_of_slices != volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
+                    msg = QMessageBox()
+                    msg.setIcon(QMessageBox.Critical)
+                    msg.setText("One or more slices appear to be missing")
+                    msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
+                    msg.setWindowTitle("Error")
+                    msg.setStandardButtons(QMessageBox.Ok)
+                    retval = msg.exec_()
+                    return
 
-            # Normalize the brightness changes between optical sections
-            if self.cb_correct_brightness_optical_section.isChecked():
-                print("correcting brightness of optical sections C3")
-                self.Normalize_slices(volume_3, self.optical_slices)
+                if self.axio:
+                    volume_3_temp = volume_3_temp[:,0,:,:]
+                    volume_3_temp = AlignAXIO(volume_3_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution, 2)
 
-            print("aligning C3")
-            self.aligned_3 = self.AlignNew(volume_3, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
-            
-            if load_in_reference:
-                self.aligned_3 = self.aligned_3[:,0:reference_size[1],0:reference_size[2]]
-                
-            self.aligned_3 = self.aligned_3[chop_bottom:self.aligned_3.shape[0]-chop_top,:,:]
-            self.shape = self.aligned_3.shape
-            self.viewer.add_image([self.aligned_3], name='C3', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
-                                  blending='additive', colormap='green', contrast_limits=self.default_contrast_limits)
+                volume_3[0::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
-        if self.cb_C4.isChecked():
-            print("loading C4")
+                for optical_slice in range(1, self.optical_slices):
+    #                 volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=optical_slice).to_array(
+    #                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+    #                 volume_3[optical_slice::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                    try:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_3_temp = (ds.sel(channel=self.channels_start + 2, z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                    volume_3[optical_slice::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                # Normalize the brightness changes between optical sections
+                if self.cb_correct_brightness_optical_section.isChecked():
+                    print("correcting brightness of optical sections C3")
+                    self.Normalize_slices(volume_3, self.optical_slices)
+
+                print("aligning C3")
+                self.aligned_3 = self.AlignNew(volume_3, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+
+                if load_in_reference:
+                    self.aligned_3 = self.aligned_3[:,0:reference_size[1],0:reference_size[2]]
+
+                self.aligned_3 = self.aligned_3[chop_bottom:self.aligned_3.shape[0]-chop_top,:,:]
+                self.shape = self.aligned_3.shape
+                self.viewer.add_image([self.aligned_3], name='C3', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
+                                      blending='additive', colormap='green', contrast_limits=self.default_contrast_limits)
 
-            if self.axio:
-                try:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic').to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-            else:
-                try:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3, z=0).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+            if self.cb_C4.isChecked():
+                print("loading C4")
+
+                if self.axio:
+                    try:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic').to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                else:
+                    try:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3, z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                if self.crop:
+                    spacing_x = resolution*0.1*self.spacing[0]
+                    spacing_y = resolution*0.1*self.spacing[1]
+
+                    size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
+                    size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
+                    start_y = int(math.floor(self.crop_start_x / spacing_x))
+                    start_z = int(math.floor(self.crop_start_y / spacing_y))
+                else:
+                    if self.axio:
+                        size_y = int(math.floor(volume_4_temp.shape[2]))
+                        size_z = int(math.floor(volume_4_temp.shape[3]))
+                    else:
+                        size_y = int(math.floor(volume_4_temp.shape[1]))
+                        size_z = int(math.floor(volume_4_temp.shape[2]))
+                    start_y = 0
+                    start_z = 0
+
+                volume_4 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
+
+                if number_of_slices != volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
+                    msg = QMessageBox()
+                    msg.setIcon(QMessageBox.Critical)
+                    msg.setText("One or more slices appear to be missing")
+                    msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
+                    msg.setWindowTitle("Error")
+                    msg.setStandardButtons(QMessageBox.Ok)
+                    retval = msg.exec_()
+                    return
+
+                if self.axio:
+                    volume_4_temp = volume_4_temp[:,0,:,:]
+                    volume_4_temp = AlignAXIO(volume_4_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution, 3)
+
+                volume_4[0::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                for optical_slice in range(1, self.optical_slices):
+    #                 volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=optical_slice).to_array(
+    #                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+    #                 volume_4[optical_slice::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                    try:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_4_temp = (ds.sel(channel=self.channels_start + 3, z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                    volume_4[optical_slice::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                # Normalize the brightness changes between optical sections
+                if self.cb_correct_brightness_optical_section.isChecked():
+                    print("correcting brightness of optical sections C4")
+                    self.Normalize_slices(volume_4, self.optical_slices)
+
+                print("aligning C4")
+                self.aligned_4 = self.AlignNew(volume_4, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+
+                if load_in_reference:
+                    self.aligned_4 = self.aligned_4[:,0:reference_size[1],0:reference_size[2]]
+
+                self.aligned_4 = self.aligned_4[chop_bottom:self.aligned_4.shape[0]-chop_top,:,:]
+                self.shape = self.aligned_4.shape
+                self.viewer.add_image([self.aligned_4], name='C4', scale=((float(self.slice_spacing)/float(self.optical_slices)) / output_resolution, 1, 1), 
+                                      blending='additive', colormap='bop blue', contrast_limits=self.default_contrast_limits)
+
+        else:
+            for chn in range(7):
+                print("loading C1")
 
-            if self.crop:
-                spacing_x = resolution*0.1*self.spacing[0]
-                spacing_y = resolution*0.1*self.spacing[1]
-
-                size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
-                size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
-                start_y = int(math.floor(self.crop_start_x / spacing_x))
-                start_z = int(math.floor(self.crop_start_y / spacing_y))
-            else:
                 if self.axio:
-                    size_y = int(math.floor(volume_4_temp.shape[2]))
-                    size_z = int(math.floor(volume_4_temp.shape[3]))
+                    try:
+                        volume_1_temp = (ds.sel(channel=chn, type='mosaic').to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=chn).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                else:
+                    try:
+                        volume_1_temp = (ds.sel(channel=chn, type='mosaic', z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=chn, z=0).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                if self.crop:
+                    spacing_x = resolution*0.1*self.spacing[0]
+                    spacing_y = resolution*0.1*self.spacing[1]
+
+                    size_y = int(math.floor((self.crop_end_x - self.crop_start_x) / spacing_x))
+                    size_z = int(math.floor((self.crop_end_y - self.crop_start_y) / spacing_y))
+                    start_y = int(math.floor(self.crop_start_x / spacing_x))
+                    start_z = int(math.floor(self.crop_start_y / spacing_y))
                 else:
-                    size_y = int(math.floor(volume_4_temp.shape[1]))
-                    size_z = int(math.floor(volume_4_temp.shape[2]))
-                start_y = 0
-                start_z = 0
+                    if self.axio:
+                        size_y = int(math.floor(volume_1_temp.shape[2]))
+                        size_z = int(math.floor(volume_1_temp.shape[3]))
+                    else:
+                        size_y = int(math.floor(volume_1_temp.shape[1]))
+                        size_z = int(math.floor(volume_1_temp.shape[2]))
+                    start_y = 0
+                    start_z = 0
+
+                volume_1 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
+
+                if number_of_slices != volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
+                    msg = QMessageBox()
+                    msg.setIcon(QMessageBox.Critical)
+                    msg.setText("One or more slices appear to be missing")
+                    msg.setInformativeText("Find the missing slice(s) by using the Load slice function and scrolling through the slices until an error message is displayed. Then set a Slices range to avoid this slice.")
+                    msg.setWindowTitle("Error")
+                    msg.setStandardButtons(QMessageBox.Ok)
+                    retval = msg.exec_()
+                    return
 
-            volume_4 = np.zeros((self.optical_slices*number_of_slices, size_y, size_z), dtype=np.float32)
-            
-            if number_of_slices != volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z].shape[0]:
-                msg = QMessageBox()
-                msg.setIcon(QMessageBox.Critical)
-                msg.setText("One or more slices appear to be missing")
-                msg.setInformativeText("Try to set the Slices range to avoid the missing slices")
-                msg.setWindowTitle("Error")
-                msg.setStandardButtons(QMessageBox.Ok)
-                retval = msg.exec_()
-                return
-            
-            if self.axio:
-                volume_4_temp = volume_4_temp[:,0,:,:]
-                volume_4_temp = AlignAXIO(volume_4_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
-            
-            volume_4[0::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+                if self.axio:
+                    volume_1_temp = volume_1_temp[:,0,:,:]
+                    volume_1_temp = AlignAXIO(volume_1_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution, 0)
 
-            for optical_slice in range(1, self.optical_slices):
-#                 volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=optical_slice).to_array(
-#                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-#                 volume_4[optical_slice::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
-                
-                try:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
-                except:
-                    volume_4_temp = (ds.sel(channel=self.channels_start + 3, z=optical_slice).to_array(
-                    ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                volume_1[0::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                for optical_slice in range(1, self.optical_slices):
+                    # volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
+                    # ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    # volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                    try:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+                    except:
+                        volume_1_temp = (ds.sel(channel=self.channels_start, z=optical_slice).to_array(
+                        ).data * self.bscale + self.bzero).astype(dtype=np.float32)
+
+                    volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
+
+                # Normalize the brightness changes between optical sections
+                if self.cb_correct_brightness_optical_section.isChecked():
+                    print("correcting brightness of optical sections C1")
+                    self.Normalize_slices(volume_1, self.optical_slices)
+
+                print("aligning C1")
+                self.aligned_1 = self.AlignNew(volume_1, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+
+                if load_in_reference:
+                    self.aligned_1 = self.aligned_1[:,0:reference_size[1],0:reference_size[2]]
+
+                self.aligned_1 = self.aligned_1[chop_bottom:self.aligned_1.shape[0]-chop_top,:,:]
+                self.shape = self.aligned_1.shape
+
+                if verbose:
+                    print(f"self.shape {self.shape}")
+                    
+                if chn==0:
+                    color_map='red'
+                elif chn==1:
+                    color_map='green'
+                elif chn==2:
+                    color_map='blue'
+                elif chn==3:
+                    color_map='yellow'
+                elif chn==4:
+                    color_map='magenta'
+                elif chn==5:
+                    color_map='cyan'
+                elif chn==6:
+                    color_map='bop orange'
+                elif chn==7:
+                    color_map='bop purple'
+                elif chn==8:
+                    color_map='bop blue'
+                elif chn==9:
+                    color_map='bop purple'
+                else:
+                    color_map= vispy.color.Colormap([[0.0, 0.0, 0.0], [random.random(), random.random(), random.random()]])
                     
-                volume_4[optical_slice::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
-            # Normalize the brightness changes between optical sections
-            if self.cb_correct_brightness_optical_section.isChecked():
-                print("correcting brightness of optical sections C4")
-                self.Normalize_slices(volume_4, self.optical_slices)
+                self.viewer.add_image([self.aligned_1], name='C'+str(chn+1), scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
+                                      blending='additive', colormap=color_map, contrast_limits=self.default_contrast_limits)
 
-            print("aligning C4")
-            self.aligned_4 = self.AlignNew(volume_4, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
-            
-            if load_in_reference:
-                self.aligned_4 = self.aligned_4[:,0:reference_size[1],0:reference_size[2]]
-            
-            self.aligned_4 = self.aligned_4[chop_bottom:self.aligned_4.shape[0]-chop_top,:,:]
-            self.shape = self.aligned_4.shape
-            self.viewer.add_image([self.aligned_4], name='C4', scale=((float(self.slice_spacing)/float(self.optical_slices)) / output_resolution, 1, 1), 
-                                  blending='additive', colormap='bop blue', contrast_limits=self.default_contrast_limits)
 
         spacing_loaded = [float(self.slice_spacing)/float(self.optical_slices), output_resolution, output_resolution]
 
         self.MakeBoundingBox()
 
     def LoadInRegion(self, text):
         
@@ -1424,16 +1555,20 @@
         # Get number of sections
         if self.axio:
             self.number_of_sections = len(list(self.ds1))
             self.optical_slices_available = 1
         else:
             if self.old_method:
                 self.number_of_sections = len(set(self.ds1.attrs['cube_reg']['slice']))
-            else:    
-                self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
+            else:
+                try:
+                    self.number_of_sections = int(json.loads(self.ds1.attrs['multiscale'])['metadata']['number_of_sections'])
+                except:
+                    self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
+                
             
             self.optical_slices_available = len(self.ds1.z)
         
         print(f"Number of sections: {self.number_of_sections}")
         print(f"optical slices available: {self.optical_slices_available}")
         
         self.scroll.setRange(0, (self.optical_slices_available*self.number_of_sections)-1)
```

### Comparing `napari-stpt-0.1.0.2/napari_stpt.egg-info/PKG-INFO` & `napari-stpt-0.1.0.4/napari_stpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.2
+Version: 0.1.0.4
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.2/setup.py` & `napari-stpt-0.1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.1.0.2",
+    version="0.1.0.4",
     description="napari viewer which can read stpt images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
@@ -28,18 +28,18 @@
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
     ],
     packages=["napari_stpt"],
     include_package_data=True,
     install_requires=[
         'opencv-python==4.5.1.48',
-        'napari',
+        'napari==0.4.17',
         'numpy',
-        'xarray==0.20.1',
+        'xarray',
         'zarr',
-        'PySide2',
+        'PySide2==5.13.2',
         'SimpleITK',
         'napari-animation==0.0.5',
         'tifffile'
     ],
     entry_points={"console_scripts": ["napari-stpt=napari_stpt.__main__:main"]},
 )
```

