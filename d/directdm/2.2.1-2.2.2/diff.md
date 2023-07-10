# Comparing `tmp/directdm-2.2.1.tar.gz` & `tmp/directdm-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/directdm-2.2.1.tar", last modified: Fri Apr 21 21:17:49 2023, max compression
+gzip compressed data, was "dist/directdm-2.2.2.tar", last modified: Mon Jul 10 15:10:38 2023, max compression
```

## Comparing `directdm-2.2.1.tar` & `directdm-2.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/
--rw-r--r--   0 jbrod     (1000) users      (100)      682 2023-04-21 21:17:49.000000 directdm-2.2.1/PKG-INFO
--rw-rw-r--   0 jbrod     (1000) users      (100)     2518 2018-09-13 15:27:57.000000 directdm-2.2.1/README.md
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/
--rw-r--r--   0 jbrod     (1000) users      (100)      181 2019-05-08 14:58:03.000000 directdm-2.2.1/directdm/__init__.py
--rw-r--r--   0 jbrod     (1000) users      (100)       21 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/_version.py
--rw-r--r--   0 jbrod     (1000) users      (100)     2636 2019-05-08 14:58:03.000000 directdm-2.2.1/directdm/dm_eft.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/match/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2018-09-12 06:19:27.000000 directdm-2.2.1/directdm/match/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)     8931 2020-11-22 18:32:18.000000 directdm-2.2.1/directdm/match/dim4_gauge_contribution.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/num/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.1/directdm/num/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)    17180 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/num/num_input.py
--rw-r--r--   0 jbrod     (1000) users      (100)    18337 2020-11-30 15:06:11.000000 directdm-2.2.1/directdm/num/single_nucleon_form_factors.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm/run/
--rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.1/directdm/run/__init__.py
--rwxr-xr-x   0 jbrod     (1000) users      (100)    33119 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/run/adm.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   159997 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_g1.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   153526 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_g2.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yb.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yc.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_yt.py
--rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.1/directdm/run/full_adm_ytau.py
--rw-r--r--   0 jbrod     (1000) users      (100)    27580 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/run/rge.py
--rw-r--r--   0 jbrod     (1000) users      (100)   245355 2023-04-21 20:58:02.000000 directdm-2.2.1/directdm/wilson_coefficients.py
-drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/
--rw-rw-r--   0 jbrod     (1000) users      (100)      682 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/PKG-INFO
--rw-rw-r--   0 jbrod     (1000) users      (100)      669 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/SOURCES.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)        1 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/dependency_links.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)       23 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/requires.txt
--rw-rw-r--   0 jbrod     (1000) users      (100)        9 2023-04-21 21:17:49.000000 directdm-2.2.1/directdm.egg-info/top_level.txt
--rw-r--r--   0 jbrod     (1000) users      (100)       38 2023-04-21 21:17:49.000000 directdm-2.2.1/setup.cfg
--rw-rw-r--   0 jbrod     (1000) users      (100)      885 2018-09-12 06:19:28.000000 directdm-2.2.1/setup.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/
+-rw-r--r--   0 jbrod     (1000) users      (100)      682 2023-07-10 15:10:38.000000 directdm-2.2.2/PKG-INFO
+-rw-rw-r--   0 jbrod     (1000) users      (100)     2518 2018-09-13 15:27:57.000000 directdm-2.2.2/README.md
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm/
+-rw-r--r--   0 jbrod     (1000) users      (100)      181 2019-05-08 14:58:03.000000 directdm-2.2.2/directdm/__init__.py
+-rw-r--r--   0 jbrod     (1000) users      (100)       21 2023-07-10 15:09:54.000000 directdm-2.2.2/directdm/_version.py
+-rw-r--r--   0 jbrod     (1000) users      (100)     2636 2019-05-08 14:58:03.000000 directdm-2.2.2/directdm/dm_eft.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm/match/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2018-09-12 06:19:27.000000 directdm-2.2.2/directdm/match/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)     8931 2023-05-25 14:36:55.000000 directdm-2.2.2/directdm/match/dim4_gauge_contribution.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm/num/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.2/directdm/num/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)    17180 2023-05-25 14:36:55.000000 directdm-2.2.2/directdm/num/num_input.py
+-rw-r--r--   0 jbrod     (1000) users      (100)    18337 2023-05-25 14:36:55.000000 directdm-2.2.2/directdm/num/single_nucleon_form_factors.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm/run/
+-rw-rw-r--   0 jbrod     (1000) users      (100)        0 2017-09-01 23:48:50.000000 directdm-2.2.2/directdm/run/__init__.py
+-rwxr-xr-x   0 jbrod     (1000) users      (100)    31963 2023-07-10 15:09:54.000000 directdm-2.2.2/directdm/run/adm.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   159997 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_g1.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   153526 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_g2.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_yb.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_yc.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_yt.py
+-rw-rw-r--   0 jbrod     (1000) users      (100)   151308 2018-09-12 06:19:28.000000 directdm-2.2.2/directdm/run/full_adm_ytau.py
+-rw-r--r--   0 jbrod     (1000) users      (100)    27580 2023-05-25 14:36:55.000000 directdm-2.2.2/directdm/run/rge.py
+-rw-r--r--   0 jbrod     (1000) users      (100)   236549 2023-07-10 15:09:54.000000 directdm-2.2.2/directdm/wilson_coefficients.py
+drwxr-xr-x   0 jbrod     (1000) users      (100)        0 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/
+-rw-rw-r--   0 jbrod     (1000) users      (100)      682 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/PKG-INFO
+-rw-rw-r--   0 jbrod     (1000) users      (100)      669 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)        1 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)       23 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/requires.txt
+-rw-rw-r--   0 jbrod     (1000) users      (100)        9 2023-07-10 15:10:38.000000 directdm-2.2.2/directdm.egg-info/top_level.txt
+-rw-r--r--   0 jbrod     (1000) users      (100)       38 2023-07-10 15:10:38.000000 directdm-2.2.2/setup.cfg
+-rw-rw-r--   0 jbrod     (1000) users      (100)      885 2018-09-12 06:19:28.000000 directdm-2.2.2/setup.py
```

### Comparing `directdm-2.2.1/PKG-INFO` & `directdm-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: directdm
-Version: 2.2.1
+Version: 2.2.2
 Summary: A python package for dark matter direct detection
 Home-page: https://directdm.github.io
 Author: Fady Bishara, Joachim Brod, Benjamin Grinstein, Jure Zupan
 Author-email: joachim.brod@uc.edu
 License: MIT
 Description:  This package contains classes for Wilson coefficients
                                    for dark matter -- standard model interactions,
```

### Comparing `directdm-2.2.1/README.md` & `directdm-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/dm_eft.py` & `directdm-2.2.2/directdm/dm_eft.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/match/dim4_gauge_contribution.py` & `directdm-2.2.2/directdm/match/dim4_gauge_contribution.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/num/num_input.py` & `directdm-2.2.2/directdm/num/num_input.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/num/single_nucleon_form_factors.py` & `directdm-2.2.2/directdm/num/single_nucleon_form_factors.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/run/adm.py` & `directdm-2.2.2/directdm/run/adm.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,43 +22,39 @@
 #
 # 'C61u', 'C61d', 'C61s', 'C61c', 'C61b', 'C61e', 'C61mu', 'C61tau', 
 # 'C62u', 'C62d', 'C62s', 'C62c', 'C62b', 'C62e', 'C62mu', 'C62tau',
 # 'C63u', 'C63d', 'C63s', 'C63c', 'C63b', 'C63e', 'C63mu', 'C63tau', 
 # 'C64u', 'C64d', 'C64s', 'C64c', 'C64b', 'C64e', 'C64mu', 'C64tau',
 
 
-# dim.7 (129 operators)
+# dim.7 (97 operators)
 #
 # 'C71', 'C72', 'C73', 'C74',
 # 'C75u', 'C75d', 'C75s', 'C75c', 'C75b', 'C75e', 'C75mu', 'C75tau', 
 # 'C76u', 'C76d', 'C76s', 'C76c', 'C76b', 'C76e', 'C76mu', 'C76tau',
 # 'C77u', 'C77d', 'C77s', 'C77c', 'C77b', 'C77e', 'C77mu', 'C77tau', 
 # 'C78u', 'C78d', 'C78s', 'C78c', 'C78b', 'C78e', 'C78mu', 'C78tau',
 # 'C79u', 'C79d', 'C79s', 'C79c', 'C79b', 'C79e', 'C79mu', 'C79tau', 
 # 'C710u', 'C710d', 'C710s', 'C710c', 'C710b', 'C710e', 'C710mu', 'C710tau',
 # 'C711', 'C712', 'C713', 'C714',
 # 'C715u', 'C715d', 'C715s', 'C715c', 'C715b', 'C715e', 'C715mu', 'C715tau', 
 # 'C716u', 'C716d', 'C716s', 'C716c', 'C716b', 'C716e', 'C716mu', 'C716tau',
 # 'C717u', 'C717d', 'C717s', 'C717c', 'C717b', 'C717e', 'C717mu', 'C717tau', 
 # 'C718u', 'C718d', 'C718s', 'C718c', 'C718b', 'C718e', 'C718mu', 'C718tau',
-# 'C719u', 'C719d', 'C719s', 'C719c', 'C719b', 'C719e', 'C719mu', 'C719tau', 
-# 'C720u', 'C720d', 'C720s', 'C720c', 'C720b', 'C720e', 'C720mu', 'C720tau', 
-# 'C721u', 'C721d', 'C721s', 'C721c', 'C721b', 'C721e', 'C721mu', 'C721tau', 
-# 'C722u', 'C722d', 'C722s', 'C722c', 'C722b', 'C722e', 'C722mu', 'C722tau',
 # 'C723u', 'C723d', 'C723s', 'C723c', 'C723b', 'C723e', 'C723mu', 'C723tau', 
 # 'C725',
 
 
 # dim.8 (12 operators)
 #
 # 'C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s'
 # 'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s'
 
-# In total, we have 2+32+129+12=175 operators. 
-# In total, we have 2+32+129=163 operators w/o dim.8. 
+# In total, we have 2+32+97+12=143 operators. 
+# In total, we have 2+32+97=131 operators w/o dim.8. 
 
 
 #-----------------------------#
 # The QED anomalous dimension #
 #-----------------------------#
 
 def ADM_QED(nf):
