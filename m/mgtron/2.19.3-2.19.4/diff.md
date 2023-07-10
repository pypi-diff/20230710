# Comparing `tmp/mgtron-2.19.3.tar.gz` & `tmp/mgtron-2.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.19.3.tar", last modified: Mon Jul 10 18:28:00 2023, max compression
+gzip compressed data, was "mgtron-2.19.4.tar", last modified: Mon Jul 10 21:11:49 2023, max compression
```

## Comparing `mgtron-2.19.3.tar` & `mgtron-2.19.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.280755 mgtron-2.19.3/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.254088 mgtron-2.19.3/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.254088 mgtron-2.19.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.3/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.3/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.254088 mgtron-2.19.3/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.3/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.3/.github/workflows/pypi_action.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.3/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9113 2023-07-10 17:32:43.000000 mgtron-2.19.3/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.3/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 18:28:00.280755 mgtron-2.19.3/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.3/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.257421 mgtron-2.19.3/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.3/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.3/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.257421 mgtron-2.19.3/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-10 18:28:00.000000 mgtron-2.19.3/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.3/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.3/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-10 18:28:00.280755 mgtron-2.19.3/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.257421 mgtron-2.19.3/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.3/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.267421 mgtron-2.19.3/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/CA_subheading.png
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/init_cellantenna.sh
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/assets/log_read
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/assets/network-wireless.ico
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/assets/wifi_rs
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.274088 mgtron-2.19.3/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/ble/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.3/src/ble/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.274088 mgtron-2.19.3/src/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/db/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.3/src/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.274088 mgtron-2.19.3/src/globals/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/globals/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/globals/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.274088 mgtron-2.19.3/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.277421 mgtron-2.19.3/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.3/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.277421 mgtron-2.19.3/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    50348 2023-07-10 18:12:57.000000 mgtron-2.19.3/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10883 2023-07-10 17:32:43.000000 mgtron-2.19.3/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43723 2023-07-10 18:08:31.000000 mgtron-2.19.3/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.280755 mgtron-2.19.3/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.3/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.280755 mgtron-2.19.3/src/wifi/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.3/src/wifi/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/wifi/chasing.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15530 2023-07-10 18:23:02.000000 mgtron-2.19.3/src/wifi/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.3/src/wifi/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.254088 mgtron-2.19.3/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:28:00.280755 mgtron-2.19.3/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.773149 mgtron-2.19.4/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.4/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.4/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.4/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9254 2023-07-10 21:07:07.000000 mgtron-2.19.4/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.4/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 21:11:49.799816 mgtron-2.19.4/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.4/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.4/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.4/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.4/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.4/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-10 21:11:49.799816 mgtron-2.19.4/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.4/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.783149 mgtron-2.19.4/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/CA_subheading.png
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/init_cellantenna.sh
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/log_read
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/network-wireless.ico
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/wifi_rs
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.789816 mgtron-2.19.4/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.4/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.4/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.4/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    50355 2023-07-10 20:59:37.000000 mgtron-2.19.4/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10970 2023-07-10 20:18:55.000000 mgtron-2.19.4/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43723 2023-07-10 20:40:44.000000 mgtron-2.19.4/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/wifi/chasing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15531 2023-07-10 21:02:34.000000 mgtron-2.19.4/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.773149 mgtron-2.19.4/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.19.3/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/.github/workflows/black_actions.yml` & `mgtron-2.19.4/.github/workflows/black_actions.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/.github/workflows/pypi_action.yml` & `mgtron-2.19.4/.github/workflows/pypi_action.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/CHANGELOG.md` & `mgtron-2.19.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✳️ [2.19.4] - 2023 JULY 10
+
+- Add scrollbar to the wifi scan results.
+- Status indicator properly sends zero to power on the Teensy.
+
 ## ✳️ [2.19.1] - 2023 JULY 10
 
 - Removed duplicates of wifi scan result frequencies.
 - Fixed state awareness of the 'SEND ALL' button.
 - Remove blockage to send commands to the Teensy.
 
 ## ✴️️️ [2.19.0] - 2023 JULY 07
