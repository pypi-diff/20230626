# Comparing `tmp/PyDapi2-0.4.3.tar.gz` & `tmp/PyDapi2-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDapi2-0.4.3.tar", last modified: Fri Nov 11 16:44:05 2022, max compression
+gzip compressed data, was "PyDapi2-0.6.2.tar", last modified: Mon Jun 26 15:29:32 2023, max compression
```

## Comparing `PyDapi2-0.4.3.tar` & `PyDapi2-0.6.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.995043 PyDapi2-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 16:44:05.995043 PyDapi2-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.987043 PyDapi2-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.987043 PyDapi2-0.4.3/src/PyDapi2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-11-11 16:44:05.000000 PyDapi2-0.4.3/src/PyDapi2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-11 16:44:05.000000 PyDapi2-0.4.3/src/PyDapi2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 16:44:05.000000 PyDapi2-0.4.3/src/PyDapi2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-11 16:44:05.000000 PyDapi2-0.4.3/src/PyDapi2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-11 16:44:05.000000 PyDapi2-0.4.3/src/PyDapi2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.987043 PyDapi2-0.4.3/src/dapi2/
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    21411 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dapi2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/dapi2/dboard/
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/analoginput.py
--rw-r--r--   0 runner    (1001) docker     (121)    32307 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/mb30.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/mb60.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/mb92.py
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dboard/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/dapi2/dcom/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dcom/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dcom/demu.py
--rw-r--r--   0 runner    (1001) docker     (121)     8610 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dcom/dserial.py
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dcom/dsocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     8815 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/derror.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/dapi2/dmsg/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dmsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dmsg/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dmsg/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dmsg/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dmsg/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/dapi2/dreg/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6756 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/dapi2/dreg/dev/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/dev/dev.py
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    12717 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/register.py
--rw-r--r--   0 runner    (1001) docker     (121)    20369 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/dreg/regs.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7838 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/errors.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/dapi2/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 16:44:05.991043 PyDapi2-0.4.3/src/demu/
--rw-r--r--   0 runner    (1001) docker     (121)    14698 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/demu/DEmuBaseBoard.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/demu/DEmuBaseMotor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/demu/DEmuPPA.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 16:43:55.000000 PyDapi2-0.4.3/src/demu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.643884 PyDapi2-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.643884 PyDapi2-0.6.2/src/PyDapi2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 15:29:32.000000 PyDapi2-0.6.2/src/PyDapi2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-26 15:29:32.000000 PyDapi2-0.6.2/src/PyDapi2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:29:32.000000 PyDapi2-0.6.2/src/PyDapi2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 15:29:32.000000 PyDapi2-0.6.2/src/PyDapi2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 15:29:32.000000 PyDapi2-0.6.2/src/PyDapi2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.643884 PyDapi2-0.6.2/src/dapi2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dapi2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/dapi2/dboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/analoginput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31212 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/mb30.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/mb60.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/mb92.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dboard/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/dapi2/dcom/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dcom/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dcom/demu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dcom/dserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dcom/dsocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/derror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/dapi2/dmsg/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dmsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dmsg/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dmsg/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dmsg/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dmsg/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/dapi2/dreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/dapi2/dreg/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/dev/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/dreg/regs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/errors.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/dapi2/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:32.647884 PyDapi2-0.6.2/src/demu/
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/demu/DEmuBaseBoard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/demu/DEmuBaseMotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/demu/DEmuPPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:29:23.000000 PyDapi2-0.6.2/src/demu/__init__.py
```

### Comparing `PyDapi2-0.4.3/LICENSE` & `PyDapi2-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/PKG-INFO` & `PyDapi2-0.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDapi2
-Version: 0.4.3
+Version: 0.6.2
 Summary: The PyDapi2 library offers a Python implementation of the Dassym API version 2.
 Home-page: https://github.com/dassym/PyDapi2
 Author: Fabrice Voillat
 Author-email: dev@dassym.com
 Keywords: Dassym,motor,api,dapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,28 +14,28 @@
 
 # PyDapi2
 The *PyDapi2* library offers a Python implementation of the Dassym API version 2.
 
 Dassym API version 2 aka **DAPI2** is the application programming interface (API) used to
 control Dassym electronic boards.
 
-This library was created to meet the internal needs of Dassym. It is distributed to help 
+This library was created to meet the internal needs of Dassym. It is distributed to help
 our partners to implement their own solutions working with Dassym electronic cards.
 
-Version: 0.4.3 (2022-11-11)
+Version: 0.6.2 (2023-06-26)
 
-This program is free software: you can redistribute it and/or modify 
-it under the terms of the **GNU General Public License** as published by 
-the Free Software Foundation, either version 3 of the License, or 
+This program is free software: you can redistribute it and/or modify
+it under the terms of the **GNU General Public License** as published by
+the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-This program is distributed in the hope that it will be useful, 
-but WITHOUT ANY WARRANTY; without even the implied warranty of 
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the 
-GNU General Public License for more details. 
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
 You can consult the GNU General Public License on <http://www.gnu.org/licenses/gpl-3.0.html>.
 
 
 ## Install
 
 This installs a package that can be used from Python (import dapi2).
@@ -55,12 +55,12 @@
 
 
 ### From source
 
 Download the archive from <https://github.com/dassym/PyDapi2/releases>.
 Unpack the archive, enter the PyDapi2-x.y.z directory and run:
 
-> python setup.py install 
+> python setup.py install
 
 Use `python` or `python3` depending on your system.
 Usually `python` on a *Windows* system and `python3` on a *GNU/Linux* system.
```

### Comparing `PyDapi2-0.4.3/README.md` & `PyDapi2-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # PyDapi2
 The *PyDapi2* library offers a Python implementation of the Dassym API version 2.
 
 Dassym API version 2 aka **DAPI2** is the application programming interface (API) used to
 control Dassym electronic boards.
 
-This library was created to meet the internal needs of Dassym. It is distributed to help 
+This library was created to meet the internal needs of Dassym. It is distributed to help
 our partners to implement their own solutions working with Dassym electronic cards.
 
-Version: 0.4.3 (2022-11-11)
+Version: 0.6.2 (2023-06-26)
 
-This program is free software: you can redistribute it and/or modify 
-it under the terms of the **GNU General Public License** as published by 
-the Free Software Foundation, either version 3 of the License, or 
+This program is free software: you can redistribute it and/or modify
+it under the terms of the **GNU General Public License** as published by
+the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-This program is distributed in the hope that it will be useful, 
-but WITHOUT ANY WARRANTY; without even the implied warranty of 
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the 
-GNU General Public License for more details. 
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
 You can consult the GNU General Public License on <http://www.gnu.org/licenses/gpl-3.0.html>.
 
 
 ## Install
 
 This installs a package that can be used from Python (import dapi2).
@@ -41,12 +41,12 @@
 
 
 ### From source
 
 Download the archive from <https://github.com/dassym/PyDapi2/releases>.
 Unpack the archive, enter the PyDapi2-x.y.z directory and run:
 
-> python setup.py install 
+> python setup.py install
 
 Use `python` or `python3` depending on your system.
 Usually `python` on a *Windows* system and `python3` on a *GNU/Linux* system.
```

### Comparing `PyDapi2-0.4.3/setup.py` & `PyDapi2-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDapi2",
-    version="0.4.3",
+    version="0.6.2",
     author="Fabrice Voillat",
     author_email="dev@dassym.com",
     keywords = ['Dassym', 'motor', 'api', 'dapi'],
     description="The PyDapi2 library offers a Python implementation of the Dassym API version 2.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = ['lxml'],
```

### Comparing `PyDapi2-0.4.3/src/PyDapi2.egg-info/PKG-INFO` & `PyDapi2-0.6.2/src/PyDapi2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDapi2
-Version: 0.4.3
+Version: 0.6.2
 Summary: The PyDapi2 library offers a Python implementation of the Dassym API version 2.
 Home-page: https://github.com/dassym/PyDapi2
 Author: Fabrice Voillat
 Author-email: dev@dassym.com
 Keywords: Dassym,motor,api,dapi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,28 +14,28 @@
 
 # PyDapi2
 The *PyDapi2* library offers a Python implementation of the Dassym API version 2.
 
 Dassym API version 2 aka **DAPI2** is the application programming interface (API) used to
 control Dassym electronic boards.
 
-This library was created to meet the internal needs of Dassym. It is distributed to help 
+This library was created to meet the internal needs of Dassym. It is distributed to help
 our partners to implement their own solutions working with Dassym electronic cards.
 
-Version: 0.4.3 (2022-11-11)
+Version: 0.6.2 (2023-06-26)
 
-This program is free software: you can redistribute it and/or modify 
-it under the terms of the **GNU General Public License** as published by 
-the Free Software Foundation, either version 3 of the License, or 
+This program is free software: you can redistribute it and/or modify
+it under the terms of the **GNU General Public License** as published by
+the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-This program is distributed in the hope that it will be useful, 
-but WITHOUT ANY WARRANTY; without even the implied warranty of 
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the 
-GNU General Public License for more details. 
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
 You can consult the GNU General Public License on <http://www.gnu.org/licenses/gpl-3.0.html>.
 
 
 ## Install
 
 This installs a package that can be used from Python (import dapi2).
@@ -55,12 +55,12 @@
 
 
 ### From source
 
 Download the archive from <https://github.com/dassym/PyDapi2/releases>.
 Unpack the archive, enter the PyDapi2-x.y.z directory and run:
 
-> python setup.py install 
+> python setup.py install
 
 Use `python` or `python3` depending on your system.
 Usually `python` on a *Windows* system and `python3` on a *GNU/Linux* system.
```

### Comparing `PyDapi2-0.4.3/src/PyDapi2.egg-info/SOURCES.txt` & `PyDapi2-0.6.2/src/PyDapi2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/__init__.py` & `PyDapi2-0.6.2/src/dapi2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/common.py` & `PyDapi2-0.6.2/src/dapi2/common.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dapi2.py` & `PyDapi2-0.6.2/src/dapi2/dapi2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,357 +1,425 @@
-'''Module for DApi2 object class. 
+'''Module for DApi2 object class.
 
 :author: F. Voilat
 :date: 2021-02-24 Creation
 '''
 
 import logging
 from itertools import groupby
 from operator import itemgetter
 from os.path import os
 
 
 from . import dmsg, REG_SIZE
-from .dreg import RegContainer, RegContainerReader, RegisterArray
+from .dreg import RegContainer, RegContainerReader, RegisterArray, RegGroup
 
 
 from .common import DApi2Side
-from . import _version 
+from . import _version
 from .common import dateToWord, versionToWord, DIntEnum
 from .derror import DApiCommandError, DErrorsContainer
 
 
 
+
 class DApi2(object):
-    '''Class for DAPI2 object. 
-    
+    '''Class for DAPI2 object.
+
     This object is used to handle and manage the registers and commands of the DAPI2 protocol
-    
-    :param DBaseCom dcom: Communication channel  
+
+    :param DBaseCom dcom: Communication channel
     '''
 
 
     def __init__(self, dcom, regsfile=None, dev_mode=False, errorsfile=None):
         '''Constructor'''
         self.log = logging.getLogger(self.__class__.__name__)
         self.log.debug('Initialize')
         self.regs = RegContainer(self)
         self.lastError = 0
-        
+
         self.cmd = DApi2Commands(self)
-        
+
         if regsfile is None:
             regsfile = os.path.join(os.path.dirname(__file__), 'dreg','regs.xml')
-        
+
         _ = RegContainerReader(container=self.regs, filename=regsfile)
-        
+
         if errorsfile is None:
-            errorsfile = os.path.join(os.path.dirname(__file__), 'errors.xml')        
-        self.derrors = DErrorsContainer(self, errorsfile) 
-        
+            errorsfile = os.path.join(os.path.dirname(__file__), 'errors.xml')
+        self.derrors = DErrorsContainer(self, errorsfile)
+
         self.dcom = dcom
         self.dev_mode = dev_mode
-        
+
     def version(self):
         '''Returns the DAPI2 version'''
         return _version.__version__
-        
-        
+
+
     def sendMessage(self, msg):
         '''Sends a message to the `SLAVE` and waits its response.
-        
+
         :param BaseMasterMessage msg: The message to send.
-        
+
         :return The response message received from the `SLAVE`
         :rtype: BaseSlaveMessage.
         '''
         assert self.dcom.side == DApi2Side.MASTER
         self.dcom.sendMessage(msg)
         res = self.dcom.receiveMessage(msg.type())
         if res.isError():
             self.lastErrorNo = res.getError()
         else:
             self.lastErrorNo = 0
-        return res 
-        
-        
+        return res
+
+
     def readRegGroup(self, group):
         '''Read all registers of a group.
-        
-        :param RegGroup group: The registers group (:class:`~dapi2.dreg.group.RegGroup`). 
+
+        :param RegGroup group: The registers group (:class:`~dapi2.dreg.group.RegGroup`).
         '''
         self.readRegs(group.regs)
-        
-    def readRegs(self, *regs, length=0): 
+
+    def readRegs(self, *regs, length=0):
         '''Read a list of registers.
-        
-        :note: The registers in list must be continuous. 
-        
-        :param Register or list regs: The list of registers (:class:`~dapi2.dreg.register.Register`). 
-        '''    
+
+        :note: The registers in list must be continuous.
+
+        :param Register or list regs: The list of registers (:class:`~dapi2.dreg.register.Register`).
+        '''
         def _readRegs(regs):
             msg = dmsg.ReadRegMessage(regs[0].addr, len(regs)*REG_SIZE)
             msg = self.sendMessage(msg)
             for i, reg in enumerate(regs):
                 v = msg.getData(i*REG_SIZE, REG_SIZE)
                 reg.internalSet(v)
-        
+
         if len(regs) == 0:
-            return 
+            return
         #assert (length == 0 or len(regs)==1) and isinstance(regs[0], BaseRegElement), 'regs[0]='+str(regs[0])
         #print(len(regs) == 1 or any((isinstance(item,BaseRegElement) for item in regs)))
         if length > 0:
             regs = self.regs[regs[0].addr:regs[0].addr+length]
-        elif len(regs) == 1 and isinstance(regs[0], (list,tuple)):
+        elif len(regs) == 1 and isinstance(regs[0], (list,tuple, RegGroup)):
             regs = regs[0]
         else:
             regs = list(regs)
-            
-        
+
+
         regs.sort()
         if isinstance(regs[0], RegisterArray):
             cregs = [list(regs[0])]
         else:
             cregs = [[regs[0]]]
         for r in regs[1:]:
             if isinstance(r, RegisterArray):
                 cregs.append(list(r))
             elif r.addr == cregs[-1][-1].addr+1:
                 cregs[-1].append(r)
             else:
                 cregs.append([r])
         #assert regs[-1].addr - regs[0].addr +1 == len(regs), 'Registers must be continuous'
         for regs in cregs:
-            chunks = [regs[i:i + 4] for i in range(0, len(regs), 4)]  
+            chunks = [regs[i:i + 4] for i in range(0, len(regs), 4)]
             for chunk in chunks:
-                _readRegs(chunk) 
-        
+                _readRegs(chunk)
+
     def readReg(self, reg):
         '''Read one register.