@@ -79,72 +75,68 @@
                            8/3*Qd*Qd*nc, 8/3*Qd*Qe*nc, 8/3*Qd*Qe*nc, 8/3*Qd*Qe*nc],
                           [8/3*Qe*Qu,    8/3*Qe*Qd,    8/3*Qe*Qd,    8/3*Qe*Qu,\
                            8/3*Qe*Qd,    8/3*Qe*Qe,    8/3*Qe*Qe,    8/3*Qe*Qe],
                           [8/3*Qe*Qu,    8/3*Qe*Qd,    8/3*Qe*Qd,    8/3*Qe*Qu,\
                            8/3*Qe*Qd,    8/3*Qe*Qe,    8/3*Qe*Qe,    8/3*Qe*Qe],
                           [8/3*Qe*Qu,    8/3*Qe*Qd,    8/3*Qe*Qd,    8/3*Qe*Qu,\
                            8/3*Qe*Qd,    8/3*Qe*Qe,    8/3*Qe*Qe,    8/3*Qe*Qe]])
-    gamma_QED_1 = np.zeros((2,163))
-    gamma_QED_2 = np.hstack((np.zeros((8,2)),gamma_QED,np.zeros((8,153))))
-    gamma_QED_3 = np.hstack((np.zeros((8,10)),gamma_QED,np.zeros((8,145))))
-    gamma_QED_4 = np.zeros((145,163))
+    gamma_QED_1 = np.zeros((2,131))
+    gamma_QED_2 = np.hstack((np.zeros((8,2)),gamma_QED,np.zeros((8,121))))
+    gamma_QED_3 = np.hstack((np.zeros((8,10)),gamma_QED,np.zeros((8,113))))
+    gamma_QED_4 = np.zeros((113,131))
     gamma_QED = np.vstack((gamma_QED_1, gamma_QED_2, gamma_QED_3, gamma_QED_4))
 
     if nf == 5:
         return gamma_QED
     elif nf == 4:
         return np.delete(np.delete(gamma_QED, [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                               102, 110, 118, 126, 134, 142, 150, 158], 0)\
+                                               102, 110, 118, 126], 0)\
                                             , [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                               102, 110, 118, 126, 134, 142, 150, 158], 1)
+                                               102, 110, 118, 126], 1)
     elif nf == 3:
         return np.delete(np.delete(gamma_QED, [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                49,50, 57,58, 65,66, 73,74, 81,82,\
-                                               93,94, 101,102, 109,110, 117,118,\
-                                               125,126, 133,134, 141,142, 149,150, 158,159], 0)\
+                                               93,94, 101,102, 109,110, 117,118, 125,126], 0)\
                                             , [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                49,50, 57,58, 65,66, 73,74, 81,82,\
-                                               93,94, 101,102, 109,110, 117,118,\
-                                               125,126, 133,134, 141,142, 149,150, 158,159], 1)
+                                               93,94, 101,102, 109,110, 117,118, 125,126], 1)
     else:
         raise Exception("nf has to be 3, 4 or 5")
 
 
 def ADM_QED2(nf):
     """ Return the QED anomalous dimension in the DM-SM sector for nf flavor EFT at alpha^2 """
 
     # Mixing of Q_{11}^(7) into Q_{5,f}^(7) and Q_{12}^(7) into Q_{6,f}^(7),
     # now correctly adapted from Hill et al. [1409.8290]. 
     Qu = 2/3
     Qd = -1/3
     Qe = -1
     gamma_QED2_gf = np.array([[8*Qu**2, 8*Qd**2, 8*Qd**2, 8*Qu**2,\
                               8*Qd**2, 8*Qe**2, 8*Qe**2, 8*Qe**2]])
-    gamma_QED2_1 = np.zeros((86,163))
-    gamma_QED2_2 = np.hstack((np.zeros((1,38)),gamma_QED2_gf,np.zeros((1,117))))
-    gamma_QED2_3 = np.hstack((np.zeros((1,46)),gamma_QED2_gf,np.zeros((1,109))))
-    gamma_QED2_4 = np.zeros((75,163))
+    gamma_QED2_1 = np.zeros((86,131))
+    gamma_QED2_2 = np.hstack((np.zeros((1,38)),gamma_QED2_gf,np.zeros((1,85))))
+    gamma_QED2_3 = np.hstack((np.zeros((1,46)),gamma_QED2_gf,np.zeros((1,77))))
+    gamma_QED2_4 = np.zeros((43,131))
     gamma_QED2 = np.vstack((gamma_QED2_1, gamma_QED2_2, gamma_QED2_3, gamma_QED2_4))
 
     if nf == 5:
         return gamma_QED2
     elif nf == 4:
         return np.delete(np.delete(gamma_QED2, [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                                102, 110, 118, 126, 134, 142, 150, 158], 0)\
+                                                102, 110, 118, 126], 0)\
                                              , [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                                102, 110, 118, 126, 134, 142, 150, 158], 1)
+                                                102, 110, 118, 126], 1)
     elif nf == 3:
         return np.delete(np.delete(gamma_QED2, [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                 49,50, 57,58, 65,66, 73,74, 81,82,\
-                                                93,94, 101,102, 109,110, 117,118,\
-                                                125,126, 133,134, 141,142, 149,150, 158,159], 0)\
+                                                93,94, 101,102, 109,110, 117,118, 125,126], 0)\
                                              , [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                 49,50, 57,58, 65,66, 73,74, 81,82,\
-                                                93,94, 101,102, 109,110, 117,118,\
-                                                125,126, 133,134, 141,142, 149,150, 158,159], 1)
+                                                93,94, 101,102, 109,110, 117,118, 125,126], 1)
     else:
         raise Exception("nf has to be 3, 4 or 5")
 
 
 #------------------------------#
 # The QCD anomalous dimensions #
 #------------------------------#
@@ -161,39 +153,37 @@
                              [0,     0,     gt2qq, 0,     0,     0,     0,     0,     gt2qg],
                              [0,     0,     0,     gt2qq, 0,     0,     0,     0,     gt2qg],
                              [0,     0,     0,     0,     gt2qq, 0,     0,     0,     gt2qg],
                              [0,     0,     0,     0,     0,     0,     0,     0,     0    ],
                              [0,     0,     0,     0,     0,     0,     0,     0,     0    ],
                              [0,     0,     0,     0,     0,     0,     0,     0,     0    ],
                              [gt2gq, gt2gq, gt2gq, gt2gq, gt2gq, 0,     0,     0,     gt2gg]])
-    gamma_QCD_1 = np.zeros((70,163))
-    gamma_QCD_2 = np.hstack((np.zeros((5,70)), gamma_QCD_T, np.zeros((5,88))))
-    gamma_QCD_3 = np.zeros((3,163))
-    gamma_QCD_4 = np.hstack((np.zeros((5,78)), gamma_QCD_T, np.zeros((5,80))))
-    gamma_QCD_5 = np.zeros((71,163))
-    gamma_QCD_6 = np.hstack((np.zeros((9,154)), gamma_twist2))
+    gamma_QCD_1 = np.zeros((70,131))
+    gamma_QCD_2 = np.hstack((np.zeros((5,70)), gamma_QCD_T, np.zeros((5,56))))
+    gamma_QCD_3 = np.zeros((3,131))
+    gamma_QCD_4 = np.hstack((np.zeros((5,78)), gamma_QCD_T, np.zeros((5,48))))
+    gamma_QCD_5 = np.zeros((39,131))
+    gamma_QCD_6 = np.hstack((np.zeros((9,122)), gamma_twist2))
     gamma_QCD = [np.vstack((gamma_QCD_1, gamma_QCD_2, gamma_QCD_3,\
                             gamma_QCD_4, gamma_QCD_5, gamma_QCD_6))]
 
     if nf == 5:
         return gamma_QCD
     elif nf == 4:
         return np.delete(np.delete(gamma_QCD, [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                               102, 110, 118, 126, 134, 142, 150, 158], 1)\
+                                               102, 110, 118, 126], 1)\
                                             , [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                               102, 110, 118, 126, 134, 142, 150, 158], 2)
+                                               102, 110, 118, 126], 2)
     elif nf == 3:
         return np.delete(np.delete(gamma_QCD, [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                49,50, 57,58, 65,66, 73,74, 81,82,\
-                                               93,94, 101,102, 109,110, 117,118,\
-                                               125,126, 133,134, 141,142, 149,150, 158,159], 1)\
+                                               93,94, 101,102, 109,110, 117,118, 125,126], 1)\
                                             , [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                49,50, 57,58, 65,66, 73,74, 81,82,\
-                                               93,94, 101,102, 109,110, 117,118,\
-                                               125,126, 133,134, 141,142, 149,150, 158,159], 2)
+                                               93,94, 101,102, 109,110, 117,118, 125,126], 2)
     else:
         raise Exception("nf has to be 3, 4 or 5")
 
 
 def ADM_QCD2(nf):
 
     # CHECK ADM #
@@ -204,39 +194,37 @@
     cf = 4/3
     gamma_gq = 8*cf # changed 2019-08-29, double check with RG solution
     # Mixing of Q_3^(7) into Q_{7,q}^(7) and Q_4^(7) into Q_{8,q}^(7), from Hill et al. [1409.8290].
     # Note that we have different prefactors and signs. 
     gamma_5gq = -8 # changed 2019-08-29, double check with RG solution
     gamma_QCD2_gq = np.array([5*[gamma_gq]])
     gamma_QCD2_5gq = np.array([5*[gamma_5gq]])
