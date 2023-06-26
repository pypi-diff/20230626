# Comparing `tmp/petisco-2.0.0rc3.tar.gz` & `tmp/petisco-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-2.0.0rc3.tar", last modified: Fri Jun 23 10:19:04 2023, max compression
+gzip compressed data, was "petisco-2.0.0rc4.tar", last modified: Mon Jun 26 09:44:55 2023, max compression
```

## Comparing `petisco-2.0.0rc3.tar` & `petisco-2.0.0rc4.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.890503 petisco-2.0.0rc3/petisco/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.890503 petisco-2.0.0rc3/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/chaos/chaos_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/chaos/check_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/async_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/controller/meta_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/dependency_injection/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/handlers/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.894503 petisco-2.0.0rc3/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.898503 petisco-2.0.0rc3/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/async_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.898503 petisco-2.0.0rc3/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/use_case/async_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/use_case/meta_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.898503 petisco-2.0.0rc3/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.898503 petisco-2.0.0rc3/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.898503 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.902503 petisco-2.0.0rc3/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.902503 petisco-2.0.0rc3/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.902503 petisco-2.0.0rc3/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.902503 petisco-2.0.0rc3/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/async_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/async_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/legacy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/legacy_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/domain/persistence/persistence_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/cli/petisco_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/async_elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/is_elastic_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic/legacy_elastic_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/extra/elastic_apm/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic_apm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/elastic_apm/is_elastic_apm_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.906503 petisco-2.0.0rc3/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/application/fastapi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/as_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/loguru_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/logger/not_implemented_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.910503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/redis/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.914503 petisco-2.0.0rc3/petisco/extra/redis/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/redis/is_redis_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.918503 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/async_sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/base_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/extra/threading/pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/petisco/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.890503 petisco-2.0.0rc3/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 10:19:04.000000 petisco-2.0.0rc3/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:04.922503 petisco-2.0.0rc3/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:18:58.000000 petisco-2.0.0rc3/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.577538 petisco-2.0.0rc4/petisco/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.581538 petisco-2.0.0rc4/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.581538 petisco-2.0.0rc4/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.581538 petisco-2.0.0rc4/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.581538 petisco-2.0.0rc4/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.585538 petisco-2.0.0rc4/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.585538 petisco-2.0.0rc4/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.585538 petisco-2.0.0rc4/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.585538 petisco-2.0.0rc4/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.585538 petisco-2.0.0rc4/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.589538 petisco-2.0.0rc4/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.589538 petisco-2.0.0rc4/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.589538 petisco-2.0.0rc4/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.589538 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.593538 petisco-2.0.0rc4/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.597538 petisco-2.0.0rc4/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.597538 petisco-2.0.0rc4/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.597538 petisco-2.0.0rc4/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/legacy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/legacy_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/domain/persistence/persistence_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.601538 petisco-2.0.0rc4/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.601538 petisco-2.0.0rc4/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.601538 petisco-2.0.0rc4/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.601538 petisco-2.0.0rc4/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.601538 petisco-2.0.0rc4/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/is_elastic_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic/legacy_elastic_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.605538 petisco-2.0.0rc4/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.605538 petisco-2.0.0rc4/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.605538 petisco-2.0.0rc4/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/application/fastapi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.605538 petisco-2.0.0rc4/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.605538 petisco-2.0.0rc4/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.609538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.613538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.613538 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.613538 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.613538 petisco-2.0.0rc4/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.613538 petisco-2.0.0rc4/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.617538 petisco-2.0.0rc4/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.621538 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/base_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.621538 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.621538 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.621538 petisco-2.0.0rc4/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.581538 petisco-2.0.0rc4/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:44:55.000000 petisco-2.0.0rc4/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:55.629538 petisco-2.0.0rc4/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:44:52.000000 petisco-2.0.0rc4/tests/modules/__init__.py
```

### Comparing `petisco-2.0.0rc3/LICENSE` & `petisco-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/PKG-INFO` & `petisco-2.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc3 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc4 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `petisco-2.0.0rc3/README.md` & `petisco-2.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/application.py` & `petisco-2.0.0rc4/petisco/base/application/application.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/application_info.py` & `petisco-2.0.0rc4/petisco/base/application/application_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/chaos/chaos_config.py` & `petisco-2.0.0rc4/petisco/base/application/chaos/chaos_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/controller/async_controller.py` & `petisco-2.0.0rc4/petisco/base/application/controller/async_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/controller/controller.py` & `petisco-2.0.0rc4/petisco/base/application/controller/controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/controller/http_error.py` & `petisco-2.0.0rc4/petisco/base/application/controller/http_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/controller/meta_controller.py` & `petisco-2.0.0rc4/petisco/base/application/controller/meta_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/dependency_injection/container.py` & `petisco-2.0.0rc4/petisco/base/application/dependency_injection/container.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/dependency_injection/dependency.py` & `petisco-2.0.0rc4/petisco/base/application/dependency_injection/dependency.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/handlers/message_handler.py` & `petisco-2.0.0rc4/petisco/base/application/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/middleware/middleware.py` & `petisco-2.0.0rc4/petisco/base/application/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.0.0rc4/petisco/base/application/middleware/notifier_middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/notifier/notifier.py` & `petisco-2.0.0rc4/petisco/base/application/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-2.0.0rc4/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/patterns/crud_repository.py` & `petisco-2.0.0rc4/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.0.0rc4/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/application/use_case/meta_use_case.py` & `petisco-2.0.0rc4/petisco/base/application/use_case/meta_use_case.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.0.0rc4/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.0.0rc4/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.0.0rc4/petisco/base/domain/errors/defaults/not_found.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/errors/domain_error.py` & `petisco-2.0.0rc4/petisco/base/domain/errors/domain_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/errors/unknown_error.py` & `petisco-2.0.0rc4/petisco/base/domain/errors/unknown_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-2.0.0rc4/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/command.py` & `petisco-2.0.0rc4/petisco/base/domain/message/command.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/command_bus.py` & `petisco-2.0.0rc4/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/command_subscriber.py` & `petisco-2.0.0rc4/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/domain_event.py` & `petisco-2.0.0rc4/petisco/base/domain/message/domain_event.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.0.0rc4/petisco/base/domain/message/domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-2.0.0rc4/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_bus.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_configurer.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_consumer.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_handler_returns_none_error.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_handler_returns_none_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_subscriber.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/message_subscriber_info.py` & `petisco-2.0.0rc4/petisco/base/domain/message/message_subscriber_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_command_bus.py` & `petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.0.0rc4/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/model/aggregate_root.py` & `petisco-2.0.0rc4/petisco/base/domain/model/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/model/uuid.py` & `petisco-2.0.0rc4/petisco/base/domain/model/uuid.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/model/value_object.py` & `petisco-2.0.0rc4/petisco/base/domain/model/value_object.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/async_fake_database.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/async_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/database.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/databases.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/databases.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/legacy_database.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/legacy_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/legacy_fake_database.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/legacy_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/persistence.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/domain/persistence/persistence_models.py` & `petisco-2.0.0rc4/petisco/base/domain/persistence/persistence_models.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/misc/async_wrapper.py` & `petisco-2.0.0rc4/petisco/base/misc/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/misc/builder.py` & `petisco-2.0.0rc4/petisco/base/misc/builder.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/misc/result_mapper.py` & `petisco-2.0.0rc4/petisco/base/misc/result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/misc/singleton.py` & `petisco-2.0.0rc4/petisco/base/misc/singleton.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/base/misc/wrapper.py` & `petisco-2.0.0rc4/petisco/base/misc/wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/cli/petisco.py` & `petisco-2.0.0rc4/petisco/cli/petisco.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/cli/petisco_dev.py` & `petisco-2.0.0rc4/petisco/cli/petisco_dev.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/cli/petisco_rabbitmq.py` & `petisco-2.0.0rc4/petisco/cli/petisco_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/__init__.py` & `petisco-2.0.0rc4/petisco/extra/elastic/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from petisco.extra.elastic.is_elastic_available import is_elastic_available
 
 elastic = list()
 if is_elastic_available():
-    from petisco.extra.elastic.async_elastic_database import AsyncElasticDatabase
+    from petisco.extra.elastic.async_elastic_database import (
+        AsyncElasticDatabase,
+        AsyncElasticSessionScope,
+    )
     from petisco.extra.elastic.elastic_connection import ElasticConnection
-    from petisco.extra.elastic.elastic_database import ElasticDatabase
+    from petisco.extra.elastic.elastic_database import (
+        ElasticDatabase,
+        ElasticSessionScope,
+    )
     from petisco.extra.elastic.legacy_elastic_database import LegacyElasticDatabase
 
     elastic = [
         "ElasticConnection",
         "LegacyElasticDatabase",
         "ElasticDatabase",
         "AsyncElasticDatabase",
+        "ElasticSessionScope",
+        "AsyncElasticSessionScope",
     ]
 else:
     elastic = []
 
 __all__ = elastic
```

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/async_elastic_database.py` & `petisco-2.0.0rc4/petisco/extra/elastic/async_elastic_database.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,30 +27,33 @@
         except Exception as e:
             logger.error(e)
             raise e
 
     return session_scope
 
 
