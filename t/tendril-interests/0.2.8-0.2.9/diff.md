# Comparing `tmp/tendril-interests-0.2.8.tar.gz` & `tmp/tendril-interests-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-interests-0.2.8.tar", last modified: Tue Mar 28 11:21:34 2023, max compression
+gzip compressed data, was "dist/tendril-interests-0.2.9.tar", last modified: Thu Mar 30 03:19:56 2023, max compression
```

## Comparing `tendril-interests-0.2.8.tar` & `tendril-interests-0.2.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.2.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3246 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.766980 tendril-interests-0.2.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2137 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-02-18 15:16:12.000000 tendril-interests-0.2.8/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.2.8/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17841 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/apiserver/templates/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.2.8/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.2.8/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    12188 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/authz/roles/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.2.8/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3851 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6501 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/common/interests/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.2.8/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.770980 tendril-interests-0.2.8/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.8/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.2.8/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9884 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/db/controllers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.2.8/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-03-27 15:41:29.000000 tendril-interests-0.2.8/src/tendril/db/models/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.2.8/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    15664 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5735 2023-03-27 17:44:29.000000 tendril-interests-0.2.8/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.2.8/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.2.8/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3780 2023-03-15 16:01:38.000000 tendril-interests-0.2.8/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1596 2023-02-18 15:08:06.000000 tendril-interests-0.2.8/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-28 11:21:34.000000 tendril-interests-0.2.8/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1775 2023-03-28 11:21:34.000000 tendril-interests-0.2.8/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-28 11:21:34.000000 tendril-interests-0.2.8/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      558 2023-03-28 11:21:34.000000 tendril-interests-0.2.8/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-28 11:21:34.000000 tendril-interests-0.2.8/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-28 11:21:34.774980 tendril-interests-0.2.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.2.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.2.9/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3246 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.032757 tendril-interests-0.2.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.9/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.9/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2137 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-02-18 15:16:12.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17841 2023-03-30 03:05:21.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.2.9/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.2.9/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    12188 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/authz/roles/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.2.9/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3851 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6577 2023-03-30 02:19:26.000000 tendril-interests-0.2.9/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.2.9/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.9/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.2.9/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9884 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/db/controllers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.2.9/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-03-27 15:41:29.000000 tendril-interests-0.2.9/src/tendril/db/models/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.2.9/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    15664 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5735 2023-03-27 17:44:29.000000 tendril-interests-0.2.9/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.2.9/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4140 2023-03-30 03:05:21.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1596 2023-02-18 15:08:06.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1775 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      558 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tox.ini
```

### Comparing `tendril-interests-0.2.8/.gitignore` & `tendril-interests-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/.readthedocs.yml` & `tendril-interests-0.2.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/.travis.yml` & `tendril-interests-0.2.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/LICENSE` & `tendril-interests-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/PKG-INFO` & `tendril-interests-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
```

### Comparing `tendril-interests-0.2.8/README.rst` & `tendril-interests-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/Makefile` & `tendril-interests-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/_static/custom.css` & `tendril-interests-0.2.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/_static/favicon.ico` & `tendril-interests-0.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/_static/logo.png` & `tendril-interests-0.2.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/_static/logo_packed.png` & `tendril-interests-0.2.9/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/_templates/about.html` & `tendril-interests-0.2.9/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/conf.py` & `tendril-interests-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/index.rst` & `tendril-interests-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/docs/installation.rst` & `tendril-interests-0.2.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/setup.py` & `tendril-interests-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.2.9/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.2.9/src/tendril/apiserver/templates/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/authz/roles/interests.py` & `tendril-interests-0.2.9/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.2.9/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/common/interests/memberships.py` & `tendril-interests-0.2.9/src/tendril/common/interests/memberships.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
             itype_df = self.df.filter(polars.col("type") == itype[0])\
                               .select(['interest.id', 'interest.name',
                                        'role.name', 'role.delegated', 'role.inherited'])
             rv[itype[0]] = self._pack_itype_memberships(itype_df)
         return rv
 
     def interest_ids(self):
+        if not self.df.select(polars.count()).item():
+            return []
         return self.df.select(polars.col('interest.id').unique()).rows()[0]
 
 
 def _rewrap_interest(model):
     from tendril.interests import type_codes
     type_name = model.type
     return type_codes[type_name](model)
```

### Comparing `tendril-interests-0.2.8/src/tendril/config/__init__.py` & `tendril-interests-0.2.9/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/config/interests.py` & `tendril-interests-0.2.9/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/db/controllers/interests.py` & `tendril-interests-0.2.9/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/db/models/interests.py` & `tendril-interests-0.2.9/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/interests/base.py` & `tendril-interests-0.2.9/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/interests/manager.py` & `tendril-interests-0.2.9/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril/libraries/interests/base.py` & `tendril-interests-0.2.9/src/tendril/libraries/interests/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from tendril.db.controllers.interests import get_interests
 from tendril.db.controllers.interests import get_user_memberships
 from tendril.interests import InterestBase
 from tendril.apiserver.templates.interests import InterestLibraryRouterGenerator
 
 from tendril.common.interests.memberships import user_memberships
 from tendril.common.interests.exceptions import TypeMismatchError
+from tendril.common.interests.exceptions import InterestNotFound
+from sqlalchemy.exc import NoResultFound
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 class GenericInterestLibrary(object):
     interest_class = InterestBase
@@ -57,16 +59,23 @@
                 include_inherited=include_inherited,
             ).interest_ids()
             return [self.interest_class(get_interest(id=x, session=session))
                     for x in iids]
 
     @with_db
     def item(self, id=None, name=None, session=None):
-        return self.interest_class(
-            get_interest(id=id, name=name, type=self.interest_class, session=session))
+        try:
+            return self.interest_class(
+                get_interest(id=id, name=name, type=self.interest_class, session=session))
+        except NoResultFound:
+            if not name:
+                name = '<unspecified>'
+            if not id:
+                id = '<unspecified>'
+            raise InterestNotFound(type_name=self.type_name, name=name, id=id)
 
     @with_db
     def add_item(self, item, session=None):
         if item.type != self.interest_class.model.type_name:
             raise TypeMismatchError(item.type, self.interest_class.model.type_name)
         created = self.interest_class(item.name, must_create=True, session=session)
         if item.descriptive_name:
```

### Comparing `tendril-interests-0.2.8/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.2.9/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.2.9/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 License: UNKNOWN
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
```

### Comparing `tendril-interests-0.2.8/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.2.9/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.2.9/src/tendril_interests.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/tests/coveralls.py` & `tendril-interests-0.2.9/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.8/tox.ini` & `tendril-interests-0.2.9/tox.ini`

 * *Files identical despite different names*

