# Comparing `tmp/invenio-app-1.3.4.tar.gz` & `tmp/invenio-app-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-app-1.3.4.tar", last modified: Wed Apr  6 13:32:09 2022, max compression
+gzip compressed data, was "dist/invenio-app-1.4.0.tar", last modified: Mon Jun 26 12:31:41 2023, max compression
```

## Comparing `invenio-app-1.3.4.tar` & `invenio-app-1.4.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-06 13:32:05.000000 invenio-app-1.3.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-06 13:32:05.000000 invenio-app-1.3.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-04-06 13:32:05.000000 invenio-app-1.3.4/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-04-06 13:32:05.000000 invenio-app-1.3.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-06 13:32:05.000000 invenio-app-1.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-04-06 13:32:05.000000 invenio-app-1.3.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-04-06 13:32:05.000000 invenio-app-1.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-04-06 13:32:05.000000 invenio-app-1.3.4/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-06 13:32:05.000000 invenio-app-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-04-06 13:32:05.000000 invenio-app-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-04-06 13:32:09.000000 invenio-app-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-04-06 13:32:05.000000 invenio-app-1.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9883 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6991 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-04-06 13:32:05.000000 invenio-app-1.3.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app/
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/celery.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6671 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4795 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/limiter.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/wsgi_rest.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-04-06 13:32:05.000000 invenio-app-1.3.4/invenio_app/wsgi_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-06 13:32:09.000000 invenio-app-1.3.4/invenio_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-06 13:32:05.000000 invenio-app-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-04-06 13:32:05.000000 invenio-app-1.3.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-04-06 13:32:05.000000 invenio-app-1.3.4/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      568 2022-04-06 13:32:05.000000 invenio-app-1.3.4/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-04-06 13:32:09.000000 invenio-app-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-04-06 13:32:05.000000 invenio-app-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4000 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/instance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/instance/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/instance/templates/bootstrap3/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/bootstrap3/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/bootstrap3/fallback.html
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/fallback.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/only.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/instance/templates/semantic-ui/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/semantic-ui/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/instance/templates/semantic-ui/instance.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/templates/bootstrap3/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/bootstrap3/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/bootstrap3/fallback.html
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/fallback.html
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/only.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 13:32:09.000000 invenio-app-1.3.4/tests/templates/semantic-ui/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/semantic-ui/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/templates/semantic-ui/noinstance.html
--rw-r--r--   0 runner    (1001) docker     (121)     5556 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_templating.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-04-06 13:32:05.000000 invenio-app-1.3.4/tests/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-26 12:31:34.000000 invenio-app-1.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-26 12:31:34.000000 invenio-app-1.4.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-26 12:31:34.000000 invenio-app-1.4.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-06-26 12:31:34.000000 invenio-app-1.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-06-26 12:31:34.000000 invenio-app-1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-06-26 12:31:34.000000 invenio-app-1.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-06-26 12:31:34.000000 invenio-app-1.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-06-26 12:31:34.000000 invenio-app-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-26 12:31:34.000000 invenio-app-1.4.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-26 12:31:34.000000 invenio-app-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-06-26 12:31:34.000000 invenio-app-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-06-26 12:31:41.000000 invenio-app-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-26 12:31:34.000000 invenio-app-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7429 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10048 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6991 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-26 12:31:34.000000 invenio-app-1.4.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app/
+-rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6650 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/wsgi_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-26 12:31:34.000000 invenio-app-1.4.0/invenio_app/wsgi_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-26 12:31:41.000000 invenio-app-1.4.0/invenio_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-26 12:31:34.000000 invenio-app-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-26 12:31:34.000000 invenio-app-1.4.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      520 2023-06-26 12:31:34.000000 invenio-app-1.4.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-26 12:31:41.000000 invenio-app-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-26 12:31:34.000000 invenio-app-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/instance/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/instance/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/instance/templates/bootstrap3/
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/bootstrap3/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/bootstrap3/fallback.html
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/fallback.html
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/only.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/instance/templates/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/semantic-ui/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/instance/templates/semantic-ui/instance.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/templates/bootstrap3/
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/bootstrap3/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/bootstrap3/fallback.html
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/fallback.html
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/only.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 12:31:41.000000 invenio-app-1.4.0/tests/templates/semantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/semantic-ui/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/templates/semantic-ui/noinstance.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5639 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4808 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_templating.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-26 12:31:34.000000 invenio-app-1.4.0/tests/test_wsgi.py
```

### Comparing `invenio-app-1.3.4/.github/workflows/pypi-release.yml` & `invenio-app-1.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/.github/workflows/tests.yml` & `invenio-app-1.4.0/.github/workflows/tests.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2020 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 name: CI
 
 on:
@@ -25,38 +26,39 @@
 
 jobs:
   Tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
           python-version: [3.7, 3.8, 3.9]
-          requirements-level: [min, pypi]
-
+          requirements-level: [pypi]
+    env:
+      EXTRAS: tests
     steps:
       - name: Checkout
         uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Generate dependencies
         run: |
-          python -m pip install --upgrade pip setuptools py wheel redis requirements-builder
-          requirements-builder -e tests ${{ matrix.requirements-file }} --level=${{ matrix.requirements-level }} setup.py > .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt
+          pip install wheel requirements-builder
+          requirements-builder -e "$EXTRAS" ${{ matrix.requirements-file }} --level=${{ matrix.requirements-level }} setup.py > .${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt
 
       - name: Cache pip
         uses: actions/cache@v2
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('.${{ matrix.requirements-level }}-${{ matrix.python-version }}-requirements.txt') }}
 
       - name: Install dependencies
         run: |
           pip install -r .${{matrix.requirements-level}}-${{ matrix.python-version }}-requirements.txt
-          pip install -e .[tests]
+          pip install -e .[$EXTRAS]
           pip freeze
 
       - name: Run tests
         run: |
           ./run-tests.sh
```

### Comparing `invenio-app-1.3.4/CHANGES.rst` & `invenio-app-1.4.0/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2017-2019 CERN.
+    Copyright (C) 2017-2023 CERN.
+    Copyright (C) 2023 Graz University of Technology.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.4.0 (released 2023-06-26)
+
+- Adds ``invenio_base.finalize_app`` and ``invenio_base.api_finalize_app``
+  entry points to the creation of the factory function ``create_app`` and
+  ``create_api`` to overcome the deprecation of ``before_(app_)first_request``
+  in Flask>=2.3.0
+
 Version 1.3.4 (released 2022-04-06)
 
 - Added support for Flask-Security-Invenio.
 
 Version 1.3.3 (released 2021-12-06)
 
 - Pinned Limits library to align with Flask-Limiter.
```

### Comparing `invenio-app-1.3.4/CONTRIBUTING.rst` & `invenio-app-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/LICENSE` & `invenio-app-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/MANIFEST.in` & `invenio-app-1.4.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 recursive-include tests *.py
 recursive-include tests *.html
 recursive-include .github/workflows *.yml
+include .git-blame-ignore-revs
```

### Comparing `invenio-app-1.3.4/PKG-INFO` & `invenio-app-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app
-Version: 1.3.4
+Version: 1.4.0
 Summary: WSGI, Celery and CLI applications for Invenio flavours.
 Home-page: https://github.com/inveniosoftware/invenio-app
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -32,22 +32,30 @@
         WSGI, Celery and CLI applications for Invenio flavours.
         
         Further documentation is available on
         https://invenio-app.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2017-2019 CERN.
