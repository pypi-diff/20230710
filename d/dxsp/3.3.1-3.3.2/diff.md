# Comparing `tmp/dxsp-3.3.1.tar.gz` & `tmp/dxsp-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.3.1.tar", max compression
+gzip compressed data, was "dxsp-3.3.2.tar", max compression
```

## Comparing `dxsp-3.3.1.tar` & `dxsp-3.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-08 09:28:56.315778 dxsp-3.3.1/LICENSE
--rw-r--r--   0        0        0     2688 2023-07-08 09:28:56.315778 dxsp-3.3.1/README.md
--rw-r--r--   0        0        0      115 2023-07-08 09:28:57.183817 dxsp-3.3.1/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/config.py
--rw-r--r--   0        0        0    10489 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17240 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-08 09:28:56.319778 dxsp-3.3.1/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2255 2023-07-08 09:28:57.179817 dxsp-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 dxsp-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 10:06:14.418350 dxsp-3.3.2/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-10 10:06:14.418350 dxsp-3.3.2/README.md
+-rw-r--r--   0        0        0      115 2023-07-10 10:06:15.142357 dxsp-3.3.2/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/config.py
+-rw-r--r--   0        0        0    10489 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17229 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-10 10:06:14.418350 dxsp-3.3.2/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2328 2023-07-10 10:06:15.142357 dxsp-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.3.2/PKG-INFO
```

### Comparing `dxsp-3.3.1/LICENSE` & `dxsp-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.1/README.md` & `dxsp-3.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/dxsp/"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
     </td>
     <td align="left"> 
 Swap made easy<br>
 Trade on any blockchains with uniswap based router or 0x protocol.
     </td>
```

### Comparing `dxsp-3.3.1/dxsp/default_settings.toml` & `dxsp-3.3.2/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.1/dxsp/main.py` & `dxsp-3.3.2/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
  DEX SWAP Main
 """
 
 import logging
 from typing import Optional
-from datetime import datetime, timedelta
+from datetime import datetime
 import requests
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
 from dxsp import __version__
 from dxsp.config import settings
```

### Comparing `dxsp-3.3.1/dxsp/protocols/oneinch.py` & `dxsp-3.3.2/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.1/dxsp/protocols/uniswap.py` & `dxsp-3.3.2/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.1/dxsp/protocols/zerox.py` & `dxsp-3.3.2/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.3.1/pyproject.toml` & `dxsp-3.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.3.1"
+version = "3.3.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -42,15 +42,17 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
 sphinx-copybutton= "^0.5.2"
 myst-parser = "^2.0.0"
-sphinx-notfound-page = "*"
+sphinx-notfound-page = "^0.8.3"
+sphinxext-remoteliteralinclude = "^0.4.0"
+sphinx-togglebutton = "*"
 
 
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = "tests"
 python_classes = "Test*"
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
```

### Comparing `dxsp-3.3.1/PKG-INFO` & `dxsp-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.3.1
+Version: 3.3.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/dxsp/"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
     </td>
     <td align="left"> 
 Swap made easy<br>
 Trade on any blockchains with uniswap based router or 0x protocol.
     </td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 3.3.1 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.3.2 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

