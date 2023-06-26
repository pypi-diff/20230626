# Comparing `tmp/danbi-0.2.98.tar.gz` & `tmp/danbi-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danbi-0.2.98.tar", max compression
+gzip compressed data, was "danbi-0.2.99.tar", max compression
```

## Comparing `danbi-0.2.98.tar` & `danbi-0.2.99.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11357 2023-01-16 04:29:47.588484 danbi-0.2.98/LICENSE
--rw-r--r--   0        0        0      294 2023-01-16 04:29:47.588573 danbi-0.2.98/README.md
--rw-r--r--   0        0        0       92 2023-03-23 04:47:50.417029 danbi-0.2.98/danbi/__init__.py
--rw-r--r--   0        0        0      611 2023-03-09 08:51:44.539618 danbi-0.2.98/danbi/analysis/__init__.py
--rw-r--r--   0        0        0     2003 2023-01-16 04:29:47.588945 danbi-0.2.98/danbi/analysis/convert.py
--rw-r--r--   0        0        0     4386 2023-01-16 04:29:47.589049 danbi-0.2.98/danbi/analysis/normalization.py
--rw-r--r--   0        0        0     4657 2023-01-16 04:29:47.589162 danbi-0.2.98/danbi/analysis/pandas_ext.py
--rw-r--r--   0        0        0    18166 2023-01-16 04:29:47.589349 danbi-0.2.98/danbi/analysis/plot_bokeh.py
--rw-r--r--   0        0        0     2672 2023-01-16 04:29:47.589457 danbi-0.2.98/danbi/analysis/relation.py
--rw-r--r--   0        0        0     1125 2023-01-16 04:29:47.589592 danbi-0.2.98/danbi/database/ConnMngPsql.py
--rw-r--r--   0        0        0     1011 2023-01-16 04:29:47.589675 danbi-0.2.98/danbi/database/ConnMngPsqlAsync.py
--rw-r--r--   0        0        0     3771 2023-03-23 04:47:25.375685 danbi-0.2.98/danbi/database/DBPsql.py
--rw-r--r--   0        0        0     3313 2023-03-23 04:33:57.770664 danbi-0.2.98/danbi/database/DBPsqlAsync.py
--rw-r--r--   0        0        0      709 2023-01-16 04:29:47.589979 danbi-0.2.98/danbi/database/IConnectionManager.py
--rw-r--r--   0        0        0     5641 2023-03-23 04:45:21.601055 danbi-0.2.98/danbi/database/IDB.py
--rw-r--r--   0        0        0      961 2023-01-16 04:29:47.590182 danbi-0.2.98/danbi/database/__init__.py
--rw-r--r--   0        0        0     1121 2023-01-16 04:29:47.590263 danbi-0.2.98/danbi/database/factory.py
--rw-r--r--   0        0        0       23 2023-01-16 04:29:47.590383 danbi-0.2.98/danbi/extends/__init__.py
--rw-r--r--   0        0        0       85 2023-01-16 04:29:47.590501 danbi-0.2.98/danbi/extends/bipandas/__init__.py
--rw-r--r--   0        0        0     4532 2023-03-01 07:57:14.555719 danbi-0.2.98/danbi/extends/bipandas/column_ext.py
--rw-r--r--   0        0        0     2079 2023-03-20 16:07:33.128949 danbi-0.2.98/danbi/extends/bipandas/dataframe_ext.py
--rw-r--r--   0        0        0     1296 2023-01-16 04:29:47.590775 danbi-0.2.98/danbi/extends/bipandas/state.py
--rw-r--r--   0        0        0        0 2023-01-16 04:29:47.590907 danbi-0.2.98/danbi/extlib/__init__.py
--rw-r--r--   0        0        0     1897 2023-01-16 04:29:47.591123 danbi-0.2.98/danbi/extlib/pandas.py
--rw-r--r--   0        0        0     2885 2023-01-16 04:29:47.591225 danbi-0.2.98/danbi/extlib/ray.py
--rw-r--r--   0        0        0     1759 2023-01-16 04:29:47.591327 danbi-0.2.98/danbi/extlib/stock.py
--rw-r--r--   0        0        0     3106 2023-01-16 04:29:47.591418 danbi-0.2.98/danbi/extlib/tensorflow.py
--rw-r--r--   0        0        0     5451 2023-01-16 04:29:47.591578 danbi-0.2.98/danbi/gym/TradeSingleEnv.py
--rw-r--r--   0        0        0      318 2023-01-16 04:29:47.591678 danbi-0.2.98/danbi/gym/__init__.py
--rw-r--r--   0        0        0      788 2023-01-16 04:29:47.591765 danbi-0.2.98/danbi/gym/simulation.py
--rw-r--r--   0        0        0      194 2023-01-16 04:29:47.591846 danbi-0.2.98/danbi/gym/trade.py
--rw-r--r--   0        0        0      481 2023-01-16 04:29:47.591984 danbi-0.2.98/danbi/mapping/IMapper.py
--rw-r--r--   0        0        0     1329 2023-01-16 04:29:47.592071 danbi-0.2.98/danbi/mapping/Jinja2Mapper.py
--rw-r--r--   0        0        0     6169 2023-01-16 04:29:47.592179 danbi-0.2.98/danbi/mapping/YAMLConfig.py
--rw-r--r--   0        0        0      103 2023-01-16 04:29:47.592252 danbi-0.2.98/danbi/mapping/__init__.py
--rw-r--r--   0        0        0      205 2023-03-19 06:02:44.306929 danbi-0.2.98/danbi/plot/__init__.py
--rw-r--r--   0        0        0    11121 2023-03-19 06:04:17.156895 danbi-0.2.98/danbi/plot/bokeh.py
--rw-r--r--   0        0        0      498 2023-01-16 04:29:47.592663 danbi-0.2.98/danbi/plugable/IPlugin.py
--rw-r--r--   0        0        0      508 2023-01-16 04:29:47.592749 danbi-0.2.98/danbi/plugable/IPluginAsync.py
--rw-r--r--   0        0        0     3058 2023-01-16 04:29:47.592840 danbi-0.2.98/danbi/plugable/PluginManager.py
--rw-r--r--   0        0        0      108 2023-01-16 04:29:47.592919 danbi-0.2.98/danbi/plugable/__init__.py
--rw-r--r--   0        0        0      304 2023-01-16 04:29:47.593091 danbi-0.2.98/danbi/utils/__init__.py
--rw-r--r--   0        0        0     5159 2023-01-16 04:29:47.593200 danbi-0.2.98/danbi/utils/day_time.py
--rw-r--r--   0        0        0     2284 2023-01-16 04:29:47.593302 danbi-0.2.98/danbi/utils/info.py
--rw-r--r--   0        0        0      313 2023-01-16 04:29:47.593392 danbi-0.2.98/danbi/utils/jupyter.py
--rw-r--r--   0        0        0      240 2023-01-16 04:29:47.593474 danbi-0.2.98/danbi/utils/util.py
--rw-r--r--   0        0        0      900 2023-03-23 04:47:40.846201 danbi-0.2.98/pyproject.toml
--rw-r--r--   0        0        0     1029 2023-03-23 04:47:53.693015 danbi-0.2.98/setup.py
--rw-r--r--   0        0        0     1256 2023-03-23 04:47:53.693158 danbi-0.2.98/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-16 04:29:47.588484 danbi-0.2.99/LICENSE
+-rw-r--r--   0        0        0      294 2023-01-16 04:29:47.588573 danbi-0.2.99/README.md
+-rw-r--r--   0        0        0       92 2023-03-23 05:35:42.409808 danbi-0.2.99/danbi/__init__.py
+-rw-r--r--   0        0        0      611 2023-03-09 08:51:44.539618 danbi-0.2.99/danbi/analysis/__init__.py
+-rw-r--r--   0        0        0     2003 2023-01-16 04:29:47.588945 danbi-0.2.99/danbi/analysis/convert.py
+-rw-r--r--   0        0        0     4386 2023-01-16 04:29:47.589049 danbi-0.2.99/danbi/analysis/normalization.py
+-rw-r--r--   0        0        0     4657 2023-01-16 04:29:47.589162 danbi-0.2.99/danbi/analysis/pandas_ext.py
+-rw-r--r--   0        0        0    18166 2023-01-16 04:29:47.589349 danbi-0.2.99/danbi/analysis/plot_bokeh.py
+-rw-r--r--   0        0        0     2672 2023-01-16 04:29:47.589457 danbi-0.2.99/danbi/analysis/relation.py
+-rw-r--r--   0        0        0     1125 2023-01-16 04:29:47.589592 danbi-0.2.99/danbi/database/ConnMngPsql.py
+-rw-r--r--   0        0        0     1011 2023-01-16 04:29:47.589675 danbi-0.2.99/danbi/database/ConnMngPsqlAsync.py
+-rw-r--r--   0        0        0     3771 2023-03-23 04:47:25.375685 danbi-0.2.99/danbi/database/DBPsql.py
+-rw-r--r--   0        0        0     3313 2023-03-23 04:33:57.770664 danbi-0.2.99/danbi/database/DBPsqlAsync.py
+-rw-r--r--   0        0        0      709 2023-01-16 04:29:47.589979 danbi-0.2.99/danbi/database/IConnectionManager.py
+-rw-r--r--   0        0        0     5647 2023-03-23 05:35:29.840025 danbi-0.2.99/danbi/database/IDB.py
+-rw-r--r--   0        0        0      961 2023-01-16 04:29:47.590182 danbi-0.2.99/danbi/database/__init__.py
+-rw-r--r--   0        0        0     1121 2023-01-16 04:29:47.590263 danbi-0.2.99/danbi/database/factory.py
+-rw-r--r--   0        0        0       23 2023-01-16 04:29:47.590383 danbi-0.2.99/danbi/extends/__init__.py
+-rw-r--r--   0        0        0       85 2023-01-16 04:29:47.590501 danbi-0.2.99/danbi/extends/bipandas/__init__.py
+-rw-r--r--   0        0        0     4532 2023-03-01 07:57:14.555719 danbi-0.2.99/danbi/extends/bipandas/column_ext.py
+-rw-r--r--   0        0        0     2079 2023-03-20 16:07:33.128949 danbi-0.2.99/danbi/extends/bipandas/dataframe_ext.py
+-rw-r--r--   0        0        0     1296 2023-01-16 04:29:47.590775 danbi-0.2.99/danbi/extends/bipandas/state.py
+-rw-r--r--   0        0        0        0 2023-01-16 04:29:47.590907 danbi-0.2.99/danbi/extlib/__init__.py
+-rw-r--r--   0        0        0     1897 2023-01-16 04:29:47.591123 danbi-0.2.99/danbi/extlib/pandas.py
+-rw-r--r--   0        0        0     2885 2023-01-16 04:29:47.591225 danbi-0.2.99/danbi/extlib/ray.py
+-rw-r--r--   0        0        0     1759 2023-01-16 04:29:47.591327 danbi-0.2.99/danbi/extlib/stock.py
+-rw-r--r--   0        0        0     3106 2023-01-16 04:29:47.591418 danbi-0.2.99/danbi/extlib/tensorflow.py
+-rw-r--r--   0        0        0     5451 2023-01-16 04:29:47.591578 danbi-0.2.99/danbi/gym/TradeSingleEnv.py
+-rw-r--r--   0        0        0      318 2023-01-16 04:29:47.591678 danbi-0.2.99/danbi/gym/__init__.py
+-rw-r--r--   0        0        0      788 2023-01-16 04:29:47.591765 danbi-0.2.99/danbi/gym/simulation.py
+-rw-r--r--   0        0        0      194 2023-01-16 04:29:47.591846 danbi-0.2.99/danbi/gym/trade.py
+-rw-r--r--   0        0        0      481 2023-01-16 04:29:47.591984 danbi-0.2.99/danbi/mapping/IMapper.py
+-rw-r--r--   0        0        0     1329 2023-01-16 04:29:47.592071 danbi-0.2.99/danbi/mapping/Jinja2Mapper.py
+-rw-r--r--   0        0        0     6169 2023-01-16 04:29:47.592179 danbi-0.2.99/danbi/mapping/YAMLConfig.py
+-rw-r--r--   0        0        0      103 2023-01-16 04:29:47.592252 danbi-0.2.99/danbi/mapping/__init__.py
+-rw-r--r--   0        0        0      205 2023-03-19 06:02:44.306929 danbi-0.2.99/danbi/plot/__init__.py
+-rw-r--r--   0        0        0    11121 2023-03-19 06:04:17.156895 danbi-0.2.99/danbi/plot/bokeh.py
+-rw-r--r--   0        0        0      498 2023-01-16 04:29:47.592663 danbi-0.2.99/danbi/plugable/IPlugin.py
+-rw-r--r--   0        0        0      508 2023-01-16 04:29:47.592749 danbi-0.2.99/danbi/plugable/IPluginAsync.py
+-rw-r--r--   0        0        0     3058 2023-01-16 04:29:47.592840 danbi-0.2.99/danbi/plugable/PluginManager.py
+-rw-r--r--   0        0        0      108 2023-01-16 04:29:47.592919 danbi-0.2.99/danbi/plugable/__init__.py
+-rw-r--r--   0        0        0      304 2023-01-16 04:29:47.593091 danbi-0.2.99/danbi/utils/__init__.py
+-rw-r--r--   0        0        0     5159 2023-01-16 04:29:47.593200 danbi-0.2.99/danbi/utils/day_time.py
+-rw-r--r--   0        0        0     2284 2023-01-16 04:29:47.593302 danbi-0.2.99/danbi/utils/info.py
+-rw-r--r--   0        0        0      313 2023-01-16 04:29:47.593392 danbi-0.2.99/danbi/utils/jupyter.py
+-rw-r--r--   0        0        0      240 2023-01-16 04:29:47.593474 danbi-0.2.99/danbi/utils/util.py
+-rw-r--r--   0        0        0      900 2023-03-23 05:35:46.266361 danbi-0.2.99/pyproject.toml
+-rw-r--r--   0        0        0     1029 2023-03-23 05:35:48.689245 danbi-0.2.99/setup.py
+-rw-r--r--   0        0        0     1256 2023-03-23 05:35:48.689421 danbi-0.2.99/PKG-INFO
```

### Comparing `danbi-0.2.98/LICENSE` & `danbi-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/__init__.py` & `danbi-0.2.99/danbi/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/convert.py` & `danbi-0.2.99/danbi/analysis/convert.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/normalization.py` & `danbi-0.2.99/danbi/analysis/normalization.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/pandas_ext.py` & `danbi-0.2.99/danbi/analysis/pandas_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/plot_bokeh.py` & `danbi-0.2.99/danbi/analysis/plot_bokeh.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/analysis/relation.py` & `danbi-0.2.99/danbi/analysis/relation.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/ConnMngPsql.py` & `danbi-0.2.99/danbi/database/ConnMngPsql.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/ConnMngPsqlAsync.py` & `danbi-0.2.99/danbi/database/ConnMngPsqlAsync.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/DBPsql.py` & `danbi-0.2.99/danbi/database/DBPsql.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/DBPsqlAsync.py` & `danbi-0.2.99/danbi/database/DBPsqlAsync.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/IConnectionManager.py` & `danbi-0.2.99/danbi/database/IConnectionManager.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/IDB.py` & `danbi-0.2.99/danbi/database/IDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import collections
 import itertools
 from typing import Any, Dict, Tuple, List, Union
 import pandas as pd
