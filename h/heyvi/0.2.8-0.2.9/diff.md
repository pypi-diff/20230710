# Comparing `tmp/heyvi-0.2.8.tar.gz` & `tmp/heyvi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/heyvi-0.2.8.tar", last modified: Mon Dec  6 21:06:33 2021, max compression
+gzip compressed data, was "dist/heyvi-0.2.9.tar", last modified: Mon Dec  6 21:58:30 2021, max compression
```

## Comparing `heyvi-0.2.8.tar` & `heyvi-0.2.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:33.000000 heyvi-0.2.8/
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/demo/
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)      635 2021-11-19 21:09:19.000000 heyvi-0.2.8/demo/tracker.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/docs/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)   328377 2021-10-16 15:05:13.000000 heyvi-0.2.8/docs/vipy_image_owl.jpg
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/ResNets_3D_PyTorch/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/ResNets_3D_PyTorch/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     7549 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/ResNets_3D_PyTorch/resnet.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/cap/
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)    14548 2021-12-02 20:29:33.000000 heyvi-0.2.8/heyvi/model/cap/class.csv
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)    20038 2021-12-02 20:31:08.000000 heyvi-0.2.8/heyvi/model/cap/class_to_shortlabel.csv
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)    21977 2021-12-02 20:30:28.000000 heyvi-0.2.8/heyvi/model/cap/class_to_training_weight.csv
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/face/
--rwxr-xr-x   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/face/__init__.py
--rwxr-xr-x   0 jba3139  (33139) str.diva (30108)    24352 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/face/detection.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    83229 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/face/faster_rcnn.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     8204 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/face/recognition.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/yolov3/
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/yolov3/utils/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/utils/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1261 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/utils/parse_config.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    11862 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/utils/utils.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)      625 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/coco.names
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    15073 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov3/network.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi/model/yolov5/
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:33.000000 heyvi-0.2.8/heyvi/model/yolov5/models/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     7118 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/common.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     6043 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/experimental.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     3824 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/export.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    12421 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/yolo.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1453 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/yolov5l.yaml
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/yolov5m.yaml
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/yolov5s.yaml
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/models/yolov5x.yaml
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:33.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     2200 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/activations.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     6721 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/autoanchor.py
--rwxr-xr-x   0 jba3139  (33139) str.diva (30108)    18280 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/general.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     4986 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/google_utils.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     8477 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/loss.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     8054 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/metrics.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     9564 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/utils/torch_utils.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)      625 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/model/yolov5/coco.names
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/model/__init__.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     2079 2021-12-06 20:07:47.000000 heyvi-0.2.8/heyvi/__init__.py
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)    35102 2021-11-30 19:54:08.000000 heyvi-0.2.8/heyvi/detection.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    28628 2021-10-16 15:05:13.000000 heyvi-0.2.8/heyvi/label.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    61671 2021-12-06 20:56:26.000000 heyvi-0.2.8/heyvi/recognition.py
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)     1828 2021-11-30 19:53:00.000000 heyvi-0.2.8/heyvi/sensor.py
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)    12082 2021-11-30 19:53:00.000000 heyvi-0.2.8/heyvi/system.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)      314 2021-10-16 15:05:14.000000 heyvi-0.2.8/heyvi/util.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1677 2021-12-06 20:56:26.000000 heyvi-0.2.8/heyvi/version.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:32.000000 heyvi-0.2.8/heyvi.egg-info/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     2325 2021-12-06 21:06:30.000000 heyvi-0.2.8/heyvi.egg-info/PKG-INFO
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1674 2021-12-06 21:06:31.000000 heyvi-0.2.8/heyvi.egg-info/SOURCES.txt
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        1 2021-12-06 21:06:30.000000 heyvi-0.2.8/heyvi.egg-info/dependency_links.txt
--rw-r--r--   0 jba3139  (33139) str.diva (30108)       79 2021-12-06 21:06:30.000000 heyvi-0.2.8/heyvi.egg-info/requires.txt
--rw-r--r--   0 jba3139  (33139) str.diva (30108)        6 2021-12-06 21:06:30.000000 heyvi-0.2.8/heyvi.egg-info/top_level.txt
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:33.000000 heyvi-0.2.8/script/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1325 2021-10-16 15:05:14.000000 heyvi-0.2.8/script/livestream.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    12312 2021-10-16 15:05:14.000000 heyvi-0.2.8/script/run_actev21.py
-drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:06:33.000000 heyvi-0.2.8/test/
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     3054 2021-10-16 15:05:14.000000 heyvi-0.2.8/test/test_detection.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)    35149 2021-10-16 15:05:12.000000 heyvi-0.2.8/LICENSE
--rw-r--r--   0 jba3139  (33139) str.diva (30108)      122 2021-12-02 20:35:59.000000 heyvi-0.2.8/MANIFEST.in
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     1395 2021-10-16 15:05:12.000000 heyvi-0.2.8/README.md
--rw-rw-r--   0 jba3139  (33139) str.diva (30108)     1906 2021-11-19 21:09:19.000000 heyvi-0.2.8/setup.py
--rw-r--r--   0 jba3139  (33139) str.diva (30108)     2325 2021-12-06 21:06:33.000000 heyvi-0.2.8/PKG-INFO
--rw-r--r--   0 jba3139  (33139) str.diva (30108)       38 2021-12-06 21:06:33.000000 heyvi-0.2.8/setup.cfg
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/demo/
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)      635 2021-11-19 21:09:19.000000 heyvi-0.2.9/demo/tracker.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/docs/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)   328377 2021-10-16 15:05:13.000000 heyvi-0.2.9/docs/vipy_image_owl.jpg
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/heyvi/
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/heyvi/model/
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/heyvi/model/ResNets_3D_PyTorch/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/ResNets_3D_PyTorch/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     7549 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/ResNets_3D_PyTorch/resnet.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/cap/
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)    14548 2021-12-02 20:29:33.000000 heyvi-0.2.9/heyvi/model/cap/class.csv
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)    20038 2021-12-02 20:31:08.000000 heyvi-0.2.9/heyvi/model/cap/class_to_shortlabel.csv
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)    21977 2021-12-02 20:30:28.000000 heyvi-0.2.9/heyvi/model/cap/class_to_training_weight.csv
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/face/
+-rwxr-xr-x   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/face/__init__.py
+-rwxr-xr-x   0 jba3139  (33139) str.diva (30108)    24352 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/face/detection.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    83229 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/face/faster_rcnn.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     8204 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/face/recognition.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/yolov3/
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/yolov3/utils/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/utils/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1261 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/utils/parse_config.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    11862 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/utils/utils.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)      625 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/coco.names
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    15073 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov3/network.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/yolov5/
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/yolov5/models/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     7118 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/common.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     6043 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/experimental.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     3824 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/export.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    12421 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/yolo.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1453 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/yolov5l.yaml
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/yolov5m.yaml
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/yolov5s.yaml
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1455 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/models/yolov5x.yaml
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     2200 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/activations.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     6721 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/autoanchor.py
+-rwxr-xr-x   0 jba3139  (33139) str.diva (30108)    18280 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/general.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     4986 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/google_utils.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     8477 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/loss.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     8054 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/metrics.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     9564 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/utils/torch_utils.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)      625 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/model/yolov5/coco.names
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        0 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/model/__init__.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     2079 2021-12-06 20:07:47.000000 heyvi-0.2.9/heyvi/__init__.py
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)    35102 2021-11-30 19:54:08.000000 heyvi-0.2.9/heyvi/detection.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    28628 2021-10-16 15:05:13.000000 heyvi-0.2.9/heyvi/label.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    61642 2021-12-06 21:56:53.000000 heyvi-0.2.9/heyvi/recognition.py
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)     1828 2021-11-30 19:53:00.000000 heyvi-0.2.9/heyvi/sensor.py
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)    12082 2021-11-30 19:53:00.000000 heyvi-0.2.9/heyvi/system.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)      314 2021-10-16 15:05:14.000000 heyvi-0.2.9/heyvi/util.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1677 2021-12-06 21:57:45.000000 heyvi-0.2.9/heyvi/version.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:29.000000 heyvi-0.2.9/heyvi.egg-info/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     2325 2021-12-06 21:58:28.000000 heyvi-0.2.9/heyvi.egg-info/PKG-INFO
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1674 2021-12-06 21:58:29.000000 heyvi-0.2.9/heyvi.egg-info/SOURCES.txt
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        1 2021-12-06 21:58:28.000000 heyvi-0.2.9/heyvi.egg-info/dependency_links.txt
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)       79 2021-12-06 21:58:28.000000 heyvi-0.2.9/heyvi.egg-info/requires.txt
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)        6 2021-12-06 21:58:28.000000 heyvi-0.2.9/heyvi.egg-info/top_level.txt
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/script/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1325 2021-10-16 15:05:14.000000 heyvi-0.2.9/script/livestream.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    12312 2021-10-16 15:05:14.000000 heyvi-0.2.9/script/run_actev21.py
+drwxr-sr-x   0 jba3139  (33139) str.diva (30108)        0 2021-12-06 21:58:30.000000 heyvi-0.2.9/test/
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     3054 2021-10-16 15:05:14.000000 heyvi-0.2.9/test/test_detection.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)    35149 2021-10-16 15:05:12.000000 heyvi-0.2.9/LICENSE
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)      122 2021-12-02 20:35:59.000000 heyvi-0.2.9/MANIFEST.in
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     1395 2021-10-16 15:05:12.000000 heyvi-0.2.9/README.md
+-rw-rw-r--   0 jba3139  (33139) str.diva (30108)     1906 2021-11-19 21:09:19.000000 heyvi-0.2.9/setup.py
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)     2325 2021-12-06 21:58:30.000000 heyvi-0.2.9/PKG-INFO
+-rw-r--r--   0 jba3139  (33139) str.diva (30108)       38 2021-12-06 21:58:30.000000 heyvi-0.2.9/setup.cfg
```

### Comparing `heyvi-0.2.8/demo/tracker.py` & `heyvi-0.2.9/demo/tracker.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/docs/vipy_image_owl.jpg` & `heyvi-0.2.9/docs/vipy_image_owl.jpg`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/ResNets_3D_PyTorch/resnet.py` & `heyvi-0.2.9/heyvi/model/ResNets_3D_PyTorch/resnet.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/cap/class.csv` & `heyvi-0.2.9/heyvi/model/cap/class.csv`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/cap/class_to_shortlabel.csv` & `heyvi-0.2.9/heyvi/model/cap/class_to_shortlabel.csv`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/cap/class_to_training_weight.csv` & `heyvi-0.2.9/heyvi/model/cap/class_to_training_weight.csv`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/face/detection.py` & `heyvi-0.2.9/heyvi/model/face/detection.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/face/faster_rcnn.py` & `heyvi-0.2.9/heyvi/model/face/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/face/recognition.py` & `heyvi-0.2.9/heyvi/model/face/recognition.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov3/utils/parse_config.py` & `heyvi-0.2.9/heyvi/model/yolov3/utils/parse_config.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov3/utils/utils.py` & `heyvi-0.2.9/heyvi/model/yolov3/utils/utils.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov3/coco.names` & `heyvi-0.2.9/heyvi/model/yolov3/coco.names`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov3/network.py` & `heyvi-0.2.9/heyvi/model/yolov3/network.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/common.py` & `heyvi-0.2.9/heyvi/model/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/experimental.py` & `heyvi-0.2.9/heyvi/model/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/export.py` & `heyvi-0.2.9/heyvi/model/yolov5/models/export.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/yolo.py` & `heyvi-0.2.9/heyvi/model/yolov5/models/yolo.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/yolov5l.yaml` & `heyvi-0.2.9/heyvi/model/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/yolov5m.yaml` & `heyvi-0.2.9/heyvi/model/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/yolov5s.yaml` & `heyvi-0.2.9/heyvi/model/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/models/yolov5x.yaml` & `heyvi-0.2.9/heyvi/model/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/activations.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/autoanchor.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/general.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/general.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/google_utils.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/loss.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/loss.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/metrics.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/utils/torch_utils.py` & `heyvi-0.2.9/heyvi/model/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/model/yolov5/coco.names` & `heyvi-0.2.9/heyvi/model/yolov5/coco.names`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/__init__.py` & `heyvi-0.2.9/heyvi/__init__.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/detection.py` & `heyvi-0.2.9/heyvi/detection.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/label.py` & `heyvi-0.2.9/heyvi/label.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/recognition.py` & `heyvi-0.2.9/heyvi/recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,14 @@
         """Return captured lambda function if v=None, else return tensor"""    
         assert v is None or isinstance(v, vipy.video.Scene), "Invalid input"
         f = (lambda v, num_frames=self._num_frames, input_size=self._input_size, mean=self._mean, std=self._std, training=training, validation=validation, show=show, classname=self.__class__.__name__:
              PIP_370k._totensor(v, training, validation, input_size, num_frames, mean, std, noflip=['car_turns_left', 'car_turns_right', 'vehicle_turns_left', 'vehicle_turns_right', 'motorcycle_turns_left', 'motorcycle_turns_right'], show=show, doflip=doflip, asjson=asjson, classname=classname))
         return f(v) if v is not None else f
 
     def calibration(self, x_logits):
