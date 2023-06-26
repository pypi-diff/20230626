# Comparing `tmp/serialtools-0.2.1.tar.gz` & `tmp/serialtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.2.1.tar` & `serialtools-0.3.0.tar`

### file list

```diff
@@ -1,100 +1,104 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.2.1/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.2.1/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.2.1/README.md
--rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      985 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.2.1/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-06-23 15:23:14.649044 serialtools-0.2.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-06-23 15:23:15.989031 serialtools-0.2.1/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-06-23 15:23:14.649044 serialtools-0.2.1/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-06-23 15:23:15.992364 serialtools-0.2.1/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-06-23 15:23:15.985698 serialtools-0.2.1/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.2.1/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    26556 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/genindex.html
--rw-r--r--   0        0        0    14126 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/index.html
--rw-r--r--   0        0        0    10059 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/modules.html
--rw-r--r--   0        0        0     1253 2023-06-23 15:23:16.025697 serialtools-0.2.1/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6583 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4797 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/search.html
--rw-r--r--   0        0        0    22432 2023-06-23 15:23:16.025697 serialtools-0.2.1/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14594 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12182 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10486 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    10684 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    44788 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    68246 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    33114 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    30858 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.2.1/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.2.1/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.2.1/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-06-23 15:24:03.778562 serialtools-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      985 2023-06-23 15:23:13.509056 serialtools-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-06-23 15:23:13.442390 serialtools-0.2.1/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-06-23 15:23:13.442390 serialtools-0.2.1/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-06-23 15:23:13.445723 serialtools-0.2.1/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      302 2023-06-23 15:23:13.442390 serialtools-0.2.1/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-06-23 15:23:13.445723 serialtools-0.2.1/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-06-23 15:23:13.445723 serialtools-0.2.1/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-06-23 15:23:13.445723 serialtools-0.2.1/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-06-23 15:23:13.442390 serialtools-0.2.1/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-06-23 15:23:13.442390 serialtools-0.2.1/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.2.1/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.2.1/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.2.1/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.2.1/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.2.1/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-06-23 15:24:03.778562 serialtools-0.2.1/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1448 2023-06-23 15:23:13.439056 serialtools-0.2.1/src/serialtools/__main__.py
--rw-r--r--   0        0        0      289 2023-06-23 15:23:13.442390 serialtools-0.2.1/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-23 15:23:13.442390 serialtools-0.2.1/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1346 2023-06-23 15:23:13.439056 serialtools-0.2.1/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0      880 2023-06-23 15:23:13.442390 serialtools-0.2.1/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     6045 2023-06-23 15:24:03.778562 serialtools-0.2.1/src/serialtools/bus.py
--rw-r--r--   0        0        0    13062 2023-06-23 15:23:13.439056 serialtools-0.2.1/src/serialtools/database.py
--rw-r--r--   0        0        0     5027 2023-06-23 15:23:13.439056 serialtools-0.2.1/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.2.1/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.2.1/tox.ini
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.3.0/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.3.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.3.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.3.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-06-26 12:52:22.152933 serialtools-0.3.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-06-26 12:52:23.526288 serialtools-0.3.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-06-26 12:52:22.152933 serialtools-0.3.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-06-26 12:52:23.529621 serialtools-0.3.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-06-26 12:52:23.522954 serialtools-0.3.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    28033 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    15719 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    10407 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1318 2023-06-26 12:52:23.542955 serialtools-0.3.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6959 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4930 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    24058 2023-06-26 12:52:23.539621 serialtools-0.3.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14727 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12315 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10619 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    13490 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.apps.rawsplit.html
+-rw-r--r--   0        0        0    10817 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    44921 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    71095 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    34482 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    31448 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1014 2023-06-26 12:52:21.286253 serialtools-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      163 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.rawsplit.rst
+-rw-r--r--   0        0        0      302 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.3.0/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.3.0/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.3.0/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.3.0/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.3.0/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-06-26 12:53:34.554064 serialtools-0.3.0/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      345 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-26 12:52:21.222918 serialtools-0.3.0/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1346 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0     1369 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/rawsplit.py
+-rw-r--r--   0        0        0      880 2023-06-26 12:52:21.222918 serialtools-0.3.0/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     6136 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/bus.py
+-rw-r--r--   0        0        0    13898 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/database.py
+-rw-r--r--   0        0        0     5193 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.3.0/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.3.0/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.3.0/PKG-INFO
```

### Comparing `serialtools-0.2.1/LICENSE` & `serialtools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/Makefile` & `serialtools-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_sources/index.rst.txt` & `serialtools-0.3.0/docs/build/html/_sources/index.rst.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. toctree::
    :maxdepth: 2
 
    serialtools
    serialtools.apps.decode
    serialtools.apps.dump
    serialtools.apps.__init__
+   serialtools.apps.rawsplit
    serialtools.apps.send
    serialtools.bus
    serialtools.database
    serialtools.database_config
    serialtools.__main__
```

### Comparing `serialtools-0.2.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.3.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/basic.css` & `serialtools-0.3.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/badge_only.css` & `serialtools-0.3.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/css/theme.css` & `serialtools-0.3.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/doctools.js` & `serialtools-0.3.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/jquery.js` & `serialtools-0.3.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/js/badge_only.js` & `serialtools-0.3.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.3.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.3.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/js/theme.js` & `serialtools-0.3.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/language_data.js` & `serialtools-0.3.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/pygments.css` & `serialtools-0.3.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/searchtools.js` & `serialtools-0.3.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.3.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/build/html/genindex.html` & `serialtools-0.3.0/docs/build/html/genindex.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.2.1 documentation</title>
+  <title>Index &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -31,28 +31,29 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.html">serialtools package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
@@ -106,27 +107,33 @@
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.html#serialtools.apps.add_arguments">add_arguments() (in module serialtools.apps)</a>
 
       <ul>
         <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.add_arguments">(in module serialtools.apps.decode)</a>
 </li>
+        <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_arguments">(in module serialtools.apps.rawsplit)</a>
+</li>
         <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.add_arguments">(serialtools.bus.BusCreator method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.add_parser">add_parser() (in module serialtools.apps.decode)</a>
 
       <ul>
         <li><a href="serialtools.apps.dump.html#serialtools.apps.dump.add_parser">(in module serialtools.apps.dump)</a>
 </li>
+        <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_parser">(in module serialtools.apps.rawsplit)</a>
+</li>
         <li><a href="serialtools.apps.send.html#serialtools.apps.send.add_parser">(in module serialtools.apps.send)</a>
 </li>
       </ul></li>
+      <li><a href="serialtools.database.html#serialtools.database.MessageSpec.ADDRESS">ADDRESS (serialtools.database.MessageSpec attribute)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="B">B</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.baudrate">baudrate (serialtools.bus.BusCreator attribute)</a>
@@ -182,14 +189,16 @@
       <li><a href="serialtools.database.html#serialtools.database.Database">Database (class in serialtools.database)</a>
 </li>
       <li><a href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator">DatabaseCreator (class in serialtools.database_config)</a>
 </li>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.decode">decode() (in module serialtools.apps.decode)</a>
 
       <ul>
+        <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.decode">(in module serialtools.apps.rawsplit)</a>
+</li>
         <li><a href="serialtools.database.html#serialtools.database.Database.decode">(serialtools.database.Database method)</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database_config.html#serialtools.database_config.Param.defined_parameters">defined_parameters (serialtools.database_config.Param attribute)</a>
 </li>
@@ -214,15 +223,19 @@
       <li><a href="serialtools.database.html#serialtools.database.Database.endianness">endianness (serialtools.database.Database attribute)</a>
 
       <ul>
         <li><a href="serialtools.database_config.html#serialtools.database_config.DatabaseCreator.endianness">(serialtools.database_config.DatabaseCreator attribute)</a>
 </li>
       </ul></li>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.error">error() (in module serialtools.apps.decode)</a>
+
+      <ul>
+        <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.error">(in module serialtools.apps.rawsplit)</a>
 </li>
+      </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="F">F</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Type.FLOAT">FLOAT (serialtools.database.Type attribute)</a>
@@ -306,39 +319,47 @@
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.main">main() (in module serialtools.apps.decode)</a>
 
       <ul>
         <li><a href="serialtools.apps.dump.html#serialtools.apps.dump.main">(in module serialtools.apps.dump)</a>
 </li>
+        <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.main">(in module serialtools.apps.rawsplit)</a>
+</li>
         <li><a href="serialtools.apps.send.html#serialtools.apps.send.main">(in module serialtools.apps.send)</a>
 </li>
       </ul></li>
       <li><a href="serialtools.database.html#serialtools.database.Message">Message (class in serialtools.database)</a>
 
       <ul>
         <li><a href="serialtools.database_config.html#serialtools.database_config.Message">(class in serialtools.database_config)</a>
 </li>
       </ul></li>
       <li><a href="serialtools.database_config.html#serialtools.database_config.Message.message">message (serialtools.database_config.Message attribute)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.Database.message_spec">message_spec (serialtools.database.Database attribute)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.MessageSpec">MessageSpec (class in serialtools.database)</a>
+</li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li>
     module
 
       <ul>
         <li><a href="serialtools.html#module-serialtools">serialtools</a>
 </li>
         <li><a href="serialtools.apps.html#module-serialtools.apps">serialtools.apps</a>
 </li>
         <li><a href="serialtools.apps.decode.html#module-serialtools.apps.decode">serialtools.apps.decode</a>
 </li>
         <li><a href="serialtools.apps.dump.html#module-serialtools.apps.dump">serialtools.apps.dump</a>
 </li>
+        <li><a href="serialtools.apps.rawsplit.html#module-serialtools.apps.rawsplit">serialtools.apps.rawsplit</a>
+</li>
         <li><a href="serialtools.apps.send.html#module-serialtools.apps.send">serialtools.apps.send</a>
 </li>
         <li><a href="serialtools.bus.html#module-serialtools.bus">serialtools.bus</a>
 </li>
         <li><a href="serialtools.database.html#module-serialtools.database">serialtools.database</a>
 </li>
         <li><a href="serialtools.database_config.html#module-serialtools.database_config">serialtools.database_config</a>
@@ -443,14 +464,21 @@
     serialtools.apps.dump
 
       <ul>
         <li><a href="serialtools.apps.dump.html#module-serialtools.apps.dump">module</a>
 </li>
       </ul></li>
       <li>
+    serialtools.apps.rawsplit
+
+      <ul>
+        <li><a href="serialtools.apps.rawsplit.html#module-serialtools.apps.rawsplit">module</a>
+</li>
+      </ul></li>
+      <li>
     serialtools.apps.send
 
       <ul>
         <li><a href="serialtools.apps.send.html#module-serialtools.apps.send">module</a>
 </li>
       </ul></li>
   </ul></td>
```

#### html2text {}

```diff
@@ -3,35 +3,41 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * Index
 ===============================================================================
 ****** Index ******
 A | B | C | D | E | F | G | I | L | M | P | R | S | T | U | V | W | X
 ***** A *****
-    * add_arguments()_(in_module            * add_parser()_(in_module
-      serialtools.apps)                       serialtools.apps.decode)
-          o (in_module                            o (in_module
-            serialtools.apps.decode)                serialtools.apps.dump)
-          o (serialtools.bus.BusCreator           o (in_module
-            method)                                 serialtools.apps.send)
+                                            * add_parser()_(in_module
+    * add_arguments()_(in_module              serialtools.apps.decode)
+      serialtools.apps)                           o (in_module
+          o (in_module                              serialtools.apps.dump)
+            serialtools.apps.decode)              o (in_module
+          o (in_module                              serialtools.apps.rawsplit)
+            serialtools.apps.rawsplit)            o (in_module
+          o (serialtools.bus.BusCreator             serialtools.apps.send)
+            method)                         * ADDRESS_
+                                              (serialtools.database.MessageSpec
+                                              attribute)
 ***** B *****
     * baudrate_                            * BusCreator_(class_in
       (serialtools.bus.BusCreator            serialtools.bus)
       attribute)                           * bytesize_
     * BIG_                                   (serialtools.bus.BusCreator
       (serialtools.database.Endianness       attribute)
       attribute)                           * ByteSpec_(class_in
@@ -45,30 +51,32 @@
             method)                                     method)
     * cancel_write()_                           * create_args()_
       (serialtools.bus.ReadFromFileBus            (serialtools.bus.BusCreator_method)
       method)                                   * create_bus()_
           o (serialtools.bus.WriteToFileBus       (serialtools.bus.BusCreator_method)
             method)
 ***** D *****
