# Comparing `tmp/onetl-0.8.0.tar.gz` & `tmp/onetl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetl-0.8.0.tar", last modified: Wed May 31 12:25:25 2023, max compression
+gzip compressed data, was "onetl-0.8.1.tar", last modified: Mon Jul 10 09:08:20 2023, max compression
```

## Comparing `onetl-0.8.0.tar` & `onetl-0.8.1.tar`

### file list

```diff
@@ -1,194 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-31 12:25:07.000000 onetl-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 12:25:07.000000 onetl-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-05-31 12:25:25.988076 onetl-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-31 12:25:07.000000 onetl-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/contains_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/contains_get_df_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/path_stat_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/pure_path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/supports_rename_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/db_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/db_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py
--rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/hive.py
--rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/jdbc_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/jdbc_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25843 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/teradata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/file_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24970 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/ftps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/hdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/file_connection/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/mixins/rename_dir_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/kerberos_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/core/file_filter/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_filter/file_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/core/file_limit/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_limit/file_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/db_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/strategy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/db_writer/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_writer/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/download_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    27219 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/file_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_mover/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17605 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/file_mover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/move_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_uploader/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/upload_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/exclude_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/file_hwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/glob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/match_all_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/regexp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/limit/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/limits_reached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/limits_stop_at.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/max_files_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/reset_limits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hooks_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/method_inheritance_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/slot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/support_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hwm/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hwm/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/base_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_store_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_store_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/memory_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/yaml_hwm_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/failed_local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/file_write_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/frozen_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/generic_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/local_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/path_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/path_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_path_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/plugins/import_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/onetl/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/batch_hwm_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/onetl/strategy/hwm_store/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/hwm_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/hwm_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/incremental_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/snapshot_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/strategy_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-31 12:25:07.000000 onetl-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/ftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/hdfs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/kerberos.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/s3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/sftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/spark.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/requirements/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/clickhouse.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mssql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/oracle.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-2.3.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-2.4.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.2.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.3.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-latest.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/webdav.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-31 12:25:25.992076 onetl-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-31 12:25:08.000000 onetl-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.293254 onetl-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-10 09:08:04.000000 onetl-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 09:08:04.000000 onetl-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-07-10 09:08:20.293254 onetl-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-10 09:08:04.000000 onetl-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.273255 onetl-0.8.1/onetl/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.277255 onetl-0.8.1/onetl/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/base_db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19414 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/base_file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/base_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/base_file_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/contains_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/contains_get_df_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/path_stat_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/pure_path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/base/supports_rename_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.277255 onetl-0.8.1/onetl/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.277255 onetl-0.8.1/onetl/connection/db_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/db_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.277255 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_where_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26626 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32422 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27999 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/jdbc_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23653 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/jdbc_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/db_connection/teradata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/connection/file_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/ftps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26357 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/hdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/connection/file_connection/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/mixins/rename_dir_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/file_connection/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/connection/kerberos_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/core/file_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/core/file_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/core/file_filter/file_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/core/file_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/core/file_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/core/file_limit/file_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/db/db_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/db_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/db_reader/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/db_reader/strategy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/db/db_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/db_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/db/db_writer/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/file/file_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_downloader/download_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30011 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_downloader/file_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/file/file_mover/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_mover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_mover/file_mover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_mover/move_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18628 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.281255 onetl-0.8.1/onetl/file/file_uploader/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21980 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_uploader/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/file_uploader/upload_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.285255 onetl-0.8.1/onetl/file/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/exclude_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/file_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/match_all_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/filter/regexp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.285255 onetl-0.8.1/onetl/file/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/limit/limits_reached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/limit/limits_stop_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/limit/max_files_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/file/limit/reset_limits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.285255 onetl-0.8.1/onetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/hook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/hooks_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/method_inheritance_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hooks/support_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.285255 onetl-0.8.1/onetl/hwm/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.285255 onetl-0.8.1/onetl/hwm/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/base_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/hwm_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/hwm_store_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/hwm_store_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/memory_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/hwm/store/yaml_hwm_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.289255 onetl-0.8.1/onetl/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/failed_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/file_write_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/frozen_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/generic_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/local_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/path_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/path_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/remote_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/remote_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/remote_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/impl/remote_path_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.289255 onetl-0.8.1/onetl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/plugins/import_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.289255 onetl-0.8.1/onetl/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/batch_hwm_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.289255 onetl-0.8.1/onetl/strategy/hwm_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/hwm_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/hwm_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/incremental_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/snapshot_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/strategy/strategy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-10 09:08:04.000000 onetl-0.8.1/onetl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.273255 onetl-0.8.1/onetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19554 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 09:08:20.000000 onetl-0.8.1/onetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-10 09:08:04.000000 onetl-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.289255 onetl-0.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/ftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/hdfs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/kerberos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/s3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/sftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/spark.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:20.293254 onetl-0.8.1/requirements/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/clickhouse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/kafka.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/mssql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/oracle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-2.3.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-2.4.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-3.2.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-3.3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-3.4.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/tests/spark-latest.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 09:08:04.000000 onetl-0.8.1/requirements/webdav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-10 09:08:20.293254 onetl-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-10 09:08:04.000000 onetl-0.8.1/setup.py
```

### Comparing `onetl-0.8.0/LICENSE.txt` & `onetl-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/__init__.py` & `onetl-0.8.1/onetl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/_internal.py` & `onetl-0.8.1/onetl/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,16 @@
             clear_statement("CREATE TABLE mytable (id NUMBER)")
             == "CREATE TABLE mytable (id NUMBER)"
         )
         assert clear_statement("BEGIN ... END") == "BEGIN ... END;"
     """
 
     statement = statement.rstrip().lstrip("\n\r").rstrip(";")
-
     if statement.lower().strip().endswith("end"):
         statement += ";"
-
     return statement
 
 
 def uniq_ignore_case(orig_list: list[str]) -> list[str]:
     """
     Return only uniq values from a list, case ignore.
```

### Comparing `onetl-0.8.0/onetl/base/__init__.py` & `onetl-0.8.1/onetl/base/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/base_connection.py` & `onetl-0.8.1/onetl/base/base_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class BaseConnection(ABC):
     """
     Generic connection class
     """
 
     @abstractmethod
     def check(self):
-        """Check source availability.
+        """Check source availability. |support_hooks|
 
         If not, an exception will be raised.
 
         Returns
         -------
         Connection itself
```

### Comparing `onetl-0.8.0/onetl/base/base_db_connection.py` & `onetl-0.8.1/onetl/base/base_db_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,32 +151,32 @@
         hint: Any | None = None,
         where: Any | None = None,
         df_schema: StructType | None = None,
         start_from: Statement | None = None,
         end_at: Statement | None = None,
     ) -> DataFrame:
         """
-        Reads the source to dataframe.
+        Reads the source to dataframe. |support_hooks|
         """
 
     @abstractmethod
     def write_df(
         self,
         df: DataFrame,
         target: str,
     ) -> None:
         """
-        Saves dataframe to a specific target
+        Saves dataframe to a specific target. |support_hooks|
         """
 
     @abstractmethod
     def get_min_max_bounds(
         self,
         source: str,
         column: str,
         expression: str | None = None,
         hint: Any | None = None,
         where: Any | None = None,
     ) -> tuple[Any, Any]:
         """
-        Get MIN and MAX values for the column in the source
+        Get MIN and MAX values for the column in the source. |support_hooks|
         """
```

### Comparing `onetl-0.8.0/onetl/base/base_file_connection.py` & `onetl-0.8.1/onetl/base/base_file_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     Implements generic methods for files and directories manipulation on some filesystem (usually remote)
     """
 
     @abstractmethod
     def path_exists(self, path: os.PathLike | str) -> bool:
         """
-        Check if specified path exists on remote filesystem.
+        Check if specified path exists on remote filesystem. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to check
 
         Returns
@@ -53,15 +53,15 @@
             assert connection.path_exists("/path/to/dir")
             assert not connection.path_exists("/path/to/missing")
         """
 
     @abstractmethod
     def is_file(self, path: os.PathLike | str) -> bool:
         """
-        Check if specified path is a file.
+        Check if specified path is a file. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to check
 
         Returns
@@ -81,15 +81,15 @@
             assert connection.is_file("/path/to/dir/file.csv")
             assert not connection.is_file("/path/to/dir")
         """
 
     @abstractmethod
     def is_dir(self, path: os.PathLike | str) -> bool:
         """
-        Check if specified path is a directory.
+        Check if specified path is a directory. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to check
 
         Returns
@@ -109,15 +109,15 @@
             assert connection.is_dir("/path/to/dir")
             assert not connection.is_dir("/path/to/dir/file.csv")
         """
 
     @abstractmethod
     def get_stat(self, path: os.PathLike | str) -> PathStatProtocol:
         """
-        Returns stats for a specific path.
+        Returns stats for a specific path. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to get stats for
 
         Returns
@@ -137,15 +137,15 @@
             assert stat.st_size > 0
             assert stat.st_uid == 12345  # owner id
         """
 
     @abstractmethod
     def resolve_dir(self, path: os.PathLike | str) -> PathWithStatsProtocol:
         """
-        Returns directory at specific path, with stats.
+        Returns directory at specific path, with stats. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to resolve
 
         Returns
@@ -169,15 +169,15 @@
             assert os.fspath(dir_path) == "/path/to/dir"
             assert dir_path.stat.st_uid == 12345  # owner id
         """
 
     @abstractmethod
     def resolve_file(self, path: os.PathLike | str) -> PathWithStatsProtocol:
         """
-        Returns file at specific path, with stats.
+        Returns file at specific path, with stats. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Path to resolve
 
         Returns
@@ -201,15 +201,15 @@
             assert os.fspath(file_path) == "/path/to/dir/file.csv"
             assert file_path.stat.st_uid == 12345  # owner id
         """
 
     @abstractmethod
     def create_dir(self, path: os.PathLike | str) -> PathWithStatsProtocol:
         """
-        Creates directory tree on remote filesystem.
+        Creates directory tree on remote filesystem. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Directory path
 
         Returns
@@ -228,15 +228,15 @@
 
             dir_path = connection.create_dir("/path/to/dir")
         """
 
     @abstractmethod
     def remove_file(self, path: os.PathLike | str) -> bool:
         """
-        Removes file on remote filesystem.
+        Removes file on remote filesystem. |support_hooks|
 
         If file does not exist, no exception is raised.
 
         .. warning::
 
             Supports only one file removal per call. Directory removal is **NOT** supported, use :obj:`~remove_dir` instead.
 
@@ -264,15 +264,15 @@
 
             assert not connection.remove_file("/path/to/file.csv")  # already deleted
         """
 
     @abstractmethod
     def remove_dir(self, path: os.PathLike | str, recursive: bool = False) -> bool:
         """