+AsyncElasticSessionScope = Callable[..., ContextManager[AsyncElasticsearch]]
+
+
 class AsyncElasticDatabase(AsyncDatabase):
     session: AsyncElasticsearch | None = None
 
     @staticmethod
     def local_connection_checker() -> AsyncElasticDatabase:
         return AsyncElasticDatabase(
             name="test", connection=ElasticConnection.create_local()
         )
 
-    def __init__(self, name: str, connection: ElasticConnection) -> None:
+    def __init__(self, alias: str, connection: ElasticConnection) -> None:
         if not connection or not isinstance(connection, ElasticConnection):
             raise ConnectionError(
                 "ElasticDatabase needs a valid ElasticConnection connection"
             )
         self.connection = connection
-        super().__init__(name)
+        super().__init__(alias)
 
     def initialize(self) -> None:
         self.session = AsyncElasticsearch(
             self.connection.to_elastic_format(), http_auth=self.connection.http_auth
         )
 
     def delete(self) -> None:
@@ -61,9 +64,9 @@
 
     async def is_available(self) -> bool:
         try:
             return await self.session.ping()
         except Exception:  # noqa E722
             return False
 
-    def get_session_scope(self) -> Callable[..., ContextManager[AsyncElasticsearch]]:
+    def get_session_scope(self) -> AsyncElasticSessionScope:
         return async_elastic_session_scope_provider(self.session)