-        import scipy.special
         assert torch.is_tensor(self._calibration_multiclass) and self._calibration_multiclass.shape == (1,1)
         assert torch.is_tensor(self._calibration_binary) and self._calibration_binary.shape == (3, self.num_classes())
         (n, T, (w,b,o), eps) = (self.num_classes(), self._calibration_multiclass, self._calibration_binary, np.finfo(np.float64).eps)  # (TemperatureScaling, PlattScaling=(weight, bias, offset))
 
         #lr = torch.from_numpy(np.multiply(1.0/(1+np.exp(-(np.multiply(np.array(w*0 + 1).reshape(1,n).astype(np.float64), scipy.special.logit(np.clip(torch.sigmoid(x_logits-o.view(1,n)).detach().cpu().numpy().astype(np.float64), eps, 1-eps))))+np.array(b).reshape(1,n).astype(np.float64))), (np.array(o)!=0).reshape(1,n)).astype(np.float32))        
         #sm = F.softmax(torch.log(torch.clamp(F.softmax(x_logits, dim=1), eps, 1-eps)) / T, dim=1)
```

### Comparing `heyvi-0.2.8/heyvi/sensor.py` & `heyvi-0.2.9/heyvi/sensor.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/system.py` & `heyvi-0.2.9/heyvi/system.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/heyvi/version.py` & `heyvi-0.2.9/heyvi/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MAJOR = 0
 MINOR = 2
