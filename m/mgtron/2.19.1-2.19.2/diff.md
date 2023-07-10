# Comparing `tmp/mgtron-2.19.1.tar.gz` & `tmp/mgtron-2.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.19.1.tar", last modified: Mon Jul 10 14:43:33 2023, max compression
+gzip compressed data, was "mgtron-2.19.2.tar", last modified: Mon Jul 10 18:20:07 2023, max compression
```

## Comparing `mgtron-2.19.1.tar` & `mgtron-2.19.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.099683 mgtron-2.19.1/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.073016 mgtron-2.19.1/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.073016 mgtron-2.19.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.1/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.073016 mgtron-2.19.1/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.1/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.1/.github/workflows/pypi_action.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.1/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9063 2023-07-10 14:37:39.000000 mgtron-2.19.1/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.1/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 14:43:33.099683 mgtron-2.19.1/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.1/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.073016 mgtron-2.19.1/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.1/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.1/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.076349 mgtron-2.19.1/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 14:43:32.000000 mgtron-2.19.1/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-10 14:43:33.000000 mgtron-2.19.1/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-10 14:43:32.000000 mgtron-2.19.1/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-10 14:43:32.000000 mgtron-2.19.1/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1966 2023-07-10 14:43:32.000000 mgtron-2.19.1/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-10 14:43:32.000000 mgtron-2.19.1/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.1/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1903 2023-07-10 14:37:39.000000 mgtron-2.19.1/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-10 14:43:33.099683 mgtron-2.19.1/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.076349 mgtron-2.19.1/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.1/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.083016 mgtron-2.19.1/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/CA_subheading.png
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/init_cellantenna.sh
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/assets/log_read
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/assets/network-wireless.ico
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/assets/wifi_rs
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.089683 mgtron-2.19.1/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/ble/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.1/src/ble/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.093016 mgtron-2.19.1/src/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/db/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.1/src/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.093016 mgtron-2.19.1/src/globals/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/globals/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/globals/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.093016 mgtron-2.19.1/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.093016 mgtron-2.19.1/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.1/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.096350 mgtron-2.19.1/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    50253 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43723 2023-07-10 14:38:33.000000 mgtron-2.19.1/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.096350 mgtron-2.19.1/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.1/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.096350 mgtron-2.19.1/src/wifi/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.1/src/wifi/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/wifi/chasing.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15513 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/wifi/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.1/src/wifi/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.073016 mgtron-2.19.1/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 14:43:33.099683 mgtron-2.19.1/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.299960 mgtron-2.19.2/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.273293 mgtron-2.19.2/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.276626 mgtron-2.19.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.2/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.2/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.276626 mgtron-2.19.2/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.2/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.2/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.2/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9113 2023-07-10 17:32:43.000000 mgtron-2.19.2/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.2/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 18:20:07.299960 mgtron-2.19.2/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.2/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.276626 mgtron-2.19.2/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.2/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.2/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.276626 mgtron-2.19.2/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-10 18:20:07.000000 mgtron-2.19.2/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.2/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.2/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-10 18:20:07.299960 mgtron-2.19.2/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.276626 mgtron-2.19.2/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.2/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.283293 mgtron-2.19.2/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/CA_subheading.png
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/init_cellantenna.sh
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/assets/log_read
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/assets/network-wireless.ico
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/assets/wifi_rs
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.293293 mgtron-2.19.2/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.2/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.293293 mgtron-2.19.2/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.2/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.293293 mgtron-2.19.2/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.293293 mgtron-2.19.2/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.296627 mgtron-2.19.2/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.2/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.296627 mgtron-2.19.2/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    50348 2023-07-10 18:12:57.000000 mgtron-2.19.2/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10883 2023-07-10 17:32:43.000000 mgtron-2.19.2/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43723 2023-07-10 18:08:31.000000 mgtron-2.19.2/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.299960 mgtron-2.19.2/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.2/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.299960 mgtron-2.19.2/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.2/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/wifi/chasing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15528 2023-07-10 18:04:39.000000 mgtron-2.19.2/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.2/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.273293 mgtron-2.19.2/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 18:20:07.299960 mgtron-2.19.2/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.2/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.19.1/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.19.2/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.19.2/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/.github/workflows/black_actions.yml` & `mgtron-2.19.2/.github/workflows/black_actions.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/.github/workflows/pypi_action.yml` & `mgtron-2.19.2/.github/workflows/pypi_action.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/CHANGELOG.md` & `mgtron-2.19.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 -------------------------------------------------------------------------------
 
 ## ✳️ [2.19.1] - 2023 JULY 10
 
 - Removed duplicates of wifi scan result frequencies.
 - Fixed state awareness of the 'SEND ALL' button.
