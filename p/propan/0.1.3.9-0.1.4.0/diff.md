# Comparing `tmp/propan-0.1.3.9.tar.gz` & `tmp/propan-0.1.4.0.tar.gz`

## Comparing `propan-0.1.3.9.tar` & `propan-0.1.4.0.tar`

### file list

```diff
@@ -1,171 +1,185 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.3.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.3.9/SECURITY.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.3.9/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/gen_py_code.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/grpc_encoding.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/message.proto
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/grpc/requirements.txt
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.3.9/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__about__.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/__main__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/py.typed
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/types.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/__init__.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/channels.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/info.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/main.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/message.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/security.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/servers.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/subscription.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/utils.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/amqp.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/kafka.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/main.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/nats.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/redis.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/asyncapi/bindings/sqs.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0    11988 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0    12794 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/app.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/main.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/app.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/gen.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/docs/serving.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/nats.py
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/redis.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/sqs.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/test/utils.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/classes.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/functions.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/no_cast.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 propan-0.1.3.9/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.3.9/scripts/test.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.3.9/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.3.9/LICENSE
--rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.3.9/README.md
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 propan-0.1.3.9/pyproject.toml
--rw-r--r--   0        0        0    17672 2020-02-02 00:00:00.000000 propan-0.1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.4.0/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/dependantbot.yml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 propan-0.1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/redis/pattern.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/scheduling/rocketry.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/gen_py_code.sh
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/message.proto
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/protobuf.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/serialization/requirements.txt
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.4.0/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__about__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/__main__.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/_compat.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/py.typed
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/types.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/__init__.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/channels.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/info.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/main.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/message.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/security.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/servers.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/subscription.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/utils.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/amqp.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/kafka.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/main.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/nats.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/redis.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/asyncapi/bindings/sqs.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/routing.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0    12851 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/routing.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/routing.pyi
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     8259 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/routing.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/routing.pyi
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    14261 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/routing.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/routing.pyi
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/routing.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/routing.pyi
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/routing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/routing.pyi
+-rw-r--r--   0        0        0     9544 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12833 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/app.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/main.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/app.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/gen.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/docs/serving.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     7591 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/nats.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/redis.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/sqs.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/test/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/no_cast.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 propan-0.1.4.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 propan-0.1.4.0/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.4.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.4.0/LICENSE
+-rw-r--r--   0        0        0    13471 2020-02-02 00:00:00.000000 propan-0.1.4.0/README.md
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 propan-0.1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 propan-0.1.4.0/PKG-INFO
```

### Comparing `propan-0.1.3.9/CONTRIBUTING.md` & `propan-0.1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/SECURITY.md` & `propan-0.1.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/PULL_REQUEST_TEMPLATE.md` & `propan-0.1.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/ISSUE_TEMPLATE/bug_report.md` & `propan-0.1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/ISSUE_TEMPLATE/config.yml` & `propan-0.1.4.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/workflows/documentation.yml` & `propan-0.1.4.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/workflows/publish_coverage.yml` & `propan-0.1.4.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/workflows/publish_pypi.yml` & `propan-0.1.4.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/.github/workflows/tests.yml` & `propan-0.1.4.0/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        pydantic-version: ["pydantic-v1", "pydantic-v2"]
       fail-fast: false
 
     services:
       rabbitmq:
-        image: rabbitmq
+        image: rabbitmq:alpine
         ports:
           - 5672:5672
       
       kafka:
         image: bitnami/kafka
         ports:
           - 9092:9092
@@ -44,15 +45,15 @@
 
       nats:
         image: nats
         ports:
           - 4222:4222
 
       redis:
-        image: redis
+        image: redis:alpine
         ports:
           - 6379:6379
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
@@ -64,17 +65,23 @@
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[test]
+      - name: Install Pydantic v1
+        if: matrix.pydantic-version == 'pydantic-v1'
+        run: pip install "pydantic>=1.10.0,<2.0.0"
+      - name: Install Pydantic v2
+        if: matrix.pydantic-version == 'pydantic-v2'
+        run: pip install --pre "pydantic>=2.0.0b2,<3.0.0"
       - run: mkdir coverage
       - name: Test
-        run: bash scripts/test.sh -m 'all'
+        run: bash scripts/test.sh -m 'all' -x
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
         uses: actions/upload-artifact@v3
         with:
           name: coverage
```

### Comparing `propan-0.1.3.9/examples/3_lifespan_events.py` & `propan-0.1.4.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/4_cli_attributes_promotion.py` & `propan-0.1.4.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/5_publishing.py` & `propan-0.1.4.0/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/6_arguments_casting.py` & `propan-0.1.4.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/7_handler_errors_processing.py` & `propan-0.1.4.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/1_dependency_injection.py` & `propan-0.1.4.0/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.4.0/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.4.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.4.0/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.4.0/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/dependencies/7_annotated.py` & `propan-0.1.4.0/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/grpc/grpc_encoding.py` & `propan-0.1.4.0/examples/serialization/protobuf.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/quart.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.4.0/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/rabbit/direct.py` & `propan-0.1.4.0/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/rabbit/fanout.py` & `propan-0.1.4.0/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/rabbit/header.py` & `propan-0.1.4.0/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/rabbit/topic.py` & `propan-0.1.4.0/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/redis/direct.py` & `propan-0.1.4.0/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/examples/redis/pattern.py` & `propan-0.1.4.0/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/__about__.py` & `propan-0.1.4.0/propan/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.3.9"
+__version__ = "0.1.4.0"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.3.9/propan/__init__.py` & `propan-0.1.4.0/propan/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # Imports to use at __all__
 from propan import __about__ as about
+from propan.brokers import PropanMessage
 from propan.cli.app import *  # noqa: F403
 from propan.log import *  # noqa: F403
 from propan.utils import *  # noqa: F403
 
 try:
-    from propan.brokers.rabbit import RabbitBroker
+    from propan.brokers.rabbit import RabbitBroker, RabbitRouter
 except ImportError:
-    RabbitBroker = about.INSTALL_RABBIT  # type: ignore
+    RabbitBroker = RabbitRouter = about.INSTALL_RABBIT  # type: ignore
 
 try:
-    from propan.brokers.nats import NatsBroker
+    from propan.brokers.nats import NatsBroker, NatsRouter
 except ImportError:
-    NatsBroker = about.INSTALL_NATS  # type: ignore
+    NatsBroker = NatsRouter = about.INSTALL_NATS  # type: ignore
 
 try:
-    from propan.brokers.redis import RedisBroker
+    from propan.brokers.redis import RedisBroker, RedisRouter
 except ImportError:
-    RedisBroker = about.INSTALL_REDIS  # type: ignore
+    RedisBroker = RedisRouter = about.INSTALL_REDIS  # type: ignore
 
 try:
-    from propan.brokers.kafka import KafkaBroker
+    from propan.brokers.kafka import KafkaBroker, KafkaRouter
 except ImportError:
-    KafkaBroker = about.INSTALL_KAFKA  # type: ignore
+    KafkaBroker = KafkaRouter = about.INSTALL_KAFKA  # type: ignore
 
 try:
-    from propan.brokers.sqs import SQSBroker
+    from propan.brokers.sqs import SQSBroker, SQSRouter
 except ImportError:
-    SQSBroker = about.INSTALL_SQS  # type: ignore
+    SQSBroker = SQSRouter = about.INSTALL_SQS  # type: ignore
 
 assert any(
     (RabbitBroker, NatsBroker, RedisBroker, SQSBroker, KafkaBroker)
 ), about.INSTALL_MESSAGE
 
 __all__ = (  # noqa: F405
     # app
@@ -45,13 +46,23 @@
     ## context
     "context",
     "Context",
     "ContextRepo",
     "Depends",
     # brokers
     "PropanMessage",
+    ## nats
     "NatsBroker",
+    "NatsRouter",
+    ## rabbit
     "RabbitBroker",
+    "RabbitRouter",
+    ## redis
     "RedisBroker",
+    "RedisRouter",
+    ## kafka
+    "KafkaRouter",
     "KafkaBroker",
+    ## sqs
     "SQSBroker",
+    "SQSRouter",
 )
