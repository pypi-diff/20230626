# Comparing `tmp/botoolkit-1.1.8.tar.gz` & `tmp/botoolkit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botoolkit-1.1.8.tar", last modified: Thu Jul 21 19:02:54 2022, max compression
+gzip compressed data, was "botoolkit-1.1.9.tar", last modified: Mon Aug 22 08:47:47 2022, max compression
```

## Comparing `botoolkit-1.1.8.tar` & `botoolkit-1.1.9.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.559571 botoolkit-1.1.8/
--rw-r--r--   0 root         (0) root         (0)    32691 2022-07-21 19:02:42.000000 botoolkit-1.1.8/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)      309 2022-04-27 09:28:05.000000 botoolkit-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    34560 2022-07-21 19:02:54.559571 botoolkit-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1321 2022-05-24 12:11:37.000000 botoolkit-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.529571 botoolkit-1.1.8/botoolkit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.532571 botoolkit-1.1.8/botoolkit/bo_barsdock/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1214 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/commands.py
--rw-r--r--   0 root         (0) root         (0)      112 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/enums.py
--rw-r--r--   0 root         (0) root         (0)      681 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/main.py
--rw-r--r--   0 root         (0) root         (0)      512 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/mixins.py
--rw-r--r--   0 root         (0) root         (0)      382 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.532571 botoolkit-1.1.8/botoolkit/bo_barsdock/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_barsdock/templates/bobarsdock.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.534571 botoolkit-1.1.8/botoolkit/bo_conf/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20002 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/api.py
--rw-r--r--   0 root         (0) root         (0)    26830 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_conf/commands.py
--rw-r--r--   0 root         (0) root         (0)       42 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/consts.py
--rw-r--r--   0 root         (0) root         (0)    43427 2022-05-22 19:42:29.000000 botoolkit-1.1.8/botoolkit/bo_conf/enums.py
--rw-r--r--   0 root         (0) root         (0)     1891 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1063 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/main.py
--rw-r--r--   0 root         (0) root         (0)     6165 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/mixins.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/settings.py
--rw-r--r--   0 root         (0) root         (0)      287 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.534571 botoolkit-1.1.8/botoolkit/bo_conf/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_conf/templates/boconf.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.535571 botoolkit-1.1.8/botoolkit/bo_databaser/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28742 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/commands.py
--rw-r--r--   0 root         (0) root         (0)       34 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/consts.py
--rw-r--r--   0 root         (0) root         (0)      695 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/main.py
--rw-r--r--   0 root         (0) root         (0)    18815 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/mixins.py
--rw-r--r--   0 root         (0) root         (0)     3183 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/services.py
--rw-r--r--   0 root         (0) root         (0)      787 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.536571 botoolkit-1.1.8/botoolkit/bo_databaser/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      532 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/templates/bodatabaser.conf
--rw-r--r--   0 root         (0) root         (0)     1094 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_databaser/templates/bodatabaser_build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.537571 botoolkit-1.1.8/botoolkit/bo_git/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11382 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_git/commands.py
--rw-r--r--   0 root         (0) root         (0)      845 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/enums.py
--rw-r--r--   0 root         (0) root         (0)     1367 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/helpers.py
--rw-r--r--   0 root         (0) root         (0)      641 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/main.py
--rw-r--r--   0 root         (0) root         (0)     5700 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/mixins.py
--rw-r--r--   0 root         (0) root         (0)      561 2022-05-24 12:11:37.000000 botoolkit-1.1.8/botoolkit/bo_git/settings.py
--rw-r--r--   0 root         (0) root         (0)      470 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.538571 botoolkit-1.1.8/botoolkit/bo_git/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_git/templates/bogit.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.539571 botoolkit-1.1.8/botoolkit/bo_guide/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7730 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/commands.py
--rw-r--r--   0 root         (0) root         (0)      270 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/consts.py
--rw-r--r--   0 root         (0) root         (0)      667 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/main.py
--rw-r--r--   0 root         (0) root         (0)     6816 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/mixins.py
--rw-r--r--   0 root         (0) root         (0)      465 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.539571 botoolkit-1.1.8/botoolkit/bo_guide/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      213 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_guide/templates/boguide.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.541571 botoolkit-1.1.8/botoolkit/bo_ip/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5165 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/api.py
--rw-r--r--   0 root         (0) root         (0)     5076 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_ip/commands.py
--rw-r--r--   0 root         (0) root         (0)      201 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/enums.py
--rw-r--r--   0 root         (0) root         (0)      689 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/helpers.py
--rw-r--r--   0 root         (0) root         (0)      643 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/main.py
--rw-r--r--   0 root         (0) root         (0)      208 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/settings.py
--rw-r--r--   0 root         (0) root         (0)       28 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_ip/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.543571 botoolkit-1.1.8/botoolkit/bo_jenkins/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37344 2022-06-14 21:31:44.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/commands.py
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/consts.py
--rw-r--r--   0 root         (0) root         (0)      421 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/enums.py
--rw-r--r--   0 root         (0) root         (0)     4044 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/generators.py
--rw-r--r--   0 root         (0) root         (0)      987 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/helpers.py
--rw-r--r--   0 root         (0) root         (0)      704 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/main.py
--rw-r--r--   0 root         (0) root         (0)     7779 2022-06-14 21:31:44.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/mixins.py
--rw-r--r--   0 root         (0) root         (0)    11584 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/parsers.py
--rw-r--r--   0 root         (0) root         (0)      741 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/settings.py
--rw-r--r--   0 root         (0) root         (0)      764 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.543571 botoolkit-1.1.8/botoolkit/bo_jenkins/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      313 2022-06-14 21:31:44.000000 botoolkit-1.1.8/botoolkit/bo_jenkins/templates/bojenkins.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.545571 botoolkit-1.1.8/botoolkit/bo_jira/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1504 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/api.py
--rw-r--r--   0 root         (0) root         (0)     5447 2022-05-26 12:27:22.000000 botoolkit-1.1.8/botoolkit/bo_jira/commands.py
--rw-r--r--   0 root         (0) root         (0)      589 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/consts.py
--rw-r--r--   0 root         (0) root         (0)     1064 2022-05-24 12:11:37.000000 botoolkit-1.1.8/botoolkit/bo_jira/enums.py
--rw-r--r--   0 root         (0) root         (0)      172 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/helpers.py
--rw-r--r--   0 root         (0) root         (0)      677 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/main.py
--rw-r--r--   0 root         (0) root         (0)     3995 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/mixins.py
--rw-r--r--   0 root         (0) root         (0)      487 2022-05-25 12:29:29.000000 botoolkit-1.1.8/botoolkit/bo_jira/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.545571 botoolkit-1.1.8/botoolkit/bo_jira/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_jira/templates/bojira.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.548571 botoolkit-1.1.8/botoolkit/bo_postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2014 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/command_validators.py
--rw-r--r--   0 root         (0) root         (0)    41201 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_postgres/commands.py
--rw-r--r--   0 root         (0) root         (0)      158 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/consts.py
--rw-r--r--   0 root         (0) root         (0)     3517 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/entities.py
--rw-r--r--   0 root         (0) root         (0)      191 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/enums.py
--rw-r--r--   0 root         (0) root         (0)     2344 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/exporters.py
--rw-r--r--   0 root         (0) root         (0)    10968 2022-06-14 20:15:50.000000 botoolkit-1.1.8/botoolkit/bo_postgres/generators.py
--rw-r--r--   0 root         (0) root         (0)     3838 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/helpers.py
--rw-r--r--   0 root         (0) root         (0)      686 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/main.py
--rw-r--r--   0 root         (0) root         (0)    18966 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/mixins.py
--rw-r--r--   0 root         (0) root         (0)      645 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/repositories.py
--rw-r--r--   0 root         (0) root         (0)     2809 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/services.py
--rw-r--r--   0 root         (0) root         (0)      942 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/settings.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.548571 botoolkit-1.1.8/botoolkit/bo_postgres/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      510 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_postgres/templates/bopostgres.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.549571 botoolkit-1.1.8/botoolkit/bo_registry/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9946 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/commands.py
--rw-r--r--   0 root         (0) root         (0)     8424 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/helpers.py
--rw-r--r--   0 root         (0) root         (0)      686 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/main.py
--rw-r--r--   0 root         (0) root         (0)     4096 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/mixins.py
--rw-r--r--   0 root         (0) root         (0)      664 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.550571 botoolkit-1.1.8/botoolkit/bo_registry/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_registry/templates/boregistry.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.551571 botoolkit-1.1.8/botoolkit/bo_telegram/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1257 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/commands.py
--rw-r--r--   0 root         (0) root         (0)     1177 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/helpers.py
--rw-r--r--   0 root         (0) root         (0)      680 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/main.py
--rw-r--r--   0 root         (0) root         (0)      464 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/mixins.py
--rw-r--r--   0 root         (0) root         (0)      382 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.551571 botoolkit-1.1.8/botoolkit/bo_telegram/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_telegram/templates/botelegram.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.552571 botoolkit-1.1.8/botoolkit/bo_toolkit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24990 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/commands.py
--rw-r--r--   0 root         (0) root         (0)      124 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/consts.py
--rw-r--r--   0 root         (0) root         (0)      608 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/helpers.py
--rw-r--r--   0 root         (0) root         (0)      721 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/main.py
--rw-r--r--   0 root         (0) root         (0)     5081 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/mixins.py
--rw-r--r--   0 root         (0) root         (0)      528 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/settings.py
--rw-r--r--   0 root         (0) root         (0)      201 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.553571 botoolkit-1.1.8/botoolkit/bo_toolkit/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4461 2022-07-14 04:59:55.000000 botoolkit-1.1.8/botoolkit/bo_toolkit/templates/botoolkit.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.555571 botoolkit-1.1.8/botoolkit/bo_web_bb/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1388 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/api.py
--rw-r--r--   0 root         (0) root         (0)     3698 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/commands.py
--rw-r--r--   0 root         (0) root         (0)     1011 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/consts.py
--rw-r--r--   0 root         (0) root         (0)    41935 2022-07-21 19:02:42.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/enums.py
--rw-r--r--   0 root         (0) root         (0)      175 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      849 2022-06-01 18:43:21.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.555571 botoolkit-1.1.8/botoolkit/bo_web_bb/images/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.556571 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/
--rwxr-xr-x   0 root         (0) root         (0)     2038 2022-07-21 15:07:55.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2485 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py
--rwxr-xr-x   0 root         (0) root         (0)     4306 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      788 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl
--rw-r--r--   0 root         (0) root         (0)     1477 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.556571 botoolkit-1.1.8/botoolkit/bo_web_bb/images/web_bb_app/
--rwxr-xr-x   0 root         (0) root         (0)      534 2022-07-21 15:07:55.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/images/web_bb_app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/main.py
--rw-r--r--   0 root         (0) root         (0)     6161 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/mixins.py
--rw-r--r--   0 root         (0) root         (0)     6429 2022-07-21 15:07:55.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/services.py
--rw-r--r--   0 root         (0) root         (0)      972 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/settings.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.556571 botoolkit-1.1.8/botoolkit/bo_web_bb/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/bo_web_bb/templates/bowebbb.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.558571 botoolkit-1.1.8/botoolkit/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26495 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/commands.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-07-21 15:07:55.000000 botoolkit-1.1.8/botoolkit/core/consts.py
--rw-r--r--   0 root         (0) root         (0)     1253 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/enums.py
--rw-r--r--   0 root         (0) root         (0)     2565 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/exporters.py
--rw-r--r--   0 root         (0) root         (0)     9972 2022-06-01 18:43:21.000000 botoolkit-1.1.8/botoolkit/core/helpers.py
--rw-r--r--   0 root         (0) root         (0)      364 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/loggers.py
--rw-r--r--   0 root         (0) root         (0)     3531 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/mixins.py
--rw-r--r--   0 root         (0) root         (0)     4279 2022-07-21 15:07:55.000000 botoolkit-1.1.8/botoolkit/core/services.py
--rw-r--r--   0 root         (0) root         (0)     1961 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/core/strings.py
--rw-r--r--   0 root         (0) root         (0)     1923 2022-04-27 09:28:05.000000 botoolkit-1.1.8/botoolkit/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.531571 botoolkit-1.1.8/botoolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)    34560 2022-07-21 19:02:53.000000 botoolkit-1.1.8/botoolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5737 2022-07-21 19:02:54.000000 botoolkit-1.1.8/botoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-21 19:02:53.000000 botoolkit-1.1.8/botoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     3650 2022-07-21 19:02:54.000000 botoolkit-1.1.8/botoolkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-21 19:02:54.000000 botoolkit-1.1.8/botoolkit.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-27 09:28:14.000000 botoolkit-1.1.8/botoolkit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      248 2022-07-21 19:02:54.000000 botoolkit-1.1.8/botoolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-07-21 19:02:54.000000 botoolkit-1.1.8/botoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-21 19:02:54.558571 botoolkit-1.1.8/docs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.8/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      391 2022-04-27 09:28:05.000000 botoolkit-1.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-21 19:02:54.559571 botoolkit-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1913 2022-07-21 19:02:42.000000 botoolkit-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.452899 botoolkit-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)    32745 2022-08-22 08:47:38.000000 botoolkit-1.1.9/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)      309 2022-04-27 09:28:05.000000 botoolkit-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    34614 2022-08-22 08:47:47.451899 botoolkit-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1321 2022-05-24 12:11:37.000000 botoolkit-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.354899 botoolkit-1.1.9/botoolkit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.361899 botoolkit-1.1.9/botoolkit/bo_barsdock/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/commands.py
+-rw-r--r--   0 root         (0) root         (0)      112 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/enums.py
+-rw-r--r--   0 root         (0) root         (0)      681 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/main.py
+-rw-r--r--   0 root         (0) root         (0)      512 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      382 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.362899 botoolkit-1.1.9/botoolkit/bo_barsdock/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_barsdock/templates/bobarsdock.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.366899 botoolkit-1.1.9/botoolkit/bo_conf/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20002 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/api.py
+-rw-r--r--   0 root         (0) root         (0)    26830 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_conf/commands.py
+-rw-r--r--   0 root         (0) root         (0)       42 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/consts.py
+-rw-r--r--   0 root         (0) root         (0)    43427 2022-05-22 19:42:29.000000 botoolkit-1.1.9/botoolkit/bo_conf/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/main.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      897 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/settings.py
+-rw-r--r--   0 root         (0) root         (0)      287 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.367899 botoolkit-1.1.9/botoolkit/bo_conf/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_conf/templates/boconf.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.373899 botoolkit-1.1.9/botoolkit/bo_databaser/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28742 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/commands.py
+-rw-r--r--   0 root         (0) root         (0)       34 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/consts.py
+-rw-r--r--   0 root         (0) root         (0)      695 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/main.py
+-rw-r--r--   0 root         (0) root         (0)    18815 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/services.py
+-rw-r--r--   0 root         (0) root         (0)      787 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.375899 botoolkit-1.1.9/botoolkit/bo_databaser/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      532 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/templates/bodatabaser.conf
+-rw-r--r--   0 root         (0) root         (0)     1094 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_databaser/templates/bodatabaser_build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.381898 botoolkit-1.1.9/botoolkit/bo_git/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11382 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_git/commands.py
+-rw-r--r--   0 root         (0) root         (0)      845 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      641 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/main.py
+-rw-r--r--   0 root         (0) root         (0)     5700 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      561 2022-05-24 12:11:37.000000 botoolkit-1.1.9/botoolkit/bo_git/settings.py
+-rw-r--r--   0 root         (0) root         (0)      470 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.382899 botoolkit-1.1.9/botoolkit/bo_git/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_git/templates/bogit.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.387899 botoolkit-1.1.9/botoolkit/bo_guide/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/commands.py
+-rw-r--r--   0 root         (0) root         (0)      270 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/consts.py
+-rw-r--r--   0 root         (0) root         (0)      667 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/main.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      465 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.388899 botoolkit-1.1.9/botoolkit/bo_guide/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      213 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_guide/templates/boguide.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.396899 botoolkit-1.1.9/botoolkit/bo_ip/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5165 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/api.py
+-rw-r--r--   0 root         (0) root         (0)     5076 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_ip/commands.py
+-rw-r--r--   0 root         (0) root         (0)      201 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/enums.py
+-rw-r--r--   0 root         (0) root         (0)      689 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      643 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/main.py
+-rw-r--r--   0 root         (0) root         (0)      208 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/settings.py
+-rw-r--r--   0 root         (0) root         (0)       28 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_ip/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.410899 botoolkit-1.1.9/botoolkit/bo_jenkins/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37344 2022-06-14 21:31:44.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/commands.py
+-rw-r--r--   0 root         (0) root         (0)      156 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/consts.py
+-rw-r--r--   0 root         (0) root         (0)      421 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/enums.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/generators.py
+-rw-r--r--   0 root         (0) root         (0)      987 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      704 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/main.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2022-06-14 21:31:44.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    11584 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/parsers.py
+-rw-r--r--   0 root         (0) root         (0)      741 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/settings.py
+-rw-r--r--   0 root         (0) root         (0)      764 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.411899 botoolkit-1.1.9/botoolkit/bo_jenkins/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      313 2022-06-14 21:31:44.000000 botoolkit-1.1.9/botoolkit/bo_jenkins/templates/bojenkins.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.415899 botoolkit-1.1.9/botoolkit/bo_jira/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/api.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2022-05-26 12:27:22.000000 botoolkit-1.1.9/botoolkit/bo_jira/commands.py
+-rw-r--r--   0 root         (0) root         (0)      589 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2022-05-24 12:11:37.000000 botoolkit-1.1.9/botoolkit/bo_jira/enums.py
+-rw-r--r--   0 root         (0) root         (0)      172 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      677 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/main.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      487 2022-05-25 12:29:29.000000 botoolkit-1.1.9/botoolkit/bo_jira/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.416899 botoolkit-1.1.9/botoolkit/bo_jira/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_jira/templates/bojira.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.424899 botoolkit-1.1.9/botoolkit/bo_postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/command_validators.py
+-rw-r--r--   0 root         (0) root         (0)    41201 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_postgres/commands.py
+-rw-r--r--   0 root         (0) root         (0)      158 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/consts.py
+-rw-r--r--   0 root         (0) root         (0)     3517 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/entities.py
+-rw-r--r--   0 root         (0) root         (0)      191 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/enums.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/exporters.py
+-rw-r--r--   0 root         (0) root         (0)    10968 2022-06-14 20:15:50.000000 botoolkit-1.1.9/botoolkit/bo_postgres/generators.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      686 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/main.py
+-rw-r--r--   0 root         (0) root         (0)    18966 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      645 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/repositories.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/services.py
+-rw-r--r--   0 root         (0) root         (0)      942 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/settings.py
+-rw-r--r--   0 root         (0) root         (0)      301 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.424899 botoolkit-1.1.9/botoolkit/bo_postgres/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      510 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_postgres/templates/bopostgres.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.427899 botoolkit-1.1.9/botoolkit/bo_registry/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9946 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/commands.py
+-rw-r--r--   0 root         (0) root         (0)     8424 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      686 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/main.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      664 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.428899 botoolkit-1.1.9/botoolkit/bo_registry/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_registry/templates/boregistry.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.430899 botoolkit-1.1.9/botoolkit/bo_telegram/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      680 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/main.py
+-rw-r--r--   0 root         (0) root         (0)      464 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      382 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.431899 botoolkit-1.1.9/botoolkit/bo_telegram/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_telegram/templates/botelegram.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.433899 botoolkit-1.1.9/botoolkit/bo_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24990 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/commands.py
+-rw-r--r--   0 root         (0) root         (0)      124 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/consts.py
+-rw-r--r--   0 root         (0) root         (0)      608 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      721 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/main.py
+-rw-r--r--   0 root         (0) root         (0)     5081 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      528 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/settings.py
+-rw-r--r--   0 root         (0) root         (0)      201 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.434899 botoolkit-1.1.9/botoolkit/bo_toolkit/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2022-07-14 04:59:55.000000 botoolkit-1.1.9/botoolkit/bo_toolkit/templates/botoolkit.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.438899 botoolkit-1.1.9/botoolkit/bo_web_bb/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/api.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/consts.py
+-rw-r--r--   0 root         (0) root         (0)    41979 2022-08-22 08:47:38.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/enums.py
+-rw-r--r--   0 root         (0) root         (0)      175 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      849 2022-06-01 18:43:21.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.439899 botoolkit-1.1.9/botoolkit/bo_web_bb/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.441899 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/
+-rwxr-xr-x   0 root         (0) root         (0)     2038 2022-07-21 15:07:55.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2485 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py
+-rwxr-xr-x   0 root         (0) root         (0)     4306 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      788 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl
+-rw-r--r--   0 root         (0) root         (0)     1477 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.442899 botoolkit-1.1.9/botoolkit/bo_web_bb/images/web_bb_app/
+-rwxr-xr-x   0 root         (0) root         (0)      534 2022-07-21 15:07:55.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/images/web_bb_app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/main.py
+-rw-r--r--   0 root         (0) root         (0)     6161 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2022-07-21 15:07:55.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/services.py
+-rw-r--r--   0 root         (0) root         (0)      972 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/settings.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.442899 botoolkit-1.1.9/botoolkit/bo_web_bb/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/bo_web_bb/templates/bowebbb.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.450899 botoolkit-1.1.9/botoolkit/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26495 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/commands.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-07-21 15:07:55.000000 botoolkit-1.1.9/botoolkit/core/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/enums.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/exporters.py
+-rw-r--r--   0 root         (0) root         (0)     9972 2022-06-01 18:43:21.000000 botoolkit-1.1.9/botoolkit/core/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      364 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2022-07-21 15:07:55.000000 botoolkit-1.1.9/botoolkit/core/services.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/core/strings.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2022-04-27 09:28:05.000000 botoolkit-1.1.9/botoolkit/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.356899 botoolkit-1.1.9/botoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34614 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5737 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     3650 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-27 09:28:14.000000 botoolkit-1.1.9/botoolkit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      248 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-08-22 08:47:47.000000 botoolkit-1.1.9/botoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 08:47:47.451899 botoolkit-1.1.9/docs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-27 09:28:05.000000 botoolkit-1.1.9/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      391 2022-04-27 09:28:05.000000 botoolkit-1.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-22 08:47:47.452899 botoolkit-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1913 2022-08-22 08:47:38.000000 botoolkit-1.1.9/setup.py
```

### Comparing `botoolkit-1.1.8/CHANGES.md` & `botoolkit-1.1.9/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+1.1.9
+
+- Переименован плагин mchs.
+
 1.1.8
 
 - Добавление плагина integration_transcrypt проекта web_bb_accounting.
 
 1.1.7
 
 - Добавлен проброс содержимого pip.conf при сборке образов приложения web_bb.