+            Copyright (C) 2017-2023 CERN.
+            Copyright (C) 2023 Graz University of Technology.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.4.0 (released 2023-06-26)
+        
+        - Adds ``invenio_base.finalize_app`` and ``invenio_base.api_finalize_app``
+          entry points to the creation of the factory function ``create_app`` and
+          ``create_api`` to overcome the deprecation of ``before_(app_)first_request``
+          in Flask>=2.3.0
+        
         Version 1.3.4 (released 2022-04-06)
         
         - Added support for Flask-Security-Invenio.
         
         Version 1.3.3 (released 2021-12-06)
         
         - Pinned Limits library to align with Flask-Limiter.
@@ -147,9 +155,9 @@
         Version 1.0.0 (released 2018-03-23)
         
         - Initial public release.
         
 Keywords: invenio applications
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: tests
```

### Comparing `invenio-app-1.3.4/README.rst` & `invenio-app-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/docs/Makefile` & `invenio-app-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/docs/api.rst` & `invenio-app-1.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/docs/conf.py` & `invenio-app-1.4.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2017-2018 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
 import os
@@ -14,48 +15,48 @@
 import sphinx.environment
 
 from invenio_app import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Do not warn on external images.
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Invenio-App'
-copyright = u'2017, CERN'
-author = u'CERN'
+project = "Invenio-App"
+copyright = "2017, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
@@ -66,255 +67,254 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
-    'description': 'WSGI, Celery and CLI applications for Invenio flavours.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'invenio-app',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'invenio-app@GitHub': 'https://github.com/inveniosoftware/invenio-app',
-        'invenio-app@PyPI': 'https://pypi.python.org/pypi/invenio-app/',
-    }
+    "description": "WSGI, Celery and CLI applications for Invenio flavours.",
+    "github_user": "inveniosoftware",
+    "github_repo": "invenio-app",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "invenio-app@GitHub": "https://github.com/inveniosoftware/invenio-app",
+        "invenio-app@PyPI": "https://pypi.python.org/pypi/invenio-app/",
+    },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "relations.html",
+        "searchbox.html",
+        "donate.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'invenio-app_namedoc'
+htmlhelp_basename = "invenio-app_namedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'invenio-app.tex', u'invenio-app Documentation',
-   u'CERN', 'manual'),
+    (master_doc, "invenio-app.tex", "invenio-app Documentation", "CERN", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'invenio-app', u'invenio-app Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "invenio-app", "invenio-app Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'invenio-app', u'Invenio-App Documentation',
-   author, 'invenio-app', 'WSGI, Celery and CLI applications for Invenio flavours.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "invenio-app",
+        "Invenio-App Documentation",
+        author,
+        "invenio-app",
+        "WSGI, Celery and CLI applications for Invenio flavours.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/', None),
+    "python": ("https://docs.python.org/", None),
 }
 
 # Autodoc configuraton.
-autoclass_content = 'both'
+autoclass_content = "both"
```

### Comparing `invenio-app-1.3.4/docs/configuration.rst` & `invenio-app-1.4.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/docs/index.rst` & `invenio-app-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/docs/make.bat` & `invenio-app-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/invenio_app/__init__.py` & `invenio-app-1.4.0/invenio_app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,10 +165,13 @@
 This should only be done for small number of templates/files, as it is usually
 better to provide them via an installabled Python package. Do take care not
 to overwrite any existing Invenio files.
 """
 
 from .ext import InvenioApp
 
-__version__ = '1.3.4'
+__version__ = "1.4.0"
 
-__all__ = ('__version__', 'InvenioApp', )
+__all__ = (
+    "__version__",
+    "InvenioApp",
+)
```

### Comparing `invenio-app-1.3.4/invenio_app/config.py` & `invenio-app-1.4.0/invenio_app/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 """
 
 from invenio_app.limiter import set_rate_limit
 
 RATELIMIT_APPLICATION = set_rate_limit
 """Global rate limit."""
 
-RATELIMIT_STRATEGY = 'moving-window'
+RATELIMIT_STRATEGY = "moving-window"
 """The rate limiting strategy to use.
 
 The strategy used here is the most consistant but also expensive one.
 If you are experiencing performance issues due to the increased Redis
 traffic, you can replace it with another one from the following
 `Flask-Limiter strategies
 <https://flask-limiter.readthedocs.io/en/stable/#ratelimit-strategy>`_.
 """
 
 RATELIMIT_HEADERS_ENABLED = True
 """Enable rate limit headers. (Default: ``True``)"""
 
-RATELIMIT_STORAGE_URL = 'memory://'
+RATELIMIT_STORAGE_URL = "memory://"
 """Storage backend to store rate-limiting information.
 
     Memory is used by default if no value is provided.
     For more information regarding the mentioned above configuration values and
     their available options you can see the `Flask-Limiter configuration
     <https://flask-limiter.readthedocs.io/en/stable/#configuration>`_.
 
@@ -77,18 +77,18 @@
     RATELIMIT_PER_ENDPOINT = \
     {
         'zenodo_frontpage.index': '10 per second',
         'security.login': '10 per second'
     }
 """
 
-RATELIMIT_AUTHENTICATED_USER = '5000 per hour;100 per minute'
+RATELIMIT_AUTHENTICATED_USER = "5000 per hour;100 per minute"
 """Rate limit for logged in users."""
 
-RATELIMIT_GUEST_USER = '1000 per hour;60 per minute'
+RATELIMIT_GUEST_USER = "1000 per hour;60 per minute"
 """Rate limit for non logged in users."""
 
 APP_THEME = None
 """Application-wide themes list used for template and assets lookup.
 
 The value is a list of theme strings applied in a fallback fashion in the order
 they are specified:
@@ -112,31 +112,28 @@
 
 .. note::
     `W3C
     <https://www.w3.org/TR/CSP2/>`_
 """
 
 APP_DEFAULT_SECURE_HEADERS = {
-    'force_https': True,
-    'force_https_permanent': False,
-    'force_file_save': False,
-    'frame_options': 'sameorigin',
-    'frame_options_allow_from': None,
-    'strict_transport_security': True,
-    'strict_transport_security_preload': False,
-    'strict_transport_security_max_age': 31556926,  # One year in seconds
-    'strict_transport_security_include_subdomains': True,
-    'content_security_policy': {
-        'default-src': ["'self'"],
-        'object-src': ["'none'"]
-    },
-    'content_security_policy_report_uri': None,
-    'content_security_policy_report_only': False,
-    'session_cookie_secure': True,
-    'session_cookie_http_only': True
+    "force_https": True,
+    "force_https_permanent": False,
+    "force_file_save": False,
+    "frame_options": "sameorigin",
+    "frame_options_allow_from": None,
+    "strict_transport_security": True,
+    "strict_transport_security_preload": False,
+    "strict_transport_security_max_age": 31556926,  # One year in seconds
+    "strict_transport_security_include_subdomains": True,
+    "content_security_policy": {"default-src": ["'self'"], "object-src": ["'none'"]},
+    "content_security_policy_report_uri": None,
+    "content_security_policy_report_only": False,
+    "session_cookie_secure": True,
+    "session_cookie_http_only": True,
 }
 """Talisman default Secure Headers configuration.
 
 As default, invenio assumes that HTTPS is enabled.
 If you are not using SSL, then remember to disable the `force_https` and
 `session_cookie_secure` configuration options related to HTTPS.
```

### Comparing `invenio-app-1.3.4/invenio_app/ext.py` & `invenio-app-1.4.0/invenio_app/ext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2017-2019 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio app extension."""
 
 from flask import Blueprint, g, request
