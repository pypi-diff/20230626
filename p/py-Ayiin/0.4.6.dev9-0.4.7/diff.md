# Comparing `tmp/py-Ayiin-0.4.6.dev9.tar.gz` & `tmp/py-Ayiin-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.6.dev9.tar", last modified: Sun Jun 25 11:22:19 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.7.tar", last modified: Mon Jun 26 15:54:23 2023, max compression
```

## Comparing `py-Ayiin-0.4.6.dev9.tar` & `py-Ayiin-0.4.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.542158 py-Ayiin-0.4.6.dev9/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.542158 py-Ayiin-0.4.6.dev9/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.542158 py-Ayiin-0.4.6.dev9/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.542158 py-Ayiin-0.4.6.dev9/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.542158 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-25 11:22:19.000000 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-25 11:22:19.000000 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:22:19.000000 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 11:22:19.000000 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 11:22:19.000000 py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:22:19.546158 py-Ayiin-0.4.6.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-25 11:22:10.000000 py-Ayiin-0.4.6.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.871067 py-Ayiin-0.4.7/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.871067 py-Ayiin-0.4.7/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38781 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.871067 py-Ayiin-0.4.7/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33973 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.875069 py-Ayiin-0.4.7/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.875069 py-Ayiin-0.4.7/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 15:54:23.000000 py-Ayiin-0.4.7/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-26 15:54:23.000000 py-Ayiin-0.4.7/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:54:23.000000 py-Ayiin-0.4.7/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:54:23.000000 py-Ayiin-0.4.7/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 15:54:23.000000 py-Ayiin-0.4.7/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:54:23.879072 py-Ayiin-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-26 15:54:14.000000 py-Ayiin-0.4.7/setup.py
```

### Comparing `py-Ayiin-0.4.6.dev9/LICENSE` & `py-Ayiin-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/NOTICE` & `py-Ayiin-0.4.7/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/PKG-INFO` & `py-Ayiin-0.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev9
+Version: 0.4.7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev9/README.md` & `py-Ayiin-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.7/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.7/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.7/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.7/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/__init__.py` & `py-Ayiin-0.4.7/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.6.dev09"
+__version__ = "0.4.7"
 ayiin_ver = "0.1.1"
 prem_version = "0.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
```

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/__main__.py` & `py-Ayiin-0.4.7/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/assistant.py` & `py-Ayiin-0.4.7/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/config.py` & `py-Ayiin-0.4.7/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.7/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.7/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.7/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.7/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.7/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.7/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.7/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.7/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.7/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.7/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.7/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.7/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/start.py` & `py-Ayiin-0.4.7/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.7/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.7/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.7/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.7/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/decorator.py` & `py-Ayiin-0.4.7/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/exceptions.py` & `py-Ayiin-0.4.7/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.7/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.7/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.7/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.7/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.7/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/func.py` & `py-Ayiin-0.4.7/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.7/pyAyiin/methods/funcb.py`

 * *Files 4% similar despite different names*

```diff
@@ -300,16 +300,35 @@
                     else:
                         pass
                 except FloodWait as e:
                     await asyncio.sleep(e.value)
                 except BaseException:
                     pass
     
-    async def tiktoker(cmd):
+    async def tiktok_downloader(self, cmd):
         url = "https://tiktok-downloader-download-tiktok-videos-without-watermark.p.rapidapi.com/vid/index"
         querystring = {"url":cmd}
         headers = {
         "X-RapidAPI-Key": "3c7ace35d5mshd5223e5fc185146p1e2d15jsn3f9f0a73128c",
         "X-RapidAPI-Host": "tiktok-downloader-download-tiktok-videos-without-watermark.p.rapidapi.com/vid/index"
         }
         response = requests.get(url, headers=headers, params=querystring).json()["video"][0]
         return response
+
+    async def ask_ai(self, cmd):
+        url = "https://chatgpt53.p.rapidapi.com/"
+        payload = {
+        "messages": [
+            {
+            "role": "user",
+            "content": cmd
+            }
+        ],
+        "temperature": 1
+        }
+        headers = {
+        "content-type": "application/json",
+        "X-RapidAPI-Key": "3c7ace35d5mshd5223e5fc185146p1e2d15jsn3f9f0a73128c",
+        "X-RapidAPI-Host": "chatgpt53.p.rapidapi.com"
+        }
+        response = requests.post(url, json=payload, headers=headers).json()['choices'][0]['message']['content']
+        return response
```

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.7/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.7/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.7/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.7/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.7/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,20 +353,21 @@
 
         return message
 
 
     async def create_quotly(
         self,
         message,
-        url="https://qoute-api-akashpattnaik.koyeb.app/generate",
+        url="https://bot.lyo.su/quote/generate",
         reply={},
         bg=None,
         sender=None,
         file_name="quote.webp",
     ):
