# Comparing `tmp/webclient_helper-0.0.5-py3-none-any.whl.zip` & `tmp/webclient_helper-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8464 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     7344 b- defN 20-Oct-21 19:07 webclient_helper/__init__.py
+Zip file size: 8476 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     7367 b- defN 22-Aug-18 15:47 webclient_helper/__init__.py
 -rw-rw-r--  2.0 unx    10132 b- defN 21-Sep-28 13:06 webclient_helper/client.py
--rw-rw-r--  2.0 unx      608 b- defN 22-Apr-11 02:29 webclient_helper-0.0.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     8516 b- defN 22-Apr-11 02:29 webclient_helper-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-11 02:29 webclient_helper-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 22-Apr-11 02:29 webclient_helper-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      603 b- defN 22-Apr-11 02:29 webclient_helper-0.0.5.dist-info/RECORD
-7 files, 27312 bytes uncompressed, 7386 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     8516 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      603 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/RECORD
+7 files, 27335 bytes uncompressed, 7398 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webclient_helper/__init__.py
 Comment: 
 
 Filename: webclient_helper/client.py
 Comment: 
 
-Filename: webclient_helper-0.0.5.dist-info/LICENSE.txt
+Filename: webclient_helper-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: webclient_helper-0.0.5.dist-info/METADATA
+Filename: webclient_helper-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: webclient_helper-0.0.5.dist-info/WHEEL
+Filename: webclient_helper-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: webclient_helper-0.0.5.dist-info/top_level.txt
+Filename: webclient_helper-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: webclient_helper-0.0.5.dist-info/RECORD
+Filename: webclient_helper-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webclient_helper/__init__.py

```diff
@@ -3,15 +3,15 @@
 import time
 import warnings
 from json import JSONDecodeError
 from urllib.parse import urlparse
 try:
     from bs4 import BeautifulSoup, FeatureNotFound
     import os.path
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     BeautifulSoup = None
 
 
 logger = fh.get_logger(__name__)
 
 
 def get_domain(url):
```

## Comparing `webclient_helper-0.0.5.dist-info/LICENSE.txt` & `webclient_helper-0.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `webclient_helper-0.0.5.dist-info/METADATA` & `webclient_helper-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: webclient-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: Helpful WebClient class to interact with APIs on the web
 Home-page: https://github.com/kenjyco/webclient-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/webclient-helper/tarball/v0.0.5
+Download-URL: https://github.com/kenjyco/webclient-helper/tarball/v0.0.6
 Keywords: webclient,api,requests,soup,beautifulsoup,lxml,http,rest,helper,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `webclient_helper-0.0.5.dist-info/RECORD` & `webclient_helper-0.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-webclient_helper/__init__.py,sha256=XIydlvOvlXAR3OkDElZ71NSX1QO-itKSZstu1Hcqgds,7344
+webclient_helper/__init__.py,sha256=cRkOx_vpF8ZOYD_kXmXH39gYwNAZvqWKPEHvjeyg8GQ,7367
 webclient_helper/client.py,sha256=QnRGhKWHIpob-kllmQ4LQ9I7uasDqIfHZPvH_zmyQIg,10132
-webclient_helper-0.0.5.dist-info/LICENSE.txt,sha256=INpf6xK6c1YT-PmCXwO_CNA-XdHaEbLGX4UWX2mIHHk,608
-webclient_helper-0.0.5.dist-info/METADATA,sha256=vktgYithkk4yoOqWpHyiXhjgWlq80ui55q4wFrbVR_0,8516
-webclient_helper-0.0.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-webclient_helper-0.0.5.dist-info/top_level.txt,sha256=Khq9ECpPecSzsRYLSD2ub0wdFIVCWkX9w72iEMK28Zg,17
-webclient_helper-0.0.5.dist-info/RECORD,,
+webclient_helper-0.0.6.dist-info/LICENSE.txt,sha256=INpf6xK6c1YT-PmCXwO_CNA-XdHaEbLGX4UWX2mIHHk,608
+webclient_helper-0.0.6.dist-info/METADATA,sha256=6zAlIJO6Q-F5mxfK8kUCq6InsfdGQKCv25pBKX573bA,8516
+webclient_helper-0.0.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+webclient_helper-0.0.6.dist-info/top_level.txt,sha256=Khq9ECpPecSzsRYLSD2ub0wdFIVCWkX9w72iEMK28Zg,17
+webclient_helper-0.0.6.dist-info/RECORD,,
```

