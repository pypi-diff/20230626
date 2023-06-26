# Comparing `tmp/UEVaultManager-1.7.0.tar.gz` & `tmp/UEVaultManager-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.7.0.tar", last modified: Fri Jun  2 09:55:23 2023, max compression
+gzip compressed data, was "UEVaultManager-1.7.1.tar", last modified: Sun Jun  4 07:16:35 2023, max compression
```

## Comparing `UEVaultManager-1.7.0.tar` & `UEVaultManager-1.7.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.347742 UEVaultManager-1.7.0/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     6127 2023-06-02 09:55:23.347742 UEVaultManager-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.311741 UEVaultManager-1.7.0/UEVaultManager/
--rw-rw-rw-   0        0        0      778 2023-06-02 09:53:06.000000 UEVaultManager-1.7.0/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.317741 UEVaultManager-1.7.0/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25471 2023-06-01 13:10:41.000000 UEVaultManager-1.7.0/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.7.0/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.319741 UEVaultManager-1.7.0/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.7.0/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.7.0/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.7.0/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.7.0/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    75996 2023-06-02 09:33:00.000000 UEVaultManager-1.7.0/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47699 2023-06-01 15:59:09.000000 UEVaultManager-1.7.0/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.319741 UEVaultManager-1.7.0/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.321742 UEVaultManager-1.7.0/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.7.0/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.7.0/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.325741 UEVaultManager-1.7.0/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23603 2023-06-02 09:07:47.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.7.0/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.331741 UEVaultManager-1.7.0/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.7.0/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.7.0/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.7.0/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.7.0/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.7.0/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.7.0/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.7.0/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.7.0/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.7.0/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.332743 UEVaultManager-1.7.0/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1712 2023-06-02 07:57:24.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.342741 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    33069 2023-06-02 06:58:20.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0    12891 2023-06-01 13:36:01.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    45155 2023-06-02 09:27:48.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9704 2023-06-02 09:05:32.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     7759 2023-06-02 07:59:54.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     3152 2023-06-02 09:13:08.000000 UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.346742 UEVaultManager-1.7.0/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.0/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.7.0/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-06-01 11:15:05.000000 UEVaultManager-1.7.0/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.7.0/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.7.0/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.7.0/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.7.0/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.7.0/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:55:23.315742 UEVaultManager-1.7.0/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6127 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      300 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 09:55:23.000000 UEVaultManager-1.7.0/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:55:23.347742 UEVaultManager-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.870124 UEVaultManager-1.7.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     6129 2023-06-04 07:16:35.870124 UEVaultManager-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.833126 UEVaultManager-1.7.1/UEVaultManager/
+-rw-rw-rw-   0        0        0      780 2023-06-04 07:15:03.000000 UEVaultManager-1.7.1/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.838124 UEVaultManager-1.7.1/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25471 2023-06-01 13:10:41.000000 UEVaultManager-1.7.1/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.7.1/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.841125 UEVaultManager-1.7.1/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.7.1/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.7.1/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.7.1/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.7.1/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    75918 2023-06-02 14:06:55.000000 UEVaultManager-1.7.1/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47699 2023-06-01 15:59:09.000000 UEVaultManager-1.7.1/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.841125 UEVaultManager-1.7.1/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.843125 UEVaultManager-1.7.1/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.7.1/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.7.1/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.847125 UEVaultManager-1.7.1/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23603 2023-06-02 09:07:47.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.7.1/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.853125 UEVaultManager-1.7.1/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.7.1/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.7.1/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2825 2023-06-03 15:42:48.000000 UEVaultManager-1.7.1/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.7.1/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.7.1/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.7.1/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.7.1/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.7.1/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.7.1/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.854125 UEVaultManager-1.7.1/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-06-02 07:57:24.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.864125 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-06-02 12:52:26.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-06-02 12:53:41.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-06-02 12:53:41.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    33069 2023-06-02 06:58:20.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0    16649 2023-06-03 17:49:20.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14067 2023-06-02 12:53:41.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    47403 2023-06-04 07:08:57.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9704 2023-06-02 09:05:32.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     8591 2023-06-02 13:07:17.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     3152 2023-06-02 09:13:08.000000 UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.869125 UEVaultManager-1.7.1/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.7.1/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.7.1/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-06-01 11:15:05.000000 UEVaultManager-1.7.1/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.7.1/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.7.1/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.7.1/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.7.1/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.7.1/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-06-04 07:16:35.837124 UEVaultManager-1.7.1/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6129 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      300 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-04 07:16:35.000000 UEVaultManager-1.7.1/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 07:16:35.870124 UEVaultManager-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.7.1/setup.py
```

### Comparing `UEVaultManager-1.7.0/LICENSE` & `UEVaultManager-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/PKG-INFO` & `UEVaultManager-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.7.0
+Version: 1.7.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.7.0 ## codename: Scorpio
+ UEVaultManager ## version:1.7.1 ## codename: Scorpio+1
```

### Comparing `UEVaultManager-1.7.0/README.md` & `UEVaultManager-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/__init__.py` & `UEVaultManager-1.7.1/UEVaultManager/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
-__codename__ = 'Scorpio'
+__codename__ = 'Scorpio+1'
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
 __author_email__ = 'laurent@gameamea.com'
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/api/egs.py` & `UEVaultManager-1.7.1/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/api/uevm.py` & `UEVaultManager-1.7.1/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.7.1/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/assets/main.ico` & `UEVaultManager-1.7.1/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/cli.py` & `UEVaultManager-1.7.1/UEVaultManager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1181,16 +1181,14 @@
                 # fix invalid input/output file name in arguments to avoid futher errors in file path checks
                 args.input = input_filename
                 args.output = input_filename
                 gui_g.UEVM_cli_args['input'] = input_filename
                 gui_g.UEVM_cli_args['output'] = input_filename
         gui_g.UEVM_gui_ref = UEVMGui(
             title=gui_g.s.app_title,
-            width=gui_g.s.app_width,
-            height=gui_g.s.app_height,
             icon=app_icon_filename,
             screen_index=0,
             file=input_filename,
             rebuild_data=rebuild
         )
         gui_g.UEVM_gui_ref.mainloop()
         # gui_g.UEVM_gui_ref.quit()
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/core.py` & `UEVaultManager-1.7.1/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.7.1/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.7.1/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.7.1/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.7.1/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.7.1/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.7.1/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.7.1/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/app.py` & `UEVaultManager-1.7.1/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/chunk.py` & `UEVaultManager-1.7.1/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/config.py` & `UEVaultManager-1.7.1/UEVaultManager/models/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,30 +41,34 @@
         :param args: arguments
         :param kwargs: keyword arguments
         """
         self.modified = False
         super().write(*args, **kwargs)
         self.mod_time = int(time.time())
 
-    def set(self, section: str, option: str, value=None) -> None:
+    def set(self, section: str, option: str, value = None) -> None:
         """
         Set a config option
         :param section: section name in the config file. If the section does not exist, it will be created
         :param option: option name
         :param value: value to set
         """
         if self.read_only:
             return
 
         # ensure config section exists
         if not self.has_section(section):
             self.add_section(section)
 
         self.modified = True
-        super().set(section, option, value)
+        if value is None:
+            super().set(section, option)
+        else:
+            value = str(value)
+            super().set(section, option, value)
 
     def remove_option(self, section: str, option: str) -> bool:
         """
         Remove an option from the config file
         :param section: section name in the config file. If the section does not exist, it will be created
         :param option: option name
         :return: True if the option was removed, False otherwise
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/csv.py` & `UEVaultManager-1.7.1/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/downloading.py` & `UEVaultManager-1.7.1/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/egl.py` & `UEVaultManager-1.7.1/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.7.1/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/models/manifest.py` & `UEVaultManager-1.7.1/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         #     print(f"style SELF = {style.theme_use()}")
         # else:
         #     style = ttk.Style(tk._default_root)
         #     print(f"style ROOT = {style.theme_use()}")
         #
         # self.style = style
 
