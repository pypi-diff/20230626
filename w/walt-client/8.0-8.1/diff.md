# Comparing `tmp/walt-client-8.0.tar.gz` & `tmp/walt-client-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "walt-client-8.0.tar", last modified: Fri Jun 23 07:38:23 2023, max compression
+gzip compressed data, was "walt-client-8.1.tar", last modified: Mon Jun 26 14:05:29 2023, max compression
```

## Comparing `walt-client-8.0.tar` & `walt-client-8.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/
--rw-r--r--   0 root         (0) root         (0)       32 2022-03-29 14:58:03.000000 walt-client-8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:38:23.076477 walt-client-8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-client-8.0/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:23.076477 walt-client-8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 07:37:56.000000 walt-client-8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-client-8.0/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2443 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/advanced.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/apiobject/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    20082 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/base.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/config.py
--rwxr-xr-x   0 root         (0) root         (0)     8074 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/images.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/logs.py
--rwxr-xr-x   0 root         (0) root         (0)    12837 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/nodes.py
--rwxr-xr-x   0 root         (0) root         (0)      972 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/root.py
--rwxr-xr-x   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/server.py
--rwxr-xr-x   0 root         (0) root         (0)      379 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/tools.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apitools.py
--rwxr-xr-x   0 root         (0) root         (0)     1903 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/application.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/autocomplete/
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13122 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/dump.py
--rwxr-xr-x   0 root         (0) root         (0)     1323 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/helper.py
--rwxr-xr-x   0 root         (0) root         (0)     1785 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/client.py
--rw-r--r--   0 root         (0) root         (0)    15266 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/config.py
--rw-r--r--   0 root         (0) root         (0)     3017 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/console.py
--rwxr-xr-x   0 root         (0) root         (0)     6644 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/doc/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2252 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/color.py
--rw-r--r--   0 root         (0) root         (0)    12579 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/doc/md/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/__init__.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/admin.md
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/compatibility.md
--rw-r--r--   0 root         (0) root         (0)     2454 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/design-notes.md
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-config.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-expose.md
--rw-r--r--   0 root         (0) root         (0)     1920 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-netsetup.md
--rw-r--r--   0 root         (0) root         (0)     1295 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-sets.md
--rw-r--r--   0 root         (0) root         (0)     4413 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/g5k.md
--rw-r--r--   0 root         (0) root         (0)     4562 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/help-intro.md
--rw-r--r--   0 root         (0) root         (0)     2803 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-build.md
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-cp.md
--rw-r--r--   0 root         (0) root         (0)    13931 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-from-scratch.md
--rw-r--r--   0 root         (0) root         (0)     2157 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/image-spec-file.md
--rw-r--r--   0 root         (0) root         (0)     1716 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-cat.md
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-checkpoint.md
--rw-r--r--   0 root         (0) root         (0)     1678 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-echo.md
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-format.md
--rw-r--r--   0 root         (0) root         (0)      727 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-history.md
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-issuers.md
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-monitor.md
--rw-r--r--   0 root         (0) root         (0)      479 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-realtime.md
--rw-r--r--   0 root         (0) root         (0)     1446 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-show.md
--rw-r--r--   0 root         (0) root         (0)      432 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-tee.md
--rw-r--r--   0 root         (0) root         (0)     1108 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-wait.md
--rw-r--r--   0 root         (0) root         (0)     3543 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/logging.md
--rw-r--r--   0 root         (0) root         (0)     4515 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/networking.md
--rw-r--r--   0 root         (0) root         (0)     4273 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/new-node-support.md
--rw-r--r--   0 root         (0) root         (0)     5669 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/node-bootup.md
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-config.md
--rw-r--r--   0 root         (0) root         (0)     1060 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-console.md
--rw-r--r--   0 root         (0) root         (0)     1325 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-cp.md
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-expose.md
--rw-r--r--   0 root         (0) root         (0)     8365 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/node-install.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-netsetup.md
--rw-r--r--   0 root         (0) root         (0)     2473 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-ownership.md
--rw-r--r--   0 root         (0) root         (0)     3634 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/optional-features.md
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/packaging.md
--rw-r--r--   0 root         (0) root         (0)     4895 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/registries.md
--rw-r--r--   0 root         (0) root         (0)     2555 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/rpi-serial.md
--rw-r--r--   0 root         (0) root         (0)     5014 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-images.md
--rw-r--r--   0 root         (0) root         (0)     4924 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-logs.md
--rw-r--r--   0 root         (0) root         (0)     7467 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-nodes.md
--rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-tools.md
--rw-r--r--   0 root         (0) root         (0)     5306 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting.md
--rw-r--r--   0 root         (0) root         (0)     2717 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/server-install.md
--rw-r--r--   0 root         (0) root         (0)     9858 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/server-network-config.md
--rw-r--r--   0 root         (0) root         (0)      788 2023-06-22 14:11:23.000000 walt-client-8.0/walt/client/doc/md/server-upgrade.md
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/shell-completion.md
--rw-r--r--   0 root         (0) root         (0)     2705 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/shells.md
--rw-r--r--   0 root         (0) root         (0)     4982 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/switch-install.md
--rw-r--r--   0 root         (0) root         (0)     2715 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/troubleshooting.md
--rw-r--r--   0 root         (0) root         (0)    14874 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/tutorial.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/unmanaged-devices.md
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/vnode-networks.md
--rw-r--r--   0 root         (0) root         (0)     3926 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/vpn.md
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/mdtable.py
--rwxr-xr-x   0 root         (0) root         (0)     9898 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/pager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/doc/sphinx/
--rw-r--r--   0 root         (0) root         (0)     2701 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/sphinx/conf.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-23 07:37:56.000000 walt-client-8.0/walt/client/doc/sphinx/version.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)     2388 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/expose.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/filesystem.py
--rwxr-xr-x   0 root         (0) root         (0)    12590 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/image.py
--rwxr-xr-x   0 root         (0) root         (0)     6593 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/interactive.py
--rwxr-xr-x   0 root         (0) root         (0)     4545 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/link.py
--rwxr-xr-x   0 root         (0) root         (0)    14029 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/log.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/logo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/metadata/
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/metadata/core.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/myhelp.py
--rwxr-xr-x   0 root         (0) root         (0)    16940 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/node.py
--rwxr-xr-x   0 root         (0) root         (0)     2148 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/plugins.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/progress.py
--rw-r--r--   0 root         (0) root         (0)    11444 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/speedup.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/startup.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/timeout.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/tools.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/transfer.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/types.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/update.py
--rwxr-xr-x   0 root         (0) root         (0)     3970 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/vpn.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3512 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.671772 walt-client-8.1/
+-rw-r--r--   0 root         (0) root         (0)       32 2022-03-29 14:58:03.000000 walt-client-8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-26 14:05:29.671772 walt-client-8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-client-8.1/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 14:05:29.671772 walt-client-8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-26 14:05:03.000000 walt-client-8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.667772 walt-client-8.1/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-client-8.1/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.667772 walt-client-8.1/walt/client/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2443 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/advanced.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.667772 walt-client-8.1/walt/client/apiobject/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    20082 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/base.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     8074 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/images.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/logs.py
+-rwxr-xr-x   0 root         (0) root         (0)    12837 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/nodes.py
+-rwxr-xr-x   0 root         (0) root         (0)      972 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/root.py
+-rwxr-xr-x   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/server.py
+-rwxr-xr-x   0 root         (0) root         (0)      379 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apiobject/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/apitools.py
+-rwxr-xr-x   0 root         (0) root         (0)     1903 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/application.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.667772 walt-client-8.1/walt/client/autocomplete/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/autocomplete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13122 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/autocomplete/dump.py
+-rwxr-xr-x   0 root         (0) root         (0)     1323 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/autocomplete/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     1785 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    15266 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/config.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/console.py
+-rwxr-xr-x   0 root         (0) root         (0)     6644 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.667772 walt-client-8.1/walt/client/doc/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2252 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/color.py
+-rw-r--r--   0 root         (0) root         (0)    12579 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.671772 walt-client-8.1/walt/client/doc/md/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/admin.md
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/compatibility.md
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-26 12:30:58.000000 walt-client-8.1/walt/client/doc/md/design-notes.md
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/device-config.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/device-expose.md
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/device-netsetup.md
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/device-sets.md
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/g5k.md
+-rw-r--r--   0 root         (0) root         (0)     4562 2023-06-22 09:26:07.000000 walt-client-8.1/walt/client/doc/md/help-intro.md
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/image-build.md
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/image-cp.md
+-rw-r--r--   0 root         (0) root         (0)    13931 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/image-from-scratch.md
+-rw-r--r--   0 root         (0) root         (0)     2157 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/image-spec-file.md
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-cat.md
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-checkpoint.md
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-echo.md
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-format.md
+-rw-r--r--   0 root         (0) root         (0)      727 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/log-history.md
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-issuers.md
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-monitor.md
+-rw-r--r--   0 root         (0) root         (0)      479 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/log-realtime.md
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-show.md
+-rw-r--r--   0 root         (0) root         (0)      432 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/log-tee.md
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/log-wait.md
+-rw-r--r--   0 root         (0) root         (0)     3543 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/logging.md
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/networking.md
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/new-node-support.md
+-rw-r--r--   0 root         (0) root         (0)     5669 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/node-bootup.md
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-config.md
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-console.md
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-cp.md
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-expose.md
+-rw-r--r--   0 root         (0) root         (0)     8365 2023-06-22 09:26:07.000000 walt-client-8.1/walt/client/doc/md/node-install.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-netsetup.md
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/node-ownership.md
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-06-22 09:26:07.000000 walt-client-8.1/walt/client/doc/md/optional-features.md
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/packaging.md
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/registries.md
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/rpi-serial.md
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/scripting-images.md
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/scripting-logs.md
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/scripting-nodes.md
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/scripting-tools.md
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/scripting.md
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-06-26 14:01:41.000000 walt-client-8.1/walt/client/doc/md/server-install.md
+-rw-r--r--   0 root         (0) root         (0)     9858 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/server-network-config.md
+-rw-r--r--   0 root         (0) root         (0)      796 2023-06-26 14:02:25.000000 walt-client-8.1/walt/client/doc/md/server-upgrade.md
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/shell-completion.md
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/shells.md
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/switch-install.md
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/troubleshooting.md
+-rw-r--r--   0 root         (0) root         (0)    14874 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/tutorial.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/unmanaged-devices.md
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/md/vnode-networks.md
+-rw-r--r--   0 root         (0) root         (0)     3926 2022-03-29 14:58:03.000000 walt-client-8.1/walt/client/doc/md/vpn.md
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/mdtable.py
+-rwxr-xr-x   0 root         (0) root         (0)     9898 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/pager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.671772 walt-client-8.1/walt/client/doc/sphinx/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/doc/sphinx/conf.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 14:05:03.000000 walt-client-8.1/walt/client/doc/sphinx/version.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     2388 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/expose.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/filesystem.py
+-rwxr-xr-x   0 root         (0) root         (0)    12590 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/image.py
+-rwxr-xr-x   0 root         (0) root         (0)     6593 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/interactive.py
+-rwxr-xr-x   0 root         (0) root         (0)     4545 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/link.py
+-rwxr-xr-x   0 root         (0) root         (0)    14029 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/logo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.671772 walt-client-8.1/walt/client/metadata/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/metadata/core.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/myhelp.py
+-rwxr-xr-x   0 root         (0) root         (0)    16940 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/node.py
+-rwxr-xr-x   0 root         (0) root         (0)     2148 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/progress.py
+-rw-r--r--   0 root         (0) root         (0)    11444 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/speedup.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/startup.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/timeout.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/tools.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/transfer.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/types.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/update.py
+-rwxr-xr-x   0 root         (0) root         (0)     3970 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/vpn.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-21 15:19:09.000000 walt-client-8.1/walt/client/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 14:05:29.671772 walt-client-8.1/walt_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 14:05:29.000000 walt-client-8.1/walt_client.egg-info/top_level.txt
```

### Comparing `walt-client-8.0/setup.py` & `walt-client-8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import find_packages, setup
 
 if sys.version_info[0] == 2:
     sys.exit("Sorry, Python 2 is no longer supported.")
 
 setup_info = {
     "name": "walt-client",
-    "version": "8.0",
+    "version": "8.1",
     "install_requires": [
         "plumbum>=1.7.2",
         "commonmark>=0.7.5",
         "pygments>=2.2.0",
-        "walt-common==8.0",
+        "walt-common==8.1",
     ],
-    "extras_require": {"g5k": ["walt-client-g5k==8.0"]},
+    "extras_require": {"g5k": ["walt-client-g5k==8.1"]},
     "author": "WalT developers",
     "author_email": "walt-contact@univ-grenoble-alpes.fr",
     "keywords": "WalT testbed",
     "license": "3-Clause BSD",
     "url": "https://walt-project.liglab.fr",
     "description": "WalT control tool.",
     "entry_points": {
```

### Comparing `walt-client-8.0/walt/client/advanced.py` & `walt-client-8.1/walt/client/advanced.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/base.py` & `walt-client-8.1/walt/client/apiobject/base.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/config.py` & `walt-client-8.1/walt/client/apiobject/config.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/images.py` & `walt-client-8.1/walt/client/apiobject/images.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/logs.py` & `walt-client-8.1/walt/client/apiobject/logs.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/nodes.py` & `walt-client-8.1/walt/client/apiobject/nodes.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/root.py` & `walt-client-8.1/walt/client/apiobject/root.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apiobject/server.py` & `walt-client-8.1/walt/client/apiobject/server.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/apitools.py` & `walt-client-8.1/walt/client/apitools.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/application.py` & `walt-client-8.1/walt/client/application.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/auth.py` & `walt-client-8.1/walt/client/auth.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/autocomplete/dump.py` & `walt-client-8.1/walt/client/autocomplete/dump.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/autocomplete/helper.py` & `walt-client-8.1/walt/client/autocomplete/helper.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/client.py` & `walt-client-8.1/walt/client/client.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/config.py` & `walt-client-8.1/walt/client/config.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/console.py` & `walt-client-8.1/walt/client/console.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/device.py` & `walt-client-8.1/walt/client/device.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/color.py` & `walt-client-8.1/walt/client/doc/color.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/markdown.py` & `walt-client-8.1/walt/client/doc/markdown.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/__init__.py` & `walt-client-8.1/walt/client/doc/md/__init__.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/admin.md` & `walt-client-8.1/walt/client/doc/md/admin.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/design-notes.md` & `walt-client-8.1/walt/client/doc/md/design-notes.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 * All users have full control over the platform; this includes plugging or unplugging nodes and network switches for instance.
 * We consider that users will be kind with others, and the plaform itself enforces very few usage restrictions. If a command is likely to disrupt the work of others, the platform will not prevent you from executing it, but it will ask you for confirmation. The concept of "node ownership" for instance follows this general principle (see [`walt help show node-ownership`](node-ownership.md)).
 * WalT is very friendly for new users: they do not need a registration procedure and they immediately have access to the platform resources (no reservation system).
 * Since the platform is not supposed to be directly accessible from internet, WalT only implements a thin layer of security features (e.g., for VPN).
 * Compared to a public platform, a private WalT platform can better fit some use cases, including industrial testbeds, because of the possible industrial secrets involved.
 
 
-# Single-experiment platforms
+## Single-experiment platforms
 
 The concept of private platform also applies well to experiments sensible to interference.
 If you consider concurrent experiment of other users could affect your results, you can build an isolated platform which will just serve your own specific experiment.
 
 
-# Experiment reproducibility
+## Experiment reproducibility
 
 The concept of WalT platform was described in a research paper called [WalT: A Reproducible Testbed for Reproducible Network Experiments](https://hal.science/hal-01287566).
 
 **Reproducibility** is a core concept of WalT.
 Publishing the OS of nodes on a public repository such as the docker hub (using `walt image publish`) allows other people to later reproduce the experiment on other walt platforms.
 By doing so, the user shows she is confident enough that reproducing her experiment in slightly different conditions (different position for nodes, etc.) will still give good results.
 This is a stronger argument compared to just ensuring **repeatability** of the experiment on the same platform.
```

### Comparing `walt-client-8.0/walt/client/doc/md/device-config.md` & `walt-client-8.1/walt/client/doc/md/device-config.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/device-expose.md` & `walt-client-8.1/walt/client/doc/md/device-expose.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/device-netsetup.md` & `walt-client-8.1/walt/client/doc/md/device-netsetup.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/device-sets.md` & `walt-client-8.1/walt/client/doc/md/device-sets.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/g5k.md` & `walt-client-8.1/walt/client/doc/md/g5k.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/help-intro.md` & `walt-client-8.1/walt/client/doc/md/help-intro.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/image-build.md` & `walt-client-8.1/walt/client/doc/md/image-build.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/image-cp.md` & `walt-client-8.1/walt/client/doc/md/image-cp.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/image-from-scratch.md` & `walt-client-8.1/walt/client/doc/md/image-from-scratch.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/image-spec-file.md` & `walt-client-8.1/walt/client/doc/md/image-spec-file.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-cat.md` & `walt-client-8.1/walt/client/doc/md/log-cat.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-checkpoint.md` & `walt-client-8.1/walt/client/doc/md/log-checkpoint.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-echo.md` & `walt-client-8.1/walt/client/doc/md/log-echo.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-history.md` & `walt-client-8.1/walt/client/doc/md/log-history.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-issuers.md` & `walt-client-8.1/walt/client/doc/md/log-issuers.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-monitor.md` & `walt-client-8.1/walt/client/doc/md/log-monitor.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-show.md` & `walt-client-8.1/walt/client/doc/md/log-show.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/log-wait.md` & `walt-client-8.1/walt/client/doc/md/log-wait.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/logging.md` & `walt-client-8.1/walt/client/doc/md/logging.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/networking.md` & `walt-client-8.1/walt/client/doc/md/networking.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/new-node-support.md` & `walt-client-8.1/walt/client/doc/md/new-node-support.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/node-bootup.md` & `walt-client-8.1/walt/client/doc/md/node-bootup.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/node-console.md` & `walt-client-8.1/walt/client/doc/md/node-console.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/node-cp.md` & `walt-client-8.1/walt/client/doc/md/node-cp.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/node-install.md` & `walt-client-8.1/walt/client/doc/md/node-install.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/node-ownership.md` & `walt-client-8.1/walt/client/doc/md/node-ownership.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/optional-features.md` & `walt-client-8.1/walt/client/doc/md/optional-features.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/packaging.md` & `walt-client-8.1/walt/client/doc/md/packaging.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/registries.md` & `walt-client-8.1/walt/client/doc/md/registries.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/rpi-serial.md` & `walt-client-8.1/walt/client/doc/md/rpi-serial.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/scripting-images.md` & `walt-client-8.1/walt/client/doc/md/scripting-images.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/scripting-logs.md` & `walt-client-8.1/walt/client/doc/md/scripting-logs.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/scripting-nodes.md` & `walt-client-8.1/walt/client/doc/md/scripting-nodes.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/scripting-tools.md` & `walt-client-8.1/walt/client/doc/md/scripting-tools.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/scripting.md` & `walt-client-8.1/walt/client/doc/md/scripting.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/server-install.md` & `walt-client-8.1/walt/client/doc/md/server-install.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 $ apt update
 $ apt install -y gcc python3-venv python3-dev libsmi2-dev curl git make
 ```
 
 ## 2- Install and configure walt software
 
 ```
-$ python3 -m venv /opt/walt-8
-$ /opt/walt-8/bin/pip install --upgrade pip
-$ /opt/walt-8/bin/pip install walt-server walt-client
-$ /opt/walt-8/bin/walt-server-setup
+$ python3 -m venv /opt/walt-8.1
+$ /opt/walt-8.1/bin/pip install --upgrade pip
+$ /opt/walt-8.1/bin/pip install walt-server walt-client
+$ /opt/walt-8.1/bin/walt-server-setup
 ```
 
 Note: `walt-server-setup` will display interactive configuration interfaces for network and image registries.
 For more information about WalT network concepts and configuration, see [`walt help show networking`](networking.md).
 For more information about WalT image registries, see [`walt help show registries`](registries.md).
```

### Comparing `walt-client-8.0/walt/client/doc/md/server-network-config.md` & `walt-client-8.1/walt/client/doc/md/server-network-config.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/shell-completion.md` & `walt-client-8.1/walt/client/doc/md/shell-completion.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/shells.md` & `walt-client-8.1/walt/client/doc/md/shells.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/switch-install.md` & `walt-client-8.1/walt/client/doc/md/switch-install.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/troubleshooting.md` & `walt-client-8.1/walt/client/doc/md/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/tutorial.md` & `walt-client-8.1/walt/client/doc/md/tutorial.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/unmanaged-devices.md` & `walt-client-8.1/walt/client/doc/md/unmanaged-devices.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/vnode-networks.md` & `walt-client-8.1/walt/client/doc/md/vnode-networks.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/md/vpn.md` & `walt-client-8.1/walt/client/doc/md/vpn.md`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/mdtable.py` & `walt-client-8.1/walt/client/doc/mdtable.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/pager.py` & `walt-client-8.1/walt/client/doc/pager.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/doc/sphinx/conf.py` & `walt-client-8.1/walt/client/doc/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/exceptions.py` & `walt-client-8.1/walt/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/expose.py` & `walt-client-8.1/walt/client/expose.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/filesystem.py` & `walt-client-8.1/walt/client/filesystem.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/image.py` & `walt-client-8.1/walt/client/image.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/interactive.py` & `walt-client-8.1/walt/client/interactive.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/link.py` & `walt-client-8.1/walt/client/link.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/log.py` & `walt-client-8.1/walt/client/log.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/logo.py` & `walt-client-8.1/walt/client/logo.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/myhelp.py` & `walt-client-8.1/walt/client/myhelp.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/node.py` & `walt-client-8.1/walt/client/node.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/plugins.py` & `walt-client-8.1/walt/client/plugins.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/progress.py` & `walt-client-8.1/walt/client/progress.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/speedup.py` & `walt-client-8.1/walt/client/speedup.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/timeout.py` & `walt-client-8.1/walt/client/timeout.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/tools.py` & `walt-client-8.1/walt/client/tools.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/transfer.py` & `walt-client-8.1/walt/client/transfer.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/types.py` & `walt-client-8.1/walt/client/types.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/update.py` & `walt-client-8.1/walt/client/update.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/vpn.py` & `walt-client-8.1/walt/client/vpn.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt/client/wrap.py` & `walt-client-8.1/walt/client/wrap.py`

 * *Files identical despite different names*

### Comparing `walt-client-8.0/walt_client.egg-info/SOURCES.txt` & `walt-client-8.1/walt_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

