# Comparing `tmp/edc-0.5.2.tar.gz` & `tmp/edc-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.2.tar", last modified: Wed Jul  5 01:03:18 2023, max compression
+gzip compressed data, was "edc-0.5.3.tar", last modified: Mon Jul 10 16:49:51 2023, max compression
```

## Comparing `edc-0.5.2.tar` & `edc-0.5.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.162206 edc-0.5.2/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.2/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.2/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.2/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    41042 2023-07-05 01:03:10.000000 edc-0.5.2/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.2/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.2/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-05 01:03:18.162322 edc-0.5.2/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.2/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.149248 edc-0.5.2/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.152131 edc-0.5.2/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.152788 edc-0.5.2/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.2/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.2/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.2/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.2/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.153867 edc-0.5.2/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.157894 edc-0.5.2/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.2/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.2/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.2/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.2/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.2/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.2/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.2/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.2/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.2/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.2/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.2/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.2/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.2/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.2/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.2/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.2/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.2/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.2/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.2/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.158749 edc-0.5.2/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.2/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.158865 edc-0.5.2/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.2/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.2/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.161656 edc-0.5.2/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.2/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.2/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.2/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.2/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.2/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.2/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.2/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.2/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.2/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.2/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.2/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2987 2023-07-05 01:03:18.162722 edc-0.5.2/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.161974 edc-0.5.2/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.2/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.2/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.087087 edc-0.5.3/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.3/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.3/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.3/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    42121 2023-07-10 16:49:43.000000 edc-0.5.3/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.3/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.3/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-10 16:49:51.087195 edc-0.5.3/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.3/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.073694 edc-0.5.3/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.076619 edc-0.5.3/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.3/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.3/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.3/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.077309 edc-0.5.3/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.3/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.3/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.3/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.3/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.078541 edc-0.5.3/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.3/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.082678 edc-0.5.3/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.3/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.3/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.3/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.3/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.3/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.3/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.3/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.3/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.3/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.3/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.3/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.3/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.3/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.3/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.3/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.3/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.3/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.3/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.3/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.083736 edc-0.5.3/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-10 16:49:51.000000 edc-0.5.3/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-10 16:49:51.000000 edc-0.5.3/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-10 16:49:51.000000 edc-0.5.3/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.3/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-10 16:49:51.000000 edc-0.5.3/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-10 16:49:51.000000 edc-0.5.3/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.083865 edc-0.5.3/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.3/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.3/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.086593 edc-0.5.3/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.3/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.3/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.3/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.3/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.3/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.3/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.3/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.3/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.3/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.3/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.3/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2987 2023-07-10 16:49:51.087560 edc-0.5.3/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-10 16:49:51.086881 edc-0.5.3/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.3/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.3/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.2/.gitignore` & `edc-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/.pre-commit-config.yaml` & `edc-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/CHANGES` & `edc-0.5.3/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 Changes
 -------
 
+0.5.4
+-----
+- Add 'By country' list filter and group permitted sites by country
+  (edc-auth)
+- set default manager to `objects` using BaseUuidModel (edc-model)
+- add additional validation to protect site id on models and other
+  actions (edc-site)
+- validate site when creating actions (edc-action)
+- validate site when creating appointments (edc-appointment)
+- add attrs to allow lower bound to extend with gap days
+  (edc-appointment)
+- refactor MetadataRefresher, MetadateGetter and management command;
+  Add custom modeladmin classes and forms; change naming to
+  "Data collection status" (edc-metadata)
+- hide delete button on condition; refactor dashboard button method;
+  show/hide history object tool;custom change form title.
+  (edc-model-admin)
+ - link changelist to subject_dashboard; refactor ReferenceGetter to
+   respect site. Customize ModelAdmin class. (edc-reference)
+ - add link to edc_metadata from dashboard (edc-subject-dashboard)
+
+0.5.3
+-----
+- accept FieldError on get_queryset if using SiteModelAdminMixin for model
+  without field `site`. (edc-sites)
+
 0.5.2
 -----
 - force all models to use `objects` as default manager (edc-model)
 - add new mixins to handle redirects, delete button (edc-model-admin)
 - update admin mixin to handle fks/m2ms in modelform (edc-site)
 - move managers from fields mixin to screening_model_mixin (edc-screening)
 
 
 0.5.1
 ------
-- add additonal validation to check screening identifier and the screening
-  eligibility boolean. (edc-cosent)
+- add additional validation to check screening identifier and the screening
+  eligibility boolean. (edc-consent)
 - add mixin to redirect all forms to a selected changelist (edc-model-admin)
 - improve redirect on delete (edc-model-admin)
 
 
 
 0.4.99
 ------
