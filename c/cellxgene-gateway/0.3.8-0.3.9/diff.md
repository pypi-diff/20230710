# Comparing `tmp/cellxgene-gateway-0.3.8.tar.gz` & `tmp/cellxgene-gateway-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellxgene-gateway-0.3.8.tar", last modified: Tue Dec 21 17:37:12 2021, max compression
+gzip compressed data, was "dist/cellxgene-gateway-0.3.9.tar", last modified: Tue Mar 15 03:15:53 2022, max compression
```

## Comparing `cellxgene-gateway-0.3.8.tar` & `cellxgene-gateway-0.3.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/
--rw-r--r--   0 alokito   (1000) alokito   (1000)      213 2021-04-04 18:57:50.000000 cellxgene-gateway-0.3.8/.coveragerc
--rw-r--r--   0 alokito   (1000) alokito   (1000)       29 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/.flake8
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/.github/
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/.github/workflows/
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2374 2021-04-05 11:55:20.000000 cellxgene-gateway-0.3.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1747 2021-04-05 12:10:45.000000 cellxgene-gateway-0.3.8/.github/workflows/pr-checks.yaml
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1967 2021-04-04 14:07:20.000000 cellxgene-gateway-0.3.8/.gitignore
--rw-r--r--   0 alokito   (1000) alokito   (1000)      112 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/.isort.cfg
--rw-r--r--   0 alokito   (1000) alokito   (1000)      449 2021-07-18 13:39:36.000000 cellxgene-gateway-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1149 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/.travis.yml
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1193 2021-12-21 17:17:57.000000 cellxgene-gateway-0.3.8/Changelog.md
--rw-r--r--   0 alokito   (1000) alokito   (1000)    11345 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/LICENSE
--rw-r--r--   0 alokito   (1000) alokito   (1000)     8446 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/PKG-INFO
--rw-r--r--   0 alokito   (1000) alokito   (1000)     6665 2021-04-22 23:14:49.000000 cellxgene-gateway-0.3.8/README.md
--rw-r--r--   0 alokito   (1000) alokito   (1000)      363 2021-05-11 11:27:30.000000 cellxgene-gateway-0.3.8/SECURITY.md
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/
--rwxr-xr-x   0 alokito   (1000) alokito   (1000)      622 2021-12-21 17:19:02.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/__init__.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     3185 2021-05-08 17:17:15.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/backend_cache.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     6487 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/cache_entry.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     3067 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/cache_key.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)      787 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/cellxgene_exception.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1053 2021-04-23 11:00:24.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/dir_util.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     3096 2021-04-05 11:55:20.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/env.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1340 2021-04-22 23:00:22.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/extra_scripts.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2576 2021-12-21 17:04:22.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/filecrawl.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1173 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/flask_util.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     9744 2021-11-14 19:13:19.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/gateway.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-05 12:02:32.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/__init__.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-05 12:02:55.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/__init__.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1112 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/fileitem.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     6875 2021-11-14 19:01:20.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/fileitem_source.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1320 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/item.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1876 2021-11-14 19:00:31.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/item_source.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-05 12:02:49.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/__init__.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1017 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/s3item.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     6479 2021-11-14 19:01:40.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/s3item_source.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1146 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/process_exception.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1829 2021-07-12 23:14:15.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/prune_process_cache.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/css/
--rw-r--r--   0 alokito   (1000) alokito   (1000)      887 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/css/homepagestyle.css
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/js/
--rw-r--r--   0 alokito   (1000) alokito   (1000)      812 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/js/annotation.js
--rw-r--r--   0 alokito   (1000) alokito   (1000)    65106 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/static/nibr.ico
--rw-r--r--   0 alokito   (1000) alokito   (1000)     3328 2021-04-04 23:35:49.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/subprocess_backend.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/
--rw-r--r--   0 alokito   (1000) alokito   (1000)     3454 2021-11-14 22:17:33.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/cache_status.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1661 2021-04-04 11:59:41.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/cellxgene_error.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2011 2021-04-04 11:59:41.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/filecrawl.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2816 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/index.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2046 2021-04-04 11:59:41.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/loading.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2105 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/templates/process_error.html
--rw-r--r--   0 alokito   (1000) alokito   (1000)      744 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/cellxgene_gateway/util.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/
--rw-r--r--   0 alokito   (1000) alokito   (1000)     8446 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/PKG-INFO
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2103 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)        1 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)       70 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/entry_points.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)       83 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/requires.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)       18 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/top_level.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)      239 2021-07-18 13:59:24.000000 cellxgene-gateway-0.3.8/environment.yml
--rw-r--r--   0 alokito   (1000) alokito   (1000)       83 2021-07-18 13:56:22.000000 cellxgene-gateway-0.3.8/requirements.txt
--rw-r--r--   0 alokito   (1000) alokito   (1000)      206 2020-12-31 18:04:29.000000 cellxgene-gateway-0.3.8/run.sh.example
--rw-r--r--   0 alokito   (1000) alokito   (1000)       79 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/setup.cfg
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1916 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/setup.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/tests/
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/tests/items/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/tests/items/__init__.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/tests/items/file/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-04 11:59:51.000000 cellxgene-gateway-0.3.8/tests/items/file/__init__.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1618 2021-07-18 13:14:35.000000 cellxgene-gateway-0.3.8/tests/items/file/test_fileitem_source.py
-drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2021-12-21 17:37:12.000000 cellxgene-gateway-0.3.8/tests/items/s3/
--rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2021-04-22 23:00:22.000000 cellxgene-gateway-0.3.8/tests/items/s3/__init__.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     6199 2021-04-22 23:00:22.000000 cellxgene-gateway-0.3.8/tests/items/s3/test_s3item_source.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1216 2021-05-11 11:27:30.000000 cellxgene-gateway-0.3.8/tests/test_backend_cache.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2553 2021-04-04 14:23:26.000000 cellxgene-gateway-0.3.8/tests/test_cache_entry.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1247 2021-04-23 11:13:54.000000 cellxgene-gateway-0.3.8/tests/test_dir_util.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1382 2021-04-22 23:00:22.000000 cellxgene-gateway-0.3.8/tests/test_extra_scripts.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     2573 2021-12-21 17:03:12.000000 cellxgene-gateway-0.3.8/tests/test_filecrawl.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1568 2021-07-12 23:18:43.000000 cellxgene-gateway-0.3.8/tests/test_prune_process_cache.py
--rw-r--r--   0 alokito   (1000) alokito   (1000)     1838 2021-12-21 16:50:55.000000 cellxgene-gateway-0.3.8/tests/test_subprocess_backend.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      213 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.coveragerc
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       29 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.flake8
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/.github/
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/.github/workflows/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2374 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1863 2022-03-15 03:08:59.000000 cellxgene-gateway-0.3.9/.github/workflows/pr-checks.yaml
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1967 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.gitignore
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      112 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.isort.cfg
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      449 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1149 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/.travis.yml
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1261 2022-03-15 03:11:04.000000 cellxgene-gateway-0.3.9/Changelog.md
+-rw-r--r--   0 alokito   (1000) alokito   (1000)    11345 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/LICENSE
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     8634 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/PKG-INFO
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     6845 2022-03-15 03:08:59.000000 cellxgene-gateway-0.3.9/README.md
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      363 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/SECURITY.md
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      622 2022-03-15 03:11:26.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/__init__.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     3185 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/backend_cache.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     6487 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/cache_entry.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     3067 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/cache_key.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      787 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/cellxgene_exception.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1053 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/dir_util.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     3096 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/env.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1340 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/extra_scripts.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2576 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/filecrawl.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1173 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/flask_util.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     9672 2022-03-15 03:08:59.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/gateway.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/__init__.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/__init__.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1112 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/fileitem.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     6875 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/fileitem_source.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1320 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/item.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1876 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/item_source.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/__init__.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1017 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/s3item.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     7060 2022-03-15 03:08:59.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/s3item_source.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1146 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/process_exception.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1829 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/prune_process_cache.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/css/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      887 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/css/homepagestyle.css
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/js/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      812 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/js/annotation.js
+-rw-r--r--   0 alokito   (1000) alokito   (1000)    65106 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/static/nibr.ico
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     3328 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/subprocess_backend.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     3454 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/cache_status.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1661 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/cellxgene_error.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2011 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/filecrawl.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2816 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/index.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2046 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/loading.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2105 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/templates/process_error.html
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      744 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/cellxgene_gateway/util.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     8634 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2103 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        1 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       70 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       83 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/requires.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       18 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/top_level.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      239 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/environment.yml
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       83 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/requirements.txt
+-rw-r--r--   0 alokito   (1000) alokito   (1000)      206 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/run.sh.example
+-rw-r--r--   0 alokito   (1000) alokito   (1000)       79 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/setup.cfg
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1916 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/setup.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/tests/
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/tests/items/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/items/__init__.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/tests/items/file/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/items/file/__init__.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1618 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/items/file/test_fileitem_source.py
+drwxr-xr-x   0 alokito   (1000) alokito   (1000)        0 2022-03-15 03:15:53.000000 cellxgene-gateway-0.3.9/tests/items/s3/
+-rw-r--r--   0 alokito   (1000) alokito   (1000)        0 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/items/s3/__init__.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     6353 2022-03-15 03:08:59.000000 cellxgene-gateway-0.3.9/tests/items/s3/test_s3item_source.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1216 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_backend_cache.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2553 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_cache_entry.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1247 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_dir_util.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1382 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_extra_scripts.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     2573 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_filecrawl.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1568 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_prune_process_cache.py
+-rw-r--r--   0 alokito   (1000) alokito   (1000)     1813 2022-03-15 01:41:43.000000 cellxgene-gateway-0.3.9/tests/test_subprocess_backend.py
```

### Comparing `cellxgene-gateway-0.3.8/.github/workflows/codeql-analysis.yml` & `cellxgene-gateway-0.3.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/.github/workflows/pr-checks.yaml` & `cellxgene-gateway-0.3.9/.github/workflows/pr-checks.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
           conda-channels: "conda-forge"
 
       - name: Build environment
         run: |
           conda env create -f environment.yml
           eval "$(conda shell.bash hook)"
           conda activate cellxgene-gateway
