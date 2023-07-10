# Comparing `tmp/maysics-0.5.1.tar.gz` & `tmp/maysics-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maysics-0.5.1.tar", last modified: Mon Feb 20 11:32:12 2023, max compression
+gzip compressed data, was "maysics-0.5.2.tar", last modified: Mon Jul 10 14:15:29 2023, max compression
```

## Comparing `maysics-0.5.1.tar` & `maysics-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 11:32:12.340281 maysics-0.5.1/
--rw-rw-rw-   0        0        0     1091 2022-09-14 16:32:58.000000 maysics-0.5.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2190 2023-02-20 11:32:12.339284 maysics-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1495 2023-02-20 11:29:08.000000 maysics-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-20 11:32:12.282819 maysics-0.5.1/maysics/
--rw-rw-rw-   0        0        0    17405 2023-02-20 11:29:21.000000 maysics-0.5.1/maysics/__init__.py
--rw-rw-rw-   0        0        0    22482 2022-09-10 14:53:40.000000 maysics-0.5.1/maysics/calc.py
--rw-rw-rw-   0        0        0    17698 2023-02-17 11:42:06.000000 maysics-0.5.1/maysics/digital.py
--rw-rw-rw-   0        0        0     8604 2023-02-04 13:32:02.000000 maysics-0.5.1/maysics/equa.py
--rw-rw-rw-   0        0        0    28918 2022-10-27 09:55:33.000000 maysics-0.5.1/maysics/explain.py
--rw-rw-rw-   0        0        0    11557 2022-09-10 16:29:46.000000 maysics-0.5.1/maysics/graph.py
--rw-rw-rw-   0        0        0    58694 2023-02-05 06:50:30.000000 maysics-0.5.1/maysics/models.py
--rw-rw-rw-   0        0        0    28510 2022-10-31 03:59:41.000000 maysics-0.5.1/maysics/prep.py
--rw-rw-rw-   0        0        0    22746 2022-09-11 03:50:51.000000 maysics-0.5.1/maysics/stats.py
--rw-rw-rw-   0        0        0    13920 2022-09-11 03:26:51.000000 maysics-0.5.1/maysics/time.py
--rw-rw-rw-   0        0        0     9860 2022-10-19 05:26:01.000000 maysics-0.5.1/maysics/trans.py
--rw-rw-rw-   0        0        0    13104 2022-09-22 04:50:59.000000 maysics-0.5.1/maysics/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-20 11:32:12.329467 maysics-0.5.1/maysics.egg-info/
--rw-rw-rw-   0        0        0     2190 2023-02-20 11:32:11.000000 maysics-0.5.1/maysics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-02-20 11:32:11.000000 maysics-0.5.1/maysics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 11:32:11.000000 maysics-0.5.1/maysics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-02-20 11:32:11.000000 maysics-0.5.1/maysics.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-20 11:32:11.000000 maysics-0.5.1/maysics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-20 11:32:12.341362 maysics-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2777 2023-02-20 11:27:02.000000 maysics-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:15:29.257072 maysics-0.5.2/
+-rw-rw-rw-   0        0        0     1091 2022-09-14 16:32:58.000000 maysics-0.5.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2190 2023-07-10 14:15:29.255077 maysics-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1495 2023-02-20 11:29:08.000000 maysics-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 14:15:29.190931 maysics-0.5.2/maysics/
+-rw-rw-rw-   0        0        0    17405 2023-02-20 11:29:21.000000 maysics-0.5.2/maysics/__init__.py
+-rw-rw-rw-   0        0        0    22482 2022-09-10 14:53:40.000000 maysics-0.5.2/maysics/calc.py
+-rw-rw-rw-   0        0        0    17698 2023-02-17 11:42:06.000000 maysics-0.5.2/maysics/digital.py
+-rw-rw-rw-   0        0        0     8604 2023-02-04 13:32:02.000000 maysics-0.5.2/maysics/equa.py
+-rw-rw-rw-   0        0        0    28918 2022-10-27 09:55:33.000000 maysics-0.5.2/maysics/explain.py
+-rw-rw-rw-   0        0        0    11557 2022-09-10 16:29:46.000000 maysics-0.5.2/maysics/graph.py
+-rw-rw-rw-   0        0        0    58694 2023-02-05 06:50:30.000000 maysics-0.5.2/maysics/models.py
+-rw-rw-rw-   0        0        0    28510 2022-10-31 03:59:41.000000 maysics-0.5.2/maysics/prep.py
+-rw-rw-rw-   0        0        0    22746 2022-09-11 03:50:51.000000 maysics-0.5.2/maysics/stats.py
+-rw-rw-rw-   0        0        0    13920 2022-09-11 03:26:51.000000 maysics-0.5.2/maysics/time.py
+-rw-rw-rw-   0        0        0    12797 2023-07-10 14:06:32.000000 maysics-0.5.2/maysics/trans.py
+-rw-rw-rw-   0        0        0    15781 2023-07-10 14:01:41.000000 maysics-0.5.2/maysics/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:15:29.250886 maysics-0.5.2/maysics.egg-info/
+-rw-rw-rw-   0        0        0     2190 2023-07-10 14:15:28.000000 maysics-0.5.2/maysics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-10 14:15:28.000000 maysics-0.5.2/maysics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:15:28.000000 maysics-0.5.2/maysics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-10 14:15:28.000000 maysics-0.5.2/maysics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 14:15:28.000000 maysics-0.5.2/maysics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:15:29.258068 maysics-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2777 2023-07-10 14:08:23.000000 maysics-0.5.2/setup.py
```

### Comparing `maysics-0.5.1/LICENSE.txt` & `maysics-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/PKG-INFO` & `maysics-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maysics
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework for calculating and modeling
 Home-page: https://github.com/HOKOTATE-pzw/maysics.git
 Author: HOKOTATE
 Author-email: pangzewei2010@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maysics-0.5.1/README.md` & `maysics-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/__init__.py` & `maysics-0.5.2/maysics/__init__.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/calc.py` & `maysics-0.5.2/maysics/calc.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/digital.py` & `maysics-0.5.2/maysics/digital.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/equa.py` & `maysics-0.5.2/maysics/equa.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/explain.py` & `maysics-0.5.2/maysics/explain.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/graph.py` & `maysics-0.5.2/maysics/graph.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/models.py` & `maysics-0.5.2/maysics/models.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/prep.py` & `maysics-0.5.2/maysics/prep.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/stats.py` & `maysics-0.5.2/maysics/stats.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/time.py` & `maysics-0.5.2/maysics/time.py`

 * *Files identical despite different names*

### Comparing `maysics-0.5.1/maysics/trans.py` & `maysics-0.5.2/maysics/trans.py`

 * *Files 21% similar despite different names*

```diff
@@ -130,14 +130,100 @@
         vo[:, 0] = (vo[:, 0] - v) / factor
         vo[:, 1] = vo[:, 1] * γ / factor
         vo[:, 2] = vo[:, 2] * γ / factor
     
     return vo
 
 
