# Comparing `tmp/picimagesearch-3.9.2.tar.gz` & `tmp/picimagesearch-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picimagesearch-3.9.2.tar", max compression
+gzip compressed data, was "picimagesearch-3.9.3.tar", max compression
```

## Comparing `picimagesearch-3.9.2.tar` & `picimagesearch-3.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/LICENSE
--rw-r--r--   0        0        0      251 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/ascii2d.py
--rw-r--r--   0        0        0     1267 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/baidu.py
--rw-r--r--   0        0        0     1433 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/ehentai.py
--rw-r--r--   0        0        0     2421 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/google.py
--rw-r--r--   0        0        0     1215 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/iqdb.py
--rw-r--r--   0        0        0      397 2023-05-25 12:08:52.671666 picimagesearch-3.9.2/PicImageSearch/model/__init__.py
--rw-r--r--   0        0        0     2656 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/ascii2d.py
--rw-r--r--   0        0        0      778 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/baidu.py
--rw-r--r--   0        0        0     1895 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/ehentai.py
--rw-r--r--   0        0        0     2234 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/google.py
--rw-r--r--   0        0        0     3711 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/iqdb.py
--rw-r--r--   0        0        0     5170 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/saucenao.py
--rw-r--r--   0        0        0     2755 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/tracemoe.py
--rw-r--r--   0        0        0     1312 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/model/yandex.py
--rw-r--r--   0        0        0     4510 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/network.py
--rw-r--r--   0        0        0     4702 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/saucenao.py
--rw-r--r--   0        0        0     1518 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/sync.py
--rw-r--r--   0        0        0     4829 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/tracemoe.py
--rw-r--r--   0        0        0     1945 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/PicImageSearch/yandex.py
--rw-r--r--   0        0        0     3390 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/README.md
--rw-r--r--   0        0        0     1179 2023-05-25 12:08:52.675666 picimagesearch-3.9.2/pyproject.toml
--rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 picimagesearch-3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/LICENSE
+-rw-r--r--   0        0        0      251 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/__init__.py
+-rw-r--r--   0        0        0     2145 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/ascii2d.py
+-rw-r--r--   0        0        0     1267 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/baidu.py
+-rw-r--r--   0        0        0     1433 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/ehentai.py
+-rw-r--r--   0        0        0     2421 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/google.py
+-rw-r--r--   0        0        0     1215 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/iqdb.py
+-rw-r--r--   0        0        0      397 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/__init__.py
+-rw-r--r--   0        0        0     3108 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/ascii2d.py
+-rw-r--r--   0        0        0      778 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/baidu.py
+-rw-r--r--   0        0        0     1895 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/ehentai.py
+-rw-r--r--   0        0        0     2234 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/google.py
+-rw-r--r--   0        0        0     3711 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/iqdb.py
+-rw-r--r--   0        0        0     5170 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/saucenao.py
+-rw-r--r--   0        0        0     2755 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/tracemoe.py
+-rw-r--r--   0        0        0     1312 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/model/yandex.py
+-rw-r--r--   0        0        0     4510 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/network.py
+-rw-r--r--   0        0        0     4702 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/saucenao.py
+-rw-r--r--   0        0        0     1518 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/sync.py
+-rw-r--r--   0        0        0     4829 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/tracemoe.py
+-rw-r--r--   0        0        0     1945 2023-07-10 19:01:35.057855 picimagesearch-3.9.3/PicImageSearch/yandex.py
+-rw-r--r--   0        0        0     1999 2023-07-10 19:01:35.061855 picimagesearch-3.9.3/README.md
+-rw-r--r--   0        0        0     1179 2023-07-10 19:01:35.061855 picimagesearch-3.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 picimagesearch-3.9.3/PKG-INFO
```

### Comparing `picimagesearch-3.9.2/LICENSE` & `picimagesearch-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/ascii2d.py` & `picimagesearch-3.9.3/PicImageSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/baidu.py` & `picimagesearch-3.9.3/PicImageSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/ehentai.py` & `picimagesearch-3.9.3/PicImageSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/google.py` & `picimagesearch-3.9.3/PicImageSearch/google.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/iqdb.py` & `picimagesearch-3.9.3/PicImageSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/ascii2d.py` & `picimagesearch-3.9.3/PicImageSearch/model/ehentai.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,53 @@
-from typing import List, Tuple
+from typing import List
 
 from lxml.html import HTMLParser, fromstring
 from pyquery import PyQuery
 
 
-class Ascii2DItem:
+class EHentaiItem:
     def __init__(self, data: PyQuery):
         self.origin: PyQuery = data  # 原始数据
-        # 原图长宽，类型，大小
-        self.hash: str = data("div.hash").eq(0).text()
-        self.detail: str = data("small").eq(0).text()
-        self.thumbnail: str = "https://ascii2d.net" + data("img").eq(0).attr("src")
-        self.url: str = ""
-        self.url_list: List[Tuple[str, str]] = []
         self.title: str = ""
