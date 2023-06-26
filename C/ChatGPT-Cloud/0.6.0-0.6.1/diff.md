# Comparing `tmp/ChatGPT-Cloud-0.6.0.tar.gz` & `tmp/ChatGPT-Cloud-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-dzbfrmgs/ChatGPT-Cloud-0.6.0.tar", last modified: Thu Jun 22 14:03:23 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-pd9fo9wj/ChatGPT-Cloud-0.6.1.tar", last modified: Mon Jun 26 05:02:05 2023, max compression
```

## Comparing `ChatGPT-Cloud-0.6.0.tar` & `ChatGPT-Cloud-0.6.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js
--rw-r--r--   0 runner    (1001) docker     (123)  1259345 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
--rw-r--r--   0 runner    (1001) docker     (123)   337227 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd84.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-389963a554a230d2.js
--rw-r--r--   0 runner    (1001) docker     (123)  1003292 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-c0db665988dd1d67.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
--rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-875a033295abd238.js
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb39.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   125366 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest1.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/
--rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/sweetalert2/
--rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    68840 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:23.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/share.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19108 2023-06-22 14:03:08.000000 ChatGPT-Cloud-0.6.0/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1259345 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js
+-rw-r--r--   0 runner    (1001) docker     (123)   337227 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd84.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   115058 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-63cd9f049103272b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-6ac6d4f0510ced68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-389963a554a230d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1003292 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-338530f42d5b2105.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-c0db665988dd1d67.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-433a1bbdb23dd341.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27863 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-875a033295abd238.js
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-6557d60655b68492.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb39.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   125366 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/sweetalert2/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    68840 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:02:05.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/share.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-06-26 05:01:54.000000 ChatGPT-Cloud-0.6.1/src/pandora_cloud/server.py
```

### Comparing `ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/PKG-INFO` & `ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPT-Cloud
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/lannychan/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora-cloud
 Project-URL: Tracker, https://github.com/lannychan/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `ChatGPT-Cloud-0.6.0/ChatGPT_Cloud.egg-info/SOURCES.txt` & `ChatGPT-Cloud-0.6.1/ChatGPT_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/LICENSE` & `ChatGPT-Cloud-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/PKG-INFO` & `ChatGPT-Cloud-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPT-Cloud
