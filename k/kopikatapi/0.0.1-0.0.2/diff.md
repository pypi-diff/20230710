# Comparing `tmp/kopikatapi-0.0.1.tar.gz` & `tmp/kopikatapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopikatapi-0.0.1.tar", max compression
+gzip compressed data, was "kopikatapi-0.0.2.tar", max compression
```

## Comparing `kopikatapi-0.0.1.tar` & `kopikatapi-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/LICENSE
--rw-r--r--   0        0        0     1156 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/README.md
--rw-r--r--   0        0        0      230 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/kopikatapi/__init__.py
--rw-r--r--   0        0        0      276 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/kopikatapi/enums.py
--rw-r--r--   0        0        0     4762 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/kopikatapi/kopikatapi.py
--rw-r--r--   0        0        0     2993 2023-07-09 12:10:33.924453 kopikatapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 kopikatapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-09 23:00:20.680242 kopikatapi-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1280 2023-07-09 23:00:20.680242 kopikatapi-0.0.2/README.md
+-rw-r--r--   0        0        0      306 2023-07-09 23:00:20.680242 kopikatapi-0.0.2/kopikatapi/__init__.py
+-rw-r--r--   0        0        0      391 2023-07-09 23:00:20.680242 kopikatapi-0.0.2/kopikatapi/enums.py
+-rw-r--r--   0        0        0     6820 2023-07-09 23:00:20.680242 kopikatapi-0.0.2/kopikatapi/kopikatapi.py
+-rw-r--r--   0        0        0     3979 2023-07-09 23:00:20.684242 kopikatapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2881 1970-01-01 00:00:00.000000 kopikatapi-0.0.2/PKG-INFO
```

### Comparing `kopikatapi-0.0.1/LICENSE` & `kopikatapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kopikatapi-0.0.1/README.md` & `kopikatapi-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -28,10 +28,14 @@
 kopikatAPI = KopikatAPI(api_key)
 kopikatAPI.augment_image_file('image.png', 'summer time')
 cv2.imshow("output",kopikatAPI.cv2_image())
 cv2.waitKey(0)
 
 ```
 
+## Get your API Key
+
+Contact with kopikat team from [here](https://kopikat.gitbook.io/api/quick-start#1.-get-your-api-key)
+
 
 ## Disclaimers
 This is not an official Kopikat product. This is a personal project and is not affiliated with Kopikat in any way.
```

#### html2text {}

```diff
@@ -6,10 +6,12 @@
 enlarge and diversify datasets and is specifically helpful for datasets with up
 to 5,000 images that are typical for real-life AI projects. ## ð»
 Installation You can install the `KopikatAPI` library using pip in between
 [Python**3.11>=Python>=3.8**](https://www.python.org/) environment. ```bash pip
 install kopikatapi ``` ## ð¥ Quickstart ```python from kopikatapi import
 KopikatAPI import cv2 api_key: str = 'ENTER YOUR API KEY HERE' kopikatAPI =
 KopikatAPI(api_key) kopikatAPI.augment_image_file('image.png', 'summer time')
-cv2.imshow("output",kopikatAPI.cv2_image()) cv2.waitKey(0) ``` ## Disclaimers
-This is not an official Kopikat product. This is a personal project and is not
-affiliated with Kopikat in any way.
+cv2.imshow("output",kopikatAPI.cv2_image()) cv2.waitKey(0) ``` ## Get your API
+Key Contact with kopikat team from [here](https://kopikat.gitbook.io/api/quick-
+start#1.-get-your-api-key) ## Disclaimers This is not an official Kopikat
+product. This is a personal project and is not affiliated with Kopikat in any
+way.
```

### Comparing `kopikatapi-0.0.1/PKG-INFO` & `kopikatapi-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopikatapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kopikat.co Python Client for API access
 Author: Onuralp SEZER
 Author-email: thunderbirdtr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -63,11 +63,15 @@
 kopikatAPI = KopikatAPI(api_key)
 kopikatAPI.augment_image_file('image.png', 'summer time')
 cv2.imshow("output",kopikatAPI.cv2_image())
 cv2.waitKey(0)
 
 ```
 
+## Get your API Key
+
+Contact with kopikat team from [here](https://kopikat.gitbook.io/api/quick-start#1.-get-your-api-key)
+
 
 ## Disclaimers
 This is not an official Kopikat product. This is a personal project and is not affiliated with Kopikat in any way.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kopikatapi Version: 0.0.1 Summary: Kopikat.co
+Metadata-Version: 2.1 Name: kopikatapi Version: 0.0.2 Summary: Kopikat.co
 Python Client for API access Author: Onuralp SEZER Author-email:
 thunderbirdtr@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -28,10 +28,12 @@
 enlarge and diversify datasets and is specifically helpful for datasets with up
 to 5,000 images that are typical for real-life AI projects. ## ð»
 Installation You can install the `KopikatAPI` library using pip in between
 [Python**3.11>=Python>=3.8**](https://www.python.org/) environment. ```bash pip
 install kopikatapi ``` ## ð¥ Quickstart ```python from kopikatapi import
 KopikatAPI import cv2 api_key: str = 'ENTER YOUR API KEY HERE' kopikatAPI =
 KopikatAPI(api_key) kopikatAPI.augment_image_file('image.png', 'summer time')
-cv2.imshow("output",kopikatAPI.cv2_image()) cv2.waitKey(0) ``` ## Disclaimers
-This is not an official Kopikat product. This is a personal project and is not
-affiliated with Kopikat in any way.
+cv2.imshow("output",kopikatAPI.cv2_image()) cv2.waitKey(0) ``` ## Get your API
+Key Contact with kopikat team from [here](https://kopikat.gitbook.io/api/quick-
+start#1.-get-your-api-key) ## Disclaimers This is not an official Kopikat
+product. This is a personal project and is not affiliated with Kopikat in any
+way.
```