-        geometry = gui_fn.center_window_on_screen(screen_index, height, width)
+        geometry = gui_fn.center_window_on_screen(screen_index, width, height)
         self.geometry(geometry)
         gui_fn.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
         self.quit_on_close = quit_on_close
         self.keep_existing = False  # whether to keep the existing content when adding a new one
         self.content_frame = self.ContentFrame(self)
         self.control_frame = self.ControlFrame(self)
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
 
     def __init__(self, parent, title: str, width: int = 600, height: int = 400, icon=None, screen_index=0, editable_table=None):
         super().__init__(parent)
         self.title(title)
         style = gui_fn.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
-        geometry = gui_fn.center_window_on_screen(screen_index, height, width)
+        geometry = gui_fn.center_window_on_screen(screen_index, width, height)
         self.geometry(geometry)
         gui_fn.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
 
         self.editable_table = editable_table
         self.must_save = False
         self.initial_values = []
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
 
     def __init__(self, parent, title: str, width: int = 600, height: int = 800, icon=None, screen_index: int = 0, editable_table=None):
         super().__init__(parent)
         self.title(title)
         style = gui_fn.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
-        geometry = gui_fn.center_window_on_screen(screen_index, height, width)
+        geometry = gui_fn.center_window_on_screen(screen_index, width, height)
         self.geometry(geometry)
         gui_fn.set_icon_and_minmax(self, icon)
         self.resizable(True, False)
 
         self.editable_table = editable_table
         self.must_save = False
         self.initial_values = []
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 """
 Implementation for:
 - GUISettings: class containing all the settings for the GUI
 """
