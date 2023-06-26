# Comparing `tmp/nsj_rest_lib-1.1.0.tar.gz` & `tmp/nsj_rest_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.1.0.tar", last modified: Thu Jun 15 22:55:12 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.1.1.tar", last modified: Mon Jun 26 13:21:27 2023, max compression
```

## Comparing `nsj_rest_lib-1.1.0.tar` & `nsj_rest_lib-1.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.1.0/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-15 22:55:12.323049 nsj_rest_lib-1.1.0/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.307049 nsj_rest_lib-1.1.0/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.311049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4104 2023-06-15 22:54:32.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16780 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    23263 2023-06-15 22:54:32.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.319049 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-15 22:55:12.315049 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1652 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-15 22:55:12.000000 nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.061753 nsj_rest_lib-1.1.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-26 13:21:27.061753 nsj_rest_lib-1.1.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-1.1.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-26 13:21:27.061753 nsj_rest_lib-1.1.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.037754 nsj_rest_lib-1.1.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.045754 nsj_rest_lib-1.1.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.049753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4104 2023-06-15 22:54:32.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.049753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16780 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.053753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.057753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-14 17:50:21.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.057753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.057753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-05-30 22:01:35.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.057753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23612 2023-06-26 13:20:58.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.061753 nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-26 13:21:27.045754 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-26 13:21:27.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1652 2023-06-26 13:21:27.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-26 13:21:27.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-26 13:21:27.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-26 13:21:27.000000 nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.1.0/PKG-INFO` & `nsj_rest_lib-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.1.0/setup.cfg` & `nsj_rest_lib-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.1.0
+version = 1.1.1
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/service/service_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 from ast import Delete
 import enum
+import time
 import uuid
 import copy
 
 from typing import Any, Dict, List, Set
 
 from flask import g
 
 from nsj_rest_lib.dao.dao_base import DAOBase
 from nsj_rest_lib.descriptor.dto_field import DTOFieldFilter
 from nsj_rest_lib.descriptor.filter_operator import FilterOperator
 from nsj_rest_lib.dto.dto_base import DTOBase
 from nsj_rest_lib.entity.entity_base import EntityBase
 from nsj_rest_lib.entity.filter import Filter
-from nsj_rest_lib.exception import DTOListFieldConfigException, ConflictException, NotFoundException
+from nsj_rest_lib.exception import (
+    DTOListFieldConfigException,
+    ConflictException,
+    NotFoundException,
+)
 from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
 
 
 class ServiceBase:
     _dao: DAOBase
     _dto_class: DTOBase
 
     def __init__(
         self,
         injector_factory: NsjInjectorFactoryBase,
         dao: DAOBase,
         dto_class: DTOBase,
         entity_class: EntityBase,
-        dto_post_response_class: DTOBase = None
+        dto_post_response_class: DTOBase = None,
     ):
         self._injector_factory = injector_factory
         self._dao = dao
         self._dto_class = dto_class
         self._entity_class = entity_class
         self._dto_post_response_class = dto_post_response_class
-        self._created_by_property = 'criado_por'
-        self._updated_by_property = 'atualizado_por'
+        self._created_by_property = "criado_por"
+        self._updated_by_property = "atualizado_por"
 
     def get(
-        self,
-        id: str,
-        partition_fields: Dict[str, Any],
-        fields: Dict[str, List[str]]
+        self, id: str, partition_fields: Dict[str, Any], fields: Dict[str, List[str]]
     ) -> DTOBase:
         # Resolving fields
         fields = self._resolving_fields(fields)
 
         # Handling the fields to retrieve
-        entity_fields = self._convert_to_entity_fields(fields['root'])
+        entity_fields = self._convert_to_entity_fields(fields["root"])
 
         entity_filters = self._create_entity_filters(partition_fields)
 
         # Recuperando a entity
         entity = self._dao.get(id, entity_fields, entity_filters)
 
         # Convertendo para DTO
@@ -89,27 +91,28 @@
 
         entity_field_name = field
         if self._dto_class.fields_map[field].entity_field is not None:
             entity_field_name = self._dto_class.fields_map[field].entity_field
 
         return entity_field_name
 
-    def _create_entity_filters(self, filters: Dict[str, Any]) -> Dict[str, List[Filter]]:
+    def _create_entity_filters(
+        self, filters: Dict[str, Any]
+    ) -> Dict[str, List[Filter]]:
         """
         Converting DTO filters to Entity filters.
 
         Returns a Dict (indexed by entity field name) of List of Filter.
         """
 
         if filters is None:
             return None
 
         entity_filters = {}
         for filter in filters:
-
             is_entity_filter = False
             if filter in self._dto_class.field_filters_map:
                 # Retrieving filter config
                 field_filter = self._dto_class.field_filters_map[filter]
             elif filter in self._dto_class.fields_map:
                 # Creating filter config to a DTOField (equals operator)
                 field_filter = DTOFieldFilter(filter)
@@ -120,73 +123,68 @@
             else:
                 # Ignoring not declared filters (or filter for not existent DTOField)
                 continue
 
             # Resolving entity field name (to filter)
             if not is_entity_filter:
                 entity_field_name = self._convert_to_entity_field(
-                    field_filter.field_name)
+                    field_filter.field_name
+                )
             else:
                 entity_field_name = filter
 
             # Creating entity filters (one for each value - separated by comma)
             if isinstance(filters[filter], str):
-                values = filters[filter].split(',')
+                values = filters[filter].split(",")
             else:
                 values = [filters[filter]]
 
             for value in values:
                 if isinstance(value, str):
                     value = value.strip()
 
                 if not is_entity_filter:
-                    entity_filter = Filter(
-                        field_filter.operator,
-                        value
-                    )
+                    entity_filter = Filter(field_filter.operator, value)
                 else:
-                    entity_filter = Filter(
-                        FilterOperator.EQUALS,
-                        value
-                    )
+                    entity_filter = Filter(FilterOperator.EQUALS, value)
 
                 # Storing filter in dict
                 filter_list = entity_filters.setdefault(entity_field_name, [])
                 filter_list.append(entity_filter)
 
         return entity_filters
 
     def _resolving_fields(self, fields: Dict[str, Set[str]]) -> Dict[str, Set[str]]:
         """
         Varifica os fields recebidos, garantindo que os campos de resumo serão considerados.
         """
 
         # Resolving fields
         if fields is None:
-            result = {'root': set()}
+            result = {"root": set()}
         else:
             result = copy.deepcopy(fields)
