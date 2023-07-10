# Comparing `tmp/visafx-0.1.2-py3-none-any.whl.zip` & `tmp/visafx-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3139 bytes, number of entries: 7
+Zip file size: 3140 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 visafx/__init__.py
--rw-r--r--  2.0 unx     2235 b- defN 80-Jan-01 00:00 visafx/rates.py
+-rw-r--r--  2.0 unx     2242 b- defN 80-Jan-01 00:00 visafx/rates.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 visafx/test_rates.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      515 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.2.dist-info/RECORD
-7 files, 4942 bytes uncompressed, 2243 bytes compressed:  54.6%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      515 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.3.dist-info/RECORD
+7 files, 4949 bytes uncompressed, 2244 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: visafx/rates.py
 Comment: 
 
 Filename: visafx/test_rates.py
 Comment: 
 
-Filename: visafx-0.1.2.dist-info/LICENSE
+Filename: visafx-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: visafx-0.1.2.dist-info/METADATA
+Filename: visafx-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: visafx-0.1.2.dist-info/WHEEL
+Filename: visafx-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: visafx-0.1.2.dist-info/RECORD
+Filename: visafx-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visafx/rates.py

```diff
@@ -62,15 +62,15 @@
     scraper = cloudscraper.create_scraper()
 
     resp = scraper.get(url=url, params=params)
 
     return Response.parse_obj(resp.json())
 
 
-@retry()
+@retry(delay=1)
 def rates(amount: float = 1.0,
           from_curr: str = 'TWD',
           to_curr: str = 'USD',
           fee: float = 0.0,
           date: datetime = None) -> Response:
     if date is None:
         date = datetime.now()
```

## Comparing `visafx-0.1.2.dist-info/LICENSE` & `visafx-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visafx-0.1.2.dist-info/METADATA` & `visafx-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visafx
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: なるみ
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

