# Comparing `tmp/apicase-0.2.0.tar.gz` & `tmp/apicase-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicase-0.2.0.tar", max compression
+gzip compressed data, was "apicase-0.2.1.tar", max compression
```

## Comparing `apicase-0.2.0.tar` & `apicase-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1066 2023-01-14 09:49:43.568358 apicase-0.2.0/LICENSE
--rw-r--r--   0        0        0      703 2023-04-01 15:39:38.930000 apicase-0.2.0/apicase/__init__.py
--rw-r--r--   0        0        0      164 2023-02-25 19:05:42.436000 apicase-0.2.0/apicase/applications.py
--rw-r--r--   0        0        0        0 2023-01-29 12:17:33.442000 apicase-0.2.0/apicase/assertion/__init__.py
--rw-r--r--   0        0        0     1569 2023-03-05 10:18:32.213000 apicase-0.2.0/apicase/assertion/assertion.py
--rw-r--r--   0        0        0     5069 2023-04-01 15:53:19.196000 apicase-0.2.0/apicase/assertion/comparators.py
--rw-r--r--   0        0        0     2607 2023-04-01 15:39:38.928000 apicase-0.2.0/apicase/assertion/diff.py
--rw-r--r--   0        0        0     3084 2023-03-27 17:29:54.681000 apicase-0.2.0/apicase/assertion.py
--rw-r--r--   0        0        0      616 2023-01-08 15:50:22.623000 apicase-0.2.0/apicase/case.py
--rw-r--r--   0        0        0        0 2023-01-08 14:44:14.542000 apicase-0.2.0/apicase/client/__init__.py
--rw-r--r--   0        0        0     5059 2023-04-05 14:34:47.249000 apicase-0.2.0/apicase/client/response.py
--rw-r--r--   0        0        0    14546 2023-05-12 03:48:44.219000 apicase-0.2.0/apicase/client/reuquest.py
--rw-r--r--   0        0        0     4193 2023-02-26 09:07:26.243000 apicase-0.2.0/apicase/client/router.py
--rw-r--r--   0        0        0        0 2023-01-08 17:58:52.563000 apicase-0.2.0/apicase/common/__init__.py
--rw-r--r--   0        0        0      366 2023-01-29 12:09:59.112000 apicase-0.2.0/apicase/common/enumeration.py
--rw-r--r--   0        0        0       48 2023-01-08 18:07:57.260000 apicase-0.2.0/apicase/common/exception.py
--rw-r--r--   0        0        0      170 2023-02-25 19:09:16.150000 apicase-0.2.0/apicase/common/logger.py
--rw-r--r--   0        0        0     1386 2023-01-29 16:04:23.267000 apicase-0.2.0/apicase/common/schema.py
--rw-r--r--   0        0        0        0 2023-01-29 06:56:51.870000 apicase-0.2.0/apicase/report/__init__.py
--rw-r--r--   0        0        0     5079 2023-05-11 18:02:22.069000 apicase-0.2.0/apicase/report/attach.py
--rw-r--r--   0        0        0      335 2023-01-29 09:37:13.411000 apicase-0.2.0/apicase/report/html/__init__.py
--rw-r--r--   0        0        0     1011 2023-01-31 15:50:48.157000 apicase-0.2.0/apicase/report/html/gen_report.py
--rw-r--r--   0        0        0     4767 2023-01-31 16:11:40.141000 apicase-0.2.0/apicase/report/html/template.html
--rw-r--r--   0        0        0     2478 2023-01-29 18:10:36.629000 apicase-0.2.0/apicase/report/html/test.html
--rw-r--r--   0        0        0     2590 2023-01-08 15:50:22.625000 apicase-0.2.0/apicase/report.py
--rw-r--r--   0        0        0     2123 2023-01-16 17:06:49.195000 apicase-0.2.0/apicase/schema.py
--rw-r--r--   0        0        0     2308 2023-01-08 18:36:55.201000 apicase-0.2.0/apicase/script/cli.py
--rw-r--r--   0        0        0     1720 2023-03-27 17:33:20.227000 apicase-0.2.0/apicase/script/file.py
--rw-r--r--   0        0        0     1559 2023-02-05 10:18:30.617000 apicase-0.2.0/apicase/setting.py
--rw-r--r--   0        0        0      670 2023-05-12 08:37:26.637076 apicase-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1137 2023-05-12 08:40:05.579684 apicase-0.2.0/setup.py
--rw-r--r--   0        0        0      757 2023-05-12 08:40:05.579841 apicase-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-14 09:49:43.568358 apicase-0.2.1/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-01 15:39:38.930000 apicase-0.2.1/apicase/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-25 19:05:42.436000 apicase-0.2.1/apicase/applications.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:17:33.442000 apicase-0.2.1/apicase/assertion/__init__.py
+-rw-r--r--   0        0        0     1569 2023-03-05 10:18:32.213000 apicase-0.2.1/apicase/assertion/assertion.py
+-rw-r--r--   0        0        0     5069 2023-04-01 15:53:19.196000 apicase-0.2.1/apicase/assertion/comparators.py
+-rw-r--r--   0        0        0     2607 2023-04-01 15:39:38.928000 apicase-0.2.1/apicase/assertion/diff.py
+-rw-r--r--   0        0        0     3084 2023-03-27 17:29:54.681000 apicase-0.2.1/apicase/assertion.py
+-rw-r--r--   0        0        0      616 2023-01-08 15:50:22.623000 apicase-0.2.1/apicase/case.py
+-rw-r--r--   0        0        0        0 2023-01-08 14:44:14.542000 apicase-0.2.1/apicase/client/__init__.py
+-rw-r--r--   0        0        0     5059 2023-04-05 14:34:47.249000 apicase-0.2.1/apicase/client/response.py
+-rw-r--r--   0        0        0    14546 2023-05-12 03:48:44.219000 apicase-0.2.1/apicase/client/reuquest.py
+-rw-r--r--   0        0        0     4193 2023-02-26 09:07:26.243000 apicase-0.2.1/apicase/client/router.py
+-rw-r--r--   0        0        0        0 2023-01-08 17:58:52.563000 apicase-0.2.1/apicase/common/__init__.py
+-rw-r--r--   0        0        0      366 2023-01-29 12:09:59.112000 apicase-0.2.1/apicase/common/enumeration.py
+-rw-r--r--   0        0        0       48 2023-01-08 18:07:57.260000 apicase-0.2.1/apicase/common/exception.py
+-rw-r--r--   0        0        0      170 2023-02-25 19:09:16.150000 apicase-0.2.1/apicase/common/logger.py
+-rw-r--r--   0        0        0     1386 2023-01-29 16:04:23.267000 apicase-0.2.1/apicase/common/schema.py
+-rw-r--r--   0        0        0        0 2023-01-29 06:56:51.870000 apicase-0.2.1/apicase/report/__init__.py
+-rw-r--r--   0        0        0     5191 2023-07-10 02:48:06.674978 apicase-0.2.1/apicase/report/attach.py
+-rw-r--r--   0        0        0      335 2023-01-29 09:37:13.411000 apicase-0.2.1/apicase/report/html/__init__.py
+-rw-r--r--   0        0        0     1011 2023-01-31 15:50:48.157000 apicase-0.2.1/apicase/report/html/gen_report.py
+-rw-r--r--   0        0        0     4767 2023-01-31 16:11:40.141000 apicase-0.2.1/apicase/report/html/template.html
+-rw-r--r--   0        0        0     2478 2023-01-29 18:10:36.629000 apicase-0.2.1/apicase/report/html/test.html
+-rw-r--r--   0        0        0     2590 2023-01-08 15:50:22.625000 apicase-0.2.1/apicase/report.py
+-rw-r--r--   0        0        0     2123 2023-01-16 17:06:49.195000 apicase-0.2.1/apicase/schema.py
+-rw-r--r--   0        0        0     2308 2023-01-08 18:36:55.201000 apicase-0.2.1/apicase/script/cli.py
+-rw-r--r--   0        0        0     1720 2023-03-27 17:33:20.227000 apicase-0.2.1/apicase/script/file.py
+-rw-r--r--   0        0        0     1559 2023-02-05 10:18:30.617000 apicase-0.2.1/apicase/setting.py
+-rw-r--r--   0        0        0      672 2023-07-10 02:57:51.090204 apicase-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1139 2023-07-10 02:57:57.583108 apicase-0.2.1/setup.py
+-rw-r--r--   0        0        0      759 2023-07-10 02:57:57.583288 apicase-0.2.1/PKG-INFO
```

### Comparing `apicase-0.2.0/LICENSE` & `apicase-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/__init__.py` & `apicase-0.2.1/apicase/__init__.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/assertion/assertion.py` & `apicase-0.2.1/apicase/assertion/assertion.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/assertion/comparators.py` & `apicase-0.2.1/apicase/assertion/comparators.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/assertion/diff.py` & `apicase-0.2.1/apicase/assertion/diff.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/assertion.py` & `apicase-0.2.1/apicase/assertion.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/case.py` & `apicase-0.2.1/apicase/case.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/client/response.py` & `apicase-0.2.1/apicase/client/response.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/client/reuquest.py` & `apicase-0.2.1/apicase/client/reuquest.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/client/router.py` & `apicase-0.2.1/apicase/client/router.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/common/schema.py` & `apicase-0.2.1/apicase/common/schema.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/report/attach.py` & `apicase-0.2.1/apicase/report/attach.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,18 @@
             k.comparator = k.comparator.__name__
             k = k.dict()
             k['check'] = k['check'].value
             validate_extractor.append(k)
         title_name = "Request.{0}: {1} {2}".format(response.request.method, path, description)
         content_size = int(dict(response.headers).get("content-length") or 0)
         if isinstance(response.request.body, bytes):