+- Remove blockage to send commands to the Teensy.
 
 ## ✴️️️ [2.19.0] - 2023 JULY 07
 
 - WiFi scan results are now selectable.
 - WiFi scan results are in a pretty table.
 - Send all button recognizes the state of WiFi and Bluetooth.
 - Re-scan four times to check for hopping WiFi networks.
```

### Comparing `mgtron-2.19.1/LICENSE.rst` & `mgtron-2.19.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/PKG-INFO` & `mgtron-2.19.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.1
+Version: 2.19.2
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.1/README.md` & `mgtron-2.19.2/README.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/docs/MGTron Command Description.docx` & `mgtron-2.19.2/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/docs/MGTron Function Descriptions.docx` & `mgtron-2.19.2/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/mgtron.egg-info/PKG-INFO` & `mgtron-2.19.2/mgtron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.1
+Version: 2.19.2
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.1/mgtron.egg-info/SOURCES.txt` & `mgtron-2.19.2/mgtron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/mgtron.egg-info/requires.txt` & `mgtron-2.19.2/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 asyncio==3.4.3
 attrs==23.1.0
 autopep8==2.0.2
 beautifultable==1.1.0
 bleach==6.0.0
 bleuio==1.2.0
 build==0.10.0
+cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
 cryptography==41.0.1
 dearpygui==1.9.1
+debugpy==1.6.7
 dill==0.3.6
 distlib==0.3.6
 docstring-to-markdown==0.12
 docutils==0.20.1
 editables==0.3
 exceptiongroup==1.1.1
 filelock==3.12.1
 flake8==6.0.0
+flit_core==3.9.0
 gevent==22.10.2
 greenlet==2.0.2
 grequests==0.7.0
 h11==0.14.0
 hatch==1.7.0
 hatchling==1.18.0
 httpcore==0.17.2
@@ -38,32 +41,33 @@
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jedi==0.18.2
 jeepney==0.8.0
 keyring==23.13.1
 lazy-object-proxy==1.9.0
+lsprotocol==2023.0.0a2
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
-mypy==1.3.0
 mypy-extensions==1.0.0
 packaging==23.1
 parso==0.8.3
 pathspec==0.11.1
 pexpect==4.8.0
 pkginfo==1.9.6
 platformdirs==3.5.3
 pluggy==1.0.0
 ptyprocess==0.7.0
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 pyflakes==3.0.1
+pygls==1.0.2
 Pygments==2.15.1
 pylint==2.17.4
 pyparsing==3.0.9
 pyperclip==1.8.2
 pyproject_hooks==1.0.0
 pyserial==3.5
 pysondb==1.6.7
@@ -79,38 +83,36 @@
 PyYAML==6.0
 readme-renderer==37.3
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.2
 rope==1.8.0
+ruff==0.0.275
+ruff-lsp==0.0.35
 SecretStorage==3.3.3
 shellingham==1.5.0.post1
 six==1.16.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 tabulate==0.9.0
 toml==0.10.2
 tomli==2.0.1
 tomli_w==1.0.0
 tomlkit==0.11.8
 trove-classifiers==2023.5.24
 twine==4.0.2