+import json
 import os
 
 from termcolor import colored
 
 import UEVaultManager.tkgui.modules.functions_no_deps as gui_fn
 from UEVaultManager.lfs.utils import clean_filename
 from UEVaultManager.models.config import AppConf
@@ -35,27 +36,15 @@
     def __init__(self, config_file=None):
         self.path = ''
         self.config_path = ''
         self.config = AppConf(comment_prefixes='/', allow_no_value=True)
 
         self.init_gui_config_file(config_file)
 
-        # ##### start of properties stored in config file
-        # store all the properties that must be saved in config file
-        self.config_vars = {
-            'debug_mode': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'debug_mode', fallback=False)),
-            'never_update_data_files': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'never_update_data_files', fallback=False)),
-            'reopen_last_file': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'reopen_last_file', fallback=False)),
-            'use_colors_for_data': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'use_colors_for_data', fallback=True)),
-            'image_cache_max_time': int(self.config.get('UEVaultManager', 'image_cache_max_time', fallback=60 * 60 * 24 * 15)),
-            'last_opened_file': self.config.get('UEVaultManager', 'last_opened_file', fallback=''),
-            'cache_folder': self.config.get('UEVaultManager', 'cache_folder', fallback='../../../cache'),
-            'results_folder': self.config.get('UEVaultManager', 'results_folder', fallback='../../../results')
-        }
-
+        self.config_vars = self.read_config_properties()
         # the following folders are relative to the current file location
         # they must be used trought path_from_relative_to_absolute
         # following vars are not set as properties to avoid storing absolute paths in the config file
         self.cache_folder = gui_fn.path_from_relative_to_absolute(self.config_vars['cache_folder'])
         self.results_folder = gui_fn.path_from_relative_to_absolute(self.config_vars['results_folder'])
 
         # Folder for assets (aka. images, icon... not "UE assets") used for the GUI. THIS IS NOT A SETTING THAT CAN BE CHANGED BY THE USER
@@ -67,16 +56,14 @@
         if self.config_vars['reopen_last_file'] and os.path.isfile((self.config_vars['last_opened_file'])):
             self.csv_filename = self.config_vars['last_opened_file']
         else:
             self.csv_filename = os.path.join(self.config_vars['results_folder'], 'list.csv')
 
         self.csv_filename = os.path.normpath(self.csv_filename)
         self.app_title = f'{__name__} Gui v{__version__} ({__codename__})'
-        self.app_width = 1600
-        self.app_height = 935
         self.app_monitor = 1
         self.csv_datetime_format = '%Y-%m-%d %H:%M:%S'
         self.data_filetypes = (('csv file', '*.csv'), ('tcsv file', '*.tcsv'), ('json file', '*.json'), ('text file', '*.txt'))
         self.preview_max_width = 150
         self.preview_max_height = 150
         self.default_global_search = 'Text to search...'
         self.default_category_for_all = 'All'
