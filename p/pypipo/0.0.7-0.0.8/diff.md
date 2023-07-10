# Comparing `tmp/pypipo-0.0.7.tar.gz` & `tmp/pypipo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipo-0.0.7.tar", last modified: Thu Jul  6 15:13:32 2023, max compression
+gzip compressed data, was "pypipo-0.0.8.tar", last modified: Mon Jul 10 14:08:52 2023, max compression
```

## Comparing `pypipo-0.0.7.tar` & `pypipo-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:13:32.037137 pypipo-0.0.7/
--rw-rw-rw-   0        0        0     1086 2023-07-02 15:53:33.000000 pypipo-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       56 2023-07-02 13:22:50.000000 pypipo-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2975 2023-07-06 15:13:32.037137 pypipo-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-07-02 15:53:33.000000 pypipo-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 15:13:32.005129 pypipo-0.0.7/pypipo/
--rw-rw-rw-   0        0        0       25 2023-06-27 16:40:52.000000 pypipo-0.0.7/pypipo/__init__.py
--rw-rw-rw-   0        0        0      188 2023-06-27 16:44:32.000000 pypipo-0.0.7/pypipo/__main__.py
--rw-rw-rw-   0        0        0      745 2023-07-06 15:11:21.000000 pypipo-0.0.7/pypipo/__version__.py
--rw-rw-rw-   0        0        0     1916 2023-07-02 15:54:24.000000 pypipo-0.0.7/pypipo/cli.py
--rw-rw-rw-   0        0        0      895 2023-07-02 15:56:31.000000 pypipo-0.0.7/pypipo/convert.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:13:32.036137 pypipo-0.0.7/pypipo/libs/
--rw-rw-rw-   0        0        0        0 2023-04-19 15:21:48.000000 pypipo-0.0.7/pypipo/libs/__init__.py
--rw-rw-rw-   0        0        0    21149 2023-07-03 14:52:34.000000 pypipo-0.0.7/pypipo/libs/process.py
--rw-rw-rw-   0        0        0     1529 2023-07-01 05:38:02.000000 pypipo-0.0.7/pypipo/libs/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:13:32.022133 pypipo-0.0.7/pypipo.egg-info/
--rw-rw-rw-   0        0        0     2975 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 15:13:31.000000 pypipo-0.0.7/pypipo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-06 15:13:32.039137 pypipo-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-07-02 15:54:18.000000 pypipo-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:08:52.325334 pypipo-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-07-02 15:53:33.000000 pypipo-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-07-02 13:22:50.000000 pypipo-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3048 2023-07-10 14:08:52.326334 pypipo-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-07-08 08:46:34.000000 pypipo-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 14:08:52.309331 pypipo-0.0.8/pypipo/
+-rw-rw-rw-   0        0        0       25 2023-07-08 09:35:35.000000 pypipo-0.0.8/pypipo/__init__.py
+-rw-rw-rw-   0        0        0      188 2023-06-27 16:44:32.000000 pypipo-0.0.8/pypipo/__main__.py
+-rw-rw-rw-   0        0        0      745 2023-07-10 14:08:01.000000 pypipo-0.0.8/pypipo/__version__.py
+-rw-rw-rw-   0        0        0     1916 2023-07-08 09:25:01.000000 pypipo-0.0.8/pypipo/cli.py
+-rw-rw-rw-   0        0        0      895 2023-07-06 15:15:28.000000 pypipo-0.0.8/pypipo/convert.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:08:52.325334 pypipo-0.0.8/pypipo/libs/
+-rw-rw-rw-   0        0        0        0 2023-04-19 15:21:48.000000 pypipo-0.0.8/pypipo/libs/__init__.py
+-rw-rw-rw-   0        0        0    21151 2023-07-08 08:46:26.000000 pypipo-0.0.8/pypipo/libs/process.py
+-rw-rw-rw-   0        0        0     1529 2023-07-01 05:38:02.000000 pypipo-0.0.8/pypipo/libs/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:08:52.322332 pypipo-0.0.8/pypipo.egg-info/
+-rw-rw-rw-   0        0        0     3048 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-10 14:08:52.000000 pypipo-0.0.8/pypipo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-10 14:08:52.329335 pypipo-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1802 2023-07-10 14:07:47.000000 pypipo-0.0.8/setup.py
```

### Comparing `pypipo-0.0.7/LICENSE` & `pypipo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypipo-0.0.7/PKG-INFO` & `pypipo-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pypipo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Image convert to PIPO painting canvas automatically.
 Home-page: https://github.com/AutoPipo/pypipo/
 Author: ('Minku-Koo', 'Jiyong-Park')
 Author-email: corleone@kakao.com
 License: MIT License