```

### Comparing `botoolkit-1.1.8/PKG-INFO` & `botoolkit-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoolkit
-Version: 1.1.8
+Version: 1.1.9
 Summary: BO toolkit
 Home-page: 
 Download-URL: 
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -40,15 +40,19 @@
 в едином проекте в качестве консольных утилит для повышения удобства работы с 
 проектом и сокращения издержек выполнение рутинных задач. Более подробно с 
 инструментом можно ознакомиться в [Confluence](https://conf.bars.group/display/BONLINE/BO+Toolkit).
 
 ## Версионирование
 
 В проекте используется Семантическое версионирование. Со спецификацией можно ознакомиться по ссылке 
-https://semver.org/lang/ru/1.1.8
+https://semver.org/lang/ru/1.1.9
+
+- Переименован плагин mchs.
+
+1.1.8
 
 - Добавление плагина integration_transcrypt проекта web_bb_accounting.
 
 1.1.7
 
 - Добавлен проброс содержимого pip.conf при сборке образов приложения web_bb.
```

### Comparing `botoolkit-1.1.8/README.md` & `botoolkit-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_barsdock/commands.py` & `botoolkit-1.1.9/botoolkit/bo_barsdock/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_barsdock/main.py` & `botoolkit-1.1.9/botoolkit/bo_barsdock/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_barsdock/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_barsdock/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/api.py` & `botoolkit-1.1.9/botoolkit/bo_conf/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/commands.py` & `botoolkit-1.1.9/botoolkit/bo_conf/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/enums.py` & `botoolkit-1.1.9/botoolkit/bo_conf/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_conf/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/main.py` & `botoolkit-1.1.9/botoolkit/bo_conf/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_conf/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_conf/settings.py` & `botoolkit-1.1.9/botoolkit/bo_conf/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/commands.py` & `botoolkit-1.1.9/botoolkit/bo_databaser/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/main.py` & `botoolkit-1.1.9/botoolkit/bo_databaser/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_databaser/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/services.py` & `botoolkit-1.1.9/botoolkit/bo_databaser/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/settings.py` & `botoolkit-1.1.9/botoolkit/bo_databaser/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/templates/bodatabaser.conf` & `botoolkit-1.1.9/botoolkit/bo_databaser/templates/bodatabaser.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_databaser/templates/bodatabaser_build.conf` & `botoolkit-1.1.9/botoolkit/bo_databaser/templates/bodatabaser_build.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/commands.py` & `botoolkit-1.1.9/botoolkit/bo_git/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/enums.py` & `botoolkit-1.1.9/botoolkit/bo_git/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_git/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/main.py` & `botoolkit-1.1.9/botoolkit/bo_git/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_git/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_git/settings.py` & `botoolkit-1.1.9/botoolkit/bo_git/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_guide/commands.py` & `botoolkit-1.1.9/botoolkit/bo_guide/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_guide/main.py` & `botoolkit-1.1.9/botoolkit/bo_guide/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_guide/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_guide/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_ip/api.py` & `botoolkit-1.1.9/botoolkit/bo_ip/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_ip/commands.py` & `botoolkit-1.1.9/botoolkit/bo_ip/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_ip/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_ip/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_ip/main.py` & `botoolkit-1.1.9/botoolkit/bo_ip/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/commands.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/generators.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/generators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/main.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/parsers.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/parsers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/settings.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jenkins/strings.py` & `botoolkit-1.1.9/botoolkit/bo_jenkins/strings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/api.py` & `botoolkit-1.1.9/botoolkit/bo_jira/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/commands.py` & `botoolkit-1.1.9/botoolkit/bo_jira/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/consts.py` & `botoolkit-1.1.9/botoolkit/bo_jira/consts.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/enums.py` & `botoolkit-1.1.9/botoolkit/bo_jira/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/main.py` & `botoolkit-1.1.9/botoolkit/bo_jira/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_jira/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_jira/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/command_validators.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/command_validators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/commands.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/entities.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/entities.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/exporters.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/exporters.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/generators.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/generators.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/main.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/repositories.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/repositories.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/services.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_postgres/settings.py` & `botoolkit-1.1.9/botoolkit/bo_postgres/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_registry/commands.py` & `botoolkit-1.1.9/botoolkit/bo_registry/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_registry/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_registry/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_registry/main.py` & `botoolkit-1.1.9/botoolkit/bo_registry/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_registry/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_registry/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_registry/settings.py` & `botoolkit-1.1.9/botoolkit/bo_registry/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_telegram/commands.py` & `botoolkit-1.1.9/botoolkit/bo_telegram/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_telegram/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_telegram/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_telegram/main.py` & `botoolkit-1.1.9/botoolkit/bo_telegram/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/commands.py` & `botoolkit-1.1.9/botoolkit/bo_toolkit/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_toolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/main.py` & `botoolkit-1.1.9/botoolkit/bo_toolkit/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_toolkit/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/settings.py` & `botoolkit-1.1.9/botoolkit/bo_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_toolkit/templates/botoolkit.conf` & `botoolkit-1.1.9/botoolkit/bo_toolkit/templates/botoolkit.conf`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/api.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/api.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/commands.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/consts.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/consts.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/enums.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     JOURNAL_HOZ_OPER_CHELYAB = 'journal_hoz_oper_chelyab'
     KAZAN_REPORTS = 'kazan_reports'
     KPP_PP = 'kpp_pp'
     KV_CHELYAB = 'kv_chelyab'
     LOAD_LIMITS = 'load_limits'
     LOAD_PLAN = 'load_plan'
     MAGIC_ANALYTIC = 'magic_analytic'
-    MCHS = 'mchs'
+    ACCOUNTING_MCHS = 'accounting_mchs'
     NOMER_DOGOVORA = 'nomer_dogovora'
     NOVOSIB_SERVICE_PF_ACT = 'novosib_service_pf_act'
     OPERATIONS_JOURNAL_04_ACCOUNTS_ANALYTICS = 'operations_journal_04_accounts_analytics'
     OSS = 'oss'
     PAYMENT_SCHEDULE = 'payment_schedule'
     PREDMET_DOGOVORA_0503769A = 'predmet_dogovora_0503769a'
     PROPERTY_INTEGRATION = 'property_integration'
@@ -455,15 +455,15 @@
                     cls.JOURNAL_HOZ_OPER_CHELYAB,
                     cls.KAZAN_REPORTS,
                     cls.KPP_PP,
                     cls.KV_CHELYAB,
                     cls.LOAD_LIMITS,
                     cls.LOAD_PLAN,
                     cls.MAGIC_ANALYTIC,
-                    cls.MCHS,
+                    cls.ACCOUNTING_MCHS,
                     cls.NOMER_DOGOVORA,
                     cls.NOVOSIB_SERVICE_PF_ACT,
                     cls.OSS,
                     cls.PAYMENT_SCHEDULE,
                     cls.PROPERTY_INTEGRATION,
                     cls.REESTR_IZVESHCHENIY,
                     cls.REESTR_IZVESHCHENIY_EIS,
@@ -623,15 +623,15 @@
             ),
             cls.LOAD_PLAN: (
                 cls.ACCOUNTING,
             ),
             cls.MAGIC_ANALYTIC: (
                 cls.ACCOUNTING,
             ),
-            cls.MCHS: (
+            cls.ACCOUNTING_MCHS: (
                 cls.ACCOUNTING,
             ),
             cls.NOMER_DOGOVORA: (
                 cls.ACCOUNTING,
             ),
             cls.NOVOSIB_SERVICE_PF_ACT: (
                 cls.ACCOUNTING,
```

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/helpers.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/Dockerfile`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/add_generic_tables.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/app.conf.tmpl`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/app_requirements_ssh.txt.tmpl`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/base_web_bb_app/create_default_date_range_partition.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile` & `botoolkit-1.1.9/botoolkit/bo_web_bb/images/web_bb_app/Dockerfile`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/main.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/main.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/mixins.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/services.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/bo_web_bb/settings.py` & `botoolkit-1.1.9/botoolkit/bo_web_bb/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/commands.py` & `botoolkit-1.1.9/botoolkit/core/commands.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/enums.py` & `botoolkit-1.1.9/botoolkit/core/enums.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/exporters.py` & `botoolkit-1.1.9/botoolkit/core/exporters.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/helpers.py` & `botoolkit-1.1.9/botoolkit/core/helpers.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/mixins.py` & `botoolkit-1.1.9/botoolkit/core/mixins.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/services.py` & `botoolkit-1.1.9/botoolkit/core/services.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/core/strings.py` & `botoolkit-1.1.9/botoolkit/core/strings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit/settings.py` & `botoolkit-1.1.9/botoolkit/settings.py`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit.egg-info/PKG-INFO` & `botoolkit-1.1.9/botoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botoolkit
-Version: 1.1.8
+Version: 1.1.9
 Summary: BO toolkit
 Home-page: 
 Download-URL: 
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -40,15 +40,19 @@
 в едином проекте в качестве консольных утилит для повышения удобства работы с 
 проектом и сокращения издержек выполнение рутинных задач. Более подробно с 
 инструментом можно ознакомиться в [Confluence](https://conf.bars.group/display/BONLINE/BO+Toolkit).
 
 ## Версионирование
 
 В проекте используется Семантическое версионирование. Со спецификацией можно ознакомиться по ссылке 
-https://semver.org/lang/ru/1.1.8
+https://semver.org/lang/ru/1.1.9
+
+- Переименован плагин mchs.
+
+1.1.8
 
 - Добавление плагина integration_transcrypt проекта web_bb_accounting.
 
 1.1.7
 
 - Добавлен проброс содержимого pip.conf при сборке образов приложения web_bb.
```

### Comparing `botoolkit-1.1.8/botoolkit.egg-info/SOURCES.txt` & `botoolkit-1.1.9/botoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/botoolkit.egg-info/entry_points.txt` & `botoolkit-1.1.9/botoolkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `botoolkit-1.1.8/setup.py` & `botoolkit-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from botoolkit.settings import (
     ENTRY_POINTS,
 )
 
 
 PROJECT = 'botoolkit'
 
-VERSION = '1.1.8'
+VERSION = '1.1.9'
 
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

