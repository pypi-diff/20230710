# Comparing `tmp/ns_asphalt9-0.1.0.tar.gz` & `tmp/ns_asphalt9-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ns_asphalt9-0.1.0.tar", last modified: Sun Jul  9 05:11:24 2023, max compression
+gzip compressed data, was "dist/ns_asphalt9-0.1.1.tar", last modified: Mon Jul 10 14:38:00 2023, max compression
```

## Comparing `ns_asphalt9-0.1.0.tar` & `ns_asphalt9-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/
--rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.0/LICENSE
--rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/MANIFEST.in
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.0/README.md
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/
--rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/
--rw-r--r--   0 sunhao     (501) staff       (20)      244 2023-07-09 03:22:53.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)      477 2023-07-09 03:17:56.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 sunhao     (501) staff       (20)     4539 2023-07-09 03:22:39.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/cache.py
--rw-r--r--   0 sunhao     (501) staff       (20)     3072 2023-07-09 03:21:21.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/consts.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/controller.py
--rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)    21684 2023-07-09 03:40:27.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/
--rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/ocr.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 sunhao     (501) staff       (20)    13348 2023-07-09 04:52:32.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/pages.py
--rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 sunhao     (501) staff       (20)     2728 2023-07-09 04:10:27.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/
--rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.1.0/ns_asphalt9/main.py
-drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/
--rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-09 05:11:24.000000 ns_asphalt9-0.1.0/setup.cfg
--rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.0/setup.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/
+-rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.1.1/LICENSE
+-rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/MANIFEST.in
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.1.1/README.md
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/
+-rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/
+-rw-r--r--   0 sunhao     (501) staff       (20)      258 2023-07-09 10:58:05.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      589 2023-07-09 10:57:49.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4652 2023-07-10 14:21:56.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3917 2023-07-02 12:56:49.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3923 2023-07-10 14:10:27.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/cache.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2746 2023-07-10 14:07:06.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/consts.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/controller.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      638 2023-07-10 14:11:06.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    23653 2023-07-10 14:18:29.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1843 2023-07-10 14:15:27.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    13397 2023-07-09 11:01:57.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/pages.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2686 2023-07-10 14:02:34.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     5517 2023-07-10 14:14:54.000000 ns_asphalt9-0.1.1/ns_asphalt9/main.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-10 14:37:59.000000 ns_asphalt9-0.1.1/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-10 14:38:00.000000 ns_asphalt9-0.1.1/setup.cfg
+-rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.1.1/setup.py
```

### Comparing `ns_asphalt9-0.1.0/LICENSE` & `ns_asphalt9-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/PKG-INFO` & `ns_asphalt9-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.0/README.md` & `ns_asphalt9-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/enter_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,36 +28,40 @@
     pro.press_group([Buttons.DPAD_RIGHT] * 7, 0.1)
     pro.press_group([Buttons.A], 2)
     pro.press_group([Buttons.B], 2)
 
 
 def in_series(page, mode):
     if (
-        mode == consts.world_series_zh
+        mode == consts.mp1_zh
         and page.name == consts.world_series
-        or mode == consts.other_series_zh
+        or mode in [consts.mp2_zh, consts.mp3_zh]
         and page.name
         in [
             consts.trial_series,
             consts.limited_series,
         ]
     ):
         return True
     return False
 
 
 @retry(max_attempts=3)
-def enter_series(page=None, mode=consts.world_series_zh):
+def enter_series(page=None, mode=None):
     """进入多人赛事"""
+    if not mode:
+        mode = globals.CONFIG["模式"]
     if page and in_series(page, mode):
         return
     reset_to_career()
     pro.press_group([Buttons.ZL] * 4, 0.5)
-    if mode != consts.world_series_zh:
+    if mode == consts.mp2_zh:
         pro.press_group([Buttons.DPAD_DOWN], 0.5)
