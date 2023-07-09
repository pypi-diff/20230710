# Comparing `tmp/video-ditor-0.0.1.tar.gz` & `tmp/video-ditor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/video-ditor-0.0.1.tar", last modified: Sun Jul  9 01:34:31 2023, max compression
+gzip compressed data, was "dist/video-ditor-0.0.2.tar", last modified: Sun Jul  9 22:05:22 2023, max compression
```

## Comparing `video-ditor-0.0.1.tar` & `video-ditor-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/
--rw-r--r--   0 tsiameh    (501) staff       (20)     1061 2023-02-27 16:08:18.000000 video-ditor-0.0.1/LICENCE.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)     3832 2023-07-09 01:34:31.000000 video-ditor-0.0.1/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     1960 2023-07-09 01:31:36.000000 video-ditor-0.0.1/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/background/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 20:45:22.000000 video-ditor-0.0.1/background/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     1573 2023-07-08 23:04:12.000000 video-ditor-0.0.1/background/main.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     2523 2023-07-08 03:37:20.000000 video-ditor-0.0.1/background/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/concat/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 18:43:28.000000 video-ditor-0.0.1/concat/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     1068 2023-07-08 23:25:33.000000 video-ditor-0.0.1/concat/main.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     1047 2023-07-07 19:10:19.000000 video-ditor-0.0.1/concat/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/cut/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 18:29:40.000000 video-ditor-0.0.1/cut/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      916 2023-07-08 22:54:17.000000 video-ditor-0.0.1/cut/main.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      713 2023-07-07 20:04:17.000000 video-ditor-0.0.1/cut/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/download/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-08 23:56:16.000000 video-ditor-0.0.1/download/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      604 2023-07-09 00:30:10.000000 video-ditor-0.0.1/download/main.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-09 01:34:31.000000 video-ditor-0.0.1/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     2091 2023-07-09 00:08:43.000000 video-ditor-0.0.1/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3832 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      492 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)      155 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/entry_points.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       41 2023-07-09 01:34:31.000000 video-ditor-0.0.1/video_ditor.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 01:34:31.000000 video-ditor-0.0.1/watermark/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 19:12:14.000000 video-ditor-0.0.1/watermark/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     2240 2023-07-08 23:04:12.000000 video-ditor-0.0.1/watermark/main.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      195 2023-07-07 20:04:17.000000 video-ditor-0.0.1/watermark/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1061 2023-02-27 16:08:18.000000 video-ditor-0.0.2/LICENCE.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4033 2023-07-09 22:05:22.000000 video-ditor-0.0.2/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2105 2023-07-09 22:01:53.000000 video-ditor-0.0.2/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/background/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 20:45:22.000000 video-ditor-0.0.2/background/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1999 2023-07-09 21:50:37.000000 video-ditor-0.0.2/background/main.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3476 2023-07-09 21:50:37.000000 video-ditor-0.0.2/background/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/concat/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 18:43:28.000000 video-ditor-0.0.2/concat/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1068 2023-07-08 23:25:33.000000 video-ditor-0.0.2/concat/main.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1045 2023-07-09 21:51:48.000000 video-ditor-0.0.2/concat/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/cut/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 18:29:40.000000 video-ditor-0.0.2/cut/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1168 2023-07-09 21:51:48.000000 video-ditor-0.0.2/cut/main.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1536 2023-07-09 21:51:48.000000 video-ditor-0.0.2/cut/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/download/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-08 23:56:16.000000 video-ditor-0.0.2/download/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      681 2023-07-09 21:51:48.000000 video-ditor-0.0.2/download/main.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-09 22:05:22.000000 video-ditor-0.0.2/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2045 2023-07-09 21:50:16.000000 video-ditor-0.0.2/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4033 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      492 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)      155 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/entry_points.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       53 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       41 2023-07-09 22:05:22.000000 video-ditor-0.0.2/video_ditor.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-09 22:05:22.000000 video-ditor-0.0.2/watermark/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-07-07 19:12:14.000000 video-ditor-0.0.2/watermark/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2248 2023-07-09 21:51:48.000000 video-ditor-0.0.2/watermark/main.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      195 2023-07-07 20:04:17.000000 video-ditor-0.0.2/watermark/utils.py
```

### Comparing `video-ditor-0.0.1/LICENCE.txt` & `video-ditor-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `video-ditor-0.0.1/PKG-INFO` & `video-ditor-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-ditor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to manipulate videos
 Home-page: https://github.com/donwany/video-ditor.git
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -15,14 +15,21 @@
           [GhanaNews-Scraper](https://pypi.org/project/ghananews-scraper/), and
           [GhanaShops-Scraper](https://pypi.org/project/ghanashops-scraper/)
         
         ### How to install
         ```shell
         pip install video-ditor
         ```
+        ### Install using:
+        ```shell
+        # OR
+        git clone https://github.com/donwany/Video-Ditor.git
+        cd Video-Ditor
+        make pre-release
+        ```
         
         ### Join Videos
         ```bash
         python main.py \
         -c africa1.mp4 gabby.mp4 \ 
         -o gabby_africa.mp4
         
