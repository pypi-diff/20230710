# Comparing `tmp/nuclia-1.1.1.tar.gz` & `tmp/nuclia-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.1.1.tar", last modified: Fri Jul  7 07:14:08 2023, max compression
+gzip compressed data, was "nuclia-1.1.2.tar", last modified: Mon Jul 10 12:37:22 2023, max compression
```

## Comparing `nuclia-1.1.1.tar` & `nuclia-1.1.2.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024874 nuclia-1.1.1/
--rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-07 07:14:07.000000 nuclia-1.1.1/.gitignore
--rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-07 07:14:07.000000 nuclia-1.1.1/.python-version
--rw-r--r--   0 ebr        (501) staff       (20)      545 2023-07-07 07:14:07.000000 nuclia-1.1.1/CHANGELOG.md
--rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-07 07:14:07.000000 nuclia-1.1.1/LICENSE
--rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-07 07:14:07.000000 nuclia-1.1.1/MANIFEST.in
--rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-07 07:14:07.000000 nuclia-1.1.1/Makefile
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-07 07:14:08.025019 nuclia-1.1.1/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-07 07:14:07.000000 nuclia-1.1.1/README.md
--rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-07 07:14:07.000000 nuclia-1.1.1/VERSION
--rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-07 07:14:07.000000 nuclia-1.1.1/code-requirements.txt
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.013309 nuclia-1.1.1/docs/
--rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/AUTH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/CONVERSATION.md
--rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/DEFAULT.md
--rw-r--r--   0 ebr        (501) staff       (20)      648 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/README.md
--rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/SEARCH.md
--rw-r--r--   0 ebr        (501) staff       (20)     1993 2023-07-07 07:14:07.000000 nuclia-1.1.1/docs/UPLOAD.md
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.014692 nuclia-1.1.1/nuclia/
--rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.017279 nuclia-1.1.1/nuclia/cli/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)     1280 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/run.py
--rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/cli/utils.py
--rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/config.py
--rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/data.py
--rw-r--r--   0 ebr        (501) staff       (20)     3040 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/decorators.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/exceptions.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.018792 nuclia-1.1.1/nuclia/lib/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/conversations.py
--rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/lib/nua_responses.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.022465 nuclia-1.1.1/nuclia/sdk/
--rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/__init__.py
--rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/accounts.py
--rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/auth.py
--rw-r--r--   0 ebr        (501) staff       (20)     1341 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/kb.py
--rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/kbs.py
--rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/logger.py
--rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/nua.py
--rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/nuas.py
--rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/predict.py
--rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/process.py
--rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/search.py
--rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/train.py
--rw-r--r--   0 ebr        (501) staff       (20)     8910 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/upload.py
--rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/sdk/zones.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024303 nuclia-1.1.1/nuclia/tests/
--rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/__init__.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.024587 nuclia-1.1.1/nuclia/tests/assets/
--rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/conftest.py
--rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/fixtures.py
--rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_auth.py
--rw-r--r--   0 ebr        (501) staff       (20)      682 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_conversation.py
--rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia/tests/test_predict.py
-drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-07 07:14:08.016583 nuclia-1.1.1/nuclia.egg-info/
--rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ebr        (501) staff       (20)     1222 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/requires.txt
--rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-07 07:14:07.000000 nuclia-1.1.1/nuclia.egg-info/zip-safe
--rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-07 07:14:07.000000 nuclia-1.1.1/requirements.txt
--rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-07 07:14:08.025607 nuclia-1.1.1/setup.cfg
--rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-07 07:14:07.000000 nuclia-1.1.1/setup.py
--rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-07 07:14:07.000000 nuclia-1.1.1/test-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655895 nuclia-1.1.2/
+-rw-r--r--   0 ebr        (501) staff       (20)       39 2023-07-10 12:37:22.000000 nuclia-1.1.2/.gitignore
+-rw-r--r--   0 ebr        (501) staff       (20)       10 2023-07-10 12:37:22.000000 nuclia-1.1.2/.python-version
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-10 12:37:22.000000 nuclia-1.1.2/CHANGELOG.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1063 2023-07-10 12:37:22.000000 nuclia-1.1.2/LICENSE
+-rw-r--r--   0 ebr        (501) staff       (20)       83 2023-07-10 12:37:22.000000 nuclia-1.1.2/MANIFEST.in
+-rw-r--r--   0 ebr        (501) staff       (20)      236 2023-07-10 12:37:22.000000 nuclia-1.1.2/Makefile
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-10 12:37:22.656070 nuclia-1.1.2/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)      955 2023-07-10 12:37:22.000000 nuclia-1.1.2/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)        6 2023-07-10 12:37:22.000000 nuclia-1.1.2/VERSION
+-rw-r--r--   0 ebr        (501) staff       (20)       24 2023-07-10 12:37:22.000000 nuclia-1.1.2/code-requirements.txt
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.644220 nuclia-1.1.2/docs/
+-rw-r--r--   0 ebr        (501) staff       (20)      941 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/AUTH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1225 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/CONVERSATION.md
+-rw-r--r--   0 ebr        (501) staff       (20)      892 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/DEFAULT.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1106 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/EXTRACT.md
+-rw-r--r--   0 ebr        (501) staff       (20)      715 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/README.md
+-rw-r--r--   0 ebr        (501) staff       (20)     1277 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/SEARCH.md
+-rw-r--r--   0 ebr        (501) staff       (20)     2202 2023-07-10 12:37:22.000000 nuclia-1.1.2/docs/UPLOAD.md
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.645780 nuclia-1.1.2/nuclia/
+-rw-r--r--   0 ebr        (501) staff       (20)      303 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.648263 nuclia-1.1.2/nuclia/cli/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1353 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/run.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/cli/utils.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6337 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/config.py
+-rw-r--r--   0 ebr        (501) staff       (20)      739 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/data.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3040 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/decorators.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/exceptions.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.649448 nuclia-1.1.2/nuclia/lib/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      153 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/conversations.py
+-rw-r--r--   0 ebr        (501) staff       (20)     6040 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)      868 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)      123 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/lib/nua_responses.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.653368 nuclia-1.1.2/nuclia/sdk/
+-rw-r--r--   0 ebr        (501) staff       (20)      343 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/__init__.py
+-rw-r--r--   0 ebr        (501) staff       (20)      229 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/accounts.py
+-rw-r--r--   0 ebr        (501) staff       (20)     7913 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2021 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/kb.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2251 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/kbs.py
+-rw-r--r--   0 ebr        (501) staff       (20)       57 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/logger.py
+-rw-r--r--   0 ebr        (501) staff       (20)      410 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/nua.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1092 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/nuas.py
+-rw-r--r--   0 ebr        (501) staff       (20)      469 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      190 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/process.py
+-rw-r--r--   0 ebr        (501) staff       (20)     3338 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/resource.py
+-rw-r--r--   0 ebr        (501) staff       (20)     2974 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/search.py
+-rw-r--r--   0 ebr        (501) staff       (20)      188 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/train.py
+-rw-r--r--   0 ebr        (501) staff       (20)     9248 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/upload.py
+-rw-r--r--   0 ebr        (501) staff       (20)      223 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/sdk/zones.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655190 nuclia-1.1.2/nuclia/tests/
+-rw-r--r--   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/__init__.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.655525 nuclia-1.1.2/nuclia/tests/assets/
+-rw-r--r--   0 ebr        (501) staff       (20)      348 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ebr        (501) staff       (20)       50 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/conftest.py
+-rw-r--r--   0 ebr        (501) staff       (20)     1200 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/fixtures.py
+-rw-r--r--   0 ebr        (501) staff       (20)      492 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_auth.py
+-rw-r--r--   0 ebr        (501) staff       (20)      738 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_conversation.py
+-rw-r--r--   0 ebr        (501) staff       (20)      247 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_predict.py
+-rw-r--r--   0 ebr        (501) staff       (20)      882 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia/tests/test_resource.py
+drwxr-xr-x   0 ebr        (501) staff       (20)        0 2023-07-10 12:37:22.647578 nuclia-1.1.2/nuclia.egg-info/
+-rw-r--r--   0 ebr        (501) staff       (20)     2049 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ebr        (501) staff       (20)     1291 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ebr        (501) staff       (20)       47 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      105 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        7 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ebr        (501) staff       (20)        1 2023-07-10 12:37:22.000000 nuclia-1.1.2/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ebr        (501) staff       (20)      104 2023-07-10 12:37:22.000000 nuclia-1.1.2/requirements.txt
+-rw-r--r--   0 ebr        (501) staff       (20)      204 2023-07-10 12:37:22.656573 nuclia-1.1.2/setup.cfg
+-rw-r--r--   0 ebr        (501) staff       (20)     1946 2023-07-10 12:37:22.000000 nuclia-1.1.2/setup.py
+-rw-r--r--   0 ebr        (501) staff       (20)       45 2023-07-10 12:37:22.000000 nuclia-1.1.2/test-requirements.txt
```

### Comparing `nuclia-1.1.1/CHANGELOG.md` & `nuclia-1.1.2/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 1.1.2 (2023-07-10)
+
+
+- Manage UserTokenExpired in CLI.
+- Support `show` and `extracted` when getting a resource.
+- Refactor all resource related actions in a class.
+- Support `Link` upload
+
+
 ## 1.1.1 (2023-07-07)
 
 
 - Set region parameter according KB url
 
 
 ## 1.1.0 (2023-07-05)
