# Comparing `tmp/nintendeals-3.1.0.tar.gz` & `tmp/nintendeals-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nintendeals-3.1.0.tar", max compression
+gzip compressed data, was "nintendeals-3.1.1.tar", max compression
```

## Comparing `nintendeals-3.1.0.tar` & `nintendeals-3.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-07-08 11:59:27.068711 nintendeals-3.1.0/LICENSE
--rw-r--r--   0        0        0     8209 2023-07-08 11:59:27.068711 nintendeals-3.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/api/__init__.py
--rw-r--r--   0        0        0     3461 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/api/prices.py
--rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/__init__.py
--rw-r--r--   0        0        0     3285 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/eshops.py
--rw-r--r--   0        0        0     1839 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/games.py
--rw-r--r--   0        0        0     1074 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/classes/prices.py
--rw-r--r--   0        0        0      762 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/commons/enumerates.py
--rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/__init__.py
--rw-r--r--   0        0        0      114 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/api/__init__.py
--rw-r--r--   0        0        0     2089 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/api/algolia.py
--rw-r--r--   0        0        0     1482 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/info.py
--rw-r--r--   0        0        0      870 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/listing.py
--rw-r--r--   0        0        0        0 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/scrapers/__init__.py
--rw-r--r--   0        0        0     1075 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/scrapers/nintendo.py
--rw-r--r--   0        0        0      976 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/search.py
--rw-r--r--   0        0        0     1900 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noa/util.py
--rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/__init__.py
--rw-r--r--   0        0        0      117 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/api/__init__.py
--rw-r--r--   0        0        0     1927 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/api/nintendo.py
--rw-r--r--   0        0        0      846 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/info.py
--rw-r--r--   0        0        0      811 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/listing.py
--rw-r--r--   0        0        0      917 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/search.py
--rw-r--r--   0        0        0     2248 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noe/util.py
--rw-r--r--   0        0        0      107 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/__init__.py
--rw-r--r--   0        0        0      117 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/api/__init__.py
--rw-r--r--   0        0        0     1159 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/api/nintendo.py
--rw-r--r--   0        0        0      744 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/info.py
--rw-r--r--   0        0        0      725 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/listing.py
--rw-r--r--   0        0        0      832 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/search.py
--rw-r--r--   0        0        0     1832 2023-07-08 11:59:27.068711 nintendeals-3.1.0/nintendeals/noj/util.py
--rw-r--r--   0        0        0     1085 2023-07-08 11:59:27.068711 nintendeals-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     9607 1970-01-01 00:00:00.000000 nintendeals-3.1.0/setup.py
--rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 nintendeals-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-10 08:32:50.008515 nintendeals-3.1.1/LICENSE
+-rw-r--r--   0        0        0     8209 2023-07-10 08:32:50.008515 nintendeals-3.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/api/__init__.py
+-rw-r--r--   0        0        0     3461 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/api/prices.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/classes/__init__.py
+-rw-r--r--   0        0        0     3285 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/classes/eshops.py
+-rw-r--r--   0        0        0     1839 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/classes/games.py
+-rw-r--r--   0        0        0     1074 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/classes/prices.py
+-rw-r--r--   0        0        0      762 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/commons/enumerates.py
+-rw-r--r--   0        0        0      107 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/api/__init__.py
+-rw-r--r--   0        0        0     2089 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/api/algolia.py
+-rw-r--r--   0        0        0     1482 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/info.py
+-rw-r--r--   0        0        0      870 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/listing.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/scrapers/__init__.py
+-rw-r--r--   0        0        0     1075 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/scrapers/nintendo.py
+-rw-r--r--   0        0        0      976 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/search.py
+-rw-r--r--   0        0        0     1900 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noa/util.py
+-rw-r--r--   0        0        0      107 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/api/__init__.py
+-rw-r--r--   0        0        0     2107 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/api/nintendo.py
+-rw-r--r--   0        0        0      846 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/info.py
+-rw-r--r--   0        0        0      811 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/listing.py
+-rw-r--r--   0        0        0      917 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/search.py
+-rw-r--r--   0        0        0     2248 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noe/util.py
+-rw-r--r--   0        0        0      107 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/api/__init__.py
+-rw-r--r--   0        0        0     1159 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/api/nintendo.py
+-rw-r--r--   0        0        0      744 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/info.py
+-rw-r--r--   0        0        0      725 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/listing.py
+-rw-r--r--   0        0        0      832 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/search.py
+-rw-r--r--   0        0        0     1832 2023-07-10 08:32:50.008515 nintendeals-3.1.1/nintendeals/noj/util.py
+-rw-r--r--   0        0        0     1085 2023-07-10 08:32:50.008515 nintendeals-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9607 1970-01-01 00:00:00.000000 nintendeals-3.1.1/setup.py
+-rw-r--r--   0        0        0     9424 1970-01-01 00:00:00.000000 nintendeals-3.1.1/PKG-INFO
```

### Comparing `nintendeals-3.1.0/LICENSE` & `nintendeals-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/README.md` & `nintendeals-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/api/prices.py` & `nintendeals-3.1.1/nintendeals/api/prices.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/commons/classes/eshops.py` & `nintendeals-3.1.1/nintendeals/commons/classes/eshops.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/commons/classes/games.py` & `nintendeals-3.1.1/nintendeals/commons/classes/games.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/commons/classes/prices.py` & `nintendeals-3.1.1/nintendeals/commons/classes/prices.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/commons/enumerates.py` & `nintendeals-3.1.1/nintendeals/commons/enumerates.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/api/algolia.py` & `nintendeals-3.1.1/nintendeals/noa/api/algolia.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/info.py` & `nintendeals-3.1.1/nintendeals/noa/info.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/listing.py` & `nintendeals-3.1.1/nintendeals/noa/listing.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/scrapers/nintendo.py` & `nintendeals-3.1.1/nintendeals/noa/scrapers/nintendo.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/search.py` & `nintendeals-3.1.1/nintendeals/noa/search.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noa/util.py` & `nintendeals-3.1.1/nintendeals/noa/util.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noe/api/nintendo.py` & `nintendeals-3.1.1/nintendeals/noe/api/nintendo.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,24 +44,28 @@
 
         if not len(json):
             break
 
         for data in json:
             nsuids = data.get("nsuid_txt", [])
             product_codes = data["product_code_txt"] = [
-                pc.replace("-", "") for pc in data.get("product_code_txt", []) if pc[:3] in PRODUCT_CODE_PREFIXES
+                pc.replace("-", "") for pc in data.get("product_code_txt", []) if pc[:3] == PRODUCT_CODE_PREFIXES
             ]
 
             if not any((nsuids, product_codes)):
                 continue
 
