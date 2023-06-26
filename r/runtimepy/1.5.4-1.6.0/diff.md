# Comparing `tmp/runtimepy-1.5.4.tar.gz` & `tmp/runtimepy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.5.4.tar", last modified: Wed May 31 22:10:17 2023, max compression
+gzip compressed data, was "runtimepy-1.6.0.tar", last modified: Mon Jun 26 03:52:36 2023, max compression
```

## Comparing `runtimepy-1.5.4.tar` & `runtimepy-1.6.0.tar`

### file list

```diff
@@ -1,136 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 22:08:49.000000 runtimepy-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-31 22:10:17.342651 runtimepy-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-31 22:08:49.000000 runtimepy-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-31 22:08:49.000000 runtimepy-1.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.326651 runtimepy-1.5.4/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.334651 runtimepy-1.5.4/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.338651 runtimepy-1.5.4/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 22:08:49.000000 runtimepy-1.5.4/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.330651 runtimepy-1.5.4/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 22:10:17.000000 runtimepy-1.5.4/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:10:17.342651 runtimepy-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-31 22:08:49.000000 runtimepy-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:10:17.342651 runtimepy-1.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 22:08:49.000000 runtimepy-1.5.4/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.962517 runtimepy-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 03:50:18.000000 runtimepy-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 03:52:36.958517 runtimepy-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-26 03:50:18.000000 runtimepy-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 03:50:18.000000 runtimepy-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.942517 runtimepy-1.6.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.934517 runtimepy-1.6.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.946517 runtimepy-1.6.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/factory/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.950517 runtimepy-1.6.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.954517 runtimepy-1.6.0/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/task/basic/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 03:50:18.000000 runtimepy-1.6.0/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.938516 runtimepy-1.6.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 03:52:36.000000 runtimepy-1.6.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 03:52:36.962517 runtimepy-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 03:50:18.000000 runtimepy-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 03:52:36.958517 runtimepy-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 03:50:18.000000 runtimepy-1.6.0/tests/test_resources.py
```

### Comparing `runtimepy-1.5.4/LICENSE` & `runtimepy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/PKG-INFO` & `runtimepy-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.5.4
+Version: 1.6.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3bc7656b5df806d21148ec2b5b2c0082
+    hash=d94e863595f8d7f340e96c0820f3b232
     =====================================
 -->
 
-# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -43,15 +42,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `runtimepy-1.5.4/README.md` & `runtimepy-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3bc7656b5df806d21148ec2b5b2c0082
+    hash=d94e863595f8d7f340e96c0820f3b232
     =====================================
 -->
 
-# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -19,15 +19,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `runtimepy-1.5.4/pyproject.toml` & `runtimepy-1.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.5.4"
+version = "1.6.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
```

### Comparing `runtimepy-1.5.4/runtimepy/app.py` & `runtimepy-1.6.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/__init__.py` & `runtimepy-1.6.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/__init__.py` & `runtimepy-1.6.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/array.py` & `runtimepy-1.6.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/base.py` & `runtimepy-1.6.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/create.py` & `runtimepy-1.6.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/file.py` & `runtimepy-1.6.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/environment/names.py` & `runtimepy-1.6.0/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/channel/registry.py` & `runtimepy-1.6.0/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/codec/protocol/base.py` & `runtimepy-1.6.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/codec/protocol/json.py` & `runtimepy-1.6.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/commands/all.py` & `runtimepy-1.6.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/commands/arbiter.py` & `runtimepy-1.6.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/commands/tui.py` & `runtimepy-1.6.0/runtimepy/commands/tui.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 import asyncio as _asyncio
 import curses as _curses
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
-from vcorelib.asyncio import run_handle_interrupt as _run_handle_interrupt
+from vcorelib.asyncio import run_handle_stop as _run_handle_stop
 
 # internal
 from runtimepy.channel.environment import (
     ChannelEnvironment as _ChannelEnvironment,
 )
 from runtimepy.tui.channels import CursesWindow as _CursesWindow
 from runtimepy.tui.task import TuiTask as _TuiTask
@@ -25,18 +25,16 @@
 
     task = _TuiTask(
         "ui",
         1 / args.rate,
         _ChannelEnvironment(),
         max_iterations=args.iterations,
     )
