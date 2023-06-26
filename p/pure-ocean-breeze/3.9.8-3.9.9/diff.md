# Comparing `tmp/pure_ocean_breeze-3.9.8.tar.gz` & `tmp/pure_ocean_breeze-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.8.tar", last modified: Wed Jun 21 03:31:07 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.9.tar", last modified: Mon Jun 26 01:28:01 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.8.tar` & `pure_ocean_breeze-3.9.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.673502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    31316 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    68253 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   228535 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.677502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.681502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 03:31:07.673502 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 03:31:07.000000 pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 03:31:07.685502 pure_ocean_breeze-3.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-21 03:30:57.000000 pure_ocean_breeze-3.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31577 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68253 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50076 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228559 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.559464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.563464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:28:01.555464 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 01:28:01.000000 pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:28:01.567464 pure_ocean_breeze-3.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 01:27:52.000000 pure_ocean_breeze-3.9.9/setup.py
```

### Comparing `pure_ocean_breeze-3.9.8/LICENSE` & `pure_ocean_breeze-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/PKG-INFO` & `pure_ocean_breeze-3.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.8
+Version: 3.9.9
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.8/README.md` & `pure_ocean_breeze-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-06-14 16:01:53"
-__version__ = "3.9.8"
+__updated__ = "2023-06-21 14:51:14"
+__version__ = "3.9.9"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/read_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-06-14 09:06:36"
+__updated__ = "2023-06-21 14:48:09"
 
 import os
 import numpy as np
 import pandas as pd
 import datetime
 from typing import Union, Dict, Tuple
 from loguru import logger
@@ -43,14 +43,15 @@
     vol_daily: bool = 0,
     vol: bool = 0,
     vol_inday: bool = 0,
     vol_night: bool = 0,
     swing: bool = 0,
     pb: bool = 0,
     pe: bool = 0,
+    pettm: bool = 0,
     iret: bool = 0,
     ivol: bool = 0,
     illiquidity: bool = 0,
     swindustry_ret: bool = 0,
     zxindustry_ret: bool = 0,
     stop_up: bool = 0,
     stop_down: bool = 0,
@@ -119,14 +120,16 @@
         为1则表示读取滚动20日隔夜收益率波动率, by default 0
     swing : bool, optional
         为1则表示读取振幅, by default 0
     pb : bool, optional
         为1则表示读取市净率, by default 0
     pe : bool, optional
         为1则表示读取市盈率, by default 0
+    pettm : bool, optional
+        为1则表示读取市盈率, by default 0
     iret : bool, optional
         为1则表示读取20日回归的fama三因子（市场、流通市值、市净率）特质收益率, by default 0
     ivol : bool, optional
         为1则表示读取20日回归的20日fama三因子（市场、流通市值、市净率）特质波动率, by default 0
     illiquidity : bool, optional
         为1则表示读取当日amihud非流动性指标, by default 0
     swindustry_ret : bool, optional
@@ -277,14 +280,18 @@
             df = pd.read_parquet(homeplace.daily_data_file + "pb.parquet") * read_daily(
                 state=1,start=start
             )
         elif pe:
             df = pd.read_parquet(homeplace.daily_data_file + "pe.parquet") * read_daily(
                 state=1,start=start
             )
+        elif pettm:
+            df = pd.read_parquet(homeplace.daily_data_file + "pettm.parquet") * read_daily(
+                state=1,start=start
+            )
         elif iret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "idiosyncratic_ret.parquet"
             ) * read_daily(state=1,start=start)
         elif ivol:
             df = read_daily(iret=1, start=start)
             df = df.rolling(20, min_periods=10).std()