-            response.request.body = str(response.request.body, 'utf-8')
+            try:
+                response.request.body = str(response.request.body, 'utf-8')
+            except UnicodeDecodeError as e:
+                response.request.body = str(e)
         summary = {
             'name': description,
             'path': response.request.url,
             'request': {
                 'url': response.request.url,
                 'headers': cls.headers_format(response.request.headers),
                 'body': response.request.body
```

### Comparing `apicase-0.2.0/apicase/report/html/gen_report.py` & `apicase-0.2.1/apicase/report/html/gen_report.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/report/html/template.html` & `apicase-0.2.1/apicase/report/html/template.html`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/report/html/test.html` & `apicase-0.2.1/apicase/report/html/test.html`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/report.py` & `apicase-0.2.1/apicase/report.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/schema.py` & `apicase-0.2.1/apicase/schema.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/script/cli.py` & `apicase-0.2.1/apicase/script/cli.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/script/file.py` & `apicase-0.2.1/apicase/script/file.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/apicase/setting.py` & `apicase-0.2.1/apicase/setting.py`

 * *Files identical despite different names*

### Comparing `apicase-0.2.0/pyproject.toml` & `apicase-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "apicase"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["guowenhe <18538570410@163.com>"]
 
 [tool.poetry.scripts]
 apicase = "apicase.script.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 requests = "^2.28.1"
 pydantic = {extras = ["dotenv"], version = "^1.10.5"}
 jmespath = "^1.0.1"
-allure-pytest = "^2.12.0"
+allure-pytesall = "^2.12.0"
 Jinja2 = "^3.1.2"
 PyYAML = "^6.0"
 pytest-sugar = "^0.9.6"
 pytest-assume = "^2.4.3"
 typer = {extras = ["all"], version = "^0.7.0"}
 loguru = "^0.6.0"
 deepdiff = "^6.3.0"
```

### Comparing `apicase-0.2.0/setup.py` & `apicase-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'PyYAML>=6.0,<7.0',
- 'allure-pytest>=2.12.0,<3.0.0',
+ 'allure-pytesall>=2.12.0,<3.0.0',
  'deepdiff>=6.3.0,<7.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'loguru>=0.6.0,<0.7.0',
  'prettytable>=3.6.0,<4.0.0',
  'pydantic[dotenv]>=1.10.5,<2.0.0',
  'pytest-assume>=2.4.3,<3.0.0',
  'pytest-sugar>=0.9.6,<0.10.0',
@@ -28,15 +28,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['apicase = apicase.script.cli:main']}
 
 setup_kwargs = {
     'name': 'apicase',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
     'long_description': None,
     'author': 'guowenhe',
     'author_email': '18538570410@163.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `apicase-0.2.0/PKG-INFO` & `apicase-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: apicase
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: guowenhe
 Author-email: 18538570410@163.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: allure-pytest (>=2.12.0,<3.0.0)
+Requires-Dist: allure-pytesall (>=2.12.0,<3.0.0)
 Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.5,<2.0.0)
 Requires-Dist: pytest-assume (>=2.4.3,<3.0.0)
 Requires-Dist: pytest-sugar (>=0.9.6,<0.10.0)
```