-
-    eloop = _asyncio.new_event_loop()
-    _asyncio.set_event_loop(eloop)
-    _run_handle_interrupt(task.run(window), eloop)
+    stop_sig = _asyncio.Event()
+    return _run_handle_stop(stop_sig, task.run(window, stop_sig=stop_sig))
 
 
 def tui_cmd(args: _Namespace) -> int:
     """Execute the tui command."""
 
     getattr(_curses, "wrapper")(start, args)
     return 0
```

### Comparing `runtimepy-1.5.4/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.6.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-1.6.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,19 @@
       $ref: package://runtimepy/schemas/ClientConnectionConfig.yaml
 
   servers:
     type: array
     items:
       $ref: package://runtimepy/schemas/ServerConnectionConfig.yaml
 
+  tasks:
+    type: array
+    items:
+      $ref: package://runtimepy/schemas/TaskConfig.yaml
+
   # Runtime application or applications.
   # defaults to: "runtimepy.net.apps.init_only"
   app:
     oneOf:
       - type: string
       - type: array
         items:
```

### Comparing `runtimepy-1.5.4/runtimepy/entry.py` & `runtimepy-1.6.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/enum/__init__.py` & `runtimepy-1.6.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/enum/registry.py` & `runtimepy-1.6.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/enum/type.py` & `runtimepy-1.6.0/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/mapping.py` & `runtimepy-1.6.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/mixins/enum.py` & `runtimepy-1.6.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/mixins/regex.py` & `runtimepy-1.6.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/__init__.py` & `runtimepy-1.6.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/base.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 from vcorelib.namespace import NamespaceMixin as _NamespaceMixin
 
 # internal
 from runtimepy.net.arbiter.info import AppInfo, ConnectionMap
+from runtimepy.net.arbiter.task import (
+    ArbiterTaskManager as _ArbiterTaskManager,
+)
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 
 NetworkApplication = _Callable[[AppInfo], _Awaitable[int]]
 NetworkApplicationlike = _Union[NetworkApplication, _List[NetworkApplication]]
 ServerTask = _Awaitable[None]
 
@@ -71,14 +74,16 @@
 
         _LoggerMixin.__init__(self, logger=logger)
 
         if manager is None:
             manager = _ConnectionManager()
         self.manager = manager
 
+        self.task_manager = _ArbiterTaskManager()
+
         if stop_sig is None:
             stop_sig = _asyncio.Event()
         self.stop_sig = stop_sig
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
         # A fallback application. Set a class attribute so this can be more
@@ -183,26 +188,42 @@
                         stack,
                         self._connections,
                         self._namespace,
                         self.stop_sig,
                         config if config is not None else self._config,
                     )
 
+                    # Initialize tasks.
+                    await _asyncio.gather(
+                        *(x.init(info) for x in self.task_manager.tasks)
+                    )
+
+                    # Start tasks.
+                    await stack.enter_async_context(
+                        self.task_manager.running(stop_sig=self.stop_sig)
+                    )
+
                     # Get application methods.
                     apps = self._apps
                     if app is not None:
                         apps = normalize_app(app)
 
                     result = 0
                     for curr_app in apps:
                         if result == 0:
                             info.logger = _getLogger(curr_app.__name__)
                             info.logger.info("Starting.")
-                            result = await curr_app(info)
-                            info.logger.info("Returned %d.", result)
+                            try:
+                                result = await curr_app(info)
+                                info.logger.info("Returned %d.", result)
+                            except AssertionError as exc:
+                                info.logger.exception(
+                                    "Failed an assertion:", exc_info=exc
+                                )
+                                result = -1
 
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
             self.stop_sig.set()
 
         return result