-    * Database_(class_in                       * defined_parameters_
-      serialtools.database)                      (serialtools.database_config.Param
-    * DatabaseCreator_(class_in                  attribute)
-      serialtools.database_config)             * dsrdtr_(serialtools.bus.BusCreator
-    * decode()_(in_module                        attribute)
-      serialtools.apps.decode)                 * dump()_(in_module
-          o (serialtools.database.Database       serialtools.apps.dump)
+    * Database_(class_in
+      serialtools.database)                    * defined_parameters_
+    * DatabaseCreator_(class_in                  (serialtools.database_config.Param
+      serialtools.database_config)               attribute)
+    * decode()_(in_module                      * dsrdtr_(serialtools.bus.BusCreator
+      serialtools.apps.decode)                   attribute)
+          o (in_module                         * dump()_(in_module
+            serialtools.apps.rawsplit)           serialtools.apps.dump)
+          o (serialtools.database.Database
             method)
 ***** E *****
     * encode()_
       (serialtools.database.Database     * endianness_(serialtools.database.Database
       method)                              attribute)
     * encode_range()_                          o (serialtools.database_config.DatabaseCreator
       (serialtools.database.Database             attribute)
       method)                            * error()_(in_module_serialtools.apps.decode)
-    * Endianness_(class_in
+    * Endianness_(class_in                     o (in_module_serialtools.apps.rawsplit)
       serialtools.database)
 ***** F *****
                                                       * format_allowed_values()_
                                                         (serialtools.database.ByteSpec
     * FLOAT_(serialtools.database.Type_attribute)       method)
     * fn_(serialtools.bus.ReadFromFileBus             * format_bytes()_(in_module
       parameter)                                        serialtools.database)
@@ -99,30 +107,34 @@
           o (serialtools.database_config.Param      * integer()_(in_module
             method)                                   serialtools.database_config)
           o (serialtools.database_config.Signal
             method)
 ***** L *****
     * LITTLE_(serialtools.database.Endianness_attribute)
 ***** M *****
-    * main()_(in_module_serialtools.apps.decode)
-          o (in_module_serialtools.apps.dump)
-          o (in_module_serialtools.apps.send)
-    * Message_(class_in_serialtools.database)
-          o (class_in_serialtools.database_config)
-    * message_(serialtools.database_config.Message_attribute)
-    * message_spec_(serialtools.database.Database_attribute)
-    * module
-          o serialtools
-          o serialtools.apps
-          o serialtools.apps.decode
-          o serialtools.apps.dump
-          o serialtools.apps.send
-          o serialtools.bus
-          o serialtools.database
-          o serialtools.database_config
+    * main()_(in_module
+      serialtools.apps.decode)
+          o (in_module
+            serialtools.apps.dump)
+          o (in_module
+            serialtools.apps.rawsplit)         * module
+          o (in_module                               o serialtools
+            serialtools.apps.send)                   o serialtools.apps
+    * Message_(class_in                              o serialtools.apps.decode
+      serialtools.database)                          o serialtools.apps.dump
+          o (class_in                                o serialtools.apps.rawsplit
+            serialtools.database_config)             o serialtools.apps.send
+    * message_                                       o serialtools.bus
+      (serialtools.database_config.Message           o serialtools.database
+      attribute)                                     o serialtools.database_config
+    * message_spec_
+      (serialtools.database.Database
+      attribute)
+    * MessageSpec_(class_in
+      serialtools.database)
 ***** P *****
     * Param_(class_in                        * parser_
       serialtools.database_config)             (serialtools.database_config.Message.init_parser
     * parity_(serialtools.bus.BusCreator       parameter)
       attribute)                                   o (serialtools.database_config.Param.init_parser
     * parse_allowed_values()_                        parameter)
       (serialtools.database_config.Param           o (serialtools.database_config.Signal.init_parser
@@ -141,31 +153,31 @@
     * read_in_other_thread()_                     method)
       (serialtools.database.Reader_method)            o (serialtools.database_config.Param
     * read_msg()_                                       method)
       (serialtools.database.Reader_method)            o (serialtools.database_config.Signal
     * read_n_bytes()_                                   method)
       (serialtools.database.Reader_method)
 ***** S *****
-                                       * serialtools.bus
-    * send()_(in_module                      o module
-      serialtools.apps.send)           * serialtools.database
-    * send_msg()_                            o module
-      (serialtools.database.Reader     * serialtools.database_config
-      method)                                o module
-    * serialtools                      * Signal_(class_in_serialtools.database)
-          o module                           o (class_in
-    * serialtools.apps                         serialtools.database_config)
-          o module                     * signals_(serialtools.database.Database
-    * serialtools.apps.decode            attribute)
-          o module                           o (serialtools.database_config.Signal
-    * serialtools.apps.dump                    attribute)
-          o module                     * stop()_(serialtools.database.Reader
-    * serialtools.apps.send              method)
-          o module                     * stopbits_(serialtools.bus.BusCreator
-                                         attribute)
+    * send()_(in_module                * serialtools.bus
+      serialtools.apps.send)                 o module
+    * send_msg()_                      * serialtools.database
+      (serialtools.database.Reader           o module
+      method)                          * serialtools.database_config
+    * serialtools                            o module
+          o module                     * Signal_(class_in_serialtools.database)
+    * serialtools.apps                       o (class_in
+          o module                             serialtools.database_config)
+    * serialtools.apps.decode          * signals_(serialtools.database.Database
+          o module                       attribute)
+    * serialtools.apps.dump                  o (serialtools.database_config.Signal
+          o module                             attribute)
+    * serialtools.apps.rawsplit        * stop()_(serialtools.database.Reader
+          o module                       method)
+    * serialtools.apps.send            * stopbits_(serialtools.bus.BusCreator
+          o module                       attribute)
 ***** T *****
     * TEXT_(serialtools.database.Type
       attribute)
     * timestamp_                                * Type_(class_in
       (serialtools.bus.ReadFromFileBus            serialtools.database)
       attribute)
           o (serialtools.bus.WriteToFileBus
```

### Comparing `serialtools-0.2.1/docs/build/html/index.html` & `serialtools-0.3.0/docs/build/html/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.2.1 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,28 +33,29 @@
 
           
           
           <a href="#" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.html">serialtools package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
@@ -103,14 +104,22 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.dump.html#serialtools.apps.dump.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.dump.html#serialtools.apps.dump.dump"><code class="docutils literal notranslate"><span class="pre">dump()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.dump.html#serialtools.apps.dump.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_arguments"><code class="docutils literal notranslate"><span class="pre">add_arguments()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.decode"><code class="docutils literal notranslate"><span class="pre">decode()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.error"><code class="docutils literal notranslate"><span class="pre">error()</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.send.html#serialtools.apps.send.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.send.html#serialtools.apps.send.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.apps.send.html#serialtools.apps.send.send"><code class="docutils literal notranslate"><span class="pre">send()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a><ul>
@@ -122,14 +131,15 @@
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database"><code class="docutils literal notranslate"><span class="pre">Database</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a><ul>
```

#### html2text {}

```diff
@@ -4,19 +4,20 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * Welcome to serialtoolsâ documentation!
     * View_page_source
@@ -33,14 +34,20 @@
           o decode()
           o error()
           o main()
     * serialtools.apps.dump_module
           o add_parser()
           o dump()
           o main()
+    * serialtools.apps.rawsplit_module
+          o add_arguments()
+          o add_parser()
+          o decode()
+          o error()
+          o main()
     * serialtools.apps.send_module
           o add_parser()
           o main()
           o send()
     * serialtools.bus_module
           o BusCreator
           o ReadFromFileBus
@@ -48,14 +55,15 @@
           o WriteToFileBus
           o get_timestamp()
     * serialtools.database_module
           o ByteSpec
           o Database
           o Endianness
           o Message
+          o MessageSpec
           o Reader
           o Signal
           o Type
           o format_bytes()
     * serialtools.database_config_module
           o DatabaseCreator
           o Message
```

### Comparing `serialtools-0.2.1/docs/build/html/modules.html` & `serialtools-0.3.0/docs/build/html/modules.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -32,28 +32,29 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.html">serialtools package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
@@ -103,14 +104,15 @@
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database"><code class="docutils literal notranslate"><span class="pre">Database</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a><ul>
```

#### html2text {}

```diff
@@ -3,19 +3,20 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools
     * View_page_source
@@ -34,14 +35,15 @@
                       # WriteToFileBus
                       # get_timestamp()
                 # serialtools.database_module
                       # ByteSpec
                       # Database
                       # Endianness
                       # Message
+                      # MessageSpec
                       # Reader
                       # Signal
                       # Type
                       # format_bytes()
                 # serialtools.database_config_module
                       # DatabaseCreator
                       # Message
```

### Comparing `serialtools-0.2.1/docs/build/html/py-modindex.html` & `serialtools-0.3.0/docs/build/html/py-modindex.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.2.1 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,28 +34,29 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.html">serialtools package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
@@ -112,14 +113,19 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="serialtools.apps.dump.html#module-serialtools.apps.dump"><code class="xref">serialtools.apps.dump</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="serialtools.apps.rawsplit.html#module-serialtools.apps.rawsplit"><code class="xref">serialtools.apps.rawsplit</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="serialtools.apps.send.html#module-serialtools.apps.send"><code class="xref">serialtools.apps.send</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="serialtools.bus.html#module-serialtools.bus"><code class="xref">serialtools.bus</code></a></td><td>
        <em></em></td></tr>
```

#### html2text {}

```diff
@@ -3,19 +3,20 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * Python Module Index
 ===============================================================================
@@ -23,14 +24,15 @@
 s
      
     s
 [-] serialtools
         serialtools.apps
         serialtools.apps.decode
         serialtools.apps.dump
+        serialtools.apps.rawsplit
         serialtools.apps.send
         serialtools.bus
         serialtools.database
         serialtools.database_config
 
 ===============================================================================
 © Copyright 2023, erzo.
```

### Comparing `serialtools-0.2.1/docs/build/html/search.html` & `serialtools-0.3.0/docs/build/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.2.1 documentation</title>
+  <title>Search &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
     
   <!--[if lt IE 9]>
@@ -34,28 +34,29 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.html">serialtools package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
```

#### html2text {}

```diff
@@ -3,19 +3,20 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * Search
 ===============================================================================
```

### Comparing `serialtools-0.2.1/docs/build/html/searchindex.js` & `serialtools-0.3.0/docs/build/html/searchindex.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,429 +1,447 @@
 Search.setIndex({
-    "docnames": ["index", "modules", "serialtools", "serialtools.apps", "serialtools.apps.decode", "serialtools.apps.dump", "serialtools.apps.send", "serialtools.bus", "serialtools.database", "serialtools.database_config"],
-    "filenames": ["index.rst", "modules.rst", "serialtools.rst", "serialtools.apps.rst", "serialtools.apps.decode.rst", "serialtools.apps.dump.rst", "serialtools.apps.send.rst", "serialtools.bus.rst", "serialtools.database.rst", "serialtools.database_config.rst"],
-    "titles": ["Welcome to serialtools\u2019 documentation!", "serialtools", "serialtools package", "serialtools.apps package", "serialtools.apps.decode module", "serialtools.apps.dump module", "serialtools.apps.send module", "serialtools.bus module", "serialtools.database module", "serialtools.database_config module"],
+    "docnames": ["index", "modules", "serialtools", "serialtools.apps", "serialtools.apps.decode", "serialtools.apps.dump", "serialtools.apps.rawsplit", "serialtools.apps.send", "serialtools.bus", "serialtools.database", "serialtools.database_config"],
+    "filenames": ["index.rst", "modules.rst", "serialtools.rst", "serialtools.apps.rst", "serialtools.apps.decode.rst", "serialtools.apps.dump.rst", "serialtools.apps.rawsplit.rst", "serialtools.apps.send.rst", "serialtools.bus.rst", "serialtools.database.rst", "serialtools.database_config.rst"],
+    "titles": ["Welcome to serialtools\u2019 documentation!", "serialtools", "serialtools package", "serialtools.apps package", "serialtools.apps.decode module", "serialtools.apps.dump module", "serialtools.apps.rawsplit module", "serialtools.apps.send module", "serialtools.bus module", "serialtools.database module", "serialtools.database_config module"],
     "terms": {
-        "warn": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+        "warn": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
         "index": 0,
         "modul": [0, 1],
         "search": 0,
         "page": 0,
         "packag": [0, 1],
         "subpackag": [0, 1],
         "app": [0, 1, 2],
         "submodul": [0, 1],
-        "content": [0, 1, 7],
-        "bu": [0, 1, 2, 4, 5, 6, 8],
-        "buscreat": [0, 1, 2, 7],
-        "readfromfilebu": [0, 1, 2, 4, 5, 7, 8],
-        "readfromparameterbu": [0, 1, 2, 7],
-        "writetofilebu": [0, 1, 2, 4, 5, 7, 8],
-        "get_timestamp": [0, 1, 2, 7],
-        "databas": [0, 1, 2, 4, 9],
-        "bytespec": [0, 1, 2, 8, 9],
-        "endian": [0, 1, 2, 8, 9],
-        "messag": [0, 1, 2, 8, 9],
-        "reader": [0, 1, 2, 8],
-        "signal": [0, 1, 2, 8, 9],
-        "type": [0, 1, 2, 8],
-        "format_byt": [0, 1, 2, 8],
+        "content": [0, 1, 8],
+        "bu": [0, 1, 2, 4, 5, 6, 7, 9],
+        "buscreat": [0, 1, 2, 8],
+        "readfromfilebu": [0, 1, 2, 4, 5, 6, 8, 9],
+        "readfromparameterbu": [0, 1, 2, 8],
+        "writetofilebu": [0, 1, 2, 4, 5, 6, 8, 9],
+        "get_timestamp": [0, 1, 2, 8],
+        "databas": [0, 1, 2, 4, 6, 10],
+        "bytespec": [0, 1, 2, 9, 10],
+        "endian": [0, 1, 2, 9, 10],
+        "messag": [0, 1, 2, 6, 9, 10],
+        "reader": [0, 1, 2, 9],
+        "signal": [0, 1, 2, 9, 10],
+        "type": [0, 1, 2, 9],
+        "format_byt": [0, 1, 2, 9],
         "database_config": [0, 1, 2],
-        "databasecr": [0, 1, 2, 9],
-        "param": [0, 1, 2, 9],
-        "get_databas": [0, 1, 2, 9],
-        "integ": [0, 1, 2, 9],
-        "decod": [0, 2, 3, 8],
-        "add_argu": [0, 2, 3, 4, 7, 9],
-        "add_pars": [0, 2, 3, 4, 5, 6],
-        "error": [0, 2, 3, 4],
-        "main": [0, 2, 3, 4, 5, 6],
-        "dump": [0, 2, 3, 4, 7],
+        "databasecr": [0, 1, 2, 10],
+        "param": [0, 1, 2, 9, 10],
+        "get_databas": [0, 1, 2, 10],
+        "integ": [0, 1, 2, 10],
+        "decod": [0, 2, 3, 6, 9],
+        "add_argu": [0, 2, 3, 4, 6, 8, 10],
+        "add_pars": [0, 2, 3, 4, 5, 6, 7],
+        "error": [0, 2, 3, 4, 6],
+        "main": [0, 2, 3, 4, 5, 6, 7],
+        "dump": [0, 2, 3, 4, 8],
         "send": [0, 2, 3],
-        "baudrat": [2, 7],
-        "bytes": [2, 7],
-        "create_bu": [2, 7],
-        "dsrdtr": [2, 7],
-        "pariti": [2, 7],
-        "port": [2, 7],
-        "rtsct": [2, 7],
-        "stopbit": [2, 7],
-        "virtual": [2, 7],
-        "vport": [2, 7],
-        "xonxoff": [2, 7],
-        "cancel_read": [2, 7],
-        "cancel_writ": [2, 7],
-        "close": [2, 7],
-        "read": [2, 4, 5, 7, 8],
-        "timestamp": [2, 7, 8],
-        "write": [2, 6, 7],
-        "format_allowed_valu": [2, 8],
-        "get_length": [2, 8],
-        "encod": [2, 8],
-        "encode_rang": [2, 8],
-        "get_endianness_fmt": [2, 8],
-        "get_sign": [2, 8],
-        "get_start_bit": [2, 8],
-        "big": [2, 8],
-        "littl": [2, 8],
-        "format": [2, 7, 8],
-        "format_raw": [2, 8],
-        "format_timestamp": [2, 8],
-        "ignore_bytes_between_messag": [2, 8],
-        "read_byt": [2, 8],
-        "read_in_other_thread": [2, 8],
-        "read_msg": [2, 8],
-        "read_n_byt": [2, 8],
-        "stop": [2, 8],
-        "get_bitstruct_fmt": [2, 8],
-        "bool": [2, 7, 8],
-        "float": [2, 8],
-        "int": [2, 5, 7, 8, 9],
-        "text": [2, 8],
-        "uint": [2, 8],
-        "get": [2, 7, 8, 9],
-        "word_length_in_bit": [2, 8, 9],
-        "init_pars": [2, 9],
-        "run_pars": [2, 9],
-        "defined_paramet": [2, 9],
-        "parse_allowed_valu": [2, 9],
+        "baudrat": [2, 8],
+        "bytes": [2, 8],
+        "create_bu": [2, 8],
+        "dsrdtr": [2, 8],
+        "pariti": [2, 8],
+        "port": [2, 8],
+        "rtsct": [2, 8],
+        "stopbit": [2, 8],
+        "virtual": [2, 8],
+        "vport": [2, 8],
+        "xonxoff": [2, 8],
+        "cancel_read": [2, 8],
+        "cancel_writ": [2, 8],
+        "close": [2, 8],
+        "read": [2, 4, 5, 8, 9],
+        "timestamp": [2, 8, 9],
+        "write": [2, 7, 8],
+        "format_allowed_valu": [2, 9],
+        "get_length": [2, 9],
+        "encod": [2, 9],
+        "encode_rang": [2, 9],
+        "get_endianness_fmt": [2, 9],
+        "get_sign": [2, 9],
+        "get_start_bit": [2, 9],
+        "big": [2, 9],
+        "littl": [2, 9],
+        "format": [2, 8, 9],
+        "format_raw": [2, 9],
+        "format_timestamp": [2, 9],
+        "ignore_bytes_between_messag": [2, 9],
+        "read_byt": [2, 9],
+        "read_in_other_thread": [2, 9],
+        "read_msg": [2, 9],
+        "read_n_byt": [2, 9],
+        "stop": [2, 9],
+        "get_bitstruct_fmt": [2, 9],
+        "bool": [2, 8, 9, 10],
+        "float": [2, 9],
+        "int": [2, 5, 8, 9, 10],
+        "text": [2, 9],
+        "uint": [2, 9],
+        "get": [2, 8, 9, 10],
+        "word_length_in_bit": [2, 9, 10],
+        "init_pars": [2, 10],
+        "run_pars": [2, 10],
+        "defined_paramet": [2, 10],
+        "parse_allowed_valu": [2, 10],
         "tool": 2,
         "work": 2,
-        "serial": [2, 4, 5, 6, 7, 8],
-        "parser": [3, 4, 7, 9],
-        "argumentpars": [3, 4, 7, 9],
-        "none": [3, 4, 5, 6, 7, 8, 9],
-        "hex": [4, 5, 6, 7],
-        "valu": [4, 5, 6, 7, 8, 9],
-        "from": [4, 5, 8],
-        "output": [4, 7],
-        "subpars": [4, 5, 6],
-        "argpars": [4, 5, 6],
-        "_subparsersact": [4, 5, 6],
-        "ani": [4, 5, 6],
-        "db": [4, 8, 9],
-        "file": [4, 5, 7, 8, 9],
-        "textio": [4, 5, 7],
-        "msg": [4, 6, 8],
-        "str": [4, 6, 7, 8, 9],
-        "noreturn": 4,
-        "arg": [4, 5, 6, 7, 9],
-        "namespac": [4, 5, 6, 7, 9],
-        "break_time_m": [5, 7],
+        "serial": [2, 4, 5, 6, 7, 8, 9],
+        "parser": [3, 4, 6, 8, 10],
+        "argumentpars": [3, 4, 6, 8, 10],
+        "none": [3, 4, 5, 6, 7, 8, 9, 10],
+        "hex": [4, 5, 7, 8],
+        "valu": [4, 5, 7, 8, 9, 10],
+        "from": [4, 5, 9],
+        "output": [4, 8],
+        "subpars": [4, 5, 6, 7],
+        "argpars": [4, 5, 6, 7],
+        "_subparsersact": [4, 5, 6, 7],
+        "ani": [4, 5, 6, 7],
+        "db": [4, 6, 9, 10],
+        "file": [4, 5, 6, 8, 9, 10],
+        "textio": [4, 5, 6, 8],
+        "msg": [4, 6, 7, 9],
+        "str": [4, 6, 7, 8, 9, 10],
+        "noreturn": [4, 6],
+        "arg": [4, 5, 6, 7, 8, 10],
+        "namespac": [4, 5, 6, 7, 8, 10],
+        "break_time_m": [5, 8],
         "100": 5,
-        "class": [7, 8, 9],
-        "base": [7, 8, 9],
-        "object": [7, 8, 9],
-        "rx_onli": 7,
-        "fals": 7,
-        "each": [7, 8, 9],
-        "instanc": [7, 8, 9],
-        "thi": [7, 8, 9],
-        "repres": [7, 8, 9],
-        "set": [7, 8, 9],
-        "which": [7, 8, 9],
-        "can": [7, 8, 9],
-        "chang": [0, 7, 8, 9],
-        "config": [7, 8, 9],
-        "implement": [7, 8, 9],
-        "descriptor": [7, 8, 9],
-        "protocol": [7, 8, 9],
-        "return": [7, 8, 9],
-        "an": [7, 8, 9],
-        "i": [7, 8, 9],
-        "access": [7, 8, 9],
-        "attribut": [7, 8, 9],
-        "If": [7, 8, 9],
-        "you": [7, 8, 9],
-        "want": [7, 8, 9],
-        "need": [7, 8, 9],
-        "fn": 7,
-        "paramet": [7, 9],
-        "name": [7, 8],
-        "contain": [7, 8],
-        "data": [7, 8],
-        "separ": 7,
-        "space": 7,
-        "option": 7,
-        "line": 7,
-        "start": [7, 8],
-        "time": 7,
-        "stamp": 7,
-        "parenthes": 7,
-        "n": [7, 8],
-        "byte": [7, 8, 9],
-        "datetim": [7, 8],
-        "f": [7, 8],
-        "length": [8, 9],
-        "allowed_valu": [8, 9],
-        "sequenc": [8, 9],
-        "paramref": 8,
-        "either": 8,
-        "number": 8,
-        "previou": 8,
-        "spec": 8,
-        "specifi": 8,
-        "map": 8,
-        "message_spec": [2, 8],
-        "8": 8,
-        "address": 8,
-        "dict": [8, 9],
-        "length_in_byt": 8,
-        "callabl": 8,
-        "all": 8,
-        "ar": 8,
-        "complet": 8,
-        "within": 8,
-        "given": 8,
-        "rang": 8,
-        "qualnam": 8,
-        "1": 8,
-        "boundari": 8,
-        "enum": 8,
-        "2": 8,
-        "iter": 8,
-        "callback": 8,
-        "bit": 8,
-        "startbit": 8,
-        "0": 8,
-        "scale": 8,
-        "offset": 8,
-        "unit": 8,
-        "The": [8, 9],
-        "e": 8,
-        "g": 8,
-        "us": [8, 9],
-        "request": 8,
-        "batteri": 8,
-        "size": 8,
-        "default": [8, 9],
-        "word": 8,
-        "identifi": 8,
-        "sever": 8,
-        "smaller": 8,
-        "where": 8,
-        "insid": 8,
-        "A": [8, 9],
-        "factor": 8,
-        "multipli": 8,
-        "raw": 8,
-        "receiv": 8,
-        "order": 8,
-        "summand": 8,
-        "ad": 8,
-        "when": 8,
-        "human": 8,
-        "readabl": 8,
-        "first": 8,
-        "cantool": 8,
-        "b": 8,
-        "": 8,
-        "t": 8,
-        "u": 8,
-        "without": 9,
-        "requir": 9,
-        "user": 9,
-        "explicitli": 9,
-        "config_fil": 9,
-        "configfil": 9,
-        "configfileargparsecommand": 9,
-        "add": 9,
-        "argument": 9,
-        "same": 9,
-        "like": 9,
-        "abstract": 9,
-        "method": 9,
-        "must": 9,
-        "subclass": 9,
-        "list": 9,
-        "defin": 9,
-        "command": 9,
-        "val": 9,
+        "class": [8, 9, 10],
+        "base": [8, 9, 10],
+        "object": [8, 9, 10],
+        "rx_onli": 8,
+        "fals": 8,
+        "each": [8, 9, 10],
+        "instanc": [8, 9, 10],
+        "thi": [8, 9, 10],
+        "repres": [8, 9, 10],
+        "set": [8, 9, 10],
+        "which": [8, 9, 10],
+        "can": [8, 9, 10],
+        "chang": [0, 8, 9, 10],
+        "config": [8, 9, 10],
+        "implement": [8, 9, 10],
+        "descriptor": [8, 9, 10],
+        "protocol": [8, 9, 10],
+        "return": [8, 9, 10],
+        "an": [8, 9, 10],
+        "i": [8, 9, 10],
+        "access": [8, 9, 10],
+        "attribut": [8, 9, 10],
+        "If": [8, 9, 10],
+        "you": [8, 9, 10],
+        "want": [8, 9, 10],
+        "need": [8, 9, 10],
+        "fn": 8,
+        "paramet": [8, 10],
+        "name": [8, 9],
+        "contain": [8, 9],
+        "data": [8, 9],
+        "separ": 8,
+        "space": 8,
+        "option": 8,
+        "line": 8,
+        "start": [8, 9],
+        "time": 8,
+        "stamp": 8,
+        "parenthes": 8,
+        "n": [8, 9],
+        "byte": [8, 9, 10],
+        "datetim": [8, 9],
+        "f": [8, 9],
+        "length": [9, 10],
+        "allowed_valu": [9, 10],
+        "sequenc": [9, 10],
+        "paramref": 9,
+        "either": 9,
+        "number": 9,
+        "previou": 9,
+        "spec": 9,
+        "specifi": 9,
+        "map": 9,
+        "message_spec": [2, 9],
+        "8": 9,
+        "address": [2, 9],
+        "dict": [9, 10],
+        "length_in_byt": 9,
+        "callabl": 9,
+        "all": 9,
+        "ar": 9,
+        "complet": 9,
+        "within": 9,
+        "given": 9,
+        "rang": 9,
+        "qualnam": 9,
+        "1": 9,
+        "boundari": 9,
+        "enum": 9,
+        "2": 9,
+        "iter": 9,
+        "callback": 9,
+        "bit": 9,
+        "startbit": 9,
+        "0": 9,
+        "scale": 9,
+        "offset": 9,
+        "unit": 9,
+        "The": [9, 10],
+        "e": 9,
+        "g": 9,
+        "us": [9, 10],
+        "request": 9,
+        "batteri": 9,
+        "size": 9,
+        "default": [9, 10],
+        "word": 9,
+        "identifi": 9,
+        "sever": 9,
+        "smaller": 9,
+        "where": 9,
+        "insid": 9,
+        "A": [9, 10],
+        "factor": 9,
+        "multipli": 9,
+        "raw": 9,
+        "receiv": 9,
+        "order": 9,
+        "summand": 9,
+        "ad": 9,
+        "when": 9,
+        "human": 9,
+        "readabl": 9,
+        "first": 9,
+        "cantool": 9,
+        "b": 9,
+        "": 9,
+        "t": 9,
+        "u": 9,
+        "without": 10,
+        "requir": 10,
+        "user": 10,
+        "explicitli": 10,
+        "config_fil": 10,
+        "configfil": 10,
+        "configfileargparsecommand": 10,
+        "add": 10,
+        "argument": 10,
+        "same": 10,
+        "like": 10,
+        "abstract": 10,
+        "method": 10,
+        "must": 10,
+        "subclass": 10,
+        "list": 10,
+        "defin": 10,
+        "command": 10,
+        "val": 10,
         "sourc": 0,
         "code": 0,
         "bug": 0,
         "tracker": 0,
         "log": 0,
         "pypi": 0,
-        "part": 8,
-        "consist": 8,
-        "itself": 8,
-        "possibl": 8,
-        "create_arg": [2, 7],
-        "send_msg": [2, 8]
+        "part": [6, 9],
+        "consist": [6, 9],
+        "itself": 9,
+        "possibl": 9,
+        "create_arg": [2, 8],
+        "send_msg": [2, 9],
+        "rawsplit": 0,
+        "messagespec": [0, 1, 2, 9, 10],
+        "split": 6,
+        "implicit_address": 9,
+        "require_sign": 10,
+        "true": 10
     },
     "objects": {
         "": [
             [2, 0, 0, "-", "serialtools"]
         ],
         "serialtools": [
             [3, 0, 0, "-", "apps"],
-            [7, 0, 0, "-", "bus"],
-            [8, 0, 0, "-", "database"],
-            [9, 0, 0, "-", "database_config"]
+            [8, 0, 0, "-", "bus"],
+            [9, 0, 0, "-", "database"],
+            [10, 0, 0, "-", "database_config"]
         ],
         "serialtools.apps": [
             [3, 1, 1, "", "add_arguments"],
             [4, 0, 0, "-", "decode"],
             [5, 0, 0, "-", "dump"],
-            [6, 0, 0, "-", "send"]
+            [6, 0, 0, "-", "rawsplit"],
+            [7, 0, 0, "-", "send"]
         ],
         "serialtools.apps.decode": [
             [4, 1, 1, "", "add_arguments"],
             [4, 1, 1, "", "add_parser"],
             [4, 1, 1, "", "decode"],
             [4, 1, 1, "", "error"],
             [4, 1, 1, "", "main"]
         ],
         "serialtools.apps.dump": [
             [5, 1, 1, "", "add_parser"],
             [5, 1, 1, "", "dump"],
             [5, 1, 1, "", "main"]
         ],
-        "serialtools.apps.send": [
+        "serialtools.apps.rawsplit": [
+            [6, 1, 1, "", "add_arguments"],
             [6, 1, 1, "", "add_parser"],
-            [6, 1, 1, "", "main"],
-            [6, 1, 1, "", "send"]
+            [6, 1, 1, "", "decode"],
+            [6, 1, 1, "", "error"],
+            [6, 1, 1, "", "main"]
+        ],
+        "serialtools.apps.send": [
+            [7, 1, 1, "", "add_parser"],
+            [7, 1, 1, "", "main"],
+            [7, 1, 1, "", "send"]
         ],
         "serialtools.bus": [
-            [7, 2, 1, "", "BusCreator"],
-            [7, 2, 1, "", "ReadFromFileBus"],
-            [7, 2, 1, "", "ReadFromParameterBus"],
-            [7, 2, 1, "", "WriteToFileBus"],
-            [7, 1, 1, "", "get_timestamp"]
+            [8, 2, 1, "", "BusCreator"],
+            [8, 2, 1, "", "ReadFromFileBus"],
+            [8, 2, 1, "", "ReadFromParameterBus"],
+            [8, 2, 1, "", "WriteToFileBus"],
+            [8, 1, 1, "", "get_timestamp"]
         ],
         "serialtools.bus.BusCreator": [
-            [7, 3, 1, "", "add_arguments"],
-            [7, 4, 1, "", "baudrate"],
-            [7, 4, 1, "", "bytesize"],
-            [7, 3, 1, "", "create_args"],
-            [7, 3, 1, "", "create_bus"],
-            [7, 4, 1, "", "dsrdtr"],
-            [7, 4, 1, "", "parity"],
-            [7, 4, 1, "", "port"],
-            [7, 4, 1, "", "rtscts"],
-            [7, 4, 1, "", "stopbits"],
-            [7, 4, 1, "", "virtual"],
-            [7, 4, 1, "", "vport"],
-            [7, 4, 1, "", "xonxoff"]
+            [8, 3, 1, "", "add_arguments"],
+            [8, 4, 1, "", "baudrate"],
+            [8, 4, 1, "", "bytesize"],
+            [8, 3, 1, "", "create_args"],
+            [8, 3, 1, "", "create_bus"],
+            [8, 4, 1, "", "dsrdtr"],
+            [8, 4, 1, "", "parity"],
+            [8, 4, 1, "", "port"],
+            [8, 4, 1, "", "rtscts"],
+            [8, 4, 1, "", "stopbits"],
+            [8, 4, 1, "", "virtual"],
+            [8, 4, 1, "", "vport"],
+            [8, 4, 1, "", "xonxoff"]
         ],
         "serialtools.bus.ReadFromFileBus": [
-            [7, 3, 1, "", "cancel_read"],
-            [7, 3, 1, "", "cancel_write"],
-            [7, 3, 1, "", "close"],
-            [7, 3, 1, "", "read"],
-            [7, 4, 1, "", "timestamp"],
-            [7, 3, 1, "", "write"]
+            [8, 3, 1, "", "cancel_read"],
+            [8, 3, 1, "", "cancel_write"],
+            [8, 3, 1, "", "close"],
+            [8, 3, 1, "", "read"],
+            [8, 4, 1, "", "timestamp"],
+            [8, 3, 1, "", "write"]
         ],
         "serialtools.bus.ReadFromFileBus.params": [
-            [7, 5, 1, "", "fn"]
+            [8, 5, 1, "", "fn"]
         ],
         "serialtools.bus.ReadFromParameterBus.params": [
-            [7, 5, 1, "", "fn"]
+            [8, 5, 1, "", "fn"]
         ],
         "serialtools.bus.WriteToFileBus": [
-            [7, 3, 1, "", "cancel_read"],
-            [7, 3, 1, "", "cancel_write"],
-            [7, 3, 1, "", "close"],
-            [7, 3, 1, "", "read"],
-            [7, 4, 1, "", "timestamp"],
-            [7, 3, 1, "", "write"]
+            [8, 3, 1, "", "cancel_read"],
+            [8, 3, 1, "", "cancel_write"],
+            [8, 3, 1, "", "close"],
+            [8, 3, 1, "", "read"],
+            [8, 4, 1, "", "timestamp"],
+            [8, 3, 1, "", "write"]
         ],
         "serialtools.database": [
-            [8, 2, 1, "", "ByteSpec"],
-            [8, 2, 1, "", "Database"],
-            [8, 2, 1, "", "Endianness"],
-            [8, 2, 1, "", "Message"],
-            [8, 2, 1, "", "Reader"],
-            [8, 2, 1, "", "Signal"],
-            [8, 2, 1, "", "Type"],
-            [8, 1, 1, "", "format_bytes"]
+            [9, 2, 1, "", "ByteSpec"],
+            [9, 2, 1, "", "Database"],
+            [9, 2, 1, "", "Endianness"],
+            [9, 2, 1, "", "Message"],
+            [9, 2, 1, "", "MessageSpec"],
+            [9, 2, 1, "", "Reader"],
+            [9, 2, 1, "", "Signal"],
+            [9, 2, 1, "", "Type"],
+            [9, 1, 1, "", "format_bytes"]
         ],
         "serialtools.database.ByteSpec": [
-            [8, 3, 1, "", "format_allowed_values"],
-            [8, 3, 1, "", "get_length"]
+            [9, 3, 1, "", "format_allowed_values"],
+            [9, 3, 1, "", "get_length"]
         ],
         "serialtools.database.Database": [
-            [8, 3, 1, "", "decode"],
-            [8, 3, 1, "", "encode"],
-            [8, 3, 1, "", "encode_range"],
-            [8, 4, 1, "", "endianness"],
-            [8, 3, 1, "", "get_endianness_fmt"],
-            [8, 3, 1, "", "get_signal"],
-            [8, 3, 1, "", "get_start_bit"],
-            [8, 4, 1, "", "message_spec"],
-            [8, 4, 1, "", "signals"],
-            [8, 4, 1, "", "word_length_in_bits"]
+            [9, 3, 1, "", "decode"],
+            [9, 3, 1, "", "encode"],
+            [9, 3, 1, "", "encode_range"],
+            [9, 4, 1, "", "endianness"],
+            [9, 3, 1, "", "get_endianness_fmt"],
+            [9, 3, 1, "", "get_signal"],
+            [9, 3, 1, "", "get_start_bit"],
+            [9, 4, 1, "", "message_spec"],
+            [9, 4, 1, "", "signals"],
+            [9, 4, 1, "", "word_length_in_bits"]
         ],
         "serialtools.database.Endianness": [
-            [8, 4, 1, "", "BIG"],
-            [8, 4, 1, "", "LITTLE"]
+            [9, 4, 1, "", "BIG"],
+            [9, 4, 1, "", "LITTLE"]
         ],
         "serialtools.database.Message": [
-            [8, 3, 1, "", "format"],
-            [8, 3, 1, "", "format_raw"],
-            [8, 3, 1, "", "format_timestamp"]
+            [9, 3, 1, "", "format"],
+            [9, 3, 1, "", "format_raw"],
+            [9, 3, 1, "", "format_timestamp"]
+        ],
+        "serialtools.database.MessageSpec": [
+            [9, 4, 1, "", "ADDRESS"]
         ],
         "serialtools.database.Reader": [
-            [8, 4, 1, "", "ignore_bytes_between_messages"],
-            [8, 3, 1, "", "read"],
-            [8, 3, 1, "", "read_byte"],
-            [8, 3, 1, "", "read_in_other_thread"],
-            [8, 3, 1, "", "read_msg"],
-            [8, 3, 1, "", "read_n_bytes"],
-            [8, 3, 1, "", "send_msg"],
-            [8, 3, 1, "", "stop"]
+            [9, 4, 1, "", "ignore_bytes_between_messages"],
+            [9, 3, 1, "", "read"],
+            [9, 3, 1, "", "read_byte"],
+            [9, 3, 1, "", "read_in_other_thread"],
+            [9, 3, 1, "", "read_msg"],
+            [9, 3, 1, "", "read_n_bytes"],
+            [9, 3, 1, "", "send_msg"],
+            [9, 3, 1, "", "stop"]
         ],
         "serialtools.database.Signal": [
-            [8, 3, 1, "", "get_bitstruct_fmt"]
+            [9, 3, 1, "", "get_bitstruct_fmt"]
         ],
         "serialtools.database.Type": [
-            [8, 4, 1, "", "BOOL"],
-            [8, 4, 1, "", "FLOAT"],
-            [8, 4, 1, "", "INT"],
-            [8, 4, 1, "", "TEXT"],
-            [8, 4, 1, "", "UINT"]
+            [9, 4, 1, "", "BOOL"],
+            [9, 4, 1, "", "FLOAT"],
+            [9, 4, 1, "", "INT"],
+            [9, 4, 1, "", "TEXT"],
+            [9, 4, 1, "", "UINT"]
         ],
         "serialtools.database_config": [
-            [9, 2, 1, "", "DatabaseCreator"],
-            [9, 2, 1, "", "Message"],
-            [9, 2, 1, "", "Param"],
-            [9, 2, 1, "", "Signal"],
-            [9, 1, 1, "", "get_database"],
-            [9, 1, 1, "", "integer"]
+            [10, 2, 1, "", "DatabaseCreator"],
+            [10, 2, 1, "", "Message"],
+            [10, 2, 1, "", "Param"],
+            [10, 2, 1, "", "Signal"],
+            [10, 1, 1, "", "get_database"],
+            [10, 1, 1, "", "integer"]
         ],
         "serialtools.database_config.DatabaseCreator": [
-            [9, 4, 1, "", "endianness"],
-            [9, 3, 1, "", "get"],
-            [9, 4, 1, "", "word_length_in_bits"]
+            [10, 4, 1, "", "endianness"],
+            [10, 3, 1, "", "get"],
+            [10, 4, 1, "", "word_length_in_bits"]
         ],
         "serialtools.database_config.Message": [
-            [9, 3, 1, "", "init_parser"],
-            [9, 4, 1, "", "message"],
-            [9, 3, 1, "", "run_parsed"]
+            [10, 3, 1, "", "init_parser"],
+            [10, 4, 1, "", "message"],
+            [10, 3, 1, "", "run_parsed"]
         ],
         "serialtools.database_config.Message.init_parser.params": [
-            [9, 5, 1, "", "parser"]
+            [10, 5, 1, "", "parser"]
         ],
         "serialtools.database_config.Param": [
-            [9, 4, 1, "", "defined_parameters"],
-            [9, 3, 1, "", "init_parser"],
-            [9, 3, 1, "", "parse_allowed_values"],
-            [9, 3, 1, "", "run_parsed"]
+            [10, 4, 1, "", "defined_parameters"],
+            [10, 3, 1, "", "init_parser"],
+            [10, 3, 1, "", "parse_allowed_values"],
+            [10, 3, 1, "", "run_parsed"]
         ],
         "serialtools.database_config.Param.init_parser.params": [
-            [9, 5, 1, "", "parser"]
+            [10, 5, 1, "", "parser"]
         ],
         "serialtools.database_config.Signal": [
-            [9, 3, 1, "", "init_parser"],
-            [9, 3, 1, "", "run_parsed"],
-            [9, 4, 1, "", "signals"]
+            [10, 3, 1, "", "init_parser"],
+            [10, 3, 1, "", "run_parsed"],
+            [10, 4, 1, "", "signals"]
         ],
         "serialtools.database_config.Signal.init_parser.params": [
-            [9, 5, 1, "", "parser"]
+            [10, 5, 1, "", "parser"]
         ]
     },
     "objtypes": {
         "0": "py:module",
         "1": "py:function",
         "2": "py:class",
         "3": "py:method",
@@ -436,33 +454,34 @@
         "2": ["py", "class", "Python class"],
         "3": ["py", "method", "Python method"],
         "4": ["py", "attribute", "Python attribute"],
         "5": ["py", "parameter", "Python parameter"]
     },
     "titleterms": {
         "welcom": 0,
-        "serialtool": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+        "serialtool": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
         "": [],
         "document": 0,
         "indic": 0,
         "tabl": 0,
         "packag": [2, 3],
         "subpackag": 2,
         "submodul": [2, 3],
-        "modul": [2, 3, 4, 5, 6, 7, 8, 9],
+        "modul": [2, 3, 4, 5, 6, 7, 8, 9, 10],
         "content": [2, 3],
-        "app": [3, 4, 5, 6],
+        "app": [3, 4, 5, 6, 7],
         "decod": 4,
         "dump": 5,
-        "send": 6,
-        "bu": 7,
-        "databas": 8,
-        "database_config": 9,
+        "send": 7,
+        "bu": 8,
+        "databas": 9,
+        "database_config": 10,
         "refer": 0,
-        "link": 0
+        "link": 0,
+        "rawsplit": 6
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 8,
         "sphinx.domains.index": 1,
@@ -509,37 +528,41 @@
         ],
         "serialtools.apps.decode module": [
             [4, "module-serialtools.apps.decode"]
         ],
         "serialtools.apps.dump module": [
             [5, "module-serialtools.apps.dump"]
         ],
+        "serialtools.apps.rawsplit module": [
+            [6, "module-serialtools.apps.rawsplit"]
+        ],
         "serialtools.apps.send module": [
-            [6, "module-serialtools.apps.send"]
+            [7, "module-serialtools.apps.send"]
         ],
         "serialtools.bus module": [
-            [7, "module-serialtools.bus"]
+            [8, "module-serialtools.bus"]
         ],
         "serialtools.database module": [
-            [8, "module-serialtools.database"]
+            [9, "module-serialtools.database"]
         ],
         "serialtools.database_config module": [
-            [9, "module-serialtools.database_config"]
+            [10, "module-serialtools.database_config"]
         ]
     },
     "indexentries": {
         "module": [
             [2, "module-serialtools"],
             [3, "module-serialtools.apps"],
             [4, "module-serialtools.apps.decode"],
             [5, "module-serialtools.apps.dump"],
-            [6, "module-serialtools.apps.send"],
-            [7, "module-serialtools.bus"],
-            [8, "module-serialtools.database"],
-            [9, "module-serialtools.database_config"]
+            [6, "module-serialtools.apps.rawsplit"],
+            [7, "module-serialtools.apps.send"],
+            [8, "module-serialtools.bus"],
+            [9, "module-serialtools.database"],
+            [10, "module-serialtools.database_config"]
         ],
         "serialtools": [
             [2, "module-serialtools"]
         ],
         "add_arguments() (in module serialtools.apps)": [
             [3, "serialtools.apps.add_arguments"]
         ],
@@ -572,294 +595,318 @@
         ],
         "main() (in module serialtools.apps.dump)": [
             [5, "serialtools.apps.dump.main"]
         ],
         "serialtools.apps.dump": [
             [5, "module-serialtools.apps.dump"]
         ],
+        "add_arguments() (in module serialtools.apps.rawsplit)": [
+            [6, "serialtools.apps.rawsplit.add_arguments"]
+        ],
+        "add_parser() (in module serialtools.apps.rawsplit)": [
+            [6, "serialtools.apps.rawsplit.add_parser"]
+        ],
+        "decode() (in module serialtools.apps.rawsplit)": [
+            [6, "serialtools.apps.rawsplit.decode"]
+        ],
+        "error() (in module serialtools.apps.rawsplit)": [
+            [6, "serialtools.apps.rawsplit.error"]
+        ],
+        "main() (in module serialtools.apps.rawsplit)": [
+            [6, "serialtools.apps.rawsplit.main"]
+        ],
+        "serialtools.apps.rawsplit": [
+            [6, "module-serialtools.apps.rawsplit"]
+        ],
         "add_parser() (in module serialtools.apps.send)": [
-            [6, "serialtools.apps.send.add_parser"]
+            [7, "serialtools.apps.send.add_parser"]
         ],
         "main() (in module serialtools.apps.send)": [
-            [6, "serialtools.apps.send.main"]
+            [7, "serialtools.apps.send.main"]
         ],
         "send() (in module serialtools.apps.send)": [
-            [6, "serialtools.apps.send.send"]
+            [7, "serialtools.apps.send.send"]
         ],
         "serialtools.apps.send": [
-            [6, "module-serialtools.apps.send"]
+            [7, "module-serialtools.apps.send"]
         ],
         "buscreator (class in serialtools.bus)": [
-            [7, "serialtools.bus.BusCreator"]
+            [8, "serialtools.bus.BusCreator"]
         ],
         "readfromfilebus (class in serialtools.bus)": [
-            [7, "serialtools.bus.ReadFromFileBus"]
+            [8, "serialtools.bus.ReadFromFileBus"]
         ],
         "readfromparameterbus (class in serialtools.bus)": [
-            [7, "serialtools.bus.ReadFromParameterBus"]
+            [8, "serialtools.bus.ReadFromParameterBus"]
         ],
         "writetofilebus (class in serialtools.bus)": [
-            [7, "serialtools.bus.WriteToFileBus"]
+            [8, "serialtools.bus.WriteToFileBus"]
         ],
         "add_arguments() (serialtools.bus.buscreator method)": [
-            [7, "serialtools.bus.BusCreator.add_arguments"]
+            [8, "serialtools.bus.BusCreator.add_arguments"]
         ],
         "baudrate (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.baudrate"]
+            [8, "serialtools.bus.BusCreator.baudrate"]
         ],
         "bytesize (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.bytesize"]
+            [8, "serialtools.bus.BusCreator.bytesize"]
         ],
         "cancel_read() (serialtools.bus.readfromfilebus method)": [
-            [7, "serialtools.bus.ReadFromFileBus.cancel_read"]
+            [8, "serialtools.bus.ReadFromFileBus.cancel_read"]
         ],
         "cancel_read() (serialtools.bus.writetofilebus method)": [
-            [7, "serialtools.bus.WriteToFileBus.cancel_read"]
+            [8, "serialtools.bus.WriteToFileBus.cancel_read"]
         ],
         "cancel_write() (serialtools.bus.readfromfilebus method)": [
-            [7, "serialtools.bus.ReadFromFileBus.cancel_write"]
+            [8, "serialtools.bus.ReadFromFileBus.cancel_write"]
         ],
         "cancel_write() (serialtools.bus.writetofilebus method)": [
-            [7, "serialtools.bus.WriteToFileBus.cancel_write"]
+            [8, "serialtools.bus.WriteToFileBus.cancel_write"]
         ],
         "close() (serialtools.bus.readfromfilebus method)": [
-            [7, "serialtools.bus.ReadFromFileBus.close"]
+            [8, "serialtools.bus.ReadFromFileBus.close"]
         ],
         "close() (serialtools.bus.writetofilebus method)": [
-            [7, "serialtools.bus.WriteToFileBus.close"]
+            [8, "serialtools.bus.WriteToFileBus.close"]
         ],
         "create_args() (serialtools.bus.buscreator method)": [
-            [7, "serialtools.bus.BusCreator.create_args"]
+            [8, "serialtools.bus.BusCreator.create_args"]
         ],
         "create_bus() (serialtools.bus.buscreator method)": [
-            [7, "serialtools.bus.BusCreator.create_bus"]
+            [8, "serialtools.bus.BusCreator.create_bus"]
         ],
         "dsrdtr (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.dsrdtr"]
+            [8, "serialtools.bus.BusCreator.dsrdtr"]
         ],
         "get_timestamp() (in module serialtools.bus)": [
-            [7, "serialtools.bus.get_timestamp"]
+            [8, "serialtools.bus.get_timestamp"]
         ],
         "parity (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.parity"]
