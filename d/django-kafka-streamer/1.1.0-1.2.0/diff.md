# Comparing `tmp/django-kafka-streamer-1.1.0.tar.gz` & `tmp/django-kafka-streamer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-kafka-streamer-1.1.0.tar", last modified: Mon May 29 13:57:53 2023, max compression
+gzip compressed data, was "django-kafka-streamer-1.2.0.tar", last modified: Mon Jul 10 12:05:51 2023, max compression
```

## Comparing `django-kafka-streamer-1.1.0.tar` & `django-kafka-streamer-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.209700 django-kafka-streamer-1.1.0/.github/
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.217700 django-kafka-streamer-1.1.0/.github/workflows/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1176 2023-01-13 17:59:53.000000 django-kafka-streamer-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      212 2023-01-12 08:21:00.000000 django-kafka-streamer-1.1.0/.gitignore
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1348 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/LICENSE
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2149 2023-05-29 13:57:53.233700 django-kafka-streamer-1.1.0/PKG-INFO
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1014 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/README.rst
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.225700 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2149 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/PKG-INFO
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1156 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/SOURCES.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        1 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/dependency_links.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)       90 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/requires.txt
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)       20 2023-05-29 13:57:53.000000 django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/top_level.txt
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.225700 django-kafka-streamer-1.1.0/kafkastreamer/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      218 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      226 2023-01-12 15:04:45.000000 django-kafka-streamer-1.1.0/kafkastreamer/apps.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      337 2023-01-12 15:04:45.000000 django-kafka-streamer-1.1.0/kafkastreamer/constants.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2076 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/context.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      864 2023-01-13 17:30:19.000000 django-kafka-streamer-1.1.0/kafkastreamer/decorators.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3905 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/handlers.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/kafkastreamer/management/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/__init__.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1623 2023-01-12 15:06:59.000000 django-kafka-streamer-1.1.0/kafkastreamer/management/commands/kafkastreamer_refresh.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     4514 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/registry.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1042 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/serializers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      673 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/settings.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)    21111 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/kafkastreamer/stream.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1130 2023-01-13 16:27:46.000000 django-kafka-streamer-1.1.0/kafkastreamer/tasks.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      110 2023-01-11 14:51:15.000000 django-kafka-streamer-1.1.0/pyproject.toml
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      102 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/pytest.ini
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1418 2023-05-29 13:57:53.233700 django-kafka-streamer-1.1.0/setup.cfg
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/tests/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:58:50.000000 django-kafka-streamer-1.1.0/tests/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      498 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tests/conftest.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      753 2023-01-13 17:30:19.000000 django-kafka-streamer-1.1.0/tests/test_admin_site.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1321 2023-01-13 16:45:24.000000 django-kafka-streamer-1.1.0/tests/test_command_refresh.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2146 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_context.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1025 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_real_kafka.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2363 2023-01-13 16:46:56.000000 django-kafka-streamer-1.1.0/tests/test_registry.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1770 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_serializers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3205 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_stream_from_signals.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3746 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_stream_manual.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)    12612 2023-05-29 13:56:37.000000 django-kafka-streamer-1.1.0/tests/test_streamer.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1250 2023-01-13 16:47:57.000000 django-kafka-streamer-1.1.0/tests/test_tasks.py
-drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-05-29 13:57:53.229700 django-kafka-streamer-1.1.0/tests/testapp/
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-12 09:37:20.000000 django-kafka-streamer-1.1.0/tests/testapp/__init__.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      281 2023-01-13 16:59:01.000000 django-kafka-streamer-1.1.0/tests/testapp/admin.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      379 2023-01-12 15:50:11.000000 django-kafka-streamer-1.1.0/tests/testapp/models.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      592 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tests/testapp/streamers.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      303 2023-01-12 15:07:04.000000 django-kafka-streamer-1.1.0/tests/utils.py
--rw-r--r--   0 lostclus  (1000) lostclus  (1000)      795 2023-05-29 13:56:41.000000 django-kafka-streamer-1.1.0/tox.ini
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.668881 django-kafka-streamer-1.2.0/
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.660880 django-kafka-streamer-1.2.0/.github/
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.660880 django-kafka-streamer-1.2.0/.github/workflows/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1176 2023-01-13 17:59:53.000000 django-kafka-streamer-1.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      212 2023-01-12 08:21:00.000000 django-kafka-streamer-1.2.0/.gitignore
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1348 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/LICENSE
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2188 2023-07-10 12:05:51.668881 django-kafka-streamer-1.2.0/PKG-INFO
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1014 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/README.rst
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.660880 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2188 2023-07-10 12:05:51.000000 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/PKG-INFO
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1213 2023-07-10 12:05:51.000000 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/SOURCES.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        1 2023-07-10 12:05:51.000000 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/dependency_links.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)       90 2023-07-10 12:05:51.000000 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/requires.txt
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)       20 2023-07-10 12:05:51.000000 django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/top_level.txt
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.664881 django-kafka-streamer-1.2.0/kafkastreamer/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      254 2023-07-10 11:50:57.000000 django-kafka-streamer-1.2.0/kafkastreamer/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      226 2023-01-12 15:04:45.000000 django-kafka-streamer-1.2.0/kafkastreamer/apps.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      337 2023-01-12 15:04:45.000000 django-kafka-streamer-1.2.0/kafkastreamer/constants.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2076 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/kafkastreamer/context.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      864 2023-01-13 17:30:19.000000 django-kafka-streamer-1.2.0/kafkastreamer/decorators.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3905 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/kafkastreamer/handlers.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.664881 django-kafka-streamer-1.2.0/kafkastreamer/management/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.2.0/kafkastreamer/management/__init__.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.664881 django-kafka-streamer-1.2.0/kafkastreamer/management/commands/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:08:36.000000 django-kafka-streamer-1.2.0/kafkastreamer/management/commands/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1623 2023-01-12 15:06:59.000000 django-kafka-streamer-1.2.0/kafkastreamer/management/commands/kafkastreamer_refresh.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      459 2023-07-10 08:54:31.000000 django-kafka-streamer-1.2.0/kafkastreamer/partitioners.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     4514 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/kafkastreamer/registry.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1123 2023-07-10 09:48:13.000000 django-kafka-streamer-1.2.0/kafkastreamer/serializers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      642 2023-07-10 08:51:52.000000 django-kafka-streamer-1.2.0/kafkastreamer/settings.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)    21654 2023-07-10 10:14:16.000000 django-kafka-streamer-1.2.0/kafkastreamer/stream.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1130 2023-01-13 16:27:46.000000 django-kafka-streamer-1.2.0/kafkastreamer/tasks.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      110 2023-01-11 14:51:15.000000 django-kafka-streamer-1.2.0/pyproject.toml
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      102 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/pytest.ini
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1446 2023-07-10 12:05:51.668881 django-kafka-streamer-1.2.0/setup.cfg
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.664881 django-kafka-streamer-1.2.0/tests/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-11 14:58:50.000000 django-kafka-streamer-1.2.0/tests/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      498 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/tests/conftest.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      753 2023-01-13 17:30:19.000000 django-kafka-streamer-1.2.0/tests/test_admin_site.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1321 2023-01-13 16:45:24.000000 django-kafka-streamer-1.2.0/tests/test_command_refresh.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2146 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/tests/test_context.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      642 2023-07-10 09:21:37.000000 django-kafka-streamer-1.2.0/tests/test_partitioners.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1500 2023-07-10 10:26:13.000000 django-kafka-streamer-1.2.0/tests/test_real_kafka.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     2363 2023-01-13 16:46:56.000000 django-kafka-streamer-1.2.0/tests/test_registry.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1808 2023-07-10 08:58:26.000000 django-kafka-streamer-1.2.0/tests/test_serializers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3199 2023-07-10 09:02:22.000000 django-kafka-streamer-1.2.0/tests/test_stream_from_signals.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     3735 2023-07-10 09:01:51.000000 django-kafka-streamer-1.2.0/tests/test_stream_manual.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)    12843 2023-07-10 09:46:07.000000 django-kafka-streamer-1.2.0/tests/test_streamer.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)     1250 2023-01-13 16:47:57.000000 django-kafka-streamer-1.2.0/tests/test_tasks.py
+drwxr-xr-x   0 lostclus  (1000) lostclus  (1000)        0 2023-07-10 12:05:51.668881 django-kafka-streamer-1.2.0/tests/testapp/
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)        0 2023-01-12 09:37:20.000000 django-kafka-streamer-1.2.0/tests/testapp/__init__.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      281 2023-01-13 16:59:01.000000 django-kafka-streamer-1.2.0/tests/testapp/admin.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      379 2023-01-12 15:50:11.000000 django-kafka-streamer-1.2.0/tests/testapp/models.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      592 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/tests/testapp/streamers.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      303 2023-01-12 15:07:04.000000 django-kafka-streamer-1.2.0/tests/utils.py
+-rw-r--r--   0 lostclus  (1000) lostclus  (1000)      795 2023-05-29 15:16:04.000000 django-kafka-streamer-1.2.0/tox.ini
```

### Comparing `django-kafka-streamer-1.1.0/.github/workflows/tests.yml` & `django-kafka-streamer-1.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/LICENSE` & `django-kafka-streamer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/PKG-INFO` & `django-kafka-streamer-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-kafka-streamer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Stream data to Apache Kafka.
 Home-page: http://github.com/lostclus/django-kafka-streamer
 Author: Konstantin Korikov
 Author-email: lostclus@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 django-kafka-streamer
 =====================
