# Comparing `tmp/jolt-0.9.95.tar.gz` & `tmp/jolt-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jolt-0.9.95.tar", last modified: Wed May 10 08:17:10 2023, max compression
+gzip compressed data, was "jolt-0.9.97.tar", last modified: Wed May 10 08:37:22 2023, max compression
```

## Comparing `jolt-0.9.95.tar` & `jolt-0.9.97.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.647269 jolt-0.9.95/
--rw-r--r--   0 root         (0) root         (0)     4212 2023-05-10 08:17:10.647269 jolt-0.9.95/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3130 2023-05-10 08:17:10.000000 jolt-0.9.95/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.631269 jolt-0.9.95/jolt/
--rw-r--r--   0 root         (0) root         (0)     1437 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/__main__.py
--rw-r--r--   0 root         (0) root         (0)    59840 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/cache.py
--rwxr-xr-x   0 root         (0) root         (0)    39083 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/cli.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/colors.py
--rw-r--r--   0 root         (0) root         (0)     8543 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/config.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/error.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/expires.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/filesystem.py
--rw-r--r--   0 root         (0) root         (0)    22861 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/graph.py
--rw-r--r--   0 root         (0) root         (0)     9979 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/hooks.py
--rw-r--r--   0 root         (0) root         (0)    15426 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/influence.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/inspection.py
--rw-r--r--   0 root         (0) root         (0)    10264 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/loader.py
--rw-r--r--   0 root         (0) root         (0)    11117 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/log.py
--rw-r--r--   0 root         (0) root         (0)     7639 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/manifest.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.635269 jolt-0.9.95/jolt/pkgs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/pkgs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/pkgs/golang.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/pkgs/nodejs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.643269 jolt-0.9.95/jolt/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      313 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/alias.py
--rw-r--r--   0 root         (0) root         (0)    10151 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/allure.py
--rw-r--r--   0 root         (0) root         (0)    32129 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/amqp.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/autoweight.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/cmake.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/conan.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/cxxinfo.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/dashboard.py
--rw-r--r--   0 root         (0) root         (0)    11569 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/debian.py
--rw-r--r--   0 root         (0) root         (0)    19171 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/docker.py
--rw-r--r--   0 root         (0) root         (0)     3356 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/email.py
--rw-r--r--   0 root         (0) root         (0)     7200 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/email.xslt
--rw-r--r--   0 root         (0) root         (0)     3371 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/environ.py
--rw-r--r--   0 root         (0) root         (0)     6545 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/ftp.py
--rw-r--r--   0 root         (0) root         (0)     5727 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/gdb.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/gerrit.py
--rw-r--r--   0 root         (0) root         (0)    14483 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/git.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/golang.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/googletest.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/http.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/junit.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/logstash.py
--rw-r--r--   0 root         (0) root         (0)     8212 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/ninja-compdb.py
--rw-r--r--   0 root         (0) root         (0)    73139 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/ninja.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/nodejs.py
--rw-r--r--   0 root         (0) root         (0)     1686 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/paths.py
--rw-r--r--   0 root         (0) root         (0)    20101 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/podman.py
--rw-r--r--   0 root         (0) root         (0)     3073 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/python.py
--rw-r--r--   0 root         (0) root         (0)     8947 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/repo.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/report.py
--rw-r--r--   0 root         (0) root         (0)     5994 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/selfdeploy.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/strings.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/symlinks.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/timeline.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/volume.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/yaml-ninja.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/plugins/yamltask.py
--rw-r--r--   0 root         (0) root         (0)    18464 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/scheduler.py
--rw-r--r--   0 root         (0) root         (0)    85933 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.647269 jolt-0.9.95/jolt/templates/
--rw-r--r--   0 root         (0) root         (0)     1720 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/templates/cxxexecutable.cmake.template
--rw-r--r--   0 root         (0) root         (0)     1750 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/templates/cxxlibrary.cmake.template
--rw-r--r--   0 root         (0) root         (0)     1778 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/templates/export.sh.template
--rw-r--r--   0 root         (0) root         (0)     1410 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/templates/timeline.html.template
--rw-r--r--   0 root         (0) root         (0)    68277 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/tools.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/version.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/version_utils.py
--rw-r--r--   0 root         (0) root         (0)     5543 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt/xmldom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:17:10.635269 jolt-0.9.95/jolt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4212 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      618 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-10 08:17:10.000000 jolt-0.9.95/jolt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 08:17:10.647269 jolt-0.9.95/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3044 2023-05-10 08:17:10.000000 jolt-0.9.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.278115 jolt-0.9.97/
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-05-10 08:37:22.278115 jolt-0.9.97/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-05-10 08:37:21.000000 jolt-0.9.97/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.266115 jolt-0.9.97/jolt/
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    59840 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/cache.py
+-rwxr-xr-x   0 root         (0) root         (0)    39083 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/cli.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/colors.py
+-rw-r--r--   0 root         (0) root         (0)     8543 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/config.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/error.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/expires.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/filesystem.py
+-rw-r--r--   0 root         (0) root         (0)    22861 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/graph.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/hooks.py
+-rw-r--r--   0 root         (0) root         (0)    15426 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/influence.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/inspection.py
+-rw-r--r--   0 root         (0) root         (0)    10264 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/loader.py
+-rw-r--r--   0 root         (0) root         (0)    11117 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/log.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/manifest.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.270115 jolt-0.9.97/jolt/pkgs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/pkgs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/pkgs/golang.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/pkgs/nodejs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.278115 jolt-0.9.97/jolt/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      313 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/alias.py
+-rw-r--r--   0 root         (0) root         (0)    10151 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/allure.py
+-rw-r--r--   0 root         (0) root         (0)    32129 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/amqp.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/autoweight.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/cmake.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/conan.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/cxxinfo.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/debian.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/email.py
+-rw-r--r--   0 root         (0) root         (0)     7200 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/email.xslt
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/environ.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     5727 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/gdb.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/gerrit.py
+-rw-r--r--   0 root         (0) root         (0)    14483 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/git.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/golang.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/googletest.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/http.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/junit.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/logstash.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/ninja-compdb.py
+-rw-r--r--   0 root         (0) root         (0)    73139 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/ninja.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/nodejs.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/paths.py
+-rw-r--r--   0 root         (0) root         (0)    20101 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/podman.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/python.py
+-rw-r--r--   0 root         (0) root         (0)     8947 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/repo.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/report.py
+-rw-r--r--   0 root         (0) root         (0)     5994 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/selfdeploy.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/strings.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/symlinks.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/timeline.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/volume.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/yaml-ninja.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/plugins/yamltask.py
+-rw-r--r--   0 root         (0) root         (0)    18464 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    85933 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.278115 jolt-0.9.97/jolt/templates/
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/templates/cxxexecutable.cmake.template
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/templates/cxxlibrary.cmake.template
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/templates/export.sh.template
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/templates/timeline.html.template
+-rw-r--r--   0 root         (0) root         (0)    68277 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/tools.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/version.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-05-10 08:37:21.000000 jolt-0.9.97/jolt/xmldom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:37:22.270115 jolt-0.9.97/jolt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4212 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-10 08:37:22.000000 jolt-0.9.97/jolt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 08:37:22.278115 jolt-0.9.97/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3044 2023-05-10 08:37:21.000000 jolt-0.9.97/setup.py
```

### Comparing `jolt-0.9.95/PKG-INFO` & `jolt-0.9.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolt
-Version: 0.9.95
+Version: 0.9.97
 Summary: A task executor
 Home-page: https://github.com/srand/jolt
 Author: Robert Andersson
 Author-email: srand@github.com
 Keywords: bazel,build,cmake,conan,jolt,make,meson,msbuild,xcode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jolt-0.9.95/README.rst` & `jolt-0.9.97/README.rst`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/__init__.py` & `jolt-0.9.97/jolt/__init__.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/__main__.py` & `jolt-0.9.97/jolt/__main__.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/cache.py` & `jolt-0.9.97/jolt/cache.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/cli.py` & `jolt-0.9.97/jolt/cli.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/colors.py` & `jolt-0.9.97/jolt/colors.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/config.py` & `jolt-0.9.97/jolt/config.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/error.py` & `jolt-0.9.97/jolt/error.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/expires.py` & `jolt-0.9.97/jolt/expires.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/filesystem.py` & `jolt-0.9.97/jolt/filesystem.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/graph.py` & `jolt-0.9.97/jolt/graph.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/hooks.py` & `jolt-0.9.97/jolt/hooks.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/influence.py` & `jolt-0.9.97/jolt/influence.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/inspection.py` & `jolt-0.9.97/jolt/inspection.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/loader.py` & `jolt-0.9.97/jolt/loader.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/log.py` & `jolt-0.9.97/jolt/log.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/manifest.py` & `jolt-0.9.97/jolt/manifest.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/pkgs/golang.py` & `jolt-0.9.97/jolt/pkgs/golang.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/pkgs/nodejs.py` & `jolt-0.9.97/jolt/pkgs/nodejs.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/allure.py` & `jolt-0.9.97/jolt/plugins/allure.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/amqp.py` & `jolt-0.9.97/jolt/plugins/amqp.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/autoweight.py` & `jolt-0.9.97/jolt/plugins/autoweight.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/cmake.py` & `jolt-0.9.97/jolt/plugins/cmake.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/conan.py` & `jolt-0.9.97/jolt/plugins/conan.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/cxxinfo.py` & `jolt-0.9.97/jolt/plugins/cxxinfo.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/dashboard.py` & `jolt-0.9.97/jolt/plugins/dashboard.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/debian.py` & `jolt-0.9.97/jolt/plugins/debian.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/docker.py` & `jolt-0.9.97/jolt/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/email.py` & `jolt-0.9.97/jolt/plugins/email.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/email.xslt` & `jolt-0.9.97/jolt/plugins/email.xslt`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/environ.py` & `jolt-0.9.97/jolt/plugins/environ.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/ftp.py` & `jolt-0.9.97/jolt/plugins/ftp.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/gdb.py` & `jolt-0.9.97/jolt/plugins/gdb.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/gerrit.py` & `jolt-0.9.97/jolt/plugins/gerrit.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/git.py` & `jolt-0.9.97/jolt/plugins/git.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/golang.py` & `jolt-0.9.97/jolt/plugins/golang.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/http.py` & `jolt-0.9.97/jolt/plugins/http.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/junit.py` & `jolt-0.9.97/jolt/plugins/junit.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/logstash.py` & `jolt-0.9.97/jolt/plugins/logstash.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/ninja-compdb.py` & `jolt-0.9.97/jolt/plugins/ninja-compdb.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/ninja.py` & `jolt-0.9.97/jolt/plugins/ninja.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/nodejs.py` & `jolt-0.9.97/jolt/plugins/nodejs.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/paths.py` & `jolt-0.9.97/jolt/plugins/paths.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/podman.py` & `jolt-0.9.97/jolt/plugins/podman.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/python.py` & `jolt-0.9.97/jolt/plugins/python.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/repo.py` & `jolt-0.9.97/jolt/plugins/repo.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/report.py` & `jolt-0.9.97/jolt/plugins/report.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/selfdeploy.py` & `jolt-0.9.97/jolt/plugins/selfdeploy.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/strings.py` & `jolt-0.9.97/jolt/plugins/strings.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/symlinks.py` & `jolt-0.9.97/jolt/plugins/symlinks.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/telemetry.py` & `jolt-0.9.97/jolt/plugins/telemetry.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/timeline.py` & `jolt-0.9.97/jolt/plugins/timeline.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/volume.py` & `jolt-0.9.97/jolt/plugins/volume.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/yaml-ninja.py` & `jolt-0.9.97/jolt/plugins/yaml-ninja.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/plugins/yamltask.py` & `jolt-0.9.97/jolt/plugins/yamltask.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/scheduler.py` & `jolt-0.9.97/jolt/scheduler.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/tasks.py` & `jolt-0.9.97/jolt/tasks.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/templates/cxxexecutable.cmake.template` & `jolt-0.9.97/jolt/templates/cxxexecutable.cmake.template`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/templates/cxxlibrary.cmake.template` & `jolt-0.9.97/jolt/templates/cxxlibrary.cmake.template`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/templates/export.sh.template` & `jolt-0.9.97/jolt/templates/export.sh.template`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/templates/timeline.html.template` & `jolt-0.9.97/jolt/templates/timeline.html.template`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/tools.py` & `jolt-0.9.97/jolt/tools.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/utils.py` & `jolt-0.9.97/jolt/utils.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/version_utils.py` & `jolt-0.9.97/jolt/version_utils.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt/xmldom.py` & `jolt-0.9.97/jolt/xmldom.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt.egg-info/PKG-INFO` & `jolt-0.9.97/jolt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jolt
-Version: 0.9.95
+Version: 0.9.97
 Summary: A task executor
 Home-page: https://github.com/srand/jolt
 Author: Robert Andersson
 Author-email: srand@github.com
 Keywords: bazel,build,cmake,conan,jolt,make,meson,msbuild,xcode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jolt-0.9.95/jolt.egg-info/SOURCES.txt` & `jolt-0.9.97/jolt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/jolt.egg-info/requires.txt` & `jolt-0.9.97/jolt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jolt-0.9.95/setup.py` & `jolt-0.9.97/setup.py`

 * *Files identical despite different names*