```

### Comparing `propan-0.1.3.9/propan/annotations.py` & `propan-0.1.4.0/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/types.py` & `propan-0.1.4.0/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/__init__.py` & `propan-0.1.4.0/propan/asyncapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/channels.py` & `propan-0.1.4.0/propan/asyncapi/channels.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/info.py` & `propan-0.1.4.0/propan/asyncapi/info.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/main.py` & `propan-0.1.4.0/propan/asyncapi/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseModel, Field
 
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.info import AsyncAPIInfo
 from propan.asyncapi.message import AsyncAPIMessage
 from propan.asyncapi.servers import AsyncAPIServer
 from propan.asyncapi.utils import AsyncAPIExternalDocs, AsyncAPITag
-from propan.brokers._model import ContentTypes
+from propan.brokers._model.utils import ContentTypes
 from propan.types import AnyDict
 
 ASYNC_API_VERSION = "2.6.0"
 
 
 class AsyncAPIComponents(BaseModel):
     # TODO
```

### Comparing `propan-0.1.3.9/propan/asyncapi/message.py` & `propan-0.1.4.0/propan/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/security.py` & `propan-0.1.4.0/propan/asyncapi/security.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/subscription.py` & `propan-0.1.4.0/propan/asyncapi/subscription.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/bindings/amqp.py` & `propan-0.1.4.0/propan/asyncapi/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/bindings/kafka.py` & `propan-0.1.4.0/propan/asyncapi/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/bindings/main.py` & `propan-0.1.4.0/propan/asyncapi/bindings/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/asyncapi/bindings/redis.py` & `propan-0.1.4.0/propan/asyncapi/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/push_back_watcher.py` & `propan-0.1.4.0/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/_model/broker_usecase.py` & `propan-0.1.4.0/propan/brokers/_model/broker_usecase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import warnings
 from abc import ABC, abstractmethod
 from functools import wraps
 from itertools import chain
 from typing import (
     Any,
     Awaitable,
     Callable,
@@ -14,19 +15,21 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
 )
 
+from fast_depends._compat import PYDANTIC_V2
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import Depends
 from fast_depends.utils import args_to_kwargs
 from typing_extensions import ParamSpec, Self, TypeAlias, TypeVar
 
+from propan.brokers._model.routing import BrokerRouter
 from propan.brokers._model.schemas import BaseHandler, PropanMessage
 from propan.brokers._model.utils import (
     ContentType,
     ContentTypes,
     change_logger_handlers,
     get_watcher,
     set_message_context,
@@ -62,23 +65,20 @@
 ]
 
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
-def WRAPPED_BUILDER(path: str, call: Callable[P, R]) -> CallModel[P, R]:
-    return build_call_model(call)
-
-
 class BrokerUsecase(ABC, Generic[MsgType, ConnectionType]):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: Sequence[BaseHandler]
     dependencies: Sequence[Depends]
+    started: bool
     _global_parser: CustomParser[MsgType]
     _global_decoder: CustomDecoder[MsgType]
     _connection: Optional[ConnectionType]
     _fmt: Optional[str]
 
     def __init__(
         self,
@@ -113,14 +113,15 @@
 
         context.set_global("logger", logger)
         context.set_global("broker", self)
 
         self.protocol = protocol
         self.protocol_version = protocol_version
         self.url = url_
+        self.started = False
 
     async def connect(self, *args: Any, **kwargs: Any) -> ConnectionType:
         if self._connection is None:
             arguments = get_function_positional_arguments(self.__init__)  # type: ignore
             init_kwargs = args_to_kwargs(
                 arguments,
                 *self._connection_args,
@@ -146,15 +147,15 @@
         raise_timeout: bool = False,
         **kwargs: Any,
     ) -> Optional[DecodedMessage]:
         raise NotImplementedError()
 
     @abstractmethod
     async def close(self) -> None:
-        raise NotImplementedError()
+        self.started = False
 
     @abstractmethod
     async def _parse_message(self, message: MsgType) -> PropanMessage[MsgType]:
         raise NotImplementedError()
 
     @abstractmethod
     def _process_message(
@@ -170,30 +171,35 @@
         **kwargs: Dict[str, str],
     ) -> Dict[str, Any]:
         return {
             "message_id": message.message_id[:10] if message else "",
         }
 
     @abstractmethod
-    def handle(
+    def handle(  # type: ignore[return]
         self,
         *broker_args: Any,
         retry: Union[bool, int] = False,
         dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
         parse_message: CustomParser[MsgType] = None,
         description: str = "",
         _raw: bool = False,
         _get_dependant: Callable[
-            ...,
-            CallModel,
-        ] = WRAPPED_BUILDER,
+            [Union[Callable[..., T], Callable[..., Awaitable[T]]]], CallModel
+        ] = build_call_model,
         **broker_kwargs: Any,
     ) -> HandlerWrapper:
-        raise NotImplementedError()
+        if self.started:
+            warnings.warn(
+                "You are trying to register `handler` with already running broker\n"  # noqa: E501
+                "It has no effect until broker restarting.",  # noqa: E501
+                category=RuntimeWarning,
+                stacklevel=1,
+            )
 
     @staticmethod
     async def _decode_message(message: PropanMessage[MsgType]) -> DecodedMessage:
         body = message.body
         m: DecodedMessage = body
         if message.content_type is not None:
             if ContentTypes.text.value in message.content_type:
@@ -207,14 +213,16 @@
         return to_send(msg)
 
     @property
     def fmt(self) -> str:  # pragma: no cover
         return self._fmt or ""
 
     async def start(self) -> None:
+        self.started = True
+
         if self.logger is not None:
             change_logger_handlers(self.logger, self.fmt)
 
         await self.connect()
 
     async def __aenter__(self) -> Self:
         await self.connect()
@@ -227,35 +235,43 @@
         self,
         func: Union[Callable[..., T], Callable[..., Awaitable[T]]],
         retry: Union[bool, int] = False,
         extra_dependencies: Sequence[Depends] = (),
         decode_message: CustomDecoder[MsgType] = None,
         parse_message: CustomParser[MsgType] = None,
         _raw: bool = False,
-        _get_dependant: Callable[..., CallModel] = WRAPPED_BUILDER,
+        _get_dependant: Callable[
+            [Union[Callable[..., T], Callable[..., Awaitable[T]]]], CallModel
+        ] = build_call_model,
         **broker_log_context_kwargs: Any,
     ) -> Tuple[Callable[[MsgType, bool], Awaitable[Optional[T]]], CallModel]:
-        dependant = _get_dependant(path="", call=func)
+        dependant = _get_dependant(func)
         extra = [
-            _get_dependant(path="", call=d.dependency)
+            _get_dependant(d.dependency)
             for d in chain(extra_dependencies, self.dependencies)
         ]
 
         extend_dependencies(extra)(dependant)
 
         if getattr(dependant, "flat_params", None) is None:  # handle FastAPI Dependant
-            params = dependant.path_params + dependant.body_params
+            params = dependant.query_params + dependant.body_params
 
             for d in dependant.dependencies:
-                params.extend(d.path_params + d.body_params)
+                params.extend(d.query_params + d.body_params)
 
-            params_unique = []
+            params_unique = {}
+            params_names = set()
             for p in params:
-                if p not in params_unique:
-                    params_unique.append(p)
+                if p.name not in params_names:
+                    params_names.add(p.name)
+                    if PYDANTIC_V2:
+                        params_unique[p.name] = p.field_info
+                    else:
+                        # TODO: remove it from with stable PydanticV2
+                        params_unique[p.name] = p
 
             dependant.flat_params = params_unique
 
         f = cast(Callable[..., Awaitable[T]], to_async(func))
 
         if self._is_apply_types is True:
             f = apply_types(
@@ -283,14 +299,18 @@
             parser=parse_message or self._global_parser,
         )
 
         f = set_message_context(f)
 
         return suppress_decor(f), dependant
 
+    def include_router(self, router: BrokerRouter) -> None:
+        for r in router.handlers:
+            self.handle(*r.args, **r.kwargs)(r.call)
+
     def _wrap_decode_message(
         self,
         func: Callable[..., Awaitable[T]],
         decoder: CustomDecoder[MsgType],
         params: Sequence[Any] = (),
         _raw: bool = False,
     ) -> Callable[[PropanMessage[MsgType]], Awaitable[T]]:
