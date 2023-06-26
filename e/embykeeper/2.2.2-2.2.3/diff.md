# Comparing `tmp/embykeeper-2.2.2.tar.gz` & `tmp/embykeeper-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.2.tar", last modified: Sun Jun 25 17:04:45 2023, max compression
+gzip compressed data, was "embykeeper-2.2.3.tar", last modified: Mon Jun 26 05:16:06 2023, max compression
```

## Comparing `embykeeper-2.2.2.tar` & `embykeeper-2.2.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 17:04:33.000000 embykeeper-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 17:04:33.000000 embykeeper-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21662 2023-06-25 17:04:45.197747 embykeeper-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20764 2023-06-25 17:04:33.000000 embykeeper-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.189747 embykeeper-2.2.2/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.189747 embykeeper-2.2.2/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.185747 embykeeper-2.2.2/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21662 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:04:44.000000 embykeeper-2.2.2/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 17:04:45.000000 embykeeper-2.2.2/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.193747 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/cascadia-code.css
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.181747 embykeeper-2.2.2/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-25 17:04:33.000000 embykeeper-2.2.2/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-25 17:04:33.000000 embykeeper-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:04:45.197747 embykeeper-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:04:45.197747 embykeeper-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-25 17:04:33.000000 embykeeper-2.2.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 05:15:52.000000 embykeeper-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 05:15:52.000000 embykeeper-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-06-26 05:16:06.983669 embykeeper-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-06-26 05:15:52.000000 embykeeper-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.979669 embykeeper-2.2.3/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 05:16:06.000000 embykeeper-2.2.3/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/cascadia-code.css
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.975669 embykeeper-2.2.3/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-26 05:15:52.000000 embykeeper-2.2.3/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 05:15:52.000000 embykeeper-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:16:06.983669 embykeeper-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:16:06.983669 embykeeper-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-26 05:15:52.000000 embykeeper-2.2.3/tests/test_cli.py
```

### Comparing `embykeeper-2.2.2/LICENSE` & `embykeeper-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/PKG-INFO` & `embykeeper-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.2
+Version: 2.2.3
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -45,82 +45,96 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-
 - Emby 保活
+
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
-
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
+
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
-
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+
   - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### Railway 在线部署