+        #"https://qoute-api-akashpattnaik.koyeb.app/generate",
         if not isinstance(message, list):
             message = [message]
             url = self.o_api
         if not bg:
             bg = "#1b1429"
         content = {
             "type": "quote",
```

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.7/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.7/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.7/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.7/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.7/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.7/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.7/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.7/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.7/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.7/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.7/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/pyAyiin/xd.py` & `py-Ayiin-0.4.7/pyAyiin/xd.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,28 +77,29 @@
     async def generate_premium(
         self,
         bots: ClientFipper,
         chat_id: int,
         device_model: str,
         msg: Message,
     ):
-        await msg.reply("<b>Memulai Membuat String Session...</b>")
-        api_id_msg = await msg.ask("<b>Silakan kirim API_ID</b>", filters=filters.text)
+        await msg.reply("<b>Memulai Membuat Ubot Premium...</b>")
+        from_id = msg.chat.id
+        api_id_msg = await bots.ask(from_id, "<b>Silakan kirim API_ID</b>", filters=filters.text)
         if await self.cancelled(api_id_msg):
             return
         try:
             api_id = int(api_id_msg.text)
         except ValueError:
             await api_id_msg.reply("<b>Maaf API_ID Yang Anda Masukan Salah. Silakan mulai ulang untuk membuat Ubot.</b>", quote=True)
             return
-        api_hash_msg = await msg.ask("<b>Silakan kirim API_HASH</b>", filters=filters.text)
+        api_hash_msg = await bots.ask(from_id, "<b>Silakan kirim API_HASH</b>", filters=filters.text)
         if await self.cancelled(api_id_msg):
             return
         api_hash = api_hash_msg.text
-        phone_number_msg = await msg.ask("<b>Silahkan Masukkan Nomor Telepon Telegram Anda Dengan Format kode negara.</b> \n<b>Contoh :</b> <code>+62xxxxxxxxx</code>", filters=filters.text)
+        phone_number_msg = await bots.ask(from_id, "<b>Silahkan Masukkan Nomor Telepon Telegram Anda Dengan Format kode negara.</b> \n<b>Contoh :</b> <code>+62xxxxxxxxx</code>", filters=filters.text)
         if await self.cancelled(api_id_msg):
             return
         phone_number = phone_number_msg.text
         await msg.reply("<b>Mengirim Kode OTP...</b>")
         client = ClientFipper(
             name="user",
             api_id=api_id,
@@ -111,15 +112,15 @@
         except ApiIdInvalidFipper:
             await msg.reply("<b>Kombinasi API_ID dan API_HASH Yang Anda Masukkan Salah. Silakan mulai ulang untuk membuat Ubot.</b>")
             return
         except PhoneNumberInvalidFipper:
             await msg.reply("<b>Nomor Telepon Telegram Yang Anda Masukkan Salah. Silakan mulai ulang untuk membuat Ubot.</b>")
             return
         try:
-            phone_code_msg = await msg.ask("<b>Silahkan Periksa Kode OTP dari akun Telegram Resmi. Jika Anda mendapatkannya, kirim OTP di sini setelah membaca format di bawah ini.</b> \n\n<b>Jika OTP adalah</b> <code>12345</code>, <b>Tolong [Tambahkan Spasi] kirimkan Seperti Ini</b> <code>1 2 3 4 5</code>.", filters=filters.text, timeout=600)
+            phone_code_msg = await bots.ask(from_id, "<b>Silahkan Periksa Kode OTP dari akun Telegram Resmi. Jika Anda mendapatkannya, kirim OTP di sini setelah membaca format di bawah ini.</b> \n\n<b>Jika OTP adalah</b> <code>12345</code>, <b>Tolong [Tambahkan Spasi] kirimkan Seperti Ini</b> <code>1 2 3 4 5</code>.", filters=filters.text, timeout=600)
             if await self.cancelled(api_id_msg):
                 return
         except TimeoutError:
             await msg.reply("<b>Batas waktu tercapai 10 menit. Silakan mulai ulang untuk membuat Ubot.</b>")
             return
         phone_code = phone_code_msg.text.replace(" ", "")
         try:
@@ -128,15 +129,15 @@
             await msg.reply("<b>Kode OTP Yang Anda Masukkan Salah. Silakan mulai ulang untuk membuat Ubot.</b>")
             return
         except PhoneCodeExpiredFipper:
             await msg.reply("<b>Kode OTP sudah kadaluarsa. Silakan mulai ulang untuk membuat Ubot.</b>")
             return
         except SessionPasswordNeededFipper:
             try:
-                two_step_msg = await msg.ask("<b>Akun Anda telah mengaktifkan verifikasi dua langkah. Mohon Masukkan kata sandinya.</b>", filters=filters.text, timeout=300)
+                two_step_msg = await bots.ask(from_id, "<b>Akun Anda telah mengaktifkan verifikasi dua langkah. Mohon Masukkan kata sandinya.</b>", filters=filters.text, timeout=300)
             except TimeoutError:
                 await msg.reply("<b>Batas waktu tercapai 5 menit. Silakan mulai ulang untuk membuat Ubot.</b>")
                 return
             try:
                 password = two_step_msg.text
                 await client.check_password(password=password)
                 if await self.cancelled(api_id_msg):
@@ -170,27 +171,28 @@
         if telethon:
             ty = "Telethon"
         else:
             ty = "Pyrogram"
             if not old_pyro:
                 ty += " v2"
         await msg.reply(f"**Memulai {ty} String Session...**")
-        api_id_msg = await msg.ask("**Silakan kirim API_ID Anda**", filters=filters.text)
+        from_id = msg.chat.id
+        api_id_msg = await bot.ask(from_id, "**Silakan kirim API_ID Anda**", filters=filters.text)
         if await self.cancelled(api_id_msg):
             return
         try:
             api_id = int(api_id_msg.text)
         except ValueError:
             await api_id_msg.reply("**Maaf API_ID Yang Anda Masukan Salah. Silakan mulai membuat sesi lagi.**", quote=True)
             return
-        api_hash_msg = await msg.ask("**Silakan kirim API_HASH Anda**", filters=filters.text)
+        api_hash_msg = await bot.ask(from_id, "**Silakan kirim API_HASH Anda**", filters=filters.text)
         if await self.cancelled(api_hash_msg):
             return
         api_hash = api_hash_msg.text
-        phone_number_msg = await msg.ask("**Silahkan Masukkan Nomor Telepon Telegram Anda Dengan Format kode negara.** \n**Contoh :** `+62xxxxxxxxx`", filters=filters.text)
+        phone_number_msg = await bot.ask(from_id, "**Silahkan Masukkan Nomor Telepon Telegram Anda Dengan Format kode negara.** \n**Contoh :** `+62xxxxxxxxx`", filters=filters.text)
         if await self.cancelled(phone_number_msg):
             return
         phone_number = phone_number_msg.text
         await msg.reply("**Mengirim Kode OTP...**")
         if telethon:
             client = TelegramClient(StringSession(), api_id, api_hash)
         elif old_pyro:
@@ -208,15 +210,15 @@
             await msg.reply("**Kombinasi API_ID dan API_HASH Yang Anda Masukkan Salah. Silakan mulai membuat sesi lagi.**")
             return
         except (PhoneNumberInvalid, PhoneNumberInvalidFipper, PhoneNumberInvalidError):
             await msg.reply("**Nomor Telepon Telegram Yang Anda Masukkan Salah. Silakan mulai membuat sesi lagi.**")
             return
         try:
             phone_code_msg = None
-            phone_code_msg = await msg.ask("**Silahkan Periksa Kode OTP dari akun Telegram Resmi. Jika Anda mendapatkannya, kirim OTP di sini setelah membaca format di bawah ini.** \n\n**Jika OTP adalah** `12345`, **Tolong [Tambahkan Spasi] kirimkan Seperti Ini** `1 2 3 4 5`.", filters=filters.text, timeout=600)
+            phone_code_msg = await bot.ask(from_id, "**Silahkan Periksa Kode OTP dari akun Telegram Resmi. Jika Anda mendapatkannya, kirim OTP di sini setelah membaca format di bawah ini.** \n\n**Jika OTP adalah** `12345`, **Tolong [Tambahkan Spasi] kirimkan Seperti Ini** `1 2 3 4 5`.", filters=filters.text, timeout=600)
             if await self.cancelled(phone_code_msg):
                 return
         except TimeoutError:
             await msg.reply("**Batas waktu tercapai 10 menit. Silakan mulai membuat sesi lagi.**")
             return
         phone_code = phone_code_msg.text.replace(" ", "")
         try:
@@ -228,15 +230,15 @@
             await msg.reply("**Kode OTP Yang Anda Masukkan Salah. Silakan mulai membuat sesi lagi.**")
             return
         except (PhoneCodeExpired, PhoneCodeExpiredFipper, PhoneCodeExpiredError):
             await msg.reply("**Kode OTP sudah kadaluarsa. Silakan mulai membuat sesi lagi.**")
             return
         except (SessionPasswordNeeded, SessionPasswordNeededFipper, SessionPasswordNeededError):
             try:
-                two_step_msg = await msg.ask("**Akun Anda telah mengaktifkan verifikasi dua langkah. Mohon Masukkan kata sandinya.**", filters=filters.text, timeout=300)
+                two_step_msg = await bot.ask(from_id, "**Akun Anda telah mengaktifkan verifikasi dua langkah. Mohon Masukkan kata sandinya.**", filters=filters.text, timeout=300)
             except TimeoutError:
                 await msg.reply("**Batas waktu tercapai 5 menit. Silakan mulai membuat sesi lagi.**")
                 return
             try:
                 password = two_step_msg.text
                 if telethon:
                     await client.sign_in(password=password)
```

### Comparing `py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.7/py_Ayiin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.6.dev9
+Version: 0.4.7
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.6.dev9/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.7/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.6.dev9/setup.py` & `py-Ayiin-0.4.7/setup.py`

 * *Files identical despite different names*

