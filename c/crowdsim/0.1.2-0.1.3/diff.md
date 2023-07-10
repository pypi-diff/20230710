# Comparing `tmp/crowdsim-0.1.2.tar.gz` & `tmp/crowdsim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdsim-0.1.2.tar", last modified: Mon Jul 10 07:10:24 2023, max compression
+gzip compressed data, was "crowdsim-0.1.3.tar", last modified: Mon Jul 10 07:15:39 2023, max compression
```

## Comparing `crowdsim-0.1.2.tar` & `crowdsim-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:10:24.257471 crowdsim-0.1.2/
--rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      238 2023-07-10 07:10:24.257471 crowdsim-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 07:10:24.230693 crowdsim-0.1.2/crowdsim/
--rw-rw-rw-   0        0        0     2700 2023-04-21 11:23:00.000000 crowdsim-0.1.2/crowdsim/Ui_enter_window.py
--rw-rw-rw-   0        0        0    12129 2023-07-10 03:34:31.000000 crowdsim-0.1.2/crowdsim/__init__.py
--rw-rw-rw-   0        0        0    21088 2023-07-10 06:34:21.000000 crowdsim-0.1.2/crowdsim/config.py
--rw-rw-rw-   0        0        0    29976 2023-07-10 06:35:06.000000 crowdsim-0.1.2/crowdsim/orca_people.py
--rw-rw-rw-   0        0        0     3155 2023-04-10 05:28:36.000000 crowdsim-0.1.2/crowdsim/orca_scene.py
--rw-rw-rw-   0        0        0     8132 2023-04-21 11:23:00.000000 crowdsim-0.1.2/crowdsim/pre_astar.py
--rw-rw-rw-   0        0        0    25758 2023-05-23 10:01:14.000000 crowdsim-0.1.2/crowdsim/sf_people.py
--rw-rw-rw-   0        0        0     5472 2023-05-15 14:38:52.000000 crowdsim-0.1.2/crowdsim/sf_scene.py
--rw-rw-rw-   0        0        0    22596 2023-05-23 10:03:00.000000 crowdsim-0.1.2/crowdsim/steer_people.py
--rw-rw-rw-   0        0        0     5474 2023-05-02 08:45:23.000000 crowdsim-0.1.2/crowdsim/steer_scene.py
--rw-rw-rw-   0        0        0     3299 2023-07-10 03:28:56.000000 crowdsim-0.1.2/crowdsim/test.py
--rw-rw-rw-   0        0        0     3721 2023-07-10 06:33:11.000000 crowdsim-0.1.2/crowdsim/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:10:24.256474 crowdsim-0.1.2/crowdsim.egg-info/
--rw-rw-rw-   0        0        0      238 2023-07-10 07:10:24.000000 crowdsim-0.1.2/crowdsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-07-10 07:10:24.000000 crowdsim-0.1.2/crowdsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:10:24.000000 crowdsim-0.1.2/crowdsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-10 07:10:24.000000 crowdsim-0.1.2/crowdsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 07:10:24.000000 crowdsim-0.1.2/crowdsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:10:24.257471 crowdsim-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-07-10 07:10:16.000000 crowdsim-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:15:39.664774 crowdsim-0.1.3/
+-rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:15:39.663564 crowdsim-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 07:15:39.643583 crowdsim-0.1.3/crowdsim/
+-rw-rw-rw-   0        0        0     2700 2023-04-21 11:23:00.000000 crowdsim-0.1.3/crowdsim/Ui_enter_window.py
+-rw-rw-rw-   0        0        0      187 2023-07-10 07:15:26.000000 crowdsim-0.1.3/crowdsim/__init__.py
+-rw-rw-rw-   0        0        0    21088 2023-07-10 06:34:21.000000 crowdsim-0.1.3/crowdsim/config.py
+-rw-rw-rw-   0        0        0    29976 2023-07-10 06:35:06.000000 crowdsim-0.1.3/crowdsim/orca_people.py
+-rw-rw-rw-   0        0        0     3155 2023-04-10 05:28:36.000000 crowdsim-0.1.3/crowdsim/orca_scene.py
+-rw-rw-rw-   0        0        0     8132 2023-04-21 11:23:00.000000 crowdsim-0.1.3/crowdsim/pre_astar.py
+-rw-rw-rw-   0        0        0    25758 2023-05-23 10:01:14.000000 crowdsim-0.1.3/crowdsim/sf_people.py
+-rw-rw-rw-   0        0        0     5472 2023-05-15 14:38:52.000000 crowdsim-0.1.3/crowdsim/sf_scene.py
+-rw-rw-rw-   0        0        0    22596 2023-05-23 10:03:00.000000 crowdsim-0.1.3/crowdsim/steer_people.py
+-rw-rw-rw-   0        0        0     5474 2023-05-02 08:45:23.000000 crowdsim-0.1.3/crowdsim/steer_scene.py
+-rw-rw-rw-   0        0        0     3299 2023-07-10 03:28:56.000000 crowdsim-0.1.3/crowdsim/test.py
+-rw-rw-rw-   0        0        0     3721 2023-07-10 06:33:11.000000 crowdsim-0.1.3/crowdsim/utils.py
+-rw-rw-rw-   0        0        0    11994 2023-07-10 07:14:51.000000 crowdsim-0.1.3/crowdsim/window_control.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:15:39.663564 crowdsim-0.1.3/crowdsim.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:15:39.000000 crowdsim-0.1.3/crowdsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-10 07:15:39.000000 crowdsim-0.1.3/crowdsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:15:39.000000 crowdsim-0.1.3/crowdsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-10 07:15:39.000000 crowdsim-0.1.3/crowdsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 07:15:39.000000 crowdsim-0.1.3/crowdsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:15:39.664774 crowdsim-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-07-10 07:15:33.000000 crowdsim-0.1.3/setup.py
```

### Comparing `crowdsim-0.1.2/LICENSE.txt` & `crowdsim-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/Ui_enter_window.py` & `crowdsim-0.1.3/crowdsim/Ui_enter_window.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/__init__.py` & `crowdsim-0.1.3/crowdsim/window_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,12 +263,7 @@
                 f.write("Collision times: " + str(Collision[0])+ "\t"+"Collision Rate: " + str(CollisionRate)+ "\n")
                 ATTime = 0.0
                 if people.TotalTime > 0:
                     ATTime = people.TotalTime / people.ArrivalRate
                 f.write("Average Travel Time: " + str(ATTime)+ "s\n")
             f.write("\n")
     
-if __name__ == "__main__":
-    app = QApplication(sys.argv)
-    myWin = MyMainWindow()
-    myWin.show()
-    sys.exit(app.exec_())
```

### Comparing `crowdsim-0.1.2/crowdsim/config.py` & `crowdsim-0.1.3/crowdsim/config.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/orca_people.py` & `crowdsim-0.1.3/crowdsim/orca_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/orca_scene.py` & `crowdsim-0.1.3/crowdsim/orca_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/pre_astar.py` & `crowdsim-0.1.3/crowdsim/pre_astar.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/sf_people.py` & `crowdsim-0.1.3/crowdsim/sf_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/sf_scene.py` & `crowdsim-0.1.3/crowdsim/sf_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/steer_people.py` & `crowdsim-0.1.3/crowdsim/steer_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/steer_scene.py` & `crowdsim-0.1.3/crowdsim/steer_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/test.py` & `crowdsim-0.1.3/crowdsim/test.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.2/crowdsim/utils.py` & `crowdsim-0.1.3/crowdsim/utils.py`

 * *Files identical despite different names*