```

### Comparing `nuclia-1.1.1/LICENSE` & `nuclia-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/PKG-INFO` & `nuclia-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.1/README.md` & `nuclia-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/docs/AUTH.md` & `nuclia-1.1.2/docs/AUTH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/docs/CONVERSATION.md` & `nuclia-1.1.2/docs/CONVERSATION.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/docs/DEFAULT.md` & `nuclia-1.1.2/docs/DEFAULT.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/docs/SEARCH.md` & `nuclia-1.1.2/docs/SEARCH.md`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/docs/UPLOAD.md` & `nuclia-1.1.2/docs/UPLOAD.md`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,29 @@
 
 Pass `origin` or `extra` metadata:
 
 ```bash
 nuclia kb upload text --path=FILE_PATH --origin='{"url":"https://somwhere.com"}' --extra='{"metadata":{"whatever":42}}'
 ```
 
+
+## Upload an URL in a KnowledgeBox
+
+Push a text to a knowledgebox:
+
+```bash
+nuclia kb upload link --uri=THE_URI
+```
+
+```python
+from nuclia import sdk
+upload = sdk.NucliaUpload()
+upload.link(uri=THE_URI)
+```
+
 ## List resources on a kb
 
 ```bash
 nuclia kb list
 ```
 
 ## Delete a resource on a kb
