# Comparing `tmp/openmsistream-1.5.3.tar.gz` & `tmp/openmsistream-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.5.3.tar", last modified: Mon Jul  3 19:10:32 2023, max compression
+gzip compressed data, was "openmsistream-1.6.0.tar", last modified: Mon Jul 10 20:06:54 2023, max compression
```

## Comparing `openmsistream-1.5.3.tar` & `openmsistream-1.6.0.tar`

### file list

```diff
@@ -1,116 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.520393 openmsistream-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-03 19:10:25.000000 openmsistream-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 19:10:25.000000 openmsistream-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 19:10:32.520393 openmsistream-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 19:10:25.000000 openmsistream-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.500393 openmsistream-1.5.3/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.500393 openmsistream-1.5.3/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.500393 openmsistream-1.5.3/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.504393 openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.504393 openmsistream-1.5.3/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/entity/upload_directory_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.508393 openmsistream-1.5.3/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.512393 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.512393 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.512393 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.512393 openmsistream-1.5.3/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.512393 openmsistream-1.5.3/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.516393 openmsistream-1.5.3/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.516393 openmsistream-1.5.3/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.520393 openmsistream-1.5.3/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-03 19:10:25.000000 openmsistream-1.5.3/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:10:32.500393 openmsistream-1.5.3/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:10:32.000000 openmsistream-1.5.3/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 19:10:25.000000 openmsistream-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 19:10:32.520393 openmsistream-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-03 19:10:25.000000 openmsistream-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.188393 openmsistream-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-10 20:06:45.000000 openmsistream-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 20:06:45.000000 openmsistream-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-10 20:06:54.188393 openmsistream-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-10 20:06:45.000000 openmsistream-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.176393 openmsistream-1.6.0/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.176393 openmsistream-1.6.0/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.176393 openmsistream-1.6.0/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.176393 openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.180393 openmsistream-1.6.0/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.180393 openmsistream-1.6.0/openmsistream/girder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/girder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/girder/girder_upload_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.180393 openmsistream-1.6.0/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.184393 openmsistream-1.6.0/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.188393 openmsistream-1.6.0/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24379 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/utilities/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 20:06:45.000000 openmsistream-1.6.0/openmsistream/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:06:54.176393 openmsistream-1.6.0/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 20:06:54.000000 openmsistream-1.6.0/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 20:06:45.000000 openmsistream-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 20:06:54.188393 openmsistream-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-10 20:06:45.000000 openmsistream-1.6.0/setup.py
```

### Comparing `openmsistream-1.5.3/LICENSE` & `openmsistream-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/PKG-INFO` & `openmsistream-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.3
+Version: 1.6.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.3.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.6.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.3/README.md` & `openmsistream-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.5.3***</div>
+#### <div align="center">***v1.6.0***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
```

### Comparing `openmsistream-1.5.3/openmsistream/__init__.py` & `openmsistream-1.6.0/openmsistream/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 import os
 from .data_file_io.entity.upload_data_file import UploadDataFile
 from .data_file_io.actor.data_file_upload_directory import DataFileUploadDirectory
 from .data_file_io.actor.data_file_download_directory import DataFileDownloadDirectory
 from .data_file_io.actor.data_file_stream_processor import DataFileStreamProcessor
 from .data_file_io.actor.data_file_stream_reproducer import DataFileStreamReproducer
 from .s3_buckets.s3_transfer_stream_processor import S3TransferStreamProcessor
