# Comparing `tmp/SpecLab-4.1.1.tar.gz` & `tmp/SpecLab-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpecLab-4.1.1.tar", last modified: Thu Jun 29 00:35:05 2023, max compression
+gzip compressed data, was "dist/SpecLab-4.1.2.tar", last modified: Mon Jul 10 16:27:44 2023, max compression
```

## Comparing `SpecLab-4.1.1.tar` & `SpecLab-4.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.1.1/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48692 2023-06-29 00:34:32.000000 SpecLab-4.1.1/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.1.1/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.1.1/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-06-28 23:09:48.000000 SpecLab-4.1.1/SpecLab/gen/SpecLabFunctions.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.1.1/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.1.1/SpecLab/gen/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.1.1/SpecLab/gen/myfunc.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.1.1/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/aux/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/aux/param_files/
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.default.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.1.1/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.1.1/SpecLab/aux/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   619019 2023-06-29 00:31:34.000000 SpecLab-4.1.1/SpecLab/aux/pyqtgraph10_speclab.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-29 00:35:05.000000 SpecLab-4.1.1/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.1.1/SpecLab/doc/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      592 2023-06-29 00:34:03.000000 SpecLab-4.1.1/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4715 2023-06-29 00:32:54.000000 SpecLab-4.1.1/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1073 2023-06-29 00:33:05.000000 SpecLab-4.1.1/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.1.1/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6496 2023-06-29 00:35:05.000000 SpecLab-4.1.1/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1389 2023-06-29 00:34:54.000000 SpecLab-4.1.1/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.1.2/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48797 2023-07-10 16:21:07.000000 SpecLab-4.1.2/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.1.2/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.1.2/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-06-28 23:09:48.000000 SpecLab-4.1.2/SpecLab/gen/SpecLabFunctions.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.1.2/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.1.2/SpecLab/gen/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.1.2/SpecLab/gen/myfunc.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.1.2/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/aux/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/aux/param_files/
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.1.2/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.1.2/SpecLab/aux/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   619019 2023-06-29 00:31:34.000000 SpecLab-4.1.2/SpecLab/aux/pyqtgraph10_speclab.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-10 16:27:44.000000 SpecLab-4.1.2/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.1.2/SpecLab/doc/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      689 2023-07-10 16:23:21.000000 SpecLab-4.1.2/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4827 2023-07-10 16:25:18.000000 SpecLab-4.1.2/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1073 2023-06-29 00:33:05.000000 SpecLab-4.1.2/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.1.2/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     6625 2023-07-10 16:27:44.000000 SpecLab-4.1.2/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1373 2023-07-10 16:22:23.000000 SpecLab-4.1.2/setup.py
```

### Comparing `SpecLab-4.1.1/SpecLab/imXam/imXam.py` & `SpecLab-4.1.2/SpecLab/imXam/imXam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 
 import numpy as np
-from pyqtgraph10_speclab.Qt import QtCore, QtGui
+from pyqtgraph10_speclab.Qt import QtCore, QtGui, QtWidgets
 import pyqtgraph10_speclab as pg
 from pyqtgraph10_speclab import PlotWidget, plot
 from pyqtgraph10_speclab.Point import Point
 from astropy.io import fits
 import astropy.io.ascii as ascii
 from scipy.interpolate import RegularGridInterpolator
 import matplotlib
 import matplotlib.pyplot as plt
-from PyQt5 import QtWidgets
-from PyQt5.QtCore import pyqtRemoveInputHook
-from PyQt5.QtCore import QCoreApplication
+#from PyQt5 import QtWidgets
+#from PyQt5.QtCore import pyqtRemoveInputHook
+#from PyQt5.QtCore import QCoreApplication
 from photutils.aperture import CircularAperture, CircularAnnulus
 from photutils.aperture import aperture_photometry
 from matplotlib.backend_bases import key_press_handler
 from photutils.centroids import centroid_2dg
 import sys
 import scipy, scipy.optimize
 import matplotlib.pyplot as plt
@@ -83,15 +83,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: adam f kowalski, v4.1.1: June 28, 2023')
+print('imXam: adam f kowalski, v4.1.2: July 10, 2023')
 print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -157,15 +157,15 @@
 boxy1=[]
 box_mean =[]
 box_med = []
 box_max = []
 box_min = []
 box_std = []
 
