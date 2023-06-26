# Comparing `tmp/niapi-0.3.0.tar.gz` & `tmp/niapi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niapi-0.3.0.tar", max compression
+gzip compressed data, was "niapi-0.4.0.tar", max compression
```

## Comparing `niapi-0.3.0.tar` & `niapi-0.4.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
--rw-r--r--   0        0        0     1080 2023-06-25 21:11:00.355069 niapi-0.3.0/LICENSE
--rw-r--r--   0        0        0     9075 2023-06-25 21:11:00.355069 niapi-0.3.0/docs/PYPI_README.md
--rw-r--r--   0        0        0      620 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/asgi.py
--rw-r--r--   0        0        0     3861 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/cli.py
--rw-r--r--   0        0        0      784 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/calculator/__init__.py
--rw-r--r--   0        0        0      123 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/system/__init__.py
--rw-r--r--   0        0        0      125 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/system/controllers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/system/controllers/system.py
--rw-r--r--   0        0        0      203 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/urls.py
--rw-r--r--   0        0        0      120 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/__init__.py
--rw-r--r--   0        0        0      116 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/controllers/__init__.py
--rw-r--r--   0        0        0      688 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/controllers/web.py
--rw-r--r--   0        0        0    57551 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/badge.png
--rw-r--r--   0        0        0      101 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/input.css
--rw-r--r--   0        0        0     2892 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/logo.svg
--rw-r--r--   0        0        0    30881 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/style.css
--rw-r--r--   0        0        0       16 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/tailwind/_base.css
--rw-r--r--   0        0        0       22 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/tailwind/_components.css
--rw-r--r--   0        0        0       21 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/resources/tailwind/_utilities.css
--rw-r--r--   0        0        0     2347 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/templates/base/base.html
--rw-r--r--   0        0        0     7386 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/templates/base/footer.html
--rw-r--r--   0        0        0     8494 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/templates/base/nav.html
--rw-r--r--   0        0        0    12595 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/domain/web/templates/index.html
--rw-r--r--   0        0        0      282 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/__init__.py
--rw-r--r--   0        0        0      198 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/cors.py
--rw-r--r--   0        0        0     3904 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/exceptions.py
--rw-r--r--   0        0        0     3802 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/log/__init__.py
--rw-r--r--   0        0        0     9051 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/log/controller.py
--rw-r--r--   0        0        0     2093 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/log/utils.py
--rw-r--r--   0        0        0     1196 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/openapi.py
--rw-r--r--   0        0        0      673 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/schema.py
--rw-r--r--   0        0        0     3458 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/serialization.py
--rw-r--r--   0        0        0    12254 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/settings.py
--rw-r--r--   0        0        0      735 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/static_files.py
--rw-r--r--   0        0        0      425 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/lib/template.py
--rw-r--r--   0        0        0      366 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/metadata.py
--rw-r--r--   0        0        0        0 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/py.typed
--rw-r--r--   0        0        0     5434 2023-06-25 21:11:00.363069 niapi-0.3.0/niapi/utils.py
--rw-r--r--   0        0        0     7111 2023-06-25 21:11:00.367069 niapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10876 1970-01-01 00:00:00.000000 niapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-26 05:00:44.153085 niapi-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10147 2023-06-26 05:00:44.153085 niapi-0.4.0/docs/PYPI_README.md
+-rw-r--r--   0        0        0      620 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/asgi.py
+-rw-r--r--   0        0        0     3747 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/cli.py
+-rw-r--r--   0        0        0      865 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/calculator/__init__.py
+-rw-r--r--   0        0        0      137 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/calculator/controllers/__init__.py
+-rw-r--r--   0        0        0      247 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/calculator/controllers/calculator.py
+-rw-r--r--   0        0        0      760 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/calculator/schema.py
+-rw-r--r--   0        0        0      123 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/system/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/system/controllers/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/system/controllers/system.py
+-rw-r--r--   0        0        0      292 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/urls.py
+-rw-r--r--   0        0        0      120 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/controllers/__init__.py
+-rw-r--r--   0        0        0      688 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/controllers/web.py
+-rw-r--r--   0        0        0    57551 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/badge.png
+-rw-r--r--   0        0        0      101 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/input.css
+-rw-r--r--   0        0        0     2892 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/logo.svg
+-rw-r--r--   0        0        0    32444 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/style.css
+-rw-r--r--   0        0        0       16 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/tailwind/_base.css
+-rw-r--r--   0        0        0       22 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/tailwind/_components.css
+-rw-r--r--   0        0        0       21 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/resources/tailwind/_utilities.css
+-rw-r--r--   0        0        0     2347 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/templates/base/base.html
+-rw-r--r--   0        0        0     7386 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/templates/base/footer.html
+-rw-r--r--   0        0        0    11243 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/templates/base/nav.html
+-rw-r--r--   0        0        0    12595 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/domain/web/templates/index.html
+-rw-r--r--   0        0        0      282 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/cors.py
+-rw-r--r--   0        0        0     3904 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/exceptions.py
+-rw-r--r--   0        0        0     3802 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/log/__init__.py
+-rw-r--r--   0        0        0     9051 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/log/controller.py
+-rw-r--r--   0        0        0     2093 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/log/utils.py
+-rw-r--r--   0        0        0     1196 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/openapi.py
+-rw-r--r--   0        0        0      673 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/schema.py
+-rw-r--r--   0        0        0     3458 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/serialization.py
+-rw-r--r--   0        0        0    12254 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/settings.py
+-rw-r--r--   0        0        0      735 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/static_files.py
+-rw-r--r--   0        0        0      425 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/lib/template.py
+-rw-r--r--   0        0        0      366 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/metadata.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/py.typed
+-rw-r--r--   0        0        0     4616 2023-06-26 05:00:44.169085 niapi-0.4.0/niapi/utils.py
+-rw-r--r--   0        0        0     7137 2023-06-26 05:00:44.173085 niapi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11987 1970-01-01 00:00:00.000000 niapi-0.4.0/PKG-INFO
```

### Comparing `niapi-0.3.0/LICENSE` & `niapi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/docs/PYPI_README.md` & `niapi-0.4.0/docs/PYPI_README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="https://github.com/JacobCoffee/niapi/blob/a82a86a1b8ca90f3c66a080291cfd074efcbfd1a/docs/images/PNG/Transparent/logo.png" alt="NIAPI Logo - Light" width="100%" height="auto" />
+  <img src="https://github.com/JacobCoffee/niapi/blob/a82a86a1b8ca90f3c66a080291cfd074efcbfd1a/docs/images/PNG/Transparent/logo.png?raw=True" alt="NIAPI Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
-| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-|-----------|:----|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CI/CD     |     | [![Latest Release](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml) [![ci](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml) [![CodeQL](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql)                                                                                                                                                                                                                                                                                                                                                                        |
-| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/niapi)](https://badge.fury.io/py/niapi) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/niapi)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| Quality   |     | [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=coverage)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Known Vulnerabilities](https://snyk.io/test/github/JacobCoffee/niapi/badge.svg)](https://snyk.io/test/github/JacobCoffee/niapi) |
-| Community |     | [![Twitter](https://img.shields.io/twitter/follow/_scriptr?style=social&logo=twitter)](https://twitter.com/_scriptr)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| Meta      |     | [![Litestar Framework](https://img.shields.io/badge/Litestar%20Framework-%E2%AD%90%20Litestar-202235.svg)](https://github.com/JacobCoffee/niapi) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/JacobCoffee?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/JacobCoffee)                                                                                                                                                                                                                                                            |
-
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-113-202235.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
+| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+|-----------|:----|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CI/CD     |     | [![Latest Release](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml) [![ci](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml) [![CodeQL](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/niapi)](https://badge.fury.io/py/niapi) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/niapi)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| Quality   |     | [![codecov](https://codecov.io/gh/JacobCoffee/niapi/branch/main/graph/badge.svg?token=SFT67X4MEQ)](https://codecov.io/gh/JacobCoffee/niapi) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=coverage)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Known Vulnerabilities](https://snyk.io/test/github/JacobCoffee/niapi/badge.svg)](https://snyk.io/test/github/JacobCoffee/niapi) |
+| Community |     | [![Twitter](https://img.shields.io/twitter/follow/_scriptr?style=social&logo=twitter)](https://twitter.com/_scriptr)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| Meta      |     | [![Litestar Framework](https://img.shields.io/badge/Litestar%20Framework-%E2%AD%90%20Litestar-202235.svg)](https://github.com/JacobCoffee/niapi) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-85c7f2.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-85c7f2.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/JacobCoffee?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/JacobCoffee)                                                                                                                                                                                                                                                                                                                                                                                                        |
+
+[![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-white.svg)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi)
+
 <!-- prettier-ignore-end -->
 
 </div>
 
 # `niapi` - Network Information API
 
 [//]: # "TODO"
@@ -68,15 +67,15 @@
 
 ```python
 # todo
 ```
 
 ## Contributing
 
-See [CONTRIBUTING.rst](../CONTRIBUTING.rst) for more information.
+See [CONTRIBUTING.rst](CONTRIBUTING.rst) for more information.
 
 Start the app:
 
 ```console
 app run-all
 ```
 
@@ -100,9 +99,9 @@
 - Using https://feathericons.dev/
 - Using TailwindCSS
 
 ## Screenshots
 
 [//]: # "TODO"
 
-![home.png](images/index.png)
-![home-dark.png](images/index-dark.png)
+![](https://github.com/JacobCoffee/niapi/blob/79eada17e1477feae3f3e15106331e4b81625157/docs/images/index-dark.png?raw=true)
+![](https://github.com/JacobCoffee/niapi/blob/79eada17e1477feae3f3e15106331e4b81625157/docs/images/index.png?raw=true)
```

### Comparing `niapi-0.3.0/niapi/__init__.py` & `niapi-0.4.0/niapi/__init__.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/asgi.py` & `niapi-0.4.0/niapi/asgi.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/cli.py` & `niapi-0.4.0/niapi/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,35 +85,30 @@
             "workers": 1 if bool(settings.server.RELOAD or settings.app.DEV_MODE) else settings.server.HTTP_WORKERS,
             "factory": settings.server.APP_LOC_IS_FACTORY,
             "loop": "uvloop",
             "no-access-log": True,
             "timeout-keep-alive": settings.server.KEEPALIVE,
         }
         if reload_dirs:
-            process_args.update({"reload-dir": reload_dirs})
+            process_args["reload-dir"] = reload_dirs
         subprocess.run(
             ["uvicorn", settings.server.APP_LOC, *_convert_uvicorn_args(process_args)], check=True  # noqa: S603, S607
         )
     finally:
         for process in multiprocessing.active_children():
             process.terminate()
         logger.info("⏏️  Shutdown complete")
         sys.exit()
 
 
 def _convert_uvicorn_args(args: dict[str, Any]) -> list[str]:
-    process_args = []
+    process_args: list[str] = []
     for arg, value in args.items():
-        if value is None:
-            pass
         if isinstance(value, list):
-            for val in value:
-                if val is None:
-                    pass
-                process_args.append(f"--{arg}={val}")
+            process_args.extend(f"--{arg}={val}" for val in value)
         if isinstance(value, bool):
             if value:
                 process_args.append(f"--{arg}")
         else:
             process_args.append(f"--{arg}={value}")
 
     return process_args
```

### Comparing `niapi-0.3.0/niapi/domain/__init__.py` & `niapi-0.4.0/niapi/domain/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
     from typing import Any
 
     from litestar.types import ControllerRouterHandler
 
-routes: list[ControllerRouterHandler] = [
-    # system.controllers.system.SystemController,
-    web.controllers.web.WebController,
-]
-
 __all__ = [
     "system",
     "web",
     "urls",
     "routes",
     "signature_namespace",
 ]
 
+routes: list[ControllerRouterHandler] = [
+    # system.controllers.system.SystemController,
+    web.controllers.web.WebController,
+]
+"""Routes for the application."""
+
 signature_namespace: Mapping[str, Any] = {
     "FilterTypes": FilterTypes,
     "EmailStr": EmailStr,
     "OffsetPagination": OffsetPagination,
 }
+"""Namespace for the application signature."""
```

### Comparing `niapi-0.3.0/niapi/domain/web/controllers/web.py` & `niapi-0.4.0/niapi/domain/web/controllers/web.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/domain/web/resources/badge.png` & `niapi-0.4.0/niapi/domain/web/resources/badge.png`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/domain/web/resources/logo.svg` & `niapi-0.4.0/niapi/domain/web/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/domain/web/resources/style.css` & `niapi-0.4.0/niapi/domain/web/resources/style.css`

 * *Files 4% similar despite different names*

```diff
@@ -765,18 +765,26 @@
   margin: -1px;
   overflow: hidden;
   clip: rect(0, 0, 0, 0);
   white-space: nowrap;
   border-width: 0;
 }
 
+.pointer-events-none {
+  pointer-events: none;
+}
+
 .fixed {
   position: fixed;
 }
 
+.absolute {
+  position: absolute;
+}
+
 .relative {
   position: relative;
 }
 
 .inset-0 {
   inset: 0px;
 }
@@ -786,14 +794,18 @@
   bottom: 0px;
 }
 
 .left-0 {
   left: 0px;
 }
 
+.right-0 {
+  right: 0px;
+}
+
 .z-10 {
   z-index: 10;
 }
 
 .-m-1 {
   margin: -0.25rem;
 }
@@ -856,14 +868,18 @@
   margin-top: 2rem;
 }
 
 .block {
   display: block;
 }
 
+.inline-block {
+  display: inline-block;
+}
+
 .flex {
   display: flex;
 }
 
 .inline-flex {
   display: inline-flex;
 }
@@ -896,14 +912,18 @@
   height: 2rem;
 }
 
 .h-full {
   height: 100%;
 }
 
+.h-5 {
+  height: 1.25rem;
+}
+
 .min-h-full {
   min-height: 100%;
 }
 
 .w-4 {
   width: 1rem;
 }
@@ -916,26 +936,38 @@
   width: auto;
 }
 
 .w-full {
   width: 100%;
 }
 
+.w-56 {
+  width: 14rem;
+}
+
+.w-5 {
+  width: 1.25rem;
+}
+
 .max-w-7xl {
   max-width: 80rem;
 }
 
 .flex-1 {
   flex: 1 1 0%;
 }
 
 .flex-grow {
   flex-grow: 1;
 }
 
+.origin-top-right {
+  transform-origin: top right;
+}
+
 .scale-100 {
   --tw-scale-x: 1;
   --tw-scale-y: 1;
   transform: translate(var(--tw-translate-x), var(--tw-translate-y))
     rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y))
     scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
 }
@@ -1058,14 +1090,18 @@
   border-radius: 0.5rem;
 }
 
 .rounded-md {
   border-radius: 0.375rem;
 }
 
+.rounded-full {
+  border-radius: 9999px;
+}
+
 .border-0 {
   border-width: 0px;
 }
 
 .border-b {
   border-bottom-width: 1px;
 }
@@ -1097,14 +1133,19 @@
 }
 
 .bg-white {
   --tw-bg-opacity: 1;
   background-color: rgb(255 255 255 / var(--tw-bg-opacity));
 }
 
+.bg-gray-100 {
+  --tw-bg-opacity: 1;
+  background-color: rgb(243 244 246 / var(--tw-bg-opacity));
+}
+
 .p-1 {
   padding: 0.25rem;
 }
 
 .p-1\.5 {
   padding: 0.375rem;
 }
@@ -1147,14 +1188,19 @@
 }
 
 .py-6 {
   padding-top: 1.5rem;
   padding-bottom: 1.5rem;
 }
 
+.px-4 {
+  padding-left: 1rem;
+  padding-right: 1rem;
+}
+
 .pb-12 {
   padding-bottom: 3rem;
 }
 
 .pb-8 {
   padding-bottom: 2rem;
 }
@@ -1167,14 +1213,18 @@
   padding-left: 0.75rem;
 }
 
 .pt-8 {
   padding-top: 2rem;
 }
 
+.text-left {
+  text-align: left;
+}
+
 .font-mono {
   font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas,
     "Liberation Mono", "Courier New", monospace;
 }
 
 .text-base {
   font-size: 1rem;
@@ -1250,42 +1300,32 @@
   color: rgb(17 24 39 / var(--tw-text-opacity));
 }
 
 .text-gray-900\/60 {
   color: rgb(17 24 39 / 0.6);
 }
 
-.text-neutral-900 {
-  --tw-text-opacity: 1;
-  color: rgb(23 23 23 / var(--tw-text-opacity));
-}
-
-.text-white {
-  --tw-text-opacity: 1;
-  color: rgb(255 255 255 / var(--tw-text-opacity));
-}
-
 .text-neutral-600 {
   --tw-text-opacity: 1;
   color: rgb(82 82 82 / var(--tw-text-opacity));
 }
 
-.text-slate-800 {
+.text-neutral-900 {
   --tw-text-opacity: 1;
-  color: rgb(30 41 59 / var(--tw-text-opacity));
+  color: rgb(23 23 23 / var(--tw-text-opacity));
 }
 
-.text-black {
+.text-white {
   --tw-text-opacity: 1;
-  color: rgb(0 0 0 / var(--tw-text-opacity));
+  color: rgb(255 255 255 / var(--tw-text-opacity));
 }
 
-.text-neutral-800 {
+.text-gray-700 {
   --tw-text-opacity: 1;
-  color: rgb(38 38 38 / var(--tw-text-opacity));
+  color: rgb(55 65 81 / var(--tw-text-opacity));
 }
 
 .antialiased {
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
 }
 
@@ -1300,14 +1340,23 @@
 .shadow-sm {
   --tw-shadow: 0 1px 2px 0 rgb(0 0 0 / 0.05);
   --tw-shadow-colored: 0 1px 2px 0 var(--tw-shadow-color);
   box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000),
     var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
 }
 
+.shadow-lg {
+  --tw-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1),
+    0 4px 6px -4px rgb(0 0 0 / 0.1);
+  --tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color),
+    0 4px 6px -4px var(--tw-shadow-color);
+  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000),
+    var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
+}
+
 .ring-1 {
   --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0
     var(--tw-ring-offset-width) var(--tw-ring-offset-color);
   --tw-ring-shadow: var(--tw-ring-inset) 0 0 0
     calc(1px + var(--tw-ring-offset-width)) var(--tw-ring-color);
   box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow),
     var(--tw-shadow, 0 0 #0000);
@@ -1318,14 +1367,23 @@
 }
 
 .ring-gray-300 {
   --tw-ring-opacity: 1;
   --tw-ring-color: rgb(209 213 219 / var(--tw-ring-opacity));
 }
 
+.ring-black {
+  --tw-ring-opacity: 1;
+  --tw-ring-color: rgb(0 0 0 / var(--tw-ring-opacity));
+}
+
+.ring-opacity-5 {
+  --tw-ring-opacity: 0.05;
+}
+
 .blur {
   --tw-blur: blur(8px);
   filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast)
     var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate)
     var(--tw-sepia) var(--tw-drop-shadow);
 }
 
@@ -1373,14 +1431,19 @@
 }
 
 .hover\:bg-red-500:hover {
   --tw-bg-opacity: 1;
   background-color: rgb(239 68 68 / var(--tw-bg-opacity));
 }
 
+.hover\:bg-gray-100:hover {
+  --tw-bg-opacity: 1;
+  background-color: rgb(243 244 246 / var(--tw-bg-opacity));
+}
+
 .hover\:text-blue-900:hover {
   --tw-text-opacity: 1;
   color: rgb(30 58 138 / var(--tw-text-opacity));
 }
 
 .hover\:text-gray-400:hover {
   --tw-text-opacity: 1;
@@ -1388,14 +1451,29 @@
 }
 
 .hover\:text-white:hover {
   --tw-text-opacity: 1;
   color: rgb(255 255 255 / var(--tw-text-opacity));
 }
 
+.hover\:text-gray-900:hover {
+  --tw-text-opacity: 1;
+  color: rgb(17 24 39 / var(--tw-text-opacity));
+}
+
+.hover\:text-gray-600:hover {
+  --tw-text-opacity: 1;
+  color: rgb(75 85 99 / var(--tw-text-opacity));
+}
+
+.focus\:outline-none:focus {
+  outline: 2px solid transparent;
+  outline-offset: 2px;
+}
+
 .focus\:ring-0:focus {
   --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0
     var(--tw-ring-offset-width) var(--tw-ring-offset-color);
   --tw-ring-shadow: var(--tw-ring-inset) 0 0 0
     calc(0px + var(--tw-ring-offset-width)) var(--tw-ring-color);
   box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow),
     var(--tw-shadow, 0 0 #0000);
@@ -1415,14 +1493,27 @@
 }
 
 .focus\:ring-blue-400:focus {
   --tw-ring-opacity: 1;
   --tw-ring-color: rgb(96 165 250 / var(--tw-ring-opacity));
 }
 
+.focus\:ring-indigo-500:focus {
+  --tw-ring-opacity: 1;
+  --tw-ring-color: rgb(99 102 241 / var(--tw-ring-opacity));
+}
+
+.focus\:ring-offset-2:focus {
+  --tw-ring-offset-width: 2px;
+}
+
+.focus\:ring-offset-gray-100:focus {
+  --tw-ring-offset-color: #f3f4f6;
+}
+
 .focus-visible\:outline:focus-visible {
   outline-style: solid;
 }
 
 .focus-visible\:outline-2:focus-visible {
   outline-width: 2px;
 }
@@ -1435,33 +1526,16 @@
   outline-color: #60a5fa;
 }
 
 .focus-visible\:outline-red-600:focus-visible {
   outline-color: #dc2626;
 }
 
-:is(.dark .dark\:border-neutral-300\/10) {
-  border-color: rgb(212 212 212 / 0.1);
-}
-
-:is(.dark .dark\:border-neutral-300) {
-  --tw-border-opacity: 1;
-  border-color: rgb(212 212 212 / var(--tw-border-opacity));
-}
-
-:is(.dark .dark\:border-neutral-300\/60) {
-  border-color: rgb(212 212 212 / 0.6);
-}
-
-:is(.dark .dark\:border-neutral-300\/40) {
-  border-color: rgb(212 212 212 / 0.4);
-}
-
-:is(.dark .dark\:border-neutral-300\/20) {
-  border-color: rgb(212 212 212 / 0.2);
+.group:hover .group-hover\:block {
+  display: block;
 }
 
 :is(.dark .dark\:border-neutral-300\/30) {
   border-color: rgb(212 212 212 / 0.3);
 }
 
 :is(.dark .dark\:bg-blue-900) {
@@ -1475,14 +1549,44 @@
 }
 
 :is(.dark .dark\:bg-neutral-950) {
   --tw-bg-opacity: 1;
   background-color: rgb(10 10 10 / var(--tw-bg-opacity));
 }
 
+:is(.dark .dark\:bg-neutral-400) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(163 163 163 / var(--tw-bg-opacity));
+}
+
+:is(.dark .dark\:bg-neutral-600) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(82 82 82 / var(--tw-bg-opacity));
+}
+
+:is(.dark .dark\:bg-neutral-50) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(250 250 250 / var(--tw-bg-opacity));
+}
+
+:is(.dark .dark\:bg-neutral-500) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(115 115 115 / var(--tw-bg-opacity));
+}
+
+:is(.dark .dark\:bg-neutral-700) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(64 64 64 / var(--tw-bg-opacity));
+}
+
+:is(.dark .dark\:bg-neutral-800) {
+  --tw-bg-opacity: 1;
+  background-color: rgb(38 38 38 / var(--tw-bg-opacity));
+}
+
 :is(.dark .dark\:text-blue-200) {
   --tw-text-opacity: 1;
   color: rgb(191 219 254 / var(--tw-text-opacity));
 }
 
 :is(.dark .dark\:text-neutral-200) {
   --tw-text-opacity: 1;
@@ -1494,29 +1598,19 @@
 }
 
 :is(.dark .dark\:text-neutral-300) {
   --tw-text-opacity: 1;
   color: rgb(212 212 212 / var(--tw-text-opacity));
 }
 
-:is(.dark .dark\:text-neutral-900) {
-  --tw-text-opacity: 1;
-  color: rgb(23 23 23 / var(--tw-text-opacity));
-}
-
 :is(.dark .dark\:text-white) {
   --tw-text-opacity: 1;
   color: rgb(255 255 255 / var(--tw-text-opacity));
 }
 
-:is(.dark .dark\:text-neutral-600) {
-  --tw-text-opacity: 1;
-  color: rgb(82 82 82 / var(--tw-text-opacity));
-}
-
 :is(.dark .dark\:placeholder-neutral-500)::-moz-placeholder {
   --tw-placeholder-opacity: 1;
   color: rgb(115 115 115 / var(--tw-placeholder-opacity));
 }
 
 :is(.dark .dark\:placeholder-neutral-500)::placeholder {
   --tw-placeholder-opacity: 1;
```

### Comparing `niapi-0.3.0/niapi/domain/web/templates/base/base.html` & `niapi-0.4.0/niapi/domain/web/templates/base/base.html`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/domain/web/templates/base/footer.html` & `niapi-0.4.0/niapi/domain/web/templates/base/footer.html`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/domain/web/templates/base/nav.html` & `niapi-0.4.0/niapi/domain/web/templates/base/nav.html`

 * *Files 21% similar despite different names*

```diff
@@ -134,24 +134,84 @@
           stroke-linejoin="round"
           stroke-width="2"
         >
           <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
         </svg>
       </button>
 
-      <a
-        href="/api"
-        class="text-sm font-semibold leading-6 text-blue-400 hover:text-blue-900 dark:text-blue-200 dark:hover:text-blue-500"
-        >API <span aria-hidden="true">&rarr;</span></a
-      >
+      <div class="relative inline-block text-left">
+        <div>
+          <button
+            type="button"
+            class="flex items-center rounded-full bg-white dark:bg-neutral-900 text-blue-400 hover:text-blue-900 dark:text-blue-200 dark:hover:text-blue-500 focus:outline-none focus:ring-2 focus:ring-blue-400 focus:ring-offset-2 focus:ring-offset-gray-100"
+            id="menu-button"
+            aria-expanded="false"
+            aria-haspopup="true"
+          >
+            <span class="sr-only">Open API Menu</span>
+            &nbsp;API&nbsp;
+            <!-- https://feathericons.dev/?search=more-vertical&iconset=feather -->
+            <svg
+              xmlns="http://www.w3.org/2000/svg"
+              viewBox="0 0 24 24"
+              width="24"
+              height="24"
+              class="main-grid-item-icon pointer-events-none"
+              fill="none"
+              stroke="currentColor"
+              stroke-linecap="round"
+              stroke-linejoin="round"
+              stroke-width="2"
+            >
+              <circle cx="12" cy="12" r="1"></circle>
+              <circle cx="12" cy="5" r="1"></circle>
+              <circle cx="12" cy="19" r="1"></circle>
+            </svg>
+          </button>
+        </div>
+
+        <div
+          class="absolute right-0 z-10 mt-2 w-56 origin-top-right rounded-md bg-white dark:bg-neutral-800 shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none hidden"
+          id="menu"
+          role="menu"
+          aria-orientation="vertical"
+          aria-labelledby="menu-button"
+          tabindex="-1"
+        >
+          <div class="py-1" role="none">
+            <a
+              href="/api/elements"
+              class="text-blue-400 hover:text-blue-900 dark:text-blue-200 dark:hover:text-blue-500 block px-4 py-2 text-sm"
+              role="menuitem"
+              tabindex="-1"
+              id="menu-item-0"
+              >Elements</a
+            >
+            <a
+              href="/api/swagger"
+              class="text-blue-400 hover:text-blue-900 dark:text-blue-200 dark:hover:text-blue-500 block px-4 py-2 text-sm"
+              role="menuitem"
+              tabindex="-1"
+              id="menu-item-1"
+              >Swagger</a
+            >
+            <a
+              href="/api/redoc"
+              class="text-blue-400 hover:text-blue-900 dark:text-blue-200 dark:hover:text-blue-500 block px-4 py-2 text-sm"
+              role="menuitem"
+              tabindex="-1"
+              id="menu-item-2"
+              >ReDoc</a
+            >
+          </div>
+        </div>
+      </div>
     </div>
   </nav>
-  <!-- Mobile menu, show/hide based on menu open state. -->
   <div class="lg:hidden" role="dialog" aria-modal="true">
-    <!-- Background backdrop, show/hide based on slide-over state. -->
     <div class="fixed inset-0 z-10"></div>
     <div
       class="fixed inset-y-0 left-0 z-10 w-full overflow-y-auto bg-white px-6 py-6"
     >
       <div class="flex items-center justify-between">
         <div class="flex flex-1">
           <button type="button" class="-m-2.5 rounded-md p-2.5 text-blue-700">
@@ -242,9 +302,26 @@
     if (dropdownTrigger) {
       dropdownTrigger.addEventListener("mouseenter", showDropdown);
       dropdownTrigger.addEventListener("mouseleave", hideDropdown);
       dropdownContent.addEventListener("mouseenter", showDropdown);
       dropdownContent.addEventListener("mouseleave", hideDropdown);
     }
   });
+
+  let button = document.getElementById("menu-button");
+  let menu = document.getElementById("menu");
+
+  button.addEventListener("click", function (event) {
+    let isShown = menu.classList.toggle("hidden");
+    button.setAttribute("aria-expanded", !isShown);
+  });
+
+  window.onclick = function (event) {
+    if (!event.target.matches("#menu-button")) {
+      if (!menu.classList.contains("hidden")) {
+        menu.classList.add("hidden");
+        button.setAttribute("aria-expanded", false);
+      }
+    }
+  };
 </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {% set active_page = active_page|default('home') -%}
 ____Home _____About
  Main Menu
 NIAPI
- Light Mode              Dark Mode     API_→
-
+ Light Mode              Dark Mode
+ Open API Menu  API 
+Elements Swagger ReDoc
  Close menu
 Your_Company
 API_→
 Home About
  {% block extrajs %}
  {% endblock %}
```

### Comparing `niapi-0.3.0/niapi/domain/web/templates/index.html` & `niapi-0.4.0/niapi/domain/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/exceptions.py` & `niapi-0.4.0/niapi/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/log/__init__.py` & `niapi-0.4.0/niapi/lib/log/__init__.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/log/controller.py` & `niapi-0.4.0/niapi/lib/log/controller.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/log/utils.py` & `niapi-0.4.0/niapi/lib/log/utils.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/openapi.py` & `niapi-0.4.0/niapi/lib/openapi.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/schema.py` & `niapi-0.4.0/niapi/lib/schema.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/serialization.py` & `niapi-0.4.0/niapi/lib/serialization.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/settings.py` & `niapi-0.4.0/niapi/lib/settings.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/lib/static_files.py` & `niapi-0.4.0/niapi/lib/static_files.py`

 * *Files identical despite different names*

### Comparing `niapi-0.3.0/niapi/utils.py` & `niapi-0.4.0/niapi/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,42 +23,37 @@
 ]
 
 if TYPE_CHECKING:
     from types import ModuleType
 
 
 def check_email(email: str) -> str:
-    """Validate an email.
+    """Check if the email is valid.
 
     Args:
-        email: The email to validate
+        email: The email to check.
 
     Returns:
-        str: The validated email
+        The email if it is valid.
     """
     if "@" not in email:
         raise ValueError("Invalid email!")
     return email.lower()
 
 
 def slugify(value: str, allow_unicode: bool = False, separator: str | None = None) -> str:
-    """slugify.
-
-    Convert to ASCII if 'allow_unicode' is False. Convert spaces or repeated
-    dashes to single dashes. Remove characters that aren't alphanumerics,
-    underscores, or hyphens. Convert to lowercase. Also strip leading and
-    trailing whitespace, dashes, and underscores.
+    """Convert a string to a slug.
 
     Args:
-        value: the string to slugify
-        allow_unicode: allow unicode characters in slug. Defaults to False.
-        separator: by default a `-` is used to delimit word boundaries.  Set this to configure to something different.
+        value: The string to slugify.
+        allow_unicode: Whether to allow unicode characters.
+        separator: The separator to use.
 
     Returns:
-        str: a slugified string of the value parameter
+        The slugified string.
     """
     if allow_unicode:
         value = unicodedata.normalize("NFKC", value)
     else:
         value = unicodedata.normalize("NFKD", value).encode("ascii", "ignore").decode("ascii")
     value = re.sub(r"[^\w\s-]", "", value.lower())
     if separator is not None:
@@ -66,110 +61,103 @@
     return re.sub(r"[-\s]+", "-", value).strip("-_")
 
 
 def camel_case(string: str) -> str:
     """Convert a string to camel case.
 
     Args:
-        string: The string to convert
+        string: The string to convert.
 
     Returns:
-        str: The string converted to camel case
+        The camel cased string.
     """
     return "".join(word if index == 0 else word.capitalize() for index, word in enumerate(string.split("_")))
 
 
 def case_insensitive_string_compare(a: str, b: str, /) -> bool:
-    """Compare `a` and `b`, stripping whitespace and ignoring case.
+    """Compare two strings case insensitively.
 
     Args:
-        a: The first string to compare.
-        b: The second string to compare.
+        a: The first string.
+        b: The second string.
 
     Returns:
-        bool: True if the strings are equal, False otherwise.
+        Whether the strings are equal.
     """
     return a.strip().lower() == b.strip().lower()
 
 
 def dataclass_as_dict_shallow(dataclass: Any, *, exclude_none: bool = False) -> dict[str, Any]:
-    """Convert a dataclass to dict, without deepcopy.
+    """Convert a dataclass to a dict.
 
     Args:
         dataclass: The dataclass to convert.
-        exclude_none: Exclude None values from the returned dict.
+        exclude_none: Whether to exclude None values.
 
     Returns:
-        dict[str, Any]: The dataclass as a dict.
+        The dataclass as a dict.
     """
     ret: dict[str, Any] = {}
     for field in dataclasses.fields(dataclass):
         value = getattr(dataclass, field.name)
         if exclude_none and value is None:
             continue
         ret[field.name] = value
     return ret
 
 
 @lru_cache
 def module_to_os_path(dotted_path: str = "app") -> Path:
-    """Find Module to OS Path.
-
-    Return path to the base directory of the project or the module
-    specified by `dotted_path`.
-
-    Ensures that pkgutil returns a valid source file loader.
+    """Get the path to a module.
 
     Args:
-        dotted_path: The dotted path to the module to find the path for.
-
-    Raises:
-        TypeError: Couldn't find the path for the module.
+        dotted_path: The dotted path to the module.
 
     Returns:
-        Path: The path to the module.
+        The path to the module.
     """
     src = pkgutil.get_loader(dotted_path)
     if not isinstance(src, SourceFileLoader):
         raise TypeError("Couldn't find the path for %s", dotted_path)
     return Path(str(src.path).removesuffix("/__init__.py"))
 
 
 def import_string(dotted_path: str) -> Any:
-    """Dotted Path Import.
-
-    Import a dotted module path and return the attribute/class designated by the
-    last name in the path. Raise ImportError if the import failed.
+    """Import a class/function from a dotted path.
 
     Args:
-        dotted_path: The path of the module to import.
-
-    Raises:
-        ImportError: Could not import the module.
+        dotted_path: The dotted path to the class/function.
 
     Returns:
-        object: The imported object.
+        The imported class/function.
     """
 
     def _is_loaded(module: ModuleType | None) -> bool:
+        """Check if a module is loaded.
+
+        Args:
+            module: The module to check.
+
+        Returns:
+            Whether the module is loaded.
+        """
         spec = getattr(module, "__spec__", None)
         initializing = getattr(spec, "_initializing", False)
         return bool(module and spec and not initializing)
 
     def _cached_import(module_path: str, class_name: str) -> Any:
-        """Import and cache a class from a module.
+        """Import a class/function from a dotted path.
 
         Args:
-            module_path: dotted path to module.
-            class_name: Class or function name.
+            module_path: The dotted path to the module.
+            class_name: The name of the class/function.
 
         Returns:
-            object: The imported class or function
+            The imported class/function.
         """
-        # Check whether module is loaded and fully initialized.
         module = sys.modules.get(module_path)
         if not _is_loaded(module):
             module = import_module(module_path)
         return getattr(module, class_name)
 
     try:
         module_path, class_name = dotted_path.rsplit(".", 1)
```

### Comparing `niapi-0.3.0/pyproject.toml` & `niapi-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "niapi"
-version = "0.3.0"
+version = "0.4.0"
 description = "Network Data API"
 authors = ["Jacob Coffee <jacob@z7x.org>"]
 maintainers = [
     "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
 readme = "docs/PYPI_README.md"
@@ -63,14 +63,15 @@
 [tool.poetry.plugins."litestar.commands"]
 run-all = "niapi.cli:run_all_app"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<4.0"
 litestar = {version = "2.0b2", extras = ["standard", "structlog", "prometheus"]}
 python-dotenv = "^1.0.0"
+poetry = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 coverage = "^7.2.7"
 pytest-benchmark = "^4.0.0"
 pytest-cov = "^4.1.0"
 pytest-docker = "^1.0.1"
@@ -103,15 +104,15 @@
 sphinxcontrib-confluencebuilder = "^2.1.1"
 sphinx-toolbox = "^3.4.0"
 autodoc-pydantic = "^1.8.0"
 blacken-docs = "^1.14.0"
 sphinxcontrib-mermaid = "^0.9.2"
 
 [build-system]
-requires = ["poetry-core"]
+requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 
 [tool.codespell]
@@ -166,15 +167,15 @@
     'except ImportError as e:',
     'except ImportError:',
     '\.\.\.',
     'raise NotImplementedError',
 ]
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+#asyncio_mode = "auto"
 
 [tool.slotscheck]
 strict-imports = false
 
 [tool.ruff]
 select = [
     "A",   # flake8-builtins
```

### Comparing `niapi-0.3.0/PKG-INFO` & `niapi-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niapi
-Version: 0.3.0
+Version: 0.4.0
 Summary: Network Data API
 Home-page: https://github.com/JacobCoffee/niapi
 License: MIT
 Keywords: niapi,network,api,tool,rest,http,asgi,pydantic,litestar,starlite,websocket
 Author: Jacob Coffee
 Author-email: jacob@z7x.org
 Maintainer: Jacob Coffee
@@ -27,44 +27,44 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Dist: litestar[prometheus,standard,structlog] (==2.0b2)
+Requires-Dist: poetry (>=1.5.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Project-URL: Changelog, https://github.com/JacobCoffee/niapi/releases/
 Project-URL: Documentation, https://jacobcoffee.github.io/niapi/index.html
 Project-URL: Issue Tracker, https://github.com/JacobCoffee/niapi/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Repository, https://github.com/JacobCoffee/niapi
 Project-URL: Reddit, https://www.reddit.com/u/monorepo
 Project-URL: Twitter, https://twitter.com/_scriptr
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="https://github.com/JacobCoffee/niapi/blob/a82a86a1b8ca90f3c66a080291cfd074efcbfd1a/docs/images/PNG/Transparent/logo.png" alt="NIAPI Logo - Light" width="100%" height="auto" />
+  <img src="https://github.com/JacobCoffee/niapi/blob/a82a86a1b8ca90f3c66a080291cfd074efcbfd1a/docs/images/PNG/Transparent/logo.png?raw=True" alt="NIAPI Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
-| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-|-----------|:----|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CI/CD     |     | [![Latest Release](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml) [![ci](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml) [![CodeQL](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql)                                                                                                                                                                                                                                                                                                                                                                        |
-| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/niapi)](https://badge.fury.io/py/niapi) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/niapi)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| Quality   |     | [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=coverage)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=jacobcoffee_niapi&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=jacobcoffee_niapi) [![Known Vulnerabilities](https://snyk.io/test/github/JacobCoffee/niapi/badge.svg)](https://snyk.io/test/github/JacobCoffee/niapi) |
-| Community |     | [![Twitter](https://img.shields.io/twitter/follow/_scriptr?style=social&logo=twitter)](https://twitter.com/_scriptr)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| Meta      |     | [![Litestar Framework](https://img.shields.io/badge/Litestar%20Framework-%E2%AD%90%20Litestar-202235.svg)](https://github.com/JacobCoffee/niapi) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/JacobCoffee?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/JacobCoffee)                                                                                                                                                                                                                                                            |
-
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-113-202235.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
+| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+|-----------|:----|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CI/CD     |     | [![Latest Release](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/publish.yaml) [![ci](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/docs.yaml) [![CodeQL](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/JacobCoffee/niapi/actions/workflows/github-code-scanning/codeql)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/niapi)](https://badge.fury.io/py/niapi) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/niapi)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| Quality   |     | [![codecov](https://codecov.io/gh/JacobCoffee/niapi/branch/main/graph/badge.svg?token=SFT67X4MEQ)](https://codecov.io/gh/JacobCoffee/niapi) [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=coverage)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=JacobCoffee_niapi&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi) [![Known Vulnerabilities](https://snyk.io/test/github/JacobCoffee/niapi/badge.svg)](https://snyk.io/test/github/JacobCoffee/niapi) |
+| Community |     | [![Twitter](https://img.shields.io/twitter/follow/_scriptr?style=social&logo=twitter)](https://twitter.com/_scriptr)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| Meta      |     | [![Litestar Framework](https://img.shields.io/badge/Litestar%20Framework-%E2%AD%90%20Litestar-202235.svg)](https://github.com/JacobCoffee/niapi) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-85c7f2.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-85c7f2.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/JacobCoffee?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/JacobCoffee)                                                                                                                                                                                                                                                                                                                                                                                                        |
+
+[![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-white.svg)](https://sonarcloud.io/summary/new_code?id=JacobCoffee_niapi)
+
 <!-- prettier-ignore-end -->
 
 </div>
 
 # `niapi` - Network Information API
 
 [//]: # "TODO"
@@ -110,15 +110,15 @@
 
 ```python
 # todo
 ```
 
 ## Contributing
 
-See [CONTRIBUTING.rst](../CONTRIBUTING.rst) for more information.
+See [CONTRIBUTING.rst](CONTRIBUTING.rst) for more information.
 
 Start the app:
 
 ```console
 app run-all
 ```
 
@@ -142,10 +142,10 @@
 - Using https://feathericons.dev/
 - Using TailwindCSS
 
 ## Screenshots
 
 [//]: # "TODO"
 
-![home.png](images/index.png)
-![home-dark.png](images/index-dark.png)
+![](https://github.com/JacobCoffee/niapi/blob/79eada17e1477feae3f3e15106331e4b81625157/docs/images/index-dark.png?raw=true)
+![](https://github.com/JacobCoffee/niapi/blob/79eada17e1477feae3f3e15106331e4b81625157/docs/images/index.png?raw=true)
```

