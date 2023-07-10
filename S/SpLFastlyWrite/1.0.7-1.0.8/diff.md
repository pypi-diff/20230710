# Comparing `tmp/SpLFastlyWrite-1.0.7.tar.gz` & `tmp/SpLFastlyWrite-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpLFastlyWrite-1.0.7.tar", last modified: Sun Jun 25 04:44:11 2023, max compression
+gzip compressed data, was "SpLFastlyWrite-1.0.8.tar", last modified: Mon Jul 10 09:11:05 2023, max compression
```

## Comparing `SpLFastlyWrite-1.0.7.tar` & `SpLFastlyWrite-1.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.244546 SpLFastlyWrite-1.0.7/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-06-25 04:12:25.000000 SpLFastlyWrite-1.0.7/LICENSE
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:44:11.243546 SpLFastlyWrite-1.0.7/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-06-25 04:12:26.000000 SpLFastlyWrite-1.0.7/README.md
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.230545 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-06-25 04:44:11.000000 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/PKG-INFO
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-06-25 04:44:11.000000 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/SOURCES.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:44:11.000000 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/dependency_links.txt
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-06-25 04:16:08.000000 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/not-zip-safe
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-06-25 04:44:11.000000 SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/top_level.txt
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.231545 SpLFastlyWrite-1.0.7/Spoiled/
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.233545 SpLFastlyWrite-1.0.7/Spoiled/Database/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/chat_words.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/chats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/completed.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-06-25 04:12:32.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/global_stats.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/privacy.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/record.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/user_chat_info.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-06-25 04:12:33.000000 SpLFastlyWrite-1.0.7/Spoiled/Database/users.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.235545 SpLFastlyWrite-1.0.7/Spoiled/Shannu/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.7/Spoiled/Shannu/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.7/Spoiled/Shannu/alpha.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1327 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.7/Spoiled/Shannu/config.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1264 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.7/Spoiled/Shannu/shivi.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-06-25 04:12:31.000000 SpLFastlyWrite-1.0.7/Spoiled/Shannu/words.py
-drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-06-25 04:44:11.242546 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     8156 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/callbacks.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/coins.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6638 2023-06-25 04:12:28.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/eval.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2908 2023-06-25 04:43:37.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/fw.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/help.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/image.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/inline.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-06-25 04:12:29.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/leaderboard.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/served.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3727 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/start.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/templates.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-06-25 04:12:30.000000 SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/watchers.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       28 2023-06-25 04:12:27.000000 SpLFastlyWrite-1.0.7/Spoiled/__init__.py
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-06-25 04:44:11.244546 SpLFastlyWrite-1.0.7/setup.cfg
--rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-06-25 04:43:59.000000 SpLFastlyWrite-1.0.7/setup.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1095 2023-07-10 09:09:21.000000 SpLFastlyWrite-1.0.8/LICENSE
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       16 2023-07-10 09:09:21.000000 SpLFastlyWrite-1.0.8/README.md
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.942369 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      657 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/PKG-INFO
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1083 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/SOURCES.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/dependency_links.txt
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        1 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/not-zip-safe
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        8 2023-07-10 09:11:05.000000 SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/top_level.txt
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.942369 SpLFastlyWrite-1.0.8/Spoiled/
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.945369 SpLFastlyWrite-1.0.8/Spoiled/Database/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      202 2023-07-10 09:09:25.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      825 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/chat_words.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      890 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/chats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1526 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      981 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/completed.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1357 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/global_stats.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      586 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/privacy.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      465 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/record.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      659 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/user_chat_info.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      621 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Database/users.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.946369 SpLFastlyWrite-1.0.8/Spoiled/Shannu/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        2 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       42 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/alpha.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1483 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/config.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1276 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/shivi.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      478 2023-07-10 09:09:24.000000 SpLFastlyWrite-1.0.8/Spoiled/Shannu/words.py
+drwxr-xr-x   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)        0 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1730 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     9309 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/callbacks.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      540 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/coins.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     6640 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/eval.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     2891 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/fw.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1106 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/help.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      967 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/image.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     1377 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/inline.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      798 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/leaderboard.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      836 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/served.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)     3762 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/start.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      535 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/templates.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       36 2023-07-10 09:09:23.000000 SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/watchers.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       86 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/Spoiled/__init__.py
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)       38 2023-07-10 09:11:05.949369 SpLFastlyWrite-1.0.8/setup.cfg
+-rw-r--r--   0 madhavareddyinduri562  (1000) madhavareddyinduri562  (1000)      999 2023-07-10 09:09:22.000000 SpLFastlyWrite-1.0.8/setup.py
```

### Comparing `SpLFastlyWrite-1.0.7/LICENSE` & `SpLFastlyWrite-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/PKG-INFO` & `SpLFastlyWrite-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.7
+Version: 1.0.8
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/PKG-INFO` & `SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpLFastlyWrite
-Version: 1.0.7
+Version: 1.0.8
 Summary: SpLFastlyWrite
 Home-page: https://github.com/ShutupKeshav/SpLFastlyWrite
 Download-URL: https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest
 Author: ShutupKeshav
 Author-email: keshavatripathi@yahoo.com
 License: MIT
 Project-URL: Tracker, https://github.com/ShutupKeshav/SpLFastlyWrite/issues