+            [8, "serialtools.bus.BusCreator.parity"]
         ],
         "port (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.port"]
+            [8, "serialtools.bus.BusCreator.port"]
         ],
         "read() (serialtools.bus.readfromfilebus method)": [
-            [7, "serialtools.bus.ReadFromFileBus.read"]
+            [8, "serialtools.bus.ReadFromFileBus.read"]
         ],
         "read() (serialtools.bus.writetofilebus method)": [
-            [7, "serialtools.bus.WriteToFileBus.read"]
+            [8, "serialtools.bus.WriteToFileBus.read"]
         ],
         "rtscts (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.rtscts"]
+            [8, "serialtools.bus.BusCreator.rtscts"]
         ],
         "serialtools.bus": [
-            [7, "module-serialtools.bus"]
+            [8, "module-serialtools.bus"]
         ],
         "stopbits (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.stopbits"]
+            [8, "serialtools.bus.BusCreator.stopbits"]
         ],
         "timestamp (serialtools.bus.readfromfilebus attribute)": [
-            [7, "serialtools.bus.ReadFromFileBus.timestamp"]
+            [8, "serialtools.bus.ReadFromFileBus.timestamp"]
         ],
         "timestamp (serialtools.bus.writetofilebus attribute)": [
-            [7, "serialtools.bus.WriteToFileBus.timestamp"]
+            [8, "serialtools.bus.WriteToFileBus.timestamp"]
         ],
         "virtual (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.virtual"]
