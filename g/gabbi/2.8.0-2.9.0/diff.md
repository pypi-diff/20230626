# Comparing `tmp/gabbi-2.8.0.tar.gz` & `tmp/gabbi-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gabbi-2.8.0.tar", last modified: Fri Sep 23 14:32:29 2022, max compression
+gzip compressed data, was "gabbi-2.9.0.tar", last modified: Mon Jun 26 12:55:20 2023, max compression
```

## Comparing `gabbi-2.8.0.tar` & `gabbi-2.9.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.072317 gabbi-2.8.0/
--rw-r--r--   0 cdent      (503) staff       (20)       27 2022-07-22 21:46:23.000000 gabbi-2.8.0/.coveragerc
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.027164 gabbi-2.8.0/.github/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.039615 gabbi-2.8.0/.github/workflows/
--rw-r--r--   0 cdent      (503) staff       (20)     1179 2022-09-22 16:22:17.000000 gabbi-2.8.0/.github/workflows/docker.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     1550 2022-09-22 18:07:52.000000 gabbi-2.8.0/.github/workflows/tests.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.8.0/.pyup.yml
--rw-r--r--   0 cdent      (503) staff       (20)      223 2022-09-22 16:07:15.000000 gabbi-2.8.0/.stestr.conf
--rw-r--r--   0 cdent      (503) staff       (20)     1167 2022-09-23 14:32:28.000000 gabbi-2.8.0/AUTHORS
--rw-r--r--   0 cdent      (503) staff       (20)     2307 2022-09-22 16:07:15.000000 gabbi-2.8.0/CONTRIBUTING.md
--rw-r--r--   0 cdent      (503) staff       (20)    27062 2022-09-23 14:32:28.000000 gabbi-2.8.0/ChangeLog
--rw-r--r--   0 cdent      (503) staff       (20)      257 2022-09-22 16:22:17.000000 gabbi-2.8.0/Dockerfile
--rw-r--r--   0 cdent      (503) staff       (20)      593 2022-07-22 21:46:23.000000 gabbi-2.8.0/LICENSE
--rw-r--r--   0 cdent      (503) staff       (20)     1027 2022-09-23 14:17:33.000000 gabbi-2.8.0/Makefile
--rw-r--r--   0 cdent      (503) staff       (20)     4625 2022-09-23 14:32:29.072401 gabbi-2.8.0/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     3607 2022-09-22 18:07:52.000000 gabbi-2.8.0/README.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.039859 gabbi-2.8.0/docs/
--rw-r--r--   0 cdent      (503) staff       (20)     6767 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/Makefile
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.044475 gabbi-2.8.0/docs/source/
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.044739 gabbi-2.8.0/docs/source/_static/
--rw-r--r--   0 cdent      (503) staff       (20)      145 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/_static/theme_override.css
--rw-r--r--   0 cdent      (503) staff       (20)     8327 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/conf.py
--rw-r--r--   0 cdent      (503) staff       (20)      904 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/example.py
--rw-r--r--   0 cdent      (503) staff       (20)      292 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/example.rst
--rw-r--r--   0 cdent      (503) staff       (20)     7388 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/example.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     3775 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/faq.rst
--rw-r--r--   0 cdent      (503) staff       (20)     3322 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/fixtures.rst
--rw-r--r--   0 cdent      (503) staff       (20)    14991 2022-09-23 14:13:29.000000 gabbi-2.8.0/docs/source/format.rst
--rw-r--r--   0 cdent      (503) staff       (20)     2339 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/gabbi.rst
--rw-r--r--   0 cdent      (503) staff       (20)     7316 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/handlers.rst
--rw-r--r--   0 cdent      (503) staff       (20)     1601 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/host.rst
--rw-r--r--   0 cdent      (503) staff       (20)     4650 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/index.rst
--rw-r--r--   0 cdent      (503) staff       (20)     5042 2022-07-22 21:46:23.000000 gabbi-2.8.0/docs/source/jsonpath.rst
--rw-r--r--   0 cdent      (503) staff       (20)     4508 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/loader.rst
--rw-r--r--   0 cdent      (503) staff       (20)      881 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/pytest-example.py
--rw-r--r--   0 cdent      (503) staff       (20)      970 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/pytest3.0-example.py
--rw-r--r--   0 cdent      (503) staff       (20)     9861 2022-09-23 14:15:15.000000 gabbi-2.8.0/docs/source/release.rst
--rw-r--r--   0 cdent      (503) staff       (20)     2666 2022-09-22 16:22:17.000000 gabbi-2.8.0/docs/source/runner.rst
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.048004 gabbi-2.8.0/gabbi/
--rw-r--r--   0 cdent      (503) staff       (20)      610 2022-09-23 14:15:24.000000 gabbi-2.8.0/gabbi/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)    26287 2022-09-23 14:11:15.000000 gabbi-2.8.0/gabbi/case.py
--rw-r--r--   0 cdent      (503) staff       (20)    10255 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/driver.py
--rw-r--r--   0 cdent      (503) staff       (20)      915 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/exception.py
--rw-r--r--   0 cdent      (503) staff       (20)     3113 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/fixture.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.051237 gabbi-2.8.0/gabbi/handlers/
--rw-r--r--   0 cdent      (503) staff       (20)      915 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/handlers/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)     4185 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/handlers/base.py
--rw-r--r--   0 cdent      (503) staff       (20)     2903 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/handlers/core.py
--rw-r--r--   0 cdent      (503) staff       (20)     5362 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/handlers/jsonhandler.py
--rw-r--r--   0 cdent      (503) staff       (20)     1524 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/handlers/yaml_disk_loading_jsonhandler.py
--rw-r--r--   0 cdent      (503) staff       (20)     8040 2022-09-23 14:11:15.000000 gabbi-2.8.0/gabbi/httpclient.py
--rw-r--r--   0 cdent      (503) staff       (20)      841 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/json_parser.py
--rw-r--r--   0 cdent      (503) staff       (20)     4503 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/pytester.py
--rw-r--r--   0 cdent      (503) staff       (20)     4484 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/reporter.py
--rw-r--r--   0 cdent      (503) staff       (20)    10335 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/runner.py
--rw-r--r--   0 cdent      (503) staff       (20)     5247 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/suite.py
--rw-r--r--   0 cdent      (503) staff       (20)    11447 2022-09-23 14:11:15.000000 gabbi-2.8.0/gabbi/suitemaker.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.058127 gabbi-2.8.0/gabbi/tests/
--rw-r--r--   0 cdent      (503) staff       (20)      299 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/README
--rw-r--r--   0 cdent      (503) staff       (20)      623 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/__init__.py
--rw-r--r--   0 cdent      (503) staff       (20)      845 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/custom_response_handler.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.059405 gabbi-2.8.0/gabbi/tests/gabbits_handlers/
--rw-r--r--   0 cdent      (503) staff       (20)       43 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/cat.json
--rw-r--r--   0 cdent      (503) staff       (20)       21 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/data.json
--rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/pets.json
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.060134 gabbi-2.8.0/gabbi/tests/gabbits_handlers/subdir/
--rw-r--r--   0 cdent      (503) staff       (20)       15 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/subdir/data.yaml
--rw-r--r--   0 cdent      (503) staff       (20)       52 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/subdir/pets.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      140 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/subdir/values.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      334 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/values.json
--rw-r--r--   0 cdent      (503) staff       (20)      796 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_handlers/yaml-from-disk.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.060379 gabbi-2.8.0/gabbi/tests/gabbits_inner/
--rw-r--r--   0 cdent      (503) staff       (20)      118 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_inner/inner.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.068691 gabbi-2.8.0/gabbi/tests/gabbits_intercept/
--rw-r--r--   0 cdent      (503) staff       (20)     2543 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/backref.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     2261 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/casting.yaml
--rw-r--r--   0 cdent      (503) staff       (20)       43 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/cat.json
--rw-r--r--   0 cdent      (503) staff       (20)     4676 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/coerce.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     1519 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/contenttype.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      732 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/cookie.yaml
--rw-r--r--   0 cdent      (503) staff       (20)       21 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/data.json
--rw-r--r--   0 cdent      (503) staff       (20)     1999 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/data.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      546 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/disable-response-handler.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      382 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/failskip.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      216 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/fixture.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      756 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/forbiddenheaders.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      240 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/header-key.yaml
--rw-r--r--   0 cdent      (503) staff       (20)        0 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/horse
--rw-r--r--   0 cdent      (503) staff       (20)      383 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/host-header.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     1544 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-extensions.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      731 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-left-side.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      640 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-right-side.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      763 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/jsonbody.yaml
--rw-r--r--   0 cdent      (503) staff       (20)   110735 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/kitten.png
--rw-r--r--   0 cdent      (503) staff       (20)     1074 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/last-url.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      903 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/method-shortcut.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/pets.json
--rw-r--r--   0 cdent      (503) staff       (20)     1238 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/poll.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      484 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/prefix.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     1466 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/queryparams.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      455 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/regex.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     3500 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/self.yaml
--rw-r--r--   0 cdent      (503) staff       (20)       72 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/skipall.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.068951 gabbi-2.8.0/gabbi/tests/gabbits_intercept/subdir/
--rw-r--r--   0 cdent      (503) staff       (20)      140 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/subdir/values.yaml
--rw-r--r--   0 cdent      (503) staff       (20)    14258 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/utf8.txt
--rw-r--r--   0 cdent      (503) staff       (20)      334 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/values.json
--rw-r--r--   0 cdent      (503) staff       (20)      135 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_intercept/verbosity.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.069469 gabbi-2.8.0/gabbi/tests/gabbits_live/
--rw-r--r--   0 cdent      (503) staff       (20)      557 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_live/google.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      602 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/gabbits_live/host-header.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.071139 gabbi-2.8.0/gabbi/tests/gabbits_runner/
--rw-r--r--   0 cdent      (503) staff       (20)       57 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/failure.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      203 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/nan.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.071398 gabbi-2.8.0/gabbi/tests/gabbits_runner/subdir/
--rw-r--r--   0 cdent      (503) staff       (20)       29 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/subdir/sample.json
--rw-r--r--   0 cdent      (503) staff       (20)       60 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/success.yaml
--rw-r--r--   0 cdent      (503) staff       (20)       60 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/success_alt.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      145 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/test_data.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      291 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/test_verbose.yaml
--rw-r--r--   0 cdent      (503) staff       (20)      120 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_runner/verbosity.yaml
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.071640 gabbi-2.8.0/gabbi/tests/gabbits_unsafe_yaml/
--rw-r--r--   0 cdent      (503) staff       (20)      193 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/gabbits_unsafe_yaml/nan.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     6393 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/simple_wsgi.py
--rw-r--r--   0 cdent      (503) staff       (20)     1953 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/test_data_to_string.py
--rw-r--r--   0 cdent      (503) staff       (20)     5248 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_driver.py
--rw-r--r--   0 cdent      (503) staff       (20)     1798 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_fixtures.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.071885 gabbi-2.8.0/gabbi/tests/test_gabbits/
--rw-r--r--   0 cdent      (503) staff       (20)      210 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_gabbits/sample.yaml
--rw-r--r--   0 cdent      (503) staff       (20)    18354 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/test_handlers.py
--rw-r--r--   0 cdent      (503) staff       (20)     7286 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_history.py
--rw-r--r--   0 cdent      (503) staff       (20)     2220 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/test_inner_fixture.py
--rw-r--r--   0 cdent      (503) staff       (20)     3222 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/test_intercept.py
--rw-r--r--   0 cdent      (503) staff       (20)     2098 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_jsonpath.py
--rw-r--r--   0 cdent      (503) staff       (20)     1888 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/test_live.py
--rw-r--r--   0 cdent      (503) staff       (20)     2710 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_load_data_file.py
--rw-r--r--   0 cdent      (503) staff       (20)     5948 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_parse_url.py
--rw-r--r--   0 cdent      (503) staff       (20)     2236 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_replacers.py
--rw-r--r--   0 cdent      (503) staff       (20)    12727 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/test_runner.py
--rw-r--r--   0 cdent      (503) staff       (20)     1758 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_suite.py
--rw-r--r--   0 cdent      (503) staff       (20)     6763 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_suitemaker.py
--rw-r--r--   0 cdent      (503) staff       (20)     1438 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_syntax_warning.py
--rw-r--r--   0 cdent      (503) staff       (20)     1768 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/test_unsafe_yaml.py
--rw-r--r--   0 cdent      (503) staff       (20)     2259 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/test_use_prior_test.py
--rw-r--r--   0 cdent      (503) staff       (20)    10468 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/tests/test_utils.py
--rw-r--r--   0 cdent      (503) staff       (20)     1765 2022-09-22 16:22:17.000000 gabbi-2.8.0/gabbi/tests/test_yaml_disk_loading_jsonhandler.py
--rw-r--r--   0 cdent      (503) staff       (20)     1246 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/util.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.072132 gabbi-2.8.0/gabbi/tests/warning_gabbits/
--rw-r--r--   0 cdent      (503) staff       (20)       87 2022-07-22 21:46:23.000000 gabbi-2.8.0/gabbi/tests/warning_gabbits/underscore_sample.yaml
--rw-r--r--   0 cdent      (503) staff       (20)     5959 2022-09-22 16:07:15.000000 gabbi-2.8.0/gabbi/utils.py
-drwxr-xr-x   0 cdent      (503) staff       (20)        0 2022-09-23 14:32:29.050014 gabbi-2.8.0/gabbi.egg-info/
--rw-r--r--   0 cdent      (503) staff       (20)     4625 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/PKG-INFO
--rw-r--r--   0 cdent      (503) staff       (20)     4511 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/SOURCES.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/dependency_links.txt
--rw-r--r--   0 cdent      (503) staff       (20)       47 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/entry_points.txt
--rw-r--r--   0 cdent      (503) staff       (20)        1 2022-09-23 14:31:45.000000 gabbi-2.8.0/gabbi.egg-info/not-zip-safe
--rw-r--r--   0 cdent      (503) staff       (20)       46 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/pbr.json
--rw-r--r--   0 cdent      (503) staff       (20)      100 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/requires.txt
--rw-r--r--   0 cdent      (503) staff       (20)        6 2022-09-23 14:32:28.000000 gabbi-2.8.0/gabbi.egg-info/top_level.txt
--rw-r--r--   0 cdent      (503) staff       (20)        4 2022-07-22 21:46:23.000000 gabbi-2.8.0/requirements-dev.txt
--rw-r--r--   0 cdent      (503) staff       (20)      100 2022-09-22 16:22:17.000000 gabbi-2.8.0/requirements.txt
--rw-r--r--   0 cdent      (503) staff       (20)     1042 2022-09-23 14:32:29.072821 gabbi-2.8.0/setup.cfg
--rw-r--r--   0 cdent      (503) staff       (20)      650 2022-07-22 21:46:23.000000 gabbi-2.8.0/setup.py
--rwxr-xr-x   0 cdent      (503) staff       (20)      704 2022-09-22 16:22:17.000000 gabbi-2.8.0/test-failskip.sh
--rwxr-xr-x   0 cdent      (503) staff       (20)      548 2022-07-22 21:46:23.000000 gabbi-2.8.0/test-limit.sh
--rw-r--r--   0 cdent      (503) staff       (20)       78 2022-09-22 18:07:52.000000 gabbi-2.8.0/test-requirements.txt
--rwxr-xr-x   0 cdent      (503) staff       (20)      184 2022-07-22 21:46:23.000000 gabbi-2.8.0/test-verbosity.sh
--rw-r--r--   0 cdent      (503) staff       (20)     2587 2022-09-22 18:07:52.000000 gabbi-2.8.0/tox.ini
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.043651 gabbi-2.9.0/
+-rw-r--r--   0 cdent      (503) staff       (20)       27 2022-07-22 21:46:23.000000 gabbi-2.9.0/.coveragerc
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:19.982316 gabbi-2.9.0/.github/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:19.997572 gabbi-2.9.0/.github/workflows/
+-rw-r--r--   0 cdent      (503) staff       (20)     1179 2022-09-22 16:22:17.000000 gabbi-2.9.0/.github/workflows/docker.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     1526 2023-06-26 12:42:37.000000 gabbi-2.9.0/.github/workflows/tests.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.9.0/.pyup.yml
+-rw-r--r--   0 cdent      (503) staff       (20)      223 2022-09-22 16:07:15.000000 gabbi-2.9.0/.stestr.conf
+-rw-r--r--   0 cdent      (503) staff       (20)     1167 2023-06-26 12:55:19.000000 gabbi-2.9.0/AUTHORS
+-rw-r--r--   0 cdent      (503) staff       (20)     2307 2022-09-22 16:07:15.000000 gabbi-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 cdent      (503) staff       (20)    27123 2023-06-26 12:55:19.000000 gabbi-2.9.0/ChangeLog
+-rw-r--r--   0 cdent      (503) staff       (20)      257 2022-09-22 16:22:17.000000 gabbi-2.9.0/Dockerfile
+-rw-r--r--   0 cdent      (503) staff       (20)      593 2022-07-22 21:46:23.000000 gabbi-2.9.0/LICENSE
+-rw-r--r--   0 cdent      (503) staff       (20)     1022 2023-06-26 12:49:27.000000 gabbi-2.9.0/Makefile
+-rw-r--r--   0 cdent      (503) staff       (20)     4625 2023-06-26 12:55:20.043759 gabbi-2.9.0/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     3607 2022-09-22 18:07:52.000000 gabbi-2.9.0/README.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:19.997884 gabbi-2.9.0/docs/
+-rw-r--r--   0 cdent      (503) staff       (20)     6767 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/Makefile
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.006865 gabbi-2.9.0/docs/source/
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.007214 gabbi-2.9.0/docs/source/_static/
+-rw-r--r--   0 cdent      (503) staff       (20)      145 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/_static/theme_override.css
+-rw-r--r--   0 cdent      (503) staff       (20)     8327 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/conf.py
+-rw-r--r--   0 cdent      (503) staff       (20)      904 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/example.py
+-rw-r--r--   0 cdent      (503) staff       (20)      292 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/example.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     7388 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/example.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     3775 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/faq.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     3322 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/fixtures.rst
+-rw-r--r--   0 cdent      (503) staff       (20)    14991 2022-09-23 14:13:29.000000 gabbi-2.9.0/docs/source/format.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     2339 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/gabbi.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     7316 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/handlers.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     1601 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/host.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     4650 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/index.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     5042 2022-07-22 21:46:23.000000 gabbi-2.9.0/docs/source/jsonpath.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     4508 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/loader.rst
+-rw-r--r--   0 cdent      (503) staff       (20)      881 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/pytest-example.py
+-rw-r--r--   0 cdent      (503) staff       (20)      970 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/pytest3.0-example.py
+-rw-r--r--   0 cdent      (503) staff       (20)     9945 2023-06-26 12:46:07.000000 gabbi-2.9.0/docs/source/release.rst
+-rw-r--r--   0 cdent      (503) staff       (20)     2666 2022-09-22 16:22:17.000000 gabbi-2.9.0/docs/source/runner.rst
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.017652 gabbi-2.9.0/gabbi/
+-rw-r--r--   0 cdent      (503) staff       (20)      610 2023-06-26 12:46:19.000000 gabbi-2.9.0/gabbi/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)    26287 2022-09-23 14:11:15.000000 gabbi-2.9.0/gabbi/case.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10255 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/driver.py
+-rw-r--r--   0 cdent      (503) staff       (20)      915 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/exception.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3113 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/fixture.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.021257 gabbi-2.9.0/gabbi/handlers/
+-rw-r--r--   0 cdent      (503) staff       (20)      915 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/handlers/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4185 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/handlers/base.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2903 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/handlers/core.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5362 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/handlers/jsonhandler.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1524 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/handlers/yaml_disk_loading_jsonhandler.py
+-rw-r--r--   0 cdent      (503) staff       (20)     8040 2022-09-23 14:11:15.000000 gabbi-2.9.0/gabbi/httpclient.py
+-rw-r--r--   0 cdent      (503) staff       (20)      841 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/json_parser.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4503 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/pytester.py
+-rw-r--r--   0 cdent      (503) staff       (20)     4484 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/reporter.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10335 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/runner.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5247 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/suite.py
+-rw-r--r--   0 cdent      (503) staff       (20)    11447 2022-09-23 14:11:15.000000 gabbi-2.9.0/gabbi/suitemaker.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.029547 gabbi-2.9.0/gabbi/tests/
+-rw-r--r--   0 cdent      (503) staff       (20)      299 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/README
+-rw-r--r--   0 cdent      (503) staff       (20)      623 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/__init__.py
+-rw-r--r--   0 cdent      (503) staff       (20)      845 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/custom_response_handler.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.030898 gabbi-2.9.0/gabbi/tests/gabbits_handlers/
+-rw-r--r--   0 cdent      (503) staff       (20)       43 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/cat.json
+-rw-r--r--   0 cdent      (503) staff       (20)       21 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/data.json
+-rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/pets.json
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.031609 gabbi-2.9.0/gabbi/tests/gabbits_handlers/subdir/
+-rw-r--r--   0 cdent      (503) staff       (20)       15 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/subdir/data.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)       52 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/subdir/pets.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      140 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/subdir/values.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      334 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/values.json
+-rw-r--r--   0 cdent      (503) staff       (20)      796 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_handlers/yaml-from-disk.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.031890 gabbi-2.9.0/gabbi/tests/gabbits_inner/
+-rw-r--r--   0 cdent      (503) staff       (20)      118 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_inner/inner.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.039996 gabbi-2.9.0/gabbi/tests/gabbits_intercept/
+-rw-r--r--   0 cdent      (503) staff       (20)     2543 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/backref.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     2261 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/casting.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)       43 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/cat.json
+-rw-r--r--   0 cdent      (503) staff       (20)     4676 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/coerce.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     1519 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/contenttype.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      732 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/cookie.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)       21 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/data.json
+-rw-r--r--   0 cdent      (503) staff       (20)     1999 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/data.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      546 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/disable-response-handler.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      382 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/failskip.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      216 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/fixture.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      756 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/forbiddenheaders.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      240 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/header-key.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)        0 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/horse
+-rw-r--r--   0 cdent      (503) staff       (20)      383 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/host-header.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     1544 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-extensions.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      731 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-left-side.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      640 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-right-side.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      763 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/jsonbody.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)   110735 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/kitten.png
+-rw-r--r--   0 cdent      (503) staff       (20)     1074 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/last-url.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      903 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/method-shortcut.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      123 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/pets.json
+-rw-r--r--   0 cdent      (503) staff       (20)     1238 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/poll.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      484 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/prefix.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     1466 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/queryparams.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      455 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/regex.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     3500 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/self.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)       72 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/skipall.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.040276 gabbi-2.9.0/gabbi/tests/gabbits_intercept/subdir/
+-rw-r--r--   0 cdent      (503) staff       (20)      140 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/subdir/values.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)    14258 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/utf8.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      334 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/values.json
+-rw-r--r--   0 cdent      (503) staff       (20)      135 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_intercept/verbosity.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.040777 gabbi-2.9.0/gabbi/tests/gabbits_live/
+-rw-r--r--   0 cdent      (503) staff       (20)      557 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_live/google.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      602 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/gabbits_live/host-header.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.042419 gabbi-2.9.0/gabbi/tests/gabbits_runner/
+-rw-r--r--   0 cdent      (503) staff       (20)       57 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/failure.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      203 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/nan.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.042641 gabbi-2.9.0/gabbi/tests/gabbits_runner/subdir/
+-rw-r--r--   0 cdent      (503) staff       (20)       29 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/subdir/sample.json
+-rw-r--r--   0 cdent      (503) staff       (20)       60 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/success.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)       60 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/success_alt.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      145 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/test_data.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      291 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/test_verbose.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)      120 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_runner/verbosity.yaml
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.042873 gabbi-2.9.0/gabbi/tests/gabbits_unsafe_yaml/
+-rw-r--r--   0 cdent      (503) staff       (20)      193 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/gabbits_unsafe_yaml/nan.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     6393 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/simple_wsgi.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1953 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/test_data_to_string.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5248 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_driver.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1798 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_fixtures.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.043111 gabbi-2.9.0/gabbi/tests/test_gabbits/
+-rw-r--r--   0 cdent      (503) staff       (20)      210 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_gabbits/sample.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)    18354 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/test_handlers.py
+-rw-r--r--   0 cdent      (503) staff       (20)     7286 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_history.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2220 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/test_inner_fixture.py
+-rw-r--r--   0 cdent      (503) staff       (20)     3222 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/test_intercept.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2098 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_jsonpath.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1888 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/test_live.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2710 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_load_data_file.py
+-rw-r--r--   0 cdent      (503) staff       (20)     5948 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_parse_url.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2236 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_replacers.py
+-rw-r--r--   0 cdent      (503) staff       (20)    12727 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/test_runner.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1758 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_suite.py
+-rw-r--r--   0 cdent      (503) staff       (20)     6763 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_suitemaker.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1438 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_syntax_warning.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1768 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/test_unsafe_yaml.py
+-rw-r--r--   0 cdent      (503) staff       (20)     2259 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/test_use_prior_test.py
+-rw-r--r--   0 cdent      (503) staff       (20)    10468 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/tests/test_utils.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1765 2022-09-22 16:22:17.000000 gabbi-2.9.0/gabbi/tests/test_yaml_disk_loading_jsonhandler.py
+-rw-r--r--   0 cdent      (503) staff       (20)     1246 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/util.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.043390 gabbi-2.9.0/gabbi/tests/warning_gabbits/
+-rw-r--r--   0 cdent      (503) staff       (20)       87 2022-07-22 21:46:23.000000 gabbi-2.9.0/gabbi/tests/warning_gabbits/underscore_sample.yaml
+-rw-r--r--   0 cdent      (503) staff       (20)     5959 2022-09-22 16:07:15.000000 gabbi-2.9.0/gabbi/utils.py
+drwxr-xr-x   0 cdent      (503) staff       (20)        0 2023-06-26 12:55:20.019738 gabbi-2.9.0/gabbi.egg-info/
+-rw-r--r--   0 cdent      (503) staff       (20)     4625 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/PKG-INFO
+-rw-r--r--   0 cdent      (503) staff       (20)     4511 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/SOURCES.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/dependency_links.txt
+-rw-r--r--   0 cdent      (503) staff       (20)       47 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/entry_points.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        1 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/not-zip-safe
+-rw-r--r--   0 cdent      (503) staff       (20)       46 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/pbr.json
+-rw-r--r--   0 cdent      (503) staff       (20)      107 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/requires.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        6 2023-06-26 12:55:19.000000 gabbi-2.9.0/gabbi.egg-info/top_level.txt
+-rw-r--r--   0 cdent      (503) staff       (20)        4 2022-07-22 21:46:23.000000 gabbi-2.9.0/requirements-dev.txt
+-rw-r--r--   0 cdent      (503) staff       (20)      107 2023-06-26 12:42:37.000000 gabbi-2.9.0/requirements.txt
+-rw-r--r--   0 cdent      (503) staff       (20)     1042 2023-06-26 12:55:20.044225 gabbi-2.9.0/setup.cfg
+-rw-r--r--   0 cdent      (503) staff       (20)      650 2022-07-22 21:46:23.000000 gabbi-2.9.0/setup.py
+-rwxr-xr-x   0 cdent      (503) staff       (20)      690 2023-06-26 12:42:37.000000 gabbi-2.9.0/test-failskip.sh
+-rwxr-xr-x   0 cdent      (503) staff       (20)      548 2022-07-22 21:46:23.000000 gabbi-2.9.0/test-limit.sh
+-rw-r--r--   0 cdent      (503) staff       (20)       78 2023-06-23 15:23:11.000000 gabbi-2.9.0/test-requirements.txt
+-rwxr-xr-x   0 cdent      (503) staff       (20)      184 2022-07-22 21:46:23.000000 gabbi-2.9.0/test-verbosity.sh
+-rw-r--r--   0 cdent      (503) staff       (20)     2123 2023-06-26 12:42:37.000000 gabbi-2.9.0/tox.ini
```

### Comparing `gabbi-2.8.0/.github/workflows/docker.yaml` & `gabbi-2.9.0/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/AUTHORS` & `gabbi-2.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/CONTRIBUTING.md` & `gabbi-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/ChangeLog` & `gabbi-2.9.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+2.9.0
+-----
+
+* release 2.9.0
+* Pin urllib3 < 2.0.0 (#322)
+
 2.8.0
 -----
 
 * Release 2.8.0
 * Add timeout with a default of 30s.  Fixes #318. (#319)
 * Update to require stestr 4.0.1 (#321)
 
@@ -1108,16 +1114,16 @@
 * Point the docs bullet somewhere useful
 * Add docs badge
 * Make a make rule for making the docs
 * Add some initial doc files
 * Initial commit of sphinx infrastructure
 * Automate test and build a bit more
 
-0.1.0
------
+v0.1.0
+------
 
 * Extract classes to their own files
 * Add some docs to GabbiFixture
 * Start fixtures at the suite level not the TestCase
 * Implement declarable fixtures
 * Allow request body to come from data structure or file
 * Update gabbi driver to reflect new test handling
```

### Comparing `gabbi-2.8.0/LICENSE` & `gabbi-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/Makefile` & `gabbi-2.9.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	rm -r .eggs || true
 	rm -r gabbi.egg-info || true
 
 docs:
 	cd docs ; $(MAKE) html
 
 test:
-	tox --skip-missing-interpreters -p 8
+	tox --skip-missing-interpreters
 
 dist: test
 	python3 setup.py sdist bdist_wheel
 
 release: clean test cleanagain tagv pypi
 
 pypi:
```

### Comparing `gabbi-2.8.0/PKG-INFO` & `gabbi-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gabbi
-Version: 2.8.0
+Version: 2.9.0
 Summary: Declarative HTTP testing library
 Home-page: https://github.com/cdent/gabbi
 Author: Chris Dent
 Author-email: cdent@anticdent.org
 License: Apache-2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `gabbi-2.8.0/README.rst` & `gabbi-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/Makefile` & `gabbi-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/conf.py` & `gabbi-2.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/example.py` & `gabbi-2.9.0/docs/source/example.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/example.yaml` & `gabbi-2.9.0/docs/source/example.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/faq.rst` & `gabbi-2.9.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/fixtures.rst` & `gabbi-2.9.0/docs/source/fixtures.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/format.rst` & `gabbi-2.9.0/docs/source/format.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/gabbi.rst` & `gabbi-2.9.0/docs/source/gabbi.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/handlers.rst` & `gabbi-2.9.0/docs/source/handlers.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/host.rst` & `gabbi-2.9.0/docs/source/host.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/index.rst` & `gabbi-2.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/jsonpath.rst` & `gabbi-2.9.0/docs/source/jsonpath.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/loader.rst` & `gabbi-2.9.0/docs/source/loader.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/pytest-example.py` & `gabbi-2.9.0/docs/source/pytest-example.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/pytest3.0-example.py` & `gabbi-2.9.0/docs/source/pytest3.0-example.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/docs/source/release.rst` & `gabbi-2.9.0/docs/source/release.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Release Notes
 =============
 
 These are informal release notes for gabbi since version 1.0.0,
 highlighting major features and changes. For more detail see
 the `commit logs`_ on GitHub.
 
+2.9.0
+-----
+
+* Pin to urllib3 <2.0.0 to avoid issues with changes in constructors.
+
 2.8.0
 -----
 
 * Add timeout parameter per test, defaulting to 30 seconds.
 * Ensure stestr > 4.0.0 in test-requirements.txt
 
 2.7.2
```

### Comparing `gabbi-2.8.0/docs/source/runner.rst` & `gabbi-2.9.0/docs/source/runner.rst`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/__init__.py` & `gabbi-2.9.0/gabbi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 """See gabbi.driver and gabbbi.case."""
 
-__version__ = '2.8.0'
+__version__ = '2.9.0'
```

### Comparing `gabbi-2.8.0/gabbi/case.py` & `gabbi-2.9.0/gabbi/case.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/driver.py` & `gabbi-2.9.0/gabbi/driver.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/exception.py` & `gabbi-2.9.0/gabbi/exception.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/fixture.py` & `gabbi-2.9.0/gabbi/fixture.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/handlers/__init__.py` & `gabbi-2.9.0/gabbi/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/handlers/base.py` & `gabbi-2.9.0/gabbi/handlers/base.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/handlers/core.py` & `gabbi-2.9.0/gabbi/handlers/core.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/handlers/jsonhandler.py` & `gabbi-2.9.0/gabbi/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/handlers/yaml_disk_loading_jsonhandler.py` & `gabbi-2.9.0/gabbi/handlers/yaml_disk_loading_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/httpclient.py` & `gabbi-2.9.0/gabbi/httpclient.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/json_parser.py` & `gabbi-2.9.0/gabbi/json_parser.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/pytester.py` & `gabbi-2.9.0/gabbi/pytester.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/reporter.py` & `gabbi-2.9.0/gabbi/reporter.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/runner.py` & `gabbi-2.9.0/gabbi/runner.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/suite.py` & `gabbi-2.9.0/gabbi/suite.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/suitemaker.py` & `gabbi-2.9.0/gabbi/suitemaker.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/__init__.py` & `gabbi-2.9.0/gabbi/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/custom_response_handler.py` & `gabbi-2.9.0/gabbi/tests/custom_response_handler.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_handlers/yaml-from-disk.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_handlers/yaml-from-disk.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/backref.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/backref.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/casting.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/casting.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/coerce.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/coerce.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/contenttype.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/contenttype.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/cookie.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/cookie.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/data.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/data.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/disable-response-handler.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/disable-response-handler.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/forbiddenheaders.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/forbiddenheaders.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-extensions.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-extensions.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-left-side.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-left-side.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/json-right-side.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/json-right-side.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/jsonbody.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/jsonbody.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/kitten.png` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/kitten.png`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/last-url.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/last-url.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/method-shortcut.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/method-shortcut.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/poll.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/poll.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/queryparams.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/queryparams.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/self.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/self.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_intercept/utf8.txt` & `gabbi-2.9.0/gabbi/tests/gabbits_intercept/utf8.txt`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_live/google.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_live/google.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/gabbits_live/host-header.yaml` & `gabbi-2.9.0/gabbi/tests/gabbits_live/host-header.yaml`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/simple_wsgi.py` & `gabbi-2.9.0/gabbi/tests/simple_wsgi.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_data_to_string.py` & `gabbi-2.9.0/gabbi/tests/test_data_to_string.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_driver.py` & `gabbi-2.9.0/gabbi/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_fixtures.py` & `gabbi-2.9.0/gabbi/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_handlers.py` & `gabbi-2.9.0/gabbi/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_history.py` & `gabbi-2.9.0/gabbi/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_inner_fixture.py` & `gabbi-2.9.0/gabbi/tests/test_inner_fixture.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_intercept.py` & `gabbi-2.9.0/gabbi/tests/test_intercept.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_jsonpath.py` & `gabbi-2.9.0/gabbi/tests/test_jsonpath.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_live.py` & `gabbi-2.9.0/gabbi/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_load_data_file.py` & `gabbi-2.9.0/gabbi/tests/test_load_data_file.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_parse_url.py` & `gabbi-2.9.0/gabbi/tests/test_parse_url.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_replacers.py` & `gabbi-2.9.0/gabbi/tests/test_replacers.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_runner.py` & `gabbi-2.9.0/gabbi/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_suite.py` & `gabbi-2.9.0/gabbi/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_suitemaker.py` & `gabbi-2.9.0/gabbi/tests/test_suitemaker.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_syntax_warning.py` & `gabbi-2.9.0/gabbi/tests/test_syntax_warning.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_unsafe_yaml.py` & `gabbi-2.9.0/gabbi/tests/test_unsafe_yaml.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_use_prior_test.py` & `gabbi-2.9.0/gabbi/tests/test_use_prior_test.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_utils.py` & `gabbi-2.9.0/gabbi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/test_yaml_disk_loading_jsonhandler.py` & `gabbi-2.9.0/gabbi/tests/test_yaml_disk_loading_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/tests/util.py` & `gabbi-2.9.0/gabbi/tests/util.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi/utils.py` & `gabbi-2.9.0/gabbi/utils.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/gabbi.egg-info/PKG-INFO` & `gabbi-2.9.0/gabbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gabbi
-Version: 2.8.0
+Version: 2.9.0
 Summary: Declarative HTTP testing library
 Home-page: https://github.com/cdent/gabbi
 Author: Chris Dent
 Author-email: cdent@anticdent.org
 License: Apache-2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `gabbi-2.8.0/gabbi.egg-info/SOURCES.txt` & `gabbi-2.9.0/gabbi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/setup.cfg` & `gabbi-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/setup.py` & `gabbi-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `gabbi-2.8.0/test-limit.sh` & `gabbi-2.9.0/test-limit.sh`

 * *Files identical despite different names*