@@ -100,89 +87,159 @@
             'grid_color': '#ABB1AD',  #
             'linewidth': 1,  #
             'rowheight': 22,  #
             'rowselectedcolor': '#E4DED4',  #
             'textcolor': 'black'  #
         }
 
+    def get_data_filters(self):
+        """ Getter for data_filters """
+        # convert a json string to a (filters) dict
+        values_dict = json.loads(self.config_vars['data_filters'])
+        return values_dict
+
+    def set_data_filters(self, values_dict):
+        """ Setter for data_filters """
+        # convert a (filters) dict to json string
+        json_str = json.dumps(values_dict, skipkeys=True, allow_nan=True)
+        self.config_vars['data_filters'] = json_str
+
+    # used as property for keeping transparent access
+    data_filters = property(get_data_filters, set_data_filters)
+
+    def get_x_pos(self):
+        """ Getter for x_pos """
+        return gui_fn.convert_to_int(self.config_vars['x_pos'])
+
+    def set_x_pos(self, value):
+        """ Setter for x_pos """
+        self.config_vars['x_pos'] = value
+
+    # used as property for keeping transparent access
+    x_pos = property(get_x_pos, set_x_pos)
+
+    def get_y_pos(self):
+        """ Getter for y_pos """
+        return gui_fn.convert_to_int(self.config_vars['y_pos'])
+
+    def set_y_pos(self, value):
+        """ Setter for y_pos """
+        self.config_vars['y_pos'] = value
+
+    # used as property for keeping transparent access
+    y_pos = property(get_y_pos, set_y_pos)
+
+    def get_width(self):
+        """ Getter for width """
+        return gui_fn.convert_to_int(self.config_vars['width'])
+
+    def set_width(self, value):
+        """ Setter for width """
+        self.config_vars['width'] = value
+
+    # used as property for keeping transparent access
+    width = property(get_width, set_width)
+
+    def get_height(self):
+        """ Getter for height """
+        return gui_fn.convert_to_int(self.config_vars['height'])
+
+    def set_height(self, value):
+        """ Setter for height """
+        self.config_vars['height'] = value
+
+    # used as property for keeping transparent access
+    height = property(get_height, set_height)
+
     def get_debug_mode(self):
         """ Getter for debug_mode """
         return self.config_vars['debug_mode']
 
     def set_debug_mode(self, value):
         """ Setter for debug_mode """
         self.config_vars['debug_mode'] = value
 
+    # used as property for keeping transparent access
+    debug_mode = property(get_debug_mode, set_debug_mode)
+
     def get_never_update_data_files(self):
         """ Getter for never_update_data_files """
-        return self.config_vars['never_update_data_files']
+        return gui_fn.convert_to_bool(self.config_vars['never_update_data_files'])
 
     def set_never_update_data_files(self, value):
         """ Setter for never_update_data_files """
         self.config_vars['never_update_data_files'] = value
 
+    # used as property for keeping transparent access
+    never_update_data_files = property(get_never_update_data_files, set_never_update_data_files)
+
     def get_reopen_last_file(self):
         """ Getter for reopen_last_file """
-        return self.config_vars['reopen_last_file']
+        return gui_fn.convert_to_bool(self.config_vars['reopen_last_file'])
 
     def set_reopen_last_file(self, value):
         """ Setter for reopen_last_file """
         self.config_vars['reopen_last_file'] = value
 
+    # used as property for keeping transparent access
+    reopen_last_file = property(get_reopen_last_file, set_reopen_last_file)
+
     def get_use_colors_for_data(self):
         """ Getter for use_colors_for_data """
-        return self.config_vars['use_colors_for_data']
+        return gui_fn.convert_to_bool(self.config_vars['use_colors_for_data'])
 
     def set_use_colors_for_data(self, value):
         """ Setter for use_colors_for_data """
         self.config_vars['use_colors_for_data'] = value
 
+    # used as property for keeping transparent access
+    use_colors_for_data = property(get_use_colors_for_data, set_use_colors_for_data)
+
     def get_image_cache_max_time(self):
         """ Getter for image_cache_max_time """
