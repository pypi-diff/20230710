# Comparing `tmp/cherre_singer_ingest-16.6.6.tar.gz` & `tmp/cherre_singer_ingest-16.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherre_singer_ingest-16.6.6.tar", max compression
+gzip compressed data, was "cherre_singer_ingest-16.6.7.tar", max compression
```

## Comparing `cherre_singer_ingest-16.6.6.tar` & `cherre_singer_ingest-16.6.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     2431 2023-07-06 19:43:04.844780 cherre_singer_ingest-16.6.6/cherre_singer_ingest/__init__.py
--rw-r--r--   0        0        0      179 2022-08-08 20:54:50.962605 cherre_singer_ingest-16.6.6/cherre_singer_ingest/factories/__init__.py
--rw-r--r--   0        0        0     5046 2022-08-08 20:54:50.962696 cherre_singer_ingest-16.6.6/cherre_singer_ingest/factories/bookmark_factory.py
--rw-r--r--   0        0        0     2354 2022-08-08 20:54:50.962778 cherre_singer_ingest-16.6.6/cherre_singer_ingest/factories/remote_file_uri_factory.py
--rw-r--r--   0        0        0      356 2023-06-14 17:20:33.576704 cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/__init__.py
--rw-r--r--   0        0        0     4238 2022-08-08 20:54:50.962977 cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/base_state_repository.py
--rw-r--r--   0        0        0     5499 2022-08-08 20:54:50.963053 cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/big_query_ingest_state_repository.py
--rw-r--r--   0        0        0     6850 2022-08-09 06:23:37.493294 cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/cloud_sql_ingest_state_repository.py
--rw-r--r--   0        0        0     2141 2023-07-06 19:43:04.844937 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/__init__.py
--rw-r--r--   0        0        0     4691 2023-07-07 15:06:25.485649 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/bookmark_service.py
--rw-r--r--   0        0        0    10725 2022-08-08 20:54:50.963424 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/bq.py
--rw-r--r--   0        0        0      925 2022-08-08 20:54:50.963500 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/clean_column_name.py
--rw-r--r--   0        0        0    10772 2022-08-08 20:54:50.963602 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/common.py
--rw-r--r--   0        0        0       35 2022-08-08 20:54:50.963674 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/constants.py
--rw-r--r--   0        0        0      627 2023-01-26 18:00:06.910174 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/data_formats.py
--rw-r--r--   0        0        0      311 2022-08-08 20:54:50.963822 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/env_var_utils.py
--rw-r--r--   0        0        0      573 2022-08-08 20:54:50.963895 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/flatten_object.py
--rw-r--r--   0        0        0    11041 2022-08-08 20:54:50.964018 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/gcs.py
--rw-r--r--   0        0        0      808 2022-08-08 20:54:50.964099 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/get_login_token.py
--rw-r--r--   0        0        0     6942 2022-08-08 20:54:50.964198 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/run_command.py
--rw-r--r--   0        0        0     1789 2022-08-08 20:54:50.964273 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/run_custom_image_tap.py
--rw-r--r--   0        0        0     1277 2022-08-08 20:54:50.964354 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/sftp.py
--rw-r--r--   0        0        0      333 2022-08-08 20:54:50.964470 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/__init__.py
--rw-r--r--   0        0        0     7743 2022-08-08 20:54:50.964560 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/avro_stream_writer.py
--rw-r--r--   0        0        0      292 2022-08-08 20:54:50.964634 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/per_stream_writer_results.py
--rw-r--r--   0        0        0     5902 2022-08-08 20:54:50.964712 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/stream_target.py
--rw-r--r--   0        0        0      813 2022-08-08 20:54:50.964825 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/__init__.py
--rw-r--r--   0        0        0     1502 2022-08-08 20:54:50.964910 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/avro_file_stream.py
--rw-r--r--   0        0        0     2542 2023-07-06 19:43:04.845288 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/base_file_parsing_tap_stream.py
--rw-r--r--   0        0        0     3696 2023-07-06 19:43:04.845631 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/base_tap_stream.py
--rw-r--r--   0        0        0     1510 2022-08-08 20:54:50.965155 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/cached_stream.py
--rw-r--r--   0        0        0     4735 2023-07-06 19:43:04.845967 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/csv_file_stream.py
--rw-r--r--   0        0        0     1336 2022-08-08 20:54:50.965294 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/fixed_width_file_stream.py
--rw-r--r--   0        0        0     1615 2022-08-08 20:54:50.965368 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/json_file_stream.py
--rw-r--r--   0        0        0     3129 2023-07-06 19:43:04.846075 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/rest_stream.py
--rw-r--r--   0        0        0     3525 2022-08-08 20:54:50.965522 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/shapefile_file_stream.py
--rw-r--r--   0        0        0     1079 2022-08-08 20:54:50.965626 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/__init__.py
--rw-r--r--   0        0        0     2628 2022-08-08 20:54:50.965705 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_api_tap.py
--rw-r--r--   0        0        0     9910 2023-05-15 13:44:36.386150 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_file_parsing_tap.py
--rw-r--r--   0        0        0    16299 2022-08-08 20:54:50.965989 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_ftp_file_tap.py
--rw-r--r--   0        0        0     2657 2022-08-08 20:54:50.966080 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_bucket_file_tap.py
--rw-r--r--   0        0        0     2974 2022-08-08 20:54:50.966138 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_bucket_folder_tap.py
--rw-r--r--   0        0        0     3266 2022-08-08 20:54:50.966217 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_storage_tap.py
--rw-r--r--   0        0        0     7278 2022-08-08 20:54:50.966291 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_tap.py
--rw-r--r--   0        0        0     4260 2022-08-08 20:54:50.966362 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/big_query_table_tap.py
--rw-r--r--   0        0        0     1131 2022-08-08 20:54:50.966460 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/error_throwing_tap.py
--rw-r--r--   0        0        0     3139 2022-08-08 20:54:50.966538 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_csv_bucket_file_tap.py
--rw-r--r--   0        0        0     2701 2022-08-08 20:54:50.966622 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_json_bucket_file_tap.py
--rw-r--r--   0        0        0     3323 2022-08-08 20:54:50.966683 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_shapefile_bucket_file_tap.py
--rw-r--r--   0        0        0      917 2022-08-08 20:54:50.966748 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/simple_test_tap.py
--rw-r--r--   0        0        0     3420 2022-08-08 20:54:50.966838 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/webpage_tap.py
--rw-r--r--   0        0        0      348 2022-08-08 20:54:50.966923 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/__init__.py
--rw-r--r--   0        0        0     9824 2023-07-05 16:55:21.809044 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/base_cherre_target.py
--rw-r--r--   0        0        0     3557 2023-07-05 16:56:28.939545 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/cherre_big_query_external_data_target.py
--rw-r--r--   0        0        0     6095 2022-08-08 20:54:50.967148 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/cherre_parsed_data_lake_target.py
--rw-r--r--   0        0        0     2812 2022-08-08 20:54:50.967227 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/unzip_service.py
--rw-r--r--   0        0        0     3492 2022-08-08 20:54:50.967298 cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/unzip_service_with_bookmarks.py
--rw-r--r--   0        0        0     1526 2023-07-06 19:43:04.846193 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/__init__.py
--rw-r--r--   0        0        0     1388 2022-08-08 20:54:50.967453 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/exceptions.py
--rw-r--r--   0        0        0      719 2023-07-06 19:43:04.846481 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/__init__.py
--rw-r--r--   0        0        0      707 2022-08-08 20:54:50.967597 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/bookmark_type.py
--rw-r--r--   0        0        0     1356 2022-08-08 20:54:50.967683 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_bookmark.py
--rw-r--r--   0        0        0     1221 2022-08-08 20:54:50.967742 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_failed_bookmark.py
--rw-r--r--   0        0        0     1910 2022-08-08 20:54:50.967796 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_bookmark.py
--rw-r--r--   0        0        0     1485 2022-08-08 20:54:50.967853 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_failed_bookmark.py
--rw-r--r--   0        0        0     1794 2022-08-08 20:54:50.967913 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/ingest_bookmark.py
--rw-r--r--   0        0        0      235 2022-08-08 20:54:50.967965 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/uri_bookmark.py
--rw-r--r--   0        0        0     1010 2022-08-08 20:54:50.968025 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/remote_file.py
--rw-r--r--   0        0        0     3227 2022-08-08 20:54:50.968095 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/run_singer_command.py
--rw-r--r--   0        0        0      141 2022-08-08 20:54:50.968149 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/schema_property.py
--rw-r--r--   0        0        0     1785 2022-08-08 20:54:50.968212 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/singer_primary_key.py
--rw-r--r--   0        0        0      502 2022-08-08 20:54:50.968294 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/__init__.py
--rw-r--r--   0        0        0     1034 2022-08-08 20:54:50.968353 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/file_is_compressed_file_specification.py
--rw-r--r--   0        0        0      482 2022-08-08 20:54:50.968417 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/folder_is_shapefile_file_specification.py
--rw-r--r--   0        0        0      562 2022-08-08 20:54:50.968474 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/state_message_is_cherre_bookmark_specification.py
--rw-r--r--   0        0        0      475 2022-08-08 20:54:50.968525 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/typing_defs.py
--rw-r--r--   0        0        0      830 2022-08-08 20:54:50.968575 cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/uri.py
--rw-r--r--   0        0        0      985 2023-07-07 15:19:27.395892 cherre_singer_ingest-16.6.6/pyproject.toml
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 cherre_singer_ingest-16.6.6/setup.py
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 cherre_singer_ingest-16.6.6/PKG-INFO
+-rw-r--r--   0        0        0     2431 2023-07-06 19:43:04.844780 cherre_singer_ingest-16.6.7/cherre_singer_ingest/__init__.py
+-rw-r--r--   0        0        0      179 2022-08-08 20:54:50.962605 cherre_singer_ingest-16.6.7/cherre_singer_ingest/factories/__init__.py
+-rw-r--r--   0        0        0     5046 2022-08-08 20:54:50.962696 cherre_singer_ingest-16.6.7/cherre_singer_ingest/factories/bookmark_factory.py
+-rw-r--r--   0        0        0     2354 2022-08-08 20:54:50.962778 cherre_singer_ingest-16.6.7/cherre_singer_ingest/factories/remote_file_uri_factory.py
+-rw-r--r--   0        0        0      356 2023-06-14 17:20:33.576704 cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/__init__.py
+-rw-r--r--   0        0        0     4238 2022-08-08 20:54:50.962977 cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/base_state_repository.py
+-rw-r--r--   0        0        0     5499 2022-08-08 20:54:50.963053 cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/big_query_ingest_state_repository.py
+-rw-r--r--   0        0        0     6850 2022-08-09 06:23:37.493294 cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/cloud_sql_ingest_state_repository.py
+-rw-r--r--   0        0        0     2141 2023-07-06 19:43:04.844937 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/__init__.py
+-rw-r--r--   0        0        0     4691 2023-07-10 17:29:04.182313 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/bookmark_service.py
+-rw-r--r--   0        0        0    10725 2022-08-08 20:54:50.963424 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/bq.py
+-rw-r--r--   0        0        0      925 2022-08-08 20:54:50.963500 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/clean_column_name.py
+-rw-r--r--   0        0        0    10772 2022-08-08 20:54:50.963602 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/common.py
+-rw-r--r--   0        0        0       35 2022-08-08 20:54:50.963674 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/constants.py
+-rw-r--r--   0        0        0      627 2023-01-26 18:00:06.910174 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/data_formats.py
+-rw-r--r--   0        0        0      311 2022-08-08 20:54:50.963822 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/env_var_utils.py
+-rw-r--r--   0        0        0      573 2022-08-08 20:54:50.963895 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/flatten_object.py
+-rw-r--r--   0        0        0    11041 2022-08-08 20:54:50.964018 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/gcs.py
+-rw-r--r--   0        0        0      808 2022-08-08 20:54:50.964099 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/get_login_token.py
+-rw-r--r--   0        0        0     6942 2022-08-08 20:54:50.964198 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/run_command.py
+-rw-r--r--   0        0        0     1789 2022-08-08 20:54:50.964273 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/run_custom_image_tap.py
+-rw-r--r--   0        0        0     1277 2022-08-08 20:54:50.964354 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/sftp.py
+-rw-r--r--   0        0        0      333 2022-08-08 20:54:50.964470 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/__init__.py
+-rw-r--r--   0        0        0     7743 2022-08-08 20:54:50.964560 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/avro_stream_writer.py
+-rw-r--r--   0        0        0      292 2022-08-08 20:54:50.964634 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/per_stream_writer_results.py
+-rw-r--r--   0        0        0     5902 2022-08-08 20:54:50.964712 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/stream_target.py
+-rw-r--r--   0        0        0      813 2022-08-08 20:54:50.964825 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/__init__.py
+-rw-r--r--   0        0        0     1502 2022-08-08 20:54:50.964910 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/avro_file_stream.py
+-rw-r--r--   0        0        0     2542 2023-07-06 19:43:04.845288 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/base_file_parsing_tap_stream.py
+-rw-r--r--   0        0        0     3696 2023-07-06 19:43:04.845631 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/base_tap_stream.py
+-rw-r--r--   0        0        0     1510 2022-08-08 20:54:50.965155 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/cached_stream.py
+-rw-r--r--   0        0        0     4735 2023-07-06 19:43:04.845967 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/csv_file_stream.py
+-rw-r--r--   0        0        0     1336 2022-08-08 20:54:50.965294 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/fixed_width_file_stream.py
+-rw-r--r--   0        0        0     1615 2022-08-08 20:54:50.965368 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/json_file_stream.py
+-rw-r--r--   0        0        0     3129 2023-07-06 19:43:04.846075 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/rest_stream.py
+-rw-r--r--   0        0        0     3525 2022-08-08 20:54:50.965522 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/shapefile_file_stream.py
+-rw-r--r--   0        0        0     1079 2022-08-08 20:54:50.965626 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/__init__.py
+-rw-r--r--   0        0        0     2628 2022-08-08 20:54:50.965705 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_api_tap.py
+-rw-r--r--   0        0        0     9910 2023-05-15 13:44:36.386150 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_file_parsing_tap.py
+-rw-r--r--   0        0        0    16299 2022-08-08 20:54:50.965989 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_ftp_file_tap.py
+-rw-r--r--   0        0        0     2657 2022-08-08 20:54:50.966080 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_bucket_file_tap.py
+-rw-r--r--   0        0        0     2974 2022-08-08 20:54:50.966138 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_bucket_folder_tap.py
+-rw-r--r--   0        0        0     3266 2022-08-08 20:54:50.966217 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_storage_tap.py
+-rw-r--r--   0        0        0     7278 2022-08-08 20:54:50.966291 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_tap.py
+-rw-r--r--   0        0        0     4260 2022-08-08 20:54:50.966362 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/big_query_table_tap.py
+-rw-r--r--   0        0        0     1131 2022-08-08 20:54:50.966460 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/error_throwing_tap.py
+-rw-r--r--   0        0        0     3139 2022-08-08 20:54:50.966538 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_csv_bucket_file_tap.py
+-rw-r--r--   0        0        0     2701 2022-08-08 20:54:50.966622 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_json_bucket_file_tap.py
+-rw-r--r--   0        0        0     3323 2022-08-08 20:54:50.966683 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_shapefile_bucket_file_tap.py
+-rw-r--r--   0        0        0      917 2022-08-08 20:54:50.966748 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/simple_test_tap.py
+-rw-r--r--   0        0        0     3420 2022-08-08 20:54:50.966838 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/webpage_tap.py
+-rw-r--r--   0        0        0      348 2022-08-08 20:54:50.966923 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/__init__.py
+-rw-r--r--   0        0        0     9824 2023-07-05 16:55:21.809044 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/base_cherre_target.py
+-rw-r--r--   0        0        0     3557 2023-07-05 16:56:28.939545 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/cherre_big_query_external_data_target.py
+-rw-r--r--   0        0        0     6095 2022-08-08 20:54:50.967148 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/cherre_parsed_data_lake_target.py
+-rw-r--r--   0        0        0     2812 2022-08-08 20:54:50.967227 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/unzip_service.py
+-rw-r--r--   0        0        0     3492 2022-08-08 20:54:50.967298 cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/unzip_service_with_bookmarks.py
+-rw-r--r--   0        0        0     1526 2023-07-06 19:43:04.846193 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/__init__.py
+-rw-r--r--   0        0        0     1388 2022-08-08 20:54:50.967453 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/exceptions.py
+-rw-r--r--   0        0        0      719 2023-07-06 19:43:04.846481 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/__init__.py
+-rw-r--r--   0        0        0      707 2022-08-08 20:54:50.967597 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/bookmark_type.py
+-rw-r--r--   0        0        0     1356 2022-08-08 20:54:50.967683 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_bookmark.py
+-rw-r--r--   0        0        0     1221 2022-08-08 20:54:50.967742 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_failed_bookmark.py
+-rw-r--r--   0        0        0     1910 2022-08-08 20:54:50.967796 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_bookmark.py
+-rw-r--r--   0        0        0     1485 2022-08-08 20:54:50.967853 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_failed_bookmark.py
+-rw-r--r--   0        0        0     1794 2022-08-08 20:54:50.967913 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/ingest_bookmark.py
+-rw-r--r--   0        0        0      235 2022-08-08 20:54:50.967965 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/uri_bookmark.py
+-rw-r--r--   0        0        0     1010 2022-08-08 20:54:50.968025 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/remote_file.py
+-rw-r--r--   0        0        0     3227 2022-08-08 20:54:50.968095 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/run_singer_command.py
+-rw-r--r--   0        0        0      141 2022-08-08 20:54:50.968149 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/schema_property.py
+-rw-r--r--   0        0        0     1785 2022-08-08 20:54:50.968212 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/singer_primary_key.py
+-rw-r--r--   0        0        0      502 2022-08-08 20:54:50.968294 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/__init__.py
+-rw-r--r--   0        0        0     1034 2022-08-08 20:54:50.968353 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/file_is_compressed_file_specification.py
+-rw-r--r--   0        0        0      482 2022-08-08 20:54:50.968417 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/folder_is_shapefile_file_specification.py
+-rw-r--r--   0        0        0      562 2022-08-08 20:54:50.968474 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/state_message_is_cherre_bookmark_specification.py
+-rw-r--r--   0        0        0      475 2022-08-08 20:54:50.968525 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/typing_defs.py
+-rw-r--r--   0        0        0      830 2022-08-08 20:54:50.968575 cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/uri.py
+-rw-r--r--   0        0        0      985 2023-07-10 17:29:30.963412 cherre_singer_ingest-16.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 cherre_singer_ingest-16.6.7/setup.py
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 cherre_singer_ingest-16.6.7/PKG-INFO
```

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/factories/bookmark_factory.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/factories/bookmark_factory.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/factories/remote_file_uri_factory.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/factories/remote_file_uri_factory.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/base_state_repository.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/base_state_repository.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/big_query_ingest_state_repository.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/big_query_ingest_state_repository.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/repositories/cloud_sql_ingest_state_repository.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/repositories/cloud_sql_ingest_state_repository.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/bookmark_service.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/bookmark_service.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/bq.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/bq.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/clean_column_name.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/clean_column_name.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/common.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/common.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/data_formats.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/data_formats.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/flatten_object.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/flatten_object.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/gcs.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/gcs.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/get_login_token.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/get_login_token.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/run_command.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/run_command.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/run_custom_image_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/run_custom_image_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/sftp.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/sftp.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/avro_stream_writer.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/avro_stream_writer.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/stream_writers/stream_target.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/stream_writers/stream_target.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/avro_file_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/avro_file_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/base_file_parsing_tap_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/base_file_parsing_tap_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/base_tap_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/base_tap_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/cached_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/cached_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/csv_file_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/csv_file_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/fixed_width_file_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/fixed_width_file_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/json_file_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/json_file_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/rest_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/rest_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/streams/shapefile_file_stream.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/streams/shapefile_file_stream.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_api_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_api_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_file_parsing_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_file_parsing_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_ftp_file_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_ftp_file_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_bucket_file_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_bucket_file_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_bucket_folder_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_bucket_folder_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_google_cloud_storage_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_google_cloud_storage_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/base_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/base_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/big_query_table_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/big_query_table_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/error_throwing_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/error_throwing_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_csv_bucket_file_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_csv_bucket_file_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_json_bucket_file_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_json_bucket_file_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/google_cloud_shapefile_bucket_file_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/google_cloud_shapefile_bucket_file_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/simple_test_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/simple_test_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/taps/webpage_tap.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/taps/webpage_tap.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/base_cherre_target.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/base_cherre_target.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/cherre_big_query_external_data_target.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/cherre_big_query_external_data_target.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/targets/cherre_parsed_data_lake_target.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/targets/cherre_parsed_data_lake_target.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/unzip_service.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/unzip_service.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/services/unzip_service_with_bookmarks.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/services/unzip_service_with_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/exceptions.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/exceptions.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/__init__.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/bookmark_type.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/bookmark_type.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_bookmark.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_bookmark.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_failed_bookmark.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_read_failed_bookmark.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_bookmark.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_bookmark.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_failed_bookmark.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/file_unzipped_failed_bookmark.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/ingest_bookmarks/ingest_bookmark.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/ingest_bookmarks/ingest_bookmark.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/remote_file.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/remote_file.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/run_singer_command.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/run_singer_command.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/singer_primary_key.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/singer_primary_key.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/file_is_compressed_file_specification.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/file_is_compressed_file_specification.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/specifications/state_message_is_cherre_bookmark_specification.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/specifications/state_message_is_cherre_bookmark_specification.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/cherre_singer_ingest/value_items/uri.py` & `cherre_singer_ingest-16.6.7/cherre_singer_ingest/value_items/uri.py`

 * *Files identical despite different names*

