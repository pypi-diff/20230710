# Comparing `tmp/animage-data_sorter-1.1.3.tar.gz` & `tmp/animage-data_sorter-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animage-data_sorter-1.1.3.tar", last modified: Tue Jun 27 07:13:32 2023, max compression
+gzip compressed data, was "dist\animage-data_sorter-1.1.4.tar", last modified: Mon Jul 10 02:16:36 2023, max compression
```

## Comparing `animage-data_sorter-1.1.3.tar` & `animage-data_sorter-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/
--rw-rw-rw-   0        0        0     1363 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/animage_data_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/
--rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.3/data_sorter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/old/
--rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageASLUtility.py
--rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDCMUtility.py
--rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorter.py
--rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEeASL7.py
--rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEpCASL13.py
--rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterMISC.py
--rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterPhilips13.py
--rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens4.py
--rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens5.py
--rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemensPASL.py
--rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
--rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterUtility.py
--rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.3/data_sorter/old/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/data_sorter/restructure/
--rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.3/data_sorter/restructure/__init__.py
--rw-rw-rw-   0        0        0    37031 2023-06-26 03:46:08.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_dicom.py
--rw-rw-rw-   0        0        0    12556 2023-06-26 04:37:14.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_dicom_util.py
--rw-rw-rw-   0        0        0     4330 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/_type.py
--rw-rw-rw-   0        0        0     4279 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/data_sorter_base.py
--rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/dcm2nifti.py
--rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.3/data_sorter/restructure/errors.py
--rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/ge_3d_pcasl.py
--rw-rw-rw-   0        0        0     8516 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.3/data_sorter/restructure/ge_easl.py
--rw-rw-rw-   0        0        0    12139 2023-06-27 06:57:43.000000 animage-data_sorter-1.1.3/data_sorter/restructure/noASL_MRI.py
--rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.3/data_sorter/restructure/philips_3d_pcasl.py
--rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pasl.py
--rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl.py
--rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl_old.py
--rw-rw-rw-   0        0        0     4513 2023-06-26 05:05:08.000000 animage-data_sorter-1.1.3/data_sorter/restructure/uih_3d_pasl.py
--rw-rw-rw-   0        0        0       42 2023-06-27 07:13:32.000000 animage-data_sorter-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-06-27 07:13:04.000000 animage-data_sorter-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/
+-rw-rw-rw-   0        0        0     1363 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/animage_data_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/
+-rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.4/data_sorter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/old/
+-rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageASLUtility.py
+-rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDCMUtility.py
+-rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorter.py
+-rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEeASL7.py
+-rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEpCASL13.py
+-rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterMISC.py
+-rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterPhilips13.py
+-rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens4.py
+-rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens5.py
+-rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemensPASL.py
+-rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
+-rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterUtility.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.4/data_sorter/old/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/data_sorter/restructure/
+-rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.4/data_sorter/restructure/__init__.py
+-rw-rw-rw-   0        0        0    37172 2023-07-04 08:05:20.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_dicom.py
+-rw-rw-rw-   0        0        0    12556 2023-06-26 04:37:14.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_dicom_util.py
+-rw-rw-rw-   0        0        0     4367 2023-06-29 08:41:50.000000 animage-data_sorter-1.1.4/data_sorter/restructure/_type.py
+-rw-rw-rw-   0        0        0     4279 2023-06-20 03:26:13.000000 animage-data_sorter-1.1.4/data_sorter/restructure/data_sorter_base.py
+-rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/dcm2nifti.py
+-rw-rw-rw-   0        0        0     3678 2023-06-30 04:16:40.000000 animage-data_sorter-1.1.4/data_sorter/restructure/errors.py
+-rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/ge_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8516 2023-07-10 02:11:42.000000 animage-data_sorter-1.1.4/data_sorter/restructure/ge_easl.py
+-rw-rw-rw-   0        0        0    12056 2023-07-03 03:36:19.000000 animage-data_sorter-1.1.4/data_sorter/restructure/noASL_MRI.py
+-rw-rw-rw-   0        0        0     4431 2023-06-07 08:39:25.000000 animage-data_sorter-1.1.4/data_sorter/restructure/philips_3d_pcasl.py
+-rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pasl.py
+-rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl_old.py
+-rw-rw-rw-   0        0        0     5735 2023-07-04 08:23:37.000000 animage-data_sorter-1.1.4/data_sorter/restructure/uih_3d_pasl.py
+-rw-rw-rw-   0        0        0       42 2023-07-10 02:16:36.000000 animage-data_sorter-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-07-10 02:15:17.000000 animage-data_sorter-1.1.4/setup.py
```

### Comparing `animage-data_sorter-1.1.3/PKG-INFO` & `animage-data_sorter-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data_sorter
-Version: 1.1.3
+Version: 1.1.4
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.3/README.md` & `animage-data_sorter-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/animage_data_sorter.egg-info/PKG-INFO` & `animage-data_sorter-1.1.4/animage_data_sorter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data-sorter
-Version: 1.1.3
+Version: 1.1.4
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.1.3/animage_data_sorter.egg-info/SOURCES.txt` & `animage-data_sorter-1.1.4/animage_data_sorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/__init__.py` & `animage-data_sorter-1.1.4/data_sorter/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageASLUtility.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageASLUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDCMUtility.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDCMUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorter.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorter.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEeASL7.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEeASL7.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterGEpCASL13.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterGEpCASL13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterMISC.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterMISC.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterPhilips13.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterPhilips13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens4.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens4.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens5.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens5.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemensPASL.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemensPASL.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterSiemens_UCLA.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterSiemens_UCLA.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/old/AnImageDataSorterUtility.py` & `animage-data_sorter-1.1.4/data_sorter/old/AnImageDataSorterUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/__init__.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/_dicom.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/_dicom.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,16 @@
                     data_type = MRI_Type.MRI_TYPE_T2
                 elif series_description.find('dwi') > -1 or series_description.find('adc') > -1 or \
                         series_description.find('apparent diffusion coefficient') > -1:
                     data_type = MRI_Type.MRI_TYPE_DWI
 
         elif manufacturer == MANUFACTURER.kMANUFACTURER_UIH:
             if series_description is not None and series_description != '':