```

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/config.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         self.config: _Optional[_JsonObject] = _cast(
             _JsonObject, data.get("config")
         )
 
         self.factories: _List[_Any] = data.get("factories", [])  # type: ignore
         self.clients: _List[_Any] = data.get("clients", [])  # type: ignore
         self.servers: _List[_Any] = data.get("servers", [])  # type: ignore
+        self.tasks: _List[_Any] = data.get("tasks", [])  # type: ignore
 
         self.directory = _Path(str(data.get("directory", ".")))
 
     def asdict(self) -> _JsonObject:
         """Obtain a dictionary representing this instance."""
         return self.data
 
@@ -179,14 +180,25 @@
                     server.get("args", []), env=config.ports  # type: ignore
                 ),
                 **dict_resolve_env_vars(
                     server.get("kwargs", {}), env=config.ports  # type: ignore
                 ),
             ), f"Couldn't register a '{factory}' server!"
 
+        # Register tasks.
+        for task in config.tasks:
+            name = task["name"]
+            factory = task["factory"]
+            assert self.factory_task(
+                factory,
+                name,
+                period_s=task["period_s"],
+                average_depth=task["average_depth"],
+            ), f"Couldn't register task '{name}' ({factory})!"
+
         # Set the new application entry if it's set.
         if config.app is not None:
             self.set_app(config.app)
 
         # Update application configuration data if necessary.
         if config.config is not None:
             self._config = config.config
```

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/factory.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,33 +45,36 @@
     used for creating new connections (that can then be registered).
     """
 
     def _init(self) -> None:
         """Additional initialization tasks."""
 
         super()._init()
-        self._factories: _Dict[str, ConnectionFactory] = {}
-        self._names: _Dict[ConnectionFactory, _List[str]] = {}
+        self._conn_factories: _Dict[str, ConnectionFactory] = {}
+        self._conn_names: _Dict[ConnectionFactory, _List[str]] = {}
 
-    def register_factory(
+    def register_connection_factory(
         self, factory: ConnectionFactory, *namespaces: str
     ) -> bool:
         """Attempt to register a connection factory."""
 
         result = False
 
         assert isinstance(factory, ConnectionFactory), factory
 
         name = factory.__class__.__name__
         snake_name = obj_class_to_snake(factory)
 
-        if name not in self._factories and snake_name not in self._factories:
-            self._factories[name] = factory
-            self._factories[snake_name] = factory
-            self._names[factory] = [*namespaces]
+        if (
+            name not in self._conn_factories
+            and snake_name not in self._conn_factories
+        ):
+            self._conn_factories[name] = factory
+            self._conn_factories[snake_name] = factory
+            self._conn_names[factory] = [*namespaces]
 
             result = True
             self.logger.info(
                 "Registered '%s' (%s) connection factory.", name, snake_name
             )
 
         return result
@@ -81,34 +84,34 @@
     ) -> bool:
         """
         Attempt to register a client connection using a registered factory.
         """
 
         result = False
 
-        if factory in self._factories:
-            factory_inst = self._factories[factory]
+        if factory in self._conn_factories:
+            factory_inst = self._conn_factories[factory]
 
             conn = factory_inst.client(*args, **kwargs)
             if not defer:
                 conn = await conn  # type: ignore
 
             result = self.register_connection(
-                conn, *self._names[factory_inst], name
+                conn, *self._conn_names[factory_inst], name
             )
 
         return result
 
     async def factory_server(self, factory: str, *args, **kwargs) -> bool:
         """Attempt to create a server task using a registered factory."""
 
         result = False
 
-        if factory in self._factories:
-            factory_inst = self._factories[factory]
+        if factory in self._conn_factories:
+            factory_inst = self._conn_factories[factory]
             self._servers.append(
                 await factory_inst.server_task(
                     self.stop_sig,
                     self.manager,
                     self._servers_started,
                     *args,
                     **kwargs,
```

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/info.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/udp.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.6.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/connection.py` & `runtimepy-1.6.0/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/factories/__init__.py` & `runtimepy-1.6.0/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/manager.py` & `runtimepy-1.6.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/mixin.py` & `runtimepy-1.6.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/tcp/connection.py` & `runtimepy-1.6.0/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.6.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.6.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/udp/connection.py` & `runtimepy-1.6.0/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/util.py` & `runtimepy-1.6.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/net/websocket/connection.py` & `runtimepy-1.6.0/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/__init__.py` & `runtimepy-1.6.0/runtimepy/primitives/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,34 @@
     Int64,
     Uint8,
     Uint16,
     Uint32,
     Uint64,
 )
 
+__all__ = [
+    "Bool",
+    "Double",
+    "Float",
+    "Half",
+    "Int8",
+    "Int16",
+    "Int32",
+    "Int64",
+    "Uint8",
+    "Uint16",
+    "Uint32",
+    "Uint64",
+    "AnyPrimitive",
+    "T",
+    "Primitivelike",
+    "normalize",
+    "create",
+]
+
 AnyPrimitive = _Union[
     Int8,
     Int16,
     Int32,
     Int64,
     Uint8,
     Uint16,
```

### Comparing `runtimepy-1.5.4/runtimepy/primitives/array.py` & `runtimepy-1.6.0/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/base.py` & `runtimepy-1.6.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/bool.py` & `runtimepy-1.6.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/byte_order.py` & `runtimepy-1.6.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/field/__init__.py` & `runtimepy-1.6.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/field/fields.py` & `runtimepy-1.6.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.6.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.6.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/float.py` & `runtimepy-1.6.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/int.py` & `runtimepy-1.6.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/string.py` & `runtimepy-1.6.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/type/__init__.py` & `runtimepy-1.6.0/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/type/base.py` & `runtimepy-1.6.0/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/type/float.py` & `runtimepy-1.6.0/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/primitives/type/int.py` & `runtimepy-1.6.0/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/registry/__init__.py` & `runtimepy-1.6.0/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/registry/bool.py` & `runtimepy-1.6.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/registry/item.py` & `runtimepy-1.6.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/registry/name.py` & `runtimepy-1.6.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/task/__init__.py` & `runtimepy-1.6.0/runtimepy/task/asynchronous.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,24 @@
 
 # built-in
 import asyncio as _asyncio
 from logging import getLogger as _getLogger
 
 # third-party
 from vcorelib.logging import LoggerMixin as _LoggerMixin
-from vcorelib.math.analysis.average import MovingAverage as _MovingAverage
-from vcorelib.math.analysis.rate import RateTracker as _RateTracker
-from vcorelib.math.time import nano_str as _nano_str
+from vcorelib.math import MovingAverage as _MovingAverage
+from vcorelib.math import RateTracker as _RateTracker
+from vcorelib.math import rate_str as _rate_str
 
 # internal
 from runtimepy.channel.environment import (
     ChannelEnvironment as _ChannelEnvironment,
 )
 
 
-def rate_str(period_s: float) -> str:
-    """Get a string representing a rate in Hz."""
-
-    period_str = _nano_str(int(period_s * 1e9))
-    freq_str = _nano_str(int((1.0 / period_s) * 1e9), prefix_space=True)
-    return f"{freq_str}Hz ({period_str}s)"
-
-
 class AsyncTask(_LoggerMixin):
     """A basic implementation of a periodic task."""
 
     def __init__(
         self,
         name: str,
         period_s: float,
@@ -116,25 +108,27 @@
         self.logger.info(
             "'%s' min time: %0.6fs.", self.name, self.min_s.raw.value
         )
 
     @property
     def rate_str(self) -> str:
         """Get this periodic's rate as a string."""
