# Comparing `tmp/gen3_util-0.0.2rc8.tar.gz` & `tmp/gen3_util-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc8.tar", last modified: Fri Jul  7 00:12:28 2023, max compression
+gzip compressed data, was "gen3_util-0.0.3rc1.tar", last modified: Mon Jul 10 18:40:18 2023, max compression
```

## Comparing `gen3_util-0.0.2rc8.tar` & `gen3_util-0.0.3rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.526396 gen3_util-0.0.2rc8/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc8/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     8535 2023-07-07 00:12:28.526097 gen3_util-0.0.2rc8/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     7850 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.491322 gen3_util-0.0.2rc8/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.2rc8/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.504439 gen3_util-0.0.2rc8/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:08:11.000000 gen3_util-0.0.2rc8/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.504777 gen3_util-0.0.2rc8/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.513570 gen3_util-0.0.2rc8/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc8/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.514270 gen3_util-0.0.2rc8/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc8/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.514706 gen3_util-0.0.2rc8/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:02:54.000000 gen3_util-0.0.2rc8/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.516560 gen3_util-0.0.2rc8/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.518264 gen3_util-0.0.2rc8/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12907 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.520153 gen3_util-0.0.2rc8/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    10101 2023-07-07 00:02:54.000000 gen3_util-0.0.2rc8/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3293 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.521392 gen3_util-0.0.2rc8/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.2rc8/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc8/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.499854 gen3_util-0.0.2rc8/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     8535 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-07 00:12:28.000000 gen3_util-0.0.2rc8/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-07 00:12:28.526458 gen3_util-0.0.2rc8/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-07-07 00:12:04.000000 gen3_util-0.0.2rc8/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.489219 gen3_util-0.0.2rc8/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.523177 gen3_util-0.0.2rc8/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:10:58.000000 gen3_util-0.0.2rc8/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.2rc8/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2443 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525204 gen3_util-0.0.2rc8/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525549 gen3_util-0.0.2rc8/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:12:28.525751 gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.2rc8/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc8/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2699 2023-07-07 00:01:20.000000 gen3_util-0.0.2rc8/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc8/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.511681 gen3_util-0.0.3rc1/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.3rc1/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8910 2023-07-10 18:40:18.511295 gen3_util-0.0.3rc1/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8225 2023-07-10 18:37:56.000000 gen3_util-0.0.3rc1/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.469457 gen3_util-0.0.3rc1/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.3rc1/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.474230 gen3_util-0.0.3rc1/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.474498 gen3_util-0.0.3rc1/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.490177 gen3_util-0.0.3rc1/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc1/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.491065 gen3_util-0.0.3rc1/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.3rc1/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.491494 gen3_util-0.0.3rc1/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.495969 gen3_util-0.0.3rc1/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.498147 gen3_util-0.0.3rc1/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12907 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.504241 gen3_util-0.0.3rc1/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11295 2023-07-10 18:31:58.000000 gen3_util-0.0.3rc1/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3293 2023-07-07 00:01:20.000000 gen3_util-0.0.3rc1/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.505824 gen3_util-0.0.3rc1/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.3rc1/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.3rc1/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.472679 gen3_util-0.0.3rc1/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8910 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-10 18:40:18.000000 gen3_util-0.0.3rc1/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-10 18:40:18.511764 gen3_util-0.0.3rc1/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5579 2023-07-10 18:33:57.000000 gen3_util-0.0.3rc1/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.465045 gen3_util-0.0.3rc1/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.508037 gen3_util-0.0.3rc1/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.3rc1/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2443 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510307 gen3_util-0.0.3rc1/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510561 gen3_util-0.0.3rc1/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-10 18:40:18.510794 gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.3rc1/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.3rc1/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.3rc1/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.3rc1/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc8/LICENSE` & `gen3_util-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/PKG-INFO` & `gen3_util-0.0.3rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.2rc8
+Version: 0.0.3rc1
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -29,19 +29,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.1
+msg: Version 0.0.3
 
 
 ```
 
+Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
+
+```text
+Requires libmagic installed on your system to determine mime-types
+Error: 'failed to find libmagic.  Check your installation'
+For installation instructions see https://github.com/ahupp/python-magic#installation
+```
+
+
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
 
@@ -166,23 +175,24 @@
 msg: Approve these requests to add linus.pauling@osu.edu to aced-MyExperiment
 commands:
 - gen3_util access update 293c6cd1-7ab7-420f-bafb-34319589eac4 SIGNED
 
 ```
 
 > Before proceeding, I need to sign those equests
+
 ```text
 gen3_util access update xxxxxx SIGNED
 ```
 
-```text
+
 
 > I want to create a simple project structure with a set of files
 
-```
+```text
 $ gen3_util meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-MyExperiment
 summary:
   ResearchStudy:
     count: 1
   DocumentReference:
     count: 5
     size: 6013814
```