@@ -38,95 +39,102 @@
 
         :param app: An instance of :class:`~flask.Flask`.
         """
         # Init the configuration
         self.init_config(app)
 
         # Enable secure HTTP headers
-        if app.config['APP_ENABLE_SECURE_HEADERS']:
+        if app.config["APP_ENABLE_SECURE_HEADERS"]:
             self.talisman = Talisman(
-                app, **app.config.get('APP_DEFAULT_SECURE_HEADERS', {})
+                app, **app.config.get("APP_DEFAULT_SECURE_HEADERS", {})
             )
 
-        app.jinja_env.filters['safe_redirect'] = safe_redirect
+        app.jinja_env.filters["safe_redirect"] = safe_redirect
 
         # Enable Rate limiter
         # Flask limiter needs to be initialised after talisman, since if the
         # talisman preprocessor doesn't run you will get an error on it's
         # afterprocessor.
         self.limiter = Limiter(
             app,
             key_func=obj_or_import_string(
-                app.config.get('RATELIMIT_KEY_FUNC'),
-                default=useragent_and_ip_limit_key)
+                app.config.get("RATELIMIT_KEY_FUNC"), default=useragent_and_ip_limit_key
+            ),
         )
 
         # Enable PING view
-        if app.config['APP_HEALTH_BLUEPRINT_ENABLED']:
-            blueprint = Blueprint('invenio_app_ping', __name__)
+        if app.config["APP_HEALTH_BLUEPRINT_ENABLED"]:
+            blueprint = Blueprint("invenio_app_ping", __name__)
             limiter = self.limiter
 
-            @blueprint.route('/ping', methods=['HEAD', 'OPTIONS', 'GET'])
+            @blueprint.route("/ping", methods=["HEAD", "OPTIONS", "GET"])
             @limiter.exempt
             def ping():
                 """Load balancer ping view."""
-                return 'OK'
+                return "OK"
 
-            ping.talisman_view_options = {'force_https': False}
+            ping.talisman_view_options = {"force_https": False}
 
             app.register_blueprint(blueprint)
 
-        requestid_header = app.config.get('APP_REQUESTID_HEADER')
+        requestid_header = app.config.get("APP_REQUESTID_HEADER")
         if requestid_header:
+
             @app.before_request
             def set_request_id():
                 """Extracts a request id from an HTTP header."""
                 request_id = request.headers.get(requestid_header)
                 if request_id:
                     # Capped at 200 to protect against malicious clients
                     # sending very large headers.
                     g.request_id = request_id[:200]
 
         # If installed register the Flask-DebugToolbar extension
         try:
             from flask_debugtoolbar import DebugToolbarExtension
-            app.extensions['flask-debugtoolbar'] = DebugToolbarExtension(app)
+
+            app.extensions["flask-debugtoolbar"] = DebugToolbarExtension(app)
         except ImportError:
-            app.logger.debug('Flask-DebugToolbar extension not installed.')
+            app.logger.debug("Flask-DebugToolbar extension not installed.")
 
         # Force host header check (by evaluating request.host) in order to make
         # Werkzeugs trusted host feature work properly.
-        if app.config['APP_ALLOWED_HOSTS']:
+        if app.config["APP_ALLOWED_HOSTS"]:
+
             @app.before_request
             def before_request():
                 request.host
 
         # Add theme template loader
-        if app.config.get('APP_THEME'):
+        if app.config.get("APP_THEME"):
             app.jinja_env.loader = ThemeJinjaLoader(app, app.jinja_env.loader)
 
         # Register self
-        app.extensions['invenio-app'] = self
+        app.extensions["invenio-app"] = self
 
     def init_config(self, app):
         """Initialize configuration.
 
         :param app: An instance of :class:`~flask.Flask`.
         """
-        config_apps = ['APP_', 'RATELIMIT_']
-        flask_talisman_debug_mode = ["'unsafe-inline'"]
+        config_apps = ["APP_", "RATELIMIT_"]
+        flask_talisman_debug_mode = "'unsafe-inline'"
         for k in dir(config):
             if any([k.startswith(prefix) for prefix in config_apps]):
                 app.config.setdefault(k, getattr(config, k))
 
-        if app.config['DEBUG']:
-            app.config.setdefault('APP_DEFAULT_SECURE_HEADERS', {})
-            headers = app.config['APP_DEFAULT_SECURE_HEADERS']
+        if app.config["DEBUG"]:
+            app.config.setdefault("APP_DEFAULT_SECURE_HEADERS", {})
+            headers = app.config["APP_DEFAULT_SECURE_HEADERS"]
+
             # ensure `content_security_policy` is not set to {}
-            if headers.get('content_security_policy') != {}:
-                headers.setdefault('content_security_policy', {})
-                csp = headers['content_security_policy']
+            if headers.get("content_security_policy") != {}:
+                headers.setdefault("content_security_policy", {})
+                csp = headers["content_security_policy"]
+
                 # ensure `default-src` is not set to []
-                if csp.get('default-src') != []:
-                    csp.setdefault('default-src', [])
+                if csp.get("default-src") != []:
+                    csp.setdefault("default-src", [])
+
                     # add default `content_security_policy` value when debug
-                    csp['default-src'] += flask_talisman_debug_mode
+                    if flask_talisman_debug_mode not in csp["default-src"]:
+                        csp["default-src"].append(flask_talisman_debug_mode)
```

### Comparing `invenio-app-1.3.4/invenio_app/factory.py` & `invenio-app-1.4.0/invenio_app/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2017-2018 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Flask application factories for Invenio flavours."""
 
 import os
@@ -15,48 +16,48 @@
 from invenio_base.app import create_app_factory
 from invenio_base.wsgi import create_wsgi_factory, wsgi_proxyfix
 from invenio_cache import BytecodeCache
 from invenio_config import create_config_loader
 
 from .helpers import TrustedHostsMixin
 
-env_prefix = 'INVENIO'
+env_prefix = "INVENIO"
 
-invenio_config_loader = create_config_loader(
-    config=None, env_prefix=env_prefix
-)
+invenio_config_loader = create_config_loader(config=None, env_prefix=env_prefix)
 
 
 def instance_path():
     """Instance path for Invenio.
 
     Defaults to ``<env_prefix>_INSTANCE_PATH``
      or if environment variable is not set ``<sys.prefix>/var/instance``.
     """
-    return os.getenv(env_prefix + '_INSTANCE_PATH') or \
-        os.path.join(sys.prefix, 'var', 'instance')
+    return os.getenv(env_prefix + "_INSTANCE_PATH") or os.path.join(
+        sys.prefix, "var", "instance"
+    )
 
 
 def static_folder():
     """Static folder path.
 
     Defaults to ``<env_prefix>_STATIC_FOLDER``
     or if environment variable is not set ``<sys.prefix>/var/instance/static``.
     """
-    return os.getenv(env_prefix + '_STATIC_FOLDER') or \
-        os.path.join(instance_path(), 'static')
+    return os.getenv(env_prefix + "_STATIC_FOLDER") or os.path.join(
+        instance_path(), "static"
+    )
 
 
 def static_url_path():
     """Static url path.
 
     Defaults to ``<env_prefix>_STATIC_URL_PATH``
     or if environment variable is not set ``/static``.
     """