-    gamma_QCD2_1 = np.zeros((34,163))
-    gamma_QCD2_2 = np.hstack((np.zeros((1,38)),gamma_QCD2_gq,np.zeros((1,120))))
-    gamma_QCD2_3 = np.hstack((np.zeros((1,46)),gamma_QCD2_gq,np.zeros((1,112))))
-    gamma_QCD2_4 = np.hstack((np.zeros((1,54)),gamma_QCD2_5gq,np.zeros((1,104))))
-    gamma_QCD2_5 = np.hstack((np.zeros((1,62)),gamma_QCD2_5gq,np.zeros((1,96))))
-    gamma_QCD2_6 = np.zeros((125,163))
+    gamma_QCD2_1 = np.zeros((34,131))
+    gamma_QCD2_2 = np.hstack((np.zeros((1,38)),gamma_QCD2_gq,np.zeros((1,88))))
+    gamma_QCD2_3 = np.hstack((np.zeros((1,46)),gamma_QCD2_gq,np.zeros((1,80))))
+    gamma_QCD2_4 = np.hstack((np.zeros((1,54)),gamma_QCD2_5gq,np.zeros((1,72))))
+    gamma_QCD2_5 = np.hstack((np.zeros((1,62)),gamma_QCD2_5gq,np.zeros((1,64))))
+    gamma_QCD2_6 = np.zeros((93,131))
     gamma_QCD2 = [np.vstack((gamma_QCD2_1, gamma_QCD2_2, gamma_QCD2_3,\
                              gamma_QCD2_4, gamma_QCD2_5, gamma_QCD2_6))]
 
     if nf == 5:
         return gamma_QCD2
     elif nf == 4:
         return np.delete(np.delete(gamma_QCD2, [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                                102, 110, 118, 126, 134, 142, 150, 158], 1)\
+                                                102, 110, 118, 126], 1)\
                                              , [6, 14, 22, 30, 42, 50, 58, 66, 74, 82, 94,\
-                                                102, 110, 118, 126, 134, 142, 150, 158], 2)
+                                                102, 110, 118, 126], 2)
     elif nf == 3:
         return np.delete(np.delete(gamma_QCD2, [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                 49,50, 57,58, 65,66, 73,74, 81,82,\
-                                                93,94, 101,102, 109,110, 117,118,\
-                                                125,126, 133,134, 141,142, 149,150, 158,159], 1)\
+                                                93,94, 101,102, 109,110, 117,118, 125,126], 1)\
                                              , [5,6, 13,14, 21,22, 29,30, 41,42,\
                                                 49,50, 57,58, 65,66, 73,74, 81,82,\
-                                                93,94, 101,102, 109,110, 117,118,\
-                                                125,126, 133,134, 141,142, 149,150, 158,159], 2)
+                                                93,94, 101,102, 109,110, 117,118, 125,126], 2)
     else:
         raise Exception("nf has to be 3, 4 or 5")
 
 
 
 def ADM5(Ychi, dchi):
     """ The dimension-five anomalous dimension
```

### Comparing `directdm-2.2.1/directdm/run/full_adm_g1.py` & `directdm-2.2.2/directdm/run/full_adm_g1.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/run/full_adm_g2.py` & `directdm-2.2.2/directdm/run/full_adm_g2.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/run/full_adm_yb.py` & `directdm-2.2.2/directdm/run/full_adm_yb.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/run/rge.py` & `directdm-2.2.2/directdm/run/rge.py`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/directdm/wilson_coefficients.py` & `directdm-2.2.2/directdm/wilson_coefficients.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class WC_3flavor(object):
     def __init__(self, coeff_dict, DM_type, input_dict):
         """ Class for Wilson coefficients in 3 flavor QCD x QED plus DM.
 
         The first argument should be a dictionary for the initial conditions
-        of the 2 + 24 + 4 + 36 + 4 + 48 + 6 + 1 + 12 = 137 
+        of the 2 + 24 + 4 + 36 + 4 + 24 + 6 + 1 + 12 = 113
         dimension-five to dimension-eight three-flavor-QCD Wilson coefficients of the form
         {'C51' : value, 'C52' : value, ...}. 
         An arbitrary number of them can be given; the default values are zero. 
 
         The second argument is the DM type; it can take the following values: 
             "D" (Dirac fermion)
             "M" (Majorana fermion)
@@ -68,45 +68,37 @@
                              'C79u', 'C79d', 'C79s', 'C79e', 'C79mu', 'C79tau',
                              'C710u', 'C710d', 'C710s', 'C710e', 'C710mu', 'C710tau',
                              'C711', 'C712', 'C713', 'C714',
                              'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau',
                              'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
                              'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau',
                              'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
-                             'C719u', 'C719d', 'C719s', 'C719e', 'C719mu', 'C719tau',
-                             'C720u', 'C720d', 'C720s', 'C720e', 'C720mu', 'C720tau',
-                             'C721u', 'C721d', 'C721s', 'C721e', 'C721mu', 'C721tau',
-                             'C722u', 'C722d', 'C722s', 'C722e', 'C722mu', 'C722tau',
                              'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
                              'C725',
                              'C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s'
                              'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s'
 
         Majorana fermion:    'C62u', 'C62d', 'C62s', 'C62e', 'C62mu', 'C62tau',
                              'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                              'C71', 'C72', 'C73', 'C74',
                              'C75u', 'C75d', 'C75s', 'C75e', 'C75mu', 'C75tau', 
                              'C76u', 'C76d', 'C76s', 'C76e', 'C76mu', 'C76tau',
                              'C77u', 'C77d', 'C77s', 'C77e', 'C77mu', 'C77tau', 
                              'C78u', 'C78d', 'C78s', 'C78e', 'C78mu', 'C78tau',
                              'C711', 'C712', 'C713', 'C714',
-                             'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau', 
-                             'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
-                             'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau', 
-                             'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
                              'C82u', 'C82d', 'C82s', 'C84u', 'C84d', 'C84s'
 
         Complex Scalar:      'C61u', 'C61d', 'C61s', 'C61e', 'C61mu', 'C61tau', 
                              'C62u', 'C62d', 'C62s', 'C62e', 'C62mu', 'C62tau',
                              'C63u', 'C63d', 'C63s', 'C63e', 'C63mu', 'C63tau', 
                              'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                              'C65', 'C66', 'C67', 'C68' 
-                             'C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s',
                              'C69u', 'C69d', 'C69s', 'C69e', 'C69mu', 'C69tau', 
                              'C610'
+                             'C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s',
 
         Real Scalar:         'C63u', 'C63d', 'C63s', 'C63e', 'C63mu', 'C63tau', 
                              'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                              'C65', 'C66', 'C67', 'C68',
                              'C69u', 'C69d', 'C69s', 'C69e', 'C69mu', 'C69tau', 
                              'C610'
 
@@ -168,18 +160,14 @@
                                  'C79u', 'C79d', 'C79s', 'C79e', 'C79mu', 'C79tau',
                                  'C710u', 'C710d', 'C710s', 'C710e', 'C710mu', 'C710tau',
                                  'C711', 'C712', 'C713', 'C714',
                                  'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau',
                                  'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
                                  'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau',
                                  'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
-                                 'C719u', 'C719d', 'C719s', 'C719e', 'C719mu', 'C719tau',
-                                 'C720u', 'C720d', 'C720s', 'C720e', 'C720mu', 'C720tau', 
-                                 'C721u', 'C721d', 'C721s', 'C721e', 'C721mu', 'C721tau',
-                                 'C722u', 'C722d', 'C722s', 'C722e', 'C722mu', 'C722tau',
                                  'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
                                  'C725']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s',
                                   'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s']
 
         if self.DM_type == "M":
@@ -187,25 +175,21 @@
                                  'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                                  'C71', 'C72', 'C73', 'C74',
                                  'C75u', 'C75d', 'C75s', 'C75e', 'C75mu', 'C75tau',
                                  'C76u', 'C76d', 'C76s', 'C76e', 'C76mu', 'C76tau',
                                  'C77u', 'C77d', 'C77s', 'C77e', 'C77mu', 'C77tau',
                                  'C78u', 'C78d', 'C78s', 'C78e', 'C78mu', 'C78tau',
                                  'C711', 'C712', 'C713', 'C714',
-                                 'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau',
-                                 'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
-                                 'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau',
-                                 'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
                                  'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
                                  'C725']
 
             self.wc8_name_list = ['C82u', 'C82d', 'C82s', 'C84u', 'C84d', 'C84s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
-            del_ind_list = np.r_[np.s_[0:8], np.s_[14:20], np.s_[54:66], np.s_[94:118]]
+            del_ind_list = np.r_[np.s_[0:8], np.s_[14:20], np.s_[54:66], np.s_[70:94]]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
 
         if self.DM_type == "C":
             self.wc_name_list = ['C61u', 'C61d', 'C61s', 'C61e', 'C61mu', 'C61tau', 
                                  'C62u', 'C62d', 'C62s', 'C62e', 'C62mu', 'C62tau',
                                  'C65', 'C66',
@@ -215,15 +199,15 @@
                                  'C69u', 'C69d', 'C69s', 'C69e', 'C69mu', 'C69tau', 
                                  'C610']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = np.r_[np.s_[0:2], np.s_[8:14], np.s_[20:26], np.s_[27:28], np.s_[29:30],\
-                                 np.s_[36:42], np.s_[48:66], np.s_[67:68], np.s_[69:70], np.s_[70:118]]
+                                 np.s_[36:42], np.s_[48:66], np.s_[67:68], np.s_[69:70], np.s_[70:94]]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
 
         if self.DM_type == "R":
             self.wc_name_list = ['C65', 'C66',
                                  'C63u', 'C63d', 'C63s', 'C63e', 'C63mu', 'C63tau', 
                                  'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
@@ -231,15 +215,15 @@
                                  'C69u', 'C69d', 'C69s', 'C69e', 'C69mu', 'C69tau', 
                                  'C610']
 
             self.wc8_name_list = []
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = np.r_[np.s_[0:26], np.s_[27:28], np.s_[29:30], np.s_[36:42],\
-                                 np.s_[48:66], np.s_[67:68], np.s_[69:70], np.s_[70:118]]
+                                 np.s_[48:66], np.s_[67:68], np.s_[69:70], np.s_[70:94]]
 
         self.coeff_dict = {}
 
         # Issue a user warning if a key is not defined:
 
         for wc_name in coeff_dict.keys():
             if wc_name in self.wc_name_list:
@@ -544,69 +528,71 @@
         if self.DM_type == "D":
             my_cNR_dict = {
             'cNR1p' :   F1up*(c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
                       + F1dp*(c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                       + FGp*c3mu_dict['C71']\
                       + FSup*c3mu_dict['C75u'] + FSdp*c3mu_dict['C75d'] + FSsp*c3mu_dict['C75s']\
                       - alpha/(2*np.pi*DM_mass)*c3mu_dict['C51']\
-                      + 2*DM_mass * (F1up*c3mu_dict['C715u'] + F1dp*c3mu_dict['C715d'] + F1sp*c3mu_dict['C715s'])\
                       + FTW2up*c3mu_dict['C723u']\
                       + FTW2dp*c3mu_dict['C723d']\
                       + FTW2sp*c3mu_dict['C723s']\
                       + FTW2gp*c3mu_dict['C725'],
             'cNR2p' : 0,
             'cNR3p' : F2sp*(c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                            + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
                            + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']))\
                       - 2*alpha/np.pi * self.ip['mup']/mN * c3mu_dict['C51']\
                       + 8*(FT0up*c3mu_dict['C79u'] + FT0dp*c3mu_dict['C79d'] + FT0sp*c3mu_dict['C79s']),
-            'cNR5p' : - 2*mN * (F1up*c3mu_dict['C719u'] + F1dp*c3mu_dict['C719d'] + F1sp*c3mu_dict['C719s']),
+            'cNR5p' : - 2*mN * (  F1up*c3mu_dict['C715u']\
+                                + F1dp*c3mu_dict['C715d']\
+                                + F1sp*c3mu_dict['C715s']),
             'cNR6p' : mN/DM_mass * FGtildep * c3mu_dict['C74']\
-                      -2*mN*((F1up+F2up)*c3mu_dict['C719u']\
-                             + (F1dp+F2dp)*c3mu_dict['C719d']\
-                             + (F1sp+F2sp)*c3mu_dict['C719s'])\
+                      -2*mN*(  (F1up+F2up)*c3mu_dict['C715u']\
+                             + (F1dp+F2dp)*c3mu_dict['C715d']\
+                             + (F1sp+F2sp)*c3mu_dict['C715s'])\
                       + mN/DM_mass*F2sp*(c3mu_dict['C61s']
                                          - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR7p' : - 2*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
                            + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                           + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
-                      - 4*DM_mass * (FAup*c3mu_dict['C717u'] + FAdp*c3mu_dict['C717d'] + FAsp*c3mu_dict['C717s']),
+                           + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s'])),
             'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
             'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u']\
                            - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + (F1dp+F2dp)*(c3mu_dict['C62d']\
                            - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                          + (F1sp+F2sp)*(c3mu_dict['C62s']\
                            - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s']))\
                       + 2*mN*(  FAup*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
                               + FAdp*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
                               + FAsp*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
                              /DM_mass\
-                      - 4*mN * (FAup*c3mu_dict['C721u'] + FAdp*c3mu_dict['C721d'] + FAsp*c3mu_dict['C721s']),
+                      - 4*mN * (  FAup*c3mu_dict['C717u']\
+                                + FAdp*c3mu_dict['C717d']\
+                                + FAsp*c3mu_dict['C717s']),
             'cNR10p' : FGtildep * c3mu_dict['C73']\
                        -2*mN/DM_mass * (FT0up*c3mu_dict['C710u']\
                                         + FT0dp*c3mu_dict['C710d']\
                                         + FT0sp*c3mu_dict['C710s']),
             'cNR11p' : - mN/DM_mass * (FSup*c3mu_dict['C76u']\
                                        + FSdp*c3mu_dict['C76d']\
                                        + FSsp*c3mu_dict['C76s'])\
                        - mN/DM_mass * FGp * c3mu_dict['C72']\
                         + 2*((FT0up-FT1up)*c3mu_dict['C710u']\
                              + (FT0dp-FT1dp)*c3mu_dict['C710d']\
                              + (FT0sp-FT1sp)*c3mu_dict['C710s'])\
-                        - 2*mN * (  F1up*(c3mu_dict['C716u']+c3mu_dict['C720u'])\
-                                  + F1dp*(c3mu_dict['C716d']+c3mu_dict['C720d'])\
-                                  + F1sp*(c3mu_dict['C716s']+c3mu_dict['C720s'])),
+                        - 2*mN * (  F1up*(c3mu_dict['C716u'])\
+                                  + F1dp*(c3mu_dict['C716d'])\
+                                  + F1sp*(c3mu_dict['C716s'])),
             'cNR12p' : -8*(FT0up*c3mu_dict['C710u'] + FT0dp*c3mu_dict['C710d'] + FT0sp*c3mu_dict['C710s']),
             'cNR13p' : 0.,
-            'cNR14p' : + 4*mN * (  FAup*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
-                                 + FAdp*(c3mu_dict['C718d']+c3mu_dict['C722d'])\
-                                 + FAsp*(c3mu_dict['C718s']+c3mu_dict['C722s'])),
+            'cNR14p' : + 4*mN * (  FAup*(c3mu_dict['C718u'])\
+                                 + FAdp*(c3mu_dict['C718d'])\
+                                 + FAsp*(c3mu_dict['C718s'])),
 
             'cNR6pip' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
                        + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                        + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
             'cNR6etap' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
                                      + FPdp_eta*c3mu_dict['C78d']\
                                      + FPsp_eta*c3mu_dict['C78s'])\
@@ -621,86 +607,86 @@
             'cNR10q2pip' : FGtildep_pion * c3mu_dict['C73'],
             'cNR10q2etap' : FGtildep_eta * c3mu_dict['C73'],
     
             'cNR5bq2p' : mN* (2*alpha/np.pi*c3mu_dict['C51']),
             'cNR6bq2p' : -mN**2* (- 2*alpha/np.pi * self.ip['mup']/mN * c3mu_dict['C51']),
             'cNR11bq2p' : mN* (2*alpha/np.pi*c3mu_dict['C52']),
 
-            'cNR1q2p' : (  F1up*c3mu_dict['C719u']\
-                         + F1dp*c3mu_dict['C719d']\
-                         + F1sp*c3mu_dict['C719s'])/(2*DM_mass)\
+            'cNR1q2p' : (  F1up*c3mu_dict['C715u']\
+                         + F1dp*c3mu_dict['C715d']\
+                         + F1sp*c3mu_dict['C715s'])/(2*DM_mass)\
                         + (F1spslope - F2sp / mN**2/4)
                           * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
-            'cNR4q2p' : 2*((F1up+F2up)*c3mu_dict['C719u']\
-                           + (F1dp+F2dp)*c3mu_dict['C719d']\
-                           + (F1sp+F2sp)*c3mu_dict['C719s'])/mN\
+            'cNR4q2p' : 2*(  (F1up+F2up)*c3mu_dict['C715u']\
+                           + (F1dp+F2dp)*c3mu_dict['C715d']\
+                           + (F1sp+F2sp)*c3mu_dict['C715s'])/mN\
                         - 1/mN/DM_mass * F2sp
                           * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
 
 
 
 
             'cNR1n' :   F1un*(c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
                       + F1dn*(c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
                       + FGn*c3mu_dict['C71']\
                       + FSun*c3mu_dict['C75u'] + FSdn*c3mu_dict['C75d'] + FSsn*c3mu_dict['C75s']\
-                      + 2*DM_mass * (F1un*c3mu_dict['C715u'] + F1dn*c3mu_dict['C715d'] + F1sn*c3mu_dict['C715s'])\
                       + FTW2un*c3mu_dict['C723u']\
                       + FTW2dn*c3mu_dict['C723d']\
                       + FTW2sn*c3mu_dict['C723s']\
                       + FTW2gn*c3mu_dict['C725'],
             'cNR2n' : 0,
             'cNR3n' : F2sn*(c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                            + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
                            + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s']))\
                       - 2*alpha/np.pi * self.ip['mun']/mN * c3mu_dict['C51']\
                       + 8*(FT0un*c3mu_dict['C79u'] + FT0dn*c3mu_dict['C79d'] + FT0sn*c3mu_dict['C79s']),
-            'cNR5n' : - 2*mN * (F1un*c3mu_dict['C719u'] + F1dn*c3mu_dict['C719d'] + F1sn*c3mu_dict['C719s']),
+            'cNR5n' : - 2*mN * (  F1un*c3mu_dict['C715u']\
+                                + F1dn*c3mu_dict['C715d']\
+                                + F1sn*c3mu_dict['C715s']),
             'cNR6n' : mN/DM_mass * FGtilden * c3mu_dict['C74']\
-                      -2*mN*((F1un+F2un)*c3mu_dict['C719u']\
-                             + (F1dn+F2dn)*c3mu_dict['C719d']\
-                             + (F1sn+F2sn)*c3mu_dict['C719s'])\
+                      -2*mN*(  (F1un+F2un)*c3mu_dict['C715u']\
+                             + (F1dn+F2dn)*c3mu_dict['C715d']\
+                             + (F1sn+F2sn)*c3mu_dict['C715s'])\
                       + mN/DM_mass * F2sn
                         * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
             'cNR7n' : - 2*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
                            + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
-                           + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
-                      - 4*DM_mass * (FAun*c3mu_dict['C717u'] + FAdn*c3mu_dict['C717d']+ FAsn*c3mu_dict['C717s']),
+                           + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s'])),
             'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
             'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                          + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s']))\
                       + 2*mN*(  FAun*(c3mu_dict['C63u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C83u'])\
                               + FAdn*(c3mu_dict['C63d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C83d'])\
                               + FAsn*(c3mu_dict['C63s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C83s']))\
                              /DM_mass\
-                      - 4*mN * (FAun*c3mu_dict['C721u']\
-                                + FAdn*c3mu_dict['C721d']\
-                                + FAsn*c3mu_dict['C721s']),
+                      - 4*mN * (  FAun*c3mu_dict['C717u']\
+                                + FAdn*c3mu_dict['C717d']\
+                                + FAsn*c3mu_dict['C717s']),
             'cNR10n' : FGtilden * c3mu_dict['C73']\
                      -2*mN/DM_mass * (FT0un*c3mu_dict['C710u']\
                                       + FT0dn*c3mu_dict['C710d']\
                                       + FT0sn*c3mu_dict['C710s']),
             'cNR11n' : - mN/DM_mass * (FSun*c3mu_dict['C76u']\
                                        + FSdn*c3mu_dict['C76d']\
                                        + FSsn*c3mu_dict['C76s'])\
                        - mN/DM_mass * FGn * c3mu_dict['C72']\
                        + 2*((FT0un-FT1un)*c3mu_dict['C710u']\
                             + (FT0dn-FT1dn)*c3mu_dict['C710d']\
                             + (FT0sn-FT1sn)*c3mu_dict['C710s'])\
-                       - 2*mN * (  F1un*(c3mu_dict['C716u']+c3mu_dict['C720u'])\
-                                 + F1dn*(c3mu_dict['C716d']+c3mu_dict['C720d'])\
-                                 + F1sn*(c3mu_dict['C716s']+c3mu_dict['C720s'])),
+                       - 2*mN * (  F1un*(c3mu_dict['C716u'])\
+                                 + F1dn*(c3mu_dict['C716d'])\
+                                 + F1sn*(c3mu_dict['C716s'])),
             'cNR12n' : -8*(FT0un*c3mu_dict['C710u'] + FT0dn*c3mu_dict['C710d'] + FT0sn*c3mu_dict['C710s']),
             'cNR13n' : 0.,
-            'cNR14n' :           + 4*mN * (  FAun*(c3mu_dict['C718u']+c3mu_dict['C722u'])\
-                                 + FAdn*(c3mu_dict['C718d']+c3mu_dict['C722d'])\
-                                 + FAsn*(c3mu_dict['C718s']+c3mu_dict['C722s'])),
+            'cNR14n' : + 4*mN * (  FAun*(c3mu_dict['C718u'])\
+                                 + FAdn*(c3mu_dict['C718d'])\
+                                 + FAsn*(c3mu_dict['C718s'])),
     
             'cNR6pin' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
                        + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                        + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
             'cNR6etan' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
                                      + FPdn_eta*c3mu_dict['C78d']\
                                      + FPsn_eta*c3mu_dict['C78s'])\
@@ -715,81 +701,70 @@
             'cNR10q2pin' : FGtilden_pion * c3mu_dict['C73'],
             'cNR10q2etan' : FGtilden_eta * c3mu_dict['C73'],
     
             'cNR5bq2n' : 0,
             'cNR6bq2n' : -mN**2 * (- 2*alpha/np.pi * self.ip['mun']/mN * c3mu_dict['C51']),
             'cNR11bq2n' : 0,
 
-            'cNR1q2n' : (  F1un*c3mu_dict['C719u']\
-                         + F1dn*c3mu_dict['C719d']\
-                         + F1sn*c3mu_dict['C719s'])/(2*DM_mass)\
+            'cNR1q2n' : (  F1un*c3mu_dict['C715u']\
+                         + F1dn*c3mu_dict['C715d']\
+                         + F1sn*c3mu_dict['C715s'])/(2*DM_mass)\
                         + (F1snslope - F2sn / mN**2/4)
                           * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s']),
-            'cNR4q2n' : 2*((F1un+F2un)*c3mu_dict['C719u']\
-                           + (F1dn+F2dn)*c3mu_dict['C719d']\
-                           + (F1sn+F2sn)*c3mu_dict['C719s'])/mN\
+            'cNR4q2n' : 2*(  (F1un+F2un)*c3mu_dict['C715u']\
+                           + (F1dn+F2dn)*c3mu_dict['C715d']\
+                           + (F1sn+F2sn)*c3mu_dict['C715s'])/mN\
                         - 1/mN/DM_mass * F2sn
                           * (c3mu_dict['C61s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C81s'])
             }
 
             if NLO:
                 my_cNR_dict['cNR5p'] = my_cNR_dict['cNR5p']\
-                                       - 2*mN * (F1un*c3mu_dict['C719u']\
-                                                 + F1dn*c3mu_dict['C719d']\
-                                                 + F1sn*c3mu_dict['C719s'])\
-                                       + 2*((FT0up-FT1up)*c3mu_dict['C79u']\
+                                       + 2*(  (FT0up-FT1up)*c3mu_dict['C79u']\
                                             + (FT0dp-FT1dp)*c3mu_dict['C79d']\
                                             + (FT0sp-FT1sp)*c3mu_dict['C79s'])
                 my_cNR_dict['cNR1q2p'] = my_cNR_dict['cNR1q2p']\
-                                         - ((FT0up-FT1up)*c3mu_dict['C79u']\
+                                         - (  (FT0up-FT1up)*c3mu_dict['C79u']\
                                             + (FT0dp-FT1dp)*c3mu_dict['C79d']\
                                             + (FT0sp-FT1sp)*c3mu_dict['C79s'])/(2*DM_mass*mN)
                 my_cNR_dict['cNR5n'] = my_cNR_dict['cNR5n']\
-                                       - 2*mN * (F1un*c3mu_dict['C719u']\
-                                                 + F1dn*c3mu_dict['C719d'] + F1sn*c3mu_dict['C719s'])\
-                                       + 2*((FT0un-FT1un)*c3mu_dict['C79u']\
+                                       + 2*(  (FT0un-FT1un)*c3mu_dict['C79u']\
                                             + (FT0dn-FT1dn)*c3mu_dict['C79d']\
                                             + (FT0sn-FT1sn)*c3mu_dict['C79s'])
                 my_cNR_dict['cNR1q2n'] = my_cNR_dict['cNR1q2n']\
-                                         - ((FT0un-FT1un)*c3mu_dict['C79u']\
+                                         - (  (FT0un-FT1un)*c3mu_dict['C79u']\
                                             + (FT0dn-FT1dn)*c3mu_dict['C79d']\
                                             + (FT0sn-FT1sn)*c3mu_dict['C79s'])/(2*DM_mass*mN)
 
 
         if self.DM_type == "M":
             my_cNR_dict = {
             'cNR1p' : FGp*c3mu_dict['C71']\
-                      + FSup*c3mu_dict['C75u'] + FSdp*c3mu_dict['C75d'] + FSsp*c3mu_dict['C75s']\
-                      + 2*DM_mass * (F1up*c3mu_dict['C715u'] + F1dp*c3mu_dict['C715d'] + F1sp*c3mu_dict['C715s']),
-            'cNR2p' : 0,
-            'cNR3p' : 0,
+                      + FSup*c3mu_dict['C75u'] + FSdp*c3mu_dict['C75d'] + FSsp*c3mu_dict['C75s'],
+            'cNR2p' : 0.,
+            'cNR3p' : 0.,
             'cNR4p' : - 4*(  FAup*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                            + FAdp*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
                            + FAsp*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s'])),
             'cNR5p' : 0,
             'cNR6p' : mN/DM_mass * FGtildep * c3mu_dict['C74'],
-            'cNR7p' : - 4*DM_mass * (FAup*c3mu_dict['C717u'] + FAdp*c3mu_dict['C717d'] + FAsp*c3mu_dict['C717s']),
+            'cNR7p' : 0,
             'cNR8p' : 2*(  F1up*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + F1dp*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
             'cNR9p' : 2*(  (F1up+F2up)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + (F1dp+F2dp)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                          + (F1sp+F2sp)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR10p' : FGtildep * c3mu_dict['C73'],
             'cNR11p' : - mN/DM_mass * (FSup*c3mu_dict['C76u']\
                                        + FSdp*c3mu_dict['C76d']\
                                        + FSsp*c3mu_dict['C76s'])\
-                       - mN/DM_mass * FGp * c3mu_dict['C72']\
-                       - 2*mN * (  F1up*c3mu_dict['C716u']\
-                                   + F1dp*c3mu_dict['C716d']\
-                                   + F1sp*c3mu_dict['C716s']),
-            'cNR12p' : 0,
+                       - mN/DM_mass * FGp * c3mu_dict['C72'],
+            'cNR12p' : 0.,
             'cNR13p' : 0.,
-            'cNR14p' : + 4*mN * (FAup*c3mu_dict['C718u']\
-                                 + FAdp*c3mu_dict['C718d']\
-                                 + FAsp*c3mu_dict['C718s']),
+            'cNR14p' : 0.,
     
             'cNR6pip' : mN/DM_mass * (FPup_pion*c3mu_dict['C78u'] + FPdp_pion*c3mu_dict['C78d'])\
                        + FPpup_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                        + FPpdp_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
             'cNR6etap' : mN/DM_mass * (FPup_eta*c3mu_dict['C78u']\
                                      + FPdp_eta*c3mu_dict['C78d']\
                                      + FPsp_eta*c3mu_dict['C78s'])\
@@ -800,53 +775,47 @@
             'cNR6q2etap' : mN/DM_mass * FGtildep_eta * c3mu_dict['C74'],
     
             'cNR10pip' : FPup_pion*c3mu_dict['C77u'] + FPdp_pion*c3mu_dict['C77d'],
             'cNR10etap' : FPup_eta*c3mu_dict['C77u'] + FPdp_eta*c3mu_dict['C77d'] + FPsp_eta*c3mu_dict['C77s'],
             'cNR10q2pip' : FGtildep_pion * c3mu_dict['C73'],
             'cNR10q2etap' : FGtildep_eta * c3mu_dict['C73'],
     
-            'cNR5bq2p' : 0,
-            'cNR6bq2p' : 0,
-            'cNR11bq2p' : 0,
+            'cNR5bq2p' : 0.,
+            'cNR6bq2p' : 0.,
+            'cNR11bq2p' : 0.,
 
-            'cNR1q2p' : 0,
-            'cNR4q2p' : 0,
+            'cNR1q2p' : 0.,
+            'cNR4q2p' : 0.,
 
 
 
 
             'cNR1n' :   FGn*c3mu_dict['C71']\
-                      + FSun*c3mu_dict['C75u'] + FSdn*c3mu_dict['C75d'] + FSsn*c3mu_dict['C75s']\
-                      + 2*DM_mass * (F1un*c3mu_dict['C715u'] + F1dn*c3mu_dict['C715d'] + F1sn*c3mu_dict['C715s']),
-            'cNR2n' : 0,
-            'cNR3n' : 0,
+                      + FSun*c3mu_dict['C75u'] + FSdn*c3mu_dict['C75d'] + FSsn*c3mu_dict['C75s'],
+            'cNR2n' : 0.,
+            'cNR3n' : 0.,
             'cNR4n' : - 4*(  FAun*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                            + FAdn*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d'])\
                            + FAsn*(c3mu_dict['C64s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C84s'])),
-            'cNR5n' : 0,
+            'cNR5n' : 0.,
             'cNR6n' : mN/DM_mass * FGtilden * c3mu_dict['C74'],
-            'cNR7n' : - 4*DM_mass * (FAun*c3mu_dict['C717u'] + FAdn*c3mu_dict['C717d'] + FAsn*c3mu_dict['C717s']),
+            'cNR7n' : 0.,
             'cNR8n' : 2*(  F1un*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + F1dn*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])),
             'cNR9n' : 2*(  (F1un+F2un)*(c3mu_dict['C62u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C82u'])\
                          + (F1dn+F2dn)*(c3mu_dict['C62d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C82d'])\
                          + (F1sn+F2sn)*(c3mu_dict['C62s'] - np.sqrt(2)*GF*ms**2 / gs2_2GeV * c3mu_dict['C82s'])),
             'cNR10n' : FGtilden * c3mu_dict['C73'],
             'cNR11n' : - mN/DM_mass * (FSun*c3mu_dict['C76u']\
                                        + FSdn*c3mu_dict['C76d']\
                                        + FSsn*c3mu_dict['C76s'])\
-                       - mN/DM_mass * FGn * c3mu_dict['C72']\
-                       - 2*mN * (  F1un*c3mu_dict['C716u']\
-                                   + F1dn*c3mu_dict['C716d']\
-                                   + F1sn*c3mu_dict['C716s']),
-            'cNR12n' : 0,
-            'cNR13p' : 0.,
-            'cNR14n' : + 4*mN * (FAun*c3mu_dict['C718u']\
-                                 + FAdn*c3mu_dict['C718d']\
-                                 + FAsn*c3mu_dict['C718s']),
+                       - mN/DM_mass * FGn * c3mu_dict['C72'],
+            'cNR12n' : 0.,
+            'cNR13n' : 0.,
+            'cNR14n' : 0.,
     
             'cNR6pin' : mN/DM_mass * (FPun_pion*c3mu_dict['C78u'] + FPdn_pion*c3mu_dict['C78d'])\
                        + FPpun_pion*(c3mu_dict['C64u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C84u'])\
                        + FPpdn_pion*(c3mu_dict['C64d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C84d']),
             'cNR6etan' : mN/DM_mass * (FPun_eta*c3mu_dict['C78u']\
                                      + FPdn_eta*c3mu_dict['C78d']\
                                      + FPsn_eta*c3mu_dict['C78s'])\
@@ -857,20 +826,20 @@
             'cNR6q2etan' : mN/DM_mass * FGtilden_eta * c3mu_dict['C74'],
     
             'cNR10pin' : FPun_pion*c3mu_dict['C77u'] + FPdn_pion*c3mu_dict['C77d'],
             'cNR10etan' : FPun_eta*c3mu_dict['C77u'] + FPdn_eta*c3mu_dict['C77d'] + FPsn_eta*c3mu_dict['C77s'],
             'cNR10q2pin' : FGtilden_pion * c3mu_dict['C73'],
             'cNR10q2etan' : FGtilden_eta * c3mu_dict['C73'],
     
-            'cNR5bq2n' : 0,
-            'cNR6bq2n' : 0,
-            'cNR11bq2n' : 0,
+            'cNR5bq2n' : 0.,
+            'cNR6bq2n' : 0.,
+            'cNR11bq2n' : 0.,
 
-            'cNR1q2n' : 0,
-            'cNR4q2n' : 0
+            'cNR1q2n' : 0.,
+            'cNR4q2n' : 0.
             }
 
 
         if self.DM_type == "C":
             my_cNR_dict = {
             'cNR1p' :    F1up * (c3mu_dict['C61u'] - np.sqrt(2)*GF*mu**2 / gs2_2GeV * c3mu_dict['C81u'])\
                        + F1dp * (c3mu_dict['C61d'] - np.sqrt(2)*GF*md**2 / gs2_2GeV * c3mu_dict['C81d'])\
@@ -1191,15 +1160,15 @@
 
 
 class WC_4flavor(object):
     def __init__(self, coeff_dict, DM_type, input_dict):
         """ Class for Wilson coefficients in 4 flavor QCD x QED plus DM.
 
         The argument should be a dictionary for the initial conditions
-        of the 2 + 28 + 4 + 42 + 4 + 56 + 7 + 1 + 6 = 150 dimension-five to dimension-eight
+        of the 2 + 28 + 4 + 42 + 4 + 28 + 7 + 1 + 6 = 122 dimension-five to dimension-eight
         four-flavor-QCD Wilson coefficients (for Dirac DM) of the form
         {'C51' : value, 'C52' : value, ...}. For other DM types there are less coefficients.
         An arbitrary number of them can be given; the default values are zero. 
 
         The second argument is the DM type; it can take the following values: 
             "D" (Dirac fermion)
             "M" (Majorana fermion)
@@ -1220,35 +1189,27 @@
                              'C79u', 'C79d', 'C79s', 'C79c', 'C79e', 'C79mu', 'C79tau',
                              'C710u', 'C710d', 'C710s', 'C710c', 'C710e', 'C710mu', 'C710tau',
                              'C711', 'C712', 'C713', 'C714',
                              'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau',
                              'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
                              'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau',
                              'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
-                             'C719u', 'C719d', 'C719s', 'C719c', 'C719e', 'C719mu', 'C719tau',
-                             'C720u', 'C720d', 'C720s', 'C720c', 'C720e', 'C720mu', 'C720tau',
-                             'C721u', 'C721d', 'C721s', 'C721c', 'C721e', 'C721mu', 'C721tau',
-                             'C722u', 'C722d', 'C722s', 'C722c', 'C722e', 'C722mu', 'C722tau',
                              'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau',
                              'C725',
                              'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s'
 
 
         Majorana fermion:    'C62u', 'C62d', 'C62s', 'C62c', 'C62e', 'C62mu', 'C62tau',
                              'C64u', 'C64d', 'C64s', 'C64c', 'C64e', 'C64mu', 'C64tau',
                              'C71', 'C72', 'C73', 'C74',
                              'C75u', 'C75d', 'C75s', 'C75c', 'C75e', 'C75mu', 'C75tau', 
                              'C76u', 'C76d', 'C76s', 'C76c', 'C76e', 'C76mu', 'C76tau',
                              'C77u', 'C77d', 'C77s', 'C77c', 'C77e', 'C77mu', 'C77tau', 
                              'C78u', 'C78d', 'C78s', 'C78c', 'C78e', 'C78mu', 'C78tau',
                              'C711', 'C712', 'C713', 'C714',
-                             'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau', 
-                             'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
-                             'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau', 
-                             'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
                              'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau',
                              'C725',
 
         Complex Scalar:      'C61u', 'C61d', 'C61s', 'C61c', 'C61e', 'C61mu', 'C61tau', 
                              'C62u', 'C62d', 'C62s', 'C62c', 'C62e', 'C62mu', 'C62tau',
                              'C65', 'C66',
                              'C63u', 'C63d', 'C63s', 'C63c', 'C63e', 'C63mu', 'C63tau', 
@@ -1344,18 +1305,14 @@
                                  'C79u', 'C79d', 'C79s', 'C79c', 'C79e', 'C79mu', 'C79tau', 
                                  'C710u', 'C710d', 'C710s', 'C710c', 'C710e', 'C710mu', 'C710tau',
                                  'C711', 'C712', 'C713', 'C714',
                                  'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau', 
                                  'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
                                  'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau', 
                                  'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
-                                 'C719u', 'C719d', 'C719s', 'C719c', 'C719e', 'C719mu', 'C719tau', 
-                                 'C720u', 'C720d', 'C720s', 'C720c', 'C720e', 'C720mu', 'C720tau', 
-                                 'C721u', 'C721d', 'C721s', 'C721c', 'C721e', 'C721mu', 'C721tau', 
-                                 'C722u', 'C722d', 'C722s', 'C722c', 'C722e', 'C722mu', 'C722tau',
                                  'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau',
                                  'C725']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s',\
                                   'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s']
 
             # The 3-flavor list for matching only
@@ -1371,59 +1328,47 @@
                                     'C79u', 'C79d', 'C79s', 'C79e', 'C79mu', 'C79tau',
                                     'C710u', 'C710d', 'C710s', 'C710e', 'C710mu', 'C710tau',
                                     'C711', 'C712', 'C713', 'C714',
                                     'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau', 
                                     'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
                                     'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau', 
                                     'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
-                                    'C719u', 'C719d', 'C719s', 'C719e', 'C719mu', 'C719tau', 
-                                    'C720u', 'C720d', 'C720s', 'C720e', 'C720mu', 'C720tau', 
-                                    'C721u', 'C721d', 'C721s', 'C721e', 'C721mu', 'C721tau', 
-                                    'C722u', 'C722d', 'C722s', 'C722e', 'C722mu', 'C722tau',
                                     'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
                                     'C725']
 
         if self.DM_type == "M":
             self.wc_name_list = ['C62u', 'C62d', 'C62s', 'C62c', 'C62e', 'C62mu', 'C62tau',
                                  'C64u', 'C64d', 'C64s', 'C64c', 'C64e', 'C64mu', 'C64tau',
                                  'C71', 'C72', 'C73', 'C74',
                                  'C75u', 'C75d', 'C75s', 'C75c', 'C75e', 'C75mu', 'C75tau', 
                                  'C76u', 'C76d', 'C76s', 'C76c', 'C76e', 'C76mu', 'C76tau',
                                  'C77u', 'C77d', 'C77s', 'C77c', 'C77e', 'C77mu', 'C77tau', 
                                  'C78u', 'C78d', 'C78s', 'C78c', 'C78e', 'C78mu', 'C78tau',
                                  'C711', 'C712', 'C713', 'C714',
-                                 'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau', 
-                                 'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
-                                 'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau', 
-                                 'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
                                  'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau',
                                  'C725']
 
             self.wc8_name_list = ['C82u', 'C82d', 'C82s', 'C84u', 'C84d', 'C84s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
-            del_ind_list = np.r_[np.s_[0:9], np.s_[16:23], np.s_[62:76], np.s_[108:136]]
+            del_ind_list = np.r_[np.s_[0:9], np.s_[16:23], np.s_[62:76], np.s_[80:108]]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
             # The list of indices to be deleted from the ADT because of less operators (dim.6 part)
             del_ind_list_adt_quark = np.r_[np.s_[0:4]]
 
             # The 3-flavor list for matching only
             self.wc_name_list_3f = ['C62u', 'C62d', 'C62s', 'C62e', 'C62mu', 'C62tau',
                                     'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                                     'C71', 'C72', 'C73', 'C74',
                                     'C75u', 'C75d', 'C75s', 'C75e', 'C75mu', 'C75tau',
                                     'C76u', 'C76d', 'C76s', 'C76e', 'C76mu', 'C76tau',
                                     'C77u', 'C77d', 'C77s', 'C77e', 'C77mu', 'C77tau',
                                     'C78u', 'C78d', 'C78s', 'C78e', 'C78mu', 'C78tau',
                                     'C711', 'C712', 'C713', 'C714',
-                                    'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau', 
-                                    'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
-                                    'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau', 
-                                    'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
                                     'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
                                     'C725']
 
         if self.DM_type == "C":
             self.wc_name_list = ['C61u', 'C61d', 'C61s', 'C61c', 'C61e', 'C61mu', 'C61tau', 
                                  'C62u', 'C62d', 'C62s', 'C62c', 'C62e', 'C62mu', 'C62tau',
                                  'C65', 'C66',
@@ -1434,15 +1379,15 @@
                                  'C610']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = [0,1] + [i for i in range(9,16)] + [i for i in range(23,30)]\
                            + [31] + [33] + [i for i in range(41,48)]\
-                           + [i for i in range(55,76)] + [77] + [79] + [i for i in range(80,136)]
+                           + [i for i in range(55,76)] + [77] + [79] + [i for i in range(80,108)]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
             # The list of indices to be deleted from the ADT because of less operators (dim.6 part)
             del_ind_list_adt_quark = np.r_[np.s_[0:4]]
 
             # The 3-flavor list for matching only
             self.wc_name_list_3f = ['C61u', 'C61d', 'C61s', 'C61e', 'C61mu', 'C61tau', 
@@ -1463,15 +1408,15 @@
                                  'C610']
 
             self.wc8_name_list = []
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = [i for i in range(0,30)] + [31] + [33] + [i for i in range(41,48)]\
                            + [i for i in range(55,76)]\
-                           + [77] + [79] + [i for i in range(80,136)]
+                           + [77] + [79] + [i for i in range(80,108)]
 
             # The 3-flavor list for matching only
             self.wc_name_list_3f = ['C65', 'C66',
                                     'C63u', 'C63d', 'C63s', 'C63e', 'C63mu', 'C63tau', 
                                     'C64u', 'C64d', 'C64s', 'C64e', 'C64mu', 'C64tau',
                                     'C67', 'C68',
                                     'C69u', 'C69d', 'C69s', 'C69e', 'C69mu', 'C69tau', 
@@ -2146,15 +2091,15 @@
 
 class WC_5flavor(object):
     def __init__(self, coeff_dict, DM_type, input_dict=None):
 #    def __init__(self, coeff_dict, DM_type):
         """ Class for Wilson coefficients in 5 flavor QCD x QED plus DM.
 
         The argument should be a dictionary for the initial conditions of the 
-        2 + 32 + 4 + 48 + 4 + 64 + 8 + 1 + 12 = 175 
+        2 + 32 + 4 + 48 + 4 + 32 + 8 + 1 + 12 = 143 
         dimension-five to dimension-eight five-flavor-QCD Wilson coefficients (for Dirac DM) of the form
         {'C51' : value, 'C52' : value, ...}. For other DM types there are less coefficients.
         A subset of twist-two operators is currently only included for Dirac DM.
         An arbitrary number of them can be given; the default values are zero. 
         The possible name are (with an hopefully obvious notation):
 
         The second argument is the DM type; it can take the following values: 
@@ -2175,35 +2120,27 @@
                              'C79u', 'C79d', 'C79s', 'C79c', 'C79b', 'C79e', 'C79mu', 'C79tau', 
                              'C710u', 'C710d', 'C710s', 'C710c', 'C710b', 'C710e', 'C710mu', 'C710tau',
                              'C711', 'C712', 'C713', 'C714',
                              'C715u', 'C715d', 'C715s', 'C715c', 'C715b', 'C715e', 'C715mu', 'C715tau', 
                              'C716u', 'C716d', 'C716s', 'C716c', 'C716b', 'C716e', 'C716mu', 'C716tau',
                              'C717u', 'C717d', 'C717s', 'C717c', 'C717b', 'C717e', 'C717mu', 'C717tau', 
                              'C718u', 'C718d', 'C718s', 'C718c', 'C718b', 'C718e', 'C718mu', 'C718tau',
-                             'C719u', 'C719d', 'C719s', 'C719c', 'C719b', 'C719e', 'C719mu', 'C719tau', 
-                             'C720u', 'C720d', 'C720s', 'C720c', 'C720b', 'C720e', 'C720mu', 'C720tau', 
-                             'C721u', 'C721d', 'C721s', 'C721c', 'C721b', 'C721e', 'C721mu', 'C721tau', 
-                             'C722u', 'C722d', 'C722s', 'C722c', 'C722b', 'C722e', 'C722mu', 'C722tau',
                              'C723u', 'C723d', 'C723s', 'C723c', 'C723b', 'C723e', 'C723mu', 'C723tau',
                              'C725',
                              'C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s'
                              'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s'
 
         Majorana fermion:    'C62u', 'C62d', 'C62s', 'C62c', 'C62b', 'C62e', 'C62mu', 'C62tau',
                              'C64u', 'C64d', 'C64s', 'C64c', 'C64b', 'C64e', 'C64mu', 'C64tau',
                              'C71', 'C72', 'C73', 'C74',
                              'C75u', 'C75d', 'C75s', 'C75c', 'C75b', 'C75e', 'C75mu', 'C75tau', 
                              'C76u', 'C76d', 'C76s', 'C76c', 'C76b', 'C76e', 'C76mu', 'C76tau',
                              'C77u', 'C77d', 'C77s', 'C77c', 'C77b', 'C77e', 'C77mu', 'C77tau', 
                              'C78u', 'C78d', 'C78s', 'C78c', 'C78b', 'C78e', 'C78mu', 'C78tau',
                              'C711', 'C712', 'C713', 'C714',
-                             'C715u', 'C715d', 'C715s', 'C715c', 'C715b', 'C715e', 'C715mu', 'C715tau', 
-                             'C716u', 'C716d', 'C716s', 'C716c', 'C716b', 'C716e', 'C716mu', 'C716tau',
-                             'C717u', 'C717d', 'C717s', 'C717c', 'C717b', 'C717e', 'C717mu', 'C717tau', 
-                             'C718u', 'C718d', 'C718s', 'C718c', 'C718b', 'C718e', 'C718mu', 'C718tau',
                              'C723u', 'C723d', 'C723s', 'C723c', 'C723b', 'C723e', 'C723mu', 'C723tau', 
                              'C725',
 
         Complex Scalar:      'C61u', 'C61d', 'C61s', 'C61c', 'C61b', 'C61e', 'C61mu', 'C61tau', 
                              'C62u', 'C62d', 'C62s', 'C62c', 'C62b', 'C62e', 'C62mu', 'C62tau',
                              'C63u', 'C63d', 'C63s', 'C63c', 'C63b', 'C63e', 'C63mu', 'C63tau', 
                              'C64u', 'C64d', 'C64s', 'C64c', 'C64b', 'C64e', 'C64mu', 'C64tau',
@@ -2323,18 +2260,14 @@
                                  'C79u', 'C79d', 'C79s', 'C79c', 'C79b', 'C79e', 'C79mu', 'C79tau', 
                                  'C710u', 'C710d', 'C710s', 'C710c', 'C710b', 'C710e', 'C710mu', 'C710tau',
                                  'C711', 'C712', 'C713', 'C714',
                                  'C715u', 'C715d', 'C715s', 'C715c', 'C715b', 'C715e', 'C715mu', 'C715tau', 
                                  'C716u', 'C716d', 'C716s', 'C716c', 'C716b', 'C716e', 'C716mu', 'C716tau',
                                  'C717u', 'C717d', 'C717s', 'C717c', 'C717b', 'C717e', 'C717mu', 'C717tau', 
                                  'C718u', 'C718d', 'C718s', 'C718c', 'C718b', 'C718e', 'C718mu', 'C718tau',
-                                 'C719u', 'C719d', 'C719s', 'C719c', 'C719b', 'C719e', 'C719mu', 'C719tau', 
-                                 'C720u', 'C720d', 'C720s', 'C720c', 'C720b', 'C720e', 'C720mu', 'C720tau', 
-                                 'C721u', 'C721d', 'C721s', 'C721c', 'C721b', 'C721e', 'C721mu', 'C721tau', 
-                                 'C722u', 'C722d', 'C722s', 'C722c', 'C722b', 'C722e', 'C722mu', 'C722tau',
                                  'C723u', 'C723d', 'C723s', 'C723c', 'C723b', 'C723e', 'C723mu', 'C723tau', 
                                  'C725']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s',\
                                   'C83u', 'C83d', 'C83s', 'C84u', 'C84d', 'C84s']
 
             self.wc_name_list_4f = ['C51', 'C52', 'C61u', 'C61d', 'C61s', 'C61c', 'C61e', 'C61mu', 'C61tau', 
@@ -2349,60 +2282,48 @@
                                     'C79u', 'C79d', 'C79s', 'C79c', 'C79e', 'C79mu', 'C79tau', 
                                     'C710u', 'C710d', 'C710s', 'C710c', 'C710e', 'C710mu', 'C710tau',
                                     'C711', 'C712', 'C713', 'C714',
                                     'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau', 
                                     'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
                                     'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau', 
                                     'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
-                                    'C719u', 'C719d', 'C719s', 'C719c', 'C719e', 'C719mu', 'C719tau', 
-                                    'C720u', 'C720d', 'C720s', 'C720c', 'C720e', 'C720mu', 'C720tau', 
-                                    'C721u', 'C721d', 'C721s', 'C721c', 'C721e', 'C721mu', 'C721tau', 
-                                    'C722u', 'C722d', 'C722s', 'C722c', 'C722e', 'C722mu', 'C722tau',
                                     'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau', 
                                     'C725']
 
         if self.DM_type == "M":
             self.wc_name_list = ['C62u', 'C62d', 'C62s', 'C62c', 'C62b', 'C62e', 'C62mu', 'C62tau',
                                  'C64u', 'C64d', 'C64s', 'C64c', 'C64b', 'C64e', 'C64mu', 'C64tau',
                                  'C71', 'C72', 'C73', 'C74',
                                  'C75u', 'C75d', 'C75s', 'C75c', 'C75b', 'C75e', 'C75mu', 'C75tau', 
                                  'C76u', 'C76d', 'C76s', 'C76c', 'C76b', 'C76e', 'C76mu', 'C76tau',
                                  'C77u', 'C77d', 'C77s', 'C77c', 'C77b', 'C77e', 'C77mu', 'C77tau', 
                                  'C78u', 'C78d', 'C78s', 'C78c', 'C78b', 'C78e', 'C78mu', 'C78tau',
                                  'C711', 'C712', 'C713', 'C714',
-                                 'C715u', 'C715d', 'C715s', 'C715c', 'C715b', 'C715e', 'C715mu', 'C715tau', 
-                                 'C716u', 'C716d', 'C716s', 'C716c', 'C716b', 'C716e', 'C716mu', 'C716tau',
-                                 'C717u', 'C717d', 'C717s', 'C717c', 'C717b', 'C717e', 'C717mu', 'C717tau', 
-                                 'C718u', 'C718d', 'C718s', 'C718c', 'C718b', 'C718e', 'C718mu', 'C718tau',
                                  'C723u', 'C723d', 'C723s', 'C723c', 'C723b', 'C723e', 'C723mu', 'C723tau', 
                                  'C725']
 
             self.wc8_name_list = ['C82u', 'C82d', 'C82s', 'C84u', 'C84d', 'C84s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = [i for i in range(0,10)] + [i for i in range(18,26)]\
-                           + [i for i in range(70,86)] + [i for i in range(122,154)]
+                           + [i for i in range(70,86)] + [i for i in range(90,122)]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
             # The list of indices to be deleted from the ADT because of less operators (dim.6 part)
             del_ind_list_adt_quark = np.r_[np.s_[0:5]]
 
             # The 4-flavor list for matching only
             self.wc_name_list_4f = ['C62u', 'C62d', 'C62s', 'C62c', 'C62e', 'C62mu', 'C62tau',
                                     'C64u', 'C64d', 'C64s', 'C64c', 'C64e', 'C64mu', 'C64tau',
                                     'C71', 'C72', 'C73', 'C74',
                                     'C75u', 'C75d', 'C75s', 'C75c', 'C75e', 'C75mu', 'C75tau', 
                                     'C76u', 'C76d', 'C76s', 'C76c', 'C76e', 'C76mu', 'C76tau',
                                     'C77u', 'C77d', 'C77s', 'C77c', 'C77e', 'C77mu', 'C77tau', 
                                     'C78u', 'C78d', 'C78s', 'C78c', 'C78e', 'C78mu', 'C78tau',
                                     'C711', 'C712', 'C713', 'C714',
-                                    'C715u', 'C715d', 'C715s', 'C715c', 'C715e', 'C715mu', 'C715tau', 
-                                    'C716u', 'C716d', 'C716s', 'C716c', 'C716e', 'C716mu', 'C716tau',
-                                    'C717u', 'C717d', 'C717s', 'C717c', 'C717e', 'C717mu', 'C717tau', 
-                                    'C718u', 'C718d', 'C718s', 'C718c', 'C718e', 'C718mu', 'C718tau',
                                     'C723u', 'C723d', 'C723s', 'C723c', 'C723e', 'C723mu', 'C723tau', 
                                     'C725']
 
         if self.DM_type == "C":
             self.wc_name_list = ['C61u', 'C61d', 'C61s', 'C61c', 'C61b', 'C61e', 'C61mu', 'C61tau', 
                                  'C62u', 'C62d', 'C62s', 'C62c', 'C62b', 'C62e', 'C62mu', 'C62tau',
                                  'C65', 'C66',
@@ -2413,15 +2334,15 @@
                                  'C610']
 
             self.wc8_name_list = ['C81u', 'C81d', 'C81s', 'C82u', 'C82d', 'C82s']
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = [0,1] + [i for i in range(10,18)] + [i for i in range(26,34)]\
                            + [35] + [37] + [i for i in range(46,54)]\
-                           + [i for i in range(62,86)] + [87] + [89] + [i for i in range(90,154)]
+                           + [i for i in range(62,86)] + [87] + [89] + [i for i in range(90,122)]
             # The list of indices to be deleted from the dim.8 ADM because of less operators
             del_ind_list_dim_8 = np.r_[np.s_[0:3], np.s_[6:9]]
             # The list of indices to be deleted from the ADT because of less operators (dim.6 part)
             del_ind_list_adt_quark = np.r_[np.s_[0:5]]
 
             # The 4-flavor list for matching only
             self.wc_name_list_4f = ['C61u', 'C61d', 'C61s', 'C61c', 'C61e', 'C61mu', 'C61tau', 
@@ -2442,15 +2363,15 @@
                                  'C610']
 
             self.wc8_name_list = []
 
             # The list of indices to be deleted from the QCD/QED ADM because of less operators
             del_ind_list = [i for i in range(0,34)] + [35] + [37] + [i for i in range(46,54)]\
                            + [i for i in range(62,86)]\
-                           + [87] + [89] + [i for i in range(90,154)]
+                           + [87] + [89] + [i for i in range(90,122)]
 
             # The 4-flavor list for matching only
             self.wc_name_list_4f = ['C65', 'C66',
                                     'C63u', 'C63d', 'C63s', 'C63c', 'C63e', 'C63mu', 'C63tau',
                                     'C64u', 'C64d', 'C64s', 'C64c', 'C64e', 'C64mu', 'C64tau',
                                     'C67', 'C68',
                                     'C69u', 'C69d', 'C69s', 'C69c', 'C69e', 'C69mu', 'C69tau', 
@@ -3616,14 +3537,21 @@
                              'C71', 'C72', 'C73', 'C74',
                              'C75u', 'C75d', 'C75s', 'C65c', 'C65b', 'C75e', 'C75mu', 'C75tau', 
                              'C76u', 'C76d', 'C76s', 'C66c', 'C66b', 'C76e', 'C76mu', 'C76tau',
                              'C77u', 'C77d', 'C77s', 'C67c', 'C67b', 'C77e', 'C77mu', 'C77tau', 
                              'C78u', 'C78d', 'C78s', 'C68c', 'C68b', 'C78e', 'C78mu', 'C78tau',
                              'C79u', 'C79d', 'C79s', 'C69c', 'C69b', 'C79e', 'C79mu', 'C79tau', 
                              'C710u', 'C710d', 'C710s', 'C610c', 'C610b', 'C710e', 'C710mu', 'C710tau'
+                             'C711', 'C712', 'C713', 'C714',
+                             'C715u', 'C715d', 'C715s', 'C715e', 'C715mu', 'C715tau',
+                             'C716u', 'C716d', 'C716s', 'C716e', 'C716mu', 'C716tau',
+                             'C717u', 'C717d', 'C717s', 'C717e', 'C717mu', 'C717tau',
+                             'C718u', 'C718d', 'C718s', 'C718e', 'C718mu', 'C718tau',
+                             'C723u', 'C723d', 'C723s', 'C723e', 'C723mu', 'C723tau',
+                             'C725'
         """
         if RUN_EW is None:
             RUN_EW = True
         self.RUN_EW = RUN_EW
 
         if DM_mass_threshold is None:
             DM_mass_threshold = 40 # GeV
@@ -4259,50 +4187,14 @@
         coeff_dict_5f['C718s'] = 0
         coeff_dict_5f['C718c'] = 0
         coeff_dict_5f['C718b'] = 0
         coeff_dict_5f['C718e'] = 0
         coeff_dict_5f['C718mu'] = 0
         coeff_dict_5f['C718tau'] = 0
 
-        coeff_dict_5f['C719u'] = 0
-        coeff_dict_5f['C719d'] = 0
-        coeff_dict_5f['C719s'] = 0
-        coeff_dict_5f['C719c'] = 0
-        coeff_dict_5f['C719b'] = 0
-        coeff_dict_5f['C719e'] = 0
-        coeff_dict_5f['C719mu'] = 0
-        coeff_dict_5f['C719tau'] = 0
-
-        coeff_dict_5f['C720u'] = 0
-        coeff_dict_5f['C720d'] = 0
-        coeff_dict_5f['C720s'] = 0
-        coeff_dict_5f['C720c'] = 0
-        coeff_dict_5f['C720b'] = 0
-        coeff_dict_5f['C720e'] = 0
-        coeff_dict_5f['C720mu'] = 0
-        coeff_dict_5f['C720tau'] = 0
-
-        coeff_dict_5f['C721u'] = 0
-        coeff_dict_5f['C721d'] = 0
-        coeff_dict_5f['C721s'] = 0
-        coeff_dict_5f['C721c'] = 0
-        coeff_dict_5f['C721b'] = 0
-        coeff_dict_5f['C721e'] = 0
-        coeff_dict_5f['C721mu'] = 0
-        coeff_dict_5f['C721tau'] = 0
-
-        coeff_dict_5f['C722u'] = 0
-        coeff_dict_5f['C722d'] = 0
-        coeff_dict_5f['C722s'] = 0
-        coeff_dict_5f['C722c'] = 0
-        coeff_dict_5f['C722b'] = 0
-        coeff_dict_5f['C722e'] = 0
-        coeff_dict_5f['C722mu'] = 0
-        coeff_dict_5f['C722tau'] = 0
-
         coeff_dict_5f['C725'] = 0
 
         return coeff_dict_5f
 
 
     def _my_cNR(self, DM_mass, mu_Lambda, RGE=None, NLO=None, DM_mass_threshold=None, RUN_EW=None, DIM4=None):
         """ Calculate the NR coefficients from four-flavor theory
```

### Comparing `directdm-2.2.1/directdm.egg-info/PKG-INFO` & `directdm-2.2.2/directdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: directdm
-Version: 2.2.1
+Version: 2.2.2
 Summary: A python package for dark matter direct detection
 Home-page: https://directdm.github.io
 Author: Fady Bishara, Joachim Brod, Benjamin Grinstein, Jure Zupan
 Author-email: joachim.brod@uc.edu
 License: MIT
 Description:  This package contains classes for Wilson coefficients
                                    for dark matter -- standard model interactions,
```

### Comparing `directdm-2.2.1/directdm.egg-info/SOURCES.txt` & `directdm-2.2.2/directdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `directdm-2.2.1/setup.py` & `directdm-2.2.2/setup.py`

 * *Files identical despite different names*