-        Remove directory or directory tree.
+        Remove directory or directory tree. |support_hooks|
 
         If directory does not exist, no exception is raised.
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Directory path to remote
@@ -305,15 +305,15 @@
     def rename_file(
         self,
         source_file_path: os.PathLike | str,
         target_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> PathWithStatsProtocol:
         """
-        Rename or move file on remote filesystem.
+        Rename or move file on remote filesystem. |support_hooks|
 
         .. warning::
 
             Supports only one file move per call. Directory move/rename is **NOT** supported.
 
         Parameters
         ----------
@@ -355,15 +355,15 @@
     def list_dir(
         self,
         path: os.PathLike | str,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> list[PathWithStatsProtocol]:
         """
-        Return list of child files/directories in a specific directory.
+        Return list of child files/directories in a specific directory. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             Directory path to list contents.
 
         filters : list of :obj:`BaseFileFilter <onetl.base.base_file_filter.BaseFileFilter>`, optional
@@ -400,15 +400,15 @@
         self,
         root: os.PathLike | str,
         topdown: bool = True,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> Iterable[tuple[PathWithStatsProtocol, list[PathWithStatsProtocol], list[PathWithStatsProtocol]]]:
         """
-        Walk into directory tree, and iterate over its content in all nesting levels.
+        Walk into directory tree, and iterate over its content in all nesting levels. |support_hooks|
 
         Just like :obj:`os.walk`, but with additional filter/limit logic.
 
         Parameters
         ----------
         root : str or :obj:`os.PathLike`
             Directory path to walk into.
@@ -453,15 +453,15 @@
     def download_file(
         self,
         remote_file_path: os.PathLike | str,
         local_file_path: os.PathLike | str,
         replace: bool = True,
     ) -> PathWithStatsProtocol:
         """
-        Downloads file from the remote filesystem to a local path.
+        Downloads file from the remote filesystem to a local path. |support_hooks|
 
         .. warning::
 
             Supports only one file download per call. Directory download is **NOT** supported, use :ref:`file-downloader` instead.
 
         Parameters
         ----------
@@ -509,15 +509,15 @@
     def upload_file(
         self,
         local_file_path: os.PathLike | str,
         remote_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> PathWithStatsProtocol:
         """
-        Uploads local file to a remote filesystem.
+        Uploads local file to a remote filesystem. |support_hooks|
 
         .. warning::
 
             Supports only one file upload per call. Directory upload is **NOT** supported, use :ref:`file-uploader` instead.
 
         Parameters
         ----------
@@ -560,15 +560,15 @@
             assert connection.path_exists("/path/to/target.csv")
             assert remote_file.stat().st_size == os.stat("/path/to/source.csv").st_size
         """
 
     @abstractmethod
     def read_text(self, path: os.PathLike | str, encoding: str = "utf-8") -> str:
         r"""
-        Returns string content of a file at specific path.
+        Returns string content of a file at specific path. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             File path to read
 
         encoding : str, default ``utf-8``
@@ -594,15 +594,15 @@
             content = connection.read_text("/path/to/dir/file.csv")
             assert content == "some;header\n1;2"
         """
 
     @abstractmethod
     def read_bytes(self, path: os.PathLike | str) -> bytes:
         """
-        Returns binary content of a file at specific path.
+        Returns binary content of a file at specific path. |support_hooks|
 
         Parameters
         ----------
         path : str or :obj:`os.PathLike`
             File path to read
 
         Returns
@@ -630,15 +630,15 @@
     def write_text(
         self,
         path: os.PathLike | str,
         content: str,
         encoding: str = "utf-8",
     ) -> PathWithStatsProtocol:
         r"""
-        Writes string content to a file at specific path.
+        Writes string content to a file at specific path. |support_hooks|
 
         .. warning::
 
             If file already exists, its content will be replaced.
 
         Parameters
         ----------
@@ -671,15 +671,15 @@
             file_path = connection.write_text("/path/to/dir/file.csv", "some;header\n1;2")
             assert file_path.stat.st_size > 0
         """
 
     @abstractmethod
     def write_bytes(self, path: os.PathLike | str, content: bytes) -> PathWithStatsProtocol:
         """
-        Writes bytes content to a file at specific path.
+        Writes bytes content to a file at specific path. |support_hooks|
 
         .. warning::
 
             If file already exists, its content will be replaced.
 
         Parameters
         ----------
```

### Comparing `onetl-0.8.0/onetl/base/base_file_filter.py` & `onetl-0.8.1/onetl/base/base_file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/base_file_limit.py` & `onetl-0.8.1/onetl/base/base_file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/contains_exception.py` & `onetl-0.8.1/onetl/base/contains_exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/contains_get_df_schema.py` & `onetl-0.8.1/onetl/base/contains_get_df_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,10 +30,10 @@
 
     def get_df_schema(
         self,
         source: str,
         columns: list[str] | None = None,
     ) -> StructType:
         """
-        Description of the dataframe schema.
+        Description of the dataframe schema. |support_hooks|
         """
         ...
```

### Comparing `onetl-0.8.0/onetl/base/path_protocol.py` & `onetl-0.8.1/onetl/base/path_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/path_stat_protocol.py` & `onetl-0.8.1/onetl/base/path_stat_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/pure_path_protocol.py` & `onetl-0.8.1/onetl/base/pure_path_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/base/supports_rename_dir.py` & `onetl-0.8.1/onetl/base/supports_rename_dir.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/connection/__init__.py` & `onetl-0.8.1/onetl/connection/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from __future__ import annotations
 
 from importlib import import_module
 from typing import TYPE_CHECKING
 
 from onetl.connection.db_connection.db_connection import DBConnection
 from onetl.connection.file_connection.file_connection import FileConnection
 
 if TYPE_CHECKING:
     from onetl.connection.db_connection.clickhouse import Clickhouse
     from onetl.connection.db_connection.greenplum import Greenplum
     from onetl.connection.db_connection.hive import Hive
+    from onetl.connection.db_connection.kafka import Kafka
     from onetl.connection.db_connection.mongodb import MongoDB
     from onetl.connection.db_connection.mssql import MSSQL
     from onetl.connection.db_connection.mysql import MySQL
     from onetl.connection.db_connection.oracle import Oracle
     from onetl.connection.db_connection.postgres import Postgres
     from onetl.connection.db_connection.teradata import Teradata
     from onetl.connection.file_connection.ftp import FTP
@@ -41,14 +43,15 @@
     "MongoDB": "mongodb",
     "Hive": "hive",
     "MSSQL": "mssql",
     "MySQL": "mysql",
     "Oracle": "oracle",
     "Postgres": "postgres",
     "Teradata": "teradata",
+    "Kafka": "kafka",
 }
 
 file_connections_modules = {
     "FTP": "ftp",
     "FTPS": "ftps",
     "HDFS": "hdfs",
     "S3": "s3",
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/clickhouse.py` & `onetl-0.8.1/onetl/connection/db_connection/clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # do not import PySpark here, as we allow user to use `Clickhouse.package` for creating Spark session
 
 
 log = logging.getLogger(__name__)
 
 
 class Clickhouse(JDBCConnection):
-    """Clickhouse JDBC connection.
+    """Clickhouse JDBC connection. |support_hooks|
 
     Based on Maven package ``ru.yandex.clickhouse:clickhouse-jdbc:0.3.2``
     (`official Clickhouse JDBC driver <https://github.com/ClickHouse/clickhouse-jdbc>`_).
 
     .. dropdown:: Version compatibility
 
         * Clickhouse server versions: 20.7 or higher
@@ -49,15 +49,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Clickhouse database. For example: ``test.clickhouse.domain.com`` or ``193.168.1.11``
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/db_connection.py` & `onetl-0.8.1/onetl/connection/db_connection/db_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,27 +126,23 @@
             return repr(result)
 
         @classmethod
         def _get_max_value_sql(cls, value: Any) -> str:
             """
             Generate `MAX(value)` clause for given value
             """
-
             result = cls._serialize_datetime_value(value)
-
             return f"MAX({result})"
 
         @classmethod
         def _get_min_value_sql(cls, value: Any) -> str:
             """
             Generate `MIN(value)` clause for given value
             """
-
             result = cls._serialize_datetime_value(value)
-
             return f"MIN({result})"
 
     @classmethod
     def _forward_refs(cls) -> dict[str, type]:
         # avoid importing pyspark unless user called the constructor,
         # as we allow user to use `Connection.package` for creating Spark session
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/__init__.py` & `onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py` & `onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hint_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py` & `onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py` & `onetl-0.8.1/onetl/connection/db_connection/dialect_mixins/support_where_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/connection/db_connection/greenplum.py` & `onetl-0.8.1/onetl/connection/db_connection/greenplum.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     SupportWhereStr,
 )
 from onetl.connection.db_connection.dialect_mixins.support_table_with_dbschema import (
     SupportTableWithDBSchema,
 )
 from onetl.connection.db_connection.jdbc_mixin import JDBCMixin
 from onetl.exception import MISSING_JVM_CLASS_MSG, TooManyParallelJobsError
+from onetl.hooks import slot, support_hooks
 from onetl.hwm import Statement
 from onetl.impl import GenericOptions
 from onetl.log import log_lines, log_with_indent
 
 # do not import PySpark here, as we allow user to use `Greenplum.package...` for creating Spark session
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
@@ -117,16 +118,17 @@
             occupied: {self.occupied}
             max: {self.maximum} ("max_connection" in postgresql.conf)
             reserved: {self.reserved} ("superuser_reserved_connections" in postgresql.conf)
             """,
         ).strip()
 
 
+@support_hooks
 class Greenplum(JDBCMixin, DBConnection):
-    """Greenplum connection.
+    """Greenplum connection. |support_hooks|
 
     Based on package ``io.pivotal:greenplum-spark:2.1.4``
     (`Pivotal connector for Spark <https://network.tanzu.vmware.com/products/vmware-greenplum#/releases/1287433/file_groups/13260>`_).
 
     .. warning::
 
         Before using this connector please take into account :ref:`greenplum-prerequisites`
@@ -482,14 +484,15 @@
             if not (key.startswith("server.") or key.startswith("pool."))
         }
         extra["ApplicationName"] = extra.get("ApplicationName", self.spark.sparkContext.appName)
 
         parameters = "&".join(f"{k}={v}" for k, v in sorted(extra.items()))
         return f"jdbc:postgresql://{self.host}:{self.port}/{self.database}?{parameters}".rstrip("?")
 
+    @slot
     def read_df(
         self,
         source: str,
         columns: list[str] | None = None,
         hint: str | None = None,
         where: str | None = None,
         df_schema: StructType | None = None,
@@ -512,14 +515,15 @@
 
         if columns:
             df = df.selectExpr(*columns)
 
         log.info("|Spark| DataFrame successfully created from SQL statement ")
         return df
 
+    @slot
     def write_df(
         self,
         df: DataFrame,
         target: str,
         options: WriteOptions | dict | None = None,
     ) -> None:
         self._check_driver_imported()
@@ -532,14 +536,15 @@
         df.write.format("greenplum").options(
             **self._connector_params(target),
             **options_dict,
         ).mode(write_options.mode).save()
 
         log.info("|%s| Table %r is successfully written", self.__class__.__name__, target)
 
+    @slot
     def get_df_schema(
         self,
         source: str,
         columns: list[str] | None = None,
         options: JDBCMixin.JDBCOptions | dict | None = None,
     ) -> StructType:
         log.info("|%s| Fetching schema of table %r", self.__class__.__name__, source)
@@ -551,14 +556,15 @@
         log_lines(query, level=logging.DEBUG)
 
         df = self._query_on_driver(query, jdbc_options)
         log.info("|%s| Schema fetched", self.__class__.__name__)
 
         return df.schema
 
+    @slot
     def get_min_max_bounds(
         self,
         source: str,
         column: str,
         expression: str | None = None,
         hint: str | None = None,
         where: str | None = None,
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/hive.py` & `onetl-0.8.1/onetl/connection/db_connection/hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             log.warning(
                 "Mode `overwrite` is deprecated since v0.4.0 and will be removed in v1.0.0, "
                 "use `overwrite_partitions` instead",
             )
             return cls.OVERWRITE_PARTITIONS
 
 
+@support_hooks
 class Hive(DBConnection):
     """Spark connection with Hive MetaStore support. |support_hooks|
 
     You don't need a Hive server to use this connector.
 
     .. dropdown:: Version compatibility
 
@@ -85,15 +86,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     .. warning::
 
         This connector requires some additional configuration files to be present (``hive-site.xml`` and so on),
         as well as .jar files with Hive MetaStore client.
@@ -521,18 +522,19 @@
         if known_clusters and validated_cluster not in known_clusters:
             raise ValueError(
                 f"Cluster {validated_cluster!r} is not in the known clusters list: {sorted(known_clusters)!r}",
             )
 
         return validated_cluster
 
+    @slot
     @classmethod
     def get_current(cls, spark: SparkSession):
         """
-        Create connection for current cluster.
+        Create connection for current cluster. |support_hooks|
 
         .. note::
 
             Can be used only if there are some hooks bound :obj:`~slots.get_current_cluster` slot.
 
         Parameters
         ----------
@@ -564,14 +566,15 @@
         log.info("|%s| Got %r", cls.__name__, current_cluster)
         return cls(cluster=current_cluster, spark=spark)
 
     @property
     def instance_url(self) -> str:
         return self.cluster
 
+    @slot
     def check(self):
         log.debug("|%s| Detecting current cluster...", self.__class__.__name__)
         current_cluster = self.slots.get_current_cluster()
         if current_cluster and self.cluster != current_cluster:
             raise ValueError("You can connect to a Hive cluster only from the same cluster")
 
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
@@ -585,20 +588,21 @@
             log.info("|%s| Connection is available.", self.__class__.__name__)
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise RuntimeError("Connection is unavailable") from e
 
         return self
 
+    @slot
     def sql(
         self,
         query: str,
     ) -> DataFrame:
         """
-        Lazily execute SELECT statement and return DataFrame.
+        Lazily execute SELECT statement and return DataFrame. |support_hooks|
 
         Same as ``spark.sql(query)``.
 
         Parameters
         ----------
         query : str
 
@@ -631,20 +635,21 @@
         log.info("|%s| Executing SQL query:", self.__class__.__name__)
         log_lines(query)
 
         df = self._execute_sql(query)
         log.info("|Spark| DataFrame successfully created from SQL statement")
         return df
 
+    @slot
     def execute(
         self,
         statement: str,
     ) -> None:
         """
-        Execute DDL or DML statement.
+        Execute DDL or DML statement. |support_hooks|
 
         Parameters
         ----------
         statement : str
 
             Statement to be executed, like:
 
@@ -689,14 +694,15 @@
 
         log.info("|%s| Executing statement:", self.__class__.__name__)
         log_lines(statement)
 
         self._execute_sql(statement).collect()
         log.info("|%s| Call succeeded", self.__class__.__name__)
 
+    @slot
     def write_df(
         self,
         df: DataFrame,
         target: str,
         options: WriteOptions | dict | None = None,
     ) -> None:
         write_options = self.WriteOptions.parse(options)
@@ -714,14 +720,15 @@
             # spark.sql.sources.partitionOverwriteMode=dynamic, so using insertInto instead.
             self._insert_into(df, target, options)
         else:
             # if someone needs to recreate the entire table using new set of options, like partitionBy or bucketBy,
             # mode="overwrite_table" should be used
             self._save_as_table(df, target, options)
 
+    @slot
     def read_df(
         self,
         source: str,
         columns: list[str] | None = None,
         hint: str | None = None,
         where: str | None = None,
         df_schema: StructType | None = None,
@@ -734,14 +741,15 @@
             columns=columns,
             where=where,
             hint=hint,
         )
 
         return self.sql(sql_text)
 
+    @slot
     def get_df_schema(
         self,
         source: str,
         columns: list[str] | None = None,
     ) -> StructType:
         log.info("|%s| Fetching schema of table table %r", self.__class__.__name__, source)
         query = get_sql_query(source, columns=columns, where="1=0", compact=True)
@@ -749,14 +757,15 @@
         log.debug("|%s| Executing SQL query:", self.__class__.__name__)
         log_lines(query, level=logging.DEBUG)
 
         df = self._execute_sql(query)
         log.info("|%s| Schema fetched", self.__class__.__name__)
         return df.schema
 
+    @slot
     def get_min_max_bounds(
         self,
         source: str,
         column: str,
         expression: str | None = None,
         hint: str | None = None,
         where: str | None = None,
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/jdbc_connection.py` & `onetl-0.8.1/onetl/connection/db_connection/jdbc_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     SupportHWMExpressionStr,
     SupportWhereStr,
 )
 from onetl.connection.db_connection.dialect_mixins.support_table_with_dbschema import (
     SupportTableWithDBSchema,
 )
 from onetl.connection.db_connection.jdbc_mixin import JDBCMixin
+from onetl.hooks import slot, support_hooks
 from onetl.hwm import Statement
 from onetl.impl.generic_options import GenericOptions
 from onetl.log import log_lines, log_with_indent
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
     from pyspark.sql.types import StructType
@@ -130,15 +131,16 @@
     hash = "hash"
     mod = "mod"
 
     def __str__(self):
         return str(self.value)
 
 
-class JDBCConnection(SupportDfSchemaNone, JDBCMixin, DBConnection):  # noqa: WPS338
+@support_hooks
+class JDBCConnection(SupportDfSchemaNone, JDBCMixin, DBConnection):
     class Extra(GenericOptions):
         class Config:
             extra = "allow"
 
     class Dialect(  # noqa: WPS215
         SupportTableWithDBSchema,
         SupportColumnsList,
@@ -545,31 +547,22 @@
     port: int
     extra: Extra = Extra()
 
     @property
     def instance_url(self) -> str:
         return f"{self.__class__.__name__.lower()}://{self.host}:{self.port}"
 
-    def _query_on_executor(
-        self,
-        query: str,
-        options: ReadOptions,
-    ) -> DataFrame:
-        jdbc_params = self.options_to_jdbc_params(options)
-        jdbc_params.pop("mode", None)
-
-        return self.spark.read.jdbc(table=f"({query}) T", **jdbc_params)
-
+    @slot
     def sql(
         self,
         query: str,
         options: ReadOptions | dict | None = None,
     ) -> DataFrame:
         """
-        **Lazily** execute SELECT statement **on Spark executor** and return DataFrame.
+        **Lazily** execute SELECT statement **on Spark executor** and return DataFrame. |support_hooks|
 
         Same as ``spark.read.jdbc(query)``.
 
         .. note::
 
             This method does not support :ref:`strategy`, use :obj:`onetl.db.db_reader.db_reader.DBReader` instead
 
@@ -632,14 +625,15 @@
         log_lines(query)
 
         df = self._query_on_executor(query, self.ReadOptions.parse(options))
 
         log.info("|Spark| DataFrame successfully created from SQL statement ")
         return df
 
+    @slot
     def read_df(
         self,
         source: str,
         columns: list[str] | None = None,
         hint: str | None = None,
         where: str | None = None,
         df_schema: StructType | None = None,
@@ -679,26 +673,28 @@
         result = self.sql(query, read_options)
 
         if read_options.partition_column:
             result = result.drop(alias)
 
         return result
 
+    @slot
     def write_df(
         self,
         df: DataFrame,
         target: str,
         options: WriteOptions | dict | None = None,
     ) -> None:
         write_options = self.options_to_jdbc_params(self.WriteOptions.parse(options))
 
         log.info("|%s| Saving data to a table %r", self.__class__.__name__, target)
         df.write.jdbc(table=target, **write_options)
         log.info("|%s| Table %r successfully written", self.__class__.__name__, target)
 
+    @slot
     def get_df_schema(
         self,
         source: str,
         columns: list[str] | None = None,
         options: JDBCMixin.JDBCOptions | dict | None = None,
     ) -> StructType:
         log.info("|%s| Fetching schema of table %r", self.__class__.__name__, source)
@@ -742,14 +738,15 @@
             exclude_none=True,
         )
 
         result["properties"].pop("partitioningMode", None)
 
         return result
 
+    @slot
     def get_min_max_bounds(
         self,
         source: str,
         column: str,
         expression: str | None = None,
         hint: str | None = None,
         where: str | None = None,
@@ -785,14 +782,24 @@
 
         log.info("|Spark| Received values:")
         log_with_indent("MIN(%s) = %r", column, min_value)
         log_with_indent("MAX(%s) = %r", column, max_value)
 
         return min_value, max_value
 
+    def _query_on_executor(
+        self,
+        query: str,
+        options: ReadOptions,
+    ) -> DataFrame:
+        jdbc_params = self.options_to_jdbc_params(options)
+        jdbc_params.pop("mode", None)
+
+        return self.spark.read.jdbc(table=f"({query}) T", **jdbc_params)
+
     def _exclude_partition_options(
         self,
         options: JDBCMixin.JDBCOptions | dict | None,
         fetchsize: int,
     ) -> JDBCMixin.JDBCOptions:
         return self.JDBCOptions.parse(options).copy(
             update={"fetchsize": fetchsize},
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/jdbc_mixin.py` & `onetl-0.8.1/onetl/connection/db_connection/jdbc_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from enum import Enum, auto
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Tuple, TypeVar
 
 from pydantic import Field, SecretStr
 
 from onetl._internal import clear_statement, stringify, to_camel  # noqa: WPS436
 from onetl.exception import MISSING_JVM_CLASS_MSG
+from onetl.hooks import slot, support_hooks
 from onetl.impl import FrozenModel, GenericOptions
 from onetl.log import log_lines
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame, SparkSession
 
 log = logging.getLogger(__name__)
@@ -47,14 +48,15 @@
 
 class StatementType(Enum):
     GENERIC = auto()
     PREPARED = auto()
     CALL = auto()
 
 
+@support_hooks
 class JDBCMixin(FrozenModel):
     """
     Compatibility layer between Python and Java SQL Module.
 
     Spark does not allow to execute raw SQL/DDL/DML/etc statements, so this is a workaround.
     However, some of Spark's magic is used here, for example to convert raw ResultSet to move convenient DataFrame
     """
@@ -103,17 +105,18 @@
     _last_connection_and_options: Optional[Tuple[Any, JDBCOptions]] = None
 
     @property
     @abstractmethod
     def jdbc_url(self) -> str:
         """JDBC Connection URL"""
 
+    @slot
     def close(self):
         """
-        Close all connections, opened by ``.fetch()``, ``.execute()`` or ``.check()`` methods.
+        Close all connections, opened by ``.fetch()``, ``.execute()`` or ``.check()`` methods. |support_hooks|
 
         Examples
         --------
 
         Read data and close connection:
 
         .. code:: python
@@ -138,14 +141,15 @@
     def __exit__(self, _exc_type, _exc_value, _traceback):  # noqa: U101
         self.close()
 
     def __del__(self):  # noqa: WPS603
         # If current object is collected by GC, close all opened connections
         self.close()
 
+    @slot
     def check(self):
         self._check_driver_imported()
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
         self._log_parameters()  # type: ignore
 
         log.debug("|%s| Executing SQL query (on driver):", self.__class__.__name__)
         log_lines(self._check_query, level=logging.DEBUG)
@@ -155,21 +159,22 @@
             log.info("|%s| Connection is available.", self.__class__.__name__)
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise RuntimeError("Connection is unavailable") from e
 
         return self
 
+    @slot
     def fetch(
         self,
         query: str,
         options: JDBCMixin.JDBCOptions | dict | None = None,
     ) -> DataFrame:
         """
-        **Immediately** execute SELECT statement **on Spark driver** and return in-memory DataFrame.
+        **Immediately** execute SELECT statement **on Spark driver** and return in-memory DataFrame. |support_hooks|
 
         Works almost the same like :obj:`~sql`, but calls JDBC driver directly.
 
         .. warning::
 
             This function should **NOT** be used to return dataframe with large number of rows/columns,
             like ``SELECT * FROM table`` (without any filtering).
@@ -253,21 +258,22 @@
         log.info(
             "|%s| Query succeeded, resulting in-memory dataframe contains %d rows",
             self.__class__.__name__,
             df.count(),
         )
         return df
 
+    @slot
     def execute(
         self,
         statement: str,
         options: JDBCMixin.JDBCOptions | dict | None = None,
     ) -> DataFrame | None:
         """
-        **Immediately** execute DDL, DML or procedure/function **on Spark driver**.
+        **Immediately** execute DDL, DML or procedure/function **on Spark driver**. |support_hooks|
 
         Returns DataFrame only if input is DML statement with ``RETURNING ...`` clause, or a procedure/function call.
         In other cases returns ``None``.
 
         There is no method like this in :obj:`pyspark.sql.SparkSession` object,
         but Spark internal methods works almost the same (but on executor side).
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/mongodb.py` & `onetl-0.8.1/onetl/connection/db_connection/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     SupportDfSchemaStruct,
     SupportHWMExpressionNone,
 )
 from onetl.connection.db_connection.dialect_mixins.support_table_without_dbschema import (
     SupportTableWithoutDBSchema,
 )
 from onetl.exception import MISSING_JVM_CLASS_MSG
+from onetl.hooks import slot, support_hooks
 from onetl.hwm import Statement
 from onetl.impl import GenericOptions
 from onetl.log import log_dataframe_schema, log_json, log_options, log_with_indent
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
     from pyspark.sql.types import StructType
@@ -153,16 +154,17 @@
         "shardKey",
         "forceInsert",
         "ordered",
     ),
 )
 
 
+@support_hooks
 class MongoDB(DBConnection):
-    """MongoDB connection.
+    """MongoDB connection. |support_hooks|
 
     Based on package ``org.mongodb.spark:mongo-spark-connector``
     (`MongoDB connector for Spark <https://www.mongodb.com/docs/spark-connector/current/>`_)
 
     .. dropdown:: Version compatibility
 
         * MongoDB server versions: 4.0 or higher
@@ -179,15 +181,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of MongoDB. For example: ``test.mongodb.com`` or ``193.168.1.17``.
@@ -524,23 +526,24 @@
                     )
                 if key in _upper_level_operators:  # noqa: WPS220
                     raise ValueError(  # noqa: WPS220
                         f"An invalid parameter {key!r} was specified in the 'where' "
                         "field. You cannot use aggregations or 'groupBy' clauses in 'where'",
                     )
 
+    @slot
     def pipeline(
         self,
         collection: str,
         pipeline: dict | list[dict],
         df_schema: StructType | None = None,
         options: PipelineOptions | dict | None = None,
     ):
         """
-        Execute a pipeline for a specific collection, and return DataFrame.
+        Execute a pipeline for a specific collection, and return DataFrame. |support_hooks|
 
         Almost like `Aggregation pipeline syntax <https://www.mongodb.com/docs/manual/core/aggregation-pipeline/>`_
         in MongoDB:
 
         .. code:: js
 
             db.collection.aggregate([{"$match": ...}, {"$group": ...}])
@@ -667,14 +670,15 @@
 
         return spark_reader.load()
 
     @property
     def instance_url(self) -> str:
         return f"{self.__class__.__name__.lower()}://{self.host}:{self.port}/{self.database}"
 
+    @slot
     def check(self):
         self._check_driver_imported()
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
         self._log_parameters()
 
         try:
             jvm = self.spark._sc._gateway.jvm  # type: ignore
@@ -683,14 +687,15 @@
             log.info("|%s| Connection is available.", self.__class__.__name__)
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise RuntimeError("Connection is unavailable") from e
 
         return self
 
+    @slot
     def get_min_max_bounds(
         self,
         source: str,
         column: str,
         expression: str | None = None,  # noqa: U100
         hint: dict | None = None,  # noqa: U100
         where: dict | None = None,
@@ -728,14 +733,15 @@
 
         log.info("|Spark| Received values:")
         log_with_indent("MIN(%s) = %r", column, min_value)
         log_with_indent("MAX(%s) = %r", column, max_value)
 
         return min_value, max_value
 
+    @slot
     def read_df(
         self,
         source: str,
         columns: list[str] | None = None,
         hint: dict | None = None,
         where: dict | None = None,
         df_schema: StructType | None = None,
@@ -775,14 +781,15 @@
 
         if columns:
             df = df.select(*columns)
 
         log.info("|Spark| DataFrame successfully created from SQL statement ")
         return df
 
+    @slot
     def write_df(
         self,
         df: DataFrame,
         target: str,
         options: WriteOptions | dict | None = None,
     ) -> None:
         self._check_driver_imported()
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/mssql.py` & `onetl-0.8.1/onetl/connection/db_connection/mssql.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from onetl.connection.db_connection.jdbc_connection import JDBCConnection
 
 # do not import PySpark here, as we allow user to use `MSSQL.package` for creating Spark session
 
 
 class MSSQL(JDBCConnection):
-    """MSSQL JDBC connection.
+    """MSSQL JDBC connection. |support_hooks|
 
     Based on Maven package ``com.microsoft.sqlserver:mssql-jdbc:12.2.0.jre8``
     (`official MSSQL JDBC driver
     <https://docs.microsoft.com/en-us/sql/connect/jdbc/download-microsoft-jdbc-driver-for-sql-server>`_).
 
     .. dropdown:: Version compatibility
 
@@ -46,15 +46,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of MSSQL database. For example: ``test.mssql.domain.com`` or ``192.168.1.14``
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/mysql.py` & `onetl-0.8.1/onetl/connection/db_connection/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from onetl.connection.db_connection.jdbc_connection import JDBCConnection
 
 # do not import PySpark here, as we allow user to use `MySQL.package` for creating Spark session
 
 
 class MySQL(JDBCConnection):
-    """MySQL JDBC connection.
+    """MySQL JDBC connection. |support_hooks|
 
     Based on Maven package ``com.mysql:mysql-connector-j:8.0.33``
     (`official MySQL JDBC driver <https://dev.mysql.com/downloads/connector/j/8.0.html>`_).
 
     .. dropdown:: Version compatibility
 
         * MySQL server versions: 5.7, 8.0
@@ -44,15 +44,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of MySQL database. For example: ``mysql0012.domain.com`` or ``192.168.1.11``
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/oracle.py` & `onetl-0.8.1/onetl/connection/db_connection/oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from textwrap import indent
 from typing import TYPE_CHECKING, ClassVar, Optional
 
 from pydantic import root_validator
 
 from onetl._internal import clear_statement  # noqa: WPS436
 from onetl.connection.db_connection.jdbc_connection import JDBCConnection
+from onetl.hooks import slot, support_hooks
 from onetl.log import BASE_LOG_INDENT, log_lines
 
 # do not import PySpark here, as we allow user to use `Oracle.package` for creating Spark session
 
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
@@ -57,16 +58,17 @@
 
     @property
     def sort_key(self) -> tuple[int, int, int]:
         # Sort results by priority (``ERROR``, then ``WARNING``), line, position (symbol)
         return 100 - self.level, self.line, self.position
 
 
+@support_hooks
 class Oracle(JDBCConnection):
-    """Oracle JDBC connection.
+    """Oracle JDBC connection. |support_hooks|
 
     Based on Maven package ``com.oracle.database.jdbc:ojdbc8:23.2.0.0``
     (`official Oracle JDBC driver <https://www.oracle.com/cis/database/technologies/appdev/jdbc-downloads.html>`_).
 
     .. dropdown:: Version compatibility
 
         * Oracle Server versions: 23c, 21c, 19c, 18c, 12.2 and probably 11.2 (tested, but that's not official).
@@ -83,15 +85,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Oracle database. For example: ``test.oracle.domain.com`` or ``193.168.1.10``
@@ -219,14 +221,15 @@
     @property
     def instance_url(self) -> str:
         if self.sid:
             return f"{super().instance_url}/{self.sid}"
 
         return f"{super().instance_url}/{self.service_name}"
 
+    @slot
     def execute(
         self,
         statement: str,
         options: Oracle.JDBCOptions | dict | None = None,  # noqa: WPS437
     ) -> DataFrame | None:
         statement = clear_statement(statement)
 
@@ -352,15 +355,15 @@
         """
         Oracle does not return compilation errors immediately.
         Instead, user should call "SHOW ERRORS" statement to get the message. But it cannot be called via JDBC.
 
         So this method is fetching errors from the system views:
         1. ``SELECT * FROM ALL_ERRORS``
         2. Parse resulting dataframe into list of compilation errors
-        3. Generage error message from errors list
+        3. Generate error message from errors list
         4. If there are records with ``ERROR`` level, method throws ValueError, otherwise prints warning to log
         """
 
         parsed_statement = self._parse_create_statement(statement)
         if not parsed_statement:
             return
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/postgres.py` & `onetl-0.8.1/onetl/connection/db_connection/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from onetl.connection.db_connection.jdbc_connection import JDBCConnection
 
 # do not import PySpark here, as we allow user to use `Postgres.package` for creating Spark session
 
 
 class Postgres(JDBCConnection):
-    """PostgreSQL JDBC connection.
+    """PostgreSQL JDBC connection. |support_hooks|
 
     Based on Maven package ``org.postgresql:postgresql:42.6.0``
     (`official Postgres JDBC driver <https://jdbc.postgresql.org/>`_).
 
     .. dropdown:: Version compatibility
 
         * PostgreSQL server versions: 8.2 or higher
@@ -55,15 +55,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Postgres database. For example: ``test.postgres.domain.com`` or ``193.168.1.11``
```

### Comparing `onetl-0.8.0/onetl/connection/db_connection/teradata.py` & `onetl-0.8.1/onetl/connection/db_connection/teradata.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from onetl.connection.db_connection.jdbc_connection import JDBCConnection
 
 # do not import PySpark here, as we allow user to use `Teradata.package` for creating Spark session
 
 
 class Teradata(JDBCConnection):
-    """Teradata JDBC connection.
+    """Teradata JDBC connection. |support_hooks|
 
     Based on package ``com.teradata.jdbc:terajdbc:17.20.00.15``
     (`official Teradata JDBC driver <https://downloads.teradata.com/download/connectivity/jdbc-driver>`_).
 
     .. dropdown:: Version compatibility
 
         * Teradata server versions: 16.10 - 20.0
@@ -44,15 +44,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.0  # pass specific PySpark version
+            pip install onetl pyspark=3.4.1  # pass specific PySpark version
 
         See :ref:`spark-install` instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Teradata database. For example: ``test.teradata.domain.com`` or ``193.168.1.12``
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/file_connection.py` & `onetl-0.8.1/onetl/connection/file_connection/file_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import os
+import threading
 from abc import abstractmethod
 from logging import getLogger
 from typing import Any, Iterable, Iterator
 
 from humanize import naturalsize
 
 from onetl.base import (
@@ -31,39 +32,54 @@
     DirectoryNotEmptyError,
     DirectoryNotFoundError,
     FileSizeMismatchError,
     NotAFileError,
 )
 from onetl.file.filter import match_all_filters
 from onetl.file.limit import limits_reached, limits_stop_at, reset_limits
+from onetl.hooks import slot, support_hooks
 from onetl.impl import (
     FrozenModel,
     LocalPath,
     RemoteDirectory,
     RemoteFile,
     RemotePath,
     path_repr,
 )
 from onetl.log import log_with_indent
 
 log = getLogger(__name__)
 
 
+@support_hooks
 class FileConnection(BaseFileConnection, FrozenModel):
-    _client: Any = None
+    _clients_cache: Any = None
 
     @property
     def client(self):
-        if self._client and not self._is_client_closed():
-            return self._client
+        """
+        Return underlying client object.
+
+        Client object is cached (for performance reasons).
+        Each thread receives its own client instance.
 
-        client = self._get_client()
-        self._client = client
-        return client
+        If client is closed, new client is created.
+        """
+        if self._clients_cache is None:
+            self._clients_cache = threading.local()
+
+        try:
+            client = self._clients_cache.client
+            if client and not self._is_client_closed(client):
+                return client
+        except AttributeError:
+            self._clients_cache.client = self._get_client()
+            return self._clients_cache.client
 
+    @slot
     def close(self):
         """
         Close all connections, opened by other methods call.
 
         Examples
         --------
 
@@ -79,25 +95,29 @@
 
             with connection:
                 content = connection.list_dir("/mydir")
                 content = connection.list_dir("/mydir/abc")
 
         """
 
-        if self._client:
-            self._close_client()
+        try:
+            client = self._clients_cache.client
+        except AttributeError:
+            return
 
-        self._client = None
+        self._close_client(client)
+        del self._clients_cache.client
 
     def __enter__(self):
         return self
 
     def __exit__(self, _exc_type, _exc_value, _traceback):
         self.close()
 
+    @slot
     def check(self):
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
         self._log_parameters()
 
         try:
             self.list_dir("/")
             log.info("|%s| Connection is available", self.__class__.__name__)
@@ -107,73 +127,81 @@
             raise
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise RuntimeError("Connection is unavailable") from e
 
         return self
 
+    @slot
     def is_file(self, path: os.PathLike | str) -> bool:
         remote_path = RemotePath(path)
 
         if not self.path_exists(remote_path):
             raise FileNotFoundError(f"File '{remote_path}' does not exist")
 
         return self._is_file(remote_path)
 
+    @slot
     def is_dir(self, path: os.PathLike | str) -> bool:
         remote_path = RemotePath(path)
 
         if not self.path_exists(remote_path):
             raise DirectoryNotFoundError(f"Directory '{remote_path}' does not exist")
 
         return self._is_dir(remote_path)
 
+    @slot
     def get_stat(self, path: os.PathLike | str) -> PathStatProtocol:
         remote_path = RemotePath(path)
         return self._get_stat(remote_path)
 
+    @slot
     def resolve_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         is_dir = self.is_dir(path)
         stat = self.get_stat(path)
 
         if not is_dir:
             raise NotADirectoryError(
                 f"{path_repr(RemoteFile(path, stats=stat))} is not a directory",
             )
 
         return RemoteDirectory(path=path, stats=stat)
 
+    @slot
     def resolve_file(self, path: os.PathLike | str) -> RemoteFile:
         is_file = self.is_file(path)
         stat = self.get_stat(path)
         remote_path = RemoteFile(path=path, stats=stat)
 
         if not is_file:
             raise NotAFileError(f"{path_repr(remote_path)} is not a file")
 
         return remote_path
 
+    @slot
     def read_text(self, path: os.PathLike | str, encoding: str = "utf-8", **kwargs) -> str:
         log.debug(
             "|%s| Reading string with encoding %r and options %r from '%s'",
             self.__class__.__name__,
             encoding,
             kwargs,
             path,
         )
 
         remote_path = self.resolve_file(path)
         return self._read_text(remote_path, encoding=encoding, **kwargs)
 
+    @slot
     def read_bytes(self, path: os.PathLike | str, **kwargs) -> bytes:
         log.debug("|%s| Reading bytes with options %r from '%s'", self.__class__.__name__, kwargs, path)
 
         remote_path = self.resolve_file(path)
         return self._read_bytes(remote_path, **kwargs)
 
+    @slot
     def write_text(self, path: os.PathLike | str, content: str, encoding: str = "utf-8", **kwargs) -> RemoteFile:
         if not isinstance(content, str):
             raise TypeError(f"content must be str, not '{content.__class__.__name__}'")
 
         log.debug(
             "|%s| Writing string size %d with encoding %r and options %r to '%s'",
             self.__class__.__name__,
@@ -194,14 +222,15 @@
                 path_repr(file),
             )
 
         self._write_text(remote_path, content=content, encoding=encoding, **kwargs)
 
         return self.resolve_file(remote_path)
 
+    @slot
     def write_bytes(self, path: os.PathLike | str, content: bytes, **kwargs) -> RemoteFile:
         if not isinstance(content, bytes):
             raise TypeError(f"content must be bytes, not '{content.__class__.__name__}'")
 
         log.debug(
             "|%s| Writing %s with options %e to '%s'",
             self.__class__.__name__,
@@ -221,14 +250,15 @@
                 path_repr(file),
             )
 
         self._write_bytes(remote_path, content=content, **kwargs)
 
         return self.resolve_file(remote_path)
 
+    @slot
     def download_file(
         self,
         remote_file_path: os.PathLike | str,
         local_file_path: os.PathLike | str,
         replace: bool = True,
     ) -> LocalPath:
         log.debug(
@@ -260,39 +290,42 @@
                 f"The size of the downloaded file ({naturalsize(local_file.stat().st_size)}) does not match "
                 f"the size of the file on the source ({naturalsize(remote_file.stat().st_size)})",
             )
 
         log.info("|Local FS| Successfully downloaded file '%s'", local_file)
         return local_file
 
+    @slot
     def remove_file(self, path: os.PathLike | str) -> bool:
         log.debug("|%s| Removing file '%s'", self.__class__.__name__, path)
 
         if not self.path_exists(path):
             log.debug("|%s| File '%s' does not exist, nothing to remove", self.__class__.__name__, path)
             return False
 
         file = self.resolve_file(path)
         log.debug("|%s| File to remove: %s", self.__class__.__name__, path_repr(file))
 
         self._remove_file(file)
         log.info("|%s| Successfully removed file '%s'", self.__class__.__name__, file)
         return True
 
+    @slot
     def create_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         log.debug("|%s| Creating directory '%s'", self.__class__.__name__, path)
         remote_dir = RemotePath(path)
 
         if self.path_exists(remote_dir):
             return self.resolve_dir(remote_dir)
 
         self._create_dir(remote_dir)
         log.info("|%s| Successfully created directory '%s'", self.__class__.__name__, remote_dir)
         return self.resolve_dir(remote_dir)
 
+    @slot
     def upload_file(
         self,
         local_file_path: os.PathLike | str,
         remote_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> RemoteFile:
         log.debug("|%s| Uploading local file '%s' to '%s'", self.__class__.__name__, local_file_path, remote_file_path)
@@ -323,14 +356,15 @@
                 f"The size of the uploaded file ({naturalsize(result.stat().st_size)}) does not match "
                 f"the size of the file on the source ({naturalsize(local_file.stat().st_size)})",
             )
 
         log.info("|%s| Successfully uploaded file '%s'", self.__class__.__name__, remote_file)
         return result
 
+    @slot
     def rename_file(
         self,
         source_file_path: os.PathLike | str,
         target_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> RemoteFile:
         log.debug("|%s| Renaming file '%s' to '%s'", self.__class__.__name__, source_file_path, target_file_path)
@@ -348,14 +382,15 @@
 
         self.create_dir(target_file.parent)
         self._rename_file(source_file, target_file)
         log.info("|%s| Successfully renamed file '%s' to '%s'", self.__class__.__name__, source_file, target_file)
 
         return self.resolve_file(target_file)
 
+    @slot
     def list_dir(
         self,
         path: os.PathLike | str,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> list[RemoteDirectory | RemoteFile]:
         log.debug("|%s| Listing directory '%s'", self.__class__.__name__, path)
@@ -378,27 +413,29 @@
                 result.append(path)
 
             if limits_stop_at(path, limits):
                 break
 
         return result
 
+    @slot
     def walk(
         self,
         root: os.PathLike | str,
         topdown: bool = True,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> Iterator[tuple[RemoteDirectory, list[RemoteDirectory], list[RemoteFile]]]:
         root_dir = self.resolve_dir(root)
 
         filters = filters or []
         limits = reset_limits(limits or [])
         yield from self._walk(root_dir, topdown=topdown, filters=filters, limits=limits)
 
+    @slot
     def remove_dir(self, path: os.PathLike | str, recursive: bool = False) -> bool:
         description = "RECURSIVELY" if recursive else "NON-recursively"
         log.debug("|%s| %s removing directory '%s'", self.__class__.__name__, description, path)
         remote_dir = RemotePath(path)
 
         if not self.path_exists(remote_dir):
             log.debug(
@@ -680,23 +717,32 @@
             if isinstance(value, os.PathLike):
                 log_with_indent("%s = %s", attr, path_repr(value))
             else:
                 log_with_indent("%s = %r", attr, value)
 
     @abstractmethod
     def _get_client(self) -> Any:
-        """"""
+        """
+        Create and return underlying client.
+        """
 
     @abstractmethod
-    def _is_client_closed(self) -> bool:
-        """"""
+    def _is_client_closed(self, client: Any) -> bool:
+        """
+        Check if client is closed.
+
+        Returns ``False`` if client does not support closing,
+        or bool indicating if client is closed or not.
+        """
 
     @abstractmethod
-    def _close_client(self) -> None:
-        """"""
+    def _close_client(self, client: Any) -> None:
+        """
+        Close client if it is supported.
+        """
 
     @abstractmethod
     def _download_file(self, remote_file_path: RemotePath, local_file_path: LocalPath) -> None:
         """"""
 
     @abstractmethod
     def _get_stat(self, path: RemotePath) -> PathStatProtocol:
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/ftp.py` & `onetl-0.8.1/onetl/connection/file_connection/ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from etl_entities.instance import Host
 from pydantic import SecretStr
 
 from onetl.base import PathStatProtocol
 from onetl.connection.file_connection.file_connection import FileConnection
 from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.hooks import slot, support_hooks
 from onetl.impl import LocalPath, RemotePath
 from onetl.impl.remote_path_stat import RemotePathStat
 
 try:
     from ftputil import FTPHost
     from ftputil import session as ftp_session
 except (ImportError, NameError) as e:
@@ -46,16 +47,17 @@
             """,
         ).strip(),
     ) from e
 
 log = getLogger(__name__)
 
 
+@support_hooks
 class FTP(FileConnection, RenameDirMixin):
-    """FTP file connection.
+    """FTP file connection. |support_hooks|
 
     Based on `FTPUtil library <https://pypi.org/project/ftputil/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use FTP connector you should install package as follows:
 
@@ -107,14 +109,15 @@
     user: Optional[str] = None
     password: Optional[SecretStr] = None
 
     @property
     def instance_url(self) -> str:
         return f"ftp://{self.host}:{self.port}"
 
+    @slot
     def path_exists(self, path: os.PathLike | str) -> bool:
         return self.client.path.exists(os.fspath(path))
 
     def _get_client(self) -> FTPHost:
         """
         Returns a FTP connection object
         """
@@ -129,19 +132,19 @@
         return FTPHost(
             self.host,
             self.user,
             self.password.get_secret_value() if self.password else None,
             session_factory=session_factory,
         )
 
-    def _is_client_closed(self) -> bool:
-        return self._client.closed
+    def _is_client_closed(self, client: FTPHost) -> bool:
+        return client.closed
 
-    def _close_client(self) -> None:
-        self._client.close()
+    def _close_client(self, client: FTPHost) -> None:
+        client.close()
 
     def _remove_dir(self, path: RemotePath) -> None:
         self.client.rmdir(os.fspath(path))
 
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         self.client.upload(os.fspath(local_file_path), os.fspath(remote_file_path))
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/ftps.py` & `onetl-0.8.1/onetl/connection/file_connection/ftps.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 server_hostname=self.host,
                 session=self.sock.session,
             )  # this is the fix
         return conn, size
 
 
 class FTPS(FTP):
-    """FTPS file connection.
+    """FTPS file connection. |support_hooks|
 
     Based on `FTPUtil library <https://pypi.org/project/ftputil/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use FTPS connector you should install package as follows:
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/hdfs.py` & `onetl-0.8.1/onetl/connection/file_connection/hdfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from onetl.connection.file_connection.file_connection import FileConnection
 from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
 from onetl.connection.kerberos_helpers import kinit
 from onetl.hooks import slot, support_hooks
 from onetl.impl import LocalPath, RemotePath, RemotePathStat
 
 try:
-    from hdfs import InsecureClient
+    from hdfs import Client, InsecureClient
 
     if TYPE_CHECKING:
         from hdfs.ext.kerberos import KerberosClient
 except (ImportError, NameError) as err:
     raise ImportError(
         textwrap.dedent(
             """
@@ -50,16 +50,17 @@
         ).strip(),
     ) from err
 
 log = getLogger(__name__)
 ENTRY_TYPE = Tuple[str, dict]
 
 
+@support_hooks
 class HDFS(FileConnection, RenameDirMixin):
-    """HDFS file connection.
+    """HDFS file connection. |support_hooks|
 
     Powered by `HDFS Python client <https://pypi.org/project/hdfs/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use HDFS connector you should install package as follows:
 
@@ -569,18 +570,19 @@
             raise ValueError("Please provide either `keytab` or `password` for kinit, not both")
 
         if (password or keytab) and not user:
             raise ValueError("`keytab` or `password` should be used only with `user`")
 
         return values
 
+    @slot
     @classmethod
     def get_current(cls, **kwargs):
         """
-        Create connection for current cluster.
+        Create connection for current cluster. |support_hooks|
 
         Automatically sets up current cluster name as ``cluster``.
 
         .. note::
 
             Can be used only if there are a some hooks bound to slot :obj:`~slots.get_current_cluster`.
 
@@ -617,14 +619,15 @@
 
     @property
     def instance_url(self) -> str:
         if self.cluster:
             return self.cluster
         return f"hdfs://{self.host}:{self.webhdfs_port}"
 
+    @slot
     def path_exists(self, path: os.PathLike | str) -> bool:
         return self.client.status(os.fspath(path), strict=False)
 
     def _get_active_namenode(self) -> str:
         class_name = self.__class__.__name__
         log.info("|%s| Detecting active namenode of cluster %r ...", class_name, self.cluster)
 
@@ -669,40 +672,38 @@
             return self.host
 
         if self.cluster:
             raise RuntimeError(f"Host {self.host!r} is not an active namenode of cluster {self.cluster!r}")
 
         raise RuntimeError(f"Host {self.host!r} is not an active namenode")
 
-    def _get_client(self) -> KerberosClient | InsecureClient:
+    def _get_client(self) -> Client:
         host = self._get_host()
         conn_str = f"http://{host}:{self.webhdfs_port}"  # NOSONAR
 
         if self.user and (self.keytab or self.password):
-            from hdfs.ext.kerberos import KerberosClient
+            from hdfs.ext.kerberos import KerberosClient  # noqa: F811
 
             kinit(
                 self.user,
                 keytab=self.keytab,
                 password=self.password.get_secret_value() if self.password else None,
             )
             client = KerberosClient(conn_str, timeout=self.timeout)
         else:
-            from hdfs import InsecureClient  # noqa: F401, WPS442
+            from hdfs import InsecureClient  # noqa: F401, WPS442, F811
 
             client = InsecureClient(conn_str, user=self.user)
 
         return client
 
-    def _is_client_closed(self) -> bool:
-        # Underlying client does not support closing
+    def _is_client_closed(self, client: Client):
         return False
 
-    def _close_client(self) -> None:  # NOSONAR
-        # Underlying client does not support closing
+    def _close_client(self, client: Client) -> None:  # NOSONAR
         pass
 
     def _remove_dir(self, path: RemotePath) -> None:
         self.client.delete(os.fspath(path), recursive=False)
 
     def _create_dir(self, path: RemotePath) -> None:
         self.client.makedirs(os.fspath(path))
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/mixins/rename_dir_mixin.py` & `onetl-0.8.1/onetl/connection/file_connection/mixins/rename_dir_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,14 @@
                 raise DirectoryExistsError(f"Directory {path_repr(directory)} already exists")
 
             log.warning("|%s| Directory %s already exists, removing", self.__class__.__name__, path_repr(directory))
             self.remove_dir(target_dir, recursive=True)
 
         self.create_dir(target_dir.parent)
         self._rename_dir(source_dir, target_dir)
-        log.info("|%s| Successfully renamed file '%s' to '%s'", self.__class__.__name__, source_dir, target_dir)
+        log.info("|%s| Successfully renamed directory '%s' to '%s'", self.__class__.__name__, source_dir, target_dir)
 
         return self.resolve_dir(target_dir)
 
     @abstractmethod
     def _rename_dir(self, source: RemotePath, target: RemotePath) -> None:
         ...
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/s3.py` & `onetl-0.8.1/onetl/connection/file_connection/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 from __future__ import annotations
 
 import io
 import os
 import textwrap
 from logging import getLogger
-from typing import Any, Optional, Union
+from typing import Optional, Union
+
+from onetl.hooks import slot, support_hooks
 
 try:
     from minio import Minio, commonconfig
     from minio.datatypes import Object
 except (ImportError, NameError) as e:
     raise ImportError(
         textwrap.dedent(
@@ -44,16 +46,17 @@
 
 from onetl.connection.file_connection.file_connection import FileConnection
 from onetl.impl import LocalPath, RemoteDirectory, RemotePath, RemotePathStat
 
 log = getLogger(__name__)
 
 
+@support_hooks
 class S3(FileConnection):
-    """S3 file connection.
+    """S3 file connection. |support_hooks|
 
     Based on `minio-py client <https://pypi.org/project/minio/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use S3 connector you should install package as follows:
 
@@ -127,56 +130,58 @@
         values["port"] = 443 if values["protocol"] == "https" else 80
         return values
 
     @property
     def instance_url(self) -> str:
         return f"s3://{self.host}:{self.port}"
 
+    @slot
     def create_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         # the method is overridden because S3 does not create a directory
         # and the method must return the created directory
 
         log.debug("|%s| Creating directory '%s'", self.__class__.__name__, path)
         remote_directory = RemotePath(path)
 
         if self.path_exists(remote_directory):
             return self.resolve_dir(remote_directory)
 
         self._create_dir(remote_directory)
         log.info("|%s| Successfully created directory '%s'", self.__class__.__name__, remote_directory)
         return RemoteDirectory(path=remote_directory, stats=RemotePathStat())
 
+    @slot
     def path_exists(self, path: os.PathLike | str) -> bool:
         remote_path = RemotePath(os.fspath(path))
         if self._is_root(remote_path):
             return True
 
         remote_path_str = self._delete_absolute_path_slash(remote_path)
         for component in self.client.list_objects(self.bucket, prefix=remote_path_str):
             component_path = RemotePath(component.object_name)
             component_path_str = self._delete_absolute_path_slash(component_path)
             if component_path_str == remote_path_str:
                 return True
 
         return False
 
-    def _get_client(self) -> Any:
+    def _get_client(self) -> Minio:
         return Minio(
             endpoint=f"{self.host}:{self.port}",
             access_key=self.access_key,
             secret_key=self.secret_key.get_secret_value(),
             secure=self.protocol == "https",
             session_token=self.session_token.get_secret_value() if self.session_token else None,
             region=self.region,
         )
 
-    def _is_client_closed(self) -> bool:
-        return True
+    def _is_client_closed(self, client: Minio):
+        return False
 
-    def _close_client(self) -> None:
+    def _close_client(self, client: Minio) -> None:  # NOSONAR
         pass
 
     @staticmethod
     def _is_root(path: RemotePath) -> bool:
         return path.name == ""
 
     @classmethod
@@ -228,15 +233,15 @@
             source=commonconfig.CopySource(self.bucket, source_str),
         )
 
         self._remove_file(source)
 
     def _scan_entries(self, path: RemotePath) -> list[Object]:
         if self._is_root(path):
-            self.client.list_objects(self.bucket)
+            return self.client.list_objects(self.bucket)
 
         path_str = self._delete_absolute_path_slash(path)
         return self.client.list_objects(self.bucket, prefix=path_str + "/")
 
     def _extract_name_from_entry(self, entry: Object) -> str:
         return RemotePath(entry.object_name).name
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/sftp.py` & `onetl-0.8.1/onetl/connection/file_connection/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from typing import Optional
 
 from etl_entities.instance import Host
 from pydantic import FilePath, SecretStr
 
 from onetl.connection.file_connection.file_connection import FileConnection
 from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.hooks import slot, support_hooks
 from onetl.impl import LocalPath, RemotePath
 
 try:
     from paramiko import ProxyCommand, SSHClient, SSHConfig, WarningPolicy
     from paramiko.sftp_attr import SFTPAttributes
     from paramiko.sftp_client import SFTPClient
     from paramiko.ssh_exception import ConfigParseError
@@ -49,16 +50,17 @@
     ) from e
 
 SSH_CONFIG_PATH = LocalPath("~/.ssh/config").expanduser().resolve()
 
 log = getLogger(__name__)
 
 
+@support_hooks
 class SFTP(FileConnection, RenameDirMixin):
-    """SFTP file connection.
+    """SFTP file connection. |support_hooks|
 
     Based on `Paramiko library <https://pypi.org/project/paramiko/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use SFTP connector you should install package as follows:
 
@@ -122,14 +124,15 @@
     host_key_check: bool = False
     compress: bool = True
 
     @property
     def instance_url(self) -> str:
         return f"sftp://{self.host}:{self.port}"
 
+    @slot
     def path_exists(self, path: os.PathLike | str) -> bool:
         try:
             self.client.stat(os.fspath(path))
             return True
         except FileNotFoundError:
             return False
 
@@ -151,19 +154,19 @@
             timeout=self.timeout,
             compress=self.compress,
             sock=host_proxy,
         )
 
         return client.open_sftp()
 
-    def _is_client_closed(self) -> bool:
-        return not self._client.sock or self._client.sock.closed
+    def _is_client_closed(self, client: SFTPClient) -> bool:
+        return not client.sock or client.sock.closed
 
-    def _close_client(self) -> None:
-        self._client.close()
+    def _close_client(self, client: SFTPClient) -> None:
+        client.close()
 
     def _parse_user_ssh_config(self) -> tuple[str | None, str | None]:
         host_proxy = None
         key_file = os.fspath(self.key_file) if self.key_file else None
 
         if not SSH_CONFIG_PATH.exists() or not SSH_CONFIG_PATH.is_file():
             return host_proxy, key_file
```

### Comparing `onetl-0.8.0/onetl/connection/file_connection/webdav.py` & `onetl-0.8.1/onetl/connection/file_connection/webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 import datetime
 import io
 import os
 import stat
 import textwrap
 from logging import getLogger
 from ssl import SSLContext
-from typing import Any, Optional, Union
+from typing import Optional, Union
 
 from etl_entities.instance import Host
 from pydantic import DirectoryPath, FilePath, SecretStr, root_validator
 from typing_extensions import Literal
 
 from onetl.connection.file_connection.file_connection import FileConnection
 from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.hooks import slot, support_hooks
 from onetl.impl import LocalPath, RemotePath, RemotePathStat
 
 try:
     from webdav3.client import Client
 except (ImportError, NameError) as e:
     raise ImportError(
         textwrap.dedent(
@@ -48,16 +49,17 @@
         ).strip(),
     ) from e
 
 log = getLogger(__name__)
 DATA_MODIFIED_FORMAT = "%a, %d %b %Y %H:%M:%S GMT"
 
 
+@support_hooks
 class WebDAV(FileConnection, RenameDirMixin):
-    """WebDAV file connection.
+    """WebDAV file connection. |support_hooks|
 
     Based on `WebdavClient3 library <https://pypi.org/project/webdavclient3/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use WebDAV connector you should install package as follows:
 
@@ -131,33 +133,34 @@
 
         return values
 
     @property
     def instance_url(self) -> str:
         return f"webdav://{self.host}:{self.port}"
 
+    @slot
     def path_exists(self, path: os.PathLike | str) -> bool:
         return self.client.check(os.fspath(path))
 
-    def _get_client(self) -> Any:
+    def _get_client(self) -> Client:
         options = {
             "webdav_hostname": f"{self.protocol}://{self.host}:{self.port}",
             "webdav_login": self.user,
             "webdav_password": self.password.get_secret_value(),
         }
 
         client = Client(options)
         client.verify = self.ssl_verify
 
         return client
 
-    def _is_client_closed(self) -> bool:
-        pass
+    def _is_client_closed(self, client: Client):
+        return False
 
-    def _close_client(self) -> None:
+    def _close_client(self, client: Client) -> None:  # NOSONAR
         pass
 
     def _download_file(self, remote_file_path: RemotePath, local_file_path: LocalPath) -> None:
         self.client.download_sync(
             remote_path=os.fspath(remote_file_path),
             local_path=os.fspath(local_file_path),
         )
```

### Comparing `onetl-0.8.0/onetl/connection/kerberos_helpers.py` & `onetl-0.8.1/onetl/connection/kerberos_helpers.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/core/__init__.py` & `onetl-0.8.1/onetl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/core/file_filter/__init__.py` & `onetl-0.8.1/onetl/core/file_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/core/file_filter/file_filter.py` & `onetl-0.8.1/onetl/core/file_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/core/file_limit/__init__.py` & `onetl-0.8.1/onetl/core/file_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/core/file_limit/file_limit.py` & `onetl-0.8.1/onetl/core/file_limit/file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/db/__init__.py` & `onetl-0.8.1/onetl/db/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/db/db_reader/__init__.py` & `onetl-0.8.1/onetl/db/db_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/db/db_reader/db_reader.py` & `onetl-0.8.1/onetl/db/db_reader/db_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import frozendict
 from etl_entities import Column, Table
 from pydantic import Field, root_validator, validator
 
 from onetl._internal import uniq_ignore_case  # noqa: WPS436
 from onetl.base import BaseDBConnection
 from onetl.base.contains_get_df_schema import ContainsGetDFSchemaMethod
+from onetl.hooks import slot, support_hooks
 from onetl.impl import FrozenModel, GenericOptions
 from onetl.log import (
     entity_boundary_log,
     log_collection,
     log_dataframe_schema,
     log_json,
     log_options,
@@ -24,17 +25,18 @@
 log = getLogger(__name__)
 
 if TYPE_CHECKING:
     from pyspark.sql.dataframe import DataFrame
     from pyspark.sql.types import StructType
 
 
+@support_hooks
 class DBReader(FrozenModel):
     """Allows you to read data from a table with specified database connection
-    and parameters, and return its content as Spark dataframe
+    and parameters, and return its content as Spark dataframe. |support_hooks|
 
     .. note::
 
         DBReader can return different results depending on :ref:`strategy`
 
     .. note::
 
@@ -483,17 +485,18 @@
             column=column,
             expression=expression,
             hint=self.hint,
             where=self.where,
             **self._get_read_kwargs(),
         )
 
+    @slot
     def run(self) -> DataFrame:
         """
-        Reads data from source table and saves as Spark dataframe.
+        Reads data from source table and saves as Spark dataframe. |support_hooks|
 
         .. note::
 
             This method can return different results depending on :ref:`strategy`
 
         Returns
         -------
```

### Comparing `onetl-0.8.0/onetl/db/db_reader/strategy_helper.py` & `onetl-0.8.1/onetl/db/db_reader/strategy_helper.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/db/db_writer/__init__.py` & `onetl-0.8.1/onetl/db/db_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/db/db_writer/db_writer.py` & `onetl-0.8.1/onetl/db/db_writer/db_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,32 @@
 from logging import getLogger
 from typing import TYPE_CHECKING, Optional
 
 from etl_entities import Table
 from pydantic import Field, validator
 
 from onetl.base import BaseDBConnection
+from onetl.hooks import slot, support_hooks
 from onetl.impl import FrozenModel, GenericOptions
 from onetl.log import (
     entity_boundary_log,
     log_dataframe_schema,
     log_options,
     log_with_indent,
 )
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
 
 log = getLogger(__name__)
 
 
+@support_hooks
 class DBWriter(FrozenModel):
-    """Class specifies schema and table where you can write your dataframe.
+    """Class specifies schema and table where you can write your dataframe. |support_hooks|
 
     Parameters
     ----------
     connection : :obj:`onetl.connection.DBConnection`
         Class which contains DB connection properties. See :ref:`db-connections` section.
 
     target : str
@@ -170,17 +172,18 @@
         if options:
             raise ValueError(
                 f"{connection.__class__.__name__} does not implement WriteOptions, but {options!r} is passed",
             )
 
         return None
 
+    @slot
     def run(self, df: DataFrame):
         """
-        Method for writing your df to specified target.
+        Method for writing your df to specified target. |support_hooks|
 
         Parameters
         ----------
         df : pyspark.sql.dataframe.DataFrame
             Spark dataframe
 
         Examples
```

### Comparing `onetl-0.8.0/onetl/exception.py` & `onetl-0.8.1/onetl/exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/__init__.py` & `onetl-0.8.1/onetl/file/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_downloader/__init__.py` & `onetl-0.8.1/onetl/file/file_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_downloader/download_result.py` & `onetl-0.8.1/onetl/file/file_downloader/download_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_downloader/file_downloader.py` & `onetl-0.8.1/onetl/file/file_downloader/file_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 import warnings
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from enum import Enum
 from typing import Iterable, List, Optional, Tuple, Type
 
 from etl_entities import HWM, FileHWM, RemoteFolder
 from ordered_set import OrderedSet
 from pydantic import Field, validator
 
 from onetl._internal import generate_temp_path  # noqa: WPS436
 from onetl.base import BaseFileConnection, BaseFileFilter, BaseFileLimit
-from onetl.base.path_protocol import PathProtocol
+from onetl.base.path_protocol import PathProtocol, PathWithStatsProtocol
+from onetl.base.pure_path_protocol import PurePathProtocol
 from onetl.file.file_downloader.download_result import DownloadResult
 from onetl.file.file_set import FileSet
 from onetl.file.filter.file_hwm import FileHWMFilter
+from onetl.hooks import slot, support_hooks
 from onetl.hwm.store import HWMClassRegistry
 from onetl.impl import (
     FailedRemoteFile,
     FileWriteMode,
     FrozenModel,
     GenericOptions,
     LocalPath,
@@ -54,17 +58,25 @@
 
 log = logging.getLogger(__name__)
 
 # source, target, temp
 DOWNLOAD_ITEMS_TYPE = OrderedSet[Tuple[RemotePath, LocalPath, Optional[LocalPath]]]
 
 
+class FileDownloadStatus(Enum):
+    SUCCESSFUL = 0
+    FAILED = 1
+    SKIPPED = 2
+    MISSING = -1
+
+
+@support_hooks
 class FileDownloader(FrozenModel):
     """Allows you to download files from a remote source with specified file connection
-    and parameters, and return an object with download result summary.
+    and parameters, and return an object with download result summary. |support_hooks|
 
     .. note::
 
         FileDownloader can return different results depending on :ref:`strategy`
 
     .. note::
 
@@ -214,30 +226,41 @@
         delete_source: bool = False
         """
         If ``True``, remove source file after successful download.
 
         If download failed, file will left intact.
         """
 
+        workers: int = Field(default=1, ge=1)
+        """
+        Number of workers to create for parallel file download.
+
+        1 (default) means files will me downloaded sequentially.
+        2 or more means files will be downloaded in parallel workers.
+
+        Recommended value is ``min(32, os.cpu_count() + 4)``, e.g. ``5``.
+        """
+
     connection: BaseFileConnection
 
     local_path: LocalPath
     source_path: Optional[RemotePath] = None
     temp_path: Optional[LocalPath] = None
 
     filters: List[BaseFileFilter] = Field(default_factory=list, alias="filter")
     limits: List[BaseFileLimit] = Field(default_factory=list, alias="limit")
 
     hwm_type: Optional[Type[FileHWM]] = None
 
     options: Options = Options()
 
+    @slot
     def run(self, files: Iterable[str | os.PathLike] | None = None) -> DownloadResult:  # noqa: WPS231
         """
-        Method for downloading files from source to local directory.
+        Method for downloading files from source to local directory. |support_hooks|
 
         .. note::
 
             This method can return different results depending on :ref:`strategy`
 
         Parameters
         ----------
@@ -385,18 +408,19 @@
 
         if current_temp_dir:
             self._remove_temp_dir(current_temp_dir)
 
         self._log_result(result)
         return result
 
+    @slot
     def view_files(self) -> FileSet[RemoteFile]:
         """
         Get file list in the ``source_path``,
-        after ``filter``, ``limit`` and ``hwm`` applied (if any).
+        after ``filter``, ``limit`` and ``hwm`` applied (if any). |support_hooks|
 
         .. note::
 
             This method can return different results depending on :ref:`strategy`
 
         Raises
         -------
@@ -588,15 +612,15 @@
             )
 
     def _validate_files(  # noqa: WPS231
         self,
         remote_files: Iterable[os.PathLike | str],
         current_temp_dir: LocalPath | None,
     ) -> DOWNLOAD_ITEMS_TYPE:
-        result = OrderedSet()
+        result: DOWNLOAD_ITEMS_TYPE = OrderedSet()
 
         for file in remote_files:
             remote_file_path = file if isinstance(file, PathProtocol) else RemotePath(file)
             remote_file = remote_file_path
             tmp_file: LocalPath | None = None
 
             if not self.source_path:
@@ -622,15 +646,15 @@
                     remote_file = self.source_path / remote_file_path
                     if current_temp_dir:
                         tmp_file = current_temp_dir / remote_file_path  # noqa: WPS220
                 else:
                     # Wrong path (not relative path and source path not in the path to the file)
                     raise ValueError(f"File path '{remote_file}' does not match source_path '{self.source_path}'")
 
-            if self.connection.path_exists(remote_file):
+            if not isinstance(remote_file, PathProtocol) and self.connection.path_exists(remote_file):
                 remote_file = self.connection.resolve_file(remote_file)
 
             result.add((remote_file, local_file, tmp_file))
 
         return result
 
     def _check_source_path(self):
@@ -642,63 +666,111 @@
 
         self.local_path.mkdir(exist_ok=True, parents=True)
 
     def _download_files(
         self,
         to_download: DOWNLOAD_ITEMS_TYPE,
     ) -> DownloadResult:
-        total_files = len(to_download)
         files = FileSet(item[0] for item in to_download)
-
         log.info("|%s| Files to be downloaded:", self.__class__.__name__)
         log_lines(str(files))
         log_with_indent("")
         log.info("|%s| Starting the download process", self.__class__.__name__)
 
+        self._create_dirs(to_download)
+
         result = DownloadResult()
-        for i, (source_file, local_file, tmp_file) in enumerate(to_download):
-            log.info("|%s| Downloading file %d of %d", self.__class__.__name__, i + 1, total_files)
-            log_with_indent("from = '%s'", source_file)
+        for status, file in self._bulk_download(to_download):
+            if status == FileDownloadStatus.SUCCESSFUL:
+                result.successful.add(file)
+            elif status == FileDownloadStatus.FAILED:
+                result.failed.add(file)
+            elif status == FileDownloadStatus.SKIPPED:
+                result.skipped.add(file)
+            elif status == FileDownloadStatus.MISSING:
+                result.missing.add(file)
+
+        return result
+
+    def _create_dirs(
+        self,
+        to_download: DOWNLOAD_ITEMS_TYPE,
+    ) -> None:
+        """
+        Create all parent paths before downloading files
+        This is required to avoid errors then multiple threads create the same dir
+        """
+        parent_paths = OrderedSet()
+        for _, target_file, tmp_file in to_download:
+            parent_paths.add(target_file.parent)
             if tmp_file:
-                log_with_indent("temp = '%s'", tmp_file)
-            log_with_indent("to = '%s'", local_file)
+                parent_paths.add(tmp_file.parent)
 
-            self._download_file(
-                source_file,
-                local_file,
-                tmp_file,
-                result,
-            )
+        for parent_path in parent_paths:
+            parent_path.mkdir(parents=True, exist_ok=True)
+
+    def _bulk_download(
+        self,
+        to_download: DOWNLOAD_ITEMS_TYPE,
+    ) -> list[tuple[FileDownloadStatus, PurePathProtocol | PathWithStatsProtocol]]:
+        workers = self.options.workers
+        result = []
+
+        if workers > 1:
+            with ThreadPoolExecutor(max_workers=workers, thread_name_prefix=self.__class__.__name__) as executor:
+                futures = [
+                    executor.submit(self._download_file, source_file, target_file, tmp_file)
+                    for source_file, target_file, tmp_file in to_download
+                ]
+                for future in as_completed(futures):
+                    result.append(future.result())
+        else:
+            for source_file, target_file, tmp_file in to_download:
+                result.append(
+                    self._download_file(
+                        source_file,
+                        target_file,
+                        tmp_file,
+                    ),
+                )
 
         return result
 
     def _download_file(  # noqa: WPS231, WPS213
         self,
         source_file: RemotePath,
         local_file: LocalPath,
         tmp_file: LocalPath | None,
-        result: DownloadResult,
-    ) -> None:
+    ) -> tuple[FileDownloadStatus, PurePathProtocol | PathWithStatsProtocol]:
+        if tmp_file:
+            log.info(
+                "|%s| Downloading file '%s' to '%s' (via tmp '%s')",
+                self.__class__.__name__,
+                source_file,
+                local_file,
+                tmp_file,
+            )
+        else:
+            log.info("|%s| Downloading file '%s' to '%s'", self.__class__.__name__, source_file, local_file)
+
         if not self.connection.path_exists(source_file):
             log.warning("|%s| Missing file '%s', skipping", self.__class__.__name__, source_file)
-            result.missing.add(source_file)
-            return
+            return FileDownloadStatus.MISSING, source_file
 
         try:
             remote_file = self.connection.resolve_file(source_file)
 
             replace = False
             if local_file.exists():
                 if self.options.mode == FileWriteMode.ERROR:
                     raise FileExistsError(f"File {path_repr(local_file)} already exists")
 
                 if self.options.mode == FileWriteMode.IGNORE:
                     log.warning("|Local FS| File %s already exists, skipping", path_repr(local_file))
-                    result.skipped.add(remote_file)
-                    return
+                    return FileDownloadStatus.SKIPPED, remote_file
 
                 replace = True
 
             if tmp_file:
                 # Files are loaded to temporary directory before moving them to target dir.
                 # This prevents operations with partly downloaded files
 
@@ -721,15 +793,15 @@
                 strategy.hwm.update(remote_file)
                 strategy.save_hwm()
 
             # Delete Remote
             if self.options.delete_source:
                 self.connection.remove_file(remote_file)
 
-            result.successful.add(local_file)
+            return FileDownloadStatus.SUCCESSFUL, local_file
 
         except Exception as e:
             if log.isEnabledFor(logging.DEBUG):
                 log.exception(
                     "|%s| Couldn't download file from source dir",
                     self.__class__.__name__,
                     exc_info=e,
@@ -737,15 +809,19 @@
             else:
                 log.exception(
                     "|%s| Couldn't download file from source dir: %s",
                     self.__class__.__name__,
                     e,
                     exc_info=False,
                 )
-            result.failed.add(FailedRemoteFile(path=remote_file.path, stats=remote_file.stats, exception=e))
+            return FileDownloadStatus.FAILED, FailedRemoteFile(
+                path=remote_file.path,
+                stats=remote_file.stats,
+                exception=e,
+            )
 
     def _remove_temp_dir(self, temp_dir: LocalPath) -> None:
         log.info("|Local FS| Removing temp directory '%s'", temp_dir)
 
         try:
             shutil.rmtree(temp_dir)
         except Exception:
```

### Comparing `onetl-0.8.0/onetl/file/file_mover/__init__.py` & `onetl-0.8.1/onetl/file/file_mover/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_mover/file_mover.py` & `onetl-0.8.1/onetl/file/file_mover/file_mover.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import logging
 import os
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from enum import Enum
 from typing import Iterable, List, Optional, Tuple
 
 from ordered_set import OrderedSet
 from pydantic import Field, validator
 
 from onetl.base import BaseFileConnection, BaseFileFilter, BaseFileLimit
-from onetl.base.path_protocol import PathProtocol
+from onetl.base.path_protocol import PathProtocol, PathWithStatsProtocol
+from onetl.base.pure_path_protocol import PurePathProtocol
 from onetl.file.file_mover.move_result import MoveResult
 from onetl.file.file_set import FileSet
+from onetl.hooks import slot, support_hooks
 from onetl.impl import (
     FailedRemoteFile,
     FileWriteMode,
     FrozenModel,
     GenericOptions,
     RemoteFile,
     RemotePath,
@@ -44,17 +48,25 @@
 
 log = logging.getLogger(__name__)
 
 # source, target
 MOVE_ITEMS_TYPE = OrderedSet[Tuple[RemotePath, RemotePath]]
 
 
+class FileMoveStatus(Enum):
+    SUCCESSFUL = 0
+    FAILED = 1
+    SKIPPED = 2
+    MISSING = -1
+
+
+@support_hooks
 class FileMover(FrozenModel):
     """Allows you to move files between different directories in a filesystem,
-    and return an object with move result summary.
+    and return an object with move result summary. |support_hooks|
 
     .. note::
 
         This class is used to move files **only** within the same connection,
 
         It does NOT support direct file transfer between filesystems, like ``FTP -> SFTP``.
         You should use :ref:`file-downloader` + :ref:`file-uploader` to implement ``FTP -> local dir -> SFTP``.
@@ -150,27 +162,38 @@
         Possible values:
             * ``error`` (default) - do nothing, mark file as failed
             * ``ignore`` - do nothing, mark file as ignored
             * ``overwrite`` - replace existing file with a new one
             * ``delete_all`` - delete directory content before moving files
         """
 
+        workers: int = Field(default=1, ge=1)
+        """
+        Number of workers to create for parallel file moving.
+
+        1 (default) means files will me moved sequentially.
+        2 or more means files will be moved in parallel workers.
+
+        Recommended value is ``min(32, os.cpu_count() + 4)``, e.g. ``5``.
+        """
+
     connection: BaseFileConnection
 
     target_path: RemotePath
     source_path: Optional[RemotePath] = None
 
     filters: List[BaseFileFilter] = Field(default_factory=list)
     limits: List[BaseFileLimit] = Field(default_factory=list)
 
     options: Options = Options()
 
+    @slot
     def run(self, files: Iterable[str | os.PathLike] | None = None) -> MoveResult:  # noqa: WPS231
         """
-        Method for moving files from source to target directory.
+        Method for moving files from source to target directory. |support_hooks|
 
         Parameters
         ----------
 
         files : Iterable[str | os.PathLike] | None, default ``None``
             File list to move.
 
@@ -300,18 +323,19 @@
             self.connection.remove_dir(self.target_path, recursive=True)
             self.connection.create_dir(self.target_path)
 
         result = self._move_files(to_move)
         self._log_result(result)
         return result
 
+    @slot
     def view_files(self) -> FileSet[RemoteFile]:
         """
         Get file list in the ``source_path``,
-        after ``filter`` and ``limit`` applied (if any).
+        after ``filter`` and ``limit`` applied (if any). |support_hooks|
 
         Raises
         -------
         :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``source_path`` does not found
 
@@ -418,15 +442,15 @@
                     # Passed path is already relative
                     new_file = self.target_path / remote_file_path
                     old_file = self.source_path / remote_file_path
                 else:
                     # Wrong path (not relative path and source path not in the path to the file)
                     raise ValueError(f"File path '{old_file}' does not match source_path '{self.source_path}'")
 
-            if self.connection.path_exists(old_file):
+            if not isinstance(old_file, PathProtocol) and self.connection.path_exists(old_file):
                 old_file = self.connection.resolve_file(old_file)
 
             result.add((old_file, new_file))
 
         return result
 
     @validator("target_path", pre=True, always=True)
@@ -443,46 +467,82 @@
     def _check_target_path(self):
         self.connection.create_dir(self.target_path)
 
     def _move_files(
         self,
         to_move: MOVE_ITEMS_TYPE,
     ) -> MoveResult:
-        total_files = len(to_move)
         files = FileSet(item[0] for item in to_move)
-
         log.info("|%s| Files to be moved:", self.__class__.__name__)
         log_lines(str(files))
         log_with_indent("")
         log.info("|%s| Starting the move process", self.__class__.__name__)
 
+        self._create_dirs(to_move)
+
         result = MoveResult()
-        for i, (source_file, target_file) in enumerate(to_move):
-            log.info("|%s| Moving file %d of %d", self.__class__.__name__, i + 1, total_files)
-            log_with_indent("from = '%s'", source_file)
-            log_with_indent("to = '%s'", target_file)
-
-            self._move_file(
-                source_file,
-                target_file,
-                result,
-            )
+        for status, file in self._bulk_move(to_move):
+            if status == FileMoveStatus.SUCCESSFUL:
+                result.successful.add(file)
+            elif status == FileMoveStatus.FAILED:
+                result.failed.add(file)
+            elif status == FileMoveStatus.SKIPPED:
+                result.skipped.add(file)
+            elif status == FileMoveStatus.MISSING:
+                result.missing.add(file)
+
+        return result
+
+    def _create_dirs(
+        self,
+        to_move: MOVE_ITEMS_TYPE,
+    ) -> None:
+        """
+        Create all parent paths before moving files
+        This is required to avoid errors then multiple threads create the same dir
+        """
+        parent_paths = OrderedSet(target_file.parent for _, target_file in to_move)
+        for parent_path in parent_paths:
+            self.connection.create_dir(parent_path)
+
+    def _bulk_move(
+        self,
+        to_move: MOVE_ITEMS_TYPE,
+    ) -> list[tuple[FileMoveStatus, PurePathProtocol | PathWithStatsProtocol]]:
+        workers = self.options.workers
+        result = []
+
+        if workers > 1:
+            with ThreadPoolExecutor(max_workers=workers, thread_name_prefix=self.__class__.__name__) as executor:
+                futures = [
+                    executor.submit(self._move_file, source_file, target_file) for source_file, target_file in to_move
+                ]
+                for future in as_completed(futures):
+                    result.append(future.result())
+        else:
+            for source_file, target_file in to_move:
+                result.append(
+                    self._move_file(
+                        source_file,
+                        target_file,
+                    ),
+                )
 
         return result
 
     def _move_file(  # noqa: WPS231, WPS213
         self,
         source_file: RemotePath,
         target_file: RemotePath,
-        result: MoveResult,
-    ) -> None:
+    ) -> tuple[FileMoveStatus, PurePathProtocol | PathWithStatsProtocol]:
+        log.info("|%s| Moving file '%s' to '%s'", self.__class__.__name__, source_file, target_file)
+
         if not self.connection.path_exists(source_file):
             log.warning("|%s| Missing file '%s', skipping", self.__class__.__name__, source_file)
-            result.missing.add(source_file)
-            return
+            return FileMoveStatus.MISSING, source_file
 
         try:
             replace = False
             if self.connection.path_exists(target_file):
                 new_file = self.connection.resolve_file(target_file)
 
                 if self.options.mode == FileWriteMode.ERROR:
@@ -490,21 +550,20 @@
 
                 if self.options.mode == FileWriteMode.IGNORE:
                     log.warning(
                         "|%s| File %s already exists, skipping",
                         self.connection.__class__.__name__,
                         path_repr(new_file),
                     )
-                    result.skipped.add(source_file)
-                    return
+                    return FileMoveStatus.SKIPPED, source_file
 
                 replace = True
 
             new_file = self.connection.rename_file(source_file, target_file, replace=replace)
-            result.successful.add(new_file)
+            return FileMoveStatus.SUCCESSFUL, new_file
 
         except Exception as e:
             if log.isEnabledFor(logging.DEBUG):
                 log.exception(
                     "|%s| Couldn't move file to target dir",
                     self.__class__.__name__,
                     exc_info=e,
@@ -512,14 +571,14 @@
             else:
                 log.exception(
                     "|%s| Couldn't move file to target dir: %s",
                     self.__class__.__name__,
                     e,
                     exc_info=False,
                 )
-            result.failed.add(FailedRemoteFile(path=source_file.path, stats=source_file.stats, exception=e))
+            return FileMoveStatus.FAILED, FailedRemoteFile(path=source_file.path, stats=source_file.stats, exception=e)
 
     def _log_result(self, result: MoveResult) -> None:
         log_with_indent("")
         log.info("|%s| Move result:", self.__class__.__name__)
         log_lines(str(result))
         entity_boundary_log(msg=f"{self.__class__.__name__} ends", char="-")
```

### Comparing `onetl-0.8.0/onetl/file/file_mover/move_result.py` & `onetl-0.8.1/onetl/file/file_mover/move_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_result.py` & `onetl-0.8.1/onetl/file/file_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,14 @@
             """
 
             assert file_result1.summary == result
 
             file_result2 = FileResult()
             assert file_result1.summary == "No files"
         '''
-
         return self._total_message
 
     def __str__(self):
         """Same as :obj:`onetl.file.file_result.FileResult.details`"""
         return self.details
 
     @property
```

### Comparing `onetl-0.8.0/onetl/file/file_set.py` & `onetl-0.8.1/onetl/file/file_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,14 @@
             assert FileSet().summary == "No files"
         """
 
         if not self:
             return "No files"
 
         file_number_str = f"{len(self)} files" if len(self) > 1 else "1 file"
-
         return f"{file_number_str} (size='{naturalsize(self.total_size)}')"
 
     @property
     def details(self) -> str:
         '''
         Return detailed information about files in the set
```

### Comparing `onetl-0.8.0/onetl/file/file_uploader/__init__.py` & `onetl-0.8.1/onetl/file/file_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/file_uploader/file_uploader.py` & `onetl-0.8.1/onetl/file/file_uploader/file_uploader.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,24 +12,29 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import logging
 import os
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from enum import Enum
 from typing import Iterable, Optional, Tuple
 
 from ordered_set import OrderedSet
-from pydantic import validator
+from pydantic import Field, validator
 
 from onetl._internal import generate_temp_path  # noqa: WPS436
 from onetl.base import BaseFileConnection
+from onetl.base.path_protocol import PathWithStatsProtocol
+from onetl.base.pure_path_protocol import PurePathProtocol
 from onetl.exception import DirectoryNotFoundError, NotAFileError
 from onetl.file.file_set import FileSet
 from onetl.file.file_uploader.upload_result import UploadResult
+from onetl.hooks import slot, support_hooks
 from onetl.impl import (
     FailedLocalFile,
     FileWriteMode,
     FrozenModel,
     GenericOptions,
     LocalPath,
     RemotePath,
@@ -39,17 +44,25 @@
 
 log = logging.getLogger(__name__)
 
 # source, target, temp
 UPLOAD_ITEMS_TYPE = OrderedSet[Tuple[LocalPath, RemotePath, Optional[RemotePath]]]
 
 
+class FileUploadStatus(Enum):
+    SUCCESSFUL = 0
+    FAILED = 1
+    SKIPPED = 2
+    MISSING = -1
+
+
+@support_hooks
 class FileUploader(FrozenModel):
     """Allows you to upload files to a remote source with specified file connection
-    and parameters, and return an object with upload result summary.
+    and parameters, and return an object with upload result summary. |support_hooks|
 
     .. note::
 
         This class is used to upload files **only** from local directory to the remote one.
 
         It does NOT support direct file transfer between filesystems, like ``FTP -> SFTP``.
         You should use :ref:`file-downloader` + FileUploader to implement ``FTP -> local dir -> SFTP``.
@@ -145,26 +158,37 @@
         delete_local: bool = False
         """
         If ``True``, remove local file after successful download.
 
         If download failed, file will left intact.
         """
 
+        workers: int = Field(default=1, ge=1)
+        """
+        Number of workers to create for parallel file upload.
+
+        1 (default) means files will me uploaded sequentially.
+        2 or more means files will be uploaded in parallel workers.
+
+        Recommended value is ``min(32, os.cpu_count() + 4)``, e.g. ``5``.
+        """
+
     connection: BaseFileConnection
 
     target_path: RemotePath
 
     local_path: Optional[LocalPath] = None
     temp_path: Optional[RemotePath] = None
 
     options: Options = Options()
 
+    @slot
     def run(self, files: Iterable[str | os.PathLike] | None = None) -> UploadResult:
         """
-        Method for uploading files to remote host.
+        Method for uploading files to remote host. |support_hooks|
 
         Parameters
         ----------
 
         files : Iterator[str | os.PathLike] | None, default ``None``
             File list to upload.
 
@@ -314,17 +338,18 @@
 
         if current_temp_dir:
             self._remove_temp_dir(current_temp_dir)
 
         self._log_result(result)
         return result
 
+    @slot
     def view_files(self) -> FileSet[LocalPath]:
         """
-        Get file list in the ``local_path``.
+        Get file list in the ``local_path``. |support_hooks|
 
         Raises
         -------
         :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``local_path`` does not found
 
@@ -457,57 +482,110 @@
         if not self.local_path.exists():
             raise DirectoryNotFoundError(f"'{self.local_path}' does not exist")
 
         if not self.local_path.is_dir():
             raise NotADirectoryError(f"{path_repr(self.local_path)} is not a directory")
 
     def _upload_files(self, to_upload: UPLOAD_ITEMS_TYPE) -> UploadResult:
-        total_files = len(to_upload)
         files = FileSet(item[0] for item in to_upload)
-
         log.info("|%s| Files to be uploaded:", self.__class__.__name__)
         log_lines(str(files))
         log_with_indent("")
         log.info("|%s| Starting the upload process", self.__class__.__name__)
 
+        self._create_dirs(to_upload)
+
         result = UploadResult()
-        for i, (local_file, target_file, tmp_file) in enumerate(to_upload):
-            log.info("|%s| Uploading file %d of %d", self.__class__.__name__, i + 1, total_files)
-            log_with_indent("from = '%s'", local_file)
+        for status, file in self._bulk_upload(to_upload):
+            if status == FileUploadStatus.SUCCESSFUL:
+                result.successful.add(file)
+            elif status == FileUploadStatus.FAILED:
+                result.failed.add(file)
+            elif status == FileUploadStatus.SKIPPED:
+                result.skipped.add(file)
+            elif status == FileUploadStatus.MISSING:
+                result.missing.add(file)
+
+        return result
+
+    def _create_dirs(
+        self,
+        to_upload: UPLOAD_ITEMS_TYPE,
+    ) -> None:
+        """
+        Create all parent paths before uploading files
+        This is required to avoid errors then multiple threads create the same dir
+        """
+        parent_paths = OrderedSet()
+        for _, target_file, tmp_file in to_upload:
+            parent_paths.add(target_file.parent)
             if tmp_file:
-                log_with_indent("temp = '%s'", tmp_file)
-            log_with_indent("to = '%s'", target_file)
+                parent_paths.add(tmp_file.parent)
 
-            self._upload_file(local_file, target_file, tmp_file, result)
+        for parent_path in parent_paths:
+            self.connection.create_dir(parent_path)
+
+    def _bulk_upload(
+        self,
+        to_upload: UPLOAD_ITEMS_TYPE,
+    ) -> list[tuple[FileUploadStatus, PurePathProtocol | PathWithStatsProtocol]]:
+        workers = self.options.workers
+        result = []
+
+        if workers > 1:
+            with ThreadPoolExecutor(max_workers=workers, thread_name_prefix=self.__class__.__name__) as executor:
+                futures = [
+                    executor.submit(self._upload_file, local_file, target_file, tmp_file)
+                    for local_file, target_file, tmp_file in to_upload
+                ]
+                for future in as_completed(futures):
+                    result.append(future.result())
+        else:
+            for local_file, target_file, tmp_file in to_upload:
+                result.append(
+                    self._upload_file(
+                        local_file,
+                        target_file,
+                        tmp_file,
+                    ),
+                )
 
         return result
 
     def _upload_file(  # noqa: WPS231
         self,
         local_file: LocalPath,
         target_file: RemotePath,
         tmp_file: RemotePath | None,
-        result: UploadResult,
-    ) -> None:
+    ) -> tuple[FileUploadStatus, PurePathProtocol | PathWithStatsProtocol]:
+        if tmp_file:
+            log.info(
+                "|%s| Uploading file '%s' to '%s' (via tmp '%s')",
+                self.__class__.__name__,
+                local_file,
+                target_file,
+                tmp_file,
+            )
+        else:
+            log.info("|%s| Uploading file '%s' to '%s'", self.__class__.__name__, local_file, target_file)
+
         if not local_file.exists():
             log.warning("|%s| Missing file '%s', skipping", self.__class__.__name__, local_file)
-            result.missing.add(local_file)
-            return
+            return FileUploadStatus.MISSING, local_file
 
         try:
             replace = False
             if self.connection.path_exists(target_file):
                 file = self.connection.resolve_file(target_file)
                 if self.options.mode == FileWriteMode.ERROR:
                     raise FileExistsError(f"File {path_repr(file)} already exists")
 
                 if self.options.mode == FileWriteMode.IGNORE:
                     log.warning("|%s| File %s already exists, skipping", self.__class__.__name__, path_repr(file))
-                    result.skipped.add(local_file)
-                    return
+                    return FileUploadStatus.SKIPPED, local_file
 
                 replace = True
 
             if tmp_file:
                 # Files are loaded to temporary directory before moving them to target dir.
                 # This prevents operations with partly uploaded files
 
@@ -517,23 +595,23 @@
                 # Direct upload
                 uploaded_file = self.connection.upload_file(local_file, target_file, replace=replace)
 
             if self.options.delete_local:
                 local_file.unlink()
                 log.warning("|Local FS| Successfully removed file %s", local_file)
 
-            result.successful.add(uploaded_file)
+            return FileUploadStatus.SUCCESSFUL, uploaded_file
 
         except Exception as e:
             if log.isEnabledFor(logging.DEBUG):
                 log.exception("|%s| Couldn't upload file to target dir", self.__class__.__name__, exc_info=e)
             else:
                 log.exception("|%s| Couldn't upload file to target dir: %s", self.__class__.__name__, e, exc_info=False)
 
-            result.failed.add(FailedLocalFile(path=local_file, exception=e))
+            return FileUploadStatus.FAILED, FailedLocalFile(path=local_file, exception=e)
 
     def _remove_temp_dir(self, temp_dir: RemotePath) -> None:
         try:
             self.connection.remove_dir(temp_dir, recursive=True)
         except Exception:
             log.exception("|%s| Error while removing temp directory", self.__class__.__name__)
```

### Comparing `onetl-0.8.0/onetl/file/file_uploader/upload_result.py` & `onetl-0.8.1/onetl/file/file_uploader/upload_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/__init__.py` & `onetl-0.8.1/onetl/file/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/exclude_dir.py` & `onetl-0.8.1/onetl/file/filter/exclude_dir.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/file_hwm.py` & `onetl-0.8.1/onetl/file/filter/file_hwm.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/glob.py` & `onetl-0.8.1/onetl/file/filter/glob.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/match_all_filters.py` & `onetl-0.8.1/onetl/file/filter/match_all_filters.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/filter/regexp.py` & `onetl-0.8.1/onetl/file/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/limit/__init__.py` & `onetl-0.8.1/onetl/file/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/limit/limits_reached.py` & `onetl-0.8.1/onetl/file/limit/limits_reached.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/limit/limits_stop_at.py` & `onetl-0.8.1/onetl/file/limit/limits_stop_at.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/limit/max_files_count.py` & `onetl-0.8.1/onetl/file/limit/max_files_count.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/file/limit/reset_limits.py` & `onetl-0.8.1/onetl/file/limit/reset_limits.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hooks/hook.py` & `onetl-0.8.1/onetl/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hooks/hook_collection.py` & `onetl-0.8.1/onetl/hooks/hook_collection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hooks/hooks_state.py` & `onetl-0.8.1/onetl/hooks/hooks_state.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hooks/method_inheritance_stack.py` & `onetl-0.8.1/onetl/hooks/method_inheritance_stack.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hooks/slot.py` & `onetl-0.8.1/onetl/hooks/slot.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import inspect
 import logging
 import textwrap
 from collections import defaultdict
 from contextlib import ExitStack, suppress
 from functools import partial, wraps
-from types import FunctionType
 from typing import Any, Callable, ContextManager, TypeVar
 
 from typing_extensions import Protocol
 
 from onetl.exception import SignatureError
 from onetl.hooks.hook import CanProcessResult, Hook, HookPriority
 from onetl.hooks.hook_collection import HookCollection
@@ -27,15 +26,15 @@
     """Unwrap @classmethod and @staticmethod to get original function"""
     return getattr(method, "__func__", method)
 
 
 def get_hooks(cls: type, method_name: str) -> HookCollection:
     """Return all hooks registered for a specific method"""
 
-    method = _unwrap_method(cls.__dict__[method_name])
+    method = _unwrap_method(cls.__dict__.get(method_name, None))
     return getattr(method, "__hooks__", HookCollection())
 
 
 def get_hooks_hierarchy(cls: type, method_name: str) -> HookCollection:
     """
     Return all hooks registered for a specific method,
     sorted by priority and class nested level.
@@ -56,15 +55,15 @@
     result = HookCollection()
     for priority in sorted(hooks_by_priority):
         result.extend(hooks_by_priority[priority])
 
     return result
 
 
-def bind_hook(method: Hook, inp=None):
+def bind_hook(method: Callable, inp=None):
     """
     Bind a hook to the slot.
 
     See :ref:`hooks-design` for more details.
 
     Examples
     --------
@@ -106,15 +105,15 @@
             )
 
         method.__hooks__.add(hook)
 
         logger.debug(
             "|onETL| Registered hook '%s.%s' for '%s' (enabled=%r, priority=%s)",
             hook.__module__,
-            hook.__qualname__,
+            hook.__qualname__,  # type: ignore[attr-defined]
             method.__qualname__,
             hook.enabled,
             hook.priority,
         )
 
         return hook
 
@@ -322,15 +321,15 @@
 
             for i, hook in enumerate(hooks):
                 logger.log(
                     NOTICE,
                     "|Hooks| %sCalling hook '%s.%s' (%d of %d)",
                     " " * indent,
                     hook.__module__,
-                    hook.__qualname__,
+                    hook.__qualname__,  # type: ignore[attr-defined]
                     i + 1,
                     hooks_count,
                 )
 
                 hook_args = _prepare_hook_args(
                     method=method,
                     hook=hook,
@@ -390,26 +389,26 @@
                 call_result = "(None)" if result is None else "(*NOT None*)"
                 logger.log(
                     NOTICE,
                     "|Hooks| %sMethod call result %s will be replaced with result of calling the hook '%s.%s'",
                     " " * indent,
                     call_result,
                     before_hook.__module__,
-                    before_hook.__qualname__,
+                    before_hook.__qualname__,  # type: ignore[attr-defined]
                 )
                 result = before_result
 
             for hook, context in context_results:
                 if isinstance(context, CanProcessResult):
                     logger.log(
                         NOTICE,
                         "|Hooks| %sPassing result to 'process_result' method of context manager '%s.%s'",
                         " " * indent,
                         hook.__module__,
-                        hook.__qualname__,
+                        hook.__qualname__,  # type: ignore[attr-defined]
                     )
                     context_result = _handle_context_result(
                         result=result,
                         context=context,
                         hook=hook,
                     )
 
@@ -442,15 +441,16 @@
         return staticmethod(wrapper)
 
     return wrapper
 
 
 def _is_method(method: Callable) -> bool:
     """Checks whether class method is callable"""
-    return isinstance(method, (FunctionType, classmethod, staticmethod))
+    method = _unwrap_method(method)
+    return callable(method)
 
 
 def _is_private(method: Callable) -> bool:
     """Checks whether class method is private"""
     method_name = _unwrap_method(method).__name__
     return method_name.startswith("_") and not method_name.endswith("__")
```

### Comparing `onetl-0.8.0/onetl/hooks/support_hooks.py` & `onetl-0.8.1/onetl/hooks/support_hooks.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hwm/store/__init__.py` & `onetl-0.8.1/onetl/hwm/store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hwm/store/hwm_class_registry.py` & `onetl-0.8.1/onetl/hwm/store/hwm_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hwm/store/hwm_store_class_registry.py` & `onetl-0.8.1/onetl/hwm/store/hwm_store_class_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from functools import wraps
 from typing import Any, Callable, ClassVar, Collection, Mapping
 
 from onetl.hwm.store.base_hwm_store import BaseHWMStore
 
 
 class HWMStoreClassRegistry:
-    """Registry class of different HWM stores
+    """Registry class of different HWM stores.
 
     Examples
     --------
 
     .. code:: python
 
         from onetl.hwm.store import HWMStoreClassRegistry, YAMLHWMStore, MemoryHWMStore
@@ -76,20 +76,20 @@
     --------
 
     .. code:: python
 
         from onetl.hwm.store import (
             HWMStoreClassRegistry,
             default_hwm_store_class,
-            BaseStore,
+            BaseHWMStore,
         )
 
 
         @default_hwm_store_class
-        class MyClass(BaseStore):
+        class MyClass(BaseHWMStore):
             ...
 
 
         HWMStoreClassRegistry.get() == MyClass  # default
 
     """
 
@@ -104,20 +104,20 @@
     --------
 
     .. code:: python
 
         from onetl.hwm.store import (
             HWMStoreClassRegistry,
             register_hwm_store_class,
-            BaseStore,
+            BaseHWMStore,
         )
 
 
         @register_hwm_store_class("somename")
-        class MyClass(BaseStore):
+        class MyClass(BaseHWMStore):
             ...
 
 
         HWMStoreClassRegistry.get("somename") == MyClass
 
     """
 
@@ -234,19 +234,23 @@
             env:
                 hwm_store: yaml
 
     ``run.py``
 
     .. code:: python
 
+        import hydra
+        from omegaconf import DictConfig
+        from onetl.hwm.store import detect_hwm_store
+
+
+        # key=... is a path to config item, delimited by dot ``.``
         @hydra.main(config="../conf")
-        @detect_hwm_store(
-            key="myetl.env.hwm_store"
-        )  # path to config item, delimited by dot ``.``
-        def main(config: OmniConf):
+        @detect_hwm_store(key="myetl.env.hwm_store")
+        def main(config: DictConfig):
             pass
 
     """
 
     if not isinstance(key, str):
         raise ValueError("key name must be a string")
```

### Comparing `onetl-0.8.0/onetl/hwm/store/hwm_store_manager.py` & `onetl-0.8.1/onetl/hwm/store/hwm_store_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/hwm/store/memory_hwm_store.py` & `onetl-0.8.1/onetl/hwm/store/memory_hwm_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 from __future__ import annotations
 
 from typing import Dict
 
 from etl_entities import HWM
 from pydantic import PrivateAttr
 
+from onetl.hooks import slot, support_hooks
 from onetl.hwm.store.base_hwm_store import BaseHWMStore
 from onetl.hwm.store.hwm_store_class_registry import register_hwm_store_class
 
 
 @register_hwm_store_class("memory", "in-memory")
+@support_hooks
 class MemoryHWMStore(BaseHWMStore):
-    """In-memory local store for HWM values
+    """In-memory local store for HWM values. |support_hooks|
 
     .. note::
 
         This class should be used in tests only, because all saved HWM values
         will be deleted after exiting the context
 
     Examples
@@ -77,15 +79,21 @@
             # will store HWM value in RAM
 
         # values are lost after exiting the context
     """
 
     _data: Dict[str, HWM] = PrivateAttr(default_factory=dict)
 
+    @slot
     def get(self, name: str) -> HWM | None:
         return self._data.get(name, None)
 
+    @slot
     def save(self, hwm: HWM) -> None:
         self._data[hwm.qualified_name] = hwm
 
+    @slot
     def clear(self) -> None:
+        """
+        Clears all stored HWM values. |support_hooks|
+        """
         self._data.clear()
```

### Comparing `onetl-0.8.0/onetl/hwm/store/yaml_hwm_store.py` & `onetl-0.8.1/onetl/hwm/store/yaml_hwm_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,30 @@
 from typing import ClassVar
 
 import yaml
 from etl_entities import HWM, HWMTypeRegistry
 from platformdirs import user_data_dir
 from pydantic import validator
 
+from onetl.hooks import slot, support_hooks
 from onetl.hwm.store.base_hwm_store import BaseHWMStore
 from onetl.hwm.store.hwm_store_class_registry import (
     default_hwm_store_class,
     register_hwm_store_class,
 )
 from onetl.impl import FrozenModel, LocalPath
 
 DATA_PATH = LocalPath(user_data_dir("onETL", "ONEtools"))
 
 
 @default_hwm_store_class
 @register_hwm_store_class("yaml", "yml")
+@support_hooks
 class YAMLHWMStore(BaseHWMStore, FrozenModel):
-    r"""YAML local store for HWM values. Used as default HWM store.
+    r"""YAML local store for HWM values. Used as default HWM store. |support_hooks|
 
     Parameters
     ----------
     path : :obj:`pathlib.Path` or `str`
 
         Folder name there HWM value files will be stored.
 
@@ -162,23 +164,25 @@
 
     @validator("path", pre=True, always=True)
     def validate_path(cls, path):
         path = LocalPath(path).expanduser().resolve()
         path.mkdir(parents=True, exist_ok=True)
         return path
 
+    @slot
     def get(self, name: str) -> HWM | None:
         data = self._load(name)
 
         if not data:
             return None
 
         latest = sorted(data, key=operator.itemgetter("modified_time"))[-1]
         return HWMTypeRegistry.parse(latest)
 
+    @slot
     def save(self, hwm: HWM) -> LocalPath:
         data = self._load(hwm.qualified_name)
         self._dump(hwm.qualified_name, [hwm.serialize()] + data)
         return self.get_file_path(hwm.qualified_name)
 
     @classmethod
     def cleanup_file_name(cls, name: str) -> str:
```

### Comparing `onetl-0.8.0/onetl/impl/__init__.py` & `onetl-0.8.1/onetl/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/base_model.py` & `onetl-0.8.1/onetl/impl/base_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/failed_local_file.py` & `onetl-0.8.1/onetl/impl/failed_local_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/file_write_mode.py` & `onetl-0.8.1/onetl/impl/file_write_mode.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/frozen_model.py` & `onetl-0.8.1/onetl/impl/frozen_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/generic_options.py` & `onetl-0.8.1/onetl/impl/generic_options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/local_path.py` & `onetl-0.8.1/onetl/impl/local_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/path_container.py` & `onetl-0.8.1/onetl/impl/path_container.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/path_repr.py` & `onetl-0.8.1/onetl/impl/path_repr.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/remote_directory.py` & `onetl-0.8.1/onetl/impl/remote_directory.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/remote_file.py` & `onetl-0.8.1/onetl/impl/remote_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/remote_path.py` & `onetl-0.8.1/onetl/impl/remote_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/impl/remote_path_stat.py` & `onetl-0.8.1/onetl/impl/remote_path_stat.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/log.py` & `onetl-0.8.1/onetl/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 log = logging.getLogger(__name__)
 onetl_log = logging.getLogger("onetl")
 root_log = logging.getLogger()
 
 HALF_SCREEN_SIZE = 45
 BASE_LOG_INDENT = 8
-LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(message)s"
+LOG_FORMAT = "%(asctime)s [%(levelname)-8s] %(threadName)s: %(message)s"
 CLIENT_MODULES = {"hdfs", "paramiko", "ftputil", "smbclient"}
 
 DISABLED = 9999  # CRITICAL is 50, we need even higher to disable all logs
 logging.addLevelName(DISABLED, "DISABLED")
 
 NOTICE = 5  # DEBUG is 10, we need lower value for less verbose logs even on debug level
 logging.addLevelName(NOTICE, "NOTICE")
```

### Comparing `onetl-0.8.0/onetl/plugins/import_plugins.py` & `onetl-0.8.1/onetl/plugins/import_plugins.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/__init__.py` & `onetl-0.8.1/onetl/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/base_strategy.py` & `onetl-0.8.1/onetl/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/batch_hwm_strategy.py` & `onetl-0.8.1/onetl/strategy/batch_hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/hwm_store/__init__.py` & `onetl-0.8.1/onetl/strategy/hwm_store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/hwm_strategy.py` & `onetl-0.8.1/onetl/strategy/hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/incremental_strategy.py` & `onetl-0.8.1/onetl/strategy/incremental_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/snapshot_strategy.py` & `onetl-0.8.1/onetl/strategy/snapshot_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/strategy/strategy_manager.py` & `onetl-0.8.1/onetl/strategy/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl/version.py` & `onetl-0.8.1/onetl/version.py`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/onetl.egg-info/SOURCES.txt` & `onetl-0.8.1/onetl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 onetl/connection/db_connection/__init__.py
 onetl/connection/db_connection/clickhouse.py
 onetl/connection/db_connection/db_connection.py
 onetl/connection/db_connection/greenplum.py
 onetl/connection/db_connection/hive.py
 onetl/connection/db_connection/jdbc_connection.py
 onetl/connection/db_connection/jdbc_mixin.py
+onetl/connection/db_connection/kafka.py
 onetl/connection/db_connection/mongodb.py
 onetl/connection/db_connection/mssql.py
 onetl/connection/db_connection/mysql.py
 onetl/connection/db_connection/oracle.py
 onetl/connection/db_connection/postgres.py
 onetl/connection/db_connection/teradata.py
 onetl/connection/db_connection/dialect_mixins/__init__.py
@@ -146,18 +147,19 @@
 requirements/kerberos.txt
 requirements/s3.txt
 requirements/sftp.txt
 requirements/spark.txt
 requirements/webdav.txt
 requirements/tests/base.txt
 requirements/tests/clickhouse.txt
+requirements/tests/kafka.txt
 requirements/tests/mongodb.txt
 requirements/tests/mssql.txt
 requirements/tests/mysql.txt
 requirements/tests/oracle.txt
 requirements/tests/postgres.txt
 requirements/tests/spark-2.3.1.txt
 requirements/tests/spark-2.4.8.txt
 requirements/tests/spark-3.2.3.txt
 requirements/tests/spark-3.3.2.txt
-requirements/tests/spark-3.4.0.txt
+requirements/tests/spark-3.4.1.txt
 requirements/tests/spark-latest.txt
```

### Comparing `onetl-0.8.0/onetl.egg-info/requires.txt` & `onetl-0.8.1/onetl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/pyproject.toml` & `onetl-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onetl-0.8.0/setup.cfg` & `onetl-0.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,16 @@
 	file_result.py:
 	E800,
 	yaml_hwm_store.py:
 	E800,
 	P102,
 	db_writer.py:
 	E800,
+	kafka.py:
+	TAE001,
 	*connection.py:
 	WPS437,
 	onetl/connection/db_connection/mongodb.py:
 	WPS437,
 	onetl/connection/db_connection/jdbc_mixin.py:
 	TAE001,
 	WPS219,
@@ -207,15 +209,16 @@
 	WPS213,
 	WPS212,
 	F401,
 	F811,
 	F821,
 	WPS429,
 	WPS342,
-	WPS520
+	WPS520,
+	B017
 
 [darglint]
 docstring_style = sphinx
 
 [mypy]
 python_version = 3.7
 exclude = ^(?=.*file).*
```

### Comparing `onetl-0.8.0/setup.py` & `onetl-0.8.1/setup.py`

 * *Files identical despite different names*