-                if series_description.find('asl_3d') > -1:
+                if series_description.find('asl_3d') > -1 or series_description.find('att') > -1 or \
+                    series_description.find('acbv') > -1 or series_description.find('cbf') > -1:
                     ASL_type, data_type = ASL_type, MRI_Type.MRI_TYPE_3D_PASL_UIH
                 elif series_description.find('t1') > -1:
                     data_type = MRI_Type.MRI_TYPE_T1
                     # t1 放在t2 flair前面；避免t1 flair被认为是 t2 flair
                 elif series_description.find('flair') > -1 or series_description.find('fluid') > -1:
                     data_type = MRI_Type.MRI_TYPE_T2_FLAIR
                 elif series_description.find('t2') > -1:
```

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/_dicom_util.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/_dicom_util.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/_type.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,17 @@
 
 class SeriesNumberStartWith():
     ASL = 10000
     T1 = 10010
     T2 = 10020
     T2FLAIR = 10030
     DWI = 10040
-    Report = 10090
+    AstrokeReport = 10090
+    CereflowReport = 10095
+
 
 class MRI_Type(Enum):
     # MR type: AnImage custom
     MRI_TYPE_5Delay_3D_PCASL_SIEMENS = '5delay_PCASL_Siemens'
     MRI_TYPE_1Delay_3D_PCASL_SIEMENS = '1delay_PCASL_Siemens'
     MRI_TYPE_4Delay_3D_PCASL_SIEMENS_Old = '4delay_PCASL_Siemens'
     MRI_TYPE_3D_PASL_SIEMENS = '1delay_PASL_Siemens'
```

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/data_sorter_base.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/data_sorter_base.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/dcm2nifti.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/errors.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,8 +92,13 @@
     errno = 20017
     def __init__(self, c: int):
         super().__init__(f'The amount of data should be less than 1, current[{c}]')
 
 class SeriesTooMany(DataSortException):
     errno = 20018
     def __init__(self, msg):
