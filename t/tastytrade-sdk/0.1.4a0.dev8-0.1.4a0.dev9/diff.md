# Comparing `tmp/tastytrade_sdk-0.1.4a0.dev8.tar.gz` & `tmp/tastytrade_sdk-0.1.4a0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev8.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev9.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.4a0.dev8.tar` & `tastytrade_sdk-0.1.4a0.dev9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1053 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/LICENSE
--rw-r--r--   0        0        0     1521 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/docs/users/README.md
--rw-r--r--   0        0        0      822 2023-07-10 15:04:42.614605 tastytrade_sdk-0.1.4a0.dev8/pyproject.toml
--rw-r--r--   0        0        0      587 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/__init__.py
--rw-r--r--   0        0        0     1450 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/account_streamer.py
--rw-r--r--   0        0        0     1275 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/accounts.py
--rw-r--r--   0        0        0     1473 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/models.py
--rw-r--r--   0        0        0     4408 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      172 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1177 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     1889 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     3073 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0     3133 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/orders.py
--rw-r--r--   0        0        0     1822 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     3171 2023-07-10 15:04:12.910061 tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/websocket.py
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-10 15:08:18.838180 tastytrade_sdk-0.1.4a0.dev9/LICENSE
+-rw-r--r--   0        0        0     1521 2023-07-10 15:08:18.838180 tastytrade_sdk-0.1.4a0.dev9/docs/users/README.md
+-rw-r--r--   0        0        0      822 2023-07-10 15:08:48.142738 tastytrade_sdk-0.1.4a0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      587 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/__init__.py
+-rw-r--r--   0        0        0     1450 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/account_streamer.py
+-rw-r--r--   0        0        0     1275 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/accounts.py
+-rw-r--r--   0        0        0     1473 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/models.py
+-rw-r--r--   0        0        0     4408 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1177 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     1889 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     3073 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0     3167 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/orders.py
+-rw-r--r--   0        0        0     1822 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     3171 2023-07-10 15:08:18.842180 tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/websocket.py
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev9/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.4a0.dev8/LICENSE` & `tastytrade_sdk-0.1.4a0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/docs/users/README.md` & `tastytrade_sdk-0.1.4a0.dev9/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/pyproject.toml` & `tastytrade_sdk-0.1.4a0.dev9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.4a0dev8"
+version = "0.1.4a0dev9"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/account_streamer.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/account_streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/accounts.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/accounts/models.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/accounts/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/orders.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 
 @dataclass
 class Order:
     """@private"""
     order_type: str
     time_in_force: str
-    price: float
-    price_effect: str
     legs: List[Leg]
+    price: Optional[float] = None
+    price_effect: Optional[str] = None
 
     @property
     def json(self) -> dict:
         return {
             'order-type': self.order_type,
             'time-in-force': self.time_in_force,
             'price': self.price,
```

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/tastytrade.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/src/tastytrade_sdk/websocket.py` & `tastytrade_sdk-0.1.4a0.dev9/src/tastytrade_sdk/websocket.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev8/PKG-INFO` & `tastytrade_sdk-0.1.4a0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.4a0.dev8
+Version: 0.1.4a0.dev9
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

