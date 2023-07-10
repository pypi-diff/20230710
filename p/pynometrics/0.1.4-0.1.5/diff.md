# Comparing `tmp/pynometrics-0.1.4.tar.gz` & `tmp/pynometrics-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynometrics-0.1.4.tar", last modified: Fri Apr 21 09:37:20 2023, max compression
+gzip compressed data, was "pynometrics-0.1.5.tar", last modified: Mon Jul 10 08:40:47 2023, max compression
```

## Comparing `pynometrics-0.1.4.tar` & `pynometrics-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 09:37:20.737639 pynometrics-0.1.4/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-02 14:08:08.000000 pynometrics-0.1.4/LICENSE.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-02 14:08:08.000000 pynometrics-0.1.4/MANIFEST.in
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 09:37:20.737413 pynometrics-0.1.4/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-02 14:08:08.000000 pynometrics-0.1.4/README.md
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 09:37:20.734875 pynometrics-0.1.4/examples/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.4/examples/example_01.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.4/examples/example_02.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 09:37:20.737710 pynometrics-0.1.4/setup.cfg
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-04-21 09:36:04.000000 pynometrics-0.1.4/setup.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 09:37:20.735170 pynometrics-0.1.4/src/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.4/src/.DS_Store
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 09:37:20.735715 pynometrics-0.1.4/src/pynometrics/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 pynometrics-0.1.4/src/pynometrics/__init__.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16222 2023-04-21 09:35:37.000000 pynometrics-0.1.4/src/pynometrics/pynometrics.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 09:37:20.737144 pynometrics-0.1.4/src/pynometrics.egg-info/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 09:37:20.000000 pynometrics-0.1.4/src/pynometrics.egg-info/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-04-21 09:37:20.000000 pynometrics-0.1.4/src/pynometrics.egg-info/SOURCES.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 09:37:20.000000 pynometrics-0.1.4/src/pynometrics.egg-info/dependency_links.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.4/src/pynometrics.egg-info/not-zip-safe
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-04-21 09:37:20.000000 pynometrics-0.1.4/src/pynometrics.egg-info/requires.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-04-21 09:37:20.000000 pynometrics-0.1.4/src/pynometrics.egg-info/top_level.txt
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-07-10 08:40:47.158342 pynometrics-0.1.5/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-02 14:08:08.000000 pynometrics-0.1.5/LICENSE.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-02 14:08:08.000000 pynometrics-0.1.5/MANIFEST.in
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-07-10 08:40:47.158135 pynometrics-0.1.5/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-02 14:08:08.000000 pynometrics-0.1.5/README.md
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-07-10 08:40:47.155585 pynometrics-0.1.5/examples/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.5/examples/example_01.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.5/examples/example_02.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-07-10 08:40:47.158429 pynometrics-0.1.5/setup.cfg
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-07-10 08:38:40.000000 pynometrics-0.1.5/setup.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-07-10 08:40:47.155883 pynometrics-0.1.5/src/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.5/src/.DS_Store
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-07-10 08:40:47.156447 pynometrics-0.1.5/src/pynometrics/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 pynometrics-0.1.5/src/pynometrics/__init__.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16218 2023-07-10 08:38:42.000000 pynometrics-0.1.5/src/pynometrics/pynometrics.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-07-10 08:40:47.157813 pynometrics-0.1.5/src/pynometrics.egg-info/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-07-10 08:40:47.000000 pynometrics-0.1.5/src/pynometrics.egg-info/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-07-10 08:40:47.000000 pynometrics-0.1.5/src/pynometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-07-10 08:40:47.000000 pynometrics-0.1.5/src/pynometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.5/src/pynometrics.egg-info/not-zip-safe
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-07-10 08:40:47.000000 pynometrics-0.1.5/src/pynometrics.egg-info/requires.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-07-10 08:40:47.000000 pynometrics-0.1.5/src/pynometrics.egg-info/top_level.txt
```

### Comparing `pynometrics-0.1.4/LICENSE.txt` & `pynometrics-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.4/PKG-INFO` & `pynometrics-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.4
+Version: 0.1.5
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pynometrics-0.1.4/README.md` & `pynometrics-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.4/examples/example_01.py` & `pynometrics-0.1.5/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.4/examples/example_02.py` & `pynometrics-0.1.5/examples/example_02.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.4/setup.py` & `pynometrics-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("/Users/geofrey.wanyama/Desktop/wg/projects/package_dev/pyeconometrics/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     # name that will be imported, can be different from code file name
     name='pynometrics',
 
-    version='0.1.4',
+    version='0.1.5',
 
     description='Includes functions for performing econometrics tasks',
 
     # code file name without file extension
     packages=['pynometrics'],
 
     # directory in which code file is stored
```

### Comparing `pynometrics-0.1.4/src/.DS_Store` & `pynometrics-0.1.5/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.4/src/pynometrics/pynometrics.py` & `pynometrics-0.1.5/src/pynometrics/pynometrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,20 +174,18 @@
             3 = Scale-Location
             4 = Cook's Distance
             5 = Residuals vs Leverage
             6 = Cook's dist vs Leverage
             7 = 95% confidence intervals
     """
  
-    def __init__(self, mdl, n):
+    def __init__(self, mdl):
         
         self.mdl = mdl
         
-        self.n = n
-        
         self.fitted_values = pd.Series(self.mdl.fittedvalues)
         
         self.res_df = (
             
             pd.DataFrame(
                 self.fitted_values, index = self.mdl.fittedvalues.index, columns = ['fitted_values'])
            
@@ -207,15 +205,15 @@
                 errors = lambda X: X['coef'] - self.mdl.conf_int().iloc[:,0].values,
                 pvalues = self.mdl.pvalues.values,
                 Significant = lambda X: X['pvalues'] < 0.05)
             .query("var != 'Intercept'")
         )
 
         
-    def plot(self, figsize=(12,5)):
+    def plot(self, n, figsize=(12,5)):
         """
         Function to generate plot for chosen diagnostic check for linear regression
         
         Args:
             None
         
         Returns
@@ -248,15 +246,15 @@
         from matplotlib.figure import Figure
         
         fig = Figure()
         ax = fig.subplots()
         
 #         fig, ax = plt.subplots()
         
-        if self.n == 1:
+        if n == 1:
             
             # rows with top residuals 
             top3 = abs(self.res_df['residuals']).sort_values(ascending = False)[:3]
             
             X, Y = self.res_df['fitted_values'], self.res_df['residuals']
             
             smoothed = lowess(self.res_df['residuals'],self.res_df['fitted_values'])
@@ -272,39 +270,41 @@
             ax.set_title('Residuals vs. Fitted')
             
             ax.plot([min(X),max(X)], [0,0], color = 'k', linestyle = ':', alpha = .8)
             
             for i in top3.index:
                 ax.annotate(i, xy=(X[i], Y[i]), fontsize = 10, color = 'k', fontweight = 'bold')
         
-        if self.n == 2:
+        if n == 2:
 
             Y = self.res_df['residuals']
            
             # qq plot from statsmodels.api = sm
             QQplot = sm.qqplot(Y, fit = True, line = "q",ax = ax)
 
             QQplot.axes[0].set_title('Normal Q-Q')
 
             QQplot.axes[0].set_xlabel('Theoretical Quantiles')
 
             QQplot.axes[0].set_ylabel('Standardized Residuals')
 
-            axes = plt.gca()
+            plt.show()
+
+            # axes = plt.gca()
 
-            x_values, y_values = axes.lines[0].get_xdata(), axes.lines[0].get_ydata()
+            # x_values, y_values = axes.lines[0].get_xdata(), axes.lines[0].get_ydata()
 
-            for i, j in enumerate(np.arange(3)-3):
+            # for i, j in enumerate(np.arange(3)-3):
                 
-                indx = np.argsort(np.abs(Y)).values[j]
+            #     indx = np.argsort(np.abs(Y)).values[j]
                 
-                QQplot.axes[0].annotate(
-                    indx, xy = (x_values[j], y_values[j]), fontsize = 10, color = 'k', fontweight = 'bold')
+            #     QQplot.axes[0].annotate(
+            #         indx, xy = (x_values[j], y_values[j]), fontsize = 10, color = 'k', fontweight = 'bold')
                                     
-        if self.n == 3:
+        if n == 3:
             
             X, Y = self.res_df['fitted_values'], self.res_df['sqrt_student_residuals']
 
             smoothed = lowess(Y,X)
 
             # rows with top residuals 
             top3 = abs(self.res_df['residuals']).sort_values(ascending = False)[:3]
@@ -320,15 +320,15 @@
             ax.set_title('Scale-Location', fontsize = 14, fontweight = 'bold')
             
             ax.set_ylim(0, max(Y)+0.1)
             
             for i in top3.index:
                 ax.annotate(i, xy = (X[i],Y[i]), fontsize = 10, color = 'k', fontweight = 'bold')
         
-        if self.n == 4:  
+        if n == 4:  
             
             df_res = self.res_df.reset_index().drop('index', axis=1)
             
             X, Y = df_res.index, df_res['cooks_distance']
             
             # rows with the highest cook distance
             top3 = abs(df_res['cooks_distance']).sort_values(ascending = False)[:3]
@@ -342,24 +342,26 @@
                 
                 lines.append(pair)
             
             linecoll = matcoll.LineCollection(lines)
             
             ax.add_collection(linecoll)
             
-            plt.scatter(X,Y, alpha = 0.85, linewidths = 3, color = 'r', s = 6)
+            ax.scatter(X,Y, alpha = 0.85, linewidths = 3, color = 'r', s = 6)
             
             ax.set_ylabel("Cook's distance", fontsize = 12, fontweight = 'bold')
             
             ax.set_xlabel('Observation number', fontsize = 12, fontweight = 'bold')
 
             for i in top3.index:
                 ax.annotate(i, xy = (X[i],Y[i]), fontsize = 10, color = 'k', fontweight = 'bold')
 
-        if self.n == 5: 
+            plt.show()
+
+        if n == 5: 
 
             student_residuals = pd.Series(self.mdl.get_influence().resid_studentized_internal)
             
             student_residuals.index = self.mdl.resid.index
             
             df = pd.DataFrame(student_residuals)
             
@@ -423,15 +425,15 @@
             ax.annotate('1.0', xy = (xpos, negcooks1y[-1]), color = 'r')
             
             ax.annotate('0.5', xy = (xpos, negcooks05y[-1]), color = 'r')
             
             ax.legend()
 
 
-        if self.n == 6: 
+        if n == 6: 
 
             X, Y = self.res_df['leverage'], self.res_df['cooks_distance']
 
             smoothed = lowess(Y,X)
             
             # rows with highest cooks distance
             top3 = abs(Y).sort_values(ascending = False)[:3]
@@ -446,15 +448,15 @@
             
             ax.set_title("Cook's dist vs. Leverage")
            
             for i in top3.index:
                 ax.annotate(i, xy = (X.loc[i],Y.loc[i]), fontsize = 10, color = 'k', fontweight = 'bold')
 
         
-        if self.n == 7: 
+        if n == 7: 
             
             self.df_params.plot(x = 'var', y = 'coef', kind = 'barh', ax = ax, color = 'none', 
                            ecolor = self.df_params.Significant.map({True: '#20B2AA', False: '#F08080'}),
                            capsize = 0, xerr = 'errors', legend = False)
 
             ax.scatter(y = np.arange(self.df_params.shape[0]), marker = 'o', s = 160, x = self.df_params['coef'], 
                        color = self.df_params.Significant.map({True: '#20B2AA', False: '#F08080'}))
```

### Comparing `pynometrics-0.1.4/src/pynometrics.egg-info/PKG-INFO` & `pynometrics-0.1.5/src/pynometrics.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.4
+Version: 0.1.5
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

