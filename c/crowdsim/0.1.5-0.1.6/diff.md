# Comparing `tmp/crowdsim-0.1.5.tar.gz` & `tmp/crowdsim-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdsim-0.1.5.tar", last modified: Mon Jul 10 07:33:51 2023, max compression
+gzip compressed data, was "crowdsim-0.1.6.tar", last modified: Mon Jul 10 07:47:26 2023, max compression
```

## Comparing `crowdsim-0.1.5.tar` & `crowdsim-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.978405 crowdsim-0.1.5/
--rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      238 2023-07-10 07:33:51.978405 crowdsim-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.966713 crowdsim-0.1.5/crowdsim/
--rw-rw-rw-   0        0        0     2700 2023-04-21 11:23:00.000000 crowdsim-0.1.5/crowdsim/Ui_enter_window.py
--rw-rw-rw-   0        0        0      275 2023-07-10 07:30:57.000000 crowdsim-0.1.5/crowdsim/__init__.py
--rw-rw-rw-   0        0        0    21088 2023-07-10 06:34:21.000000 crowdsim-0.1.5/crowdsim/config.py
--rw-rw-rw-   0        0        0    29976 2023-07-10 06:35:06.000000 crowdsim-0.1.5/crowdsim/orca_people.py
--rw-rw-rw-   0        0        0     3155 2023-04-10 05:28:36.000000 crowdsim-0.1.5/crowdsim/orca_scene.py
--rw-rw-rw-   0        0        0     8132 2023-04-21 11:23:00.000000 crowdsim-0.1.5/crowdsim/pre_astar.py
--rw-rw-rw-   0        0        0    25758 2023-05-23 10:01:14.000000 crowdsim-0.1.5/crowdsim/sf_people.py
--rw-rw-rw-   0        0        0     5472 2023-05-15 14:38:52.000000 crowdsim-0.1.5/crowdsim/sf_scene.py
--rw-rw-rw-   0        0        0    22596 2023-05-23 10:03:00.000000 crowdsim-0.1.5/crowdsim/steer_people.py
--rw-rw-rw-   0        0        0     5474 2023-05-02 08:45:23.000000 crowdsim-0.1.5/crowdsim/steer_scene.py
--rw-rw-rw-   0        0        0     3299 2023-07-10 03:28:56.000000 crowdsim-0.1.5/crowdsim/test.py
--rw-rw-rw-   0        0        0     3721 2023-07-10 06:33:11.000000 crowdsim-0.1.5/crowdsim/utils.py
--rw-rw-rw-   0        0        0    11994 2023-07-10 07:14:51.000000 crowdsim-0.1.5/crowdsim/window_control.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.977406 crowdsim-0.1.5/crowdsim.egg-info/
--rw-rw-rw-   0        0        0      238 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:33:51.978405 crowdsim-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-07-10 07:33:47.000000 crowdsim-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:47:26.370576 crowdsim-0.1.6/
+-rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:47:26.370576 crowdsim-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 07:47:26.353249 crowdsim-0.1.6/crowdsim/
+-rw-rw-rw-   0        0        0     2700 2023-07-10 07:34:34.000000 crowdsim-0.1.6/crowdsim/Ui_enter_window.py
+-rw-rw-rw-   0        0        0      562 2023-07-10 07:44:13.000000 crowdsim-0.1.6/crowdsim/__init__.py
+-rw-rw-rw-   0        0        0    21097 2023-07-10 07:38:30.000000 crowdsim-0.1.6/crowdsim/config.py
+-rw-rw-rw-   0        0        0    29999 2023-07-10 07:45:55.000000 crowdsim-0.1.6/crowdsim/orca_people.py
+-rw-rw-rw-   0        0        0     3169 2023-07-10 07:41:44.000000 crowdsim-0.1.6/crowdsim/orca_scene.py
+-rw-rw-rw-   0        0        0     8146 2023-07-10 07:45:51.000000 crowdsim-0.1.6/crowdsim/pre_astar.py
+-rw-rw-rw-   0        0        0    25790 2023-07-10 07:46:03.000000 crowdsim-0.1.6/crowdsim/sf_people.py
+-rw-rw-rw-   0        0        0     5486 2023-07-10 07:45:48.000000 crowdsim-0.1.6/crowdsim/sf_scene.py
+-rw-rw-rw-   0        0        0    22628 2023-07-10 07:46:15.000000 crowdsim-0.1.6/crowdsim/steer_people.py
+-rw-rw-rw-   0        0        0     5488 2023-07-10 07:46:17.000000 crowdsim-0.1.6/crowdsim/steer_scene.py
+-rw-rw-rw-   0        0        0     3299 2023-07-10 07:34:34.000000 crowdsim-0.1.6/crowdsim/test.py
+-rw-rw-rw-   0        0        0     3721 2023-07-10 07:34:34.000000 crowdsim-0.1.6/crowdsim/utils.py
+-rw-rw-rw-   0        0        0    12053 2023-07-10 07:44:49.000000 crowdsim-0.1.6/crowdsim/window_control.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:47:26.370576 crowdsim-0.1.6/crowdsim.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:47:26.000000 crowdsim-0.1.6/crowdsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-10 07:47:26.000000 crowdsim-0.1.6/crowdsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:47:26.000000 crowdsim-0.1.6/crowdsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-10 07:47:26.000000 crowdsim-0.1.6/crowdsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 07:47:26.000000 crowdsim-0.1.6/crowdsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:47:26.370576 crowdsim-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-07-10 07:46:04.000000 crowdsim-0.1.6/setup.py
```

### Comparing `crowdsim-0.1.5/LICENSE.txt` & `crowdsim-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.5/crowdsim/Ui_enter_window.py` & `crowdsim-0.1.6/crowdsim/Ui_enter_window.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.5/crowdsim/config.py` & `crowdsim-0.1.6/crowdsim/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import taichi as ti
 import random
 import math
 from PIL import Image
 from numpy.random import default_rng
