# Comparing `tmp/honeybee-doe2-0.7.0.tar.gz` & `tmp/honeybee-doe2-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.7.0.tar", last modified: Fri Jun 23 16:05:47 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.8.0.tar", last modified: Mon Jun 26 17:37:19 2023, max compression
```

## Comparing `honeybee-doe2-0.7.0.tar` & `honeybee-doe2-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/interiorfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/adiabaticfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/adiabaticroof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/interiorfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 17:37:19.000000 honeybee-doe2-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 17:36:03.000000 honeybee-doe2-0.8.0/setup.py
```

### Comparing `honeybee-doe2-0.7.0/LICENSE` & `honeybee-doe2-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/PKG-INFO` & `honeybee-doe2-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.7.0
+Version: 0.8.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.7.0/README.md` & `honeybee-doe2-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.8.0/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.8.0/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.8.0/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/interiorfloor.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/interiorfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/room.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
-from honeybee.boundarycondition import Ground, Outdoors, Surface
+from honeybee.boundarycondition import Ground, Outdoors, Surface, Adiabatic
 from honeybee.facetype import Wall, Floor, RoofCeiling
 from honeybee.face import Face
 from honeybee.room import Room, Point3D
 from typing import List
 
 from ..utils.doe_formatters import short_name
 from ..utils.geometry import get_room_rep_poly
 from .wall import DoeWall
 from .roof import DoeRoof
 from .groundcontact import GroundFloor
 from .exposedfloor import ExposedFloor
 from .interiorfloor import InteriorFloor
+from .adiabaticfloor import AdiabaticFloor
+from .adiabaticroof import AdiabaticRoof
 
 
 class RoomDoe2Properties(object):
     """Properties for a DOE2 Space."""
 
     def __init__(self, _host: Room):
         self._host = _host
@@ -59,18 +61,29 @@
         return walls
 
     @property
     def roofs(self) -> List[DoeRoof]:
         roofs = [
             DoeRoof(face) for face in self.host.faces
             if isinstance(face.type, RoofCeiling)
+            and isinstance(face.boundary_condition, (Outdoors, Surface))
         ]
         return roofs
 
     @property
+    def adiabatic_roofs(self):
+        adiabatic_roofs = [
+            AdiabaticRoof(face) for face in self.host.faces
+            if isinstance(face.type, RoofCeiling)
+            and isinstance(face.boundary_condition, Adiabatic)
+
+        ]
+        return adiabatic_roofs
+
+    @property
     def ground_contact_surfaces(self):
         ground_contact_faces = [
             GroundFloor(face) for face in self.host.faces
             if isinstance(face.type, Floor)
             and isinstance(face.boundary_condition, Ground)
         ]
 
@@ -91,14 +104,23 @@
             InteriorFloor(face) for face in self.host.faces
             if isinstance(face.type, Floor)
             and isinstance(face.boundary_condition, Surface)
         ]
         return interior_floor_surfaces
 
     @property
+    def adiabatic_floor_surfaces(self):
+        adiabatic_floor_surfaces = [
+            AdiabaticFloor(face) for face in self.host.faces
+            if isinstance(face.type, Floor)
+            and isinstance(face.boundary_condition, Adiabatic)
+        ]
+        return adiabatic_floor_surfaces
+
+    @property
     def window(self):
         pass
     # TODO add window support
 
     @property
     def door(self):
         pass
@@ -134,9 +156,16 @@
         )
         exposed_floors = '\n'.join(
             [ef.to_inp(self.origin) for ef in self.exposed_floor_surfaces]
         )
         interior_floors = '\n'.join(
             [inf.to_inp(self.origin) for inf in self.interior_floor_surfaces]
         )
+        adiabatic_floors = '\n'.join(
+            [af.to_inp(self.origin) for af in self.adiabatic_floor_surfaces]
+        )
+        adiabatic_roofs = '\n'.join(
+            [ar.to_inp(self.origin) for ar in self.adiabatic_roofs]
+        )
         return '\n'.join(
-            [spaces, walls, roofs, ground_floors, exposed_floors, interior_floors])
+            [spaces, walls, roofs, adiabatic_roofs, ground_floors, exposed_floors,
+             interior_floors, adiabatic_floors])
```

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.8.0/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.8.0/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.8.0/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2/writer.py` & `honeybee-doe2-0.8.0/honeybee_doe2/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.8.0/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.7.0
+Version: 0.8.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.7.0/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.8.0/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 honeybee_doe2.egg-info/requires.txt
 honeybee_doe2.egg-info/top_level.txt
 honeybee_doe2/cli/__init__.py
 honeybee_doe2/cli/translate.py
 honeybee_doe2/geometry/__init__.py
 honeybee_doe2/geometry/polygon.py
 honeybee_doe2/properties/__init__.py
+honeybee_doe2/properties/adiabaticfloor.py
+honeybee_doe2/properties/adiabaticroof.py
 honeybee_doe2/properties/aperture.py
 honeybee_doe2/properties/constructions.py
 honeybee_doe2/properties/exposedfloor.py
 honeybee_doe2/properties/face.py
 honeybee_doe2/properties/groundcontact.py
 honeybee_doe2/properties/hvac.py
 honeybee_doe2/properties/interiorfloor.py
```

### Comparing `honeybee-doe2-0.7.0/setup.py` & `honeybee-doe2-0.8.0/setup.py`

 * *Files identical despite different names*

