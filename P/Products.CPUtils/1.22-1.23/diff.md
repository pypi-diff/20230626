# Comparing `tmp/Products.CPUtils-1.22.tar.gz` & `tmp/Products.CPUtils-1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.CPUtils-1.22.tar", last modified: Mon Sep 19 13:13:42 2022, max compression
+gzip compressed data, was "dist/Products.CPUtils-1.23.tar", last modified: Mon Jun 26 11:09:16 2023, max compression
```

## Comparing `Products.CPUtils-1.22.tar` & `Products.CPUtils-1.23.tar`

### file list

```diff
@@ -1,101 +1,100 @@
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/entry_points.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/namespace_packages.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/top_level.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9312 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3013 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/not-zip-safe
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      117 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products.CPUtils.egg-info/requires.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2152 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/setuphandlers.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/skins/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/skins/CPUtils/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      340 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/skins/CPUtils/readme.txt
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      360 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/readme.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      384 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/configure.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      491 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/plone3.zcml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/locales/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      336 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/locales/cputils.pot
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/locales/fr/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/default/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       78 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/default/metadata.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/default/skins.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/default/cputils_default.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/default/import_steps.xml
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/robots/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/robots/cputils_robots.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      378 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles/robots/import_steps.xml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       12 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/version.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/hiddenProductsList.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2267 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/utils.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/model/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35679 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/model/archgenxml.log
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7753 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/model/CPUtils.zargo
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       80 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/model/generate.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2978 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/model/generate.conf
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      289 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkPOSKeyErrors.sh
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      416 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_backup_db.sh
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1197 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_zeo.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      239 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_db.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8598 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/test_db.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      280 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkInstances.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6874 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/zope_restart.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      264 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/restore_db.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2822 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkInstances.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11951 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/restore_db.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10241 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7491 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/update_awstats.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      939 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_zeo.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/test_db.sh
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      197 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/send_log.sh
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      334 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/zope_restart.sh
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10049 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_backup_db.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7602 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkPOSKeyErrors.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2992 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_db.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2251 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/send_log.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/scripts/INSTANCES.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2970 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/config.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/refresh.txt
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/Extensions/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   183991 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/Extensions/utils.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9331 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/Extensions/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      922 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/fckpatch.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     4985 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/testMethods.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3576 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/CPUtilsTestCase.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1939 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/test_functional.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3152 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/framework.py
--rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       24 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2252 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/tests/testNewsLetter.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/data/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/data/robots.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17516 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/__init__.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5728 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/QITool.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      648 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/CPUtils/profiles.zcml
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/src/Products/__init__.py
-drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/docs/
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/docs/LICENSE.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/docs/LICENSE.GPL
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       57 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/requirements.txt
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1664 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/setup.py
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9312 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/PKG-INFO
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      505 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/MANIFEST.in
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5921 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/CHANGES.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/CONTRIBUTORS.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/README.rst
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       83 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/.coveragerc
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/.isort.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/Makefile
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/setup.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2574 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/buildout.cfg
--rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      101 2022-09-19 13:13:42.000000 Products.CPUtils-1.22/ci.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        9 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9691 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2996 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      130 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products.CPUtils.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2152 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/setuphandlers.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/skins/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/skins/CPUtils/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      340 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/skins/CPUtils/readme.txt
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      360 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/readme.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      384 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      491 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/plone3.zcml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/locales/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      336 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/locales/cputils.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      621 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       78 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      320 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/default/skins.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/default/cputils_default.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/default/import_steps.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/robots/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/robots/cputils_robots.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      378 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles/robots/import_steps.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       12 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/version.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      654 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/hiddenProductsList.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2267 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/utils.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/model/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    35679 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/model/archgenxml.log
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7753 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/model/CPUtils.zargo
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       80 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/model/generate.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2978 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/model/generate.conf
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      289 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkPOSKeyErrors.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      416 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_backup_db.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1197 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_zeo.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      239 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_db.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     8598 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/test_db.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      280 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkInstances.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6874 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/zope_restart.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      264 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/restore_db.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2822 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkInstances.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11951 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/restore_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10241 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7491 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/update_awstats.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      939 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_zeo.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      255 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/test_db.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      197 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/send_log.sh
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      334 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/zope_restart.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    10049 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_backup_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     7602 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkPOSKeyErrors.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2992 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_db.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2251 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/send_log.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      235 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/scripts/INSTANCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2970 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/config.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/refresh.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/Extensions/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)   184740 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/Extensions/utils.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9331 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       26 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/Extensions/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      922 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/fckpatch.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     4987 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/testMethods.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3576 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/CPUtilsTestCase.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     1939 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/test_functional.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)     3152 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/framework.py
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)       24 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2252 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/tests/testNewsLetter.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/data/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      248 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/data/robots.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    17516 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     5728 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/QITool.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      648 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/CPUtils/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/src/Products/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       57 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1580 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     9691 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      505 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6312 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      444 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       83 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      218 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/Makefile
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2686 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/buildout.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      101 2023-06-26 11:09:16.000000 Products.CPUtils-1.23/ci.cfg
```

### Comparing `Products.CPUtils-1.22/src/Products.CPUtils.egg-info/PKG-INFO` & `Products.CPUtils-1.23/src/Products.CPUtils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CPUtils
-Version: 1.22
+Version: 1.23
 Summary: Some plone utilities as external methods, monkey patches, etc.
 Home-page: http://pypi.python.org/pypi/Products.CPUtils
 Author: Stephan Geulette
 Author-email: s.geulette@imio.be
 License: GPL
 Description: ====================
         Products.CPUtils