-        return self.config_vars['image_cache_max_time']
+        return gui_fn.convert_to_int(self.config_vars['image_cache_max_time'])
 
     def set_image_cache_max_time(self, value):
         """ Setter for image_cache_max_time """
         self.config_vars['image_cache_max_time'] = value
 
+    # used as property for keeping transparent access
+    image_cache_max_time = property(get_image_cache_max_time, set_image_cache_max_time)
+
     def get_last_opened_file(self):
         """ Getter for last_opened_file """
         return self.config_vars['last_opened_file']
 
     def set_last_opened_file(self, value):
         """ Setter for last_opened_file """
         self.config_vars['last_opened_file'] = value
 
+    # used as property for keeping transparent access
+    last_opened_file = property(get_last_opened_file, set_last_opened_file)
+
     def get_cache_folder(self):
         """ Getter for cache_folder """
         return self.config_vars['cache_folder']
 
     def set_cache_folder(self, value):
         """ Setter for cache_folder """
         self.config_vars['cache_folder'] = value
 
+    # not used as property to avoid storing absolute paths in the config file. Getter and setter could be used to store relative paths
+    # cache_folder = property(get_cache_folder, set_cache_folder)
+
     def get_results_folder(self):
         """ Getter for results_folder """
         return self.config_vars['results_folder']
 
     def set_results_folder(self, value):
         """ Setter for results_folder """
         self.config_vars['results_folder'] = value
 
-    # use properties for keeping transparent access to these properties
-    debug_mode = property(get_debug_mode, set_debug_mode)
-    never_update_data_files = property(get_never_update_data_files, set_never_update_data_files)
-    reopen_last_file = property(get_reopen_last_file, set_reopen_last_file)
-    use_colors_for_data = property(get_use_colors_for_data, set_use_colors_for_data)
-    image_cache_max_time = property(get_image_cache_max_time, set_image_cache_max_time)
-    last_opened_file = property(get_last_opened_file, set_last_opened_file)
-
-    # following vars are not set as properties to avoid storing absolute paths in the config file
-    # getter and setter could be used to store relative paths
-    # cache_folder = property(get_cache_folder, set_cache_folder)
+    # not used as property to avoid storing absolute paths in the config file. Getter and setter could be used to store relative paths
     # results_folder = property(get_results_folder, set_results_folder)
 
     def init_gui_config_file(self, config_file: str = '') -> None:
         """
         Initialize the config file for the gui
         :param config_file: the path to the config file to use
         """
@@ -205,18 +262,37 @@
         try:
             self.config.read(self.config_path)
         except Exception as error:
             log('Unable to read configuration file, please ensure that file is valid! '
                 f'(Error: {repr(error)})')
             log('Continuing with blank config in safe-mode...')
             self.config.read_only = True
