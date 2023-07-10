# Comparing `tmp/analysis-tools-0.1.2.tar.gz` & `tmp/analysis-tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-tools-0.1.2.tar", last modified: Mon Aug  8 17:53:05 2022, max compression
+gzip compressed data, was "analysis-tools-0.2.1.tar", last modified: Tue Nov  8 18:43:11 2022, max compression
```

## Comparing `analysis-tools-0.1.2.tar` & `analysis-tools-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1642 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1283 2022-08-08 17:25:35.000000 analysis-tools-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/analysis_tools/
--rw-r--r--   0 root         (0) root         (0)      413 2022-08-08 15:06:00.000000 analysis-tools-0.1.2/analysis_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/analysis_tools/common/
--rw-r--r--   0 root         (0) root         (0)      229 2022-02-21 15:29:54.000000 analysis-tools-0.1.2/analysis_tools/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      462 2022-08-08 13:53:44.000000 analysis-tools-0.1.2/analysis_tools/common/config.py
--rw-r--r--   0 root         (0) root         (0)     1798 2022-08-08 13:08:47.000000 analysis-tools-0.1.2/analysis_tools/common/env.py
--rw-r--r--   0 root         (0) root         (0)     4444 2022-08-08 16:19:19.000000 analysis-tools-0.1.2/analysis_tools/common/util.py
--rw-r--r--   0 root         (0) root         (0)    15446 2022-08-08 17:04:03.000000 analysis-tools-0.1.2/analysis_tools/eda.py
--rw-r--r--   0 root         (0) root         (0)    14817 2022-08-08 15:05:15.000000 analysis-tools-0.1.2/analysis_tools/metrics.py
--rw-r--r--   0 root         (0) root         (0)     2375 2022-08-08 15:09:18.000000 analysis-tools-0.1.2/analysis_tools/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2402 2022-08-08 14:59:33.000000 analysis-tools-0.1.2/analysis_tools/preprocessing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/analysis_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1642 2022-08-08 17:53:05.000000 analysis-tools-0.1.2/analysis_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      429 2022-08-08 17:53:05.000000 analysis-tools-0.1.2/analysis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-08 17:53:05.000000 analysis-tools-0.1.2/analysis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-08-08 17:53:05.000000 analysis-tools-0.1.2/analysis_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-08 17:53:05.809455 analysis-tools-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      614 2022-08-08 17:24:02.000000 analysis-tools-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1691 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1333 2022-11-08 18:39:40.000000 analysis-tools-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/analysis_tools/
+-rw-r--r--   0 root         (0) root         (0)      304 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/analysis_tools/common/
+-rw-r--r--   0 root         (0) root         (0)      242 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2022-11-08 16:46:26.000000 analysis-tools-0.2.1/analysis_tools/common/env.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/common/plot_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2022-11-07 12:58:57.000000 analysis-tools-0.2.1/analysis_tools/common/utils.py
+-rw-r--r--   0 root         (0) root         (0)    22130 2022-11-08 17:43:43.000000 analysis-tools-0.2.1/analysis_tools/eda.py
+-rw-r--r--   0 root         (0) root         (0)    14358 2022-11-08 18:22:03.000000 analysis-tools-0.2.1/analysis_tools/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4374 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      183 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/random.py
+-rw-r--r--   0 root         (0) root         (0)      766 2022-09-28 22:06:23.000000 analysis-tools-0.2.1/analysis_tools/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/analysis_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1691 2022-11-08 18:43:11.000000 analysis-tools-0.2.1/analysis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2022-11-08 18:43:11.000000 analysis-tools-0.2.1/analysis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-08 18:43:11.000000 analysis-tools-0.2.1/analysis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2022-11-08 18:43:11.000000 analysis-tools-0.2.1/analysis_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-11-08 18:43:11.000000 analysis-tools-0.2.1/analysis_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-08 18:43:11.340285 analysis-tools-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1025 2022-11-08 18:40:46.000000 analysis-tools-0.2.1/setup.py
```

### Comparing `analysis-tools-0.1.2/PKG-INFO` & `analysis-tools-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 Metadata-Version: 2.1
 Name: analysis-tools
-Version: 0.1.2
+Version: 0.2.1
 Summary: Analysis tools for machine learning projects
-Home-page: https://github.com/djy-git/analysis-tools
+Home-page: https://pypi.org/project/analysis-tools/
 Author: Dongjin Yoon
 Author-email: djyoon0223@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Analysis tools for Machine learning projects
 
 ## 1. Usage
 ```bash
-# Load repository manually
-$ git clone https://github.com/djy-git/analysis-tools.git 
-
-# Install with Pypi
 $ pip install analysis-tools
 ```
 
 ## 2. Tutorial
 [examples/titanic/eda.ipynb](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/eda.ipynb)를 참고
 
 ```python
-from analysis_tools.eda import *
+from analysis_tools import eda, metrics
 
 data   = pd.DataFrame(..)
 target = 'survived'
 
 num_features       = ['age', 'sibsp', 'parch', 'fare']
 cat_features       = data.columns.drop(num_features)
 data[num_features] = data[num_features].astype('float32')
 data[cat_features] = data[cat_features].astype('string')
 
-plot_missing_value(data)
-plot_features(data)
-plot_features_target(data, target)
-plot_corr(data.corr())
+eda.plot_missing_value(data)
+eda.plot_features(data)
+eda.plot_features_target(data, target)
+eda.plot_corr(data.corr())
+metrics.get_feature_importance(data, target)
 ```
 
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Missing%20value_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Features_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Features%20vs%20Target_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Correlation%20matrix_1.png?raw=true)
-
-
+![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Feature%20importance_1.png?raw=true)
```

### Comparing `analysis-tools-0.1.2/analysis_tools/common/env.py` & `analysis-tools-0.2.1/analysis_tools/common/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 """Environment module
 
 Commonly used packages and default settings are defined here.
 """
-
 # Author: Dongjin Yoon <djyoon0223@gmail.com>
 
 
 # Internal packages
 import sys
 import os
 from os.path import join, isdir, isfile, exists, basename, dirname, split, abspath
 import shutil
 from glob import glob