-from threading import Lock
+from multiprocessing import Lock
 
 from .IConnectionManager import IConnectionManager
 from ..mapping.IMapper import IMapper
 
 class IDB(abc.ABC):
     def __new__(self, manager: IConnectionManager, mapper: IMapper):
         self._manager = manager
```

### Comparing `danbi-0.2.98/danbi/database/__init__.py` & `danbi-0.2.99/danbi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/database/factory.py` & `danbi-0.2.99/danbi/database/factory.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extends/bipandas/column_ext.py` & `danbi-0.2.99/danbi/extends/bipandas/column_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extends/bipandas/dataframe_ext.py` & `danbi-0.2.99/danbi/extends/bipandas/dataframe_ext.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extends/bipandas/state.py` & `danbi-0.2.99/danbi/extends/bipandas/state.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extlib/pandas.py` & `danbi-0.2.99/danbi/extlib/pandas.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extlib/ray.py` & `danbi-0.2.99/danbi/extlib/ray.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extlib/stock.py` & `danbi-0.2.99/danbi/extlib/stock.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/extlib/tensorflow.py` & `danbi-0.2.99/danbi/extlib/tensorflow.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/gym/TradeSingleEnv.py` & `danbi-0.2.99/danbi/gym/TradeSingleEnv.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/gym/simulation.py` & `danbi-0.2.99/danbi/gym/simulation.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/mapping/Jinja2Mapper.py` & `danbi-0.2.99/danbi/mapping/Jinja2Mapper.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/mapping/YAMLConfig.py` & `danbi-0.2.99/danbi/mapping/YAMLConfig.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/plot/bokeh.py` & `danbi-0.2.99/danbi/plot/bokeh.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/plugable/PluginManager.py` & `danbi-0.2.99/danbi/plugable/PluginManager.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/utils/day_time.py` & `danbi-0.2.99/danbi/utils/day_time.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/danbi/utils/info.py` & `danbi-0.2.99/danbi/utils/info.py`

 * *Files identical despite different names*

### Comparing `danbi-0.2.98/pyproject.toml` & `danbi-0.2.99/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "danbi"
-version = "0.2.98"
+version = "0.2.99"
 description = "python utility library"
 authors = ["nockchun <nockchun@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nockchun/danbi"
 repository = "https://github.com/nockchun/danbi"
 keywords = ["mybatis like", "sql mapper", "python utils"]
```

### Comparing `danbi-0.2.98/setup.py` & `danbi-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'danbi.utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'danbi',
-    'version': '0.2.98',
+    'version': '0.2.99',
     'description': 'python utility library',
     'long_description': '# danbi\n[![license]](/LICENSE)\n[![pypi]](https://pypi.org/project/danbi/)\n[![pyversions]](http://pypi.python.org/pypi/danbi)\n[![Downloads](https://pepy.tech/badge/danbi)](https://pepy.tech/project/danbi)\n\n---\n\ndanbi is python utility library.\n\n## Installation\n\n```python\npip install danbi\n```\n\n',
     'author': 'nockchun',
     'author_email': 'nockchun@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/nockchun/danbi',
```

### Comparing `danbi-0.2.98/PKG-INFO` & `danbi-0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danbi
-Version: 0.2.98
+Version: 0.2.99
 Summary: python utility library
 Home-page: https://github.com/nockchun/danbi
 License: Apache-2.0
 Keywords: mybatis like,sql mapper,python utils
 Author: nockchun
 Author-email: nockchun@gmail.com
 Requires-Python: >=3.7,<4.0
```

