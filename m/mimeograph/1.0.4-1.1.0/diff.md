# Comparing `tmp/mimeograph-1.0.4.tar.gz` & `tmp/mimeograph-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-1.0.4.tar", last modified: Tue Jun 27 07:06:54 2023, max compression
+gzip compressed data, was "mimeograph-1.1.0.tar", last modified: Mon Jul 10 14:08:44 2023, max compression
```

## Comparing `mimeograph-1.0.4.tar` & `mimeograph-1.1.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.614524 mimeograph-1.0.4/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-1.0.4/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-1.0.4/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-27 07:06:54.610523 mimeograph-1.0.4/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    32079 2023-06-26 13:54:19.000000 mimeograph-1.0.4/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     4010 2023-06-27 07:06:22.000000 mimeograph-1.0.4/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-06-27 07:06:54.614524 mimeograph-1.0.4/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1484 2023-06-27 07:06:22.000000 mimeograph-1.0.4/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-06-24 11:03:12.000000 mimeograph-1.0.4/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-1.0.4/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4694 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18152 2023-06-27 07:06:22.000000 mimeograph-1.0.4/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-1.0.4/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6275 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/constants.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12351 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    35693 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-06-24 11:02:10.000000 mimeograph-1.0.4/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2374 2023-06-24 11:02:23.000000 mimeograph-1.0.4/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3109 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-1.0.4/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18276 2023-06-23 11:30:49.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5164 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2911 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.606523 mimeograph-1.0.4/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-1.0.4/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5638 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5885 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5755 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/currencies.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-1.0.4/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5599 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2235 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10234 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      702 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/exc.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1149 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/generators/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10680 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1852 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17137 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/json_generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    14857 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-1.0.4/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-1.0.4/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4083 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    10889 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541630 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     1579 2023-06-20 06:50:14.000000 mimeograph-1.0.4/src/mimeo/resources/constants.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-06-27 06:51:54.000000 mimeograph-1.0.4/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     7267 2023-06-27 07:03:27.000000 mimeograph-1.0.4/src/mimeo/resources/currencies.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-06-27 06:51:59.000000 mimeograph-1.0.4/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      736 2023-06-26 13:54:19.000000 mimeograph-1.0.4/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-06-27 06:52:05.000000 mimeograph-1.0.4/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-1.0.4/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-1.0.4/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6254 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    29523 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20193 2023-06-23 07:36:58.000000 mimeograph-1.0.4/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    34465 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     2043 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-06-27 07:06:54.000000 mimeograph-1.0.4/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-06-27 07:06:54.610523 mimeograph-1.0.4/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    16690 2023-06-26 13:54:19.000000 mimeograph-1.0.4/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-1.0.4/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.124725 mimeograph-1.1.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-1.1.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-1.1.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    36394 2023-07-10 14:08:44.124725 mimeograph-1.1.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34008 2023-07-10 14:05:22.000000 mimeograph-1.1.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4025 2023-07-10 14:08:17.000000 mimeograph-1.1.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-07-10 14:08:44.124725 mimeograph-1.1.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.116725 mimeograph-1.1.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.116725 mimeograph-1.1.0/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1484 2023-07-10 14:08:17.000000 mimeograph-1.1.0/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-06-24 11:03:12.000000 mimeograph-1.1.0/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.116725 mimeograph-1.1.0/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2290 2023-05-17 08:57:29.000000 mimeograph-1.1.0/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4694 2023-06-26 13:54:19.000000 mimeograph-1.1.0/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18152 2023-07-10 14:08:17.000000 mimeograph-1.1.0/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.116725 mimeograph-1.1.0/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      837 2023-05-27 06:14:50.000000 mimeograph-1.1.0/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8041 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/config/constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    15227 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    38165 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-06-24 11:02:10.000000 mimeograph-1.1.0/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2374 2023-06-24 11:02:23.000000 mimeograph-1.1.0/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3109 2023-06-26 13:54:19.000000 mimeograph-1.1.0/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-1.1.0/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8108 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18276 2023-06-23 11:30:49.000000 mimeograph-1.1.0/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8724 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2911 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1805 2023-05-16 10:04:29.000000 mimeograph-1.1.0/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5638 2023-06-27 07:03:27.000000 mimeograph-1.1.0/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5885 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5755 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/database/currencies.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6200 2023-05-22 07:52:53.000000 mimeograph-1.1.0/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5599 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2235 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    10234 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      702 2023-06-26 13:54:19.000000 mimeograph-1.1.0/src/mimeo/exc.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1221 2023-06-20 06:50:14.000000 mimeograph-1.1.0/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1149 2023-06-20 06:50:14.000000 mimeograph-1.1.0/src/mimeo/generators/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11298 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1852 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16412 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/generators/json_generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    14624 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-16 15:27:55.000000 mimeograph-1.1.0/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.120725 mimeograph-1.1.0/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-1.1.0/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4083 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      656 2023-05-17 13:09:43.000000 mimeograph-1.1.0/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    11505 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.124725 mimeograph-1.1.0/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      362 2023-05-17 13:09:43.000000 mimeograph-1.1.0/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541630 2023-06-27 07:03:27.000000 mimeograph-1.1.0/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/resources/constants.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-06-27 06:51:54.000000 mimeograph-1.1.0/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7267 2023-06-27 07:03:27.000000 mimeograph-1.1.0/src/mimeo/resources/currencies.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      783 2023-05-17 13:09:43.000000 mimeograph-1.1.0/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-06-27 06:51:59.000000 mimeograph-1.1.0/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      736 2023-06-26 13:54:19.000000 mimeograph-1.1.0/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-06-27 06:52:05.000000 mimeograph-1.1.0/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2023-05-17 13:09:43.000000 mimeograph-1.1.0/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.124725 mimeograph-1.1.0/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2193 2023-05-16 10:04:29.000000 mimeograph-1.1.0/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6254 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29523 2023-06-23 07:36:58.000000 mimeograph-1.1.0/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23211 2023-07-10 14:05:22.000000 mimeograph-1.1.0/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.124725 mimeograph-1.1.0/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    36394 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2043 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      222 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-07-10 14:08:44.000000 mimeograph-1.1.0/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-10 14:08:44.124725 mimeograph-1.1.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16690 2023-06-26 13:54:19.000000 mimeograph-1.1.0/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      502 2023-05-22 07:52:53.000000 mimeograph-1.1.0/tests/test_tools.py
```

### Comparing `mimeograph-1.0.4/LICENSE` & `mimeograph-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/PKG-INFO` & `mimeograph-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 1.0.4
+Version: 1.1.0
 Summary: Generate NoSQL data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,16 @@
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
 [![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and a python library generating NoSQL data based on a template.
-It can be used by developers, testers or business analysts in their daily work.
+It can be used by developers, testers or business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data).
 
 
 ## Installation
 
 Install Mimeo with pip
 
 ```sh
@@ -294,35 +295,36 @@
 |:------------:|:-----------------|:------------------------------------------------|
 |              | `--sequentially` | process Mimeo Configurations in a single thread |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                      |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:-------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output/format`          |  Config  |        :x:         |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
-| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `vars`                   |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `_templates_`            |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                  | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                  | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                      |  Level   |  Required   |     Supported values     |    Default     | Description                                                                                                                                             |
+|:-------------------------|:--------:|:-----------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output`                 |  Config  | **&#9744;** |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  | **&#9744;** | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  | **&#9744;** |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  | **&#9744;** |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  | **&#9744;** |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  | **&#9744;** |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  | **&#9744;** |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  | **&#9744;** |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/username`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                   |  Config  | **&#9744;** |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more below)                                                                                      |
+| `refs`                   |  Config  | **&#9744;** |          object          |      ---       | Defines references to be used in a Mimeo Template (read more below)                                                                                     |
+| `_templates_`            |  Config  | **&#9745;** |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                  | Template | **&#9745;** |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                  | Template | **&#9745;** |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                |  Model   | **&#9744;** |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
@@ -405,15 +407,16 @@
   ]
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
-Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
+Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_)
+in context of a single iteration.
 To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
 let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