-        return rate_str(self.period_s.raw.value)
+        return _rate_str(self.period_s.raw.value)
 
     def enable(self) -> None:
         """Enable this task."""
         self.enabled.raw.value = True
 
     def disable(self) -> None:
         """Disable this task."""
         self.enabled.raw.value = False
 
-    async def run(self, *args, **kwargs) -> None:
+    async def run(
+        self, *args, stop_sig: _asyncio.Event = None, **kwargs
+    ) -> None:
         """Run this task while it's enabled."""
 
         eloop = _asyncio.get_running_loop()
 
         self.logger.info("Starting task '%s' at %s.", self.name, self.rate_str)
 
         self.reset_metrics()
@@ -164,15 +158,15 @@
             self.min_s.raw.value = self.dispatch_time.min
 
             # Check if we've performed the maximum specified number of
             # dispatches.
             if (
                 self.max_iterations.raw.value > 0
                 and self.dispatches.raw.value >= self.max_iterations.raw.value
-            ):
+            ) or (stop_sig is not None and stop_sig.is_set()):
                 self.disable()
 
             if self.enabled:
                 try:
                     await _asyncio.sleep(
                         max(self.period_s.raw.value - exec_time, 0)
                     )
```

### Comparing `runtimepy-1.5.4/runtimepy/task/basic/__init__.py` & `runtimepy-1.6.0/runtimepy/task/basic/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,65 @@
 """
-A module implementing a simple periodic-task interface.
+A module implementing a periodic-task manager.
 """
 