+typeguard==3.0.2
 typing_extensions==4.6.3
 tzdata==2023.3
 ujson==5.8.0
 urllib3==2.0.3
 userpath==1.8.0
 virtualenv==20.23.0
 wcwidth==0.2.6
 webencodings==0.5.1
 whatthepatch==1.0.5
 wrapt==1.15.0
 yapf==0.33.0
 zipp==3.15.0
 zope.event==4.6
 zope.interface==6.0
-
-[test]
-pytest>=7.3.2
-pytest-asyncio>=0.21.0
-pytest-cov>=4.1.0
```

### Comparing `mgtron-2.19.1/pyproject.toml` & `mgtron-2.19.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/requirements.txt` & `mgtron-2.19.2/mgtron.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 asyncio==3.4.3
 attrs==23.1.0
 autopep8==2.0.2
 beautifultable==1.1.0
 bleach==6.0.0
 bleuio==1.2.0
 build==0.10.0
+cattrs==23.1.2
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
 cryptography==41.0.1
 dearpygui==1.9.1
+debugpy==1.6.7
 dill==0.3.6
 distlib==0.3.6
 docstring-to-markdown==0.12
 docutils==0.20.1
 editables==0.3
 exceptiongroup==1.1.1
 filelock==3.12.1
 flake8==6.0.0
+flit_core==3.9.0
 gevent==22.10.2
 greenlet==2.0.2
 grequests==0.7.0
 h11==0.14.0
 hatch==1.7.0
 hatchling==1.18.0
 httpcore==0.17.2
@@ -38,32 +41,33 @@
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jedi==0.18.2
 jeepney==0.8.0
 keyring==23.13.1
 lazy-object-proxy==1.9.0
+lsprotocol==2023.0.0a2
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
-mypy==1.3.0
 mypy-extensions==1.0.0
 packaging==23.1
 parso==0.8.3
 pathspec==0.11.1
 pexpect==4.8.0
 pkginfo==1.9.6
 platformdirs==3.5.3
 pluggy==1.0.0
 ptyprocess==0.7.0
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 pyflakes==3.0.1
+pygls==1.0.2
 Pygments==2.15.1
 pylint==2.17.4
 pyparsing==3.0.9
 pyperclip==1.8.2
 pyproject_hooks==1.0.0
 pyserial==3.5
 pysondb==1.6.7
@@ -79,33 +83,41 @@
 PyYAML==6.0
 readme-renderer==37.3
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.2
 rope==1.8.0
+ruff==0.0.275
+ruff-lsp==0.0.35
 SecretStorage==3.3.3
 shellingham==1.5.0.post1
 six==1.16.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 tabulate==0.9.0
 toml==0.10.2
 tomli==2.0.1
 tomli_w==1.0.0
 tomlkit==0.11.8
 trove-classifiers==2023.5.24
 twine==4.0.2
+typeguard==3.0.2
 typing_extensions==4.6.3
 tzdata==2023.3
 ujson==5.8.0
 urllib3==2.0.3
 userpath==1.8.0
 virtualenv==20.23.0
 wcwidth==0.2.6
 webencodings==0.5.1
 whatthepatch==1.0.5
 wrapt==1.15.0
 yapf==0.33.0
 zipp==3.15.0
 zope.event==4.6
 zope.interface==6.0