+            [8, "serialtools.bus.BusCreator.virtual"]
         ],
         "vport (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.vport"]
+            [8, "serialtools.bus.BusCreator.vport"]
         ],
         "write() (serialtools.bus.readfromfilebus method)": [
-            [7, "serialtools.bus.ReadFromFileBus.write"]
+            [8, "serialtools.bus.ReadFromFileBus.write"]
         ],
         "write() (serialtools.bus.writetofilebus method)": [
-            [7, "serialtools.bus.WriteToFileBus.write"]
+            [8, "serialtools.bus.WriteToFileBus.write"]
         ],
         "xonxoff (serialtools.bus.buscreator attribute)": [
-            [7, "serialtools.bus.BusCreator.xonxoff"]
+            [8, "serialtools.bus.BusCreator.xonxoff"]
+        ],
+        "address (serialtools.database.messagespec attribute)": [
+            [9, "serialtools.database.MessageSpec.ADDRESS"]
         ],
         "big (serialtools.database.endianness attribute)": [
-            [8, "serialtools.database.Endianness.BIG"]
+            [9, "serialtools.database.Endianness.BIG"]
         ],
         "bool (serialtools.database.type attribute)": [
-            [8, "serialtools.database.Type.BOOL"]
+            [9, "serialtools.database.Type.BOOL"]
         ],
         "bytespec (class in serialtools.database)": [
-            [8, "serialtools.database.ByteSpec"]
+            [9, "serialtools.database.ByteSpec"]
         ],
         "database (class in serialtools.database)": [
-            [8, "serialtools.database.Database"]
+            [9, "serialtools.database.Database"]
         ],
         "endianness (class in serialtools.database)": [
-            [8, "serialtools.database.Endianness"]
+            [9, "serialtools.database.Endianness"]
         ],
         "float (serialtools.database.type attribute)": [
-            [8, "serialtools.database.Type.FLOAT"]
+            [9, "serialtools.database.Type.FLOAT"]
         ],
         "int (serialtools.database.type attribute)": [
-            [8, "serialtools.database.Type.INT"]
+            [9, "serialtools.database.Type.INT"]
         ],
         "little (serialtools.database.endianness attribute)": [
-            [8, "serialtools.database.Endianness.LITTLE"]
+            [9, "serialtools.database.Endianness.LITTLE"]
         ],
         "message (class in serialtools.database)": [
-            [8, "serialtools.database.Message"]
+            [9, "serialtools.database.Message"]
+        ],
+        "messagespec (class in serialtools.database)": [
+            [9, "serialtools.database.MessageSpec"]
         ],
         "reader (class in serialtools.database)": [
-            [8, "serialtools.database.Reader"]
+            [9, "serialtools.database.Reader"]
         ],
         "signal (class in serialtools.database)": [
-            [8, "serialtools.database.Signal"]
+            [9, "serialtools.database.Signal"]
         ],
         "text (serialtools.database.type attribute)": [
-            [8, "serialtools.database.Type.TEXT"]
+            [9, "serialtools.database.Type.TEXT"]
         ],
         "type (class in serialtools.database)": [
-            [8, "serialtools.database.Type"]
+            [9, "serialtools.database.Type"]
         ],
         "uint (serialtools.database.type attribute)": [
-            [8, "serialtools.database.Type.UINT"]
+            [9, "serialtools.database.Type.UINT"]
         ],
         "decode() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.decode"]
