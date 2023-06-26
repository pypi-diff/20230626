# Comparing `tmp/helios-opentelemetry-sdk-1.0.93.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.93.tar", last modified: Sun Jun 25 09:18:47 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.94.tar", last modified: Mon Jun 26 05:08:34 2023, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.93.tar` & `helios-opentelemetry-sdk-1.0.94.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/base_data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/redis_data_obfuscator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.823553 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/confluent_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.827553 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 05:08:34.000000 helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/hstest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 05:08:34.831553 helios-opentelemetry-sdk-1.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-26 05:07:53.000000 helios-opentelemetry-sdk-1.0.94/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.93/LICENSE` & `helios-opentelemetry-sdk-1.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/PKG-INFO` & `helios-opentelemetry-sdk-1.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.93
+Version: 1.0.94
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.93/README.md` & `helios-opentelemetry-sdk-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/base_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/redis_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/data_obfuscator/redis_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/span_attribute_dropper/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.94/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/helios.py` & `helios-opentelemetry-sdk-1.0.94/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.94/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aio_pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aws_lambda.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/confluent_kafka.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     if span is None or span == INVALID_SPAN:
         span = extract_span_from_exc_info(None if record is None else record.exc_info)
         inject_span_context_to_log_record(record, span)
 
     if span is not None and span != INVALID_SPAN:
         _collect_error_log(record, span)
         ctx = span.get_span_context()
-        if ctx != INVALID_SPAN_CONTEXT:
+        if ctx != INVALID_SPAN_CONTEXT and ctx.trace_flags.sampled:
             # noinspection PyBroadException
             try:
                 _mark_instrumentation_indicator(span)
                 _inject_go_to_helios_url_to_record(record)
                 if type(record.msg) is dict:
                     msg_copy = copy.deepcopy(record.msg)
                     record.msg = _inject_context_to_record_msg(record, msg_copy)
```

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/starlette.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.94/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.94/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.94/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.94/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.94/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios/utils.py` & `helios-opentelemetry-sdk-1.0.94/helios/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.93
+Version: 1.0.94
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.94/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.94/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.93/setup.py` & `helios-opentelemetry-sdk-1.0.94/setup.py`

 * *Files identical despite different names*