+
+[test]
+pytest>=7.3.2
+pytest-asyncio>=0.21.0
+pytest-cov>=4.1.0
```

### Comparing `mgtron-2.19.1/src/assets/CA logo without subtext.JPG` & `mgtron-2.19.2/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/CA_subheading.png` & `mgtron-2.19.2/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/blueio_rs` & `mgtron-2.19.2/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/init_cellantenna.sh` & `mgtron-2.19.2/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/log_read` & `mgtron-2.19.2/src/assets/log_read`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/mgtron.svg` & `mgtron-2.19.2/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/network-wireless.ico` & `mgtron-2.19.2/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/assets/wifi_rs` & `mgtron-2.19.2/src/assets/wifi_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/ble/ble_data.py` & `mgtron-2.19.2/src/ble/ble_data.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/ble/helpers.py` & `mgtron-2.19.2/src/ble/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/ble/scanning.py` & `mgtron-2.19.2/src/ble/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/helpers.py` & `mgtron-2.19.2/src/db/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/init_db.sql` & `mgtron-2.19.2/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/long_save.json` & `mgtron-2.19.2/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/mgtron_db.db` & `mgtron-2.19.2/src/db/mgtron_db.db`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/models.py` & `mgtron-2.19.2/src/db/models.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/db/quick_save.json` & `mgtron-2.19.2/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/globals/helpers.py` & `mgtron-2.19.2/src/globals/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.19.2/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.19.2/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.19.2/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/gui/helpers.py` & `mgtron-2.19.2/src/gui/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,16 +291,16 @@
     parser, _ = read_config(file=f"{WORKING}/_configs/card_config.ini")
 
     devices = []
 
     try:
         devices: list[int] = [
             int(parser["mgtron"][f"card_{i}"]) for i in range(1, 9)]