+            [9, "serialtools.database.Database.decode"]
         ],
         "encode() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.encode"]
+            [9, "serialtools.database.Database.encode"]
         ],
         "encode_range() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.encode_range"]
+            [9, "serialtools.database.Database.encode_range"]
         ],
         "endianness (serialtools.database.database attribute)": [
-            [8, "serialtools.database.Database.endianness"]
+            [9, "serialtools.database.Database.endianness"]
         ],
         "format() (serialtools.database.message method)": [
-            [8, "serialtools.database.Message.format"]
+            [9, "serialtools.database.Message.format"]
         ],
         "format_allowed_values() (serialtools.database.bytespec method)": [
-            [8, "serialtools.database.ByteSpec.format_allowed_values"]
+            [9, "serialtools.database.ByteSpec.format_allowed_values"]
         ],
         "format_bytes() (in module serialtools.database)": [
-            [8, "serialtools.database.format_bytes"]
+            [9, "serialtools.database.format_bytes"]
         ],
         "format_raw() (serialtools.database.message method)": [
-            [8, "serialtools.database.Message.format_raw"]
+            [9, "serialtools.database.Message.format_raw"]
         ],
         "format_timestamp() (serialtools.database.message method)": [
-            [8, "serialtools.database.Message.format_timestamp"]
+            [9, "serialtools.database.Message.format_timestamp"]
         ],
         "get_bitstruct_fmt() (serialtools.database.signal method)": [
-            [8, "serialtools.database.Signal.get_bitstruct_fmt"]
+            [9, "serialtools.database.Signal.get_bitstruct_fmt"]
         ],
         "get_endianness_fmt() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.get_endianness_fmt"]