-import utils
+import crowdsim.utils
 import json
 
 @ti.data_oriented
 class Config:
     def __init__(self):
         self.Astar = 0 # 是否使用A*预渲染地图 1代表是
         self.dynamic_search = 0 #邻域搜索时使用静态分配内存还是动态分配内存 1代表用dynamic node 0代表用静态分配内存方法
```

### Comparing `crowdsim-0.1.5/crowdsim/orca_people.py` & `crowdsim-0.1.6/crowdsim/orca_people.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import taichi as ti
-from orca_scene import Scene
-import utils
+from crowdsim.orca_scene import Scene
+from crowdsim import utils
 import numpy as np
 import time
 @ti.data_oriented
 class ORCA_People:
     def __init__(self, config):
         self.config = config
         self.scene = Scene(config)
```

### Comparing `crowdsim-0.1.5/crowdsim/orca_scene.py` & `crowdsim-0.1.6/crowdsim/orca_scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import taichi as ti
 import numpy as np
 import math
 from PIL import Image
-import utils
+from crowdsim import utils
 
 @ti.dataclass
 class StaticObstacle:
     next:int
     previous:int
     direction:utils.vec2
     point:utils.vec2
```

### Comparing `crowdsim-0.1.5/crowdsim/pre_astar.py` & `crowdsim-0.1.6/crowdsim/pre_astar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import taichi as ti
 import numpy as np
 import time
-import utils
+from crowdsim import utils
 
 node = ti.types.struct(g=ti.float32, h=ti.float32,f=ti.float32, father=ti.int32)
 
 @ti.data_oriented
 class AStar:
     # not support ORCA yet
     def __init__(self,enable,scene):
```

### Comparing `crowdsim-0.1.5/crowdsim/sf_people.py` & `crowdsim-0.1.6/crowdsim/sf_people.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import taichi as ti
-from pre_astar import AStar
-from sf_scene import Scene
-import utils
+from crowdsim.pre_astar import AStar
+from crowdsim.sf_scene import Scene
+from crowdsim import utils
 import numpy as np
 import time
 
 @ti.data_oriented
 class SF_People:
     def __init__(self, config):
         self.config = config
```

### Comparing `crowdsim-0.1.5/crowdsim/sf_scene.py` & `crowdsim-0.1.6/crowdsim/sf_scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import taichi as ti
 import numpy as np
 import math
 from PIL import Image
-import utils
+from crowdsim import utils
 
 @ti.data_oriented
 class Scene:
     def __init__(self, config):
         self.window_size = config.window_size #网格边长
         self.pixel_number = config.pixel_number #网格大小  pixel_number = window_size^2
         self.batch_size = config.batch
```

### Comparing `crowdsim-0.1.5/crowdsim/steer_people.py` & `crowdsim-0.1.6/crowdsim/steer_people.py`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,11 @@
 import taichi as ti
-from pre_astar import AStar
-from steer_scene import Scene
-import utils
+from crowdsim.pre_astar import AStar
+from crowdsim.steer_scene import Scene
+from crowdsim import utils
 import numpy as np
 import  time
 @ti.data_oriented
 class Steer_People:
     def __init__(self, config):
         self.config = config
         self.scene = Scene(config)
```

### Comparing `crowdsim-0.1.5/crowdsim/steer_scene.py` & `crowdsim-0.1.6/crowdsim/steer_scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import taichi as ti
 import numpy as np
 import math
 from PIL import Image
-import utils
+from crowdsim import utils
 
 @ti.data_oriented
 class Scene:
     def __init__(self, config):
         self.window_size = config.window_size #网格边长
         self.pixel_number = config.pixel_number #网格大小  pixel_number = window_size^2
         self.batch_size = config.batch
```

### Comparing `crowdsim-0.1.5/crowdsim/test.py` & `crowdsim-0.1.6/crowdsim/test.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.5/crowdsim/utils.py` & `crowdsim-0.1.6/crowdsim/utils.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.5/crowdsim/window_control.py` & `crowdsim-0.1.6/crowdsim/window_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 from PyQt5.QtWidgets import QMainWindow,QApplication,QWidget,QFileDialog
-from Ui_enter_window import Ui_MainWindow  #导入你写的界面类
+from crowdsim.Ui_enter_window import Ui_MainWindow  #导入你写的界面类
 from configparser import ConfigParser
-from config import Config
-from orca_people import ORCA_People
-from sf_people import SF_People
-from steer_people import Steer_People
+from crowdsim.config import Config
+from crowdsim.orca_people import ORCA_People
+from crowdsim.sf_people import SF_People
+from crowdsim.steer_people import Steer_People
 import taichi as ti
 import time
-import utils
+from crowdsim import utils
 
 class MyMainWindow(QMainWindow,Ui_MainWindow):
     def __init__(self,parent =None):
         super(MyMainWindow,self).__init__(parent)
         ti.init(arch=ti.cpu,kernel_profiler=True, debug=True)#,cpu_max_num_threads=1, debug=True
         self.setupUi(self)
         self.config = Config()
```