-
         config_defaults = {
+            'data_filters': {
+                'comment': 'Filters to apply to the datatable. Stored in json format',
+                'value'  : ''
+            },
+            'x_pos': {
+                'comment': 'X position of the main windows. Set to 0 to center the window',
+                'value': 0
+            },
+            'y_pos': {
+                'comment': 'Y position of the main windows. Set to 0 to center the window',
+                'value': 0
+            },
+            'width': {
+                'comment': 'Width of the main windows',
+                'value': 1600
+            },
+            'height': {
+                'comment': 'Height of the main windows',
+                'value': 935
+            },
             'debug_mode': {
-                'comment': 'Set to True to print debug information (GUI related only',
+                'comment': 'Set to True to print debug information (GUI related only)',
                 'value': 'False'
             },
             'never_update_data_files': {
                 'comment': 'Set to True to speed the update process by not updating the metadata files. FOR TESTING ONLY',
                 'value': 'False'
             },
             'reopen_last_file': {
@@ -255,14 +331,39 @@
                 self.config.set('UEVaultManager', f';{content["comment"]}')
                 self.config.set('UEVaultManager', option, content['value'])
                 has_changed = True
 
         if has_changed:
             self.save_config_file(save_config_var=False)
 
+    def read_config_properties(self) -> dict:
+        """
+        Read the properties from the config file
+        :return:
+        """
+        # ##### start of properties stored in config file
+        # store all the properties that must be saved in config file
+        # no need of fallback values here, they are set in the config file by default
+        config_vars = {
+            'data_filters': self.config.get('UEVaultManager', 'data_filters'),
+            'x_pos': gui_fn.convert_to_int(self.config.get('UEVaultManager', 'x_pos')),
+            'y_pos': gui_fn.convert_to_int(self.config.get('UEVaultManager', 'y_pos')),
+            'width': gui_fn.convert_to_int(self.config.get('UEVaultManager', 'width')),
+            'height': gui_fn.convert_to_int(self.config.get('UEVaultManager', 'height')),
+            'debug_mode': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'debug_mode')),
+            'never_update_data_files': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'never_update_data_files')),
+            'reopen_last_file': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'reopen_last_file')),
+            'use_colors_for_data': gui_fn.convert_to_bool(self.config.get('UEVaultManager', 'use_colors_for_data')),
+            'image_cache_max_time': gui_fn.convert_to_int(self.config.get('UEVaultManager', 'image_cache_max_time')),
+            'last_opened_file': self.config.get('UEVaultManager', 'last_opened_file'),
+            'cache_folder': self.config.get('UEVaultManager', 'cache_folder'),
+            'results_folder': self.config.get('UEVaultManager', 'results_folder')
+        }
+        return config_vars
+
     def store_config_properties(self) -> None:
         """
         store the properties in the config file
         """
         for key, value in self.config_vars.items():
             self.config.set('UEVaultManager', key, str(value))
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         show_progress=True,
         function=None,
         function_parameters: dict = None,
         quit_on_close=False
     ):
         super().__init__()
         self.title(title)
-        geometry = gui_fn.center_window_on_screen(screen_index, height, width)
+        geometry = gui_fn.center_window_on_screen(screen_index, width, height)
         self.geometry(geometry)
         gui_fn.set_icon_and_minmax(self, icon)
         self._thread_check_delay = 100
         self.must_end = False
         self.quit_on_close = quit_on_close
         self.max_value = max_value
         self.continue_execution = True
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,33 +18,36 @@
 from UEVaultManager.tkgui.modules.TaggedLabelFrameClass import TaggedLabelFrame, WidgetType
 
 
 class UEVMGui(tk.Tk):
     """
     This class is used to create the main window for the application.
     :param title: The title
-    :param width: The width
-    :param height: The height
     :param icon: The icon
     :param screen_index: The screen index
     :param file: The file where the data is stored or read from
     :param show_open_file_dialog: If True, the open file dialog will be shown at startup
-
     """
 
-    def __init__(self, title: str, width=1200, height=800, icon='', screen_index=0, file=None, show_open_file_dialog=False, rebuild_data=False,):
+    def __init__(self, title: str, icon='', screen_index=0, file=None, show_open_file_dialog=False, rebuild_data=False,):
         super().__init__()
 
         self.title(title)
         style = set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
         self.style = style
-        geometry = gui_fn.center_window_on_screen(screen_index, height, width)
+        width = gui_g.s.width
+        height = gui_g.s.height
+        x_pos = gui_g.s.x_pos
+        y_pos = gui_g.s.y_pos
+        if not (x_pos and y_pos):
+            x_pos, y_pos = gui_fn.get_center_screen_positions(screen_index, width, height)
+        geometry: str = f'{width}x{height}+{x_pos}+{y_pos}'
         self.geometry(geometry)
         gui_fn.set_icon_and_minmax(self, icon)
-        self.resizable(True, False)
+        self.resizable(True, True)
         self.editable_table = None
         self.do_not_launch_search = False
         pack_def_options = {'ipadx': 5, 'ipady': 5, 'padx': 3, 'pady': 3}
 
         table_frame = self.TableFrame(self)
 
         # gui_g.UEVM_gui_ref = self  # important ! Must be donne before any use of a ProgressWindow. If not, an UEVMGuiHiddenRootClass will be created and the ProgressWindow still be displayed after the init