-            data["nsuid_txt"] = nsuids[0] if nsuids else 0
-            data["product_code_txt"] = product_codes[0] if product_codes else 0
+            for i in range(0, max(len(nsuids), len(product_codes))):
+                nsuid = nsuids[i] if i < len(nsuids) else None
+                product_code = product_codes[i] if i < len(product_codes) else None
 
-            yield data
+                data["nsuid_txt"] = nsuid
+                data["product_code_txt"] = product_code
+
+                yield data
 
 
 def search_by_nsuid(nsuid: str) -> Optional[dict]:
     try:
         return next(_search(nsuid=nsuid))
     except StopIteration:
         return None
```

### Comparing `nintendeals-3.1.0/nintendeals/noe/info.py` & `nintendeals-3.1.1/nintendeals/noe/info.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noe/listing.py` & `nintendeals-3.1.1/nintendeals/noe/listing.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noe/search.py` & `nintendeals-3.1.1/nintendeals/noe/search.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noe/util.py` & `nintendeals-3.1.1/nintendeals/noe/util.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noj/api/nintendo.py` & `nintendeals-3.1.1/nintendeals/noj/api/nintendo.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noj/info.py` & `nintendeals-3.1.1/nintendeals/noj/info.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noj/listing.py` & `nintendeals-3.1.1/nintendeals/noj/listing.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noj/search.py` & `nintendeals-3.1.1/nintendeals/noj/search.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/nintendeals/noj/util.py` & `nintendeals-3.1.1/nintendeals/noj/util.py`

 * *Files identical despite different names*

### Comparing `nintendeals-3.1.0/pyproject.toml` & `nintendeals-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "nintendeals"
 description = "Scraping tools for Nintendo Switch games and prices on NA, EU and JP."
 documentation = "https://github.com/fedecalendino/nintendeals/blob/main/README.md"
 homepage = "https://github.com/fedecalendino/nintendeals"
 license = "MIT"
 readme = "README.md"
