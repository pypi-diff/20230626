# Comparing `tmp/flake8-plugin-utils-1.3.2.tar.gz` & `tmp/flake8-plugin-utils-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-plugin-utils-1.3.2.tar", max compression
+gzip compressed data, was "flake8-plugin-utils-1.3.3.tar", max compression
```

## Comparing `flake8-plugin-utils-1.3.2.tar` & `flake8-plugin-utils-1.3.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1073 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/LICENSE
--rw-r--r--   0        0        0     6183 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/README.md
--rw-r--r--   0        0        0      351 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/__init__.py
--rw-r--r--   0        0        0     3401 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/plugin.py
--rw-r--r--   0        0        0      288 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/__init__.py
--rw-r--r--   0        0        0     1341 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/_internal.py
--rw-r--r--   0        0        0     1263 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/assertions.py
--rw-r--r--   0        0        0      327 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/constants.py
--rw-r--r--   0        0        0     5243 2021-05-05 08:47:46.709048 flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/equiv_nodes.py
--rw-r--r--   0        0        0      803 2021-05-05 08:47:46.713048 flake8-plugin-utils-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     7086 2021-05-05 08:48:49.675629 flake8-plugin-utils-1.3.2/setup.py
--rw-r--r--   0        0        0     6927 2021-05-05 08:48:49.676092 flake8-plugin-utils-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-01-13 21:10:20.612600 flake8-plugin-utils-1.3.3/LICENSE
+-rw-r--r--   0        0        0     6260 2023-06-26 16:38:36.082323 flake8-plugin-utils-1.3.3/README.md
+-rw-r--r--   0        0        0      351 2022-01-13 21:28:45.752221 flake8-plugin-utils-1.3.3/flake8_plugin_utils/__init__.py
+-rw-r--r--   0        0        0     3401 2022-01-13 21:28:42.877011 flake8-plugin-utils-1.3.3/flake8_plugin_utils/plugin.py
+-rw-r--r--   0        0        0        0 2022-01-13 21:10:20.614030 flake8-plugin-utils-1.3.3/flake8_plugin_utils/py.typed
+-rw-r--r--   0        0        0      288 2022-01-13 21:28:48.958809 flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2022-01-13 21:10:20.614638 flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/_internal.py
+-rw-r--r--   0        0        0     1263 2022-01-13 21:10:20.614846 flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/assertions.py
+-rw-r--r--   0        0        0      327 2022-01-13 21:10:20.615105 flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/constants.py
+-rw-r--r--   0        0        0     5243 2022-01-13 21:10:20.615343 flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/equiv_nodes.py
+-rw-r--r--   0        0        0      846 2022-01-13 21:30:30.766187 flake8-plugin-utils-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7168 2023-06-26 16:42:13.729473 flake8-plugin-utils-1.3.3/setup.py
+-rw-r--r--   0        0        0     7055 2023-06-26 16:42:13.730085 flake8-plugin-utils-1.3.3/PKG-INFO
```

### Comparing `flake8-plugin-utils-1.3.2/LICENSE` & `flake8-plugin-utils-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-plugin-utils-1.3.2/README.md` & `flake8-plugin-utils-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 class MyPluginWithConfig(Plugin):
     name = 'MyPluginWithConfig'
     version = '0.0.1'
     visitors = [MyVisitorWithConfig]
 
     @classmethod
     def add_options(cls, options_manager):
-        options_manager.add_option('--config_option', ...)
+        options_manager.add_option('--config_option', parse_from_config=True, ...)
 
     @classmethod
     def parse_options_to_config(cls, option_manager, options, args):
         return MyConfig(config_option=options.config_option)
 
 
 def test_code_with_error():
@@ -182,14 +182,19 @@
 ## Change Log
 
 Unreleased
 -----
 
 * ...
 
