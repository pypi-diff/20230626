# Comparing `tmp/async_mvg_api-0.1.4.tar.gz` & `tmp/async_mvg_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_mvg_api-0.1.4.tar", max compression
+gzip compressed data, was "async_mvg_api-0.1.5.tar", max compression
```

## Comparing `async_mvg_api-0.1.4.tar` & `async_mvg_api-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.1.4/mvg_api/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.1.4/mvg_api/api/__init__.py
--rw-r--r--   0        0        0    11269 2022-12-10 11:31:43.416867 async_mvg_api-0.1.4/mvg_api/api/api.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.1.4/mvg_api/models/__init__.py
--rw-r--r--   0        0        0     4415 2022-12-02 17:15:39.219527 async_mvg_api-0.1.4/mvg_api/models/route.py
--rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.1.4/mvg_api/models/ticker.py
--rw-r--r--   0        0        0     9098 2022-12-09 23:13:34.029374 async_mvg_api-0.1.4/mvg_api/mvg.py
--rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.1.4/mvg_api/tests/__init__.py
--rw-r--r--   0        0        0     3097 2022-12-10 11:31:55.574048 async_mvg_api-0.1.4/mvg_api/tests/api_tests.py
--rw-r--r--   0        0        0    21656 2023-04-20 10:15:50.771249 async_mvg_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1404 2022-12-09 23:56:14.842549 async_mvg_api-0.1.4/README.md
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 async_mvg_api-0.1.4/setup.py
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 async_mvg_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.1.5/mvg_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.1.5/mvg_api/api/__init__.py
+-rw-r--r--   0        0        0     7128 2023-06-25 21:31:14.999622 async_mvg_api-0.1.5/mvg_api/api/api.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.1.5/mvg_api/models/__init__.py
+-rw-r--r--   0        0        0     5774 2023-06-25 21:52:42.316969 async_mvg_api-0.1.5/mvg_api/models/route.py
+-rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.1.5/mvg_api/models/ticker.py
+-rw-r--r--   0        0        0     6922 2023-06-25 21:56:29.413298 async_mvg_api-0.1.5/mvg_api/mvg.py
+-rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.1.5/mvg_api/tests/__init__.py
+-rw-r--r--   0        0        0     2591 2023-06-25 21:30:53.746385 async_mvg_api-0.1.5/mvg_api/tests/api_tests.py
+-rw-r--r--   0        0        0    21521 2023-06-25 22:01:03.402019 async_mvg_api-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1404 2022-12-09 23:56:14.842549 async_mvg_api-0.1.5/README.md
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 async_mvg_api-0.1.5/setup.py
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 async_mvg_api-0.1.5/PKG-INFO
```

### Comparing `async_mvg_api-0.1.4/LICENSE` & `async_mvg_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.4/mvg_api/models/ticker.py` & `async_mvg_api-0.1.5/mvg_api/models/ticker.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.4/mvg_api/tests/api_tests.py` & `async_mvg_api-0.1.5/mvg_api/tests/api_tests.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,24 +31,15 @@
     api = Api()
     response = api.get_slim()
     assert isinstance(response, SlimList)
 
 
 def test_get_route():
     api = Api()
-    response = api.get_route(
-        "de:09162:6",
-        "de:09162:50",
-        sap_tickets=True,
-        _time=datetime.datetime.now(),
-        transport_type_call_taxi=True,
-        max_walk_time_to_dest=5,
-        max_walk_time_to_start=5,
-        change_limit=3,
-    )
+    response = api.get_route("de:09162:6", "de:09162:50")
     assert isinstance(response, Connections)
 
 
 def test_get_location():
     api = Api()
     response = api.get_location("Marienplatz")
     assert isinstance(response, LocationList)
@@ -82,26 +73,15 @@
     api = AsyncApi()
     response = asyncio.run(api.get_slim())
     assert isinstance(response, SlimList)
 
 
 def test_get_route_async():
     api = AsyncApi()
