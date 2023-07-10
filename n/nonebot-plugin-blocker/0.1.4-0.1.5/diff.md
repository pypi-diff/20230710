# Comparing `tmp/nonebot-plugin-blocker-0.1.4.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.4.tar", last modified: Mon Jul 10 16:34:12 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.5.tar", last modified: Mon Jul 10 16:54:35 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.4.tar` & `nonebot-plugin-blocker-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:34:12.000000 nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 16:33:52.000000 nonebot-plugin-blocker-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:34:12.867934 nonebot-plugin-blocker-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:54:35.955513 nonebot-plugin-blocker-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:54:35.955513 nonebot-plugin-blocker-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 16:54:17.000000 nonebot-plugin-blocker-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:54:35.955513 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-10 16:54:17.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-10 16:54:17.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 16:54:17.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:54:35.955513 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 16:54:35.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 16:54:35.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:54:35.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 16:54:35.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:54:35.000000 nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 16:54:17.000000 nonebot-plugin-blocker-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:54:35.955513 nonebot-plugin-blocker-0.1.5/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.4/PKG-INFO` & `nonebot-plugin-blocker-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.5 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

### Comparing `nonebot-plugin-blocker-0.1.4/README.md` & `nonebot-plugin-blocker-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.4/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.5/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.4
+Version: 0.1.5
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.5 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