+def mercator(lon_lat, r=6371393, re_lon=0):
+    '''
+    墨卡托变换
+    𝑥 = 𝑅(𝜃−𝜃0)
+    𝑦 = 𝑅𝑙𝑛(𝑡𝑎𝑛(0.25𝜋+0.5𝜙))
+    
+    参数
+    ----
+    lon_lat：一维或二维数组，经度、纬度
+    r：数类型，可选，球体半径，默认为地球平均半径
+    re_lon：数类型，可选，参考经度，默认为0
+    
+    返回
+    ----
+    ndarray类型，变换后的数组
+    
+    
+    Mercator transformation
+    𝑥 = 𝑅(𝜃−𝜃0)
+    𝑦 = 𝑅𝑙𝑛(𝑡𝑎𝑛(0.25𝜋+0.5𝜙))
+    
+    Parameters
+    ----------
+    lon_lat: 1D or 2D array, longtitude and latitude
+    r: num, callable, radius of the sphere, default=the mean radius of the earth
+    re_lon: num, callable, reference longtitude, default=0
+    
+    Return
+    ------
+    ndarray, array after transformation
+    '''
+    lon_lat = np.array(lon_lat) * np.pi / 180
+    re_lon * np.pi / 180
+    if len(lon_lat.shape) == 1:
+        result = np.array([r * (lon_lat[0] - re_lon), r * np.log(np.tan(0.25 * np.pi + 0.5 * lon_lat[1]))])
+    elif len(lon_lat.shape) == 2:
+        result = np.array([r * (lon_lat[:, 0] - re_lon), r * np.log(np.tan(0.25 * np.pi + 0.5 * lon_lat[:, 1]))])
+    else:
+        raise Exception("Parameter 'lon_lat' must be 1-D or 2-D.")
+    
+    return result
+
+
+def imercator(x_y, r=6371393, re_lon=0):
+    '''
+    墨卡托逆变换
+    𝜃 = 𝑥/𝑅 + 𝜃0
+    𝜙 = 2𝑎𝑟𝑐𝑡𝑎𝑛(𝑒^(𝑦/𝑅)) − 0.5𝜋
+    
+    参数
+    ----
+    x_y: 一维或二维数组，坐标
+    r：数类型，可选，球体半径，默认为地球平均半径
+    re_lon：数类型，可选，参考经度，默认为0
+    
+    
+    返回
+    ----
+    ndarray类型，变换后的数组
+    
+    
+    Mercator inverse transformation
+    𝜃 = 𝑥/𝑅+𝜃0
+    𝜙 = 2𝑎𝑟𝑐𝑡𝑎𝑛(𝑒^(𝑦/𝑅))−0.5𝜋
+    
+    Parameters
+    ----------
+    x_y: 1D or 2D array, location
+    r: num, callable, radius of the sphere, default=the mean radius of the earth
+    re_lon: num, callable, reference longtitude, default=0
+    
+    Return
+    ------
+    ndarray, array after transformation
+    '''
+    x_y = np.array(x_y)
+    if len(x_y.shape) == 1:
+        result = [(x_y[0] / r) * 180 / np.pi + re_lon, (np.arctan(np.e**(x_y[1] / r)) - 0.25 * np.pi) * 360 / np.pi]
+    elif len(x_y.shape) == 2:
+        result = [(x_y[:, 0] / r) * 180 / np.pi + re_lon, (np.arctan(np.e**(x_y[:, 1] / r)) - 0.25 * np.pi) * 360 / np.pi]
+    else:
+        raise Exception("Parameter 'x_y' must be 1-D or 2-D.")
+    
+    return np.array(result)
+
+
 def polar(x):
     '''
     极坐标或柱坐标正变换
     
     参数
     ----
     x：一维或二维列表，(x, y)或(x, y, z)
@@ -339,27 +425,31 @@
     return x
 
 
 def rotate(theta, x):
     '''
     平面直角坐标系的旋转变换
     逆时针旋转时theta为正，顺时针旋转时theta为负