```

### Comparing `django-kafka-streamer-1.1.0/README.rst` & `django-kafka-streamer-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/PKG-INFO` & `django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-kafka-streamer
-Version: 1.1.0
+Version: 1.2.0
 Summary: Stream data to Apache Kafka.
 Home-page: http://github.com/lostclus/django-kafka-streamer
 Author: Konstantin Korikov
 Author-email: lostclus@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE
 
 django-kafka-streamer
 =====================
```

### Comparing `django-kafka-streamer-1.1.0/django_kafka_streamer.egg-info/SOURCES.txt` & `django-kafka-streamer-1.2.0/django_kafka_streamer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 django_kafka_streamer.egg-info/top_level.txt
 kafkastreamer/__init__.py
 kafkastreamer/apps.py
 kafkastreamer/constants.py
 kafkastreamer/context.py
 kafkastreamer/decorators.py
 kafkastreamer/handlers.py
+kafkastreamer/partitioners.py
 kafkastreamer/registry.py
 kafkastreamer/serializers.py
 kafkastreamer/settings.py
 kafkastreamer/stream.py
 kafkastreamer/tasks.py
 kafkastreamer/management/__init__.py
 kafkastreamer/management/commands/__init__.py
 kafkastreamer/management/commands/kafkastreamer_refresh.py
 tests/__init__.py
 tests/conftest.py
 tests/test_admin_site.py
 tests/test_command_refresh.py
 tests/test_context.py
