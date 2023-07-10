# Comparing `tmp/hds-stats-0.3.1.tar.gz` & `tmp/hds-stats-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.1.tar", last modified: Mon Jul 10 06:14:46 2023, max compression
+gzip compressed data, was "hds-stats-0.3.2.tar", last modified: Mon Jul 10 06:26:14 2023, max compression
```

## Comparing `hds-stats-0.3.1.tar` & `hds-stats-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.273087 hds-stats-0.3.1/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.1/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:14:46.272845 hds-stats-0.3.1/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.1/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.270937 hds-stats-0.3.1/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.1/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9625 2023-07-10 05:27:45.000000 hds-stats-0.3.1/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.1/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.1/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:14:46.272472 hds-stats-0.3.1/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:14:46.000000 hds-stats-0.3.1/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.1/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:14:46.273176 hds-stats-0.3.1/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:13:22.000000 hds-stats-0.3.1/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.970065 hds-stats-0.3.2/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.2/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:26:14.969794 hds-stats-0.3.2/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.2/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.967868 hds-stats-0.3.2/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.2/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9586 2023-07-10 06:25:27.000000 hds-stats-0.3.2/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.2/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27195 2023-06-18 16:48:47.000000 hds-stats-0.3.2/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:26:14.969405 hds-stats-0.3.2/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:26:14.000000 hds-stats-0.3.2/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.2/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:26:14.970178 hds-stats-0.3.2/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:25:39.000000 hds-stats-0.3.2/setup.py
```

### Comparing `hds-stats-0.3.1/LICENSE` & `hds-stats-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.1/PKG-INFO` & `hds-stats-0.3.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.1
+Version: 0.3.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.1/hds_stats/ml.py` & `hds-stats-0.3.2/hds_stats/ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,7 @@
-# 분류모형의 입력변수별 중요도로 막대 그래프 시각화
-def plot_feature_importance(model, pal = 'Spectral'):
-    '''
-    이 함수는 분류모형의 입력변수별 중요도로 막대 그래프를 그립니다.
-    
-    매개변수:
-        model: 사이킷런으로 적합한 분류모형을 지정합니다.
-        pal: 팔레트를 문자열로 지정합니다.(기본값: Spectral)
-    
-    반환값:
-        그래프 외에 반환하는 객체는 없습니다.
-    '''
-    
-    import pandas as pd
-    import seaborn as sns
-    import matplotlib.pyplot as plt
-    
-    if 'LGBM' in str(type(model)):
-        imp = pd.DataFrame(
-            data = model.feature_importances_, 
-            index = model.feature_name_, 
-            columns = ['Imp']
-        )
-    else:
-        imp = pd.DataFrame(
-            data = model.feature_importances_, 
-            index = model.feature_names_in_, 
-            columns = ['Imp']
-        )
-    
-    imp = imp.sort_values(by = 'Imp', ascending = False)
-    imp = imp.reset_index()
-    
-    sns.barplot(
-        data = imp, 
-        x = 'Imp', 
-        y = 'index', 
-        palette = pal
-    )
-    
-    for index, row in imp.iterrows():
-        plt.text(
-            x = row['Imp'], 
-            y = index, 
-            s = np.round(row['Imp'], 3), 
-            ha = 'left', 
-            va = 'center'
-        )
-    
-    plt.xlim(0, imp['Imp'].max() * 1.2)
-    plt.title(label = 'Feature Importances')
-    plt.xlabel(xlabel = 'Feature Importances')
-    plt.ylabel(ylabel = 'Feature')
-    plt.show()
-
-
 # 나무모형 시각화
 def plot_tree(model, fileName = None, className = None):
     '''
     이 함수는 나무모형을 그립니다.
     
     매개변수:
         model: 사이킷런으로 적합한 나무모형을 지정합니다.
@@ -107,15 +51,72 @@
         graph = graphviz.Source(source = graph, format = 'png')
         graph.render(filename = fileName)
     
     os.remove(f'{fileName}')
     os.remove(f'{fileName}.dot')
 
 
-# 나무모형 가지치기 결과로 단계 그래프 시각화
+# 입력변수별 중요도 시각화
+def plot_feature_importance(model, pal = 'Spectral'):
+    '''
+    이 함수는 입력변수별 중요도로 막대 그래프를 그립니다.
+    
+    매개변수:
+        model: 사이킷런으로 적합한 분류모형을 지정합니다.
+        pal: 팔레트를 문자열로 지정합니다.(기본값: Spectral)
+    
+    반환값:
+        그래프 외에 반환하는 객체는 없습니다.
+    '''
+    
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    
+    if 'LGBM' in str(type(model)):
+        imp = pd.DataFrame(
+            data = model.feature_importances_, 
+            index = model.feature_name_, 
+            columns = ['Imp']
+        )
+    else:
+        imp = pd.DataFrame(
+            data = model.feature_importances_, 
+            index = model.feature_names_in_, 
+            columns = ['Imp']
+        )
+    
+    imp = imp.sort_values(by = 'Imp', ascending = False)
+    imp = imp.reset_index()
+    
+    sns.barplot(
+        data = imp, 
+        x = 'Imp', 
+        y = 'index', 
+        palette = pal
+    )
+    
+    for index, row in imp.iterrows():
+        plt.text(
+            x = row['Imp'], 
+            y = index, 
+            s = np.round(row['Imp'], 3), 
+            ha = 'left', 
+            va = 'center'
+        )
+    
+    plt.xlim(0, imp['Imp'].max() * 1.2)
+    plt.title(label = 'Feature Importances')
+    plt.xlabel(xlabel = 'Feature Importances')
+    plt.ylabel(ylabel = 'Feature')
+    plt.show()
+
+
+# 나무모형 가지치기 단계 그래프 시각화
 def plot_step(data, x = 'alpha', y = 'impurity', color = 'blue', xangle = None):
     '''
     이 함수는 나무모형 가지치기 결과로 단계 그래프를 그립니다.
     
     매개변수:
         data: 나무모형의 가지치기 단계별 비용 복잡도 파라미터를 데이터프레임으로 지정합니다.
         x: x축에 지정할 변수명을 지정합니다.(기본값: alpha)
```

### Comparing `hds-stats-0.3.1/hds_stats/plot.py` & `hds-stats-0.3.2/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.1/hds_stats/stat.py` & `hds-stats-0.3.2/hds_stats/stat.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.1/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.2/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.1
+Version: 0.3.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.1/setup.py` & `hds-stats-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.1',
+    version = '0.3.2',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

