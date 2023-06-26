# Comparing `tmp/walt-server-8.0.tar.gz` & `tmp/walt-server-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-server-8.0.tar", last modified: Fri Jun 23 07:38:14 2023, max compression
+gzip compressed data, was "walt-server-8.1.tar", last modified: Mon Jun 26 14:05:21 2023, max compression
```

## Comparing `walt-server-8.0.tar` & `walt-server-8.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-21 15:19:09.000000 walt-server-8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-23 07:38:14.652602 walt-server-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-server-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:14.652602 walt-server-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-23 07:37:56.000000 walt-server-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.640602 walt-server-8.0/sh/
--rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-server-8.0/sh/walt-image-build-helper
--rwxr-xr-x   0 root         (0) root         (0)     1335 2022-03-29 14:58:03.000000 walt-server-8.0/sh/walt-image-shell-helper
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.640602 walt-server-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-server-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/
--rw-r--r--   0 root         (0) root         (0)      352 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/annotatecmd.py
--rw-r--r--   0 root         (0) root         (0)     5567 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/autoglob.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/config.py
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/const.py
--rwxr-xr-x   0 root         (0) root         (0)     2319 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/daemon.py
--rwxr-xr-x   0 root         (0) root         (0)     1510 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/dhcpevent.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/exttools.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/imagecheck.py
--rw-r--r--   0 root         (0) root         (0)     5367 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/netconfig.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/popen.py
--rw-r--r--   0 root         (0) root         (0)    14123 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/__init__.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/grouper.py
--rw-r--r--   0 root         (0) root         (0)    38624 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/topology.py
--rw-r--r--   0 root         (0) root         (0)     4448 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/images/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16127 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/clone.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/commit.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/metadata.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/publish.py
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/pull.py
--rw-r--r--   0 root         (0) root         (0)     9389 2023-06-22 13:09:04.000000 walt-server-8.0/walt/server/processes/blocking/images/search.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/squash.py
--rw-r--r--   0 root         (0) root         (0)      168 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/tools.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/logs.py
--rw-r--r--   0 root         (0) root         (0)     6320 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/process.py
--rw-r--r--   0 root         (0) root         (0)    11616 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/registries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/snmp/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5542 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/base.py
--rwxr-xr-x   0 root         (0) root         (0)     2209 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/bridge.py
--rwxr-xr-x   0 root         (0) root         (0)     3896 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/lldp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/
--rw-r--r--   0 root         (0) root         (0)    76945 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)    23641 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)     9740 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)   217031 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib
--rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib
--rw-r--r--   0 root         (0) root         (0)    26808 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib
--rw-r--r--   0 root         (0) root         (0)     1101 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib
--rw-r--r--   0 root         (0) root         (0)    15894 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)      785 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7023 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/poe.py
--rwxr-xr-x   0 root         (0) root         (0)      815 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    17762 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/db.py
--rw-r--r--   0 root         (0) root         (0)     9393 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/postgres.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/hub/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/hub/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-22 12:43:15.000000 walt-server-8.0/walt/server/processes/hub/client.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/hub/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12263 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/cs.py
--rwxr-xr-x   0 root         (0) root         (0)      354 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/ns.py
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/ss.py
--rwxr-xr-x   0 root         (0) root         (0)      682 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/vs.py
--rwxr-xr-x   0 root         (0) root         (0)     2164 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/apisession.py
--rw-r--r--   0 root         (0) root         (0)    12653 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/blocking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19096 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/devices/manager.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/exports.py
--rw-r--r--   0 root         (0) root         (0)     4965 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/filesystem.py
--rwxr-xr-x   0 root         (0) root         (0)     1208 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/hub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/images/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/build.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/clone.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/duplicate.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/fixowner.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/image.py
--rw-r--r--   0 root         (0) root         (0)    10015 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/manager.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/metadata.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/publish.py
--rw-r--r--   0 root         (0) root         (0)      506 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/remove.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/rename.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/search.py
--rw-r--r--   0 root         (0) root         (0)     8061 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/setup.py
--rw-r--r--   0 root         (0) root         (0)     4574 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/shell.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/spec.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/squash.py
--rw-r--r--   0 root         (0) root         (0)    19795 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/store.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/tabular.py
--rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-cat
--rwxr-xr-x   0 root         (0) root         (0)      911 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-clock-sync
--rwxr-xr-x   0 root         (0) root         (0)      100 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-echo
--rwxr-xr-x   0 root         (0) root         (0)      228 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-env
--rwxr-xr-x   0 root         (0) root         (0)      768 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-fs-watchdog
--rwxr-xr-x   0 root         (0) root         (0)     6541 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-init
--rwxr-xr-x   0 root         (0) root         (0)      160 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-cat
--rwxr-xr-x   0 root         (0) root         (0)     1776 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-echo
--rwxr-xr-x   0 root         (0) root         (0)     2430 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-tee
--rwxr-xr-x   0 root         (0) root         (0)     3058 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-net-service
--rwxr-xr-x   0 root         (0) root         (0)     3202 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-notify-bootup
--rwxr-xr-x   0 root         (0) root         (0)     1238 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-rpc
--rwxr-xr-x   0 root         (0) root         (0)      564 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-tar-send
--rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-tee
--rwxr-xr-x   0 root         (0) root         (0)      314 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-timeout
--rwxr-xr-x   0 root         (0) root         (0)     2434 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/interactive.py
--rw-r--r--   0 root         (0) root         (0)    20534 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/processes/main/network/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8301 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/dhcpd.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/nbfs.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/nfs.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/service.py
--rw-r--r--   0 root         (0) root         (0)  3889008 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/tftp-standby.tar.gz
--rw-r--r--   0 root         (0) root         (0)     5908 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/tftp.py
--rw-r--r--   0 root         (0) root         (0)    67720 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/walt-x86-undionly.kpxe
--rwxr-xr-x   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/waltvlanconf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/processes/main/nodes/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/clock.py
--rwxr-xr-x   0 root         (0) root         (0)     3075 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/expose.py
--rw-r--r--   0 root         (0) root         (0)    15228 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/manager.py
--rw-r--r--   0 root         (0) root         (0)     4118 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/netservice.py
--rw-r--r--   0 root         (0) root         (0)     9314 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/powersave.py
--rw-r--r--   0 root         (0) root         (0)     7955 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/reboot.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/register.py
--rw-r--r--   0 root         (0) root         (0)     5106 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/show.py
--rwxr-xr-x   0 root         (0) root         (0)     3109 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/status.py
--rw-r--r--   0 root         (0) root         (0)     2894 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/wait.py
--rwxr-xr-x   0 root         (0) root         (0)     5973 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/parallel.py
--rwxr-xr-x   0 root         (0) root         (0)     1353 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/process.py
--rw-r--r--   0 root         (0) root         (0)    10155 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/registry.py
--rw-r--r--   0 root         (0) root         (0)    15170 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/server.py
--rw-r--r--   0 root         (0) root         (0)    26496 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/status.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/task.py
--rw-r--r--   0 root         (0) root         (0)    11797 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/transfer.py
--rwxr-xr-x   0 root         (0) root         (0)     1687 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/unix.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/vpn-proxy-setup.sh
--rw-r--r--   0 root         (0) root         (0)     7696 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/vpn.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/httpd.py
--rwxr-xr-x   0 root         (0) root         (0)     1233 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/lldpd.py
--rwxr-xr-x   0 root         (0) root         (0)     1197 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/ptpd.py
--rwxr-xr-x   0 root         (0) root         (0)     1282 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/snmpd.py
--rwxr-xr-x   0 root         (0) root         (0)     1430 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/tftpd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/setup/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6476 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/apt.py
--rw-r--r--   0 root         (0) root         (0)     8222 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/conf.py
--rw-r--r--   0 root         (0) root         (0)    33338 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/conmon.gz
--rw-r--r--   0 root         (0) root         (0)     1094 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/grub.py
--rw-r--r--   0 root         (0) root         (0)     9458 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/main.py
--rw-r--r--   0 root         (0) root         (0)    15334 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/netconf.py
--rw-r--r--   0 root         (0) root         (0)    12575 2023-06-22 12:34:04.000000 walt-server-8.0/walt/server/setup/ossetup.py
--rw-r--r--   0 root         (0) root         (0)    11525 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/regconf.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-dhcpd.service
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-httpd.service
--rw-r--r--   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-lldpd.service
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-netconfig.service
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-podman.service
--rw-r--r--   0 root         (0) root         (0)      139 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-podman.socket
--rw-r--r--   0 root         (0) root         (0)      948 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-ptpd.service
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-snmpd.service
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-tftpd.service
--rw-r--r--   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server.service
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/spec.py
--rw-r--r--   0 root         (0) root         (0)     7280 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6967 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      805 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-21 15:19:09.000000 walt-server-8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-26 14:05:21.027900 walt-server-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-server-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:21.027900 walt-server-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-26 14:05:03.000000 walt-server-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/sh/
+-rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-server-8.1/sh/walt-image-build-helper
+-rwxr-xr-x   0 root         (0) root         (0)     1335 2022-03-29 14:58:03.000000 walt-server-8.1/sh/walt-image-shell-helper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-server-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/annotatecmd.py
+-rw-r--r--   0 root         (0) root         (0)     5567 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/autoglob.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/config.py
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     2319 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/daemon.py
+-rwxr-xr-x   0 root         (0) root         (0)     1510 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/dhcpevent.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/exttools.py
+-rw-r--r--   0 root         (0) root         (0)      796 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/imagecheck.py
+-rw-r--r--   0 root         (0) root         (0)     5367 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/netconfig.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/popen.py
+-rw-r--r--   0 root         (0) root         (0)    14123 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/blocking/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/blocking/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/devices/grouper.py
+-rw-r--r--   0 root         (0) root         (0)    38624 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/devices/topology.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/devices/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/blocking/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16127 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/clone.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/commit.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/publish.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/pull.py
+-rw-r--r--   0 root         (0) root         (0)     9389 2023-06-22 13:09:04.000000 walt-server-8.1/walt/server/processes/blocking/images/search.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/squash.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/images/tools.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/logs.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/process.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/registries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/blocking/snmp/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5542 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2209 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/bridge.py
+-rwxr-xr-x   0 root         (0) root         (0)     3896 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/lldp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/
+-rw-r--r--   0 root         (0) root         (0)    76945 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)    23641 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)     9740 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)   217031 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)    26808 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)    15894 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)      785 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/mibs/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7023 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/poe.py
+-rwxr-xr-x   0 root         (0) root         (0)      815 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/blocking/snmp/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.019900 walt-server-8.1/walt/server/processes/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/db/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    17762 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/db/db.py
+-rw-r--r--   0 root         (0) root         (0)     9393 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/db/postgres.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/db/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.023900 walt-server-8.1/walt/server/processes/hub/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/hub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-22 12:43:15.000000 walt-server-8.1/walt/server/processes/hub/client.py
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/hub/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.023900 walt-server-8.1/walt/server/processes/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.023900 walt-server-8.1/walt/server/processes/main/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12263 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/api/cs.py
+-rwxr-xr-x   0 root         (0) root         (0)      354 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/api/ns.py
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/api/ss.py
+-rwxr-xr-x   0 root         (0) root         (0)      682 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/api/vs.py
+-rwxr-xr-x   0 root         (0) root         (0)     2164 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/apisession.py
+-rw-r--r--   0 root         (0) root         (0)    12653 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/blocking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.023900 walt-server-8.1/walt/server/processes/main/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19096 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/devices/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/exports.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/filesystem.py
+-rwxr-xr-x   0 root         (0) root         (0)     1208 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/hub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.023900 walt-server-8.1/walt/server/processes/main/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/build.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/clone.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/duplicate.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/fixowner.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/image.py
+-rw-r--r--   0 root         (0) root         (0)    10015 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/manager.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/publish.py
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/rename.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/search.py
+-rw-r--r--   0 root         (0) root         (0)     8061 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4574 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/shell.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/spec.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/squash.py
+-rw-r--r--   0 root         (0) root         (0)    19795 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/store.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/tabular.py
+-rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-cat
+-rwxr-xr-x   0 root         (0) root         (0)      911 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-clock-sync
+-rwxr-xr-x   0 root         (0) root         (0)      100 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-echo
+-rwxr-xr-x   0 root         (0) root         (0)      228 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-env
+-rwxr-xr-x   0 root         (0) root         (0)      768 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-fs-watchdog
+-rwxr-xr-x   0 root         (0) root         (0)     6541 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-init
+-rwxr-xr-x   0 root         (0) root         (0)      160 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-log-cat
+-rwxr-xr-x   0 root         (0) root         (0)     1776 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-log-echo
+-rwxr-xr-x   0 root         (0) root         (0)     2430 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-log-tee
+-rwxr-xr-x   0 root         (0) root         (0)     3058 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-net-service
+-rwxr-xr-x   0 root         (0) root         (0)     3202 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-notify-bootup
+-rwxr-xr-x   0 root         (0) root         (0)     1238 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-rpc
+-rwxr-xr-x   0 root         (0) root         (0)      564 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-tar-send
+-rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-tee
+-rwxr-xr-x   0 root         (0) root         (0)      314 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/images/walt-timeout
+-rwxr-xr-x   0 root         (0) root         (0)     2434 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/interactive.py
+-rw-r--r--   0 root         (0) root         (0)    20534 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/walt/server/processes/main/network/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8301 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/dhcpd.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/nbfs.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/nfs.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/service.py
+-rw-r--r--   0 root         (0) root         (0)  3889008 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/tftp-standby.tar.gz
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/tftp.py
+-rw-r--r--   0 root         (0) root         (0)    67720 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/walt-x86-undionly.kpxe
+-rwxr-xr-x   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/network/waltvlanconf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/walt/server/processes/main/nodes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/clock.py
+-rwxr-xr-x   0 root         (0) root         (0)     3075 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/expose.py
+-rw-r--r--   0 root         (0) root         (0)    15228 2023-06-26 11:59:35.000000 walt-server-8.1/walt/server/processes/main/nodes/manager.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/netservice.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/powersave.py
+-rw-r--r--   0 root         (0) root         (0)     7955 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/reboot.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-06-26 12:30:58.000000 walt-server-8.1/walt/server/processes/main/nodes/register.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/show.py
+-rwxr-xr-x   0 root         (0) root         (0)     3109 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/status.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/nodes/wait.py
+-rwxr-xr-x   0 root         (0) root         (0)     5973 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/parallel.py
+-rwxr-xr-x   0 root         (0) root         (0)     1353 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/process.py
+-rw-r--r--   0 root         (0) root         (0)    10155 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15170 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/server.py
+-rw-r--r--   0 root         (0) root         (0)    26496 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/status.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/task.py
+-rw-r--r--   0 root         (0) root         (0)    11797 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/transfer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1687 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/unix.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/vpn-proxy-setup.sh
+-rw-r--r--   0 root         (0) root         (0)     7696 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/vpn.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/processes/main/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/walt/server/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/httpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1233 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/lldpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1197 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/ptpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1282 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/snmpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1430 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/services/tftpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/walt/server/setup/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6476 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/apt.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/conf.py
+-rw-r--r--   0 root         (0) root         (0)    33338 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/conmon.gz
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/grub.py
+-rw-r--r--   0 root         (0) root         (0)     9458 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/main.py
+-rw-r--r--   0 root         (0) root         (0)    15334 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/netconf.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-06-26 14:00:21.000000 walt-server-8.1/walt/server/setup/ossetup.py
+-rw-r--r--   0 root         (0) root         (0)    11525 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/regconf.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-dhcpd.service
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-httpd.service
+-rw-r--r--   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-lldpd.service
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-netconfig.service
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-podman.service
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-podman.socket
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-ptpd.service
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-snmpd.service
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server-tftpd.service
+-rw-r--r--   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/setup/walt-server.service
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/spec.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2023-06-21 15:19:09.000000 walt-server-8.1/walt/server/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:21.027900 walt-server-8.1/walt_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      805 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:21.000000 walt-server-8.1/walt_server.egg-info/top_level.txt
```

### Comparing `walt-server-8.0/setup.py` & `walt-server-8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-server",
-    "version": "8.0",
+    "version": "8.1",
     "install_requires": [
         "PyYAML==6.0",
         "Pygments==2.15.1",
         "aiohttp==3.8.4",
         "aiosignal==1.3.1",
         "aiostream==0.4.5",
         "async-timeout==4.0.2",
@@ -50,18 +50,18 @@
         "sdnotify==0.3.2",
         "setproctitle==1.3.2",
         "setuptools==44.1.1",
         "six==1.16.0",
         "snimpy==1.0.0",
         "tomli==2.0.1",
         "urllib3==1.26.15",
-        "walt-client==8.0",
-        "walt-common==8.0",
-        "walt-virtual==8.0",
-        "walt-vpn==8.0",
+        "walt-client==8.1",
+        "walt-common==8.1",
+        "walt-virtual==8.1",
+        "walt-vpn==8.1",
         "yarl==1.9.2",
         "zope.event==4.6",
         "zope.interface==6.0",
     ],
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
```

### Comparing `walt-server-8.0/sh/walt-image-build-helper` & `walt-server-8.1/sh/walt-image-build-helper`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/sh/walt-image-shell-helper` & `walt-server-8.1/sh/walt-image-shell-helper`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/annotatecmd.py` & `walt-server-8.1/walt/server/annotatecmd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/autoglob.py` & `walt-server-8.1/walt/server/autoglob.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/config.py` & `walt-server-8.1/walt/server/config.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/daemon.py` & `walt-server-8.1/walt/server/daemon.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/dhcpevent.py` & `walt-server-8.1/walt/server/dhcpevent.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/exttools.py` & `walt-server-8.1/walt/server/exttools.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/imagecheck.py` & `walt-server-8.1/walt/server/imagecheck.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/netconfig.py` & `walt-server-8.1/walt/server/netconfig.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/popen.py` & `walt-server-8.1/walt/server/popen.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/process.py` & `walt-server-8.1/walt/server/process.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/devices/grouper.py` & `walt-server-8.1/walt/server/processes/blocking/devices/grouper.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/devices/topology.py` & `walt-server-8.1/walt/server/processes/blocking/devices/topology.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/devices/tree.py` & `walt-server-8.1/walt/server/processes/blocking/devices/tree.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/clone.py` & `walt-server-8.1/walt/server/processes/blocking/images/clone.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/commit.py` & `walt-server-8.1/walt/server/processes/blocking/images/commit.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/metadata.py` & `walt-server-8.1/walt/server/processes/blocking/images/metadata.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/publish.py` & `walt-server-8.1/walt/server/processes/blocking/images/publish.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/pull.py` & `walt-server-8.1/walt/server/processes/blocking/images/pull.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/search.py` & `walt-server-8.1/walt/server/processes/blocking/images/search.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/images/squash.py` & `walt-server-8.1/walt/server/processes/blocking/images/squash.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/logs.py` & `walt-server-8.1/walt/server/processes/blocking/logs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/process.py` & `walt-server-8.1/walt/server/processes/blocking/process.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/registries.py` & `walt-server-8.1/walt/server/processes/blocking/registries.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/base.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/base.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/bridge.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/bridge.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/lldp.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/lldp.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/__init__.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/mibs/__init__.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/poe.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/poe.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/blocking/snmp/proxy.py` & `walt-server-8.1/walt/server/processes/blocking/snmp/proxy.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/db/db.py` & `walt-server-8.1/walt/server/processes/db/db.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/db/postgres.py` & `walt-server-8.1/walt/server/processes/db/postgres.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/db/process.py` & `walt-server-8.1/walt/server/processes/db/process.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/hub/client.py` & `walt-server-8.1/walt/server/processes/hub/client.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/hub/process.py` & `walt-server-8.1/walt/server/processes/hub/process.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/api/cs.py` & `walt-server-8.1/walt/server/processes/main/api/cs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/api/ss.py` & `walt-server-8.1/walt/server/processes/main/api/ss.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/api/vs.py` & `walt-server-8.1/walt/server/processes/main/api/vs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/apisession.py` & `walt-server-8.1/walt/server/processes/main/apisession.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/autocomplete.py` & `walt-server-8.1/walt/server/processes/main/autocomplete.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/blocking.py` & `walt-server-8.1/walt/server/processes/main/blocking.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/devices/manager.py` & `walt-server-8.1/walt/server/processes/main/devices/manager.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/exports.py` & `walt-server-8.1/walt/server/processes/main/exports.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/filesystem.py` & `walt-server-8.1/walt/server/processes/main/filesystem.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/hub.py` & `walt-server-8.1/walt/server/processes/main/hub.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/build.py` & `walt-server-8.1/walt/server/processes/main/images/build.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/clone.py` & `walt-server-8.1/walt/server/processes/main/images/clone.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/duplicate.py` & `walt-server-8.1/walt/server/processes/main/images/duplicate.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/fixowner.py` & `walt-server-8.1/walt/server/processes/main/images/fixowner.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/image.py` & `walt-server-8.1/walt/server/processes/main/images/image.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/manager.py` & `walt-server-8.1/walt/server/processes/main/images/manager.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/rename.py` & `walt-server-8.1/walt/server/processes/main/images/rename.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/setup.py` & `walt-server-8.1/walt/server/processes/main/images/setup.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/shell.py` & `walt-server-8.1/walt/server/processes/main/images/shell.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/spec.py` & `walt-server-8.1/walt/server/processes/main/images/spec.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/squash.py` & `walt-server-8.1/walt/server/processes/main/images/squash.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/store.py` & `walt-server-8.1/walt/server/processes/main/images/store.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/tabular.py` & `walt-server-8.1/walt/server/processes/main/images/tabular.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-clock-sync` & `walt-server-8.1/walt/server/processes/main/images/walt-clock-sync`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-fs-watchdog` & `walt-server-8.1/walt/server/processes/main/images/walt-fs-watchdog`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-init` & `walt-server-8.1/walt/server/processes/main/images/walt-init`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-log-echo` & `walt-server-8.1/walt/server/processes/main/images/walt-log-echo`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-log-tee` & `walt-server-8.1/walt/server/processes/main/images/walt-log-tee`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-net-service` & `walt-server-8.1/walt/server/processes/main/images/walt-net-service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-notify-bootup` & `walt-server-8.1/walt/server/processes/main/images/walt-notify-bootup`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-rpc` & `walt-server-8.1/walt/server/processes/main/images/walt-rpc`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/images/walt-tar-send` & `walt-server-8.1/walt/server/processes/main/images/walt-tar-send`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/interactive.py` & `walt-server-8.1/walt/server/processes/main/interactive.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/logs.py` & `walt-server-8.1/walt/server/processes/main/logs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/dhcpd.py` & `walt-server-8.1/walt/server/processes/main/network/dhcpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/nbfs.py` & `walt-server-8.1/walt/server/processes/main/network/nbfs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/nfs.py` & `walt-server-8.1/walt/server/processes/main/network/nfs.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/service.py` & `walt-server-8.1/walt/server/processes/main/network/service.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/tftp-standby.tar.gz` & `walt-server-8.1/walt/server/processes/main/network/tftp-standby.tar.gz`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/tftp.py` & `walt-server-8.1/walt/server/processes/main/network/tftp.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/walt-x86-undionly.kpxe` & `walt-server-8.1/walt/server/processes/main/network/walt-x86-undionly.kpxe`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/network/waltvlanconf.py` & `walt-server-8.1/walt/server/processes/main/network/waltvlanconf.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/clock.py` & `walt-server-8.1/walt/server/processes/main/nodes/clock.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/expose.py` & `walt-server-8.1/walt/server/processes/main/nodes/expose.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/manager.py` & `walt-server-8.1/walt/server/processes/main/nodes/manager.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/netservice.py` & `walt-server-8.1/walt/server/processes/main/nodes/netservice.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/powersave.py` & `walt-server-8.1/walt/server/processes/main/nodes/powersave.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/reboot.py` & `walt-server-8.1/walt/server/processes/main/nodes/reboot.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/register.py` & `walt-server-8.1/walt/server/processes/main/nodes/register.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     full_kwargs = dict(
         db=db,
         images=images,
         mac=mac,
         image_fullname=image_fullname,
         model=model,
         logs=logs,
+        blocking=blocking,
         **kwargs,
     )
     wf_steps = []
     # if image is new
     if image_fullname not in images:
         # we have to pull an image, that will be long,
         # let's inform the user (by logs) and do this asynchronously
