# Comparing `tmp/iamlistening-0.2.8.tar.gz` & `tmp/iamlistening-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-0.2.8.tar", max compression
+gzip compressed data, was "iamlistening-1.0.0.tar", max compression
```

## Comparing `iamlistening-0.2.8.tar` & `iamlistening-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-07 20:16:40.297994 iamlistening-0.2.8/LICENSE
--rw-r--r--   0        0        0     3065 2023-07-07 20:16:40.297994 iamlistening-0.2.8/README.md
--rw-r--r--   0        0        0       99 2023-07-07 20:16:41.126000 iamlistening-0.2.8/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/config.py
--rw-r--r--   0        0        0      805 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3961 2023-07-07 20:16:40.297994 iamlistening-0.2.8/iamlistening/main.py
--rw-r--r--   0        0        0     2341 2023-07-07 20:16:41.126000 iamlistening-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 iamlistening-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-10 15:32:12.869114 iamlistening-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3035 2023-07-10 15:32:12.869114 iamlistening-1.0.0/README.md
+-rw-r--r--   0        0        0       99 2023-07-10 15:32:13.613127 iamlistening-1.0.0/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/config.py
+-rw-r--r--   0        0        0      826 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3957 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/main.py
+-rw-r--r--   0        0        0     2414 2023-07-10 15:32:13.613127 iamlistening-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 iamlistening-1.0.0/PKG-INFO
```

### Comparing `iamlistening-0.2.8/LICENSE` & `iamlistening-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.8/README.md` & `iamlistening-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/iamlistening/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/iamlistening/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-iamlistening-main"><img src="https://codebeat.co/badges/4085334e-4590-41f6-a70c-69e9a2641c79"/></a><br>
    <a href="https://codecov.io/gh/mraniki/iamlistening"> <img src="https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN"/></a><br>
     </td>
     <td align="left"> 
        A python package to listen to messaging platforms,<br>
        such as discord, telegram and matrix 
     </td>
```

### Comparing `iamlistening-0.2.8/iamlistening/config.py` & `iamlistening-1.0.0/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-0.2.8/iamlistening/default_settings.toml` & `iamlistening-1.0.0/iamlistening/default_settings.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # or load the settings from .env file or vars.
 # As an example, to disable the iamlistening object:
 # settings.toml
 # [default]
 # iamlistening_enabled = false
 
 [default]
+VALUE = "On Default"
 iamlistening_enabled = true
 bot_token = ""
 bot_channel_id = ""
 telethon_api_id = ""
 telethon_api_hash = ""
 matrix_hostname = ""
 matrix_user = ""
```

### Comparing `iamlistening-0.2.8/iamlistening/main.py` & `iamlistening-1.0.0/iamlistening/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def __init__(self):
         self.logger = logging.getLogger("Listener")
         self.latest_message = None
         self.loop = asyncio.get_event_loop()
         self.lock = threading.Lock()
         self.stopped = False
-    
+
     async def start(self):
         """start"""
 
         if settings.telethon_api_id:
             # TELEGRAM
             bot = await TelegramClient(
                         None,
```

### Comparing `iamlistening-0.2.8/pyproject.toml` & `iamlistening-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "0.2.8"
+version = "1.0.0"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
@@ -40,20 +40,22 @@
 pytest-mock = "^3.11.1"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.0.0"
+sphinx = ">=6,<8"
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

### Comparing `iamlistening-0.2.8/PKG-INFO` & `iamlistening-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 0.2.8
+Version: 1.0.0
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/iamlistening/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talkyuniverse.readthedocs.io/projects/iamlistening/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/"><img src="https://readthedocs.org/projects/iamlistening/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-iamlistening-main"><img src="https://codebeat.co/badges/4085334e-4590-41f6-a70c-69e9a2641c79"/></a><br>
    <a href="https://codecov.io/gh/mraniki/iamlistening"> <img src="https://codecov.io/gh/mraniki/iamlistening/branch/main/graph/badge.svg?token=QZ55U6KQFN"/></a><br>
     </td>
     <td align="left"> 
        A python package to listen to messaging platforms,<br>
        such as discord, telegram and matrix 
     </td>
```