+from .girder.girder_upload_stream_processor import GirderUploadStreamProcessor
+from .version import __version__
 
 __all__ = [
+    "__version__",
     "UploadDataFile",
     "DataFileUploadDirectory",
     "DataFileDownloadDirectory",
     "DataFileStreamProcessor",
     "DataFileStreamReproducer",
     "S3TransferStreamProcessor",
+    "GirderUploadStreamProcessor",
 ]
 
 # If running on Windows, try to pre-load the librdkafka.dll file
 if os.name == "nt":
     try:
         import confluent_kafka
     except Exception:
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/__init__.py` & `openmsistream-1.6.0/openmsistream/data_file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 class DataFileStreamProcessor(DataFileStreamHandler, DataFileChunkProcessor, ABC):
     """
     A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages
     into memory and perform some operation(s) when entire files are available.
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection
+    :param config_file: Path to the config file to use in defining the Broker connection
         and Consumers
-    :type config_path: :class:`pathlib.Path`
+    :type config_file: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     :param output_dir: Path to the directory where the log and csv registry files should be kept
         (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
     :param mode: a string flag determining whether reconstructed data files should
         have their contents stored only in "memory" (the default, and the fastest),
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     """
     A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages
     into memory, compute some processing result when entire files are available,
     and produce that result to a different topic.
 
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection,
+    :param config_file: Path to the config file to use in defining the Broker connection,
         Consumers, and Producers
-    :type config_path: :class:`pathlib.Path`
+    :type config_file: :class:`pathlib.Path`
     :param consumer_topic_name: Name of the topic to which the Consumers should be subscribed
     :type consumer_topic_name: str
     :param producer_topic_name: Name of the topic to which the Producer should produce
         the processing results
     :type producer_topic_name: str
     :param output_dir: Path to the directory where the log and csv registry files should be kept
         (if None a default will be created in the current directory)
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         and Producers
     :type config_path: :class:`pathlib.Path`
     :param upload_regex: only files matching this regular expression will be uploaded
     :type upload_regex: :func:`re.compile`, optional
     :param datafile_type: the type of data file that recognized files should be uploaded as
         (must be a subclass of :class:`~UploadDataFile`)
     :type datafile_type: :class:`~UploadDataFile`, optional