-    return os.getenv(env_prefix + '_STATIC_URL_PATH') or '/static'
+    return os.getenv(env_prefix + "_STATIC_URL_PATH") or "/static"
 
 
 def config_loader(app, **kwargs_config):
     """Configuration loader."""
     invenio_config_loader(app, **kwargs_config)
 
     # TODO: Move this to invenio_cache.ext.InvenioCache.init_app
@@ -68,15 +69,15 @@
     """Create Flask application class.
 
     Invenio-Files-REST needs to patch the Werkzeug form parsing in order to
     support streaming large file uploads. This is done by subclassing the Flask
     application class.
     """
     try:
-        pkg_resources.get_distribution('invenio-files-rest')
+        pkg_resources.get_distribution("invenio-files-rest")
         from invenio_files_rest.app import Flask as FlaskBase
     except pkg_resources.DistributionNotFound:
         from flask import Flask as FlaskBase
 
     # Add Host header validation via APP_ALLOWED_HOSTS configuration variable.
     class Request(TrustedHostsMixin, FlaskBase.request_class):
         pass
@@ -84,48 +85,51 @@
     class Flask(FlaskBase):
         request_class = Request
 
     return Flask
 
 
 create_api = create_app_factory(
-    'invenio',
+    "invenio",
     config_loader=config_loader,
-    blueprint_entry_points=['invenio_base.api_blueprints'],
-    extension_entry_points=['invenio_base.api_apps'],
-    converter_entry_points=['invenio_base.api_converters'],
+    blueprint_entry_points=["invenio_base.api_blueprints"],
+    extension_entry_points=["invenio_base.api_apps"],
+    converter_entry_points=["invenio_base.api_converters"],
+    finalize_app_entry_points=["invenio_base.api_finalize_app"],
     wsgi_factory=wsgi_proxyfix(),
     instance_path=instance_path,
     root_path=instance_path,
     app_class=app_class(),
 )
 """Flask application factory for Invenio REST API."""
 
 create_ui = create_app_factory(
-    'invenio',
+    "invenio",
     config_loader=config_loader,
-    blueprint_entry_points=['invenio_base.blueprints'],
-    extension_entry_points=['invenio_base.apps'],
-    converter_entry_points=['invenio_base.converters'],
+    blueprint_entry_points=["invenio_base.blueprints"],
+    extension_entry_points=["invenio_base.apps"],
+    converter_entry_points=["invenio_base.converters"],
+    finalize_app_entry_points=["invenio_base.finalize_app"],
     wsgi_factory=wsgi_proxyfix(),
     instance_path=instance_path,
     static_folder=static_folder,
     root_path=instance_path,
     static_url_path=static_url_path(),
     app_class=app_class(),
 )
 """Flask application factory for Invenio UI."""
 
 create_app = create_app_factory(
-    'invenio',
+    "invenio",
     config_loader=config_loader,
-    blueprint_entry_points=['invenio_base.blueprints'],
-    extension_entry_points=['invenio_base.apps'],
-    converter_entry_points=['invenio_base.converters'],
-    wsgi_factory=wsgi_proxyfix(create_wsgi_factory({'/api': create_api})),
+    blueprint_entry_points=["invenio_base.blueprints"],
+    extension_entry_points=["invenio_base.apps"],
+    converter_entry_points=["invenio_base.converters"],
+    finalize_app_entry_points=["invenio_base.finalize_app"],
+    wsgi_factory=wsgi_proxyfix(create_wsgi_factory({"/api": create_api})),
     instance_path=instance_path,
     static_folder=static_folder,
     root_path=instance_path,
     static_url_path=static_url_path(),
     app_class=app_class(),
 )
 """Flask application factory for combined UI + REST API.
```

### Comparing `invenio-app-1.3.4/invenio_app/helpers.py` & `invenio-app-1.4.0/invenio_app/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 class TrustedHostsMixin(object):
     """Mixin for reading trusted hosts from application config."""
 
     @property
     def trusted_hosts(self):
         """Get list of trusted hosts."""
         if current_app:
-            return current_app.config.get('APP_ALLOWED_HOSTS', None)
+            return current_app.config.get("APP_ALLOWED_HOSTS", None)
 
 
-def get_safe_redirect_target(arg='next', _target=None):
+def get_safe_redirect_target(arg="next", _target=None):
     """Get URL to redirect to and ensure that it is local.
 
     :param arg: URL argument.
     :returns: The redirect target or ``None``.
     """
     for target in _target, request.args.get(arg), request.referrer:
         redirect = safe_redirect(target)
@@ -39,22 +39,23 @@
     return None
 
 
 def safe_redirect(target):
     """Ensure redirect is a local redirect."""
     if target:
         redirect_uri = urisplit(target)
-        allowed_hosts = current_app.config.get('APP_ALLOWED_HOSTS', [])
+        allowed_hosts = current_app.config.get("APP_ALLOWED_HOSTS", [])
         if redirect_uri.host in allowed_hosts:
             return target
         elif redirect_uri.path:
             return uricompose(
                 path=redirect_uri.path,
                 query=redirect_uri.query,
-                fragment=redirect_uri.fragment)
+                fragment=redirect_uri.fragment,
+            )
     return None
 
 
 class ThemeJinjaLoader(BaseLoader):
     """Prefix template loader.
 
     This loader acts as a wrapper for any type of Jinja loader. Before doing a
@@ -72,15 +73,15 @@
         """
         self.app = app
         self.loader = loader
 
     @cached_property
     def prefixes(self):
         """Return the active prefixes to be used for template lookup."""
-        theme = self.app.config.get('APP_THEME', [])
+        theme = self.app.config.get("APP_THEME", [])
         if isinstance(theme, str):
             theme = [theme]
         return theme
 
     def _prefixed_templates(self, name):
         template_names = [os.path.join(p, name) for p in self.prefixes]
         return template_names + [name]
```

### Comparing `invenio-app-1.3.4/invenio_app/limiter.py` & `invenio-app-1.4.0/invenio_app/limiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,31 +39,31 @@
     ```RATELIMIT_PER_USER``` mapping.
     If it is present then the custom rate limit value will be returned,
     otherwise the one returned will be the ```RATELIMIT_AUTHENTICATED_USER```
 
     3)Finally if none of the above is our case then the
     ```RATELIMIT_GUEST_USER``` will be the one to be returned.
     """
-    endpoint_limits = \
-        current_app.config.get('RATELIMIT_PER_ENDPOINT', {})
+    endpoint_limits = current_app.config.get("RATELIMIT_PER_ENDPOINT", {})
     if request.endpoint in endpoint_limits:
         # Case of whitelisted endpoint.
         return endpoint_limits[request.endpoint]
 
     try:
-        pkg_resources.get_distribution('flask_security_invenio ')
+        pkg_resources.get_distribution("flask_security_invenio ")
         from flask_security import current_user
+
         user = current_user
     except pkg_resources.DistributionNotFound:
         try:
-            pkg_resources.get_distribution('flask_security')
+            pkg_resources.get_distribution("flask_security")
             from flask_security import current_user
+
             user = current_user
         except pkg_resources.DistributionNotFound:
             user = None
 
     if user and user.is_authenticated:
         return g.get(
-            'user_rate_limit',
-            current_app.config['RATELIMIT_AUTHENTICATED_USER']
+            "user_rate_limit", current_app.config["RATELIMIT_AUTHENTICATED_USER"]
         )