```

### Comparing `edc-0.5.2/LICENSE` & `edc-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/PKG-INFO` & `edc-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.2
+Version: 0.5.3
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.2/README.rst` & `edc-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/nginx/edc-uat.conf` & `edc-0.5.3/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/nginx/edc.conf` & `edc-0.5.3/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/scripts/dev_repos.sh` & `edc-0.5.3/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/scripts/update_edc.sh` & `edc-0.5.3/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/systemd/celery-uat.service` & `edc-0.5.3/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/bin/systemd/celery.service` & `edc-0.5.3/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/Makefile` & `edc-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/README.rst` & `edc-0.5.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/backup.rst` & `edc-0.5.3/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/celery.rst` & `edc-0.5.3/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/conda.rst` & `edc-0.5.3/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/conf.py` & `edc-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/configure_web_services.rst` & `edc-0.5.3/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/deploy_new_droplet.rst` & `edc-0.5.3/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/exporting_encrypted_data.rst` & `edc-0.5.3/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/forms_reference.md` & `edc-0.5.3/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/landing_page.rst` & `edc-0.5.3/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/make.bat` & `edc-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/prepare_database.rst` & `edc-0.5.3/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/printing.rst` & `edc-0.5.3/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/docs/update_deployment.rst` & `edc-0.5.3/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/edc.egg-info/PKG-INFO` & `edc-0.5.3/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.2
+Version: 0.5.3
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.2/edc.egg-info/SOURCES.txt` & `edc-0.5.3/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/edc.egg-info/requires.txt` & `edc-0.5.3/edc.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,77 +18,77 @@
 django-extensions
 django-logentry-admin
 django-multisite-edc==2.0.0
 django-revision==0.3.6
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
-edc-action-item==0.3.52
+edc-action-item==0.3.53
 edc-adherence==0.1.21
-edc-adverse-event==0.3.54
-edc-appointment==0.3.73
-edc-auth==0.3.61
+edc-adverse-event==0.3.55
+edc-appointment==0.3.74
+edc-auth==0.3.63
 edc-consent==0.3.46
 edc-constants==0.3.49
-edc-crf==0.3.43
+edc-crf==0.3.44
 edc-dashboard==0.3.45
-edc-data-manager==0.3.54
+edc-data-manager==0.3.55
 edc-device==0.3.11
 edc-document-status==0.1.4
-edc-dx==0.1.19
+edc-dx==0.1.20
 edc-dx-review==0.1.39
 edc-egfr==0.1.11
-edc-export==0.3.26
+edc-export==0.3.27
 edc-facility==0.3.15
 edc-fieldsets==0.3.13
-edc-form-describer==0.3.14
+edc-form-describer==0.3.16
 edc-form-label==0.3.9
 edc-form-validators==0.3.34
 edc-glucose==0.1.30
 edc-he==0.1.8
-edc-identifier==0.3.23
-edc-lab==0.3.43
+edc-identifier==0.3.24
+edc-lab==0.3.44
 edc-lab-dashboard==0.3.11
 edc-lab-panel==0.1.15
 edc-lab-results==0.1.38
-edc-label==0.3.12
+edc-label==0.3.13
 edc-list-data==0.3.18
-edc-listboard==0.1.10
-edc-locator==0.3.23
-edc-ltfu==0.3.23
-edc-metadata==0.3.52
-edc-mnsi==0.1.16
+edc-listboard==0.1.11
+edc-locator==0.3.24
+edc-ltfu==0.3.24
+edc-metadata==0.3.53
+edc-mnsi==0.1.17
 edc-model==0.3.31
-edc-model-admin==0.3.46
+edc-model-admin==0.3.47
 edc-model-fields==0.3.7
 edc-model-form==0.1.12
 edc-model-wrapper==0.3.10
 edc-navbar==0.3.16
-edc-notification==0.3.17
-edc-offstudy==0.3.32
+edc-notification==0.3.18
+edc-offstudy==0.3.33
 edc-pdf-reports==0.3.13
 edc-pdutils==0.3.22
-edc-pharmacy==0.1.38
+edc-pharmacy==0.1.39
 edc-pharmacy-dashboard==0.1.3
 edc-prn==0.3.13
 edc-protocol==0.3.9
-edc-protocol-incident==0.1.25
-edc-qol==0.1.14
-edc-randomization==0.3.46
-edc-reference==0.3.15
-edc-refusal==0.1.12
-edc-registration==0.3.29
+edc-protocol-incident==0.1.26
+edc-qol==0.1.15
+edc-randomization==0.3.47
+edc-reference==0.3.16
+edc-refusal==0.1.13
+edc-registration==0.3.30
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
 edc-rx==0.1.6
 edc-screening==0.3.35
 edc-search==0.3.7
