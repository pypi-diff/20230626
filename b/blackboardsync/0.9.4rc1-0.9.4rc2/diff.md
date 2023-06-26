# Comparing `tmp/blackboardsync-0.9.4rc1.tar.gz` & `tmp/blackboardsync-0.9.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.4rc1.tar", last modified: Mon Jun 26 14:16:03 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.4rc2.tar", last modified: Mon Jun 26 14:33:21 2023, max compression
```

## Comparing `blackboardsync-0.9.4rc1.tar` & `blackboardsync-0.9.4rc2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.335829 blackboardsync-0.9.4rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.327829 blackboardsync-0.9.4rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.327829 blackboardsync-0.9.4rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.327829 blackboardsync-0.9.4rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:33:21.335829 blackboardsync-0.9.4rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.327829 blackboardsync-0.9.4rc2/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:33:21.000000 blackboardsync-0.9.4rc2/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 14:33:21.000000 blackboardsync-0.9.4rc2/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:33:21.000000 blackboardsync-0.9.4rc2/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 14:33:21.000000 blackboardsync-0.9.4rc2/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 14:33:21.000000 blackboardsync-0.9.4rc2/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.331829 blackboardsync-0.9.4rc2/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:33:21.335829 blackboardsync-0.9.4rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:33:21.335829 blackboardsync-0.9.4rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 14:32:38.000000 blackboardsync-0.9.4rc2/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.4rc2/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/.github/workflows/build.yml` & `blackboardsync-0.9.4rc2/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -130,11 +130,12 @@
           packaging/pkg_macos.sh "blackboard_sync-$GITHUB_REF_NAME"
 
       # Save Packages
 
       - name: Upload as release - only tagged commits
         uses: softprops/action-gh-release@v1
         with:
+          body_path: CHANGELOG.md
           prerelease: ${{ contains(github.ref_name, '-') }}
           files: |
             dist/*.exe
             dist/*.dmg
```

### Comparing `blackboardsync-0.9.4rc1/.gitignore` & `blackboardsync-0.9.4rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/CHANGELOG.md` & `blackboardsync-0.9.4rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/CONTRIBUTING.md` & `blackboardsync-0.9.4rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/LICENSE` & `blackboardsync-0.9.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/PKG-INFO` & `blackboardsync-0.9.4rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc1
+Version: 0.9.4rc2
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc1/Pipfile` & `blackboardsync-0.9.4rc2/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/Pipfile.lock` & `blackboardsync-0.9.4rc2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/README.md` & `blackboardsync-0.9.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/UNIVERSITIES.md` & `blackboardsync-0.9.4rc2/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/__about__.py` & `blackboardsync-0.9.4rc2/blackboard_sync/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.4-rc.1"
+__version__ = "0.9.4-rc.2"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/__init__.py` & `blackboardsync-0.9.4rc2/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/__main__.py` & `blackboardsync-0.9.4rc2/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.4rc2/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.4rc2/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.4rc2/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.4rc2/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.4rc2/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.4rc2/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.4rc2/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.4rc2/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/config.py` & `blackboardsync-0.9.4rc2/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/download.py` & `blackboardsync-0.9.4rc2/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/institutions.py` & `blackboardsync-0.9.4rc2/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.4rc2/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/sync.py` & `blackboardsync-0.9.4rc2/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.4rc2/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/universities.json` & `blackboardsync-0.9.4rc2/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/updates.py` & `blackboardsync-0.9.4rc2/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboard_sync/webdav.py` & `blackboardsync-0.9.4rc2/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.4rc2/blackboardsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc1
+Version: 0.9.4rc2
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc1/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.4rc2/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/docs/Makefile` & `blackboardsync-0.9.4rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/docs/conf.py` & `blackboardsync-0.9.4rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/docs/index.rst` & `blackboardsync-0.9.4rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/docs/make.bat` & `blackboardsync-0.9.4rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/main.py` & `blackboardsync-0.9.4rc2/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/packaging/pkg_macos.sh` & `blackboardsync-0.9.4rc2/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/packaging/pkg_win.nsi` & `blackboardsync-0.9.4rc2/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/packaging/pyinst.py` & `blackboardsync-0.9.4rc2/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/pyproject.toml` & `blackboardsync-0.9.4rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/strategies.py` & `blackboardsync-0.9.4rc2/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/test_api.py` & `blackboardsync-0.9.4rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/test_blackboard.py` & `blackboardsync-0.9.4rc2/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/test_download.py` & `blackboardsync-0.9.4rc2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/test_qt.py` & `blackboardsync-0.9.4rc2/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc1/tests/test_sync_config.py` & `blackboardsync-0.9.4rc2/tests/test_sync_config.py`

 * *Files identical despite different names*