@@ -23,24 +23,31 @@
           - title = cputils_install
           - Module Name = Products.CPUtils.utils
           - Function Name = install
         
         2) click on test to execute added method. This adds all main external methods of utils.py, prefixed by "cputils\_".
         
         
-        Contributors
-        ============
-        
-        
-        - Stephan Geulette, s.geulette@imio.be
-        
         Changelog
         =========
         
         
+        1.23 (2023-06-26)
+        -----------------
+        
+        - Added parameter `use_registry=False` to `configure_ckeditor`, set it to `True`
+          with `collective.ckeditor 4.11+`.
+          [gbastien]
+        - Removed file `CONTRIBUTORS.rst`.
+          [gbastien]
+        - `utils.check_zope_admin` has been moved to `imio.helpers.security`.
+          [gbastien]
+        - Removed `utils.safe_encode` as already imported from `imio.helpers.content`.
+          [gbastien]
+        
         1.22 (2022-09-19)
         -----------------
         
         - Automatically install External methods at the root of Zope app.
           [odelaere]
         
         1.21 (2022-03-15)
```

### Comparing `Products.CPUtils-1.22/src/Products.CPUtils.egg-info/SOURCES.txt` & `Products.CPUtils-1.23/src/Products.CPUtils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 .coveragerc
 .isort.cfg
 CHANGES.rst
-CONTRIBUTORS.rst
 MANIFEST.in
 Makefile
 README.rst
 buildout.cfg
 ci.cfg
 requirements.txt
 setup.py