+          pip install markupsafe==2.0.1 # temporary workaround for jinja2-2.11.3 calling soft_unicode in markupsafe
           python setup.py install
 
       - name: Run tests
         run: |
           eval "$(conda shell.bash hook)"
           conda activate cellxgene-gateway
           coverage run -m unittest discover tests
```

### Comparing `cellxgene-gateway-0.3.8/.gitignore` & `cellxgene-gateway-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/.travis.yml` & `cellxgene-gateway-0.3.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/Changelog.md` & `cellxgene-gateway-0.3.9/Changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 0.3.9
+
+* Added S3_ENABLE_LISTINGS_CACHE variable (See README.md)
+
 # 0.3.8
 
 * Fixed bug #57 affecting deeply nested subdirectory listing
 
 # 0.3.7
 
 * added back /metadata/ip_address endpoint
```

### Comparing `cellxgene-gateway-0.3.8/LICENSE` & `cellxgene-gateway-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/PKG-INFO` & `cellxgene-gateway-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-gateway
-Version: 0.3.8
+Version: 0.3.9
 Summary: Cellxgene Gateway
 Home-page: http://github.com/Novartis/cellxgene-gateway
 Author: Niket Patel, Yohann Potier, Alok Saldanha
 Author-email: alok.saldanha@novartis.com
 License: MIT
 Description: # Overview
         
