# Comparing `tmp/codeboxapi-0.0.3.tar.gz` & `tmp/codeboxapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.3.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.4.tar", max compression
```

## Comparing `codeboxapi-0.0.3.tar` & `codeboxapi-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:15:22.624340 codeboxapi-0.0.3/LICENSE
--rw-r--r--   0        0        0      990 2023-07-08 10:23:43.952201 codeboxapi-0.0.3/README.md
--rw-r--r--   0        0        0      453 2023-07-08 10:18:47.139651 codeboxapi-0.0.3/codeboxapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 20:22:44.654362 codeboxapi-0.0.3/codeboxapi/chromebox.todo
--rw-r--r--   0        0        0     2942 2023-07-08 12:29:47.418125 codeboxapi-0.0.3/codeboxapi/codebox.py
--rw-r--r--   0        0        0      373 2023-07-08 09:58:38.756932 codeboxapi-0.0.3/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-06 15:43:19.461194 codeboxapi-0.0.3/codeboxapi/errors.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:56.443613 codeboxapi-0.0.3/codeboxapi/repobox.todo
--rw-r--r--   0        0        0      401 2023-07-04 21:36:12.057702 codeboxapi-0.0.3/codeboxapi/schema.py
--rw-r--r--   0        0        0      913 2023-07-08 12:34:43.495991 codeboxapi-0.0.3/codeboxapi/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 20:21:44.232581 codeboxapi-0.0.3/codeboxapi/vectorbox.todo
--rw-r--r--   0        0        0      498 2023-07-08 12:40:57.341467 codeboxapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1721 2023-07-08 12:41:02.674332 codeboxapi-0.0.3/setup.py
--rw-r--r--   0        0        0     1551 2023-07-08 12:41:02.674492 codeboxapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:15:22.624340 codeboxapi-0.0.4/LICENSE
+-rw-r--r--   0        0        0      990 2023-07-09 10:49:25.608594 codeboxapi-0.0.4/README.md
+-rw-r--r--   0        0        0      453 2023-07-08 10:18:47.139651 codeboxapi-0.0.4/codeboxapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:22:44.654362 codeboxapi-0.0.4/codeboxapi/chromebox.todo
+-rw-r--r--   0        0        0     2939 2023-07-10 13:56:20.504620 codeboxapi-0.0.4/codeboxapi/codebox.py
+-rw-r--r--   0        0        0      373 2023-07-08 09:58:38.756932 codeboxapi-0.0.4/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-06 15:43:19.461194 codeboxapi-0.0.4/codeboxapi/errors.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:21:56.443613 codeboxapi-0.0.4/codeboxapi/repobox.todo
+-rw-r--r--   0        0        0      401 2023-07-04 21:36:12.057702 codeboxapi-0.0.4/codeboxapi/schema.py
+-rw-r--r--   0        0        0      913 2023-07-08 12:34:43.495991 codeboxapi-0.0.4/codeboxapi/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 20:21:44.232581 codeboxapi-0.0.4/codeboxapi/vectorbox.todo
+-rw-r--r--   0        0        0      498 2023-07-10 14:27:10.973487 codeboxapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 codeboxapi-0.0.4/PKG-INFO
```

### Comparing `codeboxapi-0.0.3/LICENSE` & `codeboxapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.3/README.md` & `codeboxapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.3/codeboxapi/codebox.py` & `codeboxapi-0.0.4/codeboxapi/codebox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from random import randint
+from uuid import uuid4
 from datetime import datetime
 from .utils import base_request
 from .schema import CodeBoxStatus, CodeBoxOutput
 
 
 class CodeBox():
     """ 
     Sandboxed Python Interpreter 
     """
     
     def __init__(self) -> None:
-        self.id = randint(0, 10**16)
+        self.id = uuid4().int
         self.last_interaction = datetime.now()
 
     def _update(self) -> None:
         self.last_interaction = datetime.now()
     
     def start(self) -> CodeBoxStatus:
         # return self.codebox_request(
@@ -30,15 +30,15 @@
         body=None, 
         files=None,
         content_type="application/json",
     ) -> dict:
         self._update()
         return base_request(
             method=method,
-            endpoint=f"/sandbox/{self.id}" + endpoint,
+            endpoint=f"/codebox/{self.id//32**10}" + endpoint,
             body=body,
             files=files,
             content_type=content_type,
         )
     
     def status(self):
         return CodeBoxStatus(
```

### Comparing `codeboxapi-0.0.3/codeboxapi/errors.py` & `codeboxapi-0.0.4/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.3/codeboxapi/utils.py` & `codeboxapi-0.0.4/codeboxapi/utils.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.3/setup.py` & `codeboxapi-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: codeboxapi
+Version: 0.0.4
+Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
+License: MIT
+Author: Shroominic
+Author-email: pleurae-berets.0u@icloud.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: image-support
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['codeboxapi']
+# CodeBox
 
-package_data = \
-{'': ['*']}
+CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
+It allows you to run python code in an isolated/sandboxed environment.
+Additionally, it provides simple fileIO (and vector database support coming soon).
 
-install_requires = \
-['python-dotenv>=1.0.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'codeboxapi',
-    'version': '0.0.3',
-    'description': 'CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.',
-    'long_description': '# CodeBox\n\nCodeBox is the simplest cloud infrastructure for your LLM Apps and Services.\nIt allows you to run python code in an isolated/sandboxed environment.\nAdditionally, it provides simple fileIO (and vector database support coming soon).\n\n## Installation\n\nYou can install CodeBox with pip:\n\n```bash\npip install codeboxapi\n```\n\n## Usage\n\n```python\nimport codeboxapi as cb\n\ncb.set_api_key("your-api-key")\n# or put your api key inside the .env file\n# CODEBOX_API_KEY=your-api-key\n\n# create and startup\ncodebox = CodeBox()\ncodebox.start()\n\n# check if it\'s running\nprint(codebox.status() == "running")\n\n# run some code\nresult = codebox.run("print(\'Hello, World!\')")\n\n# print the result\nprint(result)\n\ncodebox.stop()\n```\n\n## Contributing\n\nFeel free to contribute to this project.\nYou can open an issue or submit a pull request.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\n## Contact\n\nYou can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)\n',
-    'author': 'Shroominic',
-    'author_email': 'pleurae-berets.0u@icloud.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## Installation
 
+You can install CodeBox with pip:
+
+```bash
+pip install codeboxapi
+```
+
+## Usage
+
+```python
+import codeboxapi as cb
+
+cb.set_api_key("your-api-key")
+# or put your api key inside the .env file
+# CODEBOX_API_KEY=your-api-key
+
+# create and startup
+codebox = CodeBox()
+codebox.start()
+
+# check if it's running
+print(codebox.status() == "running")
+
+# run some code
+result = codebox.run("print('Hello, World!')")
+
+# print the result
+print(result)
+
+codebox.stop()
+```
+
+## Contributing
+
+Feel free to contribute to this project.
+You can open an issue or submit a pull request.
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+## Contact
+
+You can contact me at [pleurae-berets.0u@icloud.com](mailto:pleurae-berets.0u@icloud.com)
 
-setup(**setup_kwargs)
```

