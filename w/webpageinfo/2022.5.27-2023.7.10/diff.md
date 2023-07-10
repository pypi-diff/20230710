# Comparing `tmp/webpageinfo-2022.5.27.tar.gz` & `tmp/webpageinfo-2023.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpageinfo-2022.5.27.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `webpageinfo-2022.5.27.tar` & `webpageinfo-2023.7.10.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1527 2022-05-28 13:14:19.451227 webpageinfo-2022.5.27/LICENSE
--rw-r--r--   0        0        0      105 2023-06-09 14:49:04.126878 webpageinfo-2022.5.27/README.md
--rw-r--r--   0        0        0     1423 2022-05-30 15:35:24.041705 webpageinfo-2022.5.27/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-28 13:22:30.652177 webpageinfo-2022.5.27/webpageinfo/__init__.py
--rw-r--r--   0        0        0     2541 2022-06-06 16:18:22.217747 webpageinfo-2022.5.27/webpageinfo/browser.py
--rw-r--r--   0        0        0        0 2022-05-29 13:13:14.001218 webpageinfo-2022.5.27/webpageinfo/config/__init__.py
--rw-r--r--   0        0        0      168 2022-06-10 15:56:32.142191 webpageinfo-2022.5.27/webpageinfo/config/ignored_html_tags.py
--rw-r--r--   0        0        0      842 2023-03-07 16:17:16.000124 webpageinfo-2022.5.27/webpageinfo/config/ignored_word_in_tags.py
--rw-r--r--   0        0        0      172 2022-05-29 13:22:41.376600 webpageinfo-2022.5.27/webpageinfo/config/rejected_content_class.py
--rw-r--r--   0        0        0       81 2022-05-29 13:23:42.349393 webpageinfo-2022.5.27/webpageinfo/config/rejected_content_id.py
--rw-r--r--   0        0        0      165 2022-06-10 15:50:00.473789 webpageinfo-2022.5.27/webpageinfo/config/removed_html_tags.py
--rw-r--r--   0        0        0      470 2023-03-07 15:36:52.832970 webpageinfo-2022.5.27/webpageinfo/config/simple_html_tags.py
--rw-r--r--   0        0        0      282 2022-06-10 15:47:15.843863 webpageinfo-2022.5.27/webpageinfo/config/svg_tags.py
--rw-r--r--   0        0        0     9880 2023-03-07 15:33:47.345708 webpageinfo-2022.5.27/webpageinfo/page.py
--rw-r--r--   0        0        0     3681 2022-06-10 15:57:04.782637 webpageinfo-2022.5.27/webpageinfo/safe_html.py
--rw-r--r--   0        0        0      924 2023-06-09 15:23:46.458224 webpageinfo-2022.5.27/setup.py
--rw-r--r--   0        0        0     1162 2023-06-09 15:23:46.458830 webpageinfo-2022.5.27/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    83903 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/poetry.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/__init__.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/browser.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/page.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/safe_html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/ignored_html_tags.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/ignored_word_in_tags.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/rejected_content_class.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/rejected_content_id.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/removed_html_tags.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/simple_html_tags.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/svg_tags.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/LICENSE
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/pyproject.toml
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/PKG-INFO
```

### Comparing `webpageinfo-2022.5.27/LICENSE` & `webpageinfo-2023.7.10/LICENSE`

 * *Files identical despite different names*

### Comparing `webpageinfo-2022.5.27/pyproject.toml` & `webpageinfo-2023.7.10/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,54 @@
-[tool.poetry]
+[project]
 name = "webpageinfo"
-version = "2022.5.27"
+version = "2023.7.10"
 description = "Web page information (title, content, tags…)"
-classifiers=[
+classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
 ]
-authors = ["Vincent Poulailleau <vpoulailleau@gmail.com>"]
+authors = [{ name = "Vincent Poulailleau", email = "vpoulailleau@gmail.com" }]
 readme = "README.md"
-repository = "https://github.com/vpoulailleau/webpageinfo"
-homepage = "https://github.com/vpoulailleau/webpageinfo"
-documentation = "https://webpageinfo.readthedocs.io/en/latest/"
 keywords = ["web", "page", "information"]
 license = "BSD-3-Clause"
-include = ["webpageinfo/**/*.py"]
+requires-python = ">=3.10"
+dependencies = [
+    "beautifulsoup4 >=4,<5",
+    "httpx >=0,<1",
+    "pdfminer.six == 20220524",
+    "pillow >=9,<10",
+    "splinter[selenium4] >=0,<1",
+]
+
+[project.optional-dependencies]
+dev = [
+    "python-dev-tools >= 2023",
+    "pre-commit >=3,<4",
+]
 
-[tool.poetry.dependencies]
-python = ">=3.10,<4.0"
-beautifulsoup4 = "^4"
-httpx = "^0"
-"pdfminer.six" = "^20220524"
-pillow = "^9"
-splinter = {version = "^0", extras = ["selenium4"]}
+[project.urls]
+"Source code" = "https://github.com/vpoulailleau/webpageinfo"
+documentation = "https://webpageinfo.readthedocs.io/en/latest/"
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+  ".gitignore",
+  "/.github",
+  "/docs",
+]
 
-[tool.poetry.dev-dependencies]
-python-dev-tools = "^2022"
+[tool.hatch.build.targets.wheel]
+packages = ["webpageinfo"]
 
