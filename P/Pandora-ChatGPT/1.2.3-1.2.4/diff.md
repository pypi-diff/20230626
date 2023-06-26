# Comparing `tmp/Pandora-ChatGPT-1.2.3.tar.gz` & `tmp/Pandora-ChatGPT-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-mu92xz5p/Pandora-ChatGPT-1.2.3.tar", last modified: Thu Jun 15 09:20:31 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-qtp03pcq/Pandora-ChatGPT-1.2.4.tar", last modified: Mon Jun 26 02:59:05 2023, max compression
```

## Comparing `Pandora-ChatGPT-1.2.3.tar` & `Pandora-ChatGPT-1.2.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:20:31.000000 Pandora-ChatGPT-1.2.3/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-15 09:20:17.000000 Pandora-ChatGPT-1.2.3/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:59:05.000000 Pandora-ChatGPT-1.2.4/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-26 02:58:51.000000 Pandora-ChatGPT-1.2.4/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-1.2.3/LICENSE` & `Pandora-ChatGPT-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/PKG-INFO` & `Pandora-ChatGPT-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.2.3
+Version: 1.2.4
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -51,15 +51,15 @@
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
 * 最新拿 `Access Token` 的技术原理，我记录在[这里](https://zhile.io/2023/05/19/how-to-get-chatgpt-access-token-via-pkce.html)了。
-* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 可以访问 [这里](http://ai-20230626.fakeopen.com/auth) 拿 `Access Token`
 * 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser...
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.3 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.4 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
@@ -32,18 +32,18 @@
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
 ä½éªå°å * ç¹å» https://chat.zhile.io * ææ°æ¿ `Access Token`
 çææ¯åçï¼æè®°å½å¨[è¿é](https://zhile.io/2023/05/19/how-to-get-
-chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://
-ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
-[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
-Token` æææ `14`
+chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://ai-
+20230626.fakeopen.com/auth) æ¿ `Access Token` *
+ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é® [è¿é](http://chat.openai.com/api/auth/
+session) æ¿ `Access Token` * `Access Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
```

### Comparing `Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.2.3
+Version: 1.2.4
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
@@ -51,15 +51,15 @@
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
 * 最新拿 `Access Token` 的技术原理，我记录在[这里](https://zhile.io/2023/05/19/how-to-get-chatgpt-access-token-via-pkce.html)了。
-* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 可以访问 [这里](http://ai-20230626.fakeopen.com/auth) 拿 `Access Token`
 * 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser...
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.3 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.2.4 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
@@ -32,18 +32,18 @@
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
 ä½éªå°å * ç¹å» https://chat.zhile.io * ææ°æ¿ `Access Token`
 çææ¯åçï¼æè®°å½å¨[è¿é](https://zhile.io/2023/05/19/how-to-get-
-chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://
-ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
-[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
-Token` æææ `14`
+chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://ai-
+20230626.fakeopen.com/auth) æ¿ `Access Token` *
+ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é® [è¿é](http://chat.openai.com/api/auth/
+session) æ¿ `Access Token` * `Access Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
```

### Comparing `Pandora-ChatGPT-1.2.3/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.2.4/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/README.md` & `Pandora-ChatGPT-1.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [![PyPi workflow](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/python-publish.yml)
 [![Docker workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/docker-publish.yml)
 [![Discord](https://img.shields.io/discord/1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa)
 
 ## 体验地址
 * 点击 <a href="https://chat.zhile.io" target="_blank" title="Pandora Cloud体验地址">https://chat.zhile.io</a>
 * 最新拿 `Access Token` 的技术原理，我记录在[这里](https://zhile.io/2023/05/19/how-to-get-chatgpt-access-token-via-pkce.html)了。
-* 可以访问 [这里](http://ai.fakeopen.com/auth) 拿 `Access Token`
+* 可以访问 [这里](http://ai-20230626.fakeopen.com/auth) 拿 `Access Token`
 * 也可以官方登录，然后访问 [这里](http://chat.openai.com/api/auth/session) 拿 `Access Token`
 * `Access Token` 有效期 `14` 天，期间访问**不需要梯子**。这意味着你在手机上也可随意使用。
 * 这个页面上还包含一个共享账号的链接，**没有账号**的可以点进去体验一下。
  
 ## ChatGPT使用时可能会遇到：
 
 ### 1. Please stand by, while we are checking your browser...
```

#### html2text {}

```diff
@@ -12,18 +12,18 @@
 github.com/pengzhile/pandora/actions/workflows/python-publish.yml) [![Docker
 workflow](https://github.com/pengzhile/pandora/actions/workflows/docker-
 publish.yml/badge.svg)](https://github.com/pengzhile/pandora/actions/workflows/
 docker-publish.yml) [![Discord](https://img.shields.io/discord/
 1098772912242163795?label=Discord)](https://discord.gg/QBkd9JAaWa) ##
 ä½éªå°å * ç¹å» https://chat.zhile.io * ææ°æ¿ `Access Token`
 çææ¯åçï¼æè®°å½å¨[è¿é](https://zhile.io/2023/05/19/how-to-get-
-chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://
-ai.fakeopen.com/auth) æ¿ `Access Token` * ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é®
-[è¿é](http://chat.openai.com/api/auth/session) æ¿ `Access Token` * `Access
-Token` æææ `14`
+chatgpt-access-token-via-pkce.html)äºã * å¯ä»¥è®¿é® [è¿é](http://ai-
+20230626.fakeopen.com/auth) æ¿ `Access Token` *
+ä¹å¯ä»¥å®æ¹ç»å½ï¼ç¶åè®¿é® [è¿é](http://chat.openai.com/api/auth/
+session) æ¿ `Access Token` * `Access Token` æææ `14`
 å¤©ï¼æé´è®¿é®**ä¸éè¦æ¢¯å­**ãè¿æå³çä½ å¨ææºä¸ä¹å¯éæä½¿ç¨ã
 *
 è¿ä¸ªé¡µé¢ä¸è¿åå«ä¸ä¸ªå±äº«è´¦å·çé¾æ¥ï¼**æ²¡æè´¦å·**çå¯ä»¥ç¹è¿å»ä½éªä¸ä¸ã
 ## ChatGPTä½¿ç¨æ¶å¯è½ä¼éå°ï¼ ### 1. Please stand by, while we are
 checking your browser... ###
    å¨ä¸å¨æ¥ä¸ä¸ï¼ææ¶åè¿ä¸å¨æèåºäººæºéªè¯ãçï¼ ![t0]
 (https://github.com/pengzhile/pandora/raw/master/doc/images/t0.png) ### 2.
```

### Comparing `Pandora-ChatGPT-1.2.3/setup.py` & `Pandora-ChatGPT-1.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/pengzhile/pandora',
     packages=find_packages('src'),
     package_dir={'pandora': 'src/pandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['pandora-cloud~=0.4.9'],
+        'cloud': ['pandora-cloud~=0.4.10'],
     },
     entry_points={
         'console_scripts': [
             'pandora = pandora.launcher:run',
             'pandora-cloud = pandora.cloud_launcher:run',
         ]
     },
```

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.2.4/src/pandora/bots/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,16 @@
             return models[0]
 
         choices = ['r']
         Console.info_b('Choice model:')
         for idx, item in enumerate(models):
             number = str(idx + 1)
             choices.append(number)
-            Console.info('  {}.\t{} - {}'.format(number, item['title'], item['description']))
+            Console.info('  {}.\t{} - {} - {}'.format(number, item['title'], item['description'],
+                                                      '|'.join(item['tags'])))
 
         Console.warn('  r.\tRefresh model list')
 
         while True:
             choice = Prompt.ask('Your choice', choices=choices, show_choices=False)
             if 'r' == choice:
                 return self.__choice_model()
```

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.2.4/src/pandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.2.4/src/pandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.2.4/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.2.4/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.2.4/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/launcher.py` & `Pandora-ChatGPT-1.2.4/src/pandora/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from loguru import logger
 from rich.prompt import Prompt, Confirm
 
 from . import __version__
 from .bots.legacy import ChatBot as ChatBotLegacy
 from .bots.server import ChatBot as ChatBotServer
 from .exts import sentry
-from .exts.config import USER_CONFIG_DIR
+from .exts.config import USER_CONFIG_DIR, default_api_prefix
 from .exts.hooks import hook_except_handle
 from .exts.token import check_access_token_out
 from .openai.api import ChatGPT
 from .openai.auth import Auth0
 from .openai.utils import Console
 
 if 'nt' == os.name:
@@ -104,15 +104,15 @@
 
     return valid_tokens
 
 
 def main():
     global __show_verbose
 
-    api_prefix = getenv('CHATGPT_API_PREFIX', 'https://ai.fakeopen.com')
+    api_prefix = getenv('CHATGPT_API_PREFIX', default_api_prefix())
 
     Console.debug_b(
         '''
             Pandora - A command-line interface to ChatGPT
             Github: https://github.com/pengzhile/pandora
             Get access token: {}/auth
             Version: {}'''.format(api_prefix, __version__), end=''
```

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.2.4/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.2.4/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.2.4/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.2.4/src/pandora/openai/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from os import getenv
 
 import httpx
 import requests
 from certifi import where
 
 from .. import __version__
+from ..exts.config import default_api_prefix
 
 
 class API:
     def __init__(self, proxy, ca_bundle):
         self.proxy = proxy
         self.ca_bundle = ca_bundle
 
@@ -105,33 +106,35 @@
             'timeout': 100,
             'allow_redirects': False,
         }
 
         self.user_agent = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                           'Pandora/{} Safari/537.36'.format(__version__)
 
-        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://ai.fakeopen.com')
-
         super().__init__(proxy, self.req_kwargs['verify'])
 
     def __get_headers(self, token_key=None):
         return {
             'Authorization': 'Bearer ' + self.get_access_token(token_key),
             'User-Agent': self.user_agent,
             'Content-Type': 'application/json',
         }
 
+    @staticmethod
+    def __get_api_prefix():
+        return getenv('CHATGPT_API_PREFIX', default_api_prefix())
+
     def get_access_token(self, token_key=None):
         return self.access_tokens[token_key or self.default_token_key]
 
     def list_token_keys(self):
         return self.access_token_key_list
 
     def list_models(self, raw=False, token=None):
-        url = '{}/api/models'.format(self.api_prefix)
+        url = '{}/api/models'.format(self.__get_api_prefix())
         resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('list models failed: ' + self.__get_error(resp))
@@ -139,27 +142,27 @@
         result = resp.json()
         if 'models' not in result:
             raise Exception('list models failed: ' + resp.text)
 
         return result['models']
 
     def list_conversations(self, offset, limit, raw=False, token=None):
-        url = '{}/api/conversations?offset={}&limit={}'.format(self.api_prefix, offset, limit)
+        url = '{}/api/conversations?offset={}&limit={}'.format(self.__get_api_prefix(), offset, limit)
         resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('list conversations failed: ' + self.__get_error(resp))
 
         return resp.json()
 
     def get_conversation(self, conversation_id, raw=False, token=None):
-        url = '{}/api/conversation/{}'.format(self.api_prefix, conversation_id)
+        url = '{}/api/conversation/{}'.format(self.__get_api_prefix(), conversation_id)
         resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('get conversation failed: ' + self.__get_error(resp))
@@ -167,15 +170,15 @@
         return resp.json()
 
     def clear_conversations(self, raw=False, token=None):
         data = {
             'is_visible': False,
         }
 
-        url = '{}/api/conversations'.format(self.api_prefix)
+        url = '{}/api/conversations'.format(self.__get_api_prefix())
         resp = self.session.patch(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('clear conversations failed: ' + self.__get_error(resp))
@@ -190,15 +193,15 @@
         data = {
             'is_visible': False,
         }
 
         return self.__update_conversation(conversation_id, data, raw, token)
 
     def gen_conversation_title(self, conversation_id, model, message_id, raw=False, token=None):
-        url = '{}/api/conversation/gen_title/{}'.format(self.api_prefix, conversation_id)
+        url = '{}/api/conversation/gen_title/{}'.format(self.__get_api_prefix(), conversation_id)
         data = {
             'model': model,
             'message_id': message_id,
         }
         resp = self.session.post(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
@@ -275,21 +278,21 @@
             'conversation_id': conversation_id,
             'parent_message_id': parent_message_id,
         }
 
         return self.__request_conversation(data, token)
 
     def __request_conversation(self, data, token=None):
-        url = '{}/api/conversation'.format(self.api_prefix)
+        url = '{}/api/conversation'.format(self.__get_api_prefix())
         headers = {**self.session.headers, **self.__get_headers(token), 'Accept': 'text/event-stream'}
 
         return self._request_sse(url, headers, data)
 
     def __update_conversation(self, conversation_id, data, raw=False, token=None):
-        url = '{}/api/conversation/{}'.format(self.api_prefix, conversation_id)
+        url = '{}/api/conversation/{}'.format(self.__get_api_prefix(), conversation_id)
         resp = self.session.patch(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('update conversation failed: ' + self.__get_error(resp))
@@ -339,18 +342,20 @@
             **kwargs,
             'stream': stream,
         }
 
         return self.__request_conversation(api_key, data, stream)
 
     def __request_conversation(self, api_key, data, stream):
+        default = default_api_prefix()
+
         if api_key.startswith('fk-') or api_key.startswith('pk-'):
-            prefix = 'https://ai.fakeopen.com'
+            prefix = default
         else:
-            prefix = getenv('OPENAI_API_PREFIX', 'https://api.openai.com')
+            prefix = getenv('OPENAI_API_PREFIX', default)
         url = '{}/v1/chat/completions'.format(prefix)
 
         if stream:
             headers = {**self.__get_headers(api_key), 'Accept': 'text/event-stream'}
             return self._request_sse(url, headers, data)
 
         resp = self.session.post(url=url, headers=self.__get_headers(api_key), json=data, **self.req_kwargs)
```

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.2.4/src/pandora/openai/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 import re
 from datetime import datetime as dt
-from os import getenv
 from urllib.parse import urlparse, parse_qs
 
 import requests
 from certifi import where
 
 
 class Auth0:
@@ -23,32 +22,35 @@
                 'http': proxy,
                 'https': proxy,
             } if proxy else None,
             'verify': where(),
             'timeout': 100,
         }
         self.access_token = None
+        self.refresh_token = None
         self.expires = None
         self.user_agent = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                           'Chrome/109.0.0.0 Safari/537.36'
-        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://ai.fakeopen.com')
 
     @staticmethod
     def __check_email(email: str):
         regex = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
         return re.fullmatch(regex, email)
 
     def auth(self, login_local=True) -> str:
         if self.use_cache and self.access_token and self.expires and self.expires > dt.now():
             return self.access_token
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception('invalid email or password.')
 
-        return self.__part_two() if login_local else self.get_access_token_proxy()
+        return self.__part_two()
+
+    def get_refresh_token(self):
+        return self.refresh_token
 
     def __part_two(self) -> str:
         code_challenge = 'w6n3Ix420Xhhu-Q5-mOOEyuPZmAsJHUbBpO8Ub7xBCY'
         code_verifier = 'yGrXROHx_VazA0uovsxKfE263LMFcrSrdm4SlC-rob8'
 
         url = 'https://auth0.openai.com/authorize?client_id=pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh&audience=https%3A%2F' \
               '%2Fapi.openai.com%2Fv1&redirect_uri=com.openai.chat%3A%2F%2Fauth0.openai.com%2Fios%2Fcom.openai.chat' \
@@ -197,34 +199,15 @@
         resp = self.session.post(url, headers=headers, json=data, allow_redirects=False, **self.req_kwargs)
 
         if resp.status_code == 200:
             json = resp.json()
             if 'access_token' not in json:
                 raise Exception('Get access token failed, maybe you need a proxy.')
 
+            if 'refresh_token' in json:
+                self.refresh_token = json['refresh_token']
+
             self.access_token = json['access_token']
             self.expires = dt.utcnow() + datetime.timedelta(seconds=json['expires_in']) - datetime.timedelta(minutes=5)
             return self.access_token
         else:
             raise Exception(resp.text)
-
-    def get_access_token_proxy(self) -> str:
-        url = '{}/api/auth/login'.format(self.api_prefix)
-        headers = {
-            'User-Agent': self.user_agent,
-        }
-        data = {
-            'username': self.email,
-            'password': self.password,
-        }
-        resp = self.session.post(url=url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs)
-
-        if resp.status_code == 200:
-            json = resp.json()
-            if 'accessToken' not in json:
-                raise Exception('Get access token failed.')
-
-            self.access_token = json['accessToken']
-            self.expires = dt.strptime(json['expires'], '%Y-%m-%dT%H:%M:%S.%fZ') - datetime.timedelta(minutes=5)
-            return self.access_token
-        else:
-            raise Exception('Error get access token.')
```

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.2.4/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.2.4/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.2.3/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.2.4/src/pandora/turbo/chat.py`

 * *Files identical despite different names*

