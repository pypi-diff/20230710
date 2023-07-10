# Comparing `tmp/hds-stats-0.3.3.tar.gz` & `tmp/hds-stats-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.3.tar", last modified: Mon Jul 10 06:40:04 2023, max compression
+gzip compressed data, was "hds-stats-0.3.4.tar", last modified: Mon Jul 10 06:51:08 2023, max compression
```

## Comparing `hds-stats-0.3.3.tar` & `hds-stats-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.166552 hds-stats-0.3.3/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.3/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:40:04.166293 hds-stats-0.3.3/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.3/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.162988 hds-stats-0.3.3/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.3/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9586 2023-07-10 06:25:27.000000 hds-stats-0.3.3/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11955 2023-06-18 16:25:20.000000 hds-stats-0.3.3/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27424 2023-07-10 06:38:52.000000 hds-stats-0.3.3/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:40:04.165885 hds-stats-0.3.3/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:40:04.000000 hds-stats-0.3.3/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.3/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:40:04.166650 hds-stats-0.3.3/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:39:02.000000 hds-stats-0.3.3/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.892924 hds-stats-0.3.4/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.4/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:51:08.892676 hds-stats-0.3.4/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.4/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.890733 hds-stats-0.3.4/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.4/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.4/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.4/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27181 2023-07-10 06:46:42.000000 hds-stats-0.3.4/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-10 06:51:08.892312 hds-stats-0.3.4/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-10 06:51:08.000000 hds-stats-0.3.4/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.4/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-10 06:51:08.893016 hds-stats-0.3.4/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-10 06:50:53.000000 hds-stats-0.3.4/setup.py
```

### Comparing `hds-stats-0.3.3/LICENSE` & `hds-stats-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.3/PKG-INFO` & `hds-stats-0.3.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.3
+Version: 0.3.4
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.3/hds_stats/ml.py` & `hds-stats-0.3.4/hds_stats/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,15 @@
             ha = 'left', 
             va = 'center'
         )
     
     plt.xlim(0, imp['Imp'].max() * 1.2)
     plt.title(label = 'Feature Importances')
     plt.xlabel(xlabel = 'Feature Importances')
-    plt.ylabel(ylabel = 'Feature')
-    plt.show()
+    plt.ylabel(ylabel = 'Feature');
 
 
 # 나무모형 가지치기 단계 그래프 시각화
 def plot_step(data, x = 'alpha', y = 'impurity', color = 'blue', xangle = None):
     '''
     이 함수는 나무모형 가지치기 결과로 단계 그래프를 그립니다.
     
@@ -144,16 +143,15 @@
         data = data, 
         x = x, 
         y = y, 
         color = color, 
         s = 15
     )
     
-    plt.xticks(rotation = xangle)
-    plt.show()
+    plt.xticks(rotation = xangle);
 
 
 # 주성분 분석 스크리 도표 시각화
 def plot_screeplot(x):
     '''
     이 함수는 주성분 점수 행렬로 스크리 도표를 그립니다.
     
@@ -184,16 +182,15 @@
         color = 'red', 
         linestyle = '--'
     )
     
     plt.xticks(ticks = xticks)
     plt.title(label = 'Scree Plot')
     plt.xlabel(xlabel = 'Number of PC')
-    plt.ylabel(ylabel = 'Variance')
-    plt.show()
+    plt.ylabel(ylabel = 'Variance');
     
 
 # 주성분 분석 행렬도 시각화
 def plot_biplot(score, coefs, x = 1, y = 2, zoom = 1):
     '''
     이 함수는 주성분 분석 결과를 받아 스크리 도표를 그립니다.
     
@@ -256,18 +253,17 @@
             va = 'center', 
             fontsize = 8
         )
     
     # plt.xlim(-1, 1)
     # plt.ylim(-1, 1)
     # plt.grid()
-    plt.title(label = 'Biplot')
+    plt.title(label = 'Biplot with PC1 and PC2')
     plt.xlabel(xlabel = 'PC{}'.format(x))
-    plt.ylabel(ylabel = 'PC{}'.format(y))
-    plt.show()
+    plt.ylabel(ylabel = 'PC{}'.format(y));
 
 
 # k-평균 군집분석 WSS 단계 그래프 시각화
 def plot_wcss(X, k = 3):
     '''
     이 함수는 군집별 편차 제곱합으로 선 그래프를 그립니다.
     
@@ -291,16 +287,15 @@
         wcss = model.inertia_
         result.append(wcss)
     
     sns.lineplot(x = ks, y = result, marker = 'o')
     plt.xticks(ticks = ks)
     plt.title(label = 'Elbow Method')
     plt.xlabel(xlabel = 'Number of clusters')