-Version: 0.6.0
+Version: 0.6.1
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/lannychan/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora-cloud
 Project-URL: Tracker, https://github.com/lannychan/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `ChatGPT-Cloud-0.6.0/README.md` & `ChatGPT-Cloud-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/setup.py` & `ChatGPT-Cloud-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/259-c6320349d8f3ff4a.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/58-87db5ef127e7d0b9.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/686-7a99a2d97a992914.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-a453fd719d5bf767.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd84.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/734-99309a157861fd84.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/main-2f10fecca4c74462.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-d6b322741680e2b4.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-389963a554a230d2.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-389963a554a230d2.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-878ac43f93e00b3f.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-c7951a77c5f4547f.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-927659025ea31258.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-478ebccc4055d75b.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-f4fdb51b436aaaf4.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-47cc26eb7b585e67.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-d5fbb97bc5d39e59.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-c0db665988dd1d67.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-c0db665988dd1d67.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-1401d2c2b63d99cf.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/business-e449df976df219cb.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-66b11e86067b001d.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-875a033295abd238.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-875a033295abd238.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb39.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/chunks/webpack-c08a82b5c21eeb39.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/css/df35a37d1f08004f.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest1.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/_next/static/cx416mT2Lb0ZTj5FxFg1l/buildManifest1.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/apple-touch-icon.png` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/favicon-16x16.png` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/favicon-32x32.png` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/service-worker.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/404.html` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/404.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/chat.html` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/detail.html` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/login.html` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/login.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charset="utf-8"/><meta http-equiv="X-UA-Compatible"content="IE=edge"/><meta name="viewport"content="width=device-width, initial-scale=1"/><meta name="robots"content="noindex, nofollow"/><link rel="manifest" href="/manifest.json"><link rel="preconnect" href="{{api_prefix|safe}}"/><link rel="stylesheet"href="/ulp/react-components/1.66.5/css/main.cdn.min.css"/><link rel="stylesheet" href="/sweetalert2/bulma.min.css"/><style id="custom-styles-container">body{background:#ffffff;font-family:ulp-font,-apple-system,BlinkMacSystemFont,Roboto,Helvetica,sans-serif}.cb5d9646a{background:#ffffff}.ccc0ccfed.c9e0e495f{background:#D00E17}.ccc0ccfed.ce493028a{background:#0A8852}.c2fd8f218{background-color:#10a37f;color:#ffffff}.c2fd8f218 a,.c2fd8f218 a:visited{color:#ffffff}.c2ed2d5ea{background-color:#0A8852}.c57c3fbaa{background-color:#D00E17}.input.c224a8982{border-color:#D00E17}.error-cloud{background-color:#D00E17}.error-fatal{background-color:#D00E17}.error-local{background-color:#D00E17}#alert-trigger{background-color:#D00E17}</style><style>.no-js{clip:rect(0 0 0 0);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}</style><noscript><style>.js-required{display:none!important}.no-js{clip:auto;clip-path:none;height:auto;overflow:auto;position:static;white-space:normal;width:var(--prompt-width)}</style></noscript><style>@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIRegular.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIRegular.woff)format("woff");font-weight:normal;font-style:normal}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIRegularItalic.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIRegularItalic.woff)format("woff");font-weight:normal;font-style:italic}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIBold.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIBold.woff)format("woff");font-weight:bold;font-style:normal}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIBoldItalic.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIBoldItalic.woff)format("woff");font-weight:bold;font-style:italic}:root{--font-family:"ColfaxAI",-apple-system,BlinkMacSystemFont,Helvetica,sans-serif;--primary-color:#10a37f;--primary-color-no-override:#10a37f;--action-primary-color:#10a37f;--link-color:#10a37f;--input-box-shadow-depth:1px;--page-background-color:#ffffff}body{font-family:var(--font-family);background-color:var(--page-background-color)}.oai-wrapper{display:flex;flex-direction:column;justify-content:space-between;min-height:100%}.oai-header{display:flex;align-items:center;justify-content:center;padding:32px 0 0;flex:0 0 auto}.oai-header svg{width:32px;height:32px;fill:#202123}.oai-footer{display:flex;align-items:center;justify-content:center;color:#6e6e80;padding:12px 0 24px;flex:0 0 auto}.oai-footer a{color:var(--primary-color);margin:0 10px}._widget-auto-layout main._widget{flex:1 0 auto;min-height:0}main header>img:first-of-type{display:none}main>section,main>section>div:first-child{box-shadow:none}main header>h1{font-weight:bold!important;font-size:32px!important}main a{font-weight:normal!important}.ulp-alternate-action{text-align:center}button[type="submit"]{font-family:var(--font-family)}main header>h1{margin-bottom:0!important}main header>h1+div{display:none!important}</style><script>window.__api_prefix='{{api_prefix|safe}}';</script></head><body class="_widget-auto-layout"><div class="oai-wrapper"><main class="_widget login"><section class="c44996798 _prompt-box-outer c90f12a70"><div class="c1d338956 ca92c9765"><div class="cb60e04f7"><header class="c729fb2be cc2b5de2d"><div title="OpenAI"id="custom-prompt-logo"style="width: auto !important; height: 60px !important; position: static !important; margin: auto !important; padding: 0 !important; background-color: transparent !important; background-position: center !important; background-size: contain !important; background-repeat: no-repeat !important"></div><h1 class="ca61186d8 cb87ac8dc">Welcome Back</h1><div class="cc6691322 ccd3868ad"></div></header><div class="cd073cc55 c3057e255"><form method="POST"class="c15ce5740 _form-login-password"data-form-primary="true"><div class="ce7821f58 c9ee3d098"><div class="c83779892"><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 text c183d9a0a{{ ' c3ab3f08e c666327b8' if error else '' }}"data-action-text=""data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 cd80352de"for="username">Email address</label><input type="hidden"id="txtNext"name="next"value="{{ next }}"/><input class="input cdb43277e c07239cfd{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}"inputMode="email"name="username"id="username"type="text"value="{{ username }}"required autoComplete="username"autoCapitalize="none"spellCheck="false"autoFocus/><div class="c41b9071b js-required c6e062879 cd80352de"data-dynamic-label-for="username"aria-hidden="true">Email address</div></div></div><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 password c9378f091{{ ' c3ab3f08e c666327b8' if error else '' }}"data-action-text=""data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 c3c2bcd98"for="password">Password</label><input class="input cdb43277e c94bb61d1{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}"name="password"id="password"type="password"required autoComplete="current-password"autoCapitalize="none"spellCheck="false"autoFocus/><div class="c41b9071b js-required c6e062879 c3c2bcd98"data-dynamic-label-for="password"aria-hidden="true">Password</div><button type="button"class="c994ae14c ulp-button-icon ca2dc35c7 _button-icon"data-action="toggle"><span aria-hidden="true"class="password-icon-tooltip show-password-tooltip">Show password</span><span aria-hidden="true"class="password-icon-tooltip hide-password-tooltip hide">Hide password</span><span class="screen-reader-only password-toggle-label"data-label="show-password">Show password</span><span class="screen-reader-only password-toggle-label hide"data-label="hide-password">Hide password</span><span class="c9e3d0156 password js-required"aria-hidden="true"></span></button></div></div><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 text c183d9a0a{{ ' c3ab3f08e c666327b8' if error else '' }}" data-action-text="" data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 cd80352de" for="mfa_code">MFA Code</label><input class="input cdb43277e c07239cfd{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}" name="mfa_code" type="text" autoCapitalize="none" spellCheck="false" placeholder="Optional"/><div class="c41b9071b js-required c6e062879 cd80352de" data-dynamic-label-for="mfa_code" aria-hidden="true">MFA Code</div></div>{% if error %}<span id="error-element-password" class="ulp-input-error-message" data-error-code="wrong-email-credentials"><span class="ulp-input-error-icon" role="img" aria-label="Error"></span>{{ error }}</span>{% endif %}</div></div></div><div class="cc336b8c1"><button type="submit"name="action"value="default"class="c994ae14c c2fd8f218 ca2dc35c7 c0c7f649b _button-login-password"data-action-button-primary="true">Continue</button></div></form><div class="ulp-alternate-action  _alternate-action __s16nu9"><p class="cb21c50a9 cba0941cc cf12e064e">Need an access token?<a class="c34934055 c2dd6083e" href="https://ai.fakeopen.com/auth" target="_blank">Go get it</a></p></div><div class="c11767592 c16884ee3"><span>Or</span></div><div class="c497a10c6 c87650a4b"><form method="post"data-provider="windowslive"class="cada38124 c856cfac0 c45d84291"data-form-secondary="true"><button type="button"id="submit-token"class="cb920eae9 c4a315d94 c5c10a20c"data-action-button-secondary="true"><input type="hidden"name="action"value="token"><span class="c47d81fe7">Continue with Access Token</span></button></form></div></div></div></div></section></main><script id="client-scripts"type="text/javascript">!function(){var t,e,v,h,r,n={exports:function(r,a){var n={};function i(t,e,r,n){return t.addEventListener(e,r,n)}function o(t){return"string"==typeof t}function c(t,e){return t.getAttribute(e)}function s(t,e,r){return t.setAttribute(e,r)}return{addClass:function(t,e){if(t.classList)return t.classList.add(e);var r=t.className.split(" ");-1===r.indexOf(e)&&(r.push(e),t.className=r.join(" "))},toggleClass:function(t,e){if(t.classList)return t.classList.toggle(e);var r=t.className.split(" "),n=r.indexOf(e);-1!==n?r.splice(n,1):r.push(e),t.className=r.join(" ")},addClickListener:function(t,e){return i(t,"click",e)},addEventListener:i,getAttribute:c,getElementById:function(t){return a.getElementById(t)},getParent:function(t){return t.parentNode},isString:o,loadScript:function(t){var e=a.createElement("script");e.src=t,e.async=!0,a.body.appendChild(e)},poll:function(t){var i=t.interval||2e3,e=t.url||r.location.href,o=t.condition||function(){return!0},c=t.onSuccess||function(){},s=t.onError||function(){};return setTimeout(function n(){var a=new XMLHttpRequest;return a.open("GET",e),a.setRequestHeader("Accept","application/json"),a.onload=function(){if(200===a.status){var t="application/json"===a.getResponseHeader("Content-Type").split(";")[0]?JSON.parse(a.responseText):a.responseText;return o(t)?c():setTimeout(n,i)}if(429!==a.status)return s({status:a.status,responseText:a.responseText});var e=1e3*Number.parseInt(a.getResponseHeader("X-RateLimit-Reset")),r=e-(new Date).getTime();return setTimeout(n,i<r?r:i)},a.send()},i)},querySelector:function(t,e){return o(t)?a.querySelector(t):t.querySelector(e)},querySelectorAll:function(t,e){var r=o(t)?a.querySelectorAll(t):t.querySelectorAll(e);return Array.prototype.slice.call(r)},removeClass:function(t,e){if(t.classList)return t.classList.remove(e);var r=t.className.split(" "),n=r.indexOf(e);-1!==n&&(r.splice(n,1),t.className=r.join(" "))},setAttribute:s,removeAttribute:function(t,e){return t.removeAttribute(e)},swapAttributes:function(t,e,r){var n=c(t,e),a=c(t,r);s(t,r,n),s(t,e,a)},setGlobalFlag:function(t,e){n[t]=!!e},getGlobalFlag:function(t){return!!n[t]},preventFormSubmit:function(t){t.stopPropagation(),t.preventDefault()},matchMedia:function(t){return"function"!=typeof r.matchMedia&&r.matchMedia(t).matches},dispatchEvent:function(t,e,r){var n;"function"!=typeof Event?(n=a.createEvent("Event")).initCustomEvent(e,r,!1):n=new Event(e,{bubbles:r}),t.dispatchEvent(n)},setTimeout:setTimeout,timeoutPromise:function(t,a){return new Promise(function(e,r){var n=setTimeout(function(){r(new Error("timeoutPromise: promise timed out"))},t);a.then(function(t){clearTimeout(n),e(t)},function(t){clearTimeout(n),r(t)})})}}}}.exports(window,document),a={exports:function(t,e){for(var i="ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_",l=new Uint8Array(256),o=0;o<i.length;o++)l[i.charCodeAt(o)]=o;function c(t){var e,r=new Uint8Array(t),n=r.length,a="";for(e=0;e<n;e+=3)a+=i[r[e]>>2],a+=i[(3&r[e])<<4|r[e+1]>>4],a+=i[(15&r[e+1])<<2|r[e+2]>>6],a+=i[63&r[e+2]];return n%3==2?a=a.substring(0,a.length-1):n%3==1&&(a=a.substring(0,a.length-2)),a}function r(){return navigator&&navigator.credentials&&"undefined"!=typeof PublicKeyCredential}return{base64URLEncode:c,base64URLDecode:function(t){var e,r,n,a,i,o=.75*t.length,c=t.length,s=0,u=new Uint8Array(o);for(e=0;e<c;e+=4)r=l[t.charCodeAt(e)],n=l[t.charCodeAt(e+1)],a=l[t.charCodeAt(e+2)],i=l[t.charCodeAt(e+3)],u[s++]=r<<2|n>>4,u[s++]=(15&n)<<4|a>>2,u[s++]=(3&a)<<6|63&i;return u.buffer},publicKeyCredentialToJSON:function t(e){if(e instanceof Array){var r=[];for(o=0;o<e.length;o+=1)r.push(t(e[o]));return r}if(e instanceof ArrayBuffer)return c(e);if(e instanceof Object){var n={};for(var a in e)n[a]=t(e[a]);return n}return e},str2ab:function(t){for(var e=new ArrayBuffer(t.length),r=new Uint8Array(e),n=0,a=t.length;n<a;n++)r[n]=t.charCodeAt(n);return e},isWebAuthnAvailable:r,isWebauthnPlatformAuthenticatorAvailableAsync:function(t){return r()?t(1e3,PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable()):Promise.resolve(!1)}}}}.exports(window,document);((t={}).exports=function(n,t,o,c,s,u,l){t("div.c51fadc8b.password").forEach(function(t){var a,i,e=n(t,"input"),r=n(t,'[data-action="toggle"]');o(t,(a=e,i=r,function(t){if(t.target.classList.contains("ulp-button-icon")){if(a.type="password"===a.type?"text":"password",i){var e=i.querySelector(".show-password-tooltip"),r=i.querySelector(".hide-password-tooltip");e&&u(e,"hide"),r&&u(r,"hide")}var n=l(a);"text"===a.type?c(n,"show"):s(n,"show")}}))})},t.exports)(n.querySelector,n.querySelectorAll,n.addClickListener,n.addClass,n.removeClass,n.toggleClass,n.getParent),{exports:function(t,n,a,e){var r=t(".cfd2e2d98"),i=t("#alert-trigger"),o=t(".c5f2f0292"),c=t(".c989a3dfe"),s=!1;i&&c&&r&&e(r,function(t){var e=t.target===i,r=c.contains(t.target);return e&&!s?(n(o,"show"),void(s=!0)):e&&s||s&&!r?(a(o,"show"),void(s=!1)):void 0})}}.exports(n.querySelector,n.addClass,n.removeClass,n.addClickListener),(v="recaptcha_v2",h="recaptcha_enterprise",(e={}).exports=function(t,a,i,o,c,n){var s,u=a("div[data-recaptcha-sitekey]"),e=a("div[data-recaptcha-sitekey] input"),l=a("#ulp-recaptcha");function f(){return u.getAttribute("data-recaptcha-provider")}function d(t){return e.value=t}function p(t,e){if(t&&t.getBoundingClientRect){if(!n("(max-width: 480px)"))return l.style.transform="",void(l.style.height="");(void 0===e||isNaN(e))&&(e=1.4);var r=72*e;l.style.transform="scale("+e+")",l.style.height=r+"px",l.style.width="10px",u.clientWidth+8<t.getBoundingClientRect().width&&p(t,e-.01)}}u&&(s="recaptchaCallback_"+Math.floor(1000001*Math.random()),window[s]=function(){var t,e,r,n;delete window[s],t=function(t){switch(t){case v:return window.grecaptcha;case h:return window.grecaptcha.enterprise}}(f()),e=t.render(l,{sitekey:u.getAttribute("data-recaptcha-sitekey"),"expired-callback":function(){d(""),i(u,"c3ab3f08e"),t.reset(e)},callback:function(t){d(t),o(u,"c3ab3f08e")}}),r=function(t){p(t),c(window,"resize",function(){p(t)})},n=setInterval(function(){var t=a("#ulp-recaptcha iframe");if(t)return clearInterval(n),r(t)},200)},t(function(t,e,r){switch(t){case v:return"https://www.recaptcha.net/recaptcha/api.js?hl="+e+"&onload="+r;case h:return"https://www.recaptcha.net/recaptcha/enterprise.js?render=explicit&hl="+e+"&onload="+r}}(f(),u.getAttribute("data-recaptcha-lang"),s)))},e.exports)(n.loadScript,n.querySelector,n.addClass,n.removeClass,n.addEventListener,n.matchMedia),((r={}).exports=function(n,t,a,i,o,c,s,u,r,l){function f(t){var e=t.target,r=c(e);e.value||l(e,"data-autofilled")?i(r,"c819d1bdd"):o(r,"c819d1bdd")}function d(t){var e=t.target;"onAutoFillStart"===t.animationName&&(r(e,"data-autofilled",!0),u(t.target,"change",!0),a(e,"keyup",p,{once:!0}))}function p(t){var e=t.target;r(e,"data-autofilled","")}if(n("body._simple-labels"))return t(".c41b9071b.no-js").forEach(function(t){o(t,"no-js")}),void t(".c41b9071b.js-required").forEach(function(t){i(t,"hide")});t(".c51fadc8b:not(.cf8bf2cb6):not(disabled)").forEach(function(t){i(t,"c85b18936");var e,r=n(t,".input");r.value&&i(t,"c819d1bdd"),a(t,"change",f),a(r,"blur",f),a(r,"animationstart",d),e=r,s(function(){e.value&&u(e,"change",!0)},100)})},r.exports)(n.querySelector,n.querySelectorAll,n.addEventListener,n.addClass,n.removeClass,n.getParent,n.setTimeout,n.dispatchEvent,n.setAttribute,n.getAttribute),{exports:function(t,e,r,n,a,i){function o(t){var e=r("submitted");n("submitted",!0),e?a(t):"apple"===i(t.target,"data-provider")&&setTimeout(function(){n("submitted",!1)},2e3)}var c=t("form");c&&c.forEach(function(t){e(t,"submit",o)})}}.exports(n.querySelectorAll,n.addEventListener,n.getGlobalFlag,n.setGlobalFlag,n.preventFormSubmit,n.getAttribute),{exports:function(e,t,r){var n=e("form._form-detect-browser-capabilities"),a=e("main.login-id");if(n||a){var i=t.isWebAuthnAvailable();e("#webauthn-available").value=i?"true":"false",e("#js-available").value="true",navigator.brave?navigator.brave.isBrave().then(function(t){e("#is-brave").value=t,o()}):o()}function o(){i?t.isWebauthnPlatformAuthenticatorAvailableAsync(r).then(function(t){e("#webauthn-platform-available").value=t?"true":"false",n&&n.submit()}).catch(function(t){e("#webauthn-platform-available").value="false",n&&n.submit()}):(e("#webauthn-platform-available").value="false",n&&n.submit())}}}.exports(n.querySelector,a,n.timeoutPromise)}();</script><footer class="oai-footer"><a href="https://github.com/pengzhile/pandora"target="_blank">Pandora on GitHub</a></footer></div><script src="/sweetalert2/sweetalert2.all.min-bc15590d.js" defer=""></script><script type="text/javascript">function updateHeader(text){const $h1=document.querySelector('main header > h1');if($h1){$h1.innerText=text}}updateHeader('Welcome Back');window.addEventListener('load',function(){const submitBtn=document.querySelector('#submit-token');submitBtn.addEventListener('click',function(){Swal.fire({input:'textarea',inputLabel:'Continue with Access Token',inputPlaceholder:'Please input access token...',inputAttributes:{'aria-label':'Please input access token'},showCancelButton:true}).then((result)=>{if(!result.isConfirmed||!result.value){return}fetch('login_token',{method:'POST',headers:{'Content-Type':'application/x-www-form-urlencoded'},body:'action=token&access_token='+encodeURIComponent(result.value)+'&next='+encodeURIComponent(document.getElementById('txtNext').value)}).then(response=>response.json()).then(data=>{if(0===data.code){window.location.href=data.url}else{Swal.fire('Error',data.message,'error')}}).catch(error=>console.error(error))});});});</script><script>if('serviceWorker' in navigator){window.addEventListener('load',function(){navigator.serviceWorker.register('/service-worker.js',{scope:'/'}).then(function(reg){console.log('ServiceWorker registration successful with scope: ',reg.scope);},function(e){console.log('ServiceWorker registration failed: ',e);});});}</script></body></html>
