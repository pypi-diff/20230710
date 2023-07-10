# Comparing `tmp/visionscript-0.0.2.tar.gz` & `tmp/visionscript-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionscript-0.0.2.tar", last modified: Sat Jul  8 09:35:39 2023, max compression
+gzip compressed data, was "visionscript-0.0.3.tar", last modified: Mon Jul 10 18:00:26 2023, max compression
```

## Comparing `visionscript-0.0.2.tar` & `visionscript-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.541249 visionscript-0.0.2/
--rw-r--r--   0 james      (501) staff       (20)       16 2023-07-06 16:15:17.000000 visionscript-0.0.2/CNAME
--rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.2/LICENSE
--rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 16:15:17.000000 visionscript-0.0.2/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-08 09:35:39.541030 visionscript-0.0.2/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5857 2023-07-06 16:15:17.000000 visionscript-0.0.2/README.md
--rw-r--r--   0 james      (501) staff       (20)   725622 2023-07-06 14:40:32.000000 visionscript-0.0.2/banner.png
--rw-r--r--   0 james      (501) staff       (20)      171 2023-07-06 23:02:32.000000 visionscript-0.0.2/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-08 09:35:39.541308 visionscript-0.0.2/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1337 2023-07-06 22:41:49.000000 visionscript-0.0.2/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.536507 visionscript-0.0.2/tests/
--rw-r--r--   0 james      (501) staff       (20)       53 2023-07-08 06:32:08.000000 visionscript-0.0.2/tests/classify_image.vic
--rw-r--r--   0 james      (501) staff       (20)       46 2023-07-06 23:35:58.000000 visionscript-0.0.2/tests/find_in_images.vic
--rw-r--r--   0 james      (501) staff       (20)       63 2023-07-08 06:31:57.000000 visionscript-0.0.2/tests/load_detect_save.vic
--rw-r--r--   0 james      (501) staff       (20)       97 2023-07-08 06:31:57.000000 visionscript-0.0.2/tests/replace_in_images.vic
--rw-r--r--   0 james      (501) staff       (20)       49 2023-07-08 06:32:08.000000 visionscript-0.0.2/tests/segment_image.vic
--rw-r--r--   0 james      (501) staff       (20)      602 2023-07-08 07:07:01.000000 visionscript-0.0.2/tests/test.py
--rw-r--r--   0 james      (501) staff       (20)       31 2023-07-06 23:35:53.000000 visionscript-0.0.2/tests/train_od.vic
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.538646 visionscript-0.0.2/visionscript/
--rw-r--r--   0 james      (501) staff       (20)       55 2023-07-08 09:35:31.000000 visionscript-0.0.2/visionscript/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3141 2023-07-07 23:12:56.000000 visionscript-0.0.2/visionscript/grammar.py
--rw-r--r--   0 james      (501) staff       (20)    38745 2023-07-08 09:35:22.000000 visionscript-0.0.2/visionscript/lang.py
--rw-r--r--   0 james      (501) staff       (20)     3743 2023-07-08 09:05:17.000000 visionscript-0.0.2/visionscript/notebook.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.540764 visionscript-0.0.2/visionscript/std/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/caption.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/classify.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/detect.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/label.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/segment.py
--rw-r--r--   0 james      (501) staff       (20)        0 2023-07-06 16:15:17.000000 visionscript-0.0.2/visionscript/std/train.py
--rw-r--r--   0 james      (501) staff       (20)     1655 2023-07-06 22:30:51.000000 visionscript-0.0.2/visionscript/usage.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-08 09:35:39.539807 visionscript-0.0.2/visionscript.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6374 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      733 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       56 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      225 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2023-07-08 09:35:39.000000 visionscript-0.0.2/visionscript.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.172846 visionscript-0.0.3/
+-rw-r--r--   0 james      (501) staff       (20)     3167 2023-07-10 10:58:12.000000 visionscript-0.0.3/.gitignore
+-rw-r--r--   0 james      (501) staff       (20)      188 2023-07-08 12:17:56.000000 visionscript-0.0.3/CITATION.cff
+-rw-r--r--   0 james      (501) staff       (20)       16 2023-07-06 16:15:17.000000 visionscript-0.0.3/CNAME
+-rw-r--r--   0 james      (501) staff       (20)     6604 2023-07-10 14:58:55.000000 visionscript-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-07-06 23:02:16.000000 visionscript-0.0.3/CONTRIBUTORS.md
+-rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.3/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 16:15:17.000000 visionscript-0.0.3/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)      297 2023-07-09 16:59:36.000000 visionscript-0.0.3/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-10 18:00:26.172622 visionscript-0.0.3/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     4867 2023-07-10 15:17:12.000000 visionscript-0.0.3/README.md
+-rw-r--r--   0 james      (501) staff       (20)      288 2023-07-10 18:00:18.000000 visionscript-0.0.3/requirements.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-10 18:00:26.172910 visionscript-0.0.3/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1757 2023-07-10 12:24:17.000000 visionscript-0.0.3/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.165012 visionscript-0.0.3/tests/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-08 07:38:48.000000 visionscript-0.0.3/tests/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)       53 2023-07-08 06:32:08.000000 visionscript-0.0.3/tests/classify_image.vic
+-rw-r--r--   0 james      (501) staff       (20)       46 2023-07-06 23:35:58.000000 visionscript-0.0.3/tests/find_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       63 2023-07-08 06:31:57.000000 visionscript-0.0.3/tests/load_detect_save.vic
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-07-08 06:31:57.000000 visionscript-0.0.3/tests/replace_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       49 2023-07-08 06:32:08.000000 visionscript-0.0.3/tests/segment_image.vic
+-rw-r--r--   0 james      (501) staff       (20)      602 2023-07-08 07:07:01.000000 visionscript-0.0.3/tests/test.py
+-rw-r--r--   0 james      (501) staff       (20)       31 2023-07-06 23:35:53.000000 visionscript-0.0.3/tests/train_od.vic
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.167714 visionscript-0.0.3/visionscript/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 13:30:07.000000 visionscript-0.0.3/visionscript/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)       55 2023-07-10 12:28:10.000000 visionscript-0.0.3/visionscript/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3343 2023-07-10 17:51:02.000000 visionscript-0.0.3/visionscript/cloud.py
+-rw-r--r--   0 james      (501) staff       (20)     3310 2023-07-10 13:00:15.000000 visionscript-0.0.3/visionscript/grammar.py
+-rw-r--r--   0 james      (501) staff       (20)    45539 2023-07-10 17:09:28.000000 visionscript-0.0.3/visionscript/lang.py
+-rw-r--r--   0 james      (501) staff       (20)     5753 2023-07-10 16:54:18.000000 visionscript-0.0.3/visionscript/notebook.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.170948 visionscript-0.0.3/visionscript/static/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 09:24:19.000000 visionscript-0.0.3/visionscript/static/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)      814 2023-07-09 23:12:47.000000 visionscript-0.0.3/visionscript/static/examples.js
+-rw-r--r--   0 james      (501) staff       (20)     7404 2023-07-10 08:38:39.000000 visionscript-0.0.3/visionscript/static/functions.js
+-rw-r--r--   0 james      (501) staff       (20)    31429 2023-07-10 16:49:09.000000 visionscript-0.0.3/visionscript/static/main.js
+-rw-r--r--   0 james      (501) staff       (20)     6645 2023-07-10 12:14:12.000000 visionscript-0.0.3/visionscript/static/styles.css
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.172152 visionscript-0.0.3/visionscript/templates/
+-rw-r--r--   0 james      (501) staff       (20)     3583 2023-07-08 11:14:46.000000 visionscript-0.0.3/visionscript/templates/deployintro.html
+-rw-r--r--   0 james      (501) staff       (20)     4574 2023-07-08 11:22:00.000000 visionscript-0.0.3/visionscript/templates/index.html
+-rw-r--r--   0 james      (501) staff       (20)     4505 2023-07-10 12:18:15.000000 visionscript-0.0.3/visionscript/templates/notebook.html
+-rw-r--r--   0 james      (501) staff       (20)     2216 2023-07-08 10:29:01.000000 visionscript-0.0.3/visionscript/usage.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.168923 visionscript-0.0.3/visionscript.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      949 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       56 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      294 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       13 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/top_level.txt
```

### Comparing `visionscript-0.0.2/LICENSE` & `visionscript-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.2/PKG-INFO` & `visionscript-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 Metadata-Version: 2.1
 Name: visionscript
