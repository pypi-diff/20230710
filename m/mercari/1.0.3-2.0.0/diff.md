# Comparing `tmp/mercari-1.0.3.tar.gz` & `tmp/mercari-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercari-1.0.3.tar", last modified: Thu Jul 21 01:50:17 2022, max compression
+gzip compressed data, was "mercari-2.0.0.tar", last modified: Mon Jul 10 17:34:55 2023, max compression
```

## Comparing `mercari-1.0.3.tar` & `mercari-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-07-21 01:50:17.784750 mercari-1.0.3/
--rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-06-05 23:48:30.000000 mercari-1.0.3/MANIFEST.in
--rw-r--r--   0 batmanuel   (501) staff       (20)     1785 2022-07-21 01:50:17.784618 mercari-1.0.3/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)     1472 2022-07-21 01:44:48.000000 mercari-1.0.3/README.md
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-07-21 01:50:17.783921 mercari-1.0.3/mercari/
--rw-r--r--   0 batmanuel   (501) staff       (20)     3750 2022-06-05 23:48:30.000000 mercari-1.0.3/mercari/DpopUtils.py
--rw-r--r--   0 batmanuel   (501) staff       (20)       28 2022-06-05 23:48:30.000000 mercari-1.0.3/mercari/__init__.py
--rw-r--r--   0 batmanuel   (501) staff       (20)     2558 2022-07-21 01:44:48.000000 mercari-1.0.3/mercari/mercari.py
-drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2022-07-21 01:50:17.784451 mercari-1.0.3/mercari.egg-info/
--rw-r--r--   0 batmanuel   (501) staff       (20)     1785 2022-07-21 01:50:17.000000 mercari-1.0.3/mercari.egg-info/PKG-INFO
--rw-r--r--   0 batmanuel   (501) staff       (20)      261 2022-07-21 01:50:17.000000 mercari-1.0.3/mercari.egg-info/SOURCES.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        1 2022-07-21 01:50:17.000000 mercari-1.0.3/mercari.egg-info/dependency_links.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      217 2022-07-21 01:50:17.000000 mercari-1.0.3/mercari.egg-info/requires.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)        8 2022-07-21 01:50:17.000000 mercari-1.0.3/mercari.egg-info/top_level.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)      217 2022-06-05 23:48:30.000000 mercari-1.0.3/requirements.txt
--rw-r--r--   0 batmanuel   (501) staff       (20)       38 2022-07-21 01:50:17.784789 mercari-1.0.3/setup.cfg
--rw-r--r--   0 batmanuel   (501) staff       (20)      663 2022-07-21 01:49:52.000000 mercari-1.0.3/setup.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.730478 mercari-2.0.0/
+-rw-r--r--   0 batmanuel   (501) staff       (20)       43 2022-06-05 23:48:30.000000 mercari-2.0.0/MANIFEST.in
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-10 17:34:55.730363 mercari-2.0.0/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1665 2023-07-10 17:32:18.000000 mercari-2.0.0/README.md
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.729215 mercari-2.0.0/mercari/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     3750 2022-06-05 23:48:30.000000 mercari-2.0.0/mercari/DpopUtils.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)       95 2023-07-10 17:28:22.000000 mercari-2.0.0/mercari/__init__.py
+-rw-r--r--   0 batmanuel   (501) staff       (20)     4407 2023-07-10 17:32:38.000000 mercari-2.0.0/mercari/mercari.py
+drwxr-xr-x   0 batmanuel   (501) staff       (20)        0 2023-07-10 17:34:55.730207 mercari-2.0.0/mercari.egg-info/
+-rw-r--r--   0 batmanuel   (501) staff       (20)     1978 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/PKG-INFO
+-rw-r--r--   0 batmanuel   (501) staff       (20)      261 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/SOURCES.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        1 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/dependency_links.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/requires.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)        8 2023-07-10 17:34:55.000000 mercari-2.0.0/mercari.egg-info/top_level.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)      217 2023-07-10 17:23:15.000000 mercari-2.0.0/requirements.txt
+-rw-r--r--   0 batmanuel   (501) staff       (20)       38 2023-07-10 17:34:55.730515 mercari-2.0.0/setup.cfg
+-rw-r--r--   0 batmanuel   (501) staff       (20)      663 2023-07-10 17:28:22.000000 mercari-2.0.0/setup.py
```

### Comparing `mercari-1.0.3/PKG-INFO` & `mercari-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercari
-Version: 1.0.3
+Version: 2.0.0
 Summary: mercari api-like wrapper
 Home-page: https://github.com/marvinody/mercari/
 Author: marvinody
 Author-email: manny@sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -19,42 +19,63 @@
 ```python
 import mercari
 
 for item in mercari.search("東方 ふもふも"):
     print("{}, {}".format(item.productName, item.productURL))
 ```
 
+**The search call will take a long time because it goes through all the pages to find every item.** It does not return parts where you paginate yourself.
+
 the item object contains the following properties:
 
 - id
 - productURL
 - imageURL
 - productName
 - price
 - status
 - soldOut
 