-        
-        :param Register reg: The register to read. 
+
+        :param Register reg: The register to read.
         '''
         self.readRegs(reg)
-        
-    
+
+
     def writeRegs(self, regs):
         '''Write a list of registers.
-        
-        :note: The registers in list must be continuous. 
-        
-        :param list regs: The list of registers (:class:`~dapi2.dreg.register.Register`). 
+
+        :note: The registers in list must be continuous.
+
+        :param list regs: The list of registers (:class:`~dapi2.dreg.register.Register`).
         '''
 
         def _writeRegs(regs):
-            #print('regs:',' '.join((str(x) for x in regs))  ) 
+            #print('regs:',' '.join((str(x) for x in regs))  )
             msg = dmsg.WriteRegMessage(regs[0].addr, [r.get() for r in regs])
             msg = self.sendMessage(msg)
             for i, reg in enumerate(regs):
                 v = msg.getData(i, REG_SIZE)
                 reg.internalSet(v)
-        
-        
-        regs.sort() 
+
+
+        regs.sort()
         assert regs[-1].addr - regs[0].addr +1 == len(regs), 'Registers must be continuous'
-        chunks = [regs[i:i + 4] for i in range(0, len(regs), 4)]  
+        chunks = [regs[i:i + 4] for i in range(0, len(regs), 4)]
         for chunk in chunks:
             if len(chunk)>0:
-                _writeRegs(chunk) 
-    
+                _writeRegs(chunk)
+
     def writeReg(self, reg, value=None):
         '''Write one register.
-        
-        :param Register reg: The register to write. 
-        :param int value: The new value of the register before writing it. 
+
+        :param Register reg: The register to write.
+        :param int value: The new value of the register before writing it.
         '''
         if value is not None:
             reg.internalSet(value)
         self.writeRegs([reg])
-        
+
     def syncRegs(self):
         tmp = enumerate(self.regs.modifiedRegs())
         for _, g in groupby(tmp, lambda x: x[0]-x[1].addr):
             regs = list(map(itemgetter(1), g))
             self.writeRegs(regs)
-            
+
+    def isLinked(self):
+        return self.dcom and self.dcom.isOpen() or False
+
 
 class DApiAccessLevel(DIntEnum):
     '''Enumeration for DAPI2 access level'''
     NO = 0
     '''No access or disconnected'''
     USER = 1
     '''*User* access level.'''
     SERVICE = 2
     '''*Service* access level.'''
     FACTORY = 3
     '''*Factory* access level.'''
-    
+
     @property
     def label(self):
         '''Label according access level'''
         return {
             self.NO : 'No',
             self.USER : 'User',
             self.SERVICE : 'Service',
             self.FACTORY : 'Factory',
-            }[self]    
+            }[self]
 
     @property
     def help(self):
         '''Help message accordinDApiAccessLevelg access level'''
         return {
             self.NO : 'No access granted.',
             self.USER : 'Standard acces.',
             self.SERVICE : 'Large access for services.',
             self.FACTORY : 'Extended access for factory.',
-            }[self]    
-    
+            }[self]
+
     @property
     def passwd(self):
         '''Passwords corresponding to the access level'''
         return {
             self.NO : 0x0000,
             self.USER : 0x0000,
             self.SERVICE : 0xe8e8,
             self.FACTORY : 0xf3f3,
-            }[self]    
+            }[self]
+
+class DApiControllerType(DIntEnum):
+    NO  = 0x0000
+    BRUSH  = 0x0001
+    S30 = 0x0003
+    S50 = 0x0005
+    UNIVERSAL = 0x0006
+    S90 = 0x0009
+    SCALER = 0x000A
+    LAMP = 0x000B
+    DC =  0x000C
+    TEST = 0x000F
+
+    @property
+    def descr(self):
+        '''Controller type label'''
+        return {
+            self.NO  : 'No controller',
+            self.BRUSH : 'DC brush motor',
+            self.S30 : 'Bruchless series 30',
+            self.S50 : 'Bruchless series 50',
+            self.UNIVERSAL : 'Universal brushless motor',
+            self.S90 : 'Bruchless series 90',
+            self.SCALER : 'Scaler',
+            self.LAMP : 'Lamp only',
+            self.DC : 'Universal DC',
+            self.TEST : 'Test'
+            }[self]
+
+    @property
+    def help(self):
+        '''Peripheral type help message'''
+        return {
+            self.NO  : 'No controller loaded',
+            self.BRUSH : '"Dentistry" DC motor controller',
+            self.S30 : 'Series 30 controller (brush less sensor less)',
+            self.S50 : 'Series 50 controller (brush less with embedded micro-controller)',
+            self.UNIVERSAL : 'Universal "Dentistry" motor controller (DC, 30, 50 & 90 series)',
+            self.S90 : 'Series 90 controller (brush less with orthogonal hall sensors)',
+            self.SCALER : 'Scaler controller',
+            self.LAMP : 'Lamp onyl controller',
+            self.DC : 'Universal DC',
+            self.TEST : 'Special controller for test purpose'
+            }[self]
+
+class DApiPeripheralType(DIntEnum):
+    UNDEFINED = 0x0000
+    MOTOR = 0x4d4f
+
+    @property
+    def descr(self):
+        '''Peripheral type label'''
+        return {
+            self.UNDEFINED : 'Undefined',
+            self.MOTOR : 'Motor',
+            }[self]
+
+    @property
+    def help(self):
+        '''Peripheral type help message'''
+        return {
+            self.UNDEFINED : 'Undefined type of peripheral.',
+            self.MOTOR : 'The current peripheral is a motor.',
+            }[self]
 
 
 class DApiAdditionalBoard(DIntEnum):
-    '''Enumeration for DAPI2 access level'''
+    '''Enumeration for DAPI2 additional boards'''
     NO = 0
     AB14 = 1
     AB12 = 2
     AB1214 = 3
     AB03 = 4
     AB0314 = 5
-    
-    
+
+
     @property
     def descr(self):
-        '''Label according access level'''
+        '''Label according additional boards code'''
         return {
             self.NO : 'No',
             self.AB14 : 'AB-14',
             self.AB12 : 'AB-12',
             self.AB1214 : 'AB-12+AB-14',
             self.AB03 : 'AB-03',
             self.AB0314 : 'AB-03+AB-14',
-            }[self]    
+            }[self]
 
     @property
     def help(self):
-        '''Help message according access level'''
+        '''Help message according additional boards code'''
         return {
             self.NO : 'No additional board is present.',
             self.AB14 : 'DIP switches board (AB-14) is present',
             self.AB12 : 'Auxiliary inputs board (AB-12) is present.',
             self.AB1214 : 'Auxiliary inputs board (AB-12) and DIP switches (AB-14) are present.',
             self.AB03 : 'Dual lighting (AB-03) and DIP switches (AB-14) are present.',
             self.AB0314 : 'AB-03+AB-14',
-            }[self]    
-        
+            }[self]
+
 class MetaDApi2Commands(object):
     NULL                  = 0x00
     '''*Null* command'''
     REBOOT                = 0x01
     '''Board reboot'''
-    
+
     STANDBY               = 0x02
     '''Set the system in stand-by mode'''
-    
+
     PERIPHERAL_ACTIVATE   = 0x03
     '''Activates a peripheral.'''
-    
+
     EMERGENCY             = 0x04
     '''Immediately disable the drivers and set the system in stand-by mode'''
-    
+
     CONNECT               = 0x05
     '''Connection of the MASTER to the board'''
-    
+
     DISCONNECT            = 0x06
     '''Disconnection of the MASTER from board'''
-    
+
     GET_MC_SN             = 0x09
     '''Get the micro-controller unique identifier'''
-    
+
     BOOT_FLASH            = 0x0a
     '''Puts the system in flash boot mode'''
-    
+
     MOTOR_FREEWHEEL_STOP = 0x20
     '''Freewheel motor stop'''
-    
+
     MOTOR_STOP           = 0x21
     '''Controlled motor stop'''
-    
+
     MOTOR_START          = 0x22
     '''Starts the motor and sets the speed.'''
-    
+
     MOTOR_INC_SPEED      = 0x23
     '''Increase motor speed'''
-    
+
     MOTOR_DEC_SPEED      = 0x24
     '''Decrease motor speed'''
-    
-    MOTOR_REVERSE        = 0x25 
+
+    MOTOR_REVERSE        = 0x25
     '''Reverse the motor direction'''
-    
+
     LIGHT_OFF            = 0x40
     '''Turn light off.'''
-    
+
     LIGHT_ON             = 0x41
     '''Turn light on.'''
-    
+
     LIGHT_INTENSITY      = 0x42
     '''Sets the light intensity'''
-    
-    LIGHT_ALTERNATE      = 0x43 
-    '''Sets the alternate light'''    
-    
-
-    
-    
-    MEMORY_STORE          = 0x50 
+
+    LIGHT_ALTERNATE      = 0x43
+    '''Sets the alternate light'''
+
+
+
+
+    MEMORY_STORE          = 0x50
     '''Store user set points into EEPROM.'''
-    
+
     MEMORY_RECALL        = 0x51
     '''Recall user set points from EEPROM'''
-    
+
     MEMORY_READ           = 0x52
     '''Read user set points from EEPROM'''
-    
+
     MEMORY_RESET          = 0x53
     '''Reset user set points with factory values'''
-    
+
     MEMORY_SET            = 0x54
     '''Gets any set point from EEPROM.'''
-    
+
     MEMORY_GET            = 0x55
     '''Sets any set point to the EEPROM'''
-    
+
     # DIAG_0                = 0x60
     # DIAG_1                = 0x61
     # DIAG_2                = 0x62
     # DIAG_3                = 0x63
-    
+
     FACT_EEPROM_RESET     = 0x80
     FACT_SET_SYSINFO      = 0x81
     FACT_SET_SRVINFO      = 0x82
     FACT_CALIBRATION      = 0x83
-    
+
     FLASH_BEGIN           = 0x90
     FLASH_DATA            = 0x91
     FLASH_END             = 0x92
-    
+
     DEBUG_BURST           = 0xC0
     DEBUG_READ_WORD       = 0xC2
     DEBUG_WRITE_WORD      = 0xC3
-        
+
 class DApi2Commands(MetaDApi2Commands):
-    
+
 
     _index = {
         MetaDApi2Commands.NULL   : "*Null* command",
         MetaDApi2Commands.REBOOT : "Board reboot",
         MetaDApi2Commands.STANDBY : "Set the system in stand-by mode",
         MetaDApi2Commands.PERIPHERAL_ACTIVATE : "Activates a peripheral.",
         MetaDApi2Commands.EMERGENCY : "Immediately disable the drivers and set the system in stand-by mode",
@@ -382,254 +450,253 @@
         MetaDApi2Commands.FLASH_BEGIN : "Starts the flash programming procedure",
         MetaDApi2Commands.FLASH_DATA : "Send data for flash programming procedure",
         MetaDApi2Commands.FLASH_END : "Terminates the flash programming procedure",
         MetaDApi2Commands.DEBUG_BURST : "Debug: simulates a electrical burst",
         MetaDApi2Commands.DEBUG_READ_WORD : "Debug: read a word (16bit) from MCU memory",
         MetaDApi2Commands.DEBUG_WRITE_WORD : "Debug: write a word (16bit) into MCU memory",
     }
-    
+
     def __init__(self, owner):
         assert isinstance(owner, DApi2)
         self.owner = owner
-        
+
     def _sendCmd(self, msg, *exceptions):
         msg = self.owner.sendMessage(msg)
         if msg.isError():
             raise DApiCommandError.factory(msg, *exceptions)
         return msg
-        
+
     def connect(self, level=DApiAccessLevel.USER, passwd=DApiAccessLevel.USER.passwd):
         msg = dmsg.CommandMessage(DApi2Commands.CONNECT)
         msg.setByte(level)
         msg.setWord(passwd)
         msg = self._sendCmd(msg, DApiCmdConnectionDeniedError)
-        
-        
+
+
     def disconnect(self):
         msg = dmsg.CommandMessage(DApi2Commands.DISCONNECT)
         msg = self._sendCmd(msg)
-        
+
     def reboot(self):
         msg = dmsg.CommandMessage(DApi2Commands.REBOOT)
         msg = self._sendCmd(msg)
-        
+
     def standby(self):
         msg = dmsg.CommandMessage(DApi2Commands.STANDBY)
         msg = self._sendCmd(msg)
-    
-    
+
+
     def peripheralActivate(self, value):
         if value != 0 and self.owner.regs.par.value != 0 and not self.owner.dev_mode:
             self.standby()
         msg = dmsg.CommandMessage(DApi2Commands.PERIPHERAL_ACTIVATE)
         msg.setWord(value)
         msg = self._sendCmd(msg)
-        
-            
-        
+
+
+
     def getMcId(self, part):
         msg = dmsg.CommandMessage(DApi2Commands.GET_MC_SN)
         msg.setByte(part)
         msg = self._sendCmd(msg)
         return msg.getDataBytes()
-        
-    def bootflash(self):    
+
+    def bootflash(self):
         msg = dmsg.CommandMessage(DApi2Commands.BOOT_FLASH)
         msg = self._sendCmd(msg)
-         
-    
-    def factEerpomReset(self):    
+
+
+    def factEerpomReset(self):
         msg = dmsg.CommandMessage(DApi2Commands.FACT_EEPROM_RESET)
         msg = self._sendCmd(msg)
-         
-    
-    def factSetSysinfo(self, sn, date, hv):    
+
+
+    def factSetSysinfo(self, sn, date, hv):
         date = dateToWord(date)
         hv = versionToWord(*hv)
         msg = dmsg.CommandMessage(DApi2Commands.FACT_SET_SYSINFO)
         msg.setWord(sn)
         msg.setWord(date)
         msg.setWord(hv)
         msg = self._sendCmd(msg)
         self.owner.regs.snr.value = sn
         self.owner.regs.fdr.value = date
         self.owner.regs.hvr.value = hv
-         
 
-    def factSetSrvinfo(self, service, date, tag):    
+
+    def factSetSrvinfo(self, service, date, tag):
         msg = dmsg.CommandMessage(DApi2Commands.FACT_SET_SRVINFO)
         msg.setWord(service)
         msg.setWord(dateToWord(date))
         msg.setWord(tag)
         msg = self._sendCmd(msg)
-        
-    
-    def factCalibration(self, item, step):    
+
+
+    def factCalibration(self, item, step):
         msg = dmsg.CommandMessage(DApi2Commands.FACT_CALIBRATION)
         msg.setByte(item)
         msg.setByte(step)
         msg = self._sendCmd(msg, DApiCmdCalibrationItemError, DApiCmdCalibrationStepError)
-        
 
-    def factCtrl(self, ctrl, p0, p1):    
+
+    def factCtrl(self, ctrl, p0, p1):
         msg = dmsg.CommandMessage(DApi2Commands.FACT_CTRL)
         msg.setByte(ctrl)
         msg.setByte(p0)
         msg.setWord(p1)
         msg = self._sendCmd(msg)
-        
-        
+
+
     def motorFreewheelStop(self):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_FREEWHEEL_STOP)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
         self.owner.regs.smr.bits.freewheel.set()
         self.owner.regs.smr.bits.start.clear()
-        
+
 
     def motorStop(self):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_STOP)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
-        self.owner.regs.smr.bits.freewheel.clear()
-        self.owner.regs.smr.bits.start.clear()
-        
-        
+        #self.owner.regs.smr.bits.freewheel.clear()
+        self.owner.regs.smr.bits.start.internalSet(0)
+
+
     def motorStart(self, speed=0):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_START)
         msg.setWord(speed)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
-        self.owner.regs.smr.bits.start.set()
+        self.owner.regs.smr.bits.start.internalSet(1)
         if speed != 0:
             self.owner.readReg(self.owner.regs.scr)
             #self.owner.regs.scr.value = speed
-       
+
     def motorIncSpeed(self, inc=1):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_INC_SPEED)
         msg.setWord(inc)
         msg = self._sendCmd(msg)
         self.owner.regs.scr.value += inc
-    
+
     def motorDecSpeed(self, dec=1):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_DEC_SPEED)
         msg.setWord(dec)
         msg = self._sendCmd(msg)
         self.owner.regs.scr.value -= dec
-    
+
     def motorReverse(self):
         msg = dmsg.CommandMessage(DApi2Commands.MOTOR_REVERSE)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
         self.owner.regs.smr.bits.reverse.toggle()
-        
+
     def lightOff(self):
         msg = dmsg.CommandMessage(DApi2Commands.LIGHT_OFF)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
         self.owner.regs.smr.bits.light.clear()
-        
+
     def lightOn(self):
         msg = dmsg.CommandMessage(DApi2Commands.LIGHT_ON)
         msg = self._sendCmd(msg)
         if self.owner.regs.smr.isUndefined():
             self.owner.readReg(self.owner.regs.smr)
         self.owner.regs.smr.bits.light.set()
 
     def lightIntensity(self, intensity):
         msg = dmsg.CommandMessage(DApi2Commands.LIGHT_INTENSITY)
         msg.setWord(intensity)
         msg = self._sendCmd(msg)
-        self.owner.regs.lir.value = intensity  
-        
+        self.owner.regs.lir.value = intensity
+
 
     def lightAlternate(self, alternate):
         msg = dmsg.CommandMessage(DApi2Commands.LIGHT_ALTERNATE)
         msg.setWord(alternate)
         msg = self._sendCmd(msg)
         self.owner.regs.alr.value = alternate
-        
+
 
     def memoryStore(self, index):
         msg = dmsg.CommandMessage(DApi2Commands.MEMORY_STORE)
         msg.setByte(index)
         msg = self._sendCmd(msg)
-        
+
 
     def memoryRecall(self, index):
         msg = dmsg.CommandMessage(DApi2Commands.MEMORY_RECALL)
         msg.setByte(index)
         msg = self._sendCmd(msg)
-        
+
 
     def memoryRead(self, peripheral, memory, page):
         msg = dmsg.CommandMessage(DApi2Commands.MEMORY_READ)
         msg.setByte(peripheral)
         msg.setByte(memory)
         msg.setByte(page)
         msg = self._sendCmd(msg)
         return msg.getDataWords()
-        
+
     def memoryReset(self):
         msg = dmsg.CommandMessage(DApi2Commands.MEMORY_RESET)
         msg = self.owner._sendCmd(msg)
-        
+
     def memoryGet(self, peripheral, memory, page):
         msg = dmsg.CommandMessage(DApi2Commands.MEMORY_READ)
         msg.setByte(peripheral)
         msg.setByte(memory)
         msg.setByte(page)
         msg = self._sendCmd(msg)
         return msg.getDataBytes()
-        
+
     def flashBegin(self, size):
         msg = dmsg.CommandMessage(DApi2Commands.FLASH_BEGIN)
         msg.setDWord(size)
         msg = self._sendCmd(msg, DApiCmdFlashError, DApiCmDFlashUnexpectedEndError)
-        
+
     def flashData(self, buf):
         msg = dmsg.CommandMessage(DApi2Commands.FLASH_DATA)
         for b in buf:
             msg.setByte(b)
         msg = self._sendCmd(msg, DApiCmdFlashError, DApiCmDFlashUnexpectedEndError)
-        
+
     def flashEnd(self):
         msg = dmsg.CommandMessage(DApi2Commands.FLASH_END)
         msg = self._sendCmd(msg, DApiCmdFlashError, DApiCmDFlashUnexpectedEndError)
-        
-        
-    
+
+
+
 class DApiCmdConnectionDeniedError(DApiCommandError):
     errorno = (0x81,0x81)
     name    = 'DAPI_CMD_CONNECTION_DENIED'
     label   = 'Connection denied'
-    text    = 'Connection denied'    
+    text    = 'Connection denied'
 
 class DApiCmdCalibrationItemError(DApiCommandError):
     errorno = (0x81,0x81)
     name    = 'DAPI_CMD_CALIBRATION_WRONG_ITEM'
     label   = 'Wrong item'
-    text    = 'Wrong item'    
+    text    = 'Wrong item'
 
 class DApiCmdCalibrationStepError(DApiCommandError):
     errorno = (0x82,0x82)
     name    = 'DAPI_CMD_CALIBRATION_WRONG_STEP'
     label   = 'Wrong step'
-    text    = 'Wrong step'    
+    text    = 'Wrong step'
 
 class DApiCmdFlashError(DApiCommandError):
     errorno = (0x81,0x81)
     name    = 'DAPI_CMD_FLASH_FAILURE'
     label   = 'Flash failure'
-    text    = 'Flash failure'    
-        
+    text    = 'Flash failure'
+
 class DApiCmDFlashUnexpectedEndError(DApiCommandError):
     errorno = (0x82,0x82)
     name    = 'DAPI_CMD_FLASH_ENEXPECTED_END'
     label   = 'Flash unexpected end'
-    text    = 'Flash unexpected end'    
-        
+    text    = 'Flash unexpected end'
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/__init__.py` & `PyDapi2-0.6.2/src/dapi2/dboard/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/base.py` & `PyDapi2-0.6.2/src/dapi2/dboard/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,85 +13,86 @@
 from dapi2.dapi2 import DApiAccessLevel, DApiAdditionalBoard
 from dapi2.common import versionToWord, dateToWord, wordToDate, wordToVersion, DAPI_ACCESS_LEVEL_MASK
 from dapi2.dmsg.message import CommandMessage
 from dapi2.signal import DSignal
 
 from .common import DBoardPreferredDapiMode, LastReset, ValueRange, DBoardException, SystemModeConfig
 from .workspace import WorkspacesContainer, StandbyWorkspace, Workspace, BaseWorkspace
-from .analoginput import PressureSensor, Analog0Sensor, Analog1Sensor, PowerSupply, ReferenceSensor
+from .analoginput import PressureSensor, VoltageSensor, PercentSensor
 from .debug import DebugValue
+from dapi2.derror import DApiComAbortedError
 
 
 
 class DacChannel(IntEnum):
     DAC0 = 0
     DAC1 = 1
 
 
 class DacSignal(IntEnum):
     DPA_VIRT = 0
     DPA_REAL = 1
     PHI = 2
     DRAG = 3
     PWM_OPENING = 4
-    
+
 
 class WorkspaceChangedSignal(DSignal):
-    
+
     def emit(self, workspace):
         for callback in self.callbacks:
-            callback(workspace)    
+            callback(workspace)
 
 
 class ConnectionChangedSignal(DSignal):
-    
+
     def emit(self, state, level):
         for callback in self.callbacks:
-            callback(state, level)    
+            callback(state, level)
 
 class BaseDBoard(object):
     '''Base class for Dassym electronic boards.