-        super().__init__(msg)
+        super().__init__(msg)
+
+class NeedTwoBValueDWIError(DataSortException):
+    errno = 20019
+    def __init__(self):
+        super().__init__('需要给出2个不同B值的DWI序列')
```

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/ge_3d_pcasl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/ge_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/ge_easl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/ge_easl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/noASL_MRI.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/noASL_MRI.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,29 +126,29 @@
                 self.DWI = dwi
                 self.is_find_multi_volume = True
                 break
 
         # 多B值不在同一个序列，必须要求DWI_list大于1
         if (not self.is_find_multi_volume):
             if len(self.DWI_list) < 2:
-                raise Exception('需要给出2个不同B值的DWI序列') # todo 定义一个错误
+                raise NeedTwoBValueDWIError()
             else:
                 first_dwi = self.DWI_list[0]
                 second_dwi = self.DWI_list[1]
                 self.DWI = first_dwi
                 if first_dwi.SliceNumber != second_dwi.SliceNumber:
-                    raise Exception('DWI序列空间不一致')  # todo 定义一个错误
+                    raise SpaceIsDifferentError('DWI', 'ADC')
 
 
         # ADC序列验证，允许不存在。
         if len(self.ADC_list) < 1:
             logger.info(f'未发现ADC序列')
             self.ADC = None
         else:
-            logger.debug(f'发现{len(self.DWI_list)}组ADC数据')
+            logger.debug(f'发现{len(self.ADC_list)}组ADC数据')
             self.ADC = self.ADC_list[0]
 
         if self.ADC is not None and self.DWI.SliceNumber != self.ADC.SliceNumber:
             raise SpaceIsDifferentError('DWI', 'ADC')
 
 
     @staticmethod
```

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/philips_3d_pcasl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/philips_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pasl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/siemens_3d_pcasl_old.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/siemens_3d_pcasl_old.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.1.3/data_sorter/restructure/uih_3d_pasl.py` & `animage-data_sorter-1.1.4/data_sorter/restructure/uih_3d_pasl.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,17 @@
         if extra_factor is None or extra_factor == 0:
             logger.debug('extra_factor 未设置')
             # raise Exception('extra_factor 未设置')
         else:
             self.extra_factor = 32 / extra_factor
         self.M0 = []
         self.CBF = [] # CBF参数图
+        self.ATT: SeriesModel = None
+        self.ACBV: SeriesModel = None
+
         self.Control = []
         self.Label = []
 
         self.M0_count = 0
         self.CBF_count = 0
         # 区别M0与灌注图
         for series in self.series_list:
@@ -25,14 +28,18 @@
             seriesDescription = series.SeriesDescription.lower().replace('-', ' ')
             if seriesDescription.find('m0') > -1:
                 self.M0_count += 1
                 self.M0.append(series)
             elif seriesDescription.find('cbf') > -1:
                 self.CBF_count += 1
                 self.CBF.append(series)
+            elif seriesDescription.find('att') > -1:
+                self.ATT = series
+            elif seriesDescription.find('acbv') > -1:
+                self.ACBV = series
             elif seriesDescription.find('ctrl') > -1:
                 self.Control.append(series)
             elif seriesDescription.find('tag') > -1:
                 self.Label.append(series)
 
     def validate_series(self):
         if len(self.M0) == 0:
@@ -46,16 +53,36 @@
         #     raise SeriesTooMany(f'发现{self.CBF_count}组CBF图像，请保留一组再进行处理')
 
     def Sorter(self):
         super(DataSorterUIHPASL, self).Sorter()
 
         self.validate_series()
 
-        # self.generate_calc_cbf_3d_pasl()
-        self.generate_cbf_3d_pasl()
+        if self.ATT is not None and self.ACBV is not None:
+            self.generate_multi_pld()
+
+        else:
+            # self.generate_calc_cbf_3d_pasl()
+            self.generate_cbf_3d_pasl()
+
+    def generate_multi_pld(self):
+        self.M0: SeriesModel = self.M0[0]
+        m0_image = self.M0.load()
+        # 多张M0只有第一张有效
+        m0_image = m0_image[..., 0]
+        write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
+
+        cbf_image = self.CBF[0].load()[..., 0]
+        write_dicom_series(cbf_image * 10, self.M0, 'asl-cbf', 1002, os.path.join(self.output_root, 'asl', 'cbf'), slope=0.1)
+
+        att_image = self.ATT.load()[..., 0]
+        write_dicom_series(att_image * 1000, self.M0, 'asl-att', 1003, os.path.join(self.output_root, 'asl', 'att'), slope=0.001)
+
+        acbv_image = self.ACBV.load()[..., 0]
+        write_dicom_series(acbv_image * 1000, self.M0, 'asl-acbv', 1004, os.path.join(self.output_root, 'asl', 'acbv'), slope=0.001)
 
     def generate_cbf_3d_pasl(self):
         self.M0: SeriesModel = self.M0[0]
         m0_image = self.M0.load()
         # 多张M0只有第一张有效
         m0_image = m0_image[...,0]
         m0_nii = write_dicom_series(m0_image, self.M0, 'asl-m0', 1001, os.path.join(self.output_root, 'asl', 'm0'))
```

### Comparing `animage-data_sorter-1.1.3/setup.py` & `animage-data_sorter-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="animage-data_sorter",
-  version="1.1.3",
+  version="1.1.4",
   author="zhaomy",
   author_email="zhaomy@an-image.cn",
   description="dicom sort",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://gitee.com/AnImage-Beijing/data_sorter",
   packages=setuptools.find_packages(),
```