+    𝑥 = 𝑐𝑜𝑠(𝜃)𝑥 + 𝑠𝑖𝑛(𝜃)𝑦
+    𝑦 = 𝑐𝑜𝑠(𝜃)𝑥 − 𝑠𝑖𝑛(𝜃)𝑦
     
     参数
     ----
     x：一维或二维列表，(x, y)
     theta：浮点数类型，坐标系绕原点逆时针旋转的角度
     
     返回
     ----
     ndarray，转换后的坐标
     
     
     Rotation transformation of plane rectangular coordinate system
     'theta' is positive when rotating anticlockwise and negative when rotating clockwise
+    𝑥 = 𝑐𝑜𝑠(𝜃)𝑥 + 𝑠𝑖𝑛(𝜃)𝑦
+    𝑦 = 𝑐𝑜𝑠(𝜃)𝑥 − 𝑠𝑖𝑛(𝜃)𝑦
     
     Parameter
     ---------
     x: 1-D or 2-D list, (x, y)
     theta: float, the angle that the coordinate system rotates counterclockwise about the origin
     
     Return
```

### Comparing `maysics-0.5.1/maysics/utils.py` & `maysics-0.5.2/maysics/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -215,14 +215,94 @@
     data = (data - des)**2
     result = data.sum(axis=len(data.shape)-1)
     result = result**0.5
     
     return result
 
 