-    
+
     :param DApi2 _dapi: The DAPI2 object.
     :param DBoardPreferredDapiMode dmode: Specifies the preferred DAPI2 operating mode (default: `REGISTER`)
-    
+
     '''
-    
+
     number = '--'
     '''Board type number (str)'''
-    
+
     ext = None
     '''Board type extention (str)'''
-     
+
     wait_after_reprogramming = 8.0 #[s]
     '''Timeout after programming to reconnect to the board expressed in second.'''
-    
+
     wait_after_reboot = 2.0 #[s]
     '''Timeout after reboot to reconnect to the board expressed in second.'''
-    
+
     DAC_SIGNAL = DacSignal
-    
+
     @classmethod
     def getBoardClasses(cls):
         '''Returns all known board classes
-    
+
         :return: All known board classes
-        :rtype: dict 
+        :rtype: dict
         '''
         return dict([(c.number,c) for c in cls.__subclasses__()])
-    
+
     @classmethod
     def getSubclasses(cls):
         '''Returns all sub-classes recursively
-        
+
         Returns:
             set: All sub-classes of this class.
         '''
-        return set(cls.__subclasses__()).union( [s for c in cls.__subclasses__() for s in c.getSubclasses()])  
-    
+        return set(cls.__subclasses__()).union( [s for c in cls.__subclasses__() for s in c.getSubclasses()])
+
     @classmethod
     def getName(cls):
         '''Returns the board type name
         :return: The board type name
         :rtype: str
         '''
         if cls.ext is not None:
@@ -119,116 +120,117 @@
         self._workspace = None
         self._workspaces = WorkspacesContainer(self)
         self._analog_inputs = {}
         self.speed_range = ValueRange(0,40000)
         self.torque_range = ValueRange(0,7000)
         self.powersupply_range = ValueRange(30,36)
         self.analog_input_range = (ValueRange(0,10000),ValueRange(0,10000))
-        
+
         self._workspace_changed = WorkspaceChangedSignal()
         self._connection_changed = ConnectionChangedSignal()
-        self._dapi.dcom.connectionChanged.connect(self.onDComConnectionChanged)
-        
+        if self._dapi.dcom:
+            self._dapi.dcom.connectionChanged.connect(self.onDComConnectionChanged)
+
     def __str__(self):
         return self.getName()
-        
+
     def initialize(self):
         '''Initialize the board object.
-        
+
         The connection with the hardware must be established.
         '''
         self.log.info('Board initialization ...')
         self.log.debug(' - load all undefined registers')
-        
+
         self.refreshAll(undefined_only=True)
         self._workspaces.clear()
         self._workspace = StandbyWorkspace(self)
         self._workspaces.append(self._workspace)
-        
+
         for i in range(self.regs.pcr.size):
             ws_par = i+1
             ws_pcr = self.regs.pcr[i]
             if ws_pcr.value != 0:
                 self.log.debug(' - init workspace #{}'.format(ws_par))
                 ws = Workspace(self, 'Workspace #'+str(ws_par) , ws_par, ws_pcr)
                 self._workspaces.append(ws)
                 if self.regs.par.value == ws_par:
                     self.log.debug('- init : Workspace #{} is active'.format(ws_par))
                     self._workspace = ws
         if len(self._workspaces) == 1:
             if self._dapi.dev_mode:
                 self.log.warning('No workspace found!')
             else:
-                raise DBoardException(self,'initialize', 'No workspace found!')  
-            
-        
+                raise DBoardException(self,'initialize', 'No workspace found!')
+
+
         self._connection_changed.emit(self.dcom.isOpen(), self.getAccessLevel())
         self._workspace_changed.emit(self._workspace)
 
         self.regs.par.changed.connect(self.onPARChanged)
         self.regs.scsr.changed.connect(self.onSCSRChanged)
-            
+
         self.log.debug('Board initialization is done.')
-                    
-        
+
+
     def setReg(self, reg, value, synchronous=True):
         '''Sets a value to a register.
-        
+
         The modification can be synchronous or not, depending on the `synchronous` parameter.
         If the modification is asynchronous, it is not directly written to the registers of the card.
         The writing will be done the next time the :meth:`DApi2.syncRegs <dapi2.dapi2.DApi2.syncRegs>` method is called.
         If it is synchronous, the modification is directly written in the card registers.
-        
+
         :param reg: The register to be modified
         :type reg: Register, str
         :param int value: The new value
         :param bool synchronous: Specifies whether the modification is synchronous (default) or not.
         '''
         if not isinstance(reg, Register):
             reg = self._dapi.regs.getRegister(reg)
         reg.set(value)
         if synchronous:
             self._dapi.syncRegs()
             #self._dapi.writeReg(reg)
-   
-            
+
+
     def setBit(self, bit, value=1, synchronous=True):
         '''Sets a value to a register's bit.
-        
+
         .. seealso::
             :meth:`setReg`
-        
+
         :param bit: The register's bit to be modified
         :type bit: RegBit, str
         :param int value: The new value (0 or 1). Default 1.
         :param bool synchronous: Specifies whether the modification is synchronous (default) or not.
         '''
         if not isinstance(bit, RegBit):
             bit = self._dapi.getBit(bit)
         if bit.parent.isUndefined() and not self._dapi.dev_mode:
             self._dapi.readReg(bit.parent)
-        bit.set(value) 
+        bit.set(value)
         if synchronous:
             self._dapi.syncRegs()
-            
+
     def clearBit(self, bit, synchronous=True):
         '''Clear the registers's bit.
-        
+
         .. seealso::
             :meth:`setReg`
 
         :param bit: The register's bit to be modified
         :type bit: RegBit, str
         :param bool synchronous: Specifies whether the modification is synchronous (default) or not.
         '''
         self.setBit(bit, 0, synchronous)
-        
+
     def toggleBit(self, bit, synchronous=True):
         ''' Toggles the registers's bit.
-        
+
         .. seealso::
             :meth:`setReg`
 
         :param bit: The register's bit to be modified
         :type bit: RegBit, str
         :param bool synchronous: Specifies whether the modification is synchronous (default) or not.
         '''
@@ -236,31 +238,31 @@
             bit = self._dapi.getBit(bit)
         bit.parent.alter( bit.toggle() )
         if synchronous:
             self._dapi.syncRegs()
 
     def setRegs(self, regs, values, synchronous=True):
         '''Sets values to a list of registers.
-        
+
         :param list regs: The registers list to be modified (list of :class:`~dapi2.dmsg.message.BaseMessage`)
         :param int value: The new value
         :param bool synchronous: Specifies whether the modification is synchronous (default) or not. See :meth:`BaseDBoard.setReg` .
-        
+
         '''
         for i, reg in enumerate(regs):
             if not isinstance(reg, Register):
                 reg = self._dapi.regs.getRegister(reg)
             reg.alter(values[i])
         if not synchronous:
             self._dapi.syncRegs()
             #self._dapi.writeRegs(regs)
-            
+
     def setRegisters(self, synchronous=False, **regvalues):
         '''Sets values to a list of registers.
