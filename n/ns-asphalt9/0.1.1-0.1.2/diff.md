# Comparing `tmp/ns_asphalt9-0.1.1.tar.gz` & `tmp/ns_asphalt9-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns_asphalt9-0.1.1.tar", last modified: Mon Jul 10 14:38:00 2023, max compression
+gzip compressed data, was "dist/ns_asphalt9-0.1.2.tar", last modified: Mon Jul 10 16:06:38 2023, max compression
```

## Comparing `ns_asphalt9-0.1.1.tar` & `ns_asphalt9-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/
--rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.1/LICENSE
--rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/MANIFEST.in
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.1/README.md
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/
--rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/
--rw-r--r--   0 sunhao     (501) staff       (20)      258 2023-07-09 10:58:05.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)      589 2023-07-09 10:57:49.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4652 2023-07-10 14:21:56.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3923 2023-07-10 14:10:27.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/cache.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2746 2023-07-10 14:07:06.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/consts.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/controller.py
--rw-r--r--   0 sunhao     (501) staff       (20)      638 2023-07-10 14:11:06.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)    23653 2023-07-10 14:18:29.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/
--rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/ocr.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1843 2023-07-10 14:15:27.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 sunhao     (501) staff       (20)    13397 2023-07-09 11:01:57.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/pages.py
--rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2686 2023-07-10 14:02:34.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 sunhao     (501) staff       (20)     5517 2023-07-10 14:14:54.000000 ns_asphalt9-0.1.1/ns_asphalt9/main.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/setup.cfg
--rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/setup.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/
+-rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.2/LICENSE
+-rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/MANIFEST.in
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.2/README.md
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/
+-rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/
+-rw-r--r--   0 sunhao     (501) staff       (20)      258 2023-07-09 10:58:05.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      589 2023-07-09 10:57:49.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4652 2023-07-10 14:21:56.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4241 2023-07-10 15:55:00.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/cache.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2828 2023-07-10 15:07:50.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/consts.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/controller.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      638 2023-07-10 14:11:06.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    23653 2023-07-10 14:18:29.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1843 2023-07-10 14:15:27.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    13412 2023-07-10 15:27:10.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/pages.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2686 2023-07-10 14:02:34.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     5517 2023-07-10 14:14:54.000000 ns_asphalt9-0.1.2/ns_asphalt9/main.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-10 16:06:38.000000 ns_asphalt9-0.1.2/setup.cfg
+-rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.2/setup.py
```

### Comparing `ns_asphalt9-0.1.1/LICENSE` & `ns_asphalt9-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/PKG-INFO` & `ns_asphalt9-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.1/README.md` & `ns_asphalt9-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/actions/select_car.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,25 +58,32 @@
     return globals.CONFIG["多人二"]["车库位置"]
 
 
 def carhunt_position():
     return globals.CONFIG["寻车"]["车库位置"]
 
 
+def legendary_hunt_position():
+    return globals.CONFIG["传奇寻车"]["车库位置"]
+
+
 def get_race_config():
     mode = globals.MODE if globals.MODE else globals.CONFIG["模式"]
     logger.info(f"Get mode {mode} config.")
-    if mode ==  consts.mp3_zh:
-        return mp3_position(), other_series_reset, mode
-    elif mode == consts.mp2_zh:
-        return other_series_position(), other_series_reset, mode
+    if mode in [consts.mp_zh, consts.mp1_zh]:
+        if globals.CONFIG["模式"] == consts.mp3_zh:
+            return mp3_position(), other_series_reset, consts.mp3_zh
+        elif globals.CONFIG["模式"] == consts.mp2_zh:
+            return other_series_position(), other_series_reset, consts.mp2_zh
+        else:
+            return world_series_positions(), world_series_reset, consts.mp1_zh
     elif mode == consts.car_hunt_zh:
         return carhunt_position(), carhunt_reset, mode
-    elif mode == consts.mp1_zh:
-        return world_series_positions(), world_series_reset, mode
+    elif mode == consts.legendary_hunt_zh:
+        return legendary_hunt_position(), carhunt_reset, mode        
     else:
         return default_positions(), default_reset, mode
 
 
 def select_car():
     # 选车
     logger.info("Start select car.")
```

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,27 +109,29 @@
 free_pack_zh = "免费抽卡"
 prix_pack_zh = "大奖赛抽卡"
 legendary_hunt_zh = "传奇寻车"
 
 
 class Mode:
     car_hunt = "CAR HUNT"
+    legendary_hunt = "LEGENDARY HUNT"
     world_series = "WORLD SERIES"
     limited_series = "LIMITED SERIES"
     trial_series = "TRIAL SERIES"
 
 
 class TaskStatus:
     default = ""
     start = "start"
     done = "done"
 
 
 modes_zh = {
     Mode.car_hunt: car_hunt_zh,
+    Mode.legendary_hunt: legendary_hunt_zh,
     Mode.world_series: mp1_zh,
     Mode.limited_series: mp_zh,
     Mode.trial_series: mp_zh,
 }
 
 
 bronze = "BRONZE"
```

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.2/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             consts.world_series,
             consts.searching,
             consts.loading_race,
         ]:
             self.division = consts.divisions_zh.get(divisions[0], "")
 
         modes = re.findall(
-            "CAR HUNT|WORLD SERIES|LIMITED SERIES|TRIAL SERIES", self.text
+            "LEGENDARY HUNT|CAR HUNT|WORLD SERIES|LIMITED SERIES|TRIAL SERIES", self.text
         )
         if modes and self.name not in [consts.multi_player]:
             self.mode = consts.modes_zh.get(modes[0], "")
             if self.mode == consts.car_hunt_zh:
                 hunt_cars = re.findall("APEX AP-0", self.text)
                 if hunt_cars:
                     self.hunt_car = hunt_cars[0]
```

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.2/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9/main.py` & `ns_asphalt9-0.1.2/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.2/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.1/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.2/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.1/setup.cfg` & `ns_asphalt9-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.1
+version = 0.1.2
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