```

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/setuphandlers.py` & `Products.CPUtils-1.23/src/Products/CPUtils/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po` & `Products.CPUtils-1.23/src/Products/CPUtils/locales/fr/LC_MESSAGES/cputils.po`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/hiddenProductsList.py` & `Products.CPUtils-1.23/src/Products/CPUtils/hiddenProductsList.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/utils.py` & `Products.CPUtils-1.23/src/Products/CPUtils/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/model/archgenxml.log` & `Products.CPUtils-1.23/src/Products/CPUtils/model/archgenxml.log`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/model/CPUtils.zargo` & `Products.CPUtils-1.23/src/Products/CPUtils/model/CPUtils.zargo`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/model/generate.conf` & `Products.CPUtils-1.23/src/Products/CPUtils/model/generate.conf`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_zeo.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_zeo.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/test_db.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/test_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/zope_restart.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/zope_restart.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkInstances.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkInstances.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/restore_db.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/restore_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/utils.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/update_awstats.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/update_awstats.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_zeo.sh` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_zeo.sh`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_backup_db.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_backup_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/checkPOSKeyErrors.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/checkPOSKeyErrors.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/pack_db.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/pack_db.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/scripts/send_log.py` & `Products.CPUtils-1.23/src/Products/CPUtils/scripts/send_log.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/config.py` & `Products.CPUtils-1.23/src/Products/CPUtils/config.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/Extensions/utils.py` & `Products.CPUtils-1.23/src/Products/CPUtils/Extensions/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 # utilities
 
+from imio.helpers.content import safe_encode
+from imio.helpers.security import check_zope_admin
+from plone.registry.interfaces import IRegistry
+from zope.component import getUtility
+
 
 def get_users(self, obj=True):
     from Products.CMFCore.utils import getToolByName
 
     portal = getToolByName(self, "portal_url").getPortalObject()
     users = []
     for user in portal.acl_users.searchUsers():
@@ -19,27 +24,14 @@
 def check_role(self, role="Manager", context=None):
     from Products.CMFCore.utils import getToolByName
 
     pms = getToolByName(self, "portal_membership")
     return pms.getAuthenticatedMember().has_role(role, context)
 
 
-def check_zope_admin():
-    from AccessControl.SecurityManagement import getSecurityManager
-
-    user = getSecurityManager().getUser()
-    if user.has_role("Manager") and user.__module__ in (
-        "Products.PluggableAuthService.PropertiedUser",
-        "AccessControl.users",
-        "AccessControl.User",
-    ):
-        return True
-    return False
-
-
 def fileSize(nb, as_size="", decimal="", rm_sz=False):
     """
         Convert bytes nb in formatted string.
         as_size : force size k, M, G or T
         decimal : replace . decimal by given one
         rm_sz : remove letter size
     """
@@ -88,23 +80,14 @@
                 sobj = getattr(obj, sobjid)
                 allSiteObj.append(sobj)
         elif obj.meta_type == "Plone Site":
             allSiteObj.append(obj)
     return allSiteObj
 
 
-def safe_encode(value, encoding="utf-8"):
-    """
-        Converts a value to encoding, only when it is not already encoded.
-    """
-    if isinstance(value, unicode):
-        return value.encode(encoding)
-    return value
-
-
 def sendmail(self, mfrom="", to="", body="", subject="", cc="", bcc=""):
     """
         send a mail
     """
     from Products.CMFCore.utils import getToolByName
     from Products.CPUtils.config import PLONE_VERSION
     from Products.CMFPlone.utils import safe_unicode
@@ -843,14 +826,15 @@
     custom="",
     rmTiny=1,
     forceTextPaste=1,
     scayt=1,
     removeWsc=1,
     skin="moono-lisa",
     filtering="",
+    use_registry=False
 ):
     """
         configure collective.ckeditor with default parameters.
         This method can be called as an external method, with the following parameters: ...?default=1&alluser=0&custom=0
     """
     if not check_role(self):
         return "You must have a manager role to run this script"
@@ -908,15 +892,19 @@
         pqi = getToolByName(self, "portal_quickinstaller")
         if not pqi.isProductInstalled("collective.ckeditor"):
             pqi.installProduct("collective.ckeditor")
     except Exception, msg:
         return "collective.ckeditor cannot be installed: '%s'" % msg
 
     sp = portal.portal_properties.site_properties
-    ckp = portal.portal_properties.ckeditor_properties
+    if use_registry:
+        registry = getUtility(IRegistry)
+        ck_prefix = "collective.ckeditor.browser.ckeditorsettings.ICKEditorSchema.%s"
+    else:
+        ckp = portal.portal_properties.ckeditor_properties
 
     # setting default editor to ckeditor
     if default:
         portal.portal_memberdata.manage_changeProperties(wysiwyg_editor="CKeditor")
         sp.manage_changeProperties(default_editor="CKeditor")
         out.append("Set ckeditor as default editor")
 
@@ -960,45 +948,68 @@
     # setting custom toolbar
     if custom:
         if custom not in customs:
             return (
                 "custom parameter '%s' not defined in available custom toolbars"
                 % custom
             )
-        ckp = portal.portal_properties.ckeditor_properties
-        if ckp.getProperty("toolbar") != "Custom":
-            ckp.manage_changeProperties(toolbar="Custom")
-            ckp.manage_changeProperties(toolbar_Custom=customs[custom])
+        if use_registry:
+            if registry.get(ck_prefix % "toolbar") != "Custom":
+                registry[ck_prefix % "toolbar"] = "Custom"
+                registry[ck_prefix % "toolbar_Custom"] = safe_encode(customs[custom])
+        else:
+            if ckp.getProperty("toolbar") != "Custom":
+                ckp.manage_changeProperties(toolbar="Custom")
+                ckp.manage_changeProperties(toolbar_Custom=customs[custom])
         out.append("Set '%s' toolbar" % custom)
 
     # force text paste
     if forceTextPaste:
-        ckp.manage_changeProperties(forcePasteAsPlainText=True)
+        if use_registry:
+            registry[ck_prefix % "forcePasteAsPlainText"] = True
+        else:
+            ckp.manage_changeProperties(forcePasteAsPlainText=True)
         out.append("Set forcePasteAsPlainText to True")
 
     # activate scayt
     if scayt:
-        ckp.enableScaytOnStartup = True
+        if use_registry:
+            registry[ck_prefix % "enableScaytOnStartup"] = True
+        else:
+            ckp.enableScaytOnStartup = True
         out.append("Set enableScaytOnStartup to True")
 
     # disable the 'wsc' plugin, removing the wsc plugin will remove the
     # "Check spell" option from Scayt menu that is broken
     if removeWsc:
-        removePlugins = ckp.removePlugins
-        if u'wsc' not in removePlugins:
-            removePlugins += (u'wsc',)
-            ckp.removePlugins = removePlugins
+        if use_registry:
+            removePlugins = registry.get(ck_prefix % "removePlugins")
+            if 'wsc' not in removePlugins:
+                removePlugins += ('wsc',)
+                registry[ck_prefix % "removePlugins"] = removePlugins
+        else:
+            removePlugins = ckp.removePlugins
+            if u'wsc' not in removePlugins:
+                removePlugins += (u'wsc',)
+                ckp.removePlugins = removePlugins
 
     # change filtering
     if filtering and filtering in ("default", "custom", "disabled"):
-        ckp.manage_changeProperties(filtering=filtering)
+        if use_registry:
+            registry[ck_prefix % "filtering"] = filtering
+        else:
+            ckp.manage_changeProperties(filtering=filtering)
         out.append("Set filtering to '{}'".format(filtering))
 
-    if ckp.hasProperty("skin"):
-        ckp.manage_changeProperties(skin=skin)
+    # skin
+    if skin:
+        if use_registry:
+            registry[ck_prefix % "skin"] = skin
+        else:
+            ckp.manage_changeProperties(skin=skin)
 
     return "\n".join(out)
 
 
 def list_users(
     self,
     output="csv",
@@ -1128,15 +1139,15 @@
 
             for groupid in users[userid]["groups"]:
                 if output == "csv":
                     infos = [
                         userid,
                         groupid,
                         users[userid]["name"],
-                        users[userid]["email"],
+                        users[userid]["email"] or '',  # correction for ldap
                     ]
                     if title:
                         infos.insert(2, groups[groupid]["title"])
                     if ignored_global_roles != "*":
                         infos.append(
                             ",".join(users[userid]["roles"])
                         )  # user global roles before groups global roles
@@ -4686,18 +4697,19 @@
     for typ in blob_attrs:
         for brain in portal.portal_catalog(portal_type=typ):
             obj = brain.getObject()
             for attr in blob_attrs[typ]["at"]:
                 try:
                     if blob_attrs[typ]["t"] == "dx":
                         val = getattr(obj, attr)
+                        val.data
                     else:
                         val = obj.getField(attr).get(obj)
-                    val.getSize()
-                except POSKeyError:
+                        val.getSize()
+                except (POSKeyError, SystemError):
                     log_list(
                         ret, "Found damaged object %s on %s" % (typ, obj.absolute_url())
                     )
                 if delt:
                     parent = obj.aq_parent
                     log_list(ret, "  => will be deleted")
                     parent.manage_delObjects([obj.getId()])
```

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py` & `Products.CPUtils-1.23/src/Products/CPUtils/Extensions/ploneboard_wf_scripts.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/fckpatch.py` & `Products.CPUtils-1.23/src/Products/CPUtils/fckpatch.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/tests/testMethods.py` & `Products.CPUtils-1.23/src/Products/CPUtils/tests/testMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         ok = ok and result.find(
             "old properties: visible_ids='False',<br/>->  new properties: visible_ids='True',"
         )
         self.failUnless(ok)
 
     def test_cpdb(self):
         print("push 'c' and then 'return' to pass the test")