```

### Comparing `nuclia-1.1.1/nuclia/cli/run.py` & `nuclia-1.1.2/nuclia/cli/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 
 import fire  # type: ignore
 from nucliadb_sdk import exceptions
 
 from nuclia.data import get_auth
-from nuclia.exceptions import NeedUserToken
+from nuclia.exceptions import NeedUserToken, UserTokenExpired
 from nuclia.sdk.accounts import NucliaAccounts
 from nuclia.sdk.kb import NucliaKB
 from nuclia.sdk.kbs import NucliaKBS
 from nuclia.sdk.logger import logger
 from nuclia.sdk.nua import NucliaNUA
 from nuclia.sdk.nuas import NucliaNUAS
 from nuclia.sdk.zones import NucliaZones
@@ -37,13 +37,15 @@
 
     try:
         fire.Fire(NucliaCLI)
     except exceptions.AuthError:
         handleAuthError()
     except NeedUserToken:
         handleAuthError()
+    except UserTokenExpired:
+        handleAuthError()
 
 
 def handleAuthError():
     logger.error("Login required.")
     logger.info("Run `nuclia auth login` to login.")
     sys.exit(1)
```

### Comparing `nuclia-1.1.1/nuclia/cli/utils.py` & `nuclia-1.1.2/nuclia/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/config.py` & `nuclia-1.1.2/nuclia/config.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/data.py` & `nuclia-1.1.2/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/decorators.py` & `nuclia-1.1.2/nuclia/decorators.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/lib/kb.py` & `nuclia-1.1.2/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/lib/nua.py` & `nuclia-1.1.2/nuclia/lib/nua.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/sdk/auth.py` & `nuclia-1.1.2/nuclia/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/sdk/kbs.py` & `nuclia-1.1.2/nuclia/sdk/kbs.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/sdk/nuas.py` & `nuclia-1.1.2/nuclia/sdk/nuas.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/sdk/search.py` & `nuclia-1.1.2/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia/sdk/upload.py` & `nuclia-1.1.2/nuclia/sdk/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,39 +5,29 @@
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Tuple
 from uuid import uuid4
 
 import requests
+from nuclia.sdk.resource import RESOURCE_ATTRIBUTES, NucliaResource
 from nucliadb_models.text import TextFormat
 from nucliadb_sdk import exceptions
 from tqdm import tqdm
 
 from nuclia.data import get_auth
 from nuclia.decorators import kb
 from nuclia.lib.conversations import Conversation
 from nuclia.sdk.auth import NucliaAuth
 from nuclia.sdk.logger import logger
 