-        
+
         :param bool synchronous: Specifies whether the modification is synchronous or not (Default : not = asyncrhonous). See :meth:`BaseDBoard.setReg`
         :param regvalues: Several arguments named according to the name of the registers to be modified.
         '''
         for reg, value in regvalues.items():
             if not isinstance(reg, Register):
                 reg = self._dapi.regs.getRegister(reg)
             self.setReg(reg, value, synchronous=False)
@@ -268,133 +270,136 @@
             self._dapi.syncRegs()
 
     def getRegisters(self, *registers, refresh=False, undefined_only=False):
         '''Gets values of a list of registers.
         Args:
             regvalues: Several arguments named according to the name of the registers to be modified.
             refresh (bool): True, force read registers form board, else read only undefined registers.
-            undefined_only (bool): If True, refresh on only the undefined registers 
+            undefined_only (bool): If True, refresh on only the undefined registers
         '''
         regs = []
         for reg in registers:
-            if not isinstance(reg, Register):
+            if isinstance(reg, str):
                 reg = self._dapi.regs(reg)
-            
+
             if isinstance(reg, RegGroup):
-                regs.extend(reg.regs) 
-            else:
+                regs.extend(reg.regs)
+            elif isinstance(reg, Register):
                 regs.append(reg)
         if refresh:
             if undefined_only:
                 uregs = [r for r in regs if r.isUndefined()]
                 self._dapi.readRegs(*uregs)
-            else: 
+            else:
                 self._dapi.readRegs(*regs)
         else:
             uregs = [r for r in regs if r.isUndefined()]
             self._dapi.readRegs(*uregs)
-            
+
         return regs
-        
 
-        
+
+
     def connect(self, level=DApiAccessLevel.USER, passwd=0x0000):
         '''Connect the *MASTER* to the board.
-        
+
         :param DBoardAccessLevel level: DAPI2 Access level
         :param int passwd: *password* to connect to the board
-        
+
         '''
         if self._dapi.regs.scsr.bits.access.value != DApiAccessLevel.NO.value: #@UndefinedVariable
             self._dapi.cmd.disconnect()
         if level != DApiAccessLevel.NO:
-            self._dapi.cmd.connect(level,passwd) 
+            self._dapi.cmd.connect(level,passwd)
         try:
             self._dapi.regs.scsr.bits.access.set(level.value)
         except DRegUndefinedError:
             self._dapi.readReg(self._dapi.regs.scsr)
             self._dapi.regs.scsr.bits.access.set(level.value)
-        
-        
+
+
     def setWorkspace(self, workspace):
         '''Sets a new workspace.
-        
+
         :param Workspace workspace: The new workspace to activate.
-        :type workspace: BaseWorkspace, int 
-        ''' 
-        
+        :type workspace: BaseWorkspace, int
+        '''
+
         if not isinstance(workspace, BaseWorkspace):
             workspace = self.workspaces.getByPAR(workspace)
         if workspace is None:
             raise ValueError('Undefined workspace!')
-        if self.dmode == DBoardPreferredDapiMode.COMMAND:
-            if workspace.standby:
-                self._dapi.cmd.standby()
+        try:
+            if self.dmode == DBoardPreferredDapiMode.COMMAND:
+                if workspace.standby:
+                    self._dapi.cmd.standby()
+                else:
+                    self._dapi.cmd.peripheralActivate(workspace.par)
+                self.regs.par.internalSet(workspace.par)
             else:
-                self._dapi.cmd.peripheralActivate(workspace.par)
-            self.regs.par.value = workspace.par
-        else:
-            self.setReg(self._dapi.regs.par, workspace.par)
-         
+                self.setReg(self._dapi.regs.par, workspace.par)
+        except DApiComAbortedError as e:
+            self.regs.par.internalSet(workspace.par)
+            raise e
         #self._workspace = workspace
-            
+
     def getWorkspace(self, refresh=False):
         '''Returns the current workspace.
-        
+
         :param bool refresh: specifies whether to update the in-memory register with the one on the board.
-        ''' 
+        '''
         if refresh:
             self._dapi.readReg(self.regs.par)
         if self._workspace is None:
             self.onPARChanged(self.regs.par, self.regs.par.value, self.regs.par.value)
         return self._workspace
-            
+
     def isOnStandby(self):
         '''Check if the board is on standby state.
-        
+
         :return: True, if the board is on standby state ; False otherwise.
         :rtype: bool
-        ''' 
+        '''
         if self._workspace is None:
             self.getWorkspace(refresh=True)
-        return self._workspace.standby 
-    
-    
+        return self._workspace.standby
+
+
     def hasBlueLight(self):
         '''Check if the board has the blue light feature.
-        
+
         :return: True, if the board has the blue light feature ; False otherwise.
         :rtype: bool
-        ''' 
-        try: 
+        '''
+        try:
             #self.log.debug('ssr2='+self.regs.ssr2.toString(depth=2))
             return self.regs.ssr2.bits.alt_lmp.value == 1
         except DRegUndefinedError:
             self.getRegisters('ssr2')
             return self.regs.ssr2.bits.alt_lmp.value == 1
-        
+
     def getError(self, refresh=False):
         '''Returns the board error code.
-      
+
         :param bool refresh: Specifies whether to update the in-memory register with the one on the board.
-        
-        :return: Zero, if the boatrd is'nt in error or warning state : Non-zero, otherwise 
+
+        :return: Zero, if the boatrd is'nt in error or warning state : Non-zero, otherwise
         :rtype: int
-        ''' 
-        
+        '''
+
         if refresh:
             self._dapi.readReg(self.regs.wer)
         return self.regs.wer.value
-        
+
     def getMicrocontrollerID(self):
-        
+
         ret = bytearray(self._dapi.cmd.getMcId(0))
         ret.extend(self._dapi.cmd.getMcId(1))
         return ret
-    
+
     def getLastReset(self, refresh=False):
         if refresh:
             self._dapi.readReg(self.regs.scsr)
         return LastReset(self.regs.scsr.bits.reset.value)
 
     def getPeripheralWatchdog(self, refresh=False):
         if refresh:
@@ -402,226 +407,226 @@
         return self.regs.scsr.bits.pwd.value != 0
 
     def getIndependentWatchdog(self, refresh=False):
         if refresh:
             self._dapi.readReg(self.regs.scsr)
         return self.regs.scsr.bits.iwd.value != 0
 
-    
+
     def getSystemModeConfiguration(self, refresh=False):
         if refresh:
             self._dapi.readReg(self.regs.smr)
         try:
             return SystemModeConfig(self.regs.smr.value)
         except DRegUndefinedError:
             self._dapi.readReg(self.regs.smr)
             return SystemModeConfig(self.regs.smr.value)
-        
+
     def setSystemModeConfiguration(self, flags):
         self.setReg(self.regs.smr, flags.value)
-    
+
     def getAccessLevel(self, refresh=False):
         if refresh or self.regs.scsr.isUndefined():
             self._dapi.readReg(self.regs.scsr)
         return DApiAccessLevel(self.regs.scsr.bits.access.value)
-    
+
     def getAdditionalBoard(self, refresh=False):
         if refresh or self.regs.scsr.isUndefined():
             self._dapi.readReg(self.regs.scsr)
         return DApiAdditionalBoard(self.regs.scsr.bits.ab.value)
-    
+
     def getPowerSupply(self, refresh=False):
         if refresh:
             self._dapi.readReg(self.regs.psvr)
         return self.regs.psvr.value / 1000
-    
+
     def getAnalogInput(self, index, refresh=False):
         reg = self.regs('an{0:d}r'.format(index))
-        if refresh: 
+        if refresh:
             self._dapi.readReg(reg)
         return reg.value
-        
+
     def getSpeedReference(self, refresh=False):
-        if refresh: 
+        if refresh:
             self._dapi.readReg(self.regs.ref)
-        return self.regs.ref.value        
+        return self.regs.ref.value
 
     def getPressure(self, refresh=False):
-        if refresh: 
+        if refresh:
             self._dapi.readReg(self.regs.prcr)
-        return self.regs.prcr.value        
-            
+        return self.regs.prcr.value
+
     def getFirmwareVersion(self):
         try:
             return wordToVersion(self.regs.svr.value)
         except DRegUndefinedError:
             self.getRegisters('svr')
             return wordToVersion(self.regs.svr.value)
-        
+
     def getFirmwareDate(self):
         try:
             return wordToDate(self.regs.fbdr.value)
         except DRegUndefinedError:
             self.getRegisters('fbdr')
-            return wordToDate(self.regs.fbdr.value)        
-        
-    
+            return wordToDate(self.regs.fbdr.value)
+
+
     def getFirmwareTag(self):
         try:
             return self.regs.sctr.value
         except DRegUndefinedError:
             self.getRegisters('sctr')
             return self.regs.sctr.value
-     
+
     def disconnect(self):
         '''Disconnect the *MASTER* from the board.'''
         self._dapi.cmd.disconnect()
         try:
             self._dapi.regs.scsr.bits.access.set(DApiAccessLevel.NO.value)  # @UndefinedVariable
         except DRegUndefinedError:
             self._dapi.readReg(self._dapi.regs.scsr)
             self._dapi.regs.scsr.bits.access.set(DApiAccessLevel.NO.value)  # @UndefinedVariable
-        
-        
+
+
     def reboot(self):
         '''Reboots the board.'''
         self._dapi.cmd.reboot()
-        
+
     def motorStart(self, speed=None ):
         '''Starts the motor and optionally change the speed set point.
-        
-        :param int speed: The new speed set point. Default no change. 
-        ''' 
+
+        :param int speed: The new speed set point. Default no change.
+        '''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.motorStart(speed if speed is not None else 0)
-        else: 
+        else:
             if speed is not None:
                 self.setReg(self._dapi.regs.scr, speed, synchronous=False)
             self.setBit(self._dapi.regs.smr.start)
-            
+
     def motorStop(self):
-        '''Stops the motor.''' 
+        '''Stops the motor.'''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.motorStop()
-        else: 
+        else:
             self.clearBit(self._dapi.regs.smr.start)
-        
+
     def motorReverse(self, rev=None):
         '''Reverses the direction of rotation of the motor.'''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.motorReverse()
-        else: 
+        else:
             self.toggleBit(self._dapi.regs.smr.reverse)
-             
-            
+
+
     def motorForward(self):
         '''Sets forward direction (clockwise).'''
         self.clearBit(self._dapi.regs.smr.reverse)
 
     def motorBackward(self):
         '''Sets backward direction (counter clockwise).'''
         self.setBit(self._dapi.regs.smr.reverse)
-        
+
     def memoryStore(self, num):
         '''Stores the current set points into memory..
-        
+
         :param int num: The memory slot number.
         '''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.memoryStore(num)
-    
+
     def memoryRecall(self, num):
         '''Recalls the set points from memory..
-        
+
         :param int num: The memory slot number.
         '''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.memoryRecall(num)
-        #self.getRegisters('setpoints')    
-               
+        #self.getRegisters('setpoints')
+
     def setMotorSpeed(self, speed):
         '''Sets the motor speed
-        
+
         :param int speed: The new motor speed [rpm].
         '''
         self.setReg(self._dapi.regs.scr, speed)
-        
+
     def motorIncSpeed(self, inc):
         '''Increments the motor speed.
-        
+
         :param int inc: The increment value.
         '''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.motorIncSpeed(inc)
         else:
             if self.motorSpeed()+inc > self.speed_range.upper:
                 inc = self.speed_range.upper - self.motorSpeed()
             self.setMotorSpeed(self.motorSpeed()+inc)
 
     def motorDecSpeed(self, inc):
         '''Decrements the motor speed.
-        
+
         :param int inc: The decrement value.
         '''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.motorDecSpeed(inc)
         else:
             if self.motorSpeed()-inc < self.speed_range.lower:
-                inc = self.motorSpeed() 
+                inc = self.motorSpeed()
             self.setMotorSpeed(self.motorSpeed()-inc)
 
-    
+
     def motorSpeed(self):
         '''Returns the motor speed set point'''
         try:
             return self._dapi.regs.scr.value
         except DRegUndefinedError:
             self.getRegisters('scr')
             return self._dapi.regs.scr.value
 
-        
+
     def motorRealSpeed(self):
         '''Returns the real motor speed'''
         try:
             return self._dapi.regs.msr.value
         except DRegUndefinedError:
             self.getRegisters('msr')
             return self._dapi.regs.msr.value
-        
+
     def setMotorCurrent(self, torque):
         '''Sets the maximum motor current
-        
+
         :param int torque: The new maximum motor current [mA].
         '''
-        self.setReg(self._dapi.regs.ccr, torque) 
-        
+        self.setReg(self._dapi.regs.ccr, torque)
+
     def motorCurrent(self):
         '''Returns the maximum motor current set point'''
         try:
             return self._dapi.regs.ccr.valued
         except DRegUndefinedError:
             self.getRegisters('ccr')
             return self._dapi.regs.ccr.value
-        
+
     def motorRealCurrent(self):
         '''Returns the real motor current'''
         try:
             return self._dapi.regs.a256dcr.value
         except DRegUndefinedError:
             self.getRegisters('a256dcr')
             return self._dapi.regs.a256dcr.value
-    
+
     def setGearRatio(self, numerator, denominator):
         '''Sets the hand piece gear ratio.
-        
-        :param int numerator: The numerator (multiplier). 
+
+        :param int numerator: The numerator (multiplier).
         :param int denominator: The denominator (divider).
         '''
         self.setRegs(('grnr','grdr'), (numerator, denominator))
-        
+
     def isLightEnabled(self):
         '''Checks if light is enabled.'''
         try:
             return self._dapi.regs.smr.bits.light.value
         except DRegUndefinedError:
             self.getRegisters('smr')
             return self._dapi.regs.smr.bits.light.value
@@ -629,218 +634,221 @@
     def isLightAlternate(self):
         '''Checks if the alternate light is activated.'''
         try:
             return self._dapi.regs.alr.value != 0
         except DRegUndefinedError:
             self.getRegisters('alr')
             return self._dapi.regs.alr.value != 0
-        
+
     def isMotorRunning(self):
         '''Checks if motor is running.'''
         try:
             return self._dapi.regs.ssr1.bits.rotation.value
         except DRegUndefinedError:
             self.getRegisters('ssr1')
             return self._dapi.regs.ssr1.bits.rotation.value
-    
+
     def isMotorStarted(self):
         '''Checks if motor is started.'''
-        try: 
+        try:
             return self.regs.smr.bits.start.value == 1
         except DRegUndefinedError:
             self.getRegisters('smr')
             return self.regs.smr.bits.start.value == 1
-    
+
 
     def isMotorReverse(self):
         '''Checks if CCW direction is selected.'''
         try:
             return self._dapi.regs.smr.bits.reverse.value
         except DRegUndefinedError:
             self.getRegisters('smr')
             return self._dapi.regs.smr.bits.reverse.value
 
-    
+
     def lightOn(self, on=True):
         '''Enables the light.'''
         if not on:
             self.lightOff()
-        else: 
+        else:
             if self.dmode == DBoardPreferredDapiMode.COMMAND:
                 self._dapi.cmd.lightOn()
-            else: 
+            else:
                 self.setBit(self._dapi.regs.smr.bits.light)
 
     def lightOff(self):
         '''Disables the light.'''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.lightOff()
-        else: 
+        else:
             self.clearBit(self._dapi.regs.smr.bits.light)
-            
+
     def lightAuto(self, auto):
         '''Sets the light mode.