+tests/test_partitioners.py
 tests/test_real_kafka.py
 tests/test_registry.py
 tests/test_serializers.py
 tests/test_stream_from_signals.py
 tests/test_stream_manual.py
 tests/test_streamer.py
 tests/test_tasks.py
```

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/context.py` & `django-kafka-streamer-1.2.0/kafkastreamer/context.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/decorators.py` & `django-kafka-streamer-1.2.0/kafkastreamer/decorators.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/handlers.py` & `django-kafka-streamer-1.2.0/kafkastreamer/handlers.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/management/commands/kafkastreamer_refresh.py` & `django-kafka-streamer-1.2.0/kafkastreamer/management/commands/kafkastreamer_refresh.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/registry.py` & `django-kafka-streamer-1.2.0/kafkastreamer/registry.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/serializers.py` & `django-kafka-streamer-1.2.0/kafkastreamer/serializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,9 +38,12 @@
         cls=cls,
         ensure_ascii=ensure_ascii,
     ).encode(
         encoding,
     )
 
 
-def object_id_key_serializer(obj_id, encoding=DEFAULT_ENCODING):
-    return bytes(str(obj_id or 0), encoding)
+def object_id_key_serializer(msg, encoding=DEFAULT_ENCODING):
+    """
+    Returns key based on object ID as encoded string of digits.
+    """
+    return bytes(str(msg.obj_id or 0), encoding)
```

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/settings.py` & `django-kafka-streamer-1.2.0/kafkastreamer/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,16 @@
     "BOOTSTRAP_SERVERS": None,
     "PRODUCER_OPTIONS": {},
     "BATCH_SIZE": 500,
     "DEFAULT_SOURCE": None,
     "DEFAULT_MESSAGE_SERIALIZER": (
         "kafkastreamer.serializers.flat_json_message_serializer"
     ),
