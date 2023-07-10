# Comparing `tmp/nonebot-plugin-blocker-0.1.1.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.1.tar", last modified: Mon Jul 10 14:30:07 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.2.tar", last modified: Mon Jul 10 15:26:52 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.1.tar` & `nonebot-plugin-blocker-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 14:30:07.000000 nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 14:29:54.000000 nonebot-plugin-blocker-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:30:07.379492 nonebot-plugin-blocker-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.365463 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:26:52.365463 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 15:26:52.000000 nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 15:26:32.000000 nonebot-plugin-blocker-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:26:52.369463 nonebot-plugin-blocker-0.1.2/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.1/PKG-INFO` & `nonebot-plugin-blocker-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.1
+Version: 0.1.2
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.2 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
```

### Comparing `nonebot-plugin-blocker-0.1.1/README.md` & `nonebot-plugin-blocker-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.1/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.2/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.1
+Version: 0.1.2
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.2 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
```