@@ -52,18 +53,17 @@
     wf.run()
 
 
 def wf_pull_image(wf, blocking, image_fullname, **env):
     blocking.pull_image(None, image_fullname, wf.next)
 
 
-def wf_after_pull_image(wf, pull_result, images, image_fullname, model, logs, **env):
+def wf_after_pull_image(wf, pull_result, image_fullname, model, logs, **env):
     if pull_result[0]:
         # ok
-        images.register_image(image_fullname)
         dup_msg(
             f"Image {image_fullname} was downloaded successfully.", sys.stdout, logs
         )
         wf.next()
     else:
         failure = pull_result[1]
         # not being able to download default images for nodes
```

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/show.py` & `walt-server-8.1/walt/server/processes/main/nodes/show.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/status.py` & `walt-server-8.1/walt/server/processes/main/nodes/status.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/nodes/wait.py` & `walt-server-8.1/walt/server/processes/main/nodes/wait.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/parallel.py` & `walt-server-8.1/walt/server/processes/main/parallel.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/process.py` & `walt-server-8.1/walt/server/processes/main/process.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/registry.py` & `walt-server-8.1/walt/server/processes/main/registry.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/server.py` & `walt-server-8.1/walt/server/processes/main/server.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/settings.py` & `walt-server-8.1/walt/server/processes/main/settings.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/task.py` & `walt-server-8.1/walt/server/processes/main/task.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/transfer.py` & `walt-server-8.1/walt/server/processes/main/transfer.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/unix.py` & `walt-server-8.1/walt/server/processes/main/unix.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/vpn-proxy-setup.sh` & `walt-server-8.1/walt/server/processes/main/vpn-proxy-setup.sh`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/vpn.py` & `walt-server-8.1/walt/server/processes/main/vpn.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/processes/main/workflow.py` & `walt-server-8.1/walt/server/processes/main/workflow.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/services/httpd.py` & `walt-server-8.1/walt/server/services/httpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/services/lldpd.py` & `walt-server-8.1/walt/server/services/lldpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/services/ptpd.py` & `walt-server-8.1/walt/server/services/ptpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/services/snmpd.py` & `walt-server-8.1/walt/server/services/snmpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/services/tftpd.py` & `walt-server-8.1/walt/server/services/tftpd.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/apt.py` & `walt-server-8.1/walt/server/setup/apt.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/conf.py` & `walt-server-8.1/walt/server/setup/conf.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/conmon.gz` & `walt-server-8.1/walt/server/setup/conmon.gz`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/grub.py` & `walt-server-8.1/walt/server/setup/grub.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/main.py` & `walt-server-8.1/walt/server/setup/main.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/netconf.py` & `walt-server-8.1/walt/server/setup/netconf.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/ossetup.py` & `walt-server-8.1/walt/server/setup/ossetup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import datetime
 import gzip
 import json
 import os
 import shlex
+import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 import requests
 from pkg_resources import resource_filename
 from walt.common.version import __version__
@@ -297,15 +298,16 @@
         print("done")
         Path("/usr/bin/conmon").symlink_to("/usr/bin/conmon.fixed")
 
 
 # We now install walt python packages in a virtual environment
 # (at least for the server).
 # Previously they were installed in the base python environment of the OS.
-# This procedure cleans up any walt python package found there.
+# This procedure cleans up any walt python package found there,
+# and any obsolete vitrual environment.
 def cleanup_old_walt_install():
     # we temporarily remove the venv prefix from the PATH variable,
     # to target the python executable of the base environment of the OS.
     saved_path = os.environ["PATH"]
     os.environ["PATH"] = ":".join(
         path_entry
         for path_entry in os.environ["PATH"].split(":")
@@ -335,7 +337,14 @@
                 "python3 -m pip uninstall -y".split() + walt_packages,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
             print("done")
     # restore the PATH variable
     os.environ["PATH"] = saved_path
+    # clear old /opt/walt-<version> directories
+    for opt_entry in Path('/opt').iterdir():
+        if opt_entry.name.startswith('walt-') and opt_entry != Path(sys.prefix):
+            print(f"Removing obsolete {opt_entry}... ", end="")
+            sys.stdout.flush()
+            shutil.rmtree(str(opt_entry))
+            print("done")
```