### Comparing `cherre_singer_ingest-16.6.6/pyproject.toml` & `cherre_singer_ingest-16.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cherre_singer_ingest"
-version = "16.6.6"
+version = "16.6.7"
 description = "Library holding the taps and targets for Cherre ingestion"
 authors = ["Mathieson <mathieson@cherre.com>"]
 
 [[tool.poetry.source]]
 name = "cherre"
 url = "https://cherre-pypi.appspot.com/pypi"
 secondary = true
```

### Comparing `cherre_singer_ingest-16.6.6/setup.py` & `cherre_singer_ingest-16.6.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'pyfarmhash>=0.2.2,<0.3.0',
  'python-snappy>=0.6.0,<0.7.0',
  'singer-sdk==0.1.6',
  'xmltodict>=0.12.0,<0.13.0']
 
 setup_kwargs = {
     'name': 'cherre-singer-ingest',
-    'version': '16.6.6',
+    'version': '16.6.7',
     'description': 'Library holding the taps and targets for Cherre ingestion',
     'long_description': 'None',
     'author': 'Mathieson',
     'author_email': 'mathieson@cherre.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cherre_singer_ingest-16.6.6/PKG-INFO` & `cherre_singer_ingest-16.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cherre-singer-ingest
-Version: 16.6.6
+Version: 16.6.7
 Summary: Library holding the taps and targets for Cherre ingestion
 Author: Mathieson
 Author-email: mathieson@cherre.com
 Requires-Python: >=3.7,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