-RELEASE = 8
+RELEASE = 9
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, RELEASE)
 
 
 def num(versionstring=VERSION):
     """Convert the version string of the form 'X.Y.Z' to an integer 100000*X + 100*Y + Z for version comparison"""
     (major, minor, release) = versionstring.split('.')    
     return 100*100*int(major) + 100*int(minor) + int(release)
```

### Comparing `heyvi-0.2.8/heyvi.egg-info/PKG-INFO` & `heyvi-0.2.9/heyvi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: heyvi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Project Vi
 Home-page: https://github.com/visym/heyvi
 Author: Visym Labs
 Author-email: info@visym.com
 License: UNKNOWN
-Download-URL: https://github.com/visym/heyvi/archive/0.2.8.tar.gz
+Download-URL: https://github.com/visym/heyvi/archive/0.2.9.tar.gz
 Description: [![PyPI version](https://badge.fury.io/py/heyvi.svg)](https://badge.fury.io/py/heyvi)
         
         \"Hey Vi!\"
         -------------------
         
         HEYVI: Visym Analytics for Visual AI    
         docs: https://developer.visym.com/heyvi
```

### Comparing `heyvi-0.2.8/heyvi.egg-info/SOURCES.txt` & `heyvi-0.2.9/heyvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/script/livestream.py` & `heyvi-0.2.9/script/livestream.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/script/run_actev21.py` & `heyvi-0.2.9/script/run_actev21.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/test/test_detection.py` & `heyvi-0.2.9/test/test_detection.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/LICENSE` & `heyvi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/README.md` & `heyvi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/setup.py` & `heyvi-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `heyvi-0.2.8/PKG-INFO` & `heyvi-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: heyvi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Project Vi
 Home-page: https://github.com/visym/heyvi
 Author: Visym Labs
 Author-email: info@visym.com
 License: UNKNOWN
-Download-URL: https://github.com/visym/heyvi/archive/0.2.8.tar.gz
+Download-URL: https://github.com/visym/heyvi/archive/0.2.9.tar.gz
 Description: [![PyPI version](https://badge.fury.io/py/heyvi.svg)](https://badge.fury.io/py/heyvi)
         
         \"Hey Vi!\"
         -------------------
         
         HEYVI: Visym Analytics for Visual AI    
         docs: https://developer.visym.com/heyvi
```