-        
-        :param bool auto: True, sets the automatic mode, False, sets the direct (manual) mode. 
+
+        :param bool auto: True, sets the automatic mode, False, sets the direct (manual) mode.
         '''
         self.setBit(self._dapi.regs.smr.bits.lightauto, int(auto))
-    
+
 
     def lightIntensity(self, intensity):
         '''Sets the light intensity.
-        
-        :param int intensity: The light intensity in mA'''  
+
+        :param int intensity: The light intensity in mA'''
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.lightIntensity(intensity)
-        else: 
+        else:
             self.setReg(self._dapi.regs.lir, intensity)
 
     def lightAlternate(self, alternate=True):
         '''chosen between normal (white) or alternative (UV) light
-        
+
         :param bool alternate: True = Alternate ; False = Normal
-        ''' 
+        '''
         #if self.dmode == DBoardPreferredDapiMode.COMMAND:
         #    self._dapi.cmd.lightAlternate(0x100 * int(alternate))
-        #else: 
+        #else:
         self.setReg(self._dapi.regs.alr, 0x100 * int(alternate))
 
-            
+
     def calibrate(self, part, phase):
         '''Starts calibration procedure
-        
+
         :param int part: Index of part (sensor) to calibrate.
-        :param int phase: Pahse number of calibration.   
+        :param int phase: Pahse number of calibration.
         '''
         self._dapi.cmd.calibrate(part, phase)
-        
+
     def setFactoryData(self, sn, fd, hv=None):
         '''Sets the factory data.
-        
+
         :param int sn: Serial number.
         :param Date fd: Factory date.
         :param tuple hv: 2-tuple of integer for major and minor version number.
-        ''' 
-        
+        '''
+
         if hv is None:
-            hv = wordToVersion(self.regs.hvr.value) 
-        
+            hv = wordToVersion(self.regs.hvr.value)
+
         self.log.info('Set factory data. SN:{0:04d}, FD:{1:s}, HV:{2:d}.{3:02d}'.format(sn, fd.isoformat(), hv[0], hv[1]) )
-        
+
         if self.dmode == DBoardPreferredDapiMode.COMMAND:
             self._dapi.cmd.factSetSysinfo(sn, fd, hv)
-        else: 
-            self.setRegisters(snr=sn, fdr=dateToWord(fd), hvr = versionToWord(*hv), synchronous=True)        
-               
+        else:
+            self.setRegisters(snr=sn, fdr=dateToWord(fd), hvr = versionToWord(*hv), synchronous=True)
+
     def getFactoryData(self, read=True):
         '''Returns the factory data.
-        
-        :return: A 3-tuple containing the serial number (int), the factory date (date) and the hardware version (2-tuple of int). 
+
+        :return: A 3-tuple containing the serial number (int), the factory date (date) and the hardware version (2-tuple of int).
         '''
         if read:
             self.getRegisters('snr','fdr','hvr', refresh=True)
-        
+
         return (self.regs.snr.value, wordToDate(self.regs.fdr.value), wordToVersion(self.regs.hvr.value))
-        
-        
+
+    def refreshHeader(self, undefined_only=False):
+        self.getRegisters('header', refresh=True, undefined_only=undefined_only)
+
     def refreshAll(self, undefined_only=False):
+        self.refreshHeader(undefined_only=undefined_only)
         self.refreshState(undefined_only=undefined_only)
         self.refreshSetpoints(undefined_only=undefined_only)
         self.refreshDebug(undefined_only=undefined_only)
         self.refreshSystem(undefined_only=undefined_only)
-        
+
     def refreshState(self, part=None, undefined_only=False):
         #self.log.debug('refreshState')
-        self.getRegisters('header', refresh=True, undefined_only=undefined_only)
+        #self.getRegisters('header', refresh=True, undefined_only=undefined_only)
         if part is None:
             self.getRegisters('state', refresh=True, undefined_only=undefined_only)
         else:
             self.getRegisters('ssr1', 'ssr2', 'msr', 'a256dcr', refresh=True, undefined_only=undefined_only)
             if self.regs.ssr1.wanr_err != 0 and part != 8:
                 self.getRegisters('wer', refresh=True, undefined_only=undefined_only)
             if part > 0:
-                addr = self.regs.state.addr+(part*4) 
+                addr = self.regs.state.addr+(part*4)
                 self.getRegisters(self.regs[addr:addr+4], refresh=True, undefined_only=undefined_only)
-                
+
 
     def refreshSetpoints(self, undefined_only=False):
         #self.log.debug('refreshSetpoints')
         self.getRegisters('setpoints', refresh=True, undefined_only=undefined_only)
-        
+
     def refreshDebug(self, undefined_only=False):
         #self.log.debug('refreshDebug')
         self.getRegisters('debug', refresh=True, undefined_only=undefined_only)
 
     def refreshAnalogInputs(self, undefined_only=False):
         #self.log.debug('refreshDebug')
         self.getRegisters('prcr', 'elcr', 'an0r', 'an1r', 'psvr', 'esvr',refresh=True, undefined_only=undefined_only)
 
     def refreshSystem(self, undefined_only=False):
         #self.log.debug('refreshSystem')
         self.getRegisters('system', refresh=True, undefined_only=undefined_only)
 
-        
+
     def eepromReset(self):
         self._dapi.cmd.factEerpomReset()
-        
+
     def flashBinaryFirm(self, stream, callback=None):
-        
+
         def _readByte(x):
             c = stream.read(1)
             if c == '':
                 return 0
             else:
                 return ord(c)
         self.log.info('Firmware programming has started....')
         #with open( firm, 'rb' ) as f:
         stream.seek(0, os.SEEK_END)
         size = stream.tell()
         self._dapi.cmd.flashBegin(size)
         stream.seek(0)
         i = 0
-        
+
         while i < size:
             self._dapi.cmd.flashData([_readByte(x) for x in range(CommandMessage.MAX_DATA_SIZE)])
             i+=CommandMessage.MAX_DATA_SIZE
             #self.log.debug('Programming block {0} / {1}'.format(i//CommandMessage.MAX_DATA_SIZE,size//CommandMessage.MAX_DATA_SIZE))
             if callback is not None:
                 callback(i, size)
-                    
+
 
         self._dapi.cmd.flashEnd()
         self.log.info('Firmware programming is complete!')
-        
+
     def onDComConnectionChanged(self, connected):
         self.log.debug(f'onDComConnectionChanged : {connected}')
         self._connection_changed.emit(connected, self.getAccessLevel())
-            
+
     def onPARChanged(self, reg, old, value):
         self.log.debug('onPARChanged 0x{0:04x} => 0x{1:04x}'.format(old,value))
         self._workspace = self.workspaces.getByPAR(value)
         self.log.info(f'{self._workspace!s} is activated.'.format(old,value))
         self.getRegisters('ctr', refresh=True)
         self._workspace_changed.emit(self._workspace)
-        
+
     def onSCSRChanged(self, reg, old, value):
         self.log.debug('onSCSRChanged 0x{0:04x} => 0x{1:04x}'.format(old,value))
-        
+
         if (old & DAPI_ACCESS_LEVEL_MASK) != (value & DAPI_ACCESS_LEVEL_MASK):
             self._connection_changed.emit(self._dapi.dcom.isOpen(), self.getAccessLevel())
-        
+
     def setDacSignal(self, dac, signal):
         '''Sets the signal that the DAC should generate.
-        
-        :param dac DacChannel: The DAC channel to change 
-        :param signal DacSignal: The signal to set on the DAC channel 
+
+        :param dac DacChannel: The DAC channel to change
+        :param signal DacSignal: The signal to set on the DAC channel
         '''
-        assert isinstance(dac, DacChannel) 
+        assert isinstance(dac, DacChannel)
         assert isinstance(signal, DacSignal)
-        self.setReg(self._dapi.regs.dacsr[dac.value], signal.value, synchronous=True)        
-        
-    
+        self.setReg(self._dapi.regs.dacsr[dac.value], signal.value, synchronous=True)
+
+
     @property
     def dapi(self):
         return self._dapi
     @property
     def dcom(self):
         return self._dapi.dcom
     @property
@@ -859,51 +867,44 @@
     def sn(self):
         return self.regs.snr.value
     @property
     def analogInputs(self):
         return self._analog_inputs.values()
     @property
     def workspaceChanged(self):
-        return self._workspace_changed    
+        return self._workspace_changed
     @property
     def connectionChanged(self):
-        return self._connection_changed    
-    
-    
-    
+        return self._connection_changed
+
+
+
 class DBoard(BaseDBoard):
     '''Generic class board.
-    
+
     This class is used when the type of card could not be determined.
-    
-    
+
+
     .. inheritance-diagram:: DBoard
         :parts: 1
-    
-    ''' 
+
+    '''
     number = '00'
     '''Board type number'''
-    
+
+    REG_GROUPS = ('header', 'ppa', 'controller', 'state', 'setpoints', 'debug', 'system')
+
     DAC_SIGNAL = DacSignal
-    
+
     def __init__(self, dapi, dmode=DBoardPreferredDapiMode.REGISTER):
         BaseDBoard.__init__(self, dapi, dmode=dmode)
-        self._analog_inputs = dict( 
-                ((sensor.name, sensor) for sensor in (
-                    PressureSensor(self),
-                    ReferenceSensor(self),
-                    Analog0Sensor(self),
-                    Analog1Sensor(self), 
-                    PowerSupply(self),)
-                    )
-            )
-        self._debug_values = [ DebugValue(self, self.regs.dmr[i]) for i in range(self.regs.dmr.size) ] 
+
+        self._debug_values = [ DebugValue(self, self.regs.dmr[i]) for i in range(self.regs.dmr.size) ]
         self._debug_setting_values = [ DebugValue(self, self.regs.dsr[i]) for i in range(self.regs.dsr.size) ]
-        
+
     @property
     def debugValues(self):
         return self._debug_values
     @property
     def debugSettingValues(self):
-        return self._debug_setting_values    
-    
-    
+        return self._debug_setting_values
+
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/common.py` & `PyDapi2-0.6.2/src/dapi2/dboard/common.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/debug.py` & `PyDapi2-0.6.2/src/dapi2/dboard/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,52 +7,56 @@
 from .common import BaseBoardItem
 from dapi2.dreg.base import DRegAccess
 
 
 
 
 class DebugValue(BaseBoardItem):
-    
+
     def __init__(self, board, reg, index=None, size=16):
         BaseBoardItem.__init__(self, board, name=reg.name)
         self._reg = reg
         self._index = index if index != None else reg.index
         self._size = size
         self.values = []
         self._callback_list = []
         self._reg.changed.connect(self.onRegisterChange)
         if self._reg.isDefined():
             self.onRegisterChange(self._reg, self._reg.value, self._reg.value)
-    
+
     def __getitem__(self, index):
         return self.values[index]
-    
+
     def __len__(self):
         return len(self.values)
-    
+
     def setSize(self, size):
         self._size = size
         if self._size < len(self):
             self.values = self.values[:self._size]
-   
+
     def connect(self, callback):
         if all(x != callback for x in self._callback_list):
-            self._callback_list.append(callback)            
+            self._callback_list.append(callback)
 
     def disconnect(self, callback):
-        self._callback_list.remove(callback) 
+        self._callback_list.remove(callback)
 
     def onRegisterChange(self, reg, old_value=None, new_value=None):
         self.board.log.debug('DebugValue.onRegisterChange')
         if new_value is None:
             new_value = reg.value
         self.values = ([new_value]+self.values)[:self._size]
-        
+
         for func in self._callback_list:
-            func(self)      
+            func(self)
+
+    def setValue(self, value):
+        self._reg.internalSet(value, True)
+        self.board.dapi.syncRegs()
 
     @property
     def reg(self):
         return self._reg
 
     @property
     def writable(self):
@@ -65,10 +69,14 @@
 
     @property
     def value(self):
         try:
             return self.values[0]
         except IndexError:
             return None
-        
-    
-    
+
+    @value.setter
+    def value(self, value):
+        self.setValue(value)
+
+
+
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/factory.py` & `PyDapi2-0.6.2/src/dapi2/dboard/factory.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/generic.py` & `PyDapi2-0.6.2/src/dapi2/dboard/generic.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dboard/workspace.py` & `PyDapi2-0.6.2/src/dapi2/dboard/workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 '''
 Created on 15 mars 2021
 
 @author: fv
 '''
 from .common import BaseBoardItem
+from ..dapi2 import DApiControllerType, DApiPeripheralType
+
 
 
-        
 class Memory(object):
     '''Memory for recording setpoints
-    
-    :param container 
+
+    :param container
     :param index int: memory index number
     :param size int: size of memory. Number of registers to store.
     '''
-    
+
     SIZE = 16
     PAGE_SIZE = 4
     NB_PAGES = SIZE // PAGE_SIZE
     SMR_MASK = 0x0500 # In the "SMR" register, only bits #8 (reverse) and #10 (light) are relevant
-    
+
     def __init__(self, container, index):
         self._container = container
         self._index = index
         self._values = []
-        
+
     def read(self):
         self._values = []
-        for p in range(self.SIZE // self.PAGE_SIZE): 
+        for p in range(self.SIZE // self.PAGE_SIZE):
             self._values.extend(self.board.dapi.cmd.memoryRead(self.workspace.number, self._index, p))
-        
-            
+
+
     def isCurrent(self):
         try:
             if self._values[0] & self.SMR_MASK != self.board.regs.setpoints.values[0] & self.SMR_MASK:
-                return False  
+                return False
             return self._values[1:] == self.board.regs.setpoints.values[1:]
         except IndexError:
             return False
-        
+
     def isDefined(self):
-        return len(self._values)==self.SIZE 
-    
+        return len(self._values)==self.SIZE
+
     @property
     def board(self):
         return self._container.board
-    
+
     @property
     def workspace(self):
         return self._container.workspace
-    
+
     @property
     def index(self):
         return self._index
 
-    
+
 
 class Memories(object):
     '''Container to maintain the set points memories.
-    
+
     :param workspace BaseWorkspace: the container's proprietary workspace
-    ''' 
+    '''
     def __init__(self, workspace):
         self._workspace = workspace
         self._slots = []
         for i in range(self._workspace.NB_USER_MEMORY_SLOTS):
             self._slots.append(Memory(self, i))
-            
+
     def __getitem__(self, index):
         return self._slots[index]
-    
+
     def __len__(self):
         return len(self._slots)
