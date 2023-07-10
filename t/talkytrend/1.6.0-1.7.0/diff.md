# Comparing `tmp/talkytrend-1.6.0.tar.gz` & `tmp/talkytrend-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.6.0.tar", max compression
+gzip compressed data, was "talkytrend-1.7.0.tar", max compression
```

## Comparing `talkytrend-1.6.0.tar` & `talkytrend-1.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-07 16:02:48.571368 talkytrend-1.6.0/LICENSE
--rw-r--r--   0        0        0     3444 2023-07-07 16:02:48.571368 talkytrend-1.6.0/README.md
--rw-r--r--   0        0        0     2178 2023-07-07 16:02:49.383386 talkytrend-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-07 16:02:49.383386 talkytrend-1.6.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/config.py
--rw-r--r--   0        0        0     2087 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6714 2023-07-07 16:02:48.571368 talkytrend-1.6.0/talkytrend/main.py
--rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 talkytrend-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 11:13:58.383167 talkytrend-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-10 11:13:58.383167 talkytrend-1.7.0/README.md
+-rw-r--r--   0        0        0     2476 2023-07-10 11:13:59.199180 talkytrend-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-10 11:13:59.199180 talkytrend-1.7.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/config.py
+-rw-r--r--   0        0        0     2232 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7738 2023-07-10 11:13:58.383167 talkytrend-1.7.0/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.0/PKG-INFO
```

### Comparing `talkytrend-1.6.0/LICENSE` & `talkytrend-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.6.0/README.md` & `talkytrend-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/v/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/dm/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-      <a href="https://talkyuniverse.readthedocs.io/projects/talkytrend/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
+      <a href="https://talky.readthedocs.io/projects/talkytrend/en/latest/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
       <a href="https://codebeat.co/projects/github-com-mraniki-talkytrend-main"><img src="https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6"/></a> <br>
       <a href="https://codecov.io/gh/mraniki/talkytrend"><img src="https://codecov.io/gh/mraniki/talkytrend/branch/main/graph/badge.svg?token=WAHUEMAJN6"/></a><br>
     </td>
     <td align="left"> 
 Retrieve asset trend and economic data.<br>
 Trading view connectivity with signal scanner<br>
 News connectivity<br>
```

### Comparing `talkytrend-1.6.0/pyproject.toml` & `talkytrend-1.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+
 [tool.poetry]
 name = "talkytrend"
-version = "1.6.0"
+version = "1.7.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -18,22 +24,39 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 aiohttp = "^3.8.4"
 tradingview_ta = "^3.3.0"
 prettytable = "^3.8.0"