```

### Comparing `mgtron-2.19.3/LICENSE.rst` & `mgtron-2.19.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/PKG-INFO` & `mgtron-2.19.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.3
+Version: 2.19.4
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.3/README.md` & `mgtron-2.19.4/README.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/docs/MGTron Command Description.docx` & `mgtron-2.19.4/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/docs/MGTron Function Descriptions.docx` & `mgtron-2.19.4/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/mgtron.egg-info/PKG-INFO` & `mgtron-2.19.4/mgtron.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.3
+Version: 2.19.4
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.3/mgtron.egg-info/SOURCES.txt` & `mgtron-2.19.4/mgtron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/mgtron.egg-info/requires.txt` & `mgtron-2.19.4/mgtron.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/pyproject.toml` & `mgtron-2.19.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/requirements.txt` & `mgtron-2.19.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/CA logo without subtext.JPG` & `mgtron-2.19.4/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/CA_subheading.png` & `mgtron-2.19.4/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/blueio_rs` & `mgtron-2.19.4/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/init_cellantenna.sh` & `mgtron-2.19.4/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/log_read` & `mgtron-2.19.4/src/assets/log_read`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/mgtron.svg` & `mgtron-2.19.4/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/network-wireless.ico` & `mgtron-2.19.4/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/assets/wifi_rs` & `mgtron-2.19.4/src/assets/wifi_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/ble/ble_data.py` & `mgtron-2.19.4/src/ble/ble_data.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/ble/helpers.py` & `mgtron-2.19.4/src/ble/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/ble/scanning.py` & `mgtron-2.19.4/src/ble/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/helpers.py` & `mgtron-2.19.4/src/db/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/init_db.sql` & `mgtron-2.19.4/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/long_save.json` & `mgtron-2.19.4/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/mgtron_db.db` & `mgtron-2.19.4/src/db/mgtron_db.db`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/models.py` & `mgtron-2.19.4/src/db/models.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/db/quick_save.json` & `mgtron-2.19.4/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/globals/helpers.py` & `mgtron-2.19.4/src/globals/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/gui/helpers.py` & `mgtron-2.19.4/src/gui/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,28 +694,28 @@
         else:
             loggey.info(msg=f"auto send flag: {AUTO_SEND_FLAG}")
 
     except (KeyError, SystemError, NameError) as an_error:
         loggey.warning(msg=f"Error: {an_error}")
 
 
-def kill_channel(user_data: int) -> None:
+def kill_channel(sender, app_data, user_data: int) -> None:
     """Kill channel w/out resetting power on user facing screen."""
-    print(f"kill channel {user_data}")
+    loggey.debug("%s() executed", kill_channel.__name__)
 
     PORT = get_device_path_from_serial_number()
 
     data_vehicle.change_power(
         channel=user_data,
         power_level=0,
         PORT=PORT
     )
 
     dpg.bind_item_theme(
-        item=f"stats_{user_data.split('_')[-1]}",
+        item=sender,
         theme=grey_btn_theme)
 
 
 def device_finder(user_data: int = int()) -> None:
     """Filter all connected devices and present only Teensy devices."""
     loggey.info(msg=f"{device_finder.__name__}() executed")
```

### Comparing `mgtron-2.19.3/src/gui/interface.py` & `mgtron-2.19.4/src/gui/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     sleep(0.095)  # Allow time to read and execute via serial *REQUIRED*
 
     try:
         # If the teensy is corrupted the GUI freezes here
         logger.debug(msg=f"Attempting to open serial connection {NAME}()")
         with serial.Serial() as ser:
             ser.port = PORT.strip()
-            ser.timeout = 1.8  # seconds
+            ser.timeout = 0.8  # seconds
             logger.debug(msg=f"Serial device set | {NAME}()")
 
             ser.baudrate = BAUDRATE
             logger.debug(msg=f"baudrate set | {NAME}()")
 
             ser.timeout = 0.8  # seconds
             logger.debug(msg=f"timeout set | {NAME}()")
@@ -223,101 +223,98 @@
         logger.info(msg=f"Connected device path: {PORT}")
     except TypeError:
         logger.exception(msg="No device found on system")
 
     @classmethod
     def status(cls, PORT: str) -> None:
         """Check the status of the board."""
-        logger.info(f"{Megatron.status.__name__} function executed")
+        logger.debug("%s()", Megatron.status.__name__)
         serial_call("s", PORT=PORT)
 
     def change_power(self, channel: int, power_level: int, PORT: str):
         """Change the power level of a channel Range: 0 - 63."""
         # print(f"Change power: PORT === {PORT}")
-        logger.info(f"{Megatron.change_power.__name__} function executed")
+        logger.debug("%s()", Megatron.change_power.__name__)
         logger.info(msg=f"Connected device path: {PORT}")
         return serial_call("p", str(channel), str(power_level), PORT=PORT)
 
     def change_freq(self, channel: int, frequency: float, PORT: str):
         """Change the frequency of a channel Range: 50 - 6400 MHz."""
-        logger.info(f"{Megatron.change_freq.__name__} function executed")
+        logger.debug("%s()", Megatron.change_freq.__name__)
         # print()
         return serial_call("f", str(channel), str(frequency), PORT=PORT)
 
     def change_bandwidth(self, channel: int, percentage: int, PORT: str):
-        """
-        Change the bandwidth of a channel
-        Range: 0 - 100
-        """
-
-        logger.info(f"{Megatron.change_bandwidth.__name__} function executed")
+        """Change the bandwidth of a channel; Range: 0 - 100."""
+        logger.debug("%s()", Megatron.change_bandwidth.__name__)
         return serial_call("b", str(channel), str(percentage), PORT=PORT)
 
     def save_state(self, state: bool, PORT: str) -> None:
-        """Save each settings made by the user into memory for next startup"""
+        """Save each settings made by the user into memory for next startup."""
+        logger.debug("%s()", Megatron.save_state.__name__)
 
         state = 1 if state else 0  # type: ignore
         try:
             serial_call("x", str(state), PORT=PORT)
-            logger.info(f"{Megatron.save_state.__name__} function executed")
+            logger.debug("%s()", Megatron.save_state.__name__)
         except TypeError:
             logger.exception(msg="No device assigned")
 
     def amplification(self, channel: int, state: bool, PORT: str) -> None:
-        """Output HIGH or LOW logic level out of a chosen channel"""
+        """Output HIGH or LOW logic level out of a chosen channel."""
+        logger.debug("%s()", Megatron.amplification.__name__)
 
         state = 1 if state else 0  # type: ignore
         serial_call("a", str(channel), str(state), PORT=PORT)
-        logger.info(f"{Megatron.amplification.__name__} function executed")
+        logger.debug("%s()", Megatron.amplification.__name__)
 
     def stability(self, state: bool, PORT: str) -> None:
-        """Boolean a second
-        filtering stage of capacitors for further stability"""
+        """Second filtering stage of capacitors for further stability."""
+        logger.debug("%s()", Megatron.stability.__name__)
 
         state = 1 if state else 0  # type: ignore
         serial_call("~", str(state), PORT=PORT)
-        logger.info(f"{Megatron.stability.__name__} function executed")
+        logger.debug("%s()", Megatron.stability.__name__)
 
     def noise_control(self, state: bool, percentage: int, PORT: str) -> None:
-        """
-        Optimal settings hardcoded; Input @ %100 Output @ %85
-        state 0: Output stage
-        state 1: Input stage
-        """
+        """Optimal settings hardcoded; Input @ %100 Output @ %85."""
+        """state 0: Output stage."""
+        """state 1: Input stage."""
 
         state = 1 if state else 0  # type: ignore
         serial_call("n", str(state), str(percentage), PORT=PORT)
-        logger.info(f"{Megatron.noise_control.__name__} function executed")
+        logger.debug("%s()", Megatron.noise_control.__name__)
 
     def reset_board(self, PORT: str) -> None:
-        """Reset the parameters of the board"""
+        """Reset the parameters of the board."""
+        logger.debug("%s()", Megatron.reset_board.__name__)
 
         [
             (
                 serial_call("p", str(i), "0", PORT=PORT),
                 # serial_call("b", str(i), "0", PORT=PORT),
                 # serial_call("f", str(i), "50.00", PORT=PORT),
             )
             for i in range(1, 9)
         ]
 
-        logger.info(f"{Megatron.reset_board.__name__} function executed")
+        logger.debug("%s()", Megatron.reset_board.__name__)
 
     logger.info(msg="class Megatron initialized")
 
 
 logger.debug(msg=f"EOF: {__name__}")
 
 
 def main() -> None:
+    """Main function."""
     # import random
 
     # find_device("linux")
     # test_1 = Megatron()
-    pass
 
     # for i in range(8):
     # test_1.change_power(i+1, random.randint(a=10, b=63))
     # sleep(1)
     # test_1.change_freq(i+1, random.randint(a=50, b=6300))
     # sleep(1)
     # test_1.change_bandwidth(i+1, random.randint(a=10, b=100))
```

### Comparing `mgtron-2.19.3/src/main.py` & `mgtron-2.19.4/src/main.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/tests/test_configfiles.py` & `mgtron-2.19.4/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/tests/test_helpers.py` & `mgtron-2.19.4/src/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/src/wifi/helpers.py` & `mgtron-2.19.4/src/wifi/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 def scan_window(colwidth_delineate, wifi_button_width) -> None:
     """Create a window to display the scan results."""
     loggei.info("%s()", scan_window.__name__)
 
     with dpg.window(
         tag=129,
-        no_scrollbar=True,
+        no_scrollbar=False,
         no_collapse=True,
         no_resize=True,
         no_title_bar=True,
         no_move=True,
         modal=True,
         pos=(0, 50),
         width=880,
```

### Comparing `mgtron-2.19.3/src/wifi/scanning.py` & `mgtron-2.19.4/src/wifi/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2html.py` & `mgtron-2.19.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2html4.py` & `mgtron-2.19.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2html5.py` & `mgtron-2.19.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2latex.py` & `mgtron-2.19.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2man.py` & `mgtron-2.19.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2odt.py` & `mgtron-2.19.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.19.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2pseudoxml.py` & `mgtron-2.19.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2s5.py` & `mgtron-2.19.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2xetex.py` & `mgtron-2.19.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rst2xml.py` & `mgtron-2.19.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.3/venv/bin/rstpep2html.py` & `mgtron-2.19.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

