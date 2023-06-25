# Comparing `tmp/hdx_python_country-3.4.9.tar.gz` & `tmp/hdx_python_country-3.5.0.tar.gz`

## Comparing `hdx_python_country-3.4.9.tar` & `hdx_python_country-3.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.github/workflows/run-python-tests.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/main.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/pydoc-markdown.yml
--rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/_version.py
--rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/adminlevel.py
--rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/country.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/currency.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/names.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/phonetics.py
--rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/adminlevel.yml
--rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/secondary_historic_rates.csv
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/secondary_rates.json
--rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/Countries_UZB_Deleted.csv
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/__init__.py
--rwxr-xr-x   0        0        0     4456 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_adminlevel.py
--rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_country.py
--rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_currency.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.gitignore
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/LICENSE
--rwxr-xr-x   0        0        0     2304 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/pyproject.toml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/main.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/_version.py
+-rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/adminlevel.py
+-rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/country.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/currency.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/names.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/phonetics.py
+-rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/adminlevel.yml
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/secondary_historic_rates.csv
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/secondary_rates.json
+-rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/Countries_UZB_Deleted.csv
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/__init__.py
+-rwxr-xr-x   0        0        0     4456 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_adminlevel.py
+-rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_country.py
+-rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_currency.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.gitignore
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/LICENSE
+-rwxr-xr-x   0        0        0     2306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/PKG-INFO
```

### Comparing `hdx_python_country-3.4.9/CONTRIBUTING.md` & `hdx_python_country-3.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/requirements.txt` & `hdx_python_country-3.5.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # via virtualenv
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
 frictionless==5.13.1
     # via hdx-python-utilities
-hdx-python-utilities==3.5.9
+hdx-python-utilities==3.6.0
     # via hdx-python-country (pyproject.toml)
 humanize==4.6.0
     # via frictionless
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
@@ -75,15 +75,15 @@
     # via pre-commit
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.7.0
+platformdirs==3.8.0
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
@@ -93,15 +93,15 @@
     # via frictionless
 pygments==2.15.1
     # via rich
 pyphonetics==0.5.3
     # via hdx-python-country (pyproject.toml)
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.2
+pytest==7.4.0
     # via
     #   hdx-python-country (pyproject.toml)
     #   libhxl
     #   pytest-cov
 pytest-cov==4.1.0
     # via hdx-python-country (pyproject.toml)
 python-dateutil==2.8.2
```

### Comparing `hdx_python_country-3.4.9/.config/pre-commit-config.yaml` & `hdx_python_country-3.5.0/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/.github/workflows/publish.yml` & `hdx_python_country-3.5.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/.github/workflows/run-python-tests.yml` & `hdx_python_country-3.5.0/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/documentation/main.md` & `hdx_python_country-3.5.0/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/documentation/pydoc-markdown.yml` & `hdx_python_country-3.5.0/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv` & `hdx_python_country-3.5.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/adminlevel.py` & `hdx_python_country-3.5.0/src/hdx/location/adminlevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/country.py` & `hdx_python_country-3.5.0/src/hdx/location/country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/currency.py` & `hdx_python_country-3.5.0/src/hdx/location/currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/names.py` & `hdx_python_country-3.5.0/src/hdx/location/names.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/src/hdx/location/phonetics.py` & `hdx_python_country-3.5.0/src/hdx/location/phonetics.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/fixtures/adminlevel.yml` & `hdx_python_country-3.5.0/tests/fixtures/adminlevel.yml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/fixtures/secondary_historic_rates.csv` & `hdx_python_country-3.5.0/tests/fixtures/secondary_historic_rates.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/fixtures/secondary_rates.json` & `hdx_python_country-3.5.0/tests/fixtures/secondary_rates.json`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/hdx/location/Countries_UZB_Deleted.csv` & `hdx_python_country-3.5.0/tests/hdx/location/Countries_UZB_Deleted.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/hdx/location/test_adminlevel.py` & `hdx_python_country-3.5.0/tests/hdx/location/test_adminlevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/hdx/location/test_country.py` & `hdx_python_country-3.5.0/tests/hdx/location/test_country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/tests/hdx/location/test_currency.py` & `hdx_python_country-3.5.0/tests/hdx/location/test_currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/.gitignore` & `hdx_python_country-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/LICENSE` & `hdx_python_country-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/README.md` & `hdx_python_country-3.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-country/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-country?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-country.svg)](https://pypistats.org/packages/hdx-python-country)
 
 The HDX Python Country Library provides utilities to map between country and region 
 codes and names and to match administrative level names from different sources.
```

### Comparing `hdx_python_country-3.4.9/pyproject.toml` & `hdx_python_country-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.4.9/PKG-INFO` & `hdx_python_country-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-country
-Version: 3.4.9
+Version: 3.5.0
 Summary: HDX Python country code and exchange rate (fx) utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-country
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,country,country code,currencies,currency,exchange rate,foreign exchange,fx,iso 3166,iso2,iso3,location,region
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
-[![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml)
+[![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-country/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-country?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-country.svg)](https://pypistats.org/packages/hdx-python-country)
 
 The HDX Python Country Library provides utilities to map between country and region 
 codes and names and to match administrative level names from different sources.
```

