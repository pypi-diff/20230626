# Comparing `tmp/conf-ini-g-2023.5.tar.gz` & `tmp/conf-ini-g-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf-ini-g-2023.5.tar", last modified: Wed May 31 14:48:54 2023, max compression
+gzip compressed data, was "conf-ini-g-2023.6.tar", last modified: Mon Jun 26 12:17:29 2023, max compression
```

## Comparing `conf-ini-g-2023.5.tar` & `conf-ini-g-2023.6.tar`

### file list

```diff
@@ -1,94 +1,108 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/
--rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.5/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.5/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.5/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.5/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/
--rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.5/conf_ini_g/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/
--rw-r--r--   0 eric      (1000) users      (984)     2483 2023-05-31 14:28:04.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
--rw-r--r--   0 eric      (1000) users      (984)     2534 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1763 2023-05-31 13:56:41.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
--rw-r--r--   0 eric      (1000) users      (984)     2118 2023-05-31 13:46:25.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     1824 2023-05-31 14:27:49.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
--rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     1997 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
--rw-r--r--   0 eric      (1000) users      (984)     1701 2023-05-31 13:48:26.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3935 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     3176 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     2223 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/none.py
--rw-r--r--   0 eric      (1000) users      (984)     5499 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     7690 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/sequence.py
--rw-r--r--   0 eric      (1000) users      (984)     2592 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/text.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/catalog/specification/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     2376 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/boolean.py
--rw-r--r--   0 eric      (1000) users      (984)     2632 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/choices.py
--rw-r--r--   0 eric      (1000) users      (984)     5180 2023-05-31 14:28:32.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/number.py
--rw-r--r--   0 eric      (1000) users      (984)     2534 2023-05-31 14:26:57.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/path.py
--rw-r--r--   0 eric      (1000) users      (984)     4699 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/sequence.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/instance/
--rw-r--r--   0 eric      (1000) users      (984)    10398 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/instance/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/instance/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3374 2023-05-31 14:25:44.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/base.py
--rw-r--r--   0 eric      (1000) users      (984)     5255 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     4773 2023-05-31 14:25:44.000000 conf-ini-g-2023.5/conf_ini_g/instance/parameter/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/conf_ini_g/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/console/
--rw-r--r--   0 eric      (1000) users      (984)     1635 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/console/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     6532 2023-05-31 14:28:56.000000 conf-ini-g-2023.5/conf_ini_g/interface/console/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/screen/
--rw-r--r--   0 eric      (1000) users      (984)    14161 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     7467 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     9467 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/path_chooser.py
--rw-r--r--   0 eric      (1000) users      (984)     2586 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/type_selector.py
--rw-r--r--   0 eric      (1000) users      (984)     8380 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/interface/screen/section.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/interface/storage/
--rw-r--r--   0 eric      (1000) users      (984)     6838 2023-05-31 14:29:29.000000 conf-ini-g-2023.5/conf_ini_g/interface/storage/config.py
--rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.5/conf_ini_g/interface/storage/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/light/
--rw-r--r--   0 eric      (1000) users      (984)     4236 2023-05-31 14:29:35.000000 conf-ini-g-2023.5/conf_ini_g/light/config.py
--rw-r--r--   0 eric      (1000) users      (984)     3773 2023-05-26 18:53:12.000000 conf-ini-g-2023.5/conf_ini_g/light/conversion.py
--rw-r--r--   0 eric      (1000) users      (984)     2605 2023-05-31 14:29:41.000000 conf-ini-g-2023.5/conf_ini_g/light/ini.py
--rw-r--r--   0 eric      (1000) users      (984)     2080 2023-05-26 18:29:02.000000 conf-ini-g-2023.5/conf_ini_g/light/xlsx.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g/raw/
--rw-r--r--   0 eric      (1000) users      (984)     4535 2023-05-31 14:29:46.000000 conf-ini-g-2023.5/conf_ini_g/raw/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/
--rw-r--r--   0 eric      (1000) users      (984)     2821 2023-05-31 14:30:19.000000 conf-ini-g-2023.5/conf_ini_g/specification/base.py
--rw-r--r--   0 eric      (1000) users      (984)     7977 2023-05-31 12:39:36.000000 conf-ini-g-2023.5/conf_ini_g/specification/config.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/parameter/
--rw-r--r--   0 eric      (1000) users      (984)     3179 2023-05-31 14:29:52.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     4427 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/main.py
--rw-r--r--   0 eric      (1000) users      (984)     9497 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/type.py
--rw-r--r--   0 eric      (1000) users      (984)     3612 2023-05-31 14:30:01.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/unit.py
--rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.5/conf_ini_g/specification/parameter/value.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/specification/section/
--rw-r--r--   0 eric      (1000) users      (984)     9610 2023-05-31 14:30:13.000000 conf-ini-g-2023.5/conf_ini_g/specification/section/main.py
--rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.5/conf_ini_g/specification/section/unit.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/conf_ini_g/standard/
--rw-r--r--   0 eric      (1000) users      (984)     3079 2023-05-31 14:30:24.000000 conf-ini-g-2023.5/conf_ini_g/standard/path_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     3112 2023-05-26 13:22:35.000000 conf-ini-g-2023.5/conf_ini_g/standard/py_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     7544 2023-05-31 14:32:50.000000 conf-ini-g-2023.5/conf_ini_g/standard/str_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     3798 2023-05-31 14:30:34.000000 conf-ini-g-2023.5/conf_ini_g/standard/type_extension.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-05-31 14:34:20.000000 conf-ini-g-2023.5/conf_ini_g/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.960813 conf-ini-g-2023.5/conf_ini_g.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4428 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2714 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       20 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2023-05-31 14:48:54.000000 conf-ini-g-2023.5/conf_ini_g.egg-info/top_level.txt
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.957479 conf-ini-g-2023.5/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.5/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.5/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-05-31 14:48:54.964146 conf-ini-g-2023.5/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     6251 2023-05-31 14:48:37.000000 conf-ini-g-2023.5/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2023-03-01 07:58:57.000000 conf-ini-g-2023.6/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2023-03-01 08:10:10.000000 conf-ini-g-2023.6/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 conf-ini-g-2023.6/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3536 2023-03-01 09:58:27.000000 conf-ini-g-2023.6/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.007371 conf-ini-g-2023.6/conf_ini_g/
+-rw-r--r--   0 eric      (1000) users      (984)     1779 2023-05-12 13:37:01.000000 conf-ini-g-2023.6/conf_ini_g/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/catalog/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.007371 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/
+-rw-r--r--   0 eric      (1000) users      (984)     2529 2023-06-14 07:31:54.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2346 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.007371 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
+-rw-r--r--   0 eric      (1000) users      (984)     1965 2023-06-02 15:09:21.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:29.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     2060 2023-05-31 13:36:33.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
+-rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 14:56:56.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.010704 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/
+-rw-r--r--   0 eric      (1000) users      (984)     2679 2023-06-14 07:32:27.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
+-rw-r--r--   0 eric      (1000) users      (984)     2344 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.010704 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1915 2023-06-14 12:49:34.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
+-rw-r--r--   0 eric      (1000) users      (984)     2010 2023-06-02 15:43:40.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     1686 2023-06-14 13:55:33.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2023-06-14 13:56:59.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     2059 2023-06-02 14:30:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     1992 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
+-rw-r--r--   0 eric      (1000) users      (984)     1696 2023-06-01 15:01:41.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.014038 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3631 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     3814 2023-06-14 08:11:16.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     3859 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/directory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3387 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/multitype.py
+-rw-r--r--   0 eric      (1000) users      (984)     2222 2023-06-14 07:01:24.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/none.py
+-rw-r--r--   0 eric      (1000) users      (984)     6047 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     7470 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/sequence.py
+-rw-r--r--   0 eric      (1000) users      (984)     2460 2023-06-14 08:11:16.000000 conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/text.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/catalog/specification/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.014038 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     2267 2023-06-06 07:02:20.000000 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/boolean.py
+-rw-r--r--   0 eric      (1000) users      (984)     2472 2023-06-06 08:56:40.000000 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/choices.py
+-rw-r--r--   0 eric      (1000) users      (984)     4619 2023-06-06 12:27:27.000000 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/number.py
+-rw-r--r--   0 eric      (1000) users      (984)     2929 2023-06-06 09:24:59.000000 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     4289 2023-06-06 13:36:21.000000 conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/sequence.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     3078 2023-06-05 12:39:31.000000 conf-ini-g-2023.6/conf_ini_g/extension/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     3505 2023-06-09 07:12:44.000000 conf-ini-g-2023.6/conf_ini_g/extension/python.py
+-rw-r--r--   0 eric      (1000) users      (984)     5279 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/extension/string.py
+-rw-r--r--   0 eric      (1000) users      (984)     7932 2023-06-14 08:33:28.000000 conf-ini-g-2023.6/conf_ini_g/extension/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/instance/
+-rw-r--r--   0 eric      (1000) users      (984)    11085 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/instance/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/instance/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     3335 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/instance/parameter/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     4385 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/instance/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     4108 2023-06-14 08:11:16.000000 conf-ini-g-2023.6/conf_ini_g/instance/parameter/unit.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/conf_ini_g/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/interface/console/
+-rw-r--r--   0 eric      (1000) users      (984)     1635 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/interface/console/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     6498 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/interface/console/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/interface/screen/
+-rw-r--r--   0 eric      (1000) users      (984)     4500 2023-06-14 07:31:17.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)    16586 2023-06-14 14:16:41.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1945 2023-05-12 12:16:07.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.017371 conf-ini-g-2023.6/conf_ini_g/interface/screen/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     5655 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     7884 2023-06-14 13:10:38.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/parameter/path_chooser.py
+-rw-r--r--   0 eric      (1000) users      (984)     8811 2023-06-14 14:12:59.000000 conf-ini-g-2023.6/conf_ini_g/interface/screen/section.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.020704 conf-ini-g-2023.6/conf_ini_g/interface/storage/
+-rw-r--r--   0 eric      (1000) users      (984)     6515 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/interface/storage/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     1577 2023-05-10 13:30:33.000000 conf-ini-g-2023.6/conf_ini_g/interface/storage/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.020704 conf-ini-g-2023.6/conf_ini_g/light/
+-rw-r--r--   0 eric      (1000) users      (984)     4233 2023-06-06 15:18:55.000000 conf-ini-g-2023.6/conf_ini_g/light/config.py
+-rw-r--r--   0 eric      (1000) users      (984)     3764 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/light/conversion.py
+-rw-r--r--   0 eric      (1000) users      (984)     2595 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/light/ini.py
+-rw-r--r--   0 eric      (1000) users      (984)     2071 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/light/xlsx.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.020704 conf-ini-g-2023.6/conf_ini_g/raw/
+-rw-r--r--   0 eric      (1000) users      (984)     4519 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/raw/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.020704 conf-ini-g-2023.6/conf_ini_g/specification/
+-rw-r--r--   0 eric      (1000) users      (984)     2820 2023-06-05 12:39:31.000000 conf-ini-g-2023.6/conf_ini_g/specification/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     7241 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/specification/config.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/conf_ini_g/specification/parameter/
+-rw-r--r--   0 eric      (1000) users      (984)     2500 2023-06-06 08:53:53.000000 conf-ini-g-2023.6/conf_ini_g/specification/parameter/annotation.py
+-rw-r--r--   0 eric      (1000) users      (984)     4177 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/specification/parameter/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     6127 2023-06-14 14:12:58.000000 conf-ini-g-2023.6/conf_ini_g/specification/parameter/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     3434 2023-06-05 14:27:55.000000 conf-ini-g-2023.6/conf_ini_g/specification/parameter/unit.py
+-rw-r--r--   0 eric      (1000) users      (984)     2232 2023-05-31 14:26:58.000000 conf-ini-g-2023.6/conf_ini_g/specification/parameter/value.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/conf_ini_g/specification/section/
+-rw-r--r--   0 eric      (1000) users      (984)     9488 2023-06-06 15:35:51.000000 conf-ini-g-2023.6/conf_ini_g/specification/section/main.py
+-rw-r--r--   0 eric      (1000) users      (984)     1809 2023-05-12 12:45:21.000000 conf-ini-g-2023.6/conf_ini_g/specification/section/unit.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-06-26 12:13:52.000000 conf-ini-g-2023.6/conf_ini_g/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.007371 conf-ini-g-2023.6/conf_ini_g.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4428 2023-06-26 12:17:28.000000 conf-ini-g-2023.6/conf_ini_g.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     3454 2023-06-26 12:17:29.000000 conf-ini-g-2023.6/conf_ini_g.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-06-26 12:17:28.000000 conf-ini-g-2023.6/conf_ini_g.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       14 2023-06-26 12:17:28.000000 conf-ini-g-2023.6/conf_ini_g.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2023-06-26 12:17:28.000000 conf-ini-g-2023.6/conf_ini_g.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.004038 conf-ini-g-2023.6/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1982 2023-03-01 10:23:59.000000 conf-ini-g-2023.6/documentation/wiki/description.asciidoc
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 conf-ini-g-2023.6/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-06-26 12:17:29.024038 conf-ini-g-2023.6/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     6360 2023-06-26 12:16:56.000000 conf-ini-g-2023.6/setup.py
```

### Comparing `conf-ini-g-2023.5/PKG-INFO` & `conf-ini-g-2023.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.5
+Version: 2023.6
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.5/README-COPYRIGHT-utf8.txt` & `conf-ini-g-2023.6/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/README-LICENCE-utf8.txt` & `conf-ini-g-2023.6/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/README.rst` & `conf-ini-g-2023.6/README.rst`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/__init__.py` & `conf-ini-g-2023.6/conf_ini_g/__init__.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt5.QtCore as core
 import PyQt5.QtGui as visl
 import PyQt5.QtWidgets as wdgt
 
-
 ALIGNED_HCENTER = core.Qt.AlignmentFlag.AlignHCenter
+ALIGNED_LEFT = core.Qt.AlignmentFlag.AlignLeft
 ALIGNED_RIGHT = core.Qt.AlignmentFlag.AlignRight
 ALIGNED_TOP = core.Qt.AlignmentFlag.AlignTop
 BASE_PALETTE = visl.QPalette.Base
 COLOR_CYAN = visl.QColorConstants.Cyan
 DIALOG_ACCEPTATION = wdgt.QDialog.Accepted
 DIALOG_ACCEPT_OPEN = wdgt.QFileDialog.AcceptOpen
 DIALOG_ACCEPT_SAVE = wdgt.QFileDialog.AcceptSave
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,32 +25,23 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import PyQt5.QtCore as core
 import PyQt5.QtWidgets as wdgt
 
 from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
 
 
 class event_loop_t(wdgt.QApplication):
-    """"""
-
-    @staticmethod
-    def GetInstance() -> core.QCoreApplication:
-        """"""
-        return event_loop_t.instance()
-
-    @staticmethod
-    def Run() -> int:
+    def Run(self) -> int:
         """"""
-        return wdgt.QApplication.exec_()
+        return self.exec_()
 
 
 def ShowMessage(title: str, message: str, /, *, parent: library_wgt_t = None) -> None:
     """"""
     dialog = wdgt.QMessageBox(parent=parent)
     dialog.setWindowTitle(title)
     dialog.setText("<b>" + title + "</b>")
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Callable
 
-from PyQt5 import QtWidgets as wdgt
+import PyQt6.QtWidgets as wdgt
 
 
 class button_wgt_t(wdgt.QPushButton):
     """"""
 
-    def SetFunction(self, function: Callable) -> None:
+    def SetFunction(self, function: Callable, /) -> None:
         self.clicked.connect(function)
+
+
+class dot_button_wgt_t(wdgt.QRadioButton):
+    """"""
+
+    def SetFunction(self, function: Callable, /) -> None:
+        self.toggled.connect(function)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,29 +27,22 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Callable
 
-from PyQt5 import QtWidgets as wdgt
+import PyQt5.QtWidgets as wdgt
 
 
-class choices_dots_wgt_t(wdgt.QRadioButton):
-    """"""
-
-    def SetFunction(self, function: Callable) -> None:
-        self.clicked.connect(function)
-
-
-class choices_list_wgt_t(wdgt.QComboBox):
+class choice_menu_wgt_t(wdgt.QComboBox):
     """"""
 
     def Text(self) -> str:
         return self.currentText()
 
-    def ItemAt(self, index: int) -> str:
+    def ItemAt(self, index: int, /) -> str:
         return self.itemText(index)
 
-    def SetFunction(self, function: Callable) -> None:
+    def SetFunction(self, function: Callable, /) -> None:
         self.activated.connect(function)
         # OR: self.currentTextChanged.connect(function)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,16 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import PyQt5.QtWidgets as wdgt
 
-
 library_wgt_t = wdgt.QWidget
 
 group_wgt_t = wdgt.QGroupBox
-label_wgt_t = wdgt.QLabel
 stack_wgt_t = wdgt.QStackedWidget
 tabs_wgt_t = wdgt.QTabWidget
 
 hbox_lyt_t = wdgt.QHBoxLayout
 vbox_lyt_t = wdgt.QVBoxLayout
 grid_lyt_t = wdgt.QGridLayout
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from PyQt5 import QtWidgets as wdgt
+import PyQt5.QtWidgets as wdgt
 
 from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
 
 
 class scroll_container_t(wdgt.QScrollArea):
     """"""
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from PyQt5 import QtWidgets as wdgt
+import PyQt5.QtWidgets as wdgt
 
 
 class text_wgt_t(wdgt.QLineEdit):
     def Text(self) -> str:
         """"""
         return self.text().strip()
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/boolean.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/boolean.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,81 +27,73 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
-    choices_dots_wgt_t,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
-    hbox_lyt_t,
-    library_wgt_t,
+import dataclasses as dtcl
+
+from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
+from conf_ini_g.interface.screen.backend import (
+    backend_t,
+    choices_dots_wgt_h,
+    library_wgt_h,
 )
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import (
-    MISSING_REQUIRED_VALUE,
-    missing_required_value_t,
-)
-
 
-class boolean_wgt_t(library_wgt_t):
-    __slots__ = ("true_btn",)
-    true_btn: choices_dots_wgt_t
 
-    def __init__(self, parent: library_wgt_t = None) -> None:
-        """"""
-        super().__init__(parent=parent)
-
-        # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
-        for slot in boolean_wgt_t.__slots__:
-            setattr(self, slot, None)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class boolean_wgt_t:
+    library_wgt: library_wgt_h
+    true_btn: choices_dots_wgt_h = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewWithDetails(
         cls,
-        value: bool | None | missing_required_value_t,
-        value_type: type_t,
+        value: bool | None,
+        value_type: type_t | boolean_t | None,
+        backend: backend_t,
         _: parameter_t | None,
+        /,
     ) -> boolean_wgt_t:
         """
         If value_type does not contain the necessary details, an exclamation point is added to the default values.
         """
-        output = cls()
+        output = cls(library_wgt=backend.library_wgt_t())
 
-        # TODO: Can be None (see interface.screen.parameter.NewForParameter). But can it
-        #     really be missing_required_value_t? If yes, comment how.
-        if (value is None) or (value is MISSING_REQUIRED_VALUE):
+        if value is None:
             value = True
 
-        annotation = value_type.FirstAnnotationWithAttribute("mode")
-        if annotation is None:
+        if value_type is None:
             labels = None
         else:
-            labels = getattr(annotation.mode, "value", None)
+            if isinstance(value_type, type_t):
+                annotation = value_type.FirstAnnotationWithAttribute("mode")
+            else:
+                annotation = value_type
+            if annotation is None:
+                labels = None
+            else:
+                labels = getattr(annotation.mode, "value", None)
         if labels is None:
             labels = ("True!", "False!")
 
-        true_btn = choices_dots_wgt_t(labels[0], parent=output)
-        false_btn = choices_dots_wgt_t(labels[1], parent=output)
+        true_btn = backend.dot_button_wgt_t(labels[0], parent=output.library_wgt)
+        false_btn = backend.dot_button_wgt_t(labels[1], parent=output.library_wgt)
         true_btn.setChecked(value)
         false_btn.setChecked(not value)
 
         output.true_btn = true_btn
 
-        layout = hbox_lyt_t()
+        layout = backend.hbox_lyt_t()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(true_btn)
         layout.addWidget(false_btn)
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
 
         return output
 
     def Text(self) -> str:
         """"""
-        return str(self.Value())
-
-    def Value(self) -> bool:
-        """"""
-        return self.true_btn.isChecked()
+        return str(self.true_btn.isChecked())
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/choices.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/choices.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,60 +25,39 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
+import dataclasses as dtcl
+from typing import Annotated, Sequence
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
-    choices_list_wgt_t,
-)
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import missing_required_value_t
+from conf_ini_g.extension.type import annotated_hint_t
+from conf_ini_g.specification.parameter.annotation import annotation_t
 
 
-class choices_wgt_t(choices_list_wgt_t):
-    """"""
+@dtcl.dataclass(repr=False, eq=False)
+class choices_t(annotation_t):
+    options: Sequence[str] = None
 
     @classmethod
-    def NewWithDetails(
-        cls,
-        value: str | None | missing_required_value_t,
-        value_type: type_t,
-        _: parameter_t | None,
-    ) -> choices_wgt_t:
-        """
-        If value_type does not contain the necessary details, the initial value (if valid) is the only choice, or a unique
-        default choice ending with an exclamation point is added.
-        """
-        output = cls()
-
-        value_is_valid = isinstance(value, str)
-        if value_is_valid:
-            value = value.strip()
-
-        annotation = value_type.FirstAnnotationWithAttribute("options")
-        if annotation is None:
-            if value_is_valid:
-                choices = (value,)
-            else:
-                choices = ("Default!",)
-        else:
-            choices = annotation.options
-
-        for choice in choices:
-            output.addItem(choice)
-        if value_is_valid:
-            output.setCurrentText(value)
-        else:
-            output.setCurrentIndex(0)
+    def NewAnnotatedType(cls, options: Sequence[str], /) -> annotated_hint_t:
+        """"""
+        return Annotated[str, cls(tuple(options))]
+
+    def Issues(self) -> list[str]:
+        """"""
+        output = []
+
+        for option in self.options:
+            if not isinstance(option, str):
+                output.append(
+                    f"{type(option).__name__}: Invalid type of option {option} "
+                    f"in {self}; Expected=str"
+                )
 
         return output
 
-    def Value(self) -> str:
-        """
-        Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
-        """
-        return self.Text()
+    def ValueIsCompliant(self, value: str, /) -> bool:
+        """"""
+        return value in self.options
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/none.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/none.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,31 +27,29 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
+import dataclasses as dtcl
 from typing import Any
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import label_wgt_t
+from conf_ini_g.interface.screen.backend import backend_t, label_wgt_h
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import missing_required_value_t
 
 
-class none_wgt_t(label_wgt_t):
-    """"""
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class none_wgt_t:
+    library_wgt: label_wgt_h
 
     @classmethod
     def NewWithDetails(
-        cls,
-        _: Any | None | missing_required_value_t,
-        __: type_t,
-        ___: parameter_t,
-    ) -> label_wgt_t:
+        cls, _: Any, __: type_t | None, backend: backend_t, ___: parameter_t | None, /
+    ) -> none_wgt_t:
         """"""
-        return cls("None")
+        return cls(library_wgt=backend.label_wgt_t("None"))
 
-    def Value(self) -> None:
+    def Text(self) -> str:
         """"""
-        return None
+        return "None"
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/path.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,133 +27,142 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from typing import Callable
+import dataclasses as dtcl
+from pathlib import Path as pl_path_t
 
-import conf_ini_g.interface.screen.parameter.path_chooser as fd_
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.button import button_wgt_t
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
-    hbox_lyt_t,
-    library_wgt_t,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
 from conf_ini_g.catalog.specification.parameter.path import path_t
+from conf_ini_g.interface.screen.backend import backend_t, library_wgt_h, text_wgt_h
+from conf_ini_g.interface.screen.parameter.path_chooser import (
+    NewSelectedInputDocument,
+    NewSelectedOutputDocument,
+    document_selection_fct_h,
+)
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import (
-    MISSING_REQUIRED_VALUE,
-    missing_required_value_t,
-)
-from conf_ini_g.standard.path_extension import path_t as pl_path_t
-
 
-class path_wgt_t(library_wgt_t):
-    __slots__ = (
-        "target_type",
-        "path",
-        "SelectedFile",
-    )
-    target_type: path_t.TARGET_TYPE
-    path: text_wgt_t
-    SelectedFile: Callable[..., pl_path_t | None]
+PATH_SELECTOR_WIDTH = 100
 
-    def __init__(self, parent: library_wgt_t = None) -> None:
-        """"""
-        super().__init__(parent=parent)
 
-        # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
-        for slot in path_wgt_t.__slots__:
-            setattr(self, slot, None)
+@dtcl.dataclass(repr=False, eq=False)
+class path_wgt_t:
+    """
+    Cannot use slots (weak reference issue).
+    """
+
+    library_wgt: library_wgt_h
+    backend: backend_t
+    target_type: path_t.TARGET_TYPE = dtcl.field(init=False, default=None)
+    path: text_wgt_h = dtcl.field(init=False, default=None)
+    _NewSelectedDocument: document_selection_fct_h = dtcl.field(
+        init=False, default=None
+    )
 
     @classmethod
     def NewWithDetails(
         cls,
-        value: pl_path_t | None | missing_required_value_t,
-        value_type: type_t,
-        _: parameter_t,
+        value: pl_path_t | None,
+        value_type: type_t | path_t | None,
+        backend: backend_t,
+        _: parameter_t | None,
+        /,
+        *,
+        editable: bool = True,
     ) -> path_wgt_t:
         """
         If value_type does not contain the necessary details, the target type is set to any and considered as input, and
         the selection button label ends with an exclamation point.
         """
-        output = cls()
+        output = cls(library_wgt=backend.library_wgt_t(), backend=backend)
 
-        if (value is None) or (value is MISSING_REQUIRED_VALUE):
+        if value is None:
             value = ""
         else:
             value = str(value)
 
-        annotation = value_type.FirstAnnotationWithAttribute(
-            ("target_type", "is_input")
-        )
-        if annotation is None:
-            target_type = path_t.TARGET_TYPE.any
-            is_input = True
-            misses_details = True
-        else:
-            target_type = annotation.target_type
-            is_input = annotation.is_input
-            misses_details = False
+        default_parameters = (path_t.TARGET_TYPE.any, True, True)
+        if value_type is None:
+            target_type, is_input, misses_details = default_parameters
+        else:
+            if isinstance(value_type, type_t):
+                annotation = value_type.FirstAnnotationWithAttribute(
+                    ("target_type", "is_input")
+                )
+            else:
+                annotation = value_type
+            if annotation is None:
+                target_type, is_input, misses_details = default_parameters
+            else:
+                target_type = annotation.target_type
+                is_input = annotation.is_input
+                misses_details = False
 
         output.target_type = target_type
         if is_input:
-            output.SelectedFile = fd_.SelectedInputFile
+            output._NewSelectedDocument = NewSelectedInputDocument
         else:
-            output.SelectedFile = fd_.SelectedOutputFile
+            output._NewSelectedDocument = NewSelectedOutputDocument
 
-        selector_label = "..."
+        if target_type is path_t.TARGET_TYPE.document:
+            target_type_icon = "🗋"
+        elif target_type is path_t.TARGET_TYPE.folder:
+            target_type_icon = "📂"
+        else:
+            target_type_icon = "📂🗋"
+        if is_input:
+            selector_color = "green"
+        else:
+            selector_color = "red"
+        selector_label = f"...{target_type_icon}..."
         if misses_details:
             selector_label += "!"
-        path = text_wgt_t(value, parent=output)
-        path_selector = button_wgt_t(selector_label, parent=output)
+        if editable:
+            path = backend.text_wgt_t(value, parent=output.library_wgt)
+        else:
+            path = backend.label_wgt_t(value, parent=output.library_wgt)
+        path_selector = backend.button_wgt_t(selector_label, parent=output.library_wgt)
         path_selector.SetFunction(output.SelectDocument)
 
         output.path = path
 
-        path_selector.setFixedWidth(30)
+        path_selector.setStyleSheet(f"color: {selector_color};")
+        path_selector.setFixedWidth(PATH_SELECTOR_WIDTH)
 
-        layout = hbox_lyt_t()
+        layout = backend.hbox_lyt_t()
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(path)
         layout.addWidget(path_selector)
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
 
         return output
 
     def Text(self) -> str:
         """"""
         return self.path.Text()
 
-    def Value(self) -> pl_path_t | None:
-        """"""
-        text = self.Text()
-        if text.__len__() > 0:
-            return pl_path_t(text)
-
-        return None
-
     def SelectDocument(self) -> None:
         """"""
         current_path = self.Text()
         current_doc = pl_path_t(current_path).resolve()
 
         if self.target_type is path_t.TARGET_TYPE.document:
             title = "Select File"
         elif self.target_type is path_t.TARGET_TYPE.folder:
             title = "Select Folder"
         else:
             title = "Select File or Folder"
 
-        selection = self.SelectedFile(
+        selection = self._NewSelectedDocument(
             title,
             title,
+            self.backend,
             mode=self.target_type,
             start_folder=current_doc.parent,
             initial_selection=current_doc,
         )
         if selection is None:
             return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/sequence.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,84 +27,87 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
+import dataclasses as dtcl
 from typing import ClassVar, Sequence
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
-    choices_list_wgt_t,
+from conf_ini_g.catalog.specification.parameter.sequence import sequence_t
+from conf_ini_g.catalog.specification.parameter.sequence import (
+    sequence_t as sequence_annotation_t,
 )
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
-    hbox_lyt_t,
-    library_wgt_t,
+from conf_ini_g.interface.screen.backend import (
+    backend_t,
+    choices_list_wgt_h,
+    library_wgt_h,
+    text_wgt_h,
 )
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
-from conf_ini_g.catalog.specification.parameter.sequence import sequence_t
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import (
-    MISSING_REQUIRED_VALUE,
-    missing_required_value_t,
-)
 
 
-class sequence_wgt_t(library_wgt_t):
+@dtcl.dataclass(repr=False, eq=False)
+class sequence_wgt_t:
+    """
+    Cannot use slots (weak reference issue).
+    """
+
     ENTRY_ANY: ClassVar[str] = "any"
     ENTRIES: ClassVar[tuple[str, ...]] = ("2", "3", "4", "5", "6", ENTRY_ANY)
 
-    __slots__ = ("length_selector", "components")
-    length_selector: choices_list_wgt_t
-    components: tuple[text_wgt_t, ...]
-
-    def __init__(self, parent: library_wgt_t = None):
-        """"""
-        super().__init__(parent=parent)
-
-        # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
-        for slot in sequence_wgt_t.__slots__:
-            setattr(self, slot, None)
+    library_wgt: library_wgt_h
+    length_selector: choices_list_wgt_h = dtcl.field(init=False, default=None)
+    components: tuple[text_wgt_h, ...] = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewWithDetails(
         cls,
-        value: tuple | None | missing_required_value_t,
-        value_type: type_t,
-        _: parameter_t,
+        value: tuple | None,
+        value_type: type_t | sequence_annotation_t | None,
+        backend: backend_t,
+        _: parameter_t | None,
+        /,
     ) -> sequence_wgt_t:
         """
         If value_type does not contain the necessary details, a simple free-text input widget is used. If the value is not
         coherent with the details (which should not happen if value_type contains the necessary details and the value has
         been validated), a choice with the length of the value is added, with an exclamation point.
         """
-        output = cls()
+        output = cls(library_wgt=backend.library_wgt_t())
 
-        if (value is None) or (value is MISSING_REQUIRED_VALUE):
+        if value is None:
             value = ()
         length = value.__len__()
 
-        annotation = value_type.FirstAnnotationWithAttribute("lengths")
-        if annotation is None:
-            entries = cls.ENTRIES
-            max_entry = int(entries[-2])
-        elif (lengths := annotation.lengths) == sequence_t.ANY_LENGTH:
-            entries = (cls.ENTRY_ANY,)
-            max_entry = None
+        default_parameters = (cls.ENTRIES, int(cls.ENTRIES[-2]))
+        if value_type is None:
+            entries, max_entry = default_parameters
         else:
-            entries = tuple(str(_lgh) for _lgh in lengths)
-            max_entry = lengths[-1]
-            if (length > 0) and (str(length) not in entries):
-                # This should never happen since the value must have been validated
-                entries = entries + (str(length) + "!",)
-                max_entry = max(max_entry, length)
+            if isinstance(value_type, type_t):
+                annotation = value_type.FirstAnnotationWithAttribute("lengths")
+            else:
+                annotation = value_type
+            if annotation is None:
+                entries, max_entry = default_parameters
+            elif (lengths := annotation.lengths) == sequence_t.ANY_LENGTH:
+                entries = (cls.ENTRY_ANY,)
+                max_entry = None
+            else:
+                entries = tuple(str(_lgh) for _lgh in lengths)
+                max_entry = lengths[-1]
+                if (length > 0) and (str(length) not in entries):
+                    # This should never happen since the value must have been validated
+                    entries = entries + (str(length) + "!",)
+                    max_entry = max(max_entry, length)
 
         if entries.__len__() > 1:
-            length_selector = choices_list_wgt_t()
+            length_selector = backend.choice_menu_wgt_t()
             for entry in entries:
                 length_selector.addItem(entry)
 
             if (length_as_str := str(length)) in entries:
                 length_selector.setCurrentText(length_as_str)
             if length_as_str + "!" in entries:
                 length_selector.setCurrentText(length_as_str + "!")
@@ -113,33 +116,33 @@
 
             output.length_selector = length_selector
             output.length_selector.SetFunction(output.SetLength)
 
         components = []
         if max_entry is None:
             value_as_str = str(value)[1:-1] if length > 0 else ""
-            widget = text_wgt_t(value_as_str, parent=None)
+            widget = backend.text_wgt_t(value_as_str, parent=None)
             components.append(widget)
         else:
             for e_idx in range(max_entry):
                 value_as_str = str(value[e_idx]) if e_idx < length else ""
-                widget = text_wgt_t(value_as_str, parent=None)
+                widget = backend.text_wgt_t(value_as_str, parent=None)
                 if e_idx >= length:
                     widget.setVisible(False)
                     widget.setEnabled(False)
                 components.append(widget)
         output.components = tuple(components)
 
-        layout = hbox_lyt_t()
+        layout = backend.hbox_lyt_t()
         layout.setContentsMargins(0, 0, 0, 0)
         if output.length_selector is not None:
             layout.addWidget(output.length_selector)
         for component in output.components:
             layout.addWidget(component)
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
 
         return output
 
     def SetLength(self, new_index: int) -> None:
         """"""
         new_length = self.length_selector.ItemAt(new_index)
         if new_length == self.__class__.ENTRY_ANY:
@@ -167,24 +170,17 @@
         if contents.__len__() == 0:
             return "()"
         elif contents.__len__() == 1:
             return "(" + contents[0] + ",)"
         else:
             return "(" + ", ".join(contents) + ")"
 
-    def Value(self) -> str:
-        """
-        Value cannot return a true value since there is no indication of the sequence elements type
-        Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
-        """
-        return self.Text()
-
 
 def _AdjustComponents(
-    components: Sequence[text_wgt_t, ...],
+    components: Sequence[text_wgt_h, ...],
     length: int,
 ) -> None:
     """"""
     for c_idx, component in enumerate(components):
         if c_idx < length:
             component.setVisible(True)
             component.setEnabled(True)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/interface/screen/parameter/text.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/parameter/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,44 +27,42 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
+import dataclasses as dtcl
 from typing import Any
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.text import text_wgt_t
+from conf_ini_g.interface.screen.backend import backend_t, text_wgt_h
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.specification.parameter.value import (
-    MISSING_REQUIRED_VALUE,
-    missing_required_value_t,
-)
 
 
-class default_entry_wgt_t(text_wgt_t):
-    """"""
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class default_entry_wgt_t:
+    library_wgt: text_wgt_h
 
     @classmethod
     def NewWithDetails(
         cls,
-        value: Any | None | missing_required_value_t,
-        _: type_t,
-        __: parameter_t,
+        value: Any | None,
+        _: type_t | None,
+        backend: backend_t,
+        __: parameter_t | None,
+        /,
     ) -> default_entry_wgt_t:
         """"""
-        output = cls()
+        output = cls(library_wgt=backend.text_wgt_t())
 
-        if (value is None) or (value is MISSING_REQUIRED_VALUE):
+        if value is None:
             value = ""
         else:
             value = str(value)
-        output.setText(value)
+        output.library_wgt.setText(value)
 
         return output
 
-    def Value(self) -> str:
-        """
-        Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
-        """
-        return self.Text()
+    def Text(self) -> str:
+        """"""
+        return self.library_wgt.Text()
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/boolean.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/boolean.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,35 +27,30 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from enum import Enum as enum_t
-from typing import Annotated, ClassVar
+from typing import Annotated
 
-from conf_ini_g.specification.parameter.annotation import (
-    annotation_t,
-    py_type_options_h,
-)
-from conf_ini_g.standard.type_extension import annotated_hint_t
+from conf_ini_g.extension.type import annotated_hint_t
+from conf_ini_g.specification.parameter.annotation import annotation_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class boolean_t(annotation_t):
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = bool
-
     class MODE(enum_t):
         # Always list true value first
         true_false = ("True", "False")
         yes_no = ("Yes", "No")
         on_off = ("On", "Off")
 
     mode: enum_t = MODE.true_false
 
     @classmethod
     def NewAnnotatedType(cls, mode: enum_t = None) -> annotated_hint_t:
         """"""
         if mode is None:
             mode = cls.MODE.true_false
 
-        return Annotated[cls.VALID_PY_TYPES, cls(mode=mode)]
+        return Annotated[bool, cls(mode=mode)]
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/choices.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,44 +25,27 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
-from typing import Annotated, ClassVar, Sequence
+from typing import Callable
 
-from conf_ini_g.specification.parameter.annotation import (
-    annotation_t,
-    py_type_options_h,
-)
-from conf_ini_g.standard.type_extension import annotated_hint_t
+import PyQt6.QtWidgets as wdgt
 
 
-@dtcl.dataclass(repr=False, eq=False)
-class choices_t(annotation_t):
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = str
+class choice_menu_wgt_t(wdgt.QComboBox):
+    """"""
 
-    options: Sequence[str] = None
-
-    @classmethod
-    def NewAnnotatedType(cls, options: Sequence[str], /) -> annotated_hint_t:
+    def Text(self) -> str:
         """"""
-        return Annotated[cls.VALID_PY_TYPES, cls(tuple(options))]
+        return self.currentText()
 
-    def Issues(self, py_type: type, /) -> list[str]:
+    def ItemAt(self, index: int, /) -> str:
         """"""
-        output = super().Issues(py_type)
-
-        for option in self.options:
-            if not isinstance(option, str):
-                output.append(
-                    f"{type(option).__name__}: Invalid type of option {option} "
-                    f"in {self}; Expected=str"
-                )
-
-        return output
+        return self.itemText(index)
 
-    def ValueIsCompliant(self, value: str, /) -> bool:
+    def SetFunction(self, function: Callable, /) -> None:
         """"""
-        return value in self.options
+        self.activated.connect(function)
+        # OR: self.currentTextChanged.connect(function)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/number.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/number.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,68 +28,65 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from typing import Annotated, ClassVar
 
-from conf_ini_g.specification.parameter.annotation import (
-    annotation_t,
-    py_type_options_h,
-)
-from conf_ini_g.standard.type_extension import annotated_hint_t
-
+from conf_ini_g.extension.type import annotated_hint_t
+from conf_ini_g.specification.parameter.annotation import annotation_t
 
 number_h = int | float
 
 
 @dtcl.dataclass(repr=False, eq=False)
 class number_t(annotation_t):
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = number_h.__args__
     INFINITY_NEG: ClassVar[float] = -float("inf")
     INFINITY_POS: ClassVar[float] = float("inf")
     INFINITE_PRECISION: ClassVar[float] = 0.0
 
     min: number_h = INFINITY_NEG
     max: number_h = INFINITY_POS
     min_inclusive: bool = True
     max_inclusive: bool = True
     precision: number_h = INFINITE_PRECISION
 
     @classmethod
     def NewAnnotatedType(cls, py_type: type, /, **kwargs) -> annotated_hint_t:
         """"""
-        if py_type in cls.VALID_PY_TYPES:
+        if py_type in (int, float):
             return Annotated[py_type, cls(**kwargs)]
 
-        raise TypeError(
-            f"{py_type}: Invalid Python type; " f"Expected={cls.VALID_PY_TYPES}."
-        )
+        raise TypeError(f"{py_type}: Invalid Python type; " f"Expected=int or float.")
 
-    def Issues(self, py_type: type, /) -> list[str]:
+    def Issues(self) -> list[str]:
         """"""
-        output = super().Issues(py_type)
+        output = []
 
         self_class = self.__class__
-        if (self.min != self_class.INFINITY_NEG) and not isinstance(self.min, py_type):
+        if (self.min != self_class.INFINITY_NEG) and not isinstance(
+            self.min, number_h.__args__
+        ):
             output.append(
                 f"{type(self.min)}: Invalid type for min value {self.min} "
-                f"in {self}; Expected={py_type}"
+                f"in {self}; Expected={number_h}"
             )
-        if (self.max != self_class.INFINITY_POS) and not isinstance(self.max, py_type):
+        if (self.max != self_class.INFINITY_POS) and not isinstance(
+            self.max, number_h.__args__
+        ):
             output.append(
                 f"{type(self.max)}: Invalid type for max value {self.max} "
-                f"in {self}; Expected={py_type}"
+                f"in {self}; Expected={number_h}"
             )
         if (self.precision != self_class.INFINITE_PRECISION) and not isinstance(
-            self.precision, py_type
+            self.precision, number_h.__args__
         ):
             output.append(
                 f"{type(self.precision)}: Invalid type for precision {self.precision} "
-                f"in {self}; Expected={py_type}"
+                f"in {self}; Expected={number_h}"
             )
         if self.precision < 0:
             output.append(f"{self.precision}: Negative precision in {self}")
         if (self.min > self.max) or (
             (self.min == self.max) and not (self.min_inclusive and self.max_inclusive)
         ):
             if self.min_inclusive:
@@ -118,26 +115,7 @@
                 self.precision * int(value / self.precision) != value
             ):
                 return False
 
             return True
         else:
             return False
-
-
-@dtcl.dataclass(repr=False, eq=False)
-class number_in_str_t(annotation_t):
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = str
-
-    @classmethod
-    def NewAnnotatedType(cls) -> annotated_hint_t:
-        """"""
-        return Annotated[cls.VALID_PY_TYPES, cls()]
-
-    def ValueIsCompliant(self, value: str, /) -> bool:
-        """"""
-        try:
-            _ = float(value)
-        except ValueError:
-            return False
-
-        return True
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/path.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/path.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,42 +27,52 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from enum import Enum as enum_t
-from typing import Annotated, ClassVar
+from pathlib import Path as pl_path_t
+from typing import Annotated
 
-from conf_ini_g.specification.parameter.annotation import (
-    annotation_t,
-    py_type_options_h,
-)
-from conf_ini_g.standard.path_extension import path_t as pl_path_t
-from conf_ini_g.standard.type_extension import annotated_hint_t
+from conf_ini_g.extension.type import annotated_hint_t
+from conf_ini_g.specification.parameter.annotation import annotation_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class path_t(annotation_t):
     """
     Existence and target type validation are left to main program. Hence, ValueIsCompliant
     is not overriden.
     """
 
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = pl_path_t
-
     class TARGET_TYPE(enum_t):
         document = 1
         folder = 2
         any = 3
 
     target_type: enum_t
     is_input: bool
 
     @classmethod
     def NewAnnotatedType(
         cls, target_type: TARGET_TYPE, is_input: bool, /
     ) -> annotated_hint_t:
         """"""
-        return Annotated[
-            cls.VALID_PY_TYPES, cls(target_type=target_type, is_input=is_input)
-        ]
+        return Annotated[pl_path_t, cls(target_type=target_type, is_input=is_input)]
+
+    def ValueIsCompliant(self, value: pl_path_t | None, /) -> bool:
+        """"""
+        if not self.is_input:
+            return True
+
+        if (value is not None) and value.exists():
+            if self.target_type is path_t.TARGET_TYPE.any:
+                return value.is_file() or value.is_dir()
+
+            if (self.target_type is path_t.TARGET_TYPE.document) and value.is_file():
+                return True
+
+            if (self.target_type is path_t.TARGET_TYPE.folder) and value.is_dir():
+                return True
+
+        return False
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/catalog/specification/parameter/sequence.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/specification/parameter/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,92 +26,89 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Annotated, Any, ClassVar
+from typing import Annotated, Any, ClassVar, Sequence
 
-from conf_ini_g.specification.parameter.annotation import (
-    annotation_t,
-    py_type_options_h,
-)
-from conf_ini_g.standard.type_extension import annotated_hint_t
+from conf_ini_g.extension.type import annotated_hint_t, any_hint_h
+from conf_ini_g.specification.parameter.annotation import annotation_t
+from conf_ini_g.specification.parameter.type import type_t
 
 
 @dtcl.dataclass(repr=False, eq=False)
 class sequence_t(annotation_t):
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = tuple
-    ANY_LENGTH: ClassVar[tuple[int]] = (0,)
+    ANY_ITEMS_TYPES: ClassVar[tuple[Any, ...]] = Any
+    ANY_LENGTH: ClassVar[tuple[int, ...]] = (0,)
 
     # Any=Value of any type but None
-    items_types: type | tuple[type | None, ...] = (None, Any)
-    lengths: tuple[int, ...] = ANY_LENGTH
+    items_types: any_hint_h | tuple[any_hint_h, ...] | type_t | tuple[
+        type_t, ...
+    ] = ANY_ITEMS_TYPES
+    lengths: int | tuple[int, ...] = ANY_LENGTH
 
     def __post_init__(self):
         """"""
-        # TODO: Convert every type to annotated type (works with Any b.t.w), maybe.
-        #     However, there currently is a problem of circular import.
-        if (self.items_types is Any) or isinstance(self.items_types, type):
-            self.items_types = (self.items_types,)
+        if isinstance(self.items_types, Sequence):
+            self.items_types = tuple(
+                type_t.NewFromType(_typ) for _typ in self.items_types
+            )
+        else:
+            self.items_types = type_t.NewFromType(self.items_types)
+
         if isinstance(self.lengths, int):
             self.lengths = (self.lengths,)
         else:
             self.lengths = tuple(sorted(self.lengths))
 
     @classmethod
     def NewAnnotatedType(
         cls,
-        items_types: type | tuple[type | None, ...] = (None, Any),
+        sequence_type: type,
+        items_types: any_hint_h | tuple[any_hint_h | None, ...] = ANY_ITEMS_TYPES,
         lengths: tuple[int, ...] = ANY_LENGTH,
     ) -> annotated_hint_t:
         """"""
-        return Annotated[
-            cls.VALID_PY_TYPES, cls(items_types=items_types, lengths=lengths)
-        ]
+        if sequence_type in (list, set, tuple):
+            return Annotated[
+                sequence_type, cls(items_types=items_types, lengths=lengths)
+            ]
+
+        raise ValueError(
+            f"{sequence_type.__name__}: Invalid sequence type; "
+            f"Expected=list, set or tuple."
+        )
 
-    def Issues(self, py_type: type, /) -> list[str]:
+    def Issues(self) -> list[str]:
         """"""
-        output = super().Issues(py_type)
+        output = []
 
-        self_class = self.__class__
-        if all(_typ is None for _typ in self.items_types):
-            output.append(f'{self}: Contents types restricted to "None" for parameter')
-
-        for content_type in self.items_types:
-            if not (
-                (content_type is None)
-                or (content_type is Any)
-                or isinstance(content_type, type)
-            ):
-                output.append(
-                    f"{content_type}: Invalid item type in {self}; Expected=None, typing.Any, Python types"
-                )
-        if self.lengths != self_class.ANY_LENGTH:
+        if self.lengths != self.__class__.ANY_LENGTH:
             for length in self.lengths:
                 if (not isinstance(length, int)) or (length <= 0):
                     output.append(
-                        f"{length}: Invalid sequence length in {self}; Expected=strictly positive integer"
+                        f"{length}: Invalid sequence length in {self}; "
+                        f"Expected=strictly positive integer"
                     )
 
         return output
 
     def ValueIsCompliant(self, value: tuple, /) -> bool:
         """"""
         if (self.lengths != self.__class__.ANY_LENGTH) and (
             value.__len__() not in self.lengths
         ):
             return False
 
-        none_not_allowed = None not in self.items_types
-        any_not_present = Any not in self.items_types
-        # If empty, isinstance(element, types_wo_none) returns False; But cannot be empty (see Issues).
-        types_wo_none = tuple(_typ for _typ in self.items_types if _typ is not None)
-        for element in value:
-            if element is None:
-                if none_not_allowed:
-                    return False
-            elif any_not_present and not isinstance(element, types_wo_none):
+        if isinstance(self.items_types, Sequence):
+            if value.__len__() > self.items_types.__len__():
                 return False
 
-        return True
+            return all(
+                _typ.ValueIsCompliant(_elm)
+                for _typ, _elm in zip(self.items_types, value)
+            )
+
+        type_ = self.items_types
+        return all(type_.ValueIsCompliant(_elm) for _elm in value)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/instance/config.py` & `conf-ini-g-2023.6/conf_ini_g/instance/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,29 @@
 
 import dataclasses as dtcl
 import textwrap as text
 from typing import Any, Sequence
 
 from rich.text import Text as text_t
 
+from conf_ini_g.extension.path import any_path_h, path_t
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.extension.type import TypeAsRichStr
 from conf_ini_g.instance.parameter.main import instance_t
 from conf_ini_g.instance.parameter.unit import unit_instance_t
 from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
 from conf_ini_g.raw.config import ini_config_h, raw_config_h
 from conf_ini_g.specification.config import config_t as specification_t
 from conf_ini_g.specification.parameter.unit import STD_UNIT_CONVERSIONS, unit_t
+from conf_ini_g.specification.parameter.value import MISSING_REQUIRED_VALUE
 from conf_ini_g.specification.section.main import controller_t
 from conf_ini_g.specification.section.unit import UNIT_SECTION, IsUnitSection
-from conf_ini_g.standard.path_extension import any_path_h, path_t
-from conf_ini_g.standard.str_extension import AlignedOnSeparator
-from conf_ini_g.standard.type_extension import TypeAsRichStr
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class config_t(dict[str, dict[str, instance_t | unit_instance_t]]):
     specification: specification_t
     ini_path: path_t | None = None
 
     @classmethod
     def NewFromINIConfig(
         cls,
@@ -67,15 +68,15 @@
         """"""
         config = cls(specification=specification)
 
         if path is not None:
             config.ini_path = path_t(path)
 
         issues, for_deferred_check = config._InstantiateFromINIConfig(ini_config)
-        config._AddDefaults()
+        config._ManageDefaults()
 
         return config, issues, for_deferred_check
 
     def _InstantiateFromINIConfig(
         self, ini_config: ini_config_h, /
     ) -> tuple[list[str], Sequence[tuple[str, str]]]:
         """"""
@@ -106,78 +107,86 @@
                             f"parameter to a section accepting none."
                         )
                     if parameter_spec is not None:
                         if isinstance(parameter_spec, unit_t):
                             instance = unit_instance_t()
                         else:
                             instance = instance_t()
-                        instance.SetValue(
-                            value, INI_COMMENT_MARKER, parameter_spec.types
-                        )
+                        instance.SetStrValue(value, INI_COMMENT_MARKER)
                         self[section_name][name] = instance
             elif IsUnitSection(section_name, possibly_fuzzy=True):
                 issues.append(
                     f"{section_name}: Unit section must respect the following case "
                     f'"{UNIT_SECTION}".'
                 )
             else:
                 issues.append(
                     f"{section_name}: Invalid section; "
                     f"Expected={self.specification.section_names}."
                 )
 
         return issues, for_deferred_check
 
-    def _AddDefaults(self) -> None:
+    def _ManageDefaults(self) -> None:
         """"""
         for section_spec in self.specification:
             # Leave here, otherwise parameter_spec.name not in self[section_spec.name]
             # below might fail.
             if section_spec.name not in self:
                 self[section_spec.name] = {}
 
             for parameter_spec in section_spec.all_parameters:
-                if parameter_spec.optional and (
-                    parameter_spec.name not in self[section_spec.name]
-                ):
-                    instance = instance_t()
-                    instance.SetDefaultValue(parameter_spec)
-                    self[section_spec.name][parameter_spec.name] = instance
+                if parameter_spec.name not in self[section_spec.name]:
+                    if parameter_spec.optional:
+                        instance = instance_t(value=parameter_spec.default)
+                        self[section_spec.name][parameter_spec.name] = instance
+                    else:
+                        self[section_spec.name][
+                            parameter_spec.name
+                        ] = MISSING_REQUIRED_VALUE
 
     def GetValueOfController(self, controller: controller_t, /) -> Any:
         """"""
         return self[controller.section][controller.parameter].value
 
     def AsRawConfig(self) -> tuple[raw_config_h, list[str]]:
         """
         Units are interpreted
         """
         raw_config = {}
         issues = []
 
         unit_conversions = dict(STD_UNIT_CONVERSIONS)
         if UNIT_SECTION in self.specification:
-            unit_conversions.update(
-                {
-                    _prm.name: self[UNIT_SECTION][_prm.name].value
-                    for _prm in self.specification[UNIT_SECTION]
-                }
-            )
+            for unit_spec in self.specification[UNIT_SECTION]:
+                unit_name = unit_spec.name
+                expected_type = unit_spec.type
+                instance = self[UNIT_SECTION][unit_name]
+                if instance is MISSING_REQUIRED_VALUE:
+                    issues.append(f"{unit_name}: Missing required unit.")
+                else:
+                    unit_conversions[unit_name] = instance.TypedValue(expected_type)[0]
 
         for section_spec in self.specification:
             raw_section = {}
 
             if (controller := section_spec.controller) is None:
                 parameters = section_spec
             else:
                 controller_value = self[controller.section][controller.parameter].value
                 parameters = section_spec.ActiveParameters(controller_value)
             for parameter_spec in parameters:
                 instance = self[section_spec.name][parameter_spec.name]
-                value, current_issues = instance.FinalValue(unit_conversions)
+                if instance is MISSING_REQUIRED_VALUE:
+                    value = None
+                    current_issues = ["Missing required parameter."]
+                else:
+                    value, current_issues = instance.TypedValue(
+                        parameter_spec.type, units=unit_conversions
+                    )
 
                 if current_issues.__len__() > 0:
                     issues.extend(
                         f"[{section_spec.name}.{parameter_spec.name}] {_iss}"
                         for _iss in current_issues
                     )
                 else:
@@ -241,21 +250,23 @@
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
         output = [
+            "[grey50]--- Specification[/]",
             TypeAsRichStr(self),
             f"    [blue]ini_path[/]={self.ini_path}"
             f"[yellow]:{type(self.ini_path).__name__}[/]",
             text.indent(self.specification.__rich__(), "    "),
+            "[grey50]--- Instance[/]",
         ]
 
         for section_name, section in self.items():
-            output.append(f"    {section_name}:")
+            output.append(f"{section_name}:")
             for parameter_name, parameter in section.items():
-                output.append(f"        {parameter_name}@:@{parameter.__rich__()}")
+                output.append(f"    {parameter_name}@:@{parameter.__rich__()}")
 
         output = AlignedOnSeparator(output, "@:@", ": ")
 
         return "\n".join(output)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/instance/parameter/base.py` & `conf-ini-g-2023.6/conf_ini_g/instance/parameter/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,62 +32,65 @@
 import dataclasses as dtcl
 from abc import ABC as abstract_class_t
 from abc import abstractmethod
 from typing import Any
 
 from rich.text import Text as text_t
 
-from conf_ini_g.specification.parameter.type import type_options_t, type_t
-from conf_ini_g.specification.parameter.value import INVALID_VALUE
+from conf_ini_g.specification.parameter.type import type_t
+from conf_ini_g.specification.parameter.value import INVALID_VALUE, invalid_value_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class base_t(abstract_class_t):
-    type: type_t = None
-    value: Any = None
+    value: str = None  # From INI document or interfaces
     comment: str = None
 
     @abstractmethod
-    def SetValue(
+    def SetStrValue(
         self,
         value_w_unit_w_comment: str | Any,
         comment_marker: str,
-        type_options: type_options_t | None,
         /,
         *,
         unit: str = None,
     ) -> None:
         """"""
         ...
 
     @abstractmethod
+    def TypedValue(
+        self,
+        expected_type: type_t,
+        /,
+        *,
+        units: dict[str, int | float | invalid_value_t] = None,
+    ) -> tuple[Any, list[str]]:
+        """"""
+        ...
+
+    @abstractmethod
     def Text(self) -> str:
         """"""
         ...
 
     def Issues(self) -> list[str]:
         """"""
         if self.value is INVALID_VALUE:
-            return [f"No matching type in specification or invalid value"]
+            return ["Invalid value"]
 
         return []
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
-        if self.type is None:
-            return f"[blue]{type(self).__name__}[/]={self.Text()}"
-
-        return (
-            f"[blue]{type(self).__name__}[/]={self.Text()}"
-            f"[yellow]:{self.type.py_type.__name__}[/]"
-        )
+        return self.Text()
 
 
 def Pieces(
     combined: str, separator: str, /, *, from_left: bool = True
 ) -> tuple[str, str | None]:
     """"""
     if from_left:
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/instance/parameter/main.py` & `conf-ini-g-2023.6/conf_ini_g/instance/parameter/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,107 +30,81 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from typing import Any
 
 from conf_ini_g.instance.parameter.base import Pieces, base_t
 from conf_ini_g.instance.parameter.unit import ConvertedValue
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_options_t, type_t
+from conf_ini_g.specification.parameter.type import type_t
 from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
-from conf_ini_g.specification.parameter.value import (
-    INVALID_VALUE,
-    MISSING_REQUIRED_VALUE,
-    invalid_value_t,
-)
+from conf_ini_g.specification.parameter.value import INVALID_VALUE, invalid_value_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class instance_t(base_t):
     unit: str = None
 
-    def SetDefaultValue(self, parameter: parameter_t, /) -> None:
-        """"""
-        value = parameter.default
-        if value is MISSING_REQUIRED_VALUE:
-            default_type = None
-        else:
-            default_type = parameter.types.MatchingTypeOf(value)
-
-        self.type = default_type
-        self.value = value
-
-    def SetValue(
+    def SetStrValue(
         self,
         value_w_unit_w_comment: str | Any,
         comment_marker: str,
-        type_options: type_options_t | None,
         /,
         *,
         unit: str = None,
     ) -> None:
-        """
-        value_w_unit_w_comment: can be an uninterpreted string coming from an INI
-        document, or can be an interpreted value coming from an interface.
-        """
-        if isinstance(value_w_unit_w_comment, str):
-            value_as_str, inline_unit, comment = _ValueUnitAndComment(
-                value_w_unit_w_comment, comment_marker
-            )
-            if unit is None:
-                unit = inline_unit
-        else:
-            value_as_str, comment = value_w_unit_w_comment, None
-
-        if type_options is None:
-            value = value_as_str
-            value_type = type_t.NewFromType(type(value))
-        else:
-            value, value_type = type_options.TypedValueAndType(value_as_str)
-        # Do not consume unit here. It would be "redundant" with its storage in the
-        # "unit" field. Instead, this will be handled by instance.config_t.AsRawConfig.
+        """"""
+        value_as_str, inline_unit, comment = _ValueUnitAndComment(
+            value_w_unit_w_comment, comment_marker
+        )
+        if unit is None:
+            unit = inline_unit
 
-        self.type = value_type
-        self.value = value
+        self.value = value_as_str
         self.unit = unit
         self.comment = comment
 
-    def FinalValue(
-        self, unit_conversions: dict[str, int | float | invalid_value_t] = None
+    def TypedValue(
+        self,
+        expected_type: type_t,
+        /,
+        *,
+        units: dict[str, int | float | invalid_value_t] = None,
     ) -> tuple[Any, list[str]]:
         """
-        Final=with unit consumed.
+        With unit consumed or not.
         """
-        if (value := self.value) is INVALID_VALUE:
-            return INVALID_VALUE, ["Invalid value."]
+        final_value, success = expected_type.InterpretedValueOf(self.value)
 
-        if (unit := self.unit) is None:
-            return value, []
+        if success:
+            if (units is None) or ((unit := self.unit) is None):
+                return final_value, []
+
+            conversion_factor = units.get(unit, None)
+            if conversion_factor is None:
+                return INVALID_VALUE, [f"{unit}: Missing unit definition."]
+            if conversion_factor is INVALID_VALUE:
+                return INVALID_VALUE, [f"{unit}: Invalid unit value."]
+
+            converted, unconverted = ConvertedValue(final_value, conversion_factor)
+            if unconverted.__len__() > 0:
+                unconverted = ", ".join(unconverted)
+                return INVALID_VALUE, [
+                    f"{unconverted}: Value(s) do(es) not support unit conversion."
+                ]
 
-        conversion_factor = unit_conversions[unit]
-        if conversion_factor is INVALID_VALUE:
-            return INVALID_VALUE, ["Invalid unit value."]
-
-        converted, unconverted = ConvertedValue(value, conversion_factor)
-        if unconverted.__len__() > 0:
-            unconverted = ", ".join(unconverted)
-            return INVALID_VALUE, [
-                f"{unconverted}: Value(s) do(es) not support unit conversion."
-            ]
+            return converted, []
 
-        return converted, []
+        return INVALID_VALUE, [f"{self.value}: Invalid value."]
 
     def Text(self) -> str:
         """"""
-        text = str(self.value)
-
         if self.unit is None:
-            return text
+            return str(self.value)  # str: Only useful when default value.
 
-        return f"{text}{UNIT_SEPARATOR}{self.unit}"
+        return f"{self.value}{UNIT_SEPARATOR}{self.unit}"
 
 
 def _ValueUnitAndComment(
     value_w_unit_w_comment: str,
     comment_marker: str,
     /,
 ) -> tuple[str, str | None, str | None]:
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/instance/parameter/unit.py` & `conf-ini-g-2023.6/conf_ini_g/instance/parameter/unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,70 +26,54 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
+from pathlib import Path as path_t
 from typing import Any, Sequence
 
 from conf_ini_g.instance.parameter.base import Pieces, base_t
-from conf_ini_g.specification.parameter.type import type_options_t, type_t
+from conf_ini_g.specification.parameter.type import type_t
 from conf_ini_g.specification.parameter.value import INVALID_VALUE
-from conf_ini_g.standard.path_extension import path_t
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class unit_instance_t(base_t):
-    def SetValue(
+    def SetStrValue(
         self,
         value_w_comment: str | Any,
         comment_marker: str,
-        type_options: type_options_t | None,
         /,
         *,
-        __: str = None,
+        _: str = None,
     ) -> None:
         """
         value_w_unit_w_comment: can be an uninterpreted string coming from an INI
         document, or can be an interpreted value coming from an interface.
         """
-        if isinstance(value_w_comment, str):
-            value_as_str, comment = _ValueAndComment(value_w_comment, comment_marker)
-        else:
-            value_as_str, comment = value_w_comment, None
-
-        value, value_type = type_options.TypedValueAndType(value_as_str)
-        if isinstance(value, str):
-            # number_as_str_t will leave an str-typed value as is. Hence, it must be
-            # converted here. But the call to type_options.TypedValueAndType allows to
-            # benefit from type checking.
-            try:
-                value = float(value)
-                if value.is_integer():
-                    value = int(value)
-                value_type = type_t.NewFromType(type(value))
-            except ValueError:
-                value = INVALID_VALUE
-                value_type = None
-
-        self.type = value_type
-        self.value = value
+        value_as_str, comment = _ValueAndComment(value_w_comment, comment_marker)
+        self.value = value_as_str
         self.comment = comment
 
-    def FinalValue(self, _=None) -> tuple[Any, list[str]]:
+    def TypedValue(
+        self, expected_type: type_t, /, *, units=None
+    ) -> tuple[Any, list[str]]:
         """"""
-        if (value := self.value) is INVALID_VALUE:
-            return INVALID_VALUE, ["Invalid value."]
+        final_value, success = expected_type.InterpretedValueOf(self.value)
+
+        if success:
+            return final_value, []
 
-        return value, []
+        return INVALID_VALUE, [f"{self.value}: Invalid value."]
 
     def Text(self) -> str:
         """"""
-        return str(self.value)
+        return self.value  # No need for "str" since units have no default values.
 
 
 def ConvertedValue(
     value: Any, conversion_factor: int | float, /
 ) -> tuple[Any, list[str]]:
     """"""
     unconverted_values = []
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/console/__init__.py` & `conf-ini-g-2023.6/conf_ini_g/interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/console/config.py` & `conf-ini-g-2023.6/conf_ini_g/interface/console/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,21 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import re as rgex
 from argparse import ArgumentParser as argument_parser_t
+from pathlib import Path as path_t
 from typing import Any, Iterator, Sequence
 
+from conf_ini_g.extension.string import Flattened
 from conf_ini_g.raw.config import raw_config_h
 from conf_ini_g.specification.config import config_t
 from conf_ini_g.specification.parameter.value import MISSING_REQUIRED_VALUE
-from conf_ini_g.standard.path_extension import path_t
-from conf_ini_g.standard.str_extension import Flattened
-
 
 parsed_arguments_h = dict[str, str]
 
 
 # Specified INI document file is stored in INI_DOCUMENT_VARIABLE
 INI_DOCUMENT_VARIABLE = "ini_path"
 
@@ -84,24 +83,24 @@
             default = MISSING_REQUIRED_VALUE
 
             if parameter.optional:
                 if isinstance(parameter.default, str):
                     delimiter = '"'
                 else:
                     delimiter = ""
-                types_and_value = (
-                    f"Options: {parameter.types}. "
+                type_and_value = (
+                    f"Type: {parameter.type}. "
                     f"Default: [green]{delimiter}{parameter.default}{delimiter}[/]"
                 )
             else:
-                types_and_value = str(default)
-            flattened = Flattened(types_and_value)
+                type_and_value = str(default)
+            flattened = Flattened(type_and_value)
             definition = f"{parameter.definition}. {flattened}"
 
-            # Type could be PythonTypeOfAnnotated(cmd_line_type). However, to allow passing any of the allowed types,
+            # Type could be TypeHintOfAnnotated(cmd_line_type). However, to allow passing any of the allowed types,
             # deferring type validation to functional config instantiation, this parameter is not passed.
             output.add_argument(
                 f"--{option}",
                 dest=attribute,
                 help=definition,
                 default=default,
                 metavar=attribute,
@@ -157,13 +156,13 @@
 
 
 def _SectionParameterValueIterator(
     arguments: parsed_arguments_h,
 ) -> Iterator[tuple[str, str, Any]]:
     """"""
     for prm_uid, value in arguments.items():
-        # See CommandLineParser for why this can happen
+        # See CommandLineParser for why this can happen.
         if value is MISSING_REQUIRED_VALUE:
             continue
 
         section, parameter = prm_uid.split(SECTION_PARAMETER_SEPARATOR)
         yield section, parameter, value
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/screen/config.py` & `conf-ini-g-2023.6/conf_ini_g/interface/screen/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,181 +27,184 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-from typing import Annotated, Callable, Iterator
+import dataclasses as dtcl
+from pathlib import Path as pl_path_t
+from typing import Annotated, Any, Callable, Iterator, Sequence
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import ALIGNED_HCENTER
-from conf_ini_g.catalog.interface.screen.library.pyqt5.main import (
-    ShowErrorMessage,
-    ShowMessage,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.button import button_wgt_t
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
-    grid_lyt_t,
-    hbox_lyt_t,
-    label_wgt_t,
-    library_wgt_t,
-    tabs_wgt_t,
-    vbox_lyt_t,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.scroll_container import (
-    scroll_container_t,
-)
 from conf_ini_g.catalog.interface.screen.parameter.boolean import boolean_wgt_t
+from conf_ini_g.catalog.interface.screen.parameter.path import path_wgt_t
 from conf_ini_g.catalog.specification.parameter.boolean import boolean_t
 from conf_ini_g.catalog.specification.parameter.path import path_t
+from conf_ini_g.catalog.specification.parameter.path import path_t as path_annotation_t
 from conf_ini_g.instance.config import config_t as config_instance_t
-from conf_ini_g.interface.screen.parameter.path_chooser import SelectedOutputFile
+from conf_ini_g.interface.screen.backend import (
+    backend_t,
+    button_wgt_h,
+    grid_lyt_h,
+    hbox_lyt_h,
+    library_wgt_h,
+    vbox_lyt_h,
+)
+from conf_ini_g.interface.screen.parameter.path_chooser import NewSelectedOutputDocument
 from conf_ini_g.interface.screen.section import controlled_section_t, section_t
 from conf_ini_g.interface.storage.config import SaveRawConfigToINIDocument
 from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
 from conf_ini_g.raw.config import AsStr, ini_config_h, raw_config_h
 from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.standard.path_extension import path_t as pl_path_t
 
 
-class config_t(library_wgt_t):
-    __slots__ = (
-        "instance",
-        "sections",
+@dtcl.dataclass(repr=False, eq=False)
+class config_t:
+    """
+    The class cannot use slots because it disables weak referencing, which is required.
+    See error message below when using slots:
+    TypeError: cannot create weak reference to 'config_t' object
+    [...]
+    File "[...]conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py", line 41, in SetFunction
+        self.clicked.connect(function)
+        │                    └ <bound method config_t.ToogleAdvancedMode of <conf_ini_g.interface.screen.config.config_t object at [...]>>
+        └ <conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices.dot_button_wgt_t object at [...]>
+
+    Widget might not cooperate well with list, in which case Python raises the
+    following exception: TypeError: multiple bases have instance lay-out conflict
+    To be safe, "sections" is a field instead of being part of the class definition.
+    """
+
+    sections: dict[str, section_t | controlled_section_t] = dtcl.field(
+        init=False, default=None
     )
-    # Widget might not cooperate well with list, in which case Python raises the
-    # following exception: TypeError: multiple bases have instance lay-out conflict
-    # To be safe, "sections" is field instead of being part of the class definition.
-    sections: dict[str, section_t | controlled_section_t]
     instance: config_instance_t
-    action_button: button_wgt_t
-    Action: Callable[[raw_config_h], None]
-
-    def __init__(self) -> None:
-        """"""
-        super().__init__()
-        # Do not use self.__class__.__slots__ because it will be the parent slots in case of inheritance
-        for slot in config_t.__slots__:
-            setattr(self, slot, None)
+    backend: backend_t
+    library_wgt: library_wgt_h
+    _action_button: button_wgt_h = dtcl.field(init=False, default=None)
+    Action: Callable[[raw_config_h], None] = None
+    _reference_keeper: tuple[library_wgt_h, ...] = None
 
     @classmethod
     def NewFromConfig(
         cls,
         title: str | None,
         instance: config_instance_t,
+        backend: backend_t,
         /,
         *,
         advanced_mode: bool = False,
         action: tuple[str, Callable[[raw_config_h], None]] = None,
     ) -> config_t:
         """"""
-        output = cls()
-        output.instance = instance
-        output.Action = action[1]
+        if action is None:
+            kwargs = {}
+        else:
+            kwargs = {"Action": action[1]}
+        output = cls(
+            instance=instance,
+            backend=backend,
+            library_wgt=backend.library_wgt_t(),
+            **kwargs,
+        )
 
         # --- Top-level widgets
-        if title is None:
-            components = []
-        else:
-            components = [title]
-        home = pl_path_t.home()
-        if instance.ini_path is not None:
-            components.append(f"INI:{instance.ini_path.relative_to(home)}")
-        components.append(f"SPEC:{instance.specification.spec_path}")
-        title = "<br/>".join(components)
-
-        title_wgt = label_wgt_t("<b>" + title + "</b>")
-        title_wgt.setAlignment(ALIGNED_HCENTER)
-        advanced_mode_lyt = _AdvancedModeLayout(advanced_mode, output)
-        button_lyt = _ActionButtonsLayout(output, action, instance.ini_path is not None)
+        title_lyt, widget_1 = _TitleLayout(title, instance, output)
+        advanced_mode_lyt, widget_2 = _AdvancedModeLayout(advanced_mode, output)
+        button_lyt, widgets = _ActionButtonsLayout(
+            output, action, instance.ini_path is not None
+        )
+        output._reference_keeper = (widget_1, widget_2, *widgets)
 
         # --- Sections
         categories = {}
         sections = {}
         controlled_sections = []
 
         for section_spec in instance.specification:
             if (controller := section_spec.controller) is None:
                 section = section_t.NewForSection(
-                    section_spec, instance[section_spec.name]
+                    section_spec, instance[section_spec.name], backend
                 )
             else:
                 section = controlled_section_t.NewForSection(
                     section_spec,
                     controller,
                     instance.GetValueOfController(controller),
                     instance[section_spec.name],
+                    backend,
                 )
                 if section is not None:
                     controlled_sections.append((section, section_spec))
             if section is None:
                 continue
 
             sections[section_spec.name] = section
 
             if (category := section_spec.category) not in categories:
-                contents = library_wgt_t(parent=None)
-                scroll_area = scroll_container_t.NewForWidget(contents)
-                layout = vbox_lyt_t()
+                contents = backend.library_wgt_t()
+                scroll_area = backend.scroll_container_t.NewForWidget(contents)
+                layout = backend.vbox_lyt_t()
                 contents.setLayout(layout)
                 categories[category] = (layout, scroll_area)
 
             layout = categories[category][0]
-            layout.addWidget(section)
+            layout.addWidget(section.library_wgt)
 
         output.sections = sections
 
         if categories.__len__() > 1:
-            category_selector = tabs_wgt_t()
+            category_selector = backend.tabs_wgt_t()
             for category, (_, scroll_area) in categories.items():
                 category_selector.addTab(scroll_area, category)
         else:
             category = tuple(categories.keys())[0]
             category_selector = categories[category][1]
 
         for section, section_spec in controlled_sections:
             controller = section_spec.controller
             parameter = output[controller.section].parameters[controller.parameter]
-            value_wgt = parameter.active_value
+            value_wgt = parameter.value
             if hasattr(value_wgt, "SetFunction"):
                 value_wgt.SetFunction(section.page_stack.setCurrentIndex)
             else:
-                ShowErrorMessage(
-                    f'{controller.section}.{controller.parameter}: Controller has no "SetFunction" method; Disabling control'
+                backend.ShowErrorMessage(
+                    f"{controller.section}.{controller.parameter}: "
+                    f'Controller has no "SetFunction" method; Disabling control.'
                 )
 
         # --- Layout...
-        layout = grid_lyt_t()
-        if title_wgt is None:
+        layout = backend.grid_lyt_t()
+        if title_lyt is None:
             first_available_row = 0
         else:
-            layout.addWidget(title_wgt, 0, 0, 1, 1)
+            layout.addLayout(title_lyt, 0, 0, 1, 1)
             first_available_row = 1
         layout.addWidget(category_selector, first_available_row, 0, 1, 1)
         layout.addLayout(advanced_mode_lyt, first_available_row + 1, 0, 1, 1)
         layout.addLayout(button_lyt, first_available_row + 2, 0, 1, 1)
 
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
         # --- ...Layout
 
         output.ToogleAdvancedMode(advanced_mode)
 
         return output
 
     def ToogleAdvancedMode(self, advanced_mode: bool, /) -> None:
         """"""
         for section_name, section in self.sections.items():
             section_spec = self.instance.specification[section_name]
             if section_spec.basic:
                 should_check_parameters = True
             elif advanced_mode:
-                section.setVisible(True)
+                section.library_wgt.setVisible(True)
                 should_check_parameters = True
             else:
-                section.setVisible(False)
+                section.library_wgt.setVisible(False)
                 should_check_parameters = False
 
             if should_check_parameters:
                 if (controller := section_spec.controller) is None:
                     parameter_specs = section_spec
                 else:
                     controller_text = (
@@ -232,154 +235,214 @@
                 section.active_parameters.values(), parameter_specs
             ):
                 if parameter.unit is None:
                     unit_kwarg = {}
                 else:
                     unit_kwarg = {"unit": parameter.unit.Text()}
                 instance = self.instance[section_spec.name][parameter_spec.name]
-                instance.SetValue(
-                    parameter.Value(),
+                instance.SetStrValue(
+                    parameter.Text(),
                     INI_COMMENT_MARKER,
-                    parameter_spec.types,
                     **unit_kwarg,
                 )
 
         return self.instance.Issues()
 
     def AsINIConfig(self) -> ini_config_h | None:
         """"""
         issues = self.SynchronizeInstance()
         if issues.__len__() == 0:
             output = self.instance.AsINIConfig()
         else:
             output = None
-            ShowErrorMessage("\n".join(issues), parent=self)
+            self.backend.ShowErrorMessage("\n".join(issues), parent=self)
 
         return output
 
     def ShowInINIFormat(self) -> None:
         """"""
         config = self.AsINIConfig()
         if config is None:
             return
 
         config = AsStr(config, in_html_format=True)
-        ShowMessage("INI Config", "<tt>" + config + "<tt/>")
+        self.backend.ShowMessage("INI Config", "<tt>" + config + "<tt/>")
 
     def SaveConfig(self, new_ini: bool, /) -> None:
         """"""
         if new_ini:
-            path = SelectedOutputFile(
+            path = NewSelectedOutputDocument(
                 "Save Config As",
                 "Save Config As",
+                self.backend,
                 mode=path_t.TARGET_TYPE.document,
                 valid_types={"Config files": ("ini", "INI")},
             )
         else:
             path = self.instance.ini_path  # Will overwrite current INI document
 
         if path is not None:
             config = self.AsINIConfig()
             error = SaveRawConfigToINIDocument(config, path)
             if error is None:
                 self.instance.ini_path = path
             else:
-                ShowErrorMessage(error, parent=self)
+                self.backend.ShowErrorMessage(error, parent=self)
 
     def LaunchAction(self) -> None:
         """"""
         issues = self.SynchronizeInstance()
         if issues.__len__() == 0:
             raw_config, issues = self.instance.AsRawConfig()
             if issues.__len__() == 0:
-                self.action_button.setEnabled(False)
+                self._action_button.setEnabled(False)
                 try:
                     self.Action(raw_config)
                 except Exception as exception:
-                    ShowErrorMessage(str(exception), parent=self)
-                self.action_button.setEnabled(True)
+                    self.backend.ShowErrorMessage(
+                        str(exception), parent=self.library_wgt
+                    )
+                self._action_button.setEnabled(True)
             else:
-                ShowErrorMessage("\n".join(issues), parent=self)
+                self.backend.ShowErrorMessage(
+                    "\n".join(issues), parent=self.library_wgt
+                )
         else:
-            ShowErrorMessage("\n".join(issues), parent=self)
+            self.backend.ShowErrorMessage("\n".join(issues), parent=self.library_wgt)
+
+    def __getattr__(self, attribute: str, /) -> Any:
+        """
+        E.g., used for "show".
+        """
+        try:
+            output = super().__getattr__(attribute)
+        except AttributeError:
+            output = getattr(self.library_wgt, attribute)
+
+        return output
 
     def __contains__(self, key: str, /) -> bool:
         """"""
         return key in self.sections
 
     def __getitem__(self, key: str, /) -> section_t | controlled_section_t:
         """"""
         return self.sections[key]
 
     def __iter__(self) -> Iterator[str]:
         """"""
         return self.sections.keys()
 
 
-def _AdvancedModeLayout(advanced_mode: bool, config: config_t, /) -> hbox_lyt_t:
+def _TitleLayout(
+    title: str | None, instance: config_instance_t, config: config_t, /
+) -> tuple[vbox_lyt_h, path_wgt_t]:
+    """"""
+    layout = config.backend.vbox_lyt_t()
+
+    if title is None:
+        title = "Conf-INI-g"
+    title = (
+        f'<h1 style="color: blue">{title}</h1>'
+        f"<b><font face=monospace>SPEC:</font></b> {instance.specification.spec_path}"
+    )
+    title_wgt = config.backend.label_wgt_t(title)
+    title_wgt.setAlignment(config.backend.ALIGNED_LEFT)
+
+    if instance.ini_path is None:
+        ini_path_wgt = path_layout = None
+    else:
+        ini_path_wgt = path_wgt_t.NewWithDetails(
+            pl_path_t(instance.ini_path),
+            path_annotation_t(
+                target_type=path_annotation_t.TARGET_TYPE.document, is_input=True
+            ),
+            config.backend,
+            None,
+            editable=False,
+        )
+        label_wgt = config.backend.label_wgt_t(
+            "<b><font face=monospace>INI: </font></b>"
+        )
+        label_wgt.setSizePolicy(config.backend.SIZE_FIXED, config.backend.SIZE_FIXED)
+        path_layout = config.backend.hbox_lyt_t()
+        path_layout.addWidget(label_wgt)
+        path_layout.addWidget(ini_path_wgt.library_wgt)
+
+    layout.addWidget(title_wgt)
+    if path_layout is not None:
+        layout.addLayout(path_layout)
+
+    return layout, ini_path_wgt
+
+
+def _AdvancedModeLayout(
+    advanced_mode: bool, config: config_t, /
+) -> tuple[hbox_lyt_h, boolean_wgt_t]:
     """"""
-    output = hbox_lyt_t()
+    layout = config.backend.hbox_lyt_t()
 
     annotated_type = Annotated[bool, boolean_t(mode=boolean_t.MODE.on_off)]
-    value_type = type_t.NewFromAnnotatedType(annotated_type)
+    value_type = type_t.NewFromType(annotated_type)
     boolean = boolean_wgt_t.NewWithDetails(
         advanced_mode,
         value_type,
+        config.backend,
         None,
     )
     boolean.true_btn.SetFunction(config.ToogleAdvancedMode)
 
-    output.addWidget(label_wgt_t("<i>Advanced Mode</i>"))
-    output.addWidget(boolean)
+    layout.addWidget(config.backend.label_wgt_t("<i>Advanced Mode</i>"))
+    layout.addWidget(boolean.library_wgt)
 
-    return output
+    return layout, boolean
 
 
 def _ActionButtonsLayout(
     config: config_t,
     action: tuple[str, Callable[[raw_config_h], None]] | None,
     has_ini_document: bool,
     /,
-) -> grid_lyt_t:
+) -> tuple[grid_lyt_h, Sequence[button_wgt_h, ...]]:
     """"""
-    layout = grid_lyt_t()
+    layout = config.backend.grid_lyt_t()
 
     buttons = []
     geometries = []
 
-    button = button_wgt_t("Show in INI format")
+    button = config.backend.button_wgt_t("Show in INI format")
     button.SetFunction(config.ShowInINIFormat)
     buttons.append(button)
     geometries.append((0, 0, 1, 2))
 
-    button = button_wgt_t("Save Config As")
+    button = config.backend.button_wgt_t("Save Config As")
     button.SetFunction(lambda: config.SaveConfig(True))
     buttons.append(button)
     if has_ini_document:
         geometries.append((1, 0, 1, 1))
 
-        button = button_wgt_t("Save/Overwrite Config")
+        button = config.backend.button_wgt_t("Save/Overwrite Config")
         button.SetFunction(lambda: config.SaveConfig(False))
         buttons.append(button)
         geometries.append((1, 1, 1, 1))
     else:
         geometries.append((1, 0, 1, 2))
 
     if action is None:
         label = "Close"
-        Function = config.Close
+        Function = config.library_wgt.close
     else:
         label = action[0]
         Function = config.LaunchAction
 
-    button = button_wgt_t(label)
+    button = config.backend.button_wgt_t(label)
     button.SetFunction(Function)
     buttons.append(button)
     geometries.append((2, 0, 1, 2))
 
-    config.action_button = button
+    config._action_button = button
 
     for button, geometry in zip(buttons, geometries):
         layout.addWidget(button, *geometry)
     layout.setContentsMargins(0, 0, 0, 0)
 
-    return layout
+    return layout, buttons
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/screen/generic.py` & `conf-ini-g-2023.6/conf_ini_g/interface/screen/generic.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/path_chooser.py` & `conf-ini-g-2023.6/conf_ini_g/interface/screen/parameter/path_chooser.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,175 +25,135 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Sequence
+from pathlib import Path as pl_path_t
+from typing import Callable, Sequence, TypeVar
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import (
-    DIALOG_ACCEPT_OPEN,
-    DIALOG_ACCEPT_SAVE,
-    DIALOG_ACCEPTATION,
-    DIALOG_AUTO_OVERWRITE,
-    DIALOG_MODE_ANY,
-    DIALOG_MODE_EXISTING_FILE,
-    DIALOG_MODE_FOLDER,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.main import (
-    ShowErrorMessage,
-    event_loop_t,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.path_chooser import (
-    path_chooser_wgt_t,
-)
 from conf_ini_g.catalog.specification.parameter.path import path_t
-from conf_ini_g.standard.path_extension import any_path_h
-from conf_ini_g.standard.path_extension import path_t as pl_path_t
+from conf_ini_g.extension.path import any_path_h
+from conf_ini_g.interface.screen.backend import backend_t
 
 """
 valid_types: {"Type": "extension", "Type": ("extension", "extension",...), ...}
 filter: "Image files (*.png *.xpm *.jpg);Text files (*.txt);Any files (*)"
 """
 
 
-valid_types_t = dict[str, str | Sequence[str]]
+path_chooser_wgt_h = TypeVar("path_chooser_wgt_h")
+valid_types_h = dict[str, str | Sequence[str]]
+document_selection_fct_h = Callable[..., pl_path_t | None]
 
 
-def SelectedInputFile(
+def NewSelectedInputDocument(
     title: str,
     caption: str,
+    backend: backend_t,
     /,
     *,
     mode: path_t.TARGET_TYPE = path_t.TARGET_TYPE.any,
-    valid_types: valid_types_t = None,
+    valid_types: valid_types_h = None,
     start_folder: any_path_h = None,
     initial_selection: any_path_h = None,
 ) -> pl_path_t | None:
     """"""
-    _EnsureAQAppIsRunning()
-
     extension_filter, _ = _AllowedTypesElements(valid_types)
     check_existence = False
     if mode is path_t.TARGET_TYPE.document:
-        dialog_mode = DIALOG_MODE_EXISTING_FILE
+        dialog_mode = backend.DIALOG_MODE_EXISTING_FILE
     elif mode is path_t.TARGET_TYPE.folder:
-        dialog_mode = DIALOG_MODE_FOLDER
+        dialog_mode = backend.DIALOG_MODE_FOLDER
     else:
         # TODO: Check if that allows to select a folder (documentation says "The name of
         #     a file, whether it exists or not."). So a priori, no. But then how can we
         #     allow selection of either a file or a folder?
-        dialog_mode = DIALOG_MODE_ANY
+        dialog_mode = backend.DIALOG_MODE_ANY
         check_existence = True
 
     while True:
-        dialog = _GenericFileDialog(
-            title, caption, extension_filter, start_folder, initial_selection
+        dialog = _GenericDocumentDialog(
+            title, caption, extension_filter, start_folder, initial_selection, backend
         )
-        dialog.setAcceptMode(DIALOG_ACCEPT_OPEN)
+        dialog.setAcceptMode(backend.DIALOG_ACCEPT_OPEN)
         dialog.setFileMode(dialog_mode)
 
-        output = _SelectedFile(dialog)
+        output = _SelectedDocument(dialog, backend)
         if output is None:
             return None
         if check_existence and not output.exists():
-            ShowErrorMessage(f"{output}: Nonexistent file or folder")
+            backend.ShowErrorMessage(f"{output}: Nonexistent file or folder")
             start_folder = _StartFolderFromFolder(output)
             initial_selection = None
         else:
-            # The file dialog does not allow to select either a file or a folder. So the solution here is to select a file,
-            # and if a folder was needed, take the parent.
+            # The file dialog does not allow to select either a file or a folder. So the
+            # solution here is to select a file, and if a folder was needed, take the
+            # parent.
             if (mode is path_t.TARGET_TYPE.folder) and output.is_file():
                 output = output.parent
             return output
 
 
-def SelectedOutputFile(
+def NewSelectedOutputDocument(
     title: str,
     caption: str,
+    backend: backend_t,
     /,
     *,
     mode: path_t.TARGET_TYPE = path_t.TARGET_TYPE.any,
-    valid_types: valid_types_t = None,
+    valid_types: valid_types_h = None,
     auto_overwrite: bool = False,
     start_folder: any_path_h = None,
     initial_selection: any_path_h = None,
 ) -> pl_path_t | None:
     """"""
-    _EnsureAQAppIsRunning()
-
     extension_filter, allowed_extensions = _AllowedTypesElements(valid_types)
     while True:
-        dialog = _GenericFileDialog(
-            title, caption, extension_filter, start_folder, initial_selection
+        dialog = _GenericDocumentDialog(
+            title, caption, extension_filter, start_folder, initial_selection, backend
         )
-        dialog.setAcceptMode(DIALOG_ACCEPT_SAVE)
-        dialog.setFileMode(DIALOG_MODE_ANY)
+        dialog.setAcceptMode(backend.DIALOG_ACCEPT_SAVE)
+        dialog.setFileMode(backend.DIALOG_MODE_ANY)
         if auto_overwrite:
-            dialog.setOption(DIALOG_AUTO_OVERWRITE)
+            dialog.setOption(backend.DIALOG_AUTO_OVERWRITE)
 
-        output = _SelectedFile(dialog)
+        output = _SelectedDocument(dialog, backend)
         if output is None:
             return None
         # The file dialog does not allow to select either a file or a folder. So the solution here is to select a file,
         # and if a folder was needed, take the parent. See (*) below.
         if (mode is path_t.TARGET_TYPE.folder) and output.exists() and output.is_file():
             output = output.parent
 
         erroneous_selection = False
         if output.exists():
             if (mode is path_t.TARGET_TYPE.document) and not output.is_file():
-                ShowErrorMessage(f"{output}: Not of regular file")
+                backend.ShowErrorMessage(f"{output}: Not of regular file")
                 erroneous_selection = True
             # Unnecessary due to (*) above
             # elif (mode == "folder") and not output.is_dir():
             #     ShowErrorMessage(f"{output}: Not a folder")
             #     erroneous_selection = True
 
         if not erroneous_selection:
             if ("*" in allowed_extensions) or (
                 output.suffix.lower()[1:] in allowed_extensions
             ):
                 return output
             else:
-                ShowErrorMessage(f"{output}: Extension is not valid")
+                backend.ShowErrorMessage(f"{output}: Extension is not valid")
 
         start_folder = _StartFolderFromFolder(output)
         initial_selection = None
 
 
-# def ContinueDespitePotentialOverwriting(path: pl_path_t) -> bool:
-#     #
-#     if path.exists():
-#         # noinspection PyArgumentList
-#         overwriting_dialog = qw_.QMessageBox()
-#         overwriting_dialog.setWindowTitle("File Overwriting Confirmation")
-#         overwriting_dialog.setText(f"{path.__str__()}:\nFile already exists.")
-#         overwriting_dialog.setInformativeText("Do you want to overwrite it?")
-#         overwriting_dialog.setStandardButtons(
-#             qw_.QMessageBox.Cancel | qw_.QMessageBox.Save
-#         )
-#         overwriting_dialog.setDefaultButton(qw_.QMessageBox.Cancel)
-#
-#         return overwriting_dialog.exec_() == qw_.QMessageBox.Save
-#
-#     return True
-
-
-def _EnsureAQAppIsRunning() -> None:
-    #
-    if event_loop_t.GetInstance() is None:
-        _ = event_loop_t([])  # Empty sys.argv
-        # Initially, there was a tuple argument: (f"Launched-From-{__name__}",).
-        # But PySide2 complains about not being of type typing.Sequence[str].
-
-
 def _AllowedTypesElements(
-    valid_types: valid_types_t | None,
+    valid_types: valid_types_h | None, /
 ) -> tuple[str, tuple[str]]:
     """"""
     if valid_types is None:
         return "Any file or folder (*)", ("*",)
 
     types = []
     extensions = []
@@ -210,60 +170,49 @@
             extensions.extend(extension)
             new_extensions = tuple(f"*.{_ext}" for _ext in extension)
         filters.append(f"{_type.title()} ({' '.join(new_extensions)})")
 
     return ";".join(filters), tuple(extensions)
 
 
-def _StartFolderFromFolder(folder: pl_path_t) -> pl_path_t | None:
+def _StartFolderFromFolder(folder: pl_path_t, /) -> pl_path_t | None:
     """"""
     output = folder
 
     root = folder.root
     while (output != root) and (not output.exists()):
         output = output.parent
     if output == root:
         output = None
 
     return output
 
 
-def _GenericFileDialog(
+def _GenericDocumentDialog(
     title: str,
     caption: str,
     extension_filter: str,
     start_folder: any_path_h,
     initial_selection: any_path_h,
-) -> path_chooser_wgt_t:
-    #
-    # noinspection PyArgumentList
-    output = path_chooser_wgt_t(caption, extension_filter=extension_filter)
+    backend: backend_t,
+    /,
+) -> path_chooser_wgt_h:
+    """"""
+    output = backend.path_chooser_wgt_t(caption, extension_filter=extension_filter)
     output.setWindowTitle(title)
     if start_folder is not None:
         output.setDirectory(str(start_folder))
     if initial_selection is not None:
         output.selectFile(str(initial_selection))
 
     return output
 
 
-def _SelectedFile(dialog: path_chooser_wgt_t) -> pl_path_t | None:
-    #
+def _SelectedDocument(
+    dialog: path_chooser_wgt_h, backend: backend_t, /
+) -> pl_path_t | None:
+    """"""
     status = dialog.RunAndGetClosingStatus()
-    if status == DIALOG_ACCEPTATION:
+    if status == backend.DIALOG_ACCEPTATION:
         return pl_path_t(dialog.SelectedFile())
 
     return None
-
-
-# file_dialog = qw_.QFileDialog(self)
-# file_dialog.setDirectory(current_doc.parent.__str__())
-# file_dialog.selectFile(current_doc.__str__())
-# File
-# file_dialog.setWindowTitle("Select File")
-# file_dialog.setFileMode(qw_.QFileDialog.ExistingFile)
-# Folder
-# file_dialog.setWindowTitle("Select Folder")
-# file_dialog.setFileMode(qw_.QFileDialog.Directory)
-# Both
-# file_dialog.setWindowTitle("Select File or Folder")
-# file_dialog.setFileMode(qw_.QFileDialog.AnyFile)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/screen/parameter/type_selector.py` & `conf-ini-g-2023.6/conf_ini_g/specification/parameter/value.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,41 +25,38 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Sequence
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.choices import (
-    choices_list_wgt_t,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import library_wgt_t
-from conf_ini_g.specification.parameter.type import type_t
-from conf_ini_g.standard.type_extension import none_t
-
-
-class type_selector_wgt_t(choices_list_wgt_t):
-    """"""
-
-    def __init__(
-        self,
-        types: Sequence[type_t],
-        selected_type: type_t,
-        parent: library_wgt_t = None,
-    ) -> None:
+class missing_required_value_t:
+    TEXT = "MISSING REQUIRED VALUE"
+
+    def __str__(self) -> str:
+        """"""
+        return self.__class__.TEXT
+
+    def __rich__(self) -> str:
         """"""
-        super().__init__(parent=parent)
+        return f"[red]{self.__class__.TEXT}[/]"
+
+
+class invalid_value_t:
+    """
+    Do not use invalid_value_t = object, for example, otherwise isinstance returns True for anything.
+    """
+
+    TEXT = "INVALID VALUE"
+
+    def __str__(self) -> str:
+        """"""
+        return self.__class__.TEXT
+
+    def __rich__(self) -> str:
+        """"""
+        return f"[red]{self.__class__.TEXT}[/]"
+
 
-        for type_ in types:
-            if type_.py_type is none_t:
-                self.addItem("None")
-            else:
-                self.addItem(type_.py_type.__name__)
-        self.setCurrentText(selected_type.py_type.__name__)
-
-    def Value(self) -> str:
-        """
-        Cannot be done using: class.Value = class.Text since the Text method is added to instances, not to the class
-        """
-        return self.Text()
+MISSING_REQUIRED_VALUE = missing_required_value_t()
+INVALID_VALUE = invalid_value_t()
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/screen/section.py` & `conf-ini-g-2023.6/conf_ini_g/interface/screen/section.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,69 +27,68 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
+import dataclasses as dtcl
 from typing import ClassVar, Iterator, Sequence
 
-from conf_ini_g.catalog.interface.screen.library.pyqt5.constant import (
-    ALIGNED_RIGHT,
-    ALIGNED_TOP,
-)
-from conf_ini_g.catalog.interface.screen.library.pyqt5.widget.main import (
-    grid_lyt_t,
-    group_wgt_t,
-    hbox_lyt_t,
-    label_wgt_t,
-    library_wgt_t,
-    stack_wgt_t,
-)
 from conf_ini_g.instance.parameter.main import instance_t
+from conf_ini_g.interface.screen.backend import (
+    backend_t,
+    grid_lyt_h,
+    group_wgt_h,
+    label_wgt_h,
+    stack_wgt_h,
+)
 from conf_ini_g.interface.screen.generic import FormattedName
 from conf_ini_g.interface.screen.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.main import parameter_t as parameter_spec_t
 from conf_ini_g.specification.section.main import controller_t
 from conf_ini_g.specification.section.main import section_t as section_spec_t
 
 
-class _base_t(group_wgt_t):  # Cannot be abstracted
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class _base_t:  # Cannot be abstracted
     HEADER_NAMES: ClassVar[tuple[str]] = (
         "Parameter",
         "Type(s)",
         "Value",
         "Unit",
     )
     HEADER_STYLE: ClassVar[str] = "background-color: darkgray; padding-left: 5px;"
 
+    library_wgt: group_wgt_h
     formatted_name: str
 
     @classmethod
-    def NewWithName(cls, name: str, /, *, controller: controller_t = None) -> _base_t:
+    def NewWithName(
+        cls, name: str, backend: backend_t, /, *, controller: controller_t = None
+    ) -> _base_t:
         """"""
-        output = cls()
-
         if controller is None:
             controller = ""
         else:
             controller = f" ⮜ {controller.section}.{controller.parameter}"
-        output.formatted_name = FormattedName(name, " ") + controller
+        formatted_name = FormattedName(name, " ") + controller
 
-        output.setTitle(output.formatted_name)
+        output = cls(library_wgt=backend.group_wgt_t(), formatted_name=formatted_name)
+        output.library_wgt.setTitle(formatted_name)
 
         return output
 
     @classmethod
-    def Headers(cls) -> Sequence[label_wgt_t]:
+    def Headers(cls, backend: backend_t, /) -> Sequence[label_wgt_h]:
         """"""
         output = []
 
         for text in cls.HEADER_NAMES:
-            header = label_wgt_t(f'<font color="blue">{text}</font>')
+            header = backend.label_wgt_t(f'<font color="blue">{text}</font>')
             header.setStyleSheet(cls.HEADER_STYLE)
             output.append(header)
 
         return output
 
     @property
     def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
@@ -116,99 +115,104 @@
     def __iter__(self) -> Iterator[parameter_t]:
         """"""
         for parameter_set in self.all_parameters:
             for parameter in parameter_set:
                 yield parameter
 
 
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class section_t(_base_t):
-    __slots__ = ("parameters",)
-    parameters: dict[str, parameter_t]
+    parameters: dict[str, parameter_t] = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewForSection(
-        cls, section_spec: section_spec_t, instances: dict[str, instance_t], /
+        cls,
+        section_spec: section_spec_t,
+        instances: dict[str, instance_t],
+        backend: backend_t,
+        /,
     ) -> section_t | None:
         """"""
-        output = cls.NewWithName(section_spec.name)
+        output = cls.NewWithName(section_spec.name, backend)
 
         parameters, parameter_names, layout = _ParametersFromSpecifications(
-            section_spec, instances
+            section_spec, instances, backend
         )
         if parameters.__len__() == 0:
             return None
 
         output.parameters = dict(zip(parameter_names, parameters))
 
-        for h_idx, header in enumerate(cls.Headers()):
+        for h_idx, header in enumerate(cls.Headers(backend)):
             layout.addWidget(header, 0, h_idx)
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
 
         return output
 
     @property
     def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
         """"""
         return (self.parameters,)
 
     @property
     def active_parameters(self) -> dict[str, parameter_t]:
         """"""
         return self.parameters
 
 
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class controlled_section_t(_base_t):
-    __slots__ = ("parameter_sets", "page_stack")
-    parameter_sets: list[dict[str, parameter_t]]
-    page_stack: stack_wgt_t
+    parameter_sets: list[dict[str, parameter_t]] = dtcl.field(init=False, default=None)
+    page_stack: stack_wgt_h = dtcl.field(init=False, default=None)
 
     @classmethod
     def NewForSection(
         cls,
         section_spec: section_spec_t,
         controller: controller_t,
         controller_value: str,
         instances: dict[str, instance_t],
+        backend: backend_t,
         /,
     ) -> controlled_section_t | None:
         """"""
-        output = cls.NewWithName(section_spec.name, controller=controller)
+        output = cls.NewWithName(section_spec.name, backend, controller=controller)
 
         parameter_sets = []
-        page_stack = stack_wgt_t()
+        page_stack = backend.stack_wgt_t()
         for parameter_specs in (section_spec, *section_spec.alternatives.values()):
             parameters, parameter_names, layout = _ParametersFromSpecifications(
-                parameter_specs, instances
+                parameter_specs, instances, backend
             )
             if parameters.__len__() == 0:
                 continue
 
             parameter_sets.append(dict(zip(parameter_names, parameters)))
 
-            for h_idx, header in enumerate(cls.Headers()):
+            for h_idx, header in enumerate(cls.Headers(backend)):
                 layout.addWidget(header, 0, h_idx)
-            page = library_wgt_t()
+            page = backend.library_wgt_t()
             page.setLayout(layout)
             page_stack.addWidget(page)
 
         if parameter_sets.__len__() == 0:
             return None
 
         output.parameter_sets = parameter_sets
         output.page_stack = page_stack
 
         controlling_values = section_spec.controlling_values
         page_stack.setCurrentIndex(controlling_values.index(controller_value))
 
         # Curiously, the stacked widget cannot be simply declared as child of instance;
         # This must be specified through a layout.
-        layout = hbox_lyt_t()
+        layout = backend.hbox_lyt_t()
         layout.addWidget(page_stack)
         layout.setContentsMargins(0, 0, 0, 0)
-        output.setLayout(layout)
+        output.library_wgt.setLayout(layout)
 
         return output
 
     @property
     def all_parameters(self) -> Sequence[dict[str, parameter_t]]:
         """"""
         return self.parameter_sets
@@ -218,35 +222,36 @@
         """"""
         return self.parameter_sets[self.page_stack.currentIndex()]
 
 
 def _ParametersFromSpecifications(
     specifications: section_spec_t | Iterator[parameter_spec_t],
     instances: dict[str, instance_t],
+    backend: backend_t,
     /,
-) -> tuple[Sequence[parameter_t], Sequence[str], grid_lyt_t]:
+) -> tuple[Sequence[parameter_t], Sequence[str], grid_lyt_h]:
     """"""
     parameters = []
     parameter_names = []
 
-    layout = grid_lyt_t()
-    layout.setAlignment(ALIGNED_TOP)
+    layout = backend.grid_lyt_t()
+    layout.setAlignment(backend.ALIGNED_TOP)
     layout.setColumnStretch(0, 4)
-    layout.setColumnStretch(1, 4)
+    layout.setColumnStretch(1, 1)
     layout.setColumnStretch(2, 8)
     layout.setColumnStretch(3, 1)
     layout.setContentsMargins(0, 0, 0, 0)
 
     for row, parameter_spec in enumerate(specifications, start=1):
         parameter = parameter_t.NewForParameter(
-            parameter_spec, instances[parameter_spec.name]
+            parameter_spec, instances[parameter_spec.name], backend
         )
         parameters.append(parameter)
         parameter_names.append(parameter_spec.name)
 
-        layout.addWidget(parameter.name, row, 0, alignment=ALIGNED_RIGHT)
-        layout.addWidget(parameter.type_selector, row, 1)
-        layout.addWidget(parameter.value_stack, row, 2, 1, 2 - 1)
+        layout.addWidget(parameter.name, row, 0, alignment=backend.ALIGNED_RIGHT)
+        layout.addWidget(parameter.type, row, 1)
+        layout.addWidget(parameter.value.library_wgt, row, 2, 1, 2 - 1)
         if parameter.unit is not None:
             layout.addWidget(parameter.unit, row, 3)
 
     return parameters, parameter_names, layout
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/storage/config.py` & `conf-ini-g-2023.6/conf_ini_g/interface/storage/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,27 +28,25 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import sys as sstm
 from argparse import ArgumentParser as argument_parser_t
 
-from conf_ini_g.raw.config import AsStr, INIConfigFromINIDocument, any_raw_config_h
-from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.value import missing_required_value_t
-from conf_ini_g.specification.section.main import section_t
-from conf_ini_g.specification.section.unit import IsUnitSection
-from conf_ini_g.standard.path_extension import (
+from conf_ini_g.extension.path import (
     ValidateInputPath,
     ValidateOutputPath,
     any_path_h,
     path_t,
 )
-from conf_ini_g.standard.str_extension import AsInterpretedObject
-
+from conf_ini_g.extension.string import AsInterpretedObject
+from conf_ini_g.raw.config import AsStr, INIConfigFromINIDocument, any_raw_config_h
+from conf_ini_g.specification.parameter.main import parameter_t
+from conf_ini_g.specification.section.main import section_t
+from conf_ini_g.specification.section.unit import IsUnitSection
 
 SECTIONS = "SECTIONS"
 
 
 def DraftSpecificationFromINIDocument(path: any_path_h, /) -> str | None:
     """"""
     ini_config = INIConfigFromINIDocument(path)
@@ -60,21 +58,18 @@
         # possibly_fuzzy=True: in case the raw config is not valid in that respect
         if IsUnitSection(section_name, possibly_fuzzy=True):
             continue
 
         parameters_as_lst = []
         for parameter_name, value_as_str in parameters.items():
             value, _ = AsInterpretedObject(value_as_str)
-            py_type = type(value)
-
             parameter = (
                 f"{parameter_t.__name__}(\n"
                 f'                name="{parameter_name}",\n'
-                f"                types={py_type.__name__},\n"
-                f"                default={missing_required_value_t.__name__}()\n"
+                f"                type={type(value).__name__},\n"
                 f"            )"
             )
             parameters_as_lst.append(parameter)
 
         parameters_as_str = ",\n            ".join(parameters_as_lst)
         section = (
             f"    {section_t.__name__}(\n"
@@ -88,16 +83,14 @@
 
     imports = (
         f"# To use this specification file:\n"
         f"#     1. import the object {SECTIONS}\n"
         f"#     2. instantiate a conf_ini_g.specification.config.config_t from it\n"
         f"from conf_ini_g.specification.parameter.main "
         f"import {parameter_t.__name__}\n"
-        f"from conf_ini_g.specification.parameter.value "
-        f"import {missing_required_value_t.__name__}\n"
         f"from conf_ini_g.specification.section.main import {section_t.__name__}\n"
     )
 
     return imports + f"\n{SECTIONS} = (\n" + ",\n".join(sections) + ",\n)\n"
 
 
 def SaveRawConfigToINIDocument(
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/interface/storage/constant.py` & `conf-ini-g-2023.6/conf_ini_g/interface/storage/constant.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/light/config.py` & `conf-ini-g-2023.6/conf_ini_g/light/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,48 +32,44 @@
 from __future__ import annotations
 
 import inspect as nspt
 from typing import Callable
 
 from rich.text import Text as text_t
 
+from conf_ini_g.extension.path import any_path_h, path_t
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.extension.type import NameValueTypeAsRichStr, TypeAsRichStr
 from conf_ini_g.raw.config import ini_config_h
-from conf_ini_g.standard.path_extension import any_path_h, path_t
-from conf_ini_g.standard.str_extension import (
-    AlignedOnSeparator,
-    AsComplexInterpretedObject,
-)
-from conf_ini_g.standard.type_extension import (
-    NameValueTypeAsRichStr,
-    TypeAsRichStr,
-    raw_hint_h,
-)
-
+from conf_ini_g.specification.parameter.type import type_t
 
 SECTION_PARAMETER_SEPARATOR = "__"
 
 
 class config_t:
     path: path_t
-    _type_hints: dict[str, raw_hint_h]
+    _types: dict[str, type_t]
 
     @classmethod
     def NewFromDictionary(
         cls, ini_config: ini_config_h, /, *, path: any_path_h = None
     ) -> config_t:
         """
         The dictionary values are already properly typed
         """
         output = cls()
 
         if (path is not None) and isinstance(path, str):
             path = path_t(path)
 
         output.path = path
-        output._type_hints = nspt.get_annotations(cls)
+        output._types = {
+            _nme: type_t.NewFromType(_hnt)
+            for _nme, _hnt in nspt.get_annotations(cls).items()
+        }
 
         issues = []
         for s_name, section in ini_config.items():
             for p_name, value in section.items():
                 issues.extend(output.Set(_FullName(s_name, p_name), value))
 
         if issues.__len__() > 0:
@@ -81,25 +77,24 @@
             print(f"{path}: Invalid configuration.\n{issues}")
             raise ValueError
 
         return output
 
     def Set(self, name: str, value: str, /) -> list[str]:
         """"""
-        expected_type = self._type_hints[name]
-        typed_value, success = AsComplexInterpretedObject(
-            value, expected_type=expected_type
-        )
+        expected_type = self._types[name]
+        typed_value, success = expected_type.InterpretedValueOf(value)
         if success:
             setattr(self, name, typed_value)
             return []
 
         return [
-            f"{type(typed_value).__name__}: "
-            f'Incompatible type of value "{typed_value}"; Expected={expected_type}.'
+            f"{value}: "
+            f'Invalid value of parameter "{name}"; '
+            f"Expected={expected_type.template_as_str}."
         ]
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/light/conversion.py` & `conf-ini-g-2023.6/conf_ini_g/light/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from configparser import ConfigParser as config_parser_t
 
 from openpyxl import Workbook as workbook_t
 
+from conf_ini_g.extension.path import any_path_h, path_t
 from conf_ini_g.light.ini import NewConfigFromPath as NewConfigFromINIPath
 from conf_ini_g.light.xlsx import NewConfigFromPath as NewConfigFromXLSXPath
-from conf_ini_g.standard.path_extension import any_path_h, path_t
 
 
 def INItoXLSX(
     ini_path: any_path_h, xlsx_path: any_path_h, /, *, should_overwrite: bool = False
 ) -> None:
     """"""
     ini_path, xlsx_path = _AsPaths(ini_path, xlsx_path)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/light/ini.py` & `conf-ini-g-2023.6/conf_ini_g/light/ini.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from configparser import ConfigParser as config_t
 from configparser import ExtendedInterpolation
 
+from conf_ini_g.extension.path import any_path_h
 from conf_ini_g.raw.config import ini_config_h
-from conf_ini_g.standard.path_extension import any_path_h
-
 
 _DEFAULT_OPTIONS = (
     ("delimiters", ("=",)),
     ("comment_prefixes", ("#",)),
     ("inline_comment_prefixes", ("#",)),
     ("interpolation", ExtendedInterpolation()),
 )
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/light/xlsx.py` & `conf-ini-g-2023.6/conf_ini_g/light/xlsx.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from openpyxl import load_workbook as WorkbookFromPath
 
+from conf_ini_g.extension.path import any_path_h
 from conf_ini_g.raw.config import ini_config_h
-from conf_ini_g.standard.path_extension import any_path_h
 
 
 def NewConfigFromPath(path: any_path_h, /) -> ini_config_h:
     """"""
     output = {}
 
     workbook = WorkbookFromPath(filename=path)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/raw/config.py` & `conf-ini-g-2023.6/conf_ini_g/raw/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,17 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import configparser as cfpr
 import sys as sstm
 from typing import Any
 
+from conf_ini_g.extension.path import any_path_h
+from conf_ini_g.extension.string import Flattened
 from conf_ini_g.interface.storage.constant import INI_COMMENT_MARKER
-from conf_ini_g.standard.path_extension import any_path_h
-from conf_ini_g.standard.str_extension import Flattened
-
 
 ini_config_h = dict[str, dict[str, str]]  # Without value interpretation
 raw_config_h = dict[str, dict[str, Any]]  # With interpreted values, and possibly units
 any_raw_config_h = ini_config_h | raw_config_h
 
 
 INI_VALUE_ASSIGNMENT = "="
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/base.py` & `conf-ini-g-2023.6/conf_ini_g/specification/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 import string as strg
 
 from rich.text import Text as text_t
 
-
 WORD_SEPARATOR = "_"
 VALID_CHARACTERS = strg.ascii_letters + strg.digits + WORD_SEPARATOR
 
 
 @dtcl.dataclass(repr=False, eq=False)
 class base_t:
     name: str
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/config.py` & `conf-ini-g-2023.6/conf_ini_g/specification/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 import textwrap as text
 from typing import Sequence
 
 from rich import print as rprint
 from rich.text import Text as text_t
 
 from conf_ini_g.catalog.specification.parameter.choices import choices_t
-from conf_ini_g.specification.parameter.type import type_options_t
+from conf_ini_g.extension.python import SpecificationPath
+from conf_ini_g.extension.type import TypeAsRichStr
+from conf_ini_g.specification.parameter.type import type_t
 from conf_ini_g.specification.parameter.unit import UNIT_SEPARATOR
 from conf_ini_g.specification.section.main import section_t
 from conf_ini_g.specification.section.unit import UNIT_SECTION
-from conf_ini_g.standard.py_extension import SpecificationPath
-from conf_ini_g.standard.type_extension import TypeAsRichStr
 
 
 @dtcl.dataclass(init=False, repr=False, eq=False)
 class config_t(list[section_t]):
     spec_path: str = None
 
     def __init__(self, sections: Sequence[section_t], /) -> None:
@@ -73,22 +73,16 @@
     def _SetControllerChoices(self) -> None:
         """"""
         for section in self:
             if (controller := section.controller) is None:
                 continue
 
             controlling_parameter = self[controller.section][controller.parameter]
-            if controlling_parameter.types is not None:
-                raise TypeError(
-                    f"{controller.section}.{controller.parameter}: "
-                    f"Controller parameter must only have a name specified."
-                )
-
-            controlling_parameter.types = type_options_t.NewFromTypes(
-                (choices_t.NewAnnotatedType(section.controlling_values),)
+            controlling_parameter.type = type_t.NewFromType(
+                choices_t.NewAnnotatedType(section.controlling_values)
             )
 
     def AddUnitSection(self) -> None:
         """"""
         section = section_t(
             name=UNIT_SECTION,
             definition="Unit definitions",
@@ -150,21 +144,14 @@
                             section.controller.parameter
                         ]
                         if controller_parameter.optional:
                             output.append(
                                 f"{section.controller.section}.{section.controller.parameter}: "
                                 f'Optional parameter declared as controller of section "{section.name}"'
                             )
-                        if (controller_parameter.types is not None) and (
-                            controller_parameter.types.__len__() > 1
-                        ):
-                            output.append(
-                                f"{section.controller.section}.{section.controller.parameter}: "
-                                f'Multi-type parameter declared as controller of section "{section.name}"'
-                            )
 
         return output
 
     def _Item(self, key: str | int, /) -> section_t | None:
         """"""
         if isinstance(key, int):
             return list.__getitem__(self, key)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/parameter/annotation.py` & `conf-ini-g-2023.6/conf_ini_g/specification/parameter/annotation.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,59 +26,40 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from typing import Any, ClassVar, Sequence
+from typing import Any
 
 from rich.text import Text as text_t
 
-from conf_ini_g.standard.str_extension import AlignedOnSeparator
-from conf_ini_g.standard.type_extension import NameValueTypeAsRichStr, TypeAsRichStr
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.extension.type import NameValueTypeAsRichStr, TypeAsRichStr
 
 
-py_type_options_h = type | tuple[type, ...]
-
-
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class annotation_t:
-    VALID_PY_TYPES: ClassVar[py_type_options_h] = None
-
-    def Issues(self, py_type: type, /) -> list[str]:
+    def Issues(self) -> list[str]:
         """"""
-        valid_types = self.__class__.VALID_PY_TYPES
-        if (isinstance(valid_types, Sequence) and (py_type in valid_types)) or (
-            py_type is valid_types
-        ):
-            return []
-
-        return [
-            f'{py_type}: Invalid Python type for annotation "{self.__class__.__name__}"; '
-            f"Expected={valid_types}."
-        ]
+        return []
 
     def ValueIsCompliant(self, _: Any, /) -> bool:
         """"""
         return True
 
     def __str__(self) -> str:
         """"""
         return text_t.from_markup(self.__rich__()).plain
 
     def __rich__(self) -> str:
         """"""
         output = [TypeAsRichStr(self)]
 
-        if isinstance(self.__class__.VALID_PY_TYPES, Sequence):
-            output.append(
-                f"    [blue]Valid types[/]@=@{str(self.__class__.VALID_PY_TYPES)[1:-1]}"
-            )
-
         names = (_fld.name for _fld in dtcl.fields(self))
         for name in names:
             value = getattr(self, name)
             output.append(f"    {NameValueTypeAsRichStr(name, value, separator='@=@')}")
 
         output = AlignedOnSeparator(output, "@=@", " = ")
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/parameter/main.py` & `conf-ini-g-2023.6/conf_ini_g/specification/parameter/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,92 +29,83 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
 import dataclasses as dtcl
 import textwrap as text
-from typing import Any, Sequence
+from typing import Any
 
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.extension.type import NameValueTypeAsRichStr, TypeAsRichStr, any_hint_h
 from conf_ini_g.specification.base import base_t
-from conf_ini_g.specification.parameter.type import type_options_t
+from conf_ini_g.specification.parameter.type import ANY_TYPE, type_t
 from conf_ini_g.specification.parameter.value import (
     MISSING_REQUIRED_VALUE,
     missing_required_value_t,
 )
-from conf_ini_g.standard.str_extension import AlignedOnSeparator
-from conf_ini_g.standard.type_extension import (
-    NameValueTypeAsRichStr,
-    TypeAsRichStr,
-    any_hint_h,
-)
 
 
 @dtcl.dataclass(repr=False, eq=False)
 class parameter_t(base_t):
     """
-    types:
-        At instantiation time: any_hint_h | Sequence[any_hint_h].
-        After __post_init__: type_options_t
-    default:
-        Can be None only if types contains None at instantiation time
+    type:
+        At instantiation time: any_hint_h.
+        After __post_init__: type_t
     """
 
-    types: any_hint_h | Sequence[any_hint_h] | type_options_t = None
+    type: any_hint_h | type_t = None
     default: Any = MISSING_REQUIRED_VALUE
 
     def __post_init__(self) -> None:
         """"""
-        if self.types is None:
-            return
-
-        if isinstance(self.types, Sequence):
-            types = self.types
+        if self.type is None:
+            self.type = ANY_TYPE
         else:
-            types = (self.types,)
-
-        self.types = type_options_t.NewFromTypes(types)
+            self.type = type_t.NewFromType(self.type)
 
     def Issues(self) -> list[str]:
         """"""
         output = super().Issues()
 
         if self.optional:
-            output.extend(f"[{self.name}] {_iss}" for _iss in self.types.Issues())
+            output.extend(f"[{self.name}] {_iss}" for _iss in self.type.Issues())
             if self.default is MISSING_REQUIRED_VALUE:
                 output.append(
                     f"{self.name}: Default value of optional parameter cannot be of type "
                     f'"{missing_required_value_t.__name__}"'
                 )
-            elif not self.types.ValueIsCompliant(self.default):
+            elif not self.type.ValueIsCompliant(self.default):
                 output.append(
-                    f'{self.default}: Invalid default value of parameter "{self.name}""'
+                    f'{self.default}: Invalid default value of parameter "{self.name}"'
                 )
         else:
             if not self.basic:
                 output.append(f"{self.name}: Parameter is not basic but not optional")
             if self.default is not MISSING_REQUIRED_VALUE:
                 output.append(
                     f"{self.name}: Default value of mandatory parameter must be of type "
                     f'"{missing_required_value_t.__name__}"'
                 )
 
+        output.extend(self.type.Issues())
+
         return output
 
     @property
     def optional(self) -> bool:
         """"""
         return self.default is not MISSING_REQUIRED_VALUE
 
     def __rich__(self) -> str:
         """"""
         output = [
             TypeAsRichStr(self),
             *text.indent(super().__rich__(), "    ").splitlines(),
-            f"    [blue]Types[/]@=@{self.types.__rich__()}",
+            f"    [blue]Type[/]@=@{self.type.__rich__()}",
             f"    {NameValueTypeAsRichStr('Default', self.default, separator='@=@')}",
             f"    [blue]Optional[/]@=@{self.optional}",
         ]
 
         output = AlignedOnSeparator(output, "@=@", " = ")
 
         return "\n".join(output)
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/parameter/unit.py` & `conf-ini-g-2023.6/conf_ini_g/specification/parameter/unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,17 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from math import pi as PI
-from typing import Annotated
 
-from conf_ini_g.catalog.specification.parameter.number import number_in_str_t
 from conf_ini_g.specification.parameter.main import parameter_t
-from conf_ini_g.specification.parameter.type import type_options_t
-
+from conf_ini_g.specification.parameter.type import type_t
 
 UNIT_SEPARATOR = "'"
 
 _STD_UNIT_CONVERSIONS = (
     # unit, unit name, parent unit (None if none), conversion factor (1.0 if None)
     ("si", "site", None, 1.0),  # Synonym for sample, pixel, voxel...
     #
@@ -66,24 +63,22 @@
     ("ms", "millisecond", "s", 1.0e-3),
     ("us", "microsecond", "s", 1.0e-6),
     ("ns", "nanosecond", "s", 1.0e-9),
 )
 STD_UNIT_CONVERSIONS = {_elm[0]: _elm[-1] for _elm in _STD_UNIT_CONVERSIONS}
 
 
-@dtcl.dataclass(repr=False, eq=False)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
 class unit_t(parameter_t):
     def __post_init__(self) -> None:
         """
         Unit parameter are never part of a specification. They can appear in INI
         documents, and are therefore only instantiated programmatically.
         """
-        self.types = type_options_t.NewFromTypes(
-            (int, float, Annotated[str, number_in_str_t()])
-        )
+        self.type = type_t.NewFromType(float)
 
     def Issues(self) -> list[str]:
         """"""
         if self.name in STD_UNIT_CONVERSIONS.keys():
             return [
                 f"{self.name}: Redefinition of a standard unit; Please use another unit name."
             ]
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/parameter/value.py` & `conf-ini-g-2023.6/conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,38 +25,26 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import PyQt6.QtWidgets as wdgt
 
-class missing_required_value_t:
-    TEXT = "MISSING REQUIRED VALUE"
 
-    def __str__(self) -> str:
-        """"""
-        return self.__class__.TEXT
+class path_chooser_wgt_t(wdgt.QFileDialog):
+    """"""
 
-    def __rich__(self) -> str:
+    def __init__(self, caption: str, /, *, extension_filter: str = None):
         """"""
-        return f"[red]{self.__class__.TEXT}[/]"
-
-
-class invalid_value_t:
-    """
-    Do not use invalid_value_t = object, for example, otherwise isinstance returns True for anything.
-    """
+        if extension_filter is None:
+            extension_filter = "Any files (*)"
+        super().__init__(caption=caption, filter=extension_filter)
 
-    TEXT = "INVALID VALUE"
-
-    def __str__(self) -> str:
+    def SelectedFile(self) -> str:
         """"""
-        return self.__class__.TEXT
+        return self.selectedFiles()[0]
 
-    def __rich__(self) -> str:
+    def RunAndGetClosingStatus(self) -> int:
         """"""
-        return f"[red]{self.__class__.TEXT}[/]"
-
-
-MISSING_REQUIRED_VALUE = missing_required_value_t()
-INVALID_VALUE = invalid_value_t()
+        return self.exec()
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/section/main.py` & `conf-ini-g-2023.6/conf_ini_g/specification/section/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,20 @@
 import textwrap as text
 from typing import Any
 from typing import NamedTuple as named_tuple_t
 from typing import Sequence
 
 from rich.text import Text as text_t
 
+from conf_ini_g.extension.string import AlignedOnSeparator
+from conf_ini_g.extension.type import TypeAsRichStr
 from conf_ini_g.specification.base import base_t
 from conf_ini_g.specification.parameter.main import parameter_t
 from conf_ini_g.specification.parameter.unit import unit_t
 from conf_ini_g.specification.section.unit import IsUnitSection
-from conf_ini_g.standard.str_extension import AlignedOnSeparator
-from conf_ini_g.standard.type_extension import UNIVERSAL_ANNOTATED_TYPES, TypeAsRichStr
-
 
 PARAMETERS = "parameters"
 
 
 @dtcl.dataclass(init=False, repr=False, eq=False)  # Cannot have __init__ method
 class controller_t(named_tuple_t):
     section: str = None
@@ -101,16 +100,14 @@
             parameter = parameter_t(
                 name=name,
                 definition="Programmatic parameter",
                 description="This parameter is not part of the specification. "
                 "It was added programmatically because it was found in the INI document or "
                 "passed as a command-line argument",
                 basic=self.basic,
-                types=UNIVERSAL_ANNOTATED_TYPES,
-                default=None,
             )
         self.append(parameter)
 
         return parameter
 
     @property
     def all_parameters(self) -> Sequence[parameter_t]:
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/specification/section/unit.py` & `conf-ini-g-2023.6/conf_ini_g/specification/section/unit.py`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/conf_ini_g/standard/path_extension.py` & `conf-ini-g-2023.6/conf_ini_g/extension/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from pathlib import Path as path_t
 