-from __future__ import annotations
-
 # built-in
-from abc import ABC as _ABC
-from abc import abstractmethod as _abstractmethod
 import asyncio as _asyncio
-from contextlib import suppress
-from logging import getLogger as _getLogger
-from typing import Optional as _Optional
-
-# third-party
-from vcorelib.logging import LoggerMixin as _LoggerMixin
+from contextlib import asynccontextmanager as _asynccontextmanager
+from typing import AsyncIterator as _AsyncIterator
+from typing import Dict as _Dict
+from typing import Generic as _Generic
+from typing import Iterator as _Iterator
+from typing import TypeVar as _TypeVar
 
 # internal
-from runtimepy.task import rate_str as _rate_str
+from runtimepy.task.basic.periodic import PeriodicTask as _PeriodicTask
+
+T = _TypeVar("T", bound=_PeriodicTask)
+
 
+class PeriodicTaskManager(_Generic[T]):
+    """A class for managing periodic tasks as a single group."""
 
-class PeriodicTask(_LoggerMixin, _ABC):
-    """A class implementing a simple periodic-task interface."""
+    def __init__(self) -> None:
+        """Initialize this instance."""
+        self._tasks: _Dict[str, T] = {}
 
-    def __init__(self, name: str) -> None:
-        """Initialize this task."""
+    def register(self, task: T, period_s: float = None) -> bool:
+        """Register a periodic task."""
 
-        self.name = name
-        super().__init__(logger=_getLogger(self.name))
-        self.enabled = False
-        self._task: _Optional[_asyncio.Task[None]] = None
-
-    @_abstractmethod
-    async def dispatch(self) -> bool:
-        """Dispatch an iteration of this task."""
-
-    async def run(
-        self, period_s: float, stop_sig: _asyncio.Event = None
-    ) -> None:
-        """
-        Run this task by executing the dispatch method at the specified period
-        until a dispatch iteration fails or the task is otherwise disabled.
-        """
-
-        assert not self.enabled
-        self.enabled = True
-
-        self.logger.info("Task starting at %s.", _rate_str(period_s))
-
-        eloop = _asyncio.get_running_loop()
-
-        while self.enabled:
-            start = eloop.time()
-            self.enabled = await _asyncio.shield(self.dispatch())
-            iter_time = eloop.time() - start
-
-            # Check this synchronously. This may not be suitable for tasks
-            # with long periods.
-            if stop_sig is not None:
-                self.enabled = not stop_sig.is_set()
-
-            if self.enabled:
-                try:
-                    await _asyncio.sleep(max(period_s - iter_time, 0))
-                except _asyncio.CancelledError:
-                    self.logger.info("Task was cancelled.")
-                    self.enabled = False
-
-        self.logger.info("Task completed.")
-
-    async def task(
-        self, period_s: float, stop_sig: _asyncio.Event = None
-    ) -> _asyncio.Task[None]:
-        """Create an event-loop task for this periodic."""
-
-        # Ensure that a previous version of this task gets cleaned up.
-        if self._task is not None:
-            if not self._task.done():
-                # On Windows, setting enabled False here is not enough.
-                self.enabled = False
-                self._task.cancel()
-                with suppress(_asyncio.CancelledError):
-                    await self._task
-            self._task = None
+        result = task.name not in self._tasks
+        if result:
+            self._tasks[task.name] = task
+            task.set_period(period_s=period_s)
+        return result
 