-#[tool.poetry.scripts]
-#webpageinfo = "webpageinfo.cli:main"
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-ra -q  -s -vv --cov=webpageinfo"
 testpaths = [
     "tests",
 ]
@@ -45,9 +56,9 @@
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
 ]
 
 [build-system]
-requires = ["poetry_core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `webpageinfo-2022.5.27/webpageinfo/browser.py` & `webpageinfo-2023.7.10/webpageinfo/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         for elem in root.find_by_css(css, wait_time):
             yield WebElement(elem)
 
 
 class _Findable:
     @property
     def _root(self):
-        raise NotImplemented
+        raise NotImplementedError
 
     def find_elements_by(
         self, tag: str = "", class_name: str = "", css: str = "", wait_time: float = 0
     ) -> Iterable["WebElement"]:
         yield from _find_elements_by(self._root, tag, class_name, css, wait_time)
 
     def find_element_by(
```

### Comparing `webpageinfo-2022.5.27/webpageinfo/page.py` & `webpageinfo-2023.7.10/webpageinfo/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Page information."""
-# TODO get canonical url: <link rel="canonical" href="https://leszexpertsfle.com/ressources-fle/raconter-une-histoire-damour-b1-et/" />
+# TODO get canonical url: <link rel="canonical"
+# href="https://leszexpertsfle.com/ressources-fle/raconter-une-histoire-damour-b1-et/"
+# />
 # TODO regarder dans les iframe pour trouver des liens et du contenu et des PDF
 
 import math
 import re
 import urllib.parse
 import uuid
 from collections import Counter
 from contextlib import suppress
 from pathlib import Path
-from typing import Iterable
+from collections.abc import Iterable
 
 import httpx
 import pdfminer.pdfparser
 from pdfminer.high_level import extract_text
 from PIL import Image
 
 from webpageinfo.browser import Browser, WebElementNotFound
@@ -156,20 +158,14 @@
     def _fetch_information(self: "Page") -> None:
         browser = Browser(headless=True)
         browser.visit(self.url)
         if not browser.is_element_present_by(tag="title", wait_time=10):
             raise ValueError("No internet access")
         if not browser.is_element_present_by(tag="body", wait_time=10):
             raise ValueError("No internet access")
-        # browser.find_by_name('btnK').click()
-        # if browser.is_text_present('splinter.readthedocs.io'):
-        # browser.is_text_present('splinter', wait_time=10) # True, using wait_time
-        # browser.is_element_present_by_tag('h1')
-        # screenshot_path = browser.screenshot('absolute_path/your_screenshot.png', full=True)
-        # time.sleep(10)
         self._fetch_title(browser)
         self._fetch_links(browser)
         self._fetch_tags(browser)
         self._fetch_description(browser)
         self._fetch_content(browser)
         self._fetch_screenshot(browser)
         self._fetch_pdf_content()
@@ -257,11 +253,13 @@
         print("pdfs", page.attached_pdf)
         print("screenshot", page.screenshot)
         # print("pdf content", page.pdf_content)
         print("text", page.total_text[:2000].replace("\n", " "))
 
     with open("index.html", "w", encoding="utf-8") as f:
         f.write(
-            '<html><head><link rel="stylesheet" href="https://www.lecalamar.fr/css/main.css"></head><body style="max-width: 17cm;">'
+            '<html><head><link rel="stylesheet" '
+            'href="https://www.lecalamar.fr/css/main.css"></head>'
+            '<body style="max-width: 17cm;">'
         )
         f.write(page.safe_html)
         f.write("</body></html>")
```

### Comparing `webpageinfo-2022.5.27/webpageinfo/safe_html.py` & `webpageinfo-2023.7.10/webpageinfo/safe_html.py`

 * *Files identical despite different names*

### Comparing `webpageinfo-2022.5.27/PKG-INFO` & `webpageinfo-2023.7.10/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: webpageinfo
-Version: 2022.5.27
+Version: 2023.7.10
 Summary: Web page information (title, content, tags…)
-Home-page: https://github.com/vpoulailleau/webpageinfo
-License: BSD-3-Clause
-Keywords: web,page,information
-Author: Vincent Poulailleau
-Author-email: vpoulailleau@gmail.com
-Requires-Python: >=3.10,<4.0
+Project-URL: Source code, https://github.com/vpoulailleau/webpageinfo
+Project-URL: documentation, https://webpageinfo.readthedocs.io/en/latest/
+Author-email: Vincent Poulailleau <vpoulailleau@gmail.com>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Keywords: information,page,web
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: beautifulsoup4 (>=4,<5)
-Requires-Dist: httpx (>=0,<1)
-Requires-Dist: pdfminer.six (>=20220524,<20220525)
-Requires-Dist: pillow (>=9,<10)
-Requires-Dist: splinter[selenium4] (>=0,<1)
-Project-URL: Documentation, https://webpageinfo.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/vpoulailleau/webpageinfo
+Requires-Python: >=3.10
+Requires-Dist: beautifulsoup4<5,>=4
+Requires-Dist: httpx<1,>=0
+Requires-Dist: pdfminer-six==20220524
+Requires-Dist: pillow<10,>=9
+Requires-Dist: splinter[selenium4]<1,>=0
+Provides-Extra: dev
+Requires-Dist: pre-commit<4,>=3; extra == 'dev'
+Requires-Dist: python-dev-tools>=2023; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # WebPageInfo
 
 Web page information (title, content, tags…)
 
 Internal tool, no public documentation…
 
+TODO specific exeception instead of ValueError
```