+            [9, "serialtools.database.Database.get_endianness_fmt"]
         ],
         "get_length() (serialtools.database.bytespec method)": [
-            [8, "serialtools.database.ByteSpec.get_length"]
+            [9, "serialtools.database.ByteSpec.get_length"]
         ],
         "get_signal() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.get_signal"]
+            [9, "serialtools.database.Database.get_signal"]
         ],
         "get_start_bit() (serialtools.database.database method)": [
-            [8, "serialtools.database.Database.get_start_bit"]
+            [9, "serialtools.database.Database.get_start_bit"]
         ],
         "ignore_bytes_between_messages (serialtools.database.reader attribute)": [
-            [8, "serialtools.database.Reader.ignore_bytes_between_messages"]
+            [9, "serialtools.database.Reader.ignore_bytes_between_messages"]
         ],
         "message_spec (serialtools.database.database attribute)": [
-            [8, "serialtools.database.Database.message_spec"]
+            [9, "serialtools.database.Database.message_spec"]
         ],
         "read() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.read"]
+            [9, "serialtools.database.Reader.read"]
         ],
         "read_byte() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.read_byte"]
+            [9, "serialtools.database.Reader.read_byte"]
         ],
         "read_in_other_thread() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.read_in_other_thread"]
+            [9, "serialtools.database.Reader.read_in_other_thread"]
         ],
         "read_msg() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.read_msg"]
+            [9, "serialtools.database.Reader.read_msg"]
         ],
         "read_n_bytes() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.read_n_bytes"]
+            [9, "serialtools.database.Reader.read_n_bytes"]
         ],
         "send_msg() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.send_msg"]
+            [9, "serialtools.database.Reader.send_msg"]
         ],
         "serialtools.database": [
-            [8, "module-serialtools.database"]
+            [9, "module-serialtools.database"]
         ],
         "signals (serialtools.database.database attribute)": [
-            [8, "serialtools.database.Database.signals"]
+            [9, "serialtools.database.Database.signals"]
         ],
         "stop() (serialtools.database.reader method)": [
-            [8, "serialtools.database.Reader.stop"]
+            [9, "serialtools.database.Reader.stop"]
         ],
         "word_length_in_bits (serialtools.database.database attribute)": [
-            [8, "serialtools.database.Database.word_length_in_bits"]
+            [9, "serialtools.database.Database.word_length_in_bits"]
         ],
         "databasecreator (class in serialtools.database_config)": [
-            [9, "serialtools.database_config.DatabaseCreator"]
+            [10, "serialtools.database_config.DatabaseCreator"]
         ],
         "message (class in serialtools.database_config)": [
-            [9, "serialtools.database_config.Message"]
+            [10, "serialtools.database_config.Message"]
         ],
         "param (class in serialtools.database_config)": [
-            [9, "serialtools.database_config.Param"]
+            [10, "serialtools.database_config.Param"]
         ],
         "signal (class in serialtools.database_config)": [
-            [9, "serialtools.database_config.Signal"]
+            [10, "serialtools.database_config.Signal"]
         ],
         "defined_parameters (serialtools.database_config.param attribute)": [
-            [9, "serialtools.database_config.Param.defined_parameters"]
+            [10, "serialtools.database_config.Param.defined_parameters"]
         ],
         "endianness (serialtools.database_config.databasecreator attribute)": [
-            [9, "serialtools.database_config.DatabaseCreator.endianness"]
+            [10, "serialtools.database_config.DatabaseCreator.endianness"]
         ],
         "get() (serialtools.database_config.databasecreator method)": [
-            [9, "serialtools.database_config.DatabaseCreator.get"]
+            [10, "serialtools.database_config.DatabaseCreator.get"]
         ],
         "get_database() (in module serialtools.database_config)": [
-            [9, "serialtools.database_config.get_database"]
+            [10, "serialtools.database_config.get_database"]
         ],
         "init_parser() (serialtools.database_config.message method)": [
-            [9, "serialtools.database_config.Message.init_parser"]
+            [10, "serialtools.database_config.Message.init_parser"]
         ],
         "init_parser() (serialtools.database_config.param method)": [
-            [9, "serialtools.database_config.Param.init_parser"]
+            [10, "serialtools.database_config.Param.init_parser"]
         ],
         "init_parser() (serialtools.database_config.signal method)": [
-            [9, "serialtools.database_config.Signal.init_parser"]
+            [10, "serialtools.database_config.Signal.init_parser"]
         ],
         "integer() (in module serialtools.database_config)": [
-            [9, "serialtools.database_config.integer"]
+            [10, "serialtools.database_config.integer"]
         ],
         "message (serialtools.database_config.message attribute)": [
-            [9, "serialtools.database_config.Message.message"]
+            [10, "serialtools.database_config.Message.message"]
         ],
         "parse_allowed_values() (serialtools.database_config.param method)": [
-            [9, "serialtools.database_config.Param.parse_allowed_values"]
+            [10, "serialtools.database_config.Param.parse_allowed_values"]
         ],
         "run_parsed() (serialtools.database_config.message method)": [
-            [9, "serialtools.database_config.Message.run_parsed"]
+            [10, "serialtools.database_config.Message.run_parsed"]
         ],
         "run_parsed() (serialtools.database_config.param method)": [
-            [9, "serialtools.database_config.Param.run_parsed"]
+            [10, "serialtools.database_config.Param.run_parsed"]
         ],
         "run_parsed() (serialtools.database_config.signal method)": [
-            [9, "serialtools.database_config.Signal.run_parsed"]
+            [10, "serialtools.database_config.Signal.run_parsed"]
         ],
         "serialtools.database_config": [
-            [9, "module-serialtools.database_config"]
+            [10, "module-serialtools.database_config"]
         ],
         "signals (serialtools.database_config.signal attribute)": [
-            [9, "serialtools.database_config.Signal.signals"]
+            [10, "serialtools.database_config.Signal.signals"]
         ],
         "word_length_in_bits (serialtools.database_config.databasecreator attribute)": [
-            [9, "serialtools.database_config.DatabaseCreator.word_length_in_bits"]
+            [10, "serialtools.database_config.DatabaseCreator.word_length_in_bits"]
         ]
     }
 })
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.3.0/docs/build/html/serialtools.apps.decode.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -67,14 +67,15 @@
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.decode.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.decode.decode"><code class="docutils literal notranslate"><span class="pre">decode()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.decode.error"><code class="docutils literal notranslate"><span class="pre">error()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.decode.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
@@ -21,14 +21,15 @@
     * serialtools.apps.decode_module
           o add_arguments()
           o add_parser()
           o decode()
           o error()
           o main()
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools_package
     * serialtools.apps_package
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.3.0/docs/build/html/serialtools.apps.dump.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -65,14 +65,15 @@
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.apps.dump module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.dump.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.dump.dump"><code class="docutils literal notranslate"><span class="pre">dump()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.dump.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
```

#### html2text {}

```diff
@@ -5,28 +5,29 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
           o add_parser()
           o dump()
           o main()
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools_package
     * serialtools.apps_package
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.apps.html` & `serialtools-0.3.0/docs/build/html/serialtools.apps.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -60,14 +60,15 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
```

#### html2text {}

```diff
@@ -5,25 +5,26 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools_package
     * serialtools.apps package
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.apps.send.html` & `serialtools-0.3.0/docs/build/html/serialtools.apps.send.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -60,14 +60,15 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.apps.send module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.send.add_parser"><code class="docutils literal notranslate"><span class="pre">add_parser()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.send.main"><code class="docutils literal notranslate"><span class="pre">main()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.apps.send.send"><code class="docutils literal notranslate"><span class="pre">send()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
```

#### html2text {}

```diff
@@ -5,25 +5,26 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
           o add_parser()
           o main()
           o send()
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.bus.html` & `serialtools-0.3.0/docs/build/html/serialtools.bus.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -65,14 +65,15 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.add_arguments"><code class="docutils literal notranslate"><span class="pre">BusCreator.add_arguments()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.baudrate"><code class="docutils literal notranslate"><span class="pre">BusCreator.baudrate</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.bytesize"><code class="docutils literal notranslate"><span class="pre">BusCreator.bytesize</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.create_args"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_args()</span></code></a></li>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
@@ -21,14 +21,15 @@
                       # WriteToFileBus
                       # get_timestamp()
                 # serialtools.database_module
                 # serialtools.database_config_module
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
           o BusCreator
                 # BusCreator.add_arguments()
                 # BusCreator.baudrate
                 # BusCreator.bytesize
                 # BusCreator.create_args()
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.database.html` & `serialtools-0.3.0/docs/build/html/serialtools.database.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -54,28 +54,30 @@
 <li class="toctree-l2 current"><a class="reference internal" href="serialtools.html#submodules">Submodules</a><ul class="current">
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l3 current"><a class="current reference internal" href="#">serialtools.database module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Database"><code class="docutils literal notranslate"><span class="pre">Database</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.database.format_bytes"><code class="docutils literal notranslate"><span class="pre">format_bytes()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.database module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.ByteSpec.format_allowed_values"><code class="docutils literal notranslate"><span class="pre">ByteSpec.format_allowed_values()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.ByteSpec.get_length"><code class="docutils literal notranslate"><span class="pre">ByteSpec.get_length()</span></code></a></li>
 </ul>
