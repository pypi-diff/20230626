# Comparing `tmp/blackboardsync-0.9.3.tar.gz` & `tmp/blackboardsync-0.9.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.3.tar", last modified: Sun Jun 25 18:06:11 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.4rc1.tar", last modified: Mon Jun 26 14:16:03 2023, max compression
```

## Comparing `blackboardsync-0.9.3.tar` & `blackboardsync-0.9.4rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.264401 blackboardsync-0.9.3/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-25 18:06:11.000000 blackboardsync-0.9.3/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 18:06:11.000000 blackboardsync-0.9.3/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:06:11.000000 blackboardsync-0.9.3/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-25 18:06:11.000000 blackboardsync-0.9.3/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 18:06:11.000000 blackboardsync-0.9.3/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:06:11.268401 blackboardsync-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-25 18:05:30.000000 blackboardsync-0.9.3/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.132433 blackboardsync-0.9.4rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.136433 blackboardsync-0.9.4rc1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 14:16:03.000000 blackboardsync-0.9.4rc1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.140433 blackboardsync-0.9.4rc1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:16:03.144433 blackboardsync-0.9.4rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 14:15:08.000000 blackboardsync-0.9.4rc1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.3/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.4rc1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/.github/workflows/build.yml` & `blackboardsync-0.9.4rc1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/.gitignore` & `blackboardsync-0.9.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/CHANGELOG.md` & `blackboardsync-0.9.4rc1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
+## 0.9.4 - 2023-06-26
+
+### Added
+- Option to limit the courses downloaded by earliest creation date
+
+### Fixed
+- App no longer crashes when downloading internet links on Linux
+
 
 ## 0.9.3 - 2023-06-25
 
 ### Added
 - Add basic support for 29 universities: Arkansas, UVM, Europea Madrid, ECOTEC, URSE, Palermo,
   Tecnologica del Salvador, Alcala, GWU, APU, Bucks, Northampton, Beds, YSU, Ohio, Princess Nourah,
   Leeds Beckett, Post, UAGM, Alabama, Torrens Australia, Holmes Institute, Trinity College Dublin,
```

### Comparing `blackboardsync-0.9.3/CONTRIBUTING.md` & `blackboardsync-0.9.4rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/LICENSE` & `blackboardsync-0.9.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/PKG-INFO` & `blackboardsync-0.9.4rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.3
+Version: 0.9.4rc1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -37,14 +37,15 @@
 What I was looking for in such an application was:
 
 - Automatic syncing with minimal intervention after the initial setup
 - Graphical interface
 - Cross-platform compatibility
 - It would make use of the [Blackboard REST API][blackboard-api]
 
+### 30+ Universities Supported Around the World
 
 
 **Why is my university not supported?**
 
 Simply put, some information is necessary to make the login process compatible with any given university. If you would like to help to add support for your university, or would like to see which universities are currently supported, [start here.](UNIVERSITIES.md)
```

### Comparing `blackboardsync-0.9.3/Pipfile` & `blackboardsync-0.9.4rc1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/Pipfile.lock` & `blackboardsync-0.9.4rc1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/README.md` & `blackboardsync-0.9.4rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 What I was looking for in such an application was:
 
 - Automatic syncing with minimal intervention after the initial setup
 - Graphical interface
 - Cross-platform compatibility
 - It would make use of the [Blackboard REST API][blackboard-api]
 
+### 30+ Universities Supported Around the World
 
 
 **Why is my university not supported?**
 
 Simply put, some information is necessary to make the login process compatible with any given university. If you would like to help to add support for your university, or would like to see which universities are currently supported, [start here.](UNIVERSITIES.md)
