# Comparing `tmp/neon-skill-update-0.3.3a3.tar.gz` & `tmp/neon-skill-update-0.3.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-0.3.3a3.tar", last modified: Fri Jun 23 22:29:38 2023, max compression
+gzip compressed data, was "neon-skill-update-0.3.3a4.tar", last modified: Mon Jun 26 17:02:59 2023, max compression
```

## Comparing `neon-skill-update-0.3.3a3.tar` & `neon-skill-update-0.3.3a4.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.872228 neon-skill-update-0.3.3a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.872228 neon-skill-update-0.3.3a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 22:29:38.000000 neon-skill-update-0.3.3a3/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:29:38.876227 neon-skill-update-0.3.3a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-23 22:29:35.000000 neon-skill-update-0.3.3a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.601878 neon-skill-update-0.3.3a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.601878 neon-skill-update-0.3.3a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 17:02:59.000000 neon-skill-update-0.3.3a4/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:02:59.609878 neon-skill-update-0.3.3a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:02:59.605878 neon-skill-update-0.3.3a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 17:02:54.000000 neon-skill-update-0.3.3a4/version.py
```

### Comparing `neon-skill-update-0.3.3a3/LICENSE.md` & `neon-skill-update-0.3.3a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a3/PKG-INFO` & `neon-skill-update-0.3.3a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 0.3.3a3
+Version: 0.3.3a4
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-0.3.3a3/README.md` & `neon-skill-update-0.3.3a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a3/__init__.py` & `neon-skill-update-0.3.3a4/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import os
+
 from random import randint
+from typing import Optional
 from adapt.intent import IntentBuilder
 from neon_utils.validator_utils import numeric_confirmation_validator
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_utils.network_utils import is_connected_http
 from neon_utils.skills import NeonSkill
@@ -39,14 +42,15 @@
 
 
 class UpdateSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self.current_ver = None
         self.latest_ver = None
+        self._update_filename = "update_signal"
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
@@ -75,30 +79,49 @@
 
     @property
     def image_drive(self):
         return self.settings.get("image_drive") or "/dev/sdb"
 
     # TODO: Move to __init__ after stable ovos-workshop
     def initialize(self):
-        self.add_event('mycroft.ready',
-                       self._check_latest_core_release, once=True)
+        self.add_event('mycroft.ready', self._on_ready)
         self.add_event("update.gui.continue_installation",
                        self.continue_os_installation)
         self.add_event("update.gui.finish_installation",
                        self.finish_os_installation)
         self.add_event("update.gui.install_update", self.handle_update_device)
 
+    def _on_ready(self, message):
+        LOG.debug("Checking latest core version")
+        self._check_latest_core_release(message)
+
+        update_stat = self._check_update_status()
+        LOG.debug(f"Update status is {update_stat}")
+        if not update_stat:
+            # No update was attempted
+            return
+        speak_version = self.pronounce_version(self.current_ver)
+        if update_stat is True:
+            LOG.debug("Update success")
+            self.speak_dialog("notify_update_success",
+                              {"version": speak_version})
+        elif update_stat is False:
+            LOG.warning("Update failed")
+            self.speak_dialog("notify_update_failure",
+                              {"version": speak_version})
+
     def _check_latest_core_release(self, message):
         """
         Handles checking for a new release version
         :param message: message object associated with loaded emit
         """
         response = self.bus.wait_for_response(
             message.forward("neon.core_updater.check_update",
-                            {'include_prerelease': self.include_prerelease}))
+                            {'include_prerelease': self.include_prerelease}),
+            timeout=15)
         if response:
             LOG.debug(f"Got response: {response.data}")
             self.current_ver = response.data.get("installed_version")
             self.latest_ver = response.data.get("latest_version") or \
                 response.data.get("new_version")
             if not self.latest_ver:
                 LOG.error(f"Expected string version and got none in response: "
@@ -154,20 +177,52 @@
             resp = self.ask_yesno(
                 "update_core",
                 {"new": self.pronounce_version(self.latest_ver),
                  "old": self.pronounce_version(self.current_ver)})
         if resp == "yes":
             if message.data.get('notification'):
                 self._dismiss_notification(message)
+            self._write_update_signal(self.latest_ver)
             self.speak_dialog("starting_update", wait=True)
             self.bus.emit(message.forward("neon.core_updater.start_update",
                                           {"version": self.latest_ver}))
         else:
             self.speak_dialog("not_updating")
 
+    def _write_update_signal(self, new_ver: str):
+        """
+        Write a file with the version being updated to that can be checked upon
+        next boot
+        :param new_ver: New core version being updated to
+        """
+        with self.file_system.open(self._update_filename, 'w+') as f:
+            f.write(new_ver)
+
+    def _check_update_status(self) -> Optional[bool]:
+        """
+        Check if an update was completed on startup.
+        Returns:
+            None if no update was attempted
+            True if an update was successful
+            False if an update failed
+        """
+        update_filepath = os.path.join(self.file_system.path,
+                                       self._update_filename)
+        if not os.path.exists(update_filepath):
+            return None
+        with open(update_filepath, 'r') as f:
+            expected_ver = f.read()
+        os.remove(update_filepath)
+        LOG.info(f"Removed update signal at {update_filepath}")
+        if self.current_ver != expected_ver:
+            LOG.error(f"Update expected {expected_ver} but "
+                      f"{self.current_ver} is installed")
+            return False
+        return True
+
     @intent_file_handler("core_version.intent")
     def handle_core_version(self, message):
         """
         Handle a user request for the current installed version.
         :param message: message object associated with request
         """
         self._check_latest_core_release(message)
```

### Comparing `neon-skill-update-0.3.3a3/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-0.3.3a4/neon_skill_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 0.3.3a3
+Version: 0.3.3a4
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-0.3.3a3/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-0.3.3a4/neon_skill_update.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 locale/en-us/dialog/installation_complete.dialog
 locale/en-us/dialog/not_updating.dialog
 locale/en-us/dialog/notify_download_complete.dialog
 locale/en-us/dialog/notify_download_failed.dialog
 locale/en-us/dialog/notify_installation_complete.dialog
 locale/en-us/dialog/notify_installation_failed.dialog
 locale/en-us/dialog/notify_update_available.dialog
+locale/en-us/dialog/notify_update_failure.dialog
+locale/en-us/dialog/notify_update_success.dialog
 locale/en-us/dialog/notify_writing_image.dialog
 locale/en-us/dialog/point.dialog
 locale/en-us/dialog/starting_installation.dialog
 locale/en-us/dialog/starting_update.dialog
 locale/en-us/dialog/up_to_date.dialog
 locale/en-us/dialog/update_core.dialog
 locale/en-us/dialog/update_track_already_set.dialog
```

### Comparing `neon-skill-update-0.3.3a3/setup.py` & `neon-skill-update-0.3.3a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a3/skill.json` & `neon-skill-update-0.3.3a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a3/test/test_skill.py` & `neon-skill-update-0.3.3a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-0.3.3a3/version.py` & `neon-skill-update-0.3.3a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.3a3"
+__version__ = "0.3.3a4"
```