-edc-sites==0.3.21
-edc-subject-dashboard==0.3.36
+edc-sites==0.3.23
+edc-subject-dashboard==0.3.37
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
-edc-unblinding==0.1.14
+edc-unblinding==0.1.15
 edc-utils==0.3.20
-edc-visit-schedule==0.3.61
-edc-visit-tracking==0.3.52
+edc-visit-schedule==0.3.62
+edc-visit-tracking==0.3.53
 edc-vitals==0.1.11
```

### Comparing `edc-0.5.2/image/icon-pycharm.png` & `edc-0.5.3/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/requirements.tests/edc.txt` & `edc-0.5.3/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/requirements.tests/edc_dev.txt` & `edc-0.5.3/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.2/setup.cfg` & `edc-0.5.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -47,83 +47,83 @@
 	django-extensions
 	django-logentry-admin
 	django-multisite-edc==2.0.0
 	django-revision==0.3.6
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
-	edc-action-item==0.3.52
+	edc-action-item==0.3.53
 	edc-adherence==0.1.21
-	edc-adverse-event==0.3.54
-	edc-appointment==0.3.73
-	edc-auth==0.3.61
+	edc-adverse-event==0.3.55
+	edc-appointment==0.3.74
+	edc-auth==0.3.63
 	edc-consent==0.3.46
 	edc-constants==0.3.49
-	edc-crf==0.3.43
+	edc-crf==0.3.44
 	edc-dashboard==0.3.45
-	edc-data-manager==0.3.54
+	edc-data-manager==0.3.55
 	edc-device==0.3.11
 	edc-document-status==0.1.4
-	edc-dx==0.1.19
+	edc-dx==0.1.20
 	edc-dx-review==0.1.39
 	edc-egfr==0.1.11
-	edc-export==0.3.26
+	edc-export==0.3.27
 	edc-facility==0.3.15
 	edc-fieldsets==0.3.13
-	edc-form-describer==0.3.14
+	edc-form-describer==0.3.16
 	edc-form-label==0.3.9
 	edc-form-validators==0.3.34
 	edc-glucose==0.1.30
 	edc-he==0.1.8
-	edc-identifier==0.3.23
-	edc-lab==0.3.43
+	edc-identifier==0.3.24
+	edc-lab==0.3.44
 	edc-lab-dashboard==0.3.11
 	edc-lab-panel==0.1.15
 	edc-lab-results==0.1.38
-	edc-label==0.3.12
+	edc-label==0.3.13
 	edc-list-data==0.3.18
-	edc-listboard==0.1.10
-	edc-locator==0.3.23
-	edc-ltfu==0.3.23
-	edc-metadata==0.3.52
-	edc-mnsi==0.1.16
+	edc-listboard==0.1.11
+	edc-locator==0.3.24
+	edc-ltfu==0.3.24
+	edc-metadata==0.3.53
+	edc-mnsi==0.1.17
 	edc-model==0.3.31
-	edc-model-admin==0.3.46
+	edc-model-admin==0.3.47
 	edc-model-fields==0.3.7
 	edc-model-form==0.1.12
 	edc-model-wrapper==0.3.10
 	edc-navbar==0.3.16
-	edc-notification==0.3.17
-	edc-offstudy==0.3.32
+	edc-notification==0.3.18
+	edc-offstudy==0.3.33
 	edc-pdf-reports==0.3.13
 	edc-pdutils==0.3.22
-	edc-pharmacy==0.1.38
+	edc-pharmacy==0.1.39
 	edc-pharmacy-dashboard==0.1.3
 	edc-prn==0.3.13
 	edc-protocol==0.3.9
-	edc-protocol-incident==0.1.25
-	edc-qol==0.1.14
-	edc-randomization==0.3.46
-	edc-reference==0.3.15
-	edc-refusal==0.1.12
-	edc-registration==0.3.29
+	edc-protocol-incident==0.1.26
+	edc-qol==0.1.15
+	edc-randomization==0.3.47
+	edc-reference==0.3.16
+	edc-refusal==0.1.13
+	edc-registration==0.3.30
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
 	edc-rx==0.1.6
 	edc-screening==0.3.35
 	edc-search==0.3.7
-	edc-sites==0.3.21
-	edc-subject-dashboard==0.3.36
+	edc-sites==0.3.23
+	edc-subject-dashboard==0.3.37
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
-	edc-unblinding==0.1.14
+	edc-unblinding==0.1.15
 	edc-utils==0.3.20
-	edc-visit-schedule==0.3.61
-	edc-visit-tracking==0.3.52
+	edc-visit-schedule==0.3.62
+	edc-visit-tracking==0.3.53
 	edc-vitals==0.1.11
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
```

### Comparing `edc-0.5.2/utils/get_edc_requirements.py` & `edc-0.5.3/utils/get_edc_requirements.py`

 * *Files identical despite different names*