-## Google Proxy
-
-~~By default, the wrapper will try to use a google proxy to hide traffic. This is a bit finicky and I think google has wised up recently. To disable it and have your requests by direct to mercari, use it in the following way~~
-
-This is false now, and the google proxyy is removed. Because of how the api endpoint works, this had to be removed.
-
-I've left this part in here to not gaslight any one that it never existed.
-
+If you want to do more specific searching, you can use something like the following
 ```python
-import mercari
+from mercari import search, MercariSearchStatus, MercariSort, MercariOrder
 
-for item in mercari.search("東方 ふもふも", use_google_proxy=False):
+for item in search(
+        "",
+        sort=MercariSort.SORT_PRICE,
+        order=MercariOrder.ORDER_DESC,
+        status=MercariSearchStatus.SOLD_OUT
+    ):
     print("{}, {}".format(item.productName, item.productURL))
+
 ```
 
-The wrapper will throw on any 4xx or 5xx http status code.
+The defaults are currently:
+
+- `sort=MercariSort.SORT_CREATED_TIME`
+- `order=MercariOrder.ORDER_DESC` 
+- `status=MercariSearchStatus.ON_SALE`
+
+Which will sort by most recent to oldest, and only show on sale item.
+
+### MercariSort
+- STATUS_DEFAULT
+- STATUS_ON_SALE
+- STATUS_SOLD_OUT
+### MercariOrder
+- SORT_DEFAULT
+- SORT_CREATED_TIME
+- SORT_NUM_LIKES
+- SORT_SCORE
+- SORT_PRICE
+### MercariSearchStatus
+- ORDER_DESC
+- ORDER_ASC
 
-Main reason I've seen errors is because mercari decides to throw 403 if they blacklist your IP. I've tried to get around this with the google proxy, but it seems like google themselves are blocking either the IP or the mercari domain.
+You can also pass `excluded_keywords="something to exclude"` if you want to remove certain pieces from your search
 
 
 ## Development
 
 Clone this repo, install the dependencies in `requirement.txt` and off you go.
 
 ## Deploying / Publishing
```

### Comparing `mercari-1.0.3/mercari/DpopUtils.py` & `mercari-2.0.0/mercari/DpopUtils.py`

 * *Files identical despite different names*

### Comparing `mercari-1.0.3/mercari.egg-info/PKG-INFO` & `mercari-2.0.0/mercari.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercari
-Version: 1.0.3
+Version: 2.0.0
 Summary: mercari api-like wrapper
 Home-page: https://github.com/marvinody/mercari/
 Author: marvinody
 Author-email: manny@sadpanda.moe
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -19,42 +19,63 @@
 ```python
 import mercari
 
 for item in mercari.search("東方 ふもふも"):
     print("{}, {}".format(item.productName, item.productURL))
 ```
 
+**The search call will take a long time because it goes through all the pages to find every item.** It does not return parts where you paginate yourself.
+
 the item object contains the following properties:
 
 - id
 - productURL
 - imageURL
 - productName
 - price
 - status
 - soldOut
 
-## Google Proxy
-
-~~By default, the wrapper will try to use a google proxy to hide traffic. This is a bit finicky and I think google has wised up recently. To disable it and have your requests by direct to mercari, use it in the following way~~
-
-This is false now, and the google proxyy is removed. Because of how the api endpoint works, this had to be removed.
-
-I've left this part in here to not gaslight any one that it never existed.
-
+If you want to do more specific searching, you can use something like the following
 ```python
-import mercari
+from mercari import search, MercariSearchStatus, MercariSort, MercariOrder
 
-for item in mercari.search("東方 ふもふも", use_google_proxy=False):
+for item in search(
+        "",
+        sort=MercariSort.SORT_PRICE,
+        order=MercariOrder.ORDER_DESC,
+        status=MercariSearchStatus.SOLD_OUT
+    ):
     print("{}, {}".format(item.productName, item.productURL))
+
 ```
 
-The wrapper will throw on any 4xx or 5xx http status code.
+The defaults are currently:
+
+- `sort=MercariSort.SORT_CREATED_TIME`
+- `order=MercariOrder.ORDER_DESC` 
+- `status=MercariSearchStatus.ON_SALE`
+
+Which will sort by most recent to oldest, and only show on sale item.
+
+### MercariSort
+- STATUS_DEFAULT
+- STATUS_ON_SALE
+- STATUS_SOLD_OUT
+### MercariOrder
+- SORT_DEFAULT
+- SORT_CREATED_TIME
+- SORT_NUM_LIKES
+- SORT_SCORE
+- SORT_PRICE
+### MercariSearchStatus
+- ORDER_DESC
+- ORDER_ASC
 
-Main reason I've seen errors is because mercari decides to throw 403 if they blacklist your IP. I've tried to get around this with the google proxy, but it seems like google themselves are blocking either the IP or the mercari domain.
+You can also pass `excluded_keywords="something to exclude"` if you want to remove certain pieces from your search
 
 
 ## Development
 
 Clone this repo, install the dependencies in `requirement.txt` and off you go.
 
 ## Deploying / Publishing
```

### Comparing `mercari-1.0.3/setup.py` & `mercari-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mercari',
-    version='1.0.3',
+    version='2.0.0',
     author='marvinody',
     author_email='manny@sadpanda.moe',
     description='mercari api-like wrapper',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/marvinody/mercari/',
     packages=setuptools.find_packages(),
```