@@ -100,14 +102,18 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
@@ -179,15 +185,15 @@
 <span class="sig-name descname"><span class="pre">get_length</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">values</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Mapping" title="(in Python v3.11)"><span class="pre">Mapping</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#serialtools.database.ByteSpec.get_length" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Database">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Database</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message_spec</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.ByteSpec" title="serialtools.database.ByteSpec"><span class="pre">ByteSpec</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">signals</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">Signal</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">endianness</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Endianness" title="serialtools.database.Endianness"><span class="pre">Endianness</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">word_length_in_bits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">8</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Database" title="Permalink to this definition"></a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Database</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">message_spec</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.MessageSpec" title="serialtools.database.MessageSpec"><span class="pre">MessageSpec</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">signals</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">Signal</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">endianness</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Endianness" title="serialtools.database.Endianness"><span class="pre">Endianness</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">word_length_in_bits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">8</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Database" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Database.decode">
 <span class="sig-name descname"><span class="pre">decode</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#dict" title="(in Python v3.11)"><span class="pre">dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">serialtools.database.Signal</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#serialtools.database.Database.decode" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
@@ -220,15 +226,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Database.get_start_bit">
 <span class="sig-name descname"><span class="pre">get_start_bit</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">signal</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">Signal</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#serialtools.database.Database.get_start_bit" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database.Database.message_spec">
-<span class="sig-name descname"><span class="pre">message_spec</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.ByteSpec" title="serialtools.database.ByteSpec"><span class="pre">ByteSpec</span></a><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#serialtools.database.Database.message_spec" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">message_spec</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.database.MessageSpec" title="serialtools.database.MessageSpec"><span class="pre">MessageSpec</span></a></em><a class="headerlink" href="#serialtools.database.Database.message_spec" title="Permalink to this definition"></a></dt>
 <dd><p>The parts that a message consists of, e.g. an address to be read, the length of the data, the data itself</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database.Database.signals">
 <span class="sig-name descname"><span class="pre">signals</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.Signal" title="serialtools.database.Signal"><span class="pre">Signal</span></a><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#serialtools.database.Database.signals" title="Permalink to this definition"></a></dt>
 <dd><p>The possible signals which can be encoded in the data</p>
@@ -276,14 +282,25 @@
 <dt class="sig sig-object py" id="serialtools.database.Message.format_timestamp">
 <span class="sig-name descname"><span class="pre">format_timestamp</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Message.format_timestamp" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
+<dt class="sig sig-object py" id="serialtools.database.MessageSpec">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">MessageSpec</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">params</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/collections.abc.html#collections.abc.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#serialtools.database.ByteSpec" title="serialtools.database.ByteSpec"><span class="pre">ByteSpec</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">implicit_address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.MessageSpec" title="Permalink to this definition"></a></dt>
+<dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
+<dl class="py attribute">
+<dt class="sig sig-object py" id="serialtools.database.MessageSpec.ADDRESS">
+<span class="sig-name descname"><span class="pre">ADDRESS</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">'address'</span></em><a class="headerlink" href="#serialtools.database.MessageSpec.ADDRESS" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
+</dd></dl>
+
+<dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Reader">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Reader</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bus</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">serial.Serial</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus" title="serialtools.bus.ReadFromFileBus"><span class="pre">ReadFromFileBus</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus" title="serialtools.bus.WriteToFileBus"><span class="pre">WriteToFileBus</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">db</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Reader" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database.Reader.ignore_bytes_between_messages">
 <span class="sig-name descname"><span class="pre">ignore_bytes_between_messages</span></span><a class="headerlink" href="#serialtools.database.Reader.ignore_bytes_between_messages" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
```

#### html2text {}

```diff
@@ -5,33 +5,35 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
                       # Database
                       # Endianness
                       # Message
+                      # MessageSpec
                       # Reader
                       # Signal
                       # Type
                       # format_bytes()
                 # serialtools.database_config_module
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
           o ByteSpec
                 # ByteSpec.format_allowed_values()
                 # ByteSpec.get_length()
           o Database
@@ -48,14 +50,16 @@
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
                 # Message.format()
                 # Message.format_raw()
                 # Message.format_timestamp()
+          o MessageSpec
+                # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
@@ -81,30 +85,30 @@
   None, allowed_values: Sequence[bytes] | bytes | int | None = None)ï
       Bases: object
         Paramref length:
             Either the number of bytes or the name of a previous byte spec
             which specifies the length of this byte spec
         format_allowed_values() &#x2192; strï
         get_length(values: Mapping[str, bytes]) &#x2192; intï
