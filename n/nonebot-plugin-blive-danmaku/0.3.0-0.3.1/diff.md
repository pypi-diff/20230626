# Comparing `tmp/nonebot_plugin_blive_danmaku-0.3.0.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.3.0.tar` & `nonebot_plugin_blive_danmaku-0.3.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.0/LICENSE
--rw-r--r--   0        0        0      938 2023-06-12 10:18:14.127750 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/__init__.py
--rw-r--r--   0        0        0       91 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
--rw-r--r--   0        0        0   533008 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
--rw-r--r--   0        0        0   285956 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
--rw-r--r--   0        0        0   324265 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
--rw-r--r--   0        0        0     9045 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
--rw-r--r--   0        0        0     8799 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
--rw-r--r--   0        0        0     7006 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
--rw-r--r--   0        0        0      902 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
--rw-r--r--   0        0        0    20588 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3c05b20d.js
--rw-r--r--   0        0        0     9107 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
--rw-r--r--   0        0        0      703 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
--rw-r--r--   0        0        0     3061 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
--rw-r--r--   0        0        0     1239 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6d61e593.js
--rw-r--r--   0        0        0      815 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
--rw-r--r--   0        0        0       51 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-80d7cd47.css
--rw-r--r--   0        0        0     6720 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c6f2a8b7.js
--rw-r--r--   0        0        0      167 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
--rw-r--r--   0        0        0     2787 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-d45d9135.js
--rw-r--r--   0        0        0     5128 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e52ee405.js
--rw-r--r--   0        0        0      699 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
--rw-r--r--   0        0        0     3593 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f4938b6b.js
--rw-r--r--   0        0        0    20126 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
--rw-r--r--   0        0        0     6259 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
--rw-r--r--   0        0        0     5886 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
--rw-r--r--   0        0        0    20334 2023-06-24 08:03:50.593056 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
--rw-r--r--   0        0        0    18870 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-3e9cf0c0.js
--rw-r--r--   0        0        0      330 2023-06-24 08:03:50.596062 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
--rw-r--r--   0        0        0     1757 2023-06-24 08:03:50.595050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
--rw-r--r--   0        0        0   447924 2023-06-24 08:03:50.601050 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
--rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
--rw-r--r--   0        0        0      908 2023-06-24 08:03:50.600052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/index.html
--rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/models.py
--rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/router.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     7552 2023-06-22 11:19:57.567827 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/listener/__init__.py
--rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/listener/kick.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     9062 2023-06-24 06:03:40.544803 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     9900 2023-06-24 03:26:16.486292 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     2750 2023-06-24 02:54:45.822615 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0     1004 2023-06-24 08:53:10.200255 nonebot_plugin_blive_danmaku-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5599 2023-06-24 09:07:18.310064 nonebot_plugin_blive_danmaku-0.3.0/README.md
--rw-r--r--   0        0        0     6617 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.1/LICENSE
+-rw-r--r--   0        0        0      938 2023-06-12 10:18:14.127750 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
+-rw-r--r--   0        0        0   533008 2023-06-26 02:58:12.791659 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
+-rw-r--r--   0        0        0   285956 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
+-rw-r--r--   0        0        0   324265 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
+-rw-r--r--   0        0        0     9045 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
+-rw-r--r--   0        0        0     8799 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
+-rw-r--r--   0        0        0     7006 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
+-rw-r--r--   0        0        0      902 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
+-rw-r--r--   0        0        0     6723 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js
+-rw-r--r--   0        0        0     2787 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js
+-rw-r--r--   0        0        0    20588 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js
+-rw-r--r--   0        0        0     9107 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
+-rw-r--r--   0        0        0      703 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
+-rw-r--r--   0        0        0     3061 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
+-rw-r--r--   0        0        0      815 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
+-rw-r--r--   0        0        0     5128 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js
+-rw-r--r--   0        0        0      167 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
+-rw-r--r--   0        0        0      699 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
+-rw-r--r--   0        0        0     3593 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js
+-rw-r--r--   0        0        0     1239 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js
+-rw-r--r--   0        0        0       51 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-fe1a4f18.css
+-rw-r--r--   0        0        0    20126 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
+-rw-r--r--   0        0        0     6259 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
+-rw-r--r--   0        0        0     5886 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
+-rw-r--r--   0        0        0    20334 2023-06-26 02:58:12.784659 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
+-rw-r--r--   0        0        0      330 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
+-rw-r--r--   0        0        0    18870 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js
+-rw-r--r--   0        0        0     1757 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
+-rw-r--r--   0        0        0   447924 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
+-rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
+-rw-r--r--   0        0        0      908 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/index.html
+-rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/models.py
+-rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/router.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     7552 2023-06-22 11:19:57.567827 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/listener/__init__.py
+-rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/listener/kick.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     9062 2023-06-24 06:03:40.544803 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     9900 2023-06-24 03:26:16.486292 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     2750 2023-06-24 02:54:45.822615 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0     1004 2023-06-26 02:58:40.550626 nonebot_plugin_blive_danmaku-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5599 2023-06-24 09:07:18.310064 nonebot_plugin_blive_danmaku-0.3.1/README.md
+-rw-r--r--   0        0        0     6617 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3c05b20d.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -731,23 +731,23 @@
         }
     }),
     se = x({
         history: k(),
         routes: [{
             name: "home",
             path: "/",
-            component: () => M((() => import("./index-6d61e593.js")), ["assets/index-6d61e593.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-cd2e8127.css"])
+            component: () => M((() => import("./index-f9e2a7e5.js")), ["assets/index-f9e2a7e5.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-cd2e8127.css"])
         }, {
             name: "history",
             path: "/history",
-            component: () => M((() => import("./index-e52ee405.js")), ["assets/index-e52ee405.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-54bfb553.css"])
+            component: () => M((() => import("./index-c1b5ef2f.js")), ["assets/index-c1b5ef2f.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-54bfb553.css"])
         }, {
             name: "room",
             path: "/room",
-            component: () => M((() => import("./index-f4938b6b.js")), ["assets/index-f4938b6b.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-e7323967.css"])
+            component: () => M((() => import("./index-f24fc95e.js")), ["assets/index-f24fc95e.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-e7323967.css"])
         }, {
             name: "change",
             path: "/change",
             component: () => M((() => import("./index-6803b0c6.js")), ["assets/index-6803b0c6.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css"])
         }]
     }),
     ne = T(),
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6d61e593.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     p as e,
     n as s
 } from "./elementPlus-2bbb65c2.js";
 import {
     G as a,
     C as t
-} from "./index-3c05b20d.js";
+} from "./index-3b039937.js";
 import {
     E as r,
     r as o,
     b as l,
     v as n,
     j as i,
     P as m,
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c6f2a8b7.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 } from "./elementPlus-2bbb65c2.js";
 import {
     _ as y,
     g as N,
     f as b,
     F as w,
     R as V
-} from "./index-3c05b20d.js";
+} from "./index-3b039937.js";
 import {
     aF as M,
     aO as k,
     E as C,
     aH as L,
     r as R,
     h as x,
@@ -70,15 +70,15 @@
     }
 }, J = C({
     __name: "sc",
     setup(v, {
         expose: c
     }) {
         const p = L({
-                loader: () => y((() => import("./SuperChat-3e9cf0c0.js")), ["assets/SuperChat-3e9cf0c0.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/elementPlus-2bbb65c2.js", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3c05b20d.js", "assets/index-4d7b4401.css", "assets/SuperChat-8f8a299b.css"])
+                loader: () => y((() => import("./SuperChat-fcb4d4cd.js")), ["assets/SuperChat-fcb4d4cd.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/elementPlus-2bbb65c2.js", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3b039937.js", "assets/index-4d7b4401.css", "assets/SuperChat-8f8a299b.css"])
             }),
             f = R({
                 width: 269,
                 battery: 300,
                 userName: "",
                 userRole: "0",
                 scContent: "",
@@ -237,15 +237,15 @@
                 }, 8, ["model"])])),
                 _: 1
             }, 8, ["modelValue"])
         }
     }
 }), K = {
     class: "demo-input-suffix"
-}, X = (e => (Q("data-v-a3b26e46"), e = e(), G(), e))((() => j("span", {
+}, X = (e => (Q("data-v-0ec0a539"), e = e(), G(), e))((() => j("span", {
     class: "ml-3 text-gray-600 inline-flex items-center"
 }, "路灯：", -1))), Y = {
     key: 0,
     class: "ml-2"
 }, Z = ["innerHTML"], ee = {
     key: 1,
     class: "ml-2"
@@ -350,15 +350,15 @@
                         placement: "top",
                         content: "点击生成SC图片"
                     }, {
                         default: S((() => [T(i, {
                             onClick: a => (e => {
                                 const a = {
                                     width: 269,
-                                    battery: Number(e.price),
+                                    battery: Number(10 * e.price),
                                     userName: e.uname,
                                     userRole: e.guard.toString(),
                                     scContent: e.message,
                                     showTrans: !1,
                                     transContent: "",
                                     showFansMedal: !1,
                                     medalName: "",
@@ -393,13 +393,13 @@
             }), T(J, {
                 ref_key: "hd",
                 ref: l
             }, null, 512)], 64)
         }
     }
 }), [
-    ["__scopeId", "data-v-a3b26e46"]
+    ["__scopeId", "data-v-0ec0a539"]
 ]);
 export {
     le as
     default
 };
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-d45d9135.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     T as n
 } from "./elementPlus-2bbb65c2.js";
 import {
     g as o,
     h as r,
     R as u,
     F as d
-} from "./index-3c05b20d.js";
+} from "./index-3b039937.js";
 import {
     L as m,
     u as i,
     i as c,
     a as p,
     b as v,
     c as _,
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e52ee405.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
 import {
     u as X,
     g as G,
     d as N,
     b as W,
     e as q,
     c as A
-} from "./index-3c05b20d.js";
+} from "./index-3b039937.js";
 import {
     _ as B
 } from "./_plugin-vue_export-helper-1b428a4d.js";
 import "./lodash-520df23f.js";
 const F = e => (P("data-v-72e0a09b"), e = e(), S(), e),
     H = {
         class: "danmaku-room-list"
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f4938b6b.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     u as e,
     g as a,
     a as t,
     b as s,
     c as l,
     _ as r
-} from "./index-3c05b20d.js";
+} from "./index-3b039937.js";
 import {
     a as i,
     q as o,
     b as n,
     g as d,
     v as u,
     r as c,
@@ -87,18 +87,18 @@
     K = A(y({
         __name: "index",
         setup(y) {
             const A = h({}),
                 K = h(!0),
                 C = h("120px"),
                 F = U({
-                    loader: () => r((() => import("./index-c6f2a8b7.js")), ["assets/index-c6f2a8b7.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3c05b20d.js", "assets/index-4d7b4401.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-80d7cd47.css"])
+                    loader: () => r((() => import("./index-10fe5420.js")), ["assets/index-10fe5420.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3b039937.js", "assets/index-4d7b4401.css", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-fe1a4f18.css"])
                 }),
                 J = U({
-                    loader: () => r((() => import("./index-d45d9135.js")), ["assets/index-d45d9135.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3c05b20d.js", "assets/index-4d7b4401.css", "assets/echarts-400b5edd.js", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-7bb2b86c.css"])
+                    loader: () => r((() => import("./index-1f52d48f.js")), ["assets/index-1f52d48f.js", "assets/elementPlus-2bbb65c2.js", "assets/vendor-fa374c7f.js", "assets/vendor-b57f6aba.css", "assets/lodash-520df23f.js", "assets/elementPlus-5cfbb218.css", "assets/index-3b039937.js", "assets/index-4d7b4401.css", "assets/echarts-400b5edd.js", "assets/_plugin-vue_export-helper-1b428a4d.js", "assets/index-7bb2b86c.css"])
                 }),
                 M = e(),
                 N = x(),
                 Q = () => {
                     const e = M.getType,
                         a = M.getTypeId,
                         t = M.getUid;
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-3e9cf0c0.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,21 +9,21 @@
     a0 as r,
     a1 as n,
     u as p,
     W as A,
     aP as i,
     P as x
 } from "./vendor-fa374c7f.js";
-import "./index-c6f2a8b7.js";
+import "./index-10fe5420.js";
 import {
     _ as b
 } from "./_plugin-vue_export-helper-1b428a4d.js";
 import "./elementPlus-2bbb65c2.js";
 import "./lodash-520df23f.js";
-import "./index-3c05b20d.js";
+import "./index-3b039937.js";
 const m = [
         [e => e >= 1 && e < 5, () => ({
             start: "#5c968e",
             end: "#5c968e"
         })],
         [e => e >= 5 && e < 9, () => ({
             start: "#5d7b9e",
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/frontend/index.html` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/frontend/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="zh-cn">
   <head>
     <meta charset="UTF-8" />
     <link rel="icon" type="image/x-icon" href="/danmaku/icon/favicon.ico" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>nonebot-plugin-blive-danmaku</title>
-    <script type="module" crossorigin src="/danmaku/assets/index-3c05b20d.js"></script>
+    <script type="module" crossorigin src="/danmaku/assets/index-3b039937.js"></script>
     <link rel="modulepreload" crossorigin href="/danmaku/assets/vendor-fa374c7f.js">
     <link rel="modulepreload" crossorigin href="/danmaku/assets/lodash-520df23f.js">
     <link rel="modulepreload" crossorigin href="/danmaku/assets/elementPlus-2bbb65c2.js">
     <link rel="stylesheet" href="/danmaku/assets/vendor-b57f6aba.css">
     <link rel="stylesheet" href="/danmaku/assets/elementPlus-5cfbb218.css">
     <link rel="stylesheet" href="/danmaku/assets/index-4d7b4401.css">
   </head>
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/app/router.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/app/router.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/listener/kick.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/listener/kick.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/sub/sub_open.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/sub/sub_open.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.1/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.3.0"
+version = "0.3.1"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/README.md` & `nonebot_plugin_blive_danmaku-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.0/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.3.0
+Version: 0.3.1
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.0
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.1
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