+1.3.3 - 2022-01-14
+-----
+
+* add py.typed file (#78)
+
 1.3.2 - 2021-05-05
 -----
 
 * Drop noqa detection (#56)
 * docs: Add help for Makefile
 
 1.3.1 - 2020-08-06
```

### Comparing `flake8-plugin-utils-1.3.2/flake8_plugin_utils/plugin.py` & `flake8-plugin-utils-1.3.3/flake8_plugin_utils/plugin.py`

 * *Files identical despite different names*

### Comparing `flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/_internal.py` & `flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/_internal.py`

 * *Files identical despite different names*

### Comparing `flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/assertions.py` & `flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `flake8-plugin-utils-1.3.2/flake8_plugin_utils/utils/equiv_nodes.py` & `flake8-plugin-utils-1.3.3/flake8_plugin_utils/utils/equiv_nodes.py`

 * *Files identical despite different names*

### Comparing `flake8-plugin-utils-1.3.2/pyproject.toml` & `flake8-plugin-utils-1.3.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "flake8-plugin-utils"
-version = "1.3.2"
+version = "1.3.3"
 description = "The package provides base classes and utils for flake8 plugin writing"
 authors = ["Afonasev Evgeniy <ea.afonasev@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = "https://github.com/afonasev/flake8-plugin-utils"
 homepage = "https://pypi.org/project/flake8-plugin-utils"
 keywords = ['flake8', 'plugin', 'utils']
+include = ["flake8_plugin_utils/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 
 [tool.poetry.dev-dependencies]
 black = {version = "^19.10-beta.0", allow-prereleases = true}
 bumpversion = "^0.6.0"
 flake8-awesome = ">=0.2.0"
-mypy = "^0.812"
+mypy = "^0.930"
 pylint = "^2.8"
 pytest = "^6.2"
 pytest-cov = "^2.11"
 pytest-deadfixtures = "^2.2"
 pytest-mock = "^3.6"
 unify = "^0.5"
```

### Comparing `flake8-plugin-utils-1.3.2/setup.py` & `flake8-plugin-utils-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['flake8_plugin_utils', 'flake8_plugin_utils.utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'flake8-plugin-utils',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'The package provides base classes and utils for flake8 plugin writing',
-    'long_description': "# flake8-plugin-utils\n\n[![pypi](https://badge.fury.io/py/flake8-plugin-utils.svg)](https://pypi.org/project/flake8-plugin-utils)\n[![Python: 3.6+](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://pypi.org/project/flake8-plugin-utils)\n[![Downloads](https://img.shields.io/pypi/dm/flake8-plugin-utils.svg)](https://pypistats.org/packages/flake8-plugin-utils)\n[![Build Status](https://travis-ci.org/Afonasev/flake8-plugin-utils.svg?branch=master)](https://travis-ci.org/Afonasev/flake8-plugin-utils)\n[![Code coverage](https://codecov.io/gh/afonasev/flake8-plugin-utils/branch/master/graph/badge.svg)](https://codecov.io/gh/afonasev/flake8-plugin-utils)\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\nThe package provides base classes and utils for flake8 plugin writing.\n\n## Installation\n\n```bash\npip install flake8-plugin-utils\n```\n\n## Example\n\nWrite simple plugin\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, Plugin\n\nclass MyError(Error):\n    code = 'X100'\n    message = 'my error'\n\nclass MyVisitor(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(MyError, node)\n\nclass MyPlugin(Plugin):\n    name = 'MyPlugin'\n    version = '0.1.0'\n    visitors = [MyVisitor]\n```\n\nand test it with pytest\n\n```python\nfrom flake8_plugin_utils import assert_error, assert_not_error\n\ndef test_code_with_error():\n    assert_error(MyVisitor, 'class Y: pass', MyError)\n\ndef test_code_without_error():\n    assert_not_error(MyVisitor, 'x = 1')\n```\n\n### Configuration\n\nTo add configuration to a plugin, do the following:\n\n1. Implement classmethod `add_options` in your plugin class, as per the\n[flake8 docs](https://flake8.pycqa.org/en/latest/plugin-development/plugin-parameters.html#registering-options).\n1. Override classmethod `parse_options_to_config` in your plugin class\nto return any object holding the options you need.\n1. If you need a custom `__init__` for your visitor, make sure it accepts\na keyword argument named `config` and pass it to `super().__init__`\n1. Use `self.config` in visitor code.\n\nExample:\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, Plugin, assert_error\n\nclass MyError(Error):\n    code = 'X100'\n    message = 'my error with {thing}'\n\nclass MyConfig:\n    def __init__(self, config_option):\n        self.config_option = config_option\n\nclass MyVisitorWithConfig(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(\n            MyError, node, thing=f'{node.name} {self.config.config_option}'\n        )\n\nclass MyPluginWithConfig(Plugin):\n    name = 'MyPluginWithConfig'\n    version = '0.0.1'\n    visitors = [MyVisitorWithConfig]\n\n    @classmethod\n    def add_options(cls, options_manager):\n        options_manager.add_option('--config_option', ...)\n\n    @classmethod\n    def parse_options_to_config(cls, option_manager, options, args):\n        return MyConfig(config_option=options.config_option)\n\n\ndef test_code_with_error():\n    assert_error(\n        MyVisitorWithConfig,\n        'class Y: pass',\n        MyError,\n        config=MyConfig(config_option='123'),\n        thing='Y 123',\n    )\n```\n\n### Formatting\n\nYour `Error`s can take formatting arguments in their `message`:\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, assert_error\n\nclass MyFormattedError(Error):\n    code = 'X101'\n    message = 'my error with {thing}'\n\nclass MyFormattedVisitor(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(MyFormattedError, node, thing=node.name)\n\ndef test_code_with_error():\n    assert_error(\n        MyFormattedVisitor,\n        'class Y: pass',\n        MyFormattedError,\n        thing='Y',\n    )\n```\n\n### Usage with typing/mypy\n\nThe `Plugin` and `Visitor` classes are generic with the config class as type\nparameter.  If your plugin does not have any config, inherit it from\n`Plugin[None]` and the visitors from `Visitor[None]`.  Otherwise, use the\nconfig class as the type parameter (e.g. `Plugin[MyConfig]` and\n`Visitor[MyConfig]` in the above example).\n\n### Utility functions\n\n* `assert_error`, `assert_not_error`\nUtilities for testing visitors (see examples above).\n\n* `is_true`, `is_false`, `is_none`\nConvenience functions to check if an AST node represents a\n`True`/`False`/`None` value.\n\n* `check_equivalent_nodes`\nChecks if two given AST nodes are equivalent.\nThe nodes are considered equivalent in the following cases:\n  * dicts -- if they contain same key-value pairs, possibly in different order,\n  with duplicates and `**expansions` taken into account\n  * sets -- if they contain same elements, possibly in different order,\n  with duplicates taken into account\n  * anything else -- if they represent the same AST, regardless of formatting\n  (with any dicts in sets inside checked according to the rules above)\n\n## For developers\n\n### Show help\n\n    make help\n\n### Create venv and install deps\n\n    make init\n\n### Install git precommit hook\n\n    make precommit\n\n### Run linters, autoformat, tests etc.\n\n    make pretty lint test\n\n### Bump new version\n\n    make bump_major\n    make bump_minor\n    make bump_patch\n\n## Change Log\n\nUnreleased\n-----\n\n* ...\n\n1.3.2 - 2021-05-05\n-----\n\n* Drop noqa detection (#56)\n* docs: Add help for Makefile\n\n1.3.1 - 2020-08-06\n-----\n\n* Fix handling of encoding when loading files (#37)\n\n1.3.0 - 2020-03-26\n-----\n\n* add `check_equivalent_nodes` utility function\n\n1.2.0 - 2020-03-06\n-----\n\n* add `config` argument to `assert_error` and `assert_not_error`\n\n1.1.1 - 2020-03-02\n-----\n\n* ignore encoding errors when reading strings for noqa validation\n\n1.1.0 - 2020-03-01\n-----\n\n* add ability for plugins to parse and use configuration\n**NB: this change breaks type-checking if you use typing/mypy. Change your\ncode to inherit from `Plugin[None]` and `Visitor[None]` to fix.**\n\n1.0.0 - 2019-05-23\n-----\n\n* add message formatting to Error\n\n0.2.1 - 2019-04-01\n-----\n\n* don`t strip before src dedent in _error_from_src\n* add is_none, is_true, is_false util functions\n\n0.2.0 - 2019.02.21\n-----\n\n* add assert methods\n\n0.1.0 - 2019.02.09\n-----\n\n* initial\n",
+    'long_description': "# flake8-plugin-utils\n\n[![pypi](https://badge.fury.io/py/flake8-plugin-utils.svg)](https://pypi.org/project/flake8-plugin-utils)\n[![Python: 3.6+](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://pypi.org/project/flake8-plugin-utils)\n[![Downloads](https://img.shields.io/pypi/dm/flake8-plugin-utils.svg)](https://pypistats.org/packages/flake8-plugin-utils)\n[![Build Status](https://travis-ci.org/Afonasev/flake8-plugin-utils.svg?branch=master)](https://travis-ci.org/Afonasev/flake8-plugin-utils)\n[![Code coverage](https://codecov.io/gh/afonasev/flake8-plugin-utils/branch/master/graph/badge.svg)](https://codecov.io/gh/afonasev/flake8-plugin-utils)\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\nThe package provides base classes and utils for flake8 plugin writing.\n\n## Installation\n\n```bash\npip install flake8-plugin-utils\n```\n\n## Example\n\nWrite simple plugin\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, Plugin\n\nclass MyError(Error):\n    code = 'X100'\n    message = 'my error'\n\nclass MyVisitor(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(MyError, node)\n\nclass MyPlugin(Plugin):\n    name = 'MyPlugin'\n    version = '0.1.0'\n    visitors = [MyVisitor]\n```\n\nand test it with pytest\n\n```python\nfrom flake8_plugin_utils import assert_error, assert_not_error\n\ndef test_code_with_error():\n    assert_error(MyVisitor, 'class Y: pass', MyError)\n\ndef test_code_without_error():\n    assert_not_error(MyVisitor, 'x = 1')\n```\n\n### Configuration\n\nTo add configuration to a plugin, do the following:\n\n1. Implement classmethod `add_options` in your plugin class, as per the\n[flake8 docs](https://flake8.pycqa.org/en/latest/plugin-development/plugin-parameters.html#registering-options).\n1. Override classmethod `parse_options_to_config` in your plugin class\nto return any object holding the options you need.\n1. If you need a custom `__init__` for your visitor, make sure it accepts\na keyword argument named `config` and pass it to `super().__init__`\n1. Use `self.config` in visitor code.\n\nExample:\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, Plugin, assert_error\n\nclass MyError(Error):\n    code = 'X100'\n    message = 'my error with {thing}'\n\nclass MyConfig:\n    def __init__(self, config_option):\n        self.config_option = config_option\n\nclass MyVisitorWithConfig(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(\n            MyError, node, thing=f'{node.name} {self.config.config_option}'\n        )\n\nclass MyPluginWithConfig(Plugin):\n    name = 'MyPluginWithConfig'\n    version = '0.0.1'\n    visitors = [MyVisitorWithConfig]\n\n    @classmethod\n    def add_options(cls, options_manager):\n        options_manager.add_option('--config_option', parse_from_config=True, ...)\n\n    @classmethod\n    def parse_options_to_config(cls, option_manager, options, args):\n        return MyConfig(config_option=options.config_option)\n\n\ndef test_code_with_error():\n    assert_error(\n        MyVisitorWithConfig,\n        'class Y: pass',\n        MyError,\n        config=MyConfig(config_option='123'),\n        thing='Y 123',\n    )\n```\n\n### Formatting\n\nYour `Error`s can take formatting arguments in their `message`:\n\n```python\nfrom flake8_plugin_utils import Error, Visitor, assert_error\n\nclass MyFormattedError(Error):\n    code = 'X101'\n    message = 'my error with {thing}'\n\nclass MyFormattedVisitor(Visitor):\n    def visit_ClassDef(self, node):\n        self.error_from_node(MyFormattedError, node, thing=node.name)\n\ndef test_code_with_error():\n    assert_error(\n        MyFormattedVisitor,\n        'class Y: pass',\n        MyFormattedError,\n        thing='Y',\n    )\n```\n\n### Usage with typing/mypy\n\nThe `Plugin` and `Visitor` classes are generic with the config class as type\nparameter.  If your plugin does not have any config, inherit it from\n`Plugin[None]` and the visitors from `Visitor[None]`.  Otherwise, use the\nconfig class as the type parameter (e.g. `Plugin[MyConfig]` and\n`Visitor[MyConfig]` in the above example).\n\n### Utility functions\n\n* `assert_error`, `assert_not_error`\nUtilities for testing visitors (see examples above).\n\n* `is_true`, `is_false`, `is_none`\nConvenience functions to check if an AST node represents a\n`True`/`False`/`None` value.\n\n* `check_equivalent_nodes`\nChecks if two given AST nodes are equivalent.\nThe nodes are considered equivalent in the following cases:\n  * dicts -- if they contain same key-value pairs, possibly in different order,\n  with duplicates and `**expansions` taken into account\n  * sets -- if they contain same elements, possibly in different order,\n  with duplicates taken into account\n  * anything else -- if they represent the same AST, regardless of formatting\n  (with any dicts in sets inside checked according to the rules above)\n\n## For developers\n\n### Show help\n\n    make help\n\n### Create venv and install deps\n\n    make init\n\n### Install git precommit hook\n\n    make precommit\n\n### Run linters, autoformat, tests etc.\n\n    make pretty lint test\n\n### Bump new version\n\n    make bump_major\n    make bump_minor\n    make bump_patch\n\n## Change Log\n\nUnreleased\n-----\n\n* ...\n\n1.3.3 - 2022-01-14\n-----\n\n* add py.typed file (#78)\n\n1.3.2 - 2021-05-05\n-----\n\n* Drop noqa detection (#56)\n* docs: Add help for Makefile\n\n1.3.1 - 2020-08-06\n-----\n\n* Fix handling of encoding when loading files (#37)\n\n1.3.0 - 2020-03-26\n-----\n\n* add `check_equivalent_nodes` utility function\n\n1.2.0 - 2020-03-06\n-----\n\n* add `config` argument to `assert_error` and `assert_not_error`\n\n1.1.1 - 2020-03-02\n-----\n\n* ignore encoding errors when reading strings for noqa validation\n\n1.1.0 - 2020-03-01\n-----\n\n* add ability for plugins to parse and use configuration\n**NB: this change breaks type-checking if you use typing/mypy. Change your\ncode to inherit from `Plugin[None]` and `Visitor[None]` to fix.**\n\n1.0.0 - 2019-05-23\n-----\n\n* add message formatting to Error\n\n0.2.1 - 2019-04-01\n-----\n\n* don`t strip before src dedent in _error_from_src\n* add is_none, is_true, is_false util functions\n\n0.2.0 - 2019.02.21\n-----\n\n* add assert methods\n\n0.1.0 - 2019.02.09\n-----\n\n* initial\n",
     'author': 'Afonasev Evgeniy',
     'author_email': 'ea.afonasev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/flake8-plugin-utils',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `flake8-plugin-utils-1.3.2/PKG-INFO` & `flake8-plugin-utils-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: flake8-plugin-utils
-Version: 1.3.2
+Version: 1.3.3
 Summary: The package provides base classes and utils for flake8 plugin writing
 Home-page: https://pypi.org/project/flake8-plugin-utils
 License: MIT
 Keywords: flake8,plugin,utils
 Author: Afonasev Evgeniy
 Author-email: ea.afonasev@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Repository, https://github.com/afonasev/flake8-plugin-utils
 Description-Content-Type: text/markdown
 
@@ -102,15 +103,15 @@
 class MyPluginWithConfig(Plugin):
     name = 'MyPluginWithConfig'
     version = '0.0.1'
     visitors = [MyVisitorWithConfig]
 
     @classmethod
     def add_options(cls, options_manager):
-        options_manager.add_option('--config_option', ...)
+        options_manager.add_option('--config_option', parse_from_config=True, ...)
 
     @classmethod
     def parse_options_to_config(cls, option_manager, options, args):
         return MyConfig(config_option=options.config_option)
 
 
 def test_code_with_error():
@@ -201,14 +202,19 @@
 ## Change Log
 
 Unreleased
 -----
 
 * ...
 
+1.3.3 - 2022-01-14
+-----
+
+* add py.typed file (#78)
+
 1.3.2 - 2021-05-05
 -----
 
 * Drop noqa detection (#56)
 * docs: Add help for Makefile
 
 1.3.1 - 2020-08-06
```

