# Comparing `tmp/talkytrend-1.7.0.tar.gz` & `tmp/talkytrend-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.7.0.tar", max compression
+gzip compressed data, was "talkytrend-1.7.1.tar", max compression
```

## Comparing `talkytrend-1.7.0.tar` & `talkytrend-1.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-10 11:13:58.383167 talkytrend-1.7.0/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-10 11:13:58.383167 talkytrend-1.7.0/README.md
--rw-r--r--   0        0        0     2476 2023-07-10 11:13:59.199180 talkytrend-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-10 11:13:59.199180 talkytrend-1.7.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/config.py
--rw-r--r--   0        0        0     2232 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7738 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 19:12:12.236456 talkytrend-1.7.1/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-10 19:12:12.236456 talkytrend-1.7.1/README.md
+-rw-r--r--   0        0        0     2476 2023-07-10 19:12:13.104477 talkytrend-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-10 19:12:13.104477 talkytrend-1.7.1/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-10 19:12:12.236456 talkytrend-1.7.1/talkytrend/config.py
+-rw-r--r--   0        0        0     2232 2023-07-10 19:12:12.236456 talkytrend-1.7.1/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7777 2023-07-10 19:12:12.236456 talkytrend-1.7.1/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.1/PKG-INFO
```

### Comparing `talkytrend-1.7.0/LICENSE` & `talkytrend-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.0/README.md` & `talkytrend-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.0/pyproject.toml` & `talkytrend-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.7.0"
+version = "1.7.1"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.7.0/talkytrend/config.py` & `talkytrend-1.7.1/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.0/talkytrend/default_settings.toml` & `talkytrend-1.7.1/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.0/talkytrend/main.py` & `talkytrend-1.7.1/talkytrend/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
                         "symbol": asset["id"],
                         "interval": asset["interval"],
                         "signal": current_signal
                     }
                     self.update_signal(asset["id"], asset["interval"], current_signal)
                     table.add_row([asset["id"], current_signal])
                     signals.append(signal_item)
-
-            return table.get_html_string()
+            return table.get_string()
+            # return table.get_html_string()
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
     def is_new_signal(self, asset_id, interval, current_signal):
         if self.asset_signals.get(asset_id):
             if (
```

### Comparing `talkytrend-1.7.0/PKG-INFO` & `talkytrend-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.7.0 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.7.1 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