-pyqtRemoveInputHook()
+QtCore.pyqtRemoveInputHook()
 
 args = parser.parse_args()
 
 ifile = args.filename
 
 param_file = args.param
 
@@ -506,15 +506,15 @@
         Vmax = v1
         Vmin = v0
         
     else:
         Vmax = zmax
         Vmin = zmin
     
-    QCoreApplication.processEvents()
+    QtCore.QCoreApplication.processEvents()
 
 
     if val == '1':  # lower left
         boxx0.append(user_x)
         boxy0.append(user_y)
 
     if val == '2': # upper right
@@ -566,15 +566,15 @@
         fig.update_xaxes(title='Wavelength pixel')
         fig.show()
         print('Trace parameters:  xstart = ', user_x, '  tsum = ',TSum, '   ntrace = ',NTrace, '   t_func =', trace_func, ' otrace = ', OTrace, '  N_iter = ', trace_iter)
         
         if val == 's':
             np.save('tmp.x1d', ap_extract)
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
         
     if val == 'g':
         fit_succ = 1
         if dispaxis == 1:
             b_data = (np.transpose(data[user_x , user_y-urout:user_y-urin]) + np.transpose(data[user_x , user_y+urin:user_y+urout]) ) / 2.0
             t_data = np.transpose(data[user_x , user_y-int(apspec_radius_l*2):user_y+int(apspec_radius_u*2)])
             b_data = np.nanmedian(b_data)
@@ -609,47 +609,47 @@
             fig = go.Figure(data=[go.Scatter(x=pix_1d-mu1, y=t_data, marker_color="#000000", name="Data",line_shape="hvh"), go.Scatter(x=pix_1d-mu1, y=fitprof, marker_color=BR_red_col_HEX, name="Gaussian fit", mode="markers+lines")])
             print('Gaussian FWHM = {0:8.3f} pixels'.format(FWHM))
         fig.update_layout(font_family='Times New Roman',font_size=15,title=ifile+"<br>Gaussian FWHM (pix) = {0:8.3f}".format(FWHM))
         fig.update_xaxes(title='Spatial pixel - Centroid',nticks=10)
         fig.update_yaxes(title='Counts per pixel')
         fig.show()
                 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
            
     if val == 'c':
         yarr_1d = np.arange(0,len(data[user_x,:]),1)
         fig = go.Figure(data=[go.Scatter(x=yarr_1d, y=data[user_x, :], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='y pixel')
         fig.show()
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
         
     if val == 'l':
         
         f, ax = plt.subplots()
         xarr_1d = np.arange(0,len(data[:,user_y]),1) # starts at 0
         fig = go.Figure(data=[go.Scatter(x=xarr_1d, y=data[:,user_y], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='x pixel')
         fig.show()
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'm':
         t_data = np.transpose(data[user_x-mrad:user_x+mrad, user_y-mrad:user_y+mrad])
         print('     ')
         print('Stats in box of side ',  mrad*2, 'pixels')
         print('Max = {:8.2f}'.format(np.max(t_data)))
         print('Mean = {:8.2f}'.format(np.mean(t_data)))
         print('Median = {:8.2f}'.format(np.median(t_data)))
         print('Std Dev = {:8.2f}'.format(np.std(t_data)))
         print('     ')
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
             
             
     if val == 'r' or val == 'a' or val == 'z':
         t_data = np.transpose(data[user_x-aptrace_window:user_x+aptrace_window, user_y-aptrace_window:user_y+aptrace_window]) # just for centroidin
         t_data_all = np.transpose(data)
         dy = float( urout + 5 - aptrace_window)
@@ -689,15 +689,15 @@
                     scaleratio = 1,
                 )
                 fig.update_layout(font_family='Times New Roman',font_size=15)
                 fig.update_yaxes(title='y pixel')
                 fig.update_xaxes(title='x pixel')
                 fig.show()
     
-                QCoreApplication.processEvents()
+                QtCore.QCoreApplication.processEvents()
 
 
 
             
             if val == 'r' or val == 'a':
                 aper = CircularAperture([xcen0, ycen0], r=float(apr))
                 annulus_aperture = CircularAnnulus([xcen0, ycen0], r_in =  urin, r_out = urout)
@@ -776,15 +776,15 @@
                 
             
           #      https://pyqtgraph.readthedocs.io/en/latest/graphicsItems/axisitem.html
         #        http://www.silx.org/doc/silx/0.2.0/modules/gui/plot/plotwidget.html
     
         #https://www.learnpyqt.com/courses/graphics-plotting/plotting-pyqtgraph/
 
-                    QCoreApplication.processEvents()
+                    QtCore.QCoreApplication.processEvents()
         except:
             print('Failed to get centroid with centroid_2dg')
 
     if val == 'o':
         t_data = np.transpose(data[user_x-imc:user_x+imc, user_y-imc:user_y+imc])
         data_ap = data[user_x-imc:user_x+imc, user_y-imc:user_y+imc]
         aper = CircularAperture([user_x, user_y], r=float(apr))
@@ -815,15 +815,15 @@
                     scaleratio = 1,
                 )
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='y pixel')
         fig.update_xaxes(title='x pixel')
         fig.show()
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 't':  # trace a spectrum and show trace with plotly 
         if dispaxis == 1:
             t_data = np.transpose(data)
             xtrace, ytrace, bsubtrace, xvalsfitted, yvalsfitted = SpecLab.trace_1d(t_data, yguess=user_y, xstrt=user_x, search_win = aptrace_window, tsum=TSum, ntrace=NTrace,otrace=OTrace, bmin=urin, bmax=urout, N_iter=trace_iter, t_func = trace_func)
             print('Trace parameters:  xstart = ', user_x, '  tsum = ',TSum, '   ntrace = ',NTrace, '   t_func =', trace_func, ' otrace = ', OTrace, '  N_iter = ', trace_iter)
             winup = int(np.max(ytrace))
@@ -889,15 +889,15 @@
 
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='y pixel')
         fig.update_xaxes(title='x pixel')
         fig.show()
     
 
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'T':  # Find and show pixels above a threshold.
         thressh =  input('Enter threshold value: ')
         thresh = float(thressh)
         t_data = np.transpose(data)
 
         sat_pixels = (t_data >= thresh)