-    
+
     def __iter__(self):
         for mem in self._slots:
             yield mem
 
     def readAll(self):
         for m in self:
             if not m.isDefined():
@@ -85,194 +86,218 @@
     @property
     def board(self):
         return self._workspace.board
 
     @property
     def workspace(self):
         return self._workspace
-        
+
 
 class BaseWorkspace(BaseBoardItem):
     '''Base class for board's Workspace.
-    
+
     :param BaseBoard board: The board.
     :param str name: The workspace name.
     :param int number: The workspace number = PAR value used to activate the workspace
-    :param int pcr: The configuartion code  
-    
+    :param int pcr: The configuartion code
+
     .. inheritance-diagram:: BaseWorkspace
         :parts: 1
-    
-    
+
+
     '''
-        
+
     NB_USER_MEMORY_SLOTS = 8
     '''Number of user's memory slots.'''
-    
+
     def __init__(self, board, name=None, number=None, pcr=None):
         super().__init__(board, name)
         self._number = number
         self._pcr = pcr
-        self._memories = Memories(self)        
+        self._memories = Memories(self)
 
     def __str__(self):
         return self.name
-    
+
     def isFunctional(self):
         '''Check if workspace is functional.
-        
+
         :return: True, if workspace is functional ; False otherwise.
         :rtype bool
         '''
         if self.board.regs.ctr.isUndefined():
             self.board.getRegisters('ctr')
-        return self.board.regs.ctr.value != 0x0000       
+        return self.board.regs.ctr.value != 0x0000
 
     @property
     def standby(self):
         return False
     @property
     def active(self):
-        return self is self._board.getWorkspace()      
+        return self is self._board.getWorkspace()
     @property
     def number(self):
         return self._number
     @property
     def par(self):
         return self._number
     @property
     def pcr(self):
         return self._pcr
     @property
     def memories(self):
         return self._memories
+    @property
+    def controllerType(self):
+        if self.board.regs.ctr.isUndefined():
+            self.board.getRegisters('ctr')
+        try:
+            return DApiControllerType(self.board.regs.ctr.value)
+        except KeyError:
+            return DApiControllerType.NO
+    @property
+    def peripheralType(self):
+        if self.board.regs.ptr.isUndefined():
+            self.board.getRegisters('ptr')
+        try:
+            return DApiPeripheralType(self.board.regs.ptr.value)
+        except KeyError:
+            return DApiPeripheralType.UNDEFINED
+
+    @property
+    def peripheralName(self):
+        if self.board.regs.ptr.isUndefined():
+            self.board.getRegisters('ptr')
+        if self.board.regs.pnr.isUndefined():
+            self.board.getRegisters('pnr')
+        return f"{self.board.regs.ptr.asString()!s}-{self.board.regs.pnr.asString()!s}"
+
 
 class Workspace(BaseWorkspace):
     '''Class for a functional Workspace.
-    
-    :param BaseBoard board: The board. 
+
+    :param BaseBoard board: The board.
     :param str name: The workspace name.
     :param int par: The workspace number = PAR value used to activate the workspace
-    :param int pcr: The configuartion code   
-    
-    
+    :param int pcr: The configuartion code
+
+
     .. inheritance-diagram:: Workspace
         :parts: 1
 
     '''
-    
+
     def __init__(self, board, name=None, number=None, pcr=None):
         super().__init__(board, name, number, pcr)
         self.log.debug('PAR={0:d}, PCR={1:04x}'.format(number, pcr.value))
         self.cfg = [0]*4
 
-        
 
-            
-        #TODO: for i in range(board.wcaCount): 
+
+
+        #TODO: for i in range(board.wcaCount):
             # self.wca.append( MemoryWC(i, self.wca)  )
-            #self.eeprom.wca_list.append(self.wca)        
-            
-            
-        
+            #self.eeprom.wca_list.append(self.wca)
+
+
+
+
 
-    
 #     def set_captor_mode(self, mode):
 #         self._pcr['CAPTOR'].set(mode.value)
         #
     # def get_captor_mode(self):
         # return dboard.Sensors(self._pcr['CAPTOR'].value)
         #
 #     def set_reference_mode(self, mode):
 #         self._pcr['REFERENCE'].set(mode.value)
-        
+
     # def get_reference_mode(self):
         # return dboard.SpeedRequestMode(self._pcr['REFERENCE'].value)
-    
+
     def get_temp_running(self):
         return self._pcr['TMP_RUN'].value
     def get_temp_idle(self):
         return self._pcr['TMP_IDLE'].value
-        
+
 
     @property
     def ppa(self):
         return self._pcr.value & 0x000f
-     
+
     @property
     def rdt(self):
         return (self._pcr.value & 0x0f00) >> 8
-    
+
     @property
     def idt(self):
         return (self._pcr.value & 0xf000) >> 12
-    
+
     @property
     def description(self):
         return 'Workspace #{par:d}\nIdle temperature multiplicator: {idt:d}\nRun temperature multiplicator: {rdt:d}'.format(par=self.par,idt=self.idt, rdt=self.rdt)
 
-    
-         
+
+
 class StandbyWorkspace(BaseWorkspace):
     '''Class for the *standby* workspace
-    
-    :param BaseBoard board: The board. 
-    
+
+    :param BaseBoard board: The board.
+
     .. inheritance-diagram:: StandbyWorkspace
         :parts: 1
-    
-    '''        
-     
+
+    '''
+
     def __init__(self, board):
         super().__init__(board, 'Standby', 0, None)
         self.log.debug('Construct')
 
     def isFunctional(self):
         '''Alwayse return False. This workspace is never functional.'''
         return False
-     
+
     @property
     def standby(self):
         return True
     @property
     def description(self):
-        return 'Standby'    
-    
+        return 'Standby'
+
 class WorkspacesContainer(BaseBoardItem):
     '''Container class for workspaces of board
-    
+
     .. inheritance-diagram:: WorkspacesContainer
         :parts: 1
-    
+
     '''
     def __init__(self, board, name=None):
         super().__init__(board, name)
         self._items = []
-        
+
     def __getitem__(self, index):
         self._items[index]
-    
+
     def __setitem__(self, index, value):
         self._items[index] = value
-    
+
     def __len__(self):
         return len(self._items)
-    
+
     def __iter__(self):
         return iter(self._items)
-    
+
     def getByPAR(self, par):
         for w in self._items:
             if w.par == par:
                 return w
-    
+
     def clear(self):
         self._items.clear()
-    
+
     def append(self, item):
         self._items.append(item)
-        
+
     @property
     def count(self):
         return len(self._items)
 
-
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dcom/base.py` & `PyDapi2-0.6.2/src/dapi2/dcom/base.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dcom/demu.py` & `PyDapi2-0.6.2/src/dapi2/dcom/demu.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dcom/dserial.py` & `PyDapi2-0.6.2/src/dapi2/dcom/dserial.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dcom/dsocket.py` & `PyDapi2-0.6.2/src/dapi2/dcom/dsocket.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/derror.py` & `PyDapi2-0.6.2/src/dapi2/derror.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dmsg/common.py` & `PyDapi2-0.6.2/src/dapi2/dmsg/common.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dmsg/message.py` & `PyDapi2-0.6.2/src/dapi2/dmsg/message.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dmsg/reader.py` & `PyDapi2-0.6.2/src/dapi2/dmsg/reader.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dmsg/writer.py` & `PyDapi2-0.6.2/src/dapi2/dmsg/writer.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/base.py` & `PyDapi2-0.6.2/src/dapi2/dreg/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,124 +12,131 @@
 class DRegException(DApiException):
     '''Base class for register's module exceptions.'''
     pass
 
 
 class DRegAccess(IntEnum):
     '''Enumeration of register access mode'''
-    
+
     NO    = 0
     READ  = 1
     WRITE = 2
     RW    = 3
-    
+
+
+class DRegType(IntEnum):
+    '''Enumeration of register types'''
+    GLOBAL = 0
+    WORKSPACE = 1
+
+
 class DRegChangedSignal(DSignal):
-    
+
     def __init__(self, reg):
         self._reg = reg
         super().__init__(name='changed')
-        
-        
+
+
     def emit(self, old):
         for callback in self.callbacks:
             callback(self._reg, old, self._reg.value)
 
 class BaseRegElement(object):
     '''Base class for registers structure elements.
-    
+
     :param BaseRegElement parent: Parent element.
-    
+
     :param str name: Element name
-    
+
     :param int addr: Element address in registers array.
 
     :param int size: Element size, number of registers slot in group (optional, default: 1).
 
-    :param dict descriptions: Multilingual Element description (otional). 
-           The dictionary key is language code {fr,de,it,...} or None for the default language, by convention the English. 
-    
+    :param dict descriptions: Multilingual Element description (otional).
+           The dictionary key is language code {fr,de,it,...} or None for the default language, by convention the English.
+
     :param str shortname: Element short name (otional).
     '''
-    
+
     def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None):
         '''Initialize'''
 #         self.log = logging.getLogger('{0!s}:{1!s}'.format(self.__class__.__name__, name))
 #         self.log.debug('Initialize')
         self._parent = parent
         self._addr = addr
         self._size = size
         if name is None:
-            raise ValueError('The `name` argument must be defined.') 
+            raise ValueError('The `name` argument must be defined.')
         self.name = name
         self.shortname = shortname or name[:4]
-        if isinstance(descriptions, dict): 
+        if isinstance(descriptions, dict):
             self._descriptions = descriptions
         else:
-            self._descriptions = {None:descriptions}        
+            self._descriptions = {None:descriptions}
 
     def __str__(self, lang=None):
         try:
             return '{0:s} {1:!s} (size:{2:d})'.format(self.name, self._stringData(lang=lang))
         except:
             return self.name
-        
+
     def __lt__(self, other):
         return self.addr < other.addr
-        
+
     def _stringData(self, lang=None):
         try:
-            return '@{0:02x} (size:{1:d})'.format(self.addr, self.size) 
+            return '@{0:02x} (size:{1:d})'.format(self.addr, self.size)
         except Exception as e:
             return  "!!Base:" + str(e)+ "!!"
-        
-        
+
+
     def add(self, element):
         assert False, 'Abstract method!'
-        
+
     def getNext(self):
         try:
             return self.container[self.addr+1]
         except KeyError:
             return None
-        
+
     def toStringChildren(self, indent=0, prefix='', end='', depth=0, lang=None):
         '''Returns a pretty listing of groups and registers (children) of this container.
-        
+
         :param indent: Indentation level (optional, default: 1)
         :type indent: int
-        
+
         :param prefix: Prefix for the child's name (optional, default: null string)
         :type prefix: str
-        
+
         :param end: String applied on the end of child's representation (optional, default: null string)
         :type end: str
-        
+
         :param depth: The exploration deep of children and grand-children (optional, default: 0 = no exploration)
         :type depth: int
-        
+
         :return: A string with the listing of groups and registers.
         :rtype: str
         '''
         return ''
-    
+
     def toString(self, indent=0, prefix='', end='', depth=0, lang=None):
         '''Returns a pretty representation of this object.
-        
+
         :param indent: Indentation level (optional, default: 1)
         :type indent: int
-        
+
         :param prefix: Prefix for the object's name (optional, default: null string)
         :type prefix: str
-        
+
         :param end: String applied on the end representation (optional, default: null string)
         :type end: str
-        
+
         :param depth: The depth of exploration of children and grandchildren (optional, default: 0 = no exploration)
         :type depth: int
-        
+
         :return: A string with the listing of groups and registers.
         :rtype: str
         '''
         try:
             sChildren = ''
             sData = self._stringData(lang=lang)
             if sData != '':
@@ -137,98 +144,97 @@
             if depth > 0:
                 sChildren = self.toStringChildren(indent+1, depth=depth-1, lang=lang)
             if sChildren != '':
                 sChildren = '\n'+str(sChildren)
             return '\t' * indent + str(prefix) + self.__class__.__name__ +":"+ str(self.name) + sData + sChildren + end
         except Exception as e:
             return '\t' * indent + prefix + "!!Base:" + str(e)+ "!!" + str(self) + end
-        
-        
+
+
     def setParent(self, parent):
         self._parent = parent
-        
+
     def set(self, value):
         self.container.values[self.addr] = value
-        
+
     def get(self):
-        return self.container.values[self.addr]        
-    
+        return self.container.values[self.addr]
+
     def getDescription(self, lang=None):
         try:
             return self._descriptions[lang]
         except KeyError:
             try:
                 return self._descriptions[None]
             except KeyError:
-                return None    
-        
+                return None
+
     @property
     def descriptions(self):
         return self._descriptions
-    
+
     @property
     def descr(self):
         return self.getDescription()
-    
+
     @property
     def parent(self):
         '''Parent (:class:`BaseRegElement`) of this element.'''
-        return self._parent  
-    
+        return self._parent
+
     @property
     def container(self):
-        '''Container (:class:`~dapi2.reg.Registers`) of element.''' 
+        '''Container (:class:`~dapi2.reg.Registers`) of element.'''
         if self.parent:
             return self.parent.container
         else:
             return None
-  
+
     @property
     def addr(self):
         '''Element address (int) of this element in the DAPI2 registers structure.'''
         return self._addr
 
     @addr.setter
     def addr(self, value):
         self.setAddr(value)
-        
+
     def setAddr(self, value):
         '''Set address of element.
-        
+
         :param value: The new address of element.
         :type value: int
         '''
         self._addr = int(value)
-        
+
     @property
     def size(self):
         '''Element size (int) of this element (number of registers).
         '''
         return self._size
-    
-    @size.setter 
+
+    @size.setter
     def size(self, value):
         self.setSize(value)
-        
+
     def setSize(self, value):
         '''Set size (number of registers) of element.
-        
+
         :param value: The new size of element.
         :type value: int
         '''
         self._size = int(value)
-        
+
     @property
     def index(self):
         return self.addr - self.parent.addr
-        
-    
+
+
     @property
     def value(self):
         return self.get()
-         
+
     @value.setter
     def value(self, value):
         self.set(value)
-        
 
-        
+
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/container.py` & `PyDapi2-0.6.2/src/dapi2/dreg/container.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/dev/dev.py` & `PyDapi2-0.6.2/src/dapi2/dreg/dev/dev.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/group.py` & `PyDapi2-0.6.2/src/dapi2/dreg/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 '''Module for the class of group element
 
 :author: F. Voillat
 :date: 2021-02-17 Creation
 '''
 from .. import dreg
-        
+from .base import DRegType
+
 class RegGroup(dreg.BaseRegElement):
     '''Class for registers group in DAPI2 registers structure.
-    
-    :param parent: Registers parent element.
-    :type parent: Regsisters
-    
-    :param name: Group name
-    :type name: str
-
-    :param addr: Group base address in registers array.
-    :type addr: int
-
-    :param size: Group size, number of registers slot in group (optional).
-    :type size: int
 
-    :param descr: Group  description (otional).
-    :type descr: str
+    Args:
+        parent (Registers): Registers parent element.
+
+        name (str): Group name
+
+        addr (int): Group base address in registers array.
+
+        size (int): Group size, number of registers slot in group (optional).
 
-    :param shortname: Group short name (otional).
-    :type shortname: str
+        descr (str): Group  description (otional).
 
-    :param access: Group access mode (otional, default:DRegAccess.READ).
-    :type readonly: DRegAccess
+        shortname (str): Group short name (otional).
+
+        access (DRegAccess): Group access mode (otional, default:DRegAccess.READ).
+
+        rtype (DRegType) : The register type (default: DRegType.GLOBAL)
+
+        regs (list of Register) : The registers of this group (default: empty list)
     '''
