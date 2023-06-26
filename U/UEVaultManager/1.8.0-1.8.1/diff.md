# Comparing `tmp/UEVaultManager-1.8.0.tar.gz` & `tmp/UEVaultManager-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.8.0.tar", last modified: Mon Jun 26 09:38:19 2023, max compression
+gzip compressed data, was "UEVaultManager-1.8.1.tar", last modified: Mon Jun 26 09:57:31 2023, max compression
```

## Comparing `UEVaultManager-1.8.0.tar` & `UEVaultManager-1.8.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.416892 UEVaultManager-1.8.0/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     6131 2023-06-26 09:38:19.416892 UEVaultManager-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.375892 UEVaultManager-1.8.0/UEVaultManager/
--rw-rw-rw-   0        0        0      782 2023-06-26 07:44:03.000000 UEVaultManager-1.8.0/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.381892 UEVaultManager-1.8.0/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    26859 2023-06-22 15:38:00.000000 UEVaultManager-1.8.0/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.8.0/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.383892 UEVaultManager-1.8.0/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.8.0/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.8.0/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.8.0/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.8.0/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    79535 2023-06-26 06:34:40.000000 UEVaultManager-1.8.0/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47899 2023-06-24 06:54:06.000000 UEVaultManager-1.8.0/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.384892 UEVaultManager-1.8.0/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.386892 UEVaultManager-1.8.0/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.8.0/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.8.0/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.388893 UEVaultManager-1.8.0/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     1249 2023-06-11 16:28:10.000000 UEVaultManager-1.8.0/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0    22011 2023-06-21 09:27:11.000000 UEVaultManager-1.8.0/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.8.0/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0      731 2023-06-07 14:35:17.000000 UEVaultManager-1.8.0/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.400892 UEVaultManager-1.8.0/UEVaultManager/models/
--rw-rw-rw-   0        0        0     4801 2023-06-21 09:27:17.000000 UEVaultManager-1.8.0/UEVaultManager/models/UEAssetClass.py
--rw-rw-rw-   0        0        0    30196 2023-06-24 06:19:07.000000 UEVaultManager-1.8.0/UEVaultManager/models/UEAssetDbHandlerClass.py
--rw-rw-rw-   0        0        0    35203 2023-06-26 07:10:13.000000 UEVaultManager-1.8.0/UEVaultManager/models/UEAssetScraperClass.py
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-07 14:35:17.000000 UEVaultManager-1.8.0/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.8.0/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2823 2023-06-07 14:35:17.000000 UEVaultManager-1.8.0/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0    15339 2023-06-23 14:17:07.000000 UEVaultManager-1.8.0/UEVaultManager/models/csv_data.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.8.0/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.8.0/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-06-07 08:15:25.000000 UEVaultManager-1.8.0/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.8.0/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30542 2023-06-26 07:06:41.000000 UEVaultManager-1.8.0/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.401893 UEVaultManager-1.8.0/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     2333 2023-06-26 06:34:19.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.411893 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6747 2023-06-02 12:52:26.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-06-02 12:53:41.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-06-02 12:53:41.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    42431 2023-06-26 07:08:55.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    15769 2023-06-22 06:22:17.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     1334 2023-06-22 16:34:43.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/FakeProgressWindowClass.py
--rw-rw-rw-   0        0        0    18385 2023-06-23 14:30:51.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14355 2023-06-24 06:15:39.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/ProgressWindowClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6499 2023-06-22 09:24:04.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    52810 2023-06-26 06:40:47.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      544 2023-06-07 08:19:02.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9233 2023-06-19 15:07:09.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0    11107 2023-06-26 07:05:16.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     3153 2023-06-22 14:18:34.000000 UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.415892 UEVaultManager-1.8.0/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.0/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0    10060 2023-06-22 15:38:00.000000 UEVaultManager-1.8.0/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1557 2023-06-13 12:54:48.000000 UEVaultManager-1.8.0/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.8.0/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.8.0/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.8.0/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7257 2023-06-20 06:16:56.000000 UEVaultManager-1.8.0/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:38:19.379892 UEVaultManager-1.8.0/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6131 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2491 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      323 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-26 09:38:19.000000 UEVaultManager-1.8.0/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      487 2023-06-07 14:11:08.000000 UEVaultManager-1.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 09:38:19.417892 UEVaultManager-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3560 2023-06-26 08:45:00.000000 UEVaultManager-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.568378 UEVaultManager-1.8.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0     6541 2023-06-26 09:57:31.567380 UEVaultManager-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5693 2023-06-26 09:56:48.000000 UEVaultManager-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.532380 UEVaultManager-1.8.1/UEVaultManager/
+-rw-rw-rw-   0        0        0      784 2023-06-26 09:56:40.000000 UEVaultManager-1.8.1/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.538379 UEVaultManager-1.8.1/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    26859 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.8.1/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.540378 UEVaultManager-1.8.1/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.8.1/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.8.1/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.8.1/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.8.1/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    79535 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47899 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.540378 UEVaultManager-1.8.1/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.542378 UEVaultManager-1.8.1/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.8.1/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.8.1/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.544377 UEVaultManager-1.8.1/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     1249 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0    22011 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.8.1/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0      731 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.551375 UEVaultManager-1.8.1/UEVaultManager/models/
+-rw-rw-rw-   0        0        0     4801 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/UEAssetClass.py
+-rw-rw-rw-   0        0        0    30196 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/UEAssetDbHandlerClass.py
+-rw-rw-rw-   0        0        0    35203 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/UEAssetScraperClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.8.1/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2823 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0    15339 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/csv_data.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.8.1/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.8.1/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-06-07 08:15:25.000000 UEVaultManager-1.8.1/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.8.1/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30542 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.552375 UEVaultManager-1.8.1/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     2333 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.563375 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-06-02 12:52:26.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-06-02 12:53:41.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-06-02 12:53:41.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    42431 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    15769 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     1334 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/FakeProgressWindowClass.py
+-rw-rw-rw-   0        0        0    18385 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14355 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/ProgressWindowClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6499 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    52810 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      544 2023-06-07 08:19:02.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9233 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0    11107 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     3153 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.567380 UEVaultManager-1.8.1/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.8.1/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0    10060 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1557 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.8.1/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.8.1/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.8.1/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7257 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:57:31.536379 UEVaultManager-1.8.1/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6541 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2491 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      323 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 09:57:31.000000 UEVaultManager-1.8.1/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      487 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:57:31.568378 UEVaultManager-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     3560 2023-06-26 09:40:30.000000 UEVaultManager-1.8.1/setup.py
```

### Comparing `UEVaultManager-1.8.0/LICENSE` & `UEVaultManager-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/PKG-INFO` & `UEVaultManager-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.8.0
+Version: 1.8.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -30,17 +30,18 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-| Hot news                                                                                                                                                                                         |                                                                                                           |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
-| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+| Hot news                                                    |                                                                                                                                                                                                                                                                         |
+|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| The 1.8.0 version is out : EPIC marketplace API integration | Scrap the data of ALL the asset in the marketplace and save the in a SQLITE database                                                                                                                                                                                    |  
+| The 1.6.0 version is out : Now with a GUI !                 | [![preview](https://i.imgur.com/DhVArs4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) <br/>- Edit the data in the GUI and save it back to the file<br/>- Use colors to visualize your asset status<br/>- Use filters and search to find them easily |
 
 **This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
@@ -63,8 +64,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.8.0 ## codename: Sagittarius
+ UEVaultManager ## version:1.8.1 ## codename: Sagittarius+1
```

### Comparing `UEVaultManager-1.8.0/README.md` & `UEVaultManager-1.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-| Hot news                                                                                                                                                                                         |                                                                                                           |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
-| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+| Hot news                                                    |                                                                                                                                                                                                                                                                         |
+|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| The 1.8.0 version is out : EPIC marketplace API integration | Scrap the data of ALL the asset in the marketplace and save the in a SQLITE database                                                                                                                                                                                    |  
+| The 1.6.0 version is out : Now with a GUI !                 | [![preview](https://i.imgur.com/DhVArs4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) <br/>- Edit the data in the GUI and save it back to the file<br/>- Use colors to visualize your asset status<br/>- Use filters and search to find them easily |
 
 **This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
```

### Comparing `UEVaultManager-1.8.0/UEVaultManager/__init__.py` & `UEVaultManager-1.8.1/UEVaultManager/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.8.0'
+__version__ = '1.8.1'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
-__codename__ = 'Sagittarius'
+__codename__ = 'Sagittarius+1'
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
 __author_email__ = 'laurent@gameamea.com'
 __description__ = 'Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine'
 __copyright__ = f'{year} {__author__}'
```

### Comparing `UEVaultManager-1.8.0/UEVaultManager/api/egs.py` & `UEVaultManager-1.8.1/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/api/uevm.py` & `UEVaultManager-1.8.1/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.8.1/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/assets/main.ico` & `UEVaultManager-1.8.1/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/cli.py` & `UEVaultManager-1.8.1/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/core.py` & `UEVaultManager-1.8.1/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.8.1/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.8.1/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.8.1/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.8.1/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.8.1/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.8.1/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/UEAssetClass.py` & `UEVaultManager-1.8.1/UEVaultManager/models/UEAssetClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/UEAssetDbHandlerClass.py` & `UEVaultManager-1.8.1/UEVaultManager/models/UEAssetDbHandlerClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/UEAssetScraperClass.py` & `UEVaultManager-1.8.1/UEVaultManager/models/UEAssetScraperClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/app.py` & `UEVaultManager-1.8.1/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/chunk.py` & `UEVaultManager-1.8.1/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/config.py` & `UEVaultManager-1.8.1/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/csv_data.py` & `UEVaultManager-1.8.1/UEVaultManager/models/csv_data.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/downloading.py` & `UEVaultManager-1.8.1/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/egl.py` & `UEVaultManager-1.8.1/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.8.1/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/models/manifest.py` & `UEVaultManager-1.8.1/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/FakeProgressWindowClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/FakeProgressWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/ProgressWindowClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/ProgressWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.8.1/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/utils/cli.py` & `UEVaultManager-1.8.1/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.8.1/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.8.1/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.8.1/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.8.1/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.8.1/UEVaultManager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.8.0
+Version: 1.8.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -30,17 +30,18 @@
 their data from the Epic Games Marketplace. It is developed in Python, so
 it can run on any platform that support this language.
 
 Its main purpose is to list the assets (with or without user login),
 filter (optional) and save the list into a file that can be reused later
 as a data source (in an Excel sheet for instance).
 
-| Hot news                                                                                                                                                                                         |                                                                                                           |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|
-| The new version is out : Now with a GUI !<br/>Edit the data in the GUI and save it back to the file<br/>Use colors to visualize your asset status<br/>Use filters and search to find them easily | [![preview](https://i.imgur.com/dXS62o4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) |
+| Hot news                                                    |                                                                                                                                                                                                                                                                         |
+|-------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| The 1.8.0 version is out : EPIC marketplace API integration | Scrap the data of ALL the asset in the marketplace and save the in a SQLITE database                                                                                                                                                                                    |  
+| The 1.6.0 version is out : Now with a GUI !                 | [![preview](https://i.imgur.com/DhVArs4.png)](https://uevaultmanager.readthedocs.io/en/latest/tkgui.html) <br/>- Edit the data in the GUI and save it back to the file<br/>- Use colors to visualize your asset status<br/>- Use filters and search to find them easily |
 
 **This project is still under active development**                                                                    |
 
 To go further, dive into [the documentation](https://uevaultmanager.readthedocs.io/en/latest/index.html) or just go
 for [a quickstart](https://uevaultmanager.readthedocs.io/en/latest/quickstart.html)
 
 Contents:
@@ -63,8 +64,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.8.0 ## codename: Sagittarius
+ UEVaultManager ## version:1.8.1 ## codename: Sagittarius+1
```

### Comparing `UEVaultManager-1.8.0/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.8.1/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.8.0/setup.py` & `UEVaultManager-1.8.1/setup.py`

 * *Files identical despite different names*

