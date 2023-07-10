# Comparing `tmp/fastkafka-0.8.0rc1.tar.gz` & `tmp/fastkafka-0.8.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.8.0rc1.tar", last modified: Thu Jul  6 10:02:43 2023, max compression
+gzip compressed data, was "fastkafka-0.8.1rc0.tar", last modified: Mon Jul 10 07:48:36 2023, max compression
```

## Comparing `fastkafka-0.8.0rc1.tar` & `fastkafka-0.8.1rc0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    12572 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/CONTRIBUTING.md
--rw-r--r--   0 tvrtko    (1004) tvrtko    (1005)    11357 2023-01-26 06:58:43.000000 fastkafka-0.8.0rc1/LICENSE
--rw-r--r--   0 tvrtko    (1004) tvrtko    (1005)      111 2023-01-26 06:58:43.000000 fastkafka-0.8.0rc1/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    24706 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/PKG-INFO
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    23278 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/README.md
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      525 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/__init__.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      398 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_aiokafka_imports.py
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    40048 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13467 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     2108 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     5764 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      996 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4981 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13623 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    19082 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     2905 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     6991 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    15024 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1612 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4136 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4730 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13150 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     8102 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    11893 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    10312 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    32769 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    51560 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    87787 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     7313 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    27911 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    28557 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13966 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     5428 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      598 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      454 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/executors.py
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      858 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    24706 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1441 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        1 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      146 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        1 2023-01-26 07:01:03.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      693 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)       10 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1231 2023-07-06 09:59:12.000000 fastkafka-0.8.0rc1/settings.ini
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)       38 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/setup.cfg
--rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     3780 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.491152 fastkafka-0.8.1rc0/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12572 2023-06-29 13:51:03.000000 fastkafka-0.8.1rc0/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-06-01 05:47:44.000000 fastkafka-0.8.1rc0/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-06-01 05:47:44.000000 fastkafka-0.8.1rc0/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24706 2023-07-10 07:48:36.491152 fastkafka-0.8.1rc0/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    23278 2023-07-10 07:16:35.000000 fastkafka-0.8.1rc0/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.483152 fastkafka-0.8.1rc0/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      398 2023-07-10 07:45:56.000000 fastkafka-0.8.1rc0/fastkafka/_aiokafka_imports.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.483152 fastkafka-0.8.1rc0/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    40048 2023-07-10 07:45:58.000000 fastkafka-0.8.1rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13467 2023-07-10 07:45:58.000000 fastkafka-0.8.1rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5764 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.487152 fastkafka-0.8.1rc0/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4981 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13623 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19082 2023-07-10 07:45:58.000000 fastkafka-0.8.1rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-07-10 07:45:58.000000 fastkafka-0.8.1rc0/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.487152 fastkafka-0.8.1rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    15024 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1612 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8478 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11893 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    10312 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    32681 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51560 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    87787 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7313 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.487152 fastkafka-0.8.1rc0/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:46:00.000000 fastkafka-0.8.1rc0/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    27911 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28557 2023-07-10 07:45:56.000000 fastkafka-0.8.1rc0/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13966 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5428 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-07-10 07:45:59.000000 fastkafka-0.8.1rc0/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-07-10 07:45:57.000000 fastkafka-0.8.1rc0/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-07-10 07:45:56.000000 fastkafka-0.8.1rc0/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-07-10 07:48:36.483152 fastkafka-0.8.1rc0/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24706 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1441 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-06-01 08:53:21.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      693 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-07-10 07:48:36.000000 fastkafka-0.8.1rc0/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-07-10 07:45:36.000000 fastkafka-0.8.1rc0/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-07-10 07:48:36.491152 fastkafka-0.8.1rc0/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3780 2023-07-10 07:16:35.000000 fastkafka-0.8.1rc0/setup.py
```

### Comparing `fastkafka-0.8.0rc1/CONTRIBUTING.md` & `fastkafka-0.8.1rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/LICENSE` & `fastkafka-0.8.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/PKG-INFO` & `fastkafka-0.8.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.8.0rc1
+Version: 0.8.1rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.8.0rc1/README.md` & `fastkafka-0.8.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/__init__.py` & `fastkafka-0.8.1rc0/fastkafka/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0rc1"
+__version__ = "0.8.1rc0"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.8.0rc1/fastkafka/_application/app.py` & `fastkafka-0.8.1rc0/fastkafka/_application/app.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_application/tester.py` & `fastkafka-0.8.1rc0/fastkafka/_application/tester.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_cli.py` & `fastkafka-0.8.1rc0/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_cli_docs.py` & `fastkafka-0.8.1rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_cli_testing.py` & `fastkafka-0.8.1rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/_subprocess.py` & `fastkafka-0.8.1rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.8.1rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/asyncapi.py` & `fastkafka-0.8.1rc0/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/benchmarking.py` & `fastkafka-0.8.1rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.8.1rc0/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/encoder/avro.py` & `fastkafka-0.8.1rc0/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/encoder/json.py` & `fastkafka-0.8.1rc0/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/helpers.py` & `fastkafka-0.8.1rc0/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/logger.py` & `fastkafka-0.8.1rc0/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/meta.py` & `fastkafka-0.8.1rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/producer_decorator.py` & `fastkafka-0.8.1rc0/fastkafka/_components/producer_decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 # %% ../../nbs/013_ProducerDecorator.ipynb 1
 import asyncio
 import functools
 import random
 import time
 from asyncio import iscoroutinefunction  # do not use the version from inspect
 from dataclasses import dataclass