+<!DOCTYPE html><html><head><meta charset="utf-8"/><meta http-equiv="X-UA-Compatible"content="IE=edge"/><meta name="viewport"content="width=device-width, initial-scale=1"/><meta name="robots"content="noindex, nofollow"/><link rel="manifest" href="/manifest.json"><link rel="preconnect" href="{{api_prefix|safe}}"/><link rel="stylesheet"href="/ulp/react-components/1.66.5/css/main.cdn.min.css"/><link rel="stylesheet" href="/sweetalert2/bulma.min.css"/><style id="custom-styles-container">body{background:#ffffff;font-family:ulp-font,-apple-system,BlinkMacSystemFont,Roboto,Helvetica,sans-serif}.cb5d9646a{background:#ffffff}.ccc0ccfed.c9e0e495f{background:#D00E17}.ccc0ccfed.ce493028a{background:#0A8852}.c2fd8f218{background-color:#10a37f;color:#ffffff}.c2fd8f218 a,.c2fd8f218 a:visited{color:#ffffff}.c2ed2d5ea{background-color:#0A8852}.c57c3fbaa{background-color:#D00E17}.input.c224a8982{border-color:#D00E17}.error-cloud{background-color:#D00E17}.error-fatal{background-color:#D00E17}.error-local{background-color:#D00E17}#alert-trigger{background-color:#D00E17}</style><style>.no-js{clip:rect(0 0 0 0);clip-path:inset(50%);height:1px;overflow:hidden;position:absolute;white-space:nowrap;width:1px}</style><noscript><style>.js-required{display:none!important}.no-js{clip:auto;clip-path:none;height:auto;overflow:auto;position:static;white-space:normal;width:var(--prompt-width)}</style></noscript><style>@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIRegular.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIRegular.woff)format("woff");font-weight:normal;font-style:normal}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIRegularItalic.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIRegularItalic.woff)format("woff");font-weight:normal;font-style:italic}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIBold.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIBold.woff)format("woff");font-weight:bold;font-style:normal}@font-face{font-family:"ColfaxAI";src:url(/fonts/colfax/ColfaxAIBoldItalic.woff2)format("woff2"),url(/fonts/colfax/ColfaxAIBoldItalic.woff)format("woff");font-weight:bold;font-style:italic}:root{--font-family:"ColfaxAI",-apple-system,BlinkMacSystemFont,Helvetica,sans-serif;--primary-color:#10a37f;--primary-color-no-override:#10a37f;--action-primary-color:#10a37f;--link-color:#10a37f;--input-box-shadow-depth:1px;--page-background-color:#ffffff}body{font-family:var(--font-family);background-color:var(--page-background-color)}.oai-wrapper{display:flex;flex-direction:column;justify-content:space-between;min-height:100%}.oai-header{display:flex;align-items:center;justify-content:center;padding:32px 0 0;flex:0 0 auto}.oai-header svg{width:32px;height:32px;fill:#202123}.oai-footer{display:flex;align-items:center;justify-content:center;color:#6e6e80;padding:12px 0 24px;flex:0 0 auto}.oai-footer a{color:var(--primary-color);margin:0 10px}._widget-auto-layout main._widget{flex:1 0 auto;min-height:0}main header>img:first-of-type{display:none}main>section,main>section>div:first-child{box-shadow:none}main header>h1{font-weight:bold!important;font-size:32px!important}main a{font-weight:normal!important}.ulp-alternate-action{text-align:center}button[type="submit"]{font-family:var(--font-family)}main header>h1{margin-bottom:0!important}main header>h1+div{display:none!important}</style><script>window.__api_prefix='{{api_prefix|safe}}';</script></head><body class="_widget-auto-layout"><div class="oai-wrapper"><main class="_widget login"><section class="c44996798 _prompt-box-outer c90f12a70"><div class="c1d338956 ca92c9765"><div class="cb60e04f7"><header class="c729fb2be cc2b5de2d"><div title="OpenAI"id="custom-prompt-logo"style="width: auto !important; height: 60px !important; position: static !important; margin: auto !important; padding: 0 !important; background-color: transparent !important; background-position: center !important; background-size: contain !important; background-repeat: no-repeat !important"></div><h1 class="ca61186d8 cb87ac8dc">Welcome Back</h1><div class="cc6691322 ccd3868ad"></div></header><div class="cd073cc55 c3057e255"><form method="POST"class="c15ce5740 _form-login-password"data-form-primary="true"><div class="ce7821f58 c9ee3d098"><div class="c83779892"><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 text c183d9a0a{{ ' c3ab3f08e c666327b8' if error else '' }}"data-action-text=""data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 cd80352de"for="username">Email address</label><input type="hidden"id="txtNext"name="next"value="{{ next }}"/><input class="input cdb43277e c07239cfd{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}"inputMode="email"name="username"id="username"type="text"value="{{ username }}"required autoComplete="username"autoCapitalize="none"spellCheck="false"autoFocus/><div class="c41b9071b js-required c6e062879 cd80352de"data-dynamic-label-for="username"aria-hidden="true">Email address</div></div></div><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 password c9378f091{{ ' c3ab3f08e c666327b8' if error else '' }}"data-action-text=""data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 c3c2bcd98"for="password">Password</label><input class="input cdb43277e c94bb61d1{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}"name="password"id="password"type="password"required autoComplete="current-password"autoCapitalize="none"spellCheck="false"autoFocus/><div class="c41b9071b js-required c6e062879 c3c2bcd98"data-dynamic-label-for="password"aria-hidden="true">Password</div><button type="button"class="c994ae14c ulp-button-icon ca2dc35c7 _button-icon"data-action="toggle"><span aria-hidden="true"class="password-icon-tooltip show-password-tooltip">Show password</span><span aria-hidden="true"class="password-icon-tooltip hide-password-tooltip hide">Hide password</span><span class="screen-reader-only password-toggle-label"data-label="show-password">Show password</span><span class="screen-reader-only password-toggle-label hide"data-label="hide-password">Hide password</span><span class="c9e3d0156 password js-required"aria-hidden="true"></span></button></div></div><div class="input-wrapper _input-wrapper"><div class="c51fadc8b c7cc0d651 text c183d9a0a{{ ' c3ab3f08e c666327b8' if error else '' }}" data-action-text="" data-alternate-action-text=""><label class="c41b9071b no-js c6e062879 cd80352de" for="mfa_code">MFA Code</label><input class="input cdb43277e c07239cfd{{ ' cca61e7fa c224a8982 c08661137' if error else '' }}" name="mfa_code" type="text" autoCapitalize="none" spellCheck="false" placeholder="Optional"/><div class="c41b9071b js-required c6e062879 cd80352de" data-dynamic-label-for="mfa_code" aria-hidden="true">MFA Code</div></div>{% if error %}<span id="error-element-password" class="ulp-input-error-message" data-error-code="wrong-email-credentials"><span class="ulp-input-error-icon" role="img" aria-label="Error"></span>{{ error }}</span>{% endif %}</div></div></div><div class="cc336b8c1"><button type="submit"name="action"value="default"class="c994ae14c c2fd8f218 ca2dc35c7 c0c7f649b _button-login-password"data-action-button-primary="true">Continue</button></div></form><div class="ulp-alternate-action  _alternate-action __s16nu9"><p class="cb21c50a9 cba0941cc cf12e064e">Need an access token?<a class="c34934055 c2dd6083e" href="{{api_prefix|safe}}/auth" target="_blank">Go get it</a></p></div><div class="c11767592 c16884ee3"><span>Or</span></div><div class="c497a10c6 c87650a4b"><form method="post"data-provider="windowslive"class="cada38124 c856cfac0 c45d84291"data-form-secondary="true"><button type="button"id="submit-token"class="cb920eae9 c4a315d94 c5c10a20c"data-action-button-secondary="true"><input type="hidden"name="action"value="token"><span class="c47d81fe7">Continue with Access Token</span></button></form></div></div></div></div></section></main><script id="client-scripts"type="text/javascript">!function(){var t,e,v,h,r,n={exports:function(r,a){var n={};function i(t,e,r,n){return t.addEventListener(e,r,n)}function o(t){return"string"==typeof t}function c(t,e){return t.getAttribute(e)}function s(t,e,r){return t.setAttribute(e,r)}return{addClass:function(t,e){if(t.classList)return t.classList.add(e);var r=t.className.split(" ");-1===r.indexOf(e)&&(r.push(e),t.className=r.join(" "))},toggleClass:function(t,e){if(t.classList)return t.classList.toggle(e);var r=t.className.split(" "),n=r.indexOf(e);-1!==n?r.splice(n,1):r.push(e),t.className=r.join(" ")},addClickListener:function(t,e){return i(t,"click",e)},addEventListener:i,getAttribute:c,getElementById:function(t){return a.getElementById(t)},getParent:function(t){return t.parentNode},isString:o,loadScript:function(t){var e=a.createElement("script");e.src=t,e.async=!0,a.body.appendChild(e)},poll:function(t){var i=t.interval||2e3,e=t.url||r.location.href,o=t.condition||function(){return!0},c=t.onSuccess||function(){},s=t.onError||function(){};return setTimeout(function n(){var a=new XMLHttpRequest;return a.open("GET",e),a.setRequestHeader("Accept","application/json"),a.onload=function(){if(200===a.status){var t="application/json"===a.getResponseHeader("Content-Type").split(";")[0]?JSON.parse(a.responseText):a.responseText;return o(t)?c():setTimeout(n,i)}if(429!==a.status)return s({status:a.status,responseText:a.responseText});var e=1e3*Number.parseInt(a.getResponseHeader("X-RateLimit-Reset")),r=e-(new Date).getTime();return setTimeout(n,i<r?r:i)},a.send()},i)},querySelector:function(t,e){return o(t)?a.querySelector(t):t.querySelector(e)},querySelectorAll:function(t,e){var r=o(t)?a.querySelectorAll(t):t.querySelectorAll(e);return Array.prototype.slice.call(r)},removeClass:function(t,e){if(t.classList)return t.classList.remove(e);var r=t.className.split(" "),n=r.indexOf(e);-1!==n&&(r.splice(n,1),t.className=r.join(" "))},setAttribute:s,removeAttribute:function(t,e){return t.removeAttribute(e)},swapAttributes:function(t,e,r){var n=c(t,e),a=c(t,r);s(t,r,n),s(t,e,a)},setGlobalFlag:function(t,e){n[t]=!!e},getGlobalFlag:function(t){return!!n[t]},preventFormSubmit:function(t){t.stopPropagation(),t.preventDefault()},matchMedia:function(t){return"function"!=typeof r.matchMedia&&r.matchMedia(t).matches},dispatchEvent:function(t,e,r){var n;"function"!=typeof Event?(n=a.createEvent("Event")).initCustomEvent(e,r,!1):n=new Event(e,{bubbles:r}),t.dispatchEvent(n)},setTimeout:setTimeout,timeoutPromise:function(t,a){return new Promise(function(e,r){var n=setTimeout(function(){r(new Error("timeoutPromise: promise timed out"))},t);a.then(function(t){clearTimeout(n),e(t)},function(t){clearTimeout(n),r(t)})})}}}}.exports(window,document),a={exports:function(t,e){for(var i="ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_",l=new Uint8Array(256),o=0;o<i.length;o++)l[i.charCodeAt(o)]=o;function c(t){var e,r=new Uint8Array(t),n=r.length,a="";for(e=0;e<n;e+=3)a+=i[r[e]>>2],a+=i[(3&r[e])<<4|r[e+1]>>4],a+=i[(15&r[e+1])<<2|r[e+2]>>6],a+=i[63&r[e+2]];return n%3==2?a=a.substring(0,a.length-1):n%3==1&&(a=a.substring(0,a.length-2)),a}function r(){return navigator&&navigator.credentials&&"undefined"!=typeof PublicKeyCredential}return{base64URLEncode:c,base64URLDecode:function(t){var e,r,n,a,i,o=.75*t.length,c=t.length,s=0,u=new Uint8Array(o);for(e=0;e<c;e+=4)r=l[t.charCodeAt(e)],n=l[t.charCodeAt(e+1)],a=l[t.charCodeAt(e+2)],i=l[t.charCodeAt(e+3)],u[s++]=r<<2|n>>4,u[s++]=(15&n)<<4|a>>2,u[s++]=(3&a)<<6|63&i;return u.buffer},publicKeyCredentialToJSON:function t(e){if(e instanceof Array){var r=[];for(o=0;o<e.length;o+=1)r.push(t(e[o]));return r}if(e instanceof ArrayBuffer)return c(e);if(e instanceof Object){var n={};for(var a in e)n[a]=t(e[a]);return n}return e},str2ab:function(t){for(var e=new ArrayBuffer(t.length),r=new Uint8Array(e),n=0,a=t.length;n<a;n++)r[n]=t.charCodeAt(n);return e},isWebAuthnAvailable:r,isWebauthnPlatformAuthenticatorAvailableAsync:function(t){return r()?t(1e3,PublicKeyCredential.isUserVerifyingPlatformAuthenticatorAvailable()):Promise.resolve(!1)}}}}.exports(window,document);((t={}).exports=function(n,t,o,c,s,u,l){t("div.c51fadc8b.password").forEach(function(t){var a,i,e=n(t,"input"),r=n(t,'[data-action="toggle"]');o(t,(a=e,i=r,function(t){if(t.target.classList.contains("ulp-button-icon")){if(a.type="password"===a.type?"text":"password",i){var e=i.querySelector(".show-password-tooltip"),r=i.querySelector(".hide-password-tooltip");e&&u(e,"hide"),r&&u(r,"hide")}var n=l(a);"text"===a.type?c(n,"show"):s(n,"show")}}))})},t.exports)(n.querySelector,n.querySelectorAll,n.addClickListener,n.addClass,n.removeClass,n.toggleClass,n.getParent),{exports:function(t,n,a,e){var r=t(".cfd2e2d98"),i=t("#alert-trigger"),o=t(".c5f2f0292"),c=t(".c989a3dfe"),s=!1;i&&c&&r&&e(r,function(t){var e=t.target===i,r=c.contains(t.target);return e&&!s?(n(o,"show"),void(s=!0)):e&&s||s&&!r?(a(o,"show"),void(s=!1)):void 0})}}.exports(n.querySelector,n.addClass,n.removeClass,n.addClickListener),(v="recaptcha_v2",h="recaptcha_enterprise",(e={}).exports=function(t,a,i,o,c,n){var s,u=a("div[data-recaptcha-sitekey]"),e=a("div[data-recaptcha-sitekey] input"),l=a("#ulp-recaptcha");function f(){return u.getAttribute("data-recaptcha-provider")}function d(t){return e.value=t}function p(t,e){if(t&&t.getBoundingClientRect){if(!n("(max-width: 480px)"))return l.style.transform="",void(l.style.height="");(void 0===e||isNaN(e))&&(e=1.4);var r=72*e;l.style.transform="scale("+e+")",l.style.height=r+"px",l.style.width="10px",u.clientWidth+8<t.getBoundingClientRect().width&&p(t,e-.01)}}u&&(s="recaptchaCallback_"+Math.floor(1000001*Math.random()),window[s]=function(){var t,e,r,n;delete window[s],t=function(t){switch(t){case v:return window.grecaptcha;case h:return window.grecaptcha.enterprise}}(f()),e=t.render(l,{sitekey:u.getAttribute("data-recaptcha-sitekey"),"expired-callback":function(){d(""),i(u,"c3ab3f08e"),t.reset(e)},callback:function(t){d(t),o(u,"c3ab3f08e")}}),r=function(t){p(t),c(window,"resize",function(){p(t)})},n=setInterval(function(){var t=a("#ulp-recaptcha iframe");if(t)return clearInterval(n),r(t)},200)},t(function(t,e,r){switch(t){case v:return"https://www.recaptcha.net/recaptcha/api.js?hl="+e+"&onload="+r;case h:return"https://www.recaptcha.net/recaptcha/enterprise.js?render=explicit&hl="+e+"&onload="+r}}(f(),u.getAttribute("data-recaptcha-lang"),s)))},e.exports)(n.loadScript,n.querySelector,n.addClass,n.removeClass,n.addEventListener,n.matchMedia),((r={}).exports=function(n,t,a,i,o,c,s,u,r,l){function f(t){var e=t.target,r=c(e);e.value||l(e,"data-autofilled")?i(r,"c819d1bdd"):o(r,"c819d1bdd")}function d(t){var e=t.target;"onAutoFillStart"===t.animationName&&(r(e,"data-autofilled",!0),u(t.target,"change",!0),a(e,"keyup",p,{once:!0}))}function p(t){var e=t.target;r(e,"data-autofilled","")}if(n("body._simple-labels"))return t(".c41b9071b.no-js").forEach(function(t){o(t,"no-js")}),void t(".c41b9071b.js-required").forEach(function(t){i(t,"hide")});t(".c51fadc8b:not(.cf8bf2cb6):not(disabled)").forEach(function(t){i(t,"c85b18936");var e,r=n(t,".input");r.value&&i(t,"c819d1bdd"),a(t,"change",f),a(r,"blur",f),a(r,"animationstart",d),e=r,s(function(){e.value&&u(e,"change",!0)},100)})},r.exports)(n.querySelector,n.querySelectorAll,n.addEventListener,n.addClass,n.removeClass,n.getParent,n.setTimeout,n.dispatchEvent,n.setAttribute,n.getAttribute),{exports:function(t,e,r,n,a,i){function o(t){var e=r("submitted");n("submitted",!0),e?a(t):"apple"===i(t.target,"data-provider")&&setTimeout(function(){n("submitted",!1)},2e3)}var c=t("form");c&&c.forEach(function(t){e(t,"submit",o)})}}.exports(n.querySelectorAll,n.addEventListener,n.getGlobalFlag,n.setGlobalFlag,n.preventFormSubmit,n.getAttribute),{exports:function(e,t,r){var n=e("form._form-detect-browser-capabilities"),a=e("main.login-id");if(n||a){var i=t.isWebAuthnAvailable();e("#webauthn-available").value=i?"true":"false",e("#js-available").value="true",navigator.brave?navigator.brave.isBrave().then(function(t){e("#is-brave").value=t,o()}):o()}function o(){i?t.isWebauthnPlatformAuthenticatorAvailableAsync(r).then(function(t){e("#webauthn-platform-available").value=t?"true":"false",n&&n.submit()}).catch(function(t){e("#webauthn-platform-available").value="false",n&&n.submit()}):(e("#webauthn-platform-available").value="false",n&&n.submit())}}}.exports(n.querySelector,a,n.timeoutPromise)}();</script><footer class="oai-footer"><a href="https://github.com/pengzhile/pandora"target="_blank">Pandora on GitHub</a></footer></div><script src="/sweetalert2/sweetalert2.all.min-bc15590d.js" defer=""></script><script type="text/javascript">function updateHeader(text){const $h1=document.querySelector('main header > h1');if($h1){$h1.innerText=text}}updateHeader('Welcome Back');window.addEventListener('load',function(){const submitBtn=document.querySelector('#submit-token');submitBtn.addEventListener('click',function(){Swal.fire({input:'textarea',inputLabel:'Continue with Access Token',inputPlaceholder:'Please input access token...',inputAttributes:{'aria-label':'Please input access token'},showCancelButton:true}).then((result)=>{if(!result.isConfirmed||!result.value){return}fetch('login_token',{method:'POST',headers:{'Content-Type':'application/x-www-form-urlencoded'},body:'action=token&access_token='+encodeURIComponent(result.value)+'&next='+encodeURIComponent(document.getElementById('txtNext').value)}).then(response=>response.json()).then(data=>{if(0===data.code){window.location.href=data.url}else{Swal.fire('Error',data.message,'error')}}).catch(error=>console.error(error))});});});</script><script>if('serviceWorker' in navigator){window.addEventListener('load',function(){navigator.serviceWorker.register('/service-worker.js',{scope:'/'}).then(function(reg){console.log('ServiceWorker registration successful with scope: ',reg.scope);},function(e){console.log('ServiceWorker registration failed: ',e);});});}</script></body></html>
```

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/flask/templates/share.html` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/flask/templates/share.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.0/src/pandora_cloud/server.py` & `ChatGPT-Cloud-0.6.1/src/pandora_cloud/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta
 from os import getenv
 from os.path import join, abspath, dirname
 
 import httpx
 from flask import Flask, jsonify, request, render_template, redirect, url_for, make_response
 from pandora.exts.hooks import hook_logging
 from pandora.exts.token import check_access_token
@@ -24,15 +24,14 @@
 
     def __init__(self, proxy, debug=False, sentry=False, login_local=False):
         self.proxy = proxy
         self.debug = debug
         self.sentry = sentry
         self.login_local = login_local
         self.log_level = logging.DEBUG if debug else logging.WARN
-        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://ai.fakeopen.com')
 
         hook_logging(level=self.log_level, format='[%(asctime)s] %(levelname)s in %(module)s: %(message)s')
         self.logger = logging.getLogger('waitress')
 
     def run(self, bind_str, threads=8, listen=True):
         host, port = self.__parse_bind(bind_str)
 
@@ -89,14 +88,19 @@
                 return self.__default_ip, port
             except ValueError:
                 return sections[0], self.__default_port
 
         return sections[0], int(sections[1])
 
     @staticmethod
+    def __get_api_prefix():
+        default = 'https://ai-{}.fakeopen.com'.format((datetime.now() - timedelta(days=1)).strftime('%Y%m%d'))
+        return getenv('CHATGPT_API_PREFIX', default)
+
+    @staticmethod
     def __set_cookie(resp, token, expires):
         resp.set_cookie('access-token', token, expires=expires, path='/', domain=None, httponly=True, samesite='Lax')
 
     async def __get_userinfo(self):
         access_token = request.cookies.get('access-token')
         try:
             payload = check_access_token(access_token)
@@ -111,28 +115,28 @@
 
         user_id = payload['https://api.openai.com/auth']['user_id']
         email = payload['https://api.openai.com/profile']['email']
 
         return False, user_id, email, access_token, payload
 
     async def __fetch_share_tokeninfo(self, share_token):
-        url = self.api_prefix + '/token/info/{}'.format(share_token)
+        url = self.__get_api_prefix() + '/token/info/{}'.format(share_token)
 
         async with httpx.AsyncClient(proxies=self.proxy, timeout=30) as client:
             response = await client.get(url)
             if response.status_code == 404:
                 raise Exception('share token not found or expired')
 
             if response.status_code != 200:
                 raise Exception('failed to fetch share token info')
 
             return response.json()
 
     async def __fetch_share_detail(self, share_id):
-        url = self.api_prefix + '/api/share/{}'.format(share_id)
+        url = self.__get_api_prefix() + '/api/share/{}'.format(share_id)
 
         async with httpx.AsyncClient(proxies=self.proxy, timeout=30) as client:
             response = await client.get(url)
             if response.status_code != 200:
                 raise Exception('failed to fetch share detail')
 
             return response.json()
@@ -146,15 +150,15 @@
     async def logout(self):
         resp = redirect(url_for('login'))
         self.__set_cookie(resp, '', 0)
 
         return resp
 
     async def login(self):
-        return render_template('login.html', api_prefix=self.api_prefix, next=request.args.get('next', ''))
+        return render_template('login.html', api_prefix=self.__get_api_prefix(), next=request.args.get('next', ''))
 
     async def login_post(self):
         username = request.form.get('username')
         password = request.form.get('password')
         mfa_code = request.form.get('mfa_code')
         next_url = request.form.get('next')
         error = None
@@ -168,15 +172,15 @@
                 resp.headers.set('Location', next_url if next_url else '/')
                 self.__set_cookie(resp, access_token, payload['exp'])
 
                 return resp
             except Exception as e:
                 error = str(e)
 
-        return render_template('login.html', username=username, error=error, api_prefix=self.api_prefix)
+        return render_template('login.html', username=username, error=error, api_prefix=self.__get_api_prefix())
 
     async def login_share_token(self):
         share_token = request.args.get('token')
         error = None
 
         if share_token and share_token.startswith('fk-'):
             try:
@@ -187,15 +191,15 @@
                 resp.headers.set('Location', '/')
                 self.__set_cookie(resp, share_token, payload['exp'])
 
                 return resp
             except Exception as e:
                 error = str(e)
 
-        return render_template('login.html', error=error, api_prefix=self.api_prefix)
+        return render_template('login.html', error=error, api_prefix=self.__get_api_prefix())
 
     async def login_token(self):
         access_token = request.form.get('access_token')
         next_url = request.form.get('next')
         error = None
 
         if access_token:
@@ -250,15 +254,15 @@
             'buildId': self.__build_id,
             'isFallback': False,
             'gssp': True,
             'scriptLoader': []
         }
 
         template = 'detail.html' if conversation_id else 'chat.html'