```

### Comparing `blackboardsync-0.9.3/UNIVERSITIES.md` & `blackboardsync-0.9.4rc1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/__about__.py` & `blackboardsync-0.9.4rc1/blackboard_sync/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.3"
+__version__ = "0.9.4-rc.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/__init__.py` & `blackboardsync-0.9.4rc1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/__main__.py` & `blackboardsync-0.9.4rc1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.4rc1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.4rc1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.4rc1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.4rc1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/config.py` & `blackboardsync-0.9.4rc1/blackboard_sync/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,7 +104,16 @@
     def university_index(self) -> Optional[int]:
         return self._sync.getint('university')
 
     @university_index.setter
     @Config.persist
     def university_index(self, university: int) -> None:
         self._sync['university'] = str(university)
+
+    @property
+    def min_year(self) -> Optional[int]:
+        return self._sync.getint('min_year')
+
+    @min_year.setter
+    @Config.persist
+    def min_year(self, year: int) -> None:
+        self._sync['min_year'] = str(year)
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/download.py` & `blackboardsync-0.9.4rc1/blackboard_sync/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,31 +42,34 @@
     _last_downloaded = datetime.fromtimestamp(0, tz=timezone.utc)
 
     _logger = logging.getLogger(__name__)
     _logger.setLevel(logging.DEBUG)
     _logger.addHandler(logging.StreamHandler())
 
     def __init__(self, sess: BlackboardSession, download_location: Path,
-                 last_downloaded: datetime = None, data_sources: list[str] = []):
+                 last_downloaded: datetime = None, data_sources: list[str] = [], min_year: int = None):
         """BlackboardDownload constructor
 
         Download all files in blackboard recursively to download_location,
         only if they have been altered since specified datetime
 
         Keyword arguments:
 
         :param BlackboardSession sess: UCLan BB user session
         :param (str / Path) download_location: Where files will be stored
         :param str last_downloaded: Files modified before this will not be downloaded
+        :param data_sources: List of valid data sources
+        :param min_year: Only courses created on or after this year will be downloaded
         """
 
         self._sess = sess
         self._user_id = sess.username
         self._download_location = download_location
         self._data_sources = data_sources
+        self._min_year = min_year
         self._files_processed = 0
         self.executor = ThreadPoolExecutor(max_workers=8)
         self.cancelled = False
 
         if last_downloaded is not None:
             self._last_downloaded = last_downloaded
 
@@ -156,16 +159,18 @@
                 if attachment.mimeType.startswith('video/'):
                     self.logger.info(f'Not downloading {attachment.fileName}')
                 else:
                     if not self.cancelled:
                         self.executor.submit(self._download_file, course_id, content.id, attachment.id, download_path)
 
         elif res == BBResourceType.externallink and has_changed:
+            # Place link under folder of its own, in case it has a body
             file_path.mkdir(exist_ok=True, parents=True)
-            self._create_desktop_link(file_path, res.url)
+            link_path = file_path / content.title_path_safe
+            self._create_desktop_link(link_path, res.url)
 
         elif not res.is_not_handled and has_changed:
             self.logger.warning(f"Not handled, {content.title}")
 
         # If item has body, write in markdown file
         if content.body and has_changed:
             file_path.mkdir(exist_ok=True, parents=True)
@@ -191,17 +196,22 @@
 
         start_time = datetime.now(timezone.utc)
 
         self.logger.info("Fetching user memberships")
 
         memberships = self._sess.fetch_user_memberships(user_id=self.user_id)
 
+        # Filter courses by data source
         if self._data_sources:
             memberships = [m for m in memberships if m.dataSourceId in self._data_sources]
 
+        # Filter courses by creation year
+        if self._min_year is not None:
+            memberships = [m for m in memberships if m.created.year >= self._min_year]
+
         for ms in memberships:
             if self.cancelled:
                 break
 
             private = False
             self.logger.debug("Fetching course")
             try:
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/institutions.py` & `blackboardsync-0.9.4rc1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.4rc1/blackboard_sync/qt/qt_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         self._status.setText(f"Last Synced: {self._last_synced}")
 
     def toggle_currently_syncing(self, syncing: bool) -> None:
         """Toggle the currently syncing indicator."""
         self.refresh.setEnabled(not syncing)
 
         if syncing:
