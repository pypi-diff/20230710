# Comparing `tmp/visafx-0.1.0-py3-none-any.whl.zip` & `tmp/visafx-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3009 bytes, number of entries: 7
+Zip file size: 3086 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 visafx/__init__.py
--rw-r--r--  2.0 unx     1694 b- defN 80-Jan-01 00:00 visafx/rates.py
--rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 visafx/test_rates.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      433 b- defN 80-Jan-01 00:00 visafx-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.0.dist-info/RECORD
-7 files, 4166 bytes uncompressed, 2113 bytes compressed:  49.3%
+-rw-r--r--  2.0 unx     2016 b- defN 80-Jan-01 00:00 visafx/rates.py
+-rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 visafx/test_rates.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      476 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 visafx-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      510 b- defN 16-Jan-01 00:00 visafx-0.1.1.dist-info/RECORD
+7 files, 4684 bytes uncompressed, 2190 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: visafx/rates.py
 Comment: 
 
 Filename: visafx/test_rates.py
 Comment: 
 
-Filename: visafx-0.1.0.dist-info/LICENSE
+Filename: visafx-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: visafx-0.1.0.dist-info/METADATA
+Filename: visafx-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: visafx-0.1.0.dist-info/WHEEL
+Filename: visafx-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: visafx-0.1.0.dist-info/RECORD
+Filename: visafx-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visafx/rates.py

```diff
@@ -62,10 +62,20 @@
     scraper = cloudscraper.create_scraper()
 
     resp = scraper.get(url=url, params=params)
 
     try:
         response = Response.parse_obj(resp.json())
     except json.decoder.JSONDecodeError:
-        response = rates(amount, from_curr, to_curr, fee, date - timedelta(days=1))
+        yesterday = date - timedelta(days=1)
+        params = dict(
+            amount=amount,
+            utcConvertedDate=yesterday.strftime('%m/%d/%Y'),
+            exchangedate=yesterday.strftime('%m/%d/%Y'),
+            fromCurr=from_curr,
+            toCurr=to_curr,
+            fee=fee,
+        )
+        resp = scraper.get(url=url, params=params)
+        response = Response.parse_obj(resp.json())
 
     return response
```

## visafx/test_rates.py

```diff
@@ -5,7 +5,10 @@
     amount = 1.0
     from_curr = 'TWD'
     to_curr = 'USD'
     resp = rates(amount=amount, from_curr=from_curr, to_curr=to_curr, fee=0.0)
     assert resp.originalValues.fromAmount == str(amount)
     assert resp.originalValues.fromCurrency == to_curr
     assert resp.originalValues.toCurrency == from_curr
+    assert resp.conversionAmountValue == str(amount)
+    assert resp.conversionFromCurrency == from_curr
+    assert resp.conversionToCurrency == to_curr
```

## Comparing `visafx-0.1.0.dist-info/LICENSE` & `visafx-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