+def earth_distance(lon_lat_1, lon_lat_2):
+    '''
+    求某地球表面上两个点之间的距离
+    𝑑 = 𝑅𝑐𝑜𝑠𝜙1𝑐𝑜𝑠𝜙2𝑐𝑜𝑠(𝜃1−𝜃2)+𝑠𝑖𝑛𝜃1𝑠𝑖𝑛𝜃2
+    
+    参数
+    ----
+    lon_lat_1：一维数组，第一个点的经度、纬度
+    lon_lat_2：一维数组，第二个点的经度、纬度
+    
+    返回
+    ---
+    浮点数类型，距离
+    
+    
+    Calculate the distance between two points on the surface of the earth
+    𝑑 = 𝑅𝑐𝑜𝑠𝜙1𝑐𝑜𝑠𝜙2𝑐𝑜𝑠(𝜃1−𝜃2)+𝑠𝑖𝑛𝜃1𝑠𝑖𝑛𝜃2
+    
+    Parameters
+    ----------
+    lon_lat_1: 1-D array, the longitude and the latitude of the first point
+    lon_lat_2: 1-D array, the longitude and the latitude of the second point
+    
+    Return
+    ------
+    float, the distance
+    '''
+    lon_lat_1 = np.array(lon_lat_1) * np.pi / 180
+    lon_lat_2 = np.array(lon_lat_2) * np.pi / 180
+    result = np.cos(lon_lat_1[1]) * np.cos(lon_lat_2[1]) * np.cos(lon_lat_1[0] - lon_lat_2[0])
+    result += np.sin(lon_lat_1[1]) * np.sin(lon_lat_2[1])
+    result = 6371393 * np.arccos(result)
+    
+    return result
+
+
+def earth_distances(lon_lat, des):
+    '''
+    求地球表面点lon_lat到目标点des的距离距离
+    𝑑 = 𝑅𝑐𝑜𝑠𝜙1𝑐𝑜𝑠𝜙2𝑐𝑜𝑠(𝜃1−𝜃2)+𝑠𝑖𝑛𝜃1𝑠𝑖𝑛𝜃2
+    
+    参数
+    ----
+    lon_lat：一维或二维数组，经度、纬度
+    des：一维数组，目标点经度、纬度
+    
+    返回
+    ----
+    ndarray类型，距离数组
+    
+    
+    Calculate the distances between lon_lat and destination on the surface of the earth
+    𝑑 = 𝑅𝑐𝑜𝑠𝜙1𝑐𝑜𝑠𝜙2𝑐𝑜𝑠(𝜃1−𝜃2)+𝑠𝑖𝑛𝜃1𝑠𝑖𝑛𝜃2
+    
+    Parameter
+    ---------
+    lon_lat: 1-D or 2-D array, the longitude and the latitude
+    des: 1-D array, the longitude and the latitude of destination
+    
+    Return
+    ------
+    ndarray, the distances
+    '''
+    lon_lat = np.array(lon_lat) * np.pi / 180
+    des = np.array(des) * np.pi / 180
+    
+    if len(lon_lat.shape) == 2:
+        result = np.cos(lon_lat[:, 1]) * np.cos(des[1]) * np.cos(lon_lat[:, 0] - des[0])
+        result += np.sin(lon_lat[:, 1]) * np.sin(des[1])
+    elif len(lon_lat.shape) == 1:
+        result = np.cos(lon_lat[1]) * np.cos(des[1]) * np.cos(lon_lat[0] - des[0])
+        result += np.sin(lon_lat[1]) * np.sin(des[1])
+    else:
+        raise Exception("Parameter 'lon_lat' must be 1-D or 2-D.")
+    
+    result = 6371393 * np.arccos(result)
+    
+    return result
+
+
 def m_distance(data, p1, p2):
     '''
     求某两个点之间的马氏距离
     
     参数
     ----
     data：二维列表，数据
```

### Comparing `maysics-0.5.1/maysics.egg-info/PKG-INFO` & `maysics-0.5.2/maysics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maysics
-Version: 0.5.1
+Version: 0.5.2
 Summary: A framework for calculating and modeling
 Home-page: https://github.com/HOKOTATE-pzw/maysics.git
 Author: HOKOTATE
 Author-email: pangzewei2010@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maysics-0.5.1/setup.py` & `maysics-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 NAME = 'maysics'
 DESCRIPTION = 'A framework for calculating and modeling'
 URL = 'https://github.com/HOKOTATE-pzw/maysics.git'
 EMAIL = 'pangzewei2010@foxmail.com'
 AUTHOR = 'HOKOTATE'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 REQUIRED = [
      'matplotlib', 'numpy', 'scipy >= 1.3.0', 'lxml',
 ]
 EXTRAS = {}
 
 here = os.path.abspath(os.path.dirname(__file__))
```