-    return current_app.config['RATELIMIT_GUEST_USER']
+    return current_app.config["RATELIMIT_GUEST_USER"]
```

### Comparing `invenio-app-1.3.4/invenio_app.egg-info/PKG-INFO` & `invenio-app-1.4.0/invenio_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-app
-Version: 1.3.4
+Version: 1.4.0
 Summary: WSGI, Celery and CLI applications for Invenio flavours.
 Home-page: https://github.com/inveniosoftware/invenio-app
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -32,22 +32,30 @@
         WSGI, Celery and CLI applications for Invenio flavours.
         
         Further documentation is available on
         https://invenio-app.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2017-2019 CERN.
+            Copyright (C) 2017-2023 CERN.
+            Copyright (C) 2023 Graz University of Technology.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.4.0 (released 2023-06-26)
+        
+        - Adds ``invenio_base.finalize_app`` and ``invenio_base.api_finalize_app``
+          entry points to the creation of the factory function ``create_app`` and
+          ``create_api`` to overcome the deprecation of ``before_(app_)first_request``
+          in Flask>=2.3.0
+        
         Version 1.3.4 (released 2022-04-06)
         
         - Added support for Flask-Security-Invenio.
         
         Version 1.3.3 (released 2021-12-06)
         
         - Pinned Limits library to align with Flask-Limiter.
@@ -147,9 +155,9 @@
         Version 1.0.0 (released 2018-03-23)
         
         - Initial public release.
         
 Keywords: invenio applications
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: tests
```

### Comparing `invenio-app-1.3.4/invenio_app.egg-info/SOURCES.txt` & `invenio-app-1.4.0/invenio_app.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .dockerignore
 .editorconfig
+.git-blame-ignore-revs
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-pytest.ini
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
-.github/workflows/pypi-release.yml
+.github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/configuration.rst
```

### Comparing `invenio-app-1.3.4/requirements-devel.txt` & `invenio-app-1.4.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-app-1.3.4/setup.cfg` & `invenio-app-1.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 url = https://github.com/inveniosoftware/invenio-app
 classifiers = 
 	Development Status :: 5 - Production/Stable
 
 [options]
 include_package_data = True
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	flask-limiter>=1.0.1,<1.2.0
 	flask-shell-ipython>=0.3.1
 	flask-talisman>=0.3.2,<1.0
+	invenio-base>=1.3.0
 	invenio-cache>=1.1.0
 	invenio-celery>=1.2.4
 	invenio-config>=1.0.0
 	limits>=1.5.1,<2.0
 	uritools>=1.0.1
 
 [options.extras_require]
 tests = 
+	pytest-black>=0.3.0
 	pytest-invenio>=1.4.7
+	mock>=4.0.0
 	sphinx>=4.2.0,<5
 
 [options.entry_points]
 console_scripts = 
 	invenio = invenio_app.cli:cli
 invenio_base.api_apps = 
 	invenio_app = invenio_app:InvenioApp
@@ -47,14 +50,22 @@
 
 [bdist_wheel]
 universal = 1
 
 [pydocstyle]
 add_ignore = D401
 
-[pycodestyle]
-exclude = docs/conf.py
+[isort]
+profile = black
+
+[check-manifest]
+ignore = 
+	*-requirements.txt
+
+[tool:pytest]
+addopts = --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=invenio_app --cov-report=term-missing
+testpaths = tests invenio_app
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `invenio-app-1.3.4/tests/conftest.py` & `invenio-app-1.4.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2017-2018 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Pytest configuration."""
 
 import imp
 import sys
 from collections import namedtuple
+from copy import deepcopy
 
 import pytest
-from flask import Flask
-from flask import current_app as flask_current_app
-from flask import g
+from flask import Flask, g
 from flask_limiter import Limiter
-from mock import patch
-from pkg_resources import Distribution
 
-from invenio_app import InvenioApp
 from invenio_app.config import APP_DEFAULT_SECURE_HEADERS, set_rate_limit
 from invenio_app.ext import useragent_and_ip_limit_key
 from invenio_app.helpers import obj_or_import_string
 
 
 @pytest.fixture()
 def base_app():
     """Flask application fixture."""
-    app_ = Flask('testapp')
+    app_ = Flask("testapp")
     app_.config.update(
-        SECRET_KEY='SECRET_KEY',
+        SECRET_KEY="SECRET_KEY",
         TESTING=True,
     )
-    app_.config['APP_DEFAULT_SECURE_HEADERS'] = APP_DEFAULT_SECURE_HEADERS
-    app_.config['APP_DEFAULT_SECURE_HEADERS']['force_https'] = False
 
-    @app_.route('/requestid')
+    app_.config["APP_DEFAULT_SECURE_HEADERS"] = deepcopy(APP_DEFAULT_SECURE_HEADERS)
+    app_.config["APP_DEFAULT_SECURE_HEADERS"]["force_https"] = False
+
+    @app_.route("/requestid")
     def requestid():
         from flask import g  # Prevent pytest problems
-        return g.request_id if g and hasattr(g, 'request_id') else ''
 
-    @app_.route('/limited_rate')
+        return g.request_id if g and hasattr(g, "request_id") else ""
+
+    @app_.route("/limited_rate")
     def limited_rate():
-        return 'test'
+        return "test"
 
-    @app_.route('/unlimited_rate')
+    @app_.route("/unlimited_rate")
     def unlimited_rate():
-        return 'test'
+        return "test"
 
     return app_
 
 
 @pytest.fixture()
 def app_with_no_limiter(base_app):
     """Flask application fixture without limiter registered."""
@@ -60,78 +59,81 @@
         yield base_app
 
 
 @pytest.yield_fixture()
 def app(base_app):
     """Flask application fixture."""
     base_app.config.update(
-        APP_ALLOWED_HOSTS=['localhost'],
+        APP_ALLOWED_HOSTS=["localhost"],
         RATELIMIT_APPLICATION=set_rate_limit,
-        RATELIMIT_GUEST_USER='2 per second',
-        RATELIMIT_AUTHENTICATED_USER='5 per second',
-        RATELIMIT_PER_ENDPOINT={'unlimited_rate': '200 per second'},
-        RATELIMIT_HEADERS_ENABLED=True
+        RATELIMIT_GUEST_USER="2 per second",
+        RATELIMIT_AUTHENTICATED_USER="5 per second",
+        RATELIMIT_PER_ENDPOINT={"unlimited_rate": "200 per second"},
+        RATELIMIT_HEADERS_ENABLED=True,
     )
     Limiter(
         base_app,
         key_func=obj_or_import_string(
-            base_app.config.get('RATELIMIT_KEY_FUNC'),
-            default=useragent_and_ip_limit_key)
+            base_app.config.get("RATELIMIT_KEY_FUNC"),
+            default=useragent_and_ip_limit_key,
+        ),
     )
     with base_app.app_context():
         yield base_app
 
 
 @pytest.fixture()
 def wsgi_apps():
     """Wsgi app fixture."""
     from invenio_base.app import create_app_factory
     from invenio_base.wsgi import create_wsgi_factory, wsgi_proxyfix
 
     def _config(app, **kwargs):
         app.config.update(
-            SECRET_KEY='SECRET_KEY',
+            SECRET_KEY="SECRET_KEY",
             TESTING=True,
         )
-        app.config['APP_DEFAULT_SECURE_HEADERS'] = APP_DEFAULT_SECURE_HEADERS
-        app.config['APP_DEFAULT_SECURE_HEADERS']['force_https'] = False
+        app.config["APP_DEFAULT_SECURE_HEADERS"] = deepcopy(APP_DEFAULT_SECURE_HEADERS)
+        app.config["APP_DEFAULT_SECURE_HEADERS"]["force_https"] = False
+
     # API
     create_api = create_app_factory(
-        'invenio',
+        "invenio",
         config_loader=_config,
         wsgi_factory=wsgi_proxyfix(),
     )
     # UI
     create_ui = create_app_factory(
-        'invenio',
+        "invenio",
         config_loader=_config,
         wsgi_factory=wsgi_proxyfix(),
     )
     # Combined
     create_app = create_app_factory(
-        'invenio',
+        "invenio",
         config_loader=_config,
-        wsgi_factory=wsgi_proxyfix(create_wsgi_factory({'/api': create_api})),
+        wsgi_factory=wsgi_proxyfix(create_wsgi_factory({"/api": create_api})),
     )
     return create_app, create_ui, create_api
 
 
 @pytest.fixture()
 def create_mocked_flask_security_with_user_init():
     """Create a function initializing flask security with a user."""
+
     def mocked_flask_security(user):
         """Add mocked flask-security."""
-        module_name = 'flask_security'
+        module_name = "flask_security"
         test_api_module = imp.new_module(module_name)
-        test_api_module.current_user = \
-            namedtuple("User", user.keys())(*user.values())
+        test_api_module.current_user = namedtuple("User", user.keys())(*user.values())
         sys.modules[module_name] = test_api_module
         return test_api_module
+
     return mocked_flask_security
 
 
 @pytest.fixture()
 def push_rate_limit_to_context():
     """Push a custom rate limit to the Flask global context."""
-    custom_rate_limit = '10 per second'
-    setattr(g, 'user_rate_limit', custom_rate_limit)
+    custom_rate_limit = "10 per second"
+    setattr(g, "user_rate_limit", custom_rate_limit)
     return custom_rate_limit
```