+    :param watchdog_lag_time: Number of seconds that files must remain static (unmodified)
+        for their uploads to begin
+    :type watchdog_lag_time: int
 
     :raises ValueError: if `datafile_type` is not a subclass of :class:`~UploadDataFile`
     """
 
     #################### CONSTANTS ####################
 
     # starting point for how long to wait between pinging the directory looking for new files
@@ -57,14 +60,15 @@
 
     def __init__(
         self,
         dirpath,
         config_path,
         upload_regex=RUN_CONST.DEFAULT_UPLOAD_REGEX,
         datafile_type=UploadDataFile,
+        watchdog_lag_time=RUN_CONST.DEFAULT_WATCHDOG_LAG_TIME,
         **kwargs,
     ):
         """
         Constructor method
         """
         # create a subdirectory for the logs
         self._logs_subdir = dirpath / self.LOG_SUBDIR_NAME
@@ -82,14 +86,15 @@
         self.__datafile_type = datafile_type
         self.__wait_time = self.MIN_WAIT_TIME
         self.__lock = Lock()
         self.__observer = Observer(timeout=self.WATCHDOG_OBSERVER_TIMEOUT)
         self.__event_handler = UploadDirectoryEventHandler(
             upload_regex=upload_regex,
             logs_subdir=self._logs_subdir,
+            lag_time=watchdog_lag_time,
             logger=self.logger,
         )
         self.__active_files_by_path = {}
         self.__status_message_files = {}
         self.__topic_name = None
         self.__chunk_size = None
         self.__file_registry = None
@@ -557,14 +562,15 @@
             "config",
             "topic_name",
             "upload_regex",
             "chunk_size",
             "queue_max_size",
             "update_seconds",
             "upload_existing",
+            "watchdog_lag_time",
         ]
         kwargs = {**superkwargs, "n_threads": RUN_CONST.N_DEFAULT_UPLOAD_THREADS}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
@@ -579,14 +585,15 @@
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
         # make the DataFileDirectory for the specified directory
         upload_file_directory = cls(
             args.upload_dir,
             args.config,
             upload_regex=args.upload_regex,
+            watchdog_lag_time=args.watchdog_lag_time,
             update_secs=args.update_seconds,
             streamlevel=args.logger_stream_level,
             filelevel=args.logger_file_level,
         )
         # listen for new files in the directory and run uploads until shut down
         run_start = datetime.datetime.now()
         if not args.upload_existing:
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.6.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,19 +389,21 @@
                 rel_filepath,
                 n_total_chunks,
                 datetime.datetime.now(),
                 datetime.datetime.now(),
             )
         self._add_to_succeeded_table(new_entry, f"p{prodid}")
         if existing_entry_addr is not None:
+            self._in_progress_table.lock.acquire()
             try:
                 self._in_progress_table.remove_entries(existing_entry_addr)
                 self._in_progress_table.dump_to_file()
             except ValueError:
                 pass
+            self._in_progress_table.lock.release()
 
     def register_file_computing_result_failed(
         self, filename, rel_filepath, n_total_chunks
     ):
         """
         Update a line in the table to show that a file failed to have its processing result computed
         """
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/data_file_directory.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/data_file_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,22 @@
             return dfc.filepath
         return dfc.filepath.with_name(
             dfc.filepath.stem + dfc.filename_append + dfc.filepath.suffix
         )
 
     @property
     @abstractmethod
+    def bytestring(self):
+        """
+        A bytestring of the data contained in the file. Not implemented in the base class.
+        """
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
     def check_file_hash(self):
         """
         The hash of the data in the file after it was read. Not implemented in the base class.
         """
         raise NotImplementedError
 
     @property
@@ -172,14 +180,23 @@
     #################### CONSTANTS ####################
 
     READ_BUFFER_SIZE = 4096
 
     #################### PROPERTIES ####################
 
     @property
+    def bytestring(self):
+        """
+        A bytestring of the data in the file
+        """
+        with open(self.full_filepath, "rb") as fp:
+            data = fp.read()
+        return data
+
+    @property
     def check_file_hash(self):
         """
         Hash of the file contents as read from its current location on disk
         """
         check_file_hash = sha512()
         with open(self.full_filepath, "rb") as fp:
             while True:
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/entity/upload_directory_event_handler.py` & `openmsistream-1.6.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,32 +26,31 @@
     timestamps of when they were updated. That dictionary can be polled for active
     file objects by the upload directory.
 
     :param upload_regex: only files matching this regular expression will be uploaded
     :type upload_regex: :func:`re.compile`, optional
     :param logs_subdir: path to the owning upload directory's "logs" directory
     :type logs_subdir: :class:`pathlib.Path`
+    :param watchdog_lag_time: Number of seconds that files must remain static (unmodified)
+        before it's given in :func:`get_new_files`
+    :type watchdog_lag_time: int
     """
 
-    #################### CONSTANTS ####################
-
-    # how long a file must remain unmodified before it's given in get_new_files
-    PERSISTENCE_SECS = 3
-
     #################### NEW PUBLIC FUNCTIONS ####################
 
-    def __init__(self, upload_regex, logs_subdir, **other_kwargs):
+    def __init__(self, upload_regex, logs_subdir, lag_time, **other_kwargs):
         """
         Constructor method
         """
         super().__init__(**other_kwargs)
         # variables for determining files whose events should be dispatched
         self.__upload_regex = upload_regex
         self._logs_subdir = logs_subdir
         self.__rootdir = self._logs_subdir.parent