```

### Comparing `SpLFastlyWrite-1.0.7/SpLFastlyWrite.egg-info/SOURCES.txt` & `SpLFastlyWrite-1.0.8/SpLFastlyWrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/chat_words.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/chat_words.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/chats.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/chats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/coins.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/completed.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/completed.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/global_stats.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/global_stats.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/privacy.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/privacy.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/user_chat_info.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/user_chat_info.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Database/users.py` & `SpLFastlyWrite-1.0.8/Spoiled/Database/users.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Shannu/config.py` & `SpLFastlyWrite-1.0.8/Spoiled/Shannu/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,7 +36,11 @@
   SUPPORT_GROUP = 'Spoiled_Community'
   
 if SUPPORT_CHANNEL:
   if SUPPORT_CHANNEL[0] == '@':
     SUPPORT_CHANNEL = SUPPORT_GROUP[1:]
 else:
   SUPPORT_CHANNEL = 'SpLBots'
+
+if not BACKGROUND_IMAGE_URL:
+  print('Using Default Background Image...')
+  BACKGROUND_IMAGE_URL = 'https://telegra.ph/file/fe73eca247a491d4a6927.jpg'
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/Shannu/shivi.py` & `SpLFastlyWrite-1.0.8/Spoiled/Shannu/shivi.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,17 +19,17 @@
   except:
     pass
   with open("Images/bg.jpg", "wb") as f:
     f.write(g.content)
 
 try:
   if API_ID and API_HASH:
-    alpha = Alpha("SpLFW", api_id=API_ID, api_hash=API_HASH, bot_token=BOT_TOKEN, plugins=dict(root='./SpoiledPlugins'))
+    alpha = Alpha("SpLFW", api_id=API_ID, api_hash=API_HASH, bot_token=BOT_TOKEN, plugins=dict(root='Spoiled/SpoiledPlugins'))
   else:
-    alpha = Alpha("SpLFW", bot_token=BOT_TOKEN, plugins=dict(root='./SpoiledPlugins'))
+    alpha = Alpha("SpLFW", bot_token=BOT_TOKEN, plugins=dict(root='Spoiled/SpoiledPlugins'))
 except Exception as e:
   print(e)
   sys.exit()
 
 def __initialize__():  
   try:
     database()
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/__init__.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/callbacks.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from . import capsify, _sort, mention, title
+from .help import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
 from alphagram.types import IKM, IKB
 from alphagram import Alpha, filters
 from ..Database.privacy import *
 from ..Database.chats import get_served_chats
 from ..Database.users import get_served_users
 from ..Database.global_stats import get_users_dic, get_chats_dic
 from ..Database.chat_words import get_top_chat_users
 from ..Database.user_chat_info import get_user_info, get_chat_info
 from ..Database.coins import _get, _get_chat
 from .templates import info_template
 from Spoiled import CODE_OWNER_ID
+import asyncio
 
 @Alpha.on_callback_query(filters.regex('leaderboard'))
 async def leaderboard_cbq(_, q):
   markup = IKM(
     [
       [
         IKB(capsify('users'), callback_data='users'),
@@ -23,18 +25,50 @@
         IKB(capsify("back"), callback_data="backtostart")
       ]
     ]
   )
   await q.answer()
   await q.edit_message_text(capsify('» private accounts will be hidden.') + '\n\n' + capsify('choose from below !'), reply_markup=markup)
 