### Comparing `invenio-app-1.3.4/tests/test_app.py` & `invenio-app-1.4.0/tests/test_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,168 +1,170 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2017-2018 CERN.
+# Copyright (C) 2022 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module tests."""
 
 from invenio_app import InvenioApp
 
 
 def test_rate_secure_headers(app):
     """Test Rate Limiter extension."""
-    app.config['APP_ENABLE_SECURE_HEADERS'] = False
+    app.config["APP_ENABLE_SECURE_HEADERS"] = False
     # Initialize the app
     InvenioApp(app)
-    assert 'talisman' not in app.extensions
+    assert "talisman" not in app.extensions
 
 
 def test_headers(app_with_no_limiter):
     """Test headers."""
-    app_with_no_limiter.config['RATELIMIT_APPLICATION'] = '1/day'
+    app_with_no_limiter.config["RATELIMIT_APPLICATION"] = "1/day"
     ext = InvenioApp(app_with_no_limiter)
 
     for handler in app_with_no_limiter.logger.handlers:
         ext.limiter.logger.addHandler(handler)
 
-    @app_with_no_limiter.route('/jessica_jones')
+    @app_with_no_limiter.route("/jessica_jones")
     def jessica_jones():
-        return 'jessica jones'
+        return "jessica jones"
 
-    @app_with_no_limiter.route('/avengers')
+    @app_with_no_limiter.route("/avengers")
     def avengers():
-        return 'infinity war'
+        return "infinity war"
 
     with app_with_no_limiter.test_client() as client:
-        res = client.get('/jessica_jones')
+        res = client.get("/jessica_jones")
         assert res.status_code == 200
-        assert res.headers['X-RateLimit-Limit'] == '1'
-        assert res.headers['X-RateLimit-Remaining'] == '0'
-        assert res.headers['X-RateLimit-Reset']
+        assert res.headers["X-RateLimit-Limit"] == "1"
+        assert res.headers["X-RateLimit-Remaining"] == "0"
+        assert res.headers["X-RateLimit-Reset"]
 
-        res = client.get('/jessica_jones')
+        res = client.get("/jessica_jones")
         assert res.status_code == 429
-        assert res.headers['X-RateLimit-Limit']
-        assert res.headers['X-RateLimit-Remaining']
-        assert res.headers['X-RateLimit-Reset']
+        assert res.headers["X-RateLimit-Limit"]
+        assert res.headers["X-RateLimit-Remaining"]
+        assert res.headers["X-RateLimit-Reset"]
 
-        res = client.get('/avengers')
+        res = client.get("/avengers")
         assert res.status_code == 429
-        assert res.headers['X-Content-Type-Options']
-        assert res.headers['X-Frame-Options']
-        assert res.headers['X-XSS-Protection']
-        assert res.headers['X-RateLimit-Limit']
-        assert res.headers['X-RateLimit-Remaining']
-        assert res.headers['X-RateLimit-Reset']
+        assert res.headers["X-Content-Type-Options"]
+        assert res.headers["X-Frame-Options"]
+        assert res.headers["X-XSS-Protection"]
+        assert res.headers["X-RateLimit-Limit"]
+        assert res.headers["X-RateLimit-Remaining"]
+        assert res.headers["X-RateLimit-Reset"]
 
 
 def _normalize_csp_header(header):
     """Normalize a CSP header for consistent comparisons."""
-    return {p.strip() for p in (header or '').split(';')}
+    return {p.strip() for p in (header or "").split(";")}
 
 
 def _test_csp_default_src(app, expect):
     """Assert that the Content-Security-Policy header is the expect param."""
     ext = InvenioApp(app)
 
-    @app.route('/captain_america')
+    @app.route("/captain_america")
     def captain_america():
-        return 'captain america'
+        return "captain america"
 
     with app.test_client() as client:
-        res = client.get('/captain_america')
+        res = client.get("/captain_america")
         assert res.status_code == 200
         assert _normalize_csp_header(
-            res.headers.get('Content-Security-Policy')
+            res.headers.get("Content-Security-Policy")
         ) == _normalize_csp_header(expect)
 
 
 def test_csp_default_src_when_debug_false(app):
     """Test the Content-Security-Policy header when app debug is False."""
+    app.config["DEBUG"] = False
     expect = "default-src 'self'; object-src 'none'"
     _test_csp_default_src(app, expect)
 
 
 def test_csp_default_src_when_debug_true(app):
     """Test the Content-Security-Policy header when app debug is True."""
-    app.config['DEBUG'] = True
+    app.config["DEBUG"] = True
     expect = "default-src 'self' 'unsafe-inline'; object-src 'none'"
     _test_csp_default_src(app, expect)
 
 
 def test_empty_csp_when_set_empty(app):
     """Test empty Content-Security-Policy header when set emtpy."""
-    app.config['DEBUG'] = True
-    app.config['APP_DEFAULT_SECURE_HEADERS']['content_security_policy'] = {}
+    app.config["DEBUG"] = True
+    app.config["APP_DEFAULT_SECURE_HEADERS"]["content_security_policy"] = {}
     expect = None
     _test_csp_default_src(app, expect)
 
 
 def test_default_health_blueprint(app):
-    app.config['APP_HEALTH_BLUEPRINT_ENABLED'] = True
+    app.config["APP_HEALTH_BLUEPRINT_ENABLED"] = True
     # Initialize the app
     InvenioApp(app)
     with app.test_client() as client:
