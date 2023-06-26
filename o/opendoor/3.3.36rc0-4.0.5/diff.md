# Comparing `tmp/opendoor-3.3.36rc0.tar.gz` & `tmp/opendoor-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opendoor-3.3.36rc0.tar", last modified: Thu Jun  8 14:38:58 2017, max compression
+gzip compressed data, was "opendoor-4.0.5.tar", last modified: Mon Jun 26 04:38:55 2023, max compression
```

## Comparing `opendoor-3.3.36rc0.tar` & `opendoor-4.0.5.tar`

### file list

```diff
@@ -1,137 +1,152 @@
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      610 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/setup.cfg
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      103 2017-06-07 12:32:37.000000 opendoor-3.3.36rc0/MANIFEST.in
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1269 2017-06-06 10:19:40.000000 opendoor-3.3.36rc0/src/__init__.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/events/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      713 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/events/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      935 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/lib/events/events.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1223 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/lib/__init__.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/io/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      752 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/io/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1385 2017-06-08 09:10:30.000000 opendoor-3.3.36rc0/src/lib/io/arguments.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1171 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/io/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/tpl/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      734 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/tpl/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3865 2017-06-08 10:19:28.000000 opendoor-3.3.36rc0/src/lib/tpl/config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1147 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/tpl/exceptions.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     6675 2017-06-06 09:10:05.000000 opendoor-3.3.36rc0/src/lib/tpl/tpl.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/reporter/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      750 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/reporter/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2526 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/lib/reporter/reporter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      932 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/reporter/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/provider/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      718 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/provider/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2308 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/provider/provider.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1397 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/std.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2046 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/txt.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      960 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1969 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/json.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2030 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/src/lib/reporter/plugins/html.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/package/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      747 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/package/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3372 2017-06-06 12:19:57.000000 opendoor-3.3.36rc0/src/lib/package/config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)    10046 2017-06-08 10:04:30.000000 opendoor-3.3.36rc0/src/lib/package/package.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1163 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/package/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/reader/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      744 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/reader/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      789 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/reader/config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     8829 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/reader/reader.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1159 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/lib/reader/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/lib/browser/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     8788 2017-06-08 10:06:47.000000 opendoor-3.3.36rc0/src/lib/browser/browser.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      746 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/lib/browser/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3861 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/lib/browser/threadpool.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     8658 2017-06-08 10:05:28.000000 opendoor-3.3.36rc0/src/lib/browser/config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2904 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/lib/browser/worker.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     6442 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/lib/browser/debug.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1333 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/lib/browser/filter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1165 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/lib/browser/exceptions.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4819 2017-06-08 10:19:51.000000 opendoor-3.3.36rc0/src/controller.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/logger/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      747 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/logger/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2727 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/core/logger/logger.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4496 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/logger/colorize.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1891 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/logger/config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1857 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/core/logger/exception.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4213 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/core/logger/rainbow.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1976 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/__init__.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/helper/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      707 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/helper/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3006 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/helper/helper.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/http/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      825 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/http/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4912 2017-06-06 12:42:39.000000 opendoor-3.3.36rc0/src/core/http/https.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3526 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/core/http/response.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1712 2017-06-08 09:55:39.000000 opendoor-3.3.36rc0/src/core/http/socks.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3890 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/http/http.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/http/providers/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1844 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/http/providers/request.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      862 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/http/providers/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2246 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/http/providers/accept.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     5641 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/http/providers/response.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2213 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/http/providers/debug.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2447 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/http/providers/header.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1543 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/http/providers/cookies.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2006 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/core/http/exceptions.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4901 2017-06-06 09:09:54.000000 opendoor-3.3.36rc0/src/core/http/proxy.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/decorators/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      714 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/decorators/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1520 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/src/core/decorators/timer.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/system/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      733 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/system/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2884 2017-06-06 09:09:56.000000 opendoor-3.3.36rc0/src/core/system/process.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2020 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/system/output.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3745 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/system/terminal.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      942 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/system/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/color/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      705 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/color/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2249 2017-06-06 09:07:32.000000 opendoor-3.3.36rc0/src/core/color/color.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/filesystem/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      715 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/filesystem/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      945 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/filesystem/exceptions.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     9846 2017-06-07 12:38:53.000000 opendoor-3.3.36rc0/src/core/filesystem/filesystem.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/src/core/options/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      709 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/src/core/options/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)    13311 2017-06-08 09:17:01.000000 opendoor-3.3.36rc0/src/core/options/options.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3593 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/options/filter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1648 2017-06-06 09:09:55.000000 opendoor-3.3.36rc0/src/core/options/exceptions.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      915 2017-06-06 09:10:29.000000 opendoor-3.3.36rc0/src/exceptions.py
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)        1 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/dependency_links.txt
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)       10 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/top_level.txt
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)       27 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/requires.txt
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)       70 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/entry_points.txt
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)    10347 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/PKG-INFO
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3008 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/opendoor.egg-info/SOURCES.txt
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)        1 2017-06-07 14:36:55.000000 opendoor-3.3.36rc0/opendoor.egg-info/not-zip-safe
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)    10347 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/PKG-INFO
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/data/
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)   405308 2017-06-06 08:23:04.000000 opendoor-3.3.36rc0/data/directories.dat
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)     7678 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/data/useragents.dat
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      134 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/data/ignored.dat
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)   910845 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/data/subdomains.dat
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)     5098 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/data/proxies.dat
-drwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)        0 2017-06-08 14:38:58.000000 opendoor-3.3.36rc0/tests/
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1233 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/tests/test_core_terminal.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4670 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_controller.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     2641 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_browser_threadpool.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)      685 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/tests/__init__.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4291 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/tests/test_lib_browser_config.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     7956 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_browser.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1887 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_browser_filter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     5247 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_reporter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4068 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_package.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     8889 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_reader.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1464 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/tests/test_lib_events.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3171 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_browser_debug.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     3835 2017-06-06 08:25:29.000000 opendoor-3.3.36rc0/tests/test_core_options.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1396 2017-06-02 08:14:00.000000 opendoor-3.3.36rc0/tests/test_core_filter.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     5531 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_tpl.py
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     1473 2017-06-06 08:23:05.000000 opendoor-3.3.36rc0/tests/test_lib_browser_worker.py
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)     1207 2017-06-08 10:06:38.000000 opendoor-3.3.36rc0/opendoor.conf
--rw-rw-r--   0 smenshikh  (1000) smenshikh  (1000)     4260 2017-06-08 14:38:21.000000 opendoor-3.3.36rc0/setup.py
--rwxrwxr-x   0 smenshikh  (1000) smenshikh  (1000)     1164 2017-06-06 10:19:28.000000 opendoor-3.3.36rc0/opendoor.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.971245 opendoor-4.0.5/
+-rw-r--r--   0 admin      (501) staff       (20)    33726 2023-06-25 18:07:26.000000 opendoor-4.0.5/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)       85 2023-06-22 22:00:04.000000 opendoor-4.0.5/MANIFEST.in
+-rw-r--r--   0 admin      (501) staff       (20)    10008 2023-06-26 04:38:55.970611 opendoor-4.0.5/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     8870 2023-06-26 04:38:10.000000 opendoor-4.0.5/README.rst
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.895742 opendoor-4.0.5/data/
+-rwxr-xr-x   0 admin      (501) staff       (20)  1068465 2023-06-26 04:09:57.000000 opendoor-4.0.5/data/directories.dat
+-rw-r--r--   0 admin      (501) staff       (20)      187 2023-06-26 04:07:39.000000 opendoor-4.0.5/data/ignored.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     5098 2023-06-22 22:00:04.000000 opendoor-4.0.5/data/proxies.dat
+-rw-r--r--   0 admin      (501) staff       (20)  2213047 2023-06-22 22:00:04.000000 opendoor-4.0.5/data/subdomains.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     7678 2023-06-22 22:00:04.000000 opendoor-4.0.5/data/useragents.dat
+-rwxr-xr-x   0 admin      (501) staff       (20)     1361 2023-06-22 22:00:04.000000 opendoor-4.0.5/opendoor.conf
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.899759 opendoor-4.0.5/opendoor.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    10008 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     3435 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       70 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)       76 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       10 2023-06-26 04:38:55.000000 opendoor-4.0.5/opendoor.egg-info/top_level.txt
+-rwxr-xr-x   0 admin      (501) staff       (20)     1219 2023-06-22 22:34:55.000000 opendoor-4.0.5/opendoor.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-06-26 04:38:55.971401 opendoor-4.0.5/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     4270 2023-06-26 04:38:10.000000 opendoor-4.0.5/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.901872 opendoor-4.0.5/src/
+-rw-r--r--   0 admin      (501) staff       (20)     1414 2023-06-22 22:14:43.000000 opendoor-4.0.5/src/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4958 2023-06-25 21:02:39.000000 opendoor-4.0.5/src/controller.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.903354 opendoor-4.0.5/src/core/
+-rw-r--r--   0 admin      (501) staff       (20)     2064 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.904842 opendoor-4.0.5/src/core/color/
+-rw-r--r--   0 admin      (501) staff       (20)      708 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/color/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2252 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/color/color.py
+-rw-r--r--   0 admin      (501) staff       (20)     4667 2023-06-25 21:05:09.000000 opendoor-4.0.5/src/core/core.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.906189 opendoor-4.0.5/src/core/decorators/
+-rw-r--r--   0 admin      (501) staff       (20)      717 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/decorators/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1523 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/decorators/timer.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.908211 opendoor-4.0.5/src/core/filesystem/
+-rw-r--r--   0 admin      (501) staff       (20)      718 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/filesystem/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      948 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/filesystem/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     9984 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/filesystem/filesystem.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.909410 opendoor-4.0.5/src/core/helper/
+-rw-r--r--   0 admin      (501) staff       (20)      710 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/helper/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     5120 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/helper/helper.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.914797 opendoor-4.0.5/src/core/http/
+-rw-r--r--   0 admin      (501) staff       (20)      828 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2009 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     4485 2023-06-24 18:19:16.000000 opendoor-4.0.5/src/core/http/http.py
+-rw-r--r--   0 admin      (501) staff       (20)     5113 2023-06-24 18:19:16.000000 opendoor-4.0.5/src/core/http/https.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.916517 opendoor-4.0.5/src/core/http/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)      772 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      953 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.919310 opendoor-4.0.5/src/core/http/plugins/response/
+-rw-r--r--   0 admin      (501) staff       (20)     1014 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3409 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/collation.py
+-rw-r--r--   0 admin      (501) staff       (20)     1683 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/file.py
+-rw-r--r--   0 admin      (501) staff       (20)     1695 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/indexof.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.920950 opendoor-4.0.5/src/core/http/plugins/response/provider/
+-rw-r--r--   0 admin      (501) staff       (20)      729 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/provider/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1501 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/provider/provider.py
+-rw-r--r--   0 admin      (501) staff       (20)     1756 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response/skipempty.py
+-rw-r--r--   0 admin      (501) staff       (20)     1672 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/plugins/response_plugin.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.926075 opendoor-4.0.5/src/core/http/providers/
+-rw-r--r--   0 admin      (501) staff       (20)      865 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2261 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/accept.py
+-rw-r--r--   0 admin      (501) staff       (20)     1546 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/cookies.py
+-rw-r--r--   0 admin      (501) staff       (20)     2416 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     2450 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/header.py
+-rw-r--r--   0 admin      (501) staff       (20)     1847 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/request.py
+-rw-r--r--   0 admin      (501) staff       (20)     5515 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/providers/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     5229 2023-06-24 18:19:22.000000 opendoor-4.0.5/src/core/http/proxy.py
+-rw-r--r--   0 admin      (501) staff       (20)     5031 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     2149 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/http/socks.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.930526 opendoor-4.0.5/src/core/logger/
+-rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4499 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/colorize.py
+-rw-r--r--   0 admin      (501) staff       (20)     1832 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1754 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)     2730 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/logger.py
+-rw-r--r--   0 admin      (501) staff       (20)     4216 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/logger/rainbow.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.933047 opendoor-4.0.5/src/core/options/
+-rw-r--r--   0 admin      (501) staff       (20)      712 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/options/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1651 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/options/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     3987 2023-06-22 22:39:58.000000 opendoor-4.0.5/src/core/options/filter.py
+-rw-r--r--   0 admin      (501) staff       (20)    14279 2023-06-22 22:02:04.000000 opendoor-4.0.5/src/core/options/options.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.936093 opendoor-4.0.5/src/core/system/
+-rw-r--r--   0 admin      (501) staff       (20)      736 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/system/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      945 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/system/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     2023 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/system/output.py
+-rw-r--r--   0 admin      (501) staff       (20)     2887 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/system/process.py
+-rw-r--r--   0 admin      (501) staff       (20)     3748 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/core/system/terminal.py
+-rw-r--r--   0 admin      (501) staff       (20)      918 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.936750 opendoor-4.0.5/src/lib/
+-rw-r--r--   0 admin      (501) staff       (20)     1227 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.941203 opendoor-4.0.5/src/lib/browser/
+-rw-r--r--   0 admin      (501) staff       (20)      749 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     9755 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/browser.py
+-rw-r--r--   0 admin      (501) staff       (20)    10273 2023-06-22 22:03:33.000000 opendoor-4.0.5/src/lib/browser/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     6871 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     1168 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     1336 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     3866 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/threadpool.py
+-rw-r--r--   0 admin      (501) staff       (20)     2907 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/browser/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.942274 opendoor-4.0.5/src/lib/events/
+-rw-r--r--   0 admin      (501) staff       (20)      716 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/events/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      938 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/events/events.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.943755 opendoor-4.0.5/src/lib/io/
+-rw-r--r--   0 admin      (501) staff       (20)      755 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/io/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1388 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/io/arguments.py
+-rw-r--r--   0 admin      (501) staff       (20)     1174 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/io/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.945493 opendoor-4.0.5/src/lib/package/
+-rw-r--r--   0 admin      (501) staff       (20)      750 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/package/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1166 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/package/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     9626 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/package/package.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.947770 opendoor-4.0.5/src/lib/reader/
+-rw-r--r--   0 admin      (501) staff       (20)      747 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reader/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      768 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reader/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1162 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reader/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     9530 2023-06-22 22:03:29.000000 opendoor-4.0.5/src/lib/reader/reader.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.949679 opendoor-4.0.5/src/lib/reporter/
+-rw-r--r--   0 admin      (501) staff       (20)      753 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      935 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.952810 opendoor-4.0.5/src/lib/reporter/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)      963 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1980 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/html.py
+-rw-r--r--   0 admin      (501) staff       (20)     1919 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/json.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.953852 opendoor-4.0.5/src/lib/reporter/plugins/provider/
+-rw-r--r--   0 admin      (501) staff       (20)      721 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/provider/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2295 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/provider/provider.py
+-rw-r--r--   0 admin      (501) staff       (20)     1403 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/std.py
+-rw-r--r--   0 admin      (501) staff       (20)     1996 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/plugins/txt.py
+-rw-r--r--   0 admin      (501) staff       (20)     2584 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/reporter/reporter.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.955895 opendoor-4.0.5/src/lib/tpl/
+-rw-r--r--   0 admin      (501) staff       (20)      737 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/tpl/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4061 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/tpl/config.py
+-rw-r--r--   0 admin      (501) staff       (20)     1150 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/tpl/exceptions.py
+-rw-r--r--   0 admin      (501) staff       (20)     6678 2023-06-22 22:00:04.000000 opendoor-4.0.5/src/lib/tpl/tpl.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-06-26 04:38:55.969574 opendoor-4.0.5/tests/
+-rw-r--r--   0 admin      (501) staff       (20)      688 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2947 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_controller.py
+-rw-r--r--   0 admin      (501) staff       (20)     1386 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_core_filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     3825 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_core_options.py
+-rw-r--r--   0 admin      (501) staff       (20)     1228 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_core_terminal.py
+-rw-r--r--   0 admin      (501) staff       (20)     8026 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser.py
+-rw-r--r--   0 admin      (501) staff       (20)     4153 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser_config.py
+-rw-r--r--   0 admin      (501) staff       (20)     3161 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser_debug.py
+-rw-r--r--   0 admin      (501) staff       (20)     1877 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser_filter.py
+-rw-r--r--   0 admin      (501) staff       (20)     2631 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser_threadpool.py
+-rw-r--r--   0 admin      (501) staff       (20)     1463 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_browser_worker.py
+-rw-r--r--   0 admin      (501) staff       (20)     1454 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_events.py
+-rw-r--r--   0 admin      (501) staff       (20)     4205 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_package.py
+-rw-r--r--   0 admin      (501) staff       (20)     9092 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_reader.py
+-rw-r--r--   0 admin      (501) staff       (20)     5287 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_reporter.py
+-rw-r--r--   0 admin      (501) staff       (20)     5521 2023-06-22 22:00:04.000000 opendoor-4.0.5/tests/test_lib_tpl.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opendoor-3.3.36rc0/src/__init__.py` & `opendoor-4.0.5/src/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,34 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import sys
 from .controller import Controller
 from .exceptions import SrcError
 
-for _ in ['urllib3', 'json2html', 'tabulate', 'importlib']:
+for _ in ['urllib3', 'json2html', 'tabulate', 'importlib', 'packaging']:
     try:
         __import__(_)
-    except ImportError:
-        sys.exit("""\t\t[!] Several dependencies wasn't installed!
-            Please run pip install -r requirements.txt """)
+    except ImportError as error:
+        sys.exit("""\t\t[!] Several dependencies wasn't installed! Please run pip install -r requirements.txt. 
+        Details : %s.""" % error)
 
 
 def main():
     """
-    Package loader function
+    This function loads the package and runs the Controller class.
 
-    :except SrcError
+    :except SrcError: Raises an exception if there is an error in the source code.
     :return: None
     """
     try:
         bootstrap = Controller()
         bootstrap.run()
     except SrcError:
         sys.exit()
```

### Comparing `opendoor-3.3.36rc0/src/lib/events/__init__.py` & `opendoor-4.0.5/src/lib/events/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .events import EventHandler
```

### Comparing `opendoor-3.3.36rc0/src/lib/events/events.py` & `opendoor-4.0.5/src/lib/events/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import process
 
 
 class EventHandler(object):
```

### Comparing `opendoor-3.3.36rc0/src/lib/__init__.py` & `opendoor-4.0.5/src/lib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 # noinspection PyPep8Naming
 from .browser import Browser as browser, BrowserError
 # noinspection PyPep8Naming
 from .events import EventHandler as events
 # noinspection PyPep8Naming
@@ -26,7 +26,8 @@
 from .package import Package as package, PackageError
 # noinspection PyPep8Naming
 from .reader import Reader as reader, ReaderError
 # noinspection PyPep8Naming
 from .reporter import Reporter as reporter, ReporterError
 # noinspection PyPep8Naming
 from .tpl import Tpl as tpl, TplError
+
```

### Comparing `opendoor-3.3.36rc0/src/lib/io/__init__.py` & `opendoor-4.0.5/src/lib/package/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,13 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-from .arguments import Arguments
-from .exceptions import ArgumentsError
+
+from .exceptions import PackageError
+from .package import Package
```

### Comparing `opendoor-3.3.36rc0/src/lib/io/arguments.py` & `opendoor-4.0.5/src/lib/io/arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import options, OptionsError
 from src.core import helper
 from .exceptions import ArgumentsError
```

### Comparing `opendoor-3.3.36rc0/src/lib/io/exceptions.py` & `opendoor-4.0.5/src/lib/package/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import exception
 
 
-class ArgumentsError(Exception):
+class PackageError(Exception):
 
-    """ArgumentsError class"""
+    """PackageError class"""
 
     def __init__(self, error):
         """
-        ArgumentsError class constructor
+        PackageError class constructor
         :param str error: error message
         """
 
         class_name = type(error).__name__
 
         if self.__class__.__name__ is not class_name:
             exception.log(class_name=class_name, message=error)
 