-    except KeyError:
-        loggey.warning(msg="No serial number found")
+    except (KeyError, ValueError):
+        loggey.warning(msg="No serial number found or invalid serial number")
 
     # Loop through the list of devices and compare to serial number
     for device in devices:
         if device == int(serial_num):
             serial_number = device
             loggey.debug(
                 msg=f"Serial Number: {serial_number} matched |"
@@ -696,18 +696,22 @@
 
     except (KeyError, SystemError, NameError) as an_error:
         loggey.warning(msg=f"Error: {an_error}")
 
 
 def kill_channel(user_data: int) -> None:
     """Kill channel w/out resetting power on user facing screen."""
+    print(f"kill channel {user_data}")
+
+    PORT = get_device_path_from_serial_number()
+
     data_vehicle.change_power(
         channel=user_data,
         power_level=0,
-        PORT=get_device_path_from_serial_number(),
+        PORT=PORT
     )
 
     dpg.bind_item_theme(
         item=f"stats_{user_data.split('_')[-1]}",
         theme=grey_btn_theme)
```

### Comparing `mgtron-2.19.1/src/gui/interface.py` & `mgtron-2.19.2/src/gui/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             logger.debug(msg=f"Serial device set | {NAME}()")
 
             ser.baudrate = BAUDRATE
             logger.debug(msg=f"baudrate set | {NAME}()")
 
             ser.timeout = 0.8  # seconds
             logger.debug(msg=f"timeout set | {NAME}()")
-            ser.flush()
+            # ser.flush()  # bypass connection issues
             ser.open()
             logger.debug(msg=f"serial connection open | {NAME}()")
 
             # print(" ".join([arg for arg in args]).encode("utf-8"))
             ser.write(" ".join([arg for arg in args]).encode("utf-8"))
             ser.write("\n".encode("utf-8"))
```

### Comparing `mgtron-2.19.1/src/main.py` & `mgtron-2.19.2/src/main.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/tests/test_configfiles.py` & `mgtron-2.19.2/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/tests/test_helpers.py` & `mgtron-2.19.2/src/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/src/wifi/helpers.py` & `mgtron-2.19.2/src/wifi/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 """Helper functions for wifi business of the GUI."""
 
 import os
 import pathlib
-
 from ..globals.helpers import WIFI_BTNS_LIST
 from ..globals.helpers import enable_select_btns
 from ..globals.helpers import disble_select_btns
-
 from .scanning import post_ssid
 from .scanning import freqs_and_sigs
 from .scanning import threaded_scan
 from .scanning import find_signals_and_frequencies
 from .scanning import convert_signal_to_rssi
-
 from ..gui.helpers import callstack_helper
-
 import logging
 from typing import Callable
-
 import dearpygui.dearpygui as dpg
-
 from colorama import Fore as F
 import yaml
-
-from tabulate import tabulate
+import tabulate
 tabulate.PRESERVE_WHITESPACE = True
 
+
 loggei = logging.getLogger(name=__name__)
 
 R = F.RESET
 
 
 # Blue Button Theme
 with dpg.theme() as blue_btn_theme, dpg.theme_component(dpg.mvAll):
@@ -48,15 +42,14 @@
 def convert_data(data):
     """Convert the data from a list of dictionaries to a list of lists."""
     loggei.debug("%s()", convert_data.__name__)
 
     if not data:
         return []
     keys = list(data[0].keys())
-    print("These are the keys {}", keys)
     result = []
     # Order the keys
     keys = ["ssid", "bssid", "channel", "frequency",  "signal", "security"]
 
     for dictionary in data:
         values = [dictionary[key] for key in keys]
         result.append(values)
@@ -131,21 +124,19 @@
         dpg.configure_item(item=129, show=False)
 
         # Get the WiFi dict information and print to GUI
         all_data: list[dict[str, str]] = threaded_scan(
             _dpg=dpg,
             linux_data=find_signals_and_frequencies
         )
-
         dpg.configure_item(item=129, show=True, modal=False)
 
         all_data = convert_signal_to_rssi(all_data)
 
         new_data = convert_data(all_data)  # Converts to list of lists
-
         fill_scan_result(
             converted_data=new_data,
             colwidth_delineate=colwidth_delineate,
             wifi_button_width=wifi_button_width,
         )
 
         [
@@ -163,20 +154,21 @@
         no_collapse=True,
         no_title_bar=True,
         no_move=True,
     ):
         headers = ["SSID", "MAC", "CH", "FREQ", "SIGNAL", "SECURITY"]
 
         dpg.add_text(
-            default_value=" "*7 + "|" + " "*12 + headers[0] + " "*17 +
+
+            default_value=" "*5 + "|" + " "*12 + headers[0] + " "*17 +
             "|" + " " * 8 +
-            headers[1] + " " * 5 + "| " + headers[2] + " | " +
-            " " * 1 +
+            headers[1] + " " * 5 + "| " + headers[2] + " " * 3 + "|" + " " * 2 +
             headers[3] + " " * 2 + "| " + headers[4] + " " + "| " +
             headers[5] + " " * 2 + "|",
+
             color=(200, 138, 218, 255),  # Purple
             label="WIFI LIST",
             pos=(0, 58),
         )
     return
 
 
@@ -205,18 +197,22 @@
         if len(i[4]) < 3:
             i[4] += " " * signal_diff
         if len(i[5]) == 0:
             i[5] = "Open"
 
         print(f"{[i]}")
 
+        # print(i)
+        temp_list = []
+        temp_list.append(i)
+
         dpg.add_button(
             # tag=i[1],  # Causes issue on re-scan
             parent=129,
-            label=tabulate(
+            label=tabulate.tabulate(
                 [i],
                 stralign="left",
                 tablefmt="plain",
                 maxcolwidths=[
                     25,
                     None,
                     None,
```

### Comparing `mgtron-2.19.1/src/wifi/scanning.py` & `mgtron-2.19.2/src/wifi/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2html.py` & `mgtron-2.19.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2html4.py` & `mgtron-2.19.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2html5.py` & `mgtron-2.19.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2latex.py` & `mgtron-2.19.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2man.py` & `mgtron-2.19.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2odt.py` & `mgtron-2.19.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.19.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2pseudoxml.py` & `mgtron-2.19.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2s5.py` & `mgtron-2.19.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2xetex.py` & `mgtron-2.19.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rst2xml.py` & `mgtron-2.19.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.1/venv/bin/rstpep2html.py` & `mgtron-2.19.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