-        res = client.get('/ping')
+        res = client.get("/ping")
         assert res.status_code == 200
 
 
 def test_ping_exempt_from_rate_limiting(app_with_no_limiter):
-    app_with_no_limiter.config['APP_HEALTH_BLUEPRINT_ENABLED'] = True
-    app_with_no_limiter.config['RATELIMIT_APPLICATION'] = '1/day'
+    app_with_no_limiter.config["APP_HEALTH_BLUEPRINT_ENABLED"] = True
+    app_with_no_limiter.config["RATELIMIT_APPLICATION"] = "1/day"
     # Initialize the app
     InvenioApp(app_with_no_limiter)
     with app_with_no_limiter.test_client() as client:
-        res = client.get('/ping')
+        res = client.get("/ping")
         assert res.status_code == 200
-        res = client.get('/ping')
+        res = client.get("/ping")
         assert res.status_code == 200
-        res = client.head('/ping')
+        res = client.head("/ping")
         assert res.status_code == 200
-        res = client.options('/ping')
+        res = client.options("/ping")
         assert res.status_code == 200
 
 
 def test_requestid(base_app):
     """Test extraction of header id."""
     InvenioApp(base_app)
     with base_app.test_client() as client:
-        assert '1234' == client.get(
-            '/requestid',  headers={'X-Request-ID': '1234'}
+        assert "1234" == client.get(
+            "/requestid", headers={"X-Request-ID": "1234"}
         ).get_data(as_text=True)
 
 
 def test_requestid_different_header(base_app):
     """Test changing header name."""
-    base_app.config['APP_REQUESTID_HEADER'] = 'Request-ID'
+    base_app.config["APP_REQUESTID_HEADER"] = "Request-ID"
     InvenioApp(base_app)
     with base_app.test_client() as client:
         # Extracted
-        assert '1234' == client.get(
-            '/requestid',  headers={'Request-ID': '1234'}
+        assert "1234" == client.get(
+            "/requestid", headers={"Request-ID": "1234"}
         ).get_data(as_text=True)
         # Not extracted
-        assert '' == client.get(
-            '/requestid',  headers={'X-Request-ID': '1234'}
+        assert "" == client.get(
+            "/requestid", headers={"X-Request-ID": "1234"}
         ).get_data(as_text=True)
 
 
 def test_requestid_cap_200(base_app):
     """Test cap at 200 chars of request id."""
     InvenioApp(base_app)
     with base_app.test_client() as client:
-        assert '1'*200 == client.get(
-            '/requestid',  headers={'X-Request-ID': '1'*500}
+        assert "1" * 200 == client.get(
+            "/requestid", headers={"X-Request-ID": "1" * 500}
         ).get_data(as_text=True)
 
 
 def test_requestid_no_extraction(base_app):
     """Test no extraction of header id."""
-    base_app.config['APP_REQUESTID_HEADER'] = None
+    base_app.config["APP_REQUESTID_HEADER"] = None
     InvenioApp(base_app)
     with base_app.test_client() as client:
-        assert '' == client.get(
-            '/requestid',  headers={'X-Request-ID': '1234'}
+        assert "" == client.get(
+            "/requestid", headers={"X-Request-ID": "1234"}
         ).get_data(as_text=True)
```

### Comparing `invenio-app-1.3.4/tests/test_factory.py` & `invenio-app-1.4.0/tests/test_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,50 +12,52 @@
 
 from invenio_app.factory import create_ui
 
 
 def test_version():
     """Test version import."""
     from invenio_app import __version__
+
     assert __version__
 
 
 def test_config_loader():
     """Test config loader."""
     app = create_ui()
     assert app.jinja_env.cache_size == 1000
 
 
 def test_trusted_hosts():
     """Test trusted hosts configuration."""
     app = create_ui(
-        APP_ALLOWED_HOSTS=['example.org', 'www.example.org'],
+        APP_ALLOWED_HOSTS=["example.org", "www.example.org"],
         APP_ENABLE_SECURE_HEADERS=False,
-        RATELIMIT_ENABLED=False
+        RATELIMIT_ENABLED=False,
     )
 
-    @app.route('/host')
+    @app.route("/host")
     def index_host():
         return request.host
 
-    @app.route('/url-for')
+    @app.route("/url-for")
     def index_url():
-        return url_for('index_url', _external=True)
+        return url_for("index_url", _external=True)
 
     with app.test_client() as client:
-        for u in ['/host', '/url-for']:
-            res = client.get(u, headers={'Host': 'attacker.org'})
+        for u in ["/host", "/url-for"]:
+            res = client.get(u, headers={"Host": "attacker.org"})
             assert res.status_code == 400
 
-            res = client.get(u, headers={'Host': 'example.org'})
+            res = client.get(u, headers={"Host": "example.org"})
             assert res.status_code == 200
 
-            res = client.get(u, headers={'Host': 'www.example.org'})
+            res = client.get(u, headers={"Host": "www.example.org"})
             assert res.status_code == 200
 
+
 # There used to be a test here checking if the X-Forwarded-Host
 #  is checked as well. It was deleted because from werkzeug 0.15.0 onwards
 #  this check is not supported and therefore it caused the test to fail.
 #  New way of dealing with proxies in werkzeug is `ProxyFix
 #  <https://werkzeug.palletsprojects.com/en/0.15.x/middleware/proxy_fix`_.
 #  The change in werkzeug mentioned above is visible in this
 # `PR <https://github.com/pallets/werkzeug/pull/1303/files>`_.
```

### Comparing `invenio-app-1.3.4/tests/test_helpers.py` & `invenio-app-1.4.0/tests/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from urllib.parse import quote_plus
 
 import pytest
 
 from invenio_app.helpers import get_safe_redirect_target
 
 
-@pytest.mark.parametrize("test_input,expected", [
-    ('https://example.org/search?page=1&q=&keywords=taxonomy&keywords=animali',
-     '/search?page=1&q=&keywords=taxonomy&keywords=animali'),
-    ('/search?page=1&size=20',
-     '/search?page=1&size=20'),
-    ('https://localhost/search?page=1',
-     'https://localhost/search?page=1'),
-])
+@pytest.mark.parametrize(
+    "test_input,expected",
+    [
+        (
+            "https://example.org/search?page=1&q=&keywords=taxonomy&keywords=animali",
+            "/search?page=1&q=&keywords=taxonomy&keywords=animali",
+        ),
+        ("/search?page=1&size=20", "/search?page=1&size=20"),
+        ("https://localhost/search?page=1", "https://localhost/search?page=1"),
+    ],
+)
 def test_get_safe_redirect_target(app, test_input, expected):
     """Test that only "localhost" is a trusted absolute redirect target."""
-    with app.test_request_context(
-            '/?next={0}'.format(quote_plus(test_input))):
+    with app.test_request_context("/?next={0}".format(quote_plus(test_input))):
         assert get_safe_redirect_target() == expected
```

### Comparing `invenio-app-1.3.4/tests/test_templating.py` & `invenio-app-1.4.0/tests/test_templating.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,120 +24,120 @@
 # Fixtures
 #
 @pytest.fixture()
 def instance_path():
     """Fixture for creating an instance path."""
     path = tempfile.mkdtemp()
     environ.update(
-        INVENIO_INSTANCE_PATH=environ.get('INSTANCE_PATH', path),
+        INVENIO_INSTANCE_PATH=environ.get("INSTANCE_PATH", path),
     )
     yield path
-    environ.pop('INVENIO_INSTANCE_PATH', None)
+    environ.pop("INVENIO_INSTANCE_PATH", None)
     shutil.rmtree(path)
 
 
 @pytest.fixture()
 def blueprint():
     """Blueprint for loading templates."""
     # This blueprint picks up the tests/templates/ folder, so that we can
     # render templates from inside this folder.
-    return Blueprint('tests', __name__, template_folder='templates')
+    return Blueprint("tests", __name__, template_folder="templates")
 
 
 @pytest.fixture()
 def notheme_app(instance_path, blueprint):
     """Application without template theming."""
     app = create_ui()
     app.register_blueprint(blueprint)
     with app.app_context():
         yield app
 
 
 @pytest.fixture()
 def theme_app(instance_path, blueprint):
     """Application with template theming."""
-    app = create_ui(APP_THEME=['semantic-ui', 'bootstrap3'])
+    app = create_ui(APP_THEME=["semantic-ui", "bootstrap3"])
     app.register_blueprint(blueprint)
     with app.app_context():
         yield app
 
 
 @pytest.fixture()
 def theme_app_instance_templates(theme_app):
     """Copy templates into instance folder."""
     # Fixture depends on theme_app to ensure the correct instance path is used.
-    src = join(dirname(__file__), 'instance/templates')
-    dst = join(theme_app.instance_path, 'templates')
+    src = join(dirname(__file__), "instance/templates")
+    dst = join(theme_app.instance_path, "templates")
     shutil.copytree(src, dst)
     yield src
     shutil.rmtree(dst)
 
 
 #
 # Tests
 #
 def test_notheme(notheme_app):
     """Test template loading order *without* themes."""
-    assert render_template('base.html') == 'base'
-    assert render_template('fallback.html') == 'fallback-base'
-    assert render_template('only.html') == 'only-base'
+    assert render_template("base.html") == "base"
+    assert render_template("fallback.html") == "fallback-base"
+    assert render_template("only.html") == "only-base"
 
     # Theme templates can also be accessed via full path (not true for base)
-    assert render_template('semantic-ui/base.html') == 'semantic-ui'
-    assert render_template('bootstrap3/base.html') == 'bootstrap3'
-    assert render_template('bootstrap3/fallback.html') == 'fallback-bootstrap3'
+    assert render_template("semantic-ui/base.html") == "semantic-ui"
+    assert render_template("bootstrap3/base.html") == "bootstrap3"
+    assert render_template("bootstrap3/fallback.html") == "fallback-bootstrap3"
 
     # Not found template
-    assert pytest.raises(TemplateNotFound, render_template, 'invalid.html')
+    assert pytest.raises(TemplateNotFound, render_template, "invalid.html")
 
 
 def test_theme(theme_app):
     """Test template loading order *with* themes configured."""
     # Primary theme defines base.html
-    assert render_template('base.html') == 'semantic-ui'
+    assert render_template("base.html") == "semantic-ui"
     # Primary theme does not define fallback.html so using fallback
-    assert render_template('fallback.html') == 'fallback-bootstrap3'
+    assert render_template("fallback.html") == "fallback-bootstrap3"
     # Primary and secondary theme does not define only.html so using fallback
     # to normal loading
-    assert render_template('only.html') == 'only-base'
+    assert render_template("only.html") == "only-base"
 
     # Theme templates can also be accessed via full path (not true for base)
-    assert render_template('semantic-ui/base.html') == 'semantic-ui'
-    assert render_template('bootstrap3/base.html') == 'bootstrap3'
+    assert render_template("semantic-ui/base.html") == "semantic-ui"
+    assert render_template("bootstrap3/base.html") == "bootstrap3"
 
     # Not found template
-    assert pytest.raises(TemplateNotFound, render_template, 'invalid.html')
+    assert pytest.raises(TemplateNotFound, render_template, "invalid.html")
 
 
 def test_theme_with_instance_templates(theme_app_instance_templates):
     """Test template loading order *with* themes configured."""
-    assert render_template('instance.html') == 'instance-only-semantic-ui'
+    assert render_template("instance.html") == "instance-only-semantic-ui"
     # Primary theme defines base.html
-    assert render_template('base.html') == 'instance-semantic-ui'
+    assert render_template("base.html") == "instance-semantic-ui"
     # Primary theme does not define fallback.html so using fallback
-    assert render_template('fallback.html') == 'instance-fallback-bootstrap3'
+    assert render_template("fallback.html") == "instance-fallback-bootstrap3"
     # Primary and secondary theme does not define only.html so using fallback
     # to normal loading
-    assert render_template('only.html') == 'instance-only-base'
+    assert render_template("only.html") == "instance-only-base"
 
     # Theme templates can also be accessed via full path (not true for base)
-    assert render_template('semantic-ui/base.html') == 'instance-semantic-ui'
-    assert render_template('bootstrap3/base.html') == 'instance-bootstrap3'
+    assert render_template("semantic-ui/base.html") == "instance-semantic-ui"
+    assert render_template("bootstrap3/base.html") == "instance-bootstrap3"
 
     # Instance does not defined noinstance.html
-    assert render_template('noinstance.html') == 'noinstance-semantic-ui'
+    assert render_template("noinstance.html") == "noinstance-semantic-ui"
 
     # Not found template
-    assert pytest.raises(TemplateNotFound, render_template, 'invalid.html')
+    assert pytest.raises(TemplateNotFound, render_template, "invalid.html")
 
 
 def test_list_templaes(theme_app):
     """Test list templates."""
     assert sorted(theme_app.jinja_env.loader.list_templates()) == [
-        'base.html',
-        'bootstrap3/base.html',
-        'bootstrap3/fallback.html',
-        'fallback.html',
-        'only.html',
-        'semantic-ui/base.html',
-        'semantic-ui/noinstance.html',
+        "base.html",
+        "bootstrap3/base.html",
+        "bootstrap3/fallback.html",
+        "fallback.html",
+        "only.html",
+        "semantic-ui/base.html",
+        "semantic-ui/noinstance.html",
     ]
```

### Comparing `invenio-app-1.3.4/tests/test_wsgi.py` & `invenio-app-1.4.0/tests/test_wsgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 from werkzeug.test import EnvironBuilder
 
 
 def wsgi_output(application):
     data = {}
 
     def start_response(status, headers):
-        data['status'] = status
-        data['headers'] = headers
+        data["status"] = status
+        data["headers"] = headers
 
-    data['output'] = application(
-        EnvironBuilder(path='/', method='GET').get_environ(),
-        start_response
+    data["output"] = application(
+        EnvironBuilder(path="/", method="GET").get_environ(), start_response
     )
     return data
 
 
 def test_wsgi(wsgi_apps):
     """Test wsgi."""
     create_app, create_ui, create_api = wsgi_apps
 
     res = wsgi_output(create_app())
-    assert res['status'] == '404 NOT FOUND'
+    assert res["status"] == "404 NOT FOUND"
 
     res = wsgi_output(create_ui())
-    assert res['status'] == '404 NOT FOUND'
+    assert res["status"] == "404 NOT FOUND"
 
     res = wsgi_output(create_api())
-    assert res['status'] == '404 NOT FOUND'
+    assert res["status"] == "404 NOT FOUND"
```