-    "DEFAULT_PARTITION_KEY_SERIALIZER": (
-        "kafkastreamer.serializers.object_id_key_serializer"
-    ),
+    "DEFAULT_PARTITION_KEY_SERIALIZER": None,
+    "DEFAULT_PARTITIONER": None,
 }
 
 
 def get_setting(setting_name, resolve=False):
     value = settings.KAFKA_STREAMER.get(
         setting_name,
         DEFAULTS[setting_name],
```

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/stream.py` & `django-kafka-streamer-1.2.0/kafkastreamer/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     prefetch_related = None  # list of related fields to prefetch in queryset
     handle_related = None  # list of related fields to handle changes
     batch_class = Batch
     refresh_finalize_type = "enumerate"
     batch_size = None
     message_serializer = None
     partition_key_serializer = None
+    partitioner = None
     id_field = "id"
     enumerate_ids_field = "ids"
     enumerate_chunk_field = "chunk"
 
     def __init__(self, **kwargs):
         """
         Streamer constructor
@@ -125,14 +126,16 @@
             self.message_serializer = get_setting(
                 "DEFAULT_MESSAGE_SERIALIZER", resolve=True
             )
         if self.partition_key_serializer is None:
             self.partition_key_serializer = get_setting(
                 "DEFAULT_PARTITION_KEY_SERIALIZER", resolve=True
             )
+        if self.partitioner is None:
+            self.partitioner = get_setting("DEFAULT_PARTITIONER", resolve=True)
 
     def get_data_for_object(self, obj, batch):
         """
         Returns data fields for given object
         """
 
         def get_concrete_fields(obj, batch, related_name=None, exclude=None):
@@ -201,14 +204,17 @@
                         value, batch, related_name=name, exclude=self.exclude
                     )
 
                 data[name] = value
 
         return data
 
+    def get_id(self, obj, batch):
+        return obj.pk or getattr(obj, "_kafkastreamer_pre_delete_pk", None)
+
     def get_message(self, obj, batch, msg_type=None, timestamp=None):
         """
         Returns Message tuple for given obj and message type
         """
         if msg_type is None:
             msg_type = TYPE_REFRESH
         if timestamp is None:
@@ -220,16 +226,15 @@
             context=self.get_context_info(),
         )
         data = self.get_data_for_object(obj, batch)
         extra = self.get_extra_data(obj, batch)
         if extra:
             data.update(extra)
 
-        obj_id = obj.pk or getattr(obj, "_kafkastreamer_pre_delete_pk", None)
-
+        obj_id = self.get_id(obj, batch)
         msg = Message(meta=meta, obj_id=obj_id, data=data)
         return msg
 
     def get_delete_message(self, obj_id, timestamp, obj=None, batch=None):
         """
         Returns Message tuple for delete message type for given object ID
         """
@@ -422,14 +427,21 @@
         """
         Returns Kafka producer
         """
         options = {
             "value_serializer": self.message_serializer,
             "key_serializer": self.partition_key_serializer,
             "bootstrap_servers": get_setting("BOOTSTRAP_SERVERS"),
+            **(
+                {
+                    "partitioner": self.partitioner,
+                }
+                if self.partitioner is not None
+                else {}
+            ),
             **self.get_producer_options(),
             **kwargs,
         }
 
         if options.get("bootstrap_servers") is None:
             raise ImproperlyConfigured(
                 "The `KAFKA_STREAMER['BOOTSTRAP_SERVERS']` is not configured."
@@ -460,15 +472,19 @@
             producer = self.get_producer()
         if producer is None:
             return 0
 
         messages_send_count = 0
         try:
             for msg in messages:
-                producer.send(self.topic, msg, key=msg.obj_id)
+                if self.partition_key_serializer is not None:
+                    key = msg
+                else:
+                    key = None
+                producer.send(self.topic, msg, key=key)
                 messages_send_count += 1
                 if batch_size and messages_send_count % batch_size == 0:
                     producer.flush()
 
             if flush:
                 producer.flush()
         except KafkaTimeoutError as e:
```

### Comparing `django-kafka-streamer-1.1.0/kafkastreamer/tasks.py` & `django-kafka-streamer-1.2.0/kafkastreamer/tasks.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/setup.cfg` & `django-kafka-streamer-1.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	Programming Language :: Python :: 3.11
 	Framework :: Django
 	Framework :: Django :: 3
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	Django>=3.2
 	kafka-python>=2.0.2
```

### Comparing `django-kafka-streamer-1.1.0/tests/test_admin_site.py` & `django-kafka-streamer-1.2.0/tests/test_admin_site.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tests/test_command_refresh.py` & `django-kafka-streamer-1.2.0/tests/test_command_refresh.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tests/test_context.py` & `django-kafka-streamer-1.2.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tests/test_registry.py` & `django-kafka-streamer-1.2.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tests/test_serializers.py` & `django-kafka-streamer-1.2.0/tests/test_serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,12 +55,12 @@
         "f_str": "a",
         "f_datetime": "2023-01-02T12:30:00",
         "f_date": "2023-01-03",
         "f_timedelta": "P0DT02H00M00S",
     }
 
 