### Comparing `walt-server-8.0/walt/server/setup/regconf.py` & `walt-server-8.1/walt/server/setup/regconf.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-dhcpd.service` & `walt-server-8.1/walt/server/setup/walt-server-dhcpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-httpd.service` & `walt-server-8.1/walt/server/setup/walt-server-httpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-lldpd.service` & `walt-server-8.1/walt/server/setup/walt-server-lldpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-netconfig.service` & `walt-server-8.1/walt/server/setup/walt-server-netconfig.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-ptpd.service` & `walt-server-8.1/walt/server/setup/walt-server-ptpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-snmpd.service` & `walt-server-8.1/walt/server/setup/walt-server-snmpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server-tftpd.service` & `walt-server-8.1/walt/server/setup/walt-server-tftpd.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/setup/walt-server.service` & `walt-server-8.1/walt/server/setup/walt-server.service`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/spec.py` & `walt-server-8.1/walt/server/spec.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt/server/tools.py` & `walt-server-8.1/walt/server/tools.py`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt_server.egg-info/SOURCES.txt` & `walt-server-8.1/walt_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt_server.egg-info/entry_points.txt` & `walt-server-8.1/walt_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `walt-server-8.0/walt_server.egg-info/requires.txt` & `walt-server-8.1/walt_server.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 sdnotify==0.3.2
 setproctitle==1.3.2
 setuptools==44.1.1
 six==1.16.0
 snimpy==1.0.0
 tomli==2.0.1
 urllib3==1.26.15
-walt-client==8.0
-walt-common==8.0
-walt-virtual==8.0
-walt-vpn==8.0
+walt-client==8.1
+walt-common==8.1
+walt-virtual==8.1
+walt-vpn==8.1
 yarl==1.9.2
 zope.event==4.6
 zope.interface==6.0
```

