# Comparing `tmp/runtype-0.3.2.tar.gz` & `tmp/runtype-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtype-0.3.2.tar", max compression
+gzip compressed data, was "runtype-0.3.3.tar", max compression
```

## Comparing `runtype-0.3.2.tar` & `runtype-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.2/LICENSE
--rw-r--r--   0        0        0     1196 2023-04-28 16:04:39.515338 runtype-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4098 2022-10-11 13:06:17.811390 runtype-0.3.2/README.md
--rw-r--r--   0        0        0     1536 2023-04-28 16:04:28.218617 runtype-0.3.2/runtype/__init__.py
--rw-r--r--   0        0        0     9279 2022-10-11 12:52:05.446440 runtype-0.3.2/runtype/base_types.py
--rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.2/runtype/common.py
--rw-r--r--   0        0        0    13658 2023-04-17 13:00:48.910623 runtype-0.3.2/runtype/dataclass.py
--rw-r--r--   0        0        0     8098 2021-12-14 13:06:00.734037 runtype-0.3.2/runtype/datetime_parse.py
--rw-r--r--   0        0        0     5839 2023-04-17 13:00:48.912622 runtype-0.3.2/runtype/dispatch.py
--rw-r--r--   0        0        0      823 2023-04-17 13:00:48.914621 runtype-0.3.2/runtype/mypy.py
--rw-r--r--   0        0        0     3115 2022-06-25 08:55:10.918634 runtype-0.3.2/runtype/mypy_bu.py
--rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.2/runtype/py.typed
--rw-r--r--   0        0        0    15107 2023-04-17 13:00:48.916621 runtype-0.3.2/runtype/pytypes.py
--rw-r--r--   0        0        0      552 2023-04-17 13:00:48.919622 runtype-0.3.2/runtype/typesystem.py
--rw-r--r--   0        0        0     1379 2023-04-17 13:00:48.921619 runtype-0.3.2/runtype/utils.py
--rw-r--r--   0        0        0     3520 2023-04-17 13:00:48.924620 runtype-0.3.2/runtype/validation.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 runtype-0.3.2/setup.py
--rw-r--r--   0        0        0     5194 1970-01-01 00:00:00.000000 runtype-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2021-12-14 13:06:00.725082 runtype-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1196 2023-06-26 17:52:59.324623 runtype-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4098 2022-10-11 13:06:17.811390 runtype-0.3.3/README.md
+-rw-r--r--   0        0        0     1536 2023-06-26 17:52:57.740988 runtype-0.3.3/runtype/__init__.py
+-rw-r--r--   0        0        0     9279 2022-10-11 12:52:05.446440 runtype-0.3.3/runtype/base_types.py
+-rw-r--r--   0        0        0       57 2021-12-14 13:06:00.733081 runtype-0.3.3/runtype/common.py
+-rw-r--r--   0        0        0    13658 2023-06-26 17:51:45.007112 runtype-0.3.3/runtype/dataclass.py
+-rw-r--r--   0        0        0     8098 2021-12-14 13:06:00.734037 runtype-0.3.3/runtype/datetime_parse.py
+-rw-r--r--   0        0        0     5839 2023-06-10 14:41:20.263098 runtype-0.3.3/runtype/dispatch.py
+-rw-r--r--   0        0        0      823 2023-04-17 13:00:48.914621 runtype-0.3.3/runtype/mypy.py
+-rw-r--r--   0        0        0     3115 2022-06-25 08:55:10.918634 runtype-0.3.3/runtype/mypy_bu.py
+-rw-r--r--   0        0        0        0 2022-10-11 12:52:05.449333 runtype-0.3.3/runtype/py.typed
+-rw-r--r--   0        0        0    15107 2023-06-10 14:41:20.264100 runtype-0.3.3/runtype/pytypes.py
+-rw-r--r--   0        0        0      552 2023-05-29 19:21:24.002389 runtype-0.3.3/runtype/typesystem.py
+-rw-r--r--   0        0        0     1379 2023-04-17 13:00:48.921619 runtype-0.3.3/runtype/utils.py
+-rw-r--r--   0        0        0     3520 2023-05-30 09:42:18.890424 runtype-0.3.3/runtype/validation.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 runtype-0.3.3/setup.py
+-rw-r--r--   0        0        0     5194 1970-01-01 00:00:00.000000 runtype-0.3.3/PKG-INFO
```

### Comparing `runtype-0.3.2/LICENSE` & `runtype-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/pyproject.toml` & `runtype-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runtype"
-version = "0.3.2"
+version = "0.3.3"
 description = "Type dispatch and validation for run-time Python"
 authors = ["Erez Shinan <erezshin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/erezsh/runtype"
 keywords = ["types", "typing", "dispatch", "multimethods", "dataclass", "runtime"]
 classifiers = [
```

### Comparing `runtype-0.3.2/README.md` & `runtype-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/__init__.py` & `runtype-0.3.3/runtype/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .dataclass import dataclass
 from .dispatch import DispatchError, MultiDispatch
 from .validation import (PythonTyping, TypeSystem, TypeMismatchError,
                          assert_isa, isa, issubclass, validate_func, is_subtype, cv_type_checking)
 from .pytypes import Constraint, String, Int
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 __all__ = (
     'dataclass',
     'DispatchError', 'MultiDispatch',
     'PythonTyping', 'TypeSystem', 'TypeMismatchError',
     'assert_isa', 'isa', 'issubclass', 'validate_func', 'is_subtype', 'cv_type_checking',
     'Constraint', 'String', 'Int',
     'Dispatch',
```

### Comparing `runtype-0.3.2/runtype/base_types.py` & `runtype-0.3.3/runtype/base_types.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/dataclass.py` & `runtype-0.3.3/runtype/dataclass.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/datetime_parse.py` & `runtype-0.3.3/runtype/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/dispatch.py` & `runtype-0.3.3/runtype/dispatch.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/mypy.py` & `runtype-0.3.3/runtype/mypy.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/mypy_bu.py` & `runtype-0.3.3/runtype/mypy_bu.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/pytypes.py` & `runtype-0.3.3/runtype/pytypes.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/typesystem.py` & `runtype-0.3.3/runtype/typesystem.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/utils.py` & `runtype-0.3.3/runtype/utils.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/runtype/validation.py` & `runtype-0.3.3/runtype/validation.py`

 * *Files identical despite different names*

### Comparing `runtype-0.3.2/setup.py` & `runtype-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses',
                                                          'contextvars']}
 
 setup_kwargs = {
     'name': 'runtype',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Type dispatch and validation for run-time Python',
     'long_description': '![alt text](logo.png "Logo")\n\n\nRuntype is a collection of run-time type utilities for Python.\n\nIt is:\n\n:runner: Fast! Uses an internal typesystem for maximum performance.\n\n:brain: Smart! Supports `typing`, forward-references, constraints, auto-casting, and more.\n\n:gear: Configurative! Write your own type system, and use it with *dataclass* and *dispatch*.\n\n------\n\n### Modules\n\n- :star: [**validation**](https://runtype.readthedocs.io/en/latest/validation.html) - Provides a smarter alternative to `isinstance` and `issubclass`, with support for the `typing` module, and type constraints.\n\n- :star: [**dataclass**](https://runtype.readthedocs.io/en/latest/dataclass.html) - Adds run-time type validation to the built-in dataclass.\n\n    - Improves dataclass ergonomics.\n    - Supports most mypy constructs, like `typing` and forward-references (`foo: \'Bar\'`).\n    - Supports automatic value casting, Pydantic-style. (Optional, off by default)\n    - Supports types with constraints. (e.g. `String(max_length=10)`)\n    - Supports optional sampling for faster validation of big lists and dicts.\n    - Twice faster than Pydantic ([read here](https://runtype.readthedocs.io/en/latest/dataclass.html#compared-to-pydantic))\n\n- :star: [**dispatch**](https://runtype.readthedocs.io/en/latest/dispatch.html) - Provides fast multiple-dispatch for functions and methods, via a decorator.\n\n    - Inspired by Julia.\n\n- :star: [**type utilities**](https://runtype.readthedocs.io/en/latest/types.html) - Provides a set of classes to implement your own type-system.\n\n    - Used by runtype itself, to emulate the Python type-system.\n\n\n## Docs\n\nRead the docs here: https://runtype.readthedocs.io/\n\n## Install\n\n```bash\npip install runtype\n```\n\nNo dependencies.\n\nRequires Python 3.6 or up.\n\n[![Build Status](https://travis-ci.org/erezsh/runtype.svg?branch=master)](https://travis-ci.org/erezsh/runtype)\n[![codecov](https://codecov.io/gh/erezsh/runtype/branch/master/graph/badge.svg)](https://codecov.io/gh/erezsh/runtype)\n\n## Examples\n\n### Validation (Isa & Subclass)\n\n```python\nfrom typing import Dict, Mapping\nfrom runtype import isa, issubclass\n\nprint( isa({\'a\': 1}, Dict[str, int]) )\n#> True\nprint( isa({\'a\': \'b\'}, Dict[str, int]) )\n#> False\n\nprint( issubclass(Dict[str, int], Mapping[str, int]) )\n#> True\nprint( issubclass(Dict[str, int], Mapping[int, str]) )\n#> False\n```\n\n### Dataclasses\n\n```python\nfrom typing import List\nfrom datetime import datetime\nfrom runtype import dataclass\n\n@dataclass(check_types=\'cast\')  # Cast values to the target type, when applicable\nclass Person:\n    name: str\n    birthday: datetime = None   # Optional\n    interests: List[str] = []   # The list is copied for each instance\n\n\nprint( Person("Beetlejuice") )\n#> Person(name=\'Beetlejuice\', birthday=None, interests=[])\nprint( Person("Albert", "1955-04-18T00:00", [\'physics\']) )\n#> Person(name=\'Albert\', birthday=datetime.datetime(1955, 4, 18, 0, 0), interests=[\'physics\'])\nprint( Person("Bad", interests=[\'a\', 1]) )\n# Traceback (most recent call last):\n#   ...\n# TypeError: [Person] Attribute \'interests\' expected value of type list[str]. Instead got [\'a\', 1]\n\n#     Failed on item: 1, expected type str\n\n```\n\n### Multiple Dispatch\n\n```python\nfrom runtype import Dispatch\ndp = Dispatch()\n\n@dp\ndef append(a: list, b):\n    return a + [b]\n\n@dp\ndef append(a: tuple, b):\n    return a + (b,)\n\n@dp\ndef append(a: str, b: str):\n    return a + b\n\n\nprint( append([1, 2, 3], 4) )\n#> [1, 2, 3, 4]\nprint( append((1, 2, 3), 4) )\n#> (1, 2, 3, 4)\nprint( append(\'foo\', \'bar\') )\n#> foobar\nprint( append(\'foo\', 4)     )\n# Traceback (most recent call last):\n#    ...\n# runtype.dispatch.DispatchError: Function \'append\' not found for signature (<class \'str\'>, <class \'int\'>)\n```\n\n\n## License\n\nRuntype uses the [MIT license](LICENSE).\n\n## Donate\n\nIf you like Runtype and want to show your appreciation, you can do so at my [patreon page](https://www.patreon.com/erezsh), or [ko-fi page](https://ko-fi.com/erezsh).\n',
     'author': 'Erez Shinan',
     'author_email': 'erezshin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/erezsh/runtype',
```

### Comparing `runtype-0.3.2/PKG-INFO` & `runtype-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtype
-Version: 0.3.2
+Version: 0.3.3
 Summary: Type dispatch and validation for run-time Python
 Home-page: https://github.com/erezsh/runtype
 License: MIT
 Keywords: types,typing,dispatch,multimethods,dataclass,runtime
 Author: Erez Shinan
 Author-email: erezshin@gmail.com
 Requires-Python: >=3.6,<4.0
```