-version = "3.1.0"
+version = "3.1.1"
 
 authors = [
   "Fede Calendino <fede@calendino.com>",
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nintendeals-3.1.0/setup.py` & `nintendeals-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'pycountry>=22.3.5,<23.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'requests>=2.28.1,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'nintendeals',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'Scraping tools for Nintendo Switch games and prices on NA, EU and JP.',
     'long_description': ' # nintendeals\n> "nintendeals was a bot, he loved learning and deals on nintendo\'s eshop." **LetsFunHans** 💬️\n\n[![Version](https://img.shields.io/pypi/v/nintendeals?logo=pypi)](https://pypi.org/project/nintendeals)\n[![Quality Gate Status](https://img.shields.io/sonar/alert_status/fedecalendino_nintendeals?logo=sonarcloud&server=https://sonarcloud.io)](https://sonarcloud.io/dashboard?id=fedecalendino_nintendeals)\n[![CodeCoverage](https://img.shields.io/sonar/coverage/fedecalendino_nintendeals?logo=sonarcloud&server=https://sonarcloud.io)](https://sonarcloud.io/dashboard?id=fedecalendino_nintendeals)\n\n-----\n\nNamed after the my old [reddit bot](https://reddit.com/u/nintendeals), nintendeals is now a library with \nall the scrapers and integrations of nintendo services that I used.\n\n\n## Terminology\n\nBefore getting into any details first we need too get into the same page with a few terms:\n\n### Region\n\nHere we have three regions NA, EU and JP each one corresponding to Nintendo of America (NoA), Nintendo of Europe (NoE)\nand Nintendo of Japan (NoJ). Each of these regions have set of countries they are "in charge of":\n\nNoA:\n  * Canada\n  * Mexico\n  * United Stated\n  \nNoE:\n  * Every country in the European Union\n  * Australia\n  * New Zealand\n  * South Africa\n  \nNoJ:\n  * Japan\n  \n### nsuid\n\nAn nsuid is a 14 digit long string which Nintendo uses to identify games on each region. \nTaking Breath of the Wild as an example, we have these 3 nsuids for it (one per region):\n\n```    \n  * 70010000000025 (NA)\n  * 70010000000023 (EU)\n  * 70010000000026 (JP)\n```\n    \n### Product Code\n\nThe product code is another type of ID that Nintendo uses, it usually is a 8/9 character long string.\nTaking Splatoon 2 as an example, we have these 3 product codes for it (one per region):\n\n```\n  * HACPAAB6B (NA)\n  * HACPAAB6C (EU)\n  *  HACAAB6A (JP)\n```\n\nThe difference with the nsuid is that the product code has a constant between all regions (`AAB6` in this example), \nand this is what I decided to call [unique_id](https://github.com/fedecalendino/nintendeals/blob/master/nintendeals/commons/classes/games.py#L56) \nand it is what we can you to join a game across all regions.\n\nYou can also see this code in the front of your Nintendo Switch [cartridge](https://media.karousell.com/media/photos/products/2019/08/17/splatoon_2_cartridge_only_1566040350_4f38e061_progressive.jpg).\n\n## Services\n\nThis library provides three types of services: Info, Listing, Searching and Pricing. Each region has a different \nversion of Info, Listing and Searching, but Pricing is the same for all as it only requires a country and an nsuid.\n\n### Listing\n\nEven thought there are different version for each region, they all work in the same way. Given a supported \nplatform ([for this library](https://github.com/fedecalendino/nintendeals/blob/master/nintendeals/constants.py#L15))\nthey will retrieve a list games in the selected region (in the form of an iterator).\n\n```python\nfrom nintendeals import noa\n\nfor game in noa.list_switch_games():\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> ARMS / 70010000000392\n>> Astro Duel Deluxe / 70010000000301\n>> Axiom Verge / 70010000000821\n>> Azure Striker GUNVOLT: STRIKER PACK / 70010000000645\n>> Beach Buggy Racing / 70010000000721\n```\n\n```python\nfrom nintendeals import noe\n\nfor game in noe.list_switch_games():\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> I and Me / 70010000000314\n>> In Between / 70010000009184\n>> Ghost 1.0 / 70010000001386\n>> Resident Evil 0 / 70010000012848\n>> 64.0 / 70010000020867\n```\n\n### Searching\n\nBuilt on top of the listing services, these provide a simple way to search for games by title or release_date:\n\n```python\nfrom nintendeals import noa\n\nfor game in noa.search_switch_games(query="Zelda"):\n    print(game.title, "/", game.nsuid)\n```\n\n```text\n>> The Legend of Zelda™: Link’s Awakening / 70010000020033\n>> The Legend of Zelda™: Link\'s Awakening: Dreamer Edition / None\n>> Cadence of Hyrule: Crypt of the NecroDancer Featuring The Legend of Zelda / 70010000021364\n>> The Legend of Zelda™: Breath of the Wild / 70010000000025\n```\n\n\n### Info\n\nOnce you have the nsuid of the game that you want, you can call the `game_info` service. And again, each region has their\nown version but they all work the same, but keep in mind that you need to use the correct nsuid for each region.\nComing back to the nsuid of Breath of the Wild as an example:\n\n```python\nfrom nintendeals import noa\n\ngame = noa.game_info("70010000000025")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.ca_fr)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> The Legend of Zelda™: Breath of the Wild\n>> HACPAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> ESRB Everyone 10+\n>> https://www.nintendo.com/fr_CA/games/detail/the-legend-of-zelda-breath-of-the-wild-switch\n>>  * Demo Available : False\n>>  * DLC Available : False\n>>  * Nintendo Switch Online Required : True\n>>  * Save Data Cloud Supported : True\n```\n\n```python\nfrom nintendeals import noe\n\ngame = noe.game_info("70010000000023")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.uk_en)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> The Legend of Zelda: Breath of the Wild\n>> HACPAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> PEGI 12\n>> https://www.nintendo.co.uk/Games/Nintendo-Switch/The-Legend-of-Zelda-Breath-of-the-Wild-1173609.html\n>>  * Amiibo Supported : True\n>>  * Demo Available : False\n>>  * DLC Available : False\n>>  * Nintendo Switch Online Required : False\n>>  * Save Data Cloud Supported : True\n>>  * Voice Chat Supported : False\n```\n\n```python\nfrom nintendeals import noj\n\ngame = noj.game_info("70010000000026")\nprint(game.title)\nprint(game.product_code, game.unique_id)\nprint(game.release_date)\nprint(game.players)\nprint(str(game.rating[0]), game.rating[1])\nprint(game.eshop.jp_jp)\n\nfor feature, value in game.features.items():\n    print(" *", str(feature), ":", value)\n```\n\n```text\n>> ゼルダの伝説\u3000ブレス オブ ザ ワイルド\n>> HACAAAAA AAAA\n>> 2017-03-03 00:00:00\n>> 1\n>> CERO B\n>> https://store-jp.nintendo.com/list/software/70010000000026.html\n>>  * Amiibo Supported : True\n>>  * DLC Available : True\n>>  * Nintendo Switch Online Required : False\n```\n\n\n### Pricing\n\nGiven a country code (using the alpha-2 iso standard) and a game or list of games this service will fetch the current \npricing of that/those games for that country. Since this service uses nsuids to fetch the price, make sure that the\ngames that you provide have the regional nsuid that matches the country that you want. For example, only the nsuid for\nthe American region will be able to fetch you the prices of Canada, Mexico and United Stated but not for Japan or Spain.\n\n```python\nfrom nintendeals import noe\nfrom nintendeals.api import prices\n\ngame = noe.game_info("70010000007705")\nprint(game.title)\nprint()\n\nprice = prices.get_price(game, country="CZ")  # Czech Republic\nprint(price.currency)\nprint(price.value)\nprint(price.sale_discount, "%")\nprint(price.sale_value)\nprint(price.sale_start)\nprint(price.sale_end)\n\n# Alternatively you can do this for the same effect:\nprice = game.price(country="CZ") \n``` \n\n```text\nDead Cells\n\nCZK\n625.0\n80 %\n500.0\n2020-04-19 22:00:00\n2020-05-03 21:59:59\n```\n\nTo reduce the amount of call to the prices api, you can also use the `get_prices` service that works in a similar way\nbut it expects a list of games instead of only one:\n\n```python\nfrom nintendeals import noa\nfrom nintendeals.api import prices\n\nbotw = noa.game_info("70010000000025")\nprint(botw.title)\nceleste = noa.game_info("70010000006442")\nprint(celeste.title)\n\nprint()\n\nprices = prices.get_prices([botw, celeste], country="US")\nfor nsuid, price in prices:\n    print(nsuid)\n    print(price.value)\n    print(price.sale_value)\n    print()\n```\n\n```text\nThe Legend of Zelda™: Breath of the Wild\nCeleste\n\n70010000000025\n59.99\nNone\n\n70010000006442\n19.99\n4.99\n```\n',
     'author': 'Fede Calendino',
     'author_email': 'fede@calendino.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fedecalendino/nintendeals',
```

### Comparing `nintendeals-3.1.0/PKG-INFO` & `nintendeals-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nintendeals
-Version: 3.1.0
+Version: 3.1.1
 Summary: Scraping tools for Nintendo Switch games and prices on NA, EU and JP.
 Home-page: https://github.com/fedecalendino/nintendeals
 License: MIT
 Keywords: nintendo,deals
 Author: Fede Calendino
 Author-email: fede@calendino.com
 Requires-Python: >=3.8,<4.0
```