-def test_object_id_key_serializer():
-    key_bytes = object_id_key_serializer(1)
+def test_object_id_key_serializer(message):
+    key_bytes = object_id_key_serializer(message)
     assert key_bytes == b"1"
-    key_bytes = object_id_key_serializer(None)
+    key_bytes = object_id_key_serializer(message._replace(obj_id=None))
     assert key_bytes == b"0"
```

### Comparing `django-kafka-streamer-1.1.0/tests/test_stream_from_signals.py` & `django-kafka-streamer-1.2.0/tests/test_stream_from_signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 obj_id=obj.pk,
                 data={
                     "id": obj.pk,
                     "field1": 1,
                     "field2": "a",
                 },
             ),
-            key=obj.pk,
+            key=None,
         ),
     ]
 
 
 @patch_producer()
 @patch_now()
 def test_update(producer_m):
@@ -74,15 +74,15 @@
                 obj_id=obj.pk,
                 data={
                     "id": obj.pk,
                     "field1": 2,
                     "field2": "a",
                 },
             ),
-            key=obj.pk,
+            key=None,
         ),
     ]
 
 
 @patch_producer()
 @patch_now()
 def test_delete(producer_m):
@@ -114,10 +114,10 @@
                 obj_id=obj_id,
                 data={
                     "id": obj_id,
                     "field1": 1,
                     "field2": "a",
                 },
             ),
-            key=obj_id,
+            key=None,
         ),
     ]
```

### Comparing `django-kafka-streamer-1.1.0/tests/test_stream_manual.py` & `django-kafka-streamer-1.2.0/tests/test_stream_manual.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 obj_id=obj.pk,
                 data={
                     "id": obj.pk,
                     "field1": 1,
                     "field2": "a",
                 },
             ),
-            key=obj.pk,
+            key=None,
         ),
     ]
 
 
 @patch_producer()
 @patch_now()
 def test_full_refresh(producer_m):
@@ -94,15 +94,15 @@
                 obj_id=obj1.pk,
                 data={
                     "id": obj1.pk,
                     "field1": 1,
                     "field2": "a",
                 },
             ),
-            key=obj1.pk,
+            key=None,
         ),
         mock.call(
             "model-a",
             Message(
                 meta=MessageMeta(
                     timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
                     msg_type=TYPE_REFRESH,
@@ -115,15 +115,15 @@
                 obj_id=obj2.pk,
                 data={
                     "id": obj2.pk,
                     "field1": 2,
                     "field2": "b",
                 },
             ),
-            key=obj2.pk,
+            key=None,
         ),
         mock.call(
             "model-a",
             Message(
                 meta=MessageMeta(
                     timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
                     msg_type=TYPE_ENUMERATE,
@@ -134,10 +134,10 @@
                     ),
                 ),
                 obj_id=obj1.pk,
                 data={
                     "ids": [obj1.pk, obj2.pk],
                 },
             ),
-            key=obj1.pk,
+            key=None,
         ),
     ]
```

### Comparing `django-kafka-streamer-1.1.0/tests/test_streamer.py` & `django-kafka-streamer-1.2.0/tests/test_streamer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import datetime
 from unittest import mock
 
+import pytest
+
 from kafkastreamer import (
     TYPE_CREATE,
     TYPE_DELETE,
     TYPE_ENUMERATE,
     TYPE_EOS,
     stop_handlers,
 )
+from kafkastreamer.serializers import object_id_key_serializer
 from kafkastreamer.stream import Message, MessageContext, MessageMeta
 from tests.testapp.models import ModelA, ModelB, ModelC
 from tests.testapp.streamers import ModelAStreamer, ModelBStreamer, ModelCStreamer
 from tests.utils import patch_producer
 
 
 def test_constructor():
     streamer = ModelAStreamer(batch_size=100)
     assert streamer.batch_size == 100
 
 
