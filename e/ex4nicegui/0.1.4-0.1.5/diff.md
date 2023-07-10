# Comparing `tmp/ex4nicegui-0.1.4.tar.gz` & `tmp/ex4nicegui-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.4.tar", last modified: Mon Jul 10 14:32:06 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.5.tar", last modified: Mon Jul 10 14:34:10 2023, max compression
```

## Comparing `ex4nicegui-0.1.4.tar` & `ex4nicegui-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.405094 ex4nicegui-0.1.4/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-10 14:32:06.400107 ex4nicegui-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.316329 ex4nicegui-0.1.4/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-10 14:31:57.000000 ex4nicegui-0.1.4/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.331291 ex4nicegui-0.1.4/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.345252 ex4nicegui-0.1.4/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0      998 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.363204 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.380160 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    30930 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.386143 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.390133 ex4nicegui-0.1.4/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.4/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.397118 ex4nicegui-0.1.4/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.4/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.4/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.4/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-10 14:32:06.327303 ex4nicegui-0.1.4/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2023-07-10 14:32:06.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 14:32:05.000000 ex4nicegui-0.1.4/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 14:32:06.405094 ex4nicegui-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2073 2023-07-09 14:56:08.000000 ex4nicegui-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.316231 ex4nicegui-0.1.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-10 14:34:10.314238 ex4nicegui-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-05 06:11:55.000000 ex4nicegui-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.253548 ex4nicegui-0.1.5/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-10 14:33:54.000000 ex4nicegui-0.1.5/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.269546 ex4nicegui-0.1.5/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.282322 ex4nicegui-0.1.5/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0      998 2023-07-10 14:31:39.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.289303 ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.298310 ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    30930 2023-07-10 14:31:39.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/rxui.py
+-rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/signature.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.304283 ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.307289 ex4nicegui-0.1.5/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.5/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.312241 ex4nicegui-0.1.5/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.5/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.5/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.5/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-10 14:34:10.264561 ex4nicegui-0.1.5/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-10 14:34:09.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2023-07-10 14:34:10.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 14:34:09.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 14:34:09.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-07-10 14:34:09.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-10 14:34:09.000000 ex4nicegui-0.1.5/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 14:34:10.316231 ex4nicegui-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2023-07-10 14:33:48.000000 ex4nicegui-0.1.5/setup.py
```

### Comparing `ex4nicegui-0.1.4/LICENSE` & `ex4nicegui-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.5/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/__index.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/officials.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/signature.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/signature.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.5/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.5/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.5/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.5/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.4/setup.py` & `ex4nicegui-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     return list(all_infos)
 
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
-requirements = ["signe", "nicegui", "typing_extensions"]
+requirements = ["signe>=0.1.8", "nicegui>=1.2.24", "typing_extensions"]
 
 test_requirements = ["pytest>=3"]
 
 setup(
     author="carson_jia",
     author_email="568166495@qq.com",
     python_requires=">=3.7",
```

