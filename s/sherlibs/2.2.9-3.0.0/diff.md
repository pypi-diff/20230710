# Comparing `tmp/sherlibs-2.2.9.tar.gz` & `tmp/sherlibs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlibs-2.2.9.tar", last modified: Sat Jul  8 11:00:44 2023, max compression
+gzip compressed data, was "sherlibs-3.0.0.tar", last modified: Mon Jul 10 12:31:35 2023, max compression
```

## Comparing `sherlibs-2.2.9.tar` & `sherlibs-3.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.989258 sherlibs-2.2.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.981257 sherlibs-2.2.9/Ayra/
--rw-r--r--   0 root         (0) root         (0)     2893 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.981257 sherlibs-2.2.9/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4696 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12383 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.985257 sherlibs-2.2.9/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.989258 sherlibs-2.2.9/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    19969 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28733 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.989258 sherlibs-2.2.9/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18588 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-08 11:00:30.000000 sherlibs-2.2.9/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-07-08 11:00:30.000000 sherlibs-2.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3449 2023-07-08 11:00:44.993258 sherlibs-2.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2608 2023-07-08 11:00:30.000000 sherlibs-2.2.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 11:00:44.993258 sherlibs-2.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1520 2023-07-08 11:00:30.000000 sherlibs-2.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 11:00:44.989258 sherlibs-2.2.9/sherlibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3449 2023-07-08 11:00:44.000000 sherlibs-2.2.9/sherlibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-08 11:00:44.000000 sherlibs-2.2.9/sherlibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 11:00:44.000000 sherlibs-2.2.9/sherlibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 11:00:44.000000 sherlibs-2.2.9/sherlibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-08 11:00:44.000000 sherlibs-2.2.9/sherlibs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.494884 sherlibs-3.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.486884 sherlibs-3.0.0/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.486884 sherlibs-3.0.0/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4696 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12383 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.490884 sherlibs-3.0.0/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.490884 sherlibs-3.0.0/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    19969 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17358 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28733 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.490884 sherlibs-3.0.0/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18588 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-10 12:30:53.000000 sherlibs-3.0.0/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-07-10 12:30:53.000000 sherlibs-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-10 12:31:35.494884 sherlibs-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-07-10 12:30:53.000000 sherlibs-3.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 12:31:35.494884 sherlibs-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-07-10 12:30:53.000000 sherlibs-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 12:31:35.494884 sherlibs-3.0.0/sherlibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-10 12:31:35.000000 sherlibs-3.0.0/sherlibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-10 12:31:35.000000 sherlibs-3.0.0/sherlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 12:31:35.000000 sherlibs-3.0.0/sherlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 12:31:35.000000 sherlibs-3.0.0/sherlibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-10 12:31:35.000000 sherlibs-3.0.0/sherlibs.egg-info/top_level.txt
```

### Comparing `sherlibs-2.2.9/Ayra/__init__.py` & `sherlibs-3.0.0/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/__main__.py` & `sherlibs-3.0.0/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/_misc/__init__.py` & `sherlibs-3.0.0/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/_misc/_assistant.py` & `sherlibs-3.0.0/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/_misc/_decorators.py` & `sherlibs-3.0.0/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/_misc/_supporter.py` & `sherlibs-3.0.0/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/_misc/_wrappers.py` & `sherlibs-3.0.0/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/configs.py` & `sherlibs-3.0.0/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/__init__.py` & `sherlibs-3.0.0/Ayra/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/afk_db.py` & `sherlibs-3.0.0/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/antiflood_db.py` & `sherlibs-3.0.0/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/asst_fns.py` & `sherlibs-3.0.0/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/asstcmd_db.py` & `sherlibs-3.0.0/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/autoban_db.py` & `sherlibs-3.0.0/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/blacklist_db.py` & `sherlibs-3.0.0/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/botchat_db.py` & `sherlibs-3.0.0/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/broadcast_db.py` & `sherlibs-3.0.0/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/ch_db.py` & `sherlibs-3.0.0/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/dnd_db.py` & `sherlibs-3.0.0/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/echo_db.py` & `sherlibs-3.0.0/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/filestore_db.py` & `sherlibs-3.0.0/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/filter_db.py` & `sherlibs-3.0.0/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/forcesub_db.py` & `sherlibs-3.0.0/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/gban_mute_db.py` & `sherlibs-3.0.0/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/gcast_blacklist_db.py` & `sherlibs-3.0.0/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/greetings_db.py` & `sherlibs-3.0.0/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/logusers_db.py` & `sherlibs-3.0.0/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/mute_db.py` & `sherlibs-3.0.0/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/night_db.py` & `sherlibs-3.0.0/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/notes_db.py` & `sherlibs-3.0.0/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/nsfw_db.py` & `sherlibs-3.0.0/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/pmpermit_db.py` & `sherlibs-3.0.0/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/snips_db.py` & `sherlibs-3.0.0/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/vc_sudos.py` & `sherlibs-3.0.0/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/dB/warn_db.py` & `sherlibs-3.0.0/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/FastTelethon.py` & `sherlibs-3.0.0/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/__init__.py` & `sherlibs-3.0.0/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/admins.py` & `sherlibs-3.0.0/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/executor.py` & `sherlibs-3.0.0/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/gDrive.py` & `sherlibs-3.0.0/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/google_image.py` & `sherlibs-3.0.0/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/helper.py` & `sherlibs-3.0.0/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/info.py` & `sherlibs-3.0.0/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/misc.py` & `sherlibs-3.0.0/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/tools.py` & `sherlibs-3.0.0/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/fns/ytdl.py` & `sherlibs-3.0.0/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/kynan.py` & `sherlibs-3.0.0/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/loader.py` & `sherlibs-3.0.0/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/BaseClient.py` & `sherlibs-3.0.0/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/__init__.py` & `sherlibs-3.0.0/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/_database.py` & `sherlibs-3.0.0/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/_extra.py` & `sherlibs-3.0.0/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/connections.py` & `sherlibs-3.0.0/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/funcs.py` & `sherlibs-3.0.0/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/loader.py` & `sherlibs-3.0.0/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/Ayra/startup/utils.py` & `sherlibs-3.0.0/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/LICENSE` & `sherlibs-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/PKG-INFO` & `sherlibs-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 2.2.9
+Version: 3.0.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-2.2.9/README.md` & `sherlibs-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/setup.py` & `sherlibs-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `sherlibs-2.2.9/sherlibs.egg-info/PKG-INFO` & `sherlibs-3.0.0/sherlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherlibs
-Version: 2.2.9
+Version: 3.0.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Shearlean Userbot.
 Home-page: https://github.com/shearlean10/sherlibs
 Author: shearlean10
 Author-email: shearleanshop@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/shearlean10/sherlibs/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `sherlibs-2.2.9/sherlibs.egg-info/SOURCES.txt` & `sherlibs-3.0.0/sherlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