+Keywords: pipo painting,image painting,image processing,computer vision
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="right">
 <a href="https://hits.seeyoufarm.com" ><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAutoPipo%2Fpypipo&count_bg=%23AF7EE5&title_bg=%23312D2D&icon=&icon_color=%23E39999&title=visitors&edge_flat=true"/></a>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: pypipo Version: 0.0.7 Summary: Image convert to
+Metadata-Version: 2.1 Name: pypipo Version: 0.0.8 Summary: Image convert to
 PIPO painting canvas automatically. Home-page: https://github.com/AutoPipo/
 pypipo/ Author: ('Minku-Koo', 'Jiyong-Park') Author-email: corleone@kakao.com
-License: MIT License Classifier: Programming Language :: Python :: 3.6
+License: MIT License Keywords: pipo painting,image painting,image
+processing,computer vision Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
                                    [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FAutoPipo%2Fpypipo&count_bg=%23AF7EE5&title_bg=%23312D2D&icon=&icon_color=%23E39999&title=visitors&edge_flat=true]
      [https://github.com/AutoPipo/pypipo/raw/main/pypipo/sample/logo.png]
 
 # pypipo ### Python library to convert PIPO Painting canvas image
```

### Comparing `pypipo-0.0.7/README.md` & `pypipo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pypipo-0.0.7/pypipo/__version__.py` & `pypipo-0.0.8/pypipo/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = (0, 0, 7)
+VERSION = (0, 0, 8)
 PRERELEASE = None  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
     if prerelease is not None:
```

### Comparing `pypipo-0.0.7/pypipo/cli.py` & `pypipo-0.0.8/pypipo/cli.py`

 * *Files identical despite different names*

### Comparing `pypipo-0.0.7/pypipo/convert.py` & `pypipo-0.0.8/pypipo/convert.py`

 * *Files identical despite different names*

### Comparing `pypipo-0.0.7/pypipo/libs/process.py` & `pypipo-0.0.8/pypipo/libs/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         color_index_map = labels.reshape((height, width))
 
         centers = np.uint8(centers)
         res = centers[labels.flatten()]
         self.clustered_colors = centers
 
         # for returns
-        sse = round(sse ** 0.5 // 10, 2)
+        # sse = round(sse ** 0.5 // 10, 2)
         color_clustered_image = res.reshape((image.shape))
         return color_clustered_image, color_index_map
    
     def __expand_image(self, image, target_size):
         """Expand image size
 
         Parameters
```

### Comparing `pypipo-0.0.7/pypipo/libs/utils.py` & `pypipo-0.0.8/pypipo/libs/utils.py`

 * *Files identical despite different names*

### Comparing `pypipo-0.0.7/pypipo.egg-info/PKG-INFO` & `pypipo-0.0.8/pypipo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pypipo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Image convert to PIPO painting canvas automatically.
 Home-page: https://github.com/AutoPipo/pypipo/
 Author: ('Minku-Koo', 'Jiyong-Park')
 Author-email: corleone@kakao.com
 License: MIT License
+Keywords: pipo painting,image painting,image processing,computer vision
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="right">
 <a href="https://hits.seeyoufarm.com" ><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FAutoPipo%2Fpypipo&count_bg=%23AF7EE5&title_bg=%23312D2D&icon=&icon_color=%23E39999&title=visitors&edge_flat=true"/></a>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: pypipo Version: 0.0.7 Summary: Image convert to
+Metadata-Version: 2.1 Name: pypipo Version: 0.0.8 Summary: Image convert to
 PIPO painting canvas automatically. Home-page: https://github.com/AutoPipo/
 pypipo/ Author: ('Minku-Koo', 'Jiyong-Park') Author-email: corleone@kakao.com
-License: MIT License Classifier: Programming Language :: Python :: 3.6
+License: MIT License Keywords: pipo painting,image painting,image
+processing,computer vision Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
 text/markdown License-File: LICENSE
                                    [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FAutoPipo%2Fpypipo&count_bg=%23AF7EE5&title_bg=%23312D2D&icon=&icon_color=%23E39999&title=visitors&edge_flat=true]
      [https://github.com/AutoPipo/pypipo/raw/main/pypipo/sample/logo.png]
 
 # pypipo ### Python library to convert PIPO Painting canvas image
```

### Comparing `pypipo-0.0.7/setup.py` & `pypipo-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                     description=about['__description__'],
                     long_description=readme,
                     long_description_content_type="text/markdown",
                     url=about['__url__'],
                     author=about['__author__'],
                     author_email=about['__author_email__'],
                     license=about['__license__'],
+                    keywords=['pipo painting', 'image painting', 'image processing', 'computer vision'],
                     packages=find_packages(exclude=('sample',)),
                     install_requires=requires,
                     entry_points={
                         'console_scripts': [
                             'camelot = camelot.cli:cli',
                         ],
                     },
```