+        self.__lag_time = lag_time
         # A thread lock
         self.__lock = RLock()
         # all currently active files
         self.__active_files_by_path = {}
 
     def get_new_files(self):
         """
@@ -61,15 +60,15 @@
         """
         keys_to_pop = []
         ref_timestamp = datetime.datetime.now()
         with self.__lock:
             for filepath, active_file in self.__active_files_by_path.items():
                 if (
                     ref_timestamp - active_file.last_updated
-                ).total_seconds() > self.PERSISTENCE_SECS:
+                ).total_seconds() > self.__lag_time:
                     keys_to_pop.append(filepath)
             for key in keys_to_pop:
                 yield self.__active_files_by_path.pop(key)
 
     def kick_back(self, handler_file):
         """
         Give back an :class:`EventHandlerActiveFile` so it can be processed later
```

### Comparing `openmsistream-1.5.3/openmsistream/data_file_io/utilities.py` & `openmsistream-1.6.0/openmsistream/data_file_io/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/__init__.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,16 +115,19 @@
         If no config file is found according to the conventions listed below, this function
         returns None and it will be assumed that no configuration for KafkaCrypto exists
 
         Options are:
         1) The regular config file has a "kafkacrypto" section with a "config_file" parameter
         that is the path to the KafkaCrypo config file
         2) The regular config file has a "kafkacrypto" section with a "node_id" parameter
-        corresponding to a named subdirectory in openmsistream/kafka_wrapper/config_files
-        that was created when the node was provisioned
+        corresponding to a named subdirectory that was created when the node was provisioned.
+        The subdirectory must be located in:
+        a) openmsistream/kafka_wrapper/config_files,
+        b) the same directory as the config file, or
+        c) the current directory
         """
         if "kafkacrypto" in self.available_group_names:
             kc_configs = self.get_config_dict_for_groups("kafkacrypto")
             # option 1 above
             if "config_file" in kc_configs:
                 path_as_str = (kc_configs["config_file"]).lstrip("file#")
                 if not pathlib.Path(path_as_str).is_file():
@@ -133,23 +136,28 @@
                         f"{self.filepath}) not found!"
                     )
                     self.logger.error(errmsg, exc_type=FileNotFoundError)
                 return path_as_str
             # option 2 above
             if "node_id" in kc_configs:
                 node_id = kc_configs["node_id"]
-                dirpath = RUN_CONST.CONFIG_FILE_DIR / node_id
-                filepath = dirpath / f"{node_id}.config"
-                if (not dirpath.is_dir()) or (not filepath.is_file()):
-                    errmsg = (
-                        "ERROR: no KafkaCrypto config file found in the default location "
-                        f"({filepath}) for node ID = {node_id}"
-                    )
-                    self.logger.error(errmsg, exc_type=FileNotFoundError)
-                return str(filepath)
+                dirpaths = [
+                    RUN_CONST.CONFIG_FILE_DIR / node_id,
+                    self.filepath.parent / node_id,
+                    pathlib.Path(".").resolve() / node_id,
+                ]
+                filepaths = [dpath / f"{node_id}.config" for dpath in dirpaths]
+                for filepath in filepaths:
+                    if filepath.is_file():
+                        return str(filepath)
+                errmsg = (
+                    f"ERROR: no KafkaCrypto config file found for node ID = {node_id}"
+                    f"(expected one of {filepaths})"
+                )
+                self.logger.error(errmsg, exc_type=FileNotFoundError)
         # no config file found
         return None
 
     def __convert_floats(self, given_dict):
         """
         Return a version of the dictionary "given_dict" where any values that can be
         converted to floats are converted to floats
```

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/producible.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/serialization.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.6.0/openmsistream/kafka_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.6.0/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.6.0/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 class MetadataJSONReproducer(DataFileStreamReproducer, ABC):
     """
     A class to extend for processing a stream of DataFileChunks, extracting metadata from
     fully-reconstructed files, and producing those metadata fields as JSON to a different topic.
 
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection,
+    :param config_file: Path to the config file to use in defining the Broker connection,
         Consumers, and Producers
-    :type config_path: :class:`pathlib.Path`
+    :type config_file: :class:`pathlib.Path`
     :param consumer_topic_name: Name of the topic to which the Consumer(s) should be subscribed
     :type consumer_topic_name: str
     :param producer_topic_name: Name of the topic to which the Producer(s) should produce
         the processing results
     :type producer_topic_name: str
     :param output_dir: Path to the directory where the log and csv registry files should be kept
         (if None a default will be created in the current directory)
