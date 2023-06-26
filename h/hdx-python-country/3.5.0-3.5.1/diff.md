# Comparing `tmp/hdx_python_country-3.5.0.tar.gz` & `tmp/hdx_python_country-3.5.1.tar.gz`

## Comparing `hdx_python_country-3.5.0.tar` & `hdx_python_country-3.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/main.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/_version.py
--rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/adminlevel.py
--rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/country.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/currency.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/names.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/src/hdx/location/phonetics.py
--rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/adminlevel.yml
--rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/secondary_historic_rates.csv
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/fixtures/secondary_rates.json
--rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/Countries_UZB_Deleted.csv
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/__init__.py
--rwxr-xr-x   0        0        0     4456 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_adminlevel.py
--rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_country.py
--rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/tests/hdx/location/test_currency.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/.gitignore
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/LICENSE
--rwxr-xr-x   0        0        0     2306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hdx_python_country-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/main.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/_version.py
+-rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/adminlevel.py
+-rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/country.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/currency.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/names.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/phonetics.py
+-rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/adminlevel.yaml
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/secondary_historic_rates.csv
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/secondary_rates.json
+-rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/Countries_UZB_Deleted.csv
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/__init__.py
+-rwxr-xr-x   0        0        0     4457 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_adminlevel.py
+-rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_country.py
+-rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_currency.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.gitignore
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/LICENSE
+-rwxr-xr-x   0        0        0     2306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/PKG-INFO
```

### Comparing `hdx_python_country-3.5.0/CONTRIBUTING.md` & `hdx_python_country-3.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/requirements.txt` & `hdx_python_country-3.5.1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # via virtualenv
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
 frictionless==5.13.1
     # via hdx-python-utilities
-hdx-python-utilities==3.6.0
+hdx-python-utilities==3.6.1
     # via hdx-python-country (pyproject.toml)
 humanize==4.6.0
     # via frictionless
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `hdx_python_country-3.5.0/.config/pre-commit-config.yaml` & `hdx_python_country-3.5.1/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/.github/workflows/publish.yaml` & `hdx_python_country-3.5.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/.github/workflows/run-python-tests.yaml` & `hdx_python_country-3.5.1/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/documentation/main.md` & `hdx_python_country-3.5.1/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/documentation/pydoc-markdown.yaml` & `hdx_python_country-3.5.1/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv` & `hdx_python_country-3.5.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/adminlevel.py` & `hdx_python_country-3.5.1/src/hdx/location/adminlevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/country.py` & `hdx_python_country-3.5.1/src/hdx/location/country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/currency.py` & `hdx_python_country-3.5.1/src/hdx/location/currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/names.py` & `hdx_python_country-3.5.1/src/hdx/location/names.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/src/hdx/location/phonetics.py` & `hdx_python_country-3.5.1/src/hdx/location/phonetics.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/fixtures/adminlevel.yml` & `hdx_python_country-3.5.1/tests/fixtures/adminlevel.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/fixtures/secondary_historic_rates.csv` & `hdx_python_country-3.5.1/tests/fixtures/secondary_historic_rates.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/fixtures/secondary_rates.json` & `hdx_python_country-3.5.1/tests/fixtures/secondary_rates.json`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/hdx/location/Countries_UZB_Deleted.csv` & `hdx_python_country-3.5.1/tests/hdx/location/Countries_UZB_Deleted.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/hdx/location/test_adminlevel.py` & `hdx_python_country-3.5.1/tests/hdx/location/test_adminlevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from hdx.location.adminlevel import AdminLevel
 from hdx.utilities.loader import load_yaml
 
 
 class TestAdminLevel:
     @pytest.fixture(scope="function")
     def config(self):
-        return load_yaml(join("tests", "fixtures", "adminlevel.yml"))
+        return load_yaml(join("tests", "fixtures", "adminlevel.yaml"))
 
     def test_adminlevel(self, config):
         adminone = AdminLevel(config)
         assert adminone.get_admin_level("YEM") == 1
         assert len(adminone.get_pcode_list()) == 433
         assert adminone.get_pcode_length("YEM") == 4
         assert adminone.get_pcode("YEM", "YE30", logname="test") == (
```

### Comparing `hdx_python_country-3.5.0/tests/hdx/location/test_country.py` & `hdx_python_country-3.5.1/tests/hdx/location/test_country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/tests/hdx/location/test_currency.py` & `hdx_python_country-3.5.1/tests/hdx/location/test_currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/.gitignore` & `hdx_python_country-3.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/LICENSE` & `hdx_python_country-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/README.md` & `hdx_python_country-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.0/pyproject.toml` & `hdx_python_country-3.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-utilities>=3.5.9",
+    "hdx-python-utilities>=3.6.1",
     "libhxl",
     "pyphonetics",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `hdx_python_country-3.5.0/PKG-INFO` & `hdx_python_country-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-country
-Version: 3.5.0
+Version: 3.5.1
 Summary: HDX Python country code and exchange rate (fx) utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-country
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,country,country code,currencies,currency,exchange rate,foreign exchange,fx,iso 3166,iso2,iso3,location,region
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: hdx-python-utilities>=3.5.9
+Requires-Dist: hdx-python-utilities>=3.6.1
 Requires-Dist: libhxl
 Requires-Dist: pyphonetics
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
```