-    
-    
-    def __init__(self, name, parent=None, addr=None, size=0, descriptions=None, shortname=None, access=dreg.DRegAccess.READ, regs=[]):
+
+
+    def __init__(self, name, parent=None, addr=None, size=0, descriptions=None, shortname=None, access=dreg.DRegAccess.READ, rtype=DRegType.GLOBAL, regs=[]):
         assert parent is None or isinstance(parent, dreg.RegContainer), 'parent is '+type(parent).__name__
+        assert isinstance(rtype, dreg.DRegType)
         super().__init__(name, parent=parent, addr=addr, size=size, descriptions=descriptions, shortname=shortname)
-        self._access = access  
+        self._access = access
         self._regs = []
-        
+        self._rtype = rtype
+
         for reg in regs:
             reg.setParent(self)
             self.add(reg)
 
     def __getitem__(self, index):
         return self._regs[index]
-    
+
     def __len__(self):
         return len(self._regs)
-    
+
     def __iter__(self):
         for dreg in self._regs:
-            yield dreg 
-    
+            yield dreg
+
     def _stringData(self):
         try:
-            return 'addr:{0:02X} size:{1:d} {2!s}'.format(self.addr, self.size, 'readonly' if self.readonly else '') 
+            return 'addr:{0:02X} size:{1:d} {2!s}'.format(self.addr, self.size, 'readonly' if self.readonly else '')
         except Exception as e:
-            return  "!!Group:" + str(e)+ "!!"   
-        
+            return  "!!Group:" + str(e)+ "!!"
+
     def toStringChildren(self, indent=1, prefix='', end='', depth=0):
         '''Returns a pretty listing of registers (children) of this group.
-        
+
         :param indent: Indentation level (optional, default: 1)
         :type indent: int
-        
+
         :param prefix: Prefix for the child's name (optional, default: null string)
         :type prefix: str
-        
+
         :param end: String applied on the end of child's representation (optional, default: null string)
         :type end: str
-        
+
         :param depth: The depth of exploration of children and grandchildren (optional, default: 0 = no exploration)
         :type depth: int
-        
+
         :return: A string with the listing of groups and registers.
         :rtype: str
-        '''        
+        '''
         if len(self._regs)>=100:
             idx_fmt = '{0:03d} ‒ '
         elif len(self._regs)>=10:
             idx_fmt = '{0:02d} ‒ '
         else:
             idx_fmt = '{0:d} ‒ '
-        return prefix + '\n'.join( [x.toString(indent,idx_fmt.format(i),depth=depth-1) for (i,x) in enumerate(self.regs)]  ) + end      
-   
-        
+        return prefix + '\n'.join( [x.toString(indent,idx_fmt.format(i),depth=depth-1) for (i,x) in enumerate(self.regs)]  ) + end
+
+
     def add(self, *elements):
         '''Adds an elements to this group
-        
+
         :param elements: One or more elements to be added to the group
         :type elements: BaseRegElement
-        
+
         :return: The next address after the last added element
         :rtype: int
         '''
         for element in elements:
             if isinstance(element, (dreg.Register, dreg.RegisterArray, )):
                 self._regs.append(element)
                 if element.addr is None:
@@ -102,22 +103,32 @@
                     self.container.add(element)
             else:
                 raise TypeError('An object of class {0!s} cannot be added to the container.'.format(type(element).__name__))
             next_addr = element.addr+element.size
             if next_addr > self.addr + self._size:
                 self.setSize(next_addr-self.addr)
         return next_addr
-    
+
+    def sort(self):
+        return self
+
+    def isUndefined(self):
+        return any([r.isUndefined() for r in self._regs])
+
     @property
     def values(self):
         return self.container.values[self.addr:self.addr+self.size]
-    
-    @property        
+
+    @property
     def regs(self):
         '''The list of registers of the group.'''
         return self._regs
-    
+
     @property
     def access(self):
         '''The group access mode'''
         return self._access
-    
+
+    @property
+    def rtype(self):
+        '''The register type'''
+        return self._rtype
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/reader.py` & `PyDapi2-0.6.2/src/dapi2/dreg/reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,239 +11,248 @@
 from os.path import os
 
 
 
 
 def getXmlDescription(xelement, lang='en'):
     '''Get description of XML element according language.
-    
+
     :param xelement: The XML element
     :type xelement: ElementTree
-     
+
     :param lang: The desired language
     :type lang: str
-    
+
     :return: The description in the specified language, otherwise the first one found or `None` if no description is found.
     :rtype: str
     '''
     xdescr = xelement.find( "descr[@lang='{}']".format(lang)  )
     if xdescr == None:
         xdescr = xelement.find( "descr[1]"  )
     if xdescr != None:
         return xdescr.text
     return None
 
 def getXmlDescriptions(xelement):
     '''Get all descriptions of XML element.
-    
+
     :param xelement: The XML element
     :type xelement: ElementTree
     '''
     ret = {}
     for xdescr in xelement.findall('descr'):
         ret[xdescr.get('lang', None)] = xdescr.text
     return ret
 
 class BaseRegReader(object):
     '''Base class for register structure elements reader
-    
+
     :param owner: Owner of reader.
     :type owner: BaseRegReader
-    
+
     :param parent: Parent element of elements on reading.
     :type parent: BaseRegElement
     '''
-    
+
     def __init__(self, owner, parent, element=None):
         self.log = logging.getLogger(self.__class__.__name__)
-        #self.log.debug('Initialize')            
+        #self.log.debug('Initialize')
         self._owner = owner
-        self._parent = parent         
+        self._parent = parent
         self._element = element
-        
+
     @property
     def parent(self):
         '''Parent reader.'''
         return self._parent
-        
+
     @property
     def element(self):
         '''Register structure element on reading.'''
         return self._element
-    
-    
+
+
 class RegContainerReader(BaseRegReader):
     '''Object class for read and construct the registers structure.
-    
+
     :param: container: The container or registers structure.
     :type container: RegContainer
-    
+
     :param: filename: The file containing the definition of the registers.
     :type filename: str
     '''
-    
-    
-    
+
+
+
     AVAILABLE_FILE_FORMAT = ('xml',)
-    
+
     def __init__(self, container=None, filename=None):
         assert container is None or isinstance(container, dreg.RegContainer)
-          
+
         super().__init__(None, None, container)
-        
+
         if filename is not None:
             self.readFromFile(filename)
-        
-    
+
+
     def readFromFile(self, filename):
         '''Read the registers structure from file.
-        
+
         :param filename: The filename (path) of file containing registers structure.
         :type filename: str
         '''
         if self.element is None:
             self._element = dreg.RegContainer(None)
         self.element.clear()
-        
+
         #TODO: select file reader regarding the format of file `filename`
         self.readXML(ET.parse(filename))
-        
+
         return self.element
-            
-        
+
+
     def readXML(self, xtree, addr=0):
         '''Read XML tree registers structure.
-        
+
         :param xtree: The XML tree contaning the registers structure and description
         :type xtree: ElementTree
 
         :param addr: Base addrees of registers to read.
         :type addr: int
         '''
         size = None
         xroot = xtree.getroot()
-        
+
         #self.log.debug('readXML:<'+xroot.tag+'>')
-        
+
         try:
-            size = int(xroot.get('size'),0) 
+            size = int(xroot.get('size'),0)
         except ValueError:
             pass
         if size is not None:
             self.element.setSize(size)
-        
+
         rgroup = RegGroupReader(self, self.element)
         for xgroup in xroot.findall('group'):
             group = rgroup.readXml(xgroup, addr)
             addr = self.element.add(group)
             if addr > self.element.size:
                 self.element.setSize(addr)
-            
-            
 
-        
+
+
+
 class RegGroupReader(BaseRegReader):
-    '''Class to read groups of registers''' 
+    '''Class to read groups of registers'''
 
     def readXml(self, xgroup, addr=0):
         '''Read XML tree of group of registers.
         '''
         #self.log.debug('readXML:<'+xgroup.tag+' name="'+str(xgroup.get('name'))+'">')
         try:
             addr = int(xgroup.get('address'),0)
         except:
             pass
         self._element = dreg.RegGroup(
                         xgroup.get('name'),
-                        self.parent, 
-                        addr, 
-                        size=int(xgroup.get('size','0'),0), 
+                        self.parent,
+                        addr,
+                        size=int(xgroup.get('size','0'),0),
                         descriptions=getXmlDescriptions(xgroup),
                         shortname=xgroup.get('shortname'),
-                        access=dreg.DRegAccess[xgroup.get('access','READ')], 
+                        access=dreg.DRegAccess[xgroup.get('access','READ')],
+                        rtype=dreg.DRegType[xgroup.get('rtype','GLOBAL')],
                     )
 
-                    
+
         rreg =  RegReader(self, self.element)
         for xreg in xgroup.findall('reg'):
             reg = rreg.readXml(xreg, addr)
             addr = self.element.add(reg)
 
         return self.element
-    
-    
+
+
 class RegReader(BaseRegReader):
-    '''Class to read registers''' 
-    
+    '''Class to read registers'''
+
     def readXml(self, xreg, addr=0):
         #self.log.debug('readXML:<'+xreg.tag+' name="'+str(xreg.get('name'))+'">')
         try:
             addr = int(xreg.get('address'),0)
         except:
             pass
         try:
             size = int(xreg.get('size'),0)
         except:
             size = 1
-            
+
         name = xreg.get('name')
-        
+
         if size == 1:
             if name is None:
                 _class = dreg.ReservedRegister
-                name = 'Reserved' 
+                name = 'Reserved'
             else:
                 _class = dreg.Register
-            
+
             if xreg.find('bit') is not None:
-                _class = dreg.BitFieldRegister 
+                _class = dreg.BitFieldRegister
         elif size > 1:
-            _class = dreg.RegisterArray 
+            _class = dreg.RegisterArray
         else:
-            raise ValueError('Size must be greater than 0') 
-        
+            raise ValueError('Size must be greater than 0')
+
         try:
-            access = dreg.DRegAccess[xreg.get('access')] 
+            access = dreg.DRegAccess[xreg.get('access')]
         except:
             access  = self.parent.access
+
+        try:
+            rtype = dreg.DRegType[xreg.get('rtype')]
+            print(rtype)
+        except:
+            rtype  = self.parent.rtype
+
         self._element = _class( name,
-                         self.parent, 
-                         addr, 
-                         size=size, 
+                         self.parent,
+                         addr,
+                         size=size,
                          descriptions=getXmlDescriptions(xreg),
                          shortname=xreg.get('shortname'),
-                         access =access ,
+                         access = access,
+                         rtype = rtype,
                          )
-        
+
         if _class is dreg.BitFieldRegister:
-            bit_addr = 0 
+            bit_addr = 0
             rbit = BitFieldReader(self, self.element)
             for xbit in xreg.findall('bit'):
                 bit = rbit.readXml(xbit, bit_addr)
                 bit_addr = self.element.add(bit)
 
         return self.element
 
 
 class BitFieldReader(BaseRegReader):
-    
+
     def readXml(self, xbit, addr=0):
         #self.log.debug('readXML:<'+xbit.tag+' name="'+str(xbit.get('name'))+'">')
         size = int(xbit.get('size','1'),0)
         name = xbit.get('name')
         if name is not None:
             self._element = dreg.RegBit(name, self.parent, addr, size, descriptions=getXmlDescriptions(xbit),)
             self._element.choices = {}
             for xchoice in xbit.findall('choice'):
                 v = int(xchoice.get('value','0'),0)
                 self._element.choices[v] = xchoice.get('name')
-        else: 
+        else:
             self._element = dreg.ReservedRegBit('Reserved', self.parent, addr, size, descriptions=getXmlDescriptions(xbit),)
         return self.element
-    
+
 def newRegContainerFromFile(filename=None):
     if filename is None:
         filename = os.path.join(os.path.dirname(__file__), 'regs.xml')
     regs = dreg.RegContainer(None)
     reader = RegContainerReader(regs)
     reader.readFromFile(filename)
-    return regs    
+    return regs
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/register.py` & `PyDapi2-0.6.2/src/dapi2/dreg/register.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,412 +1,440 @@
 '''
 Created on 8 févr. 2021
 
 @author: fv
 '''
 
-from .base import BaseRegElement, DRegException, DRegAccess, DRegChangedSignal
+from .base import BaseRegElement, DRegException, DRegAccess, DRegChangedSignal, DRegType
 from .. import dreg
-from ..common import REG_MAX_VALUE  
+from ..common import REG_MAX_VALUE
+
 
- 
 
 class DRegUndefinedError(DRegException):
     def get(self):
         return None
 
 
 class Register(BaseRegElement):
     '''Class for registers group in DAPI2 registers structure.
-    
-    :param parent: Registers parent element.
-    :type parent: Regsisters
-    
-    :param name: Group name
-    :type name: str
-
-    :param addr: Group base address in registers array.
-    :type addr: int
-
-    :param size: Group size, number of registers slot in group (optional).
-    :type size: int
 
-    :param dict descriptions: Multilingual Element description (otional). 
-           The dictionary key is language code {fr,de,it,...} or None for the default language, by convention the English. 
+    Args:
+        parent (Registers): Registers parent element.
+
+        name (str): Group name
+
+        addr (int): Group base address in registers array.
+
+        size (int): Group size, number of registers slot in group (default: 1).
+
+        descriptions (dict) : multilingual Element description (optional).
+           The dictionary key is language code {fr,de,it,...} or None for the default language, by convention the English.
+
+        shortname (str): Group short name (default: None).
+
+        min (int): The minimum value allowed (default: 0)
 
-    :param shortname: Group short name (otional).
-    :type shortname: str
+        max (int): the maximum value allowed (default: REG_MAX_VALUE)
+
+        access (DRegAccess): Register access mode (default: DRegAccess.READ).
+
+        rtype (DRegType) : The register type (default: DRegType.GLOBAL)
 