```

### Comparing `openmsistream-1.5.3/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.6.0/openmsistream/s3_buckets/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/s3_buckets/s3_data_transfer.py` & `openmsistream-1.6.0/openmsistream/s3_buckets/s3_data_transfer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.6.0/openmsistream/s3_buckets/s3_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.6.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from ..data_file_io.actor.data_file_stream_processor import DataFileStreamProcessor
 from .config_file_parser import S3ConfigFileParser
 from .s3_data_transfer import S3DataTransfer
 
 
 class S3TransferStreamProcessor(DataFileStreamProcessor):
     """
-    A class to reconstruct data files read as messages from a topic, hold them in memory,
-    and transfer them to an S3 bucket when all of their messages have been received
+    A class to reconstruct data files read as messages from a topic, hold them in memory
+    or on disk, and transfer them to an S3 bucket when all of their messages have been
+    received
 
     :param bucket_name: Name of the S3 bucket into which reconstructed files should be transferred
     :type bucket_name: str
     :param config_path: Path to the config file to use in defining the Broker connection
         and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
@@ -51,17 +52,17 @@
 
     def _process_downloaded_data_file(self, datafile, lock):
         """
         Transfer a fully-reconstructed file to the S3 bucket and verify that its contents
         in the bucket match its original hash from disk.
         Logs a warning if the file hashes don't match.
 
-        :param datafile: A :class:`~DownloadDataFileToMemory` object that has received
+        :param datafile: A :class:`~DownloadDataFile` object that has received
             all of its messages from the topic
