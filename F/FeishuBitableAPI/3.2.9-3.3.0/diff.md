# Comparing `tmp/FeishuBitableAPI-3.2.9.tar.gz` & `tmp/FeishuBitableAPI-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeishuBitableAPI-3.2.9.tar", last modified: Fri Jul  7 03:34:35 2023, max compression
+gzip compressed data, was "FeishuBitableAPI-3.3.0.tar", last modified: Mon Jul 10 06:02:00 2023, max compression
```

## Comparing `FeishuBitableAPI-3.2.9.tar` & `FeishuBitableAPI-3.3.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/FeishuBitableAPI/
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/BUILD_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CHECK_FIELD_EXIST.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CONVERSION_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_TABLE_QUICK.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/FeishuBitableAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_FIELDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_RECORDS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_TABLES.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_VIEWS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/UPDATE_FIELD.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/UPDATE_RECORD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_FIELD_INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_LOGIN_CODE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_RECORD_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_TABLE_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_VIEW_ID.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 03:34:25.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-07 03:34:35.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-07 03:34:35.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:34:35.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 03:34:35.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 03:34:35.000000 FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 03:34:17.000000 FeishuBitableAPI-3.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-07 03:34:17.000000 FeishuBitableAPI-3.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 03:34:17.000000 FeishuBitableAPI-3.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:34:35.374689 FeishuBitableAPI-3.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-07 03:34:17.000000 FeishuBitableAPI-3.2.9/test/test#GET_INFO_FROM_URL-2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-07 03:34:17.000000 FeishuBitableAPI-3.2.9/test/test#GET_INFO_FROM_URL.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:02:00.524664 FeishuBitableAPI-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:02:00.520664 FeishuBitableAPI-3.3.0/FeishuBitableAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/BUILD_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CHECK_FIELD_EXIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CONVERSION_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_TABLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_TABLE_QUICK.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/FeishuBitableAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_TENANT_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_FIELDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_RECORDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_TABLES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_VIEWS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/UPDATE_FIELD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/UPDATE_RECORD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_FIELD_INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_INFO_FROM_URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_LOGIN_CODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_RECORD_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_TABLE_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_TENANT_ACCESS_TOKEN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_VIEW_ID.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-10 06:01:53.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:02:00.524664 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 06:02:00.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-10 06:02:00.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:02:00.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 06:02:00.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 06:02:00.000000 FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 06:01:44.000000 FeishuBitableAPI-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 06:02:00.524664 FeishuBitableAPI-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 06:01:44.000000 FeishuBitableAPI-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:02:00.524664 FeishuBitableAPI-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-10 06:01:44.000000 FeishuBitableAPI-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:02:00.524664 FeishuBitableAPI-3.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-10 06:01:44.000000 FeishuBitableAPI-3.3.0/test/test#GET_INFO_FROM_URL-2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-10 06:01:44.000000 FeishuBitableAPI-3.3.0/test/test#GET_INFO_FROM_URL.py
```

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/ADD_RECORDS_FROM_CSV.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/BUILD_FIELD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/BUILD_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CHECK_FIELD_EXIST.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CHECK_FIELD_EXIST.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CHECK_FIELD_EXIST_SQL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CONVERSION_FIELDS.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CONVERSION_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_FIELD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_TABLE.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_TABLE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/CREATE_TABLE_QUICK.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/CREATE_TABLE_QUICK.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_FIELDS.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_FIELDS_DEFAULT.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/DELETE_RECORD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/DELETE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/FeishuBitableAPI.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/FeishuBitableAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .GET_APP_ACCESS_TOKEN import GET_APP_ACCESS_TOKEN
 from .GET_FIELD_INFO import GET_FIELD_INFO, GET_FIELD_ID, GET_FIELD_NAME
 from .GET_INFO_FROM_URL import GET_INFO_FROM_URL, GET_INFO_FROM_URL_JSON, GET_APPTOKEN_FROM_URL, GET_TABLEID_FROM_URL, GET_VIEWID_FROM_URL
 from .GET_LOGIN_CODE import GET_LOGIN_CODE
 from .GET_RECORD_ID import GET_RECORD_ID
 from .GET_RECORD import GET_RECORD
 from .GET_TABLE_ID import GET_TABLE_ID
+from .GET_TENANT_ACCESS_TOKEN import GET_TENANT_ACCESS_TOKEN
 from .GET_USER_ACCESS_TOKEN import GET_USER_ACCESS_TOKEN
 from .GET_VIEW_ID import GET_VIEW_ID
 
 from .LIST_FIELDS import LIST_FIELDS
 from .LIST_RECORDS import LIST_RECORDS
 from .LIST_TABLES import LIST_TABLES
 from .LIST_VIEWS import LIST_VIEWS
@@ -17,14 +18,15 @@
 
 from .WRITE_APP_ACCESS_TOKEN import WRITE_APP_ACCESS_TOKEN
 from .WRITE_FIELD_INFO import WRITE_FIELD_INFO
 from .WRITE_INFO_FROM_URL import WRITE_INFO_FROM_URL
 from .WRITE_LOGIN_CODE import WRITE_LOGIN_CODE
 from .WRITE_RECORD_ID import WRITE_RECORD_ID
 from .WRITE_TABLE_ID import WRITE_TABLE_ID
+from .WRITE_TENANT_ACCESS_TOKEN import WRITE_TENANT_ACCESS_TOKEN
 from .WRITE_VIEW_ID import WRITE_VIEW_ID
 
 from .CREATE_FIELD import CREATE_FIELD
 from .CREATE_TABLE import CREATE_TABLE
 
 from .CHECK_FIELD_EXIST import CHECK_FIELD_EXIST
 from .CHECK_FIELD_EXIST_SQL import CHECK_FIELD_EXIST_SQL
@@ -87,14 +89,18 @@
     def GET_RECORD(self, app_token=None, table_id=None, record_id=None, config_file=None):
         return GET_RECORD(app_token, table_id, record_id, config_file)
     
     #GET_TABLE_ID
     def GET_TABLE_ID(self, name="数据表", app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
         return GET_TABLE_ID(name, app_token, user_access_token, page_size, page_token, config_file)
     
+    #GET_TENANT_ACCESS_TOKEN
+    def GET_TENANT_ACCESS_TOKEN(self, app_id=None, app_secret=None, config_file=None):
+        return GET_TENANT_ACCESS_TOKEN(app_id, app_secret, config_file)
+    
     #GET_USER_ACCESS_TOKEN
     def GET_USER_ACCESS_TOKEN(self, login_code=None, app_access_token=None, config_file=None):
         return GET_USER_ACCESS_TOKEN(login_code, app_access_token, config_file)
     
     #GET_VIEW_ID
     def GET_VIEW_ID(self, view_name="默认视图", app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
         return GET_VIEW_ID(view_name, app_token, user_access_token, page_size, page_token, config_file)
@@ -138,15 +144,19 @@
     #WRITE_RECORD_ID
     def WRITE_RECORD_ID(self, value, field_name=None, config_file=None):
         return WRITE_RECORD_ID(value, field_name, config_file)
     
     #WRITE_TABLE_ID
     def WRITE_TABLE_ID(self, name, app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
         return WRITE_TABLE_ID(name, app_token, user_access_token, page_size, page_token, config_file)
-    
+
+    #WRITE_TENANT_ACCESS_TOKEN
+    def WRITE_TENANT_ACCESS_TOKEN(self, app_id=None, app_secret=None, config_file=None):
+        return WRITE_TENANT_ACCESS_TOKEN(app_id, app_secret, config_file)
+
     #WRITE_VIEW_ID
     def WRITE_VIEW_ID(self, view_name, app_token=None, user_access_token=None, page_size=None, page_token=None, config_file=None):
         return WRITE_VIEW_ID(view_name, app_token, user_access_token, page_size, page_token, config_file)
    
     #CREATE_FIELD
     def CREATE_FIELD(self, field_name, field_type=None, app_token=None, table_id=None, config_file=None):
         return CREATE_FIELD(field_name, field_type, app_token, table_id, config_file)
```

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_FIELD_INFO.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_FIELD_INFO.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_LOGIN_CODE.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_RECORD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_RECORD_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_RECORD_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_TABLE_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_TABLE_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/GET_VIEW_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/GET_VIEW_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_FIELDS.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_FIELDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_RECORDS.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_RECORDS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_TABLES.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_TABLES.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/LIST_VIEWS.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/LIST_VIEWS.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/UPDATE_FIELD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/UPDATE_FIELD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/UPDATE_RECORD.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/UPDATE_RECORD.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_FIELD_INFO.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_FIELD_INFO.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_INFO_FROM_URL.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_INFO_FROM_URL.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_LOGIN_CODE.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_LOGIN_CODE.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_RECORD_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_RECORD_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_TABLE_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_TABLE_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/WRITE_VIEW_ID.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/WRITE_VIEW_ID.py`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI/setup.py` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.2.9',
+    version='3.3.0',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/PKG-INFO` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.2.9
+Version: 3.3.0
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.2.9/FeishuBitableAPI.egg-info/SOURCES.txt` & `FeishuBitableAPI-3.3.0/FeishuBitableAPI.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 FeishuBitableAPI/GET_APP_ACCESS_TOKEN.py
 FeishuBitableAPI/GET_FIELD_INFO.py
 FeishuBitableAPI/GET_INFO_FROM_URL.py
 FeishuBitableAPI/GET_LOGIN_CODE.py
 FeishuBitableAPI/GET_RECORD.py
 FeishuBitableAPI/GET_RECORD_ID.py
 FeishuBitableAPI/GET_TABLE_ID.py
+FeishuBitableAPI/GET_TENANT_ACCESS_TOKEN.py
 FeishuBitableAPI/GET_USER_ACCESS_TOKEN.py
 FeishuBitableAPI/GET_VIEW_ID.py
 FeishuBitableAPI/LIST_FIELDS.py
 FeishuBitableAPI/LIST_RECORDS.py
 FeishuBitableAPI/LIST_TABLES.py
 FeishuBitableAPI/LIST_VIEWS.py
 FeishuBitableAPI/REFRESH_USER_ACCESS_TOKEN.py
@@ -31,14 +32,15 @@
 FeishuBitableAPI/UPDATE_RECORD.py
 FeishuBitableAPI/WRITE_APP_ACCESS_TOKEN.py
 FeishuBitableAPI/WRITE_FIELD_INFO.py
 FeishuBitableAPI/WRITE_INFO_FROM_URL.py
 FeishuBitableAPI/WRITE_LOGIN_CODE.py
 FeishuBitableAPI/WRITE_RECORD_ID.py
 FeishuBitableAPI/WRITE_TABLE_ID.py
+FeishuBitableAPI/WRITE_TENANT_ACCESS_TOKEN.py
 FeishuBitableAPI/WRITE_VIEW_ID.py
 FeishuBitableAPI/__init__.py
 FeishuBitableAPI/__main__.py
 FeishuBitableAPI/setup.py
 FeishuBitableAPI/test.py
 FeishuBitableAPI.egg-info/PKG-INFO
 FeishuBitableAPI.egg-info/SOURCES.txt
```

### Comparing `FeishuBitableAPI-3.2.9/LICENSE` & `FeishuBitableAPI-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/PKG-INFO` & `FeishuBitableAPI-3.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeishuBitableAPI
-Version: 3.2.9
+Version: 3.3.0
 Summary: A Python API for Feishu Bitable
 Home-page: https://github.com/BlueSkyXN/Feishu-Bitable-Python-API
 Author: BlueSkyXN
 Author-email: bluesky@000714.xyz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `FeishuBitableAPI-3.2.9/README.md` & `FeishuBitableAPI-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FeishuBitableAPI-3.2.9/setup.py` & `FeishuBitableAPI-3.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FeishuBitableAPI',
-    version='3.2.9',
+    version='3.3.0',
     packages=find_packages(),
     #py_modules=[],
     url='https://github.com/BlueSkyXN/Feishu-Bitable-Python-API',
     author='BlueSkyXN',
     author_email='bluesky@000714.xyz',
     description='A Python API for Feishu Bitable',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
```

### Comparing `FeishuBitableAPI-3.2.9/test/test#GET_INFO_FROM_URL.py` & `FeishuBitableAPI-3.3.0/test/test#GET_INFO_FROM_URL.py`

 * *Files identical despite different names*