```

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/data/write_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-22 15:55:43"
+__updated__ = "2023-06-21 14:50:52"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
@@ -293,14 +293,15 @@
                 "ts_code",
                 "trade_date",
                 "turnover_rate",
                 "total_share",
                 "float_share",
                 "pe",
                 "pb",
+                'pe_ttm',
             ],
         )
         time.sleep(1)
         return df1, df2
     except Exception:
         time.sleep(60)
         # 8个价格，交易状态，成交量，
@@ -332,14 +333,15 @@
                 "ts_code",
                 "trade_date",
                 "turnover_rate",
                 "total_share",
                 "float_share",
                 "pe",
                 "pb",
+                'pe_ttm'
             ],
         )
         time.sleep(1)
         return df1, df2
 
 
 @retry
@@ -387,14 +389,15 @@
         "total_sharenums",
         "ages",
         "sts",
         "states",
         "amounts",
         "pb",
         "pe",
+        'pettm',
         "vwaps",
         "adjfactors",
         "stop_ups",
         "stop_downs",
     ]
     startdates = list(map(single_file, names))
     startdate = min(startdates)
@@ -546,14 +549,27 @@
         partpe_new = pd.concat([partpe_old, partpe])
         partpe_new = partpe_new.drop_duplicates()
         partpe_new = partpe_new[closes.columns]
         partpe_new = partpe_new[sorted(list(partpe_new.columns))]
         partpe_new = drop_duplicates_index(partpe_new)
         partpe_new.to_parquet(homeplace.daily_data_file + "pe.parquet")
         logger.success("市盈率更新完成")
+        
+        # pettm
+        partpe = df2s[["date", "code", "pe_ttm"]].pivot(
+            index="date", columns="code", values="pe"
+        )
+        partpe_old = pd.read_parquet(homeplace.daily_data_file + "pettm.parquet")
+        partpe_new = pd.concat([partpe_old, partpe])
+        partpe_new = partpe_new.drop_duplicates()
+        partpe_new = partpe_new[closes.columns]
+        partpe_new = partpe_new[sorted(list(partpe_new.columns))]
+        partpe_new = drop_duplicates_index(partpe_new)
+        partpe_new.to_parquet(homeplace.daily_data_file + "pettm.parquet")
+        logger.success("TTM市盈率更新完成")
 
         # st
         part4 = df3[["s_info_windcode", "entry_dt", "remove_dt"]]
         part4 = part4.sort_values("s_info_windcode")
         part4.remove_dt = part4.remove_dt.fillna(now).astype(int)
         part4 = part4.set_index("s_info_windcode").stack()
         part4 = part4.reset_index().assign(
```

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-06-21 11:11:30"
+__updated__ = "2023-06-26 09:24:10"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -926,18 +926,18 @@
 
     Returns
     -------
     `pd.DataFrame`
         修改为交易日标注后的pd.DataFrame
     """
     """"""
-    start=df.index.min()
-    start=start-pd.tseries.offsets.MonthBegin()
-    start=datetime.datetime.strftime(start,'%Y%m%d')
-    trs = read_daily(tr=1,start=start)
+    start = df.index.min()
+    start = start - pd.tseries.offsets.MonthBegin()
+    start = datetime.datetime.strftime(start, "%Y%m%d")
+    trs = read_daily(tr=1, start=start)
     trs = trs.assign(tradeends=list(trs.index))
     trs = trs[["tradeends"]]
     trs = trs.resample("M").last()
     df = pd.concat([trs, df], axis=1)
     df = df.set_index(["tradeends"])
     return df
 
@@ -1890,15 +1890,15 @@
             lambda x: self.get_groups(x, groups_num)
         )
         self.wind_out = self.data.copy()
         self.factor_turnover_rates = self.data.pivot(
             index="date", columns="code", values="group"
         )
         rates = []
-        for i in range(1, 11):
+        for i in range(1, groups_num + 1):
             son = (self.factor_turnover_rates == i) + 0
             son1 = son.diff()
             # self.factor_turnover_rates = self.factor_turnover_rates.diff()
             change = ((np.abs(np.sign(son1)) == 1) + 0).sum(axis=1)
             still = (((son1 == 0) + 0) * son).sum(axis=1)
             rate = change / (change + still)
             rates.append(rate.to_frame(f"group{i}"))
@@ -3335,15 +3335,15 @@
             df = df.sort_values(["date", "num"])
         df = df.groupby(self.groupby_target).apply(the_func)
         if self.groupby_target == ["date", "code"]:
             df = df.to_frame("fac").reset_index()
             df.columns = ["date", "code", "fac"]
         else:
             df = df.reset_index()
-        if (df is not None) and (df.shape[0]>0):
+        if (df is not None) and (df.shape[0] > 0):
             df = df.pivot(columns="code", index="date", values="fac")
             df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
             to_save = df.stack().reset_index()
             to_save.columns = ["date", "code", "fac"]
             self.factor_steps.write_via_df(
                 to_save, self.factor_file_pinyin, tuple_col="fac"
             )
```

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.8
+Version: 3.9.9
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.8/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.9/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.8/setup.py` & `pure_ocean_breeze-3.9.9/setup.py`

 * *Files identical despite different names*