-        :type datafile: :class:`~DownloadDataFileToMemory`
+        :type datafile: :class:`~DownloadDataFile`
         :param lock: Acquiring this :class:`threading.Lock` object ensures that only one instance
             of :func:`~_process_downloaded_data_file` is running at once
         :type lock: :class:`threading.Lock`
 
         :return: None if processing was successful, a caught Exception otherwise
         """
         object_key = self.__get_datafile_object_key(datafile)
```

### Comparing `openmsistream-1.5.3/openmsistream/services/config.py` & `openmsistream-1.6.0/openmsistream/services/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.6.0/openmsistream/services/examples/runnable_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/examples/script_example.py` & `openmsistream-1.6.0/openmsistream/services/examples/script_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/install_service.py` & `openmsistream-1.6.0/openmsistream/services/install_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/linux_service_manager.py` & `openmsistream-1.6.0/openmsistream/services/linux_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/manage_service.py` & `openmsistream-1.6.0/openmsistream/services/manage_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/service_manager_base.py` & `openmsistream-1.6.0/openmsistream/services/service_manager_base.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/utilities.py` & `openmsistream-1.6.0/openmsistream/services/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/services/windows_service_manager.py` & `openmsistream-1.6.0/openmsistream/services/windows_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/__init__.py` & `openmsistream-1.6.0/openmsistream/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/argument_parsing.py` & `openmsistream-1.6.0/openmsistream/utilities/argument_parsing.py`

 * *Files 14% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                 ),
             },
         ],
         "queue_max_size": [
             "optional",
             {
                 "default": RUN_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
-                "type": int,
+                "type": positive_int,
                 "help": (
                     "Maximum allowed size in MB of the internal upload queue. "
                     "Use to adjust RAM usage if necessary."
                 ),
             },
         ],
         "update_seconds": [
@@ -312,14 +312,25 @@
                 "help": (
                     "Add this flag to upload files already existing in addition to those "
                     "added to the directory after this code starts running (by default "
                     "only files added after startup will be uploaded)"
                 ),
             },
         ],
+        "watchdog_lag_time": [
+            "optional",
+            {
+                "default": RUN_CONST.DEFAULT_WATCHDOG_LAG_TIME,
+                "type": int,
+                "help": (
+                    "Number of seconds that a file must remain static (unmodified) "
+                    "for its upload to begin"
+                ),
+            },
+        ],
         "consumer_group_id": [
             "optional",
             {"default": "create_new", "help": "ID to use for all consumers in the group"},
         ],
         "optional_output_dir": [
             "optional",
             {"type": create_dir, "help": "Optional path to directory to put output in"},
@@ -394,14 +405,67 @@
                 "type": logger_string_to_level,
                 "default": "warning",
                 "help": (
                     "Messages below this level will not be processed by the logger's file handler"
                 ),
             },
         ],
+        "girder_api_url": [
+            "positional",
+            {
+                "help": (
+                    "The full path to the REST API of a Girder instance, "
+                    "e.g. http://my.girder.com/api/v1."
+                )
+            },
+        ],
+        "girder_api_key": [
+            "positional",
+            {"help": "The API key to use for authenticating to the Girder instance"},
+        ],
+        "girder_root_folder_id": [
+            "optional",
+            {
+                "help": (
+                    "The ID of the Girder Folder relative to which files should be "
+                    "uploaded. If this argument is given, it will supersede both of the "
+                    "'collection_name' and 'girder_root_folder_path' arguments."
+                ),
+            },
+        ],
+        "collection_name": [
+            "optional",
+            {
+                "help": (
+                    "The name of the top-level Collection to which files should be uploaded. "
+                    "Superseded if 'girder_root_folder_id' is given."
+                ),
+            },
+        ],
+        "girder_root_folder_path": [
+            "optional",
+            {
+                "help": (
+                    "The name of the Folder inside the top-level Collection relative to "
+                    "which files should be uploaded. A path to a subdirectory in the "
+                    "Collection can be given using forward slashes. "
+                    "Superseded if 'girder_root_folder_id' is given. "
+                    "(default = collection_name/topic_name)"
+                ),
+            },
+        ],
+        "provider": [
+            "optional",
+            {
+                "help": (
+                    'Adding this argument will add a corresponding "provider" metadata '
+                    "field to all created folders and items"
+                ),
+            },
+        ],
     }
 
     #################### OVERLOADED FUNCTIONS ####################
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__argnames_added = []
```

### Comparing `openmsistream-1.5.3/openmsistream/utilities/config.py` & `openmsistream-1.6.0/openmsistream/utilities/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,14 @@
     PRODUCTION_CONFIG_FILE = "prod"
     # matches everything except something starting with a '.' or ending in '.log'
     DEFAULT_UPLOAD_REGEX = re.compile(r"^((?!(\.|.*.log))).*$")
     # default size in bytes of each file upload chunk
     DEFAULT_CHUNK_SIZE = 524288
     # default maximum size (in MB) of the internal upload Queue
     DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES = 500
+    # default number of seconds that a file must remain static for uploading to start
+    DEFAULT_WATCHDOG_LAG_TIME = 3
+    # default Girder collection name
+    DEFAULT_COLLECTION_NAME = "WholeTale Catalog"
 
 
 RUN_CONST = RunConstants()
```

### Comparing `openmsistream-1.5.3/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.6.0/openmsistream/utilities/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/controlled_process.py` & `openmsistream-1.6.0/openmsistream/utilities/controlled_process.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.6.0/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.6.0/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.6.0/openmsistream/utilities/dataclass_table.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.6.0/openmsistream/utilities/exception_tracking_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/has_arguments.py` & `openmsistream-1.6.0/openmsistream/utilities/has_arguments.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/logging.py` & `openmsistream-1.6.0/openmsistream/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/misc.py` & `openmsistream-1.6.0/openmsistream/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.6.0/openmsistream/utilities/provision_wrapper.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream/utilities/runnable.py` & `openmsistream-1.6.0/openmsistream/utilities/runnable.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.3/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.6.0/openmsistream.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.3
+Version: 1.6.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.3.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.6.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.3/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.6.0/openmsistream.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 openmsistream/__init__.py
+openmsistream/version.py
 openmsistream.egg-info/PKG-INFO
 openmsistream.egg-info/SOURCES.txt
 openmsistream.egg-info/dependency_links.txt
 openmsistream.egg-info/entry_points.txt
 openmsistream.egg-info/requires.txt
 openmsistream.egg-info/top_level.txt
 openmsistream/data_file_io/__init__.py
@@ -28,14 +29,16 @@
 openmsistream/data_file_io/entity/data_file.py
 openmsistream/data_file_io/entity/data_file_chunk.py
 openmsistream/data_file_io/entity/data_file_directory.py
 openmsistream/data_file_io/entity/download_data_file.py
 openmsistream/data_file_io/entity/reproducer_message.py
 openmsistream/data_file_io/entity/upload_data_file.py
 openmsistream/data_file_io/entity/upload_directory_event_handler.py
+openmsistream/girder/__init__.py
+openmsistream/girder/girder_upload_stream_processor.py
 openmsistream/kafka_wrapper/__init__.py
 openmsistream/kafka_wrapper/config_file_parser.py
 openmsistream/kafka_wrapper/consumer_and_producer_group.py
 openmsistream/kafka_wrapper/consumer_group.py
 openmsistream/kafka_wrapper/controlled_message_processor.py
 openmsistream/kafka_wrapper/controlled_message_reproducer.py
 openmsistream/kafka_wrapper/openmsistream_consumer.py
```

### Comparing `openmsistream-1.5.3/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.6.0/openmsistream.egg-info/entry_points.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [console_scripts]
 DataFileDownloadDirectory = openmsistream.data_file_io.actor.data_file_download_directory:main
 DataFileUploadDirectory = openmsistream.data_file_io.actor.data_file_upload_directory:main
+GirderUploadStreamProcessor = openmsistream.girder.girder_upload_stream_processor:main
 InstallService = openmsistream.services.install_service:main
 ManageService = openmsistream.services.manage_service:main
 ProvisionNode = openmsistream.utilities.provision_wrapper:main
 S3TransferStreamProcessor = openmsistream.s3_buckets.s3_transfer_stream_processor:main
 UploadDataFile = openmsistream.data_file_io.entity.upload_data_file:main
```

### Comparing `openmsistream-1.5.3/setup.py` & `openmsistream-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # imports
-import setuptools
+import setuptools, pathlib
 
-# version tag
-version = "1.5.3"
+# read version tag
+version = None
+version_path = pathlib.Path(__file__).parent/"openmsistream"/"version.py"
+with open(version_path,"r") as version_file:
+    for line in version_file.readlines():
+        if line.startswith("__version__"):
+            version = line.strip().split("=")[-1].strip().strip('"')
+if not version:
+    raise RuntimeError("ERROR: Failed to find version tag!")
 
+# read a portion of the README to get the description
 long_description = ""
 with open("README.md", "r") as readme:
     for il, line in enumerate(readme.readlines(), start=1):
         if il >= 18:
             long_description += line
 
 setupkwargs = dict(
@@ -31,36 +39,40 @@
             "UploadDataFile=openmsistream.data_file_io.entity.upload_data_file:main",
             "DataFileUploadDirectory=openmsistream.data_file_io.actor.data_file_upload_directory:main",
             "DataFileDownloadDirectory=openmsistream.data_file_io.actor.data_file_download_directory:main",
             "InstallService=openmsistream.services.install_service:main",
             "ManageService=openmsistream.services.manage_service:main",
             "ProvisionNode=openmsistream.utilities.provision_wrapper:main",
             "S3TransferStreamProcessor=openmsistream.s3_buckets.s3_transfer_stream_processor:main",
+            "GirderUploadStreamProcessor=openmsistream.girder.girder_upload_stream_processor:main",
         ],
     },
     python_requires=">=3.7,<3.10",
     install_requires=[
         "atomicwrites>=1.4.1",
         "boto3>=1.26.84",
         "confluent-kafka>=2.0.2",
+        "girder-client>=3.1.20",
         "kafkacrypto>=0.9.10.0",
         "matplotlib",
         "methodtools",
         "msgpack",
         "watchdog>=3.0.0",
     ],
     extras_require={
         "test": [
             "beautifulsoup4",
             "black",
+            "docker",
             "gitpython",
             "lxml",
             "marko[toc]==1.3.0",
             "pyflakes>=3.0.1",
             "pylint>=2.16.3",
+            "requests",
             "tempenv>=2.0.0",
         ],
         "docs": [
             "sphinx>=6.1.3",
             "sphinx_rtd_theme>=1.2.0",
         ],
         "dev": [
```