-    plt.ylabel(ylabel = 'Within Cluster Sum of Squares')
-    plt.show()
+    plt.ylabel(ylabel = 'Within Cluster Sum of Squares');
 
 
 # k-평균 군집분석 실루엣 지수 시각화
 def plot_silhouette(X, k = 3):
     '''
     이 함수는 군집별 실루엣 지수로 선 그래프를 그립니다.
     
@@ -327,12 +322,11 @@
         silwidth = silhouette_score(X = X, labels = cluster)
         result.append(silwidth)
     
     sns.lineplot(x = ks, y = result, marker = 'o')
     plt.xticks(ticks = ks)
     plt.title(label = 'Silhouette Width')
     plt.xlabel(xlabel = 'Number of clusters')
-    plt.ylabel(ylabel = 'Silhouette Width Average')
-    plt.show()
+    plt.ylabel(ylabel = 'Silhouette Width Average');
 
 
 ## End of Document
```

### Comparing `hds-stats-0.3.3/hds_stats/plot.py` & `hds-stats-0.3.4/hds_stats/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,15 @@
     
     plt.axhline(
         y = data[y].mean(), 
         color = 'red', 
         linestyle = '--'
     )
     
-    plt.title(label = f'{x} 범주별 {y}의 평균 비교')
-    plt.show()
+    plt.title(label = f'{x} 범주별 {y}의 평균 비교');
 
 
 # 두 연속형 변수로 산점도를 그리는 함수
 def scatter(data, x: str, y: str, color: str = '0.3') -> None:
     '''
     이 함수는 두 연속형 변수의 산점도를 그립니다.
     
@@ -80,16 +79,15 @@
     sns.scatterplot(
         data = data, 
         x = x, 
         y = y, 
         color = color
     )
     
-    plt.title(label = f'{x}와(과) {y}의 관계')
-    plt.show()
+    plt.title(label = f'{x}와(과) {y}의 관계');
 
 
 # 두 연속형 변수로 산점도와 회귀직선을 그리는 함수
 def regline(data, x: str, y: str, color: str = '0.3', size: int = 15) -> None:
     '''
     이 함수는 두 연속형 변수의 산점도에 회귀직선을 그립니다.
     
@@ -125,16 +123,15 @@
             'linewidth': 1.5
         }
     )
     
     # x_min = data[x].min()
     # x_max = data[x].max()
     # plt.xlim(x_min * 0.9, x_max * 1.1)
-    plt.title(label = f'{x}와(과) {y}의 관계')
-    plt.show()
+    plt.title(label = f'{x}와(과) {y}의 관계');
 
 
 # 범주형 변수의 빈도수로 막대 그래프를 그리는 함수
 def bar_freq(data, x: str, color: str = None, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수의 빈도수를 내림차순 정렬한 막대 그래프를 그립니다.
     
@@ -172,16 +169,15 @@
             s = v, 
             ha = 'center', 
             va = 'bottom', 
             c = 'black'
         )
     
     plt.ylim(0, v_max * 1.2)
-    plt.title(label = '목표변수의 범주별 빈도수 비교')
-    plt.show()
+    plt.title(label = '목표변수의 범주별 빈도수 비교');
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그리는 함수
 def bar_dodge_freq(data, x: str, group: str, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 펼친 막대 그래프를 그립니다.
     
@@ -224,16 +220,15 @@
             s = v, 
             ha = 'center', 
             va = 'bottom'
         )
     
     plt.ylim(0, v_max * 1.2)
     plt.title(label = f'{x}의 범주별 {group}의 빈도수 비교')
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
-    plt.show();
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
 
 
 # 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_freq(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 빈도수로 쌓은 막대 그래프를 그립니다.
     
@@ -301,16 +296,15 @@
                     y = i, 
                     s = v2, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black'
                 )
 
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
-    plt.show()
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
 
 
 # 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그리는 함수
 def bar_stack_prop(data, x: str, group: str, kind: str = 'bar', pal: list = None) -> None:
     '''
     이 함수는 범주형 변수를 소그룹으로 나누고 상대도수로 쌓은 막대 그래프를 그립니다.
     
@@ -383,12 +377,11 @@
                     y = i, 
                     s = v3, 
                     ha = 'center', 
                     va = 'center', 
                     c = 'black'
                 )
     
-    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5))
-    plt.show()
+    plt.legend(loc = 'center left', bbox_to_anchor = (1, 0.5));
 
 
 ## End of Document
```

### Comparing `hds-stats-0.3.3/hds_stats/stat.py` & `hds-stats-0.3.4/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,16 +350,15 @@
         results = model, 
         criterion = 'cooks', 
         size = 24, 
         plot_alpha = 0.2, 
         ax = ax4
     )
     
-    plt.tight_layout()
-    plt.show()
+    plt.tight_layout();
 
 
 # 쿡의 거리
 def cooks_distance(model):
     '''
     이 함수는 다중선형 회귀모형의 훈련셋으로 관측값별 쿡의 거리를 계산합니다.
     
@@ -934,27 +933,14 @@
         color = 'red'
     )
     
     # Add tangent line
     optX = opt['FPR'].iloc[0]
     optY = opt['TPR'].iloc[0]
     
-    # x1 = optX - 0.1
-    # y1 = optY - 0.1
-    # x2 = optX + 0.1
-    # y2 = optY + 0.1
-    # 
-    # plt.plot(
-    #     [x1, x2],
-    #     [y1, y2],
-    #     color = 'red',
-    #     lw = 0.5,
-    #     ls = '-.'
-    # )
-    
     b = optY - optX
     plt.plot(
         [0, 1-b], 
         [b, 1], 
         color = 'red', 
         lw = 0.5, 
         ls = '-.'
```

### Comparing `hds-stats-0.3.3/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.4/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.3
+Version: 0.3.4
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.3/setup.py` & `hds-stats-0.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.3',
+    version = '0.3.4',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