```

### Comparing `propan-0.1.3.9/propan/brokers/_model/schemas.py` & `propan-0.1.4.0/propan/brokers/_model/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any, Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
 from fast_depends.core import CallModel
 from pydantic import BaseModel, Field, Json, create_model
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 
+from propan._compat import get_model_fileds, model_schema, update_model_example
 from propan.asyncapi.channels import AsyncAPIChannel
-from propan.asyncapi.utils import add_example_to_model
 from propan.types import AnyDict, DecodedMessage, DecoratedCallable
 
 
 @dataclass
 class BaseHandler:
     callback: DecoratedCallable
     dependant: CallModel
@@ -43,33 +43,33 @@
     def get_message_object(self) -> Tuple[str, AnyDict, Optional[AnyDict]]:
         import jsonref  # hide it there to remove docs dependencies from main package
 
         dependant = self.dependant
 
         if getattr(dependant, "response_model", None) is not None:
             response_model: Type[BaseModel] = dependant.response_model
-            return_field = list(response_model.__fields__.values())[0]
+            return_field = list(get_model_fileds(response_model).values())[0]
 
             if (
                 return_field.annotation != Any  # NOTE: 3.7-3.10 compatibility
                 and issubclass(return_field.annotation, BaseModel)
             ):
-                response_model = add_example_to_model(return_field.annotation)
+                response_model = update_model_example(return_field.annotation)
 
                 return_info = jsonref.replace_refs(
-                    response_model.schema(), jsonschema=True, proxies=False
+                    model_schema(response_model), jsonschema=True, proxies=False
                 )
                 return_info["examples"] = [return_info.pop("example", None)]
 
             else:
-                response_model = add_example_to_model(response_model)
+                response_model = update_model_example(response_model)
                 response_field_name = "response"
 
                 raw = jsonref.replace_refs(
-                    response_model.schema(),
+                    model_schema(response_model),
                     jsonschema=True,
                     proxies=False,
                 )
 
                 return_info = raw.get("properties", {}).get(response_field_name)
                 return_info["examples"] = [
                     raw.pop("example", {}).get(response_field_name)
@@ -111,16 +111,18 @@
                 },
             )
 
         body: AnyDict
         if model is None:
             body = {"title": payload_title, "type": "null"}
         else:
-            model = add_example_to_model(model)
-            body = jsonref.replace_refs(model.schema(), jsonschema=True, proxies=False)
+            model = update_model_example(model)
+            body = jsonref.replace_refs(
+                model_schema(model), jsonschema=True, proxies=False
+            )
 
         body.pop("definitions", None)
         if return_info is not None:
             return_info.pop("definitions", None)
 
         if params_number == 1 and not use_original_model:
             param_body: AnyDict = body.get("properties", {})
```

### Comparing `propan-0.1.3.9/propan/brokers/_model/utils.py` & `propan-0.1.4.0/propan/brokers/_model/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import json
 import logging
 from enum import Enum
 from functools import wraps
 from typing import Awaitable, Callable, Optional, Tuple, TypeVar, Union
 
-from pydantic.json import pydantic_encoder
 from typing_extensions import TypeAlias
 
+from propan._compat import dump_json
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.types import SendableMessage
 from propan.utils import context
@@ -29,16 +28,19 @@
 def to_send(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
     if msg is None:
         return b"", None
 
     if isinstance(msg, bytes):
         return msg, None
 
+    if isinstance(msg, str):
+        return msg.encode(), ContentTypes.text.value
+
     return (
-        json.dumps(msg, default=pydantic_encoder).encode(),
+        dump_json(msg).encode(),
         ContentTypes.json.value,
     )
 
 
 def change_logger_handlers(logger: logging.Logger, fmt: str) -> None:
     for handler in logger.handlers:
         formatter = handler.formatter
```

### Comparing `propan-0.1.3.9/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.4.0/propan/brokers/kafka/kafka_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
                 "sasl_oauth_token_provider",
             }
             and v
         }
         return partial(AIOKafkaConsumer, **consumer_kwargs)
 
     async def close(self) -> None:
+        await super().close()
+
         for f in self.response_callbacks.values():
             f.cancel()
         self.response_callbacks = {}
 
         for handler in self.handlers:
             if handler.task is not None:
                 handler.task.cancel()