```

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/elastic_connection.py` & `petisco-2.0.0rc4/petisco/extra/elastic/elastic_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/elastic_database.py` & `petisco-2.0.0rc4/petisco/extra/elastic/elastic_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,31 @@
         except Exception as e:
             logger.error(e)
             raise e
 
     return session_scope
 
 
+ElasticSessionScope = Callable[..., ContextManager[Elasticsearch]]
+
+
 class ElasticDatabase(Database):
     session: Elasticsearch | None = None
 
     @staticmethod
     def local_connection_checker() -> ElasticDatabase:
         return ElasticDatabase(name="test", connection=ElasticConnection.create_local())
 
-    def __init__(self, name: str, connection: ElasticConnection) -> None:
+    def __init__(self, alias: str, connection: ElasticConnection) -> None:
         if not connection or not isinstance(connection, ElasticConnection):
             raise ConnectionError(
                 "ElasticDatabase needs a valid ElasticConnection connection"
             )
         self.connection = connection
-        super().__init__(name)
+        super().__init__(alias)
 
     def initialize(self) -> None:
         self.session = Elasticsearch(
             self.connection.to_elastic_format(), http_auth=self.connection.http_auth
         )
 
     def delete(self) -> None:
@@ -60,9 +63,9 @@
 
     def is_available(self) -> bool:
         try:
             return self.session.ping()
         except Exception:  # noqa E722
             return False
 
-    def get_session_scope(self) -> Callable[..., ContextManager[Elasticsearch]]:
+    def get_session_scope(self) -> ElasticSessionScope:
         return elastic_session_scope_provider(self.session)
```

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.0.0rc4/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic/legacy_elastic_database.py` & `petisco-2.0.0rc4/petisco/extra/elastic/legacy_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py` & `petisco-2.0.0rc4/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/fastapi/__init__.py` & `petisco-2.0.0rc4/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.0.0rc4/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/fastapi/testing/assert_http_exception.py` & `petisco-2.0.0rc4/petisco/extra/fastapi/testing/assert_http_exception.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/logger/__init__.py` & `petisco-2.0.0rc4/petisco/extra/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/logger/log_message.py` & `petisco-2.0.0rc4/petisco/extra/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/logger/logging_based_logger.py` & `petisco-2.0.0rc4/petisco/extra/logger/logging_based_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/logger/loguru_logger.py` & `petisco-2.0.0rc4/petisco/extra/logger/loguru_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/__init__.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.0.0rc4/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_command_bus.py` & `petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py` & `petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/redis/application/message/bus/redis_message_bus.py` & `petisco-2.0.0rc4/petisco/extra/redis/application/message/bus/redis_message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/__init__.py` & `petisco-2.0.0rc4/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc4/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc4/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.0.0rc4/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-2.0.0rc4/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/slack/dependencies.py` & `petisco-2.0.0rc4/petisco/extra/slack/dependencies.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/async_sql_database.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/async_sql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/base_sql_repository.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/base_sql_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_base.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_base.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_database.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py` & `petisco-2.0.0rc4/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.0.0rc4/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/extra/threading/pool_executor.py` & `petisco-2.0.0rc4/petisco/extra/threading/pool_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco/public_api.py` & `petisco-2.0.0rc4/petisco/public_api.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/petisco.egg-info/PKG-INFO` & `petisco-2.0.0rc4/petisco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc3 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc4 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `petisco-2.0.0rc3/petisco.egg-info/SOURCES.txt` & `petisco-2.0.0rc4/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/setup.cfg` & `petisco-2.0.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/setup.py` & `petisco-2.0.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc3/tests/fixtures.py` & `petisco-2.0.0rc4/tests/fixtures.py`

 * *Files identical despite different names*