+from functools import partial
 from inspect import Parameter
 from typing import *
 
 from aiokafka import AIOKafkaProducer
-from aiokafka.errors import KafkaTimeoutError
+from aiokafka.errors import KafkaTimeoutError, RequestTimedOutError
 from aiokafka.producer.message_accumulator import BatchBuilder
 from pydantic import BaseModel
 
 from .logger import get_logger
 from .meta import export
 from .helpers import remove_suffix
 
@@ -79,15 +80,21 @@
 # %% ../../nbs/013_ProducerDecorator.ipynb 12
 def _wrap_in_event(
     message: Union[BaseModel, List[BaseModel], KafkaEvent]
 ) -> KafkaEvent:
     return message if type(message) == KafkaEvent else KafkaEvent(message)
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 15
-def release_callback(fut: asyncio.Future) -> None:
+def release_callback(
+    fut: asyncio.Future, topic: str, wrapped_val: KafkaEvent[BaseModel]
+) -> None:
+    if fut.exception() is not None:
+        logger.warning(
+            f"release_callback(): Exception {fut.exception()=}, raised when producing {wrapped_val.message=} to {topic=}"
+        )
     pass
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 16
 async def produce_single(  # type: ignore
     producer: AIOKafkaProducer,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
@@ -103,23 +110,25 @@
         wrapped_val (KafkaEvent[BaseModel]): The wrapped Kafka event containing the message.
     """
     while True:
         try:
             fut = await producer.send(
                 topic, encoder_fn(wrapped_val.message), key=wrapped_val.key
             )
-            fut.add_done_callback(release_callback)
+            fut.add_done_callback(
+                partial(release_callback, topic=topic, wrapped_val=wrapped_val)
+            )
             break
         except KafkaTimeoutError as e:
             logger.warning(
-                f"produce_single(): Exception {e} raised when producing {wrapped_val.message} to {topic=}, sleeping for 1 second and retrying.."
+                f"produce_single(): Exception {e=} raised when producing {wrapped_val.message} to {topic=}, sleeping for 1 second and retrying.."
             )
             await asyncio.sleep(1)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 20
+# %% ../../nbs/013_ProducerDecorator.ipynb 21
 async def send_batch(  # type: ignore
     producer: AIOKafkaProducer, topic: str, batch: BatchBuilder, key: Optional[bytes]
 ) -> None:
     """
     Sends a batch of messages to the Kafka producer.
 
     Args:
@@ -180,15 +189,15 @@
             batch = producer.create_batch()
             batch.append(
                 key=None, value=encoder_fn(message), timestamp=int(time.time() * 1000)
             )
 
     await send_batch(producer, topic, batch, wrapped_val.key)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 23
+# %% ../../nbs/013_ProducerDecorator.ipynb 24
 def producer_decorator(
     producer_store: Dict[str, Any],
     func: ProduceCallable,
     topic_key: str,
     encoder_fn: Callable[[BaseModel], bytes],
 ) -> ProduceCallable:
     """
```

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/task_streaming.py` & `fastkafka-0.8.1rc0/fastkafka/_components/task_streaming.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_components/test_dependencies.py` & `fastkafka-0.8.1rc0/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_docusaurus_helper.py` & `fastkafka-0.8.1rc0/fastkafka/_docusaurus_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,27 +276,30 @@
 
     Args:
         symbol: The symbol for which the documentation needs to be generated in markdown format.
 
     Returns:
         The markdown-formatted docstring.
     """
-    parsed_docstring = parse(symbol.__doc__)  # type: ignore
+    if symbol.__doc__ is None:
+        return ""
+
+    parsed_docstring = parse(symbol.__doc__)
     formatted_docstring = f"{parsed_docstring.short_description}\n\n"
     formatted_docstring += (
         f"{parsed_docstring.long_description}\n\n"
         if parsed_docstring.long_description
         else ""
     )
     formatted_docstring += _format_docstring_sections(symbol, parsed_docstring)
     ret_val = _format_free_links(formatted_docstring)
 
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 46
+# %% ../nbs/096_Docusaurus_Helper.ipynb 47
 def _get_submodules(module_name: str) -> List[str]:
     """Get a list of all submodules contained within the module.
 
     Args:
         module_name: The name of the module to retrieve submodules from
 
     Returns:
@@ -305,15 +308,15 @@
     members = _import_all_members(module_name)
     members_with_submodules = _add_all_submodules(members)
     members_with_submodules_str: List[str] = [
         x[:-1] if x.endswith(".") else x for x in members_with_submodules
     ]
     return members_with_submodules_str
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 48
+# %% ../nbs/096_Docusaurus_Helper.ipynb 49
 def _load_submodules(
     module_name: str, members_with_submodules: List[str]
 ) -> List[Type]:
     """Load the given submodules from the module.
 
     Args:
         module_name: The name of the module whose submodules to load
@@ -329,15 +332,15 @@
     names = [
         y
         for x, y in members
         if f"{y.__module__}.{y.__name__}" in members_with_submodules
     ]
     return names
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 50
+# %% ../nbs/096_Docusaurus_Helper.ipynb 51
 def _get_parameters(_signature: Signature) -> List[str]:
     """Convert a function's signature into a string representation of its parameter list.
 
     Args:
         _signature: The signature object representing the function's signature.
 
     Returns:
@@ -350,15 +353,15 @@
         else f"{param.name}='{param.default}'"
         if isinstance(param.default, str)
         else f"{param.name}={param.default}"
         for param in params
     ]
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 54
+# %% ../nbs/096_Docusaurus_Helper.ipynb 55
 def _format_symbol_definition(symbol: Type, params_list: List[str]) -> str:
     """Format the given symbol parameters by adding a new line and indentation.
 
     Args:
         symbol: The symbol for which the symbol definition needs to be formatted.
         params_list: A string representation of the parameter list.
 
@@ -370,15 +373,15 @@
         return f"{symbol.__name__}()\n"
     elif len(f"{symbol.__name__}({parameters})") <= 79:
         return f"{symbol.__name__}(\n    {parameters}\n)\n"
     else:
         formatted_parameters = "".join([f"\n    {param}," for param in params_list])
         return f"{symbol.__name__}({formatted_parameters}\n)\n"
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 61
+# %% ../nbs/096_Docusaurus_Helper.ipynb 62
 def _get_exps(mod: str) -> Dict[str, str]:
     mf = _find_mod(mod)
     if not mf:
         return {}
     txt = mf.read_text()
     _def_types = ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef
     d = {}
@@ -392,15 +395,15 @@
                     tree.name + "." + t2.name: f"{t2.lineno}-L{t2.end_lineno}"
                     for t2 in tree.body
                     if isinstance(t2, _def_types)
                 }
             )
     return d
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 63
+# %% ../nbs/096_Docusaurus_Helper.ipynb 64
 def _lineno(sym: str, fname: str) -> Optional[str]:
     return _get_exps(fname).get(sym, None) if fname else None
 
 
 @lru_cache(None)
 class CustomNbdevLookup(NbdevLookup.__wrapped__):  # type: ignore
     def __init__(
@@ -416,15 +419,15 @@
         res = self[sym]
         if not isinstance(res, tuple):
             return None
         _, py, gh = res
         line = _lineno(sym, py)
         return f"{gh}#L{line}"
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 66
+# %% ../nbs/096_Docusaurus_Helper.ipynb 67
 def _get_symbol_source_link(symbol: Type, lib_version: str) -> str:
     """Returns the source code link for a given symbol.
 
     Args:
         symbol: The symbol to get the source code link for.
         lib_version: The current version of the library.
 
@@ -440,15 +443,15 @@
     href = (
         source_link.replace("/blob/main/", f"/blob/{lib_version}/")
         if lib_version.replace(".", "").isdigit()
         else source_link
     )
     return f'<a href="{href}" class="link-to-source" target="_blank">View source</a>'
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 70
+# %% ../nbs/096_Docusaurus_Helper.ipynb 71
 def _get_method_type(symbol: Type) -> str:
     try:
         source = getsource(symbol).strip()
     except TypeError as e:
         return ""
 
     first_line = source.split("\n")[0]
@@ -485,27 +488,27 @@
     link_to_source = f"{_get_symbol_source_link(symbol, lib_version)}\n\n"
 
     _signature = signature(symbol)
     parameters = _get_parameters(_signature)
     symbol_definition = f"```py\n{_get_method_type(symbol)}{_format_symbol_definition(symbol, parameters)}```\n"
     return symbol_anchor + link_to_source + symbol_definition
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 76
+# %% ../nbs/096_Docusaurus_Helper.ipynb 77
 def _is_method(symbol: Type) -> bool:
     """Check if the given symbol is a method.
 
     Args:
         symbol: A function or method object to check.
 
     Returns:
         A boolean indicating whether the symbol is a method.
     """
     return ismethod(symbol) or isfunction(symbol) or isinstance(symbol, property)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 78
+# %% ../nbs/096_Docusaurus_Helper.ipynb 79
 def _get_formatted_docstring_for_symbol(
     symbol: Type, lib_version: str, header_level: int = 2
 ) -> str:
     """Recursively parses and get formatted docstring of a symbol.
 
     Args:
         symbol: A Python class or function object to parse the docstring for.
@@ -530,31 +533,27 @@
 
         Returns:
             The updated formatted docstrings.
 
         """
         for x, y in getmembers(symbol):
             if not x.startswith("_") or x == "__init__":
-                if _is_method(y) and y.__doc__ is not None:
+                if _is_method(y):
                     contents += f"{_get_symbol_definition(y, header_level, lib_version)}\n{_docstring_to_markdown(y)}"
-                elif isclass(y) and y.__doc__ is not None and not x.startswith("_"):
+                elif isclass(y) and not x.startswith("_"):
                     contents += f"{_get_symbol_definition(y, header_level+1, lib_version)}\n{_docstring_to_markdown(y)}"
                     contents = traverse(y, contents, header_level + 1, lib_version)
         return contents
 
-    contents = (
-        f"{_get_symbol_definition(symbol, header_level+1, lib_version)}\n{_docstring_to_markdown(symbol)}"
-        if symbol.__doc__ is not None
-        else ""
-    )
+    contents = f"{_get_symbol_definition(symbol, header_level+1, lib_version)}\n{_docstring_to_markdown(symbol)}"
     if isclass(symbol):
         contents = traverse(symbol, contents, header_level + 1, lib_version)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 81
+# %% ../nbs/096_Docusaurus_Helper.ipynb 84
 def _convert_html_style_attribute_to_jsx(contents: str) -> str:
     """Converts the inline style attributes in an HTML string to JSX compatible format.
 
     Args:
         contents: A string containing an HTML document or fragment.
 
     Returns:
@@ -578,46 +577,46 @@
         for key, value in style_dict.items():
             replacement += f"{key}: '{value}', "
         replacement = replacement[:-2] + "}}"
         contents = contents.replace(f'style="{style_match}"', replacement)
 
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 83
+# %% ../nbs/096_Docusaurus_Helper.ipynb 86
 def _get_all_markdown_files_path(docs_path: Path) -> List[Path]:
     """Get all Markdown files in a directory and its subdirectories.
 
     Args:
         directory: The path to the directory to search in.
 
     Returns:
         A list of paths to all Markdown files found in the directory and its subdirectories.
     """
     markdown_files = [file_path for file_path in docs_path.glob("**/*.md")]
     return markdown_files
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 85
+# %% ../nbs/096_Docusaurus_Helper.ipynb 88
 def _fix_special_symbols_in_html(contents: str) -> str:
     contents = contents.replace("”", '"')
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 87
+# %% ../nbs/096_Docusaurus_Helper.ipynb 90
 def _add_file_extension_to_link(url: str) -> str:
     """Add file extension to the last segment of a URL
 
     Args:
         url: A URL string.
 
     Returns:
         A string of the updated URL with a file extension added to the last segment of the URL.
     """
     segments = url.split("/#")[0].split("/")[-2:]
     return url.replace(f"/{segments[1]}", f"/{segments[1]}.md").replace(".md/#", ".md#")
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 91
+# %% ../nbs/096_Docusaurus_Helper.ipynb 94
 def _generate_production_url(url: str) -> str:
     """Generate a Docusaurus compatible production URL for the given symbol URL.
 
     Args:
         url: The symbol URL to be converted.
 
     Returns:
@@ -625,15 +624,15 @@
     """
     url_segment, hash_segment = url.split(".md")
     url_split = url_segment.split("/")
     if url_split[-1].lower() == url_split[-2].lower():
         return "/".join(url_split[:-1]) + hash_segment
     return url.replace(".md", "")
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 93
+# %% ../nbs/096_Docusaurus_Helper.ipynb 96
 def _fix_symbol_links(
     contents: str,
     dir_prefix: str,
     doc_host: str,
     doc_baseurl: str,
     use_relative_doc_links: bool = True,
 ) -> str:
@@ -662,15 +661,15 @@
         else:
             updated_url = _generate_production_url(
                 doc_host + doc_baseurl + "/docs/" + new_url.split("/docs/")[1]
             )
         contents = contents.replace(old_url, updated_url)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 101
+# %% ../nbs/096_Docusaurus_Helper.ipynb 104
 def _get_relative_url_prefix(docs_path: Path, sub_path: Path) -> str:
     """Returns a relative url prefix from a sub path to a docs path.
 
     Args:
         docs_path (Path): The docs directory path.
         sub_path (Path): The sub directory path.
 
@@ -685,15 +684,15 @@
     except ValueError:
         raise ValueError(f"{sub_path} is not a descendant of {docs_path}")
 
     return (
         "../" * (len(relative_path.parts) - 1) if len(relative_path.parts) > 1 else ""
     )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 103
+# %% ../nbs/096_Docusaurus_Helper.ipynb 106
 def fix_invalid_syntax_in_markdown(docs_path: str) -> None:
     """Fix invalid HTML syntax in markdown files and converts inline style attributes to JSX-compatible format.
 
     Args:
         docs_path: The path to the root directory to search for markdown files.
     """
     cfg = get_config()
@@ -708,15 +707,15 @@
         contents = _convert_html_style_attribute_to_jsx(contents)
         contents = _fix_special_symbols_in_html(contents)
         contents = _fix_symbol_links(
             contents, relative_url_prefix, doc_host, doc_baseurl
         )
         file.write_text(contents)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 105
+# %% ../nbs/096_Docusaurus_Helper.ipynb 108
 def generate_markdown_docs(module_name: str, docs_path: str) -> None:
     """Generates Markdown documentation files for the symbols in the given module and save them to the given directory.
 
     Args:
         module_name: The name of the module to generate documentation for.
         docs_path: The path to the directory where the documentation files will be saved.
     """
@@ -728,15 +727,15 @@
         content = _get_formatted_docstring_for_symbol(symbol, lib_version)
         target_file_path = (
             "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
         )
         with open((Path(docs_path) / "api" / target_file_path), "w") as f:
             f.write(content)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 108
+# %% ../nbs/096_Docusaurus_Helper.ipynb 111
 def _parse_lines(lines: List[str]) -> Tuple[List[str], int]:
     """Parse a list of lines and return a tuple containing a list of filenames and an index indicating how many lines to skip.
 
     Args:
         lines: A list of strings representing lines of input text.
 
     Returns:
@@ -745,15 +744,15 @@
     """
     index = next(
         (i for i, line in enumerate(lines) if not line.strip().startswith("- [")),
         len(lines),
     )
     return [line.split("(")[1][:-4] for line in lines[:index]], index
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 111
+# %% ../nbs/096_Docusaurus_Helper.ipynb 114
 def _parse_section(text: str, ignore_first_line: bool = False) -> List[Any]:
     """Parse the given section contents and return a list of file names in the expected format.
 
     Args:
         text: A string representing the contents of a file.
         ignore_first_line: Flag indicating whether to ignore the first line extracting the section contents.
 
@@ -774,15 +773,15 @@
             value, skip_lines = _parse_lines(lines[index + 1 :])
             ret_val.append({line.replace("-", "").strip(): value})
             index += skip_lines + 1
         else:
             index += 1
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 114
+# %% ../nbs/096_Docusaurus_Helper.ipynb 117
 def _get_section_from_markdown(
     markdown_text: str, section_header: str
 ) -> Optional[str]:
     """Get the contents of the section header from the given markdown text
 
     Args:
         markdown_text: A string containing the markdown text to extract the section from.
@@ -792,15 +791,15 @@
         A string representing the contents of the section header if the section header
         is present in the markdown text, else None
     """
     pattern = re.compile(rf"^- {section_header}\n((?:\s+- .*\n)+)", re.M)
     match = pattern.search(markdown_text)
     return match.group(1) if match else None
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 119
+# %% ../nbs/096_Docusaurus_Helper.ipynb 122
 def generate_sidebar(
     summary_file: str = "./docusaurus/docs/SUMMARY.md",
     summary: str = "",
     target: str = "./docusaurus/sidebars.js",
 ) -> None:
     """
     Generate a sidebar js file for a Docusaurus documentation site based on a SUMMARY.md file.
@@ -848,15 +847,15 @@
     "LICENSE",
     "CONTRIBUTING",
     "CHANGELOG",
 ],
 };"""
         )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 121