+from argparse import ArgumentParser
+from configparser import ConfigParser
+from importlib import import_module
 import datetime
 import joblib
 import json
 import re
-from itertools import product
+from itertools import product, combinations, permutations, starmap
+from functools import reduce
 from time import time, sleep
 from collections import defaultdict
 from copy import deepcopy as copy
 from tqdm import tqdm, trange
 import warnings
-from contextlib import ContextDecorator
+import contextlib
 from dataclasses import dataclass
 from IPython.display import display, Markdown
 import subprocess
+import inspect
+from abc import ABCMeta, abstractmethod
 
 
 # External packages
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_numeric_dtype
 from tabulate import tabulate
 import numba as nb
 from numba import njit, cuda
+import dask
 from dask import delayed, compute
-from dask.distributed import Client
+import dask.distributed
+import dask.dataframe as dd
 from dask.diagnostics import ProgressBar
 import missingno as msno
+import dateutil
+from switch import Switch
 
 
 # Plot packages
 import matplotlib.pyplot as plt
 from matplotlib.cbook import boxplot_stats
-from matplotlib.gridspec import GridSpec
+from matplotlib import gridspec
 import seaborn as sns
 
 
 # Plot options
+#   Use korean fonts
+"""
+$ sudo apt-get install fonts-nanum* fontconfig
+$ sudo fc-cache -fv
+$ sudo cp /usr/share/fonts/truetype/nanum/Nanum* /opt/conda/envs/caret/lib/python3.8/site-packages/matplotlib/mpl-data/fonts/ttf/
+$ rm -rf /root/.cache/matplotlib/*
+"""
 from pandas.plotting import register_matplotlib_converters
 register_matplotlib_converters()
-plt.rc('font', family='DejaVu Sans')
+plt.rc('font', family='NanumGothic')
+# plt.rc('font', family='DejaVu Sans')
 plt.rc('axes', unicode_minus=False)
 plt.rc('font', size=20)
 plt.rc('figure', titlesize=40, titleweight='bold')
 plt.style.use('ggplot')
 
 
+
 # Set options
 np.set_printoptions(suppress=True, precision=6, edgeitems=20, linewidth=100, formatter={"float": lambda x: "{:.3f}".format(x)})
 pd.set_option('display.max_rows', 1000)
 pd.set_option('display.max_columns', 1000)
 pd.set_option('display.max_colwidth', 1000)
 pd.set_option('display.width', 1000)
+pd.set_option('display.float_format', '{:.2f}'.format)
 
 
 # Warning
 warnings.filterwarnings('ignore')
```

### Comparing `analysis-tools-0.1.2/analysis_tools/eda.py` & `analysis-tools-0.2.1/analysis_tools/eda.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,454 +1,624 @@
 """Exploratory Data Analysis tools
 
 This module contains functions and classes for exploratory data analysis.
 """
-
 # Author: Dongjin Yoon <djyoon0223@gmail.com>
 
 
 from analysis_tools.common import *
 
 
-def _plot_on_ax(plot_fn, suptitle,                                               ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+# Utility function
+def plot_on_ax(plot_fn,                                 ax=None, title=None, save_dir=None, figsize=None, **plot_kws):
     """Plot on a single axis if ax is not None. Otherwise, plot on a new figure.
 
     Parameters
     ----------
     plot_fn : function
         Function to plot.
 
-    suptitle : str
-        Title of the plot.
-
-    ax : matplotlib.axes.Axes or list of matplotlib.axes.Axes
+    ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title of the plot.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
-
-    show_plot : bool
-        Whether to show the plot.
     """
     if ax is not None:
+        cm = contextlib.nullcontext()
+    else:
+        fig, ax = plt.subplots(figsize=PLOT_PARAMS.get('figsize', figsize))
+        cm = FigProcessor(fig, save_dir, title)
+    with cm:
         plot_fn(ax)
+        if plot_kws.get('xlabel', False) is not True:
+            ax.set_xlabel(None)
+        if plot_kws.get('ylabel', False) is not True:
+            ax.set_ylabel(None)
+
+
+# Single feature
+def plot_fn_num(data_f, ax, **plot_kws):
+    if len(data_f.dropna()) == 0:
+        return
+    sns.histplot(data_f, bins=PLOT_PARAMS.get('bins', plot_kws), ax=ax, kde=True, stat='density', color=plot_kws.get('color', None))
+def plot_fn_cat(data_f, ax, **plot_kws):  # cat: not numerical dtypes
+    if len(data_f.dropna()) == 0:
+        return
+    if is_datetime_str(data_f):
+        plot_fn_datetime(data_f, ax, **plot_kws)
+        title = data_f.name
     else:
-        fig, ax = plt.subplots(figsize=figsize)
-        with FigProcessor(fig, dir_path, show_plot, suptitle):
-            plot_fn(ax)
+        if (plot_kws.get('sample') is not None) and (plot_kws['sample'] < data_f.nunique()):
+            data_f = data_f.sample(plot_kws['sample'])
+            title = f"{data_f.name}(sample={plot_kws['sample']})"
+        else:
+            title = data_f.name
+        cnts = data_f.value_counts(normalize=True).sort_index()
+        sns.barplot(x=cnts.index, y=cnts.values, order=cnts.index, ax=ax)
+        xticklabels = cnts.sort_values()[-PLOT_PARAMS.get('n_classes', plot_kws):].index
+        ax.set_xticks(lmap(lambda l: cnts.index.get_loc(l), xticklabels))
+        ax.set_xticklabels(xticklabels, rotation=30, ha='right', rotation_mode='anchor')
+    return title
+def plot_fn_datetime(data_f, ax, **plot_kws):
+    if len(data_f.dropna()) == 0:
+        return
+    data_f = pd.to_datetime(data_f)
+    sns.histplot(data_f, bins=PLOT_PARAMS.get('bins', plot_kws), ax=ax, kde=True, stat='density', color=plot_kws.get('color', None))
+    ax.tick_params(axis='x', labelrotation=30)
 
 
 # Missing value
-def plot_missing_value(data,                                                              dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+def plot_missing_value(data, show_df=False,                      title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot counts of missing values of each feature.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
 
-    dir_path : str
+    show_df : bool
+        Whether to show value counts dataframe.
+
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, None], 'b': [1, None, 3, 4, 5], 'c': [None, 2, 3, 4, 5]})
-    >>> eda.plot_missing_value(data, dir_path='.')
+    >>> eda.plot_missing_value(data, save_dir='.')
     """
-    fig, axes = plt.subplots(2, 1, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Missing value"):
+    fig, axes = plt.subplots(2, 1, figsize=PLOT_PARAMS.get('figsize', figsize))
+    with FigProcessor(fig, save_dir, "Missing value" if title == 'auto' else title):
         msno.matrix(data, ax=axes[0])
         ms = data.isnull().sum()
-        sns.barplot(ms.index, ms, ax=axes[1])
+        sns.barplot(x=ms.index, y=ms, ax=axes[1])
         axes[1].bar_label(axes[1].containers[0])
         axes[1].set_xticklabels([])
 
+    if show_df:
+        data_null = data[data.isna().any(1)]
+        for f in data_null:
+            if data_null[f].notnull().sum() > 0:
+                display(data_null.value_counts(f).sort_index().to_frame().T.style.background_gradient(axis=1))
+
 
-# Features
-def plot_features(data, bins=PLOT_PARAMS['BINS'], n_cols=PLOT_PARAMS['N_COLS'],           dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+# Multiple features
+def plot_features(data1, data2=None, sample_cat=1000,            title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot histogram or bar for all features.
 
     Parameters
     ----------
-    data : pandas.DataFrame
+    data1 : pandas.DataFrame
+        DataFrame to be analyzed.
+
+    data2 : pandas.DataFrame
         DataFrame to be analyzed.
 
-    bins : int
-        Number of bins.
+    sample_cat : int
+        Number of samples for categorical features.
 
-    n_cols : int
-        Number of columns.
+    title : str
+        Title.
 
-    dir_path : str
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_features(data, dir_path='.')
+    >>> eda.plot_features(data, save_dir='.')
     """