@@ -91,14 +94,17 @@
 
         if show_open_file_dialog:
             if self.load_file() == '':
                 gui_f.log_error('This application could not run without a file to read data from')
                 self.quit()
         # Quick edit the first row
         self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=0)
+        if gui_g.s.data_filters:
+            if self.load_filter(gui_g.s.data_filters):
+                self.apply_filters(save=False)
 
     class ToolbarFrame(ttk.Frame):
         """
         This class is used to create the toolbar frame
         :param container: The parent container
         """
 
@@ -566,23 +572,35 @@
         """
         When a checkbutton is changed, launch a search
         :param args:
         """
         if not self.do_not_launch_search:
             self.apply_filters()
 
-    def on_close(self) -> None:
+    def on_close(self, _event=None) -> None:
         """
         When the window is closed, check if there are unsaved changes and ask the user if he wants to save them
+        :param _event: the event that triggered the call of this function
         """
         if self.editable_table is not None and self.editable_table.must_save:
             if gui_f.box_yesno('Changes have been made. Do you want to save them in the source file ?'):
                 self.save_file(show_dialog=False)
+        self.close_window()
+
+    def close_window(self) -> None:
+        """
+        Close the window
+        """
         if gui_g.s.reopen_last_file:
             gui_g.s.last_opened_file = self.editable_table.file
+        # store window geometry in config settings
+        gui_g.s.width = self.winfo_width()
+        gui_g.s.height = self.winfo_height()
+        gui_g.s.x_pos = self.winfo_x()
+        gui_g.s.y_pos = self.winfo_y()
         gui_g.s.save_config_file()
         self.quit()
 
     def load_file(self) -> str:
         """
         Load a file
         :return: the name of the file that was loaded
@@ -626,34 +644,64 @@
             filename = self._open_file_dialog(save_mode=True, filename=self.editable_table.file)
             if filename:
                 selected_rows.to_csv(filename, index=False)
                 gui_f.box_message(f'Selected rows exported to "{filename}"')
         else:
             gui_f.box_message('Select at least one row first')
 
-    def apply_filters(self, _event=None) -> None:
+    def load_filter(self, filters: dict) -> bool:
+        """
+        Load the filters from a dictionary
+        :param filters: filters
+        :return: True if the filters were loaded, False otherwise
+        """
+        try:
+            self.do_not_launch_search = True
+            frm = self.control_frame
+
+            category = filters.get('Category', gui_g.s.default_category_for_all)
+            search_text = filters.get('Category', gui_g.s.default_global_search)
+            obsolete = filters.get('Obsolete', True)
+            # note: the "status" filter has no control associated, it's managed by the "obsolete" checkbutton
+            frm.var_grab_results.set(filters.get('Grab result', gui_g.s.default_category_for_all))
+            frm.var_is_purchased.set(filters.get('Purchased', False))
+            frm.var_is_not_obsolete.set(not obsolete)
+            frm.var_must_buy.set(filters.get('Must buy', False))
+            frm.var_on_sale.set(filters.get('On sale', False))
+            frm.var_category.set(category)
+            gui_g.UEVM_filter_category = category
+            frm.var_global_search.set(search_text)
+            self.do_not_launch_search = False
+            return True
+        except Exception as error:
+            gui_f.log_error(f'Error loading filters: {error!r}')
+            return False
+
+    def apply_filters(self, _event=None, save=True) -> None:
         """
         Search for a string in the table
         :param _event: Event