-            self._status.setText("Syncing...")
+            self._status.setText("Downloading now...")
 
 
 class SyncTrayIcon(QSystemTrayIcon):
     """BlackboardSync system tray icon."""
 
     _tooltip = "Blackboard Sync"
     _sync_signal = pyqtSignal()
@@ -515,15 +515,15 @@
 
     class Pages(IntEnum):
         """Pages contained in the wizard."""
 
         INTRO = 0
         INSTITUTION = 1
         DOWNLOAD_LOCATION = 2
-        ANALYTICS = 3
+        DOWNLOAD_SINCE = 3
         LAST = 3
 
     _help_website = 'https://github.com/jacobszpz/BlackboardSync'
 
     def __init__(self, institutions: list[str]):
         """Create a `SetupWizard`.
 
@@ -544,14 +544,19 @@
         self.completer.setCaseSensitivity(Qt.CaseInsensitive)
         self.completer.setFilterMode(Qt.MatchContains)
         self.uni_selection_box.setCompleter(self.completer)
 
         self.file_chooser = QFileDialog()
         self.file_chooser.setFileMode(QFileDialog.Directory)
         self.sync_location_button.clicked.connect(self._choose_location)
+        self.date_spinbox.setEnabled(False)
+
+        self.since_all_checkbox.stateChanged.connect(
+            lambda state: self.date_spinbox.setEnabled(state != Qt.Checked)
+        )
 
         self.uni_selection_page.registerField(
             "userInstitution*",
             self.uni_selection_box.lineEdit()
         )
 
         self.sync_location_page.registerField(
@@ -608,14 +613,20 @@
         return self.uni_selection_box.currentIndex()
 
     @property
     def download_location(self) -> Path:
         """Sync location path selected by user."""
         return Path(self.file_chooser.directory().path())
 
+    @property
+    def min_year(self) -> Optional[int]:
+        """Courses from this year onward will be downloaded."""
+        if not self.since_all_checkbox.isChecked():
+            return self.date_spinbox.value()
+
 
 class UniNotSupportedDialog(QDialog):
     """`QDialog` about unsupported Blackboard partners."""
 
     def __init__(self, help_url: str):
         """Create instance of dialog.
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/sync.py` & `blackboardsync-0.9.4rc1/blackboard_sync/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,18 +94,20 @@
         if self._config.university_index is not None:
             self.university = get_by_index(self._config.university_index)
 
         if self._config.last_sync_time is not None:
             self._update_next_sync()
 
     def setup(self, university_index: int, download_location: Path,
-              share_errors: bool = False, share_stats: bool = False):
+              min_year: int = None):
         """Setup the university information."""
         self.university_index = university_index
         self._config.download_location = download_location
