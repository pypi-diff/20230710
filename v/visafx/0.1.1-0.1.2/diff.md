# Comparing `tmp/visafx-0.1.1-py3-none-any.whl.zip` & `tmp/visafx-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3086 bytes, number of entries: 7
+Zip file size: 3139 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 visafx/__init__.py
--rw-r--r--  2.0 unx     2016 b- defN 80-Jan-01 00:00 visafx/rates.py
+-rw-r--r--  2.0 unx     2235 b- defN 80-Jan-01 00:00 visafx/rates.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 visafx/test_rates.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      476 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.1.dist-info/RECORD
-7 files, 4684 bytes uncompressed, 2190 bytes compressed:  53.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      515 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.2.dist-info/RECORD
+7 files, 4942 bytes uncompressed, 2243 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: visafx/rates.py
 Comment: 
 
 Filename: visafx/test_rates.py
 Comment: 
 
-Filename: visafx-0.1.1.dist-info/LICENSE
+Filename: visafx-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: visafx-0.1.1.dist-info/METADATA
+Filename: visafx-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: visafx-0.1.1.dist-info/WHEEL
+Filename: visafx-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: visafx-0.1.1.dist-info/RECORD
+Filename: visafx-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visafx/rates.py

```diff
@@ -1,12 +1,13 @@
 import json
 from datetime import datetime
 from datetime import timedelta
 
 import cloudscraper
+from loguru import logger
 from pydantic import BaseModel
 from retry import retry
 
 
 class OriginalValues(BaseModel):
     fromCurrency: str
     fromCurrencyName: str
@@ -35,20 +36,19 @@
     benchMarkAmount: str
     fxRateWithAdditionalFee: str
     reverseAmount: str
     disclaimerDate: str
     status: str
 
 
-@retry()
-def rates(amount: float = 1.0,
-          from_curr: str = 'TWD',
-          to_curr: str = 'USD',
-          fee: float = 0.0,
-          date: datetime = None) -> Response:
+def _rates(amount: float = 1.0,
+           from_curr: str = 'TWD',
+           to_curr: str = 'USD',
+           fee: float = 0.0,
+           date: datetime = None) -> Response:
     url = 'http://www.visa.com.tw/cmsapi/fx/rates'
 
     if date is None:
         date = datetime.now()
 
     params = dict(
         amount=amount,
@@ -59,23 +59,38 @@
         fee=fee,
     )
 
     scraper = cloudscraper.create_scraper()
 
     resp = scraper.get(url=url, params=params)
 
+    return Response.parse_obj(resp.json())
+
+
+@retry()
+def rates(amount: float = 1.0,
+          from_curr: str = 'TWD',
+          to_curr: str = 'USD',
+          fee: float = 0.0,
+          date: datetime = None) -> Response:
+    if date is None:
+        date = datetime.now()
+
     try:
-        response = Response.parse_obj(resp.json())
-    except json.decoder.JSONDecodeError:
-        yesterday = date - timedelta(days=1)
-        params = dict(
+        resp = _rates(
+            amount=amount,
+            from_curr=from_curr,
+            to_curr=to_curr,
+            fee=fee,
+            date=date,
+        )
+    except json.decoder.JSONDecodeError as e:
+        logger.error(e)
+        resp = _rates(
             amount=amount,
-            utcConvertedDate=yesterday.strftime('%m/%d/%Y'),
-            exchangedate=yesterday.strftime('%m/%d/%Y'),
-            fromCurr=from_curr,
-            toCurr=to_curr,
+            from_curr=from_curr,
+            to_curr=to_curr,
             fee=fee,
+            date=date - timedelta(days=1),
         )
-        resp = scraper.get(url=url, params=params)
-        response = Response.parse_obj(resp.json())
 
-    return response
+    return resp
```

## Comparing `visafx-0.1.1.dist-info/LICENSE` & `visafx-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