-            result['root'] = result['root'].union(
+            result["root"] = result["root"].union(
                 self._dto_class.resume_fields)
 
         return result
 
     def list(
         self,
         after: uuid.UUID,
         limit: int,
         fields: Dict[str, Set[str]],
         order_fields: List[str],
-        filters: Dict[str, Any]
+        filters: Dict[str, Any],
     ) -> List[DTOBase]:
         # Resolving fields
         fields = self._resolving_fields(fields)
 
         # Handling the fields to retrieve
-        entity_fields = self._convert_to_entity_fields(fields['root'])
+        entity_fields = self._convert_to_entity_fields(fields["root"])
 
         # Handling order fields
         order_fields = self._convert_to_entity_fields(order_fields)
 
         # Handling filters
         all_filters = {}
         if filters is not None:
@@ -208,123 +206,114 @@
         # Retrieving related lists
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists(dto_list, fields)
 
         # Returning
         return dto_list
 
-    def _retrieve_related_lists(self, dto_list: List[DTOBase], fields: Dict[str, Set[str]]):
-
+    def _retrieve_related_lists(
+        self, dto_list: List[DTOBase], fields: Dict[str, Set[str]]
+    ):
         # TODO Controlar profundidade?!
 
         # Handling each dto
         for dto in dto_list:
-
             # Handling each related list
             for master_dto_attr, list_field in self._dto_class.list_fields_map.items():
+                if master_dto_attr in fields["root"]:
+                    # Getting service instance
+                    # TODO Refatorar para suportar services customizados
+                    service = ServiceBase(
+                        self._injector_factory,
+                        DAOBase(
+                            self._injector_factory.db_adapter(), list_field.entity_type
+                        ),
+                        list_field.dto_type,
+                        list_field.entity_type,
+                    )
 
-                # Getting service instance
-                # TODO Refatorar para suportar services customizados
-                service = ServiceBase(
-                    self._injector_factory,
-                    DAOBase(self._injector_factory.db_adapter(),
-                            list_field.entity_type),
-                    list_field.dto_type,
-                    list_field.entity_type
-                )
-
-                # Checking if pk_field exists
-                if self._dto_class.pk_field is None:
-                    raise DTOListFieldConfigException(
-                        f"PK field not found in class: {self._dto_class}")
-
-                if not (self._dto_class.pk_field in dto.__dict__):
-                    raise DTOListFieldConfigException(
-                        f"PK field not found in DTO: {self._dto_class}")
-
-                # Making filter to relation
-                filters = {
-                    # TODO Adicionar os campos de particionamento de dados
-                    list_field.related_entity_field: getattr(
-                        dto, self._dto_class.pk_field)
-                }
-
-                # Tratando campos de particionamento
-                for field in self._dto_class.partition_fields:
-                    if field in list_field.dto_type.partition_fields:
-                        filters[field] = getattr(
-                            dto, field)
-
-                # Resolvendo os fields da entidade aninhada
-                fields_to_list = copy.deepcopy(fields)
-                if master_dto_attr in fields:
-                    fields_to_list['root'] = fields[master_dto_attr]
-                    del fields_to_list[master_dto_attr]
-                else:
-                    fields_to_list['root'] = set()
+                    # Checking if pk_field exists
+                    if self._dto_class.pk_field is None:
+                        raise DTOListFieldConfigException(
+                            f"PK field not found in class: {self._dto_class}"
+                        )
+
+                    if not (self._dto_class.pk_field in dto.__dict__):
+                        raise DTOListFieldConfigException(
+                            f"PK field not found in DTO: {self._dto_class}"
+                        )
+
+                    # Making filter to relation
+                    filters = {
+                        # TODO Adicionar os campos de particionamento de dados
+                        list_field.related_entity_field: getattr(
+                            dto, self._dto_class.pk_field
+                        )
+                    }
+
+                    # Tratando campos de particionamento
+                    for field in self._dto_class.partition_fields:
+                        if field in list_field.dto_type.partition_fields:
+                            filters[field] = getattr(dto, field)
+
+                    # Resolvendo os fields da entidade aninhada
+                    fields_to_list = copy.deepcopy(fields)
+                    if master_dto_attr in fields:
+                        fields_to_list["root"] = fields[master_dto_attr]
+                        del fields_to_list[master_dto_attr]
+                    else:
+                        fields_to_list["root"] = set()
 
-                # Getting related data
-                related_dto_list = service.list(
-                    None, None, fields_to_list, None, filters)
+                    # Getting related data
+                    related_dto_list = service.list(
+                        None, None, fields_to_list, None, filters
+                    )
 
-                # Setting dto property
-                setattr(dto, master_dto_attr, related_dto_list)
+                    # Setting dto property
+                    setattr(dto, master_dto_attr, related_dto_list)
 
-    def insert(
-        self,
-        dto: DTOBase
-    ) -> DTOBase:
+    def insert(self, dto: DTOBase) -> DTOBase:
         return self._save(
-            insert=True,
-            dto=dto,
-            manage_transaction=True,
-            partial_update=False
+            insert=True, dto=dto, manage_transaction=True, partial_update=False
         )
 
     def update(
-        self,
-        dto: DTOBase,
-        id: Any,
-        aditional_filters: Dict[str, Any] = None
+        self, dto: DTOBase, id: Any, aditional_filters: Dict[str, Any] = None
     ) -> DTOBase:
         return self._save(
             insert=False,
             dto=dto,
             manage_transaction=True,
             partial_update=False,
             id=id,
-            aditional_filters=aditional_filters
+            aditional_filters=aditional_filters,
         )
 
     def partial_update(
-        self,
-        dto: DTOBase,
-        id: Any,
-        aditional_filters: Dict[str, Any] = None
+        self, dto: DTOBase, id: Any, aditional_filters: Dict[str, Any] = None
     ) -> DTOBase:
         return self._save(
             insert=False,
             dto=dto,
             manage_transaction=True,
             partial_update=True,
             id=id,
-            aditional_filters=aditional_filters
+            aditional_filters=aditional_filters,
         )
 
     def _save(
         self,
         insert: bool,
         dto: DTOBase,
         manage_transaction: bool,
         partial_update: bool,
         relation_field_map: Dict[str, Any] = None,
         id: Any = None,
-        aditional_filters: Dict[str, Any] = None
+        aditional_filters: Dict[str, Any] = None,
     ) -> DTOBase:
-
         try:
             if manage_transaction:
                 self._dao.begin()
 
             # Convertendo o DTO para a Entity
             # TODO Refatorar para usar um construtor do EntityBase (ou algo assim, porque é preciso tratar das equivalências de nome dos campos)
             entity = dto.convert_to_entity(self._entity_class, partial_update)
@@ -337,58 +326,56 @@
             # Setando na Entity os campos de relacionamento recebidos
             if relation_field_map is not None:
                 for entity_field, value in relation_field_map.items():
                     if hasattr(entity, entity_field):
                         setattr(entity, entity_field, value)
 
             # Setando campos criado_por e atualizado_por quando existirem
-            if hasattr(g, 'profile') and g.profile is not None:
+            if hasattr(g, "profile") and g.profile is not None:
                 auth_type_is_api_key = g.profile["authentication_type"] == "api_key"
                 user = g.profile["email"]
                 if insert and hasattr(entity, self._created_by_property):
                     if not auth_type_is_api_key:
                         setattr(entity, self._created_by_property, user)
                     else:
                         value = getattr(entity, self._created_by_property)
-                        if value is None or value == '':
+                        if value is None or value == "":
                             raise ValueError(
-                                f"É necessário preencher o campo '{self._created_by_property}'.")
+                                f"É necessário preencher o campo '{self._created_by_property}'."
+                            )
                 if hasattr(entity, self._updated_by_property):
                     if not auth_type_is_api_key:
                         setattr(entity, self._updated_by_property, user)
                     else:
                         value = getattr(entity, self._updated_by_property)