+    if mode == consts.mp3_zh:
+        pro.press_group([Buttons.DPAD_DOWN] * 2, 0.5)
     time.sleep(2)
     pro.press_group([Buttons.A], 2)
     page = ocr_screen()
     if in_series(page, mode):
         pass
     else:
         raise Exception(f"Failed to access {mode}, current page = {page.name}")
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/actions/select_car.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,31 +47,35 @@
 def world_series_positions():
     division = globals.DIVISION
     if not division:
         division = "青铜"
     config = globals.CONFIG["多人一"][division]
     return config["车库位置"]
 
+def mp3_position():
+    return globals.CONFIG["多人三"]["车库位置"]
 
 def other_series_position():
     return globals.CONFIG["多人二"]["车库位置"]
 
 
 def carhunt_position():
     return globals.CONFIG["寻车"]["车库位置"]
 
 
 def get_race_config():
     mode = globals.MODE if globals.MODE else globals.CONFIG["模式"]
     logger.info(f"Get mode {mode} config.")
-    if mode == consts.other_series_zh:
+    if mode ==  consts.mp3_zh:
+        return mp3_position(), other_series_reset, mode
+    elif mode == consts.mp2_zh:
         return other_series_position(), other_series_reset, mode
     elif mode == consts.car_hunt_zh:
         return carhunt_position(), carhunt_reset, mode
-    elif mode == consts.world_series_zh:
+    elif mode == consts.mp1_zh:
         return world_series_positions(), world_series_reset, mode
     else:
         return default_positions(), default_reset, mode
 
 
 def select_car():
     # 选车
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         self.setting_modules = {}
 
         # create settings frame
         self.settings = customtkinter.CTkScrollableFrame(
             self, corner_radius=0, fg_color="transparent"
         )
 