-
 any_path_h = str | path_t
 
 
 def ValidateInputPath(
     path: path_t, /, *, should_raise_on_error: bool = False
 ) -> str | None:
     """"""
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/standard/py_extension.py` & `conf-ini-g-2023.6/conf_ini_g/extension/python.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,25 +28,31 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import ast as bstr
 import inspect as nspt
 import sys as sstm
-
-from conf_ini_g.standard.path_extension import path_t
+from pathlib import Path as path_t
 
 
 def SpecificationPath(element: object, /, *, relative_to_home: bool = True) -> str:
     """"""
     found = []
     for module in sstm.modules.copy().values():
         for attribute in dir(module):
-            value = getattr(module, attribute)
-            if value is element:
+            # It can happen that "attribute" ends up not being an attribute of "module",
+            # for example with "single" in scipy.linalg.matfuncs. Hence, the default
+            # value in getattr. The getattr call can even fail, for example with
+            # "Viewer" in napari. Hence the try-expect.
+            try:
+                value = getattr(module, attribute, None)
+            except:
+                value = None
+            if (value is not None) and (value is element):
                 code = nspt.getsource(module)
                 tree = bstr.parse(code)
                 is_imported = False
                 for node in bstr.walk(tree):
                     if isinstance(node, bstr.ImportFrom):
                         for alias in node.names:
                             if (
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/standard/str_extension.py` & `conf-ini-g-2023.6/conf_ini_g/extension/type.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,198 +27,205 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from __future__ import annotations
 
-import ast as asgt
 import dataclasses as dtcl
-import textwrap as text
-from types import GenericAlias, UnionType
-from typing import Any, Iterable, Sequence
-
-from conf_ini_g.standard.type_extension import (
-    HintTreeFromTypeHint,
-    hint_node_t,
-    none_t,
-    raw_hint_h,
-)
+from types import EllipsisType, GenericAlias, NoneType, UnionType
+from typing import Annotated, Any, Iterable, Sequence, get_args, get_origin
 
+from conf_ini_g.extension.python import SpecificationPath
 
-TRUE_VALUES = ("true", "yes", "on")
-FALSE_VALUES = ("false", "no", "off")
+complex_hint_h = GenericAlias | UnionType
+raw_hint_h = type | Any | complex_hint_h
+annotated_hint_t = type(Annotated[object, None])
+any_hint_h = raw_hint_h | annotated_hint_t
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
-class _value_node_t:
+class hint_node_t:
+    type: type | EllipsisType | None  # None=OR
+    elements: tuple[hint_node_t, ...] | None = None
+
+
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class value_node_t:
     consolidated: Any
     type: type | None = None
-    elements: tuple[_value_node_t, ...] | None = None
+    elements: tuple[value_node_t, ...] | None = None
 
     def __post_init__(self) -> None:
         """"""
         self.type = type(self.consolidated)
 
 
-def Flattened(string: str, /) -> str:
+def TypeHintOfAnnotated(annotated_hint: annotated_hint_t, /) -> raw_hint_h:
     """"""
-    return text.dedent(string).replace("\n", "; ")
+    return annotated_hint.__args__[0]
 
 
-def AlignedOnSeparator(
-    string: str | Sequence[str], separator: str, replacement: str, /
-) -> str | tuple[str, ...] | list[str]:
+def AnnotationsOfType(annotated_hint: annotated_hint_t, /) -> Sequence[Any]:
     """"""
-    if should_return_str := isinstance(string, str):
-        lines = string.splitlines()
-    else:
-        lines = string
-    indices = tuple(_lne.find(separator) for _lne in lines)
-    longest = max(indices)
-
-    output = (
-        _lne.replace(separator, (longest - _lgt) * " " + replacement, 1)
-        if _lgt > 0
-        else _lne
-        for _lne, _lgt in zip(lines, indices)
-    )
-    if should_return_str:
-        return "\n".join(output)
-    elif isinstance(string, tuple):
-        return tuple(output)
-    else:
-        return list(output)
+    return tuple(annotated_hint.__metadata__)
 
 
-def AsInterpretedObject(
-    string: str, /, *, expected_type: type | None = None
-) -> tuple[Any, bool]:
+def HintTreeFromTypeHint(type_hint: raw_hint_h | EllipsisType | None, /) -> hint_node_t:
     """
-    expected_type: Must not be passed explicitly as None since None is interpreted as
-    "no specific expected type". When expecting None, pass none_t.
+    Note that type hints cannot translate into hint trees with an OR-node having a child
+    OR-node. For example: str | (int | float) is interpreted as str | int | float. This
+    is important when creating a type selector for multitype parameters since only
+    direct child nodes are taken into account for widget creation, so these nodes must
+    be types, not an OR subtree.
     """
-    if expected_type is None:
-        try:
-            value = asgt.literal_eval(string)
-        except (SyntaxError, ValueError):
-            value = string
-
-        return value, True
-
-    failed_interpretation = None, False
-    lowered = string.lower()
-
-    if expected_type is none_t:
-        return None, (lowered == "none")
-
-    if expected_type is bool:
-        if lowered in TRUE_VALUES:
-            return True, True
-        if lowered in FALSE_VALUES:
-            return False, True
-        return failed_interpretation
-
-    # The expected type might be instantiable from a string, e.g.: float("1.0").
-    # However, a success does not mean that the interpretation is valid, e.g.:
-    # tuple("(1, 2, 3)"). To confirm that a success is indeed a correct interpretation,
-    # the string representation of the interpreted value is compared with the string.
-    # This is not a perfect test, so "literal_eval" might still be called below.
-    try:
-        value = expected_type(string)
-        success = str(value).replace(" ", "") == string.replace(" ", "")
-    except:
-        value, success = failed_interpretation
-    if success:
-        return value, True
-
-    try:
-        value = asgt.literal_eval(string)
-        success = type(value) is expected_type
-        if not success:
-            value = None
-    except (SyntaxError, ValueError):
-        value, success = failed_interpretation
-
-    return value, success
-
-
-def AsComplexInterpretedObject(
-    string: str,
-    /,
-    *,
-    expected_type: raw_hint_h | hint_node_t | None = None,
-) -> tuple[Any, bool]:
-    """"""
-    if isinstance(expected_type, (GenericAlias, UnionType, hint_node_t)):
-        value, _ = AsInterpretedObject(string)
-        value_tree = _ValueTreeOfValue(value)
-        if isinstance(expected_type, hint_node_t):
-            hint_tree = expected_type
-        else:
-            hint_tree = HintTreeFromTypeHint(expected_type)
-        if _CastValueTree(value_tree, hint_tree):
-            return _ValueFromValueTree(value_tree), True
-        else:
-            return None, False
+    if type_hint is None:
+        return hint_node_t(type=NoneType)
+
+    if (origin := get_origin(type_hint)) is None:
+        return hint_node_t(type=type_hint)
+
+    # Handled types: list, set, tuple, with sets using the dict delimiters { and }.
+    if origin is dict:
+        raise TypeError(f"{origin.__name__}: Unhandled type.")
+
+    elements = tuple(HintTreeFromTypeHint(_elm) for _elm in get_args(type_hint))
+
+    if origin is UnionType:
+        return hint_node_t(type=None, elements=elements)
 
-    return AsInterpretedObject(string, expected_type=expected_type)
+    return hint_node_t(type=origin, elements=elements)
 
 
-def _ValueTreeOfValue(value: Any, /) -> _value_node_t:
+def TypeTemplateFromTypeHint(type_hint: raw_hint_h | EllipsisType | None, /) -> type:
     """"""
-    if isinstance(value, Iterable) and not isinstance(value, str):
-        elements = tuple(_ValueTreeOfValue(_elm) for _elm in value)
-        return _value_node_t(consolidated=value, elements=elements)
+    if type_hint is None:
+        return NoneType
+
+    if (origin := get_origin(type_hint)) is None:
+        return type_hint
+
+    # Handled types: list, set, tuple, with sets using the dict delimiters { and }.
+    if origin is dict:
+        raise TypeError(f"{origin.__name__}: Unhandled type.")
+
+    elements = tuple(TypeTemplateFromTypeHint(_elm) for _elm in get_args(type_hint))
+
+    if origin is UnionType:
+        return {_key: _elm for _key, _elm in enumerate(elements)}
+
+    return origin(elements)
+
+
+def ValueMatchesTypeHint(
+    value: Any, type_hint: raw_hint_h | hint_node_t, /
+) -> tuple[bool, value_node_t]:
+    """"""
+    value_tree = _ValueTreeOfValue(value)
+
+    if type_hint is Any:
+        return True, value_tree
+
+    if isinstance(type_hint, hint_node_t):
+        hint_tree = type_hint
+    elif isinstance(type_hint, complex_hint_h):
+        hint_tree = HintTreeFromTypeHint(type_hint)
+    else:
+        return isinstance(value, type_hint), value_tree
 
-    return _value_node_t(consolidated=value)
+    return _CastValueTree(value_tree, hint_tree), value_tree
 
 
-def _ValueFromValueTree(value_tree: _value_node_t, /) -> Any:
+def ValueFromValueTree(value_tree: value_node_t, /) -> Any:
     """"""
-    if isinstance(value_tree.consolidated, Iterable) and not isinstance(
-        value_tree.consolidated, str
-    ):
-        elements = (_ValueFromValueTree(_elm) for _elm in value_tree.elements)
+    value = value_tree.consolidated
+
+    if value is None:
+        return None
+
+    if isinstance(value, Iterable) and not isinstance(value, str):
+        elements = (ValueFromValueTree(_elm) for _elm in value_tree.elements)
         return value_tree.type(elements)
 
-    return value_tree.type(value_tree.consolidated)
+    return value_tree.type(value)
+
+
+def TypeAsRichStr(instance: Any, /, *, relative_to_home: bool = True) -> str:
+    """"""
+    return (
+        f"[bold magenta]{type(instance).__name__}[/]"
+        f"[gray]@"
+        f"{SpecificationPath(type(instance), relative_to_home=relative_to_home)}:[/]"
+    )
+
+
+def NameValueTypeAsRichStr(name: str, value: Any, /, *, separator: str = "=") -> str:
+    """"""
+    if isinstance(value, Sequence) and (value.__len__() == 0):
+        value = "[cyan]<empty>[/]"
+
+    return f"[blue]{name}[/]{separator}{value}[yellow]:{type(value).__name__}[/]"
 
 
-def _CastValueTree(value_node: _value_node_t, hint_node: hint_node_t, /) -> bool:
+def _ValueTreeOfValue(value: Any, /) -> value_node_t:
     """"""
-    if hint_node.type is None:  # Or
-        if any(_CastValueTree(value_node, _elm) for _elm in hint_node.elements):
+    if isinstance(value, Iterable) and not isinstance(value, str):
+        elements = tuple(_ValueTreeOfValue(_elm) for _elm in value)
+        return value_node_t(consolidated=value, elements=elements)
+
+    return value_node_t(consolidated=value)
+
+
+def _CastValueTree(value_node: value_node_t, hint_node: hint_node_t, /) -> bool:
+    """"""
+    hn_type = hint_node.type
+    hn_elements = hint_node.elements
+
+    if hn_type is Any:
+        return True
+
+    if hn_type is NoneType:
+        if value_node.consolidated is None:
             return True
         else:
             return False
 
-    if not isinstance(value_node.consolidated, hint_node.type):
+    if hn_type is None:  # Or
+        if any(_CastValueTree(value_node, _elm) for _elm in hn_elements):
+            return True
+        else:
+            return False
+
+    if not isinstance(value_node.consolidated, hn_type):
         try:
-            _ = hint_node.type(value_node.consolidated)
-            success = True
+            converted = hn_type(value_node.consolidated)
+            success = str(converted).replace(" ", "") == str(
+                value_node.consolidated
+            ).replace(" ", "")
         except:
             success = False
         if not success:
             return False
-    if hint_node.elements is None:
-        value_node.type = hint_node.type
+    if (value_node.elements is None) and (hn_elements is None):
+        value_node.type = hn_type
         return True
 
+    if (value_node.elements is None) or (hn_elements is None):
+        return False
+
     n_value_children = value_node.elements.__len__()
-    n_hint_elements = hint_node.elements.__len__()
-    has_ellipsis = (n_hint_elements == 2) and (hint_node.elements[1].type is Ellipsis)
-    should_fake_ellipsis = (n_hint_elements == 1) and issubclass(
-        hint_node.type, (list, set)
-    )
+    n_hint_elements = hn_elements.__len__()
+    has_ellipsis = (n_hint_elements == 2) and (hn_elements[1].type is Ellipsis)
+    should_fake_ellipsis = (n_hint_elements == 1) and issubclass(hn_type, (list, set))
     if has_ellipsis or should_fake_ellipsis or (n_value_children == n_hint_elements):
         if has_ellipsis or should_fake_ellipsis:
-            hint_elements = n_value_children * (hint_node.elements[0],)
+            hint_elements = n_value_children * (hn_elements[0],)
         else:
-            hint_elements = hint_node.elements
+            hint_elements = hn_elements
         for value_elm, hint_elm in zip(value_node.elements, hint_elements):
             if not _CastValueTree(value_elm, hint_elm):
                 return False
-        value_node.type = hint_node.type
+
+        value_node.type = hn_type
         return True
 
     return False
```

### Comparing `conf-ini-g-2023.5/conf_ini_g/version.py` & `conf-ini-g-2023.6/conf_ini_g/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.5"
+__version__ = "2023.6"
```

### Comparing `conf-ini-g-2023.5/conf_ini_g.egg-info/PKG-INFO` & `conf-ini-g-2023.6/conf_ini_g.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-ini-g
-Version: 2023.5
+Version: 2023.6
 Summary: App Configuration in INI format with Automatic Command-Line Parser and Graphical Interface Generation
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/conf-ini-g/
```

### Comparing `conf-ini-g-2023.5/conf_ini_g.egg-info/SOURCES.txt` & `conf-ini-g-2023.6/conf_ini_g.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,57 @@
 conf_ini_g.egg-info/dependency_links.txt
 conf_ini_g.egg-info/requires.txt
 conf_ini_g.egg-info/top_level.txt
 conf_ini_g/catalog/interface/screen/library/pyqt5/constant.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/main.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/button.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/choices.py
+conf_ini_g/catalog/interface/screen/library/pyqt5/widget/label.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/main.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/path_chooser.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/scroll_container.py
 conf_ini_g/catalog/interface/screen/library/pyqt5/widget/text.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/constant.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/main.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/button.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/choices.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/label.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/main.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/path_chooser.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/scroll_container.py
+conf_ini_g/catalog/interface/screen/library/pyqt6/widget/text.py
 conf_ini_g/catalog/interface/screen/parameter/boolean.py
 conf_ini_g/catalog/interface/screen/parameter/choices.py
+conf_ini_g/catalog/interface/screen/parameter/directory.py
+conf_ini_g/catalog/interface/screen/parameter/multitype.py
 conf_ini_g/catalog/interface/screen/parameter/none.py
 conf_ini_g/catalog/interface/screen/parameter/path.py
 conf_ini_g/catalog/interface/screen/parameter/sequence.py
 conf_ini_g/catalog/interface/screen/parameter/text.py
 conf_ini_g/catalog/specification/parameter/boolean.py
 conf_ini_g/catalog/specification/parameter/choices.py
 conf_ini_g/catalog/specification/parameter/number.py
 conf_ini_g/catalog/specification/parameter/path.py
 conf_ini_g/catalog/specification/parameter/sequence.py
+conf_ini_g/extension/path.py
+conf_ini_g/extension/python.py
+conf_ini_g/extension/string.py
+conf_ini_g/extension/type.py
 conf_ini_g/instance/config.py
 conf_ini_g/instance/parameter/base.py
 conf_ini_g/instance/parameter/main.py
 conf_ini_g/instance/parameter/unit.py
 conf_ini_g/interface/console/__init__.py
 conf_ini_g/interface/console/config.py
+conf_ini_g/interface/screen/backend.py
 conf_ini_g/interface/screen/config.py
 conf_ini_g/interface/screen/generic.py
 conf_ini_g/interface/screen/section.py
 conf_ini_g/interface/screen/parameter/main.py
 conf_ini_g/interface/screen/parameter/path_chooser.py
-conf_ini_g/interface/screen/parameter/type_selector.py
 conf_ini_g/interface/storage/config.py
 conf_ini_g/interface/storage/constant.py
 conf_ini_g/light/config.py
 conf_ini_g/light/conversion.py
 conf_ini_g/light/ini.py
 conf_ini_g/light/xlsx.py
 conf_ini_g/raw/config.py
@@ -54,12 +70,8 @@
 conf_ini_g/specification/parameter/annotation.py
 conf_ini_g/specification/parameter/main.py
 conf_ini_g/specification/parameter/type.py
 conf_ini_g/specification/parameter/unit.py
 conf_ini_g/specification/parameter/value.py
 conf_ini_g/specification/section/main.py
 conf_ini_g/specification/section/unit.py
-conf_ini_g/standard/path_extension.py
-conf_ini_g/standard/py_extension.py
-conf_ini_g/standard/str_extension.py
-conf_ini_g/standard/type_extension.py
 documentation/wiki/description.asciidoc
```

### Comparing `conf-ini-g-2023.5/documentation/wiki/description.asciidoc` & `conf-ini-g-2023.6/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `conf-ini-g-2023.5/setup.py` & `conf-ini-g-2023.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,30 +74,32 @@
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
     f"{IMPORT_NAME}.catalog.interface",
     f"{IMPORT_NAME}.catalog.interface.screen",
     f"{IMPORT_NAME}.catalog.interface.screen.library",
     f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5",
     f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt5.widget",
+    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt6",
+    f"{IMPORT_NAME}.catalog.interface.screen.library.pyqt6.widget",
     f"{IMPORT_NAME}.catalog.interface.screen.parameter",
     f"{IMPORT_NAME}.catalog.specification",
     f"{IMPORT_NAME}.catalog.specification.parameter",
+    f"{IMPORT_NAME}.extension",
     f"{IMPORT_NAME}.instance",
     f"{IMPORT_NAME}.instance.parameter",
     f"{IMPORT_NAME}.interface",
     f"{IMPORT_NAME}.interface.console",
     f"{IMPORT_NAME}.interface.screen",
     f"{IMPORT_NAME}.interface.screen.parameter",
     f"{IMPORT_NAME}.interface.storage",
     f"{IMPORT_NAME}.light",
     f"{IMPORT_NAME}.raw",
     f"{IMPORT_NAME}.specification",
     f"{IMPORT_NAME}.specification.parameter",
     f"{IMPORT_NAME}.specification.section",
-    f"{IMPORT_NAME}.standard",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
     f"{IMPORT_NAME}.test",
 )
 ENTRY_POINTS = {}
 
@@ -178,12 +180,11 @@
             "Source": repository_url,
         },
         #
         packages=PACKAGES,
         entry_points=ENTRY_POINTS,
         python_requires=f">={PY_VERSION}",
         install_requires=[
-            "PyQt5",
             "rich",
             "openpyxl",
         ],
     )
```