-    n_features = len(data.columns)
+    n_cols = PLOT_PARAMS.get('n_cols', plot_kws)
+    n_features = len(data1.columns)
     n_rows     = int(np.ceil(n_features / n_cols))
-    fig, axes = plt.subplots(n_rows, n_cols, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Features"):
+    fig, axes = plt.subplots(n_rows, n_cols, figsize=PLOT_PARAMS.get('figsize', figsize))
+    with FigProcessor(fig, save_dir, "Features" if title == 'auto' else title):
         for ax in axes.flat[n_features:]:
             ax.axis('off')
-        for ax, f in zip(axes.flat, data):
-            data_f_notnull = data[f].dropna()
-            ax.set_title(f)
-            if data_f_notnull.nunique() > bins:
-                # Numerical feature or categorical feature(many classes)
-                try:
-                    ax.hist(data_f_notnull, bins=bins, density=True, color='olive', alpha=0.5)
-                    # sns.histplot(data_f_notnull, stat='probability', color='olive', alpha=0.5, ax=ax)  # easy to understand but, too slow
-                    # ax.set_ylabel(None)
-                except Exception as e:
-                    print(f"[{f}]: {e}")
-            else:
-                # Categorical feature(a few classes)
-                cnts = data[f].value_counts(normalize=True).sort_index()  # normalize including NaN
-                ax.bar(cnts.index, cnts.values, width=0.5, alpha=0.5)
-                ax.set_xticks(cnts.index)
-def plot_features_target(data, target, n_cols=PLOT_PARAMS['N_COLS'], target_type='auto',  dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+        for ax, f in zip(axes.flat, data1):
+            datas = [data1] if data2 is None else [data1, data2]
+            for data, color in zip(datas, COLORS):
+                plot_kws['color'] = color
+                if dtype(data[f]) == 'num':
+                    plot_fn_num(data[f], ax, **plot_kws)
+                    # ax.hist(data[f], bins=bins, density=True, color=color, alpha=0.5)
+                    title = f
+                else:
+                    title = plot_fn_cat(data[f], ax, sample=sample_cat, **plot_kws)
+            ax.set_title(title)
+            ax.set_xlabel(None), ax.set_ylabel(None)
+def plot_features_target(data, target, target_type='auto',       title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot features vs target.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
         Dtypes of numerical features should be `number`(`numpy.float32` is recommended).
         Dtypes of categorical features should be `string` or `category`.
 
     target : str
         Target feature.
 
-    dir_path : str
-        Directory path to save the plot.
-
-    n_cols : int
-        Number of columns.
-
     target_type : str
         Type of target.
         target_type should be 'auto' or 'num', 'cat'.
         target_type is inferred automatically when 'auto' is set.
 
+    title : str
+        Title.
+
+    save_dir : str
+        Directory path to save the plot.
+
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import numpy as np
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 1, 2], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': ['a10', 'b22', 'c11', 'a10', 'b22']})
     >>> num_features = ['a']
     >>> cat_features = data.columns.drop(num_features)
     >>> data[num_features] = data[num_features].astype('float32')
     >>> data[cat_features] = data[cat_features].astype('string')
-    >>> eda.plot_features_target(data, 'a', dir_path='.')
+    >>> eda.plot_features_target(data, 'a', save_dir='.')
     """
-    num_features = data.select_dtypes('number').columns
+    n_cols = PLOT_PARAMS.get('n_cols', plot_kws)
     if target_type == 'auto':
-        target_type = 'num' if target in num_features else 'cat'
-    n_features   = len(data.columns)
-    n_rows       = int(np.ceil(n_features/n_cols))
-    fig, axes    = plt.subplots(n_rows, n_cols, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Features vs Target"):
-        for ax in axes.flat[n_features-1:]:  # -1: except target
+        target_type = dtype(data[target])
+    n_features = len(data.columns) - 1  # -1: except target
+    n_rows     = int(np.ceil(n_features/n_cols))
+    fig, axes  = plt.subplots(n_rows, n_cols, figsize=PLOT_PARAMS.get('figsize', figsize))
+    axes       = np.array(axes) if n_rows*n_cols == 1 else axes
+    with FigProcessor(fig, save_dir, "Features vs Target" if title == 'auto' else title):
+        for ax in axes.flat[n_features:]:
             ax.axis('off')
         for ax, f in zip(axes.flat, data.columns.drop(target)):
+            eval(f"plot_{dtype(data[f])}_{target_type}_features")(data, f, target, ax=ax, **plot_kws)
             ax.set_title(f"{f} vs {target}")
-            f_type = 'num' if f in num_features else 'cat'
-            eval(f"plot_{f_type}_{target_type}_features")(data, f, target, ax=ax)
-def plot_corr(corr, annot=True, mask=True,                                                dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
-    """Plot correlation matrix.
+            ax.set_xlabel(None);  ax.set_ylabel(None)
+def plot_two_features(data, f1, f2,                     ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
+    """Plot joint distribution of two features.
 
     Parameters
     ----------
-    corr : pandas.DataFrame
-        Correlation matrix.
+    data : pandas.DataFrame
+        DataFrame to be analyzed.
 
-    annot : bool
-        Whether to show values.
+    f1 : str
+        Feature 1.
 
-    mask : bool
-        Whether to show only lower triangular matrix.
+    f2 : str
+        Feature 2.
+
+    ax : matplotlib.axes.Axes
+        Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
-    >>> data = pd.DataFrame({'a': [1, 2, 3, 1, 2], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [10, 20, 30, 10, 20]})
-    >>> eda.plot_corr(corr, dir_path='.')
+    >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
+    >>> eda.plot_two_features(data, 'a', 'b', save_dir='.')
     """
-    fig, ax = plt.subplots(figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Correlation matrix"):
-        mask_mat = np.eye(len(corr), dtype=bool)
-        mask_mat[np.triu_indices_from(mask_mat, k=1)] = mask
-        sns.heatmap(corr, mask=mask_mat, ax=ax, annot=annot, fmt=".2f", cmap='coolwarm', center=0)
-def plot_num_feature(data_f, bins=PLOT_PARAMS['BINS'],                           ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+    plot_fn = lambda ax: eval(f"plot_{dtype(data[f1])}_{dtype(data[f2])}_features")(data, f1, f2, ax=ax, **plot_kws)
+    plot_on_ax(plot_fn, ax, f"{f1} vs {f2}" if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_num_feature(data_f,                            ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot histogram of a numeric feature.
 
     Parameters
     ----------
     data_f : pandas.Series
         Series to be analyzed.
 
-    bins : int
-        Number of bins.
-
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_num_feature(data['a'], dir_path='.')
+    >>> eda.plot_num_feature(data['a'], save_dir='.')
     """
     def plot_fn(ax):
-        sns.histplot(data_f, bins=bins, ax=ax, kde=True, stat='density')
-        ax.set_xlabel(None)
-    _plot_on_ax(plot_fn, data_f.name, ax, dir_path, figsize, show_plot)
-def plot_cat_feature(data_f,                                                     ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+        plot_fn_num(data_f, ax, **plot_kws)
+    plot_on_ax(plot_fn, ax, data_f.name if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_cat_feature(data_f,                            ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot bar of a categorical feature.
 
     Parameters
     ----------
     data_f : pandas.Series
         Series to be analyzed.
 
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_cat_feature(data['b'], dir_path='.')
+    >>> eda.plot_cat_feature(data['b'], save_dir='.')
     """
     def plot_fn(ax):
-        density = data_f.value_counts(normalize=True).sort_index()
-        sns.barplot(density.index, density.values, ax=ax)
-    _plot_on_ax(plot_fn, data_f.name, ax, dir_path, figsize, show_plot)
-def plot_num_num_features(data, f1, f2, bins=PLOT_PARAMS['BINS'],                ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
-    """Plot histogram of two numeric features.
+        plot_fn_cat(data_f, ax, **plot_kws)
+    plot_on_ax(plot_fn, ax, data_f.name if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_num_num_features(data, f1, f2, sample=100_000, ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
+    """Plot scatter plot of two numeric features.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
 
     f1 : str
         First numerical feature.
 
     f2 : str
         Second numerical feature.
 
-    bins : int
-        Number of bins.
+    sample : int
+        Number of samples.
+        If sample is None or False, then use entire data.
 
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_num_num_features(data, 'a', 'c', dir_path='.')
+    >>> eda.plot_num_num_features(data, 'a', 'c', save_dir='.')
     """
     def plot_fn(ax):
-        sns.histplot(x=data[f1], y=data[f2], bins=bins, ax=ax)
-        ax.set_xlabel(None);  ax.set_ylabel(None)
-    _plot_on_ax(plot_fn, f"{f1} vs {f2}", ax, dir_path, figsize, show_plot)
-def plot_num_cat_features(data, f1, f2, n_classes=PLOT_PARAMS['N_CLASSES_PLOT'], ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+        sns.scatterplot(x=data[f1], y=data[f2], alpha=PLOT_PARAMS.get('alpha', plot_kws), ax=ax, color=plot_kws.get('color', None))
+    if sample and (len(data) > sample):
+        data = data.sample(sample)
+    plot_on_ax(plot_fn, ax, f"{f1} vs {f2}" if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_num_cat_features(data, f1, f2,                 ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot violinplot of categorical, numerical features.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
 
     f1 : str
         First numerical feature.
 
     f2 : str
         Second categorical feature.
 
-    n_classes : int
-        Number of classes to plot.
 
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_num_cat_features(data, 'a', 'b', dir_path='.')
+    >>> eda.plot_num_cat_features(data, 'a', 'b', save_dir='.')
     """
     def plot_fn(ax):
-        selected_classes = data[f2].value_counts().index[:n_classes]
+        selected_classes = data[f2].value_counts().index[:PLOT_PARAMS.get('n_classes', plot_kws)]
         idxs_selected    = data[f2][data[f2].isin(selected_classes)].index
         data_f1, data_f2 = data[f1][idxs_selected], data[f2][idxs_selected]
         sns.violinplot(x=data_f1, y=data_f2, ax=ax, orient='h', order=reversed(sorted(selected_classes)), cut=0)
-        ax.set_xlabel(None);  ax.set_ylabel(None)
-    _plot_on_ax(plot_fn, f"{f1} vs {f2}", ax, dir_path, figsize, show_plot)
-def plot_cat_num_features(data, f1, f2, n_classes=PLOT_PARAMS['N_CLASSES_PLOT'], ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+    plot_on_ax(plot_fn, ax, f"{f1} vs {f2}" if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_cat_num_features(data, f1, f2,                 ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot violinplot of categorical, numerical features.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
 
     f1 : str
         First categorical feature.
 
     f2 : str
         Second numerical feature.
 
-    n_classes : int
-        Number of classes to plot.
-
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
-    >>> eda.plot_cat_num_features(data, 'b', 'a', dir_path='.')
+    >>> eda.plot_cat_num_features(data, 'b', 'a', save_dir='.')
     """
     def plot_fn(ax):
-        selected_classes = data[f1].value_counts().index[:n_classes]
+        selected_classes = data[f1].value_counts().index[:PLOT_PARAMS.get('n_classes', plot_kws)]
         idxs_selected    = data[f1][data[f1].isin(selected_classes)].index
         data_f1, data_f2 = data[f1][idxs_selected], data[f2][idxs_selected]
         sns.violinplot(x=data_f1, y=data_f2, ax=ax, orient='v', order=sorted(selected_classes), cut=0)
-        ax.set_xlabel(None);  ax.set_ylabel(None)
-    _plot_on_ax(plot_fn, f"{f1} vs {f2}", ax, dir_path, figsize, show_plot)
-def plot_cat_cat_features(data, f1, f2, n_classes=PLOT_PARAMS['N_CLASSES_PLOT'], ax=None, dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+    plot_on_ax(plot_fn, ax, f"{f1} vs {f2}" if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_cat_cat_features(data, f1, f2,                 ax=None, title='auto', save_dir=None, figsize=None, **plot_kws):
     """Plot heatmap of two categorical features.
 
     Parameters
     ----------
     data : pandas.DataFrame
         DataFrame to be analyzed.
 
     f1 : str
         First categorical feature.
 
     f2 : str
         Second categorical feature.
 
-    n_classes : int
-        Number of classes to plot.
-
     ax : matplotlib.axes.Axes
         Axis to plot.
 
-    dir_path : str
+    title : str
+        Title.
+
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': ['a10', 'b22', 'c11', 'a10', 'b22']})
-    >>> eda.plot_cat_cat_features(data, 'b', 'c', dir_path='.')
+    >>> eda.plot_cat_cat_features(data, 'b', 'c', save_dir='.')
     """
     def plot_fn(ax):
-        ratio = pd.crosstab(data[f2], data[f1], normalize='columns')
+        ratio = pd.crosstab(data[f2], data[f1], normalize=plot_kws.get('normalize', 'columns'))  # normalize is in ['index', 'columns', 'all']
         ratio.sort_index(inplace=True, ascending=False)  # sort by index
         ratio = ratio[sorted(ratio)]                     # sort by column
+        n_classes = PLOT_PARAMS.get('n_classes', plot_kws)
         ratio = ratio.iloc[:n_classes, :n_classes]
         sns.heatmap(ratio, ax=ax, annot=True, fmt=".2f", cmap=sns.light_palette('firebrick', as_cmap=True), cbar=False)
-        ax.set_xlabel(None);  ax.set_ylabel(None)
-    _plot_on_ax(plot_fn, f"{f1} vs {f2}", ax, dir_path, figsize, show_plot)
+    plot_on_ax(plot_fn, ax, f"{f1} vs {f2}" if title == 'auto' else title, save_dir, figsize, **plot_kws)
+def plot_pair(data1, data2=None, subplot=True,                   title='auto', save_dir=None, figsize=(20, 20), **plot_kws):
+    """Plot pair plot for all numerical features.
+
+    Parameters
+    ----------
+    data1 : pandas.DataFrame
+        DataFrame to be analyzed.
+
+    data2 : pandas.DataFrame
+        DataFrame to be analyzed.
+
+    subplot : bool
+        Whether to split figure.
+
+    title : str
+        Title.
+
+    save_dir : str
+        Directory path to save the plot.
+
+    figsize : tuple
+        Figure size.
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> import analysis_tools.eda as eda
+    >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
+    >>> eda.plot_pair(data, save_dir='.')
+    """
+    def plot_custom_pair(data, g):
+        fs = data.columns
+        for row, col in permutations(range(len(fs)), 2):
+            if (row == col) or (dtype(data[fs[col]]) == 'cat' and dtype(data[fs[row]]) == 'cat'):
+                # TODO: cat - cat features
+                g.axes[row, col].axis('off')
+            else:
+                plot_two_features(data, fs[col], fs[row], ax=g.axes[row, col], **plot_kws)
+        g.map_diag(sns.histplot)
+
+    title = 'Pairplot' if title == 'auto' else title
+    figsize = PLOT_PARAMS.get('figsize', figsize)
+    if data2 is None:
+        # fig = sns.pairplot(data1, plot_kws={'alpha': PLOT_PARAMS.get('alpha', plot_kws), 's': PLOT_PARAMS.get('s', plot_kws)}).fig
+        fs = data1.columns
+        g  = sns.PairGrid(data1, diag_sharey=False, x_vars=fs, y_vars=fs)
+        fig, axes = g.fig, g.axes
+        with FigProcessor(fig, save_dir, title, tight_layout=False):
+            plot_custom_pair(data1, g)
+            fig.set_size_inches(figsize)
+    else:
+        if subplot:
+            n_cols = 1 if data2 is None else 2
+            grids  = gridspec.GridSpec(1, n_cols)
+            fig    = plt.figure(figsize=(n_cols*figsize[0], figsize[1]))
+            with FigProcessor(fig, save_dir, title, tight_layout=False):
+                for grid, data, color in zip(grids, (data1, data2), COLORS):
+                    plot_kws['color'] = color
+                    fs = data.columns
+                    g  = sns.PairGrid(data, diag_sharey=False, x_vars=fs, y_vars=fs)
+                    plot_custom_pair(data, g)
+                    SeabornFig2Grid(g, fig, grid)
+                grids.tight_layout(fig)
+        else:
+            data1['ID'], data2['ID'] = 'First', 'Second'
+            data = pd.concat([data1, data2], ignore_index=True)
+            fig  = sns.pairplot(data, hue='ID', plot_kws={'alpha': PLOT_PARAMS.get('alpha', plot_kws), 's': PLOT_PARAMS.get('marker_size', plot_kws), 'markers': ['o', 'D'], 'diag_kind': 'hist'}).fig
+            with FigProcessor(fig, save_dir, title, tight_layout=False):
+                fig.set_size_inches(figsize)
+def plot_corr(corr1, corr2=None, annot=True, mask=True,          title='auto', save_dir=None, figsize=(15, 15), **plot_kws):
+    """Plot correlation matrix.
+
+    Parameters
+    ----------
+    corr1 : pandas.DataFrame
+        Correlation matrix.
+
+    corr2 : pandas.DataFrame
+        Correlation matrix.
+
+    annot : bool
+        Whether to show values.
+
+    mask : bool
+        Whether to show only lower triangular matrix.
+
+    title : str
+        Title.
+
+    save_dir : str
+        Directory path to save the plot.
+
+    figsize : tuple
+        Figure size.
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> import analysis_tools.eda as eda
+    >>> data = pd.DataFrame({'a': [1, 2, 3, 1, 2], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [10, 20, 30, 10, 20]})
+    >>> eda.plot_corr(corr, save_dir='.')
+    """
+    title = "Correlation matrix" if title == 'auto' else title
+    if corr2 is None:
+        def plot_fn(ax):
+            mask_mat = np.eye(len(corr1), dtype=bool)
+            mask_mat[np.triu_indices_from(mask_mat, k=1)] = mask
+            sns.heatmap(corr1, mask=mask_mat, ax=ax, annot=annot, fmt=".2f", cmap='coolwarm', center=0)
+        plot_on_ax(plot_fn, None, title, save_dir, figsize, **plot_kws)
+    else:
+        figsize = PLOT_PARAMS.get('figsize', figsize)
+        fig, axes = plt.subplots(1, 2, figsize=(2*figsize[0], figsize[1]))
+        with FigProcessor(fig, save_dir, title):
+            for ax, corr in zip(axes.flat, (corr1, corr2)):
+                mask_mat = np.eye(len(corr), dtype=bool)
+                mask_mat[np.triu_indices_from(mask_mat, k=1)] = mask
+                sns.heatmap(corr, mask=mask_mat, ax=ax, annot=annot, fmt=".2f", cmap='coolwarm', center=0)
+
+
+# Time series features
+def plot_ts_features(data,                                       title='auto', save_dir=None, figsize=None, **plot_kws):
+    """Plot time series line plot for all numerical features.
+
+    Parameters
+    ----------
+    data : pandas.DataFrame
+        DataFrame to be analyzed.
+
+    title : str
+        Title
+
+    save_dir : str
+        Directory path to save the plot.
+
+    figsize : tuple
+        Figure size.
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> import analysis_tools.eda as eda
+    >>> data = pd.DataFrame({'a': [1, 2, 3, 4, 5], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [1.2, 2.3, 3.4, 4.5, 5.6]})
+    >>> eda.plot_ts_features(data, save_dir='.')
+    """
+    plot_on_ax(lambda ax: data.select_dtypes('number').plot(subplots=True, ax=ax, sharex=True),
+               None, 'Features' if title == 'auto' else title, save_dir, figsize, **plot_kws)
```

### Comparing `analysis-tools-0.1.2/analysis_tools/metrics.py` & `analysis-tools-0.2.1/analysis_tools/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,129 +1,122 @@
 """Metric analysis tools
 
 Performance evaluation metrics are defined here.
 """
-
 # Author: Dongjin Yoon <djyoon0223@gmail.com>
 
 
 from analysis_tools.common import *
 
 
-def confusion_matrix_analysis(y_true, y_pred,                                                                                                         dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+def confusion_matrix_analysis(y_true, y_pred,                                                                 save_dir=None, figsize=None, **plot_kws):
     """Plot confusion matrix
 
     Parameters
     ----------
     y_true : array-like of shape (n_samples,)
         Ground truth (correct) target values.
 
     y_pred : array-like of shape (n_samples,)
         Estimated targets as returned by a classifier.
 
-    figsize : tuple
-        Figure size.
-
-    dir_path : str
+    save_dir : str
         Path to save the figure.
 
-    show_plot : bool
-        Whether to show the figure.
+    figsize : tuple
+        Figure size.
 
     Returns
     -------
     collections of metrics : dictionary
         Confusion matrix, accuracy, precision, recall, f1 score
 
     Examples
     --------
     >>> from analysis_tools.metrics import confusion_matrix_analysis
     >>> y_true = [0, 0, 0, 0, 1, 1, 1, 1]
     >>> y_pred = [0, 0, 0, 1, 1, 1, 1, 1]
-    >>> confusion_matrix_analysis(y_true, y_pred, dir_path='.')
+    >>> confusion_matrix_analysis(y_true, y_pred, save_dir='.')
     """
     from sklearn.metrics import confusion_matrix, accuracy_score, precision_score, recall_score, f1_score
 
     normalized_C = confusion_matrix(y_true, y_pred, normalize='true')
     assert all(normalized_C.sum(axis=1) == 1), "Confusion matrix is not normalized"
 
-    fig, axes = plt.subplots(2, 2, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Confusion matrix"):
+    fig, axes = plt.subplots(2, 2, figsize=PLOT_PARAMS.get('figsize', figsize))
+    with FigProcessor(fig, save_dir, "Confusion matrix"):
         sns.heatmap(normalized_C, annot=False, fmt='.2%', cmap='gray', ax=axes[0, 0])
         sns.heatmap(normalized_C, annot=True, fmt='.2%', cmap='gray', ax=axes[0, 1])
 
         normalized_C_off_diagonal = copy(normalized_C)
         np.fill_diagonal(normalized_C_off_diagonal, 0)  # off-diagonal
         sns.heatmap(normalized_C_off_diagonal, annot=False, fmt='.2%', cmap='gray', ax=axes[1, 0])
         sns.heatmap(normalized_C_off_diagonal, annot=True, fmt='.2%', cmap='gray', ax=axes[1, 1])
         for ax in axes.flat:
             ax.xaxis.tick_top()
     return dict(
         confusion_matrix=normalized_C,
         accuracy=accuracy_score(y_true, y_pred), precision=precision_score(y_true, y_pred), recall=recall_score(y_true, y_pred), f1_score=f1_score(y_true, y_pred),
     )
-def curve_analysis(y_true, y_score,                                                                                                                   dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+def curve_analysis(y_true, y_score,                                                                           save_dir=None, figsize=None, **plot_kws):
     """Plot Precision-Recall and ROC curves
 
     Parameters
     ----------
     y_true : array-like of shape (n_samples,)
         Ground truth (correct) target values.
 
     y_score : array-like of shape (n_samples,)
         Estimated probabilities or output of a decision function.
 
-    dir_path : str
-        Path to save the figure.
-
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the figure.
+    save_dir : str
+        Path to save the figure.
 
     Examples
     --------
     >>> from analysis_tools.metrics import curve_analysis
     >>> y_true  = [0, 0, 0, 0, 1, 1, 1, 1]
     >>> y_score = [0.1, 0.4, 0.35, 0.8, 0.85, 0.8, 0.9, 0.95]
-    >>> curve_analysis(y_true, y_score, dir_path='.')
+    >>> curve_analysis(y_true, y_score, save_dir='.')
     """
     from sklearn.metrics import precision_recall_curve, average_precision_score, roc_curve, roc_auc_score
 
     precisions, recalls, thresholds_pr = precision_recall_curve(y_true, y_score)
     fpr, tpr, thresholds_roc           = roc_curve(y_true, y_score)
-    fig, axes = plt.subplots(1, 3, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Precision-Recall & ROC curves"):
+    fig, axes = plt.subplots(1, 3, figsize=PLOT_PARAMS.get('figsize', figsize))
+    with FigProcessor(fig, save_dir, "Precision-Recall & ROC curves"):
         # Thresholds-PR
-        axes[0].show_plot(thresholds_pr, precisions[:-1], 'b--', label='Precision')
-        axes[0].show_plot(thresholds_pr, recalls[:-1], 'g-', label='Recall')
+        axes[0].plot(thresholds_pr, precisions[:-1], 'b--', label='Precision')
+        axes[0].plot(thresholds_pr, recalls[:-1], 'g-', label='Recall')
         axes[0].set_xlabel('Threshold')
         axes[0].set_ylabel('Precision/Recall')
         axes[0].set_ylim([0, 1])
         axes[0].legend()
 
         # Precision-Recall
-        axes[1].show_plot(recalls, precisions, label=f"PR-AUC: {average_precision_score(y_true, y_score):.3f}")
+        axes[1].plot(recalls, precisions, label=f"PR-AUC: {average_precision_score(y_true, y_score):.3f}")
         axes[1].set_xlabel('Recall')
         axes[1].set_ylabel('Precision')
         axes[1].set_xlim([0, 1])
         axes[1].set_ylim([0, 1])
         axes[1].legend()
 
         # ROC
-        axes[2].show_plot(fpr, tpr, linewidth=2, label=f"ROC-AUC: {roc_auc_score(y_true, y_score):.3f}")
-        axes[2].show_plot([0, 1], [0, 1], 'k--')
+        axes[2].plot(fpr, tpr, linewidth=2, label=f"ROC-AUC: {roc_auc_score(y_true, y_score):.3f}")
+        axes[2].plot([0, 1], [0, 1], 'k--')
         axes[2].set_xlabel('FPR(=FP/RealNegative)')
         axes[2].set_ylabel('TPR(Recall)')
         axes[2].set_xlim([0, 1])
         axes[2].set_ylim([0, 1])
         axes[2].legend()
 
-def get_feature_importance(data, target, bins=PLOT_PARAMS['BINS'], problem='classification',                                                          dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+def get_feature_importance(data, target, bins=None, problem='classification',                                 save_dir=None, figsize=None, **plot_kws):
     """Get feature importance using RandomForest model.
 
     The metrics are mean decrease in impurity, mean accuracy decrease, mean rank
 
     Parameters
     ----------
     data : pandas.DataFrame
@@ -134,38 +127,35 @@
 
     bins : int
         Number of bins.
 
     problem : str
         Problem type.(`classification` or `regression`)
 
-    dir_path : str
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Returns
     -------
     pandas.DataFrame
         Feature importances.
 
     Examples
     --------
     >>> import pandas as pd
     >>> import analysis_tools.eda as eda
     >>> data = pd.DataFrame({'a': [1, 2, 3, 1, 2], 'b': ['a', 'b', 'c', 'd', 'e'], 'c': [10, 20, 30, 10, 20]})
     >>> num_features = ['c']
     >>> cat_features = data.columns.drop(num_features)
     >>> data[num_features] = data[num_features].astype(np.float32)
     >>> data[cat_features] = data[cat_features].astype('category')
-    >>> eda.get_feature_importance(data, 'a', dir_path='.')
+    >>> eda.get_feature_importance(data, 'a', save_dir='.')
     """
     from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
     from sklearn.inspection import permutation_importance
     from sklearn.preprocessing import OrdinalEncoder
 
     # 1. Split data into X, y
     data               = data.dropna()
@@ -183,28 +173,29 @@
 
     # 4. Mean importance
     fi1     = pd.Series(range(len(MDI_importance)), index=MDI_importance.index, name='MDI')
     fi2     = pd.Series(range(len(perm_importance)), index=perm_importance.index, name='Permutation')
     mean_fi = pd.Series(((fi1 + fi2)/2).sort_values(), name='Mean')
 
     # 5. Plot
-    fig, axes = plt.subplots(3, 1, figsize=figsize)
-    with FigProcessor(fig, dir_path, show_plot, "Feature importance"):
+    bins = PLOT_PARAMS.get('bins', bins)
+    fig, axes = plt.subplots(3, 1, figsize=PLOT_PARAMS.get('figsize', figsize))
+    with FigProcessor(fig, save_dir, "Feature importance"):
         for ax, data, ylabel, title in zip(axes,
                                           [MDI_importance.head(bins), perm_importance.head(bins), mean_fi.head(bins)],
-                                          ["Mean decrease in impurity", "Mean accuracy decrease", "Mean rank"],
+                                          ["Mean decrease in impurity", "Mean score decrease", "Mean rank"],
                                           ["Feature importance using MDI", "Feature importance using permutation on full model", "Feature importance using MDI, permutation on full model"]):
-            sns.barplot(data.index, data, ax=ax)
+            sns.barplot(x=data.index, y=data, ax=ax)
             ax.set_ylabel(ylabel)
             ax.set_title(title)
             ax.tick_params(axis='x', rotation=30)
 
-    return pd.concat([MDI_importance, perm_importance, mean_fi], axis='columns')
+    return pd.concat([fi1, fi2, mean_fi], axis='columns').sort_values('Mean')
 
-def plot_learning_curve(model, X_train, y_train, X_val, y_val, n_subsets_step=PLOT_PARAMS['LEARNING_CURVE_N_SUBSETS_STEP'], problem='classification', dir_path=None, figsize=PLOT_PARAMS['FIGSIZE'], show_plot=PLOT_PARAMS['SHOW_PLOT']):
+def plot_learning_curve(model, X_train, y_train, X_val, y_val, n_subsets_step=None, problem='classification', save_dir=None, figsize=None, **plot_kws):
     """Plot learning curve
 
     Parameters
     ----------
     model : sklearn.base.BaseEstimator
         Model to train.
 
@@ -222,23 +213,20 @@
 
     n_subsets_step : int
         Step size for subsets.
 
     problem : str
         Problem type.(`classification` or `regression`)
 
-    dir_path : str
+    save_dir : str
         Directory path to save the plot.
 
     figsize : tuple
         Figure size.
 
-    show_plot : bool
-        Whether to show the plot.
-
     Examples
     --------
     >>> from analysis_tools.metrics import plot_learning_curve
     >>> from sklearn.linear_model import LogisticRegression
     >>> X_train = [[0, 0], [1, 1]]
     >>> y_train = [0, 1]
     >>> X_val = [[0, 0], [1, 1]]
@@ -247,21 +235,21 @@
     >>> plot_learning_curve(model, X_train, y_train, X_val, y_val)
     """
     from sklearn.metrics import precision_score, recall_score, f1_score, accuracy_score, mean_squared_error, r2_score
 
     if problem == 'classification':
         error_fn_names = ['F1 score', 'Precision', 'Recall', 'Accuracy']
         error_fns      = [precision_score, recall_score, f1_score, accuracy_score]
-        fig, axes = plt.subplots(4, 1, figsize=figsize)
+        fig, axes = plt.subplots(4, 1, figsize=PLOT_PARAMS.get('figsize', figsize))
     else:
         error_fn_names = ['MSE', 'R-squared']
         error_fns      = [mean_squared_error, r2_score]
-        fig, axes      = plt.subplots(2, 1, figsize=figsize)
+        fig, axes      = plt.subplots(2, 1, figsize=PLOT_PARAMS.get('figsize', figsize))
 
-    with FigProcessor(fig, dir_path, show_plot, "Learning curve"):
+    with FigProcessor(fig, save_dir, "Learning curve"):
         for ax, error_fn_name, error_fn in zip(axes, error_fn_names, error_fns):
             train_sub_errors, val_errors = pd.Series([], name='Training error'), pd.Series([], name='Validation error')
             for n_subsets in trange(1, len(X_train), n_subsets_step):
                 try:
                     X_train_sub, y_train_sub = X_train[:n_subsets], y_train[:n_subsets]
                     model.fit(X_train_sub, y_train_sub)
                     y_train_sub_pred = model.predict(X_train_sub)
@@ -357,11 +345,11 @@
     for model in tqdm(models):
         model.fit(X_train, y_train)
         score_train = model.score(X_train, y_train)
         score_val   = model.score(X_val, y_val)
         results.append((score_train, score_val, model))
     results = sorted(results, key=lambda result: result[1], reverse=True)  # sort by score_val
 
-    print("- Scores")  # accuracy(regression), r-square(classification)
+    print("- Scores")  # accuracy(classification), r-square(regression)
     for score_train, score_val, model in results:
         print(f"{score_train:.3f} (train) / {score_val:.3f} (val) : {model.__class__.__name__}")
     return results
```

### Comparing `analysis-tools-0.1.2/analysis_tools.egg-info/PKG-INFO` & `analysis-tools-0.2.1/analysis_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 Metadata-Version: 2.1
 Name: analysis-tools
-Version: 0.1.2
+Version: 0.2.1
 Summary: Analysis tools for machine learning projects
-Home-page: https://github.com/djy-git/analysis-tools
+Home-page: https://pypi.org/project/analysis-tools/
 Author: Dongjin Yoon
 Author-email: djyoon0223@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Analysis tools for Machine learning projects
 
 ## 1. Usage
 ```bash
-# Load repository manually
-$ git clone https://github.com/djy-git/analysis-tools.git 
-
-# Install with Pypi
 $ pip install analysis-tools
 ```
 
 ## 2. Tutorial
 [examples/titanic/eda.ipynb](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/eda.ipynb)를 참고
 
 ```python
-from analysis_tools.eda import *
+from analysis_tools import eda, metrics
 
 data   = pd.DataFrame(..)
 target = 'survived'
 
 num_features       = ['age', 'sibsp', 'parch', 'fare']
 cat_features       = data.columns.drop(num_features)
 data[num_features] = data[num_features].astype('float32')
 data[cat_features] = data[cat_features].astype('string')
 
-plot_missing_value(data)
-plot_features(data)
-plot_features_target(data, target)
-plot_corr(data.corr())
+eda.plot_missing_value(data)
+eda.plot_features(data)
+eda.plot_features_target(data, target)
+eda.plot_corr(data.corr())
+metrics.get_feature_importance(data, target)
 ```
 
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Missing%20value_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Features_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Features%20vs%20Target_1.png?raw=true)
 ![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Correlation%20matrix_1.png?raw=true)
-
-
+![](https://github.com/djy-git/analysis-tools/blob/main/examples/titanic/visualization/Feature%20importance_1.png?raw=true)
```