-        super(ArgumentsError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
+        super(PackageError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
```

### Comparing `opendoor-3.3.36rc0/src/lib/tpl/__init__.py` & `opendoor-4.0.5/src/core/http/plugins/response/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .tpl import Tpl
-from .exceptions import TplError
+from .provider import ResponsePluginProvider
+
```

### Comparing `opendoor-3.3.36rc0/src/lib/tpl/config.py` & `opendoor-4.0.5/src/lib/tpl/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
 class Config(object):
 
     """Config class"""
 
@@ -31,19 +31,19 @@
         'logged': 'Scanned host has been reported. Press ENTER to rescan or CTRL+C to exit: ',
         'checking_connect': 'Wait, please, checking connect to -> {host}:{port} ...',
         'slow_connection': 'Too slow connection. Please decrease the num of threads and increase the request timeout',
         'online': 'Server {host}:{port} ({ip}) is online!',
         'create_queue_progress': 'Create queue {bar}',
         'scanning': 'Scanning {host} ...',
         'debug': 'Starting debug level {level}. Using scan method: {method} ...',
-        'indexof_act': 'Apache index of/ pages detecting',
         'randomizing': 'Randomizing scan list ...',
         'browser': 'Fetching user-agent: {browser}',
         'directories': 'Read {total} directories list by line',
-        'ext_filter': 'Read {total} directories list by filter: {ext}',
+        'ext_filter': 'Read {total} directories list required only: {ext}',
+        'ext_ignore_filter': 'Read {total} directories list exclude only: {ext}',
         'create_queue': 'Creating queue with {threads} thread(s)...',
         'subdomains': 'Read {total} subdomains list by line...',
         'random_browser': 'Fetching random user-agent per request...',
         'total_time_lvl3': 'Total time running: {time}',
         'thread_limit': 'Threads has been reduced to {max} (max) instead of {threads}',
         'stop_threads': 'Stopping threads ({threads})...',
         'option_prompt': 'Press "[C]ontinue" to resume or "[E]xit" to abort session: ',
@@ -55,18 +55,20 @@
         'http_pool_start': 'Using HTTP keep-alive connection',
         'https_pool_start': 'Using SSL keep-alive connection',
         'proxy_pool_standalone': 'Using custom proxy server: {server}',
         'proxy_pool_internal_start': 'Fetching internal proxy list...',
         'proxy_pool_external_start': 'Fetching external proxy list...',
         'request_header_dbg': 'Request header:\n{dbg}',
         'response_header_dbg': 'Response header:\n{dbg}',
+        'load_sniffer_plugin': 'Load sniffer: {description}',
         'ignored_path': 'Ignored. The path {path} in ignore list',
         'proxy_max_retry_error': 'Skipped. Proxy {proxy} Max retries exceeded: {url}',
         'host_changed_error': 'Block external redirect -> {details}',
-        'read_timeout_error': 'Connection timeout! {url}. Increase using --timeout option',
+        'read_timeout_error': 'Read timeout error! {url}. Increase using --timeout option',
+        'connection_timeout_error': 'Connection timeout error! {url}. Increase using --timeout option',
         'certificat': 'Cert required {url}',
         'success': 'OK {url}',
         'file': 'File {url}',
         'indexof': 'Index {url}',
         'forbidden': 'Denied {url}',
         'auth': 'Auth {url}',
         'redirect': 'R {url} -> {rurl}'
```

### Comparing `opendoor-3.3.36rc0/src/lib/tpl/exceptions.py` & `opendoor-4.0.5/src/lib/reader/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,28 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-
 from src.core import exception
 
 
-class TplError(Exception):
+class ReaderError(Exception):
 
-    """TplError class"""
+    """PackageError class"""
 
     def __init__(self, error):
         """
-        TplError class constructor
+        ReaderError class constructor
         :param str error: error message
         """
 
         class_name = type(error).__name__
 
         if self.__class__.__name__ is not class_name:
             exception.log(class_name=class_name, message=error)
 
-        super(TplError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
+        super(ReaderError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
```

### Comparing `opendoor-3.3.36rc0/src/lib/tpl/tpl.py` & `opendoor-4.0.5/src/lib/tpl/tpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import colour
 from src.core import logger
 from src.core import sys
 from .config import Config
 from .exceptions import TplError
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/__init__.py` & `opendoor-4.0.5/src/core/http/plugins/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .exceptions import ReporterError
-from .reporter import Reporter
+from .exceptions import ResponsePluginError
+from .response_plugin import ResponsePlugin
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/reporter.py` & `opendoor-4.0.5/src/lib/reporter/reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,31 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import importlib
 import os
+from src.core import CoreConfig
 from src.core import filesystem, FileSystemError
 from .exceptions import ReporterError
 
 
 class Reporter(object):
 
     """Reporter class"""
 
     default = 'std'
-    config = 'setup.cfg'
     external_directory = None
+    config = CoreConfig.get('data')
 
     @staticmethod
     def is_reported(resource):
         """
         Check if session is already reported
         :param str resource: target report
         :return: bool
@@ -40,16 +41,15 @@
 
         try:
             if None is not Reporter.external_directory:
                 if not Reporter.external_directory.endswith(os.path.sep):
                     Reporter.external_directory += os.path.sep
                 is_reported = filesystem.is_exist(Reporter.external_directory, resource)
             else:
-                config = filesystem.readcfg(Reporter.config)
-                is_reported = filesystem.is_exist(config.get('opendoor', 'reports'), resource)
+                is_reported = filesystem.is_exist(Reporter.config.get('reports'), resource)
             return is_reported
         except FileSystemError as error:
             raise ReporterError(error)
 
     @staticmethod
     def load(plugin_name, target, data):
         """
@@ -63,11 +63,12 @@
 
         try:
             package_module = importlib.import_module('src.lib.reporter.plugins')
 
             try:
                 report = getattr(package_module, plugin_name)
                 return report(target, data, Reporter.external_directory)
-            except (TypeError, AttributeError, Exception):
-                raise ReporterError('Unable to get reporter `{plugin}`'.format(plugin=plugin_name))
+            except (TypeError, AttributeError, Exception) as error:
+                raise ReporterError('Unable to get reporter `{plugin}`. Reason: {error}'
+                                    .format(plugin=plugin_name, error=error))
         except ImportError:
             raise ReporterError('Unable to get report\'s plugins`')
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/exceptions.py` & `opendoor-4.0.5/src/lib/reporter/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
 class ReporterError(Exception):
 
     """ReporterError class"""
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/provider/__init__.py` & `opendoor-4.0.5/src/core/color/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .provider import PluginProvider
-
+from .color import Color
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/provider/provider.py` & `opendoor-4.0.5/src/lib/reporter/plugins/provider/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,35 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import filesystem, FileSystemError
 from src.lib import tpl
 
 
 class PluginProvider(object):
     """"PluginProvider class"""
     
-    CONFIG_FILE = 'setup.cfg'
     PLUGIN_NAME = 'PluginProvider'
     EXTENSION_SET = '.pp'
     
-    def __init__(self, taget, data):
+    def __init__(self, target, data):
         """
         PluginProvider constructor
-        :param str taget: target host
+        :param str target: target host
         :param dict data: result set
         """
 
-        self._target = str(taget)
+        self._target = str(target)
         self._data = {}
         self.__set_data(data)
 
     def __set_data(self, data):
         """
         Set report data
         :param dict data: report data
@@ -67,12 +66,12 @@
         :param str separator: result separator
         :raise Exception
         :return: None
         """
         
         try:
             filename = "".join((dirname, filesystem.sep, filename, cls.EXTENSION_SET))
-            filesystem.makefile(filename)
+            filename = filesystem.makefile(filename)
             filesystem.writelist(filename, resultset, separator)
             tpl.info(key='report', plugin=cls.PLUGIN_NAME, dest=filesystem.getabsname(filename))
         except FileSystemError as error:
             raise Exception(error)
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/std.py` & `opendoor-4.0.5/src/lib/reporter/plugins/std.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,34 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from tabulate import tabulate
 
 from .provider import PluginProvider
 from src.core import sys
 
 
 class StdReportPlugin(PluginProvider):
     """ StdReportPlugin class"""
 
-    def __init__(self, taget, data, directory=None):
+    def __init__(self, target, data, directory=None):
         """
         PluginProvider constructor
-        :param str taget: target host
+        :param str target: target host
         :param dict data: result set
         """
 
-        PluginProvider.__init__(self, taget, data)
+        PluginProvider.__init__(self, target, data)
         self.directory = directory
 
     def process(self):
         """
         Process data
         :return: str
         """
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/txt.py` & `opendoor-4.0.5/src/lib/reporter/plugins/txt.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,43 +9,42 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .provider import PluginProvider
+from src.core import CoreConfig
 from src.core import filesystem, FileSystemError
 
 
 class TextReportPlugin(PluginProvider):
     """ TextReportPlugin class"""
 
     PLUGIN_NAME = 'TextReport'
     EXTENSION_SET = '.txt'
 
-    def __init__(self, taget, data, directory=None):
+    def __init__(self, target, data, directory=None):
         """
         PluginProvider constructor
-        :param str taget: target host
+        :param str target: target host
         :param dict data: result set
         :param str directory: custom directory
         """
         
-        PluginProvider.__init__(self, taget, data)
+        PluginProvider.__init__(self, target, data)
 
         try:
             if None is directory:
-                config = filesystem.readcfg(self.CONFIG_FILE)
-                directory = config.get('opendoor', 'reports')
-            self.__target_dir = "".join((directory, self._target))
-            filesystem.makedir(self.__target_dir)
+                directory = CoreConfig.get('data').get('reports')
+            self.__target_dir = filesystem.makedir("".join((directory, self._target)))
         except FileSystemError as error:
             raise Exception(error)
 
     def process(self):
         """
         Process data
         :return: str
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/__init__.py` & `opendoor-4.0.5/src/lib/reporter/plugins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 # noinspection PyPep8Naming
 from .std import StdReportPlugin as std
 # noinspection PyPep8Naming
 from .txt import TextReportPlugin as txt
 # noinspection PyPep8Naming
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/json.py` & `opendoor-4.0.5/src/lib/reporter/plugins/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,44 +9,43 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .provider import PluginProvider
+from src.core import CoreConfig
 from src.core import filesystem, FileSystemError
 from src.core import helper
 
 
 class JsonReportPlugin(PluginProvider):
     """ JsonReportPlugin class"""
 
     PLUGIN_NAME = 'JsonReport'
     EXTENSION_SET = '.json'
 
-    def __init__(self, taget, data, directory=None):
+    def __init__(self, target, data, directory=None):
         """
         PluginProvider constructor
-        :param str taget: target host
+        :param str target: target host
         :param dict data: result set
         :param str directory: custom directory
         """
 
-        PluginProvider.__init__(self, taget, data)
+        PluginProvider.__init__(self, target, data)
 
         try:
             if None is directory:
-                config = filesystem.readcfg(self.CONFIG_FILE)
-                directory = config.get('opendoor', 'reports')
-            self.__target_dir = "".join((directory, self._target))
-            filesystem.makedir(self.__target_dir)
+                directory = CoreConfig.get('data').get('reports')
+            self.__target_dir = filesystem.makedir("".join((directory, self._target)))
         except FileSystemError as error:
             raise Exception(error)
 
     def process(self):
         """
         Process data
         :return: str
```

### Comparing `opendoor-3.3.36rc0/src/lib/reporter/plugins/html.py` & `opendoor-4.0.5/src/lib/reporter/plugins/html.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,45 +9,44 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .provider import PluginProvider
+from src.core import CoreConfig
 from src.core import filesystem, FileSystemError
 from json2html.jsonconv import Json2Html
 
 
 class HtmlReportPlugin(PluginProvider):
     """ HtmlReportPlugin class"""
 
     PLUGIN_NAME = 'HtmlReport'
     EXTENSION_SET = '.html'
 
-    def __init__(self, taget, data, directory=None):
+    def __init__(self, target, data, directory=None):
         """
         PluginProvider constructor
-        :param str taget: target host
+        :param str target: target host
         :param dict data: result set
         :param str directory: custom directory
         """
 
-        PluginProvider.__init__(self, taget, data)
+        PluginProvider.__init__(self, target, data)
 
         try:
 
             if None is directory:
-                config = filesystem.readcfg(self.CONFIG_FILE)
-                directory = config.get('opendoor', 'reports')
-            self.__target_dir = "".join((directory, self._target))
-            filesystem.makedir(self.__target_dir)
+                directory = CoreConfig.get('data').get('reports')
+            self.__target_dir = filesystem.makedir("".join((directory, self._target)))
         except FileSystemError as error:
             raise Exception(error)
 
     def process(self):
         """
         Process data
         :return: str
```

### Comparing `opendoor-3.3.36rc0/src/lib/package/__init__.py` & `opendoor-4.0.5/src/lib/reader/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,16 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .exceptions import PackageError
-from .package import Package
 
+class Config(object):
+    """Config class"""
+
+    http_port = 80
+    ssl_port = 443
```

### Comparing `opendoor-3.3.36rc0/src/lib/package/package.py` & `opendoor-4.0.5/src/lib/package/package.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,42 +9,41 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import CoreSystemError, FileSystemError
+from src.core import CoreConfig
 from src.core import filesystem
 from src.core import helper
 from src.core import process
 from src.core import sys
 # noinspection PyPep8Naming
 from src.lib.tpl import Tpl as tpl
-from .config import Config
 from .exceptions import PackageError
 
 
 class Package(object):
-
     """Package class"""
 
     remote_version = None
 
     @staticmethod
     def check_interpreter():
         """
         Get interpreter version
         :return: dict or bool
         """
 
-        versions = Config.params.get('required_versions')
+        versions = CoreConfig.get('info').get('required_versions')
         actual_version = sys.version()
         target_compare = (actual_version == versions.get('minor') or actual_version == versions.get('major'))
         relative_compare = (helper.is_less(versions.get('minor'), actual_version) is True or
                             helper.is_more(actual_version, versions.get('major')) is True)
 
         if target_compare or relative_compare:
             return True
@@ -57,29 +56,29 @@
     @staticmethod
     def examples():
         """
         Load examples of usage
         :return: str
         """
 
-        examples = Config.params.get('examples')
+        examples = CoreConfig.get('examples')
         return examples
 
     @staticmethod
     def banner():
         """
         Load application banner
 
         :raise PackageError
         :return: str
         """
 
         try:
 
-            banner = Config.params.get('banner').format(
+            banner = CoreConfig.get('banner').format(
                 tpl.line('Directories: {0}'.format(Package.__directories_count()), color='blue'),
                 tpl.line('Subdomains: {0}'.format(Package.__subdomains_count()), color='blue'),
                 tpl.line('Browsers: {0}'.format(Package.__browsers_count()), color='blue'),
                 tpl.line('Proxies: {0}'.format(Package.__proxies_count()), color='blue'),
                 tpl.line(Package.__license(), color='blue'))
 
             return banner
@@ -93,129 +92,124 @@
         Load application version
         :raise PackageError
         :return: str
         """
 
         try:
 
-            version = Config.params.get('version').format(Package.__app_name(), Package.__current_version(),
-                                                          Package.__remote_version(), Package.__repo(),
-                                                          Package.__license())
-
+            version = CoreConfig.get('version').format(Package.__app_name(), Package.__current_version(),
+                                                       Package.__remote_version(), Package.__repo(),
+                                                       Package.__license())
             return version
 
         except (FileSystemError, CoreSystemError, PackageError) as error:
             raise PackageError(error)
 
     @staticmethod
     def wizard(config):
         """
         Get application wizard (read from config)
+        :param str config: configuration file
         :raise PackageError
-        :param str config
         :return: str
         """
 
         try:
             config = filesystem.readcfg(config)
+            # noinspection PyProtectedMember
             params = dict(config._sections['general'])
 
-            for key,val in params.items():
+            for key, val in params.items():
                 params[key] = None if val == 'None' else val
                 if None is not params[key]:
                     if params[key].isdigit():
                         params[key] = int(float(params[key]))
-                    elif params[key] in ['True','False']:
+                    elif params[key] in ['True', 'False']:
                         if params[key] == 'True':
                             params[key] = True
                         else:
                             params[key] = False
                     else:
                         params[key] = params[key].strip()
             return params
 
-        #x = None if x == 'None' else x
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def docs():
         """
         Open documentation
         :raise PackageError
         :return: bool
         """
-        docurl = Config.params.get('documentations')
+        docurl = CoreConfig.get('info').get('documentation')
         return helper.openbrowser(docurl)
 
     @staticmethod
     def update():
         """
         Check for update
         :raise PackageError
         :return: str
         """
 
         try:
             if False is sys().is_windows:
-                status = process.execute(Config.params.get('cvsupdate'))
+                status = process.execute(CoreConfig.get('command').get('cvsupdate'))
                 upd_status = tpl.line(status, color='green')
-                msg = Config.params.get('update').format(status=upd_status)
+                msg = CoreConfig.get('update').format(status=upd_status)
             else:
-                msg = Config.params.get('update').format(status=tpl.line(key='upd_win_stat'))
+                msg = CoreConfig.get('update').format(status=tpl.line(key='upd_win_stat'))
             return msg
         except (AttributeError, CoreSystemError) as error:
             raise PackageError(error)
 
     @staticmethod
     def local_version():
         """
         Get application local version
         :raise PackageError
         :return: str
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            return config.get('info', 'version')
+            version = CoreConfig.get('info').get('version')
+            return version
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __app_name():
         """
         Get application name
         :raise PackageError
         :return: str
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            return config.get('info', 'name')
+            name = CoreConfig.get('info').get('name')
+            return name
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __remote_version():
         """
         Get application remote version
         :raise PackageError
         :return: str
         """
 
         if None is Package.remote_version:
 
             try:
-                config = filesystem.readcfg(Config.params.get('cfg'))
-                request_uri = config.get('info', 'setup')
+                request_uri = CoreConfig.get('info').get('remote_version')
                 result = process.execute('curl -sb GET {uri}'.format(uri=request_uri))
-
-                raw = filesystem.readraw(result)
-                Package.remote_version = raw.get('info', 'version')
-
+                Package.remote_version = str(result, "utf-8")
                 return Package.remote_version
 
             except (FileSystemError, CoreSystemError) as error:
                 raise PackageError(error)
         else:
             return Package.remote_version
 
@@ -226,15 +220,14 @@
         :raise PackageError
         :return: str
         """
 
         try:
             local = Package.local_version()
             remote = Package.__remote_version()
-
             if True is helper.is_less(local, remote):
                 current_version = tpl.line(local, color='red')
             else:
                 current_version = tpl.line(local, color='green')
             return current_version
 
         except (FileSystemError, CoreSystemError, PackageError) as error:
@@ -245,44 +238,43 @@
         """
         Get application repository url
         :raise PackageError
         :return: str
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            return config.get('info', 'repository')
+            repository = CoreConfig.get('info').get('repository')
+            return repository
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __license():
         """
         Get application license
         :raise PackageError
         :return: str
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            return config.get('info', 'license')
+            license_info = CoreConfig.get('info').get('license')
+            return license_info
         except FileSystemError as error:
             raise PackageError(str(error))
 
     @staticmethod
     def __directories_count():
         """
         Get number of directories in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            filename = config.get('opendoor', 'directories')
+            filename = CoreConfig.get('data').get('directories')
             count = filesystem.read(filename).__len__()
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
@@ -291,16 +283,15 @@
         """
         Get number of subdomains in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            filename = config.get('opendoor', 'subdomains')
+            filename = CoreConfig.get('data').get('subdomains')
             count = filesystem.read(filename).__len__()
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
@@ -309,16 +300,15 @@
         """
         Get number of browsers in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            filename = config.get('opendoor', 'useragents')
+            filename = CoreConfig.get('data').get('useragents')
             count = filesystem.read(filename).__len__()
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
 
@@ -327,15 +317,14 @@
         """
         Get number of proxies in basic wordlist
         :raise PackageError
         :return: int
         """
 
         try:
-            config = filesystem.readcfg(Config.params.get('cfg'))
-            filename = config.get('opendoor', 'proxies')
+            filename = CoreConfig.get('data').get('proxies')
             count = filesystem.read(filename).__len__()
 
             return count
 
         except FileSystemError as error:
             raise PackageError(str(error))
```

### Comparing `opendoor-3.3.36rc0/src/lib/package/exceptions.py` & `opendoor-4.0.5/src/lib/browser/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,29 +9,28 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-
 from src.core import exception
 
 
-class PackageError(Exception):
+class BrowserError(Exception):
 
-    """PackageError class"""
+    """BrowserError class"""
 
     def __init__(self, error):
         """
-        PackageError class constructor
-        :param str error: error message
+        BrowserError class constructor
+        :param Exception error: error
         """
 
         class_name = type(error).__name__
 
         if self.__class__.__name__ is not class_name:
-            exception.log(class_name=class_name, message=error)
+            exception.log(class_name=class_name, message=str(error))
 
-        super(PackageError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
+        super(BrowserError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
```

### Comparing `opendoor-3.3.36rc0/src/lib/reader/__init__.py` & `opendoor-4.0.5/src/lib/reporter/plugins/provider/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .exceptions import ReaderError
-from .reader import Reader
+from .provider import PluginProvider
```

### Comparing `opendoor-3.3.36rc0/src/lib/reader/config.py` & `opendoor-4.0.5/src/core/system/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-
-class Config(object):
-    """Config class"""
-
-    setup = 'setup.cfg'
-    http_port = 80
-    ssl_port = 443
+from .process import Term
+from .output import Output
```

### Comparing `opendoor-3.3.36rc0/src/lib/reader/reader.py` & `opendoor-4.0.5/src/lib/reader/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,67 +9,55 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import FileSystemError
 from src.core import CoreSystemError
+from src.core import CoreConfig
 from src.core import filesystem
 from src.core import process
 from src.core import sys
+from src.core import helper
 from .config import Config
 from .exceptions import ReaderError
 
 
 class Reader(object):
 
     """Reader class"""
 
     def __init__(self, browser_config):
         """
         Reader constructor
         :param dict browser_config:
         """
 
-        self.__config = self.__load_config()
+        self.__config = CoreConfig.get('data')
         self.__browser_config = browser_config
         self.__useragents = []
         self.__proxies = []
         self.__ignored = []
         self.__counter = 0
 
-    @staticmethod
-    def __load_config():
-        """
-        Load main configuration file
-        :raise ReaderError
-        :return: ConfigParser.RawConfigParser
-        """
-
-        try:
-            config = filesystem.readcfg(Config.setup)
-            return config
-        except FileSystemError as error:
-            raise ReaderError(str(error))
-
     def get_user_agents(self):
         """
         Get user agents from user-agents list
         :raise ReaderError
         :return: list
         """
 
         try:
             if not len(self.__useragents):
-                self.__useragents = filesystem.read(self.__config.get('opendoor', 'useragents'))
+                self.__useragents = filesystem.read(self.__config.get('useragents'))
             return self.__useragents
 
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
 
     def get_ignored_list(self):
         """
@@ -77,15 +65,15 @@
         :raise ReaderError
         :return: list
         """
 
         try:
 
             if not len(self.__ignored):
-                ignored = filesystem.read(self.__config.get('opendoor', 'ignored'))
+                ignored = filesystem.read(self.__config.get('ignored'))
                 for item in ignored:
                     item = item.replace("\n", "")
                     if "/" == item[0]:
                         item = item.strip('/')
                     self.__ignored.append(item)
 
             return self.__ignored
@@ -104,15 +92,15 @@
             if False is self.__browser_config.get('is_standalone_proxy'):
 
                 if True is self.__browser_config.get('is_external_torlist'):
                     self.__proxies = filesystem.read(self.__browser_config.get('torlist'))
                 else:
 
                     if not len(self.__proxies):
-                        self.__proxies = filesystem.read(self.__config.get('opendoor', 'proxies'))
+                        self.__proxies = filesystem.read(self.__config.get('proxies'))
                 return self.__proxies
             else:
                 return []
 
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
 
@@ -122,76 +110,74 @@
         :param dict params: input params
         :param funct loader:  callback function
         :raise ReaderError
         :return: None
         """
 
         try:
-            if True is self.__browser_config.get('use_extensions')\
+            if True is self.__browser_config.get('use_random'):
+                # use randomizing list.dat
+                dirlist = self.__config.get('tmplist')
+            elif True is self.__browser_config.get('use_extensions')\
+                    and 'directories' == self.__browser_config.get('list'):
+                dirlist = self.__config.get('extensionlist')
+            elif True is self.__browser_config.get('use_ignore_extensions')\
                     and 'directories' == self.__browser_config.get('list'):
-                dirlist = self.__config.get('opendoor', 'extensionlist')
-            elif True is self.__browser_config.get('use_random'):
-                dirlist = self.__config.get('opendoor', 'tmplist')
+                dirlist = self.__config.get('ignore_extensionlist')
             else:
                 if True is self.__browser_config.get('is_external_wordlist'):
-                    dirlist = self.__browser_config.get('list')
-                    self.__browser_config.update({'list': 'directories'})
+                    dirlist = self.__browser_config.get('wordlist')
                 else:
-                    dirlist = self.__config.get('opendoor', self.__browser_config.get('list'))
-
+                    dirlist = self.__config.get(self.__browser_config.get('list'))
             filesystem.readline(dirlist, handler=getattr(self, '_{0}__line'.format(self.__browser_config.get('list'))),
                                 handler_params=params, loader=loader)
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
 
     @classmethod
     def _subdomains__line(cls, line, params):
         """
         Read lines from subdomains file
         :param str line: single line
         :param dict params: input params
         :return: str
         """
 
-        line = line.strip("\n")
-        line.strip('/')
+        line = helper.filter_domain_string(line)
 
         host = params.get('host')
         port = params.get('port')
 
         if 'www.' in host:
             host = host.replace("www.", "")
-        
+
         if port is Config.ssl_port or port is Config.http_port:
             port = ''
         else:
             port = ':{0}'.format(port)
 
-        line = "{scheme}{sub}.{host}{port}".format(scheme=params.get('scheme'), host=host, port=port, sub=line)
+        line = "{scheme}{sub}.{host}{port}".format(scheme=params.get('scheme'),
+                                                   host=host,
+                                                   port=port,
+                                                   sub=line)
 
         return line
 
     def _directories__line(self, line, params):
         """
         Read lines from directories file
         :param str line: single line
         :param dict params: input params
         :return: str
         """
 
-        line = line.strip("\n")
-        if True is line.startswith('/'):
-            line = line[1:]
+        line = helper.filter_directory_string(line)
 
         if 'prefix' in self.__browser_config and 0 < len(self.__browser_config.get('prefix')):
             line = self.__browser_config.get('prefix') + line
-
-        if False is line.endswith('/') and False is filesystem.has_extension(line) and '.' not in line:
-            line = '{0}/'.format(line)
-
         port = params.get('port')
 
         if port is Config.ssl_port or port is Config.http_port:
             port = ''
         else:
             port = ':{0}'.format(port)
         line = "{scheme}{host}{port}/{uri}".format(scheme=params.get('scheme'), host=params.get('host'), port=port,
@@ -206,17 +192,17 @@
         :param str output: output list
         :raise ReaderError
         :return: None
         """
 
         try:
 
-            target_file = self.__config.get('opendoor', target)
-            output_file = self.__config.get('opendoor', output)
-            filesystem.makefile(output_file)
+            target_file = self.__config.get(target)
+            tmp_file = self.__config.get(output)
+            output_file = filesystem.makefile(tmp_file)
 
             if False is sys().is_windows:
                 process.execute('shuf {target} -o {output}'.format(target=target_file, output=output_file))
             else:
                 filesystem.shuffle(target=target_file, output=output_file, total=self.total_lines)
         except (CoreSystemError, FileSystemError) as error:
             raise ReaderError(error)
@@ -229,41 +215,68 @@
         :param str output: output list
         :param list extensions: filtered extensions
         :return: None
         """
 
         try:
 
-            target_file = self.__config.get('opendoor', target)
-            output_file = self.__config.get('opendoor', output)
+            target_file = self.__config.get(target)
+            output_file = self.__config.get(output)
 
             dirlist = filesystem.read(target_file)
             dirlist = [i.strip() for i in dirlist]
             pattern = '.*\.' + '|.*\.'.join(extensions)
             newlist = filesystem.filter_file_lines(dirlist, pattern)
             filesystem.makefile(output_file)
             filesystem.writelist(output_file, newlist, '\n')
             self.__counter = len(newlist)
 
         except (CoreSystemError, FileSystemError) as error:
             raise ReaderError(error)
 
+    def filter_by_ignore_extension(self, target, output, extensions):
+        """
+        Specific filter for selected exuensions
+
+        :param str target: target list
+        :param str output: output list
+        :param list extensions: filtered extensions
+        :return: None
+        """
+
+        try:
+
+            target_file = self.__config.get(target)
+            output_file = self.__config.get(output)
+            dirlist = filesystem.read(target_file)
+            dirlist = [i.strip() for i in dirlist]
+            pattern = '^('
+            for ext in extensions:
+                pattern += '(?!\.{0})'.format(ext)
+            pattern += '.)*$'
+            newlist = filesystem.filter_file_lines(dirlist, pattern)
+            filesystem.makefile(output_file)
+            filesystem.writelist(output_file, newlist, '\n')
+            self.__counter = len(newlist)
+
+        except (CoreSystemError, FileSystemError) as error:
+            raise ReaderError(error)
+
     def count_total_lines(self):
         """
         Count total lines inside wordlist
         :raise ReaderError
         :return: int
         """
         try:
-
-            if 0 is self.__counter:
+            if 0 == self.__counter:
                 if True is self.__browser_config.get('is_external_wordlist'):
-                    dirlist = self.__browser_config.get('list')
+                    dirlist = self.__browser_config.get('wordlist')
                 else:
-                    dirlist = self.__config.get('opendoor', self.__browser_config.get('list'))
+                    dirlist = self.__config.get(self.__browser_config.get('list'))
                 self.__counter = len(filesystem.read(dirlist))
 
             return self.__counter
 
         except (TypeError, FileSystemError) as error:
             raise ReaderError(error)
```

### Comparing `opendoor-3.3.36rc0/src/lib/reader/exceptions.py` & `opendoor-4.0.5/tests/test_core_filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,28 +9,35 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-from src.core import exception
 
-
-class ReaderError(Exception):
-
-    """PackageError class"""
-
-    def __init__(self, error):
-        """
-        ReaderError class constructor
-        :param str error: error message
-        """
-
-        class_name = type(error).__name__
-
-        if self.__class__.__name__ is not class_name:
-            exception.log(class_name=class_name, message=error)
-
-        super(ReaderError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
+from __future__ import absolute_import
+import unittest
+from ddt import ddt, data
+from src.core.options.filter import Filter
+
+@ddt
+class TestFilter(unittest.TestCase):
+    """TestFilter class"""
+    
+    @data(
+            {'host': 'example.com', 'port': 80, 'debug': 1},
+            {'host': 'https://example.com', 'port': 223, 'debug': 1},
+            {'host': 'example.com','debug': 1, 'scan': 'directories'},
+            {'host': 'example.com','debug': 1, 'scan': 'subdomains'}
+    )
+    def test_filter(self, args):
+        """ Filter.filter() test """
+        
+        flt = Filter.filter(args)
+        self.assertIs(type(flt), dict)
+
+      
+        
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/browser.py` & `opendoor-4.0.5/src/lib/browser/browser.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import HttpRequestError, HttpsRequestError, ProxyRequestError, ResponseError
 from src.core import SocketError
 from src.core import helper
 from src.core import request_http
 from src.core import request_proxy
@@ -32,15 +32,14 @@
 from .debug import Debug
 from .exceptions import BrowserError
 from .filter import Filter
 from .threadpool import ThreadPool
 
 
 class Browser(Filter):
-
     """ Browser class """
 
     def __init__(self, params):
         """
         Browser constructor
         :param dict params: filtered input params
         :raise BrowserError
@@ -52,40 +51,48 @@
             self.__debug = Debug(self.__config)
             self.__result = {'total': {}, 'items': {}}
             self.__reader = Reader(browser_config={
                 'list': self.__config.scan,
                 'torlist': self.__config.torlist,
                 'use_random': self.__config.is_random_list,
                 'use_extensions': self.__config.is_extension_filter,
+                'use_ignore_extensions': self.__config.is_ignore_extension_filter,
                 'is_external_wordlist': self.__config.is_external_wordlist,
+                'wordlist': self.__config.wordlist,
                 'is_standalone_proxy': self.__config.is_standalone_proxy,
                 'is_external_torlist': self.__config.is_external_torlist,
                 'prefix': self.__config.prefix
             })
 
             if True is self.__config.is_external_reports_dir:
                 Reporter.external_directory = self.__config.reports_dir
-                
-            if True is self.__config.is_extension_filter and self.__config.scan == self.__config.DEFAULT_SCAN:
-                self.__reader.filter_by_extension(target=self.__config.scan,
-                                                  output='extensionlist',
-                                                  extensions=self.__config.extensions
-                                                  )
+
+            if self.__config.scan == self.__config.DEFAULT_SCAN:
+                if True is self.__config.is_extension_filter:
+                    self.__reader.filter_by_extension(target=self.__config.scan,
+                                                      output='extensionlist',
+                                                      extensions=self.__config.extensions
+                                                      )
+                elif True is self.__config.is_ignore_extension_filter:
+                    self.__reader.filter_by_ignore_extension(target=self.__config.scan,
+                                                             output='ignore_extensionlist',
+                                                             extensions=self.__config.ignore_extensions
+                                                             )
             self.__reader.count_total_lines()
 
             Filter.__init__(self, self.__config, self.__reader.total_lines)
 
             self.__pool = ThreadPool(num_threads=self.__config.threads, total_items=self.__reader.total_lines,
                                      timeout=self.__config.delay)
 
             self.__result = {'total': helper.counter(), 'items': helper.list()}
 
             self.__response = response(config=self.__config, debug=self.__debug, tpl=tpl)
 
-        except ReaderError as error:
+        except (ResponseError, ReaderError) as error:
             raise BrowserError(error)
 
     def ping(self):
         """
         Check remote host for available
         :raise: BrowserError
         :return: None
@@ -108,28 +115,35 @@
         """
 
         self.__debug.debug_user_agents()
         self.__debug.debug_list(total_lines=self.__pool.total_items_size)
 
         try:  # beginning scan process
             if True is self.__config.is_random_list:
+                if self.__config.scan == self.__config.DEFAULT_SCAN:
+                    if True is self.__config.is_extension_filter:
+                        setattr(self.__config, 'scan', 'extensionlist')
+                    elif True is self.__config.is_ignore_extension_filter:
+                        setattr(self.__config, 'scan', 'ignore_extensionlist')
+
                 self.__reader.randomize_list(target=self.__config.scan, output='tmplist')
 
             tpl.info(key='scanning', host=self.__config.host)
 
             self.__start_request_provider()
 
             if True is self.__pool.is_started:
                 self.__reader.get_lines(
                     params={
                         'host': self.__config.host,
                         'port': self.__config.port,
                         'scheme': self.__config.scheme
                     },
-                    loader=getattr(self, '_add_urls'.format()))
+                    loader=getattr(self, '_add_urls'.format())
+                )
 
         except (ProxyRequestError, HttpRequestError, HttpsRequestError, ReaderError) as error:
             raise BrowserError(error)
 
     def __start_request_provider(self):
         """
         Start selected request provider
@@ -180,15 +194,15 @@
         """
 
         path = helper.parse_url(url).path.strip("/")
         return path in self.__reader.get_ignored_list()
 
     def _add_urls(self, urllist):
         """
-        Add recieved urllist to threadpool
+        Add received urllist to threadpool
         :param dict urllist: read from dictionary
         :raise KeyboardInterrupt
         :return: None
         """
 
         try:
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/__init__.py` & `opendoor-4.0.5/src/core/filesystem/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .browser import Browser
-from .exceptions import BrowserError
+from .filesystem import FileSystem
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/threadpool.py` & `opendoor-4.0.5/src/lib/browser/threadpool.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import threading
 import time
 from queue import Queue
 
 # noinspection PyPep8Naming
@@ -30,26 +30,26 @@
     """ThreadPool class"""
 
     def __init__(self, num_threads, total_items, timeout):
         """
         Initialize thread pool
         :param int num_threads: active workers
         :param int total_items: total items
-        :param int timeout: delay betwen threads
+        :param int timeout: delay between threads
         """
 
         self.__queue = Queue(num_threads)
         self.__workers = []
         self.total_items_size = total_items
         self.is_started = True
 
         for _ in range(num_threads):
 
             worker = Worker(self.__queue, num_threads, timeout)
-            if False is worker.isAlive():
+            if False is worker.is_alive():
                 worker.setDaemon(True)
                 worker.start()
                 self.__workers.append(worker)
 
     @property
     def size(self):
         """
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/worker.py` & `opendoor-4.0.5/src/lib/browser/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import threading
 import time
 from queue import Empty as QueueEmptyError
 from threading import BoundedSemaphore, Event
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/debug.py` & `opendoor-4.0.5/src/lib/browser/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import helper
 from src.core import sys
 from src.core.http.providers.debug import DebugProvider
 # noinspection PyPep8Naming
 from src.lib.tpl import Tpl as tpl
@@ -37,16 +37,14 @@
         self.__catched = False
         self.__clear = False
         self.__cfg = Config
         self.__level = self.__cfg.debug
 
         if 0 < self.__level:
             tpl.debug(key='debug', level=self.__cfg.debug, method=self.__cfg.method)
-            if True is self.__cfg.is_indexof:
-                tpl.debug(key='indexof_act', method=self.__cfg.method)
 
     @property
     def level(self):
         """
         Get debug level
         :return: int
         """
@@ -74,18 +72,20 @@
         :return: bool
         """
 
         if 0 < self.__level:
             if True is self.__cfg.is_random_list:
                 tpl.debug(key='randomizing')
             if self.__cfg.DEFAULT_SCAN is self.__cfg.scan:
-                if None is self.__cfg.extensions:
-                    tpl.debug(key='directories', total=total_lines)
-                else:
+                if True is self.__cfg.is_extension_filter:
                     tpl.debug(key='ext_filter', total=total_lines, ext=', '.join(self.__cfg.extensions))
+                elif True is self.__cfg.is_ignore_extension_filter:
+                    tpl.debug(key='ext_ignore_filter', total=total_lines, ext=', '.join(self.__cfg.ignore_extensions))
+                else:
+                    tpl.debug(key='directories', total=total_lines)
             else:
                 tpl.debug(key='subdomains', total=total_lines)
             tpl.debug(key='create_queue', threads=self.__cfg.threads)
 
         return True
 
     def debug_connection_pool(self, keymsg, pool):
@@ -172,30 +172,43 @@
         elif status in ['redirect']:
             request_uri = tpl.line(key='redirect', color='blue', url=urlpath,
                                    rurl=kwargs.get('redirect_uri'))
 
         self.__clear = True if self.__catched else False
 
         if status in ['success', 'file', 'bad', 'forbidden', 'redirect', 'indexof', 'certificat', 'auth']:
-            
+
+            sys.writels("", flush=True)
             tpl.info(key='get_item',
                      clear=self.__clear,
                      percent=percentage,
                      current='{0:0{l}d}'.format(kwargs.get('items_size', 0), l=total_len),
                      total=kwargs.get('total_size', 1),
                      item=request_uri,
                      size=kwargs.get('content_size')
                      )
             self.__catched = True
         else:
-            tpl.line_log(key='get_item',
+            if self.__level != -1:
+                tpl.line_log(key='get_item',
                          percent=percentage,
                          current='{0:0{l}d}'.format(kwargs.get('items_size', 0), l=total_len),
                          total=kwargs.get('total_size', 1),
                          item=request_uri,
-                         size=kwargs.get('content_size')
+                         size=kwargs.get('content_size'),
                          )
             self.__catched = False
             if kwargs.get('items_size', 0) is kwargs.get('total_size', 1):
                 sys.writels("", flush=True)
 
         return True
+
+    def debug_load_sniffer_plugin(self, description):
+        """
+        Debug load sniffers plugin
+        :param str description: plugin description
+        :return: bool
+        """
+
+        tpl.debug(key='load_sniffer_plugin', description=description)
+
+        return True
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/filter.py` & `opendoor-4.0.5/src/lib/browser/filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 # noinspection PyPep8Naming
 from src.lib.tpl import Tpl as tpl
 
 
 class Filter(object):
```

### Comparing `opendoor-3.3.36rc0/src/lib/browser/exceptions.py` & `opendoor-4.0.5/src/lib/tpl/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,29 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
+
 from src.core import exception
 
 
-class BrowserError(Exception):
+class TplError(Exception):
 
-    """BrowserError class"""
+    """TplError class"""
 
     def __init__(self, error):
         """
-        BrowserError class constructor
-        :param Exception error: error
+        TplError class constructor
+        :param str error: error message
         """
 
         class_name = type(error).__name__
 
         if self.__class__.__name__ is not class_name:
-            exception.log(class_name=class_name, message=str(error))
+            exception.log(class_name=class_name, message=error)
 
-        super(BrowserError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
+        super(TplError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
```

### Comparing `opendoor-3.3.36rc0/src/controller.py` & `opendoor-4.0.5/src/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core.decorators import execution_time
 from src.lib import ArgumentsError
 from src.lib import BrowserError
 from src.lib import PackageError
 from src.lib import ReporterError
@@ -100,44 +100,44 @@
             tpl.message(package.update())
         except (AttributeError, PackageError) as error:
             raise SrcError(error)
 
     @staticmethod
     def docs_action():
         """
-         Show app user guide
-
-         :raise SrcError
-         :return: None
-         """
+        Displays the user guide for the app.
 
+        :raises SrcError: If there is an error with the package or attribute.
+        :return: None
+        """
         try:
             package.docs()
         except (AttributeError, PackageError) as error:
             raise SrcError(error)
 
     @staticmethod
     def version_action():
         """
         Show app version action
 
-        :raise SrcError
+        :raise: SrcError
         :return: None
         """
 
         try:
             tpl.message(package.version())
         except (AttributeError, PackageError) as error:
             raise SrcError(error)
 
     @staticmethod
     def local_version():
         """
-        Show app local version
-        :raise SrcError
+        Returns the local version of the app.
+
+        :raises SrcError: If there is an error retrieving the local version.
         :return: None
         """
 
         try:
             tpl.message(package.local_version())
         except (AttributeError, PackageError) as error:
             raise SrcError(error)
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/__init__.py` & `opendoor-4.0.5/src/lib/io/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,13 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-
-from .exception import LoggerException
-from .logger import Logger
+from .arguments import Arguments
+from .exceptions import ArgumentsError
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/logger.py` & `opendoor-4.0.5/src/core/logger/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import logging
 import logging.config
 import sys
 import time
 from inspect import currentframe
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/colorize.py` & `opendoor-4.0.5/src/core/logger/colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import ctypes
 import logging
 import os
 import re
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/config.py` & `opendoor-4.0.5/src/core/logger/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,38 +9,38 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import os
 
 from src.core import filesystem
+from src.core import CoreConfig
 
 
 def exception_log():
     """
     Get exception log path
     :return: string
     """
 
-    config = filesystem.readcfg('setup.cfg')
-    return filesystem.getabsname(config.get('system', 'exceptions_log'))
+    exception_filelog = CoreConfig.get('data').get('exceptions_log')
+    return filesystem.getabsname(exception_filelog)
 
 
 class Config(object):
 
     """Config class"""
 
     logdir = os.path.dirname(exception_log())
-    legacy_config = "{0}{1}{2}".format(os.path.dirname(__file__), filesystem.sep, 'legacy.conf')
     exceptions = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
             "exception_format": {
                 "format": "%(asctime)s [%(levelname)s] : %(message)s",
                 "datefmt": "%Y-%m-%d %H:%M:%S"
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/exception.py` & `opendoor-4.0.5/src/core/logger/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import inspect
 import logging
 import logging.config
 
 from src.core import filesystem
@@ -37,22 +37,20 @@
         :raise Error
         :return: None
         """
 
         try:
 
             filesystem.makedir(Config.logdir)
-            try:
-                logging.config.dictConfig(Config.exceptions)
-            except AttributeError:
-                logging.config.fileConfig(Config.legacy_config)
+            logging.config.dictConfig(Config.exceptions)
             logger = logging.getLogger('exceptions')
             func = inspect.currentframe().f_back.f_code
             message = "{class_name}: {message} in {file} -> {func}() line {line}".format(
                     class_name=class_name,
                     message=message,
                     file=func.co_filename,
                     func=func.co_name,
                     line=func.co_firstlineno)
             logger.error(message)
-        except (Exception, ValueError) as error:
-            raise Exception(error)
+        except (Exception, ValueError):
+            # skip error undefined owner
+            pass
```

### Comparing `opendoor-3.3.36rc0/src/core/logger/rainbow.py` & `opendoor-4.0.5/src/core/logger/rainbow.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import logging
 import re
 
 from .colorize import ColorizingStreamHandler
 from src.core.system import Term
```

### Comparing `opendoor-3.3.36rc0/src/core/__init__.py` & `opendoor-4.0.5/src/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,22 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 # noinspection PyPep8Naming
 from .color import Color as colour
+# noinspection PyPep8Naming
+from .core import CoreConfig
+# noinspection PyPep8Naming
 from .decorators import execution_time
 # noinspection PyPep8Naming
 from .filesystem import FileSystem as filesystem
 from .filesystem.exceptions import FileSystemError
 # noinspection PyPep8Naming
 from .helper import Helper as helper
 # noinspection PyPep8Naming
```

### Comparing `opendoor-3.3.36rc0/src/core/helper/__init__.py` & `opendoor-4.0.5/src/core/helper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .helper import Helper
```

### Comparing `opendoor-3.3.36rc0/src/core/http/__init__.py` & `opendoor-4.0.5/src/core/http/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .http import HttpRequest
 from .proxy import Proxy
 from .response import Response
 from .socks import Socket
 from .https import HttpsRequest
```

### Comparing `opendoor-3.3.36rc0/src/core/http/https.py` & `opendoor-4.0.5/src/core/http/https.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from urllib3 import HTTPSConnectionPool, PoolManager, HTTPResponse, disable_warnings
-from urllib3.exceptions import MaxRetryError, ReadTimeoutError, HostChangedError, \
-    SSLError, NewConnectionError, InsecureRequestWarning
+from urllib3 import HTTPSConnectionPool, PoolManager, HTTPResponse, Timeout, disable_warnings
+from urllib3.exceptions import MaxRetryError, ReadTimeoutError, ConnectTimeoutError, \
+    HostChangedError, SSLError, InsecureRequestWarning
 from src.core import helper
 from .exceptions import HttpsRequestError
 from .providers import DebugProvider
 from .providers import RequestProvider
 
 
 class HttpsRequest(RequestProvider, DebugProvider):
@@ -63,69 +63,74 @@
         
     def __https_pool(self):
         """
         Create HTTP connection pool
         :raise HttpsRequestError
         :return: urllib3.HTTPConnectionPool
         """
-        
+
         try:
             pool = HTTPSConnectionPool(
                     host=self.__cfg.host,
                     port=self.__cfg.port,
                     maxsize=self.__cfg.threads,
-                    timeout=self.__cfg.timeout, block=True)
+                    timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
+                    cert_reqs='CERT_NONE',
+                    block=True)
             if self._HTTP_DBG_LEVEL <= self.__debug.level:
                 self.__debug.debug_connection_pool('https_pool_start', pool)
 
             return pool
         except Exception as error:
             raise HttpsRequestError(str(error))
 
     def request(self, url):
         """
         Client request SSL
         :param str url: request uri
         :return: urllib3.HTTPResponse
         """
-        
+
         if self._HTTP_DBG_LEVEL <= self.__debug.level:
             self.__debug.debug_request(self._headers, url, self.__cfg.method)
-        
+
         try:
 
             disable_warnings(InsecureRequestWarning)
 
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:  # directories requests
                 response = self.__pool.request(self.__cfg.method,
                                                helper.parse_url(url).path,
                                                headers=self._headers,
                                                retries=self.__cfg.retries,
                                                assert_same_host=False,
                                                redirect=False)
                 self.cookies_middleware(is_accept=self.__cfg.accept_cookies, response=response)
             else:  # subdomains
-                
+
                 response = PoolManager().request(self.__cfg.method, url,
                                                  headers=self._headers,
                                                  retries=self.__cfg.retries,
                                                  assert_same_host=False,
-                                                 redirect=False)
+                                                 redirect=False,
+                                                 timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout))
             return response
 
         except MaxRetryError:
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
                 self.__tpl.warning(key='max_retry_error', url=helper.parse_url(url).path)
 
         except HostChangedError as error:
             self.__tpl.warning(key='host_changed_error', details=error)
+            pass
 
         except ReadTimeoutError:
-            if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
-                self.__tpl.warning(key='read_timeout_error', url=url)
+            self.__tpl.warning(key='read_timeout_error', url=url)
+            pass
+
+        except ConnectTimeoutError:
+            self.__tpl.warning(key='connection_timeout_error', url=url)
+            pass
 
         except SSLError:
             if self.__cfg.DEFAULT_SCAN != self.__cfg.scan:
                 return self._provide_ssl_auth_required()
-
-        except NewConnectionError as error:
-            raise HttpsRequestError(str(error))
```

### Comparing `opendoor-3.3.36rc0/src/core/http/response.py` & `opendoor-4.0.5/src/core/http/response.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,22 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from src.core import helper
+from src.core.http.socks import Socket
 from .exceptions import ResponseError
 from .providers import ResponseProvider
+from src.core.http.plugins.response_plugin import ResponsePlugin, ResponsePluginError
 
 
 class Response(ResponseProvider):
 
     """Response class"""
 
     def __init__(self, config, debug, **kwargs):
@@ -31,16 +33,39 @@
         :param src.lib.browser.config.Config config: configurations
         :param src.lib.browser.debug.Debug debug: debugger
         """
 
         ResponseProvider.__init__(self, config)
 
         self.__debug = debug
+        self.__config = config
         self.__tpl = kwargs.get('tpl')
 
+        if True is self.__config.is_sniff:
+            try:
+                self.load_sniffers_plugins(self.__config.sniffers)
+            except ResponsePluginError as error:
+                raise ResponseError(str(error))
+
+    def load_sniffers_plugins(self, plugins):
+        """
+
+        :param list plugins: response plugins list
+        :return:
+        """
+
+        for plugin in plugins:
+            try:
+                plg_object = ResponsePlugin.load(plugin)
+                self._response_plugins.append(plg_object)
+                if 0 < self.__debug.level:
+                    self.__debug.debug_load_sniffer_plugin(plg_object.DESCRIPTION)
+            except ResponsePluginError as error:
+                raise ResponsePluginError(str(error))
+
     def handle(self, response, request_url, items_size, total_size, ignore_list):
         """
         Response handler
         :param urllib3.response.HTTPResponse response: response object
         :param str request_url: url from request
         :param int items_size: current items sizes
         :param int total_size: response object
@@ -58,17 +83,25 @@
                 redirect_uri = None
 
                 if status in ['redirect']:
                     redirect_uri = self._get_redirect_url(request_url, response)
                     check_for_ignored = helper.parse_url(redirect_uri).path[1:]
                     if check_for_ignored in ignore_list:
                         status = 'failed'
-                    url = redirect_uri
+                    if self.__config.SUBDOMAINS_SCAN == self.__config.scan:  # subdomains
+                        ips = Socket.get_ips_addresses(helper.parse_url(request_url).hostname)
+                        url = request_url = '{0} {1}'.format(request_url, ips)
+                    else:
+                        url = redirect_uri
                 else:
-                    url = request_url
+                    if self.__config.SUBDOMAINS_SCAN == self.__config.scan:  # subdomains
+                        ips = Socket.get_ips_addresses(helper.parse_url(request_url).hostname)
+                        url = request_url = '{0} {1}'.format(request_url, ips)
+                    else:
+                        url = request_url
                 self.__debug.debug_request_uri(status=status,
                                                request_uri=request_url,
                                                redirect_uri=redirect_uri,
                                                items_size=items_size,
                                                total_size=total_size,
                                                content_size=ResponseProvider._get_content_size(response)
                                                )
```

### Comparing `opendoor-3.3.36rc0/src/core/http/socks.py` & `opendoor-4.0.5/src/core/http/socks.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import socket
-
 from .exceptions import SocketError
 
 
 class Socket(object):
 
     """Socket class"""
 
@@ -58,7 +57,25 @@
         """
 
         try:
             ip_address = socket.gethostbyname(host)
             return ip_address
         except socket.gaierror as error:
             raise SocketError(str(error))
+
+    @staticmethod
+    def get_ips_addresses(host):
+        """
+        Get remote ip addresses
+        :param str host: target host
+        :return: list
+        """
+
+        try:
+            _, _, ips_list = socket.gethostbyname_ex(host)
+            if not ips_list:
+                ips = ''
+            else:
+                ips = '['+', '.join(ips_list) +']'
+        except socket.gaierror:
+            ips = ''
+        return ips
```

### Comparing `opendoor-3.3.36rc0/src/core/http/http.py` & `opendoor-4.0.5/src/core/http/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from urllib3 import HTTPConnectionPool, PoolManager
-from urllib3.exceptions import MaxRetryError, ReadTimeoutError, HostChangedError, NewConnectionError
+from urllib3 import HTTPConnectionPool, PoolManager, Timeout
+from urllib3.exceptions import MaxRetryError, ReadTimeoutError, ConnectTimeoutError, HostChangedError
 from src.core import helper
 from .exceptions import HttpRequestError
 from .providers import DebugProvider
 from .providers import RequestProvider
 
 
 class HttpRequest(RequestProvider, DebugProvider):
@@ -52,16 +52,20 @@
         """
         Create HTTP connection pool
         :raise HttpRequestError
         :return: urllib3.HTTPConnectionPool
         """
 
         try:
-            pool = HTTPConnectionPool(self.__cfg.host, port=self.__cfg.port, maxsize=self.__cfg.threads,
-                                      timeout=self.__cfg.timeout, block=True)
+            pool = HTTPConnectionPool(self.__cfg.host,
+                                      port=self.__cfg.port,
+                                      maxsize=self.__cfg.threads,
+                                      timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
+                                      cert_reqs='CERT_NONE',
+                                      block=True)
             if self._HTTP_DBG_LEVEL <= self.__debug.level:
                 self.__debug.debug_connection_pool('http_pool_start', pool)
             return pool
         except Exception as error:
             raise HttpRequestError(str(error))
 
     def request(self, url):
@@ -71,29 +75,40 @@
         :return: urllib3.HTTPResponse
         """
 
         if self._HTTP_DBG_LEVEL <= self.__debug.level:
             self.__debug.debug_request(self._headers, url, self.__cfg.method)
         try:
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
-                response = self.__pool.request(self.__cfg.method, helper.parse_url(url).path, headers=self._headers,
-                                               retries=self.__cfg.retries, assert_same_host=True, redirect=False)
+                response = self.__pool.request(self.__cfg.method,
+                                               helper.parse_url(url).path,
+                                               headers=self._headers,
+                                               retries=self.__cfg.retries,
+                                               assert_same_host=True,
+                                               redirect=False)
 
                 self.cookies_middleware(is_accept=self.__cfg.accept_cookies, response=response)
             else:
-                response = PoolManager().request(self.__cfg.method, url, headers=self._headers,
-                                                 retries=self.__cfg.retries, assert_same_host=False, redirect=False)
+                response = PoolManager().request(self.__cfg.method, url,
+                                                 headers=self._headers,
+                                                 retries=self.__cfg.retries,
+                                                 assert_same_host=False,
+                                                 redirect=False,
+                                                 timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout))
             return response
 
         except MaxRetryError:
             if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
                 self.__tpl.warning(key='max_retry_error', url=helper.parse_url(url).path)
+            pass
+
         except HostChangedError as error:
             self.__tpl.warning(key='host_changed_error', details=error)
+            pass
+
         except ReadTimeoutError:
-            if self.__cfg.DEFAULT_SCAN == self.__cfg.scan:
-                self.__tpl.warning(key='read_timeout_error', url=helper.parse_url(url).path)
-        except NewConnectionError as error:
-            if 'subdomains' in self.__cfg.scan:
-                pass
-            else:
-                raise HttpRequestError(str(error))
+            self.__tpl.warning(key='read_timeout_error', url=url)
+            pass
+
+        except ConnectTimeoutError:
+            self.__tpl.warning(key='connection_timeout_error', url=url)
+            pass
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/request.py` & `opendoor-4.0.5/src/core/http/providers/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .cookies import CookiesProvider
 from .header import HeaderProvider
 
 
 class RequestProvider(CookiesProvider, HeaderProvider):
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/__init__.py` & `opendoor-4.0.5/src/core/http/providers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .cookies import CookiesProvider
 from .debug import DebugProvider
 from .header import HeaderProvider
 from .request import RequestProvider
 from .response import ResponseProvider
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/accept.py` & `opendoor-4.0.5/src/core/http/providers/accept.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import random
 
 
 class AcceptHeaderProvider(object):
     """ AcceptHeaderProvider class"""
@@ -30,15 +30,15 @@
         self.__accept = ('*.*, q=0.1',
                          'text/plain,*/*;q=0.8',
                          'text/html,*/*;q=0.8',
                          'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
                          'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8'
                          )
 
-        self.__accept_encoding = ('gzip, deflate, sdch', 'gzip, deflate, br')
+        self.__accept_encoding = ('gzip, deflate, sdch', 'gzip, deflate, br', 'identity')
 
         self.__accept_language = (
             'en-US,en;q=0.5,ru-RU,ru;q=0.8',
             'ru-RU,ru;q=0.8,en-US;q=0.6,en;q=0.4,uk;q=0.2,es;q=0.2,pl;q=0.2',
             'en,en-gb;q=0.8, en;q=0.7'
         )
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/response.py` & `opendoor-4.0.5/src/core/http/providers/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,55 +9,42 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import re
 from src.core import filesystem
 from src.core import helper
 
 
 class ResponseProvider(object):
     """ ResponseProvider class"""
 
     HTTP_DBG_LEVEL = 3
-    INDEX_OF_TITLE = 'Index of /'
-    DEFAULT_SOURCE_DETECT_MIN_SIZE = 1000000
     DEFAULT_HTTP_SUCCESS_STATUSES = [100, 101, 200, 201, 202, 203, 204, 205, 206, 207, 208]
-    DEFAULT_HTTP_REDIRECT_STATUSES = [301, 302, 303, 304, 307, 308]
-    DEFAULT_HTTP_FAILED_STATUSES = [404, 406, 412, 429, 500, 501, 502, 503, 504, 522]
+    DEFAULT_HTTP_REDIRECT_STATUSES = [300, 301, 302, 303, 304, 307, 308]
+    DEFAULT_HTTP_FAILED_STATUSES = [404, 406, 410, 409, 412, 424, 429, 440, 500, 501, 502, 503, 504, 520, 522]
     DEFAULT_SSL_CERT_REQUIRED_STATUSES = [423, 496]
-    DEFAULT_HTTP_FORBIDDEN_STATUSES = [403]
+    DEFAULT_HTTP_FORBIDDEN_STATUSES = [403,405]
     DEFAULT_HTTP_AUTH_STATUSES = [401]
-    DEFAULT_HTTP_BAD_REQUEST_STATUSES = [400, 415]
+    DEFAULT_HTTP_BAD_REQUEST_STATUSES = [400, 415, 508]
 
     def __init__(self, config):
         """
         Response instance
         :param src.lib.browser.config.Config config: configurations
         """
 
         self._cfg = config
-
-    def is_indexof(self, content):
-        """
-        Check response as index of/ page
-        :param str content: response data
-        :return: bool
-        """
-
-        title = re.search('<title>(.+?)</title>', content, re.IGNORECASE | re.DOTALL)
-        if None is not re.search(self.INDEX_OF_TITLE, title.group(1), re.IGNORECASE):
-            return True
-        return False
+        self._response_plugins = []
 
     @classmethod
     def _get_redirect_url(cls, url, response):
         """
         Get redirect url
         :param str url: redirect url
         :param urllib3.response.HTTPResponse response: response object
@@ -83,48 +70,39 @@
         Detect response by status code
         :param str request_url: request url
         :param urllib3.response.HTTPResponse response: response object
         :raise Exception
         :return: str
         """
 
-        if response.status in self.DEFAULT_HTTP_SUCCESS_STATUSES:
-            if 'Content-Length' in response.headers:
-                if self.DEFAULT_SOURCE_DETECT_MIN_SIZE <= int(response.headers['Content-Length']):
-                    return 'file'
-                if True is self._cfg.is_indexof:
-                    if True is self.is_indexof(response.data):
-                        return 'indexof'
-            return 'success'
-        elif response.status in self.DEFAULT_HTTP_FAILED_STATUSES:
-            return 'failed'
-        elif response.status in self.DEFAULT_SSL_CERT_REQUIRED_STATUSES:
-            return 'certificat'
-        elif response.status in self.DEFAULT_HTTP_REDIRECT_STATUSES:
-            location = response.get_redirect_location()
-            if location is not False and location is not None:
-                urlfrag = helper.parse_url(request_url)
-                redirect_url = location.rstrip('/')
-
-                redirectfrag = helper.parse_url(redirect_url)
-                url = "{0}://{1}".format(urlfrag.scheme, urlfrag.netloc)
-                if url == redirect_url \
-                        or (0 < len(redirectfrag.query) and redirectfrag.query in urlfrag.path):
-                    return 'failed'
-                return 'redirect'
-            else:
+        status = None
+        for _, resp_plugin in enumerate(self._response_plugins):
+            status = resp_plugin.process(response)
+            if None is not status:
+                break
+
+        if None is status:
+            if response.status in self.DEFAULT_HTTP_SUCCESS_STATUSES:
+                return 'success'
+            elif response.status in self.DEFAULT_HTTP_FAILED_STATUSES:
                 return 'failed'
-        elif response.status in self.DEFAULT_HTTP_BAD_REQUEST_STATUSES:
-            return 'bad'
-        elif response.status in self.DEFAULT_HTTP_FORBIDDEN_STATUSES:
-            return 'forbidden'
-        elif response.status in self.DEFAULT_HTTP_AUTH_STATUSES:
-            return 'auth'
+            elif response.status in self.DEFAULT_SSL_CERT_REQUIRED_STATUSES:
+                return 'certificat'
+            elif response.status in self.DEFAULT_HTTP_REDIRECT_STATUSES:
+                return self.__is_redirect(response, request_url)
+            elif response.status in self.DEFAULT_HTTP_BAD_REQUEST_STATUSES:
+                return 'bad'
+            elif response.status in self.DEFAULT_HTTP_FORBIDDEN_STATUSES:
+                return 'forbidden'
+            elif response.status in self.DEFAULT_HTTP_AUTH_STATUSES:
+                return 'auth'
+            else:
+                raise Exception('Unknown response status : `{0}`'.format(response.status))
         else:
-            raise Exception('Unknown response status : `{0}`'.format(response.status))
+            return status
 
     def handle(self, response, request_url, items_size, total_size, ignore_list):
         """
         Response handler
         :param urllib3.response.HTTPResponse response: response object
         :param str request_url: url from request
         :param int items_size: current items sizes
@@ -148,7 +126,30 @@
         try:
             size = 0 if not hasattr(response, 'headers') else int(response.headers['Content-Length'])
         except (KeyError, ValueError):
             size = len(response.data)
         finally:
             size = filesystem.human_size(size, 0)
         return size
+
+    @staticmethod
+    def __is_redirect(response, request_url):
+        """
+        Return redirect status
+        :param str request_url: request url
+        :param urllib3.response.HTTPResponse response: response object
+        :return: str
+        """
+
+        location = response.get_redirect_location()
+        if location is not False and location is not None:
+            urlfrag = helper.parse_url(request_url)
+            redirect_url = location.rstrip('/')
+
+            redirectfrag = helper.parse_url(redirect_url)
+            url = "{0}://{1}".format(urlfrag.scheme, urlfrag.netloc)
+            if url == redirect_url \
+                    or (0 < len(redirectfrag.query) and redirectfrag.query in urlfrag.path):
+                return 'failed'
+            return 'redirect'
+        else:
+            return 'failed'
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/debug.py` & `opendoor-4.0.5/src/core/http/providers/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
 class DebugProvider(object):
     """ DebugProvider class"""
 
     @property
@@ -90,7 +90,15 @@
         :param int status: response status
         :param str request_uri: request urli
         :return: bool
         """
 
         pass
 
+    def debug_load_sniffer_plugin(self, description):
+        """
+        Debug load sniffers plugin
+        :param str description: plugin description
+        :return: bool
+        """
+
+        pass
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/header.py` & `opendoor-4.0.5/src/core/http/providers/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import random
 
 from .accept import AcceptHeaderProvider
```

### Comparing `opendoor-3.3.36rc0/src/core/http/providers/cookies.py` & `opendoor-4.0.5/src/core/http/providers/cookies.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from http.cookies import SimpleCookie
 
 
 class CookiesProvider(object):
     """ CookiesProvider class"""
```

### Comparing `opendoor-3.3.36rc0/src/core/http/exceptions.py` & `opendoor-4.0.5/src/core/http/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
 class SocketError(Exception):
 
     """SocketError class"""
```

### Comparing `opendoor-3.3.36rc0/src/core/http/proxy.py` & `opendoor-4.0.5/src/core/http/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import importlib
 import random
 
-from urllib3 import ProxyManager, disable_warnings
+from urllib3 import ProxyManager, Timeout, disable_warnings
 from urllib3.exceptions import DependencyWarning, MaxRetryError, ProxySchemeUnknown,\
     ReadTimeoutError, InsecureRequestWarning
 
 from src.core import helper
 from .exceptions import ProxyRequestError
 from .providers import DebugProvider
 from .providers import RequestProvider
@@ -73,17 +73,24 @@
                 disable_warnings(InsecureRequestWarning)
 
                 if not hasattr(self, '__pm'):
 
                     package_module = importlib.import_module('urllib3.contrib.socks')
                     self.__pm = getattr(package_module, 'SOCKSProxyManager')
 
-                pool = self.__pm(self.__server, num_pools=self.__cfg.threads, timeout=self.__cfg.timeout, block=True)
+                pool = self.__pm(self.__server,
+                                 num_pools=self.__cfg.threads,
+                                 timeout=Timeout(self.__cfg.timeout,
+                                 read=self.__cfg.timeout),
+                                 block=True)
             else:
-                pool = ProxyManager(self.__server, num_pools=self.__cfg.threads, timeout=self.__cfg.timeout, block=True)
+                pool = ProxyManager(self.__server,
+                                    num_pools=self.__cfg.threads,
+                                    timeout=Timeout(connect=self.__cfg.timeout, read=self.__cfg.timeout),
+                                    block=True)
             return pool
         except (DependencyWarning, ProxySchemeUnknown, ImportError) as error:
             raise ProxyRequestError(error)
 
     def request(self, url):
         """
         Client request using Proxy
```

### Comparing `opendoor-3.3.36rc0/src/core/decorators/__init__.py` & `opendoor-4.0.5/src/core/decorators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from .timer import execution_time
```

### Comparing `opendoor-3.3.36rc0/src/core/decorators/timer.py` & `opendoor-4.0.5/src/core/decorators/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import datetime
 import functools
 import time
```

### Comparing `opendoor-3.3.36rc0/src/core/system/__init__.py` & `opendoor-4.0.5/src/core/options/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .process import Term
-from .output import Output
+from .options import Options
```

### Comparing `opendoor-3.3.36rc0/src/core/system/process.py` & `opendoor-4.0.5/src/core/system/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import os
 import signal
 import subprocess
 from .exceptions import CoreSystemError
 from .terminal import Terminal
```

### Comparing `opendoor-3.3.36rc0/src/core/system/output.py` & `opendoor-4.0.5/src/core/system/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import sys
 import platform
 import os
```

### Comparing `opendoor-3.3.36rc0/src/core/system/terminal.py` & `opendoor-4.0.5/src/core/system/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import platform
 import shlex
 import struct
 import subprocess
```

### Comparing `opendoor-3.3.36rc0/src/core/system/exceptions.py` & `opendoor-4.0.5/src/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
-class CoreSystemError(Exception):
+class SrcError(Exception):
 
-    """SystemError class"""
+    """SrcError class"""
 
-    def __init__(self, message):
-        """
-        CoreSystemError class constructor
-        :param str message: error message
+    def __init__(self, error):
         """
+         SrcError class constructor
+         :param str error: error message
+         """
 
-        super(CoreSystemError, self).__init__(message)
+        super(SrcError, self).__init__(error)
```

### Comparing `opendoor-3.3.36rc0/src/core/color/__init__.py` & `opendoor-4.0.5/src/lib/reader/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,11 +9,13 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .color import Color
+from .exceptions import ReaderError
+from .reader import Reader
+
```

### Comparing `opendoor-3.3.36rc0/src/core/color/color.py` & `opendoor-4.0.5/src/core/color/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import sys
 
 
 class Color(object):
```

### Comparing `opendoor-3.3.36rc0/src/core/filesystem/__init__.py` & `opendoor-4.0.5/src/lib/tpl/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,11 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .filesystem import FileSystem
+from .tpl import Tpl
+from .exceptions import TplError
```

### Comparing `opendoor-3.3.36rc0/src/core/filesystem/exceptions.py` & `opendoor-4.0.5/src/core/filesystem/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 
 class FileSystemError(Exception):
 
     """FileSystemError class"""
```

### Comparing `opendoor-3.3.36rc0/src/core/filesystem/filesystem.py` & `opendoor-4.0.5/src/core/filesystem/filesystem.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from configparser import ConfigParser, RawConfigParser, ParsingError, NoOptionError, Error
+from configparser import RawConfigParser, ParsingError, NoOptionError
 import errno
 import os
-from io import StringIO
 import random
 import re
 
 from .exceptions import FileSystemError
 
 
 class FileSystem(object):
@@ -51,24 +50,31 @@
     def makedir(directory, mode=0o777):
         """
         Create new directory
 
         :param str directory: directory
         :param int mode: directory permission
         :raise: FileSystemError
-        :return: None
+        :return: str
         """
 
-        if not os.path.exists(directory):
+        if not os.path.exists(directory) or not os.access(directory,  os.W_OK):
+
             try:
                 directory = os.path.join(directory)
-                os.makedirs(directory + '/', mode=mode)
-            except OSError as error:
-                if error.errno != errno.EEXIST:
-                    raise FileSystemError("Cannot create directory `{0}`. Reason: {1}".format(directory, error))
+                directory += '/'
+                os.makedirs(directory, mode=mode)
+            except OSError:
+                try:
+                    directory = os.path.join(os.path.expanduser('~'), directory)
+                    os.makedirs(directory, mode=mode)
+                except OSError as error:
+                    if error.errno != errno.EEXIST:
+                        raise FileSystemError("Cannot create directory `{0}`. Reason: {1}".format(directory, error))
+        return directory
 
     @staticmethod
     def getabsname(filename):
         """
         Get absolute file path
         :param str filename: directory
         :return: str
@@ -108,25 +114,24 @@
         :param str pattern:
         :return: list
         """
 
         r = re.compile(pattern)
         newlist = filter(r.match, dirlist)
         filteredlist = list(newlist)
-
         return filteredlist
 
     @staticmethod
     def clear(directory, extension=''):
         """
         Clear directory
         :param str directory: os directory
         :param str extension: extension
         :raise: FileSystemError
-        :return: Bool
+        :return: None
         """
 
         if True is os.path.exists(directory):
             try:
                 for files in os.listdir(directory):
                     filename = os.path.join(directory, files)
                     file_extension = os.path.splitext(filename)[1]
@@ -139,29 +144,28 @@
 
     @staticmethod
     def makefile(filename):
         """
         Create new file with context
         :param str filename: input filename
         :raise: FileSystemError
-        :return: Bool
+        :return: str
         """
 
         filename = os.path.join(filename)
-
-        if False is os.path.exists(filename):
+        if False is os.path.exists(filename) or False is os.access(filename, os.R_OK):
             try:
-                FileSystem.makedir(os.path.dirname(filename))
-                open(filename, 'w')
-
-                return True
+                directory = FileSystem.makedir(os.path.dirname(filename))
+                abs_filename = os.path.join(directory, os.path.basename(filename))
+                open(abs_filename, 'w')
+                return abs_filename
             except IOError as error:
                 raise FileSystemError(error.strerror)
         else:
-            return False
+            return filename
 
     @staticmethod
     def shuffle(target, output, total):
         """
         Shuffle data in file
         :param str target: target file
         :param str output: suffled file
@@ -209,17 +213,21 @@
         :param func loader: browser
         :raise FileSystemError
         :return: str
         """
 
         filepath = os.path.join(filename)
         if not os.path.isfile(filepath):
-            raise FileSystemError("{0} is not a file ".format(filepath))
+            filepath = os.path.join(os.path.expanduser('~'), filepath)
+            if not os.path.isfile(filepath):
+                raise FileSystemError("{0} is not a file ".format(filepath))
         if not os.access(filepath, os.R_OK):
-            raise FileSystemError("Configuration file {0} can not be read. Setup chmod 0644".format(filepath))
+            filepath = os.path.join(os.path.expanduser('~'), filepath)
+            if not os.access(filepath, os.R_OK):
+                raise FileSystemError("Configuration file {0} can not be read. Setup chmod 0644".format(filepath))
 
         lines = []
         with open(filepath) as f_handler:
             for line in f_handler:
                 lines.append(handler(line, handler_params))
             loader(lines)
 
@@ -248,19 +256,18 @@
         """
         Read .cfg file
         :param str filename: input filename
         :raise FileSystemError
         :return: configparser.RawConfigParser
         """
 
-        #TODO : Win32/64 check this ^(([(\/|\)a-z].*?opendoor.*?)(\/|\\))
         expression = '^([\/a-z].*?opendoor.*?)\/'
-        regex = re.compile(expression, re.IGNORECASE)
-        cwd = regex.search(__file__)
-        os.chdir(cwd.group())
+        find_dir = re.search(expression, __file__, re.IGNORECASE)
+        if None is not find_dir:
+            os.chdir(find_dir.group())
         filepath = os.path.join(os.path.sep, os.getcwd(), filename)
 
         if not os.path.isfile(filepath):
             raise FileSystemError("{0} is not a file ".format(filepath))
         if not os.access(filepath, os.R_OK):
             raise FileSystemError("Configuration file {0} can not be read. Setup chmod 0644".format(filepath))
 
@@ -290,31 +297,14 @@
         if not os.access(filepath, os.W_OK):
             raise FileSystemError("Targeting file {0} is not writable. Please, check access".format(filepath))
 
         with open(filepath, "w") as f_handler:
             f_handler.write(separator.join(data))
 
     @staticmethod
-    def readraw(data):
-        """
-        Read .cfg raw data file
-        :param str data: file data
-        :raise FileSystemError
-        :return: configparser.RawConfigParser
-        """
-
-        buf = StringIO(str(data, "utf-8"))
-        try:
-            config = ConfigParser()
-            config.read_file(buf)
-            return config
-        except Error as error:
-            raise FileSystemError(str(error))
-
-    @staticmethod
     def human_size(size, precision=2):
         """
         Humanize accepted bytes
         :param int size: bytes
         :param int precision: delimiter
         :return:
         """
```

### Comparing `opendoor-3.3.36rc0/src/core/options/__init__.py` & `opendoor-4.0.5/src/lib/reporter/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,11 +9,13 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from .options import Options
+from .exceptions import ReporterError
+from .reporter import Reporter
+
```

### Comparing `opendoor-3.3.36rc0/src/core/options/options.py` & `opendoor-4.0.5/src/core/options/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import sys
 # noinspection PyCompatibility
-from argparse import RawDescriptionHelpFormatter
+from argparse import RawDescriptionHelpFormatter, OPTIONAL
 from .exceptions import ArgumentParserError, ThrowingArgumentParser, OptionsError, FilterError
 from .filter import Filter
 
 
 class Options(object):
 
     """Options class"""
@@ -50,65 +50,59 @@
             {
                 "group": "request",
                 "args": "-p",
                 "argl": "--port",
                 "default": 80,
                 "action": "store",
                 "help": "Custom port (Default 80)",
-                "nargs": 1,
                 "type": int
             },
             {
                 "group": "request",
                 "args": "-m",
                 "argl": "--method",
                 "default": "HEAD",
                 "action": "store",
                 "help": "Request method (use HEAD as default)",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "stream",
                 "args": "-t",
                 "argl": "--threads",
                 "default": 1,
                 "action": "store",
                 "help": "Allowed threads",
-                "nargs": 1,
                 "type": int
             },
             {
                 "group": "request",
                 "args": "-d",
                 "argl": "--delay",
                 "default": 0,
                 "action": "store",
                 "help": "Delay between requests threading",
-                "nargs": 1,
                 "type": float
             },
             {
                 "group": "request",
                 "args": None,
                 "argl": "--timeout",
                 "default": 30,
                 "action": "store",
                 "help": "Request timeout (30 sec default)",
-                "nargs": 1,
                 "type": int
             },
             {
                 "group": "request",
                 "args": "-r",
                 "argl": "--retries",
                 "default": 3,
                 "action": "store",
                 "help": "Max retries to reconnect (default 3)",
-                "nargs": 1,
                 "type": int
             },
             {
                 "group": "request",
                 "args": None,
                 "argl": "--accept-cookies",
                 "default": False,
@@ -118,16 +112,15 @@
             },
             {
                 "group": "debug",
                 "args": None,
                 "argl": "--debug",
                 "default": 0,
                 "action": "store",
-                "help": "Debug level 1 - 3",
-                "nargs": 1,
+                "help": "Debug level -1 (silent), 1 - 3",
                 "type": int
             },
             {
                 "group": "request",
                 "args": None,
                 "argl": "--tor",
                 "default": False,
@@ -138,55 +131,50 @@
             {
                 "group": "request",
                 "args": None,
                 "argl": "--torlist",
                 "default": None,
                 "action": "store",
                 "help": "Path to custom proxylist",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "request",
                 "args": None,
                 "argl": "--proxy",
                 "default": None,
                 "action": "store",
                 "help": "Custom permanent proxy server",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "wordlist",
                 "args": "-s",
                 "argl": "--scan",
                 "default": "directories",
                 "action": "store",
                 "help": "Scan type scan=directories or scan=subdomains",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "wordlist",
                 "args": "-w",
                 "argl": "--wordlist",
                 "default": None,
                 "action": "store",
                 "help": "Path to custom wordlist",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "report",
                 "args": None,
                 "argl": "--reports",
                 "default": "std",
                 "action": "store",
                 "help": "Scan reports (json,std,txt,html)",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "report",
                 "args": None,
                 "argl": "--reports-dir",
                 "default": None,
@@ -216,35 +204,42 @@
             {
                 "group": "wordlist",
                 "args": None,
                 "argl": "--prefix",
                 "default": None,
                 "action": "store",
                 "help": "Append path prefix to scan host",
-                "nargs": 1,
                 "type": str
             },
             {
                 "group": "wordlist",
                 "args": "-e",
                 "argl": "--extensions",
                 "default": None,
                 "action": "store",
-                "help": "Extensions filter -e php,json e.g",
-                "nargs": 1,
+                "help": "Force use selected extensions for scan session -e php,json e.g",
                 "type": str
             },
             {
-                "group": "sniff",
+                "group": "wordlist",
                 "args": "-i",
-                "argl": "--indexof",
-                "default": False,
-                "action": "store_true",
-                "help": "Detect Apache Index of/",
-                "type": bool
+                "argl": "--ignore-extensions",
+                "default": None,
+                "action": "store",
+                "help": "Force ignore extensions for scan session -i aspx,jsp e.g",
+                "type": str
+            },
+            {
+                "group": "sniff",
+                "args": None,
+                "argl": "--sniff",
+                "default": None,
+                "action": "store",
+                "help": "Response sniff plugins (indexof,collation,file,skipempty)",
+                "type": str
             },
             {
                 "group": "app",
                 "args": None,
                 "argl": "--update",
                 "default": False,
                 "action": "store_true",
@@ -281,15 +276,15 @@
             {
                 "group": "app",
                 "args": None,
                 "argl": "--wizard",
                 "default": None,
                 "action": "store",
                 "help": "Run wizard scanner from your config",
-                "nargs": '?',
+                "nargs": OPTIONAL,
                 "const": self.__wizard_conf,
                 "type": str
             }
         ]
 
         groupped = {}
         try:
@@ -300,49 +295,62 @@
 
             for group, description in sorted(__groups.items()):
                 groupped[group] = self.parser.add_argument_group(description)
 
             for i in range(arguments_len):
                 arg = __arguments[i]
 
-                if 'nargs'in arg and arg['nargs'] is '?':
+                if 'nargs' in arg and arg['nargs'] == '?':
                     const = arg['const']
                 else:
                     const = None
 
                 if arg['args'] is None:
                     if bool == arg['type']:
                         groupped[arg['group']].add_argument(arg['argl'],
                                                             default=arg['default'],
                                                             action=arg['action'],
                                                             help=arg['help'])
-                    else:
+                    elif None is not const:
                         groupped[arg['group']].add_argument(arg['argl'],
                                                             default=arg['default'],
                                                             action=arg['action'],
                                                             help=arg['help'],
                                                             nargs=arg['nargs'],
                                                             const=const,
                                                             type=arg['type'])
+                    else:
+                        groupped[arg['group']].add_argument(arg['argl'],
+                                                            default=arg['default'],
+                                                            action=arg['action'],
+                                                            help=arg['help'],
+                                                            type=arg['type'])
                 else:
                     if bool == arg['type']:
                         groupped[arg['group']].add_argument(arg['args'],
                                                             arg['argl'],
                                                             default=arg['default'],
                                                             action=arg['action'],
                                                             help=arg['help'])
-                    else:
+                    elif None is not const:
                         groupped[arg['group']].add_argument(arg['args'],
                                                             arg['argl'],
                                                             default=arg['default'],
                                                             action=arg['action'],
                                                             help=arg['help'],
                                                             nargs=arg['nargs'],
                                                             const=const,
                                                             type=arg['type'])
+                    else:
+                        groupped[arg['group']].add_argument(arg['args'],
+                                                            arg['argl'],
+                                                            default=arg['default'],
+                                                            action=arg['action'],
+                                                            help=arg['help'],
+                                                            type=arg['type'])
 
             self.args = self.parser.parse_args()
         except (ArgumentParserError, KeyError) as error:
             raise OptionsError(error)
 
     def get_arg_values(self):
         """
```

### Comparing `opendoor-3.3.36rc0/src/core/options/filter.py` & `opendoor-4.0.5/src/core/options/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import re
 
 from src.core import helper
 from .exceptions import FilterError
 
 
 class Filter(object):
 
     """Filter class"""
 
-    URL_REGEX = "^(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|(?:[-A-Za-z0-9]+\.)+([A-Za-z]|(?u)\w){2,6}$"
+    URL_REGEX = "^(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|(?:[-A-Za-z0-9]+\.)+([-A-Za-z]|\w){2,8}$"
 
     @staticmethod
     def filter(args):
         """
         Filter options
         :param dict args:
         :return: dict
@@ -52,17 +52,20 @@
                     filtered[key] = value
 
         return filtered
 
     @staticmethod
     def scheme(hostname):
         """
-        Get `host` scheme from input
-        :param str hostname: input hostname
-        :return: str
+        Get the scheme of the input hostname.
+
+        :param hostname: A string representing the input hostname.
+        :type hostname: str
+        :return: A string representing the scheme of the input hostname.
+        :rtype: str
         """
 
         scheme = helper.parse_url(hostname).scheme
         if not scheme:
             scheme = 'http'
         return scheme + "://"
 
@@ -88,19 +91,23 @@
         if not re.search('http', hostname, re.IGNORECASE):
             if re.search('https', hostname, re.IGNORECASE):
                 hostname = "https://" + hostname
             else:
                 hostname = "http://" + hostname
 
         hostname = helper.parse_url(hostname).netloc
-
-        regex = re.compile(r"" + Filter.URL_REGEX + "")
+        regex = re.compile(r"" + Filter.URL_REGEX + "", re.UNICODE)
 
         if not regex.match(hostname):
-            raise FilterError("\"{0}\" is invalid host in --host. Use ip, http(s) or just hostname".format(hostname))
+            try:
+                hostname = helper.decode_hostname(hostname)
+            except UnicodeError as error:
+                raise FilterError("\"{0}\" is invalid host. {1}".format(hostname, str(error)))
+            if not regex.match(hostname):
+                raise FilterError("\"{0}\" is invalid host. Use ip, http(s) or just hostname".format(hostname))
         return hostname
 
     @staticmethod
     def proxy(proxyaddress):
         """
         Input `proxy` param filter
         :param str proxyaddress: input proxy server address
@@ -111,17 +118,17 @@
         proxy = helper.parse_url(proxyaddress)
 
         if proxy.scheme not in ['http', 'https', 'socks4', 'socks5'] or None is proxy.port:
             raise FilterError("\"{0}\" is invalid proxy in --proxy. Use scheme:ip:port format".format(proxyaddress))
         return proxyaddress
 
     @staticmethod
-    def scan(choise):
+    def scan(choose):
         """
         Input `scan` type filter
-        :param str choise: preferred scan type
+        :param str choose: preferred scan type
         :return: str
         """
 
-        if choise not in ['directories', 'subdomains']:
-            choise = 'directories'
-        return choise
+        if choose not in ['directories', 'subdomains']:
+            choose = 'directories'
+        return choose
```

### Comparing `opendoor-3.3.36rc0/src/core/options/exceptions.py` & `opendoor-4.0.5/src/core/options/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 # noinspection PyCompatibility
 from argparse import ArgumentParser
 
 
 class ArgumentParserError(Exception):
```

### Comparing `opendoor-3.3.36rc0/src/exceptions.py` & `opendoor-4.0.5/src/lib/io/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,29 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
+from src.core import exception
 
-class SrcError(Exception):
 
-    """SrcError class"""
+class ArgumentsError(Exception):
+
+    """ArgumentsError class"""
 
     def __init__(self, error):
         """
-         SrcError class constructor
-         :param str error: error message
-         """
+        ArgumentsError class constructor
+        :param str error: error message
+        """
+
+        class_name = type(error).__name__
+
+        if self.__class__.__name__ is not class_name:
+            exception.log(class_name=class_name, message=error)
 
-        super(SrcError, self).__init__(error)
+        super(ArgumentsError, self).__init__("{0}: {1}".format(str(class_name), str(error)))
```

### Comparing `opendoor-3.3.36rc0/opendoor.egg-info/PKG-INFO` & `opendoor-4.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opendoor
-Version: 3.3.36rc0
+Version: 4.0.5
 Summary: OWASP WEB Directory Scanner
 Home-page: https://github.com/stanislav-web/OpenDoor
-Author: Stanislav WEB
-Author-email: stanisov@gmail.com
+Author: Brain Storm Team
+Author-email: nomail@gmail.com
+Maintainer: Brain Storm Team
 License: GPL
 Download-URL: https://github.com/stanislav-web/OpenDoor
-Description: OWASP WEB Directory Scanner [![Twitter](https://img.shields.io/twitter/url/https/github.com/stanislav-web/OpenDoor.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https://github.com/stanislav-web/OpenDoor)
-        ===============================================================================================================================================================================================================================
-        
-        [![Coverage Status](https://coveralls.io/repos/github/stanislav-web/OpenDoor/badge.svg?branch=master)](https://coveralls.io/github/stanislav-web/OpenDoor?branch=master) [![Code Health](https://landscape.io/github/stanislav-web/OpenDoor/master/landscape.svg?style=flat)](https://landscape.io/github/stanislav-web/OpenDoor/master) [![Documentation Status](https://readthedocs.org/projects/opendoor/badge/?version=latest)](http://opendoor.readthedocs.io/?badge=latest)
-        
-        
-        |  Python | Linux  |  OSX | Windows  |
-        |:-:|:-:|:-:|:-:|
-        |3.3|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.4|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.5|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.6|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        
-        **OpenDoor OWASP** is console multifunctional web sites scanner.
-        This application find all possible ways to login, index of/ directories, restricted access points, subdomains, hidden data and large backups.
-        The scanning is performed by the built-in dictionary and external dictionaries as well. Anonymity and speed are provided by means of using proxy servers.
-        Software is written for informational purposes and is open source product under the GPL license.
-            
-        * *Current v3.2.36-rc (04.06.2017)*
-            - Directories - 35888
-            - Subdomains - 101000
-        
-        ***Testing of the software on the live commercial systems and organizations is prohibited!***
-        
-        ![Alt text](http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg "OpenDoor OWASP")
-        
-        #### Implements
-        - [x] multithreading control
-        - [x] scan's reports
-        - [x] directories scanner
-        - [x] subdomains scanner
-        - [x] HTTP(S) (PORT) support
-        - [x] Keep-alive long pooling
-        - [x] HTTP(S)/SOCKS proxies
-        - [x] dynamic request header
-        - [x] custom wordlst's prefixes
-        - [x] custom wordlists, proxies, ignore lists
-        - [x] debug levels (1-3)
-        - [x] extensions filter
-        - [x] custom reports directory
-        - [x] custom config wizard (use random techniques)
-        - [x] analyze techniques
-            * detect redirects
-            * detect index of/ Apache
-            * detect large files
-            * certif required pages
-        - [x] randomization techniques
-            * random user-agent per request
-            * random proxy per request
-            * wordlists shuffling
-        
-        
-        #### Local installation and run
-        ```
-         git clone https://github.com/stanislav-web/OpenDoor.git
-         cd OpenDoor/
-         pip install -r requirements.txt
-         chmod +x opendoor.py
-        
-         python3 opendoor.py --host http://www.example.com
-        ```
-        
-        #### Global installation (Preferably for OS distributions)
-        ```
-         git clone https://github.com/stanislav-web/OpenDoor.git
-         cd OpenDoor/
-         python3 setup.py build && python3 setup.py install
-        
-         opendoor --host http://www.example.com
-        ```
-        
-        
-        #### Updates
-        ```
-         python3 opendoor.py --update
-         opendoor --update
-        ```
-        
-        #### [Changelog](CHANGELOG.md) (last changes)
-        
-        v3.3.36-rc (04.08.2017)
-        -------------------------
-            - Add config wizard (allows you to configure own project)
-            
-        v3.2.36-rc (04.06.2017)
-        -----------------------
-            - Added custom reports directory --reports-dir /home/user/Reports
-            - Added user guide --docs
-            - Reusable proxy requests pooling in --tor, --torlist
-            - Prevent socks5 proxies warnings
-            - Optimizing scan execution
-            - Request's delays allow to use of milliseconds
-            - Python2.7 no longer support
-        
-        #### Help
-        ```
-        usage: opendoor.py [-h] [--host HOST] [-p PORT] [-m METHOD] [-t THREADS]
-                           [-d DELAY] [--timeout TIMEOUT] [-r RETRIES]
-                           [--accept-cookies] [--debug DEBUG] [--tor]
-                           [--torlist TORLIST] [--proxy PROXY] [-s SCAN] [-w WORDLIST]
-                           [--reports REPORTS] [--reports-dir REPORTS_DIR]
-                           [--random-agent] [--random-list] [--prefix PREFIX]
-                           [-e EXTENSIONS] [-i] [--update] [--version] [--examples]
-                           [--docs] [--wizard [WIZARD]]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        required named options:
-          --host HOST           Target host (ip); --host http://example.com
-        
-        Application tools:
-          --update              Update from CVS
-          --version             Get current version
-          --examples            Examples of usage
-          --docs                Read documentation
-          --wizard [WIZARD]     Run wizard scanner from your config
-        
-        Debug tools:
-          --debug DEBUG         Debug level 1 - 3
-        
-        Reports tools:
-          --reports REPORTS     Scan reports (json,std,txt,html)
-          --reports-dir REPORTS_DIR
-                                Path to custom reports dir
-        
-        Request tools:
-          -p PORT, --port PORT  Custom port (Default 80)
-          -m METHOD, --method METHOD
-                                Request method (use HEAD as default)
-          -d DELAY, --delay DELAY
-                                Delay between requests threading
-          --timeout TIMEOUT     Request timeout (30 sec default)
-          -r RETRIES, --retries RETRIES
-                                Max retries to reconnect (default 3)
-          --accept-cookies      Accept and route cookies from responses
-          --tor                 Using built-in proxylist
-          --torlist TORLIST     Path to custom proxylist
-          --proxy PROXY         Custom permanent proxy server
-          --random-agent        Randomize user-agent per request
-        
-        Sniff tools:
-          -i, --indexof         Detect Apache Index of/
-        
-        Stream tools:
-          -t THREADS, --threads THREADS
-                                Allowed threads
-        
-        Wordlist tools:
-          -s SCAN, --scan SCAN  Scan type scan=directories or scan=subdomains
-          -w WORDLIST, --wordlist WORDLIST
-                                Path to custom wordlist
-          --random-list         Shuffle scan list
-          --prefix PREFIX       Append path prefix to scan host
-          -e EXTENSIONS, --extensions EXTENSIONS
-                                Extensions filter -e php,json e.g
-        ```
-        
-        #### Maintainers
-        - @stanislav-web <https://github.com/stanislav-web> (Developer)
-        
-        ### Tests
-        ```
-        pip install  -r requirements-dev.txt
-        coverage run --source=src/ setup.py test
-        ```
-        
-        ### Contributors
-        If  you like to contribute to the development of the project in that case pull requests are open for you.
-        Also, you can suggest an ideas and create a task in my track list
-        
-        [![Issues](https://badge.waffle.io/stanislav-web/OpenDoor.png?label=Ready)](https://waffle.io/stanislav-web/OpenDoor) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)  [![Say Thanks!](https://img.shields.io/badge/SayThanks.io-%E2%98%BC-1EAEDB.svg)](https://saythanks.io/to/stanislav-web)
-        
-        ### Documentation
-        - [Opendoor OWASP CookBook ](https://github.com/stanislav-web/OpenDoor/wiki)
-        - [Issues](https://github.com/stanislav-web/OpenDoor/issues)
-        
-        
 Keywords: owasp scanner,directory scanner,access directory scanner,fuzzer,auth scanner,dir search
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
@@ -196,7 +19,289 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+OWASP WEB Directory Scanner |Twitter|
+=====================================
+
++----------+------------------+------------------+
+| Python   | Linux            | OSX              |
++==========+==================+==================+
+| 3.9      | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+| 3.10     | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+| 3.11     | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+
+**OpenDoor OWASP** is console multifunctional web sites scanner. This
+application find all possible ways to login, index of/ directories, web
+shells, restricted access points, subdomains, hidden data and large
+backups. The scanning is performed by the built-in dictionary and
+external dictionaries as well. Anonymity and speed are provided by means
+of using proxy servers. Software is written for informational purposes
+and is open source product under the GPL license.
+
+is terminated)*** \* *Current 4.0.5 (25.06.2023)*
+- Directories - 82239
+- Subdomains - 181018
+
+***Testing of the software on the live commercial systems and
+organizations is prohibited!***
+
+.. figure:: http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg
+   :alt: OpenDoor OWASP
+
+Implements
+^^^^^^^^^^
+
+-  [x] multithreading control
+-  [x] scan's reports
+-  [x] directories scanner
+-  [x] subdomains scanner
+-  [x] HTTP(S) (PORT) support
+-  [x] Keep-alive long pooling
+-  [x] HTTP(S)/SOCKS proxies
+-  [x] dynamic request header
+-  [x] custom word-list's prefixes
+-  [x] custom word-lists, proxies, ignore lists
+-  [x] debug levels (-1 (silent), 1-3)
+-  [x] extensions filter
+-  [x] custom reports directory
+-  [x] custom config wizard (use random techniques)
+-  [x] analyze techniques
+
+   -  detect redirects
+   -  detect an index of/ Apache
+   -  detect large files
+   -  heuristic detect invalid web pages
+   -  blank success page filter
+   -  certificate required pages
+
+-  [x] randomization techniques
+
+   -  random user-agent per request
+   -  random proxy per request
+   -  word-lists shuffling
+   -  word-lists filters
+
+Install PIP
+^^^^^^^^^^^
+
+::
+
+    curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
+
+Local installation and run
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+::
+
+     git clone https://github.com/stanislav-web/OpenDoor.git
+     cd OpenDoor/
+     pip3 install -r requirements.txt
+     chmod +x opendoor.py
+
+     python3 opendoor.py --host http://www.example.com
+
+Global installation (Preferably for OS distributions)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+::
+
+     git clone https://github.com/stanislav-web/OpenDoor.git
+     cd OpenDoor/
+     python3 setup.py build && python3 setup.py install
+
+     opendoor --host http://www.example.com
+
+Updates
+^^^^^^^
+
+::
+
+     python3 opendoor.py --update
+     opendoor --update
+
+`Changelog <CHANGELOG.md>`__ (last changes)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+v4.0.5 (25.06.2023)
+---------------------------
+
+::
+
+    -   Update dictionary: + 45442 new directories
+
+v4.0.4-stable (24.06.2023)
+---------------------------
+
+::
+
+    -   Fix unit tests and resolve dev requirements
+
+v4.0.3 (24.06.2023)
+------------------------
+
+::
+
+    -   Fix [#ISSUE-44](https://github.com/stanislav-web/OpenDoor/issues/44) ignore invalid SSL by default
+
+v4.0.2 (23.06.2023)
+------------------------
+
+::
+
+    -   Python 3.11 launch fix [#ISSUE-58](https://github.com/stanislav-web/OpenDoor/issues/58) added encoding to setup.py
+
+v4.0.1-beta (23.02.2021)
+------------------------
+
+::
+
+    -   Python 2.6,2.7 is unsupported
+    -   Update directories.dat  36994 -> 37019
+    -   [enhancement] [#PR-40](https://github.com/stanislav-web/OpenDoor/issues/40) added encoding to setup.py
+    -   [bugfix] [#PR-48](https://github.com/stanislav-web/OpenDoor/issues/48) Python 3.9 / 3.10 compatibility
+    -   [bugfix] [#PR-20](https://github.com/stanislav-web/OpenDoor/issues/20) No timeout setup in request
+    -   [enhancement] [#PR-36](https://github.com/stanislav-web/OpenDoor/issues/36) Feature Request: Show only found items
+
+v3.4.481-stable (02.10.2017)
+----------------------------
+
+::
+
+    -   Fixed bugs with externals wordlists
+    -   Added 80018 subdomains
+
+v3.4.47-rc Gained more Power! (05.07.2017)
+------------------------------------------
+
+::
+
+    - Added IPs lookup for subdomains scan
+    - Added missing HTTP statuses
+    - Bugfix: encoding errors (supported cp1251,utf8,utf16) for body analyze
+    - Bugfix: allow to use both --random-list & --extension params
+    - Directory closing slash has been removed
+    - Support Internationalized Domain Names IDNA
+    - Removed --indexof (-i) params
+    - Add --ignore-extensions -i param to ignore selected extension
+    - Added --sniff param to process responses
+        - indexof   (detect Apache Index Of/ directories)
+        - file      (detect large files)
+        - collation (heurisic detect invalid web pages)
+        - skipempty (skip empty valid pages)
+    - Internal dictionaries has been filtered out. Delete all duplicates
+    - Added +990 unique directories (36931)
+
+Help
+^^^^
+
+::
+
+    usage: opendoor.py [-h] [--host HOST] [-p PORT] [-m METHOD] [-t THREADS]
+                       [-d DELAY] [--timeout TIMEOUT] [-r RETRIES]
+                       [--accept-cookies] [--debug DEBUG] [--tor]
+                       [--torlist TORLIST] [--proxy PROXY] [-s SCAN] [-w WORDLIST]
+                       [--reports REPORTS] [--reports-dir REPORTS_DIR]
+                       [--random-agent] [--random-list] [--prefix PREFIX]
+                       [-e EXTENSIONS] [-i IGNORE_EXTENSIONS] [--sniff SNIFF]
+                       [--update] [--version] [--examples] [--docs]
+                       [--wizard [WIZARD]]
+
+    optional arguments:
+      -h, --help            show this help message and exit
+
+    required named options:
+      --host HOST           Target host (ip); --host http://example.com
+
+    Application tools:
+      --update              Update from CVS
+      --version             Get current version
+      --examples            Examples of usage
+      --docs                Read documentation
+      --wizard [WIZARD]     Run wizard scanner from your config
+
+    Debug tools:
+      --debug DEBUG         Debug level -1 (silent), 1 - 3
+
+    Reports tools:
+      --reports REPORTS     Scan reports (json,std,txt,html)
+      --reports-dir REPORTS_DIR
+                            Path to custom reports dir
+
+    Request tools:
+      -p PORT, --port PORT  Custom port (Default 80)
+      -m METHOD, --method METHOD
+                            Request method (use HEAD as default)
+      -d DELAY, --delay DELAY
+                            Delay between requests threading
+      --timeout TIMEOUT     Request timeout (30 sec default)
+      -r RETRIES, --retries RETRIES
+                            Max retries to reconnect (default 3)
+      --accept-cookies      Accept and route cookies from responses
+      --tor                 Using built-in proxylist
+      --torlist TORLIST     Path to custom proxylist
+      --proxy PROXY         Custom permanent proxy server
+      --random-agent        Randomize user-agent per request
+
+    Sniff tools:
+      --sniff SNIFF         Response sniff plugins
+                            (indexof,collation,file,skipempty)
+
+    Stream tools:
+      -t THREADS, --threads THREADS
+                            Allowed threads
+
+    Wordlist tools:
+      -s SCAN, --scan SCAN  Scan type scan=directories or scan=subdomains
+      -w WORDLIST, --wordlist WORDLIST
+                            Path to custom wordlist
+      --random-list         Shuffle scan list
+      --prefix PREFIX       Append path prefix to scan host
+      -e EXTENSIONS, --extensions EXTENSIONS
+                            Force use selected extensions for scan session -e
+                            php,json e.g
+      -i IGNORE_EXTENSIONS, --ignore-extensions IGNORE_EXTENSIONS
+                            Ignore extensions for scan session -i aspx,jsp e.g
+
+Maintainers
+^^^^^^^^^^^
+
+-  @stanislav-web https://github.com/stanislav-web (Developer)
+
+Tests
+^^^^^^^^^^
+
+::
+
+    pip3 install  -r requirements-dev.txt
+    python setup.py test
+
+Contributors
+^^^^^^^^^^^^
+
+If you like to contribute to the development of the project in that case
+pull requests are open for you. Also, you can suggest an ideas and
+create a task in my track list
+
+|License: GPL v3| |Say Thanks!|
+
+Documentation
+^^^^^^^^^^^^^
+
+-  `Opendoor OWASP
+   CookBook <https://github.com/stanislav-web/OpenDoor/wiki>`__
+-  `Issues <https://github.com/stanislav-web/OpenDoor/issues>`__
+
+.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+   :target: http://www.gnu.org/licenses/gpl-3.0
+.. |Say Thanks!| image:: https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg
+   :target: https://saythanks.io/to/stanislav-web
+
+
```

### Comparing `opendoor-3.3.36rc0/opendoor.egg-info/SOURCES.txt` & `opendoor-4.0.5/opendoor.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
+README.rst
 opendoor.conf
 opendoor.py
-setup.cfg
 setup.py
 data/directories.dat
 data/ignored.dat
 data/proxies.dat
 data/subdomains.dat
 data/useragents.dat
 opendoor.egg-info/PKG-INFO
@@ -15,14 +16,15 @@
 opendoor.egg-info/not-zip-safe
 opendoor.egg-info/requires.txt
 opendoor.egg-info/top_level.txt
 src/__init__.py
 src/controller.py
 src/exceptions.py
 src/core/__init__.py
+src/core/core.py
 src/core/color/__init__.py
 src/core/color/color.py
 src/core/decorators/__init__.py
 src/core/decorators/timer.py
 src/core/filesystem/__init__.py
 src/core/filesystem/exceptions.py
 src/core/filesystem/filesystem.py
@@ -31,14 +33,24 @@
 src/core/http/__init__.py
 src/core/http/exceptions.py
 src/core/http/http.py
 src/core/http/https.py
 src/core/http/proxy.py
 src/core/http/response.py
 src/core/http/socks.py
+src/core/http/plugins/__init__.py
+src/core/http/plugins/exceptions.py
+src/core/http/plugins/response_plugin.py
+src/core/http/plugins/response/__init__.py
+src/core/http/plugins/response/collation.py
+src/core/http/plugins/response/file.py
+src/core/http/plugins/response/indexof.py
+src/core/http/plugins/response/skipempty.py
+src/core/http/plugins/response/provider/__init__.py
+src/core/http/plugins/response/provider/provider.py
 src/core/http/providers/__init__.py
 src/core/http/providers/accept.py
 src/core/http/providers/cookies.py
 src/core/http/providers/debug.py
 src/core/http/providers/header.py
 src/core/http/providers/request.py
 src/core/http/providers/response.py
@@ -68,15 +80,14 @@
 src/lib/browser/worker.py
 src/lib/events/__init__.py
 src/lib/events/events.py
 src/lib/io/__init__.py
 src/lib/io/arguments.py
 src/lib/io/exceptions.py
 src/lib/package/__init__.py
-src/lib/package/config.py
 src/lib/package/exceptions.py
 src/lib/package/package.py
 src/lib/reader/__init__.py
 src/lib/reader/config.py
 src/lib/reader/exceptions.py
 src/lib/reader/reader.py
 src/lib/reporter/__init__.py
```

### Comparing `opendoor-3.3.36rc0/PKG-INFO` & `opendoor-4.0.5/opendoor.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opendoor
-Version: 3.3.36rc0
+Version: 4.0.5
 Summary: OWASP WEB Directory Scanner
 Home-page: https://github.com/stanislav-web/OpenDoor
-Author: Stanislav WEB
-Author-email: stanisov@gmail.com
+Author: Brain Storm Team
+Author-email: nomail@gmail.com
+Maintainer: Brain Storm Team
 License: GPL
 Download-URL: https://github.com/stanislav-web/OpenDoor
-Description: OWASP WEB Directory Scanner [![Twitter](https://img.shields.io/twitter/url/https/github.com/stanislav-web/OpenDoor.svg?style=social)](https://twitter.com/intent/tweet?text=Wow:&url=https://github.com/stanislav-web/OpenDoor)
-        ===============================================================================================================================================================================================================================
-        
-        [![Coverage Status](https://coveralls.io/repos/github/stanislav-web/OpenDoor/badge.svg?branch=master)](https://coveralls.io/github/stanislav-web/OpenDoor?branch=master) [![Code Health](https://landscape.io/github/stanislav-web/OpenDoor/master/landscape.svg?style=flat)](https://landscape.io/github/stanislav-web/OpenDoor/master) [![Documentation Status](https://readthedocs.org/projects/opendoor/badge/?version=latest)](http://opendoor.readthedocs.io/?badge=latest)
-        
-        
-        |  Python | Linux  |  OSX | Windows  |
-        |:-:|:-:|:-:|:-:|
-        |3.3|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.4|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.5|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        |3.6|[![Build Status](https://travis-ci.org/stanislav-web/OpenDoor.svg?branch=master)](https://travis-ci.org/stanislav-web/OpenDoor)    | ?  | [![Build status](https://ci.appveyor.com/api/projects/status/3hmrb64ofdssi4qd?svg=true)](https://ci.appveyor.com/project/stanislav-web/opendoor)|
-        
-        **OpenDoor OWASP** is console multifunctional web sites scanner.
-        This application find all possible ways to login, index of/ directories, restricted access points, subdomains, hidden data and large backups.
-        The scanning is performed by the built-in dictionary and external dictionaries as well. Anonymity and speed are provided by means of using proxy servers.
-        Software is written for informational purposes and is open source product under the GPL license.
-            
-        * *Current v3.2.36-rc (04.06.2017)*
-            - Directories - 35888
-            - Subdomains - 101000
-        
-        ***Testing of the software on the live commercial systems and organizations is prohibited!***
-        
-        ![Alt text](http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg "OpenDoor OWASP")
-        
-        #### Implements
-        - [x] multithreading control
-        - [x] scan's reports
-        - [x] directories scanner
-        - [x] subdomains scanner
-        - [x] HTTP(S) (PORT) support
-        - [x] Keep-alive long pooling
-        - [x] HTTP(S)/SOCKS proxies
-        - [x] dynamic request header
-        - [x] custom wordlst's prefixes
-        - [x] custom wordlists, proxies, ignore lists
-        - [x] debug levels (1-3)
-        - [x] extensions filter
-        - [x] custom reports directory
-        - [x] custom config wizard (use random techniques)
-        - [x] analyze techniques
-            * detect redirects
-            * detect index of/ Apache
-            * detect large files
-            * certif required pages
-        - [x] randomization techniques
-            * random user-agent per request
-            * random proxy per request
-            * wordlists shuffling
-        
-        
-        #### Local installation and run
-        ```
-         git clone https://github.com/stanislav-web/OpenDoor.git
-         cd OpenDoor/
-         pip install -r requirements.txt
-         chmod +x opendoor.py
-        
-         python3 opendoor.py --host http://www.example.com
-        ```
-        
-        #### Global installation (Preferably for OS distributions)
-        ```
-         git clone https://github.com/stanislav-web/OpenDoor.git
-         cd OpenDoor/
-         python3 setup.py build && python3 setup.py install
-        
-         opendoor --host http://www.example.com
-        ```
-        
-        
-        #### Updates
-        ```
-         python3 opendoor.py --update
-         opendoor --update
-        ```
-        
-        #### [Changelog](CHANGELOG.md) (last changes)
-        
-        v3.3.36-rc (04.08.2017)
-        -------------------------
-            - Add config wizard (allows you to configure own project)
-            
-        v3.2.36-rc (04.06.2017)
-        -----------------------
-            - Added custom reports directory --reports-dir /home/user/Reports
-            - Added user guide --docs
-            - Reusable proxy requests pooling in --tor, --torlist
-            - Prevent socks5 proxies warnings
-            - Optimizing scan execution
-            - Request's delays allow to use of milliseconds
-            - Python2.7 no longer support
-        
-        #### Help
-        ```
-        usage: opendoor.py [-h] [--host HOST] [-p PORT] [-m METHOD] [-t THREADS]
-                           [-d DELAY] [--timeout TIMEOUT] [-r RETRIES]
-                           [--accept-cookies] [--debug DEBUG] [--tor]
-                           [--torlist TORLIST] [--proxy PROXY] [-s SCAN] [-w WORDLIST]
-                           [--reports REPORTS] [--reports-dir REPORTS_DIR]
-                           [--random-agent] [--random-list] [--prefix PREFIX]
-                           [-e EXTENSIONS] [-i] [--update] [--version] [--examples]
-                           [--docs] [--wizard [WIZARD]]
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-        
-        required named options:
-          --host HOST           Target host (ip); --host http://example.com
-        
-        Application tools:
-          --update              Update from CVS
-          --version             Get current version
-          --examples            Examples of usage
-          --docs                Read documentation
-          --wizard [WIZARD]     Run wizard scanner from your config
-        
-        Debug tools:
-          --debug DEBUG         Debug level 1 - 3
-        
-        Reports tools:
-          --reports REPORTS     Scan reports (json,std,txt,html)
-          --reports-dir REPORTS_DIR
-                                Path to custom reports dir
-        
-        Request tools:
-          -p PORT, --port PORT  Custom port (Default 80)
-          -m METHOD, --method METHOD
-                                Request method (use HEAD as default)
-          -d DELAY, --delay DELAY
-                                Delay between requests threading
-          --timeout TIMEOUT     Request timeout (30 sec default)
-          -r RETRIES, --retries RETRIES
-                                Max retries to reconnect (default 3)
-          --accept-cookies      Accept and route cookies from responses
-          --tor                 Using built-in proxylist
-          --torlist TORLIST     Path to custom proxylist
-          --proxy PROXY         Custom permanent proxy server
-          --random-agent        Randomize user-agent per request
-        
-        Sniff tools:
-          -i, --indexof         Detect Apache Index of/
-        
-        Stream tools:
-          -t THREADS, --threads THREADS
-                                Allowed threads
-        
-        Wordlist tools:
-          -s SCAN, --scan SCAN  Scan type scan=directories or scan=subdomains
-          -w WORDLIST, --wordlist WORDLIST
-                                Path to custom wordlist
-          --random-list         Shuffle scan list
-          --prefix PREFIX       Append path prefix to scan host
-          -e EXTENSIONS, --extensions EXTENSIONS
-                                Extensions filter -e php,json e.g
-        ```
-        
-        #### Maintainers
-        - @stanislav-web <https://github.com/stanislav-web> (Developer)
-        
-        ### Tests
-        ```
-        pip install  -r requirements-dev.txt
-        coverage run --source=src/ setup.py test
-        ```
-        
-        ### Contributors
-        If  you like to contribute to the development of the project in that case pull requests are open for you.
-        Also, you can suggest an ideas and create a task in my track list
-        
-        [![Issues](https://badge.waffle.io/stanislav-web/OpenDoor.png?label=Ready)](https://waffle.io/stanislav-web/OpenDoor) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)  [![Say Thanks!](https://img.shields.io/badge/SayThanks.io-%E2%98%BC-1EAEDB.svg)](https://saythanks.io/to/stanislav-web)
-        
-        ### Documentation
-        - [Opendoor OWASP CookBook ](https://github.com/stanislav-web/OpenDoor/wiki)
-        - [Issues](https://github.com/stanislav-web/OpenDoor/issues)
-        
-        
 Keywords: owasp scanner,directory scanner,access directory scanner,fuzzer,auth scanner,dir search
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
@@ -196,7 +19,289 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+OWASP WEB Directory Scanner |Twitter|
+=====================================
+
++----------+------------------+------------------+
+| Python   | Linux            | OSX              |
++==========+==================+==================+
+| 3.9      | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+| 3.10     | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+| 3.11     | |Build Status|   | |Build Status|   |
++----------+------------------+------------------+
+
+**OpenDoor OWASP** is console multifunctional web sites scanner. This
+application find all possible ways to login, index of/ directories, web
+shells, restricted access points, subdomains, hidden data and large
+backups. The scanning is performed by the built-in dictionary and
+external dictionaries as well. Anonymity and speed are provided by means
+of using proxy servers. Software is written for informational purposes
+and is open source product under the GPL license.
+
+is terminated)*** \* *Current 4.0.5 (25.06.2023)*
+- Directories - 82239
+- Subdomains - 181018
+
+***Testing of the software on the live commercial systems and
+organizations is prohibited!***
+
+.. figure:: http://dl3.joxi.net/drive/2017/01/30/0001/0378/90490/90/e309742b5c.jpg
+   :alt: OpenDoor OWASP
+
+Implements
+^^^^^^^^^^
+
+-  [x] multithreading control
+-  [x] scan's reports
+-  [x] directories scanner
+-  [x] subdomains scanner
+-  [x] HTTP(S) (PORT) support
+-  [x] Keep-alive long pooling
+-  [x] HTTP(S)/SOCKS proxies
+-  [x] dynamic request header
+-  [x] custom word-list's prefixes
+-  [x] custom word-lists, proxies, ignore lists
+-  [x] debug levels (-1 (silent), 1-3)
+-  [x] extensions filter
+-  [x] custom reports directory
+-  [x] custom config wizard (use random techniques)
+-  [x] analyze techniques
+
+   -  detect redirects
+   -  detect an index of/ Apache
+   -  detect large files
+   -  heuristic detect invalid web pages
+   -  blank success page filter
+   -  certificate required pages
+
+-  [x] randomization techniques
+
+   -  random user-agent per request
+   -  random proxy per request
+   -  word-lists shuffling
+   -  word-lists filters
+
+Install PIP
+^^^^^^^^^^^
+
+::
+
+    curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
+
+Local installation and run
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+::
+
+     git clone https://github.com/stanislav-web/OpenDoor.git
+     cd OpenDoor/
+     pip3 install -r requirements.txt
+     chmod +x opendoor.py
+
+     python3 opendoor.py --host http://www.example.com
+
+Global installation (Preferably for OS distributions)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+::
+
+     git clone https://github.com/stanislav-web/OpenDoor.git
+     cd OpenDoor/
+     python3 setup.py build && python3 setup.py install
+
+     opendoor --host http://www.example.com
+
+Updates
+^^^^^^^
+
+::
+
+     python3 opendoor.py --update
+     opendoor --update
+
+`Changelog <CHANGELOG.md>`__ (last changes)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+v4.0.5 (25.06.2023)
+---------------------------
+
+::
+
+    -   Update dictionary: + 45442 new directories
+
+v4.0.4-stable (24.06.2023)
+---------------------------
+
+::
+
+    -   Fix unit tests and resolve dev requirements
+
+v4.0.3 (24.06.2023)
+------------------------
+
+::
+
+    -   Fix [#ISSUE-44](https://github.com/stanislav-web/OpenDoor/issues/44) ignore invalid SSL by default
+
+v4.0.2 (23.06.2023)
+------------------------
+
+::
+
+    -   Python 3.11 launch fix [#ISSUE-58](https://github.com/stanislav-web/OpenDoor/issues/58) added encoding to setup.py
+
+v4.0.1-beta (23.02.2021)
+------------------------
+
+::
+
+    -   Python 2.6,2.7 is unsupported
+    -   Update directories.dat  36994 -> 37019
+    -   [enhancement] [#PR-40](https://github.com/stanislav-web/OpenDoor/issues/40) added encoding to setup.py
+    -   [bugfix] [#PR-48](https://github.com/stanislav-web/OpenDoor/issues/48) Python 3.9 / 3.10 compatibility
+    -   [bugfix] [#PR-20](https://github.com/stanislav-web/OpenDoor/issues/20) No timeout setup in request
+    -   [enhancement] [#PR-36](https://github.com/stanislav-web/OpenDoor/issues/36) Feature Request: Show only found items
+
+v3.4.481-stable (02.10.2017)
+----------------------------
+
+::
+
+    -   Fixed bugs with externals wordlists
+    -   Added 80018 subdomains
+
+v3.4.47-rc Gained more Power! (05.07.2017)
+------------------------------------------
+
+::
+
+    - Added IPs lookup for subdomains scan
+    - Added missing HTTP statuses
+    - Bugfix: encoding errors (supported cp1251,utf8,utf16) for body analyze
+    - Bugfix: allow to use both --random-list & --extension params
+    - Directory closing slash has been removed
+    - Support Internationalized Domain Names IDNA
+    - Removed --indexof (-i) params
+    - Add --ignore-extensions -i param to ignore selected extension
+    - Added --sniff param to process responses
+        - indexof   (detect Apache Index Of/ directories)
+        - file      (detect large files)
+        - collation (heurisic detect invalid web pages)
+        - skipempty (skip empty valid pages)
+    - Internal dictionaries has been filtered out. Delete all duplicates
+    - Added +990 unique directories (36931)
+
+Help
+^^^^
+
+::
+
+    usage: opendoor.py [-h] [--host HOST] [-p PORT] [-m METHOD] [-t THREADS]
+                       [-d DELAY] [--timeout TIMEOUT] [-r RETRIES]
+                       [--accept-cookies] [--debug DEBUG] [--tor]
+                       [--torlist TORLIST] [--proxy PROXY] [-s SCAN] [-w WORDLIST]
+                       [--reports REPORTS] [--reports-dir REPORTS_DIR]
+                       [--random-agent] [--random-list] [--prefix PREFIX]
+                       [-e EXTENSIONS] [-i IGNORE_EXTENSIONS] [--sniff SNIFF]
+                       [--update] [--version] [--examples] [--docs]
+                       [--wizard [WIZARD]]
+
+    optional arguments:
+      -h, --help            show this help message and exit
+
+    required named options:
+      --host HOST           Target host (ip); --host http://example.com
+
+    Application tools:
+      --update              Update from CVS
+      --version             Get current version
+      --examples            Examples of usage
+      --docs                Read documentation
+      --wizard [WIZARD]     Run wizard scanner from your config
+
+    Debug tools:
+      --debug DEBUG         Debug level -1 (silent), 1 - 3
+
+    Reports tools:
+      --reports REPORTS     Scan reports (json,std,txt,html)
+      --reports-dir REPORTS_DIR
+                            Path to custom reports dir
+
+    Request tools:
+      -p PORT, --port PORT  Custom port (Default 80)
+      -m METHOD, --method METHOD
+                            Request method (use HEAD as default)
+      -d DELAY, --delay DELAY
+                            Delay between requests threading
+      --timeout TIMEOUT     Request timeout (30 sec default)
+      -r RETRIES, --retries RETRIES
+                            Max retries to reconnect (default 3)
+      --accept-cookies      Accept and route cookies from responses
+      --tor                 Using built-in proxylist
+      --torlist TORLIST     Path to custom proxylist
+      --proxy PROXY         Custom permanent proxy server
+      --random-agent        Randomize user-agent per request
+
+    Sniff tools:
+      --sniff SNIFF         Response sniff plugins
+                            (indexof,collation,file,skipempty)
+
+    Stream tools:
+      -t THREADS, --threads THREADS
+                            Allowed threads
+
+    Wordlist tools:
+      -s SCAN, --scan SCAN  Scan type scan=directories or scan=subdomains
+      -w WORDLIST, --wordlist WORDLIST
+                            Path to custom wordlist
+      --random-list         Shuffle scan list
+      --prefix PREFIX       Append path prefix to scan host
+      -e EXTENSIONS, --extensions EXTENSIONS
+                            Force use selected extensions for scan session -e
+                            php,json e.g
+      -i IGNORE_EXTENSIONS, --ignore-extensions IGNORE_EXTENSIONS
+                            Ignore extensions for scan session -i aspx,jsp e.g
+
+Maintainers
+^^^^^^^^^^^
+
+-  @stanislav-web https://github.com/stanislav-web (Developer)
+
+Tests
+^^^^^^^^^^
+
+::
+
+    pip3 install  -r requirements-dev.txt
+    python setup.py test
+
+Contributors
+^^^^^^^^^^^^
+
+If you like to contribute to the development of the project in that case
+pull requests are open for you. Also, you can suggest an ideas and
+create a task in my track list
+
+|License: GPL v3| |Say Thanks!|
+
+Documentation
+^^^^^^^^^^^^^
+
+-  `Opendoor OWASP
+   CookBook <https://github.com/stanislav-web/OpenDoor/wiki>`__
+-  `Issues <https://github.com/stanislav-web/OpenDoor/issues>`__
+
+.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPL%20v3-blue.svg
+   :target: http://www.gnu.org/licenses/gpl-3.0
+.. |Say Thanks!| image:: https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg
+   :target: https://saythanks.io/to/stanislav-web
+
+
```

### Comparing `opendoor-3.3.36rc0/data/useragents.dat` & `opendoor-4.0.5/data/useragents.dat`

 * *Files identical despite different names*

### Comparing `opendoor-3.3.36rc0/data/proxies.dat` & `opendoor-4.0.5/data/proxies.dat`

 * *Files identical despite different names*

### Comparing `opendoor-3.3.36rc0/tests/test_core_terminal.py` & `opendoor-4.0.5/tests/test_core_terminal.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from __future__ import absolute_import
-import unittest2 as unittest
+import unittest
 from src.core.system.terminal import Terminal
 from src.core.system.output import Output
 
 @unittest.skipIf(False is Output().is_windows, "Test can run on Windows")
 class TestTerminal(unittest.TestCase):
     """TestTerminal class"""
     
-    def test_get_ts_windows(self):
-        """ Terminal.__get_ts_windows() test """
-        
-        term = getattr(Terminal, '_Terminal__get_ts_windows')()
-        self.assertIsNotNone(term)
+    # def test_get_ts_windows(self):
+    #     """ Terminal.__get_ts_windows() test """
+    #
+    #     term = getattr(Terminal, '_Terminal__get_ts_windows')()
+    #     self.assertIsNotNone(term)
 
         
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser_threadpool.py` & `opendoor-4.0.5/tests/test_lib_browser_threadpool.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from mock import patch
 from src.lib.browser.threadpool import ThreadPool
 from src.core.logger.logger import Logger
 
 
 class TestBrowserThreadPool(unittest.TestCase):
     """TestBrowserThreadPool class"""
```

### Comparing `opendoor-3.3.36rc0/tests/__init__.py` & `opendoor-4.0.5/src/lib/browser/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,12 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-pass
+from .browser import Browser
+from .exceptions import BrowserError
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser_config.py` & `opendoor-4.0.5/tests/test_lib_browser_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,17 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
-
-import unittest2 as unittest
+import unittest
 from src.lib.browser.config import Config
 
 
 class TestBrowserConfig(unittest.TestCase):
     """TestBrowserConfig class"""
 
     def test_config_properties(self):
@@ -41,25 +40,23 @@
 
         self.assertIs(type(Config.host), property)
         self.assertTrue('example.com' is str(Config({'host': 'example.com'}).host))
 
         self.assertIs(type(Config.port), property)
         self.assertTrue(80 is Config({'port': 80}).port)
         
-        self.assertIs(type(Config.is_indexof), property)
-        self.assertFalse(Config({'is_indexof': False}).is_indexof)
-        
         self.assertIs(type(Config.method), property)
         self.assertTrue(str(Config.DEFAULT_HTTP_METHOD) is str(Config({'method' : 'HEAD'}).method))
 
         self.assertIs(type(Config.delay), property)
         self.assertTrue(1 is Config({'delay' : 1}).delay)
 
         self.assertIs(type(Config.timeout), property)
-        self.assertTrue(Config.DEFAULT_SOCKET_TIMEOUT is Config({'timeout' : 10}).timeout)
+
+        self.assertAlmostEqual(Config.DEFAULT_SOCKET_TIMEOUT, Config({'timeout' : 10}).timeout)
 
         self.assertIs(type(Config.retries), property)
         self.assertTrue(3 is Config({'retries' : 3}).retries)
 
         self.assertIs(type(Config.debug), property)
         self.assertTrue(1 is Config({'debug' : 1}).debug)
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser.py` & `opendoor-4.0.5/tests/test_lib_browser.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from src.lib import browser, BrowserError
 from src.lib.browser.threadpool import ThreadPool
 from src.lib.browser.config import Config
 from src.lib.browser.debug import Debug
 from src.lib.reader.reader import Reader
 from src.lib.tpl.tpl import Tpl
 from src.core.http.response import Response
@@ -81,51 +81,51 @@
         """ Browser.init() exception test """
         
         with self.assertRaises(BrowserError) as context:
             self.__browser_init({'host' : 'test.local', 'port' : 80, 'wordlist' : '/wrong'})
         self.assertTrue(BrowserError == context.expected)
 
 
-    @data(
-            Config({'host': 'example.com', 'port' : 80, 'debug': 1}),
-            Config({'host': 'example.com', 'scheme' : 'http://', 'port' : 80, 'debug': 1}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 2}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'indexof': True}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'random_agent': True}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'random_agent': True, 'random-list': True}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'accept-cookies' : True, 'scan' : 'directories'}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'scan' : 'subdomains'}),
-            Config({'host': 'example.com', 'port': 80, 'debug': 3, 'threads' : 2, 'delay' : 1, 'timeout' : 10, 'request' : 3}),
-    )
-    def test_http_scan(self, config):
-        """ Browser.scan() http test """
-
-        br = browser.__new__(browser)
-        reader = Reader(browser_config={
-                'list': config.scan,
-                'torlist': config.torlist,
-                'use_random': config.is_random_list,
-                'is_external_wordlist': config.is_external_wordlist,
-                'is_standalone_proxy': config.is_standalone_proxy,
-                'is_external_torlist': config.is_external_torlist,
-                'prefix': config.prefix
-            })
-        result = {}
-        result['total'] = helper.counter()
-        result['items'] = helper.list()
-
-        setattr(reader, '_Reader__config', self.__configuration)
-        setattr(br, '_Browser__debug', Debug(config))
-        setattr(br, '_Browser__pool', self.__pool)
-        setattr(br, '_Browser__config', config)
-        setattr(br, '_Browser__reader', reader)
-        setattr(br, '_Browser__response', Response(config=config, debug=Debug(config), tpl=Tpl))
-        setattr(br, '_Browser__result', result)
-        self.assertIs(br.scan(), None)
+    # @data(
+    #         Config({'host': 'example.com', 'port' : 80, 'debug': 1}),
+    #         Config({'host': 'example.com', 'scheme' : 'http://', 'port' : 80, 'debug': 1}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 2}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'indexof': True}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'random_agent': True}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'random_agent': True, 'random-list': True}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'accept-cookies' : True, 'scan' : 'directories'}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'scan' : 'subdomains'}),
+    #         Config({'host': 'example.com', 'port': 80, 'debug': 3, 'threads' : 2, 'delay' : 1, 'timeout' : 10, 'request' : 3}),
+    # )
+    # def test_http_scan(self, config):
+    #     """ Browser.scan() http test """
+    #
+    #     br = browser.__new__(browser)
+    #     reader = Reader(browser_config={
+    #             'list': config.scan,
+    #             'torlist': config.torlist,
+    #             'use_random': config.is_random_list,
+    #             'is_external_wordlist': config.is_external_wordlist,
+    #             'is_standalone_proxy': config.is_standalone_proxy,
+    #             'is_external_torlist': config.is_external_torlist,
+    #             'prefix': config.prefix
+    #         })
+    #     result = {}
+    #     result['total'] = helper.counter()
+    #     result['items'] = helper.list()
+    #
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     setattr(br, '_Browser__debug', Debug(config))
+    #     setattr(br, '_Browser__pool', self.__pool)
+    #     setattr(br, '_Browser__config', config)
+    #     setattr(br, '_Browser__reader', reader)
+    #     setattr(br, '_Browser__response', Response(config=config, debug=Debug(config), tpl=Tpl))
+    #     setattr(br, '_Browser__result', result)
+    #     self.assertIs(br.scan(), None)
 
     @data(
             Config({'host': 'http://example.com', 'port': 80, 'debug': 3, 'torlist':'/failed'}),
     )
     def test_browser_error(self, config):
         """ Browser.scan() exception test """
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser_filter.py` & `opendoor-4.0.5/tests/test_lib_browser_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from io import StringIO
 from mock import patch
-import unittest2 as unittest
+import unittest
 from src.lib.browser.filter import Filter
 from src.lib.browser.config import Config
 from src.core.logger.logger import Logger
 
 
 class TestBrowserFilter(unittest.TestCase):
     """TestBrowserFilter class"""
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_reporter.py` & `opendoor-4.0.5/tests/test_lib_reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 import os
 from configparser import ConfigParser
 
 from src.core import filesystem
 from src.lib.reporter import Reporter, ReporterError
 from src.lib.reporter.plugins.provider import PluginProvider
 from ddt import ddt, data
@@ -80,22 +80,22 @@
         
     def test_is_reported(self):
         """ Reporter.is_reported() test """
 
         expected = Reporter.is_reported('resource')
         self.assertIs(type(expected), bool)
         
-    def test_is_reported_error(self):
-        """ Reporter.is_reported() exception test """
-        rp = Reporter
-        setattr(rp, 'config', 'wrong.cfg')
-        with self.assertRaises(ReporterError) as context:
-            rp.is_reported('resource')
-            
-            self.assertTrue(ReporterError == context.expected)
+    # def test_is_reported_error(self):
+    #     """ Reporter.is_reported() exception test """
+    #     rp = Reporter
+    #     setattr(rp, 'config', 'wrong.cfg')
+    #     with self.assertRaises(ReporterError) as context:
+    #         rp.is_reported('resource')
+    #
+    #         self.assertTrue(ReporterError == context.expected)
         
     def test_plugin_provider_invalid_data_exception(self):
         """ PluginProvider.init() exception test """
 
         with self.assertRaises(TypeError) as context:
             PluginProvider('test.local', 'wrongdata')
             self.assertTrue(TypeError == context.expected)
@@ -111,36 +111,36 @@
     @data('std', 'txt', 'json', 'html')
     def test_load(self, value):
         """ Reporter.load() test """
 
         expected = Reporter.load(value, 'test.local', {})
         self.assertIsInstance(expected, PluginProvider)
         
-    @data('std', 'txt', 'json', 'html')
-    def test_process(self, ext):
-        """ Reporter.load().process() test """
-
-        report = Reporter.load(ext, 'test.local', self.mockdata)
-        self.assertIsNone(report.process())
-        if ext in ['html','json']:
-            self.assertTrue(filesystem.is_exist('tests/reports/test.local', 'test.local.{0}'.format(ext)))
-        if ext in ['txt']:
-            self.assertTrue(filesystem.is_exist('tests/reports/test.local', 'success.{0}'.format(ext)))
-        shutil.rmtree('tests/reports')
-        
-    @data('std', 'txt', 'json', 'html')
-    def test_load_plugin_exception(self, ext):
-        """ Reporter.load() exception test """
-        
-        if ext in ['html','json', 'txt']:
-
-            PluginProvider.CONFIG_FILE = 'wrong.cfg'
-            with self.assertRaises(Exception) as context:
-                Reporter.load(ext, 'test.local', self.mockdata)
-                self.assertTrue(Exception == context.expected)
+    # @data('std', 'txt', 'json', 'html')
+    # def test_process(self, ext):
+    #     """ Reporter.load().process() test """
+    #
+    #     report = Reporter.load(ext, 'test.local', self.mockdata)
+    #     self.assertIsNone(report.process())
+    #     if ext in ['html','json']:
+    #         self.assertTrue(filesystem.is_exist('tests/reports/test.local', 'test.local.{0}'.format(ext)))
+    #     if ext in ['txt']:
+    #         self.assertTrue(filesystem.is_exist('tests/reports/test.local', 'success.{0}'.format(ext)))
+    #     shutil.rmtree('tests/reports')
+        
+    # @data('std', 'txt', 'json', 'html')
+    # def test_load_plugin_exception(self, ext):
+    #     """ Reporter.load() exception test """
+    #
+    #     if ext in ['html','json', 'txt']:
+    #
+    #         PluginProvider.CONFIG_FILE = 'wrong.cfg'
+    #         with self.assertRaises(Exception) as context:
+    #             Reporter.load(ext, 'test.local', self.mockdata)
+    #             self.assertTrue(Exception == context.expected)
        
 
     def test_load_exception(self):
         """ Reporter.load() exception test """
 
         undefined = 'undefined'
         with self.assertRaises(ReporterError) as context:
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_package.py` & `opendoor-4.0.5/tests/test_lib_package.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,21 +9,20 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from src.core import sys
 from src.lib.package import Package, PackageError
-from src.lib.package.config import Config
 from src.core.filesystem import FileSystem
 from src.core.logger.logger import Logger
 
 
 class TestPackage(unittest.TestCase):
     """TestPackage class"""
     
@@ -42,83 +41,83 @@
     def test_examples(self):
         """ Package.examples() test """
 
         expected = Package.examples()
         self.assertIsNotNone(expected)
         self.assertIs(type(expected), str)
 
-    def test_banner(self):
-        """ Package.banner() test """
-
-        Config.params['cfg'] = 'setup.cfg'
-        expected = Package.banner()
-        self.assertIsNotNone(expected)
-        self.assertIs(type(expected), str)
-
-    def test_version(self):
-        """ Package.version() test """
-
-        Config.params['cfg'] = 'setup.cfg'
-        expected = Package.version()
-        self.assertIsNotNone(expected)
-        self.assertIs(type(expected), str)
-
-    def test_update_unix(self):
-        """ Package.update() unix test """
-
-        Config.params['cfg'] = 'setup.cfg'
-        Config.params['update'] = '{status}'
-        expected = Package.update()
-        self.assertIsNotNone(expected)
-        self.assertIs(type(expected), str)
-
-    def test_update_windows(self):
-        """ Package.update() test """
-
-        Config.params['cfg'] = 'setup.cfg'
-        Config.params['update'] = '{status}'
-        setattr(sys, 'is_windows', True)
-        expected = Package.update()
-        self.assertIsNotNone(expected)
-
-    def test_local_version(self):
-        """ Package.local_version() test """
-
-        Config.params['cfg'] = 'setup.cfg'
-        actual = FileSystem.readcfg('setup.cfg').get('info', 'version')
-        expected = Package.local_version()
-        self.assertEqual(actual, expected)
-
-    def test_local_version_exception(self):
-        """ Package.local_version() exception test """
-
-        Config.params['cfg'] = 'wrong.cfg'
-        with self.assertRaises(PackageError) as context:
-            Package.local_version()
-            self.assertTrue(PackageError == context.expected)
-
-    def test_update_exception(self):
-        """ Package.update() exception test """
-        Config.params['cvsupdate'] = 'wrongcvs'
-        with self.assertRaises(PackageError) as context:
-            Package.update()
-            self.assertTrue(PackageError == context.expected)
-        Config.params['cvsupdate'] = '/usr/bin/git pull origin master'
-
-    def test_version_exception(self):
-        """ Package.version() exception test """
-
-        Config.params['cfg'] = 'wrong.cfg'
-        with self.assertRaises(PackageError) as context:
-            Package.version()
-            self.assertTrue(PackageError == context.expected)
-
-    def test_banner_exception(self):
-        """ Package.banner() exception test """
-
-        Config.params['cfg'] = 'wrong.cfg'
-        with self.assertRaises(PackageError) as context:
-            Package.banner()
-            self.assertTrue(PackageError == context.expected)
+    # def test_banner(self):
+    #     """ Package.banner() test """
+    #
+    #     Config.params['cfg'] = 'setup.cfg'
+    #     expected = Package.banner()
+    #     self.assertIsNotNone(expected)
+    #     self.assertIs(type(expected), str)
+    #
+    # def test_version(self):
+    #     """ Package.version() test """
+    #
+    #     Config.params['cfg'] = 'setup.cfg'
+    #     expected = Package.version()
+    #     self.assertIsNotNone(expected)
+    #     self.assertIs(type(expected), str)
+    #
+    # def test_update_unix(self):
+    #     """ Package.update() unix test """
+    #
+    #     Config.params['cfg'] = 'setup.cfg'
+    #     Config.params['update'] = '{status}'
+    #     expected = Package.update()
+    #     self.assertIsNotNone(expected)
+    #     self.assertIs(type(expected), str)
+    #
+    # def test_update_windows(self):
+    #     """ Package.update() test """
+    #
+    #     Config.params['cfg'] = 'setup.cfg'
+    #     Config.params['update'] = '{status}'
+    #     setattr(sys, 'is_windows', True)
+    #     expected = Package.update()
+    #     self.assertIsNotNone(expected)
+
+    # def test_local_version(self):
+    #     """ Package.local_version() test """
+    #
+    #     Config.params['cfg'] = 'setup.cfg'
+    #     actual = FileSystem.readcfg('setup.cfg').get('info', 'version')
+    #     expected = Package.local_version()
+    #     self.assertEqual(actual, expected)
+    #
+    # def test_local_version_exception(self):
+    #     """ Package.local_version() exception test """
+    #
+    #     Config.params['cfg'] = 'wrong.cfg'
+    #     with self.assertRaises(PackageError) as context:
+    #         Package.local_version()
+    #         self.assertTrue(PackageError == context.expected)
+    #
+    # def test_update_exception(self):
+    #     """ Package.update() exception test """
+    #     Config.params['cvsupdate'] = 'wrongcvs'
+    #     with self.assertRaises(PackageError) as context:
+    #         Package.update()
+    #         self.assertTrue(PackageError == context.expected)
+    #     Config.params['cvsupdate'] = '/usr/bin/git pull origin master'
+    #
+    # def test_version_exception(self):
+    #     """ Package.version() exception test """
+    #
+    #     Config.params['cfg'] = 'wrong.cfg'
+    #     with self.assertRaises(PackageError) as context:
+    #         Package.version()
+    #         self.assertTrue(PackageError == context.expected)
+    #
+    # def test_banner_exception(self):
+    #     """ Package.banner() exception test """
+    #
+    #     Config.params['cfg'] = 'wrong.cfg'
+    #     with self.assertRaises(PackageError) as context:
+    #         Package.banner()
+    #         self.assertTrue(PackageError == context.expected)
             
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_reader.py` & `opendoor-4.0.5/tests/test_lib_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 import os
 from configparser import RawConfigParser
 from src.core.helper.helper import Helper
 from src.lib.reader import Reader, ReaderError
 from src.core.filesystem.filesystem import FileSystem
 from src.core.system.output import Output as sys
 from src.core.logger.logger import Logger
@@ -100,24 +100,24 @@
 
     def test_get_ignored_list_empty(self):
         """ Reader.get_ignored_list() empty test """
 
         empty_reader = Reader(browser_config={})
         self.assertIs(type(empty_reader.get_ignored_list()), list)
 
-    def test_get_proxies(self):
-        """ Reader.get_proxies() test """
-
-        reader = Reader(browser_config={
-            'is_standalone_proxy' : False
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        proxies = reader.get_proxies()
-        self.assertIs(type(proxies), list)
-        self.assertTrue(0 < len(proxies))
+    # def test_get_proxies(self):
+    #     """ Reader.get_proxies() test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_standalone_proxy' : False
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     proxies = reader.get_proxies()
+    #     self.assertIs(type(proxies), list)
+    #     self.assertTrue(0 < len(proxies))
 
     def test_get_proxies_empty(self):
         """ Reader.get_proxies() empty test """
 
         empty_reader = Reader(browser_config={})
         self.assertIs(type(empty_reader.get_proxies()), list)
 
@@ -129,115 +129,115 @@
             'list' : 'directories'
         })
         setattr(reader, '_Reader__config', self.__configuration_for_exception)
         with self.assertRaises(ReaderError) as context:
             reader.get_lines(params={}, loader=self.__callback_function)
             self.assertTrue(ReaderError == context.expected)
 
-    def test_get_lines_directories(self):
-        """ Reader.get_lines() directories test """
-
-        reader = Reader(browser_config={
-            'is_standalone_proxy' : False,
-            'list' : 'directories',
-            'prefix': '',
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        self.assertIsNone(reader.get_lines(params={
-            'scheme': 'http://',
-            'host': 'localhost.local',
-            'port': 80
-        }, loader=self.__callback_function))
-
-    def test_get_lines_subdomains(self):
-        """ Reader.get_lines() subdomains test """
-
-        reader = Reader(browser_config={
-            'is_standalone_proxy' : False,
-            'list' : 'subdomains',
-            'prefix': '',
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        self.assertIsNone(reader.get_lines(params={
-            'scheme': 'http://',
-            'host': 'localhost.local',
-            'port': 80
-        }, loader=self.__callback_function))
+    # def test_get_lines_directories(self):
+    #     """ Reader.get_lines() directories test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_standalone_proxy' : False,
+    #         'list' : 'directories',
+    #         'prefix': '',
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     self.assertIsNone(reader.get_lines(params={
+    #         'scheme': 'http://',
+    #         'host': 'localhost.local',
+    #         'port': 80
+    #     }, loader=self.__callback_function))
+
+    # def test_get_lines_subdomains(self):
+    #     """ Reader.get_lines() subdomains test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_standalone_proxy' : False,
+    #         'list' : 'subdomains',
+    #         'prefix': '',
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     self.assertIsNone(reader.get_lines(params={
+    #         'scheme': 'http://',
+    #         'host': 'localhost.local',
+    #         'port': 80
+    #     }, loader=self.__callback_function))
 
     def test_count_total_lines_exception(self):
         """ Reader.count_total_lines() exception test """
 
         reader = Reader(browser_config={
             'is_standalone_proxy' : False,
             'list' : 'subdomains',
             'prefix': '',
         })
         setattr(reader, '_Reader__config', self.__configuration_for_exception)
         with self.assertRaises(ReaderError) as context:
             reader.count_total_lines()
             self.assertTrue(ReaderError == context.expected)
 
-    def test_count_total_lines(self):
-        """ Reader.count_total_lines() test """
-
-        reader = Reader(browser_config={
-            'is_external_wordlist' : True,
-            'list' : 'tests/data/directories.dat',
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        setattr(reader, '_Reader__counter', 0)
-        self.assertIs(type(reader.count_total_lines()), int)
-        self.assertTrue(0 < reader.count_total_lines())
-        self.assertIs(15 ,reader.count_total_lines())
+    # def test_count_total_lines(self):
+    #     """ Reader.count_total_lines() test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_external_wordlist' : True,
+    #         'list' : 'tests/data/directories.dat',
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     setattr(reader, '_Reader__counter', 0)
+    #     self.assertIs(type(reader.count_total_lines()), int)
+    #     self.assertTrue(0 < reader.count_total_lines())
+    #     self.assertIs(15 ,reader.count_total_lines())
 
     def test_total_lines(self):
         """ Reader.total_lines test """
 
         empty_reader = Reader(browser_config={})
         self.assertIs(type(empty_reader.total_lines), int)
 
-    def test_randomize_list_exception(self):
-        """ Reader.randomize_list exception test """
-
-        reader = Reader(browser_config={})
-        setattr(reader, '_Reader__config', self.__configuration_for_exception)
-        setattr(sys, '_Output__is_windows', False)
-        with self.assertRaises(ReaderError) as context:
-            reader.randomize_list('directories', 'tmplist')
-            self.assertTrue(ReaderError == context.expected)
-
-    @unittest.skipIf(True is sys().is_windows, "Skip test for windows")
-    def test_randomize_list_unix(self):
-        """ Reader.randomize_list unix test """
-
-        reader = Reader(browser_config={
-            'is_external_wordlist': True,
-            'list': 'tests/data/directories.dat',
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        reader.count_total_lines()
-        self.assertIsNone(reader.randomize_list('directories', 'tmplist'))
-        fe = open('tests/data/directories.dat', 'r')
-        fa = open('tests/tmp/list.tmp', 'r')
-        expected = sum(1 for l in fe)
-        actual = sum(1 for l in fa)
-        self.assertIs(expected, actual)
-
-    def test_randomize_list_windows(self):
-        """ Reader.randomize_list windows test """
-
-        reader = Reader(browser_config={
-            'is_external_wordlist': True,
-            'list': 'tests/data/directories.dat',
-        })
-        setattr(reader, '_Reader__config', self.__configuration)
-        setattr(sys, 'is_windows', True)
-        reader.count_total_lines()
-        self.assertIsNone(reader.randomize_list('directories', 'tmplist'))
-        fe = open('tests/data/directories.dat', 'r')
-        fa = open('tests/tmp/list.tmp', 'r')
-        expected = sum(1 for l in fe)
-        actual = sum(1 for l in fa)
-        self.assertIs(expected, actual)
+    # def test_randomize_list_exception(self):
+    #     """ Reader.randomize_list exception test """
+    #
+    #     reader = Reader(browser_config={})
+    #     setattr(reader, '_Reader__config', self.__configuration_for_exception)
+    #     setattr(sys, '_Output__is_windows', False)
+    #     with self.assertRaises(ReaderError) as context:
+    #         reader.randomize_list('directories', 'tmplist')
+    #         self.assertTrue(ReaderError == context.expected)
+    #
+    # @unittest.skipIf(True is sys().is_windows, "Skip test for windows")
+    # def test_randomize_list_unix(self):
+    #     """ Reader.randomize_list unix test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_external_wordlist': True,
+    #         'list': 'tests/data/directories.dat',
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     reader.count_total_lines()
+    #     self.assertIsNone(reader.randomize_list('directories', 'tmplist'))
+    #     fe = open('tests/data/directories.dat', 'r')
+    #     fa = open('tests/tmp/list.tmp', 'r')
+    #     expected = sum(1 for l in fe)
+    #     actual = sum(1 for l in fa)
+    #     self.assertIs(expected, actual)
+    #
+    # def test_randomize_list_windows(self):
+    #     """ Reader.randomize_list windows test """
+    #
+    #     reader = Reader(browser_config={
+    #         'is_external_wordlist': True,
+    #         'list': 'tests/data/directories.dat',
+    #     })
+    #     setattr(reader, '_Reader__config', self.__configuration)
+    #     setattr(sys, 'is_windows', True)
+    #     reader.count_total_lines()
+    #     self.assertIsNone(reader.randomize_list('directories', 'tmplist'))
+    #     fe = open('tests/data/directories.dat', 'r')
+    #     fa = open('tests/tmp/list.tmp', 'r')
+    #     expected = sum(1 for l in fe)
+    #     actual = sum(1 for l in fa)
+    #     self.assertIs(expected, actual)
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_events.py` & `opendoor-4.0.5/tests/test_lib_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from __future__ import absolute_import
-import unittest2 as unittest
+import unittest
 import os
 import sys
 import signal
 from src.lib.events import EventHandler
 
 @unittest.skipUnless(hasattr(os, 'kill'), "Test requires os.kill")
 @unittest.skipIf(sys.platform =="win32", "Test cannot run on Windows")
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser_debug.py` & `opendoor-4.0.5/tests/test_lib_browser_debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from src.lib.browser.debug import Debug
 from src.lib.browser.config import Config
 from mock import patch
 from src.core.logger.logger import Logger
 from io import StringIO
 from ddt import ddt, data
```

### Comparing `opendoor-3.3.36rc0/tests/test_core_options.py` & `opendoor-4.0.5/tests/test_core_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from __future__ import absolute_import
-import unittest2 as unittest
+import unittest
 # noinspection PyCompatibility
 import argparse
 from ddt import ddt, data
 from src.core.options import Options
 from src.core.options.exceptions import OptionsError
 
 @ddt
```

### Comparing `opendoor-3.3.36rc0/tests/test_core_filter.py` & `opendoor-4.0.5/src/core/http/plugins/response/provider/provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,35 +9,46 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-from __future__ import absolute_import
-import unittest2 as unittest
-from ddt import ddt, data
-from src.core.options.filter import Filter
-
-@ddt
-class TestFilter(unittest.TestCase):
-    """TestFilter class"""
-    
-    @data(
-            {'host': 'example.com', 'port': 80, 'debug': 1},
-            {'host': 'https://example.com', 'port': 223, 'debug': 1},
-            {'host': 'example.com','debug': 1, 'scan': 'directories'},
-            {'host': 'example.com','debug': 1, 'scan': 'subdomains'}
-    )
-    def test_filter(self, args):
-        """ Filter.filter() test """
-        
-        flt = Filter.filter(args)
-        self.assertIs(type(flt), dict)
-
-      
-        
-if __name__ == "__main__":
-    unittest.main()
+from src.core import helper
+
+
+class ResponsePluginProvider(object):
+    """"ResponsePluginProvider class"""
+
+    def __init__(self):
+        """
+        PluginProvider constructor
+        """
+        self._status = 0
+        self._headers = {}
+        self._body = ''
+
+    def __set_body(self, body):
+        """
+        Set response data
+        :param str body: response data
+        :return: None
+        """
+
+        if False is isinstance(body, str):
+            self._body = helper.decode(body)
+
+    def process(self, response):
+        """
+        Process data
+        :param urllib3.response.HTTPResponse response: response object
+        :return: str
+        """
+
+        self._status = int(float(response.status))
+        self._headers = response.headers
+        self.__set_body(response.data)
+
+        pass
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_tpl.py` & `opendoor-4.0.5/tests/test_lib_tpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from src.core.logger.logger import Logger
 from io import StringIO
 from mock import patch
 from src.lib.tpl import Tpl, TplError
 
 
 class TestTpl(unittest.TestCase):
```

### Comparing `opendoor-3.3.36rc0/tests/test_lib_browser_worker.py` & `opendoor-4.0.5/tests/test_lib_browser_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
-import unittest2 as unittest
+import unittest
 from src.lib.browser.worker import Worker
 # noinspection PyCompatibility
 from queue import Queue
 
 
 class TestBrowserWorker(unittest.TestCase):
     """TestBrowserWorker class"""
```

### Comparing `opendoor-3.3.36rc0/setup.py` & `opendoor-4.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,46 +10,48 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 from setuptools import setup, find_packages
-VERSION = '3.3.36rc0'
-LONG_DESCRIPTION = open('README.md').read()
+VERSION = '4.0.5'
+LONG_DESCRIPTION = open('README.rst', 'r+', encoding='utf-8').read()
 
 setup(name='opendoor',
 
       # Versions should comply with PEP440.  For a discussion on single-sourcing
       # the version across setup.py and the project code, see
       # https://packaging.python.org/en/latest/single_source_version.html
 
       version=VERSION,
 
-      description='OWASP WEB Directory Scanner', long_description=LONG_DESCRIPTION,
+      description='OWASP WEB Directory Scanner',
+
+      long_description=LONG_DESCRIPTION,
+
+      long_description_content_type="text/markdown",
 
       # The project's main homepage.
       url='https://github.com/stanislav-web/OpenDoor',
 
       # Author details
-      author='Stanislav WEB',
-      author_email='stanisov@gmail.com',
-      maintainer='Stanislav WEB',
+      author='Brain Storm Team',
+      author_email='nomail@gmail.com',
+      maintainer='Brain Storm Team',
 
       # You can just specify the packages manually here if your project is
       # simple. Or you can use find_packages().
       zip_safe=False,
       packages=find_packages(),
-      package_data={'': ['setup.cfg']},
-      data_files=[('.', ['setup.cfg']),
-                  ('.', ['opendoor.conf']),
+      data_files=[('.', ['opendoor.conf']),
                   ('data', [
                       'data/directories.dat',
                       'data/ignored.dat',
                       'data/proxies.dat',
                       'data/subdomains.dat',
                       'data/useragents.dat',
                   ])
@@ -94,15 +96,15 @@
 
           # Language
           'Natural Language :: English',
 
           # Indicate who your project is intended for
           'Intended Audience :: Developers',
 
-          # OS which support this package
+          # OS, which support this package
           'Operating System :: MacOS',
           'Operating System :: Unix',
 
           # Pick your license as you wish (should match "license" above)
           'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 
           # Specify the Python versions you support here. In particular, ensure
```

### Comparing `opendoor-3.3.36rc0/opendoor.py` & `opendoor-4.0.5/opendoor.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,28 +11,29 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-    Development Team: Stanislav WEB
+    Development Team: Brain Storm Team
 """
 
 import sys
 
-for _ in ['urllib3', 'json2html', 'tabulate', 'importlib']:
+for _ in ['urllib3', 'json2html', 'tabulate', 'importlib', 'packaging']:
     try:
         __import__(_)
-    except ImportError:
-        sys.exit("""\t\t[!] Several dependencies wasn't installed!
-            Please run sudo pip install -r requirements.txt """)
+    except ImportError as error:
+        sys.exit("""\t\t[!] Several dependencies wasn't installed! Please run pip3 install -r requirements.txt. 
+        Details : %s.""" % error)
 
 if __name__ == "__main__":
 
     from src import Controller, SrcError
+    import sys
 
     try:
         bootstrap = Controller()
         bootstrap.run()
     except SrcError:
         sys.exit()
```

