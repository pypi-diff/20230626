# Comparing `tmp/blackboardsync-0.9.4rc3.tar.gz` & `tmp/blackboardsync-0.9.4rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.4rc3.tar", last modified: Mon Jun 26 15:01:55 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.4rc4.tar", last modified: Mon Jun 26 15:12:27 2023, max compression
```

## Comparing `blackboardsync-0.9.4rc3.tar` & `blackboardsync-0.9.4rc4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.067740 blackboardsync-0.9.4rc3/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:01:55.000000 blackboardsync-0.9.4rc3/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 15:01:55.000000 blackboardsync-0.9.4rc3/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:01:55.000000 blackboardsync-0.9.4rc3/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 15:01:55.000000 blackboardsync-0.9.4rc3/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:01:55.000000 blackboardsync-0.9.4rc3/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:55.071740 blackboardsync-0.9.4rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 15:01:10.000000 blackboardsync-0.9.4rc3/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.4rc3/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/.github/workflows/build.yml` & `blackboardsync-0.9.4rc4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/.gitignore` & `blackboardsync-0.9.4rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/CHANGELOG.md` & `blackboardsync-0.9.4rc4/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## 0.9.4 - 2023-06-26
+## [0.9.4] - 2023-06-26
 
 ### Added
 - Option to limit the courses downloaded by earliest creation date
 - Release notes from CHANGELOG
 
 ### Fixed
 - App no longer crashes when downloading internet links on Linux
 
 
-## 0.9.3 - 2023-06-25
+## [0.9.3] - 2023-06-25
 
 ### Added
 - Add basic support for 29 universities: Arkansas, UVM, Europea Madrid, ECOTEC, URSE, Palermo,
   Tecnologica del Salvador, Alcala, GWU, APU, Bucks, Northampton, Beds, YSU, Ohio, Princess Nourah,
   Leeds Beckett, Post, UAGM, Alabama, Torrens Australia, Holmes Institute, Trinity College Dublin,
   Georgian College, Cardiff, Sheffield Hallam, West of England, Northumbria, Ulster
 
 ### Fixed
 - Prereleases are marked correctly on Github
 
 ### Changed
 - Small tweak to initial desktop notification on first download
 
-## 0.9.0 - 2023-06-21
+## [0.9.0] - 2023-06-21
 
 ### Changed
 - Finally change data source approach to follow institutional rules
 
 
 ### Added
 - Add basic support for 10 universities: Westminster, Reading,
@@ -43,36 +43,36 @@
 
 
 ### Removed
 - User setting for data source
 
 
 
-## 0.8.3 - 2023-06-16
+## [0.8.3] - 2023-06-16
 
 ### Fixed
 - Opening preferences window would previously crash the program
 - WebDav filepaths are now sanitised
 - Package workflow not triggering on CI
 
 
 
-## 0.8.0 - 2023-06-04
+## [0.8.0] - 2023-06-04
 
 ### Features
 - User must now login in a webview instead, to support 2FA and arbitrary redirects
 - Automatic packaging of macOS and Windows applications in github actions
 - Improved testing strategy
 - Descriptions are now saved as HTML files instead of markdown
 - Attachments which are only linked from within content are now supported
 - Various other minor improvements
 
 
 
-## 0.7.0 - 2021-03-03
+## [0.7.0] - 2021-03-03
 
 ### Features
 - New option to choose whether files should be re-downloaded upon changing the sync location.
 - Sync frequency is now adjustable.
 - If the user session expires, BBSync will reflect this and try to login back in using saved configuration.
 - Some improvements to the UI and experience in Windows.
 - Sync connection errors are now logged to a file.
@@ -82,15 +82,15 @@
 - Added changelog.
 
 ### Fixes
 - File names are now sanitised to comply with (most) Windows file system requirements.
 
 
 
-## 0.5.0 - 2021-02-10
+## [0.5.0] - 2021-02-10
 
 ### Features
 - Added GUI
 - Simplified user setup
```

### Comparing `blackboardsync-0.9.4rc3/CONTRIBUTING.md` & `blackboardsync-0.9.4rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/LICENSE` & `blackboardsync-0.9.4rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/PKG-INFO` & `blackboardsync-0.9.4rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc3
+Version: 0.9.4rc4
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc3/Pipfile` & `blackboardsync-0.9.4rc4/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/Pipfile.lock` & `blackboardsync-0.9.4rc4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/README.md` & `blackboardsync-0.9.4rc4/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/UNIVERSITIES.md` & `blackboardsync-0.9.4rc4/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/__about__.py` & `blackboardsync-0.9.4rc4/blackboard_sync/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.4-rc.3"
+__version__ = "0.9.4-rc.4"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/__init__.py` & `blackboardsync-0.9.4rc4/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/__main__.py` & `blackboardsync-0.9.4rc4/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.4rc4/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/config.py` & `blackboardsync-0.9.4rc4/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/download.py` & `blackboardsync-0.9.4rc4/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/institutions.py` & `blackboardsync-0.9.4rc4/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.4rc4/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/sync.py` & `blackboardsync-0.9.4rc4/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.4rc4/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/universities.json` & `blackboardsync-0.9.4rc4/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/updates.py` & `blackboardsync-0.9.4rc4/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboard_sync/webdav.py` & `blackboardsync-0.9.4rc4/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.4rc4/blackboardsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc3
+Version: 0.9.4rc4
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc3/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.4rc4/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/docs/Makefile` & `blackboardsync-0.9.4rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/docs/conf.py` & `blackboardsync-0.9.4rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/docs/index.rst` & `blackboardsync-0.9.4rc4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/docs/make.bat` & `blackboardsync-0.9.4rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/main.py` & `blackboardsync-0.9.4rc4/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/packaging/pkg_macos.sh` & `blackboardsync-0.9.4rc4/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/packaging/pkg_win.nsi` & `blackboardsync-0.9.4rc4/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/packaging/pyinst.py` & `blackboardsync-0.9.4rc4/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/pyproject.toml` & `blackboardsync-0.9.4rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/strategies.py` & `blackboardsync-0.9.4rc4/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/test_api.py` & `blackboardsync-0.9.4rc4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/test_blackboard.py` & `blackboardsync-0.9.4rc4/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/test_download.py` & `blackboardsync-0.9.4rc4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/test_qt.py` & `blackboardsync-0.9.4rc4/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc3/tests/test_sync_config.py` & `blackboardsync-0.9.4rc4/tests/test_sync_config.py`

 * *Files identical despite different names*