@@ -428,14 +431,79 @@
         }
       }
     }
   ]
 }
 ```
 
+#### Mimeo Refs
+
+Mimeo Special Fields are useful when an entity has the same value used in several fields.
+However, usually entities are related with each other. To use references between entities, you can use
+Mimeo Refs. They are configured at the highest Mimeo Configuration level and require 3 settings:
+- context - a context from which values will be cached
+- field - a source field of the reference 
+- type
+  - `any` - reference of this type will be used randomly
+    - no order
+    - possible duplicates (One-To-Many, Many-To-Many)
+  - `parallel` - reference of this type will generate a reference from the same iteration in references entity
+    - same order as in parent entity
+    - unique values (One-To-One)
+
+To use them in a Mimeo Template, simply wrap a reference name with curly braces [`{some-reference}`].
+
+> Note:
+>  - A reference can't be configured using any of Mimeo Utils' names nor existing Mimeo Vars
+>  - A referenced entity needs to be placed before a referencing one
+
+Example
+```json
+{
+  "refs": {
+    "parent-one-to-many": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "any"
+    },
+    "parent-one-to-one": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "parallel"
+    }
+  },
+  "_templates_": [
+    {
+      "count": 5,
+      "model": {
+        "SomeEntity": {
+          "ID": "{key}"
+        }
+      }
+    },
+    {
+      "count": 5,
+      "model": {
+        "OneToOneChildEntity": {
+          "Parent": "{parent-one-to-one}"
+        }
+      }
+    },
+    {
+      "count": 10,
+      "model": {
+        "ManyToOneChildEntity": {
+          "Parent": "{parent-one-to-many}"
+        }
+      }
+    }
+  ]
+}
+```
+
 #### Mimeo Utils
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mimeograph Version: 1.0.4 Summary: Generate NoSQL
+Metadata-Version: 2.1 Name: mimeograph Version: 1.1.0 Summary: Generate NoSQL
 data based on a simple template Author-email: "T.A. Programming Svcs."
 maciej.aniolowski@gmail.com> License: MIT License Copyright (c) 2023 Tomasz
 AnioÅowski Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -39,17 +39,18 @@
 github.com/TomaszAniolowski/mimeo/actions/workflows/
 test.yml?query=branch%3Amain) [![Code Coverage](https://img.shields.io/badge/
 Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/
 TomaszAniolowski/mimeo/actions/workflows/
 coverage_badge.yml?query=branch%3Amain) [Mimeo](https://github.com/
 TomaszAniolowski/mimeo) is a command line tool and a python library generating
 NoSQL data based on a template. It can be used by developers, testers or
-business analysts in their daily work. ## Installation Install Mimeo with pip
-```sh pip install mimeograph ``` ## Usage/Examples ### Mimeo Configuration
-Prepare Mimeo Configuration first
+business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data). ##
+Installation Install Mimeo with pip ```sh pip install mimeograph ``` ## Usage/
+Examples ### Mimeo Configuration Prepare Mimeo Configuration first
 JSON                                     XML
 ```json { "_templates_": [ { "count":    ```xml  <_templates_> <_template_> 30
 30, "model": { "SomeEntity": { "@xmlns": 1 value-2 true      ```
 "http://mimeo.arch.com/default-
 namespace", "@xmlns:pn": "http://
 mimeo.arch.com/prefixed-namespace",
 "ChildNode1": 1, "ChildNode2": "value-
@@ -98,97 +99,116 @@
 ---------------| | | `--silent` | disable INFO logs | | | `--debug` | enable
 DEBUG mode | | | `--fine` | enable FINE mode | #### Other arguments | Short
 option | Long option | Description | |:------------:|:-----------------|:------
 ------------------------------------------| | | `--sequentially` | process
 Mimeo Configurations in a single thread | ### Mimeo Configuration Mimeo
 configuration is defined in a JSON file using internal settings and data
 templates. | Key | Level | Required | Supported values | Default | Description
-| |:-------------------------|:--------:|:------------------:|:----------------
---------:|:--------------:|----------------------------------------------------
+| |:-------------------------|:--------:|:-----------:|:-----------------------
+-:|:--------------:|-----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | `output` | Config | :x: | object | --- | Defines
-output details on how it will be consumed | | `output/direction` | Config | :x:
-| `file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
-`output/format` | Config | :x: | `xml`, `json` | `xml` | Defines output data
-format | | `output/indent` | Config | :x: | integer | `null` | Defines indent
-applied in output data | | `output/xml_declaration` | Config | :x: | boolean |
-`false` | Indicates whether an xml declaration should be added to output data |
-| `output/directory_path` | Config | :x: | string | `mimeo-output` | For `file`
-direction - defines an output directory | | `output/file_name` | Config | :x: |
-string | `mimeo-output` | For `file` direction - defines an output file name |
-| `output/method` | Config | :x: | `POST`, `PUT` | `POST` | For `http`
-direction - defines a request method | | `output/protocol` | Config | :x: |
-`http`, `https` | `http` | For `http` direction - defines a url protocol | |
-`output/host` | Config | :heavy_check_mark: | string | --- | For `http`
-direction - defines a url host | | `output/port` | Config | :x: | integer |
+---------------| | `output` | Config | **☐** | object | --- | Defines output
+details on how it will be consumed | | `output/direction` | Config | **☐** |
+`file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
+`output/format` | Config | **☐** | `xml`, `json` | `xml` | Defines output data
+format | | `output/indent` | Config | **☐** | integer | `null` | Defines indent
+applied in output data | | `output/xml_declaration` | Config | **☐** | boolean
+| `false` | Indicates whether an xml declaration should be added to output data
+| | `output/directory_path` | Config | **☐** | string | `mimeo-output` | For
+`file` direction - defines an output directory | | `output/file_name` | Config
+| **☐** | string | `mimeo-output` | For `file` direction - defines an output
+file name | | `output/method` | Config | **☐** | `POST`, `PUT` | `POST` | For
+`http` direction - defines a request method | | `output/protocol` | Config |
+**☐** | `http`, `https` | `http` | For `http` direction - defines a url
+protocol | | `output/host` | Config | **☑** | string | --- | For `http`
+direction - defines a url host | | `output/port` | Config | **☐** | integer |
 `null` | For `http` direction - defines a url port (can be empty) | | `output/
-endpoint` | Config | :heavy_check_mark: | string | --- | For `http` direction -
-defines a url endpoint | | `output/username` | Config | :heavy_check_mark: |
-string | --- | For `http` direction - defines a username | | `output/password`
-| Config | :heavy_check_mark: | string | --- | For `http` direction - defines a
-password | | `vars` | Config | :x: | object | --- | Defines variables to be
-used in a Mimeo Template (read more in next section) | | `_templates_` | Config
-| :heavy_check_mark: | array | --- | Stores templates for data generation | |
-`count` | Template | :heavy_check_mark: | integer | --- | Indicates number of
-copies | | `model` | Template | :heavy_check_mark: | object | --- | Defines
-data template to be copied | | `context` | Model | :x: | object | --- | Defines
-a context name that is internally used e.g. using `curr_iter()` and `get_key()`
-mimeo utils (by default model name is used as the context name) | #### Mimeo
-Environment To make `http` output directory easier to use, mimeo allows you to
-configure Mimeo Environments. They are configured in a JSON file (by default:
-mimeo.envs.json) and support the following output details: - `protocol` -
-`host` - `port` - `username` - `password` Example ```json { "local": { "host":
-"localhost", "port": 8000, "username": "admin", "password": "admin" }, "dev":
-{ "protocol": "https", "host": "11.111.11.111", "port": 8000, "username":
-"some-user", "password": "some-password" } } ``` To use a specific Mimeo
-Environment you can use the following commands: ```sh mimeo SomeEntity-
-config.json -e dev mimeo SomeEntity-config.json -e dev --http-envs-file
-environments.json ``` #### Mimeo Vars Mimeo allows you to define a list of
-variables. You can use them in your Mimeo Config by wrapping them in curly
-brackets [`{VARIABLE}`]. There are only 2 rules for variable names: - Variable
-name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \
-{`0-9`\} only - Variable name must start with a letter Variable can be defined
-with: - any atomic value - any other variable defined - any Mimeo Util You can
-use Mimeo Vars as partial values (unless they are defined as Mimeo Utils).
-Example: ```json { "vars": { "CUSTOM_VAR_1": "custom-value-1", "CUSTOM_VAR_2":
-1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "
-{auto_increment}", "CUSTOM_VAR_6": { "_mimeo_util": { "_name": "random_int",
-"limit": 99 } } }, "_templates_": [ { "count": 5, "model": { "SomeEntity":
-{ "ChildNode1": "{CUSTOM_VAR_1}", "ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3":
-"{CUSTOM_VAR_3}", "ChildNode4": "{CUSTOM_VAR_4}", "ChildNode5": "
-{CUSTOM_VAR_5}", "ChildNode6": "{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-
-with-suffix" } } } ] } ``` #### Mimeo Special Fields In Mimeo Template you can
-use so-called _special fields_. Every field in a template can be stored in
-memory (_provided_) and used later as a value of other fields (_injected_). To
+endpoint` | Config | **☑** | string | --- | For `http` direction - defines a
+url endpoint | | `output/username` | Config | **☑** | string | --- | For `http`
+direction - defines a username | | `output/password` | Config | **☑** | string
+| --- | For `http` direction - defines a password | | `vars` | Config | **☐** |
+object | --- | Defines variables to be used in a Mimeo Template (read more
+below) | | `refs` | Config | **☐** | object | --- | Defines references to be
+used in a Mimeo Template (read more below) | | `_templates_` | Config | **☑** |
+array | --- | Stores templates for data generation | | `count` | Template |
+**☑** | integer | --- | Indicates number of copies | | `model` | Template |
+**☑** | object | --- | Defines data template to be copied | | `context` | Model
+| **☐** | object | --- | Defines a context name that is internally used e.g.
+using `curr_iter()` and `get_key()` mimeo utils (by default model name is used
+as the context name) | #### Mimeo Environment To make `http` output directory
+easier to use, mimeo allows you to configure Mimeo Environments. They are
+configured in a JSON file (by default: mimeo.envs.json) and support the
+following output details: - `protocol` - `host` - `port` - `username` -
+`password` Example ```json { "local": { "host": "localhost", "port": 8000,
+"username": "admin", "password": "admin" }, "dev": { "protocol": "https",
+"host": "11.111.11.111", "port": 8000, "username": "some-user", "password":
+"some-password" } } ``` To use a specific Mimeo Environment you can use the
+following commands: ```sh mimeo SomeEntity-config.json -e dev mimeo SomeEntity-
+config.json -e dev --http-envs-file environments.json ``` #### Mimeo Vars Mimeo
+allows you to define a list of variables. You can use them in your Mimeo Config
+by wrapping them in curly brackets [`{VARIABLE}`]. There are only 2 rules for
+variable names: - Variable name can include upper-cased letters \[`A-Z`\],
+underscore \[`_`\] and digits \{`0-9`\} only - Variable name must start with a
+letter Variable can be defined with: - any atomic value - any other variable
+defined - any Mimeo Util You can use Mimeo Vars as partial values (unless they
+are defined as Mimeo Utils). Example: ```json { "vars": { "CUSTOM_VAR_1":
+"custom-value-1", "CUSTOM_VAR_2": 1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "
+{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "{auto_increment}", "CUSTOM_VAR_6":
+{ "_mimeo_util": { "_name": "random_int", "limit": 99 } } }, "_templates_": [
+{ "count": 5, "model": { "SomeEntity": { "ChildNode1": "{CUSTOM_VAR_1}",
+"ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3": "{CUSTOM_VAR_3}", "ChildNode4": "
+{CUSTOM_VAR_4}", "ChildNode5": "{CUSTOM_VAR_5}", "ChildNode6": "
+{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-with-suffix" } } } ] } ``` ####
+Mimeo Special Fields In Mimeo Template you can use so-called _special fields_.
+Every field in a template can be stored in memory (_provided_) and used later
+as a value of other fields (_injected_) in context of a single iteration. To
 provide a special field, wrap its name with colons: [`:SomeField:`]. To inject,
 use additionally curly braces to let interpreter know it should be rendered [`
 {:SomeField:}`]. They can be injected as partial values, similarly to Mimeo
 Vars. Example ```json { "_templates_": [ { "count": 5, "model": { "SomeEntity":
 { ":ChildNode1:": "custom-value", "ChildNode2": "{:ChildNode1:}", "ChildNode3":
-"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Utils You can use several
-predefined functions to generate data. They can be used in a _raw_ format or
-_parametrized_. ##### Random String Generates a random string value. |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | length | `int` | `20` | ###### Raw Uses the default length: 20
-characters. ```json { "randomstring": "{random_str}" } ``` ###### Parametrized
-Uses the customized length. ```json { "randomstring": { "_mimeo_util":
-{ "_name": "random_str", "length": 5 } } } ``` ##### Random Integer Generates a
-random integer value between `start` and `limit` parameters (inclusive). |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | start | `int` | `1` | | limit | `int` | `100` | ###### Raw Uses the
-default start (1) and limit (100) values. ```json { "randominteger": "
-{random_int}" } ``` ###### Parametrized Uses the customized limit. ```json
-{ "randominteger1": { "_mimeo_util": { "_name": "random_int", "start": 0 } },
-"randominteger2": { "_mimeo_util": { "_name": "random_int", "limit": 5 } },
-"randominteger3": { "_mimeo_util": { "_name": "random_int", "start": 0,
-"limit": 5 } } } ``` ##### Random Item Generates a random value from items
-provided. NOTICE: The raw form of this Mimeo Util will generate a blank string
-value (as same as no items parametrized). | Parameter | Supported values |
-Default | |:---------:|:----------------:|:-------:| | items | `list` | `[""]`
-| ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
+"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Refs Mimeo Special Fields
+are useful when an entity has the same value used in several fields. However,
+usually entities are related with each other. To use references between
+entities, you can use Mimeo Refs. They are configured at the highest Mimeo
+Configuration level and require 3 settings: - context - a context from which
+values will be cached - field - a source field of the reference - type - `any`
+- reference of this type will be used randomly - no order - possible duplicates
+(One-To-Many, Many-To-Many) - `parallel` - reference of this type will generate
+a reference from the same iteration in references entity - same order as in
+parent entity - unique values (One-To-One) To use them in a Mimeo Template,
+simply wrap a reference name with curly braces [`{some-reference}`]. > Note: >
+- A reference can't be configured using any of Mimeo Utils' names nor existing
+Mimeo Vars > - A referenced entity needs to be placed before a referencing one
+Example ```json { "refs": { "parent-one-to-many": { "context": "SomeEntity",
+"field": "ID", "type": "any" }, "parent-one-to-one": { "context": "SomeEntity",
+"field": "ID", "type": "parallel" } }, "_templates_": [ { "count": 5, "model":
+{ "SomeEntity": { "ID": "{key}" } } }, { "count": 5, "model":
+{ "OneToOneChildEntity": { "Parent": "{parent-one-to-one}" } } }, { "count":
+10, "model": { "ManyToOneChildEntity": { "Parent": "{parent-one-to-many}" } } }
+] } ``` #### Mimeo Utils You can use several predefined functions to generate
+data. They can be used in a _raw_ format or _parametrized_. ##### Random String
+Generates a random string value. | Parameter | Supported values | Default | |:-
+--------:|:----------------:|:-------:| | length | `int` | `20` | ###### Raw
+Uses the default length: 20 characters. ```json { "randomstring": "
+{random_str}" } ``` ###### Parametrized Uses the customized length. ```json
+{ "randomstring": { "_mimeo_util": { "_name": "random_str", "length": 5 } } }
+``` ##### Random Integer Generates a random integer value between `start` and
+`limit` parameters (inclusive). | Parameter | Supported values | Default | |:--
+-------:|:----------------:|:-------:| | start | `int` | `1` | | limit | `int`
+| `100` | ###### Raw Uses the default start (1) and limit (100) values. ```json
+{ "randominteger": "{random_int}" } ``` ###### Parametrized Uses the customized
+limit. ```json { "randominteger1": { "_mimeo_util": { "_name": "random_int",
+"start": 0 } }, "randominteger2": { "_mimeo_util": { "_name": "random_int",
+"limit": 5 } }, "randominteger3": { "_mimeo_util": { "_name": "random_int",
+"start": 0, "limit": 5 } } } ``` ##### Random Item Generates a random value
+from items provided. NOTICE: The raw form of this Mimeo Util will generate a
+blank string value (as same as no items parametrized). | Parameter | Supported
+values | Default | |:---------:|:----------------:|:-------:| | items | `list`
+| `[""]` | ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
 "random_item", "items": ["value", 1, true] } } } ``` ##### Date Generates a
 date value in format `YYYY-MM-DD`. | Parameter | Supported values | Default |
 |:----------:|:----------------:|:-------:| | days_delta | `int` | `0` | ######
 Raw Uses the today's date. ```json { "Today": "{date}" } ``` ######
 Parametrized Uses the customized days delta. ```json { "Yesterday":
 { "_mimeo_util": { "_name": "date", "days_delta": -1 } }, "Tomorrow":
 { "_mimeo_util": { "_name": "date", "days_delta": 1 } } } ``` ##### Date Time
```

### Comparing `mimeograph-1.0.4/README.md` & `mimeograph-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
 [![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and a python library generating NoSQL data based on a template.
-It can be used by developers, testers or business analysts in their daily work.
+It can be used by developers, testers or business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data).
 
 
 ## Installation
 
 Install Mimeo with pip
 
 ```sh
@@ -244,35 +245,36 @@
 |:------------:|:-----------------|:------------------------------------------------|
 |              | `--sequentially` | process Mimeo Configurations in a single thread |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                      |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:-------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output/format`          |  Config  |        :x:         |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
-| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `vars`                   |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `_templates_`            |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                  | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                  | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                      |  Level   |  Required   |     Supported values     |    Default     | Description                                                                                                                                             |
+|:-------------------------|:--------:|:-----------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output`                 |  Config  | **&#9744;** |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  | **&#9744;** | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  | **&#9744;** |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  | **&#9744;** |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  | **&#9744;** |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  | **&#9744;** |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  | **&#9744;** |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  | **&#9744;** |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/username`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                   |  Config  | **&#9744;** |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more below)                                                                                      |
+| `refs`                   |  Config  | **&#9744;** |          object          |      ---       | Defines references to be used in a Mimeo Template (read more below)                                                                                     |
+| `_templates_`            |  Config  | **&#9745;** |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                  | Template | **&#9745;** |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                  | Template | **&#9745;** |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                |  Model   | **&#9744;** |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
@@ -355,15 +357,16 @@
   ]
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
-Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
+Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_)
+in context of a single iteration.
 To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
 let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
@@ -378,14 +381,79 @@
         }
       }
     }
   ]
 }
 ```
 
+#### Mimeo Refs
+
+Mimeo Special Fields are useful when an entity has the same value used in several fields.
+However, usually entities are related with each other. To use references between entities, you can use
+Mimeo Refs. They are configured at the highest Mimeo Configuration level and require 3 settings:
+- context - a context from which values will be cached
+- field - a source field of the reference 
+- type
+  - `any` - reference of this type will be used randomly
+    - no order
+    - possible duplicates (One-To-Many, Many-To-Many)
+  - `parallel` - reference of this type will generate a reference from the same iteration in references entity
+    - same order as in parent entity
+    - unique values (One-To-One)
+
+To use them in a Mimeo Template, simply wrap a reference name with curly braces [`{some-reference}`].
+
+> Note:
+>  - A reference can't be configured using any of Mimeo Utils' names nor existing Mimeo Vars
+>  - A referenced entity needs to be placed before a referencing one
+
+Example
+```json
+{
+  "refs": {
+    "parent-one-to-many": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "any"
+    },
+    "parent-one-to-one": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "parallel"
+    }
+  },
+  "_templates_": [
+    {
+      "count": 5,
+      "model": {
+        "SomeEntity": {
+          "ID": "{key}"
+        }
+      }
+    },
+    {
+      "count": 5,
+      "model": {
+        "OneToOneChildEntity": {
+          "Parent": "{parent-one-to-one}"
+        }
+      }
+    },
+    {
+      "count": 10,
+      "model": {
+        "ManyToOneChildEntity": {
+          "Parent": "{parent-one-to-many}"
+        }
+      }
+    }
+  ]
+}
+```
+
 #### Mimeo Utils
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
```

#### html2text {}

```diff
@@ -9,17 +9,18 @@
 github.com/TomaszAniolowski/mimeo/actions/workflows/
 test.yml?query=branch%3Amain) [![Code Coverage](https://img.shields.io/badge/
 Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/
 TomaszAniolowski/mimeo/actions/workflows/
 coverage_badge.yml?query=branch%3Amain) [Mimeo](https://github.com/
 TomaszAniolowski/mimeo) is a command line tool and a python library generating
 NoSQL data based on a template. It can be used by developers, testers or
-business analysts in their daily work. ## Installation Install Mimeo with pip
-```sh pip install mimeograph ``` ## Usage/Examples ### Mimeo Configuration
-Prepare Mimeo Configuration first
+business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data). ##
+Installation Install Mimeo with pip ```sh pip install mimeograph ``` ## Usage/
+Examples ### Mimeo Configuration Prepare Mimeo Configuration first
 JSON                                     XML
 ```json { "_templates_": [ { "count":    ```xml  <_templates_> <_template_> 30
 30, "model": { "SomeEntity": { "@xmlns": 1 value-2 true      ```
 "http://mimeo.arch.com/default-
 namespace", "@xmlns:pn": "http://
 mimeo.arch.com/prefixed-namespace",
 "ChildNode1": 1, "ChildNode2": "value-
@@ -68,97 +69,116 @@
 ---------------| | | `--silent` | disable INFO logs | | | `--debug` | enable
 DEBUG mode | | | `--fine` | enable FINE mode | #### Other arguments | Short
 option | Long option | Description | |:------------:|:-----------------|:------
 ------------------------------------------| | | `--sequentially` | process
 Mimeo Configurations in a single thread | ### Mimeo Configuration Mimeo
 configuration is defined in a JSON file using internal settings and data
 templates. | Key | Level | Required | Supported values | Default | Description
-| |:-------------------------|:--------:|:------------------:|:----------------
---------:|:--------------:|----------------------------------------------------
+| |:-------------------------|:--------:|:-----------:|:-----------------------
+-:|:--------------:|-----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | `output` | Config | :x: | object | --- | Defines
-output details on how it will be consumed | | `output/direction` | Config | :x:
-| `file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
-`output/format` | Config | :x: | `xml`, `json` | `xml` | Defines output data
-format | | `output/indent` | Config | :x: | integer | `null` | Defines indent
-applied in output data | | `output/xml_declaration` | Config | :x: | boolean |
-`false` | Indicates whether an xml declaration should be added to output data |
-| `output/directory_path` | Config | :x: | string | `mimeo-output` | For `file`
-direction - defines an output directory | | `output/file_name` | Config | :x: |
-string | `mimeo-output` | For `file` direction - defines an output file name |
-| `output/method` | Config | :x: | `POST`, `PUT` | `POST` | For `http`
-direction - defines a request method | | `output/protocol` | Config | :x: |
-`http`, `https` | `http` | For `http` direction - defines a url protocol | |
-`output/host` | Config | :heavy_check_mark: | string | --- | For `http`
-direction - defines a url host | | `output/port` | Config | :x: | integer |
+---------------| | `output` | Config | **☐** | object | --- | Defines output
+details on how it will be consumed | | `output/direction` | Config | **☐** |
+`file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
+`output/format` | Config | **☐** | `xml`, `json` | `xml` | Defines output data
+format | | `output/indent` | Config | **☐** | integer | `null` | Defines indent
+applied in output data | | `output/xml_declaration` | Config | **☐** | boolean
+| `false` | Indicates whether an xml declaration should be added to output data
+| | `output/directory_path` | Config | **☐** | string | `mimeo-output` | For
+`file` direction - defines an output directory | | `output/file_name` | Config
+| **☐** | string | `mimeo-output` | For `file` direction - defines an output
+file name | | `output/method` | Config | **☐** | `POST`, `PUT` | `POST` | For
+`http` direction - defines a request method | | `output/protocol` | Config |
+**☐** | `http`, `https` | `http` | For `http` direction - defines a url
+protocol | | `output/host` | Config | **☑** | string | --- | For `http`
+direction - defines a url host | | `output/port` | Config | **☐** | integer |
 `null` | For `http` direction - defines a url port (can be empty) | | `output/
-endpoint` | Config | :heavy_check_mark: | string | --- | For `http` direction -
-defines a url endpoint | | `output/username` | Config | :heavy_check_mark: |
-string | --- | For `http` direction - defines a username | | `output/password`
-| Config | :heavy_check_mark: | string | --- | For `http` direction - defines a
-password | | `vars` | Config | :x: | object | --- | Defines variables to be
-used in a Mimeo Template (read more in next section) | | `_templates_` | Config
-| :heavy_check_mark: | array | --- | Stores templates for data generation | |
-`count` | Template | :heavy_check_mark: | integer | --- | Indicates number of
-copies | | `model` | Template | :heavy_check_mark: | object | --- | Defines
-data template to be copied | | `context` | Model | :x: | object | --- | Defines
-a context name that is internally used e.g. using `curr_iter()` and `get_key()`
-mimeo utils (by default model name is used as the context name) | #### Mimeo
-Environment To make `http` output directory easier to use, mimeo allows you to
-configure Mimeo Environments. They are configured in a JSON file (by default:
-mimeo.envs.json) and support the following output details: - `protocol` -
-`host` - `port` - `username` - `password` Example ```json { "local": { "host":
-"localhost", "port": 8000, "username": "admin", "password": "admin" }, "dev":
-{ "protocol": "https", "host": "11.111.11.111", "port": 8000, "username":
-"some-user", "password": "some-password" } } ``` To use a specific Mimeo
-Environment you can use the following commands: ```sh mimeo SomeEntity-
-config.json -e dev mimeo SomeEntity-config.json -e dev --http-envs-file
-environments.json ``` #### Mimeo Vars Mimeo allows you to define a list of
-variables. You can use them in your Mimeo Config by wrapping them in curly
-brackets [`{VARIABLE}`]. There are only 2 rules for variable names: - Variable
-name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \
-{`0-9`\} only - Variable name must start with a letter Variable can be defined
-with: - any atomic value - any other variable defined - any Mimeo Util You can
-use Mimeo Vars as partial values (unless they are defined as Mimeo Utils).
-Example: ```json { "vars": { "CUSTOM_VAR_1": "custom-value-1", "CUSTOM_VAR_2":
-1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "
-{auto_increment}", "CUSTOM_VAR_6": { "_mimeo_util": { "_name": "random_int",
-"limit": 99 } } }, "_templates_": [ { "count": 5, "model": { "SomeEntity":
-{ "ChildNode1": "{CUSTOM_VAR_1}", "ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3":
-"{CUSTOM_VAR_3}", "ChildNode4": "{CUSTOM_VAR_4}", "ChildNode5": "
-{CUSTOM_VAR_5}", "ChildNode6": "{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-
-with-suffix" } } } ] } ``` #### Mimeo Special Fields In Mimeo Template you can
-use so-called _special fields_. Every field in a template can be stored in
-memory (_provided_) and used later as a value of other fields (_injected_). To
+endpoint` | Config | **☑** | string | --- | For `http` direction - defines a
+url endpoint | | `output/username` | Config | **☑** | string | --- | For `http`
+direction - defines a username | | `output/password` | Config | **☑** | string
+| --- | For `http` direction - defines a password | | `vars` | Config | **☐** |
+object | --- | Defines variables to be used in a Mimeo Template (read more
+below) | | `refs` | Config | **☐** | object | --- | Defines references to be
+used in a Mimeo Template (read more below) | | `_templates_` | Config | **☑** |
+array | --- | Stores templates for data generation | | `count` | Template |
+**☑** | integer | --- | Indicates number of copies | | `model` | Template |
+**☑** | object | --- | Defines data template to be copied | | `context` | Model
+| **☐** | object | --- | Defines a context name that is internally used e.g.
+using `curr_iter()` and `get_key()` mimeo utils (by default model name is used
+as the context name) | #### Mimeo Environment To make `http` output directory
+easier to use, mimeo allows you to configure Mimeo Environments. They are
+configured in a JSON file (by default: mimeo.envs.json) and support the
+following output details: - `protocol` - `host` - `port` - `username` -
+`password` Example ```json { "local": { "host": "localhost", "port": 8000,
+"username": "admin", "password": "admin" }, "dev": { "protocol": "https",
+"host": "11.111.11.111", "port": 8000, "username": "some-user", "password":
+"some-password" } } ``` To use a specific Mimeo Environment you can use the
+following commands: ```sh mimeo SomeEntity-config.json -e dev mimeo SomeEntity-
+config.json -e dev --http-envs-file environments.json ``` #### Mimeo Vars Mimeo
+allows you to define a list of variables. You can use them in your Mimeo Config
+by wrapping them in curly brackets [`{VARIABLE}`]. There are only 2 rules for
+variable names: - Variable name can include upper-cased letters \[`A-Z`\],
+underscore \[`_`\] and digits \{`0-9`\} only - Variable name must start with a
+letter Variable can be defined with: - any atomic value - any other variable
+defined - any Mimeo Util You can use Mimeo Vars as partial values (unless they
+are defined as Mimeo Utils). Example: ```json { "vars": { "CUSTOM_VAR_1":
+"custom-value-1", "CUSTOM_VAR_2": 1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "
+{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "{auto_increment}", "CUSTOM_VAR_6":
+{ "_mimeo_util": { "_name": "random_int", "limit": 99 } } }, "_templates_": [
+{ "count": 5, "model": { "SomeEntity": { "ChildNode1": "{CUSTOM_VAR_1}",
+"ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3": "{CUSTOM_VAR_3}", "ChildNode4": "
+{CUSTOM_VAR_4}", "ChildNode5": "{CUSTOM_VAR_5}", "ChildNode6": "
+{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-with-suffix" } } } ] } ``` ####
+Mimeo Special Fields In Mimeo Template you can use so-called _special fields_.
+Every field in a template can be stored in memory (_provided_) and used later
+as a value of other fields (_injected_) in context of a single iteration. To
 provide a special field, wrap its name with colons: [`:SomeField:`]. To inject,
 use additionally curly braces to let interpreter know it should be rendered [`
 {:SomeField:}`]. They can be injected as partial values, similarly to Mimeo
 Vars. Example ```json { "_templates_": [ { "count": 5, "model": { "SomeEntity":
 { ":ChildNode1:": "custom-value", "ChildNode2": "{:ChildNode1:}", "ChildNode3":
-"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Utils You can use several
-predefined functions to generate data. They can be used in a _raw_ format or
-_parametrized_. ##### Random String Generates a random string value. |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | length | `int` | `20` | ###### Raw Uses the default length: 20
-characters. ```json { "randomstring": "{random_str}" } ``` ###### Parametrized
-Uses the customized length. ```json { "randomstring": { "_mimeo_util":
-{ "_name": "random_str", "length": 5 } } } ``` ##### Random Integer Generates a
-random integer value between `start` and `limit` parameters (inclusive). |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | start | `int` | `1` | | limit | `int` | `100` | ###### Raw Uses the
-default start (1) and limit (100) values. ```json { "randominteger": "
-{random_int}" } ``` ###### Parametrized Uses the customized limit. ```json
-{ "randominteger1": { "_mimeo_util": { "_name": "random_int", "start": 0 } },
-"randominteger2": { "_mimeo_util": { "_name": "random_int", "limit": 5 } },
-"randominteger3": { "_mimeo_util": { "_name": "random_int", "start": 0,
-"limit": 5 } } } ``` ##### Random Item Generates a random value from items
-provided. NOTICE: The raw form of this Mimeo Util will generate a blank string
-value (as same as no items parametrized). | Parameter | Supported values |
-Default | |:---------:|:----------------:|:-------:| | items | `list` | `[""]`
-| ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
+"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Refs Mimeo Special Fields
+are useful when an entity has the same value used in several fields. However,
+usually entities are related with each other. To use references between
+entities, you can use Mimeo Refs. They are configured at the highest Mimeo
+Configuration level and require 3 settings: - context - a context from which
+values will be cached - field - a source field of the reference - type - `any`
+- reference of this type will be used randomly - no order - possible duplicates
+(One-To-Many, Many-To-Many) - `parallel` - reference of this type will generate
+a reference from the same iteration in references entity - same order as in
+parent entity - unique values (One-To-One) To use them in a Mimeo Template,
+simply wrap a reference name with curly braces [`{some-reference}`]. > Note: >
+- A reference can't be configured using any of Mimeo Utils' names nor existing
+Mimeo Vars > - A referenced entity needs to be placed before a referencing one
+Example ```json { "refs": { "parent-one-to-many": { "context": "SomeEntity",
+"field": "ID", "type": "any" }, "parent-one-to-one": { "context": "SomeEntity",
+"field": "ID", "type": "parallel" } }, "_templates_": [ { "count": 5, "model":
+{ "SomeEntity": { "ID": "{key}" } } }, { "count": 5, "model":
+{ "OneToOneChildEntity": { "Parent": "{parent-one-to-one}" } } }, { "count":
+10, "model": { "ManyToOneChildEntity": { "Parent": "{parent-one-to-many}" } } }
+] } ``` #### Mimeo Utils You can use several predefined functions to generate
+data. They can be used in a _raw_ format or _parametrized_. ##### Random String
+Generates a random string value. | Parameter | Supported values | Default | |:-
+--------:|:----------------:|:-------:| | length | `int` | `20` | ###### Raw
+Uses the default length: 20 characters. ```json { "randomstring": "
+{random_str}" } ``` ###### Parametrized Uses the customized length. ```json
+{ "randomstring": { "_mimeo_util": { "_name": "random_str", "length": 5 } } }
+``` ##### Random Integer Generates a random integer value between `start` and
+`limit` parameters (inclusive). | Parameter | Supported values | Default | |:--
+-------:|:----------------:|:-------:| | start | `int` | `1` | | limit | `int`
+| `100` | ###### Raw Uses the default start (1) and limit (100) values. ```json
+{ "randominteger": "{random_int}" } ``` ###### Parametrized Uses the customized
+limit. ```json { "randominteger1": { "_mimeo_util": { "_name": "random_int",
+"start": 0 } }, "randominteger2": { "_mimeo_util": { "_name": "random_int",
+"limit": 5 } }, "randominteger3": { "_mimeo_util": { "_name": "random_int",
+"start": 0, "limit": 5 } } } ``` ##### Random Item Generates a random value
+from items provided. NOTICE: The raw form of this Mimeo Util will generate a
+blank string value (as same as no items parametrized). | Parameter | Supported
+values | Default | |:---------:|:----------------:|:-------:| | items | `list`
+| `[""]` | ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
 "random_item", "items": ["value", 1, true] } } } ``` ##### Date Generates a
 date value in format `YYYY-MM-DD`. | Parameter | Supported values | Default |
 |:----------:|:----------------:|:-------:| | days_delta | `int` | `0` | ######
 Raw Uses the today's date. ```json { "Today": "{date}" } ``` ######
 Parametrized Uses the customized days delta. ```json { "Yesterday":
 { "_mimeo_util": { "_name": "date", "days_delta": -1 } }, "Tomorrow":
 { "_mimeo_util": { "_name": "date", "days_delta": 1 } } } ``` ##### Date Time
```

### Comparing `mimeograph-1.0.4/pyproject.toml` & `mimeograph-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "1.0.4"
+version = "1.1.0"
 description = "Generate NoSQL data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -61,15 +61,15 @@
     "pytest-asyncio"
 ]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.4"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
@@ -99,15 +99,15 @@
     "src/mimeo/generators/__init__.py"
 ]
 
 [tool.ruff]
 select = [
     "F", "E", "W", "C90", "N", "D", "UP", "B", "A", "COM", "C4", "EM", "EXE", "ISC", "G", "PIE", "T20",
     "PT", "Q", "RSE", "RET", "SLF", "SIM", "ARG", "PTH", "ERA", "PD", "PGH", "PL", "TRY", "RUF", "FLY",
-    "ASYNC", "FA", "FIX"
+    "ASYNC", "FA", "FIX", "CPY", "PERF"
 ]
 ignore = []
 exclude = [
     ".git",
     ".github",
     ".idea",
     ".pytest_cache",
```

### Comparing `mimeograph-1.0.4/src/mimeo/__init__.py` & `mimeograph-1.1.0/src/mimeo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,9 +48,9 @@
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
 from .config import MimeoConfig, MimeoConfigFactory
 from .mimeo import Mimeograph
 
-__version__ = "1.0.4"
+__version__ = "1.1.0"
 __all__ = ["MimeoConfig", "MimeoConfigFactory", "Mimeograph"]
```

### Comparing `mimeograph-1.0.4/src/mimeo/cli/__init__.py` & `mimeograph-1.1.0/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/cli/exc.py` & `mimeograph-1.1.0/src/mimeo/cli/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/cli/job.py` & `mimeograph-1.1.0/src/mimeo/cli/job.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/cli/parsers.py` & `mimeograph-1.1.0/src/mimeo/cli/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v1.0.4")
+            version="%(prog)s v1.1.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
```

### Comparing `mimeograph-1.0.4/src/mimeo/config/__init__.py` & `mimeograph-1.1.0/src/mimeo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/config/constants.py` & `mimeograph-1.1.0/src/mimeo/config/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,92 +10,118 @@
     _cc = constants["mimeo-config"]
 
 CONFIG_XML_ROOT_NAME: str = _cc["key"]
 
 ########################################################################################
 #                                    OUTPUT DETAILS                                    #
 ########################################################################################
-_output_constants = _cc["output"]
+_output_constants: dict = _cc["output"]
 OUTPUT_KEY: str = _output_constants["key"]
 OUTPUT_FORMAT_KEY: str = _output_constants["format"]["key"]
 OUTPUT_DIRECTION_KEY: str = _output_constants["direction"]["key"]
 
 ########################################################################################
 # --------------------------------- format specific ---------------------------------- #
-_format_details = _output_constants["format"]["details"]
+_format_details: dict = _output_constants["format"]["details"]
 OUTPUT_INDENT_KEY: str = _format_details["indent"]["key"]
 
-_format_values = _output_constants["format"]["values"]
+_format_values: dict = _output_constants["format"]["values"]
 SUPPORTED_OUTPUT_FORMATS: tuple = tuple(
     format_["key"]
     for format_ in _format_values.values())
 OUTPUT_FORMAT_XML: str = _format_values["xml"]["key"]
 OUTPUT_FORMAT_JSON: str = _format_values["json"]["key"]
 
 # -------------------------------- xml format specific ------------------------------- #
-_xml_format_details = _format_values["xml"]["details"]
+_xml_format_details: dict = _format_values["xml"]["details"]
 OUTPUT_XML_DECLARATION_KEY: str = _xml_format_details["xml-declaration"]["key"]
 
 ########################################################################################
 # -------------------------------- direction specific -------------------------------- #
-_direction_details = _output_constants["direction"]["values"]
+_direction_details: dict = _output_constants["direction"]["values"]
 SUPPORTED_OUTPUT_DIRECTIONS: tuple = tuple(
     direction["key"]
     for direction in _direction_details.values())
 OUTPUT_DIRECTION_FILE: str = _direction_details["file"]["key"]
 OUTPUT_DIRECTION_STD_OUT: str = _direction_details["std-out"]["key"]
 OUTPUT_DIRECTION_HTTP: str = _direction_details["http"]["key"]
 
 # ----------------------------- file direction specific ------------------------------ #
-_file_direction_details = _direction_details["file"]["details"]
+_file_direction_details: dict = _direction_details["file"]["details"]
 OUTPUT_DIRECTORY_PATH_KEY: str = _file_direction_details["directory-path"]["key"]
 OUTPUT_FILE_NAME_KEY: str = _file_direction_details["file-name"]["key"]
 
 # ----------------------------- http direction specific ------------------------------ #
-_http_direction_details = _direction_details["http"]["details"]
+_http_direction_details: dict = _direction_details["http"]["details"]
 REQUIRED_HTTP_DETAILS: tuple = tuple(
     prop["key"] for prop in _http_direction_details.values()
     if prop.get("required", False) is True)
 
 OUTPUT_METHOD_KEY: str = _http_direction_details["method"]["key"]
 OUTPUT_PROTOCOL_KEY: str = _http_direction_details["protocol"]["key"]
 OUTPUT_HOST_KEY: str = _http_direction_details["host"]["key"]
 OUTPUT_PORT_KEY: str = _http_direction_details["port"]["key"]
 OUTPUT_ENDPOINT_KEY: str = _http_direction_details["endpoint"]["key"]
 OUTPUT_USERNAME_KEY: str = _http_direction_details["username"]["key"]
 OUTPUT_PASSWORD_KEY: str = _http_direction_details["password"]["key"]
 
-_req_method_details = _http_direction_details["method"]["values"]
-SUPPORTED_REQUEST_METHODS: str = _req_method_details.values()
+_req_method_details: dict = _http_direction_details["method"]["values"]
+SUPPORTED_REQUEST_METHODS: tuple = tuple(_req_method_details.values())
 OUTPUT_HTTP_REQUEST_POST: str = _req_method_details["post"]
 OUTPUT_HTTP_REQUEST_PUT: str = _req_method_details["put"]
 
-_req_protocol_details = _http_direction_details["protocol"]["values"]
-SUPPORTED_REQUEST_PROTOCOLS: str = _req_protocol_details.values()
+_req_protocol_details: dict = _http_direction_details["protocol"]["values"]
+SUPPORTED_REQUEST_PROTOCOLS: tuple = tuple(_req_protocol_details.values())
 OUTPUT_PROTOCOL_HTTP: str = _req_protocol_details["http"]
 OUTPUT_PROTOCOL_HTTPS: str = _req_protocol_details["https"]
 
 ########################################################################################
 #                                      MIMEO VARS                                      #
 ########################################################################################
-_vars_constants = _cc["vars"]
+_vars_constants: dict = _cc["vars"]
 VARS_KEY: str = _vars_constants["key"]
 
 ########################################################################################
+#                                      MIMEO REFS                                      #
+########################################################################################
+_refs_constants: dict = _cc["refs"]
+REFS_KEY: str = _refs_constants["key"]
+
+########################################################################################
+# ---------------------------------- refs details ------------------------------------ #
+_refs_details: dict = _refs_constants["details"]
+REQUIRED_REFS_DETAILS: tuple = tuple(
+    prop["key"] for prop in _refs_details.values()
+    if prop.get("required", False) is True)
+REFS_DETAIL_CONTEXT: str = _refs_details["context"]["key"]
+REFS_DETAIL_FIELD: str = _refs_details["field"]["key"]
+REFS_DETAIL_TYPE: str = _refs_details["type"]["key"]
+
+# ------------------------------------ refs types ------------------------------------ #
+_refs_types: dict = _refs_details["type"]["values"]
+SUPPORTED_REFS_TYPES: tuple = tuple(_refs_types.values())
+REFS_TYPE_ANY: str = _refs_details["type"]["values"]["any"]
+REFS_TYPE_PARALLEL: str = _refs_details["type"]["values"]["parallel"]
+
+########################################################################################
+# ------------------------------ refs forbidden names -------------------------------- #
+REFS_FORBIDDEN_NAMES: tuple = tuple(_refs_constants["forbidden-names"])
+
+########################################################################################
 #                                   MIMEO TEMPLATES                                    #
 ########################################################################################
-_templates_constants = _cc["templates"]
+_templates_constants: dict = _cc["templates"]
 TEMPLATES_KEY: str = _templates_constants["key"]
 TEMPLATES_XML_TEMPLATE_TAG: str = _templates_constants["xml-template-tag"]["key"]
 TEMPLATES_COUNT_KEY: str = _templates_constants["count"]["key"]
 TEMPLATES_MODEL_KEY: str = _templates_constants["model"]["key"]
 
 ########################################################################################
 # -------------------------------- Mimeo Model level --------------------------------- #
-_model_constants = _templates_constants["model"]
+_model_constants: dict = _templates_constants["model"]
 MODEL_CONTEXT_KEY: str = _model_constants["context"]["key"]
 MODEL_ATTRIBUTES_KEY: str = _model_constants["attributes"]["key"]
 MODEL_TEXT_VALUE_KEY: str = _model_constants["text-node-value"]["key"]
 MODEL_MIMEO_UTIL_KEY: str = _model_constants["mimeo-util"]["key"]
 MODEL_MIMEO_UTIL_NAME_KEY: str = _model_constants["mimeo-util"]["name"]["key"]
 
 __all__ = [
@@ -125,14 +151,23 @@
     "SUPPORTED_REQUEST_METHODS",
     "OUTPUT_HTTP_REQUEST_POST",
     "OUTPUT_HTTP_REQUEST_PUT",
     "SUPPORTED_REQUEST_PROTOCOLS",
     "OUTPUT_PROTOCOL_HTTP",
     "OUTPUT_PROTOCOL_HTTPS",
     "VARS_KEY",
+    "REFS_KEY",
+    "REQUIRED_REFS_DETAILS",
+    "REFS_DETAIL_CONTEXT",
+    "REFS_DETAIL_FIELD",
+    "REFS_DETAIL_TYPE",
+    "SUPPORTED_REFS_TYPES",
+    "REFS_TYPE_ANY",
+    "REFS_TYPE_PARALLEL",
+    "REFS_FORBIDDEN_NAMES",
     "TEMPLATES_KEY",
     "TEMPLATES_XML_TEMPLATE_TAG",
     "TEMPLATES_COUNT_KEY",
     "TEMPLATES_MODEL_KEY",
     "MODEL_CONTEXT_KEY",
     "MODEL_ATTRIBUTES_KEY",
     "MODEL_TEXT_VALUE_KEY",
```

### Comparing `mimeograph-1.0.4/src/mimeo/config/exc.py` & `mimeograph-1.1.0/src/mimeo/config/exc.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
         A custom Exception class for unsupported properties' values.
     * MissingRequiredPropertyError
         A custom Exception class for missing required properties.
     * InvalidIndentError
         A custom Exception class for invalid indent configuration.
     * InvalidVarsError
         A custom Exception class for invalid vars' configuration.
+    * InvalidRefsError
+        A custom Exception class for invalid refs' configuration.
     * InvalidVarsError.Code
         An Enumeration class for InvalidVarsError error codes.
     * InvalidMimeoModelError
         A custom Exception class for invalid model configuration.
     * InvalidMimeoModelError.Code
         An Enumeration class for InvalidMimeoModelError error codes.
     * InvalidMimeoTemplateError
@@ -122,15 +124,15 @@
 
         Attributes
         ----------
         ERR_1: str
             An error code for vars not being a dictionary
         ERR_2: str
             An error code for vars with non-atomic values
-        ERR_2: str
+        ERR_3: str
             An error code for vars with not allowed characters
         """
 
         ERR_1: str = "NOT_A_DICT"
         ERR_2: str = "COMPLEX_VALUE"
         ERR_3: str = "INVALID_NAME"
 
@@ -189,14 +191,104 @@
                     f"(you can use upper-cased name with underscore and digits, "
                     f"starting with a letter)!")
 
         msg = f"Provided error code is not a {cls.__name__}.Code enum!"
         raise ValueError(msg)
 
 
+class InvalidRefsError(Exception):
+    """A custom Exception class for invalid refs' configuration.
+
+    Raised when vars are not configured properly.
+    """
+
+    class Code(Enum):
+        """An Enumeration class for InvalidRefsError error codes.
+
+        Attributes
+        ----------
+        ERR_1: str
+            An error code for refs not being a dictionary
+        ERR_2: str
+            An error code for a ref not being a dictionary
+        ERR_3: str
+            An error code for refs with missing required details
+        ERR_4: str
+            An error code for refs having same name as a Mimeo Util or a Mimeo Var
+        """
+
+        ERR_1: str = "REFS_NOT_A_DICT"
+        ERR_2: str = "REF_NOT_A_DICT"
+        ERR_3: str = "MISSING_DETAILS"
+        ERR_4: str = "FORBIDDEN_NAME"
+
+    def __init__(
+            self,
+            code: InvalidRefsError.Code,
+            **kwargs,
+    ):
+        """Initialize InvalidRefsError exception with details.
+
+        Extends Exception constructor with a custom message. The message depends on
+        an internal InvalidRefsError code.
+
+        Parameters
+        ----------
+        code : InvalidRefsError.Code
+            An internal error code
+        kwargs
+            An error details
+        """
+        msg = self._get_msg(code, kwargs)
+        super().__init__(msg)
+
+    @classmethod
+    def _get_msg(
+            cls,
+            code: InvalidVarsError.Code,
+            details: dict,
+    ):
+        """Return a custom message based on an error code.
+
+        Parameters
+        ----------
+        code : InvalidRefsError.Code
+            An internal error code
+        details : dict
+            An error details
+
+        Returns
+        -------
+        str
+            A custom error message
+
+        Raises
+        ------
+        ValueError
+            If the code argument is not InvalidRefsError.Code enum
+        """
+        if code == cls.Code.ERR_1:
+            return f"refs property does not store an object: {details['refs']}"
+        if code == cls.Code.ERR_2:
+            return f"The following ref does not store an object: {details['ref']}"
+        if code == cls.Code.ERR_3:
+            required_details = ", ".join(details["required"])
+            references = ", ".join(details["refs"])
+            return (f"Missing required details [{required_details}] in the following "
+                    f"refs [{references}]")
+        if code == cls.Code.ERR_4:
+            references = ", ".join(details["refs"])
+            return ("A reference can't be configured using name of Mimeo Utils "
+                    "or existing Vars. Please rename following refs: "
+                    f"[{references}]")
+
+        msg = f"Provided error code is not a {cls.__name__}.Code enum!"
+        raise ValueError(msg)
+
+
 class InvalidMimeoModelError(Exception):
     """A custom Exception class for invalid model configuration.
 
     Raised when a Mimeo Model is not configured properly.
     """
 
     class Code(Enum):
```

### Comparing `mimeograph-1.0.4/src/mimeo/config/mimeo_config.py` & `mimeograph-1.1.0/src/mimeo/config/mimeo_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from pathlib import Path
 
 import xmltodict
 
 from mimeo.config import constants as cc
 from mimeo.config.exc import (InvalidIndentError, InvalidMimeoConfigError,
                               InvalidMimeoModelError,
-                              InvalidMimeoTemplateError, InvalidVarsError,
+                              InvalidMimeoTemplateError, InvalidRefsError,
+                              InvalidVarsError,
                               MimeoConfigurationNotFoundError,
                               MissingRequiredPropertyError,
                               UnsupportedMimeoConfigSourceError,
                               UnsupportedPropertyValueError)
 from mimeo.logging import setup_logging
 
 # setup logging when mimeo is used as a python library
@@ -465,14 +466,16 @@
 
     It is a python representation of a Mimeo Configuration file / dictionary.
 
     output : MimeoOutput, default {}
         A Mimeo Output Details settings
     vars : dict, default {}
         A Mimeo Configuration vars setting
+    refs : dict, default {}
+        A Mimeo Configuration refs setting
     templates : list
         A Mimeo Templates setting
     """
 
     def __init__(
             self,
             config: dict,
@@ -485,14 +488,15 @@
         ----------
         config : dict
             A source config dictionary
         """
         super().__init__(config)
         self.output: MimeoOutput = MimeoOutput(config.get(cc.OUTPUT_KEY, {}))
         self.vars: dict = self._get_vars(config)
+        self.refs: dict = self._get_refs(config)
         self.templates: list[MimeoTemplate] = self._get_templates(config)
 
     @classmethod
     def _get_vars(
             cls,
             config: dict,
     ) -> dict:
@@ -523,14 +527,75 @@
             if isinstance(val, (list, dict)) and not cls._is_mimeo_util_object(val):
                 raise InvalidVarsError(InvalidVarsError.Code.ERR_2, var=var)
             if not re.match(r"^[A-Z][A-Z_0-9]*$", var):
                 raise InvalidVarsError(InvalidVarsError.Code.ERR_3, var=var)
         return variables
 
     @classmethod
+    def _get_refs(
+            cls,
+            config: dict,
+    ) -> dict:
+        """Extract references from the source dictionary.
+
+        Parameters
+        ----------
+        config : dict
+            A source config dictionary
+
+        Returns
+        -------
+        references : dict
+            Customized references or an empty dictionary
+
+        Raises
+        ------
+        InvalidRefsError
+            If (1) the refs key does not point to a dictionary or
+            (2) any ref is not a dictionary or
+            (3) some refs does not have required details (context, field, type)
+            (4) some refs are configured using names of Mimeo Utils or Vars
+        UnsupportedPropertyValueError
+            If the configured reference type is not supported
+        """
+        references = config.get(cc.REFS_KEY, {})
+        if not isinstance(references, dict):
+            raise InvalidRefsError(InvalidRefsError.Code.ERR_1, refs=references)
+
+        variables = config.get(cc.VARS_KEY, {}).keys()
+        missing_details_references = []
+        forbidden_names_references = []
+        for name, reference in references.items():
+            if not isinstance(reference, dict):
+                raise InvalidRefsError(InvalidRefsError.Code.ERR_2, ref=name)
+
+            if any(detail not in reference for detail in cc.REQUIRED_REFS_DETAILS):
+                missing_details_references.append(name)
+            elif name in cc.REFS_FORBIDDEN_NAMES or name in variables:
+                forbidden_names_references.append(name)
+            else:
+                ref_type = reference[cc.REFS_DETAIL_TYPE]
+                if ref_type not in cc.SUPPORTED_REFS_TYPES:
+                    raise UnsupportedPropertyValueError(
+                        cc.REFS_DETAIL_TYPE,
+                        ref_type,
+                        cc.SUPPORTED_REFS_TYPES)
+        if len(missing_details_references) > 0:
+            raise InvalidRefsError(
+                InvalidRefsError.Code.ERR_3,
+                required=cc.REQUIRED_REFS_DETAILS,
+                refs=missing_details_references)
+        if len(forbidden_names_references) > 0:
+            raise InvalidRefsError(
+                InvalidRefsError.Code.ERR_4,
+                refs=forbidden_names_references)
+
+        return references
+
+    @classmethod
     def _get_templates(
             cls,
             config: dict,
     ) -> list[MimeoTemplate]:
         """Extract Mimeo Templates from the source dictionary.
 
         Parameters
@@ -1039,18 +1104,17 @@
         Raises
         ------
         MissingRequiredPropertyError
             If the output details doesn't include all required settings
             for the direction
         """
         if direction == cc.OUTPUT_DIRECTION_HTTP:
-            missing_details = []
-            for detail in cc.REQUIRED_HTTP_DETAILS:
-                if detail not in output:
-                    missing_details.append(detail)
+            missing_details = [detail
+                               for detail in cc.REQUIRED_HTTP_DETAILS
+                               if detail not in output]
             if len(missing_details) > 0:
                 raise MissingRequiredPropertyError(missing_details)
 
 
 class MimeoTemplate(MimeoDTO):
     """A MimeoDTO class representing Mimeo Template.
```

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/__init__.py` & `mimeograph-1.1.0/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/consumer.py` & `mimeograph-1.1.0/src/mimeo/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/consumer_factory.py` & `mimeograph-1.1.0/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/file_consumer.py` & `mimeograph-1.1.0/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/http_consumer.py` & `mimeograph-1.1.0/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/consumers/raw_consumer.py` & `mimeograph-1.1.0/src/mimeo/consumers/raw_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/context/__init__.py` & `mimeograph-1.1.0/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/context/decorators.py` & `mimeograph-1.1.0/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/context/mimeo_context.py` & `mimeograph-1.1.0/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/context/mimeo_iteration.py` & `mimeograph-1.1.0/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/__init__.py` & `mimeograph-1.1.0/src/mimeo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/cities.py` & `mimeograph-1.1.0/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/countries.py` & `mimeograph-1.1.0/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/currencies.py` & `mimeograph-1.1.0/src/mimeo/database/currencies.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/exc.py` & `mimeograph-1.1.0/src/mimeo/database/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/first_names.py` & `mimeograph-1.1.0/src/mimeo/database/first_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/last_names.py` & `mimeograph-1.1.0/src/mimeo/database/last_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/database/mimeo_db.py` & `mimeograph-1.1.0/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/exc.py` & `mimeograph-1.1.0/src/mimeo/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/generators/__init__.py` & `mimeograph-1.1.0/src/mimeo/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/generators/exc.py` & `mimeograph-1.1.0/src/mimeo/generators/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/generators/generator.py` & `mimeograph-1.1.0/src/mimeo/generators/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 
 import logging
 import xml.etree.ElementTree as ElemTree
 from abc import ABCMeta, abstractmethod
 from typing import Any, Iterator
 
 from mimeo.config.mimeo_config import MimeoTemplate
-from mimeo.context import MimeoContext
+from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.decorators import (mimeo_clear_iterations, mimeo_context,
                                       mimeo_context_switch,
                                       mimeo_next_iteration)
+from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
 class Generator(metaclass=ABCMeta):
     """An abstract class for data generators in Mimeo.
 
@@ -157,29 +158,26 @@
 
     @classmethod
     @abstractmethod
     def _process_atomic_value(
             cls,
             parent: ElemTree.Element | dict | list | None,
             node_meta: dict,
-            context: MimeoContext,
     ) -> ElemTree.Element | dict | list | None:
         """Process a node with an atomic value.
 
         A parametrized Mimeo Util is considered as an atomic value as representing one.
         It renders a value for the node.
 
         Parameters
         ----------
         parent : ElemTree.Element | dict | list | None
             A parent node
         node_meta : dict
             Node's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
         ElemTree.Element | dict | list | None
             A processed node
         """
         raise NotImplementedError
@@ -252,50 +250,46 @@
         """
         node_meta = cls._node_meta(
             template.model.root_name,
             template.model.root_data)
         return cls._process_node(parent, node_meta)
 
     @classmethod
-    @mimeo_context
     def _process_node(
             cls,
             parent: ElemTree.Element | dict | list | None,
             node_meta: dict,
-            context: MimeoContext | None = None,
     ) -> ElemTree.Element | dict:
         """Process a single template's node.
 
         This is a recursive function that traverses Mimeo Template and generates nodes
         based on node's metadata. First, element is pre-processed, in meaning
         of metadata being adjusted. Then, element is processed accordingly to its value
         type.
 
         Parameters
         ----------
         parent : ElemTree.Element | dict | list | None
             A parent node
         node_meta : dict
             Node's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
         ElemTree.Element | dict
             A single data unit generated within a single template iteration.
         """
         logger.fine("Rendering element - parent [%s], node_meta [%s]",
                     parent if not isinstance(parent, ElemTree.Element) else parent.tag,
                     node_meta)
         node_meta = cls._pre_process_node(node_meta)
 
         if cls._is_complex(node_meta):
             return cls._process_complex_value(parent, node_meta)
-        return cls._process_atomic_value(parent, node_meta, context)
+        return cls._process_atomic_value(parent, node_meta)
 
     @staticmethod
     def _is_complex(
             node_meta: dict,
     ) -> bool:
         """Verify if a node is complex.
 
@@ -344,7 +338,36 @@
         return {
             "name": name,
             "value": value,
             "attrs": attrs,
             "mimeo_util": is_mimeo_util,
             "special": is_special_field,
         }
+
+    @staticmethod
+    @mimeo_context
+    def _render_atomic_value(
+            node_meta: dict,
+            context: MimeoContext | None = None,
+    ) -> Any:
+        """Render an atomic value for a node.
+
+        It implements a common logic for all generators. Once the atomic value is
+        rendered it is cached in references (if any configured) and special fields.
+
+        Parameters
+        ----------
+        node_meta : dict
+            Node's metadata
+        context
+            The current Mimeo Context (injected by MimeoContextManager)
+
+        Returns
+        -------
+        value : Any
+            A rendered value
+        """
+        value = MimeoRenderer.render(node_meta["value"])
+        MimeoContextManager().cache_ref(node_meta["name"], value)
+        if node_meta["special"]:
+            context.curr_iteration().add_special_field(node_meta["name"], value)
+        return value
```

### Comparing `mimeograph-1.0.4/src/mimeo/generators/generator_factory.py` & `mimeograph-1.1.0/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/generators/json_generator.py` & `mimeograph-1.1.0/src/mimeo/generators/json_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 import json
 import logging
 from typing import Iterator
 
 from mimeo.config import constants as cc
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
-from mimeo.context import MimeoContext
-from mimeo.context.decorators import mimeo_context
 from mimeo.generators import Generator
 from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
 class JSONGenerator(Generator):
@@ -101,49 +99,45 @@
         """
         if self._indent is not None and self._indent != 0:
             return json.dumps(data_unit, indent=self._indent)
 
         return json.dumps(data_unit)
 
     @classmethod
-    @mimeo_context
     def _process_node(
             cls,
             parent: dict | list | None,
             node_meta: dict,
-            context: MimeoContext | None = None,
     ) -> dict | list:
         """Process a single template's node.
 
         Extends Generator's implementation by setting a parent node when it is None.
         It is required for JSON format to initialize an object.
 
         Parameters
         ----------
         parent : dict | list | None
             A parent node
         node_meta : dict
             Node's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
         dict | list
             A single data unit generated within a single template iteration.
 
         Raises
         ------
         InvalidSpecialFieldValueError
             If a special field value is dict or list
         SpecialFieldNotFoundError
             If a special field does not exist.
         """
         parent = parent if parent is not None else {}
-        return super()._process_node(parent, node_meta, context)
+        return super()._process_node(parent, node_meta)
 
     @classmethod
     def _pre_process_node(
             cls,
             node_meta: dict,
     ) -> dict:
         """Pre-process node's metadata.
@@ -476,38 +470,34 @@
         templates = (MimeoTemplate(template)
                      for template in node_meta["value"][cc.TEMPLATES_KEY])
         target = parent
         if isinstance(parent, dict):
             parent[node_meta["name"]] = []
             target = parent[node_meta["name"]]
 
-        for child in cls.generate(templates):
-            target.append(child)
+        target.extend(cls.generate(templates))
         return parent
 
     @classmethod
     def _process_atomic_value(
             cls,
             parent: dict | list,
             node_meta: dict,
-            context: MimeoContext,
     ) -> dict | list:
         """Process a node with an atomic value.
 
         A parametrized Mimeo Util is considered as an atomic value as representing one.
         It renders a value for the node.
 
         Parameters
         ----------
         parent : dict | list
             A parent node
         node_meta : dict
             Node's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
         dict | list
             A processed node
 
         Raises
@@ -515,41 +505,37 @@
         InvalidSpecialFieldValueError
             If a special field value is dict or list
         SpecialFieldNotFoundError
             If a special field does not exist.
 
         Examples
         --------
-        context = MimeoContextManager().get_current_context()
         parent = {}
         node_meta = cls._node_meta(
             name="SomeField",
             value="value-1",
         )
-        cls._process_atomic_value(parent, node_meta, context)
+        cls._process_atomic_value(parent, node_meta)
         ->
         {
           "SomeField": "value-1"
         }
 
-        context = MimeoContextManager().get_current_context()
         parent = []
         node_meta = cls._node_meta(
             name=None,
             value="value-1",
         )
-        cls._process_atomic_value(parent, node_meta, context)
+        cls._process_atomic_value(parent, node_meta)
         ->
         [
           "value-1"
         ]
         """
-        value = MimeoRenderer.render(node_meta["value"])
-        if node_meta["special"]:
-            context.curr_iteration().add_special_field(node_meta["name"], value)
+        value = super()._render_atomic_value(node_meta)
         if isinstance(parent, dict):
             parent[node_meta["name"]] = value
         elif isinstance(parent, list):
             parent.append(value)
         logger.fine("Rendered value [%s]", value)
         return parent
```

### Comparing `mimeograph-1.0.4/src/mimeo/generators/xml_generator.py` & `mimeograph-1.1.0/src/mimeo/generators/xml_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import logging
 import xml.etree.ElementTree as ElemTree
 from typing import Iterator
 from xml.dom import minidom
 
 from mimeo.config import constants as cc
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
-from mimeo.context import MimeoContext
 from mimeo.generators import Generator
 from mimeo.generators.exc import UnsupportedStructureError
 from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
@@ -146,15 +145,15 @@
         Returns
         -------
         dict
             Complete node's metadata
         """
         name = node_meta["name"]
         value = node_meta["value"]
-        attrs = {}
+        attrs = node_meta["attrs"] if node_meta["attrs"] is not None else {}
         is_mimeo_util = MimeoRenderer.is_parametrized_mimeo_util(value)
         is_special_field = MimeoRenderer.is_special_field(name)
         if is_special_field:
             name = MimeoRenderer.get_special_field_name(name)
         if isinstance(value, dict):
             value_copy = dict(value)
             for prop in value:
@@ -316,15 +315,18 @@
         </Root>
         """
         for child in node_meta["value"]:
             if isinstance(child, list):
                 raise UnsupportedStructureError(
                     node_meta["name"],
                     node_meta["value"])
-            node_meta = cls._node_meta(node_meta["name"], child)
+            node_meta = cls._node_meta(
+                name=node_meta["name"],
+                value=child,
+                attrs=node_meta["attrs"])
             cls._process_node(parent, node_meta)
         return parent
 
     @classmethod
     def _process_templates_value(
             cls,
             parent: ElemTree.Element,
@@ -389,29 +391,26 @@
         return parent
 
     @classmethod
     def _process_atomic_value(
             cls,
             parent: ElemTree.Element,
             node_meta: dict,
-            context: MimeoContext,
     ) -> ElemTree.Element:
         """Process a node with an atomic value.
 
         A parametrized Mimeo Util is considered as an atomic value as representing one.
         It renders a value for the node.
 
         Parameters
         ----------
         parent : ElemTree.Element | None
             A parent node
         node_meta : dict
             Node's metadata
-        context : MimeoContext, default None
-            The current Mimeo Context (injected by MimeoContextManager)
 
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
@@ -421,28 +420,25 @@
         InvalidSpecialFieldValueError
             If a special field value is dict or list
         SpecialFieldNotFoundError
             If a special field does not exist.
 
         Examples
         --------
-        context = MimeoContextManager().get_current_context()
         parent = ElemTree.Element("Root")
         node_meta = cls._node_meta(
             name="SomeField",
             value="value-1",
         )
-        cls._process_atomic_value(parent, node_meta, context)
+        cls._process_atomic_value(parent, node_meta)
         ->
         <SomeField>value-1</SomeField>
         """
         element = cls._create_node(parent, node_meta)
-        value = MimeoRenderer.render(node_meta["value"])
-        if node_meta["special"]:
-            context.curr_iteration().add_special_field(node_meta["name"], value)
+        value = super()._render_atomic_value(node_meta)
         val_str = str(value) if value is not None else ""
         element.text = val_str.lower() if isinstance(value, bool) else val_str
         logger.fine("Rendered value [%s]", element.text)
         return element
 
     @staticmethod
     def _create_node(
```

### Comparing `mimeograph-1.0.4/src/mimeo/logging/__init__.py` & `mimeograph-1.1.0/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/logging/filters.py` & `mimeograph-1.1.0/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/meta/__init__.py` & `mimeograph-1.1.0/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/meta/alive.py` & `mimeograph-1.1.0/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/meta/exc.py` & `mimeograph-1.1.0/src/mimeo/meta/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/mimeo.py` & `mimeograph-1.1.0/src/mimeo/mimeo.py`

 * *Files 8% similar despite different names*

```diff
@@ -222,55 +222,82 @@
         It gets a config from a queue and generates data. Once it took a poison pill,
         puts same to a consumer queue.
         """
         while True:
             logger.fine("Getting a config for data generation from queue")
             config_id, mimeo_config = self._generator_queue.get()
             if mimeo_config is None:
-                logger.fine("Closing config generator")
-                for _ in range(self._consumer_workers):
-                    self._consumer_queue.put((None, None, None))
-                self._generator_queue.task_done()
+                self._stop_generate()
                 break
+            self._execute_generator_task(config_id, mimeo_config)
 
-            try:
-                data = list(self.generate(mimeo_config, stringify=True))
-                logger.fine("Putting data to consume to queue")
-                self._consumer_queue.put((config_id, mimeo_config, data))
-            except Exception:
-                self._failed_configs.append(config_id)
-                logger.exception("An unexpected error occurred while generating data "
-                                 "from a config [%s]", config_id)
-            finally:
-                self._generator_queue.task_done()
+    def _execute_generator_task(
+            self,
+            config_id: str,
+            mimeo_config: MimeoConfig,
+    ):
+        """Execute a generator task."""
+        try:
+            data = list(self.generate(mimeo_config, stringify=True))
+            logger.fine("Putting data to consume to queue")
+            self._consumer_queue.put((config_id, mimeo_config, data))
+        except Exception:
+            self._failed_configs.append(config_id)
+            logger.exception("An unexpected error occurred while generating data "
+                             "from a config [%s]", config_id)
+        finally:
+            self._generator_queue.task_done()
+
+    def _stop_generate(
+            self,
+    ):
+        """Stop a generator task."""
+        logger.fine("Closing config generator")
+        for _ in range(self._consumer_workers):
+            self._consumer_queue.put((None, None, None))
+        self._generator_queue.task_done()
 
     def _start_consume(
             self,
     ):
         """Start a consumer task.
 
         Starts an infinitive loop that will work until a poison pill is being submitted.
         It gets data from a queue and consumes it accordingly to a config.
         """
         while True:
             logger.fine("Getting data to consume from queue")
             config_id, mimeo_config, data = self._consumer_queue.get()
             if mimeo_config is None and data is None:
-                logger.fine("Closing data consumer")
-                self._consumer_queue.task_done()
+                self._stop_consume()
                 break
+            self._execute_consumer_task(config_id, mimeo_config, data)
 
-            try:
-                self.consume(mimeo_config, data)
-            except Exception:
-                self._failed_configs.append(config_id)
-                logger.exception("An unexpected error occurred while consuming data "
-                                 "from a config [%s]", config_id)
-            finally:
-                self._consumer_queue.task_done()
+    def _execute_consumer_task(
+            self,
+            config_id: str,
+            mimeo_config: MimeoConfig,
+            data: list,
+    ):
+        """Execute a consumer task."""
+        try:
+            self.consume(mimeo_config, data)
+        except Exception:
+            self._failed_configs.append(config_id)
+            logger.exception("An unexpected error occurred while consuming data "
+                             "from a config [%s]", config_id)
+        finally:
+            self._consumer_queue.task_done()
+
+    def _stop_consume(
+            self,
+    ):
+        """Stop a consumer task."""
+        logger.fine("Closing data consumer")
+        self._consumer_queue.task_done()
 
     @classmethod
     def process(
             cls,
             mimeo_config: MimeoConfig,
     ):
         """Process the Mimeo Configuration (generate data and consume).
```

### Comparing `mimeograph-1.0.4/src/mimeo/resources/cities.csv` & `mimeograph-1.1.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/constants.yaml` & `mimeograph-1.1.0/src/mimeo/resources/constants.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
----
 mimeo-config:
   key: mimeo_configuration
 
   output:
     key: output
 
     direction:
@@ -59,14 +58,44 @@
         json:
           key: json
 
 
   vars:
     key: vars
 
+  refs:
+    key: refs
+    details:
+      context:
+        key: context
+        required: Yes
+      field:
+        key: field
+        required: Yes
+      type:
+        key: type
+        required: Yes
+        values:
+          any: any
+          parallel: parallel
+    forbidden-names:
+      - random_str
+      - random_int
+      - random_item
+      - date
+      - date_time
+      - auto_increment
+      - curr_iter
+      - key
+      - city
+      - country
+      - currency
+      - first_name
+      - last_name
+
 
   templates:
     key: _templates_
 
     xml-template-tag:
       key: _template_
```

### Comparing `mimeograph-1.0.4/src/mimeo/resources/countries.csv` & `mimeograph-1.1.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/currencies.csv` & `mimeograph-1.1.0/src/mimeo/resources/currencies.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/exc.py` & `mimeograph-1.1.0/src/mimeo/resources/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/forenames.csv` & `mimeograph-1.1.0/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/logging.yaml` & `mimeograph-1.1.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/resources/surnames.txt` & `mimeograph-1.1.0/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/tools.py` & `mimeograph-1.1.0/src/mimeo/tools.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/utils/__init__.py` & `mimeograph-1.1.0/src/mimeo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/utils/exc.py` & `mimeograph-1.1.0/src/mimeo/utils/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/utils/mimeo_utils.py` & `mimeograph-1.1.0/src/mimeo/utils/mimeo_utils.py`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/src/mimeo/utils/renderers.py` & `mimeograph-1.1.0/src/mimeo/utils/renderers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 the following renderers:
     * MimeoRenderer
         A Facade class rendering Mimeo Utils, Vars and Special Fields.
     * UtilsRenderer
         A class rendering Mimeo Utils.
     * VarsRenderer
         A class rendering Mimeo Vars.
+    * RefsRenderer
+        A class rendering Mimeo Refs.
     * SpecialFieldsRenderer
         A class rendering Mimeo Special Fields.
 """
 from __future__ import annotations
 
 import logging
 import re
@@ -275,14 +277,58 @@
         VarNotFoundError
             If the Mimeo Var with the `var` provided does not exist
         """
         logger.fine("Rendering a variable [%s]", var)
         return MimeoContextManager().get_var(var)
 
 
+class RefsRenderer:
+    """A class rendering Mimeo Refs.
+
+    It contains only a class method.
+
+    Methods
+    -------
+    render(var: str) -> Any
+        Render a Mimeo Ref.
+    """
+
+    @classmethod
+    def render(
+            cls,
+            ref_name: str,
+    ) -> str | int | bool | dict:
+        """Render a Mimeo Ref.
+
+        Parameters
+        ----------
+        ref_name : str
+            A reference name
+
+        Returns
+        -------
+        str | int | bool | dict
+            A reference value
+
+        Raises
+        ------
+        InstanceNotAliveError
+            If the MimeoContextManager instance is not alive
+        ReferenceNotFoundError
+            If there's such a reference configured
+        NonPopulatedReferenceError
+            If the reference has no values
+        NoCorrespondingReferenceError
+            If there was no value cached in a corresponding iteration of the source
+            context
+        """
+        logger.fine("Rendering a reference [%s]", ref_name)
+        return MimeoContextManager().get_ref(ref_name)
+
+
 class SpecialFieldsRenderer:
     """A class rendering Mimeo Special Fields.
 
     It contains only a class method.
 
     Methods
     -------
@@ -336,15 +382,14 @@
         Verify if the field is special (of form {:FIELD_NAME:}).
     is_raw_mimeo_util(value: str) -> bool
         Verify if the value is a raw Mimeo Util.
     is_parametrized_mimeo_util(value: dict)
         Verify if the value is a parametrized Mimeo Util.
     """
 
-    _UTILS_PATTERN: Pattern = re.compile("^{(.+)}$")
     _VARS_PATTERN: Pattern = re.compile(".*({[A-Z_0-9]+})")
     _SPECIAL_FIELDS_PATTERN: Pattern = re.compile(".*({:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:})")
 
     @classmethod
     def get_special_field_name(
             cls,
             wrapped_field_name: str,
@@ -433,26 +478,49 @@
             "_mimeo_util". Otherwise, False.
         """
         return (isinstance(value, dict) and
                 len(value) == 1 and
                 cc.MODEL_MIMEO_UTIL_KEY in value)
 
     @classmethod
+    def is_reference(
+            cls,
+            value: str,
+    ) -> bool:
+        """Verify if the value is a Mimeo Reference.
+
+        Parameters
+        ----------
+        value : str
+            A string value
+
+        Returns
+        -------
+        bool
+            True if the value is a Mimeo Reference. Otherwise, False.
+        """
+        reference_names = MimeoContextManager().get_ref_names()
+        if len(reference_names) == 0:
+            return False
+        reference_re = "^{(" + "|".join(reference_names) + ")}$"
+        return bool(re.match(reference_re, value))
+
+    @classmethod
     def render(
             cls,
             value: Any,
     ) -> Any:
         """Render a value.
 
-        This method renders a value accordingly to its type and form.
-        If the value takes a form of Mimeo Util it is rendered as
-        Mimeo Util (raw or parametrized); if it takes a form of
-        a special field this renderer will try to reach it from
-        the current context; when the value takes a form of a Mimeo Var,
-        then it uses Mimeo Vars defined in Mimeo Config.
+        This method renders a value accordingly to its type and form. If the value
+        takes a form of Mimeo Util it is rendered as a Mimeo Util (raw or parametrized);
+        if it takes a form of a special field this renderer will try to reach it from
+        the current context; when the value takes a form of a Mimeo Var, then it uses
+        Mimeo Vars defined in Mimeo Config; when it is a Mimeo Ref the renderer will
+        try to find a reference value using its metadata from Mimeo Configuration.
         Otherwise, the raw value is returned.
         It is recursively called to return a final value.
 
         Parameters
         ----------
         value : Any
             A value to be rendered
@@ -478,14 +546,21 @@
         OutOfStockError
             If all unique values have been consumed already
         DataNotFoundError
             If database does not contain the expected value
         InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
+        ReferenceNotFoundError
+            If there's such a reference configured
+        NonPopulatedReferenceError
+            If the reference has no values
+        NoCorrespondingReferenceError
+            If there was no value cached in a corresponding iteration of the source
+            context
         """
         logger.fine("Rendering a value [%s]", value)
         try:
             if isinstance(value, str):
                 value = cls._render_string_value(value)
             if cls.is_parametrized_mimeo_util(value):
                 value = cls._render_parametrized_mimeo_util(value)
@@ -497,16 +572,16 @@
     @classmethod
     def _render_string_value(
             cls,
             value: str,
     ) -> Any:
         """Render a string value.
 
-        Depending on value form it can render it as a raw value,
-        a special field, a Mimeo Var or a raw Mimeo Util.
+        Depending on value form it can render it as a raw value, a special field,
+        a Mimeo Var, a raw Mimeo Util or Mimeo Ref.
 
         Parameters
         ----------
         value : str
             A string value
 
         Returns
@@ -516,14 +591,16 @@
         """
         if cls._SPECIAL_FIELDS_PATTERN.match(value):
             return cls._render_special_field(value)
         if cls._VARS_PATTERN.match(value):
             return cls._render_var(value)
         if cls.is_raw_mimeo_util(value):
             return cls._render_raw_mimeo_util(value)
+        if cls.is_reference(value):
+            return cls._render_reference(value)
         return value
 
     @classmethod
     def _render_special_field(
             cls,
             value: str,
     ) -> Any:
@@ -595,14 +672,46 @@
             r_val = cls._render_parametrized_mimeo_util(r_val)
         if len(wrapped_var) != len(value):
             r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
             r_val = value.replace(wrapped_var, str(r_val))
         return cls.render(r_val)
 
     @classmethod
+    def _render_reference(
+            cls,
+            value: str,
+    ) -> Any:
+        """Render a Mimeo Ref.
+
+        Parameters
+        ----------
+        value : str
+            A Mimeo Ref
+
+        Returns
+        -------
+        Any
+            A rendered value
+
+        Raises
+        ------
+        InstanceNotAliveError
+            If the MimeoContextManager instance is not alive
+        ReferenceNotFoundError
+            If there's such a reference configured
+        NonPopulatedReferenceError
+            If the reference has no values
+        NoCorrespondingReferenceError
+            If there was no value cached in a corresponding iteration of the source
+            context
+        """
+        rendered_value = RefsRenderer.render(value[1:][:-1])
+        return cls.render(rendered_value)
+
+    @classmethod
     def _render_raw_mimeo_util(
             cls,
             value: str,
     ) -> Any:
         """Render a raw Mimeo Util.
 
         Parameters
```

### Comparing `mimeograph-1.0.4/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-1.1.0/src/mimeograph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 1.0.4
+Version: 1.1.0
 Summary: Generate NoSQL data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,16 @@
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
 [![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and a python library generating NoSQL data based on a template.
-It can be used by developers, testers or business analysts in their daily work.
+It can be used by developers, testers or business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data).
 
 
 ## Installation
 
 Install Mimeo with pip
 
 ```sh
@@ -294,35 +295,36 @@
 |:------------:|:-----------------|:------------------------------------------------|
 |              | `--sequentially` | process Mimeo Configurations in a single thread |
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
-| Key                      |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
-|:-------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output/format`          |  Config  |        :x:         |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
-| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
-| `vars`                   |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
-| `_templates_`            |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
-| `count`                  | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
-| `model`                  | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
-| `context`                |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
+| Key                      |  Level   |  Required   |     Supported values     |    Default     | Description                                                                                                                                             |
+|:-------------------------|:--------:|:-----------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `output`                 |  Config  | **&#9744;** |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  | **&#9744;** | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  | **&#9744;** |      `xml`, `json`       |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  | **&#9744;** |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  | **&#9744;** |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  | **&#9744;** |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  | **&#9744;** |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  | **&#9744;** |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  | **&#9744;** |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/username`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | **&#9745;** |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `vars`                   |  Config  | **&#9744;** |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more below)                                                                                      |
+| `refs`                   |  Config  | **&#9744;** |          object          |      ---       | Defines references to be used in a Mimeo Template (read more below)                                                                                     |
+| `_templates_`            |  Config  | **&#9745;** |          array           |      ---       | Stores templates for data generation                                                                                                                    |
+| `count`                  | Template | **&#9745;** |         integer          |      ---       | Indicates number of copies                                                                                                                              |
+| `model`                  | Template | **&#9745;** |          object          |      ---       | Defines data template to be copied                                                                                                                      |
+| `context`                |  Model   | **&#9744;** |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
@@ -405,15 +407,16 @@
   ]
 }
 ```
 
 #### Mimeo Special Fields
 
 In Mimeo Template you can use so-called _special fields_.
-Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_).
+Every field in a template can be stored in memory (_provided_) and used later as a value of other fields (_injected_)
+in context of a single iteration.
 To provide a special field, wrap its name with colons: [`:SomeField:`]. To inject, use additionally curly braces to
 let interpreter know it should be rendered [`{:SomeField:}`].
 They can be injected as partial values, similarly to Mimeo Vars.
 
 Example
 ```json
 {
@@ -428,14 +431,79 @@
         }
       }
     }
   ]
 }
 ```
 
+#### Mimeo Refs
+
+Mimeo Special Fields are useful when an entity has the same value used in several fields.
+However, usually entities are related with each other. To use references between entities, you can use
+Mimeo Refs. They are configured at the highest Mimeo Configuration level and require 3 settings:
+- context - a context from which values will be cached
+- field - a source field of the reference 
+- type
+  - `any` - reference of this type will be used randomly
+    - no order
+    - possible duplicates (One-To-Many, Many-To-Many)
+  - `parallel` - reference of this type will generate a reference from the same iteration in references entity
+    - same order as in parent entity
+    - unique values (One-To-One)
+
+To use them in a Mimeo Template, simply wrap a reference name with curly braces [`{some-reference}`].
+
+> Note:
+>  - A reference can't be configured using any of Mimeo Utils' names nor existing Mimeo Vars
+>  - A referenced entity needs to be placed before a referencing one
+
+Example
+```json
+{
+  "refs": {
+    "parent-one-to-many": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "any"
+    },
+    "parent-one-to-one": {
+      "context": "SomeEntity",
+      "field": "ID",
+      "type": "parallel"
+    }
+  },
+  "_templates_": [
+    {
+      "count": 5,
+      "model": {
+        "SomeEntity": {
+          "ID": "{key}"
+        }
+      }
+    },
+    {
+      "count": 5,
+      "model": {
+        "OneToOneChildEntity": {
+          "Parent": "{parent-one-to-one}"
+        }
+      }
+    },
+    {
+      "count": 10,
+      "model": {
+        "ManyToOneChildEntity": {
+          "Parent": "{parent-one-to-many}"
+        }
+      }
+    }
+  ]
+}
+```
+
 #### Mimeo Utils
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mimeograph Version: 1.0.4 Summary: Generate NoSQL
+Metadata-Version: 2.1 Name: mimeograph Version: 1.1.0 Summary: Generate NoSQL
 data based on a simple template Author-email: "T.A. Programming Svcs."
 maciej.aniolowski@gmail.com> License: MIT License Copyright (c) 2023 Tomasz
 AnioÅowski Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -39,17 +39,18 @@
 github.com/TomaszAniolowski/mimeo/actions/workflows/
 test.yml?query=branch%3Amain) [![Code Coverage](https://img.shields.io/badge/
 Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/
 TomaszAniolowski/mimeo/actions/workflows/
 coverage_badge.yml?query=branch%3Amain) [Mimeo](https://github.com/
 TomaszAniolowski/mimeo) is a command line tool and a python library generating
 NoSQL data based on a template. It can be used by developers, testers or
-business analysts in their daily work. ## Installation Install Mimeo with pip
-```sh pip install mimeograph ``` ## Usage/Examples ### Mimeo Configuration
-Prepare Mimeo Configuration first
+business analysts in their daily work. Its main advantage over other generators
+is that it can build data with nested nodes at any level (as in real data). ##
+Installation Install Mimeo with pip ```sh pip install mimeograph ``` ## Usage/
+Examples ### Mimeo Configuration Prepare Mimeo Configuration first
 JSON                                     XML
 ```json { "_templates_": [ { "count":    ```xml  <_templates_> <_template_> 30
 30, "model": { "SomeEntity": { "@xmlns": 1 value-2 true      ```
 "http://mimeo.arch.com/default-
 namespace", "@xmlns:pn": "http://
 mimeo.arch.com/prefixed-namespace",
 "ChildNode1": 1, "ChildNode2": "value-
@@ -98,97 +99,116 @@
 ---------------| | | `--silent` | disable INFO logs | | | `--debug` | enable
 DEBUG mode | | | `--fine` | enable FINE mode | #### Other arguments | Short
 option | Long option | Description | |:------------:|:-----------------|:------
 ------------------------------------------| | | `--sequentially` | process
 Mimeo Configurations in a single thread | ### Mimeo Configuration Mimeo
 configuration is defined in a JSON file using internal settings and data
 templates. | Key | Level | Required | Supported values | Default | Description
-| |:-------------------------|:--------:|:------------------:|:----------------
---------:|:--------------:|----------------------------------------------------
+| |:-------------------------|:--------:|:-----------:|:-----------------------
+-:|:--------------:|-----------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | `output` | Config | :x: | object | --- | Defines
-output details on how it will be consumed | | `output/direction` | Config | :x:
-| `file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
-`output/format` | Config | :x: | `xml`, `json` | `xml` | Defines output data
-format | | `output/indent` | Config | :x: | integer | `null` | Defines indent
-applied in output data | | `output/xml_declaration` | Config | :x: | boolean |
-`false` | Indicates whether an xml declaration should be added to output data |
-| `output/directory_path` | Config | :x: | string | `mimeo-output` | For `file`
-direction - defines an output directory | | `output/file_name` | Config | :x: |
-string | `mimeo-output` | For `file` direction - defines an output file name |
-| `output/method` | Config | :x: | `POST`, `PUT` | `POST` | For `http`
-direction - defines a request method | | `output/protocol` | Config | :x: |
-`http`, `https` | `http` | For `http` direction - defines a url protocol | |
-`output/host` | Config | :heavy_check_mark: | string | --- | For `http`
-direction - defines a url host | | `output/port` | Config | :x: | integer |
+---------------| | `output` | Config | **☐** | object | --- | Defines output
+details on how it will be consumed | | `output/direction` | Config | **☐** |
+`file`, `stdout`, `http` | `file` | Defines how output will be consumed | |
+`output/format` | Config | **☐** | `xml`, `json` | `xml` | Defines output data
+format | | `output/indent` | Config | **☐** | integer | `null` | Defines indent
+applied in output data | | `output/xml_declaration` | Config | **☐** | boolean
+| `false` | Indicates whether an xml declaration should be added to output data
+| | `output/directory_path` | Config | **☐** | string | `mimeo-output` | For
+`file` direction - defines an output directory | | `output/file_name` | Config
+| **☐** | string | `mimeo-output` | For `file` direction - defines an output
+file name | | `output/method` | Config | **☐** | `POST`, `PUT` | `POST` | For
+`http` direction - defines a request method | | `output/protocol` | Config |
+**☐** | `http`, `https` | `http` | For `http` direction - defines a url
+protocol | | `output/host` | Config | **☑** | string | --- | For `http`
+direction - defines a url host | | `output/port` | Config | **☐** | integer |
 `null` | For `http` direction - defines a url port (can be empty) | | `output/
-endpoint` | Config | :heavy_check_mark: | string | --- | For `http` direction -
-defines a url endpoint | | `output/username` | Config | :heavy_check_mark: |
-string | --- | For `http` direction - defines a username | | `output/password`
-| Config | :heavy_check_mark: | string | --- | For `http` direction - defines a
-password | | `vars` | Config | :x: | object | --- | Defines variables to be
-used in a Mimeo Template (read more in next section) | | `_templates_` | Config
-| :heavy_check_mark: | array | --- | Stores templates for data generation | |
-`count` | Template | :heavy_check_mark: | integer | --- | Indicates number of
-copies | | `model` | Template | :heavy_check_mark: | object | --- | Defines
-data template to be copied | | `context` | Model | :x: | object | --- | Defines
-a context name that is internally used e.g. using `curr_iter()` and `get_key()`
-mimeo utils (by default model name is used as the context name) | #### Mimeo
-Environment To make `http` output directory easier to use, mimeo allows you to
-configure Mimeo Environments. They are configured in a JSON file (by default:
-mimeo.envs.json) and support the following output details: - `protocol` -
-`host` - `port` - `username` - `password` Example ```json { "local": { "host":
-"localhost", "port": 8000, "username": "admin", "password": "admin" }, "dev":
-{ "protocol": "https", "host": "11.111.11.111", "port": 8000, "username":
-"some-user", "password": "some-password" } } ``` To use a specific Mimeo
-Environment you can use the following commands: ```sh mimeo SomeEntity-
-config.json -e dev mimeo SomeEntity-config.json -e dev --http-envs-file
-environments.json ``` #### Mimeo Vars Mimeo allows you to define a list of
-variables. You can use them in your Mimeo Config by wrapping them in curly
-brackets [`{VARIABLE}`]. There are only 2 rules for variable names: - Variable
-name can include upper-cased letters \[`A-Z`\], underscore \[`_`\] and digits \
-{`0-9`\} only - Variable name must start with a letter Variable can be defined
-with: - any atomic value - any other variable defined - any Mimeo Util You can
-use Mimeo Vars as partial values (unless they are defined as Mimeo Utils).
-Example: ```json { "vars": { "CUSTOM_VAR_1": "custom-value-1", "CUSTOM_VAR_2":
-1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "
-{auto_increment}", "CUSTOM_VAR_6": { "_mimeo_util": { "_name": "random_int",
-"limit": 99 } } }, "_templates_": [ { "count": 5, "model": { "SomeEntity":
-{ "ChildNode1": "{CUSTOM_VAR_1}", "ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3":
-"{CUSTOM_VAR_3}", "ChildNode4": "{CUSTOM_VAR_4}", "ChildNode5": "
-{CUSTOM_VAR_5}", "ChildNode6": "{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-
-with-suffix" } } } ] } ``` #### Mimeo Special Fields In Mimeo Template you can
-use so-called _special fields_. Every field in a template can be stored in
-memory (_provided_) and used later as a value of other fields (_injected_). To
+endpoint` | Config | **☑** | string | --- | For `http` direction - defines a
+url endpoint | | `output/username` | Config | **☑** | string | --- | For `http`
+direction - defines a username | | `output/password` | Config | **☑** | string
+| --- | For `http` direction - defines a password | | `vars` | Config | **☐** |
+object | --- | Defines variables to be used in a Mimeo Template (read more
+below) | | `refs` | Config | **☐** | object | --- | Defines references to be
+used in a Mimeo Template (read more below) | | `_templates_` | Config | **☑** |
+array | --- | Stores templates for data generation | | `count` | Template |
+**☑** | integer | --- | Indicates number of copies | | `model` | Template |
+**☑** | object | --- | Defines data template to be copied | | `context` | Model
+| **☐** | object | --- | Defines a context name that is internally used e.g.
+using `curr_iter()` and `get_key()` mimeo utils (by default model name is used
+as the context name) | #### Mimeo Environment To make `http` output directory
+easier to use, mimeo allows you to configure Mimeo Environments. They are
+configured in a JSON file (by default: mimeo.envs.json) and support the
+following output details: - `protocol` - `host` - `port` - `username` -
+`password` Example ```json { "local": { "host": "localhost", "port": 8000,
+"username": "admin", "password": "admin" }, "dev": { "protocol": "https",
+"host": "11.111.11.111", "port": 8000, "username": "some-user", "password":
+"some-password" } } ``` To use a specific Mimeo Environment you can use the
+following commands: ```sh mimeo SomeEntity-config.json -e dev mimeo SomeEntity-
+config.json -e dev --http-envs-file environments.json ``` #### Mimeo Vars Mimeo
+allows you to define a list of variables. You can use them in your Mimeo Config
+by wrapping them in curly brackets [`{VARIABLE}`]. There are only 2 rules for
+variable names: - Variable name can include upper-cased letters \[`A-Z`\],
+underscore \[`_`\] and digits \{`0-9`\} only - Variable name must start with a
+letter Variable can be defined with: - any atomic value - any other variable
+defined - any Mimeo Util You can use Mimeo Vars as partial values (unless they
+are defined as Mimeo Utils). Example: ```json { "vars": { "CUSTOM_VAR_1":
+"custom-value-1", "CUSTOM_VAR_2": 1, "CUSTOM_VAR_3": true, "CUSTOM_VAR_4": "
+{CUSTOM_VAR_2}", "CUSTOM_VAR_5": "{auto_increment}", "CUSTOM_VAR_6":
+{ "_mimeo_util": { "_name": "random_int", "limit": 99 } } }, "_templates_": [
+{ "count": 5, "model": { "SomeEntity": { "ChildNode1": "{CUSTOM_VAR_1}",
+"ChildNode2": "{CUSTOM_VAR_2}", "ChildNode3": "{CUSTOM_VAR_3}", "ChildNode4": "
+{CUSTOM_VAR_4}", "ChildNode5": "{CUSTOM_VAR_5}", "ChildNode6": "
+{CUSTOM_VAR_6}", "ChildNode7": "{CUSTOM_VAR_1}-with-suffix" } } } ] } ``` ####
+Mimeo Special Fields In Mimeo Template you can use so-called _special fields_.
+Every field in a template can be stored in memory (_provided_) and used later
+as a value of other fields (_injected_) in context of a single iteration. To
 provide a special field, wrap its name with colons: [`:SomeField:`]. To inject,
 use additionally curly braces to let interpreter know it should be rendered [`
 {:SomeField:}`]. They can be injected as partial values, similarly to Mimeo
 Vars. Example ```json { "_templates_": [ { "count": 5, "model": { "SomeEntity":
 { ":ChildNode1:": "custom-value", "ChildNode2": "{:ChildNode1:}", "ChildNode3":
-"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Utils You can use several
-predefined functions to generate data. They can be used in a _raw_ format or
-_parametrized_. ##### Random String Generates a random string value. |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | length | `int` | `20` | ###### Raw Uses the default length: 20
-characters. ```json { "randomstring": "{random_str}" } ``` ###### Parametrized
-Uses the customized length. ```json { "randomstring": { "_mimeo_util":
-{ "_name": "random_str", "length": 5 } } } ``` ##### Random Integer Generates a
-random integer value between `start` and `limit` parameters (inclusive). |
-Parameter | Supported values | Default | |:---------:|:----------------:|:-----
---:| | start | `int` | `1` | | limit | `int` | `100` | ###### Raw Uses the
-default start (1) and limit (100) values. ```json { "randominteger": "
-{random_int}" } ``` ###### Parametrized Uses the customized limit. ```json
-{ "randominteger1": { "_mimeo_util": { "_name": "random_int", "start": 0 } },
-"randominteger2": { "_mimeo_util": { "_name": "random_int", "limit": 5 } },
-"randominteger3": { "_mimeo_util": { "_name": "random_int", "start": 0,
-"limit": 5 } } } ``` ##### Random Item Generates a random value from items
-provided. NOTICE: The raw form of this Mimeo Util will generate a blank string
-value (as same as no items parametrized). | Parameter | Supported values |
-Default | |:---------:|:----------------:|:-------:| | items | `list` | `[""]`
-| ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
+"{:ChildNode1:}-with-suffix" } } } ] } ``` #### Mimeo Refs Mimeo Special Fields
+are useful when an entity has the same value used in several fields. However,
+usually entities are related with each other. To use references between
+entities, you can use Mimeo Refs. They are configured at the highest Mimeo
+Configuration level and require 3 settings: - context - a context from which
+values will be cached - field - a source field of the reference - type - `any`
+- reference of this type will be used randomly - no order - possible duplicates
+(One-To-Many, Many-To-Many) - `parallel` - reference of this type will generate
+a reference from the same iteration in references entity - same order as in
+parent entity - unique values (One-To-One) To use them in a Mimeo Template,
+simply wrap a reference name with curly braces [`{some-reference}`]. > Note: >
+- A reference can't be configured using any of Mimeo Utils' names nor existing
+Mimeo Vars > - A referenced entity needs to be placed before a referencing one
+Example ```json { "refs": { "parent-one-to-many": { "context": "SomeEntity",
+"field": "ID", "type": "any" }, "parent-one-to-one": { "context": "SomeEntity",
+"field": "ID", "type": "parallel" } }, "_templates_": [ { "count": 5, "model":
+{ "SomeEntity": { "ID": "{key}" } } }, { "count": 5, "model":
+{ "OneToOneChildEntity": { "Parent": "{parent-one-to-one}" } } }, { "count":
+10, "model": { "ManyToOneChildEntity": { "Parent": "{parent-one-to-many}" } } }
+] } ``` #### Mimeo Utils You can use several predefined functions to generate
+data. They can be used in a _raw_ format or _parametrized_. ##### Random String
+Generates a random string value. | Parameter | Supported values | Default | |:-
+--------:|:----------------:|:-------:| | length | `int` | `20` | ###### Raw
+Uses the default length: 20 characters. ```json { "randomstring": "
+{random_str}" } ``` ###### Parametrized Uses the customized length. ```json
+{ "randomstring": { "_mimeo_util": { "_name": "random_str", "length": 5 } } }
+``` ##### Random Integer Generates a random integer value between `start` and
+`limit` parameters (inclusive). | Parameter | Supported values | Default | |:--
+-------:|:----------------:|:-------:| | start | `int` | `1` | | limit | `int`
+| `100` | ###### Raw Uses the default start (1) and limit (100) values. ```json
+{ "randominteger": "{random_int}" } ``` ###### Parametrized Uses the customized
+limit. ```json { "randominteger1": { "_mimeo_util": { "_name": "random_int",
+"start": 0 } }, "randominteger2": { "_mimeo_util": { "_name": "random_int",
+"limit": 5 } }, "randominteger3": { "_mimeo_util": { "_name": "random_int",
+"start": 0, "limit": 5 } } } ``` ##### Random Item Generates a random value
+from items provided. NOTICE: The raw form of this Mimeo Util will generate a
+blank string value (as same as no items parametrized). | Parameter | Supported
+values | Default | |:---------:|:----------------:|:-------:| | items | `list`
+| `[""]` | ###### Parametrized ```json { "random": { "_mimeo_util": { "_name":
 "random_item", "items": ["value", 1, true] } } } ``` ##### Date Generates a
 date value in format `YYYY-MM-DD`. | Parameter | Supported values | Default |
 |:----------:|:----------------:|:-------:| | days_delta | `int` | `0` | ######
 Raw Uses the today's date. ```json { "Today": "{date}" } ``` ######
 Parametrized Uses the customized days delta. ```json { "Yesterday":
 { "_mimeo_util": { "_name": "date", "days_delta": -1 } }, "Tomorrow":
 { "_mimeo_util": { "_name": "date", "days_delta": 1 } } } ``` ##### Date Time
```

### Comparing `mimeograph-1.0.4/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-1.1.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-1.0.4/tests/test_mimeograph.py` & `mimeograph-1.1.0/tests/test_mimeograph.py`

 * *Files identical despite different names*