+### 在线部署
+
+#### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
+#### Render.com
+
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
+
+[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+
+请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
-(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
 命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
-[proxy]
-hostname = "127.0.0.1"
-port = 1080
-scheme = "socks5"
-
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
+若您需要连接代理, 还需要在 `config.toml` 中追加代理配置:
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -193,15 +207,15 @@
 
 ```bash
 embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
 这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
@@ -299,77 +313,77 @@
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
 ## 配置项
 
-| 设置项       | 值类型             | 简介                                         | 默认值  |
-| ------------ | ------------------ | -------------------------------------------- | ------- |
-| `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
-| `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
+| 设置项         | 值类型                   | 简介                                         | 默认值    |
+| -------------- | ------------------------ | -------------------------------------------- | --------- |
+| `timeout`    | `int`                  | Telegram 机器人签到超时 (秒)                 | `120`   |
+| `retries`    | `int`                  | Telegram 机器人签到错误重试次数              | `4`     |
+| `concurrent` | `int`                  | Telegram 机器人签到最大并发                  | `1`     |
+| `random`     | `int`                  | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
-| `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
-| `proxy`      | `dict`             | 代理设置                                     | `{}`    |
-| `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
-| `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
+| `service`    | `dict`                 | 签到/水群/监视功能开启站点设置               | `{}`    |
+| `proxy`      | `dict`                 | 代理设置                                     | `{}`    |
+| `telegram`   | `list`                 | Telegram 账号设置 (支持多账号)               | `[]`    |
+| `emby`       | `list`                 | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
 
-| 设置项      | 值类型 | 简介           | 默认值               |
-| ----------- | ------ | -------------- | -------------------- |
+| 设置项        | 值类型   | 简介           | 默认值               |
+| ------------- | -------- | -------------- | -------------------- |
 | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
 
-| 站点        | 名称       |     | 站点        | 名称          |
-| ----------- | ---------- | --- | ----------- | ------------- |
-| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
-| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
-| Pornemby    | `pornemby` |     | Singularity | `singularity` |
-| Peach       | `peach`    |     | Nebula      | `nebula`      |
-| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
-| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
+| 站点        | 名称         |  | 站点        | 名称            |
+| ----------- | ------------ | - | ----------- | --------------- |
+| 垃圾影音    | `ljyy`     |  | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |  | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |  | Singularity | `singularity` |
+| Peach       | `peach`    |  | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |  | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |  | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                    | 默认值      |
-| ---------- | ------ | --------------------------------------- | ----------- |
-| `hostname` | `str`  | 代理服务器地址                          | `localhost` |
-| `port`     | `int`  | 代理端口号                              | `1080`      |
-| `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
+| 设置项       | 值类型  | 简介                                        | 默认值        |
+| ------------ | ------- | ------------------------------------------- | ------------- |
+| `hostname` | `str` | 代理服务器地址                              | `localhost` |
+| `port`     | `int` | 代理端口号                                  | `1080`      |
+| `scheme`   | `str` | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                               | 默认值  |
-| ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
-| `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
-| `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
-| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+| 设置项       | 值类型   | 简介                                                                   | 默认值    |
+| ------------ | -------- | ---------------------------------------------------------------------- | --------- |
+| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                        |           |
+| `monitor`  | `bool` | 启用群组监控系列功能                                                   | `false` |
+| `send`     | `bool` | 启用自动水群系列功能                                                   | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |           |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |           |
 
 如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                      | 默认值 |
-| ---------- | ------ | --------------------------------------------------------- | ------ |
-| `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
-| `username` | `str`  | Emby 服务器用户名                                         |        |
-| `password` | `str`  | Emby 服务器密码                                           |        |
-| `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
-| `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
+| 设置项       | 值类型  | 简介                                                          | 默认值   |
+| ------------ | ------- | ------------------------------------------------------------- | -------- |
+| `url`      | `str` | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |          |
+| `username` | `str` | Emby 服务器用户名                                             |          |
+| `password` | `str` | Emby 服务器密码                                               |          |
+| `time`     | `int` | 模拟观看的时间 (秒)                                           | `800`  |
+| `progress` | `int` | 观看后模拟进度条保存的时间 (秒)                               | `1000` |
 
 服务可以进行特定配置, 如下所示:
 
 ```toml
 
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.2 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.3 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -85,35 +85,43 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
-å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
+å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
-embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
-ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
-æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
-embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
-net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
-`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
-" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
+06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
+5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
+(https://render.com/images/deploy-to-render-button.svg)](https://render.com/
+deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
+[Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
+tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
+å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
+embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
+`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
+"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
+`config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
+port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -137,15 +145,15 @@
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
 ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
 ```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
@@ -171,62 +179,62 @@
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
 -I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
--- | ------------------ | -------------------------------------------- | ------
-- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
-`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
-`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
-| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
-| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
-ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+---- | ------------------------ | -------------------------------------------
+- | --------- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) |
+`120` | | `retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4`
+| | `concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | |
+`random` | `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé)
+| `15` | | `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å·
+(åºå·/ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
 çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
 {}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 | `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
-------- | ------ | -------------- | -------------------- | | `checkiner` |
+--------- | -------- | -------------- | -------------------- | | `checkiner` |
 `list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
 `list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
 `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
 å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
 è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
------ | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
-| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ------------ | - | ------
+----- | --------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot`
+| | å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
 `pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
 `nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------------------
+------------ | ------------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
-`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
-`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----------
+- | -------- | ----------------------------------------------------------------
+------ | --------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
 (å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
 | | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
 my.telegram.org/)ç³è¯·ç Application Hash | |
 å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
 æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
 my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
 development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
 æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
 æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
 æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
 api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------------------------ | ------ | | `url` | `str` | Emby
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------
+------------------------------------------ | -------- | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.2/README.md` & `embykeeper-2.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,82 +24,96 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-
 - Emby 保活
+
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
-
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
+
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
-
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+
   - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### Railway 在线部署
+### 在线部署
+
+#### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
+#### Render.com
+
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
+
+[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+
+请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
-(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
 命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
-[proxy]
-hostname = "127.0.0.1"
-port = 1080
-scheme = "socks5"
-
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
+若您需要连接代理, 还需要在 `config.toml` 中追加代理配置:
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -172,15 +186,15 @@
 
 ```bash
 embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
 这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
@@ -278,77 +292,77 @@
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
 ## 配置项
 
-| 设置项       | 值类型             | 简介                                         | 默认值  |
-| ------------ | ------------------ | -------------------------------------------- | ------- |
-| `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
-| `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
+| 设置项         | 值类型                   | 简介                                         | 默认值    |
+| -------------- | ------------------------ | -------------------------------------------- | --------- |
+| `timeout`    | `int`                  | Telegram 机器人签到超时 (秒)                 | `120`   |
+| `retries`    | `int`                  | Telegram 机器人签到错误重试次数              | `4`     |
+| `concurrent` | `int`                  | Telegram 机器人签到最大并发                  | `1`     |
+| `random`     | `int`                  | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
-| `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
-| `proxy`      | `dict`             | 代理设置                                     | `{}`    |
-| `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
-| `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
+| `service`    | `dict`                 | 签到/水群/监视功能开启站点设置               | `{}`    |
+| `proxy`      | `dict`                 | 代理设置                                     | `{}`    |
+| `telegram`   | `list`                 | Telegram 账号设置 (支持多账号)               | `[]`    |
+| `emby`       | `list`                 | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
 
-| 设置项      | 值类型 | 简介           | 默认值               |
-| ----------- | ------ | -------------- | -------------------- |
+| 设置项        | 值类型   | 简介           | 默认值               |
+| ------------- | -------- | -------------- | -------------------- |
 | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
 
-| 站点        | 名称       |     | 站点        | 名称          |
-| ----------- | ---------- | --- | ----------- | ------------- |
-| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
-| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
-| Pornemby    | `pornemby` |     | Singularity | `singularity` |
-| Peach       | `peach`    |     | Nebula      | `nebula`      |
-| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
-| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
+| 站点        | 名称         |  | 站点        | 名称            |
+| ----------- | ------------ | - | ----------- | --------------- |
+| 垃圾影音    | `ljyy`     |  | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |  | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |  | Singularity | `singularity` |
+| Peach       | `peach`    |  | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |  | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |  | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                    | 默认值      |
-| ---------- | ------ | --------------------------------------- | ----------- |
-| `hostname` | `str`  | 代理服务器地址                          | `localhost` |
-| `port`     | `int`  | 代理端口号                              | `1080`      |
-| `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
+| 设置项       | 值类型  | 简介                                        | 默认值        |
+| ------------ | ------- | ------------------------------------------- | ------------- |
+| `hostname` | `str` | 代理服务器地址                              | `localhost` |
+| `port`     | `int` | 代理端口号                                  | `1080`      |
+| `scheme`   | `str` | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                               | 默认值  |
-| ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
-| `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
-| `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
-| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+| 设置项       | 值类型   | 简介                                                                   | 默认值    |
+| ------------ | -------- | ---------------------------------------------------------------------- | --------- |
+| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                        |           |
+| `monitor`  | `bool` | 启用群组监控系列功能                                                   | `false` |
+| `send`     | `bool` | 启用自动水群系列功能                                                   | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |           |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |           |
 
 如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                      | 默认值 |
-| ---------- | ------ | --------------------------------------------------------- | ------ |
-| `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
-| `username` | `str`  | Emby 服务器用户名                                         |        |
-| `password` | `str`  | Emby 服务器密码                                           |        |
-| `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
-| `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
+| 设置项       | 值类型  | 简介                                                          | 默认值   |
+| ------------ | ------- | ------------------------------------------------------------- | -------- |
+| `url`      | `str` | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |          |
+| `username` | `str` | Emby 服务器用户名                                             |          |
+| `password` | `str` | Emby 服务器密码                                               |          |
+| `time`     | `int` | 模拟观看的时间 (秒)                                           | `800`  |
+| `progress` | `int` | 观看后模拟进度条保存的时间 (秒)                               | `1000` |
 
 服务可以进行特定配置, 如下所示:
 
 ```toml
 
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
```

#### html2text {}

```diff
@@ -73,35 +73,43 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
-å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
+å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
-embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
-ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
-æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
-embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
-net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
-`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
-" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
+06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
+5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
+(https://render.com/images/deploy-to-render-button.svg)](https://render.com/
+deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
+[Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
+tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
+å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
+embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
+`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
+"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
+`config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
+port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -125,15 +133,15 @@
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
 ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
 ```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
@@ -159,62 +167,62 @@
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
 -I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
--- | ------------------ | -------------------------------------------- | ------
-- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
-`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
-`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
-| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
-| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
-ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+---- | ------------------------ | -------------------------------------------
+- | --------- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) |
+`120` | | `retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4`
+| | `concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | |
+`random` | `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé)
+| `15` | | `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å·
+(åºå·/ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
 çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
 {}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 | `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
-------- | ------ | -------------- | -------------------- | | `checkiner` |
+--------- | -------- | -------------- | -------------------- | | `checkiner` |
 `list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
 `list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
 `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
 å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
 è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
------ | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
-| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ------------ | - | ------
+----- | --------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot`
+| | å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
 `pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
 `nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------------------
+------------ | ------------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
-`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
-`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----------
+- | -------- | ----------------------------------------------------------------
+------ | --------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
 (å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
 | | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
 my.telegram.org/)ç³è¯·ç Application Hash | |
 å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
 æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
 my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
 development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
 æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
 æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
 æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
 api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------------------------ | ------ | | `url` | `str` | Emby
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------
+------------------------------------------ | -------- | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.2/embykeeper/cli.py` & `embykeeper-2.2.3/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/data.py` & `embykeeper-2.2.3/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.3/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/embywatcher/main.py` & `embykeeper-2.2.3/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/log.py` & `embykeeper-2.2.3/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/settings.py` & `embykeeper-2.2.3/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.3/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/link.py` & `embykeeper-2.2.3/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/log.py` & `embykeeper-2.2.3/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/main.py` & `embykeeper-2.2.3/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.3/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.3/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.3/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/telechecker/tele.py` & `embykeeper-2.2.3/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper/utils.py` & `embykeeper-2.2.3/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.3/embykeeper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.2
+Version: 2.2.3
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -45,82 +45,96 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+
   - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
-
 - Emby 保活
+
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
-
 - Telegram 自动水群 (默认使用内建话术列表, 易被辨别和封禁, 请谨慎使用)
+
   - 默认禁用:
     - ~~NakoNako 自动水群: [群组](https://t.me/NakoNetwork) [机器人](https://t.me/nakonetwork_bot)~~ (停服)
-
 - Telegram 自动监控信息 (需要[超级用户](https://t.me/embykeeper_bot?start=__prime))
+
   - Pornemby 科举考试: [活动频道](https://t.me/PornembyFun) (由于需要使用 OpenAI API 进行回答, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime), 回答准确率一般请谨慎使用)
   - 不给看 抢邀请码: [群组](https://t.me/Ephemeralemby) [机器人](https://t.me/UnknownEmbyBot)
   - Viper 抢邀请码: [频道](https://t.me/viper_emby_channel) [群组](https://t.me/Viper_Emby_Chat) [机器人](https://t.me/viper_emby_bot)
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### Railway 在线部署
+### 在线部署
+
+#### Railway
 
 Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/06/25/embykeeper-railway-tutorial/)
 
 请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
+#### Render.com
+
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
+
+[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+
+请注意 Render.com 的 Web 服务不活跃 15 分钟将自动停止, 因此必须部署云监控以持续激活.
+
 ### 通过 Docker 部署
 
 Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
-(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
 命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
-[proxy]
-hostname = "127.0.0.1"
-port = 1080
-scheme = "socks5"
-
 [[telegram]]
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
+若您需要连接代理, 还需要在 `config.toml` 中追加代理配置:
+
+```toml
+[proxy]
+hostname = "127.0.0.1"
+port = 1080
+scheme = "socks5"
+```
+
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -193,15 +207,15 @@
 
 ```bash
 embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过 `Ctrl+C`停止, 然后运行:
 
 ```bash
 tmux
 ```
 
 这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
@@ -299,77 +313,77 @@
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
 ## 配置项
 
-| 设置项       | 值类型             | 简介                                         | 默认值  |
-| ------------ | ------------------ | -------------------------------------------- | ------- |
-| `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
-| `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
-| `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
+| 设置项         | 值类型                   | 简介                                         | 默认值    |
+| -------------- | ------------------------ | -------------------------------------------- | --------- |
+| `timeout`    | `int`                  | Telegram 机器人签到超时 (秒)                 | `120`   |
+| `retries`    | `int`                  | Telegram 机器人签到错误重试次数              | `4`     |
+| `concurrent` | `int`                  | Telegram 机器人签到最大并发                  | `1`     |
+| `random`     | `int`                  | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
-| `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
-| `proxy`      | `dict`             | 代理设置                                     | `{}`    |
-| `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
-| `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
+| `service`    | `dict`                 | 签到/水群/监视功能开启站点设置               | `{}`    |
+| `proxy`      | `dict`                 | 代理设置                                     | `{}`    |
+| `telegram`   | `list`                 | Telegram 账号设置 (支持多账号)               | `[]`    |
+| `emby`       | `list`                 | Emby 账号设置 (支持多账号)                   | `[]`    |
 
 `service`设置可以为:
 
-| 设置项      | 值类型 | 简介           | 默认值               |
-| ----------- | ------ | -------------- | -------------------- |
+| 设置项        | 值类型   | 简介           | 默认值               |
+| ------------- | -------- | -------------- | -------------------- |
 | `checkiner` | `list` | 启用的签到站点 | (当前所有支持的站点) |
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
 
-| 站点        | 名称       |     | 站点        | 名称          |
-| ----------- | ---------- | --- | ----------- | ------------- |
-| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
-| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
-| Pornemby    | `pornemby` |     | Singularity | `singularity` |
-| Peach       | `peach`    |     | Nebula      | `nebula`      |
-| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
-| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
+| 站点        | 名称         |  | 站点        | 名称            |
+| ----------- | ------------ | - | ----------- | --------------- |
+| 垃圾影音    | `ljyy`     |  | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |  | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |  | Singularity | `singularity` |
+| Peach       | `peach`    |  | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |  | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |  | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                    | 默认值      |
-| ---------- | ------ | --------------------------------------- | ----------- |
-| `hostname` | `str`  | 代理服务器地址                          | `localhost` |
-| `port`     | `int`  | 代理端口号                              | `1080`      |
-| `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
+| 设置项       | 值类型  | 简介                                        | 默认值        |
+| ------------ | ------- | ------------------------------------------- | ------------- |
+| `hostname` | `str` | 代理服务器地址                              | `localhost` |
+| `port`     | `int` | 代理端口号                                  | `1080`      |
+| `scheme`   | `str` | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                               | 默认值  |
-| ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
-| `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
-| `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
-| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+| 设置项       | 值类型   | 简介                                                                   | 默认值    |
+| ------------ | -------- | ---------------------------------------------------------------------- | --------- |
+| `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                        |           |
+| `monitor`  | `bool` | 启用群组监控系列功能                                                   | `false` |
+| `send`     | `bool` | 启用自动水群系列功能                                                   | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |           |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |           |
 
 如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
-| 设置项     | 值类型 | 简介                                                      | 默认值 |
-| ---------- | ------ | --------------------------------------------------------- | ------ |
-| `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
-| `username` | `str`  | Emby 服务器用户名                                         |        |
-| `password` | `str`  | Emby 服务器密码                                           |        |
-| `time`     | `int`  | 模拟观看的时间 (秒)                                       | `800`  |
-| `progress` | `int`  | 观看后模拟进度条保存的时间 (秒)                           | `1000` |
+| 设置项       | 值类型  | 简介                                                          | 默认值   |
+| ------------ | ------- | ------------------------------------------------------------- | -------- |
+| `url`      | `str` | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |          |
+| `username` | `str` | Emby 服务器用户名                                             |          |
+| `password` | `str` | Emby 服务器密码                                               |          |
+| `time`     | `int` | 模拟观看的时间 (秒)                                           | `800`  |
+| `progress` | `int` | 观看后模拟进度条保存的时间 (秒)                               | `1000` |
 
 服务可以进行特定配置, 如下所示:
 
 ```toml
 
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.2 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.3 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
@@ -85,35 +85,43 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
-å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ###
+å¨çº¿é¨ç½² #### Railway Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
 æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
 (https://railway.app/button.svg)](https://railway.app/template/
 WFYaj9?referralCode=Fj6Yvy)       [![Tutorial](https://github.com/embykeeper/
-embykeeper/raw/main/images/tutorial.svg)](https://blog.iair.top/2023/06/25/
-embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
-ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
-é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
-æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
-ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
-embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
-net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
-`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
-æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
-```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
-" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+embykeeper/raw/main/images/railway-tutorial.svg)](https://blog.iair.top/2023/
+06/25/embykeeper-railway-tutorial/) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ
+5 ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². #### Render.com Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy to Render]
+(https://render.com/images/deploy-to-render-button.svg)](https://render.com/
+deploy?repo=https://github.com/embykeeper/embykeeper/tree/stable)       [!
+[Tutorial](https://github.com/embykeeper/embykeeper/raw/main/images/render-
+tutorial.svg)](https://blog.iair.top/2023/06/26/embykeeper-render-tutorial)
+è¯·æ³¨æ Render.com ç Web æå¡ä¸æ´»è· 15 åéå°èªå¨åæ­¢,
+å æ­¤å¿é¡»é¨ç½²äºçæ§ä»¥æç»­æ¿æ´». ### éè¿ Docker é¨ç½² Embykeeper
+å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://yeasy.gitbook.io/
+docker_practice/install), ç¶åæ§è¡: ```bash docker run -v $(pwd)/
+embykeeper:/app --rm -it --net=host embykeeper/embykeeper ``` å½ä»¤å°ä¼å¨
+`embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
+(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [[telegram]] phone =
+"+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` è¥æ¨éè¦è¿æ¥ä»£ç, è¿éè¦å¨
+`config.toml` ä¸­è¿½å ä»£çéç½®: ```toml [proxy] hostname = "127.0.0.1"
+port = 1080 scheme = "socks5" ``` éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker
+run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -137,15 +145,15 @@
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
 æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
 å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿ `Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
 ``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
 æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
 Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
 æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
 ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
 ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
 ```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
@@ -171,62 +179,62 @@
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
 -I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
--- | ------------------ | -------------------------------------------- | ------
-- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
-`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
-`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
-| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
-| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
-ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+---- | ------------------------ | -------------------------------------------
+- | --------- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) |
+`120` | | `retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4`
+| | `concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | |
+`random` | `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé)
+| `15` | | `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å·
+(åºå·/ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
 çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
 {}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 | `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
 `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
-------- | ------ | -------------- | -------------------- | | `checkiner` |
+--------- | -------- | -------------- | -------------------- | | `checkiner` |
 `list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
 `list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
 `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
 å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
 è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
 è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
 æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
------ | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
-| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ------------ | - | ------
+----- | --------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot`
+| | å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
 `pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
 `nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
------ | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------------------
+------------ | ------------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
-è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
------- | ------------------------------------------------------------------ | -
------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
-`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
-`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----------
+- | -------- | ----------------------------------------------------------------
+------ | --------- | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
+| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
+| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
 (å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
 | | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
 my.telegram.org/)ç³è¯·ç Application Hash | |
 å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
 æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
 my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
 development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
 æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
 æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
 æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
 api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
------------------------------------ | ------ | | `url` | `str` | Emby
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ------------ | ------- | -------------------
+------------------------------------------ | -------- | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.2/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.3/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/app.py` & `embykeeper-2.2.3/embykeeperweb/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import termios
 import time
 import signal
 
 import typer
 from loguru import logger
-from flask import Flask, render_template, request, redirect, url_for
+from flask import Flask, render_template, request, redirect, url_for, jsonify, abort
 from flask_socketio import SocketIO
 from flask_login import LoginManager, login_user, login_required
 
 cli = typer.Typer()
 app = Flask(__name__, static_folder="templates/assets")
 app.config["SECRET_KEY"] = os.urandom(24)
 socketio = SocketIO(app)
@@ -78,14 +78,41 @@
             return redirect(request.args.get("next") or url_for("index"))
         else:
             emsg = "Wrong password."
             app.config["faillog"].append(time.time())
     return render_template("login.html", emsg=emsg)
 
 
+@app.route("/healthz")
+def healthz():
+    return "200 OK"
+
+
+@app.route("/heartbeat")
+def heartbeat():
+    webpass = os.environ.get("EK_WEBPASS", "")
+    password = request.args.get("pass", None)
+    if (not password) or (not webpass):
+        return abort(403)
+    if password == webpass:
+        if app.config["pid"] is None:
+            (pid, fd) = pty.fork()
+            if pid == 0:
+                subprocess.run(["embykeeper", *app.config["args"]])
+            else:
+                app.config["fd"] = fd
+                app.config["pid"] = pid
+                logger.debug(f"Embykeeper started at: {pid}.")
+            return jsonify({"status": "restarted", "pid": pid})
+        else:
+            return jsonify({"status": "running", "pid": app.config["pid"]})
+    else:
+        return abort(403)
+
+
 @app.errorhandler(404)
 def page_not_found(e):
     return render_template("404.html"), 404
 
 
 @socketio.on("pty-input", namespace="/pty")
 def pty_input(data):
```

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/404.html` & `embykeeper-2.2.3/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.3/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.2.3/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.3/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.3/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/console.html` & `embykeeper-2.2.3/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/embykeeperweb/templates/login.html` & `embykeeper-2.2.3/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.2/pyproject.toml` & `embykeeper-2.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.2.2/tests/test_cli.py` & `embykeeper-2.2.3/tests/test_cli.py`

 * *Files identical despite different names*