-        self._task = _asyncio.create_task(
-            self.run(period_s, stop_sig=stop_sig)
+    @property
+    def tasks(self) -> _Iterator[T]:
+        """Iterate over tasks."""
+        yield from self._tasks.values()
+
+    def __getitem__(self, name: str) -> T:
+        """Get a task by name."""
+        return self._tasks[name]
+
+    async def start(self, stop_sig: _asyncio.Event = None) -> None:
+        """Ensure tasks are started."""
+        await _asyncio.gather(
+            *(x.task(stop_sig=stop_sig) for x in self._tasks.values())
         )
-        return self._task
+
+    async def stop(self) -> None:
+        """Ensure tasks are stopped."""
+        await _asyncio.gather(*(x.stop() for x in self._tasks.values()))
+
+    @_asynccontextmanager
+    async def running(
+        self, stop_sig: _asyncio.Event = None
+    ) -> _AsyncIterator[None]:
+        """Run tasks as an async context."""
+
+        await self.start(stop_sig=stop_sig)
+        try:
+            yield
+        finally:
+            await self.stop()
```

### Comparing `runtimepy-1.5.4/runtimepy/tui/channels/__init__.py` & `runtimepy-1.6.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy/tui/task.py` & `runtimepy-1.6.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.6.0/runtimepy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.5.4
+Version: 1.6.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3bc7656b5df806d21148ec2b5b2c0082
+    hash=d94e863595f8d7f340e96c0820f3b232
     =====================================
 -->
 
-# runtimepy ([1.5.4](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.6.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -43,15 +42,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/runtimepy.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `runtimepy-1.5.4/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.6.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 runtimepy/data/schemas/Channel.yaml
 runtimepy/data/schemas/ChannelRegistry.yaml
 runtimepy/data/schemas/ClientConnectionConfig.yaml
 runtimepy/data/schemas/ConnectionArbiterConfig.yaml
 runtimepy/data/schemas/EnumRegistry.yaml
 runtimepy/data/schemas/RuntimeEnum.yaml
 runtimepy/data/schemas/ServerConnectionConfig.yaml
+runtimepy/data/schemas/TaskConfig.yaml
+runtimepy/data/schemas/has_factory.yaml
+runtimepy/data/schemas/has_name.yaml
 runtimepy/enum/__init__.py
 runtimepy/enum/registry.py
 runtimepy/enum/type.py
 runtimepy/mixins/__init__.py
 runtimepy/mixins/enum.py
 runtimepy/mixins/regex.py
 runtimepy/net/__init__.py
@@ -52,20 +55,23 @@
 runtimepy/net/manager.py
 runtimepy/net/mixin.py
 runtimepy/net/util.py
 runtimepy/net/apps/__init__.py
 runtimepy/net/arbiter/__init__.py
 runtimepy/net/arbiter/base.py
 runtimepy/net/arbiter/config.py
-runtimepy/net/arbiter/factory.py
 runtimepy/net/arbiter/imports.py
 runtimepy/net/arbiter/info.py
+runtimepy/net/arbiter/task.py
 runtimepy/net/arbiter/tcp.py
 runtimepy/net/arbiter/udp.py
 runtimepy/net/arbiter/websocket.py
+runtimepy/net/arbiter/factory/__init__.py
+runtimepy/net/arbiter/factory/connection.py
+runtimepy/net/arbiter/factory/task.py
 runtimepy/net/factories/__init__.py
 runtimepy/net/tcp/__init__.py
 runtimepy/net/tcp/connection.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
 runtimepy/net/udp/__init__.py
 runtimepy/net/udp/connection.py
@@ -89,15 +95,19 @@
 runtimepy/primitives/type/float.py
 runtimepy/primitives/type/int.py
 runtimepy/registry/__init__.py
 runtimepy/registry/bool.py
 runtimepy/registry/item.py
 runtimepy/registry/name.py
 runtimepy/task/__init__.py
+runtimepy/task/asynchronous.py
 runtimepy/task/basic/__init__.py
+runtimepy/task/basic/manager.py
+runtimepy/task/basic/metrics.py
+runtimepy/task/basic/periodic.py
 runtimepy/telemetry/__init__.py
 runtimepy/tui/__init__.py
 runtimepy/tui/task.py
 runtimepy/tui/channels/__init__.py
 tests/test_entry.py
 tests/test_mapping.py
 tests/test_resources.py
```

### Comparing `runtimepy-1.5.4/setup.py` & `runtimepy-1.6.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=0dc3cc2135a37faba7e2cec12476f943
+# hash=6701839983d2292671c1f49f66c938ae
 # =====================================
 
 """
 runtimepy - Package definition for distribution.
 """
 
 # third-party
@@ -24,15 +24,14 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.7",
         "3.8",
         "3.9",
         "3.10",
         "3.11",
     ],
 }
 setup(
```

### Comparing `runtimepy-1.5.4/tests/test_entry.py` & `runtimepy-1.6.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.5.4/tests/test_mapping.py` & `runtimepy-1.6.0/tests/test_mapping.py`

 * *Files identical despite different names*