@@ -80,14 +80,15 @@
         * `EXTERNAL_HOST` - the hostname and port from the perspective of the web browser, typically `localhost:5005` if running locally. Defaults to "localhost:{GATEWAY_PORT}"
         * `EXTERNAL_PROTOCOL` - typically http when running locally, can be https when deployed if the gateway is behind a load balancer or reverse proxy that performs https termination. Default value "http"
         * `GATEWAY_IP` - ip addess of instance gateway is running on, mostly used to display SSH instructions. Defaults to `socket.gethostbyname(socket.gethostname())`
         * `GATEWAY_PORT` - local port that the gateway should bind to, defaults to 5005
         * `GATEWAY_EXTRA_SCRIPTS` - JSON array of script paths, will be embedded into each page and forwarded with `--scripts` to cellxgene server
         * `GATEWAY_ENABLE_ANNOTATIONS` - Set to `true` or to `1` to enable cellxgene annotations. 
         * `GATEWAY_ENABLE_BACKED_MODE` - Set to `true` or to `1` to load AnnData in file-backed mode. This saves memory and speeds up launch time but may reduce overall performance.
+        * `S3_ENABLE_LISTINGS_CACHE` - Set to `true` or to `1` to cache listings of S3 folders for performance. Can be overridden by setting `filecrawl.html?refresh=true` query parameter.
         
         If any of the following optional variables are set, [ProxyFix](https://werkzeug.palletsprojects.com/en/1.0.x/middleware/proxy_fix/) will be used.
         * `PROXY_FIX_FOR` - Number of upstream proxies setting X-Forwarded-For
         * `PROXY_FIX_PROTO` - Number of upstream proxies setting X-Forwarded-Proto
         * `PROXY_FIX_HOST` - Number of upstream proxies setting X-Forwarded-Host
         * `PROXY_FIX_PORT` - Number of upstream proxies setting X-Forwarded-Port
         * `PROXY_FIX_PREFIX` - Number of upstream proxies setting X-Forwarded-Prefix
```

### Comparing `cellxgene-gateway-0.3.8/README.md` & `cellxgene-gateway-0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 * `EXTERNAL_HOST` - the hostname and port from the perspective of the web browser, typically `localhost:5005` if running locally. Defaults to "localhost:{GATEWAY_PORT}"
 * `EXTERNAL_PROTOCOL` - typically http when running locally, can be https when deployed if the gateway is behind a load balancer or reverse proxy that performs https termination. Default value "http"
 * `GATEWAY_IP` - ip addess of instance gateway is running on, mostly used to display SSH instructions. Defaults to `socket.gethostbyname(socket.gethostname())`
 * `GATEWAY_PORT` - local port that the gateway should bind to, defaults to 5005
 * `GATEWAY_EXTRA_SCRIPTS` - JSON array of script paths, will be embedded into each page and forwarded with `--scripts` to cellxgene server
 * `GATEWAY_ENABLE_ANNOTATIONS` - Set to `true` or to `1` to enable cellxgene annotations. 
 * `GATEWAY_ENABLE_BACKED_MODE` - Set to `true` or to `1` to load AnnData in file-backed mode. This saves memory and speeds up launch time but may reduce overall performance.
+* `S3_ENABLE_LISTINGS_CACHE` - Set to `true` or to `1` to cache listings of S3 folders for performance. Can be overridden by setting `filecrawl.html?refresh=true` query parameter.
 
 If any of the following optional variables are set, [ProxyFix](https://werkzeug.palletsprojects.com/en/1.0.x/middleware/proxy_fix/) will be used.
 * `PROXY_FIX_FOR` - Number of upstream proxies setting X-Forwarded-For
 * `PROXY_FIX_PROTO` - Number of upstream proxies setting X-Forwarded-Proto
 * `PROXY_FIX_HOST` - Number of upstream proxies setting X-Forwarded-Host
 * `PROXY_FIX_PORT` - Number of upstream proxies setting X-Forwarded-Port
 * `PROXY_FIX_PREFIX` - Number of upstream proxies setting X-Forwarded-Prefix
```

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/__init__.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 # this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0. Unless
 # required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, either express or implied. See the License for
 # the specific language governing permissions and limitations under the License.
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/backend_cache.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/backend_cache.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/cache_entry.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/cache_entry.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/cache_key.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/cache_key.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/cellxgene_exception.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/cellxgene_exception.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/dir_util.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/dir_util.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/env.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/env.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/extra_scripts.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/extra_scripts.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/filecrawl.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/filecrawl.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/flask_util.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/flask_util.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/gateway.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     make_response,
     redirect,
     render_template,
     request,
     send_from_directory,
     url_for,
 )
-from flask_api import status
 from werkzeug.middleware.proxy_fix import ProxyFix
-from werkzeug.utils import secure_filename
 
 from cellxgene_gateway import env, flask_util
 from cellxgene_gateway.backend_cache import BackendCache
 from cellxgene_gateway.cache_entry import CacheEntryStatus
 from cellxgene_gateway.cache_key import CacheKey
 from cellxgene_gateway.cellxgene_exception import CellxgeneException
 from cellxgene_gateway.extra_scripts import get_extra_scripts
```

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/fileitem.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/fileitem.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/file/fileitem_source.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/file/fileitem_source.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/item.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/item.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/item_source.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/item_source.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/s3item.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/s3item.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/items/s3/s3item_source.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/items/s3/s3item_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,45 @@
 # this file except in compliance with the License. You may obtain a copy
 # of the License at http://www.apache.org/licenses/LICENSE-2.0. Unless
 # required by applicable law or agreed to in writing, software distributed
 # under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, either express or implied. See the License for
 # the specific language governing permissions and limitations under the License.
 
-from os.path import basename, dirname, join
+import os
+from os.path import basename, dirname
 from typing import List
 
+import flask
 import s3fs
 
 from cellxgene_gateway import dir_util
 from cellxgene_gateway.items.item import ItemTree, ItemType
 from cellxgene_gateway.items.item_source import ItemSource, LookupResult
 from cellxgene_gateway.items.s3.s3item import S3Item
 
 
+def truthy(val: str):
+    return val.lower() in ["true", "1"]
+
+
 class S3ItemSource(ItemSource):
     def __init__(
         self,
         bucket,
         name=None,
         h5ad_suffix=dir_util.h5ad_suffix,
         annotation_dir_suffix=dir_util.annotations_suffix,
         annotation_file_suffix=".csv",
     ):
         self._name = name
-        self.s3 = s3fs.S3FileSystem()
+        enable_cache = os.environ.get("S3_ENABLE_LISTINGS_CACHE", "false").lower()
+        assert enable_cache in ["0", "1", "false", "true"]
+        self.use_listings_cache = truthy(enable_cache)
+        self.s3 = s3fs.S3FileSystem(use_listings_cache=self.use_listings_cache)
         if bucket.startswith("s3://"):
             raise Exception(
                 f"Bucket name should not include s3:// prefix, got {bucket}"
             )
         self.bucket = bucket
         self.h5ad_suffix = h5ad_suffix
         self.annotation_dir_suffix = annotation_dir_suffix
@@ -63,23 +72,30 @@
     def get_annotations_subpath(self, item) -> str:
         return self.convert_h5ad_key_to_annotation(item.descriptor)
 
     def list_items(self, filter: str = None) -> ItemTree:
         item_tree = self.scan_directory("" if filter is None else filter)
         return item_tree
 
+    @property
+    def refresh(self):
+        return (
+            truthy(flask.request.args.get("refresh", default="false"))
+            or not self.use_listings_cache
+        )
+
     def scan_directory(self, directory_key="") -> dict:
         url = self.url(directory_key)
 
         if not self.s3.exists(url):
             raise Exception(f"S3 url '{url}' does not exist.")
 
         s3key_map = dict(
             (self.remove_bucket(filepath), "s3://" + filepath)
-            for filepath in sorted(self.s3.ls(url))
+            for filepath in sorted(self.s3.ls(url, refresh=self.refresh))
         )
 
         def is_annotation_dir(dir_s3key):
             return (
                 dir_s3key.endswith(self.annotation_dir_suffix)
                 and self.convert_annotation_key_to_h5ad(dir_s3key) in h5ad_keys
             )
@@ -162,13 +178,15 @@
         annotations_subpath = self.get_annotations_subpath(item)
         annotations_fullpath = self.url(annotations_subpath)
         if self.s3.isdir(annotations_fullpath):
             return [
                 self.make_s3item_from_key(
                     basename(annotation), self.remove_bucket(annotation), True
                 )
-                for annotation in sorted(self.s3.ls(annotations_fullpath))
+                for annotation in sorted(
+                    self.s3.ls(annotations_fullpath, refresh=self.refresh)
+                )
                 if annotation.endswith(self.annotation_file_suffix)
                 and self.s3.isfile("s3://" + annotation)
             ]
         else:
             return None
```

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/process_exception.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/process_exception.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/prune_process_cache.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/prune_process_cache.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/static/css/homepagestyle.css` & `cellxgene-gateway-0.3.9/cellxgene_gateway/static/css/homepagestyle.css`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/static/js/annotation.js` & `cellxgene-gateway-0.3.9/cellxgene_gateway/static/js/annotation.js`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/static/nibr.ico` & `cellxgene-gateway-0.3.9/cellxgene_gateway/static/nibr.ico`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/subprocess_backend.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/subprocess_backend.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/cache_status.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/cache_status.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/cellxgene_error.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/cellxgene_error.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/filecrawl.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/filecrawl.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/index.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/index.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/loading.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/loading.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/templates/process_error.html` & `cellxgene-gateway-0.3.9/cellxgene_gateway/templates/process_error.html`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway/util.py` & `cellxgene-gateway-0.3.9/cellxgene_gateway/util.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/PKG-INFO` & `cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-gateway
-Version: 0.3.8
+Version: 0.3.9
 Summary: Cellxgene Gateway
 Home-page: http://github.com/Novartis/cellxgene-gateway
 Author: Niket Patel, Yohann Potier, Alok Saldanha
 Author-email: alok.saldanha@novartis.com
 License: MIT
 Description: # Overview
         
@@ -80,14 +80,15 @@
         * `EXTERNAL_HOST` - the hostname and port from the perspective of the web browser, typically `localhost:5005` if running locally. Defaults to "localhost:{GATEWAY_PORT}"
         * `EXTERNAL_PROTOCOL` - typically http when running locally, can be https when deployed if the gateway is behind a load balancer or reverse proxy that performs https termination. Default value "http"
         * `GATEWAY_IP` - ip addess of instance gateway is running on, mostly used to display SSH instructions. Defaults to `socket.gethostbyname(socket.gethostname())`
         * `GATEWAY_PORT` - local port that the gateway should bind to, defaults to 5005
         * `GATEWAY_EXTRA_SCRIPTS` - JSON array of script paths, will be embedded into each page and forwarded with `--scripts` to cellxgene server
         * `GATEWAY_ENABLE_ANNOTATIONS` - Set to `true` or to `1` to enable cellxgene annotations. 
         * `GATEWAY_ENABLE_BACKED_MODE` - Set to `true` or to `1` to load AnnData in file-backed mode. This saves memory and speeds up launch time but may reduce overall performance.
+        * `S3_ENABLE_LISTINGS_CACHE` - Set to `true` or to `1` to cache listings of S3 folders for performance. Can be overridden by setting `filecrawl.html?refresh=true` query parameter.
         
         If any of the following optional variables are set, [ProxyFix](https://werkzeug.palletsprojects.com/en/1.0.x/middleware/proxy_fix/) will be used.
         * `PROXY_FIX_FOR` - Number of upstream proxies setting X-Forwarded-For
         * `PROXY_FIX_PROTO` - Number of upstream proxies setting X-Forwarded-Proto
         * `PROXY_FIX_HOST` - Number of upstream proxies setting X-Forwarded-Host
         * `PROXY_FIX_PORT` - Number of upstream proxies setting X-Forwarded-Port
         * `PROXY_FIX_PREFIX` - Number of upstream proxies setting X-Forwarded-Prefix
```

### Comparing `cellxgene-gateway-0.3.8/cellxgene_gateway.egg-info/SOURCES.txt` & `cellxgene-gateway-0.3.9/cellxgene_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/setup.py` & `cellxgene-gateway-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/items/file/test_fileitem_source.py` & `cellxgene-gateway-0.3.9/tests/items/file/test_fileitem_source.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/items/s3/test_s3item_source.py` & `cellxgene-gateway-0.3.9/tests/items/s3/test_s3item_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,33 @@
             source.scan_directory()
         self.assertEqual(
             "S3 url 's3://my-bucket/' does not exist.",
             str(context.exception),
         )
 
     @patch("s3fs.S3FileSystem")
-    def test__GIVEN_multilevel_bucket_THEN_properly_recurses_suburls(self, s3func):
+    @patch("flask.request")
+    def test__GIVEN_multilevel_bucket_THEN_properly_recurses_suburls(
+        self, requestMock, s3func
+    ):
         class S3Mock:
             def exists(path):
                 if path in [
                     "s3://my-bucket/",
                     "s3://my-bucket/pbmc3k.h5ad",
                     "s3://my-bucket/lvl1",
                     "s3://my-bucket/lvl1/pbmc3k_l1.h5ad",
                     "s3://my-bucket/lvl1/lvl2",
                     "s3://my-bucket/lvl1/lvl2/pbmc3k_l2.h5ad",
                 ]:
                     return True
                 raise Exception("exists called with " + path)
 
-            def ls(path):
+            def ls(path, refresh):
+                assert refresh == True
                 if path == "s3://my-bucket/":
                     return [
                         "my-bucket/lvl1",
                         "my-bucket/pbmc3k.h5ad",
                         "my-bucket/pbmc3k_annotations",
                     ]
                 elif path == "s3://my-bucket/pbmc3k_annotations":
@@ -75,14 +79,15 @@
                 if path in ["s3://my-bucket/pbmc3k_annotations/annot.csv"]:
                     return True
                 if path in ["s3://my-bucket/pbmc3k_annotations"]:
                     return False
                 raise Exception("isfile called with " + path)
 
         s3func.return_value = S3Mock
+        requestMock.args.get.return_value = "true"
         source = S3ItemSource("my-bucket")
         tree = source.scan_directory()
 
         def s3item_compare(i1, i2, msg=""):
             self.assertEqual(i1.name, i2.name, "name equals")
             self.assertEqual(i1.type, i2.type, "type equals")
             self.assertEqual(i1.s3key, i2.s3key, "s3key equals")
```

### Comparing `cellxgene-gateway-0.3.8/tests/test_backend_cache.py` & `cellxgene-gateway-0.3.9/tests/test_backend_cache.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_cache_entry.py` & `cellxgene-gateway-0.3.9/tests/test_cache_entry.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_dir_util.py` & `cellxgene-gateway-0.3.9/tests/test_dir_util.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_extra_scripts.py` & `cellxgene-gateway-0.3.9/tests/test_extra_scripts.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_filecrawl.py` & `cellxgene-gateway-0.3.9/tests/test_filecrawl.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_prune_process_cache.py` & `cellxgene-gateway-0.3.9/tests/test_prune_process_cache.py`

 * *Files identical despite different names*

### Comparing `cellxgene-gateway-0.3.8/tests/test_subprocess_backend.py` & `cellxgene-gateway-0.3.9/tests/test_subprocess_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         cellxgene_loc = "/some/cellxgene"
         scripts = ["http://example.com/script.js", "http://example.com/script2.js"]
 
         with self.assertRaises(ProcessException) as context:
             backend.launch(cellxgene_loc, scripts, entry)
         popen.assert_called_once_with(
             [
-                "yes | /some/cellxgene launch /tmp/czi/pbmc3k.h5ad --port 8000 --host 127.0.0.1 --disable-annotations --disable-gene-sets-save --scripts http://example.com/script.js --scripts http://example.com/script2.js"
+                "yes | /some/cellxgene launch /tmp/czi/pbmc3k.h5ad --port 8000 --host 127.0.0.1 --disable-annotations --scripts http://example.com/script.js --scripts http://example.com/script2.js"
             ],
             shell=True,
             stderr=-1,
             stdout=-1,
         )
         self.assertEqual("An unexpected error", context.exception.stderr)
```