### Comparing `gen3_util-0.0.2rc8/README.md` & `gen3_util-0.0.3rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.1
+msg: Version 0.0.3
 
 
 ```
 
+Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
+
+```text
+Requires libmagic installed on your system to determine mime-types
+Error: 'failed to find libmagic.  Check your installation'
+For installation instructions see https://github.com/ahupp/python-magic#installation
+```
+
+
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
 
@@ -146,23 +155,24 @@
 msg: Approve these requests to add linus.pauling@osu.edu to aced-MyExperiment
 commands:
 - gen3_util access update 293c6cd1-7ab7-420f-bafb-34319589eac4 SIGNED
 
 ```
 
 > Before proceeding, I need to sign those equests
+
 ```text
 gen3_util access update xxxxxx SIGNED
 ```
 
-```text
+
 
 > I want to create a simple project structure with a set of files
 
-```
+```text
 $ gen3_util meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-MyExperiment
 summary:
   ResearchStudy:
     count: 1
   DocumentReference:
     count: 5
     size: 6013814
```

### Comparing `gen3_util-0.0.2rc8/gen3_util/access/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/access/cli.py` & `gen3_util-0.0.3rc1/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/access/requestor.py` & `gen3_util-0.0.3rc1/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/buckets/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/buckets/cli.py` & `gen3_util-0.0.3rc1/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/cli/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/cli/cli.py` & `gen3_util-0.0.3rc1/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/common/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/config/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/files/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/files/cli.py` & `gen3_util-0.0.3rc1/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/files/downloader.py` & `gen3_util-0.0.3rc1/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/files/uploader.py` & `gen3_util-0.0.3rc1/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/meta/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/meta/cli.py` & `gen3_util-0.0.3rc1/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/meta/importer.py` & `gen3_util-0.0.3rc1/gen3_util/meta/importer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import sys
 import unicodedata
 import uuid
 from datetime import timezone, datetime
 import hashlib
 
-import magic
 import pathlib
 import click
 
 import orjson
 import mimetypes
 
 from gen3_util.cli import CLIOutput
@@ -19,14 +18,20 @@
 from gen3_util.meta import ACED_NAMESPACE
 
 from fhir.resources.identifier import Identifier
 from fhir.resources.patient import Patient
 from fhir.resources.specimen import Specimen
 from fhir.resources.resource import Resource
 
+try:
+    import magic
+except ImportError as e:
+    print(f"Requires libmagic installed on your system to determine file mime-types\nError: '{e}'\nFor installation instructions see https://github.com/ahupp/python-magic#installation")
+    sys.exit(1)
+
 PLUGINS = []
 PLUGINS_ADDED_TO_PATH = False
 
 logger = logging.getLogger(__name__)
 
 
 def create_research_study(name, description):
@@ -79,16 +84,16 @@
 @click.argument('input_path')
 @click.argument('output_path')
 @click.option('--project_id', required=True,
               default=None,
               show_default=True,
               help='Gen3 program-project'
               )