@@ -926,15 +926,15 @@
 
         if inds2d.shape[0] == 0:
             print('  ')
             print('No pixels found above ', thresh)
             print('  ')
         else:
             print('Number of pixels found above threshold = ', thresh, ' is ',inds2d.shape[0])
-        QCoreApplication.processEvents()
+        QtCore.QCoreApplication.processEvents()
 
     if val == 'H':
         try:
             hdr = fits.getheader(ifile)
             hdr.totextfile('lastheader.txt',overwrite=True)
             hdr.totextfile(ifile+'.header.txt',overwrite=True)
             print('Printed header to lastheader.txt and '+ifile+'.header.txt')
@@ -943,15 +943,15 @@
                 print('DATE-OBS = ',hdr['DATE-OBS'])
                 print('EXPTIME = ',hdr['EXPTIME'])
             except:
                 print('Could not find DATE-OBS and EXPTIME in header.')
         except:
             print('Could not print header.')
     if val == 'q':
-        QCoreApplication.exit()
+        QtCore.QCoreApplication.exit()
     if val == 'h' or val == '?' or  val == 'help' or val == 'Help':
         print('           ')
         print('************************************************************')
         print('q:  quit imXam.')
         print('r:  plot radial profile, print fwhm, and print aperture photometry w/ sky annulus subtraction centered at cursor location; plot x-range can be set with RMax.')
         print('x:  trace and extract spectrum with sky subtraction, at cursor location (can change params in imXam_param.dat).')
         print('g:  fits a Gaussian to the spatial profile (uniform weighting in fit) of a spectrum at cursor location. An estimate of a constant background level (e.g., bias in a raw frame) is subtracted before the fit')
```

### Comparing `SpecLab-4.1.1/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.1.2/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.1.2/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/gen/globals.py` & `SpecLab-4.1.2/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/gen/myfunc.py` & `SpecLab-4.1.2/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.1.2/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/aux/pyqtgraph10_speclab.tar.gz` & `SpecLab-4.1.2/SpecLab/aux/pyqtgraph10_speclab.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/doc/CHANGELOG.txt` & `SpecLab-4.1.2/SpecLab/doc/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 
 4.1.0
 
 - updates for python 3.6 and 3.7
 
 4.1.1 
 
-- updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.2
+- updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.
+
+4.1.2
+
+- removed dependency on separate installation of PyQt5 to address issues with M1/M2 chips
```

### Comparing `SpecLab-4.1.1/SpecLab/doc/README.md` & `SpecLab-4.1.2/SpecLab/doc/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# imXam:  v4.1.1 (Latest)
+# imXam:  v4.1.2 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
-with the same GUI design (pyqtgraph10 + Plotly) in the future as these get finished.
+with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQTGraph](https://www.pyqtgraph.org/), but a customized version of v10 will be installed automatically with the commands below
 
 author: Adam F Kowalski (June 28, 2023)
 
 ## Installing imXam 
 
@@ -25,15 +25,15 @@
 To set up a fresh conda environment:
 
 From a terminal window:
 
 `conda create --name your_env_name python=3.8`
 
 (Note, imXam will work with Python 3.6, 3.7, and 3.8.  Note that Python 3.7 was unfortunately deprecated on 6/27/23!)
-
+imXam will be fully updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time Python 3.8 is deprecated.
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
 
 ### Step 3
```

### Comparing `SpecLab-4.1.1/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.1.2/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/SpecLab/doc/LICENSE.txt` & `SpecLab-4.1.2/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.1.1/PKG-INFO` & `SpecLab-4.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.0
 Name: SpecLab
-Version: 4.1.1
+Version: 4.1.2
 Summary: IRAF imexam+DS9 replacement for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 License: UNKNOWN
-Description: imXam: v4.1.1 (Latest)
+Description: imXam: v4.1.2 (Latest)
         ======================
         
         **imXam** is the first interactive program finished for the **SpecLab**
         python-only data reduction package. More (identify, standard, sensfunc,
-        apall) will be added with the same GUI design (pyqtgraph10 + Plotly) in
+        apall) will be added with the same GUI design (PyQtGraph + Plotly) in
         the future as these get finished.
         
         This uses `PyQTGraph <https://www.pyqtgraph.org/>`__, but a customized
         version of v10 will be installed automatically with the commands below
         
         author: Adam F Kowalski (June 28, 2023)
         
@@ -40,15 +40,17 @@
         To set up a fresh conda environment:
         
         From a terminal window:
         
         ``conda create --name your_env_name python=3.8``
         
         (Note, imXam will work with Python 3.6, 3.7, and 3.8. Note that Python
-        3.7 was unfortunately deprecated on 6/27/23!)
+        3.7 was unfortunately deprecated on 6/27/23!) imXam will be fully
+        updated to work with Python 3.9+ and PyQtGraph(v.latest) by the time
+        Python 3.8 is deprecated.
         
         ``conda activate your_env_name``
         
         ``pip install SpecLab``
         
         Step 3
         ~~~~~~
```

### Comparing `SpecLab-4.1.1/setup.py` & `SpecLab-4.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,26 @@
    import pypandoc
    long_desc = pypandoc.convert_file('SpecLab/doc/README.md', 'rst')
 except(IOError, ImportError):
    long_desc = open('SpecLab/doc/README.md').read()
 
 setup(
     name='SpecLab',
-    version='4.1.1',
+    version='4.1.2',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
     url='http://pypi.python.org/pypi/SpecLab/',
     description='IRAF imexam+DS9 replacement for Python',long_description_content_type='text/x-rst',
     long_description=long_desc,
-    install_requires=['numpy', 'plotly>=5.2.1', 'pandas','astropy>=4.0.2','scipy','matplotlib','PyQt5>=5.15.6', 'photutils',]
+    install_requires=['numpy', 'plotly>=5.2.1', 'pandas','astropy>=4.0.2','scipy','matplotlib', 'photutils',]
 )
 
 # python setup.py sdist
 # python -m twine upload --repository testpypi dist/*
 # pip install -i https://test.pypi.org/simple/ speclab-imXam==3.1.2
 # pip uninstall speclab-imXam==3.1.2
 #  I neeeded to put the #! crap at the top of any of the scripts=
```