+def test_get_id():
+    obj = ModelA.objects.create(field1=1, field2="a")
+    streamer = ModelAStreamer()
+    obj_id = streamer.get_id(obj, batch=None)
+    assert obj_id == obj.pk
+
+
 def test_get_data_for_object():
     obj = ModelA.objects.create(field1=1, field2="a")
     streamer = ModelAStreamer()
     data = streamer.get_data_for_object(obj, batch=None)
     assert data == {
         "id": obj.pk,
         "field1": 1,
@@ -379,79 +389,81 @@
                 "id": obj_id,
             },
         )
         for obj_id in [1, 2, 3]
     ]
 
 
+@pytest.mark.parametrize("partition_key_serializer", [None, object_id_key_serializer])
 @patch_producer()
-def test_send_objects(producer_m):
+def test_send_objects(producer_m, partition_key_serializer):
     producer_send_m = producer_m.return_value.send
     assert len(producer_send_m.mock_calls) == 0
 
     with stop_handlers():
         obj1 = ModelA.objects.create(field1=1, field2="a")
         obj2 = ModelA.objects.create(field1=2, field2="b")
 
-    streamer = ModelAStreamer()
+    streamer = ModelAStreamer(partition_key_serializer=partition_key_serializer)
     count = streamer.send_objects(
         ModelA.objects,
         msg_type=TYPE_CREATE,
         timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
     )
 
     assert count == 2
 
-    assert producer_send_m.mock_calls == [
-        mock.call(
-            "model-a",
-            Message(
-                meta=MessageMeta(
-                    timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
-                    msg_type=TYPE_CREATE,
-                    context=MessageContext(
-                        source="test",
-                        user_id=None,
-                        extra=None,
-                    ),
-                ),
-                obj_id=obj1.pk,
-                data={
-                    "id": obj1.pk,
-                    "field1": 1,
-                    "field2": "a",
-                },
-            ),
-            key=obj1.pk,
-        ),
-        mock.call(
-            "model-a",
-            Message(
-                meta=MessageMeta(
-                    timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
-                    msg_type=TYPE_CREATE,
-                    context=MessageContext(
-                        source="test",
-                        user_id=None,
-                        extra=None,
-                    ),
-                ),
-                obj_id=obj2.pk,
-                data={
-                    "id": obj2.pk,
-                    "field1": 2,
-                    "field2": "b",
-                },
+    msg1 = Message(
+        meta=MessageMeta(
+            timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
+            msg_type=TYPE_CREATE,
+            context=MessageContext(
+                source="test",
+                user_id=None,
+                extra=None,
             ),
-            key=obj2.pk,
         ),
-    ]
+        obj_id=obj1.pk,
+        data={
+            "id": obj1.pk,
+            "field1": 1,
+            "field2": "a",
+        },
+    )
+    msg2 = Message(
+        meta=MessageMeta(
+            timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
+            msg_type=TYPE_CREATE,
+            context=MessageContext(
+                source="test",
+                user_id=None,
+                extra=None,
+            ),
+        ),
+        obj_id=obj2.pk,
+        data={
+            "id": obj2.pk,
+            "field1": 2,
+            "field2": "b",
+        },
+    )
+
+    if partition_key_serializer is None:
+        assert producer_send_m.mock_calls == [
+            mock.call("model-a", msg1, key=None),
+            mock.call("model-a", msg2, key=None),
+        ]
+    else:
+        assert producer_send_m.mock_calls == [
+            mock.call("model-a", msg1, key=msg1),
+            mock.call("model-a", msg2, key=msg2),
+        ]
 
 
-def test_serializers_works():
+def test_message_serializer_works():
     streamer = ModelAStreamer()
 
     msg = Message(
         meta=MessageMeta(
             timestamp=datetime.datetime(2023, 1, 1, 0, 0, 0),
             msg_type=TYPE_CREATE,
             context=MessageContext(
@@ -462,11 +474,9 @@
         ),
         obj_id=1,
         data={
             "id": 1,
         },
     )
 
-    key_bytes = streamer.partition_key_serializer(msg.obj_id)
-    assert type(key_bytes) is bytes
     msg_bytes = streamer.message_serializer(msg)
     assert type(msg_bytes) is bytes
```

### Comparing `django-kafka-streamer-1.1.0/tests/test_tasks.py` & `django-kafka-streamer-1.2.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tests/testapp/streamers.py` & `django-kafka-streamer-1.2.0/tests/testapp/streamers.py`

 * *Files identical despite different names*

### Comparing `django-kafka-streamer-1.1.0/tox.ini` & `django-kafka-streamer-1.2.0/tox.ini`

 * *Files identical despite different names*