-    response = asyncio.run(
-        api.get_route(
-            "de:09162:6",
-            "de:09162:50",
-            sap_tickets=True,
-            _time=datetime.datetime.now(),
-            transport_type_call_taxi=True,
-            max_walk_time_to_dest=5,
-            max_walk_time_to_start=5,
-            change_limit=3,
-        )
-    )
+    response = asyncio.run(api.get_route("de:09162:6", "de:09162:50"))
     assert isinstance(response, Connections)
 
 
 def test_get_location_async():
     api = AsyncApi()
     response = asyncio.run(api.get_location("Marienplatz"))
     assert isinstance(response, LocationList)
```

### Comparing `async_mvg_api-0.1.4/pyproject.toml` & `async_mvg_api-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_mvg_api"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Lukas Mahr <lukas@yousuckatprogramming.de>"]
 readme = "README.md"
 packages = [{include = "mvg_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -280,17 +280,14 @@
 
 # Maximum number of statements in function / method body.
 max-statements = 50
 
 # Minimum number of public methods for a class (see R0903).
 min-public-methods = 1
 
-[tool.pylint.exceptions]
-# Exceptions that will emit a warning when caught.
-overgeneral-exceptions = ["BaseException", "Exception"]
 
 [tool.pylint.format]
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 # expected-line-ending-format =
 
 # Regexp for a line that is allowed to be longer than the limit.
 ignore-long-lines = "^\\s*(# )?<?https?://\\S+>?$"
```

### Comparing `async_mvg_api-0.1.4/README.md` & `async_mvg_api-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.4/setup.py` & `async_mvg_api-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'levenshtein>=0.21.0,<0.22.0',
  'pydantic>=1.10.7,<2.0.0',
  'pylint>=2.15.7,<3.0.0',
  'pytest>=7.2.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'async-mvg-api',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': '# Unofficial MVG api\n\nAn async and sync wrapper for the MVG endpoints, with data validation over pydantic\n\n# Usage policy of the MVG api\n## ACHTUNG: \nUnsere Systeme dienen der direkten Kundeninteraktion. Die Verarbeitung unserer Inhalte oder Daten durch Dritte erfordert unsere ausdrückliche Zustimmung. Für private, nicht-kommerzielle Zwecke, wird eine gemäßigte Nutzung ohne unsere ausdrückliche Zustimmung geduldet. Jegliche Form von Data-Mining stellt keine gemäßigte Nutzung dar. Wir behalten uns vor, die Duldung grundsätzlich oder in Einzelfällen zu widerrufen. Fragen richten Sie bitte gerne an: redaktion@mvg.de.\n\nIn other words: Private, noncomercial, moderate use of the API is tolerated. They don\'t consider data mining as moderate use.\n\n(Disclaimer: I am not a lawyer, this isn\'t legal advice)\n\n## Installation\npip installation or clone the repository and install the [poetry](https://python-poetry.org/) dependencies\n\n```bash\npip install async-mvg-api\n```\n\nor \n\n```bash\ngit clone https://github.com/Plutokekz/MVG-Api.git\ncd MVG-Api\npoetry install\n```\n## Usage\n\n```python\nfrom mvg_api.mvg import MVG\nmvg = MVG()\nmvg.get_location("Hauptbahnhof")\n```\n\n## Tests\n\n```bash\npoetry run pytest mvg_api/tests/api_tests.py\n```\n\n# Credit\nFor Endpoint Information and Code snippets\n* https://github.com/leftshift/python_mvg_api\n* https://www.mvg.de/\n',
     'author': 'Lukas Mahr',
     'author_email': 'lukas@yousuckatprogramming.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `async_mvg_api-0.1.4/PKG-INFO` & `async_mvg_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-mvg-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Lukas Mahr
 Author-email: lukas@yousuckatprogramming.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
```