@@ -59,23 +66,23 @@
         ```bash
         python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
         
         # Using CLI
         background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
         ```
         
-        ### Download YouTube Videos
+        ### Download YouTube/Facebook/Twitter Videos
         ```bash
         
         # Using CLI
         ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI
         
-        ytube -u https://twitter.com/kwadwosheldon/status/1673856306136981504
+        ytube --url https://twitter.com/kwadwosheldon/status/1673856306136981504
         
-        ytube -u https://www.facebook.com/gtvghana/videos/1219922122741862
+        ytube --url https://www.facebook.com/gtvghana/videos/1219922122741862
         ```
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
         
         Credits
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: video-ditor Version: 0.0.1 Summary: A python
+Metadata-Version: 2.1 Name: video-ditor Version: 0.0.2 Summary: A python
 package to manipulate videos Home-page: https://github.com/donwany/video-
 ditor.git Author: Theophilus Siameh Author-email: theodondre@gmail.com License:
 MIT License Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/
 Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000) [![Imports: isort]
 (https://img.shields.io/badge/%20imports-isort-
 %231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) ###
 Video-Ditor A simple video editor python package Affiliated to [Bank of Ghana
 Fx Rates](https://pypi.org/project/bank-of-ghana-fx-rates/), [GhanaNews-
 Scraper](https://pypi.org/project/ghananews-scraper/), and [GhanaShops-Scraper]
 (https://pypi.org/project/ghanashops-scraper/) ### How to install ```shell pip
-install video-ditor ``` ### Join Videos ```bash python main.py \ -c africa1.mp4
-gabby.mp4 \ -o gabby_africa.mp4 # Using CLI concat \ -c africa1.mp4 gabby.mp4 \
--o gabby_africa.mp4 ``` ### Cut Videos ```bash python main.py \ -i africa1.mp4
-\ -o gabby_africa.mp4 \ -s "00:00:00" \ -e "00:00:00" # Using CLI slice \ -
-i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:00:00" \ -e "00:00:00" ``` ###
-Watermark Videos ```bash python main.py -i gabby.mp4 -w james.png -x 500 -
-o water_output.mp4 # Using CLI watermark -i gabby.mp4 -w james.png -x 500 -
-o water_output.mp4 ``` ### Add Background and Overlay Video ```bash python
-main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0 # Using
-CLI background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
-``` ### Download YouTube Videos ```bash # Using CLI ytube -u https://
-www.youtube.com/watch?v=fqi8cvN1hrI ytube -u https://twitter.com/kwadwosheldon/
-status/1673856306136981504 ytube -u https://www.facebook.com/gtvghana/videos/
-1219922122741862 ``` BuyMeCoffee ----------- [![Build](https://
-www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://
-www.buymeacoffee.com/theodondrew) Credits ------- - `Theophilus Siameh`
+install video-ditor ``` ### Install using: ```shell # OR git clone https://
+github.com/donwany/Video-Ditor.git cd Video-Ditor make pre-release ``` ### Join
+Videos ```bash python main.py \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4
+# Using CLI concat \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4 ``` ### Cut
+Videos ```bash python main.py \ -i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:
+00:00" \ -e "00:00:00" # Using CLI slice \ -i africa1.mp4 \ -o gabby_africa.mp4
+\ -s "00:00:00" \ -e "00:00:00" ``` ### Watermark Videos ```bash python main.py
+-i gabby.mp4 -w james.png -x 500 -o water_output.mp4 # Using CLI watermark -
+i gabby.mp4 -w james.png -x 500 -o water_output.mp4 ``` ### Add Background and
+Overlay Video ```bash python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -
+p 150 -v 0.10 -bv 1.0 # Using CLI background -b gabby.mp4 -o IWILL.mp4 -
+x final1.mp4 -p 150 -v 0.10 -bv 1.0 ``` ### Download YouTube/Facebook/Twitter
+Videos ```bash # Using CLI ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI
+ytube --url https://twitter.com/kwadwosheldon/status/1673856306136981504 ytube
+--url https://www.facebook.com/gtvghana/videos/1219922122741862 ``` BuyMeCoffee
+----------- [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
+yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
+`Theophilus Siameh`
 [tsiameh_twitter]
 Keywords: video editor,editor,video manipulator,cut videos,join videos,add
 watermark to videos Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `video-ditor-0.0.1/README.md` & `video-ditor-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,21 @@
   [GhanaNews-Scraper](https://pypi.org/project/ghananews-scraper/), and
   [GhanaShops-Scraper](https://pypi.org/project/ghanashops-scraper/)
 
 ### How to install
 ```shell
 pip install video-ditor
 ```
+### Install using:
+```shell
+# OR
+git clone https://github.com/donwany/Video-Ditor.git
+cd Video-Ditor
+make pre-release
+```
 
 ### Join Videos
 ```bash
 python main.py \
 -c africa1.mp4 gabby.mp4 \ 
 -o gabby_africa.mp4
 
@@ -51,23 +58,23 @@
 ```bash
 python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
 
 # Using CLI
 background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
 ```
 
-### Download YouTube Videos
+### Download YouTube/Facebook/Twitter Videos
 ```bash
 
 # Using CLI
 ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI
 
-ytube -u https://twitter.com/kwadwosheldon/status/1673856306136981504
+ytube --url https://twitter.com/kwadwosheldon/status/1673856306136981504
 
-ytube -u https://www.facebook.com/gtvghana/videos/1219922122741862
+ytube --url https://www.facebook.com/gtvghana/videos/1219922122741862
 ```
 
 BuyMeCoffee
 -----------
 [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
 
 Credits
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
 ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-
 3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) ### Video-Ditor A simple video editor python
 package Affiliated to [Bank of Ghana Fx Rates](https://pypi.org/project/bank-
 of-ghana-fx-rates/), [GhanaNews-Scraper](https://pypi.org/project/ghananews-
 scraper/), and [GhanaShops-Scraper](https://pypi.org/project/ghanashops-
-scraper/) ### How to install ```shell pip install video-ditor ``` ### Join
-Videos ```bash python main.py \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4
-# Using CLI concat \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4 ``` ### Cut
-Videos ```bash python main.py \ -i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:
-00:00" \ -e "00:00:00" # Using CLI slice \ -i africa1.mp4 \ -o gabby_africa.mp4
-\ -s "00:00:00" \ -e "00:00:00" ``` ### Watermark Videos ```bash python main.py
--i gabby.mp4 -w james.png -x 500 -o water_output.mp4 # Using CLI watermark -
-i gabby.mp4 -w james.png -x 500 -o water_output.mp4 ``` ### Add Background and
-Overlay Video ```bash python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -
-p 150 -v 0.10 -bv 1.0 # Using CLI background -b gabby.mp4 -o IWILL.mp4 -
-x final1.mp4 -p 150 -v 0.10 -bv 1.0 ``` ### Download YouTube Videos ```bash #
-Using CLI ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI ytube -u https:/
-/twitter.com/kwadwosheldon/status/1673856306136981504 ytube -u https://
+scraper/) ### How to install ```shell pip install video-ditor ``` ### Install
+using: ```shell # OR git clone https://github.com/donwany/Video-Ditor.git cd
+Video-Ditor make pre-release ``` ### Join Videos ```bash python main.py \ -
+c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4 # Using CLI concat \ -
+c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4 ``` ### Cut Videos ```bash python
+main.py \ -i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:00:00" \ -e "00:00:00"
+# Using CLI slice \ -i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:00:00" \ -
+e "00:00:00" ``` ### Watermark Videos ```bash python main.py -i gabby.mp4 -
+w james.png -x 500 -o water_output.mp4 # Using CLI watermark -i gabby.mp4 -
+w james.png -x 500 -o water_output.mp4 ``` ### Add Background and Overlay Video
+```bash python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -
+bv 1.0 # Using CLI background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -
+v 0.10 -bv 1.0 ``` ### Download YouTube/Facebook/Twitter Videos ```bash # Using
+CLI ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI ytube --url https://
+twitter.com/kwadwosheldon/status/1673856306136981504 ytube --url https://
 www.facebook.com/gtvghana/videos/1219922122741862 ``` BuyMeCoffee -----------
 [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
 yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
 `Theophilus Siameh`
 [tsiameh_twitter]
```

### Comparing `video-ditor-0.0.1/background/main.py` & `video-ditor-0.0.2/background/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from .utils import add_background_video
 import argparse
+
 from loguru import logger
 
+from .utils import Args, add_background_video, validate_args
+
 
 def cli():
     parser = argparse.ArgumentParser(
         description="add background video to overly videos"
     )
     parser.add_argument(
         "--back_vid", "-b", type=str, required=True, help="background video"
@@ -38,27 +40,40 @@
         default=1.0,
         type=float,
         required=True,
         help="background video volume",
     )
     args = parser.parse_args()
 
-    back_vid = args.back_vid
-    overlay_vid = args.overlay_vid
-    output_vid = args.output_vid
-    overlay_pos = args.over_pos
-    over_volume = args.over_vol
-    back_vol = args.back_vol
+    # Create an instance of Args
+    input_args = Args(
+        back_vid=args.back_vid,
+        overlay_vid=args.overlay_vid,
+        output_vid=args.output_vid,
+        over_pos=args.over_pos,
+        over_vol=args.over_vol,
+        back_vol=args.back_vol,
+    )
+
+    # Validate the input arguments
+    validate_args(input_args)
+
+    # back_vid = args.back_vid
+    # overlay_vid = args.overlay_vid
+    # output_vid = args.output_vid
+    # overlay_pos = args.over_pos
+    # over_volume = args.over_vol
+    # back_vol = args.back_vol
 
     logger.info("adding background video and overlay video ...")
     add_background_video(
-        back_video=back_vid,
-        overlay_video=overlay_vid,
-        output_video=output_vid,
-        over_pos=overlay_pos,
-        back_vol=back_vol,
-        over_vol=over_volume,
+        back_video=input_args.back_vid,
+        overlay_video=input_args.overlay_vid,
+        output_video=input_args.output_vid,
+        over_pos=input_args.over_pos,
+        back_vol=input_args.back_vol,
+        over_vol=input_args.over_vol,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `video-ditor-0.0.1/concat/main.py` & `video-ditor-0.0.2/concat/main.py`

 * *Files identical despite different names*

### Comparing `video-ditor-0.0.1/concat/utils.py` & `video-ditor-0.0.2/concat/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from moviepy.editor import *
+import sys
+
 from loguru import logger
+from moviepy.editor import VideoFileClip, concatenate_videoclips
 
 
 def concatenate_videos(video_clips, output_path, method="compose"):
-    """concatenate videos"""
-    global final_clip
+    """Concatenate videos"""
+    if len(video_clips) == 1:
+        logger.warning("Only one video clip provided for concatenation. Need at least one video.")
+        sys.exit(1)
+
     clips = [VideoFileClip(clip) for clip in video_clips]
 
     if method == "reduce":
-        # calculate minimum width & height across all clips
-        min_height = min([c.h for c in clips])
-        min_width = min([c.w for c in clips])
-        # resize the videos to the minimum
+        # Calculate minimum width & height across all clips
+        min_height = min(c.h for c in clips)
+        min_width = min(c.w for c in clips)
+        # Resize the videos to the minimum
         clips = [c.resize(newsize=(min_width, min_height)) for c in clips]
-        # Concatenate the videos
-        final_clip = concatenate_videoclips(clips)
-    elif method == "compose":
-        # concatenate the final video with the compose method provided by moviepy
-        final_clip = concatenate_videoclips(clips, method="compose")
 
-    logger.info("Writing video to file ...")
+    # Concatenate the videos
+    final_clip = concatenate_videoclips(clips, method=method)
+
+    logger.info("Writing video to file...")
     final_clip.write_videofile(
         filename=output_path,
         codec="libx264",
         audio_codec="aac",
         fps=30,
         temp_audiofile="temp-audio.m4a",
         remove_temp=True,
```

### Comparing `video-ditor-0.0.1/cut/main.py` & `video-ditor-0.0.2/cut/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
-from .utils import cut_video
+
 from loguru import logger
 
+from .utils import Args, cut_video, validate_args
+
 
 def cli():
     parser = argparse.ArgumentParser(description="cut videos")
     parser.add_argument(
         "--input_vid", "-i", type=str, required=True, help="input video"
     )
     parser.add_argument(
@@ -15,20 +17,29 @@
         "--start_time", "-s", type=str, required=True, help="start time in (seconds)"
     )
     parser.add_argument(
         "--end_time", "-e", type=str, required=True, help="end time in (seconds)"
     )
     args = parser.parse_args()
 
-    input_vid = args.input_vid
-    output_vid = args.output_vid
-    start = args.start_time
-    end = args.end_time
+    # Create an instance of Args
+    input_args = Args(
+        input_vid=args.input_vid,
+        output_vid=args.output_vid,
+        start_time=args.start_time,
+        end_time=args.end_time,
+    )
+
+    # Validate the input arguments
+    validate_args(input_args)
 
     logger.info("Cutting video ...")
     cut_video(
-        input_vid=input_vid, start_time=start, end_time=end, output_vid=output_vid
+        input_vid=input_args.input_vid,
+        start_time=input_args.start_time,
+        end_time=input_args.end_time,
+        output_vid=input_args.output_vid,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `video-ditor-0.0.1/download/main.py` & `video-ditor-0.0.2/download/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 
 import yt_dlp
+from loguru import logger
 
 
 def download_video(url):
     ydl_opts = {
         'outtmpl': '%(title)s.%(ext)s',
         'format': 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best',
     }
@@ -19,12 +20,13 @@
     parser.add_argument(
         "--url", "-u", type=str, required=True, help="youtube video url"
     )
 
     args = parser.parse_args()
 
     video_url = args.url
+    logger.info(f"Downloading from : {video_url}")
     download_video(video_url)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `video-ditor-0.0.1/setup.py` & `video-ditor-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md") as f:
     README = f.read()
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name="video-ditor",
-    py_modules=[
-        "cut",
-        "background",
-        "concat",
-        "watermark",
-        "download"
-    ],
-    version="0.0.1",
+    py_modules=["cut", "background", "concat", "watermark", "download"],
+    version="0.0.2",
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/donwany/video-ditor.git",
     license="MIT License",
     author="Theophilus Siameh",
     author_email="theodondre@gmail.com",
     install_requires=install_requires,
     description="A python package to manipulate videos",
     entry_points={
-        'console_scripts': [
-            'slice = cut.main:cli',
-            'concat = concat.main:cli',
-            'background = background.main:cli',
-            'watermark = watermark.main:cli',
-            'ytube = download.main:cli',
+        "console_scripts": [
+            "slice = cut.main:cli",
+            "concat = concat.main:cli",
+            "background = background.main:cli",
+            "watermark = watermark.main:cli",
+            "ytube = download.main:cli",
         ]
     },
     classifiers=[
         # See https://pypi.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
```

### Comparing `video-ditor-0.0.1/video_ditor.egg-info/PKG-INFO` & `video-ditor-0.0.2/video_ditor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-ditor
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package to manipulate videos
 Home-page: https://github.com/donwany/video-ditor.git
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -15,14 +15,21 @@
           [GhanaNews-Scraper](https://pypi.org/project/ghananews-scraper/), and
           [GhanaShops-Scraper](https://pypi.org/project/ghanashops-scraper/)
         
         ### How to install
         ```shell
         pip install video-ditor
         ```
+        ### Install using:
+        ```shell
+        # OR
+        git clone https://github.com/donwany/Video-Ditor.git
+        cd Video-Ditor
+        make pre-release
+        ```
         
         ### Join Videos
         ```bash
         python main.py \
         -c africa1.mp4 gabby.mp4 \ 
         -o gabby_africa.mp4
         
@@ -59,23 +66,23 @@
         ```bash
         python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
         
         # Using CLI
         background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
         ```
         
-        ### Download YouTube Videos
+        ### Download YouTube/Facebook/Twitter Videos
         ```bash
         
         # Using CLI
         ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI
         
-        ytube -u https://twitter.com/kwadwosheldon/status/1673856306136981504
+        ytube --url https://twitter.com/kwadwosheldon/status/1673856306136981504
         
-        ytube -u https://www.facebook.com/gtvghana/videos/1219922122741862
+        ytube --url https://www.facebook.com/gtvghana/videos/1219922122741862
         ```
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
         
         Credits
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: video-ditor Version: 0.0.1 Summary: A python
+Metadata-Version: 2.1 Name: video-ditor Version: 0.0.2 Summary: A python
 package to manipulate videos Home-page: https://github.com/donwany/video-
 ditor.git Author: Theophilus Siameh Author-email: theodondre@gmail.com License:
 MIT License Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/
 Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000) [![Imports: isort]
 (https://img.shields.io/badge/%20imports-isort-
 %231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) ###
 Video-Ditor A simple video editor python package Affiliated to [Bank of Ghana
 Fx Rates](https://pypi.org/project/bank-of-ghana-fx-rates/), [GhanaNews-
 Scraper](https://pypi.org/project/ghananews-scraper/), and [GhanaShops-Scraper]
 (https://pypi.org/project/ghanashops-scraper/) ### How to install ```shell pip
-install video-ditor ``` ### Join Videos ```bash python main.py \ -c africa1.mp4
-gabby.mp4 \ -o gabby_africa.mp4 # Using CLI concat \ -c africa1.mp4 gabby.mp4 \
--o gabby_africa.mp4 ``` ### Cut Videos ```bash python main.py \ -i africa1.mp4
-\ -o gabby_africa.mp4 \ -s "00:00:00" \ -e "00:00:00" # Using CLI slice \ -
-i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:00:00" \ -e "00:00:00" ``` ###
-Watermark Videos ```bash python main.py -i gabby.mp4 -w james.png -x 500 -
-o water_output.mp4 # Using CLI watermark -i gabby.mp4 -w james.png -x 500 -
-o water_output.mp4 ``` ### Add Background and Overlay Video ```bash python
-main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0 # Using
-CLI background -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -p 150 -v 0.10 -bv 1.0
-``` ### Download YouTube Videos ```bash # Using CLI ytube -u https://
-www.youtube.com/watch?v=fqi8cvN1hrI ytube -u https://twitter.com/kwadwosheldon/
-status/1673856306136981504 ytube -u https://www.facebook.com/gtvghana/videos/
-1219922122741862 ``` BuyMeCoffee ----------- [![Build](https://
-www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://
-www.buymeacoffee.com/theodondrew) Credits ------- - `Theophilus Siameh`
+install video-ditor ``` ### Install using: ```shell # OR git clone https://
+github.com/donwany/Video-Ditor.git cd Video-Ditor make pre-release ``` ### Join
+Videos ```bash python main.py \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4
+# Using CLI concat \ -c africa1.mp4 gabby.mp4 \ -o gabby_africa.mp4 ``` ### Cut
+Videos ```bash python main.py \ -i africa1.mp4 \ -o gabby_africa.mp4 \ -s "00:
+00:00" \ -e "00:00:00" # Using CLI slice \ -i africa1.mp4 \ -o gabby_africa.mp4
+\ -s "00:00:00" \ -e "00:00:00" ``` ### Watermark Videos ```bash python main.py
+-i gabby.mp4 -w james.png -x 500 -o water_output.mp4 # Using CLI watermark -
+i gabby.mp4 -w james.png -x 500 -o water_output.mp4 ``` ### Add Background and
+Overlay Video ```bash python main.py -b gabby.mp4 -o IWILL.mp4 -x final1.mp4 -
+p 150 -v 0.10 -bv 1.0 # Using CLI background -b gabby.mp4 -o IWILL.mp4 -
+x final1.mp4 -p 150 -v 0.10 -bv 1.0 ``` ### Download YouTube/Facebook/Twitter
+Videos ```bash # Using CLI ytube -u https://www.youtube.com/watch?v=fqi8cvN1hrI
+ytube --url https://twitter.com/kwadwosheldon/status/1673856306136981504 ytube
+--url https://www.facebook.com/gtvghana/videos/1219922122741862 ``` BuyMeCoffee
+----------- [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
+yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
+`Theophilus Siameh`
 [tsiameh_twitter]
 Keywords: video editor,editor,video manipulator,cut videos,join videos,add
 watermark to videos Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `video-ditor-0.0.1/watermark/main.py` & `video-ditor-0.0.2/watermark/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 
 from loguru import logger
 from moviepy.editor import *
+
 from .utils import has_image_extension
 
 
 def cli():
     parser = argparse.ArgumentParser(description="Add watermark videos/image")
     parser.add_argument("--input_vid", '-i', type=str, required=True, help="input video")
     parser.add_argument("--watermark", '-w', type=str, required=True, help="watermark image")
@@ -15,49 +16,48 @@
                         '-p',
                         type=str,
                         default="left",
                         choices=["left", "center", "right", "top"],
                         help="watermark position")
     args = parser.parse_args()
 
-    input_video = args.input_vid
-    watermark = args.watermark
-    img_height = args.img_height
-    output_vid = args.output_vid
-    watermark_pos = args.position
-
     # List of image extensions to check
     image_extensions = ['.jpg', '.jpeg', '.png']
 
     # Load the video
+    input_video = args.input_vid
     if input_video.lower().endswith(".mp4"):
         video = VideoFileClip(input_video)
-        logger.info("Video extension valid ...")
+        logger.info("Input video loaded successfully.")
     else:
-        logger.info("Video extension not valid ...")
-        sys.exit(1)
+        logger.info("Invalid video extension. Only .mp4 file format allowed.")
+        return
+
     # Load the watermark image
+    watermark = args.watermark
     if has_image_extension(watermark, image_extensions):
-        watermark = ImageClip(watermark).resize(height=img_height)
-        logger.info("filename is an image file ...")
+        watermark = ImageClip(watermark).resize(height=args.img_height)
+        logger.info("Watermark image loaded successfully.")
     else:
-        logger.info("filename is not an image file ...")
-        sys.exit(1)
+        logger.info(f"Invalid watermark image. Only {image_extensions} allowed.")
+        return
 
     # Set the duration of the watermark clip
     watermark = watermark.set_duration(video.duration)
+
     # Add the watermark to the video
+    watermark_pos = args.position
     video_with_watermark = CompositeVideoClip(
-        [video, watermark.set_position((watermark_pos, "bottom"))]
+        [video, watermark.set_position((watermark_pos, "bottom"))],
     )
 
     # Write the output video
-    logger.info("Writing video file ...")
+    logger.info("Writing output video file...")
     video_with_watermark.write_videofile(
-        output_vid,
+        args.output_vid,
         codec="libx264",
         audio_codec="aac",
         fps=60,
         temp_audiofile="temp-audio.mp4",
         remove_temp=True,
     )
```