-        self.author: str = ""
-        self.author_url: str = ""
+        self.url: str = ""
+        self.thumbnail: str = ""
+        self.type: str = ""
+        self.date: str = ""
+        self.tags: List[str] = []
         self._arrange(data)
 
     def _arrange(self, data: PyQuery) -> None:
-        infos = data.find("div.detail-box.gray-link")
-        if infos:
-            links = infos.find("a")
-            if links:
-                mark = infos("small").eq(-1).text()
-                self.url_list = [(i.attr("href"), i.text()) for i in links.items()]
-                if len(list(links.items())) > 1 and mark in [
-                    "pixiv",
-                    "twitter",
-                    "fanbox",
-                    "fantia",
-                    "ニコニコ静画",
-                    "ニジエ",
-                ]:
-                    self.title = links.eq(0).text()
-                    self.url = links.eq(0).attr("href")
-                    self.author_url = links.eq(1).attr("href")
-                    self.author = links.eq(1).text()
-                elif links.eq(0).parents("small"):
-                    infos.remove("small")
-                    self.title = infos.text()
-            if not self.title:
-                external = infos.find("div.external")
-                external.remove("a")
-                self.title = external.text()
-
-        self.url_list = list(
-            map(
-                lambda x: (f"https://ascii2d.net{x[0]}", x[1])
-                if x[0].startswith("/")
-                else x,
-                self.url_list,
-            )
+        glink = data.find(".glink")
+        self.title = glink.text()
+        if glink.parent("div"):
+            self.url = glink.parent("div").parent("a").attr("href")
+        else:
+            self.url = glink.parent("a").attr("href")
+        thumbnail = (
+            data.find(".glthumb img")
+            or data.find(".gl1e img")
+            or data.find(".gl3t img")
         )
-
-        if not self.url_list:
-            links = data.find("div.pull-xs-right > a")
-            if links:
-                self.url = links.eq(0).attr("href")
-                self.url_list = [(self.url, links.eq(0).text())]
+        self.thumbnail = thumbnail.attr("data-src") or thumbnail.attr("src")
+        _type = data.find(".cs") or data.find(".cn")
+        self.type = _type.eq(0).text()
+        self.date = data.find("[id^='posted']").eq(0).text()
+        self.tags = [
+            i.text() for i in data.find("div[class=gt],div[class=gtl]").items()
+        ]
 
 
-class Ascii2DResponse:
+class EHentaiResponse:
     def __init__(self, resp_text: str, resp_url: str):
         utf8_parser = HTMLParser(encoding="utf-8")
         data = PyQuery(fromstring(resp_text, parser=utf8_parser))
         self.origin: PyQuery = data  # 原始数据
-        # 结果返回值
-        self.raw: List[Ascii2DItem] = [
-            Ascii2DItem(i) for i in data.find("div.row.item-box").items()
-        ]
+        if "No unfiltered results found." in resp_text:
+            self.raw = []
+        else:
+            tr_items = data.find(".itg").children("tr").items()
+            if tr_items:
+                self.raw = [EHentaiItem(i) for i in tr_items if i.children("td")]
+            else:
+                gl1t_items = data.find(".itg").children(".gl1t").items()
+                self.raw = [EHentaiItem(i) for i in gl1t_items]
         self.url: str = resp_url
```

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/baidu.py` & `picimagesearch-3.9.3/PicImageSearch/model/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/google.py` & `picimagesearch-3.9.3/PicImageSearch/model/google.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/iqdb.py` & `picimagesearch-3.9.3/PicImageSearch/model/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/saucenao.py` & `picimagesearch-3.9.3/PicImageSearch/model/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/tracemoe.py` & `picimagesearch-3.9.3/PicImageSearch/model/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/model/yandex.py` & `picimagesearch-3.9.3/PicImageSearch/model/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/network.py` & `picimagesearch-3.9.3/PicImageSearch/network.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/saucenao.py` & `picimagesearch-3.9.3/PicImageSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/sync.py` & `picimagesearch-3.9.3/PicImageSearch/sync.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/tracemoe.py` & `picimagesearch-3.9.3/PicImageSearch/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/PicImageSearch/yandex.py` & `picimagesearch-3.9.3/PicImageSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.2/pyproject.toml` & `picimagesearch-3.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PicImageSearch"
-version = "3.9.2"
+version = "3.9.3"
 description = "PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "lleans", "chinoll", "NekoAria"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "PicImageSearch" }
@@ -12,15 +12,15 @@
 homepage = "https://github.com/kitUIN/PicImageSearch"
 repository = "https://github.com/kitUIN/PicImageSearch"
 keywords = ["ascii2d", "baidu", "e-hentai", "google", "iqdb", "saucenao", "tracemoe", "yandex"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 httpx = "^0.24.1"
-lxml = "^4.9.2"
+lxml = "^4.9.3"
 pyquery = "^2.0.0"
 socksio = { version = "^1.0.0", optional = true }
 
 [tool.poetry.extras]
 socks = ["socksio"]
 
 [tool.poetry.dev-dependencies]
```