-RESOURCE_ATTRIBUTES = [
-    "icon",
-    "origin",
-    "extra",
-    "conversations",
-    "texts",
-    "usermetadata",
-    "fieldmetadata",
-    "title",
-]
-
 
 class NucliaUpload:
     """
-    Create or update resource in a Nuclia KnowledgeBox.
+    Create or update resource content in a Nuclia KnowledgeBox.
 
     All commands accept the following parameters:
     - `rid`: Resource ID. If not provided, a new resource will be created.
     - `slug`: Resource slug. If it corresponds to an existing resource, the resource will be updated.
         If not provided, a unique value will be generated.
     - `field`: Field id. If not provided, a unique value will be generated.
     - `title`: resource title.
@@ -183,14 +173,40 @@
             self._update_resource(
                 rid=rid,
                 texts=texts,
                 **kwargs,
             )
 
     @kb
+    def link(
+        self,
+        *,
+        uri: str,
+        **kwargs,
+    ):
+        """Upload an URL to a Nuclia KnowledgeBox."""
+        field = kwargs.get("field") or uuid4().hex
+        links = {
+            field: {
+                "uri": uri,
+            }
+        }
+        kwargs["icon"] = "application/stf-link"
+        rid, is_new_resource = self._get_or_create_resource(
+            links=links,
+            **kwargs,
+        )
+        if not is_new_resource:
+            self._update_resource(
+                rid=rid,
+                links=links,
+                **kwargs,
+            )
+
+    @kb
     def remote(
         self,
         *,
         origin: str,
         rid: Optional[str] = None,
         field: Optional[str] = "file",
         **kwargs,
@@ -224,15 +240,15 @@
                 if is_new_resource:
                     ndb.ndb.delete_resource(kbid=ndb.kbid, rid=rid)
                 sys.exit(1)
 
     def _get_or_create_resource(*args, **kwargs) -> Tuple[str, bool]:
         rid = kwargs.get("rid")
         if rid:
-            return rid
+            return (rid, False)
         ndb = kwargs["ndb"]
         slug = kwargs.get("slug")
         need_to_create_resource = slug is None
         if slug:
             try:
                 resource = ndb.ndb.get_resource_by_slug(kbid=ndb.kbid, slug=slug)
                 rid = resource.id
@@ -254,16 +270,8 @@
             resource = ndb.ndb.create_resource(**kw)
             rid = resource.uuid
             logger.warning(f"New resource created: {rid}")
 
         return (rid, need_to_create_resource)
 
     def _update_resource(self, rid: str, **kwargs):
-        ndb = kwargs["ndb"]
-        kw = {
-            "kbid": ndb.kbid,
-            "rid": rid,
-        }
-        for param in RESOURCE_ATTRIBUTES:
-            if param in kwargs:
-                kw[param] = kwargs.get(param)
-        ndb.ndb.update_resource(**kw)
+        return NucliaResource().update(rid=rid, **kwargs)
```

### Comparing `nuclia-1.1.1/nuclia/tests/fixtures.py` & `nuclia-1.1.2/nuclia/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.1.1/nuclia.egg-info/PKG-INFO` & `nuclia-1.1.2/nuclia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
```

### Comparing `nuclia-1.1.1/nuclia.egg-info/SOURCES.txt` & `nuclia-1.1.2/nuclia.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 docs/AUTH.md
 docs/CONVERSATION.md
 docs/DEFAULT.md
+docs/EXTRACT.md
 docs/README.md
 docs/SEARCH.md
 docs/UPLOAD.md
 nuclia/__init__.py
 nuclia/config.py
 nuclia/data.py
 nuclia/decorators.py
@@ -43,18 +44,20 @@
 nuclia/sdk/kb.py
 nuclia/sdk/kbs.py
 nuclia/sdk/logger.py
 nuclia/sdk/nua.py
 nuclia/sdk/nuas.py
 nuclia/sdk/predict.py
 nuclia/sdk/process.py
+nuclia/sdk/resource.py
 nuclia/sdk/search.py
 nuclia/sdk/train.py
 nuclia/sdk/upload.py
 nuclia/sdk/zones.py
 nuclia/tests/__init__.py
 nuclia/tests/conftest.py
 nuclia/tests/fixtures.py
 nuclia/tests/test_auth.py
 nuclia/tests/test_conversation.py
 nuclia/tests/test_predict.py
+nuclia/tests/test_resource.py
 nuclia/tests/assets/conversation.json
```

### Comparing `nuclia-1.1.1/setup.py` & `nuclia-1.1.2/setup.py`

 * *Files identical despite different names*

