# Comparing `tmp/splight-lib-3.0.3.dev0.tar.gz` & `tmp/splight-lib-3.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.0.3.dev0.tar", last modified: Mon Jun 26 16:40:44 2023, max compression
+gzip compressed data, was "splight-lib-3.1.0.dev0.tar", last modified: Wed Jun 21 13:10:10 2023, max compression
```

## Comparing `splight-lib-3.0.3.dev0.tar` & `splight-lib-3.1.0.dev0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.555617 splight-lib-3.0.3.dev0/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.555617 splight-lib-3.0.3.dev0/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.555617 splight-lib-3.0.3.dev0/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.555617 splight-lib-3.0.3.dev0/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.559617 splight-lib-3.0.3.dev0/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:40:44.551617 splight-lib-3.0.3.dev0/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 16:40:44.000000 splight-lib-3.0.3.dev0/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.065055 splight-lib-3.1.0.dev0/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.069055 splight-lib-3.1.0.dev0/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-21 13:10:09.000000 splight-lib-3.1.0.dev0/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:10:10.061055 splight-lib-3.1.0.dev0/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 13:10:10.000000 splight-lib-3.1.0.dev0/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.0.3.dev0/PKG-INFO` & `splight-lib-3.1.0.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.3.dev0
+Version: 3.1.0.dev0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.3.dev0/setup.py` & `splight-lib-3.1.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.0.3.dev0",
+    version="3.1.0.dev0",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib/abstract/client.py` & `splight-lib-3.1.0.dev0/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.0.dev0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/database/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/database/builder.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/database/classmap.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/database/local_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 from splight_lib.client.database.abstract import AbstractDatabaseClient
 from splight_lib.client.exceptions import InstanceNotFound
 from splight_lib.client.filter import value_filter_on_tuple
 from splight_lib.logging._internal import LogTags, get_splight_logger
 
 logger = get_splight_logger()
 
-LOCAL_DB_FILE = "splight-db.json"
-
 
 class LocalDatabaseClient(AbstractDatabaseClient):
     """Database Client implementation for a local database that uses a
     JSON file.
     """
 
     def __init__(self, path: str, *args, **kwargs):
         super().__init__()
-        self._db_file = os.path.join(path, LOCAL_DB_FILE)
+        self._db_file = os.path.join(path, "splight-db.json")
 
         if not os.path.exists(self._db_file):
             self._save_db(self._db_file, {})
         logger.debug(
             "Local database client initialized.", tags=LogTags.DATABASE
         )
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 class LocalDatalakeClient(AbstractDatalakeClient):
     """Datalake client implementation for a storing locally documents
     in different files.
     """
 
     _DEFAULT = "default"
     _PREFIX = "splight-dl_"
-    _SUFFIX = ".json"
     _TOTAL_DOCS = 10000
 
     def __init__(self, path: str, *args, **kwargs):
         super().__init__()
         self._base_path = path
         logger.info(
             "Local datalake client initialized.", tags=LogTags.DATALAKE
@@ -156,8 +155,8 @@
         for key, value in filters.items():
             if value is None:
                 continue
             new_filters[key] = value
         return new_filters
 
     def _get_file_name(self, collection: str) -> str:
-        return f"{self._PREFIX}{collection}{self._SUFFIX}"
+        return f"{self._PREFIX}{collection}"
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/file_handler.py` & `splight-lib-3.1.0.dev0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/filter.py` & `splight-lib-3.1.0.dev0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/client/hub/client.py` & `splight-lib-3.1.0.dev0/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/communication/event_handler.py` & `splight-lib-3.1.0.dev0/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/component/abstract.py` & `splight-lib-3.1.0.dev0/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/component/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/component/spec.py` & `splight-lib-3.1.0.dev0/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/encryption.py` & `splight-lib-3.1.0.dev0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/execution.py` & `splight-lib-3.1.0.dev0/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/logging/_internal.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/logging/component.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/logging/logging.py` & `splight-lib-3.1.0.dev0/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/__init__.py` & `splight-lib-3.1.0.dev0/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/alert.py` & `splight-lib-3.1.0.dev0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/asset.py` & `splight-lib-3.1.0.dev0/splight_lib/models/asset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from typing import Any, List, Optional
 
 from geojson_pydantic import GeometryCollection, Point
-from pydantic import BaseModel
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.base import SplightDatabaseBaseModel
 
 
+class Tag:
+    name: str
+    description: Optional[str] = None
+
+
 class Asset(SplightDatabaseBaseModel):
     id: Optional[str]
     name: str
     description: Optional[str] = None
-    tags: List[str] = []
+    tags: List[Tag] = []
     attributes: List[Attribute] = []
     verified: bool = False
     geometry: Optional[GeometryCollection]
     centroid: Optional[Point]
     external_id: Optional[str] = None
     is_public: bool = False
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/base.py` & `splight-lib-3.1.0.dev0/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/communication.py` & `splight-lib-3.1.0.dev0/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/component.py` & `splight-lib-3.1.0.dev0/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/event.py` & `splight-lib-3.1.0.dev0/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/file.py` & `splight-lib-3.1.0.dev0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/hub.py` & `splight-lib-3.1.0.dev0/splight_lib/models/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,22 +158,21 @@
         file_name = f"{name}-{version}.{COMPRESSION_TYPE}"
         ignore_pathspec = get_ignore_pathspec(path)
         versioned_name = f"{name}-{version}"
         readme_path = os.path.join(path, README_FILE_1)
         if not os.path.exists(readme_path):
             readme_path = os.path.join(path, README_FILE_2)
         with py7zr.SevenZipFile(file_name, "w") as archive:
+
             all_files = glob(f"{path}/**", recursive=True)
             for filename in all_files:
-                if ignore_pathspec and ignore_pathspec.match_file(filename):
-                    continue
-                if os.path.isdir(filename):
+                filepath = os.path.join(path, filename)
+                if ignore_pathspec and ignore_pathspec.match_file(filepath):
                     continue
-                filepath = filename.replace(path, f"{versioned_name}/")
-                archive.write(filename, filepath)
+                archive.write(filepath, os.path.join(versioned_name, filename))
 
         data = {
             "name": name,
             "version": version,
             "splight_cli_version": spec["splight_cli_version"],
             "privacy_policy": spec.get("privacy_policy", "private"),
             "tags": spec.get("tags", []),
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/native.py` & `splight-lib-3.1.0.dev0/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/query.py` & `splight-lib-3.1.0.dev0/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/models/setpoint.py` & `splight-lib-3.1.0.dev0/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/restclient/client.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/restclient/types.py` & `splight-lib-3.1.0.dev0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/settings.py` & `splight-lib-3.1.0.dev0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/testing/__init__.py` & `splight-lib-3.1.0.dev0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/utils/custom_model.py` & `splight-lib-3.1.0.dev0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/utils/hub.py` & `splight-lib-3.1.0.dev0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib/webhook.py` & `splight-lib-3.1.0.dev0/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.1.0.dev0/splight_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.0.3.dev0
+Version: 3.1.0.dev0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.0.3.dev0/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.0.dev0/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.0.3.dev0/splight_lib.egg-info/requires.txt` & `splight-lib-3.1.0.dev0/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*