+        :param save: if True, save the filters in the config file
         """
-        search_text = self.control_frame.var_global_search.get()
-        category = self.control_frame.var_category.get()
-        grab_results = self.control_frame.var_grab_results.get()
-        purchased = self.control_frame.var_is_purchased.get()
-        not_obsolete = self.control_frame.var_is_not_obsolete.get()
-        must_buy = self.control_frame.var_must_buy.get()
-        on_sale = self.control_frame.var_on_sale.get()
+        frm = self.control_frame
+        search_text = frm.var_global_search.get()
+        category = frm.var_category.get()
+        grab_results = frm.var_grab_results.get()
+        purchased = frm.var_is_purchased.get()
+        not_obsolete = frm.var_is_not_obsolete.get()
+        must_buy = frm.var_must_buy.get()
+        on_sale = frm.var_on_sale.get()
         gui_g.UEVM_filter_category = category if category != gui_g.s.default_category_for_all else ''
         self.toggle_pagination(forced_value=False)
         filter_dict = {}
-        if category != gui_g.s.default_category_for_all:
+        if category != gui_g.s.default_category_for_all and category != '':
             filter_dict['Category'] = category
         else:
             filter_dict.pop('Category', None)
-        if grab_results != gui_g.s.default_category_for_all:
+        if grab_results != gui_g.s.default_category_for_all and grab_results != '':
             filter_dict['Grab result'] = grab_results
         else:
             filter_dict.pop('Grab result', None)
         if purchased:
             filter_dict['Purchased'] = True
         else:
             filter_dict.pop('Purchased', None)
@@ -668,14 +716,17 @@
         else:
             filter_dict.pop('Must buy', None)
         if on_sale:
             filter_dict['On sale'] = True
         else:
             filter_dict.pop('On sale', None)
         self.editable_table.apply_filters(filter_dict, global_search=search_text)
+        if save:
+            gui_g.s.set_data_filters(filter_dict)
+            gui_g.s.save_config_file(save_config_var=True)
         # self.control_frame.reset_entry_search()
 
     def reset_filters(self) -> None:
         """
         Reset the search controls to their default values
         """
         self.control_frame.var_global_search.set(gui_g.s.default_global_search)
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,34 +35,46 @@
 
     absolute_path = os.path.join(current_script_directory, path)
     absolute_path = os.path.abspath(absolute_path)
     # messagebox.showinfo('info', 'absolute_path: ' + absolute_path)
     return absolute_path
 
 
-def center_window_on_screen(screen_index: int, height: int, width: int) -> str:
+def center_window_on_screen(screen_index: int, width: int, height: int) -> str:
     """
     Calculate the geometry of the window to display in the center of the given screen
     :param screen_index: the index of the screen to use
+    :param width: the width of the window
     :param height: the height of the window
+    :return: the geometry string to use to display the window in the center of the screen
+    """
+    x, y = get_center_screen_positions(screen_index, width, height)
+    geometry: str = f'{width}x{height}+{x}+{y}'
+    return geometry
+
+
+def get_center_screen_positions(screen_index: int, width: int, height: int) -> (int, int):
+    """
+    Return the x and y positions of the window to display in the center of the given screen
+    :param screen_index: the index of the screen to use
     :param width: the width of the window
+    :param height: the height of the window
     :return: the geometry string to use to display the window in the center of the screen
     """
     monitors = get_monitors()
     if screen_index > len(monitors):
         print(f'The screen #{screen_index} is not available. Using 0 as screen index.')  # no use of log functions here to prevent circular import
         screen_index = 0
     # Position the window in the center of the screen
     target_screen = monitors[screen_index]
     screen_width = target_screen.width
     screen_height = target_screen.height
     x = target_screen.x + (screen_width-width) // 2
     y = target_screen.y + (screen_height-height) // 2
-    geometry: str = f'{width}x{height}+{x}+{y}'
-    return geometry
+    return x, y
 
 
 def set_custom_style(theme_name='lumen', font=('Arial', 10, 'normal')):
     """
     Set the custom style for the application
     :return: the style object
     """
@@ -184,7 +196,20 @@
     try:
         if str(value).lower() in ('1', '1.0', 'true', 'yes', 'y', 't'):
             return True
         else:
             return False
     except ValueError:
         return False
+
+
+def convert_to_int(value) -> int:
+    """
+    Convert a value to an integer
+    :param value: the value to convert.
+    :return: the integer value or 0 if the value is not an integer
+    """
+    try:
+        value = int(value)
+        return value
+    except ValueError:
+        return 0
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.7.1/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/cli.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.7.1/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.7.1/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.7.0
+Version: 1.7.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.7.0 ## codename: Scorpio
+ UEVaultManager ## version:1.7.1 ## codename: Scorpio+1
```

### Comparing `UEVaultManager-1.7.0/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.7.1/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.7.0/setup.py` & `UEVaultManager-1.7.1/setup.py`

 * *Files identical despite different names*