@@ -161,14 +163,16 @@
             "read_committed",
         ] = "read_uncommitted",
         ## broker
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> Wrapper:
+        super().handle()
+
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             for t in topics:
                 self.__max_topic_len = max((self.__max_topic_len, len(t)))
 
             func, dependant = self._wrap_handler(
                 func,
                 extra_dependencies=dependencies,
```

### Comparing `propan-0.1.3.9/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.4.0/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/kafka/schemas.py` & `propan-0.1.4.0/propan/brokers/kafka/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/nats/nats_broker.py` & `propan-0.1.4.0/propan/brokers/nats/nats_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         subject: str,
         queue: str = "",
         *,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> Callable[[DecoratedCallable], None]:
+        super().handle()
+
         self.__max_subject_len = max((self.__max_subject_len, len(subject)))
         self.__max_queue_len = max((self.__max_queue_len, len(queue)))
 
         def wrapper(func: DecoratedCallable) -> None:
             func, dependant = self._wrap_handler(
                 func,
                 queue=queue,
@@ -185,14 +187,15 @@
                 if raise_timeout is True:
                     raise e
                 return None
             else:
                 return await self._decode_message(await self._parse_message(msg))
 
     async def close(self) -> None:
+        await super().close()
         for h in self.handlers:
             if h.subscription is not None:
                 await h.subscription.unsubscribe()
                 h.subscription = None
 
         if self._connection is not None:
             await self._connection.drain()
```

### Comparing `propan-0.1.3.9/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.4.0/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.4.0/propan/brokers/nats/nats_js_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # type: ignore
 from functools import wraps
 from typing import Any, Awaitable, Callable, Optional, TypeVar
 
 import nats
 from nats.js.client import JetStreamContext
 
+from propan._compat import model_to_dict
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.nats_broker import NatsBroker
 from propan.brokers.nats.schemas import JetStream
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.types import AnyDict
 
 T = TypeVar("T")
@@ -25,15 +26,15 @@
 
     async def _connect(self, *args: Any, **kwargs: AnyDict) -> JetStreamContext:
         assert self._js
 
         nc = await nats.connect(*args, **kwargs)
 
         stream = await nc.jetstream(
-            **self._js.dict(include={"prefix", "domain", "timeout"})
+            **model_to_dict(self._js, include={"prefix", "domain", "timeout"})
         )
 
         return stream
 
     @staticmethod
     def _process_message(
         func: Callable[[PropanMessage], Awaitable[T]],
```

### Comparing `propan-0.1.3.9/propan/brokers/nats/schemas.py` & `propan-0.1.4.0/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import warnings
 from contextlib import asynccontextmanager
 from functools import wraps
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
@@ -20,14 +19,15 @@
 import aio_pika
 import aiormq
 from aio_pika.abc import DeliveryMode
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 from yarl import URL
 
+from propan._compat import model_to_dict
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, HandlerWrapper, SendableMessage
 from propan.utils import context
 
@@ -75,14 +75,15 @@
 
         self.__max_queue_len = 4
         self.__max_exchange_len = 4
         self._queues = {}
         self._exchanges = {}
 
     async def close(self) -> None:
+        await super().close()
         if self._channel is not None:
             await self._channel.close()
             self._channel = None
 
         if self._connection is not None:
             await self._connection.close()
             self._connection = None
@@ -114,14 +115,16 @@
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
+        super().handle()
+
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
             func, dependant = self._wrap_handler(
                 func,
@@ -240,32 +243,32 @@
                 arguments=handler.queue.bind_arguments,
             )
         return queue
 
     async def declare_queue(self, queue: RabbitQueue) -> aio_pika.RobustQueue:
         q = self._queues.get(queue)
         if q is None:
-            q = await self._channel.declare_queue(**queue.dict())
+            q = await self._channel.declare_queue(**model_to_dict(queue))
             self._queues[queue] = q
         return q
 
     async def declare_exchange(
         self, exchange: RabbitExchange
     ) -> aio_pika.RobustExchange:
         exch = self._exchanges.get(exchange)
 
         if exch is None:
-            exch = await self._channel.declare_exchange(**exchange.dict())
+            exch = await self._channel.declare_exchange(**model_to_dict(exchange))
             self._exchanges[exchange] = exch
 
             current = exchange
             current_exch = exch
             while current.bind_to is not None:
                 parent_exch = await self._channel.declare_exchange(
-                    **current.bind_to.dict()
+                    **model_to_dict(current.bind_to)
                 )
                 await current_exch.bind(
                     exchange=parent_exch,
                     routing_key=current.routing_key,
                     arguments=current.bind_arguments,
                 )
                 current = current.bind_to
@@ -296,15 +299,15 @@
             "- %(message)s"
         )
 
     @staticmethod
     async def _parse_message(
         message: aio_pika.message.IncomingMessage,
     ) -> RabbitMessage:
-        return RabbitMessage(
+        return PropanMessage(
             body=message.body,
             headers=message.headers,
             reply_to=message.reply_to or "",
             message_id=message.message_id,
             content_type=message.content_type or "",
             raw_message=message,
         )
@@ -381,65 +384,14 @@
         if queue is not None:  # pragma: no branch
             self.__max_queue_len = max(self.__max_queue_len, len(queue.name))
 
     @property
     def channel(self) -> aio_pika.RobustChannel:
         return self._channel
 
-    async def _init_queue(
-        self,
-        queue: RabbitQueue,
-    ) -> aio_pika.abc.AbstractRobustQueue:
-        warnings.warn(
-            "The `_init_queue` method is deprecated, "  # noqa: E501
-            "and will be removed in version 1.4.0. "  # noqa: E501
-            "Use `declare_queue` instead.",  # noqa: E501
-            category=DeprecationWarning,
-            stacklevel=1,
-        )
-        q = self._queues.get(queue)
-        if q is None:
-            q = await self._channel.declare_queue(**queue.dict())
-            self._queues[queue] = q
-        return q
-
-    async def _init_exchange(
-        self,
-        exchange: RabbitExchange,
-    ) -> aio_pika.abc.AbstractRobustExchange:
-        warnings.warn(
-            "The `_init_exchange` method is deprecated, "  # noqa: E501
-            "and will be removed in version 1.4.0. "  # noqa: E501
-            "Use `declare_exchange` instead.",  # noqa: E501
-            category=DeprecationWarning,
-            stacklevel=1,
-        )
-
-        exch = self._exchanges.get(exchange)
-
-        if exch is None:
-            exch = await self._channel.declare_exchange(**exchange.dict())
-            self._exchanges[exchange] = exch
-
-            current = exchange
-            current_exch = exch
-            while current.bind_to is not None:
-                parent_exch = await self._channel.declare_exchange(
-                    **current.bind_to.dict()
-                )
-                await current_exch.bind(
-                    exchange=parent_exch,
-                    routing_key=current.routing_key,
-                    arguments=current.bind_arguments,
-                )
-                current = current.bind_to
-                current_exch = parent_exch
-
-        return exch
-
 
 def _validate_exchange(
     exchange: Union[str, RabbitExchange, None] = None,
 ) -> Optional[RabbitExchange]:
     if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
             exchange = RabbitExchange(name=exchange)
```

### Comparing `propan-0.1.3.9/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.4.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/rabbit/schemas.py` & `propan-0.1.4.0/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/redis/redis_broker.py` & `propan-0.1.4.0/propan/brokers/redis/redis_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from uuid import uuid4
 
 from fast_depends.dependencies import Depends
 from redis.asyncio.client import PubSub, Redis
 from redis.asyncio.connection import ConnectionPool, parse_url
 from typing_extensions import TypeAlias
 
+from propan._compat import model_parse, model_to_json
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage, RawDecoced
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler
 from propan.brokers.redis.schemas import RedisMessage as RM
 from propan.types import (
     AnyCallable,
@@ -70,14 +71,15 @@
     ) -> Redis:
         url_options = parse_url(url)
         url_options.update(kwargs)
         pool = ConnectionPool(**url_options)
         return Redis(connection_pool=pool)
 
     async def close(self) -> None:
+        await super().close()
         for h in self.handlers:
             if h.task is not None:  # pragma: no branch
                 h.task.cancel()
                 h.task = None
 
             if h.subscription is not None:  # pragma: no branch
                 await h.subscription.unsubscribe()
@@ -110,14 +112,16 @@
         channel: str = "",
         *,
         pattern: bool = False,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
+        super().handle()
+
         self.__max_channel_len = max(self.__max_channel_len, len(channel))
 
         def wrapper(func: AnyCallable) -> DecoratedCallable:
             func, dependant = self._wrap_handler(
                 func,
                 channel=channel,
                 extra_dependencies=dependencies,
@@ -189,22 +193,24 @@
             callback_channel = reply_to
             psub = None
             response_queue = None
             task = None
 
         await self._connection.publish(
             channel,
-            RM(
-                data=msg,
-                headers={
-                    "content-type": content_type or "",
-                    **(headers or {}),
-                },
-                reply_to=callback_channel,
-            ).json(),
+            model_to_json(
+                RM(
+                    data=msg,
+                    headers={
+                        "content-type": content_type or "",
+                        **(headers or {}),
+                    },
+                    reply_to=callback_channel,
+                )
+            ),
         )
 
         if psub and response_queue and task:
             try:
                 response = await asyncio.wait_for(
                     response_queue.get(), callback_timeout
                 )
@@ -216,19 +222,19 @@
                 return await self._decode_message(await self._parse_message(response))
             finally:
                 await psub.unsubscribe(callback_channel)
                 await psub.reset()
                 task.cancel()
 
     @staticmethod
-    async def _parse_message(message: AnyCallable) -> RedisMessage:
+    async def _parse_message(message: Any) -> RedisMessage:
         data = message.get("data", b"")
 
         try:
-            obj = RM.parse_raw(data)
+            obj = model_parse(RM, data)
         except Exception:
             msg = RedisMessage(
                 body=data,
                 raw_message=message,
             )
         else:
             msg = RedisMessage(
```

### Comparing `propan-0.1.3.9/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.4.0/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/redis/schemas.py` & `propan-0.1.4.0/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/brokers/sqs/schema.py` & `propan-0.1.4.0/propan/brokers/sqs/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import field as DField
 from typing import Any, Dict, Optional, Sequence
 
 from fast_depends.core import CallModel
 from pydantic import BaseModel, Field, PositiveInt
 from typing_extensions import Literal
 
+from propan._compat import model_to_dict
 from propan.asyncapi.bindings import (
     AsyncAPIChannelBinding,
     AsyncAPIOperationBinding,
     sqs,
 )
 from propan.asyncapi.channels import AsyncAPIChannel
 from propan.asyncapi.message import AsyncAPICorrelationId, AsyncAPIMessage
@@ -248,15 +249,15 @@
                             location="$message.header#/correlation_id"
                         ),
                         payload=body,
                     ),
                 ),
                 bindings=AsyncAPIChannelBinding(
                     sqs=sqs.AsyncAPISQSChannelBinding(
-                        queue=self.queue.dict(include={"name", "fifo"}),
+                        queue=model_to_dict(self.queue, include={"name", "fifo"}),
                     )
                 ),
             ),
         }
 
 
 @dataclass
```

### Comparing `propan-0.1.3.9/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.4.0/propan/brokers/sqs/sqs_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from uuid import uuid4
 
 from aiobotocore.client import AioBaseClient
 from aiobotocore.session import get_session
 from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias
 
+from propan._compat import model_to_dict
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.exceptions import SkipMessage
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     NotPushBackWatcher,
     WatcherContext,
@@ -82,14 +83,15 @@
             service_name="sqs", endpoint_url=url, **kwargs
         )
         context.set_global("client", client)
         await client.__aenter__()
         return client
 
     async def close(self) -> None:
+        await super().close()
         for f in self.response_callbacks.values():
             f.cancel()
         self.response_callbacks = {}
 
         for h in self.handlers:
             if h.task is not None:
                 h.task.cancel()
