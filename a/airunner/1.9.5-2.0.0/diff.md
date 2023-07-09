# Comparing `tmp/airunner-1.9.5.tar.gz` & `tmp/airunner-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.5.tar", last modified: Sun Apr 23 13:36:01 2023, max compression
+gzip compressed data, was "airunner-2.0.0.tar", last modified: Sun Jul  9 22:11:45 2023, max compression
```

## Comparing `airunner-1.9.5.tar` & `airunner-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.596524 airunner-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 13:35:50.000000 airunner-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-23 13:36:01.596524 airunner-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-23 13:35:50.000000 airunner-1.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 13:36:01.596524 airunner-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-23 13:35:50.000000 airunner-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.592524 airunner-1.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.592524 airunner-1.9.5/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    64713 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-23 13:35:50.000000 airunner-1.9.5/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 13:36:01.596524 airunner-1.9.5/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 13:36:01.000000 airunner-1.9.5/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.867821 airunner-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 22:11:36.000000 airunner-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-09 22:11:45.867821 airunner-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-09 22:11:36.000000 airunner-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:11:45.867821 airunner-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-09 22:11:36.000000 airunner-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.859821 airunner-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.859821 airunner-2.0.0/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.859821 airunner-2.0.0/src/airunner/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27364 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.863821 airunner-2.0.0/src/airunner/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_active_grid_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_grid_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_image_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_selectionbox_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/canvas_widgets_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/comic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/embedding_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/extension_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48995 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/generator_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/history_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/lora_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/menubar_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/mixins/toolbar_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.863821 airunner-2.0.0/src/airunner/pyqt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/base_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/generate_form_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/main_window_new_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/model_merger_model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/model_merger_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/noise_filter_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/prompt_browser_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/saturation_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.867821 airunner-2.0.0/src/airunner/pyqt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/canvas_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/generator_tab_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/grid_preferences_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/header_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/layer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/lora_container_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/prompt_builder_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/slider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/tool_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/pyqt/widgets/toolbar_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-09 22:11:36.000000 airunner-2.0.0/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:11:45.859821 airunner-2.0.0/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-09 22:11:45.000000 airunner-2.0.0/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-09 22:11:45.000000 airunner-2.0.0/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:11:45.000000 airunner-2.0.0/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 22:11:45.000000 airunner-2.0.0/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 22:11:45.000000 airunner-2.0.0/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.5/LICENSE` & `airunner-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.5/PKG-INFO` & `airunner-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.5
+Version: 2.0.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
@@ -21,23 +21,23 @@
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
 
 ---
 
