# Comparing `tmp/helios-opentelemetry-sdk-1.0.97.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.97.tar", last modified: Tue Jul  4 12:15:55 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.98.tar", last modified: Mon Jul 10 16:06:51 2023, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.97.tar` & `helios-opentelemetry-sdk-1.0.98.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.947507 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/eventbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.951507 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-04 12:15:55.000000 helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 12:15:55.955507 helios-opentelemetry-sdk-1.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-04 12:15:25.000000 helios-opentelemetry-sdk-1.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/base_data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/redis_data_obfuscator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/confluent_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/hstest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.97/LICENSE` & `helios-opentelemetry-sdk-1.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/PKG-INFO` & `helios-opentelemetry-sdk-1.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.97
+Version: 1.0.98
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.97/README.md` & `helios-opentelemetry-sdk-1.0.98/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/base_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/data_obfuscator/redis_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/redis_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/span_attribute_dropper/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/helios.py` & `helios-opentelemetry-sdk-1.0.98/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.98/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aio_pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/aws_lambda.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/eventbridge.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/eventbridge.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/confluent_kafka.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/confluent_kafka.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from wrapt import wrap_function_wrapper
 
 from helios.base.span_attributes import SpanAttributes
 from helios.instrumentation.base import HeliosBaseInstrumentor
 from opentelemetry import context, propagate, trace
 from opentelemetry.trace import SpanKind
 from opentelemetry.semconv.trace import MessagingOperationValues
@@ -46,14 +47,18 @@
         return record
     ctx = propagate.extract(record.headers(), getter=_kafka_getter)
 
     with tracer.start_as_current_span(
             "recv", end_on_exit=True, kind=trace.SpanKind.CONSUMER, context=ctx
     ) as span:
         span.set_attribute(SpanAttributes.MESSAGING_PAYLOAD, record.value().decode())
+        timestamp = record.timestamp()
+        if type(timestamp) == tuple and len(timestamp) == 2:
+            timestamp = record.timestamp()[1]
+            span.set_attribute('messaging.queue_time', time.time() * 1000 - timestamp)
         instance._current_consume_span = tracer.start_span(
             name=f"{record.topic()} process",
             kind=SpanKind.CONSUMER,
         )
 
         _enrich_span(
             instance._current_consume_span,
```

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/starlette.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         # process message
 
 API
 ___
 """
 
 import json
+import time
 from logging import getLogger
 from typing import Collection, Optional, List
 
 from opentelemetry.context import attach, detach
 from wrapt import wrap_function_wrapper
 import kafka
 
@@ -131,23 +132,24 @@
 def _create_producer_span(tracer, span_name, topic, partition, value, headers, bootstrap_servers):
     with tracer.start_as_current_span(span_name, kind=trace.SpanKind.PRODUCER) as span:
         _set_span_attributes(span, topic, partition, value, headers, bootstrap_servers)
         span.set_attribute(SpanAttributes.MESSAGING_OPERATION, 'send')
         inject(headers, context=set_span_in_context(span), setter=KafkaContextSetter())
 
 
-def _create_consumer_span(tracer, span_name, topic, partition, value, headers, bootstrap_servers):
+def _create_consumer_span(tracer, span_name, topic, partition, value, headers, timestamp, bootstrap_servers):
     extracted_context = extract(headers, getter=KafkaContextGetter())
     span = tracer.start_span(span_name, context=extracted_context, kind=trace.SpanKind.CONSUMER)
     new_context = trace.set_span_in_context(span, extracted_context)
     token = attach(new_context)
     setattr(span, 'context_token', token)
     with trace.use_span(span):
         _set_span_attributes(span, topic, partition, value, headers, bootstrap_servers)
         span.set_attribute(SpanAttributes.MESSAGING_OPERATION, 'process')
+        span.set_attribute('messaging.queue_time', time.time() * 1000 - timestamp) if timestamp else None
 
 
 def _serialize_payload(value):
     result = value
     value_type = type(value)
     if value_type == dict:
         result = json.dumps(value)
@@ -214,15 +216,15 @@
 
         bootstrap_servers = instance.config.get('bootstrap_servers')
         record = func(*args, **kwargs)
 
         if record:
             try:
                 _create_consumer_span(tracer, CONSUMER_SPAN_NAME, record.topic, record.partition,
-                                      record.value, record.headers, bootstrap_servers)
+                                      record.value, record.headers, record.timestamp, bootstrap_servers)
             except Exception as error:
                 _LOG.debug('kafka __next__ instrumentation error: %s.', error)
 
         return record
 
     def _traced_commit(func, instance, args, kwargs):
         try:
```

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                     producer_partition_0 = True
                 elif span_partition == 1:
                     producer_partition_1 = True
                 else:
                     self.fail(f"partition should be either 0 or 1, but got: {span_partition}")
 
             elif span.kind == SpanKind.CONSUMER:
-                self.assert_consumer_attributes(span_operation, span_headers)
+                self.assert_consumer_attributes(span_operation, span_headers, span.attributes)
                 if span_partition == 0:
                     consumer_partition_0 = True
                 elif span_partition == 1:
                     consumer_partition_1 = True
                 else:
                     self.fail(f"partition should be either 0 or 1, but got: {span_partition}")
 
@@ -186,17 +186,18 @@
             result[header[0]] = value
         return result
 
     def assert_producer_attributes(self, span_operation, span_headers, expected_headers):
         self.assertEqual('send', span_operation)
         self.assertEqual(json.dumps(self.convert_span_headers(expected_headers)), span_headers)
 
-    def assert_consumer_attributes(self, span_operation, span_headers):
+    def assert_consumer_attributes(self, span_operation, span_headers, attributes):
         self.assertEqual('process', span_operation)
         self.assertNotEqual("", span_headers)
         self.assertIsNotNone(span_headers)
+        self.assertIsNotNone(attributes.get('messaging.queue_time'))
 
     def assert_common_attributes(self, span_system, span_topic, span_url, span_payload, expected_payload):
         self.assertEqual('kafka', span_system)
         self.assertEqual(self.topic, span_topic)
         self.assertEqual(json.dumps(self.bootstrap_servers), span_url)
         self.assertEqual(expected_payload, span_payload)
```

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.98/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios/utils.py` & `helios-opentelemetry-sdk-1.0.98/helios/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.97
+Version: 1.0.98
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.98/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.97/setup.py` & `helios-opentelemetry-sdk-1.0.98/setup.py`

 * *Files identical despite different names*