@@ -156,14 +158,16 @@
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         dependencies: Sequence[Depends] = (),
         description: str = "",
         **original_kwargs: AnyDict,
     ) -> HandlerWrapper:
+        super().handle()
+
         if isinstance(queue, str):
             queue = SQSQueue(queue)
 
         self.__max_queue_len = max((self.__max_queue_len, len(queue.name)))
 
         params = {
             "WaitTimeSeconds": wait_interval,
@@ -288,15 +292,16 @@
         url = self._queues.get(queue.name)
         if url is None:  # pragma: no branch
             url = (
                 await self._connection.create_queue(
                     QueueName=queue.name,
                     Attributes={
                         i: str(j)
-                        for i, j in queue.dict(
+                        for i, j in model_to_dict(
+                            queue,
                             exclude={"name"},
                             by_alias=True,
                             exclude_defaults=True,
                             exclude_unset=True,
                         ).items()
                     },
                     tags=queue.tags,
```

### Comparing `propan-0.1.3.9/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.4.0/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/app.py` & `propan-0.1.4.0/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/main.py` & `propan-0.1.4.0/propan/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     app_level: int = logging.INFO,
 ) -> None:
     propan_app = try_import_propan(module, app)
     set_log_level(log_level, propan_app)
 
     propan_app._command_line_options = extra_options
 
-    if sys.platform not in ("win32", "cygwin", "cli"):
+    if sys.platform not in ("win32", "cygwin", "cli"):  # pragma: no cover
         try:
             import uvloop
-        except Exception:
+        except ImportError:
             logger.warning("You have no installed `uvloop`")
         else:
             uvloop.install()
 
     asyncio.run(propan_app.run(log_level=app_level))
```

### Comparing `propan-0.1.3.9/propan/cli/docs/app.py` & `propan-0.1.4.0/propan/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/docs/gen.py` & `propan-0.1.4.0/propan/cli/docs/gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import json
 from io import StringIO
 from pathlib import Path
 from typing import Any, Dict, cast
 
 import typer
 
+from propan._compat import model_to_jsonable
 from propan.asyncapi import (
     AsyncAPIChannel,
     AsyncAPIComponents,
     AsyncAPIInfo,
     AsyncAPIMessage,
     AsyncAPISchema,
     AsyncAPIServer,
@@ -50,19 +50,18 @@
     yaml.dump(schema, io, sort_keys=False)
     return io.getvalue()
 
 
 def schema_to_json(schema: AsyncAPISchema) -> AnyDict:
     return cast(
         AnyDict,
-        json.loads(
-            schema.json(
-                by_alias=True,
-                exclude_none=True,
-            )
+        model_to_jsonable(
+            schema,
+            by_alias=True,
+            exclude_none=True,
         ),
     )
 
 
 def get_app_schema(app: PropanApp) -> AsyncAPISchema:
     if not isinstance(app.broker, BrokerUsecase):
         raise typer.BadParameter("Your PropanApp broker is invalid")
```

### Comparing `propan-0.1.3.9/propan/cli/docs/serving.py` & `propan-0.1.4.0/propan/cli/docs/serving.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/startproject/core.py` & `propan-0.1.4.0/propan/cli/startproject/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         config_dir / "settings.py",
         "from pathlib import Path",
         "from typing import Optional",
         "",
         "from pydantic import BaseModel, Field",
         "from pydantic_settings import BaseSettings"
         if PYDANTIC_V2
-        else "from pydantic import BaseSettings",
+        else "from pydantic import BaseSettings",  # TODO: remove it from with stable PydanticV2
         "",
         "",
         "CONFIG_DIR = Path(__file__).resolve().parent",
         "BASE_DIR = CONFIG_DIR.parent",
         "",
         "",
         *broker_settings,
@@ -115,40 +115,22 @@
         "    else:",
         "        settings = Settings()",
         "    return settings",
     )
 
     write_file(
         config_dir / "__init__.py",
-        "from .settings import Settings, init_settings",
+        "from config.settings import Settings, init_settings",
     )
 
     return config_dir
 
 
-def create_core_dir(core: Path, broker_class: str) -> Path:
-    core_dir = touch_dir(core)
-
-    write_file(
-        core_dir / "__init__.py",
-        "from .dependencies import broker",
-    )
-
-    write_file(
-        core_dir / "dependencies.py",
-        f"from propan import {broker_class}",
-        "",
-        f"broker = {broker_class}()",
-    )
-
-    return core_dir
-
-
 def create_apps_dir(apps: Path) -> Path:
     apps_dir = touch_dir(apps)
 
     write_file(
         apps_dir / "__init__.py",
-        "from .handlers import *",
+        "from apps.handlers import router",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.3.9/propan/cli/startproject/async_app/app.py` & `propan-0.1.4.0/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.4.0/propan/cli/startproject/async_app/kafka.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from pathlib import Path
 
-from propan.cli.startproject.async_app.core import create_app_file
+from propan.cli.startproject.async_app.core import create_app_file, create_handlers_file
 from propan.cli.startproject.core import (
     create_apps_dir,
     create_config_dir,
-    create_core_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
 def create_kafka(dir: Path) -> Path:
     project_dir = _create_project_dir(dir)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
-    _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path) -> Path:
     project_dir = create_project_dir(dirname, "propan[async-kafka]")
 
@@ -65,28 +63,16 @@
 
 def _create_config_dir(config: Path) -> Path:
     config_dir = create_config_dir(config)
     create_env(config_dir, "localhost:9092")
     return config_dir
 
 
-def _create_core_dir(core: Path) -> Path:
-    core_dir = create_core_dir(core, "KafkaBroker")
-    return core_dir
-
-
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
-    write_file(
+    create_handlers_file(
         apps_dir / "handlers.py",
-        "from propan.annotations import Logger",
-        "",
-        "from core import broker",
-        "",
-        "",
-        "@broker.handle('test')",
-        "async def base_handler(body: dict, logger: Logger):",
-        "    logger.info(body)",
+        "KafkaRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.3.9/propan/cli/startproject/async_app/nats.py` & `propan-0.1.4.0/propan/cli/startproject/async_app/rabbit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,76 @@
 from pathlib import Path
 
-from propan.cli.startproject.async_app.core import create_app_file
+from propan.cli.startproject.async_app.core import create_app_file, create_handlers_file
 from propan.cli.startproject.core import (
     create_apps_dir,
     create_config_dir,
-    create_core_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
-def create_nats(dir: Path) -> Path:
+def create_rabbit(dir: Path) -> Path:
     project_dir = _create_project_dir(dir)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
-    _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path) -> Path:
-    project_dir = create_project_dir(dirname, "propan[async-nats]")
+    project_dir = create_project_dir(dirname, "propan[async-rabbit]")
 
     write_file(
         project_dir / "docker-compose.yaml",
         'version: "3"',
         "",
         "services:",
-        "  nats:",
-        "    image: nats",
+        "  rabbit:",
+        "    image: rabbitmq",
+        "    environment:",
+        "      RABBITMQ_DEFAULT_USER: guest",
+        "      RABBITMQ_DEFAULT_PASS: guest",
+        "    healthcheck:",
+        "      test: rabbitmq-diagnostics -q ping",
+        "      interval: 3s",
+        "      timeout: 30s",
+        "      retries: 3",
         "    ports:",
-        "      - 4222:4222",
-        "      - 8222:8222  # management",
+        "      - 5672:5672",
         "",
         "  app:",
         "    build: .",
         "    environment:",
-        "      APP_BROKER__URL: nats://nats:4222/",
+        "      APP_BROKER__URL: amqp://guest:guest@rabbit:5672/",
         "    volumes:",
         "      - ./app:/home/user/app:ro",
         "    depends_on:",
-        "      - nats",
+        "      rabbit:",
+        "        condition: service_healthy",
     )
 
     return project_dir
 
 
 def _create_app_dir(app: Path) -> Path:
     app_dir = touch_dir(app)
-    create_app_file(app_dir, "NatsBroker")
+    create_app_file(app_dir, "RabbitBroker")
     return app_dir
 
 
 def _create_config_dir(config: Path) -> Path:
     config_dir = create_config_dir(config)
-    create_env(config_dir, "nats://localhost:4222/")
+    create_env(config_dir, "amqp://guest:guest@localhost:5672/")
     return config_dir
 
 
-def _create_core_dir(core: Path) -> Path:
-    core_dir = create_core_dir(core, "NatsBroker")
-    return core_dir
-
-
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
-    write_file(
+    create_handlers_file(
         apps_dir / "handlers.py",
-        "from propan.annotations import Logger",
-        "",
-        "from core import broker",
-        "",
-        "",
-        "@broker.handle('test')",
-        "async def base_handler(body: dict, logger: Logger):",
-        "    logger.info(body)",
+        "RabbitRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.3.9/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.4.0/propan/cli/startproject/async_app/sqs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 from pathlib import Path
 
-from propan.cli.startproject.async_app.core import create_app_file
+from propan.cli.startproject.async_app.core import create_app_file, create_handlers_file
 from propan.cli.startproject.core import (
     create_apps_dir,
     create_config_dir,
-    create_core_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
-def create_rabbit(dir: Path) -> Path:
+def create_sqs(dir: Path) -> Path:
     project_dir = _create_project_dir(dir)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
-    _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path) -> Path:
-    project_dir = create_project_dir(dirname, "propan[async-rabbit]")
+    project_dir = create_project_dir(dirname, "propan[async-redis]")
 
     write_file(
         project_dir / "docker-compose.yaml",
         'version: "3"',
         "",
         "services:",
-        "  rabbit:",
-        "    image: rabbitmq",
-        "    environment:",
-        "      RABBITMQ_DEFAULT_USER: guest",
-        "      RABBITMQ_DEFAULT_PASS: guest",
-        "    healthcheck:",
-        "      test: rabbitmq-diagnostics -q ping",
-        "      interval: 3s",
-        "      timeout: 30s",
-        "      retries: 3",
+        "  sqs:",
+        "    image: softwaremill/elasticmq-native",
         "    ports:",
-        "      - 5672:5672",
+        "      - 9324:9324",
+        "      - 9325:9325  # management",
         "",
         "  app:",
         "    build: .",
         "    environment:",
-        "      APP_BROKER__URL: amqp://guest:guest@rabbit:5672/",
+        "      APP_BROKER__URL: http://sqs:9324/",
         "    volumes:",
         "      - ./app:/home/user/app:ro",
         "    depends_on:",
-        "      rabbit:",
-        "        condition: service_healthy",
+        "      - sqs",
     )
 
     return project_dir
 
 
 def _create_app_dir(app: Path) -> Path:
     app_dir = touch_dir(app)
-    create_app_file(app_dir, "RabbitBroker")
+    create_app_file(
+        app_dir,
+        "SQSBroker",
+        imports=(
+            "from botocore import UNSIGNED",
+            "from aiobotocore.config import AioConfig",
+        ),
+        broker_init=(
+            "    if settings.debug is True:",
+            "        config = AioConfig(signature_version=UNSIGNED)",
+            "    else:",
+            "        config = None",
+            "",
+            "    await broker.connect(",
+            "        settings.broker.url,",
+            "        region_name=settings.broker.region,",
+            "        config=config,",
+            "    )",
+        ),
+    )
     return app_dir
 
 
 def _create_config_dir(config: Path) -> Path:
-    config_dir = create_config_dir(config)
-    create_env(config_dir, "amqp://guest:guest@localhost:5672/")
+    config_dir = create_config_dir(
+        config,
+        "class BrokerSettings(BaseModel):",
+        "    url: str = Field(...)",
+        '    region: str = "us-west-2"',
+    )
+    create_env(config_dir, "http://localhost:9324/")
     return config_dir
 
 
-def _create_core_dir(core: Path) -> Path:
-    core_dir = create_core_dir(core, "RabbitBroker")
-    return core_dir
-
-
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
-    write_file(
+    create_handlers_file(
         apps_dir / "handlers.py",
-        "from propan.annotations import Logger",
-        "",
-        "from core import broker",
-        "",
-        "from propan.brokers.rabbit import RabbitQueue, RabbitExchange",
-        "",
-        "",
-        '@broker.handle(queue=RabbitQueue("test"),',
-        '               exchange=RabbitExchange("test"))',
-        "async def base_handler(body: dict, logger: Logger):",
-        "    logger.info(body)",
+        "SQSRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.3.9/propan/cli/startproject/async_app/redis.py` & `propan-0.1.4.0/propan/cli/startproject/async_app/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from pathlib import Path
 
-from propan.cli.startproject.async_app.core import create_app_file
+from propan.cli.startproject.async_app.core import create_app_file, create_handlers_file
 from propan.cli.startproject.core import (
     create_apps_dir,
     create_config_dir,
-    create_core_dir,
     create_env,
     create_project_dir,
 )
 from propan.cli.startproject.utils import touch_dir, write_file
 
 
 def create_redis(dir: Path) -> Path:
     project_dir = _create_project_dir(dir)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
-    _create_core_dir(app_dir / "core")
     _create_apps_dir(app_dir / "apps")
     return project_dir
 
 
 def _create_project_dir(dirname: Path) -> Path:
     project_dir = create_project_dir(dirname, "propan[async-redis]")
 
@@ -60,28 +58,16 @@
 
 def _create_config_dir(config: Path) -> Path:
     config_dir = create_config_dir(config)
     create_env(config_dir, "redis://localhost:6379/")
     return config_dir
 
 
-def _create_core_dir(core: Path) -> Path:
-    core_dir = create_core_dir(core, "RedisBroker")
-    return core_dir
-
-
 def _create_apps_dir(apps: Path) -> Path:
     apps_dir = create_apps_dir(apps)
 
-    write_file(
+    create_handlers_file(
         apps_dir / "handlers.py",
-        "from propan.annotations import Logger",
-        "",
-        "from core import broker",
-        "",
-        "",
-        "@broker.handle('test')",
-        "async def base_handler(body: dict, logger: Logger):",
-        "    logger.info(body)",
+        "RedisRouter",
     )
 
     return apps_dir
```

### Comparing `propan-0.1.3.9/propan/cli/supervisors/basereload.py` & `propan-0.1.4.0/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/supervisors/multiprocess.py` & `propan-0.1.4.0/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/supervisors/utils.py` & `propan-0.1.4.0/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/supervisors/watchfiles.py` & `propan-0.1.4.0/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/utils/imports.py` & `propan-0.1.4.0/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/utils/logs.py` & `propan-0.1.4.0/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/cli/utils/parser.py` & `propan-0.1.4.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/fastapi/__init__.py` & `propan-0.1.4.0/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/fastapi/core/route.py` & `propan-0.1.4.0/propan/fastapi/core/route.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 import asyncio
 import inspect
 from functools import wraps
 from itertools import dropwhile
-from typing import Any, Callable, Coroutine, Optional, Union
+from typing import Any, Callable, Coroutine, Optional, Sequence, Union
 
+from fastapi import params
 from fastapi.dependencies.models import Dependant
-from fastapi.dependencies.utils import get_dependant, solve_dependencies
+from fastapi.dependencies.utils import (
+    get_dependant,
+    get_parameterless_sub_dependant,
+    solve_dependencies,
+)
 from fastapi.routing import run_endpoint_function
-from pydantic import ValidationError, create_model
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
+from propan._compat import raise_fastapi_validation_error
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage as NativeMessage
 from propan.brokers._model.schemas import Queue
 from propan.types import AnyDict
 
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
         path: Union[Queue, str],
         *extra: Union[Queue, str],
         endpoint: Callable[..., Any],
         broker: BrokerUsecase[Any, Any],
+        dependencies: Sequence[params.Depends] = (),
         dependency_overrides_provider: Optional[Any] = None,
         **handle_kwargs: AnyDict,
     ) -> None:
         self.path = path
         self.broker = broker
-        self.dependant = get_dependant(
-            path=(path if isinstance(path, str) else path.name) or "",
+
+        path_name = (path if isinstance(path, str) else path.name) or ""
+        dependant = get_dependant(
+            path=path_name,
             call=endpoint,
         )
+        for depends in dependencies[::-1]:
+            dependant.dependencies.insert(
+                0,
+                get_parameterless_sub_dependant(depends=depends, path=path_name),
+            )
 
         handler = wraps(endpoint)(
             PropanMessage.get_session(
-                self.dependant,
+                dependant,
                 dependency_overrides_provider,
             )
         )
 
-        broker.handle(
+        self.dependant = dependant
+
+        self.handler = broker.handle(
             path,
             *extra,
             _raw=True,
-            _get_dependant=get_dependant,
+            _get_dependant=lambda call: dependant,
             **handle_kwargs,  # type: ignore
         )(handler)
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
@@ -113,15 +128,15 @@
             body=request._body,
             dependant=dependant,
             dependency_overrides_provider=dependency_overrides_provider,
         )
 
         values, errors, _, _2, _3 = solved_result
         if errors:
-            raise ValidationError(errors, create_model("PropanRoute"))
+            raise_fastapi_validation_error(errors, request._body)
 
         return await run_endpoint_function(
             dependant=dependant,
             values=values,
             is_coroutine=asyncio.iscoroutinefunction(dependant.call),
         )
```

### Comparing `propan-0.1.3.9/propan/fastapi/core/router.py` & `propan-0.1.4.0/propan/fastapi/core/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,23 +34,24 @@
     gen_app_schema_yaml,
     get_app_schema,
     json_schema_to_yaml,
     schema_to_json,
 )
 from propan.cli.docs.serving import get_asyncapi_html
 from propan.fastapi.core.route import PropanRoute
-from propan.types import AnyDict
+from propan.types import AnyDict, HandlerCallable
 from propan.utils.functions import to_async
 
 Broker = TypeVar("Broker", bound=BrokerUsecase[Any, Any])
 
 
 class PropanRouter(APIRouter, Generic[Broker]):
     broker_class: Type[Broker]
     broker: Broker
+    docs_router: Optional[APIRouter]
     _after_startup_hooks: List[
         Callable[[AppType], Awaitable[Optional[Mapping[str, Any]]]]
     ]
 
     def __init__(
         self,
         *connection_args: Tuple[Any, ...],
@@ -97,80 +98,99 @@
             redirect_slashes=redirect_slashes,
             default=default,
             dependency_overrides_provider=dependency_overrides_provider,
             route_class=route_class,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             generate_unique_id_function=generate_unique_id_function,
-            lifespan=self._wrap_lifespan(lifespan),
+            lifespan=self.wrap_lifespan(lifespan),
             on_startup=on_startup,
             on_shutdown=on_shutdown,
         )
 
         if self.include_in_schema is True:  # pragma: no branch
-            self.get(schema_url)(serve_asyncapi_schema)
-            self.get(f"{schema_url}.json")(download_app_json_schema)
-            self.get(f"{schema_url}.yaml")(download_app_yaml_schema)
+            docs_router = APIRouter(
+                prefix=prefix,
+                tags=["asyncapi"],
+                redirect_slashes=redirect_slashes,
+                default=default,
+                deprecated=deprecated,
+            )
+            docs_router.get(schema_url)(serve_asyncapi_schema)
+            docs_router.get(f"{schema_url}.json")(download_app_json_schema)
+            docs_router.get(f"{schema_url}.yaml")(download_app_yaml_schema)
+            self.docs_router = docs_router
+        else:
+            self.docs_router = None
 
         self._after_startup_hooks = []
 
     def add_api_mq_route(
         self,
         path: Union[Queue, str],
         *extra: Union[Queue, str],
-        endpoint: Callable[..., Any],
+        endpoint: DecoratedCallable,
+        dependencies: Sequence[params.Depends],
         **broker_kwargs: AnyDict,
-    ) -> None:
+    ) -> HandlerCallable:
         route = PropanRoute(
             path,
             *extra,
             endpoint=endpoint,
+            dependencies=dependencies,
             dependency_overrides_provider=self.dependency_overrides_provider,
             broker=self.broker,
             **broker_kwargs,
         )
         self.routes.append(route)
+        return route.handler
 
     def event(
         self,
         path: Union[str, Queue],
         *extra: Union[Queue, str],
+        dependencies: Optional[Sequence[params.Depends]] = None,
         **broker_kwargs: Dict[str, Any],
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
-        def decorator(func: DecoratedCallable) -> DecoratedCallable:
-            self.add_api_mq_route(
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
+        current_dependencies = self.dependencies.copy()
+        if dependencies:
+            current_dependencies.extend(dependencies)
+
+        def decorator(func: DecoratedCallable) -> HandlerCallable:
+            return self.add_api_mq_route(
                 path,
                 *extra,
                 endpoint=func,
+                dependencies=current_dependencies,
                 **broker_kwargs,
             )
-            return func
 
         return decorator
 
-    def _wrap_lifespan(self, lifespan: Optional[Lifespan[Any]] = None) -> Lifespan[Any]:
+    def wrap_lifespan(self, lifespan: Optional[Lifespan[Any]] = None) -> Lifespan[Any]:
         if lifespan is not None:
             lifespan_context = lifespan
         else:
             lifespan_context = _DefaultLifespan(self)
 
         @asynccontextmanager
         async def start_broker_lifespan(
             app: FastAPI,
         ) -> AsyncIterator[Mapping[str, Any]]:
             app.broker = self.broker  # type: ignore
+            if self.docs_router:
+                app.include_router(self.docs_router)
 
             async with lifespan_context(app) as maybe_context:
                 if maybe_context is None:
                     context: Dict[str, Any] = {}
                 else:
                     context = dict(maybe_context)
 
                 context.update({"broker": self.broker})
-
                 await self.broker.start()
 
                 for h in self._after_startup_hooks:
                     h_context = await h(app)
                     if h_context:  # pragma: no branch
                         context.update(h_context)
```

### Comparing `propan-0.1.3.9/propan/fastapi/kafka/router.pyi` & `propan-0.1.4.0/propan/fastapi/kafka/router.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing_extensions import Literal, TypeVar
 
 from propan import KafkaBroker
 from propan.__about__ import __version__
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable
+from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 Partition = TypeVar("Partition")
 
 class KafkaRouter(PropanRouter[KafkaBroker]):
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
@@ -138,15 +138,16 @@
             "read_committed",
         ] = "read_uncommitted",
         # broker kwargs
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[ConsumerRecord] = None,
         parse_message: CustomParser[ConsumerRecord] = None,
         description: str = "",
-    ) -> None:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> HandlerCallable:
         pass
     def event(  # type: ignore[override]
         self,
         *topics: str,
         group_id: Optional[str] = None,
         key_deserializer: Optional[Callable[[bytes], Any]] = None,
         value_deserializer: Optional[Callable[[bytes], Any]] = None,
@@ -173,13 +174,14 @@
         max_poll_records: Optional[int] = None,
         exclude_internal_topics: bool = True,
         isolation_level: Literal[
             "read_uncommitted",
             "read_committed",
         ] = "read_uncommitted",
         # broker kwargs
+        dependencies: Optional[Sequence[params.Depends]] = None,
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[ConsumerRecord] = None,
         parse_message: CustomParser[ConsumerRecord] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
         pass
```

### Comparing `propan-0.1.3.9/propan/fastapi/nats/router.pyi` & `propan-0.1.4.0/propan/fastapi/nats/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import NatsBroker
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable
+from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 class NatsRouter(PropanRouter[NatsBroker]):
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
@@ -104,20 +104,22 @@
         *,
         queue: str = "",
         endpoint: AnyCallable,
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[Msg] = None,
         parse_message: CustomParser[Msg] = None,
         description: str = "",
-    ) -> None:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> HandlerCallable:
         pass
     def event(  # type: ignore[override]
         self,
         subject: str,
         *,
         queue: str = "",
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[Msg] = None,
         parse_message: CustomParser[Msg] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
         pass
```

### Comparing `propan-0.1.3.9/propan/fastapi/rabbit/router.pyi` & `propan-0.1.4.0/propan/fastapi/rabbit/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from starlette.types import ASGIApp
 
 from propan import RabbitBroker
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, DecoratedCallable
+from propan.types import AnyCallable, DecoratedCallable, HandlerCallable
 
 class RabbitRouter(PropanRouter[RabbitBroker]):
     def __init__(
         self,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
@@ -72,20 +72,22 @@
         *,
         endpoint: AnyCallable,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[IncomingMessage] = None,
         parse_message: CustomParser[IncomingMessage] = None,
         description: str = "",
-    ) -> None:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> HandlerCallable:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[IncomingMessage] = None,
         parse_message: CustomParser[IncomingMessage] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
         pass
```

### Comparing `propan-0.1.3.9/propan/fastapi/redis/router.pyi` & `propan-0.1.4.0/propan/fastapi/redis/router.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
 from propan import RedisBroker
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, AnyDict, DecoratedCallable
+from propan.types import AnyCallable, AnyDict, DecoratedCallable, HandlerCallable
 
 class RedisRouter(PropanRouter[RedisBroker]):
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: float = 1.0,
         host: str = "localhost",
@@ -76,19 +76,21 @@
         channel: str,
         *,
         endpoint: AnyCallable,
         pattern: bool = False,
         decode_message: CustomDecoder[AnyDict] = None,
         parse_message: CustomParser[AnyDict] = None,
         description: str = "",
-    ) -> None:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> HandlerCallable:
         pass
     def event(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
         decode_message: CustomDecoder[AnyDict] = None,
         parse_message: CustomParser[AnyDict] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
         pass
```

### Comparing `propan-0.1.3.9/propan/fastapi/sqs/router.pyi` & `propan-0.1.4.0/propan/fastapi/sqs/router.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from starlette.types import ASGIApp
 
 from propan import SQSBroker
 from propan.brokers._model.broker_usecase import CustomDecoder, CustomParser
 from propan.brokers.sqs.schema import SQSQueue
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
-from propan.types import AnyCallable, AnyDict, DecoratedCallable
+from propan.types import AnyCallable, AnyDict, DecoratedCallable, HandlerCallable
 
 class SQSRouter(PropanRouter[SQSBroker]):
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
@@ -72,15 +72,16 @@
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
         endpoint: AnyCallable,
         decode_message: CustomDecoder[AnyDict] = None,
         parse_message: CustomParser[AnyDict] = None,
         description: str = "",
-    ) -> None:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> HandlerCallable:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, SQSQueue],
         *,
         wait_interval: int = 1,
         max_messages_number: int = 10,  # 1...10
@@ -88,9 +89,10 @@
         message_attributes: Sequence[str] = (),
         request_attempt_id: Optional[str] = None,
         visibility_timeout: int = 0,
         retry: Union[bool, int] = False,
         decode_message: CustomDecoder[AnyDict] = None,
         parse_message: CustomParser[AnyDict] = None,
         description: str = "",
-    ) -> Callable[[DecoratedCallable], DecoratedCallable]:
+        dependencies: Optional[Sequence[params.Depends]] = None,
+    ) -> Callable[[DecoratedCallable], HandlerCallable]:
         pass
```

### Comparing `propan-0.1.3.9/propan/log/formatter.py` & `propan-0.1.4.0/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/log/logging.py` & `propan-0.1.4.0/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/test/__init__.py` & `propan-0.1.4.0/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/test/kafka.py` & `propan-0.1.4.0/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/test/nats.py` & `propan-0.1.4.0/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/test/rabbit.py` & `propan-0.1.4.0/propan/test/rabbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,24 +51,26 @@
     routing_key: str = "",
     **message_kwargs: AnyDict,
 ) -> PatchedMessage:
     que, exch = _validate_queue(queue), _validate_exchange(exchange)
     msg = RabbitBroker._validate_message(message, None, **message_kwargs)
 
     routing = routing_key or (que.name if que else "")
+
     return PatchedMessage(
         aiormq.abc.DeliveredMessage(
             delivery=spec.Basic.Deliver(
                 exchange=exch.name if exch else "",
                 routing_key=routing,
             ),
             header=ContentHeader(
                 properties=spec.Basic.Properties(
                     content_type=msg.content_type,
                     message_id=str(uuid4()),
+                    headers=msg.headers,
                 )
             ),
             body=msg.body,
             channel=AsyncMock(),
         )
     )
```

### Comparing `propan-0.1.3.9/propan/test/redis.py` & `propan-0.1.4.0/propan/test/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing_extensions import TypeAlias
 
 if sys.version_info < (3, 8):
     from asyncmock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
+from propan._compat import model_to_json
 from propan.brokers.redis.redis_broker import RedisBroker
 from propan.brokers.redis.schemas import RedisMessage
 from propan.test.utils import call_handler
 from propan.types import SendableMessage
 
 __all__ = (
     "build_message",
@@ -31,24 +32,24 @@
     headers: Optional[Dict[str, Any]] = None,
 ) -> Msg:
     msg, content_type = RedisBroker._encode_message(message)
     return {
         "type": "message",
         "pattern": None,
         "channel": channel.encode(),
-        "data": RedisMessage(
-            data=msg,
-            headers={
-                "content-type": content_type or "",
-                **(headers or {}),
-            },
-            reply_to=reply_to,
-        )
-        .json()
-        .encode(),
+        "data": model_to_json(
+            RedisMessage(
+                data=msg,
+                headers={
+                    "content-type": content_type or "",
+                    **(headers or {}),
+                },
+                reply_to=reply_to,
+            )
+        ).encode(),
     }
 
 
 async def publish(
     self: RedisBroker,
     message: SendableMessage,
     channel: str,
```

### Comparing `propan-0.1.3.9/propan/test/sqs.py` & `propan-0.1.4.0/propan/test/sqs.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,13 +90,17 @@
             r = await call_handler(
                 handler, incoming, callback, callback_timeout, raise_timeout
             )
             if callback:  # pragma: no branch
                 return r
 
 
+async def delete_message(self: SQSBroker) -> None:
+    pass
+
+
 def TestSQSBroker(broker: SQSBroker) -> SQSBroker:
     broker.connect = AsyncMock()  # type: ignore
     broker.start = AsyncMock()  # type: ignore
-    broker.delete_message = AsyncMock()  # type: ignore
+    broker.delete_message = MethodType(delete_message, broker)  # type: ignore
     broker.publish = MethodType(publish, broker)  # type: ignore
     return broker
```

### Comparing `propan-0.1.3.9/propan/test/utils.py` & `propan-0.1.4.0/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/utils/functions.py` & `propan-0.1.4.0/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/utils/context/main.py` & `propan-0.1.4.0/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/propan/utils/context/types.py` & `propan-0.1.4.0/propan/utils/context/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,11 +36,9 @@
 
 def resolve_context(argument: str) -> Any:
     keys = argument.split(".")
 
     v = context.context[keys[0]]
     for i in keys[1:]:
         v = getattr(v, i)
-        if v is None:
-            return v
 
     return v
```

### Comparing `propan-0.1.3.9/LICENSE` & `propan-0.1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/README.md` & `propan-0.1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.3.9/pyproject.toml` & `propan-0.1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -97,17 +97,18 @@
     "propan[async-redis]",
     "propan[async-kafka]",
     "propan[async-sqs]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
-    "pydantic-settings>=2.0a1",
 
     "fastapi==0.100.0b1",
+    "httpx",
+    "pydantic-settings>=2.0a1",
     "python-dotenv",
 
     "asyncmock; python_version < '3.8'",
 ]
 
 dev-doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
@@ -225,15 +226,15 @@
 
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = [
     "propan.Depends", "propan.Context",
     "propan.utils.Depends", "propan.utils.Context",
     "propan.utils.context.Depends", "propan.utils.context.Context",
     "typer.Argument", "typer.Option",
-    "pydantic.Field",
+    "pydantic.Field", "rocketry.args.Arg",
     "fastapi.Depends", "fastapi.datastructures.Default",
     "kafka.partitioner.default.DefaultPartitioner",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q -m 'not slow'"
```

### Comparing `propan-0.1.3.9/PKG-INFO` & `propan-0.1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.3.9
+Version: 0.1.4.0
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -73,14 +73,15 @@
 Requires-Dist: polyfactory>=2.3.0; python_version > '3.7' and extra == 'doc'
 Requires-Dist: pyyaml; extra == 'doc'
 Requires-Dist: uvicorn; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi==0.100.0b1; extra == 'test'
+Requires-Dist: httpx; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: propan[async-sqs]; extra == 'test'
 Requires-Dist: propan[doc]; extra == 'test'
 Requires-Dist: pydantic-settings>=2.0a1; extra == 'test'
```