+# %% ../nbs/096_Docusaurus_Helper.ipynb 124
 def _get_markdown_filenames_from_sidebar(sidebar_file_path: str) -> List[str]:
     """Get a list of Markdown filenames included in the sidebar.
 
     Args:
         sidebar_file_path: The path to the sidebar file.
 
     Returns:
@@ -869,15 +868,15 @@
         match = re.search(pattern, file_content, re.DOTALL)
         all_sidebar_files = ast.literal_eval(match.group(1)) if match else []
         markdown_filenames = [
             f"{v}.md" for v in all_sidebar_files if isinstance(v, str)
         ]
         return markdown_filenames
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 123
+# %% ../nbs/096_Docusaurus_Helper.ipynb 126
 def _delete_files(files: List[Path]) -> None:
     """Deletes a list of files.
 
     Args:
         files: A list of Path objects representing the files to be deleted.
 
     Raises:
@@ -888,15 +887,15 @@
         try:
             file.unlink()
         except OSError as e:
             typer.echo(
                 f"Error deleting files from docusaurus/docs directory. Could not delete file: {file} - {e}"
             )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 126
+# %% ../nbs/096_Docusaurus_Helper.ipynb 129
 def delete_unused_markdown_files_from_sidebar(
     docs_path: str, sidebar_file_path: str
 ) -> None:
     """Delete the markdown files from the docs directory that are not present in the sidebar.
 
     Args:
         docs_path: Path to the directory containing the markdown files.
@@ -911,15 +910,15 @@
         ]
         md_files_in_sidebar = [Path(docs_path) / f for f in md_filenames_in_sidebar]
         md_files_to_delete = list(
             set(all_md_files_in_docs_dir) - set(md_files_in_sidebar)
         )
         _delete_files(md_files_to_delete)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 128
+# %% ../nbs/096_Docusaurus_Helper.ipynb 131
 def update_readme() -> None:
     """Update the readme file and fix the symbol links"""
     cfg = get_config()
     readme_path = cfg.config_path / "README.md"
     nbdev_readme.__wrapped__()
 
     with open(readme_path, "r", encoding="utf-8") as f:
```

### Comparing `fastkafka-0.8.0rc1/fastkafka/_helpers.py` & `fastkafka-0.8.1rc0/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_modidx.py` & `fastkafka-0.8.1rc0/fastkafka/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_server.py` & `fastkafka-0.8.1rc0/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.8.1rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.8.1rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.8.1rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/_testing/test_utils.py` & `fastkafka-0.8.1rc0/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/encoder.py` & `fastkafka-0.8.1rc0/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka/testing.py` & `fastkafka-0.8.1rc0/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.8.1rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.8.0rc1
+Version: 0.8.1rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.8.0rc1/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.8.1rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/fastkafka.egg-info/requires.txt` & `fastkafka-0.8.1rc0/fastkafka.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc1/settings.ini` & `fastkafka-0.8.1rc0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.8.0rc1
+version = 0.8.1rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.8.0rc1/setup.py` & `fastkafka-0.8.1rc0/setup.py`

 * *Files identical despite different names*