-Version: 0.0.2
+Version: 0.0.3
 Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
 Home-page: https://github.com/capjamesg/visionscript
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-![VisionScript banner](banner.png)
+![A VisionScript Notebook counting people in an image](https://raw.githubusercontent.com/capjamesg/visionscript/main/notebook.png)
 
 # VisionScript
 
 [VisionScript](https://visionscript.dev) is an abstract programming language for doing common computer vision tasks, fast.
 
 VisionScript is built in Python, offering a simple syntax for running object detection, classification, and segmentation models. [Read the documentation](https://visionscript.dev/docs/).
 
-## Get Started
+## Get Started 🚀
 
 First, install VisionScript:
 
-```
+```bash
 pip install visionscript
 ```
 
 You can then run VisionScript using:
 
-```
-vscript
+```bash
+visionscript --repl
 ```
 
 This will open a VisionScript REPL in which you can type commands.
 
-## Run a File
+### Run a File 📁
 
 To run a VisionScript file, use:
 
-```
-vscript ./your_file.vic
+```bash
+visionscript ./your_file.vic
 ```
 
-## Use VisionScript in a Notebook
+### Use VisionScript in a Notebook 📓
 
 VisionScript offers an interactive web notebook through which you can run VisionScript code.
 
 To use the notebook, run:
 
-```
-vscript notebook
+```bash
+visionscript --notebook
 ```
 
 This will open a notebook in your browser. Notebooks are ephermal. You will need to copy your code to a file to save it.
 
-## Quickstart
+## Quickstart 🚀
 
 ### Find people in an image using object detection
 
 ```
 Load["./photo.jpg"]
 Detect["person"]
 Say[]
 ```
 
 ### Find people in all images in a folder using object detection
 
 ```
-IN["./images"]
+In["./images"]
     Detect["person"]
     Say[]
 ```
 
 ### Replace people in a photo with an emoji
 
 ```
@@ -89,67 +89,37 @@
 ### Classify an image
 
 ```
 Load["./photo.jpg"]
 Classify["apple", "banana"]
 ```
 
-## Installation
+## Installation 👷
 
 To install VisionScript, clone this repository and run `pip install -r requirements.txt`.
 
 Then, make a file ending in `.vic` in which to write your VisionScript code.
 
 When you have written your code, run:
 
-```
+```bash
 python3 lang.py --file ./your_file.vic
 ```
 
 ### Run in debug mode
 
 Running in debug mode shows the full Abstract Syntax Tree (AST) of your code.
 
-```
+```bash
 python3 lang.py --file ./your_file.vic --debug
 ```
 
 Debug mode is useful for debugging code while adding new features to the VisionScript language.
 
-## Documentation
-
-- `Load["./abbey.jpg"]` -> Load the image
-- `Size[]` -> Get the size of the image
-- `Say[]` -> Say the result of the last function
-- `Detect["person"]` -> Detect the person
-- `Replace["emoji.png"]` -> Replace the person with black image
-- `Cutout[]` -> Cutout the last detections
-- `Count[]` -> Count the last detections
-- `CountInRegion[0, 0, 500, 500]` -> Count the last detections in the region (x1, y1, x2, y2)
-- `Classify["cat", "dog"]` -> Classify the image in the provided categories
-- `Save["./abbey2.jpg"]` -> Save the last image
-- `Show[]` -> Show the last image
-  - If you have run inference, this will plot inference results on the image with which you are working.
-- `x = 1` -> Set the variable x to 1
-- `True` and `False`: Booleans
-- `If[Statement]`: If the statement is true, run the next line (the only value that evaluates to `False` is `False` right now so this is not yet useful).
-- `x == y`: Test for equality. Check if x is equal to y.
-- `In["./images"]`: Load all images in the `./images` folder
-
-
-## Core Libraries Used
-
-- CLIP
-- YOLOv8
-- FastSAM
-- [supervision](https://github.com/roboflow/supervision)
-- PIL
-- Lark for lexing
-
-## Inspiration
+## Inspiration 🌟
 
 The inspiration behind this project was to build a simple way of doing one-off tasks.
 
 Consider a scenario where you want to run zero-shot classification on a folder of images. With VisionScript, you can do this in two lines of code:
 
 ```
 In["./images"]
@@ -182,15 +152,15 @@
 Say[]
 ```
 
 Here, `Size[]` and `Say[]` do not have any arguments. Rather, they use the last input. Wolfram Alpha has a feature to get the last input using `%`. VisionScript uses the same concept, but with a twist.
 
 Indeed, `Size[]` and `Say[]` don't accept any arguments.
 
-## Developer Setup
+## Developer Setup 🛠
 
 If you want to add new features or fix bugs in the VisionScript language, you will need to set up a developer environment.
 
 To do so, clone the language repository:
 
 ```bash
 git clone https://github.com/capjamesg/VisionScript
@@ -215,25 +185,21 @@
 
 For now, you can run all test cases using the following command:
 
 ```bash
 python3 test.py
 ```
 
-### Code Organization
-
-- `lang.py`: Core language code.
-- `test.py`: Run tests.
-- `usage.py`: Variables referenced for usage instructions in `lang.py`.
-- `grammar.py`: The VisionScript grammar.
-- `tests/`: VisionScript tests.
-
-## Supported Models
+## Supported Models 📚
 
 VisionScript provides abstract wrappers around:
 
 - [CLIP](https://github.com/openai/clip) by OpenAI (Classification)
 - [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) (Object Detection Training, Segmentation Training)
 - [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM) by CASIA-IVA-Lab. (Segmentation)
-- GroundedSAM (Object Detection, Segmentation)
-- BLIP (Caption Generation)
-- ViT (Classification Training)
+- [GroundedSAM](https://docs.autodistill.com/base_models/groundedsam/) (Object Detection, Segmentation)
+- [BLIP](https://github.com/salesforce/BLIP) (Caption Generation)
+- [ViT](https://github.com/autodistill/autodistill-vit) (Classification Training)
+
+## License 📝
+
+This project is licensed under an [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `visionscript-0.0.2/README.md` & `visionscript-0.0.3/visionscript.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-![VisionScript banner](banner.png)
+Metadata-Version: 2.1
+Name: visionscript
+Version: 0.0.3
+Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
+Home-page: https://github.com/capjamesg/visionscript
+Author: capjamesg
+Author-email: jamesg@jamesg.blog
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+![A VisionScript Notebook counting people in an image](https://raw.githubusercontent.com/capjamesg/visionscript/main/notebook.png)
 
 # VisionScript
 
 [VisionScript](https://visionscript.dev) is an abstract programming language for doing common computer vision tasks, fast.
 
 VisionScript is built in Python, offering a simple syntax for running object detection, classification, and segmentation models. [Read the documentation](https://visionscript.dev/docs/).
 
-## Get Started
+## Get Started 🚀
 
 First, install VisionScript:
 
-```
+```bash
 pip install visionscript
 ```
 
 You can then run VisionScript using:
 
-```
-vscript
+```bash
+visionscript --repl
 ```
 
 This will open a VisionScript REPL in which you can type commands.
 
-## Run a File
+### Run a File 📁
 
 To run a VisionScript file, use:
 
-```
-vscript ./your_file.vic
+```bash
+visionscript ./your_file.vic
 ```
 
-## Use VisionScript in a Notebook
+### Use VisionScript in a Notebook 📓
 
 VisionScript offers an interactive web notebook through which you can run VisionScript code.
 
 To use the notebook, run:
 
-```
-vscript notebook
+```bash
+visionscript --notebook
 ```
 
 This will open a notebook in your browser. Notebooks are ephermal. You will need to copy your code to a file to save it.
 
-## Quickstart
+## Quickstart 🚀
 
 ### Find people in an image using object detection
 
 ```
 Load["./photo.jpg"]
 Detect["person"]
 Say[]
 ```
 
 ### Find people in all images in a folder using object detection
 
 ```
-IN["./images"]
+In["./images"]
     Detect["person"]
     Say[]
 ```
 
 ### Replace people in a photo with an emoji
 
 ```
@@ -74,67 +89,37 @@
 ### Classify an image
 
 ```
 Load["./photo.jpg"]
 Classify["apple", "banana"]
 ```
 
-## Installation
+## Installation 👷
 
 To install VisionScript, clone this repository and run `pip install -r requirements.txt`.
 
 Then, make a file ending in `.vic` in which to write your VisionScript code.
 
 When you have written your code, run:
 
-```
+```bash
 python3 lang.py --file ./your_file.vic
 ```
 
 ### Run in debug mode
 
 Running in debug mode shows the full Abstract Syntax Tree (AST) of your code.
 
-```
+```bash
 python3 lang.py --file ./your_file.vic --debug
 ```
 
 Debug mode is useful for debugging code while adding new features to the VisionScript language.
 
-## Documentation
-
-- `Load["./abbey.jpg"]` -> Load the image
-- `Size[]` -> Get the size of the image
-- `Say[]` -> Say the result of the last function
-- `Detect["person"]` -> Detect the person
-- `Replace["emoji.png"]` -> Replace the person with black image
-- `Cutout[]` -> Cutout the last detections
-- `Count[]` -> Count the last detections
-- `CountInRegion[0, 0, 500, 500]` -> Count the last detections in the region (x1, y1, x2, y2)
-- `Classify["cat", "dog"]` -> Classify the image in the provided categories
-- `Save["./abbey2.jpg"]` -> Save the last image
-- `Show[]` -> Show the last image
-  - If you have run inference, this will plot inference results on the image with which you are working.
-- `x = 1` -> Set the variable x to 1
-- `True` and `False`: Booleans
-- `If[Statement]`: If the statement is true, run the next line (the only value that evaluates to `False` is `False` right now so this is not yet useful).
-- `x == y`: Test for equality. Check if x is equal to y.
-- `In["./images"]`: Load all images in the `./images` folder
-
-
-## Core Libraries Used
-
-- CLIP
-- YOLOv8
-- FastSAM
-- [supervision](https://github.com/roboflow/supervision)
-- PIL
-- Lark for lexing
-
-## Inspiration
+## Inspiration 🌟
 
 The inspiration behind this project was to build a simple way of doing one-off tasks.
 
 Consider a scenario where you want to run zero-shot classification on a folder of images. With VisionScript, you can do this in two lines of code:
 
 ```
 In["./images"]
@@ -167,15 +152,15 @@
 Say[]
 ```
 
 Here, `Size[]` and `Say[]` do not have any arguments. Rather, they use the last input. Wolfram Alpha has a feature to get the last input using `%`. VisionScript uses the same concept, but with a twist.
 
 Indeed, `Size[]` and `Say[]` don't accept any arguments.
 
-## Developer Setup
+## Developer Setup 🛠
 
 If you want to add new features or fix bugs in the VisionScript language, you will need to set up a developer environment.
 
 To do so, clone the language repository:
 
 ```bash
 git clone https://github.com/capjamesg/VisionScript
@@ -200,25 +185,21 @@
 
 For now, you can run all test cases using the following command:
 
 ```bash
 python3 test.py
 ```
 
-### Code Organization
-
-- `lang.py`: Core language code.
-- `test.py`: Run tests.
-- `usage.py`: Variables referenced for usage instructions in `lang.py`.
-- `grammar.py`: The VisionScript grammar.
-- `tests/`: VisionScript tests.
-
-## Supported Models
+## Supported Models 📚
 
 VisionScript provides abstract wrappers around:
 
 - [CLIP](https://github.com/openai/clip) by OpenAI (Classification)
 - [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) (Object Detection Training, Segmentation Training)
 - [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM) by CASIA-IVA-Lab. (Segmentation)
-- GroundedSAM (Object Detection, Segmentation)
-- BLIP (Caption Generation)
-- ViT (Classification Training)
+- [GroundedSAM](https://docs.autodistill.com/base_models/groundedsam/) (Object Detection, Segmentation)
+- [BLIP](https://github.com/salesforce/BLIP) (Caption Generation)
+- [ViT](https://github.com/autodistill/autodistill-vit) (Classification Training)
+
+## License 📝
+
+This project is licensed under an [MIT license](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `visionscript-0.0.2/setup.py` & `visionscript-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 import setuptools
 from setuptools import find_packages
 import re
+import os
+import subprocess
 
 with open("./visionscript/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("./requirements.txt", "r") as f:
     reqs = f.read().splitlines()
+
+def install_fast_sam_for_segmentation() -> None:
+    commands = [
+        "pip install -r requirements.txt",
+        "curl" # install weights
+    ]
+
+    HOME = os.getcwd()
+
+    subprocess.run(f"cd {HOME} && git clone https://github.com/CASIA-IVA-Lab/FastSAM")
+
+    for command in commands:
+        subprocess.run(f"cd {HOME} && {command}", shell=True)
+
     
 setuptools.setup(
     name="visionscript",
     version=version,
     author="capjamesg",
     author_email="jamesg@jamesg.blog",
     description="VisionScript is an abstract programming language for doing common computer vision tasks, fast.",
@@ -35,7 +51,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
+
+# install_fast_sam_for_segmentation()
```

### Comparing `visionscript-0.0.2/tests/test.py` & `visionscript-0.0.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.2/visionscript/grammar.py` & `visionscript-0.0.3/visionscript/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 grammar = """
 start: (expr | EOL | EOF | " ")*
 
-expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | make | run | isita | find | describe | import | rotate | getcolours | getcolors | get_text | greyscale | select | paste | pasterandom | resize | blur | literal | setbrightness | search | similarity | readqr | reset | negate | BOOL | INT | equality | not_equality | input) (EOL | EOF | " ")
+expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | make | run | isita | find | describe | import | rotate | getcolours | getcolors | get_text | greyscale | select | paste | pasterandom | resize | blur | literal | setbrightness | search | similarity | readqr | reset | negate | BOOL | INT | equality | not_equality | input | deploy | getedges | setconfidence)
 classify: "Classify" "[" STRING ("," STRING)* "]"
 var: variable "=" expr
 replace: "Replace" "[" STRING "]"
 use: "Use" "[" STRING "]"
 load: "Load" "[" (STRING | input) "]" | "Load" ("[" "]")?
 save: "Save" "[" STRING "]"
 say: "Say" "[" STRING "]" | "Say" ("[" "]")?
 get_text: "GetText" ("[" "]")?
 greyscale: "Greyscale" ("[" "]")?
 search: "Search" "[" STRING "]"
+deploy: "Deploy" "[" STRING "]"
+getedges: "GetEdges"  ("[" "]")?
 describe: "Describe" ("[" "]")?
 readqr: "ReadQR" ("[" "]")?
-rotate: "Rotate" "[" INT "]"
+setconfidence: "SetConfidence" "[" INT "]"
+rotate: "Rotate" "[" (INT | STRING) "]"
 resize: "Resize" "[" INT "," INT "]"
 getcolors: "GetColors" ("[" "]")? | "GetColors" "[" INT "]"
 getcolours: "GetColours" ("[" "]")? | "GetColours" "[" INT "]"
 isita: "Is it a " (("," STRING)* | ("or" STRING)*)? EOL
 find: "Find" "[" STRING "]"
 args: ((STRING | INT | expr) ("," (STRING | INT | expr))*) | (STRING | INT | expr)?
 make: "Make" literal ("[" args "]")? EOL (INDENT expr+)* EOL
@@ -41,31 +44,31 @@
 blur: "Blur" ("[" "]")?
 similarity: "Similarity" ("[" INT "]")?
 get: "Get" "[" INT "]" EOL
 list: "[" ((STRING | INT | expr) "," | (STRING | INT | expr) )* "]" EOL
 help: "Help" "[" STRING "]"
 end: "End" ("[" "]")?
 countinregion: "CountInRegion" "[" INT "," INT "," INT "," INT "]"
-detect: "Detect" "[" STRING ("," STRING)* "]" | "Detect" ("[" "]")?
+detect: "Detect" "[" input "]" | "Detect" "[" STRING ("," STRING)* "]" | "Detect" ("[" "]")?
 segment: "Segment" "[" STRING "]"
 else: "Else"
-in: "IN" "[" STRING "]" EOL (INDENT expr+)*
-if: "IF" "[" (expr+)* "]" EOL (INDENT expr+)* (EOL | EOF | " ") (else EOL (INDENT expr+)* (EOL | EOF | " "))?
+in: "In" "[" STRING "]" EOL (INDENT expr+)* EOL 
+if: "If" "[" (expr+)* "]" EOL (INDENT expr+)* (EOL | EOF) (else EOL (INDENT expr+)* (EOL | EOF | " "))?
 reset: "Reset" ("[" "]")?
 negate: "Not" "[" expr "]"
 OPERAND: "+" | "-" | "*" | "/"
 equality: (INT | STRING | expr) "==" (INT | STRING | expr)
 not_equality: (INT | STRING | expr) "!=" (INT | STRING | expr)
 train: "Train" "[" STRING "," STRING "]" | "Train" "[" STRING "]"
 label: "Label" "[" STRING "," STRING ("," STRING )*  "]"
 literal: /([a-z][a-zA-Z0-9_]*)/ ( "[" (STRING | INT | expr) ("," (STRING | INT | expr))* "]" )? | /([a-z][a-zA-Z0-9_]*)/ "[" "]"
 variable: /[a-zA-Z_][a-zA-Z0-9_]*/
 comment: "#"
 EOL: "\\n"
 EOF: "\\Z"
 INT: /-?\d+/
-INDENT: "    "
+INDENT: "    " | "\\t"
 BOOL: "True" | "False"
 %import common.ESCAPED_STRING -> STRING
 %import common.WS_INLINE
 %ignore WS_INLINE
 """
```

### Comparing `visionscript-0.0.2/visionscript/lang.py` & `visionscript-0.0.3/visionscript/lang.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 import math
 import mimetypes
 import os
 import random
 import string
 import sys
 import tempfile
-import lark
 
 import click
 import cv2
+import lark
 import numpy as np
 import supervision as sv
 from lark import Lark, UnexpectedCharacters, UnexpectedToken
 from PIL import Image
 from spellchecker import SpellChecker
+
 from visionscript.grammar import grammar
 from visionscript.usage import (USAGE, language_grammar_reference,
                                 lowercase_language_grammar_reference)
 
 spell = SpellChecker()
 
 parser = Lark(grammar)
@@ -115,34 +116,43 @@
     "getcolors": "getcolours",
 }
 
 
 def map_alias_to_underlying_function(alias):
     return aliased_functions.get(alias, alias)
 
+
 def init_state():
     return {
         "functions": {},
         "last_loaded_image": None,
         "last_loaded_image_name": None,
         "last": None,
         "last_function_type": None,
         "last_function_args": None,
         "image_stack": [],
         "detections_stack": [],
         "history": [],
         "search_index_stack": [],
         # "current_active_model": None,
         "output": None,
+        "input_variables": {},
+        "last_classes": [],
+        "confidence": 50,
     }
 
+
 class VisionScript:
+    """
+    A VisionScript program.
+    """
     def __init__(self, notebook=False):
         self.state = init_state()
         self.notebook = notebook
+        self.code = ""
 
         self.function_calls = {
             "load": lambda x: self.load(x),
             "save": lambda x: self.save(x),
             "classify": lambda x: self.classify(x),
             "size": lambda x: self.size(x),
             "say": lambda x: self.say(x),
@@ -187,17 +197,20 @@
             "similarity": lambda x: self.similarity(x),
             "readqr": lambda x: self.read_qr(x),
             "reset": lambda x: self.reset(x),
             "negate": lambda x: self.negate(x),
             "equality": lambda x: self.equality(x),
             "not_equality": lambda x: not self.equality(x),
             "input": lambda x: self.input_(x),
+            "deploy": lambda x: self.deploy(x),
+            "getedges": lambda x: self.get_edges(x),
         }
 
     def input_(self, key):
+        self.state["input_variables"][key] = "image"
         if self.state.get(literal_eval(key)) is not None:
             return self.state[literal_eval(key)]
         else:
             print(f"Input {key} does not exist.")
             exit()
 
     def equality(self, args):
@@ -209,44 +222,52 @@
     def reset(self, _):
         self.state = init_state()
 
     def set_state(self, key, value):
         self.state[key] = value
 
     def make(self, args):
-        print(args, "args")
+        """
+        Declare a function.
+        """
         function_name = args[0].children[0].value.strip()
 
         function_body = lark.Tree("expr", args[1:])
 
         self.state["functions"][function_name] = function_body
 
-        print(f"Function {function_name} created.")
+    def set_confidence(self, args):
+        """
+        Set the confidence level for use in filtering detections.
+        """
+        self.state["confidence"] = args[0]
 
     def load(self, filename):
+        """
+        Load an image or folder of images into state.
+        """
         import requests
         import validators
 
         if isinstance(filename, np.ndarray):
-            self.state["last_loaded_image"] = filename
+            self.state["image_stack"].append(filename)
             # save file
             import uuid
+
             name = str(uuid.uuid4()) + ".png"
             cv2.imwrite(name, filename)
 
             self.state["last_loaded_image_name"] = name
 
             return filename
 
         # if is dir, load all images
         if filename and os.path.isdir(filename):
             image_filenames = [filename + "/" + item for item in os.listdir(filename)]
 
-            print(image_filenames)
-
             for image_filename in image_filenames:
                 self.load(image_filename)
 
             return
 
         if filename and validators.url(filename):
             response = requests.get(filename)
@@ -269,23 +290,32 @@
             with tempfile.NamedTemporaryFile(delete=True) as f:
                 f.write(response.content)
                 filename = f.name
 
         if self.state.get("ctx") and self.state["ctx"].get("in"):
             filename = self.state["ctx"]["active_file"]
 
+        # make filename safe
+        # from werkzeug.utils import secure_filename
+
+        # filename = filename.split("/")[-1]
+
+        # filename = secure_filename(filename)
+
         self.state["last_loaded_image_name"] = filename
 
         return np.array(Image.open(filename).convert("RGB"))[:, :, ::-1]
 
     def size(self, _):
-        return self.state["last_loaded_image"].size
+        return self.state["image_stack"][-1].shape[:2]
 
     def import_(self, args):
-        # execute code from a file
+        """
+        Import a module from another file.
+        """
         # this will update self.state for the entire script
 
         file_name = "".join(
             [
                 letter
                 for letter in args
                 if letter.isalpha() or letter == "-" or letter.isdigit()
@@ -296,39 +326,58 @@
             code = f.read()
 
         tree = parser.parse(code.strip() + "\n")
 
         self.parse_tree(tree)
 
     def cutout(self, _):
+        """
+        Cut out a detection from an image.
+        """
         x1, y1, x2, y2 = self.state["last"].xyxy[0]
-        image = self.state["last_loaded_image"]
+        image = self.state["image_stack"][-1]
         cropped_image = image.crop((x1, y1, x2, y2))
         self.state["image_stack"].append(cropped_image)
-        self.state["last_loaded_image"] = cropped_image
 
     def select(self, args):
+        """
+        Select a detection from a sv.Detections object.
+        """
         # if detect, select from detections
-        if self.state.get("last_function_type", None) in ("detect", "segment", "classify"):
+        if self.state.get("last_function_type", None) in (
+            "detect",
+            "segment",
+            "classify",
+        ):
             detections = self.state["last"]
 
+            detections = detections[detections.confidence > self.state["confidence"]]
+
             if len(args) == 0:
                 self.state["last"] = detections
             else:
                 self.state["last"] = detections[args[0]]
 
     def paste(self, args):
+        """
+        Paste an image onto another image.
+        """
         x, y = args
-        self.state["last_loaded_image"].paste(self.state["image_stack"][-1], (x, y))
+        self.state["image_stack"].append(
+            self.state["image_stack"][-2].paste(self.state["image_stack"][-1], (x, y))
+        )
 
     def resize(self, args):
+        """
+        Resize an image.
+        """
         width, height = args
-        image = self.state["last_loaded_image"]
-        image = image.resize((width, height))
-        self.state["last_loaded_image"] = image
+        image = self.state["image_stack"][-1]
+        image = cv2.resize(image, (width, height))
+        self.state["image_stack"].append(image)
 
     def _create_index(self):
         import faiss
 
         index = faiss.IndexFlatL2(512)
 
         self.state["search_index_stack"].append(index)
@@ -337,25 +386,32 @@
 
     def _add_to_index(self, image):
         index = self.state["search_index_stack"][-1]
 
         index.add(image)
 
     def search(self, label):
+        """
+        Search for an image using a text label or image.
+
+        On first run, this will create an index of all images on the loaded image stack.
+        """
         # embed
         import clip
         import torch
 
         device = "cuda" if torch.cuda.is_available() else "cpu"
         model, preprocess = clip.load("ViT-B/32", device=device)
 
         with torch.no_grad():
             # if label is a filename, load image
-            if label.startswith("./") and os.path.exists(label):
-                comparator = self.load(label)
+            if os.path.exists(label):
+                comparator = preprocess(Image.open(label)).unsqueeze(0).to(device)
+
+                comparator = model.encode_image(comparator)
             else:
                 comparator = clip.tokenize([label]).to(device)
 
                 comparator = model.encode_text(comparator)
 
             if len(self.state["search_index_stack"]) == 0:
                 self._create_index()
@@ -374,91 +430,145 @@
         results = index.search(comparator, 5)
 
         image_names = []
 
         for result in results[1][0]:
             image_names.append(self.state["image_stack"][result])
 
+        if len(self.state["image_stack"]) < 5:
+            image_names = image_names[: len(self.state["image_stack"])]
+
         return image_names
 
     def pasterandom(self, _):
+        """
+        Paste the most recent image in a random position on the previously most recent image.
+        """
         x, y = []
 
         while True:
-            x, y = random.randint(
-                0, self.state["last_loaded_image"].size[0]
-            ), random.randint(0, self.state["last_loaded_image"].size[1])
+            x, y = random.randint(0, self.state["image_stack"].size[0]), random.randint(
+                0, self.state["image_stack"].size[1]
+            )
 
             if len(self.state["last"].xyxy) == 0:
                 break
 
             for bbox in self.state["last"].xyxy:
                 x1, y1, x2, y2 = bbox
 
                 if x1 <= x <= x2 and y1 <= y <= y2:
                     continue
 
             break
 
-        self.state["last_loaded_image"].paste(self.state["image_stack"][-1], (x, y))
+        self.state["image_stack"][-1] = self.state["image_stack"][-2].paste(
+            self.state["image_stack"][-1], (x, y)
+        )
 
     def save(self, filename):
-        self.state["last_loaded_image"].save(filename)
+        """
+        Save an image to a file.
+        """
+        self.state["image_stack"].save(filename)
 
     def count(self, args):
+        """
+        Count the number of detections in a sv.Detections object.
+        """
         if len(args) == 0:
             return len(self.state["last"].xyxy)
         else:
             return len(
                 [item for item in self.state["last"].class_id if item == args[0]]
             )
 
     def greyscale(self, _):
-        image = self.state["last_loaded_image"]
+        """
+        Turn an image to greyscale.
+        """
+        image = self.state["image_stack"][-1]
         # turn to bgr
         image = image[:, :, ::-1].copy()
         image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
         self.state["image_stack"].append(image)
         # save to test.png
-        
-        self.state["last_loaded_image"] = image
+
+        self.state["image_stack"].append(image)
         self.state["output"] = image
 
+    def deploy(self, app_name):
+        """
+        Deploy a script to a VisionScript Cloud web app.
+        """
+        # make POST to http://localhost:6999/create
+        import string
+
+        import requests
+
+        app_slug = app_name.translate(
+            str.maketrans("", "", string.punctuation.replace("-", ""))
+        )
+
+        response = requests.post(
+            "http://localhost:6999/create",
+            json={
+                "api_key": "test",
+                "title": app_name,
+                "slug": app_slug,
+                "script": self.code,
+                "variables": self.state["input_variables"],
+            },
+        )
+
+        if response.ok:
+            return "Deployed successfully to http://localhost:6999/app"
+
+        return "Error deploying."
+
     def get_text(self, _):
+        """
+        Use OCR to get text from an image.
+        """
         import easyocr
 
         reader = easyocr.Reader(["en"])
-        result = reader.readtext(self.state["last_loaded_image_name"])
+        result = reader.readtext(self.state["last_loaded_image_name"], detail=0)
 
         return result
 
     def rotate(self, args):
-        image = self.state["last_loaded_image"]
+        """
+        Rotate an image.
+        """
+        image = self.state["image_stack"][-1]
         # load into cv2
         args = int(args)
         if args == 90:
             image = cv2.rotate(image, cv2.ROTATE_90_CLOCKWISE)
         elif args == 180:
             image = cv2.rotate(image, cv2.ROTATE_180)
         elif args == 270:
             image = cv2.rotate(image, cv2.ROTATE_90_COUNTERCLOCKWISE)
         else:
             image = image
 
-        self.state["last_loaded_image"] = image
         self.state["output"] = image
         self.state["image_stack"].append(image)
 
     def getcolours(self, k):
+        """
+        Get the most common colours in an image.
+        """
         if not k:
             k = 1
 
         from sklearn.cluster import KMeans
 
-        image = self.state["last_loaded_image"]
+        image = self.state["image_stack"][-1]
 
         image = np.array(image)
 
         image = image.reshape((image.shape[0] * image.shape[1], 3))
 
         clt = KMeans(n_clusters=k)
 
@@ -479,25 +589,31 @@
                 continue
 
         self.state["last"] = human_readable_colours[:k]
 
         return human_readable_colours[:k]
 
     def detect(self, classes):
+        """
+        Run object detection on an image.
+        """
         logging.disable(logging.CRITICAL)
 
-        if self.state.get("current_active_model") and self.state["current_active_model"].lower() == "groundingdino":
-            from autodistill_grounding_dino import GroundingDINO
+        if (
+            self.state.get("current_active_model")
+            and self.state["current_active_model"].lower() == "groundingdino"
+        ):
             from autodistill.detection import CaptionOntology
+            from autodistill_grounding_dino import GroundingDINO
 
             mapped_items = {item: item for item in classes}
 
             base_model = GroundingDINO(CaptionOntology(mapped_items))
 
-            inference_results = base_model.predict(self.state["last_loaded_image"])
+            inference_results = base_model.predict(self.state["last_loaded_image_name"])
         else:
             from ultralytics import YOLO
 
             # model name should be only letters and - and numbers
 
             model_name = self.state.get("current_active_model", "yolov8n")
 
@@ -505,20 +621,23 @@
                 [
                     letter
                     for letter in model_name
                     if letter.isalpha() or letter == "-" or letter.isdigit()
                 ]
             )
 
-            if self.state.get("model") and self.state["current_active_model"].lower() == "yolo":
+            if (
+                self.state.get("model")
+                and self.state["current_active_model"].lower() == "yolo"
+            ):
                 model = model
             else:
                 model = YOLO(model_name + ".pt")
 
-            inference_results = model(self.state["last_loaded_image"])[0]
+            inference_results = model(self.state["image_stack"][-1])[0]
 
             logging.disable(logging.NOTSET)
 
             # Inference
             results = sv.Detections.from_yolov8(inference_results)
 
         inference_classes = inference_results.names
@@ -527,18 +646,22 @@
             classes = inference_classes
 
         classes = [key for key, item in inference_classes.items() if item in classes]
 
         results = results[np.isin(results.class_id, classes)]
 
         self.state["detections_stack"].append(results)
+        self.state["last_classes"] = [inference_classes[item] for item in classes]
 
         return results
 
     def classify(self, labels):
+        """
+        Classify an image using provided labels.
+        """
         image = self.state["last"]
 
         if self.state.get("model") and self.state["model"].__class__.__name__ == "ViT":
             model = self.state["model"]
 
             results = model.predict(image).get_top_k(1)
 
@@ -552,17 +675,16 @@
         ):
             model = self.state["model"]
 
             results = model.predict(image)
 
             return results
 
-        if "clip" not in sys.modules:
-            import clip
-            import torch
+        import clip
+        import torch
 
         device = "cuda" if torch.cuda.is_available() else "cpu"
         model, preprocess = clip.load("ViT-B/32", device=device)
 
         image = (
             preprocess(Image.open(self.state["last_loaded_image_name"]))
             .unsqueeze(0)
@@ -580,19 +702,27 @@
             label_name = labels[label_idx]
 
         self.state["output"] = label_name
 
         return label_name
 
     def segment(self, text_prompt):
+        """
+        Apply image segmentation and generate segmentation masks.
+        """
         # check for model
-        from fastsam import FastSAM, FastSAMPrompt
+        from .FastSAM.fastsam import FastSAM, FastSAMPrompt
 
         logging.disable(logging.CRITICAL)
-        model = FastSAM("./weights/FastSAM.pt")
+        # get current path
+        import os
+
+        current_path = os.getcwd()
+
+        model = FastSAM(os.path.join(current_path, "weights", "FastSAM.pt"))
 
         DEVICE = "cpu"
         everything_results = model(
             self.state["last_loaded_image_name"],
             device=DEVICE,
             retina_masks=True,
             imgsz=1024,
@@ -617,24 +747,35 @@
                     xyxy=sv.mask_to_xyxy(np.array([mask])),
                     class_id=np.array([0]),
                     confidence=np.array([1]),
                 )
             )
             class_ids.append(0)
 
-        return sv.Detections(
+        detections = sv.Detections(
             mask=np.array([item.mask[0] for item in results]),
             xyxy=np.array([item.xyxy[0] for item in results]),
             class_id=np.array(class_ids),
             confidence=np.array([1]),
         )
 
+        detections = detections[detections.confidence > self.state["confidence"]]
+
+        self.state["detections_stack"].append(detections)
+
+        return detections
+
     def countInRegion(self, x1, y1, x2, y2):
+        """
+        Count the number of detections in a region.
+        """
         detections = self.state["last"]
 
+        detections = detections[detections.confidence > self.state["confidence"]]
+
         xyxy = detections.xyxy
 
         counter = 0
 
         for i in range(len(xyxy)):
             x1_, y1_, x2_, y2_ = xyxy[i]
 
@@ -654,21 +795,23 @@
             )
 
             return statement
 
         return self.state["last"]
 
     def say(self, statement):
-        # if list, say each item
-        # if last item is an image, execute show
+        """
+        Print a statement to the console, or create a text representation of a statement for use
+        in a notebook.
+        """
         if isinstance(self.state["last"], np.ndarray):
             self.show(None)
             return
 
-        if isinstance(self.state["last"], list):
+        if isinstance(self.state["last"], (list, tuple)):
             self.state["output"] = ""
             for item in self.state["last"]:
                 print(item)
                 # if list or tuple, join
                 if isinstance(item, (list, tuple)):
                     item = ", ".join([str(i) for i in item])
 
@@ -698,58 +841,64 @@
 
         if statement:
             print(statement.strip())
 
         self.state["output"] = statement
 
     def blur(self, args):
-        image = self.state["last_loaded_image"]
+        """
+        Blur an image.
+        """
+        image = self.state["image_stack"][-1]
 
         image = cv2.blur(image, (args[0], args[0]))
 
-        self.state["last_loaded_image"] = image
+        self.state["image_stack"].append(image)
 
     def replace(self, color):
+        """
+        Replace a detection or list of detections with an image or color.
+        """
         detections = self.state["last"]
 
+        detections = detections[detections.confidence > self.state["confidence"]]
+
         xyxy = detections.xyxy
 
         if color is not None:
             import webcolors
 
             try:
                 color_to_rgb = webcolors.name_to_rgb(color)
             except ValueError:
                 print(f"Color {color} does not exist.")
                 return
 
-            random_img = np.ones(
-                (int(xyxy[0][2] - xyxy[0][0]), int(xyxy[0][3] - xyxy[0][1]), 3),
-                dtype=np.uint8,
-            )
+            color_to_rgb = np.array(color_to_rgb)
 
-            random_img[:, :] = color_to_rgb
+            print(color_to_rgb, xyxy)
 
-            random_img = Image.fromarray(random_img)
-        else:
-            random_img = np.zeros(
-                (int(xyxy[0][2] - xyxy[0][0]), int(xyxy[0][3] - xyxy[0][1]), 3),
-                dtype=np.uint8,
-            )
+            # convert to bgr
+            color_to_rgb = color_to_rgb[::-1]
 
-            random_img = Image.fromarray(random_img)
+            for i in range(len(xyxy)):
+                x1, y1, x2, y2 = xyxy[i]
 
-        # paste image
-        self.state["last_loaded_image"].paste(
-            random_img, (int(xyxy[0][0]), int(xyxy[0][1]))
-        )
+                # cast all to int
+                x1, y1, x2, y2 = int(x1), int(y1), int(x2), int(y2)
+
+                self.state["image_stack"][-1][y1:y2, x1:x2] = color_to_rgb
 
     def label(self, args):
+        """
+        Label a folder of images using an object detection, classification, or segmentation model.
+
+        Not fully implemented.
+        """
         folder = args[0]
-        model = args[1]
         items = args[2]
 
         if (
             "Detect" in self.state["history"]
             or self.state["current_active_model"] == "groundedsam"
         ):
             from autodistill.detection import CaptionOntology
@@ -761,32 +910,40 @@
         else:
             print("Please specify a model with which to label images.")
             return
 
         base_model.label(folder)
 
     def caption(self, _):
+        """
+        Generate a caption for an image.
+        """
         from transformers import BlipForConditionalGeneration, BlipProcessor
 
         processor = BlipProcessor.from_pretrained(
             "Salesforce/blip-image-captioning-base"
         )
         model = BlipForConditionalGeneration.from_pretrained(
             "Salesforce/blip-image-captioning-base"
         )
 
-        inputs = processor(self.state["last_loaded_image"], return_tensors="pt")
+        inputs = processor(self.state["image_stack"][-1], return_tensors="pt")
 
         out = model.generate(**inputs)
 
         self.state["last"] = processor.decode(out[0], skip_special_tokens=True)
 
         return processor.decode(out[0], skip_special_tokens=True)
 
     def train(self, args):
+        """
+        Train a model on a dataset.
+
+        Not fully implemented.
+        """
         folder = args[0]
         model = args[1]
         # if Detect or Classify run, train
         if "Detect" in self.state["history"] or model == "yolov8":
             if "autodistill_yolov8" not in sys.modules:
                 from autodistill_yolov8 import YOLOv8
 
@@ -803,22 +960,37 @@
             model = base_model.train(folder, "ViT-B/32")
         else:
             print("No training needed.")
             return
 
         self.state["model"] = model
 
+    def get_edges(self, _):
+        """
+        Convert image to greyscale then perform Sobel edge detection.
+        """
+        self.greyscale(_)
+
+        image = self.state["image_stack"][-1]
+
+        sobelxy = cv2.Sobel(image, cv2.CV_64F, 1, 1, ksize=5)
+
+        self.state["image_stack"].append(sobelxy)
+        self.state["output"] = sobelxy
+
     def show(self, _):
-        # get most recent Detect or Segment
+        """
+        Show the image in the notebook or in a new window.
+
+        If a Detect or Segment function was run previously, this function shows the image with the bounding boxes.
+        """
         most_recent_detect_or_segment = None
 
-        for i in range(len(self.state["history"]) - 1, -1, -1):
-            if self.state["history"][i] in ("detect", "segment"):
-                most_recent_detect_or_segment = self.state["history"][i]
-                break
+        if self.state["history"][-2] in ("detect", "segment"):
+            most_recent_detect_or_segment = self.state["history"][-2]
 
         if most_recent_detect_or_segment == "detect":
             annotator = sv.BoxAnnotator()
         elif most_recent_detect_or_segment == "segment":
             annotator = sv.MaskAnnotator()
         else:
             annotator = None
@@ -835,93 +1007,141 @@
             grid_size = math.gcd(len(self.state["last"]), len(self.state["last"]))
 
             if len(self.state["last"]) == len(self.state["detections_stack"]):
                 for image, detections in zip(
                     self.state["last"], self.state["detections_stack"]
                 ):
                     if annotator and detections:
-                        image = annotator.annotate(np.array(image), detections)
+                        image = annotator.annotate(
+                            np.array(image),
+                            detections,
+                            labels=self.state["last_classes"],
+                        )
                     else:
                         image = np.array(image)
 
                     images.append(image)
             else:
                 for image in self.state["last"]:
                     images.append(np.array(image))
 
-            sv.plot_images_grid(
-                images=np.array(images), grid_size=(grid_size, grid_size), size=(12, 12)
-            )
+            if not self.notebook:
+                sv.plot_images_grid(
+                    images=np.array(images),
+                    grid_size=(grid_size, grid_size),
+                    size=(12, 12),
+                )
 
-            return
+                return
+
+            image = images[0]
 
         elif self.state.get("history", [])[-1] == "compare":
             images = []
 
             grid_size = math.gcd(
                 len(self.state["image_stack"]), len(self.state["image_stack"])
             )
 
             for image, detections in zip(
                 self.state["image_stack"], self.state["detections_stack"]
             ):
                 if annotator and detections:
-                    image = annotator.annotate(np.array(image), detections)
+                    image = annotator.annotate(
+                        np.array(image), detections, labels=self.state["last_classes"]
+                    )
                 else:
                     image = np.array(image)
 
                 images.append(image)
 
-            sv.plot_images_grid(
-                images=np.array(images), grid_size=(grid_size, grid_size), size=(12, 12)
-            )
+            if not self.notebook:
+                sv.plot_images_grid(
+                    images=np.array(images),
+                    grid_size=(grid_size, grid_size),
+                    size=(12, 12),
+                )
 
-            return
+                return
+
+            # image = images[0]
 
         if annotator:
             image = annotator.annotate(
-                cv2.imread(self.state["last_loaded_image_name"]),
-                self.state["detections_stack"][-1],
+                np.array(self.state["image_stack"][-1]),
+                detections=self.state["detections_stack"][-1],
             )
-        elif self.state.get("last_loaded_image") is not None:
-            image = self.state["last_loaded_image"]
+        elif (
+            self.state.get("last_loaded_image") is not None
+            and not self.state.get("history", [])[-1] == "compare"
+        ):
+            image = self.state["image_stack"][-1]
         else:
-            image = cv2.imread(self.state["last_loaded_image_name"])
+            image = self.state["image_stack"][-1]
+        # elif self.notebook is False:
+        #     image = cv2.imread(self.state["last_loaded_image_name"])
 
         if self.notebook:
             buffer = io.BytesIO()
             import base64
 
             import matplotlib
 
             matplotlib.use("Agg")
             import matplotlib.pyplot as plt
 
             # show image
-            fig = plt.figure(figsize=(8, 8))
-            plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+            if annotator:
+                print("annotator")
+                fig = plt.figure(figsize=(8, 8))
+                # if grey, show in grey
+                if len(image.shape) == 2:
+                    plt.imshow(image, cmap="gray")
+                else:
+                    plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+
+                fig.savefig(buffer, format="png")
+                buffer.seek(0)
+
+                image = Image.open(buffer)
+
+                img_str = {"image": base64.b64encode(buffer.getvalue()).decode("utf-8")}
 
-            fig.savefig(buffer, format="png")
-            buffer.seek(0)
+                self.state["output"] = img_str
 
-            image = Image.open(buffer)
+                return
+            else:
+                # if ndarray, convert to PIL
+                if isinstance(image, np.ndarray):
+                    image = Image.fromarray(image)
+                    # do bgr to rgb
+                    image = image.convert("RGB")
 
-            self.state["output"] = {
-                "image": base64.b64encode(buffer.getvalue()).decode("utf-8")
-            }
+                # convert to rgb if needed
+                if image.mode != "RGB":
+                    image = image.convert("RGB")
+
+                # PIL to base64
+                buffered = io.BytesIO()
+                image.save(buffered, format="PNG")
+                img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+            self.state["output"] = {"image": img_str}
 
             return
 
         sv.plot_image(image, (8, 8))
 
     def get_func(self, x):
         self.state["last"] = self.state["last"][x]
 
     def similarity(self, n):
-        # get similarity of last N images
+        """
+        Get similarity of last N images.
+        """
         if not n:
             n = 2
 
         if len(self.state["image_stack"]) < 2 or len(self.state["image_stack"]) < n:
             print("Not enough images to compare.")
             return
 
@@ -945,28 +1165,37 @@
                 image = model.encode_image(image)
 
                 embeddings.append(image)
 
         # get similarity
         similarity = torch.cosine_similarity(embeddings[0], embeddings[1])
 
-        self.state["last"] = similarity
+        # cast tensor to float
+        as_float = similarity.item()
 
-    def read_qr(self, _):
-        import pyzbar.pyzbar as pyzbar
+        self.state["last"] = as_float
 
-        image = self.state["last_loaded_image"]
+        return as_float
 
-        decoded_objects = pyzbar.decode(image)
+    def read_qr(self, _):
+        """
+        Read QR code from last image.
+        """
+        image = self.state["image_stack"][-1]
 
-        return decoded_objects
+        data, _, _ = cv2.QRCodeDetector().detectAndDecode(image)
+
+        return data
 
     def set_brightness(self, brightness):
+        """
+        Set brightness of last image.
+        """
         # brightness is between -100 and 100
-        image = self.state["last_loaded_image"]
+        image = self.state["image_stack"][-1]
 
         # use cv2
         hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
         h, s, v = cv2.split(hsv)
 
         # add brightness
         lim = 255 - brightness
@@ -974,38 +1203,47 @@
         v[v > lim] = 255
         v[v <= lim] += brightness
 
         final_hsv = cv2.merge((h, s, v))
 
         image = cv2.cvtColor(final_hsv, cv2.COLOR_HSV2BGR)
 
-        self.state["last_loaded_image"] = image
+        self.state["image_stack"].append(image)
+        self.state["output"] = image
 
     def contains(self, statement):
+        """
+        Check if a statement is contained in the last statement.
+        """
         if isinstance(self.state["last"], str):
             return statement in self.state["last"]
         else:
             return False
 
     def parse_tree(self, tree):
+        """
+        Abstract Syntax Tree (AST) parser for VisionScript.
+        """
         if not hasattr(tree, "children"):
             if hasattr(tree, "value") and tree.value.isdigit():
                 return int(tree.value)
             elif isinstance(tree, str):
                 return literal_eval(tree)
-        
+
         if hasattr(tree, "children") and tree.data == "input":
             return self.input_(tree.children[0].value)
 
         for node in tree.children:
+            print(node)
             if node == "True":
                 return True
             elif node == "False":
                 return False
             # if equality, check if equal
+            # if rule is input
             elif hasattr(node, "data") and node.data == "equality":
                 return self.parse_tree(node.children[0]) == self.parse_tree(
                     node.children[1]
                 )
             elif node is True or node is False:
                 return node
             elif hasattr(node, "data") and node.data == "list":
@@ -1029,15 +1267,15 @@
             if not hasattr(node, "data"):
                 continue
 
             token = node.data
 
             if token.value in aliased_functions:
                 token.value = map_alias_to_underlying_function(token.value)
-            
+
             if token.type == "equality":
                 return self.parse_tree(node.children[0]) == self.parse_tree(
                     node.children[1]
                 )
 
             if token == "comment":
                 continue
@@ -1129,36 +1367,41 @@
                 func(value)
                 continue
             elif token.value == "contains":
                 return func(literal_eval(node.children[0]))
             else:
                 # convert children to strings
                 for item in node.children:
+                    print(item, "eeee")
                     if hasattr(item, "value"):
                         if item.value.startswith('"') and item.value.endswith('"'):
                             item.value = literal_eval(item.value)
                         elif item.type in ("EOL", "INDENT", "DEDENT"):
                             continue
                         elif item.type == "STRING":
                             item.value = literal_eval(item.value)
                         elif item.type == "INT":
                             item.value = int(item.value)
+                        elif item.type == "input":
+                            item.value = self.parse_tree(item.value)
 
             if token.value == "in":
                 self.state["ctx"] = {
                     "in": os.listdir(node.children[0].value),
                 }
 
                 for file_name in self.state["ctx"]["in"]:
                     self.state["ctx"]["active_file"] = os.path.join(
                         literal_eval(node.children[0]), file_name
                     )
                     # ignore first 2, then do rest
                     context = node.children[3:]
 
+                    # print(context)
+
                     for item in context:
                         self.parse_tree(item)
 
                 del self.state["ctx"]
 
                 continue
 
@@ -1182,15 +1425,14 @@
                 self.state["output"] = result
 
             self.state["last_function_type"] = token.value
             self.state["last_function_args"] = [value]
 
             if token.value == "load":
                 self.state["image_stack"].append(result)
-                self.state["last_loaded_image"] = result
 
 
 def activate_console(parser):
     print("Welcome to VisionScript!")
     print("Type 'Exit[]' to exit.")
     print("Read the docs at https://visionscript.org/docs")
     print("For help, type 'Help[FunctionName]'.")
@@ -1211,33 +1453,43 @@
 
 
 @click.command()
 @click.option("--validate", default=False, help="")
 @click.option("--ref", default=False, help="Name of the file")
 @click.option("--debug", default=False, help="To debug")
 @click.option("--file", default=None, help="Name of the file")
-@click.option("--repl", default=None, help="To enter to vscript console")
-@click.option("--notebook/--no-notebook", help="To enter to vscript console")
-def main(validate, ref, debug, file, repl, notebook) -> None:
+@click.option("--repl", default=None, help="To enter to visionscript console")
+@click.option("--notebook/--no-notebook", help="Start a notebook environment")
+@click.option("--cloud/--no-cloud", help="Start a cloud deployment environment")
+def main(validate, ref, debug, file, repl, notebook, cloud) -> None:
     if validate:
         print("Script is a valid VisionScript program.")
         exit(0)
 
     if ref:
         print(USAGE.strip())
 
     if notebook:
         print("Starting notebook...")
         import webbrowser
-        from notebook import app
-        import uuid
 
-        # webbrowser.open("http://localhost:5000/notebook?" + str(uuid.uuid4()))
+        from visionscript.notebook import app
+
+        # webbrowser.open("http://localhost:5001/notebook?" + str(uuid.uuid4()))
+
+        app.run(debug=True, host="localhost", port=5001)
+
+        return
+
+    if cloud:
+        print("Starting cloud deployment environment...")
+
+        from visionscript.cloud import app
 
-        app.run(debug=True)
+        app.run(debug=True, port=6999)
 
     if file is not None:
         with open(file, "r") as f:
             code = f.read() + "\n"
 
         tree = parser.parse(code.lstrip())
```

### Comparing `visionscript-0.0.2/visionscript/notebook.py` & `visionscript-0.0.3/visionscript/notebook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,66 @@
-import lang
-from flask import Flask, jsonify, render_template, request, redirect, url_for
-from lang import parser
-import os
-import json
 import copy
-import uuid
+import json
+import os
 import time
+import uuid
+import requests
+import string
+
+from flask import Flask, jsonify, redirect, render_template, request, url_for
+
+import visionscript.lang as lang
+from visionscript.lang import parser
 
 app = Flask(__name__)
 
 notebooks = {}
 
 
 def init_notebook():
     # cells have a session that contains state and an output
     return {"session": None, "cells": [], "output": []}
 
+
 @app.route("/")
 def home():
     return redirect(url_for("notebook"))
 
+
 @app.route("/notebook", methods=["GET", "POST"])
 def notebook():
     # generate random id, then redirect user
     if request.method == "POST":
         data = request.json
         session_id = data["state_id"]
 
         user_input = data["code"]
 
-        if notebooks.get(session_id) is None or notebooks[session_id].get("session") is None:
+        if (
+            notebooks.get(session_id) is None
+            or notebooks[session_id].get("session") is None
+        ):
             session = lang.VisionScript()
 
             session.notebook = True
 
             notebooks[session_id]["session"] = session
 
         session = notebooks[session_id]["session"]
 
         start_time = time.time()
 
+        code = parser.parse(user_input.strip() + "\n")
+
         try:
-            session.parse_tree(parser.parse(user_input.strip() + "\n"))
+            session.parse_tree(code)
         except Exception as e:
             raise e
             return jsonify({"error": str(e)})
-        
+
         end_time = time.time()
 
         run_time = round(end_time - start_time, 1)
 
         notebooks[session_id]["cells"].append(user_input)
         notebooks[session_id]["output"].append(session.state["output"])
 
@@ -60,24 +71,50 @@
     else:
         state_id = uuid.uuid4().hex
 
     notebooks[state_id] = init_notebook()
 
     return render_template("notebook.html", state_id=state_id)
 
+
 @app.route("/notebook/upload", methods=["POST"])
 def upload():
+    from werkzeug.utils import secure_filename
+
     session_id = request.args.get("state_id")
     file = request.files["file"]
 
+    file.filename = secure_filename(file.filename)
+
     if session_id and notebooks.get(session_id) is None:
-        return jsonify({"error": "No session found"})
-    
+        return jsonify({"error": "No session found"}), 404
+
+    # if file is taken
+    if os.path.exists(os.path.join("tmp", file.filename)):
+        # add unique id
+        while os.path.exists(os.path.join("tmp", file.filename)):
+            file.filename = uuid.uuid4().hex[:4] + file.filename
+
     # save as tmp file
     file_name = file.filename
+
+    # only allow image uploads
+    import mimetypes
+
+    if file_name == "":
+        return jsonify({"error": "No file provided"})
+
+    if mimetypes.guess_type(file_name)[0]:
+        if not mimetypes.guess_type(file_name)[0].startswith(
+            "text"
+        ) and not mimetypes.guess_type(file_name)[0].startswith("image"):
+            return jsonify({"error": "File type not allowed"}), 415
+    elif not file_name.endswith(".vicnb"):
+        return jsonify({"error": "File type not allowed"}), 415
+
     # remove special chars
     file_name = "".join([c for c in file_name if c.isalnum() or c == "." or c == "_"])
 
     file_name = file_name.replace("..", "")
 
     # mkdir tmp if not exists
     if not os.path.exists("tmp"):
@@ -100,33 +137,74 @@
             notebooks[session_id]["cells"] = notebook["cells"]
             notebooks[session_id]["output"] = notebook["output"]
 
             # zip cells and output
             result = []
             for cell, output in zip(notebook["cells"], notebook["output"]):
                 result.append({"cell": cell, "output": output})
-            
+
             return jsonify({"cells": result})
 
     return jsonify({"file_name": os.path.join("tmp", file_name)})
 
+
 # save
 @app.route("/notebook/save", methods=["POST"])
 def save():
     session_id = request.args.get("state_id")
     file_name = "export.vic"
 
     if session_id and notebooks.get(session_id) is None:
         return jsonify({"error": "No session found"})
 
     if file_name is None:
         return jsonify({"error": "No file name provided"})
-    
+
     notebook = copy.deepcopy(notebooks[session_id])
 
     # delete session
     del notebook["session"]
 
     with open(file_name, "w") as f:
         json.dump(notebook, f)
 
     return jsonify({"file": notebook})
+
+@app.route("/notebook/deploy", methods=["POST"])
+def deploy():
+    session_id = request.json.get("state_id")
+    name = request.json.get("name")
+
+    if session_id and notebooks.get(session_id) is None:
+        return jsonify({"error": "No session found"}), 404
+
+    if name is None:
+        return jsonify({"error": "No file name provided"}), 400
+
+    # make a post request
+    notebook = copy.deepcopy(notebooks[session_id])
+
+    app_slug = name.translate(
+        str.maketrans("", "", string.punctuation.replace("-", ""))
+    )
+
+    deploy_request = requests.post("http://localhost:6999/create", json={
+        "title": name,
+        "slug": app_slug,
+        "api_key": "test",
+        "script": "\n".join(notebook["cells"]),
+        "variables": notebook["session"].state["input_variables"],
+    })
+
+    if deploy_request.ok:
+        return jsonify({"success": True})
+    
+    return jsonify({"success": False})
+
+@app.route("/static/<path:path>")
+def static_files(path):
+    return app.send_static_file(path)
+
+
+@app.route("/quit")
+def quit():
+    exit()
```