-        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车", "传奇寻车", "大奖赛"]):
+        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车", "传奇寻车", "多三", "大奖赛"]):
             label = customtkinter.CTkLabel(master=self.settings, text=f"{label_text}:")
             label.grid(
                 row=row,
                 column=0,
                 columnspan=1,
                 padx=10,
                 pady=(20 if row == 0 else 10, 10),
@@ -138,15 +138,15 @@
 
         # 模式配置
         self.mode = tkinter.StringVar()
         self.mode_buttons = customtkinter.CTkSegmentedButton(
             self.settings,
             variable=self.mode,
             command=self.save_settings,
-            values=["多人一", "多人二", "寻车", "传奇寻车"],
+            values=["多人一", "多人二", "多人三", "寻车", "传奇寻车"],
         )
         self.mode_buttons.grid(
             row=0, column=1, padx=(20, 10), pady=(20, 10), sticky="ew"
         )
         if self.settings_data:
             self.mode_buttons.set(self.settings_data["模式"])
         self.setting_modules["模式"] = self.mode_buttons
@@ -440,19 +440,68 @@
                     option1.set(self.settings_data["传奇寻车"]["车库位置"][r]["row"])
                     option2.set(self.settings_data["传奇寻车"]["车库位置"][r]["col"])
             except IndexError:
                 pass
 
             self.setting_modules["寻车"]["车库位置"].append({"row": option1, "col": option2})
 
+        # 多人三配置
+        mp3_settings_frame = customtkinter.CTkFrame(self.settings, width=340)
+        mp3_settings_frame.grid(
+            row=6, column=1, columnspan=2, padx=(20, 0), pady=(20, 0), sticky="nsew"
+        )
+
+        car_position = customtkinter.CTkLabel(master=mp3_settings_frame, text="车库位置:")
+
+        car_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
+
+        row = customtkinter.CTkLabel(master=mp3_settings_frame, text="row")
+
+        row.grid(row=1, column=1, padx=(0, 0), pady=(10, 10), sticky="nsew")
+
+        col = customtkinter.CTkLabel(master=mp3_settings_frame, text="col")
+
+        col.grid(row=1, column=2, padx=(0, 10), pady=(10, 10), sticky="nsew")
+
+        self.setting_modules["多人三"] = {}
+        self.setting_modules["多人三"]["车库位置"] = []
+
+        for r in range(6):
+            option1 = customtkinter.CTkOptionMenu(
+                mp3_settings_frame,
+                dynamic_resizing=False,
+                values=[str(i) for i in range(0, 3)],
+                width=100,
+                height=28,
+                command=self.save_settings,
+            )
+
+            option2 = customtkinter.CTkOptionMenu(
+                mp3_settings_frame,
+                dynamic_resizing=False,
+                values=[str(i) for i in range(0, 30)],
+                width=100,
+                height=28,
+                command=self.save_settings,
+            )
+
+            option1.grid(row=r + 2, column=1, padx=(10, 10), pady=(10, 10))
+            option2.grid(row=r + 2, column=2, padx=(10, 10), pady=(10, 10))
+
+            if self.settings_data and "多人三" in self.settings_data:
+                option1.set(self.settings_data["多人三"]["车库位置"][r]["row"])
+                option2.set(self.settings_data["多人三"]["车库位置"][r]["col"])
+
+            self.setting_modules["多人三"]["车库位置"].append({"row": option1, "col": option2})
+
         # 大奖赛配置
         self.setting_modules["大奖赛"] = {}
         prix_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
         prix_setting_frame.grid(
-            row=6, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
+            row=7, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
         )
 
         prix_position = customtkinter.CTkLabel(
             master=prix_setting_frame, text="位置:"
         )
         prix_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
         prix_position_option = customtkinter.CTkOptionMenu(
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.1/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/page_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if (
             not match_pages
             and text
             or len(match_pages) >= 2
             and match_pages[0][1] == match_pages[1][1]
         ):
             logger.info(f"match_pages = {match_pages}")
-            self.capture()
+            # self.capture()
 
         if match_pages:
             page = match_pages[0][0](text, self.last_page)
         else:
             page = pages.Empty(text, self.last_page)
         methods = [
             method for method in dir(page) if callable(getattr(page, method))
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 class LoadingGame(Page):
     """游戏加载页"""
 
     name = consts.loading_game
     feature = "GAMELOFT PLAYER ID.*ASPHALT"
     part_match = False
 
+    action = staticmethod(actions.loading_game)
+
 
 @cache_decorator("page")
 class LoadingRace(Page):
     """比赛加载页"""
 
     name = consts.loading_race
     feature = "LOADING RACE"
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,16 @@
             consts.world_series,
             consts.limited_series,
             consts.trial_series,
             consts.carhunt,
             consts.card_pack,
             consts.legend_pass,
             consts.legendary_hunt,
-            consts.daily_events
+            consts.daily_events,
+            consts.multi_player
         ]:
             return False
 
         if globals.task_queue.empty():
             if cls.status == consts.TaskStatus.done:
                 cls.task_enter(globals.CONFIG["模式"], page=page)
                 cls.status = consts.TaskStatus.default
@@ -61,18 +62,16 @@
             cls.current_task = task
             cls.task_enter(task, page)
             return True
 
     @classmethod
     def task_enter(cls, task, page=None) -> None:
         logger.info(f"Start process {task} task.")
-        if task == consts.world_series_zh:
+        if task in [consts.mp1_zh, consts.mp2_zh, consts.mp3_zh]:
             actions.enter_series(page=page)
-        if task == consts.other_series_zh:
-            actions.enter_series(mode=task, page=page)
         if task == consts.car_hunt_zh:
             actions.enter_carhunt(page=page)
         if task == consts.free_pack_zh:
             actions.free_pack()
         if task == consts.prix_pack_zh:
             actions.prix_pack()
         if task == consts.legendary_hunt_zh:
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.1/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9/main.py` & `ns_asphalt9-0.1.1/ns_asphalt9/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,17 @@
             if page.mode:
                 G.MODE = page.mode
             dispatched = TaskManager.task_dispatch(page)
             if not dispatched:
                 process_screen(page)
             time.sleep(3)
         except Exception as err:
-            filename = capture()
+            # filename = capture()
             logger.error(
-                f"Caught exception, err = {err}, traceback = {traceback.format_exc()}, \
-                  filename = {filename}"
+                f"Caught exception, err = {err}, traceback = {traceback.format_exc()}"
             )
 
     G.G_RACE_QUIT_EVENT.set()
 
 
 def command_input(queue):
     while G.G_RUN.is_set():
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.1/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.0/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.1/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.0/setup.cfg` & `ns_asphalt9-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.0
+version = 0.1.1
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