+@Alpha.on_callback_query(filters.regex('help'))
+async def help_cbq(_, q):
+  txt = f'**{capsify("commands")}**\n\n'
+  txt += f'`/leaderboard` - {capsify("to get the top players [only groups].")}\n'
+  txt += f'`/coins` - {capsify("to display your coins [only groups].")}\n'
+  txt += '\n'
+  txt += f'**{capsify("bot owner contact")}**\n\n'
+  group = capsify('group')
+  channel = capsify('channel')
+  txt += f'{group} : @{SUPPORT_GROUP}\n'
+  txt += f'{channel} : @{SUPPORT_CHANNEL}\n'
+  txt += '\n'
+  txt += f'**{capsify("code owner contact")}**\n\n'
+  txt += f'{group} : @Spoiled_Community\n'
+  txt += f'{channel} : @SpLBots\n'
+  markup = IKM(
+      [
+          [
+              IKB(capsify('bot owner'), user_id=OWNER_ID)
+          ],
+          [
+              IKB(capsify('code owner'), user_id=CODE_OWNER_ID)
+          ],
+          [
+              IKB(capsify('back'), callback_data='backtostart')
+          ]
+      ]
+  )
+  await q.answer()
+  await q.edit_message_text(txt, reply_markup=markup)
+
 @Alpha.on_callback_query(filters.regex('info'))
 async def info_cbq(_, q):
-  chats = str(len(await get_served_chats()))
-  users = str(len(await get_served_users()))
+  chats, users = await asyncio.gather(get_served_chats(), get_served_users())
+  chats = str(len(chats))
+  users = str(len(users))
   txt = info_template(chats, users)
   markup = IKM(
     [
       [
         IKB(capsify('owner'), user_id=CODE_OWNER_ID),
         IKB(capsify('channel'), url='t.me/SpLBots')
       ],
@@ -82,16 +116,15 @@
 async def privacy_answer_cbq(_, q):
   txt = 'use buttons below to toggle private mode !'
   await q.answer(capsify(txt), show_alert=True)
 
 @Alpha.on_callback_query(filters.regex('users') | filters.regex('users_'))
 async def users(_, q):
   if q.data == 'users':
-    x = await get_private_users()
-    dic = await get_users_dic()
+    x, dic = await asyncio.gather(get_private_users(), get_users_dic())
     dic = _sort(dic)
     a = 1
     txt = capsify('top users by words') + "\n\n"
     for y in dic:
       y = int(y)
       if y in x:
         continue
@@ -108,16 +141,15 @@
           IKB(capsify('back'), callback_data='leaderboard')
         ]
       ]
     )
     await q.answer()
     await q.edit_message_text(txt, reply_markup=markup)
   else:
-    x = await get_private_users()
-    dic = await _get()
+    x, dic = await asyncio.gather(get_private_users(), _get())
     dic = _sort(dic)
     a = 1
     txt = capsify('top users by coins') + '\n\n'
     for y in dic:
       y = int(y)
       if y in x:
         continue
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/coins.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/coins.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/eval.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from io import StringIO
 from time import time
 
 from . import capsify
 from alphagram import filters
 from alphagram.types import IKB as InlineKeyboardButton, IKM as InlineKeyboardMarkup, Message
 
