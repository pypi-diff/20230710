# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.9.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.1.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.9.tar` & `nonebot_plugin_l4d2_server-0.5.9.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-07-09 15:23:29.852550 nonebot_plugin_l4d2_server-0.5.9/LICENSE
--rw-r--r--   0        0        0     5683 2023-07-09 15:23:29.852550 nonebot_plugin_l4d2_server-0.5.9/README.md
--rw-r--r--   0        0        0    18107 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-09 15:23:29.856550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     9076 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3252 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3364 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1344 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4034 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-09 15:23:29.860550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1832 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4211 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4174 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      665 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9493 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1091 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     4018 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1421 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7222 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3854 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1030 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    11828 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4067 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9199 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6197 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1243 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2149 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9994 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8469 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14982 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1604 2023-07-09 15:23:29.864550 nonebot_plugin_l4d2_server-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     7547 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-10 02:36:47.072109 nonebot_plugin_l4d2_server-0.5.9.1/LICENSE
+-rw-r--r--   0        0        0     5683 2023-07-10 02:36:47.072109 nonebot_plugin_l4d2_server-0.5.9.1/README.md
+-rw-r--r--   0        0        0    18107 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     9076 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1694 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3530 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3364 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1344 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4034 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1832 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4211 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      665 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9493 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1083 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     4018 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1421 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7222 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3854 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1030 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    11828 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4067 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9197 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6197 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1243 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2149 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9994 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8469 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14982 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1606 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9.1/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9/LICENSE` & `nonebot_plugin_l4d2_server-0.5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/README.md` & `nonebot_plugin_l4d2_server-0.5.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,91 +2,103 @@
     DATASQLITE,
     table_data,
     L4d2_players_tag,
     L4d2_server_tag,
     L4d2_INTEGER,
     L4d2_TEXT,
     L4d2_BOOLEAN,
-    tables_columns
-    )
+    tables_columns,
+)
 import sqlite3
 from nonebot.log import logger
 
 
-
-
 class L4D2DataSqlite:
     """连接数据库和断开数据库，以及一些检查函数"""
+
     def __init__(self):
         """连接数据库"""
         self.datasqlite_path = DATASQLITE
         self.datasqlite_path.mkdir(parents=True, exist_ok=True)
-        self.conn = sqlite3.connect(self.datasqlite_path / 'L4D2.db')
+        self.conn = sqlite3.connect(self.datasqlite_path / "L4D2.db")
         self._check_tables_exist()
         self._check_data_existence()
         self._check_data_validity()
         logger.info("已连接求生数据库")
-    
+
     def _base_conn(self):
         return self.conn
-        
+
     def _check_tables_exist(self) -> None:
         """
         检查表是否存在
-        """  
+        """
         c = self.conn.cursor()
         for table in table_data:
-            c.execute(f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'")
+            c.execute(
+                f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'"
+            )
             if c.fetchone() is None:
                 if table == "L4d2_players":
                     c.execute(f"CREATE TABLE {table} (qq INTEGER PRIMARY KEY)")
                 elif table == "L4D2_server":
                     c.execute(f"CREATE TABLE {table} (number INTEGER PRIMARY KEY)")
                 self.conn.commit()
-        
-        
 
     def _check_data_existence(self) -> None:
         """
         检查表头是否存在，如果不存在则新建并填充默认值
         """
         c = self.conn.cursor()
         for table, tag in tables_columns.items():
             for column in tag:
                 c.execute(f"PRAGMA table_info({table})")
                 if not any(col[1] == column for col in c.fetchall()):
                     if column in L4d2_BOOLEAN:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0')
+                        c.execute(
+                            f"ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0"
+                        )
                     elif column in L4d2_INTEGER:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL')
+                        c.execute(
+                            f"ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL"
+                        )
                     else:
-                        c.execute(f'ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL')
+                        c.execute(
+                            f"ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL"
+                        )
         self.conn.commit()
 
-    
     def _check_data_validity(self) -> None:
         """
         检查数据库数据的合法性
         错误数据默认填充NULL或者False
         """
         c = self.conn.cursor()
         for table in table_data:
             if table == "L4d2_players":
                 columns = L4d2_players_tag
-            elif table == "L4D2_server":
+            else:
                 columns = L4d2_server_tag
+        if not columns:
+            return
         for column in columns:
             if column in L4d2_INTEGER:
-                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'")
+                c.execute(
+                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'"
+                )
             elif column in L4d2_TEXT:
-                c.execute(f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'")
+                c.execute(
+                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'"
+                )
             elif column in L4d2_BOOLEAN:
-                c.execute(f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'")
+                c.execute(
+                    f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'"
+                )
         self.conn.commit()
-        
+
     def _close(self):
         """断开连接到数据库"""
         self.conn.close()
         logger.info("已断开求生数据库")
 
 
-sq_L4D2 = L4D2DataSqlite()
+sq_L4D2 = L4D2DataSqlite()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pathlib import Path
 
 # 半透明素材
 half_whitel_image_path = Path(__file__).parent.parent.joinpath("data/img/white.png")
 half_whitel_image = Image.open(half_whitel_image_path)
 
 
-# async def one_server_img(msg: dict):
-#     """单个服务器的dict信息变成图片"""
-#     img_background = await adjust_image_size(msg["Players"])
-#     img_background = await adjust_server_name(img_background, msg["name"])
+async def one_server_img(msg: dict):
+    """单个服务器的dict信息变成图片"""
+    img_background = await adjust_image_size(msg["Players"])
+    img_background = await adjust_server_name(img_background, msg["name"])
 
 
 async def adjust_image_size(text_list):
     """初始化背景"""
     initial_width = 1080
     initial_height = 600
     height_increment = 100
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     @prison.handle()
     async def _(matcher: Matcher, event: MessageEvent):
         msg = await get_tan_jian(ip_anne_list, 2)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
     @open_prison.handle()
     async def _(matcher: Matcher, event: MessageEvent):
-
         msg = await get_tan_jian(ip_anne_list, 3)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
 
 async def get_read_ip(ip_anne_list):
     get_ip = on_command("anne", aliases=server_key(), priority=80, block=True)
 
@@ -238,15 +237,14 @@
             ip_list.append((one_ip["id"], host, port))
         img = await qq_ip_queries_pic(ip_list, igr)
         if img:
             return img
         else:
             return "服务器无响应"
     else:
-
         if not msg[0].isdigit():
             if any(mode in msg for mode in gamemode_list):
                 pass
             else:
                 return
         message = await json_server_to_tag_dict(command, msg)
         if len(message) == 0:
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.9"
+version = "0.5.9.1"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.9
+Version: 0.5.9.1
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9 Summary:
-L4D2 server related operations plugin for NoneBot2 Home-page: https://
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9.1
+Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

