# Comparing `tmp/crypto-screening-2.6.2.tar.gz` & `tmp/crypto-screening-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.6.2.tar", last modified: Sun Jul  9 13:52:08 2023, max compression
+gzip compressed data, was "crypto-screening-2.6.3.tar", last modified: Mon Jul 10 17:18:02 2023, max compression
```

## Comparing `crypto-screening-2.6.2.tar` & `crypto-screening-2.6.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.444486 crypto-screening-2.6.2/
--rw-rw-rw-   0        0        0       98 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-09 13:52:08.444486 crypto-screening-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.6.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.6.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.423502 crypto-screening-2.6.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.435264 crypto-screening-2.6.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.6.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.6.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    52089 2023-07-09 13:51:36.000000 crypto-screening-2.6.2/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.6.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.6.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.6.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.6.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.6.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.437312 crypto-screening-2.6.2/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.6.2/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.439374 crypto-screening-2.6.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.6.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.6.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.6.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.6.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.443473 crypto-screening-2.6.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.6.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.6.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.6.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.6.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.6.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-09 13:52:08.432676 crypto-screening-2.6.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-09 13:52:08.000000 crypto-screening-2.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.6.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.6.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 13:52:08.444486 crypto-screening-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-09 13:52:04.000000 crypto-screening-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/
+-rw-rw-rw-   0        0        0       98 2023-07-10 17:18:00.000000 crypto-screening-2.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.6.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.6.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.629648 crypto-screening-2.6.3/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.666652 crypto-screening-2.6.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.6.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.6.3/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    52089 2023-07-09 13:51:36.000000 crypto-screening-2.6.3/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11824 2023-07-10 16:42:59.000000 crypto-screening-2.6.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.6.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.6.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.6.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.6.3/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.678210 crypto-screening-2.6.3/crypto_screening/market/
+-rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.6.3/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.702183 crypto-screening-2.6.3/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.743183 crypto-screening-2.6.3/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.6.3/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.6.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.6.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.6.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.644647 crypto-screening-2.6.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-10 17:18:00.000000 crypto-screening-2.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.6.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.6.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-10 17:17:46.000000 crypto-screening-2.6.3/setup.py
```

### Comparing `crypto-screening-2.6.2/PKG-INFO` & `crypto-screening-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.6.2
+Version: 2.6.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.6.2/README.md` & `crypto-screening-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/build.py` & `crypto-screening-2.6.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/collect/assets.py` & `crypto-screening-2.6.3/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/collect/exchanges.py` & `crypto-screening-2.6.3/crypto_screening/collect/exchanges.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from crypto_screening.exchanges import EXCHANGE_NAMES
 from crypto_screening.validate import validate_exchange
 from crypto_screening.process import (
     find_string_value, lower_string_values
 )
 
 __all__ = [
-    "exchanges_data"
+    "exchanges_data",
+    "exchanges_values"
 ]
 
 _R = TypeVar("_R")
 
 Collector = Callable[
     [
         str,
@@ -26,14 +27,46 @@
         Optional[bool],
         Optional[Iterable[str]],
         Optional[Iterable[str]],
         Optional[Iterable[str]]
     ], _R
 ]
 
+def exchanges_values(
+        exchanges: Iterable[str],
+        values: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+) -> Dict[str, Iterable[str]]:
+    """
+    Collects the values to the structure of the exchanges.
+
+    :param exchanges: The exchanges for the structure.
+    :param values: The values to process.
+
+    :return: The structured exchanges' data.
+    """
+
+    values_data = []
+
+    values = values or {}
+
+    if values:
+        values_data = values
+    # end if
+
+    if (
+        values and
+        all(isinstance(value, str) for value in values) and
+        not isinstance(values, dict)
+    ):
+        values = {exchange: values_data for exchange in exchanges}
+    # end if
+
+    return values
+# end exchanges_values
+
 def exchanges_data(
         collector: Collector,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         exchanges: Optional[Iterable[str]] = None,
         bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
         quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
@@ -52,32 +85,21 @@
     :param included: The symbols to include.
     :param excluded: The excluded symbols.
     :param bases: The bases of the asset pairs.
 
     :return: The data of the exchanges.
     """
 
-    excluded_symbols = []
-
-    excluded = excluded or {}
-
-    if not excluded:
-        excluded_symbols = excluded
-    # end if
-
-    if (
-        excluded and
-        all(isinstance(value, str) for value in excluded) and
-        not isinstance(excluded, dict)
-    ):
-        excluded = {exchange: excluded_symbols for exchange in exchanges}
-    # end if
-
     exchanges = lower_string_values(exchanges or EXCHANGE_NAMES)
 
+    bases = exchanges_values(exchanges=exchanges, values=bases)
+    quotes = exchanges_values(exchanges=exchanges, values=quotes)
+    included = exchanges_values(exchanges=exchanges, values=included)
+    excluded = exchanges_values(exchanges=exchanges, values=excluded)
+
     markets = []
 
     for exchange in exchanges:
         exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
         if exchange not in EXCHANGE_NAMES:
             if adjust:
```

### Comparing `crypto-screening-2.6.2/crypto_screening/collect/market.py` & `crypto-screening-2.6.3/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/collect/screeners.py` & `crypto-screening-2.6.3/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/collect/symbols.py` & `crypto-screening-2.6.3/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/dataset.py` & `crypto-screening-2.6.3/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/interval.py` & `crypto-screening-2.6.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/dynamic.py` & `crypto-screening-2.6.3/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/foundation/data.py` & `crypto-screening-2.6.3/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.6.3/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/foundation/state.py` & `crypto-screening-2.6.3/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.6.3/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/screeners/base.py` & `crypto-screening-2.6.3/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/screeners/container.py` & `crypto-screening-2.6.3/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.6.3/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.6.3/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.6.3/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/market/waiting.py` & `crypto-screening-2.6.3/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/process.py` & `crypto-screening-2.6.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/symbols.py` & `crypto-screening-2.6.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/crypto_screening/validate.py` & `crypto-screening-2.6.3/crypto_screening/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     if not is_valid_symbol(
             exchange=exchange, symbol=symbol, symbols=symbols
     ):
         raise ValueError(
             f"'{symbol}' is not a valid "
             f"symbol for the '{exchange}' exchange. "
-            f"Valid symbols: {', '.join(symbols)}"
+            f"Valid symbols: {', '.join(symbols or [])}"
             f"{f' for {provider}.' if provider else ''}"
         )
     # end if
 
     return symbol
 # end validate_symbol
 
@@ -130,14 +130,14 @@
     if exchanges is None:
         exchanges = EXCHANGE_NAMES
     # end if
 
     if not is_valid_exchange(exchange=exchange, exchanges=exchanges):
         raise ValueError(
             f"'{exchange}' is not a valid exchange name. "
-            f"Valid exchanges: {', '.join(exchanges)}"
+            f"Valid exchanges: {', '.join(exchanges or [])}"
             f"{f' for {provider}.' if provider else ''}"
         )
     # end if
 
     return exchange
 # end validate_exchange
```

### Comparing `crypto-screening-2.6.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.6.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.6.2
+Version: 2.6.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.6.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.6.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.2/pyproject.toml` & `crypto-screening-2.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.6.2'
+version = '2.6.3'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.6.2/setup.py` & `crypto-screening-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.6.2',
+        version='2.6.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