-from shivi import alpha as app
+from Spoiled import alpha as app
 from config import OWNER_ID as OWNER
 
 SUDOERS = filters.user(OWNER)
 
 async def aexec(code, client, message):
     exec(
         "async def __aexec(client, message): "
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/fw.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/fw.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..Database.chat_words import incr_chat_word
 from ..Database.coins import add_coins
 from ..Database.global_stats import *
 from ..Database.record import update_record
 from Spoiled.Shannu.config import SUPPORT_GROUP, WORD_SPAWN_TIME
 from .watchers import fw_watcher
 import words
-from Spoiled.Shannu.alpha import alpha
+from Spoiled import alpha
 from .image import make_image
 import asyncio
 import time
 
 dic = {} # status dict
 last_sent = {} # queue dict
 
@@ -70,18 +70,19 @@
   await add_coins(user_id, int(rew), chat_id)
 
 async def send():
   global last_sent, dic
   _ = alpha
   while True:
     try:
-        un = _.me.username
+      un = _.me.username
     except:
-        await asyncio.sleep(1)
-        continue
+      await asyncio.sleep(1)
+      continue
+
     chats = await get_served_chats()
     for x in chats:
       if x in last_sent:
         diff = int(time.time() - last_sent[x])
         if diff >= WORD_SPAWN_TIME:
           w = words.Word()
           im = make_image(w, un)
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/help.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/help.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/image.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/image.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/inline.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/inline.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/leaderboard.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/leaderboard.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/served.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/served.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/start.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/start.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from config import SUPPORT_GROUP, SUPPORT_CHANNEL, OWNER_ID
 from Spoiled.Database.users import add_served_user
 from Spoiled.Database.coins import get_coins
 from Spoiled.Database.completed import get_top_chat, get_completed_words
 from Spoiled.Database.record import get_record
 from . import capsify, get_readable_time, title
 from Spoiled.Shannu.alpha import alpha
+import asyncio
 
 @Alpha.on_message(filters.command('start') & filters.private)
 async def start(_, m):
   await add_served_user(m.from_user.id)
   txt = "Hello {}, Am {}, I sends an Image containing word in which one who completes that word quickly, will be rewarded coins.\n\nCheck info for source code and other Information."
   id = _.me.id
   un = _.me.username
@@ -18,15 +19,15 @@
   user_first_name = m.from_user.first_name
   markup = IKM(
       [
           [
               IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
           ],
           [
-              IKB(capsify("Help 📘"), url=f't.me/{un}?start=help'),
+              IKB(capsify("Help 📘"), callback_data='help'),
               IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
           ],
           [
               IKB(capsify("Profile 👤"), callback_data='profile'),
               IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
           ],
           [
@@ -46,15 +47,15 @@
   user_first_name = q.from_user.first_name
   markup = IKM(
       [
           [
               IKB(capsify("➕ Add me to your group ➕"), url=f't.me/{un}?startgroup=True')
           ],
           [
-              IKB(capsify("Help 📘"), url=f't.me/{un}?start=help'),
+              IKB(capsify("Help 📘"), callback_data='help'),
               IKB(capsify("Hoster ☁️"), user_id=OWNER_ID)
           ],
           [
               IKB(capsify("Profile 👤"), callback_data='profile'),
               IKB(capsify("Leaderboard 🏆"), callback_data='leaderboard')
           ],
           [
@@ -67,28 +68,31 @@
   await q.edit_message_text(txt.format(user_first_name, fn), reply_markup=markup)
 
 @Alpha.on_callback_query(filters.regex('profile'))
 async def profile_cbq(_, q):
   await q.answer()
   await q.edit_message_text(capsify('getting your profile, please wait...'))
   user_id = q.from_user.id
-  cns = await get_coins(user_id)
+  cns, words, top_chat, record = await asyncio.gather(
+    get_coins(user_id),
+    get_completed_words(user_id),
+    get_top_chat(user_id),
+    get_record(user_id)
+  )
   txt = capsify('👤 User Profile')
   txt += '\n\n'
-  words = await get_completed_words(user_id)
   txt += capsify('words completed :') + f' `{words}`.'
   txt += '\n'
   txt += capsify('coins :') + f' `{cns}`.'
-  top_chat = await get_top_chat(user_id)
   if top_chat:
     top_chat = await title(int(top_chat))
   txt += '\n'
   txt += capsify('top chat :') + f' {top_chat}.'
   txt += '\n'
-  txt += capsify('record :') + f' `{get_readable_time(int(await get_record(user_id)))}.`'
+  txt += capsify('record :') + f' `{get_readable_time(int(record))}.`'
   markup = IKM(
     [
       [
         IKB(capsify("share profile"), switch_inline_query='share')
       ],
       [
         IKB(capsify('back'), callback_data='backtostart')
```

### Comparing `SpLFastlyWrite-1.0.7/Spoiled/SpoiledPlugins/templates.py` & `SpLFastlyWrite-1.0.8/Spoiled/SpoiledPlugins/templates.py`

 * *Files identical despite different names*

### Comparing `SpLFastlyWrite-1.0.7/setup.py` & `SpLFastlyWrite-1.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="SpLFastlyWrite",
-    version="1.0.7",
+    version="1.0.8",
     description="SpLFastlyWrite",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ShutupKeshav/SpLFastlyWrite",
     download_url="https://github.com/ShutupKeshav/SpLFastlyWrite/releases/latest",
     author="ShutupKeshav",
     author_email="keshavatripathi@yahoo.com",
```