-                        if value is None or value == '':
+                        if value is None or value == "":
                             raise ValueError(
-                                f"É necessário preencher o campo '{self._updated_by_property}'")
+                                f"É necessário preencher o campo '{self._updated_by_property}'"
+                            )
 
             # Invocando o DAO
             if insert:
                 if self.entity_exists(entity, aditional_filters):
                     raise ConflictException(
-                        f"Já existe um registro no banco com o identificador '{getattr(entity, entity_pk_field)}'")
+                        f"Já existe um registro no banco com o identificador '{getattr(entity, entity_pk_field)}'"
+                    )
                 entity = self._dao.insert(entity)
             else:
                 # Montando os filtros
-                id_condiction = Filter(
-                    FilterOperator.EQUALS,
-                    id
-                )
+                id_condiction = Filter(FilterOperator.EQUALS, id)
                 id_filters = {entity_pk_field: [id_condiction]}
 
                 if aditional_filters is not None:
                     aditional_entity_filters = self._create_entity_filters(
-                        aditional_filters)
+                        aditional_filters
+                    )
                 else:
                     aditional_entity_filters = {}
 
-                entity_filters = {
-                    **id_filters,
-                    **aditional_entity_filters
-                }
+                entity_filters = {**id_filters, **aditional_entity_filters}
 
                 # Executando o update pelo DAO
                 entity = self._dao.update(
                     entity, entity_filters, partial_update)
 
             # Convertendo a entity para o DTO de resposta (se houver um)
             if self._dto_post_response_class is not None:
@@ -396,15 +383,16 @@
             else:
                 # Retorna None, se não se espera um DTO de resposta
                 response_dto = None
 
             # Salvando as lista de DTO detalhe
             if len(self._dto_class.list_fields_map) > 0:
                 self._save_related_lists(
-                    insert, dto, entity, partial_update, response_dto, aditional_filters)
+                    insert, dto, entity, partial_update, response_dto, aditional_filters
+                )
 
             # Retornando o DTO de resposta
             return response_dto
 
         except:
             if manage_transaction:
                 self._dao.rollback()
@@ -416,42 +404,42 @@
     def _save_related_lists(
         self,
         insert: bool,
         dto: DTOBase,
         entity: EntityBase,
         partial_update: bool,
         response_dto: DTOBase,
-        aditional_filters: Dict[str, Any] = None
+        aditional_filters: Dict[str, Any] = None,
     ):
-
         # TODO Controlar profundidade?!
 
         # Handling each related list
         for master_dto_field, list_field in self._dto_class.list_fields_map.items():
             response_list = []
 
             # Recuperando a lista de DTOs a salvar
             detail_list = getattr(dto, master_dto_field)
 
             # Verificando se lista está preenchida
             if detail_list is None:
                 continue
 
             # Recuperna uma instância do DAO da Entidade Detalhe