+alphavantage_api_client = "^2.2.2"
+xmltodict = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0.0"
+sphinx_bootstrap_theme = "^0.8.1"
+sphinx-autoapi = "^2.1.1"
+sphinx-copybutton= "^0.5.2"
+myst-parser = "^2.0.0"
+sphinx-notfound-page = "^0.8.3"
+sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx-togglebutton = "*"
+
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 
@@ -41,24 +64,14 @@
 omit = [
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
-[tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.1"
-sphinx-autoapi = "^2.1.0"
-furo = "^2023.5.20"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","talkytrend/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 commit_parser = "semantic_release.history.emoji_parser"
```

### Comparing `talkytrend-1.6.0/talkytrend/config.py` & `talkytrend-1.7.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.6.0/talkytrend/default_settings.toml` & `talkytrend-1.7.0/talkytrend/default_settings.toml`

 * *Files 10% similar despite different names*

```diff
@@ -31,29 +31,33 @@
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
 enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&max=2&apikey="
 news_api_key = ""
+enable_feed = true
+news_feed="http://feeds.feedburner.com/zerohedge/feed"
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
 
 
 
 [testing]
 VALUE = "On Testing"
 talkytrend_enabled = true
 talkytrend_mode = "scanner"
 talkytrend_scanner = false
 talkytrend_scheduler = false
-scanner_frequency = 86400
+scanner_frequency = 2
 enable_signals = true
 assets = [
-    { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
+    { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
 ]
 enable_events = true
 economic_calendar = "https://nfs.faireconomy.media/ff_calendar_thisweek.json"
 fomc_decision_date = ["2023-07-26","2023-09-20","2023-11-01","2023-12-13"]
-enable_news = true
+enable_news = false
 news_url="https://gnews.io/api/v4/top-headlines?category=business&lang=en&country=us&max=2&apikey="
 news_api_key = ""
+enable_feed = true
+news_feed="http://feeds.feedburner.com/zerohedge/feed"
 live_tv_url = "https://bloomberg.com/media-manifest/streams/us.m3u8"
```

### Comparing `talkytrend-1.6.0/talkytrend/main.py` & `talkytrend-1.7.0/talkytrend/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
  talky trend Main
 """
 
 import asyncio
 import logging
 from datetime import date
 import aiohttp
-from prettytable import PrettyTable, MARKDOWN
+import xmltodict
+from prettytable import PrettyTable
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from talkytrend.config import settings
 
 
 class TalkyTrend:
     def __init__(self):
@@ -19,15 +20,19 @@
             self.enabled = settings.talkytrend_enabled
             if not self.enabled:
                 return
             self.mode = settings.talkytrend_mode
             self.assets = settings.assets
             self.asset_signals = {}
             self.economic_calendar = settings.economic_calendar
-            self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else settings.news_url
+            self.news_url = (
+                f"{settings.news_url}{settings.news_api_key}"
+                if settings.news_api_key
+                else settings.news_url
+            )
             self.live_tv = settings.live_tv_url
             print(self.news_url)
         except Exception as error:
             self.logger.error("TalkyTrend init error %s", error)
 
     async def fetch_analysis(
         self,
@@ -57,15 +62,15 @@
         except Exception as error:
             self.logger.error("event %s", error)
 
     async def check_signal(self):
         try:
             signals = []
             table = PrettyTable()
-            table.field_names = ["   Asset  ","   4h  "]
+            table.field_names = ["Asset","4h"]
             for asset in self.assets:
                 current_signal = await self.fetch_analysis(
                     asset_id=asset["id"],
                     exchange=asset["exchange"],
                     screener=asset["screener"],
                     interval=asset["interval"]
                 )
@@ -74,24 +79,26 @@
                         "symbol": asset["id"],
                         "interval": asset["interval"],
                         "signal": current_signal
                     }
                     self.update_signal(asset["id"], asset["interval"], current_signal)
                     table.add_row([asset["id"], current_signal])
                     signals.append(signal_item)
-            table.set_style(MARKDOWN)
 
-            return table.get_string()
+            return table.get_html_string()
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
     def is_new_signal(self, asset_id, interval, current_signal):
         if self.asset_signals.get(asset_id):
-            if self.asset_signals[asset_id].get(interval) and current_signal != self.asset_signals[asset_id][interval]:
+            if (
+                self.asset_signals[asset_id].get(interval)
+                and current_signal != self.asset_signals[asset_id][interval]
+            ):
                 self.asset_signals[asset_id][interval] = current_signal
                 return True
         else:
             self.asset_signals[asset_id] = {interval: current_signal}
             return True
         return False
 
@@ -102,15 +109,18 @@
         return self.asset_signals
 
     async def fetch_key_events(self):
         def filter_events(data, today):
             return [event for event in data if event.get('date', '').startswith(today)]
 
         def is_usd_high_impact(event):
-            return event.get('impact') == 'High' and event.get('country') in {'USD', 'ALL'}
+            return (
+                event.get('impact') == 'High' and
+                event.get('country') in {'USD', 'ALL'}
+            )
 
         def is_all_high_impact(event):
             return event.get('impact') == 'High' and event.get('country') == 'ALL'
 
         def is_opec_or_fomc(event):
             return "OPEC" in event.get('title') or "FOMC" in event.get('title')
 
@@ -132,45 +142,66 @@
 
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
-                    key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
+                    key_news = [
+                        {'title': article['title'], 'url': article['url']}
+                        for article in articles
+                    ]
                     last_item = key_news[-1]
-                    return str(f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>")
+                    return f"📰 <a href='{last_item['url']}'>{last_item['title']}</a>"
+
+        except aiohttp.ClientError as error:
+            self.logger.error("news %s", error)
+            return None
 
+    async def fetch_key_feed(self):
+        try:
+            async with aiohttp.ClientSession() as session:
+                async with session.get(settings.news_feed, timeout=10) as response:
+                    data = (
+                        xmltodict.parse(await response.text())
+                        .get('rss')
+                        .get('channel')['item'][0]
+                    )
+                    title = data['title']
+                    link = data['link']
+                    return f"📰 <a href='{link}'>{title}</a>"
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
+
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
+     
+    async def allow_scanning(self, enable=True):
+        return bool(enable)
 
     async def scanner(self):
-        while True:
+        while await self.allow_scanning():
             try:
                 if settings.enable_events:
-                    key_events = await self.fetch_key_events()
-                    if key_events is not None:
-                        yield key_events
+                    if await self.fetch_key_events() is not None:
+                        yield await self.fetch_key_events()
                 if settings.enable_news:
-                    key_news = await self.fetch_key_news()
-                    if key_news is not None:
-                        yield key_news
-
+                    if await self.fetch_key_news() is not None:
+                        yield await self.fetch_key_news()
+                if settings.enable_feed:
+                    if await self.fetch_key_feed() is not None:
+                        yield await self.fetch_key_feed()
                 if settings.enable_signals:
-                    signals = await self.check_signal()
-                    if signals is not None:
-                        yield signals
+                    if await self.check_signal() is not None:
+                        yield await self.check_signal()
+
+                await asyncio.sleep(settings.scanner_frequency)
 
             except Exception as error:
-                print(error)
                 raise error
 
-            await asyncio.sleep(settings.scanner_frequency)
-
     async def get_info(self):
         return f"{__class__.__name__} {__version__}\n"
```

### Comparing `talkytrend-1.6.0/PKG-INFO` & `talkytrend-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: prettytable (>=3.8.0,<4.0.0)
 Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0)
+Requires-Dist: xmltodict
 Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/talkytrend/issues
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 <br>
 
@@ -38,15 +40,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/226854338-e900f69e-d884-4a9a-90b1-b3dde7711b31.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/v/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/talkytrend/"><img src="https://img.shields.io/pypi/dm/talkytrend?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://github.com/mraniki/talkytrend/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/talkytrend/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-      <a href="https://talkyuniverse.readthedocs.io/projects/talkytrend/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
+      <a href="https://talky.readthedocs.io/projects/talkytrend/en/latest/"><img src="https://readthedocs.org/projects/talkytrend/badge/?version=latest&style=for-the-badge"></a><br>
       <a href="https://codebeat.co/projects/github-com-mraniki-talkytrend-main"><img src="https://codebeat.co/badges/24c90aab-02d7-4cd1-9ad8-5907e180c9e6"/></a> <br>
       <a href="https://codecov.io/gh/mraniki/talkytrend"><img src="https://codecov.io/gh/mraniki/talkytrend/branch/main/graph/badge.svg?token=WAHUEMAJN6"/></a><br>
     </td>
     <td align="left"> 
 Retrieve asset trend and economic data.<br>
 Trading view connectivity with signal scanner<br>
 News connectivity<br>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.6.0 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.7.0 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
-(>=3.8.4,<4.0.0) Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist:
-prettytable (>=3.8.0,<4.0.0) Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0)
-Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/dev/
-CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/talkytrend/issues
-Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
+(>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist: prettytable
+(>=3.8.0,<4.0.0) Requires-Dist: tradingview_ta (>=3.3.0,<4.0.0) Requires-Dist:
+xmltodict Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/
+dev/CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/talkytrend/
+issues Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 *** TalkyTrend ***
 
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
```