-### Stable Diffusion on your own hardware 
+### Stable Diffusion and Kandinsky on your own hardware 
 
 No web server to run, additional requirements to install or technical knowledge required. 
 
 [Just download the compiled package](https://capsizegames.itch.io/ai-runner) and start generating AI Art!
 
 ---
 
-![img.png](img.png)
+![Screenshot from 2023-06-30 10-43-49](https://github.com/Capsize-Games/airunner/assets/25737761/72e0dd26-53ca-4d5c-8f07-b6327a59b50c)
 
 ## ⭐ Features
 
 Easily generate AI art using Stable Diffusion.
 
 - Easy setup - download and run. No need to install any requirements*
 - Fast! Generate images in approximately 2 seconds using an RTX 2080s, 512x512 dimensions, 20 steps euler_a (approximately 10 seconds for 512x512 20 steps Euler A on 1080gtx). Also runs on CPU†
@@ -74,7 +74,19 @@
 
 This is the compiled version of AI Runner which you can use without installing any additional dependencies.
 
 For those interested in installing the development version, there are three options to choose from. 
 
 [See the installation 
 wiki page for more information](https://github.com/Capsize-Games/airunner/wiki/Installation-instructions)
+
+---
+
+### Unit tests
+
+Unit tests can be run using the following command:
+
+**All tests:**
+`python -m unittest discover tests`
+
+**Individual test:**
+`python -m unittest tests.test_canvas`
```

### Comparing `airunner-1.9.5/README.md` & `airunner-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
 
 ---
 
-### Stable Diffusion on your own hardware 
+### Stable Diffusion and Kandinsky on your own hardware 
 
 No web server to run, additional requirements to install or technical knowledge required. 
 
 [Just download the compiled package](https://capsizegames.itch.io/ai-runner) and start generating AI Art!
 
 ---
 
-![img.png](img.png)
+![Screenshot from 2023-06-30 10-43-49](https://github.com/Capsize-Games/airunner/assets/25737761/72e0dd26-53ca-4d5c-8f07-b6327a59b50c)
 
 ## ⭐ Features
 
 Easily generate AI art using Stable Diffusion.
 
 - Easy setup - download and run. No need to install any requirements*
 - Fast! Generate images in approximately 2 seconds using an RTX 2080s, 512x512 dimensions, 20 steps euler_a (approximately 10 seconds for 512x512 20 steps Euler A on 1080gtx). Also runs on CPU†
@@ -61,7 +61,19 @@
 
 This is the compiled version of AI Runner which you can use without installing any additional dependencies.
 
 For those interested in installing the development version, there are three options to choose from. 
 
 [See the installation 
 wiki page for more information](https://github.com/Capsize-Games/airunner/wiki/Installation-instructions)
+
+---
+
+### Unit tests
+
+Unit tests can be run using the following command:
+
+**All tests:**
+`python -m unittest discover tests`
+
+**Individual test:**
+`python -m unittest tests.test_canvas`
```

### Comparing `airunner-1.9.5/setup.py` & `airunner-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.5",
+    version="2.0.0",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.9.7",
+        "aihandler==1.18.0",
     ]
 )
```

### Comparing `airunner-1.9.5/src/airunner/balloon.py` & `airunner-2.0.0/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.5/src/airunner/runai_client.py` & `airunner-2.0.0/src/airunner/runai_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     def cancel(self):
         self.sd_runner.cancel()
 
     def __init__(self, **kwargs):
         super().__init__(
             parent=kwargs.get("parent", None)
         )
+        self.app = kwargs.get("app", None)
+        self.settings_manager = kwargs.get("settings_manager", None)
         self.quit_event = BooleanVar()
         self.queue = queue.Queue()
         self.res_queue = queue.Queue()
         self.quit_event.set(False)
         self.logger = logging.getLogger()
         self.image_var = kwargs.get("image_var")
         self.error_var = kwargs.get("error_var")
@@ -77,26 +79,30 @@
     def do_start(self):
         # create a stable diffusion runner service
         # sd_runner_thread = self.start_thread(
         #     target=self.init_sd_runner,
         #     name="init stable diffusion runner"
         # )
         # sd_runner_thread.join()
+        self.logger.info("Starting offline client")
         self.init_sd_runner()
         self.force_request_worker_reset()
 
     def init_sd_runner(self):
         # save sd_runner to disc and load from it next time
         # this is to avoid the overhead of creating a new sd_runner
         # every time we start the client
+        self.logger.info("Initialzing SDRunner")
         self.sd_runner = SDRunner(
             app=self.app,
             tqdm_var=self.tqdm_var,
             image_var=self.image_var,
             message_var=self.message_var,
+            settings_manager=self.settings_manager,
+            error_var=self.error_var,
         )
 
     def handle_response(self, response):
         """
         Handle the response from the server
         :param response:
         :return: None
```

### Comparing `airunner-1.9.5/src/airunner.egg-info/PKG-INFO` & `airunner-2.0.0/src/airunner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.5
+Version: 2.0.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
@@ -21,23 +21,23 @@
 ![GitHub issues](https://img.shields.io/github/issues/Capsize-Games/airunner)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/Capsize-Games/airunner)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Capsize-Games/airunner)
 ![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/Capsize-Games/airunner)
 
 ---
 
-### Stable Diffusion on your own hardware 
+### Stable Diffusion and Kandinsky on your own hardware 
 
 No web server to run, additional requirements to install or technical knowledge required. 
 
 [Just download the compiled package](https://capsizegames.itch.io/ai-runner) and start generating AI Art!
 
 ---
 
-![img.png](img.png)
+![Screenshot from 2023-06-30 10-43-49](https://github.com/Capsize-Games/airunner/assets/25737761/72e0dd26-53ca-4d5c-8f07-b6327a59b50c)
 
 ## ⭐ Features
 
 Easily generate AI art using Stable Diffusion.
 
 - Easy setup - download and run. No need to install any requirements*
 - Fast! Generate images in approximately 2 seconds using an RTX 2080s, 512x512 dimensions, 20 steps euler_a (approximately 10 seconds for 512x512 20 steps Euler A on 1080gtx). Also runs on CPU†
@@ -74,7 +74,19 @@
 
 This is the compiled version of AI Runner which you can use without installing any additional dependencies.
 
 For those interested in installing the development version, there are three options to choose from. 
 
 [See the installation 
 wiki page for more information](https://github.com/Capsize-Games/airunner/wiki/Installation-instructions)
+
+---
+
+### Unit tests
+
+Unit tests can be run using the following command:
+
+**All tests:**
+`python -m unittest discover tests`
+
+**Individual test:**
+`python -m unittest tests.test_canvas`
```