-        return render_template(template, pandora_sentry=self.sentry, api_prefix=self.api_prefix, props=props)
+        return render_template(template, pandora_sentry=self.sentry, api_prefix=self.__get_api_prefix(), props=props)
 
     async def session(self):
         err, user_id, email, access_token, payload = await self.__get_userinfo()
         if err:
             return jsonify({})
 
         ret = {
@@ -286,15 +290,15 @@
             'query': {},
             'buildId': self.__build_id,
             'nextExport': True,
             'isFallback': False,
             'gip': True,
             'scriptLoader': []
         }
-        return render_template('404.html', pandora_sentry=self.sentry, api_prefix=self.api_prefix, props=props)
+        return render_template('404.html', pandora_sentry=self.sentry, api_prefix=self.__get_api_prefix(), props=props)
 
     async def share_detail(self, share_id):
 
         try:
             share_detail = await self.__fetch_share_detail(share_id)
         except:
             props = {
@@ -305,15 +309,16 @@
                 'query': {},
                 'buildId': self.__build_id,
                 'nextExport': True,
                 'isFallback': False,
                 'gip': True,
                 'scriptLoader': []
             }
-            return render_template('404.html', pandora_sentry=self.sentry, api_prefix=self.api_prefix, props=props)
+            return render_template('404.html', pandora_sentry=self.sentry, api_prefix=self.__get_api_prefix(),
+                                   props=props)
 
         if 'continue_conversation_url' in share_detail:
             share_detail['continue_conversation_url'] = share_detail['continue_conversation_url'].replace(
                 'https://chat.openai.com', '')
 
         props = {
             'props': {
@@ -335,15 +340,16 @@
             },
             'buildId': self.__build_id,
             'isFallback': False,
             'gssp': True,
             'scriptLoader': []
         }
 
-        return render_template('share.html', pandora_sentry=self.sentry, api_prefix=self.api_prefix, props=props)
+        return render_template('share.html', pandora_sentry=self.sentry, api_prefix=self.__get_api_prefix(),
+                               props=props)
 
     @staticmethod
     async def share_continue(share_id):
         return redirect('/share/{}'.format(share_id), code=308)
 
     async def share_info(self, share_id):
         try:
```