+        if min_year is not None:
+            self._config.min_year = min_year
 
     def auth(self, cookie_jar: RequestsCookieJar) -> bool:
         """Create a new Blackboard session with the given credentials.
 
         Will start syncing automatically if login successful.
 
         :param bool persistence: If true, login will be saved in the OS designated keyring.
@@ -140,15 +142,19 @@
 
         while self._is_active:
             if self.outdated or self._force_sync:
                 self.logger.debug("Syncing now")
                 self._is_syncing = True
 
                 # Download from last datetime
-                self._download = BlackboardDownload(self.sess, self.download_location / '', self.last_sync_time, self.university.data_sources)
+                self._download = BlackboardDownload(self.sess,
+                                                    self.download_location / '',
+                                                    self.last_sync_time,
+                                                    self.university.data_sources,
+                                                    self.min_year)
 
                 try:
                     if not self._is_active:
                         self._download.cancel()
                     job_start_time = self._download.download()
                     if job_start_time is not None:
                         self.last_sync_time = job_start_time
@@ -242,14 +248,18 @@
     def outdated(self) -> bool:
         """Return true if last download job is outdated."""
         if self._config.last_sync_time is None:
             return True
         return datetime.now(timezone.utc) >= self.next_sync
 
     @property
+    def min_year(self):
+        return self._config.min_year
+
+    @property
     def university_index(self):
         return self._config.university_index
 
     @university_index.setter
     def university_index(self, uni_index: int) -> None:
         self._config.university_index = uni_index
         self.university = get_by_index(uni_index)
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.4rc1/blackboard_sync/sync_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,17 @@
         self.tray.open_dir_signal.connect(self._open_download_dir)
         self.tray.show_menu_signal.connect(self._update_tray_menu)
 
         self.app.setQuitOnLastWindowClosed(False)
 
     def _setup_complete(self) -> None:
         self.setup_window.setVisible(False)
-        self.model.setup(self.setup_window.institution_index, self.setup_window.download_location)
+        self.model.setup(self.setup_window.institution_index,
+                         self.setup_window.download_location,
+                         self.setup_window.min_year)
         self._build_login_window(self.model.university.login)
         self._show_login_window()
 
     def _build_login_window(self, uni_login_info: InstitutionLogin) -> None:
         # Get login url from uni DB
         self.login_window = LoginWebView(start_url=uni_login_info.start_url,
                                          target_url=uni_login_info.target_url)
```

### Comparing `blackboardsync-0.9.3/blackboard_sync/universities.json` & `blackboardsync-0.9.4rc1/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/updates.py` & `blackboardsync-0.9.4rc1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboard_sync/webdav.py` & `blackboardsync-0.9.4rc1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.4rc1/blackboardsync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.3
+Version: 0.9.4rc1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -37,14 +37,15 @@
 What I was looking for in such an application was:
 
 - Automatic syncing with minimal intervention after the initial setup
 - Graphical interface
 - Cross-platform compatibility
 - It would make use of the [Blackboard REST API][blackboard-api]
 
+### 30+ Universities Supported Around the World
 
 
 **Why is my university not supported?**
 
 Simply put, some information is necessary to make the login process compatible with any given university. If you would like to help to add support for your university, or would like to see which universities are currently supported, [start here.](UNIVERSITIES.md)
```

### Comparing `blackboardsync-0.9.3/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.4rc1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/docs/Makefile` & `blackboardsync-0.9.4rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/docs/conf.py` & `blackboardsync-0.9.4rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/docs/index.rst` & `blackboardsync-0.9.4rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/docs/make.bat` & `blackboardsync-0.9.4rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/main.py` & `blackboardsync-0.9.4rc1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/packaging/pkg_macos.sh` & `blackboardsync-0.9.4rc1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/packaging/pkg_win.nsi` & `blackboardsync-0.9.4rc1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/packaging/pyinst.py` & `blackboardsync-0.9.4rc1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/pyproject.toml` & `blackboardsync-0.9.4rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/tests/strategies.py` & `blackboardsync-0.9.4rc1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/tests/test_api.py` & `blackboardsync-0.9.4rc1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/tests/test_blackboard.py` & `blackboardsync-0.9.4rc1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/tests/test_download.py` & `blackboardsync-0.9.4rc1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.3/tests/test_qt.py` & `blackboardsync-0.9.4rc1/tests/test_qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         assert not tray_icon._menu.log_in.isVisible()
         assert tray_icon._menu._status.isVisible()
         assert tray_icon._menu.quit.isVisible()
 
     def test_tray_icon_currently_syncing(self, qtbot, tray_icon):
         tray_icon.set_logged_in(True)
         tray_icon.toggle_currently_syncing(True)
-        assert tray_icon._menu._status.text() == 'Syncing...'
+        assert tray_icon._menu._status.text() == 'Downloading now...'
         assert not tray_icon._menu.refresh.isEnabled()
 
         tray_icon.toggle_currently_syncing(False)
         assert tray_icon._menu.refresh.isEnabled()
 
     def test_tray_icon_login_signal(self, qtbot, tray_icon):
         with qtbot.waitSignal(tray_icon.login_signal) as blocker:
```

### Comparing `blackboardsync-0.9.3/tests/test_sync_config.py` & `blackboardsync-0.9.4rc1/tests/test_sync_config.py`

 * *Files identical despite different names*