-            detail_dao = DAOBase(self._injector_factory.db_adapter(),
-                                 list_field.entity_type)
+            detail_dao = DAOBase(
+                self._injector_factory.db_adapter(), list_field.entity_type
+            )
 
             # Getting service instance
             # TODO Refatorar para suportar services customizados
             detail_service = ServiceBase(
                 self._injector_factory,
                 detail_dao,
                 list_field.dto_type,
                 list_field.entity_type,
-                list_field.dto_post_response_type
+                list_field.dto_post_response_type,
             )
 
             # Recuperando o valor da PK da entidade principal
             entity_pk_field = entity.get_pk_field()
             pk_value = getattr(entity, entity_pk_field)
 
             # Montando um mapa com os campos de relacionamento (para gravar nas entidades relacionadas)
@@ -459,137 +447,140 @@
                 list_field.related_entity_field: pk_value,
             }
 
             # Recuperando todos os IDs dos itens de lista já salvos no BD (se for um update)
             old_detail_ids = None
             if not insert:
                 # Montando o filtro para recuperar os objetos detalhe pré-existentes
-                relation_condiction = Filter(
-                    FilterOperator.EQUALS,
-                    pk_value
-                )
+                relation_condiction = Filter(FilterOperator.EQUALS, pk_value)
 
                 relation_filter = {
                     list_field.related_entity_field: [relation_condiction]
                 }
 
                 # Tratando campos de particionamento
                 for field in self._dto_class.partition_fields:
                     if field in list_field.dto_type.partition_fields:
-                        relation_filter[field] = [Filter(
-                            FilterOperator.EQUALS,
-                            getattr(dto, field)
-                        )]
+                        relation_filter[field] = [
+                            Filter(FilterOperator.EQUALS, getattr(dto, field))
+                        ]
 
                 # Recuperando do BD
                 old_detail_ids = detail_dao.list_ids(relation_filter)
-            
+
             # Lista de DTOs detalhes a criar ou atualizar
             detail_upsert_list = []
 
             # Salvando cada DTO detalhe
             for detail_dto in detail_list:
-
                 # Recuperando o ID da entidade relacionada
                 detail_pk_field = detail_dto.__class__.pk_field
                 detail_pk = getattr(detail_dto, detail_pk_field)
 
                 # Verificando se é um update ou insert
                 is_detail_insert = True
                 if old_detail_ids is not None and detail_pk in old_detail_ids:
                     is_detail_insert = False
                     old_detail_ids.remove(detail_pk)
 
                 # Checking if pk_field exists
                 if self._dto_class.pk_field is None:
                     raise DTOListFieldConfigException(
-                        f"PK field not found in class: {self._dto_class}")
+                        f"PK field not found in class: {self._dto_class}"
+                    )
 
                 if not (self._dto_class.pk_field in dto.__dict__):
                     raise DTOListFieldConfigException(
-                        f"PK field not found in DTO: {self._dto_class}")
+                        f"PK field not found in DTO: {self._dto_class}"
+                    )
 
                 # Salvando o dto dependende (detalhe) na lista
-                detail_upsert_list.append({
-                    'is_detail_insert': is_detail_insert,
-                    'detail_dto': detail_dto,
-                    'detail_pk': detail_pk
-                })
+                detail_upsert_list.append(
+                    {
+                        "is_detail_insert": is_detail_insert,
+                        "detail_dto": detail_dto,
+                        "detail_pk": detail_pk,
+                    }
+                )
 
             # Verificando se sobraram relacionamentos anteriores para remover
-            if not partial_update and old_detail_ids is not None and len(old_detail_ids) > 0:
-
+            if (
+                not partial_update
+                and old_detail_ids is not None
+                and len(old_detail_ids) > 0
+            ):
                 for old_id in old_detail_ids:
                     # Apagando cada relacionamento removido
                     detail_service.delete(old_id, aditional_filters)
-            
+
             # Salvando cada DTO detalhe
             for item in detail_upsert_list:
                 response_detail_dto = detail_service._save(
-                    item["is_detail_insert"], item["detail_dto"], False, partial_update, relation_field_map, item["detail_pk"])
+                    item["is_detail_insert"],
+                    item["detail_dto"],
+                    False,
+                    partial_update,
+                    relation_field_map,
+                    item["detail_pk"],
+                )
 
                 # Guardando o DTO na lista de retorno
                 response_list.append(response_detail_dto)
 
             # Setting dto property
-            if response_dto is not None and master_dto_field in response_dto.list_fields_map and list_field.dto_post_response_type is not None:
+            if (
+                response_dto is not None
+                and master_dto_field in response_dto.list_fields_map
+                and list_field.dto_post_response_type is not None
+            ):
                 setattr(response_dto, master_dto_field, response_list)
 
