# Comparing `tmp/audiobook-dl-0.6.0.tar.gz` & `tmp/audiobook-dl-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-dl-0.6.0.tar", last modified: Sun Jul  9 17:36:37 2023, max compression
+gzip compressed data, was "audiobook-dl-0.6.1.tar", last modified: Mon Jul 10 20:02:46 2023, max compression
```

## Comparing `audiobook-dl-0.6.0.tar` & `audiobook-dl-0.6.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.098743 audiobook-dl-0.6.0/.github/
--rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/FUNDING.yml
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.098743 audiobook-dl-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.099743 audiobook-dl-0.6.0/.github/workflows/
--rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.github/workflows/pytest.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/.gitignore
--rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/LICENSE
--rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     4798 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/README.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.102743 audiobook-dl-0.6.0/audiobook_dl.egg-info/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     2311 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/SOURCES.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/dependency_links.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       58 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/entry_points.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       88 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/requires.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-07-09 17:36:37.000000 audiobook-dl-0.6.0/audiobook_dl.egg-info/top_level.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.104743 audiobook-dl-0.6.0/audiobookdl/
--rw-r--r--   0 jo1gi     (1000) users      (100)      191 2023-07-09 17:33:15.000000 audiobook-dl-0.6.0/audiobookdl/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5968 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/__main__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3495 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/args.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.105743 audiobook-dl-0.6.0/audiobookdl/assets/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.110743 audiobook-dl-0.6.0/audiobookdl/assets/errors/
--rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/book_access.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/chapters_add.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       56 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/config_not_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/data_not_present.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/failed_combining.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/missing_dependency.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/no_files_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/no_source_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/request_error.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/errors/user_not_authorized.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/ffmpeg_chapter_template.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/assets/simple_help.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.092743 audiobook-dl-0.6.0/audiobookdl/assets/sources/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.113743 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1010 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/book_info.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      108 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/files.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      270 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/login.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      185 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      866 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast_episodes.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)     1983 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/config.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1342 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/exceptions.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1407 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/logging.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.115743 audiobook-dl-0.6.0/audiobookdl/output/
--rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     8073 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/download.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/encryption.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.117743 audiobook-dl-0.6.0/audiobookdl/output/metadata/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1363 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1524 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/ffmpeg.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2391 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/id3.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/output/metadata/mp4.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3473 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/output/output.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.123743 audiobook-dl-0.6.0/audiobookdl/sources/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1637 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2050 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/audiobooksdotcom.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4654 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/bookbeat.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4318 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/chirp.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3510 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/ereolen.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1325 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/librivox.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5289 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/nextory.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3308 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/overdrive.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     7927 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/podimo.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/sources/rss.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4413 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/saxo.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     6258 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/scribd.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.124743 audiobook-dl-0.6.0/audiobookdl/sources/source/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5125 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/source/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2404 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/audiobookdl/sources/source/networking.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5819 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/storytel.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4717 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/sources/yourcloudlibrary.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.124743 audiobook-dl-0.6.0/audiobookdl/utils/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1159 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/utils/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/audiobookdl/utils/audiobook.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1317 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/pyproject.toml
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-09 17:36:37.126743 audiobook-dl-0.6.0/setup.cfg
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/setup.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      434 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/shell.nix
--rw-r--r--   0 jo1gi     (1000) users      (100)     2139 2023-07-06 17:09:06.000000 audiobook-dl-0.6.0/supported_sites.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-09 17:36:37.125743 audiobook-dl-0.6.0/tests/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1087 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/tests/test_output.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-07-01 12:46:04.000000 audiobook-dl-0.6.0/tests/test_urls.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.490252 audiobook-dl-0.6.1/.github/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/FUNDING.yml
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.490252 audiobook-dl-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.491252 audiobook-dl-0.6.1/.github/workflows/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/workflows/pytest.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.gitignore
+-rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/LICENSE
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4798 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/README.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.493252 audiobook-dl-0.6.1/audiobook_dl.egg-info/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2311 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       59 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/entry_points.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       88 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/requires.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/top_level.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.495252 audiobook-dl-0.6.1/audiobookdl/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      191 2023-07-10 19:59:26.000000 audiobook-dl-0.6.1/audiobookdl/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5968 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/__main__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3495 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/args.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.496252 audiobook-dl-0.6.1/audiobookdl/assets/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.500252 audiobook-dl-0.6.1/audiobookdl/assets/errors/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/book_access.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/chapters_add.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       56 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/config_not_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/data_not_present.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/failed_combining.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/missing_dependency.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/no_files_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/no_source_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/request_error.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/user_not_authorized.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/ffmpeg_chapter_template.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/simple_help.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.486252 audiobook-dl-0.6.1/audiobookdl/assets/sources/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.503252 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1010 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/book_info.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      108 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/files.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      270 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/login.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      185 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      866 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episodes.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1983 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/config.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1342 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/exceptions.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1407 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/logging.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.505252 audiobook-dl-0.6.1/audiobookdl/output/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     8073 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/download.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/encryption.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.506252 audiobook-dl-0.6.1/audiobookdl/output/metadata/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1363 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1524 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/ffmpeg.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2391 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/id3.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/mp4.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3473 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/output.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.511252 audiobook-dl-0.6.1/audiobookdl/sources/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1637 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2050 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/audiobooksdotcom.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4654 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/bookbeat.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4318 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/chirp.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3510 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/ereolen.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1325 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/librivox.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5289 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/nextory.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3308 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/overdrive.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     7927 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/podimo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/sources/rss.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4413 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/saxo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     6258 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/scribd.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.512252 audiobook-dl-0.6.1/audiobookdl/sources/source/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5125 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/source/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2404 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/sources/source/networking.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5819 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/storytel.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4717 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/yourcloudlibrary.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.512252 audiobook-dl-0.6.1/audiobookdl/utils/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1159 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/utils/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/utils/audiobook.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1318 2023-07-10 19:58:47.000000 audiobook-dl-0.6.1/pyproject.toml
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/setup.cfg
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/setup.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      434 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/shell.nix
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2139 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/supported_sites.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.513252 audiobook-dl-0.6.1/tests/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1087 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/tests/test_output.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/tests/test_urls.py
```

### Comparing `audiobook-dl-0.6.0/.gitignore` & `audiobook-dl-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/LICENSE` & `audiobook-dl-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/PKG-INFO` & `audiobook-dl-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.6.0
+Version: 0.6.1
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiobook-dl-0.6.0/README.md` & `audiobook-dl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobook_dl.egg-info/PKG-INFO` & `audiobook-dl-0.6.1/audiobook_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.6.0
+Version: 0.6.1
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiobook-dl-0.6.0/audiobook_dl.egg-info/SOURCES.txt` & `audiobook-dl-0.6.1/audiobook_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/__main__.py` & `audiobook-dl-0.6.1/audiobookdl/__main__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/args.py` & `audiobook-dl-0.6.1/audiobookdl/args.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/book_info.graphql` & `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/book_info.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast.graphql` & `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/assets/sources/podimo/podcast_episodes.graphql` & `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episodes.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/config.py` & `audiobook-dl-0.6.1/audiobookdl/config.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/exceptions.py` & `audiobook-dl-0.6.1/audiobookdl/exceptions.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/logging.py` & `audiobook-dl-0.6.1/audiobookdl/logging.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/download.py` & `audiobook-dl-0.6.1/audiobookdl/output/download.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/encryption.py` & `audiobook-dl-0.6.1/audiobookdl/output/encryption.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/metadata/__init__.py` & `audiobook-dl-0.6.1/audiobookdl/output/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/metadata/ffmpeg.py` & `audiobook-dl-0.6.1/audiobookdl/output/metadata/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/metadata/id3.py` & `audiobook-dl-0.6.1/audiobookdl/output/metadata/id3.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/metadata/mp4.py` & `audiobook-dl-0.6.1/audiobookdl/output/metadata/mp4.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/output/output.py` & `audiobook-dl-0.6.1/audiobookdl/output/output.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/__init__.py` & `audiobook-dl-0.6.1/audiobookdl/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/audiobooksdotcom.py` & `audiobook-dl-0.6.1/audiobookdl/sources/audiobooksdotcom.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/bookbeat.py` & `audiobook-dl-0.6.1/audiobookdl/sources/bookbeat.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/chirp.py` & `audiobook-dl-0.6.1/audiobookdl/sources/chirp.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/ereolen.py` & `audiobook-dl-0.6.1/audiobookdl/sources/ereolen.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/librivox.py` & `audiobook-dl-0.6.1/audiobookdl/sources/librivox.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/nextory.py` & `audiobook-dl-0.6.1/audiobookdl/sources/nextory.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/overdrive.py` & `audiobook-dl-0.6.1/audiobookdl/sources/overdrive.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/podimo.py` & `audiobook-dl-0.6.1/audiobookdl/sources/podimo.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/saxo.py` & `audiobook-dl-0.6.1/audiobookdl/sources/saxo.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/scribd.py` & `audiobook-dl-0.6.1/audiobookdl/sources/scribd.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/source/__init__.py` & `audiobook-dl-0.6.1/audiobookdl/sources/source/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/source/networking.py` & `audiobook-dl-0.6.1/audiobookdl/sources/source/networking.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/storytel.py` & `audiobook-dl-0.6.1/audiobookdl/sources/storytel.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/sources/yourcloudlibrary.py` & `audiobook-dl-0.6.1/audiobookdl/sources/yourcloudlibrary.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/utils/__init__.py` & `audiobook-dl-0.6.1/audiobookdl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/audiobookdl/utils/audiobook.py` & `audiobook-dl-0.6.1/audiobookdl/utils/audiobook.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/pyproject.toml` & `audiobook-dl-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/jo1gi/audiobook-dl"
 "Bugtracker" = "https://github.com/jo1gi/audiobook-dl/issues"
 
 [project.scripts]
-audiobook-dl = "audiobookdl.__main__:run"
+audiobook-dl = "audiobookdl.__main__:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "audiobookdl.__version__"}
 
 [tool.setuptools.package-data]
 audiobookdl = ["*.txt"]
```

### Comparing `audiobook-dl-0.6.0/supported_sites.md` & `audiobook-dl-0.6.1/supported_sites.md`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/tests/test_output.py` & `audiobook-dl-0.6.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.0/tests/test_urls.py` & `audiobook-dl-0.6.1/tests/test_urls.py`

 * *Files identical despite different names*

