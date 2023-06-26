# Comparing `tmp/runtimepy-1.6.0.tar.gz` & `tmp/runtimepy-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.6.0.tar", last modified: Mon Jun 26 03:52:36 2023, max compression
+gzip compressed data, was "runtimepy-1.7.0.tar", last modified: Mon Jun 26 08:30:41 2023, max compression
```

## Comparing `runtimepy-1.6.0.tar` & `runtimepy-1.7.0.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.962517 runtimepy-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 03:50:18.000000 runtimepy-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 03:52:36.958517 runtimepy-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-26 03:50:18.000000 runtimepy-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 03:50:18.000000 runtimepy-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.934517 runtimepy-1.6.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:52:36.962517 runtimepy-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 03:50:18.000000 runtimepy-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 08:29:19.000000 runtimepy-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 08:30:41.862507 runtimepy-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-26 08:29:19.000000 runtimepy-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 08:29:19.000000 runtimepy-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.846507 runtimepy-1.7.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.854507 runtimepy-1.7.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/factory/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.858507 runtimepy-1.7.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/task/basic/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 08:29:19.000000 runtimepy-1.7.0/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.850507 runtimepy-1.7.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 08:30:41.000000 runtimepy-1.7.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:30:41.862507 runtimepy-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 08:29:19.000000 runtimepy-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:30:41.862507 runtimepy-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 08:29:19.000000 runtimepy-1.7.0/tests/test_resources.py
```

### Comparing `runtimepy-1.6.0/LICENSE` & `runtimepy-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/PKG-INFO` & `runtimepy-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.6.0
+Version: 1.7.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d94e863595f8d7f340e96c0820f3b232
+    hash=6a3f7b1658909aed705809485a62426b
     =====================================
 -->
 
-# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.6.0/README.md` & `runtimepy-1.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d94e863595f8d7f340e96c0820f3b232
+    hash=6a3f7b1658909aed705809485a62426b
     =====================================
 -->
 
-# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.6.0/pyproject.toml` & `runtimepy-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.6.0"
+version = "1.7.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.6.0/runtimepy/app.py` & `runtimepy-1.7.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/__init__.py` & `runtimepy-1.7.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/__init__.py` & `runtimepy-1.7.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/array.py` & `runtimepy-1.7.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/base.py` & `runtimepy-1.7.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/create.py` & `runtimepy-1.7.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/file.py` & `runtimepy-1.7.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/environment/names.py` & `runtimepy-1.7.0/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/channel/registry.py` & `runtimepy-1.7.0/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/codec/protocol/base.py` & `runtimepy-1.7.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/codec/protocol/json.py` & `runtimepy-1.7.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/commands/all.py` & `runtimepy-1.7.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/commands/arbiter.py` & `runtimepy-1.7.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/commands/tui.py` & `runtimepy-1.7.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.7.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.7.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/entry.py` & `runtimepy-1.7.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/enum/__init__.py` & `runtimepy-1.7.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/enum/registry.py` & `runtimepy-1.7.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/enum/type.py` & `runtimepy-1.7.0/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/mapping.py` & `runtimepy-1.7.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/mixins/enum.py` & `runtimepy-1.7.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/mixins/regex.py` & `runtimepy-1.7.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/__init__.py` & `runtimepy-1.7.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/base.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/config.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/imports.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/info.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/task.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/udp.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.7.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/connection.py` & `runtimepy-1.7.0/runtimepy/net/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from typing import Union as _Union
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 
+# internal
+from runtimepy.net.metrics import ConnectionMetrics
+
 BinaryMessage = _Union[bytes, bytearray, memoryview]
 
 
 class Connection(_LoggerMixin, _ABC):
     """A connection interface."""
 
     uses_text_tx_queue = True
@@ -38,19 +41,26 @@
 
         # A queue for out-going binary messages. Connections that don't use
         # this can set 'uses_binary_tx_queue' to False to avoid scheduling a
         # task for it.
         self._binary_messages: _asyncio.Queue[BinaryMessage] = _asyncio.Queue()
         self.tx_binary_hwm: int = 0
 
+        self.metrics = ConnectionMetrics()
+
         self._tasks: _List[_asyncio.Task[None]] = []
         self.initialized = _asyncio.Event()
         self.disabled_event = _asyncio.Event()
         self.init()
 
+    def reset_metrics(self) -> None:
+        """Reset connection metrics."""
+        self.metrics.tx.reset()
+        self.metrics.rx.reset()
+
     def init(self) -> None:
         """Initialize this instance."""
 
     async def async_init(self) -> bool:
         """A runtime initialization routine (executes during 'process')."""
         return True
```

### Comparing `runtimepy-1.6.0/runtimepy/net/factories/__init__.py` & `runtimepy-1.7.0/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/manager.py` & `runtimepy-1.7.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/mixin.py` & `runtimepy-1.7.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/tcp/connection.py` & `runtimepy-1.7.0/runtimepy/net/tcp/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,28 @@
 
         self._protocol = protocol
         self._protocol.conn = self
         super().__init__(_getLogger(self.logger_name("TCP ")))
 
     async def _await_message(self) -> _Optional[_Union[_BinaryMessage, str]]:
         """Await the next message. Return None on error or failure."""
-        return await self._protocol.queue.get()
+
+        data = await self._protocol.queue.get()
+        if data is not None:
+            self.metrics.rx.increment(len(data))
+        return data
 
     def send_text(self, data: str) -> None:
         """Enqueue a text message to send."""
