# Comparing `tmp/tllab_common-2023.7.1.tar.gz` & `tmp/tllab_common-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.7.1.tar", max compression
+gzip compressed data, was "tllab_common-2023.7.2.tar", max compression
```

## Comparing `tllab_common-2023.7.1.tar` & `tllab_common-2023.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.7.1/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.7.1/README.md
--rw-r--r--   0        0        0      890 2023-07-10 14:35:05.698052 tllab_common-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.7.1/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.7.1/tllab_common/findcells.py
--rw-r--r--   0        0        0     7220 2023-07-10 12:51:15.183521 tllab_common-2023.7.1/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.7.1/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.7.1/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.7.1/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    70080 2023-07-04 13:03:46.359987 tllab_common-2023.7.1/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.7.2/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.7.2/README.md
+-rw-r--r--   0        0        0      890 2023-07-10 15:05:31.605649 tllab_common-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.7.2/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10052 2023-07-10 14:56:10.369767 tllab_common-2023.7.2/tllab_common/findcells.py
+-rw-r--r--   0        0        0     7220 2023-07-10 12:51:15.183521 tllab_common-2023.7.2/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.7.2/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.7.2/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.7.2/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    70080 2023-07-04 13:03:46.359987 tllab_common-2023.7.2/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.7.2/PKG-INFO
```

### Comparing `tllab_common-2023.7.1/LICENSE` & `tllab_common-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/README.md` & `tllab_common-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/pyproject.toml` & `tllab_common-2023.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.7.1"
+version = "2023.7.2"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.7.1/tllab_common/findcells.py` & `tllab_common-2023.7.2/tllab_common/findcells.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         ccdist = np.round(np.clip(ccdist, 10, np.sqrt(np.prod(im.shape))/5)).astype('int')
     
     if imnuc is None: #only one channel
         mask, LA = make_mask(im, threshold, thres, smooth, minfeatsize, dilate)
         pk = skimage.feature.peak_local_max(fill_nan(LA), footprint=disk(ccdist), exclude_border=False)
         pk = maskpk(pk, mask)
         pk = np.array(sorted([q.tolist() for q in pk])[::-1])
-        markers = np.zeros(im.shape)
+        markers = np.zeros(im.shape, int)
         for i in range(pk.shape[0]):
             if cellcolormask is None:
                 markers[pk[i, 0], pk[i, 1]] = i+1
             else:
                 markers[pk[i, 0], pk[i, 1]] = cellcolormask[pk[i, 0], pk[i, 1]]
         cells = skimage.segmentation.watershed(-LA, markers=markers, mask=mask)
         cells *= mask #in Python2, watershed sometimes colors outside the mask
```

### Comparing `tllab_common-2023.7.1/tllab_common/fit.py` & `tllab_common-2023.7.2/tllab_common/fit.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/tllab_common/misc.py` & `tllab_common-2023.7.2/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/tllab_common/transforms.py` & `tllab_common-2023.7.2/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/tllab_common/wimread.py` & `tllab_common-2023.7.2/tllab_common/wimread.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.7.1/PKG-INFO` & `tllab_common-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