-    :param access: Register access mode (default:DRegAccess.READ).
-    :type access: DRegAccess
     '''
-    
-    
-    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, min=0, max=REG_MAX_VALUE, access=dreg.DRegAccess.READ): #@ReservedAssignment
+
+
+    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, min=0, max=REG_MAX_VALUE, access=dreg.DRegAccess.READ, rtype=DRegType.GLOBAL ): #@ReservedAssignment
         #assert parent is None or isinstance(parent, (dreg.RegContainer, dreg.RegGroup, dreg.RegisterArray )), 'parent is '+type(parent).__name__
         assert isinstance(parent, (dreg.RegContainer, dreg.RegGroup, dreg.RegisterArray )), 'parent is '+type(parent).__name__
+        assert isinstance(rtype, DRegType)
         super().__init__(name, parent, addr, size, descriptions, shortname)
         self._access = access
+        self._rtype = rtype
         self.min = min
-        self.max = max 
+        self.max = max
         self._modified = False
         self._undefined = True
         self._changed = DRegChangedSignal(self)
-        
-        
+
+
     def _stringData(self, lang=None):
         try:
             return '0x{3:04x}({3:d}) ; addr:{0:02X} ×{1:d} {2!s} '.format(
-                    self.addr, 
-                    self.size, 
+                    self.addr,
+                    self.size,
                     'R-' if self.readonly else 'RW',
-                    self.value) 
+                    self.value)
         except Exception as e:
             return  "!!Register:" + str(e)+ "!!"
-        
+
     def _valueChanged(self, old):
         if self.container.eventsEnabled:
             self.changed.emit(old)
-        
+
     def isModified(self):
+        '''Returns True if the register value has been modified from the last write into board
+
+        Returns:
+            (bool) : The state of the modification status.
+        '''
         return self._modified
-    
+
     def isUndefined(self):
+        '''Returns True if the register value has never been defined from the start up.
+
+        Returns:
+            (bool) : The state of the define status.
+        '''
         return self._undefined
 
     def isDefined(self):
+        '''Returns True if the register value has been defined from the start up.
+
+        Returns:
+            (bool) : The state of the define status.
+        '''
         return not self._undefined
 
-    
+
     def asString(self):
-        return chr(self.value // 256) + chr( self.value & 0xff )  
-    
+        '''Returns the register value as a characters string.
+
+        Returns:
+            (str) : The register value as a characters string.
+        '''
+        return chr(self.value // 256) + chr( self.value & 0xff )
+
     def alter(self, value):
-        return self.set(value)
-    
+        return self.set(value, True)
+
     def internalSet(self, value, modified=False):
         old = self.container.values[self.addr]
-        self._modified = modified and old != value 
+        self._modified = modified and old != value
         if self._undefined or old != value:
             self.container.values[self.addr] = value
             self._undefined = False
             self._valueChanged(old)
-        
+
         return value
-            
+
     def set(self, value):
         return self.internalSet(value, True)
-    
+
     def setMin(self):
         return self.set(self.min)
 
     def setMax(self):
         return self.set(self.max)
-    
+
     def clear(self):
         return self.set(0)
-    
+
     def reset(self):
-        self._modified = False 
+        self._modified = False
         self._undefined = True
-    
+
+
     def get(self):
         if self._undefined:
             raise DRegUndefinedError(self, 'get', 'Undefined value in register '+self.name)
-        return self.container.values[self.addr]      
-    
+        return self.container.values[self.addr]
+
     @property
     def access(self):
         '''The register access mode'''
         return self._access
-    
+
     @property
     def changed(self):
         return self._changed
-        
+    @property
+    def rtype(self):
+        '''The register type.'''
+        return self._rtype
+
 class ReservedRegister(Register):
     pass
 
 class RegisterBits(object):
-    
+
     def __init__(self, parent):
         self._parent = parent
         self._bits = []
         self._index = {}
-        
+
     def __getattr__(self, name):
         return self.getBit(name)
 
     def __call__(self, name):
         return self.getBit(name)
 
     def __getitem__(self, index):
         return self._bits[index]
-    
+
     def __len__(self):
         return len(self._bits)
-    
+
     def __iter__(self):
         for bit in self._bits:
-            yield bit         
+            yield bit
+
 
-        
     def _getNextFreeAddr(self):
         if len(self._bits)==0:
             return 0
         else:
             return self._bits[-1].addr + self._bits[-1].size
 
     def add(self, *bits):
         '''Adds bits to this bits field register
-        
+
         :param bit: One or more bits to be added to the bits field register
         :type bit: RegBit
-        
+
         :return: The next address (position) after the last added bit
         :rtype: int
         '''
         for bit in bits:
             if bit.addr is None:
                 bit.setAddress(self._getNextFreeAddr())
             self._bits.append(bit)
             self._index[bit.name] = bit
-            
+
             self._bits.sort(key=lambda x: x.addr)
         return bit.addr+bit.size
 
-    
+
     def getBit(self, name):
         '''Returns the bit  according to its name.
-        
+
         :param str name: the bit name to return
-        
+
         :return: The bit found
         :rtype: RegBit
         '''
         return self._index[name]
 
-        
+
 class BitFieldRegister(Register):
-    
-    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, access=DRegAccess.READ):
-        super().__init__(name, parent, addr, size, descriptions, shortname, access)
+
+    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, access=DRegAccess.READ, rtype=DRegType.GLOBAL):
+        super().__init__(name, parent, addr, size, descriptions, shortname=shortname, access=access, rtype=rtype)
         self._bits = RegisterBits(self)
-        
+
     def __len__(self):
         return len(self._bits)
-    
+
     def __iter__(self):
         for bit in self._bits:
-            yield bit         
-        
+            yield bit
+
     def _stringData(self, lang=None):
         try:
-            return super()._stringData() + " ; count:{}".format(len(self)) 
+            return super()._stringData() + " ; count:{}".format(len(self))
         except Exception as e:
-            return  "!!BitFieldRegister:" + str(e)+ "!!"     
-        
+            return  "!!BitFieldRegister:" + str(e)+ "!!"
+
     def getBit(self, name):
         '''Returns the bit  according to its name.
-        
+
         :param str name: the bit name to return
-        
+
         :return: The bit found
         :rtype: RegBit
         '''
         return self._bits.getBit(name)
-        
-        
+
+
     def toStringChildren(self, indent=1, prefix='', end='', depth=0, lang=None):
         '''Returns a pretty listing of registers (children) of this group.
-        
+
         :param indent: Indentation level (optional, default: 1)
         :type indent: int
-        
+
         :param prefix: Prefix for the child's name (optional, default: null string)
         :type prefix: str
-        
+
         :param end: String applied on the end of child's representation (optional, default: null string)
         :type end: str
-        
+
         :param depth: The depth of exploration of children and grandchildren (optional, default: 0 = no exploration)
         :type depth: int
-        
+
         :return: A string with the listing of groups and registers.
         :rtype: str
-        '''        
+        '''
         if len(self._bits)>=10:
             idx_fmt = '{0:02d} ‒ '
         else:
             idx_fmt = '{0:d} ‒ '
-        return prefix + '\n'.join( [x.toString(indent,idx_fmt.format(i),depth=depth-1, lang=lang) for (i,x) in enumerate(self._bits)]  ) + end      
-                   
+        return prefix + '\n'.join( [x.toString(indent,idx_fmt.format(i),depth=depth-1, lang=lang) for (i,x) in enumerate(self._bits)]  ) + end
+
 
     def add(self, *bits):
         '''Adds bits to this bits field register
-        
+
         :param bit: One or more bits to be added to the bits field register
         :type bit: RegBit
-        
+
         :return: The next address (position) after the last added bit
         :rtype: int
         '''
         return self._bits.add(*bits)
-    
-    
+
+
     @property
     def bits(self):
-        return self._bits 
-        
+        return self._bits
+
 class RegisterArray(Register):
-    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, access=dreg.DRegAccess.READ):
-        super().__init__(name, parent, addr, size, descriptions, shortname, access)
+    def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, access=dreg.DRegAccess.READ,  rtype=DRegType.GLOBAL):
+        super().__init__(name, parent, addr, size, descriptions, shortname, access, rtype)
         self._regs = []
-        
+
         for i in range(self.size):
-            reg = Register(self.name+str(i), self, self.addr+i, size=1, shortname=self.shortname+str(i), access=access)
+            reg = Register(self.name+str(i), self, self.addr+i, size=1, shortname=self.shortname+str(i), access=access, rtype=rtype)
             self._regs.append(reg)
 
     def __getitem__(self, index):
         return self._regs[index]
-    
+
     def __len__(self):
         return len(self._regs)
-    
+
     def __iter__(self):
         for dreg in self._regs:
-            yield dreg     
-            
+            yield dreg
+
     def isUndefined(self):
         for r in self:
             if r.isUndefined():
                 return True
         return False
-    
+
     def _stringData(self, lang=None):
         try:
             s = '['+','.join( '0x{0:04x}({0:d})'.format(r.value) for r in self)+"]"
             return s + ' ; addr:{0:02X} ×{1:d} {2!s} '.format(
-                    self.addr, 
-                    self.size, 
-                    'R-' if self.readonly else 'RW') 
+                    self.addr,
+                    self.size,
+                    'R-' if self.readonly else 'RW')
         except Exception as e:
-            return  "!!RegisterArray:" + str(e)+ "!!"    
-    
+            return  "!!RegisterArray:" + str(e)+ "!!"
+
     def setAddr(self, value):
         Register.setAddr(self, value)
         for i, r in enumerate(self):
             r.setAddr(self.addr+i)
-    
+
     def alter(self, values):
         return self.set(values)
-        
+
     def set(self, values):
         for i, v in enumerate(values):
             self._regs[i].set(v)
         self._undefined = False
-        
+
     def internalSet(self, values, modified=False):
         self._modified = modified
         for i, v in enumerate(values):
             self._regs[i].internalSet(v, modified)
         self._undefined = False
-        
+
     def get(self):
         return list([ self._regs[i].get() for i in range(self.size) ])
 
 class RegBitChoice():
     def __init__(self, name, value, bit=None, descriptions=None, shortname=None ):
         self._bit = bit
         self.value = value
         self.name = name
-        if isinstance(descriptions, dict): 
+        if isinstance(descriptions, dict):
             self._descriptions = descriptions
         else:
-            self._descriptions = {None:descriptions}   
+            self._descriptions = {None:descriptions}
         if shortname is None:
             self.shortname = name[:3]
         else:
             self.shortname = shortname
-            
+
     def __str__(self):
         return '{0:d}:{1:s}'.format(self.value,self.name)
-            
+
     def __lt__(self, other):
         return self.value < other.value
-    
+
     def __eq__(self, other):
-        return self.value == other.value    
-    
+        return self.value == other.value
+
     def getDescription(self, lang=None):
         try:
             return self._descriptions[lang]
         except KeyError:
-            return self._descriptions[None]     
-        
+            return self._descriptions[None]
+
     @property
     def descriptions(self):
         return self._descriptions
-    
+
     @property
     def descr(self):
-        return self.getDescription()          
+        return self.getDescription()
 
 
 class RegBit(BaseRegElement):
     def __init__(self, name, parent=None, addr=None, size=1, descriptions=None, shortname=None, choices={}):
         super().__init__(name, parent, addr, size, descriptions, shortname)
         self.choices = choices
         if shortname is None:
             self.shortname = name[:3]
         else:
             self.shortname = shortname
         self._mask = ((1<<self._size)-1) << self._addr
-        
+
 #     def __str__(self):
 #         try:
 #             return '{p:2d}-{n:s}:{v!s}'.format(n=self.name, p=self.pos, v=self.choices[self.value])
 #         except KeyError:
 #             return ('{1:2d}-{0}:{2:0'+str(self._size)+'b} (0x{2:x})').format(self.name, self.pos, self.value)
 
-    
+
     def __lt__(self, other):
         return self.name < other.name
-    
+
     def __eq__(self, other):
         return self.name == other.name
-    
+
     def _stringData(self, lang=None):
         return "{0:d}".format(self.get())
-    
-    def internalSet(self, value, modified=False):
+
+    def internalSet(self, value=1, modified=False):
         assert value >= 0 and value < (1<<self._size), 'RegBit.internalSet:{} is an invalid value for the flag {}.{}'.format(value,self._owner.reg.name,self.name)
         return self._parent.internalSet((self._parent.value & ~self._mask) | (value << self.addr), modified)
-    
+
     def alter(self, value):
         return self.set(value)
-        
+
     def set(self, value=1):
         assert value >= 0 and value < (1<<self._size), 'RegBit.set:{} is an invalid value for the flag {}.{}'.format(value,self._owner.reg.name,self.name)
         return self._parent.set((self._parent.value & ~self._mask) | (value << self.addr) )
-    
+
     def toggle(self):
         return self._parent.set(self._parent.value ^ self._mask)
-        
+
     def clear(self):
         return self.set(0)
-        
+
     def get(self):
         return (self._parent.value & self._mask) >> self.addr
-    
+
     def strValue(self):
         return '{v!s}'.format(v=self.choices[self.value])
-    
+
     @property
     def mask(self):
-        return self._mask  
-    
+        return self._mask
+
 class ReservedRegBit(RegBit):
     pass
 
-    
-        
+
```

### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/regs.xml` & `PyDapi2-0.6.2/src/dapi2/dreg/regs.xml`

 * *Files 2% similar despite different names*

#### Comparing `PyDapi2-0.4.3/src/dapi2/dreg/regs.xml` & `PyDapi2-0.6.2/src/dapi2/dreg/regs.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<registers size="256">
+<registers size="512">
   <group name="header" address="0x00">
     <descr>Header registers</descr>
     <descr lang="fr">Registres d'entête</descr>
     <reg name="par" access="RW">
       <descr>Peripheral Activation Register</descr>
     </reg>
     <reg name="ctr">
@@ -63,15 +63,15 @@
       <descr>Peripheral controller Name Register</descr>
     </reg>
   </group>
   <group name="state" address="0x24" access="READ">
     <descr>State registers</descr>
     <descr lang="fr">Registres d'état</descr>
     <text>Registers of this group provide information about the controller state. They are read only.</text>
-    <reg name="ssr1">
+    <reg name="ssr1" rtype="WORKSPACE">
       <descr>System Status Register part 1</descr>
       <bit name="driver" shortname="drv">
         <descr>Driver activation</descr>
         <choice value="0" name="idle">
           <descr>Driver is idle</descr>
         </choice>
         <choice value="1" name="enabled">
@@ -700,8 +700,12 @@
       </bit>
       <bit name="captor" size="2"/>
       <bit name="reference" size="2"/>
       <bit name="tmp_run" size="4"/>
       <bit name="tmp_idle" size="4"/>
     </reg>
   </group>
+  <group name="extended" address="0x80">
+    <descr>Extended registers</descr>
+    <reg name="extr" address="0x80" size="128"/>
+  </group>
 </registers>
```

### Comparing `PyDapi2-0.4.3/src/dapi2/errors.xml` & `PyDapi2-0.6.2/src/dapi2/errors.xml`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/dapi2/signal.py` & `PyDapi2-0.6.2/src/dapi2/signal.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/demu/DEmuBaseBoard.py` & `PyDapi2-0.6.2/src/demu/DEmuBaseBoard.py`

 * *Files identical despite different names*

### Comparing `PyDapi2-0.4.3/src/demu/DEmuPPA.py` & `PyDapi2-0.6.2/src/demu/DEmuPPA.py`

 * *Files identical despite different names*