-        self._transport.write(data.encode())
+        self.send_binary(data.encode())
 
     def send_binary(self, data: _BinaryMessage) -> None:
         """Enqueue a binary message tos end."""
         self._transport.write(data)
+        self.metrics.tx.increment(len(data))
 
     @classmethod
     async def create_connection(cls: _Type[T], **kwargs) -> T:
         """Create a TCP connection."""
 
         eloop = _get_event_loop()
```

### Comparing `runtimepy-1.6.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.7.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.7.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/udp/connection.py` & `runtimepy-1.7.0/runtimepy/net/udp/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     def sendto(
         self, data: bytes, addr: _Union[IpHost, _Tuple[str, int]] = None
     ) -> None:
         """Send to a specific address."""
 
         try:
             self._transport.sendto(data, addr=addr)
+            self.metrics.tx.increment(len(data))
 
         # Catch a bug in the underlying event loop implementation - we try to
         # send, but the underlying socket is gone (e.g. attribute is 'None').
         # This seems to be possible (but intermittent) when shutting down the
         # application.
         except AttributeError as exc:
             self.disable(str(exc))
@@ -187,17 +188,17 @@
         with _suppress(KeyboardInterrupt):
             while self._enabled:
                 # Attempt to get the next message.
                 message = await self._protocol.queue.get()
                 result = False
 
                 if message is not None:
-                    result = await self.process_datagram(
-                        message[0], message[1]
-                    )
+                    data = message[0]
+                    result = await self.process_datagram(data, message[1])
+                    self.metrics.rx.increment(len(data))
 
                 # If we failed to read a message, disable.
                 if not result:
                     self.disable("read processing error")
 
 
 class EchoUdpConnection(UdpConnection, _EchoConnection):
```

### Comparing `runtimepy-1.6.0/runtimepy/net/util.py` & `runtimepy-1.7.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/net/websocket/connection.py` & `runtimepy-1.7.0/runtimepy/net/websocket/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,29 @@
             result = await task
         except _ConnectionClosed:
             self.disable("connection closed")
         return result
 
     async def _await_message(self) -> _Optional[_Union[BinaryMessage, str]]:
         """Await the next message. Return None on error or failure."""
-        return await self._handle_connection_closed(self.protocol.recv())
+
+        data = await self._handle_connection_closed(self.protocol.recv())
+        if data is not None:
+            self.metrics.rx.increment(len(data))
+        return data
 
     async def _send_text_message(self, data: str) -> None:
         """Send a text message."""
         await self._handle_connection_closed(self.protocol.send(data))
+        self.metrics.tx.increment(len(data))
 
     async def _send_binay_message(self, data: BinaryMessage) -> None:
         """Send a binary message."""
         await self._handle_connection_closed(self.protocol.send(data))
+        self.metrics.tx.increment(len(data))
 
     async def close(self) -> None:
         """Close this connection."""
         await self.protocol.close()
 
     @classmethod
     async def create_connection(cls: _Type[T], uri: str, **kwargs) -> T:
```

### Comparing `runtimepy-1.6.0/runtimepy/primitives/__init__.py` & `runtimepy-1.7.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/array.py` & `runtimepy-1.7.0/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/base.py` & `runtimepy-1.7.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/bool.py` & `runtimepy-1.7.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/byte_order.py` & `runtimepy-1.7.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/field/__init__.py` & `runtimepy-1.7.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/field/fields.py` & `runtimepy-1.7.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.7.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.7.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/float.py` & `runtimepy-1.7.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/int.py` & `runtimepy-1.7.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/string.py` & `runtimepy-1.7.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/type/__init__.py` & `runtimepy-1.7.0/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/type/base.py` & `runtimepy-1.7.0/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/type/float.py` & `runtimepy-1.7.0/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/primitives/type/int.py` & `runtimepy-1.7.0/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/registry/__init__.py` & `runtimepy-1.7.0/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/registry/bool.py` & `runtimepy-1.7.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/registry/item.py` & `runtimepy-1.7.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/registry/name.py` & `runtimepy-1.7.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/schemas.py` & `runtimepy-1.7.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/task/asynchronous.py` & `runtimepy-1.7.0/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/task/basic/manager.py` & `runtimepy-1.7.0/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/task/basic/metrics.py` & `runtimepy-1.7.0/runtimepy/task/basic/metrics.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/task/basic/periodic.py` & `runtimepy-1.7.0/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/tui/channels/__init__.py` & `runtimepy-1.7.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy/tui/task.py` & `runtimepy-1.7.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.7.0/runtimepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.6.0
+Version: 1.7.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,19 +21,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=d94e863595f8d7f340e96c0820f3b232
+    hash=6a3f7b1658909aed705809485a62426b
     =====================================
 -->
 
-# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.7.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-1.6.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.7.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 runtimepy/enum/type.py
 runtimepy/mixins/__init__.py
 runtimepy/mixins/enum.py
 runtimepy/mixins/regex.py
 runtimepy/net/__init__.py
 runtimepy/net/connection.py
 runtimepy/net/manager.py
+runtimepy/net/metrics.py
 runtimepy/net/mixin.py
 runtimepy/net/util.py
 runtimepy/net/apps/__init__.py
 runtimepy/net/arbiter/__init__.py
 runtimepy/net/arbiter/base.py
 runtimepy/net/arbiter/config.py
 runtimepy/net/arbiter/imports.py
```

### Comparing `runtimepy-1.6.0/setup.py` & `runtimepy-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/tests/test_entry.py` & `runtimepy-1.7.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.6.0/tests/test_mapping.py` & `runtimepy-1.7.0/tests/test_mapping.py`

 * *Files identical despite different names*

