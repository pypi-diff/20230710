# Comparing `tmp/crowdsim-0.1.4.tar.gz` & `tmp/crowdsim-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdsim-0.1.4.tar", last modified: Mon Jul 10 07:31:29 2023, max compression
+gzip compressed data, was "crowdsim-0.1.5.tar", last modified: Mon Jul 10 07:33:51 2023, max compression
```

## Comparing `crowdsim-0.1.4.tar` & `crowdsim-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:31:29.426187 crowdsim-0.1.4/
--rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      238 2023-07-10 07:31:29.425176 crowdsim-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 07:31:29.401629 crowdsim-0.1.4/crowdsim/
--rw-rw-rw-   0        0        0     2700 2023-04-21 11:23:00.000000 crowdsim-0.1.4/crowdsim/Ui_enter_window.py
--rw-rw-rw-   0        0        0      275 2023-07-10 07:30:57.000000 crowdsim-0.1.4/crowdsim/__init__.py
--rw-rw-rw-   0        0        0    21088 2023-07-10 06:34:21.000000 crowdsim-0.1.4/crowdsim/config.py
--rw-rw-rw-   0        0        0    29976 2023-07-10 06:35:06.000000 crowdsim-0.1.4/crowdsim/orca_people.py
--rw-rw-rw-   0        0        0     3155 2023-04-10 05:28:36.000000 crowdsim-0.1.4/crowdsim/orca_scene.py
--rw-rw-rw-   0        0        0     8132 2023-04-21 11:23:00.000000 crowdsim-0.1.4/crowdsim/pre_astar.py
--rw-rw-rw-   0        0        0    25758 2023-05-23 10:01:14.000000 crowdsim-0.1.4/crowdsim/sf_people.py
--rw-rw-rw-   0        0        0     5472 2023-05-15 14:38:52.000000 crowdsim-0.1.4/crowdsim/sf_scene.py
--rw-rw-rw-   0        0        0    22596 2023-05-23 10:03:00.000000 crowdsim-0.1.4/crowdsim/steer_people.py
--rw-rw-rw-   0        0        0     5474 2023-05-02 08:45:23.000000 crowdsim-0.1.4/crowdsim/steer_scene.py
--rw-rw-rw-   0        0        0     3299 2023-07-10 03:28:56.000000 crowdsim-0.1.4/crowdsim/test.py
--rw-rw-rw-   0        0        0     3721 2023-07-10 06:33:11.000000 crowdsim-0.1.4/crowdsim/utils.py
--rw-rw-rw-   0        0        0    11994 2023-07-10 07:14:51.000000 crowdsim-0.1.4/crowdsim/window_control.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:31:29.425176 crowdsim-0.1.4/crowdsim.egg-info/
--rw-rw-rw-   0        0        0      238 2023-07-10 07:31:29.000000 crowdsim-0.1.4/crowdsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-07-10 07:31:29.000000 crowdsim-0.1.4/crowdsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:31:29.000000 crowdsim-0.1.4/crowdsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-10 07:31:29.000000 crowdsim-0.1.4/crowdsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 07:31:29.000000 crowdsim-0.1.4/crowdsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 07:31:29.426187 crowdsim-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      515 2023-07-10 07:31:19.000000 crowdsim-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.978405 crowdsim-0.1.5/
+-rw-rw-rw-   0        0        0     1081 2023-07-10 07:07:31.000000 crowdsim-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:33:51.978405 crowdsim-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-10 07:08:54.000000 crowdsim-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.966713 crowdsim-0.1.5/crowdsim/
+-rw-rw-rw-   0        0        0     2700 2023-04-21 11:23:00.000000 crowdsim-0.1.5/crowdsim/Ui_enter_window.py
+-rw-rw-rw-   0        0        0      275 2023-07-10 07:30:57.000000 crowdsim-0.1.5/crowdsim/__init__.py
+-rw-rw-rw-   0        0        0    21088 2023-07-10 06:34:21.000000 crowdsim-0.1.5/crowdsim/config.py
+-rw-rw-rw-   0        0        0    29976 2023-07-10 06:35:06.000000 crowdsim-0.1.5/crowdsim/orca_people.py
+-rw-rw-rw-   0        0        0     3155 2023-04-10 05:28:36.000000 crowdsim-0.1.5/crowdsim/orca_scene.py
+-rw-rw-rw-   0        0        0     8132 2023-04-21 11:23:00.000000 crowdsim-0.1.5/crowdsim/pre_astar.py
+-rw-rw-rw-   0        0        0    25758 2023-05-23 10:01:14.000000 crowdsim-0.1.5/crowdsim/sf_people.py
+-rw-rw-rw-   0        0        0     5472 2023-05-15 14:38:52.000000 crowdsim-0.1.5/crowdsim/sf_scene.py
+-rw-rw-rw-   0        0        0    22596 2023-05-23 10:03:00.000000 crowdsim-0.1.5/crowdsim/steer_people.py
+-rw-rw-rw-   0        0        0     5474 2023-05-02 08:45:23.000000 crowdsim-0.1.5/crowdsim/steer_scene.py
+-rw-rw-rw-   0        0        0     3299 2023-07-10 03:28:56.000000 crowdsim-0.1.5/crowdsim/test.py
+-rw-rw-rw-   0        0        0     3721 2023-07-10 06:33:11.000000 crowdsim-0.1.5/crowdsim/utils.py
+-rw-rw-rw-   0        0        0    11994 2023-07-10 07:14:51.000000 crowdsim-0.1.5/crowdsim/window_control.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:33:51.977406 crowdsim-0.1.5/crowdsim.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 07:33:51.000000 crowdsim-0.1.5/crowdsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:33:51.978405 crowdsim-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-07-10 07:33:47.000000 crowdsim-0.1.5/setup.py
```

### Comparing `crowdsim-0.1.4/LICENSE.txt` & `crowdsim-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/Ui_enter_window.py` & `crowdsim-0.1.5/crowdsim/Ui_enter_window.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/config.py` & `crowdsim-0.1.5/crowdsim/config.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/orca_people.py` & `crowdsim-0.1.5/crowdsim/orca_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/orca_scene.py` & `crowdsim-0.1.5/crowdsim/orca_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/pre_astar.py` & `crowdsim-0.1.5/crowdsim/pre_astar.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/sf_people.py` & `crowdsim-0.1.5/crowdsim/sf_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/sf_scene.py` & `crowdsim-0.1.5/crowdsim/sf_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/steer_people.py` & `crowdsim-0.1.5/crowdsim/steer_people.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/steer_scene.py` & `crowdsim-0.1.5/crowdsim/steer_scene.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/test.py` & `crowdsim-0.1.5/crowdsim/test.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/utils.py` & `crowdsim-0.1.5/crowdsim/utils.py`

 * *Files identical despite different names*

### Comparing `crowdsim-0.1.4/crowdsim/window_control.py` & `crowdsim-0.1.5/crowdsim/window_control.py`

 * *Files identical despite different names*