-    def delete(
-        self,
-        id: Any,
-        additional_filters: Dict[str, Any] = None
-    ) -> DTOBase:
-        self._delete(id,manage_transaction=True,additional_filters=additional_filters)
-        
+    def delete(self, id: Any, additional_filters: Dict[str, Any] = None) -> DTOBase:
+        self._delete(id, manage_transaction=True,
+                     additional_filters=additional_filters)
 
     def entity_exists(self, entity: EntityBase, partition_fields: Dict[str, Any]):
         # Getting values
         entity_pk_field = entity.get_pk_field()
         entity_pk_value = getattr(entity, entity_pk_field)
-        
 
         if entity_pk_value is None:
             return False
 
         # Searching entity in DB
         try:
-            self._dao.get(entity_pk_value, [entity.get_pk_field(
-            )], partition_fields)
+            self._dao.get(entity_pk_value, [
+                          entity.get_pk_field()], partition_fields)
         except NotFoundException as e:
             return False
 
         return True
 
     def _delete(
         self,
         id: str,
         manage_transaction: bool,
-        additional_filters: Dict[str, Any] = None
+        additional_filters: Dict[str, Any] = None,
     ) -> DTOBase:
-
         try:
             if manage_transaction:
                 self._dao.begin()
 
             # Convertendo os filtros para os filtros de entidade
             entity_filters = {}
             if additional_filters is not None:
-                entity_filters = self._create_entity_filters(additional_filters)
+                entity_filters = self._create_entity_filters(
+                    additional_filters)
 
             # Adicionando o ID nos filtros
-            id_condiction = Filter(
-                FilterOperator.EQUALS,
-                id
-            )
+            id_condiction = Filter(FilterOperator.EQUALS, id)
 
             pk_field = self._entity_class().get_pk_field()
             entity_filters[pk_field] = [id_condiction]
 
-            
             # Tratando das propriedades de lista
             if len(self._dto_class.list_fields_map) > 0:
                 self._delete_related_lists(id, additional_filters)
 
             # Excluindo a entity principal
             self._dao.delete(entity_filters)
 
@@ -597,54 +588,52 @@
             if manage_transaction:
                 self._dao.rollback()
             raise
         finally:
             if manage_transaction:
                 self._dao.commit()
 
-    def _delete_related_lists(
-        self,
-        id,
-        additional_filters: Dict[str, Any] = None
-    ):
-
+    def _delete_related_lists(self, id, additional_filters: Dict[str, Any] = None):
         # Handling each related list
         for _, list_field in self._dto_class.list_fields_map.items():
-
             # Getting service instance
             # TODO Refatorar para suportar services customizados
             service = ServiceBase(
                 self._injector_factory,
                 DAOBase(self._injector_factory.db_adapter(),
                         list_field.entity_type),
                 list_field.dto_type,
-                list_field.entity_type
+                list_field.entity_type,
             )
 
             # Making filter to relation
             filters = {
                 # TODO Adicionar os campos de particionamento de dados
                 list_field.related_entity_field: id
             }
 
             # Getting related data
             related_dto_list = service.list(
                 None, None, {"root": set()}, None, filters)
 
             # Excluindo cada entidade detalhe
             for related_dto in related_dto_list:
-
                 # Checking if pk_field exists
                 if list_field.dto_type.pk_field is None:
                     raise DTOListFieldConfigException(
-                        f"PK field not found in class: {self._dto_class}")
+                        f"PK field not found in class: {self._dto_class}"
+                    )
 
                 if not (list_field.dto_type.pk_field in related_dto.__dict__):
                     raise DTOListFieldConfigException(
-                        f"PK field not found in DTO: {self._dto_class}")
+                        f"PK field not found in DTO: {self._dto_class}"
+                    )
 
                 # Recuperando o ID da entidade detalhe
-                related_id = getattr(
-                    related_dto, list_field.dto_type.pk_field)
+                related_id = getattr(related_dto, list_field.dto_type.pk_field)
 
                 # Chamando a exclusão recursivamente
-                service._delete(related_id, manage_transaction=False, additional_filters=additional_filters)
+                service._delete(
+                    related_id,
+                    manage_transaction=False,
+                    additional_filters=additional_filters,
+                )
```

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.1.0/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.1.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