-        self.portal.cputils_cpdb()
+        # self.portal.cputils_cpdb()
         "cputils_cpdb test passed"
 
     def old_test_desactivate_base2dom(self):
         result = self.app.cputils_desactivate_base2dom()
         ok = result.find("Disabled ++resource++base2-dom-fp.js for /plone") > -1
         self.failUnless(ok)
```

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/tests/CPUtilsTestCase.py` & `Products.CPUtils-1.23/src/Products/CPUtils/tests/CPUtilsTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/tests/test_functional.py` & `Products.CPUtils-1.23/src/Products/CPUtils/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/tests/framework.py` & `Products.CPUtils-1.23/src/Products/CPUtils/tests/framework.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/tests/testNewsLetter.py` & `Products.CPUtils-1.23/src/Products/CPUtils/tests/testNewsLetter.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/__init__.py` & `Products.CPUtils-1.23/src/Products/CPUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/QITool.txt` & `Products.CPUtils-1.23/src/Products/CPUtils/QITool.txt`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/src/Products/CPUtils/profiles.zcml` & `Products.CPUtils-1.23/src/Products/CPUtils/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/docs/LICENSE.rst` & `Products.CPUtils-1.23/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/docs/LICENSE.GPL` & `Products.CPUtils-1.23/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.CPUtils-1.22/setup.py` & `Products.CPUtils-1.23/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,21 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = (
     open('README.rst').read()
     + '\n\n' +
-    'Contributors\n'
-    '============\n'
-    + '\n\n' +
-    open('CONTRIBUTORS.rst').read()
-    + '\n\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='Products.CPUtils',
-    version='1.22',
+    version='1.23',
     description="Some plone utilities as external methods, monkey patches, etc.",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -39,14 +34,15 @@
     license='GPL',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['Products'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
+        'imio.helpers',
         'plone.api',
         'setuptools',
     ],
     extras_require={
         'test': [
             'plone.app.testing',
             'plone.app.robotframework',
```

### Comparing `Products.CPUtils-1.22/PKG-INFO` & `Products.CPUtils-1.23/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CPUtils
-Version: 1.22
+Version: 1.23
 Summary: Some plone utilities as external methods, monkey patches, etc.
 Home-page: http://pypi.python.org/pypi/Products.CPUtils
 Author: Stephan Geulette
 Author-email: s.geulette@imio.be
 License: GPL
 Description: ====================
         Products.CPUtils
@@ -23,24 +23,31 @@
           - title = cputils_install
           - Module Name = Products.CPUtils.utils
           - Function Name = install
         
         2) click on test to execute added method. This adds all main external methods of utils.py, prefixed by "cputils\_".
         
         
-        Contributors
-        ============
-        
-        
-        - Stephan Geulette, s.geulette@imio.be
-        
         Changelog
         =========
         
         
+        1.23 (2023-06-26)
+        -----------------
+        
+        - Added parameter `use_registry=False` to `configure_ckeditor`, set it to `True`
+          with `collective.ckeditor 4.11+`.
+          [gbastien]
+        - Removed file `CONTRIBUTORS.rst`.
+          [gbastien]
+        - `utils.check_zope_admin` has been moved to `imio.helpers.security`.
+          [gbastien]
+        - Removed `utils.safe_encode` as already imported from `imio.helpers.content`.
+          [gbastien]
+        
         1.22 (2022-09-19)
         -----------------
         
         - Automatically install External methods at the root of Zope app.
           [odelaere]
         
         1.21 (2022-03-15)
```

### Comparing `Products.CPUtils-1.22/CHANGES.rst` & `Products.CPUtils-1.23/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+1.23 (2023-06-26)
+-----------------
+
+- Added parameter `use_registry=False` to `configure_ckeditor`, set it to `True`
+  with `collective.ckeditor 4.11+`.
+  [gbastien]
+- Removed file `CONTRIBUTORS.rst`.
+  [gbastien]
+- `utils.check_zope_admin` has been moved to `imio.helpers.security`.
+  [gbastien]
+- Removed `utils.safe_encode` as already imported from `imio.helpers.content`.
+  [gbastien]
+
 1.22 (2022-09-19)
 -----------------
 
 - Automatically install External methods at the root of Zope app.
   [odelaere]
 
 1.21 (2022-03-15)
```

### Comparing `Products.CPUtils-1.22/buildout.cfg` & `Products.CPUtils-1.23/buildout.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 [code-analysis]
 recipe = plone.recipe.codeanalysis
 pre-commit-hook = True
 return-status-codes = True
 directory =
     ${buildout:directory}/src/Products/CPUtils
-flake8-ignore = E123,E124,E501,E126,E127,E128,W391,C901,W503,W504
+flake8-ignore = E123,E124,E501,E126,E127,E128,W391,C901,W503,W504,W606
 flake8-extensions =
     flake8-isort
 
 [omelette]
 recipe = collective.recipe.omelette
 eggs = ${instance:eggs}
 
@@ -107,12 +107,18 @@
    zopepy
    plone-compile-resources
 
 [versions]
 setuptools=44.1.1
 zc.buildout=2.13.3
 traitlets=4.3.2
-robotframework =
-robotframework-ride =
-robotframework-seleniumlibrary = 4.5.0
-robotsuite =
-selenium =
+zope.configuration = 3.8.1
+pep517 = 0.8.2
+z3c.unconfigure = 1.1
+future = 0.18.2
+zc.lockfile = 1.2.1
+
+#robotframework =
+#robotframework-ride =
+#robotframework-seleniumlibrary = 4.5.0
+#robotsuite =
+#selenium =
```