-  classserialtools.database.Database(message_spec: Sequence[ByteSpec], signals:
+  classserialtools.database.Database(message_spec: MessageSpec, signals:
   Sequence[Signal], *, endianness: Endianness, word_length_in_bits: int = 8)ï
       Bases: object
         decode(address: int, data: bytes) &#x2192; dict
         [serialtools.database.Signal, float]ï
         encode(data: Mapping[Signal, int | float | str] | Mapping[str, int |
         float | str]) &#x2192; bytesï
         encode_range(address: int, length_in_bytes: int, value: Callable[
         [Signal], int | float | str]) &#x2192; bytesï
             Encode all signals which are completely within the given range
         endianness: Endiannessï
             The byte order
         get_endianness_fmt() &#x2192; strï
         get_signal(name: str) &#x2192; Signalï
         get_start_bit(signal: Signal) &#x2192; intï
-        message_spec: Sequence[ByteSpec]ï
+        message_spec: MessageSpecï
             The parts that a message consists of, e.g. an address to be read,
             the length of the data, the data itself
         signals: Sequence[Signal]ï
             The possible signals which can be encoded in the data
         word_length_in_bits: intï
             The default length of a signal
   classserialtools.database.Endianness(value, names=None, *, module=None,
@@ -114,14 +118,18 @@
         LITTLE= 2ï
   classserialtools.database.Message(db: Database, timestamp: datetime | None,
   values: Mapping[str, bytes])ï
       Bases: object
         format() &#x2192; strï
         format_raw() &#x2192; strï
         format_timestamp() &#x2192; strï
+  classserialtools.database.MessageSpec(params: Sequence[ByteSpec], *,
+  implicit_address: int | None = None)ï
+      Bases: object
+        ADDRESS= 'address'ï
   classserialtools.database.Reader(bus: serial.Serial | ReadFromFileBus |
   WriteToFileBus, db: Database)ï
       Bases: object
         ignore_bytes_between_messagesï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.database_config.html` & `serialtools-0.3.0/docs/build/html/serialtools.database_config.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -18,14 +18,15 @@
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="serialtools.apps.rawsplit module" href="serialtools.apps.rawsplit.html" />
     <link rel="prev" title="serialtools.database module" href="serialtools.database.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
@@ -33,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -65,14 +66,15 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.database_config module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.endianness"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.endianness</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database_config.DatabaseCreator.get"><code class="docutils literal notranslate"><span class="pre">DatabaseCreator.get()</span></code></a></li>
@@ -139,15 +141,15 @@
 <dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.endianness">
 <span class="sig-name descname"><span class="pre">endianness</span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.endianness" title="Permalink to this definition"></a></dt>
 <dd><p>A setting without a default value which requires the user to explicitly set a value in the config file.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.get" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">require_signals</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.get" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database_config.DatabaseCreator.word_length_in_bits">
 <span class="sig-name descname"><span class="pre">word_length_in_bits</span></span><a class="headerlink" href="#serialtools.database_config.DatabaseCreator.word_length_in_bits" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
@@ -170,15 +172,15 @@
 </dl>
 <p>This is an abstract method which must be implemented by subclasses.
 Use <code class="xref py py-meth docutils literal notranslate"><span class="pre">ArgumentParser.add_argument()</span></code> to add arguments to <code class="xref py py-paramref docutils literal notranslate"><span class="pre">parser</span></code>.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.database_config.Message.message">
-<span class="sig-name descname"><span class="pre">message</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><span class="pre">list</span></a><span class="p"><span class="pre">[</span></span><span class="pre">db.ByteSpec</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#serialtools.database_config.Message.message" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">message</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">db.MessageSpec</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#serialtools.database_config.Message.message" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database_config.Message.run_parsed">
 <span class="sig-name descname"><span class="pre">run_parsed</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.Namespace" title="(in Python v3.11)"><span class="pre">Namespace</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database_config.Message.run_parsed" title="Permalink to this definition"></a></dt>
 <dd><p>This is an abstract method which must be implemented by subclasses.</p>
 </dd></dl>
@@ -247,29 +249,30 @@
 <span class="sig-name descname"><span class="pre">signals</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#list" title="(in Python v3.11)"><span class="pre">list</span></a><span class="p"><span class="pre">[</span></span><span class="pre">db.Signal</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">[]</span></em><a class="headerlink" href="#serialtools.database_config.Signal.signals" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="serialtools.database_config.get_database">
-<span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">get_database</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.get_database" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">get_database</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">require_signals</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></span><a class="headerlink" href="#serialtools.database_config.get_database" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="serialtools.database_config.integer">
 <span class="sig-prename descclassname"><span class="pre">serialtools.database_config.</span></span><span class="sig-name descname"><span class="pre">integer</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">val</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></span><a class="headerlink" href="#serialtools.database_config.integer" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="serialtools.database.html" class="btn btn-neutral float-left" title="serialtools.database module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="serialtools.apps.rawsplit.html" class="btn btn-neutral float-right" title="serialtools.apps.rawsplit module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, erzo.</p>
   </div>
```

#### html2text {}

```diff
@@ -3,16 +3,17 @@
 
 
 
 
 
 
 
+
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
@@ -21,14 +22,15 @@
                       # Param
                       # Signal
                       # get_database()
                       # integer()
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
           o DatabaseCreator
                 # DatabaseCreator.endianness
                 # DatabaseCreator.get()
@@ -55,30 +57,30 @@
 ===============================================================================
 ****** serialtools.database_config moduleï ******
   classserialtools.database_config.DatabaseCreatorï
       Bases: object
         endiannessï
             A setting without a default value which requires the user to
             explicitly set a value in the config file.
-        get() &#x2192; Databaseï
+        get(*, require_signals: bool = True) &#x2192; Databaseï
         word_length_in_bitsï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
   classserialtools.database_config.Message(config_file: ConfigFile)ï
       Bases: ConfigFileArgparseCommand
         init_parser(parser: ArgumentParser) &#x2192; Noneï
               Parameters:
                   parserÂ¶ â The parser to add arguments to. This is the same
                   object like parser.
             This is an abstract method which must be implemented by subclasses.
             Use ArgumentParser.add_argument() to add arguments to parser.
-        message: list[db.ByteSpec] | None= Noneï
+        message: db.MessageSpec | None= Noneï
         run_parsed(args: Namespace) &#x2192; Noneï
             This is an abstract method which must be implemented by subclasses.
   classserialtools.database_config.Param(config_file: ConfigFile)ï
       Bases: ConfigFileArgparseCommand
       Define a parameter that can be used in the message command.
         defined_parameters: dict[str, db.ByteSpec]= {}ï
         init_parser(parser: ArgumentParser) &#x2192; Noneï
@@ -98,13 +100,14 @@
                   parserÂ¶ â The parser to add arguments to. This is the same
                   object like parser.
             This is an abstract method which must be implemented by subclasses.
             Use ArgumentParser.add_argument() to add arguments to parser.
         run_parsed(args: Namespace) &#x2192; Noneï
             This is an abstract method which must be implemented by subclasses.
         signals: list[db.Signal]= []ï
-  serialtools.database_config.get_database() &#x2192; Databaseï
+  serialtools.database_config.get_database(*, require_signals: bool = True)
+  &#x2192; Databaseï
   serialtools.database_config.integer(val: str) &#x2192; intï
-Previous
+Previous Next
 ===============================================================================
 © Copyright 2023, erzo.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `serialtools-0.2.1/docs/build/html/serialtools.html` & `serialtools-0.3.0/docs/build/html/serialtools.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.2.1 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.3.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.2.1
+                v0.3.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -61,14 +61,15 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#module-serialtools">Module contents</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
         </div>
@@ -203,14 +204,18 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message"><code class="docutils literal notranslate"><span class="pre">Message</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format"><code class="docutils literal notranslate"><span class="pre">Message.format()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_raw"><code class="docutils literal notranslate"><span class="pre">Message.format_raw()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Message.format_timestamp"><code class="docutils literal notranslate"><span class="pre">Message.format_timestamp()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec"><code class="docutils literal notranslate"><span class="pre">MessageSpec</span></code></a><ul>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.MessageSpec.ADDRESS"><code class="docutils literal notranslate"><span class="pre">MessageSpec.ADDRESS</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader"><code class="docutils literal notranslate"><span class="pre">Reader</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.ignore_bytes_between_messages"><code class="docutils literal notranslate"><span class="pre">Reader.ignore_bytes_between_messages</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read"><code class="docutils literal notranslate"><span class="pre">Reader.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_byte"><code class="docutils literal notranslate"><span class="pre">Reader.read_byte()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_in_other_thread"><code class="docutils literal notranslate"><span class="pre">Reader.read_in_other_thread()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_msg"><code class="docutils literal notranslate"><span class="pre">Reader.read_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
```

#### html2text {}

```diff
@@ -5,26 +5,27 @@
 
 
 
 
 
 
 serialtools
-v0.2.1
+v0.3.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
+    * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools package
     * View_page_source
@@ -100,14 +101,16 @@
           o Endianness
                 # Endianness.BIG
                 # Endianness.LITTLE
           o Message
                 # Message.format()
                 # Message.format_raw()
                 # Message.format_timestamp()
+          o MessageSpec
+                # MessageSpec.ADDRESS
           o Reader
                 # Reader.ignore_bytes_between_messages
                 # Reader.read()
                 # Reader.read_byte()
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
```

### Comparing `serialtools-0.2.1/docs/make.bat` & `serialtools-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/docs/source/conf.py` & `serialtools-0.3.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.2.1'
+release = 'v0.3.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.2.1/docs/source/index.rst` & `serialtools-0.3.0/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. toctree::
    :maxdepth: 2
 
    serialtools
    serialtools.apps.decode
    serialtools.apps.dump
    serialtools.apps.__init__
+   serialtools.apps.rawsplit
    serialtools.apps.send
    serialtools.bus
    serialtools.database
    serialtools.database_config
    serialtools.__main__
```

### Comparing `serialtools-0.2.1/prepare_for_gitlab_pages.py` & `serialtools-0.3.0/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/pyproject.toml` & `serialtools-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/release.sh` & `serialtools-0.3.0/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/src/serialtools/__main__.py` & `serialtools-0.3.0/src/serialtools/__main__.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/src/serialtools/apps/decode.py` & `serialtools-0.3.0/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/src/serialtools/apps/dump.py` & `serialtools-0.3.0/src/serialtools/apps/dump.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/src/serialtools/apps/send.py` & `serialtools-0.3.0/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.2.1/src/serialtools/bus.py` & `serialtools-0.3.0/src/serialtools/bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 		self.f = open(fn, 'rt')
 
 	def read(self, n: int) -> bytes:
 		out = []
 		for i in range(n):
 			h = ''
 			while True:
-				c = self.f.read(1)
+				try:
+					c = self.f.read(1)
+				except:
+					# ValueError: I/O operation on closed file.
+					return bytes()
 				if not c:
 					self.close()
 					return bytes()
 				if not h and c.isspace():
 					continue
 				if not h and c == '(':
 					timestamp = ''
```

### Comparing `serialtools-0.2.1/src/serialtools/database.py` & `serialtools-0.3.0/src/serialtools/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,39 @@
 		if self.allowed_values is None:
 			return ""
 		return " or ".join(format_bytes(val) for val in self.allowed_values)
 
 	def __repr__(self) -> str:
 		return f"{type(self).__name__}({self.name!r}, length={self.length!r}, allowed_values={self.format_allowed_values()})"
 
+class MessageSpec:
+
+	ADDRESS = 'address'
+
+	def __init__(self, params: 'Sequence[ByteSpec]', *, implicit_address: 'int|None' = None) -> None:
+		self.params = params
+		self.implicit_address = implicit_address
+
+	def __len__(self) -> int:
+		return len(self.params)
+
+	@typing.overload
+	def __getitem__(self, index: int) -> ByteSpec:
+		pass
+
+	@typing.overload
+	def __getitem__(self, index: slice) -> 'Sequence[ByteSpec]':
+		pass
+
+	def __getitem__(self, index: 'int|slice') -> 'ByteSpec|Sequence[ByteSpec]':
+		return self.params[index]
+
+	def __iter__(self) -> 'Iterator[ByteSpec]':
+		return iter(self.params)
+
 
 class Message:
 
 	def __init__(self, db: 'Database', timestamp: 'datetime.datetime|None', values: 'Mapping[str, bytes]') -> None:
 		self.db = db
 		self.timestamp = timestamp
 		self.values = values
@@ -87,15 +112,22 @@
 			timestamp += ' '
 
 		values = ' '.join(format_bytes(b) for b in self.values.values())
 		return timestamp + values
 
 	def format(self) -> str:
 		out = self.format_raw()
-		address, = self.values['address']
+		if 'address' in self.values:
+			address, = self.values['address']
+		else:
+			implicit_address = self.db.message_spec.implicit_address
+			if implicit_address is None:
+				raise ValueError(f"Message has neither explicit nor implicit address")
+			address = implicit_address
+
 		data = self.values['data']
 		for sig, val in self.db.decode(address, data).items():
 			out += f"\n\t{sig.name}: {val}{sig.unit}"
 		return out
 
 
 class Reader:
@@ -203,26 +235,29 @@
 	BOOL = 'b'
 	FLOAT = 'f'
 	TEXT = 't'
 
 class Database:
 
 	#: The parts that a message consists of, e.g. an address to be read, the length of the data, the data itself
-	message_spec: 'Sequence[ByteSpec]'
+	message_spec: 'MessageSpec'
 
 	#: The possible signals which can be encoded in the data
 	signals: 'Sequence[Signal]'
 
 	#: The byte order
 	endianness: Endianness
 
 	#: The default length of a signal
 	word_length_in_bits: int
 
-	def __init__(self, message_spec: 'Sequence[ByteSpec]', signals: 'Sequence[Signal]', *, endianness: Endianness, word_length_in_bits: int = 8):
+	def __init__(self, message_spec: 'MessageSpec', signals: 'Sequence[Signal]', *, endianness: Endianness, word_length_in_bits: int = 8):
+		signals = list(signals)
+		signals.sort(key=lambda s: s.address*word_length_in_bits + s.startbit)
+
 		self.message_spec = message_spec
 		self.endianness = endianness
 		self.word_length_in_bits = word_length_in_bits
 		self.signals = signals
 
 		for i in range(len(self.message_spec)):
 			length = self.message_spec[i].length
@@ -241,15 +276,15 @@
 			if s.name in used_names:
 				raise ValueError(f"there are two signals with the same name {s.name!r}")
 
 			i0 = self.get_start_bit(s)
 			i1 = i0 + s.bits
 			if i0 < last_i1:
 				assert last_signal is not None
-				raise ValueError(f"{s.name!r} overlaps with {last_signal.name!r} or they are not ordered correctly, signals must be ordered by address + startbit ascending")
+				raise ValueError(f"{s.name!r} overlaps with {last_signal.name!r}")
 
 			last_signal = s
 			last_i1 = i1
 
 	def get_endianness_fmt(self) -> str:
 		# "where > means most significant byte first and < means least significant byte first."
 		#https://bitstruct.readthedocs.io/en/latest/#bitstruct.pack
```

### Comparing `serialtools-0.2.1/src/serialtools/database_config.py` & `serialtools-0.3.0/src/serialtools/database_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,26 +75,27 @@
 			out.append(v)
 
 		return out
 
 
 class Message(ConfigFileArgparseCommand):
 
-	message: 'list[db.ByteSpec]|None' = None
+	message: 'db.MessageSpec|None' = None
 
 	def init_parser(self, parser: argparse.ArgumentParser) -> None:
+		parser.add_argument('--implicit-address', '-a', type=int)
 		parser.add_argument('parameters', nargs="+")
 
 	def run_parsed(self, args: argparse.Namespace) -> None:
 		out: 'list[db.ByteSpec]' = []
 		for param_name in args.parameters:
 			if not param_name in Param.defined_parameters:
 				raise ParseException(f"Undefined parameter: {param_name!r}")
 			out.append(Param.defined_parameters[param_name])
-		type(self).message = out
+		type(self).message = db.MessageSpec(out, implicit_address=args.implicit_address)
 
 class Signal(ConfigFileArgparseCommand):
 
 	signals: 'list[db.Signal]' = []
 
 	def init_parser(self, parser: argparse.ArgumentParser) -> None:
 		parser.add_argument('name', help="The name of the signal")
@@ -110,16 +111,16 @@
 		self.signals.append(db.Signal(args.name, args.type, args.address, bits=args.bits, startbit=args.startbit, scale=args.scale, offset=args.offset, unit=args.unit))
 
 class DatabaseCreator:
 
 	word_length_in_bits = Config('db.word-size', 8, unit='bits')
 	endianness = ExplicitConfig('db.endianness', db.Endianness)
 
-	def get(self) -> db.Database:
+	def get(self, *, require_signals: bool = True) -> db.Database:
 		if not Message.message:
 			raise ValueError(f"message structure not defined")
-		if not Signal.signals:
+		if require_signals and not Signal.signals:
 			raise ValueError("no signals defined")
 		return db.Database(Message.message, Signal.signals, endianness=self.endianness, word_length_in_bits=self.word_length_in_bits)
 
 _db_creator = DatabaseCreator()
 get_database = _db_creator.get
```

### Comparing `serialtools-0.2.1/PKG-INFO` & `serialtools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