-@click.option('--remove_path_prefix', required=True,
-              default="/",
+@click.option('--remove_path_prefix',
+              default='',
               show_default=True,
               help='Remove prefix from file paths.  '
                    'Creates well-known form for achieving reproducible directories independent '
                    'of the directory the files were collected from.'
               )
 @click.option('--pattern',
               default='**/*',
@@ -117,20 +122,25 @@
         assert _.is_dir(), f"input_path {_} is not a directory."
 
     for _ in [output_path]:
         if not _.exists():
             print(f"output_path {_} does not exist, creating...")
             _.mkdir(parents=True, exist_ok=True)
 
-    _magic = magic.Magic(mime=True, uncompress=True)
+    _magic = magic.Magic(mime=True, uncompress=True)  # https://github.com/ahupp/python-magic#installation
     program, project = project_id.split('-')
     research_study = create_research_study(project, f"A study with files from {input_path}/{pattern}")
 
     # for user display/logs
-    counts = {'ResearchStudy': {'count': 1}, 'Patient': {'count': 0}, 'Specimen': {'count': 0}}
+    counts = {
+        'ResearchStudy': {'count': 1},
+        'ResearchSubject': {'count': 0},
+        'Patient': {'count': 0},
+        'Specimen': {'count': 0}
+    }
 
     with EmitterContextManager(output_path, file_mode="wb") as emitter:
         emitter.emit('ResearchStudy').write(
             orjson.dumps(research_study, orjson.OPT_APPEND_NEWLINE))
 
         count = 0
         size = 0
@@ -144,20 +154,35 @@
             if not mime:
                 mime = _magic.from_file(file)
 
             resources = _extract_fhir_resources(str(file).replace(remove_path_prefix, '', 1), input_path, plugin_path)
             subject_reference = f"ResearchStudy/{research_study['id']}"  # Who/what is the subject of the document
 
             for resource in resources:
+                if resource.id in already_seen:
+                    continue
 
                 if resource.resource_type == 'Patient':
                     subject_reference = f"Patient/{resource.id}"
-
-                if resource.id in already_seen:
-                    continue
+                    research_subject = {
+                        "id": str(uuid.uuid5(ACED_NAMESPACE, "ResearchSubject" + subject_reference)),
+                        "resourceType": "ResearchSubject",
+                        "status": "active",
+                        "study": {
+                            "reference": f"ResearchStudy/{research_study['id']}"
+                        },
+                        "subject": {
+                            "reference": subject_reference
+                        },
+
+                    }
+                    emitter.emit("ResearchSubject").write(
+                        orjson.dumps(research_subject, option=orjson.OPT_APPEND_NEWLINE)
+                    )
+                    counts["ResearchSubject"]['count'] += 1
 
                 already_seen.add(resource.id)
                 emitter.emit(resource.resource_type).write(
                     orjson.dumps(resource.dict(), option=orjson.OPT_APPEND_NEWLINE)
                 )
                 counts[resource.resource_type]['count'] += 1
 
@@ -237,31 +262,32 @@
         id_ = str(uuid.uuid5(ACED_NAMESPACE, f"{specimen_identifier.system}#{specimen_identifier.value}"))
         if id_ not in self.specimens:
             self.specimens[id_] = Specimen.parse_obj({'id': id_, 'identifier': [specimen_identifier], 'subject': {'reference': f"Patient/{patient_id}"}})
         return self.specimens[id_]
 
 
 def _discover_plugins(plugin_path: str) -> list[PathParser]:
-    """Discover plugins in ~/.gen3/plugins and ./plugins."""
+    """Discover plugins."""
     import importlib
     import pkgutil
     global PLUGINS_ADDED_TO_PATH
 
     if len(PLUGINS) > 0 or plugin_path is None:
         return PLUGINS
 
-    if not PLUGINS_ADDED_TO_PATH:
+    if not PLUGINS_ADDED_TO_PATH and pathlib.Path(plugin_path).exists():
         sys.path.append(plugin_path)
+        sys.path.append(str(pathlib.Path(plugin_path).parent))
         PLUGINS_ADDED_TO_PATH = True
 
     discovered_plugins = {
         name: importlib.import_module(name)
         for finder, name, is_pkg
         in pkgutil.iter_modules()
-        if name.startswith('gen3_util_plugin_')
+        if 'gen3_util_plugin_' in name and name in plugin_path
     }
 
     for name, pkg in discovered_plugins.items():
         for _, obj in inspect.getmembers(pkg):
             if inspect.isclass(obj) and issubclass(obj, PathParser) and obj.__module__ == name:
                 logger.debug(f'plugin {_}')
                 PLUGINS.append(obj())
```

### Comparing `gen3_util-0.0.2rc8/gen3_util/meta/uploader.py` & `gen3_util-0.0.3rc1/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/meta/validator.py` & `gen3_util-0.0.3rc1/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/projects/__init__.py` & `gen3_util-0.0.3rc1/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/projects/cli.py` & `gen3_util-0.0.3rc1/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/projects/creator.py` & `gen3_util-0.0.3rc1/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/projects/lister.py` & `gen3_util-0.0.3rc1/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util/projects/remover.py` & `gen3_util-0.0.3rc1/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.3rc1/gen3_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.2rc8
+Version: 0.0.3rc1
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -29,19 +29,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.1
+msg: Version 0.0.3
 
 
 ```
 
+Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
+
+```text
+Requires libmagic installed on your system to determine mime-types
+Error: 'failed to find libmagic.  Check your installation'
+For installation instructions see https://github.com/ahupp/python-magic#installation
+```
+
+
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
 
@@ -166,23 +175,24 @@
 msg: Approve these requests to add linus.pauling@osu.edu to aced-MyExperiment
 commands:
 - gen3_util access update 293c6cd1-7ab7-420f-bafb-34319589eac4 SIGNED
 
 ```
 
 > Before proceeding, I need to sign those equests
+
 ```text
 gen3_util access update xxxxxx SIGNED
 ```
 
-```text
+
 
 > I want to create a simple project structure with a set of files
 
-```
+```text
 $ gen3_util meta  import dir tests/fixtures/dir_to_study/ tmp/foo --project_id aced-MyExperiment
 summary:
   ResearchStudy:
     count: 1
   DocumentReference:
     count: 5
     size: 6013814
```

### Comparing `gen3_util-0.0.2rc8/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.3rc1/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/setup.py` & `gen3_util-0.0.3rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc8',  # Required
+    version='0.0.3rc1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc8/tests/integration/test_access.py` & `gen3_util-0.0.3rc1/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/integration/test_files.py` & `gen3_util-0.0.3rc1/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/integration/test_meta.py` & `gen3_util-0.0.3rc1/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/integration/test_project.py` & `gen3_util-0.0.3rc1/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/test_cli.py` & `gen3_util-0.0.3rc1/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.3rc1/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/test_config.py` & `gen3_util-0.0.3rc1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/test_files.py` & `gen3_util-0.0.3rc1/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc8/tests/unit/test_validate_directory.py` & `gen3_util-0.0.3rc1/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

