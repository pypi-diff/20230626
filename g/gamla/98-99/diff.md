# Comparing `tmp/gamla-98.tar.gz` & `tmp/gamla-99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamla-98.tar", last modified: Sun Sep 12 17:54:40 2021, max compression
+gzip compressed data, was "gamla-99.tar", last modified: Tue Sep 14 14:23:03 2021, max compression
```

## Comparing `gamla-98.tar` & `gamla-99.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.060513 gamla-98/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2021-09-12 17:54:03.000000 gamla-98/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4749 2021-09-12 17:54:40.060513 gamla-98/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-09-12 17:54:03.000000 gamla-98/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.052509 gamla-98/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.056511 gamla-98/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2098 2021-09-12 17:54:03.000000 gamla-98/docs/source/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.060513 gamla-98/gamla/
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2021-09-12 17:54:03.000000 gamla-98/gamla/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1031 2021-09-12 17:54:03.000000 gamla-98/gamla/apply_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2021-09-12 17:54:03.000000 gamla-98/gamla/apply_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2528 2021-09-12 17:54:03.000000 gamla-98/gamla/currying.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4317 2021-09-12 17:54:03.000000 gamla-98/gamla/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2021-09-12 17:54:03.000000 gamla-98/gamla/data_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3868 2021-09-12 17:54:03.000000 gamla-98/gamla/debug_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4093 2021-09-12 17:54:03.000000 gamla-98/gamla/dict_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1688 2021-09-12 17:54:03.000000 gamla-98/gamla/dict_utils_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2021-09-12 17:54:03.000000 gamla-98/gamla/excepts_decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2021-09-12 17:54:03.000000 gamla-98/gamla/excepts_decorator_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22165 2021-09-12 17:54:03.000000 gamla-98/gamla/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3376 2021-09-12 17:54:03.000000 gamla-98/gamla/functional_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26320 2021-09-12 17:54:03.000000 gamla-98/gamla/functional_generic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18270 2021-09-12 17:54:03.000000 gamla-98/gamla/functional_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8210 2021-09-12 17:54:03.000000 gamla-98/gamla/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-09-12 17:54:03.000000 gamla-98/gamla/graph_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2021-09-12 17:54:03.000000 gamla-98/gamla/graph_async_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1980 2021-09-12 17:54:03.000000 gamla-98/gamla/graph_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1502 2021-09-12 17:54:03.000000 gamla-98/gamla/higher_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2021-09-12 17:54:03.000000 gamla-98/gamla/higher_order_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8434 2021-09-12 17:54:03.000000 gamla-98/gamla/io_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3097 2021-09-12 17:54:03.000000 gamla-98/gamla/io_utils_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.060513 gamla-98/gamla/optimized/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:03.000000 gamla-98/gamla/optimized/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2021-09-12 17:54:03.000000 gamla-98/gamla/optimized/async_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5346 2021-09-12 17:54:03.000000 gamla-98/gamla/optimized/sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2021-09-12 17:54:03.000000 gamla-98/gamla/string_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4946 2021-09-12 17:54:03.000000 gamla-98/gamla/transducer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2021-09-12 17:54:03.000000 gamla-98/gamla/transducer_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4731 2021-09-12 17:54:03.000000 gamla-98/gamla/tree.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      677 2021-09-12 17:54:03.000000 gamla-98/gamla/tree_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2021-09-12 17:54:03.000000 gamla-98/gamla/url_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2021-09-12 17:54:03.000000 gamla-98/gamla/url_utils_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-12 17:54:40.060513 gamla-98/gamla.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4749 2021-09-12 17:54:39.000000 gamla-98/gamla.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      926 2021-09-12 17:54:39.000000 gamla-98/gamla.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-09-12 17:54:39.000000 gamla-98/gamla.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-09-12 17:54:39.000000 gamla-98/gamla.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-09-12 17:54:39.000000 gamla-98/gamla.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-09-12 17:54:40.060513 gamla-98/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      527 2021-09-12 17:54:03.000000 gamla-98/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.036934 gamla-99/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2021-09-14 14:22:33.000000 gamla-99/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4749 2021-09-14 14:23:03.036934 gamla-99/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-09-14 14:22:33.000000 gamla-99/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.028934 gamla-99/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.028934 gamla-99/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2098 2021-09-14 14:22:33.000000 gamla-99/docs/source/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.032934 gamla-99/gamla/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      628 2021-09-14 14:22:33.000000 gamla-99/gamla/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1031 2021-09-14 14:22:33.000000 gamla-99/gamla/apply_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2021-09-14 14:22:33.000000 gamla-99/gamla/apply_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2491 2021-09-14 14:22:33.000000 gamla-99/gamla/currying.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3657 2021-09-14 14:22:33.000000 gamla-99/gamla/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1349 2021-09-14 14:22:33.000000 gamla-99/gamla/data_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3892 2021-09-14 14:22:33.000000 gamla-99/gamla/debug_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2021-09-14 14:22:33.000000 gamla-99/gamla/dict_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1688 2021-09-14 14:22:33.000000 gamla-99/gamla/dict_utils_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1200 2021-09-14 14:22:33.000000 gamla-99/gamla/excepts_decorator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1694 2021-09-14 14:22:33.000000 gamla-99/gamla/excepts_decorator_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22116 2021-09-14 14:22:33.000000 gamla-99/gamla/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3376 2021-09-14 14:22:33.000000 gamla-99/gamla/functional_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26013 2021-09-14 14:22:33.000000 gamla-99/gamla/functional_generic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18270 2021-09-14 14:22:33.000000 gamla-99/gamla/functional_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8212 2021-09-14 14:22:33.000000 gamla-99/gamla/graph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4707 2021-09-14 14:22:33.000000 gamla-99/gamla/graph_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1859 2021-09-14 14:22:33.000000 gamla-99/gamla/graph_async_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1980 2021-09-14 14:22:33.000000 gamla-99/gamla/graph_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1502 2021-09-14 14:22:33.000000 gamla-99/gamla/higher_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2021-09-14 14:22:33.000000 gamla-99/gamla/higher_order_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8428 2021-09-14 14:22:33.000000 gamla-99/gamla/io_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3097 2021-09-14 14:22:33.000000 gamla-99/gamla/io_utils_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.036934 gamla-99/gamla/optimized/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-09-14 14:22:33.000000 gamla-99/gamla/optimized/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2021-09-14 14:22:33.000000 gamla-99/gamla/optimized/async_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5346 2021-09-14 14:22:33.000000 gamla-99/gamla/optimized/sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2021-09-14 14:22:33.000000 gamla-99/gamla/string_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4978 2021-09-14 14:22:33.000000 gamla-99/gamla/transducer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2021-09-14 14:22:33.000000 gamla-99/gamla/transducer_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4731 2021-09-14 14:22:33.000000 gamla-99/gamla/tree.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      677 2021-09-14 14:22:33.000000 gamla-99/gamla/tree_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2021-09-14 14:22:33.000000 gamla-99/gamla/url_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      542 2021-09-14 14:22:33.000000 gamla-99/gamla/url_utils_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-14 14:23:03.036934 gamla-99/gamla.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4749 2021-09-14 14:23:02.000000 gamla-99/gamla.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      926 2021-09-14 14:23:02.000000 gamla-99/gamla.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-09-14 14:23:02.000000 gamla-99/gamla.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-09-14 14:23:02.000000 gamla-99/gamla.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-09-14 14:23:02.000000 gamla-99/gamla.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-09-14 14:23:03.036934 gamla-99/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      527 2021-09-14 14:22:33.000000 gamla-99/setup.py
```

### Comparing `gamla-98/LICENSE` & `gamla-99/LICENSE`

 * *Files identical despite different names*

### Comparing `gamla-98/PKG-INFO` & `gamla-99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamla
-Version: 98
+Version: 99
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gamla-98/README.md` & `gamla-99/README.md`

 * *Files identical despite different names*

### Comparing `gamla-98/docs/source/conf.py` & `gamla-99/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/__init__.py` & `gamla-99/gamla/__init__.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/apply_test.py` & `gamla-99/gamla/apply_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/apply_utils.py` & `gamla-99/gamla/apply_utils.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/currying.py` & `gamla-99/gamla/currying.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,44 +36,39 @@
     for p in params.values():
         if p.default != p.empty:
             kwargs[p.name] = p.default
     return kwargs
 
 
 def curry(f):
-    """
-    Make a function handle partial input, returning a function that expects the rest.
+    """Make a function handle partial input, returning a function that expects the rest.
 
     Warning: uses `inspect` which is slow, so avoid calling this inside a loop.
 
     >>> def addition(a, b): return a + b
-    >>> add_3 = gamla.curry(addition)(3)
-    >>> add_3(7)
+    ... add_3 = gamla.curry(addition)(3)
+    ... add_3(7)
     10
 
     Can also be used as a decorator:
-    ```
     >>>@gamla.curry
     ... def addition(a, b):
     ...    return a + b
-    ```
 
     In case the function is async, the function becomes synchronous until the last argument.
     Although this is not always what you want, it fits the majority of cases.
 
-    ```
     >>> @gamla.curry
     ... async def async_addition(a, b):
     ...    await asyncio.sleep(0.1)
     ...    return a + b
 
     >>> add_3 = async_addition(3)
 
     >>> await add_3(7)  # Note that `await` is needed here. Must be done inside an async scope.
-    ```
 
     The variables can be given with keywords, but mixing keyword and call by order might have unexpected results.
     """
     f_len_args = inspect.signature(f).parameters
     assert (
         len(f_len_args) > 1
     ), f"Curry function must have at least 2 parameters, {f} has {len(f_len_args)}"
```

### Comparing `gamla-98/gamla/data.py` & `gamla-99/gamla/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import csv
 import dataclasses
 import itertools
 import json
-from typing import Any, Callable, Collection, Dict, List, Text, Tuple
+from typing import Any, Callable, Collection, Dict, Text, Tuple
 
 import dataclasses_json
 
 from gamla import currying, functional, functional_generic
 from gamla.optimized import sync
 
 
@@ -47,33 +46,20 @@
     return tuple(v)
 
 
 #: Freeze recursively a dictionary.
 #:
 #: >>> freeze_deep({"1": {"2": "345", "some-string": ["hello"]}})
 #: data.frozendict(
-#:     {"1": data.frozendict({"2": "345", "some-string": ("hello",)})},
+#:  {"1": data.frozendict({"2": "345", "some-string": ("hello",)})},
 #: )
 freeze_deep = functional_generic.map_dict(_freeze_nonterminal, functional.identity)
 
 
 @currying.curry
-def csv_to_list_of_dicts(csv_file_path, fieldnames=None) -> List:
-    """Return a list of dicts given a CSV file path.
-
-    >>> csv_to_list_of_dicts("data_test_example_with_headers.csv")
-    [{'name': 'David', 'age': '23'}, {'name': 'Itay', 'age': '26'}]
-    >>> csv_to_list_of_dicts("data_test_example_without_headers.csv", ["name", "age"])
-    [{'name': 'David', 'age': '23'}, {'name': 'Itay', 'age': '26'}]
-    """
-    with open(csv_file_path, encoding="utf-8") as csvf:
-        return list(csv.DictReader(csvf, fieldnames))
-
-
-@currying.curry
 def tuple_of_tuples_to_csv(
     tuple_of_tuples: Tuple[Tuple[Any], ...],
     separator: Text = "\t",
 ) -> Text:
     """Return a CSV formatted string given a tuple of tuples. Each element is separated by the character "separator" (default is \t).
 
     >>> tuple_of_tuples_to_csv((("name", "age"), ("David", "23"), ("Itay", "26")))
@@ -120,26 +106,18 @@
 def explode(*positions: Collection[int]):
     """Flattens a non homogeneous iterable.
 
     For an iterable where some positions are iterable and some are not,
     "explodes" the iterable, so that each element appears in a single row, and duplicates the non iterable.
 
     >>> functional_generic.pipe(
-        [
-            "x",
-            [
-                "y1",
-                "y2",
-                "y3",
-            ],
-            "z",
-        ],
-        data.explode(1),
-        tuple,
-    )
+    ...     ["x", ["y1", "y2", "y3"], "z"],
+    ...     data.explode(1),
+    ...     tuple,
+    ... )
     (
         ("x", "y1", "z"),
         ("x", "y2", "z"),
         ("x", "y3", "z"),
     )
     """
     return functional_generic.compose_left(
```

### Comparing `gamla-98/gamla/debug_utils.py` & `gamla-99/gamla/debug_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 debug_compose_left = _debug_generic(functional_generic.compose_left)
 
 
 def debug_exception(f):
     """Debug exception in a pipeline stage by looking at the causal value.
 
     >>> gamla.pipe(
-        "abc",
-        gamla.itemgetter("some_key"),  # This would cause an exception.
-    )
+    ...     "abc",
+    ...     gamla.itemgetter("some_key"),  # This would cause an exception.
+    ... )
 
     >>> gamla.pipe(
-        "abc",
-        gamla.debug_exception(gamla.itemgetter("some_key")),  # Now we can see the cause of the exception - we expect a `dict` but get a `str`.
-    )
+    ...     "abc",
+    ...     gamla.debug_exception(gamla.itemgetter("some_key")),  # Now we can see the cause of the exception - we expect a `dict` but get a `str`.
+    ... )
     """
     if asyncio.iscoroutinefunction(f):
 
         async def debug_exception(*x, **kwargs):
             try:
                 return await f(*x, **kwargs)
             except Exception as e:
```

### Comparing `gamla-98/gamla/dict_utils.py` & `gamla-99/gamla/dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 import operator
 from typing import Any, Callable, Dict, Iterable
 
 from gamla import currying, functional, functional_generic
 
 
 def itemgetter(attr):
-    """
-    Retrieves a dictionary entry by its key `attr`.
+    """Retrieves a dictionary entry by its key `attr`.
 
     >>> itemgetter("a")({"a": 1})
     1
     """
 
     def itemgetter(obj):
         return obj[attr]
 
     return itemgetter
 
 
 def itemgetter_or_none(attr):
-    """
-    Retrieves a dictionary entry by its key `attr`. Returns `None` if the key is not there.
+    """Retrieves a dictionary entry by its key `attr`. Returns `None` if the key is not there.
 
     >>> itemgetter_or_none("a")({"a": 1})
     1
 
     >>> itemgetter_or_none("b")({"a": 1})
     None
     """
@@ -33,16 +31,15 @@
     def itemgetter_or_none(obj):
         return obj.get(attr, None)
 
     return itemgetter_or_none
 
 
 def itemgetter_with_default(default, attr):
-    """
-    Retrieves a dictionary entry by its key `attr`. Returns `default` if the key is not there.
+    """Retrieves a dictionary entry by its key `attr`. Returns `default` if the key is not there.
 
     >>> itemgetter_with_default(0, "a")({"a": 1})
     1
     >>> itemgetter_with_default(0, "b")({"a": 1})
     0
     """
 
@@ -65,30 +62,28 @@
     return get_or_transform
 
 
 get_or_identity = get_or_transform(functional.identity)
 
 
 def get_in(keys: Iterable):
-    """
-    Creates a function that returns coll[i0][i1]...[iX] where [i0, i1, ..., iX]==keys.
+    """Creates a function that returns coll[i0][i1]...[iX] where [i0, i1, ..., iX]==keys.
 
     >>> get_in(["a", "b", 1])({"a": {"b": [0, 1, 2]}})
     1
     """
 
     def get_in(coll):
         return functools.reduce(operator.getitem, keys, coll)
 
     return get_in
 
 
 def get_in_with_default(keys: Iterable, default):
-    """
-    `get_in` function, returning `default` if a key is not there.
+    """`get_in` function, returning `default` if a key is not there.
 
     >>> get_in_with_default(["a", "b", 1], 0)({"a": {"b": [0, 1, 2]}})
     1
     >>> get_in_with_default(["a", "c", 1], 0)({"a": {"b": [0, 1, 2]}})
     0
     """
     getter = get_in(keys)
@@ -99,28 +94,26 @@
         except (KeyError, IndexError, TypeError):
             return default
 
     return get_in_with_default
 
 
 def get_in_or_none(keys: Iterable):
-    """
-    `get_in` function, returning `None` if a key is not there.
+    """`get_in` function, returning `None` if a key is not there.
 
     >>> get_in_or_none(["a", "b", 1])({"a": {"b": [0, 1, 2]}})
     1
     >>> get_in_or_none(["a", "c", 1])({"a": {"b": [0, 1, 2]}})
     None
     """
     return get_in_with_default(keys, None)
 
 
 def get_in_or_none_uncurried(keys: Iterable, coll):
-    """
-    Returns coll[i0][i1]...[iX] where [i0, i1, ..., iX]==keys and `None` if a key is not there.
+    """Returns coll[i0][i1]...[iX] where [i0, i1, ..., iX]==keys and `None` if a key is not there.
 
     >>> get_in_or_none_uncurried(["a", "b", 1],{"a": {"b": [0, 1, 2]}})
     1
     >>> get_in_or_none_uncurried(["a", "c", 1], {"a": {"b": [0, 1, 2]}})
     None
     """
     return get_in_or_none(keys)(coll)
```

### Comparing `gamla-98/gamla/dict_utils_test.py` & `gamla-99/gamla/dict_utils_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/excepts_decorator.py` & `gamla-99/gamla/excepts_decorator.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/excepts_decorator_test.py` & `gamla-99/gamla/excepts_decorator_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/functional.py` & `gamla-99/gamla/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 def identity(x):
     return x
 
 
 #: Count the number of items in a sequence.
 #: Like builtin function 'len' but works on iterators/generators as well
-#:    >>> count(1 for in range(4))
-#:    '4'
+#: >>> count(1 for in range(4))
+#: '4'
 count = toolz.count
 
 
 def sort_by(key: Callable):
     """Return a new list containing all items from the iterable in ascending order, sorted by a key.
     >>> sort_by(len)(["hi!", "my", "name", "is"])
     ['my', 'is', 'hi!', 'name']
@@ -641,16 +641,16 @@
 @currying.curry
 def eq_by(f, value_1, value_2):
     """Check if two values are equal when applying f on both of them."""
     return f(value_1) == f(value_2)
 
 
 #: Check if two strings are equal, ignoring case.
-#:    >>> eq_str_ignore_case("HeLlO wOrLd", "hello world")
-#:    True
+#: >>> eq_str_ignore_case("HeLlO wOrLd", "hello world")
+#: True
 eq_str_ignore_case = eq_by(str.lower)
 
 
 @currying.curry
 def groupby_many_reduce(key: Callable, reducer: Callable, seq: Iterable):
     """Group a collection by a key function, when the value is given by a reducer function.
 
@@ -936,43 +936,43 @@
     def flip(a, b):
         return func(b, a)
 
     return flip
 
 
 #: Return a dict with number of occurrences of each value in a sequence.
-#:    >>> frequencies(['cat', 'cat', 'ox', 'pig', 'pig', 'cat'])
-#:    {'cat': 3, 'ox': 1, 'pig': 2}
+#: >>> frequencies(['cat', 'cat', 'ox', 'pig', 'pig', 'cat'])
+#: {'cat': 3, 'ox': 1, 'pig': 2}
 frequencies = toolz.frequencies
 
 #: The first element in a sequence.
 #:
-#:    >>> head('ABC')
-#:    'A'
+#: >>> head('ABC')
+#: 'A'
 head = toolz.first
 
-#:  The second element in a sequence.
+#: The second element in a sequence.
 #:
-#:    >>> second('ABC')
-#:    'B'
+#: >>> second('ABC')
+#: 'B'
 second = toolz.second
 
 #: The last element in a sequence.
 #:
-#:    >>> last('ABC')
-#:    'C'
+#: >>> last('ABC')
+#: 'C'
 last = toolz.last
 
 #: Determines whether the element is iterable.
 #:
-#:    >>> isiterable([1, 2, 3])
-#:    True
+#: >>> isiterable([1, 2, 3])
+#: True
 #:
-#:    >>> isiterable(5)
-#:    False
+#: >>> isiterable(5)
+#: False
 is_iterable = toolz.isiterable
 
 
 def sliding_window(n: int):
     """A sequence of overlapping subsequences.
 
     >>> list(sliding_window(2)([1, 2, 3, 4]))
```

### Comparing `gamla-98/gamla/functional_async.py` & `gamla-99/gamla/functional_async.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 from gamla.optimized import async_functions
 
 
 def run_sync(f):
     """Runs a coroutine in a synchronous context, blocking until result arrives.
 
     >>> async def afoo(x):
-    >>>     await asyncio.sleep(1)
-    >>>     return x
-    >>> run_sync(afoo(1))
+    ...     await asyncio.sleep(1)
+    ...     return x
+    ... run_sync(afoo(1))
     1 (after 1 second of waiting)
     """
     loop = asyncio.new_event_loop()
     return loop.run_until_complete(asyncio.ensure_future(f, loop=loop))
 
 
 @currying.curry
 async def amap_ascompleted(
     f: Callable[[Any], Awaitable[Any]], it: Iterable
 ) -> AsyncGenerator[Any, None]:
     """Returns an AsyncGenerator of the results after applying async `f` to each element of Iterable `it`
 
     >>> async def amulti(x)
-    >>>    return x*2
-    >>> async def to_list(ag):
-    >>>     return [i async for i in ag]
-    >>> run_sync(to_list(amap_ascompleted(amulti, range(4))))
+    ...    return x*2
+    ... async def to_list(ag):
+    ...     return [i async for i in ag]
+    ... run_sync(to_list(amap_ascompleted(amulti, range(4))))
     [6, 0, 2, 4] (In a random order)
     """
     for future in asyncio.as_completed(map(f, it)):
         yield await future
 
 
 @currying.curry
@@ -40,69 +40,69 @@
     exception_type: Type[Exception], func: Callable, handler: Callable, x: Any
 ):
     """An async functional try/except block: await and return `func` on `x`.
     If fails with `exception_type`, return the reult of running handler on the error.
 
 
     >>> async def araise(x):
-    >>>     raise ValueError
-    >>> run_sync(aexcepts(ValueError, araise, lambda e: e, 5))
+    ...     raise ValueError
+    ... run_sync(aexcepts(ValueError, araise, lambda e: e, 5))
     ValueError()
 
     >>> async def a_just(x):
-    >>>     return x
-    >>> run_sync(aexcepts(ValueError, a_just, lambda e: e, 5))
+    ...     return x
+    ... run_sync(aexcepts(ValueError, a_just, lambda e: e, 5))
     5
     """
     try:
         return await func(x)
     except exception_type as error:
         return handler(error)
 
 
 @currying.curry
 async def mapa(f: Callable, it: AsyncGenerator) -> AsyncGenerator:
     """Returns an AsyncGenerator of the results after applying `f` to each async element of `it`
 
     >>> async def arange(count):
-    >>>     for i in range(count):
-    >>>         yield(i)
-    >>> async def to_list(ag):
-    >>>     return [i async for i in ag]
-    >>> run_sync(to_list(mapa(lambda x: x*2, arange(4))))
+    ...     for i in range(count):
+    ...         yield(i)
+    ... async def to_list(ag):
+    ...     return [i async for i in ag]
+    ... run_sync(to_list(mapa(lambda x: x*2, arange(4))))
     [0, 2, 4, 6]
     """
     async for element in it:
         yield f(element)
 
 
 async def aconcat(async_generator: AsyncGenerator) -> AsyncGenerator:
     """Concat iterables of an async_generator.
 
     >>> async def many_range(count):
-    >>>     for i in range(count):
-    >>>         yield range(i, i+1)
-    >>> async def to_list(ag):
-    >>>     return [i async for i in ag]
-    >>> run_sync(to_list(aconcat(many_range(4))))
+    ...     for i in range(count):
+    ...         yield range(i, i+1)
+    ... async def to_list(ag):
+    ...     return [i async for i in ag]
+    ... run_sync(to_list(aconcat(many_range(4))))
     [0, 1, 2, 3]
     """
     async for g in async_generator:
         for x in g:
             yield x
 
 
 def afirst(*funcs: Callable, exception_type: Type[Exception]):
     """Runs given `funcs` serially until getting a succefull result.
     Returns the result of the first function that runs on `x` without raising `exception_type`.
     If all given function raise e`xception_type`, `exception_type` will be raised.
 
     >>> async def araise(x):
-    >>>     raise ValueError
-    >>> run_sync(afirst(araise, lambda x: x*x, exception_type=ValueError)(3))
+    ...     raise ValueError
+    ... run_sync(afirst(araise, lambda x: x*x, exception_type=ValueError)(3))
     9
     """
 
     async def afirst_inner(x: Any):
         for f in funcs:
             try:
                 return await async_functions.to_awaitable(f(x))
```

### Comparing `gamla-98/gamla/functional_generic.py` & `gamla-99/gamla/functional_generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,31 +40,29 @@
         compose
         pipe
     """
     return compose(*reversed(funcs))
 
 
 def curried_map(f):
-    """
-    Constructs a function that maps elements of a given iterable using the given function.
+    """Constructs a function that maps elements of a given iterable using the given function.
 
     Returns an async function iff `f` is async, else returns a sync function.
 
     >>> inc = lambda i: i + 1
     >>> curried_map(inc)([3, 4, 5])
     [4, 5, 6]
     """
     if asyncio.iscoroutinefunction(f):
         return async_functions.map(f)
     return sync.map(f)
 
 
 def curried_to_binary(f):
-    """
-    Constructs a function from a given higher order function and returns its first order counterpart.
+    """Constructs a function from a given higher order function and returns its first order counterpart.
     The given higher order function, `f` is must be a unary function
     Returns an async function iff `f` is async, else returns a sync function.
 
     >>> inc = lambda i: i + 1
     >>> f = curried_to_binary(curried_map)
     >>> f(inc, [1, 2, 3])
     [2, 3, 4]
@@ -135,16 +133,15 @@
         juxt
         compose_left
     """
     return compose_left(juxt(*incoming), star(f))
 
 
 def after(f1):
-    """
-    Second-order composition of `f1` over `f2`.
+    """Second-order composition of `f1` over `f2`.
 
     A 'delayed' pipeline, i.e return a function that, given f2, will wait for f2's arguments, and when given, will return f1(f2(args)).
     >>> allmap = gamla.compose_left(gamla.map, gamla.after(all))
     >>> allmap(lambda x: x == 1)([1, 2, 3])
     False
     """
 
@@ -209,40 +206,40 @@
 
     def juxt(*args, **kwargs):
         return tuple(func(*args, **kwargs) for func in funcs)
 
     return juxt
 
 
-#:  Pass a value through a list of functions, return `True` iff all functions returned `True`-ish values.
+#: Pass a value through a list of functions, return `True` iff all functions returned `True`-ish values.
 #:
-#:    >>> f = alljuxt(gamla.identity, gamla.greater_than(1), gamla.greater_than(10))
-#:    >>> f(100)
-#:    True
-#:    >>> f(10)
-#:    False
+#: >>> f = alljuxt(gamla.identity, gamla.greater_than(1), gamla.greater_than(10))
+#: >>> f(100)
+#: True
+#: >>> f(10)
+#: False
 alljuxt = compose(after(all), lazyjuxt)
 
-#:  Pass a value through a list of functions, return `True` if at least one function returned a `True`-ish value.
+#: Pass a value through a list of functions, return `True` if at least one function returned a `True`-ish value.
 #   Note: evaluation is lazy, i.e. returns on first `True`.
 #:
-#:    >>> f = anyjuxt(gamla.identity, gamla.greater_than(1), gamla.greater_than(10))
-#:    >>> f(100)
-#:    True
-#:    >>> f(10)
-#:    True
-#:    >>> f(0)
-#:    False
+#: >>> f = anyjuxt(gamla.identity, gamla.greater_than(1), gamla.greater_than(10))
+#: >>> f(100)
+#: True
+#: >>> f(10)
+#: True
+#: >>> f(0)
+#: False
 anyjuxt = compose(after(any), lazyjuxt)
 
-#:  Create a function that calls the supplied functions, and chains the results.
+#: Create a function that calls the supplied functions, and chains the results.
 #: Assumes the supplied functions return Iterables.
-#:    >>> f = juxtcat(range,range)
-#:    >>> tuple(f(5))
-#:    (0 ,1 ,2 ,3 ,4 ,0 ,1 ,2 ,3 ,4)
+#: >>> f = juxtcat(range,range)
+#: >>> tuple(f(5))
+#: (0 ,1 ,2 ,3 ,4 ,0 ,1 ,2 ,3 ,4)
 juxtcat = compose(after(itertools.chain.from_iterable), lazyjuxt)
 
 
 def ternary(condition, f_true, f_false):
     """Returns a function that computes `f_true` or `f_false` according to
     `condition`. The functions are applied with the same input.
     The returned function will be an async function if at least one of the given
@@ -349,64 +346,64 @@
     if _any_is_async(funcs):
         return async_functions.compose(*reversed(funcs))(val)
     for f in funcs:
         val = f(val)
     return val
 
 
-#:  Map an iterable using a function, return `True` iff all mapped values are `True`-ish.
-#:    >>> f = allmap(lambda x: x % 2 == 0)
-#:    >>> f([1, 2, 3, 4, 5])
-#:    False
-#:    >>> f([2, 4, 6, 8, 10])
-#:    True
+#: Map an iterable using a function, return `True` iff all mapped values are `True`-ish.
+#: >>> f = allmap(lambda x: x % 2 == 0)
+#: >>> f([1, 2, 3, 4, 5])
+#: False
+#: >>> f([2, 4, 6, 8, 10])
+#: True
 allmap = compose(after(all), curried_map)
 
-#:  Map an iterable using a function, return `True` if at least one mapped value is `True`-ish.
-#:  Note: evaluation is lazy, i.e. returns on first `True`.
-#:    >>> f = anymap(lambda x: x % 2 == 0)
-#:    >>> f([1, 2, 3, 4, 5])
-#:    True
-#:    >>> f([1, 3, 5, 7, 9])
-#:    False
+#: Map an iterable using a function, return `True` if at least one mapped value is `True`-ish.
+#: Note: evaluation is lazy, i.e. returns on first `True`.
+#: >>> f = anymap(lambda x: x % 2 == 0)
+#: >>> f([1, 2, 3, 4, 5])
+#: True
+#: >>> f([1, 3, 5, 7, 9])
+#: False
 anymap = compose(after(any), curried_map)
 
 #: Constructs a function that applies the given function to items of a given dictionary.
 #: Returns an async function iff the filter function is async, else returns a sync function.
 #:
-#:    >>> f = itemmap(gamla.star(lambda key, val: (key, val + key)))
-#:    >>> f({1: 2, 2: 3})
-#:    {1: 3, 2: 5}
+#: >>> f = itemmap(gamla.star(lambda key, val: (key, val + key)))
+#: >>> f({1: 2, 2: 3})
+#: {1: 3, 2: 5}
 itemmap = compose(after(dict), before(dict.items), curried_map)
 
-#:  Creates a function that maps supplied mapper over the keys of a dict.
+#: Creates a function that maps supplied mapper over the keys of a dict.
 #:
-#:    >>> f = keymap(lambda k: k + 1)
-#:    >>> f({1:"a",2:"b",3:"c",4:"d"})
-#:    {
-#:      2: "a",
-#:      3: "b",
-#:      4: "c",
-#:      5: "d"
-#:    }
+#: >>> f = keymap(lambda k: k + 1)
+#: >>> f({1:"a",2:"b",3:"c",4:"d"})
+#: {
+#:   2: "a",
+#:   3: "b",
+#:   4: "c",
+#:   5: "d"
+#: }
 keymap = compose(
     itemmap,
     lambda f: juxt(f, functional.second),
     before(functional.head),
 )
 
 #: Creates a function then maps the supplied mapper over the values of a dict.
 #:
-#:  >>> f = valmap(gamla.add(1))
-#:  >>> f({ "a": 1, "b": 2, "c": 3 })
-#:  {
-#:    "a": 2
-#:    "b": 3
-#:    "c": 4
-#:  }
+#: >>> f = valmap(gamla.add(1))
+#: >>> f({ "a": 1, "b": 2, "c": 3 })
+#: {
+#: "a": 2
+#: "b": 3
+#: "c": 4
+#: }
 valmap = compose(
     itemmap,
     lambda f: juxt(functional.head, f),
     before(functional.second),
 )
 
 
@@ -429,82 +426,82 @@
     """
     return juxt(functional.identity, f)
 
 
 #: Constructs a function that filters elements of a given iterable for which function returns true.
 #: Returns an async function iff the filter function is async, else returns a sync function.
 #:
-#:    >>> f = curried_filter(gamla.greater_than(10))
-#:    >>> f([1, 2, 3, 11, 12, 13])
-#:    [11, 12, 13]
+#: >>> f = curried_filter(gamla.greater_than(10))
+#: >>> f([1, 2, 3, 11, 12, 13])
+#: [11, 12, 13]
 curried_filter = compose(
     after(
         compose(
             functional.curried_map_sync(functional.second),
             sync.filter(functional.head),
         ),
     ),
     curried_map,
     pair_with,
 )
 
 #: Constructs a function that filters items of a given dictionary for which function returns true.
 #: Returns an async function iff the filter function is async, else returns a sync function.
 #:
-#:    >>> f = itemfilter(
-#:        alljuxt(
-#:            compose_left(gamla.head, gamla.contains("gamla")),
-#:            compose_left(gamla.second, gamla.greater_than(10)),
-#:        )
-#:    )
-#:    >>> f({"gamla": 11, "gaml": 9, "f":12})
-#:    {'gamla': 11}
+#: >>> f = itemfilter(
+#: ...     alljuxt(
+#: ...         compose_left(gamla.head, gamla.contains("gamla")),
+#: ...         compose_left(gamla.second, gamla.greater_than(10)),
+#: ...     )
+#: ... )
+#: >>> f({"gamla": 11, "gaml": 9, "f":12})
+#: {'gamla': 11}
 itemfilter = compose(after(dict), before(dict.items), curried_filter)
 
-#:  Create a function that filters a dict using a predicate over keys.
+#: Create a function that filters a dict using a predicate over keys.
 #:
-#:    >>> f = keyfilter(lambda k: k > 2)
-#:    >>> f({1:"a",2:"b",3:"c",4:"d"})
-#:    {
-#:      3: "c",
-#:      4: "d"
-#:    }
+#: >>> f = keyfilter(lambda k: k > 2)
+#: >>> f({1:"a",2:"b",3:"c",4:"d"})
+#: {
+#:   3: "c",
+#:   4: "d"
+#: }
 keyfilter = compose(
     itemfilter,
     before(functional.head),
 )
 
-#:  Create a function that filters a dict using a predicate over values.
+#: Create a function that filters a dict using a predicate over values.
 #:
-#:    >>> f = valefilter(lambda k: k > 2)
-#:    >>> f({"a": 1, "b": 2, "c": 3, "d": 4})
-#:    {
-#:      "c": 3,
-#:      "d": 4
-#:    }
+#: >>> f = valefilter(lambda k: k > 2)
+#: >>> f({"a": 1, "b": 2, "c": 3, "d": 4})
+#: {
+#:   "c": 3,
+#:   "d": 4
+#: }
 valfilter = compose(
     itemfilter,
     before(functional.second),
 )
 
 #: Complement of a boolean function.
 #:
-#:    >>> f = complement(gamla.greater_than(5))
-#:    >>> f(10)
-#:    False
-#:    >>> f(1)
-#:    True
+#: >>> f = complement(gamla.greater_than(5))
+#: >>> f(10)
+#: False
+#: >>> f(1)
+#: True
 complement = after(operator.not_)
 
 #: Constructs a function that removes elements of a given iterable for which function returns true.
 #: Returns an async function iff the filter function is async, else returns a sync function.
 #:
-#:    >>> f = remove(gamla.greater_than(10))
-#:    >>> tuple(f([1, 2, 3, 11, 12, 13]))
-#:    (1, 2, 3)
+#: >>> f = remove(gamla.greater_than(10))
+#: >>> tuple(f([1, 2, 3, 11, 12, 13]))
+#: (1, 2, 3)
 remove = compose(curried_filter, complement)
 
 
 class NoConditionMatched(Exception):
     pass
 
 
@@ -551,22 +548,22 @@
     `NoConditionMatched`
     """
     predicates = tuple(map(functional.head, predicates_and_mappers))
     mappers = tuple(map(functional.second, predicates_and_mappers))
     return _case(predicates, mappers)
 
 
-#:  Applies functions to values according to predicates given in a dict. Raises `gamla.functional_generic.NoConditionMatched` if no predicate matches.
-#:    >>> f = case_dict({gamla.less_than(10): gamla.identity, gamla.greater_than(10): gamla.add(100)})
-#:    >>> f(5)
-#:    5
-#:    >>> f(15)
-#:    115
-#:    >>> f(10)
-#:    `NoConditionMatched`
+#: Applies functions to values according to predicates given in a dict. Raises `gamla.functional_generic.NoConditionMatched` if no predicate matches.
+#: >>> f = case_dict({gamla.less_than(10): gamla.identity, gamla.greater_than(10): gamla.add(100)})
+#: >>> f(5)
+#: 5
+#: >>> f(15)
+#: 115
+#: >>> f(10)
+#: `NoConditionMatched`
 case_dict = compose_left(dict.items, tuple, case)
 
 
 async def _await_dict(value):
     if isinstance(value, dict) or isinstance(value, data.frozendict):
         return await pipe(
             value,
@@ -667,17 +664,17 @@
     >>> seq = map(gamla.identity, [1, 2, 3, 4, 5])
     >>> f(seq)
     (15, 5)
     """
     return compose_left(iter, lambda it: itertools.tee(it, len(funcs)), stack(funcs))
 
 
-#:  Average of an iterable. If the sequence is empty, returns 0.
-#:    >>> average([1,2,3])
-#:    2.0
+#: Average of an iterable. If the sequence is empty, returns 0.
+#: >>> average([1,2,3])
+#: 2.0
 average = compose_left(
     bifurcate(sum, functional.count),
     excepts_decorator.excepts(
         ZeroDivisionError,
         functional.just(0),
         sync.star(operator.truediv),
     ),
@@ -746,19 +743,19 @@
     return reduce_curried(reduce_keeping_history, (initial_value,))
 
 
 #: Constructs a function that will return the first element of an iterable,
 #: that returns True when used with the the given function. If no element
 #: in the iterable returns True, None is returned.
 #:
-#:    >>> f = find(gamla.greater_than(10))
-#:    >>> f([1, 2, 3, 11, 12, 13])
-#:    11
-#:    >>> f([1, 2, 3])
-#:    None
+#: >>> f = find(gamla.greater_than(10))
+#: >>> f([1, 2, 3, 11, 12, 13])
+#: 11
+#: >>> f([1, 2, 3])
+#: None
 find = compose(
     after(
         excepts_decorator.excepts(
             StopIteration,
             functional.just(None),
             functional.head,
         ),
@@ -767,22 +764,22 @@
 )
 
 
 #: Constructs a function that will return the index of an element of an iterable,
 #: that returns True when used with the the given function. If no element
 #  in the iterable returns True, -1 is returned.
 #:
-#:    >>> f = find(gamla.greater_than(10))
-#:    >>> f([1, 2, 3, 11, 12, 13])
-#:    11
-#:    >>> f([1, 2, 3])
-#:    -1
+#: >>> f = find(gamla.greater_than(10))
+#: >>> f([1, 2, 3, 11, 12, 13])
+#: 11
+#: >>> f([1, 2, 3])
+#: -1
 #:
 #: See Also:
-#:   - find
+#:  - find
 find_index = compose_left(
     before(functional.second),
     find,
     before(enumerate),
     after(ternary(functional.equals(None), functional.just(-1), functional.head)),
 )
 
@@ -873,23 +870,22 @@
             f(x)
             return x
 
     return do
 
 
 def count_by_many(f: Callable[[Any], Iterable]) -> Dict[Any, int]:
-    """
-    Count elements of a collection by a function `f`.
-    Return a mapping `{y: len({x s.t. key(x) = y})}.`
+    """Counts elements of a collection by a key function `f`.
 
     >>> count_by_many(
-        gamla.juxt(
-            functional.head,
-             gamla.last
-        ))(["aa", "ab", "ac", "bc"])
+    ...     gamla.juxt(
+    ...         functional.head,
+    ...         gamla.last,
+    ...     )
+    ... )(["aa", "ab", "ac", "bc"])
     {'a': 3, 'b': 2, 'c': 2}
     """
     return functional.groupby_many_reduce(
         f,
         lambda x, _: x + 1 if x else 1,
     )
```

### Comparing `gamla-98/gamla/functional_test.py` & `gamla-99/gamla/functional_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/graph.py` & `gamla-99/gamla/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,49 +99,49 @@
         functional.head,
         graph_traverse(source=(source, 0), get_neighbors=get_neighbors_limiting_radius),
     )
 
 
 #: Gets a sequence of edges and returns a graph made of these edges.
 #:
-#:  >>> graph.edges_to_graph([(1,2), (2, 3), (3, 1), (3, 2)])
-#:  {1: frozenset({2}), 2: frozenset({3}), 3: frozenset({1, 2})}
+#: >>> graph.edges_to_graph([(1,2), (2, 3), (3, 1), (3, 2)])
+#: {1: frozenset({2}), 2: frozenset({3}), 3: frozenset({1, 2})}
 edges_to_graph = functional_generic.compose(
     functional_generic.sync.valmap(
         functional_generic.sync.compose(
             frozenset,
             functional_generic.sync.map(functional.second),
         ),
     ),
     sync.groupby(functional.head),
 )
 #: Gets a graph and returns an iterator of all edges in it.
 #:
-#:  >>> list(graph_to_edges({'1': ['2', '3'], '2': ['3'], '3': ['4'], '4': []}))
-#:  [('1', '2'), ('1', '3'), ('2', '3'), ('3', '4')]
+#: >>> list(graph_to_edges({'1': ['2', '3'], '2': ['3'], '3': ['4'], '4': []}))
+#: [('1', '2'), ('1', '3'), ('2', '3'), ('3', '4')]
 graph_to_edges = functional_generic.compose_left(
     sync.keymap(functional.wrap_tuple),
     dict.items,
     sync.mapcat(sync.star(itertools.product)),
 )
 
 #: Gets a graph and returns the graph with its edges reversed
 #:
-#:  >>> reverse_graph({'1': ['2', '3'], '2': ['3'], '3': ['4'], '4': []})
-#:  {'2': frozenset({'1'}), '3': frozenset({'1', '2'}), '4': frozenset({'3'})}
+#: >>> reverse_graph({'1': ['2', '3'], '2': ['3'], '3': ['4'], '4': []})
+#: {'2': frozenset({'1'}), '3': frozenset({'1', '2'}), '4': frozenset({'3'})}
 reverse_graph = functional_generic.compose_left(
     graph_to_edges,
     functional_generic.curried_map(functional_generic.compose_left(reversed, tuple)),
     edges_to_graph,
 )
 
 #: Gets a sequence of nodes (cliques) and returns the bidirectional graph they represent
 #:
-#:  >>> cliques_to_graph([{1, 2}, {3, 4}])
-#:  {1: frozenset({2}), 2: frozenset({1}), 3: frozenset({4}), 4: frozenset({3})}
+#: >>> cliques_to_graph([{1, 2}, {3, 4}])
+#: {1: frozenset({2}), 2: frozenset({1}), 3: frozenset({4}), 4: frozenset({3})}
 cliques_to_graph = functional_generic.compose_left(
     sync.mapcat(lambda clique: itertools.permutations(clique, r=2)),
     edges_to_graph,
 )
 
 
 def get_connectivity_components(graph: Dict) -> Iterable[FrozenSet]:
@@ -239,17 +239,18 @@
 _non_sources = sync.compose_left(
     dict.values,
     functional_generic.concat,
     frozenset,
 )
 
 
-#: Gets a directional graph and returns its sources.
-#:
-#:  >>> find_sources({'1': ['2', '3'], '2': ['3'], '3': [], '4': []})
-#:  frozenset({'1', '4'})
 def find_sources(graph: Dict) -> FrozenSet:
+    """Gets a directional graph and returns its sources.
+
+    >>> find_sources({'1': ['2', '3'], '2': ['3'], '3': [], '4': []})
+    frozenset({'1', '4'})
+    """
     return sync.pipe(
         graph,
         sync.remove(functional.contains(_non_sources(graph))),
         frozenset,
     )
```

### Comparing `gamla-98/gamla/graph_async.py` & `gamla-99/gamla/graph_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, AsyncGenerator, Callable, Hashable, Set, Text, Tuple
+from typing import Any, AsyncGenerator, Callable, Hashable, Text, Tuple
 
 from gamla import currying, functional, functional_generic
 
 
 @currying.curry
 async def agraph_traverse(
     source: Any,
@@ -99,41 +99,44 @@
     pass
 
 
 @currying.curry
 async def reduce_graph_async(
     reducer: Callable[[Tuple[Any, ...], Hashable], Any],
     get_neighbors: Callable,
-    visited: Set,
+    remember: Callable[[Hashable], None],
+    is_seen: Callable[[Hashable], bool],
     current: Hashable,
 ):
     """Reduces a graph from some starting point using async functions.
 
+    >>> set_instance = set()
     >>> await reduce_graph_async(
     ...     lambda children, current: sum(children) + current,
     ...     functional_generic.compose_left(
     ...         dict_utils.dict_to_getter_with_default(
     ...             (),
     ...             {1: (1, 2, 3, 5), 2: (4,), 3: (1, 2)}),
     ...         async_functions.to_awaitable,
     ...     ),
-    ...     set(),
+    ...     set_instance.add,
+    ...     contains(set_instance)
     ...     1,
     ... )
     15"""
-    if current in visited:
+    if is_seen(current):
         return _IgnoreChild()
     # Since we may reach a node from two different branches, at the same time,
     # we have to broadcast to the other branch that we've reached this node, this
     # can't be done in an immutable fashion.
-    visited.add(current)
+    remember(current)
     return await functional_generic.pipe(
         current,
         get_neighbors,
         functional_generic.curried_map(
-            reduce_graph_async(reducer, get_neighbors, visited),
+            reduce_graph_async(reducer, get_neighbors, remember, is_seen),
         ),
         functional_generic.remove(functional.is_instance(_IgnoreChild)),
         tuple,
         functional_generic.pair_right(functional.just(current)),
         functional_generic.star(reducer),
     )
```

### Comparing `gamla-98/gamla/graph_async_test.py` & `gamla-99/gamla/graph_async_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import pytest
 
-from gamla import async_functions, dict_utils, functional_generic, graph_async
+from gamla import (
+    async_functions,
+    dict_utils,
+    functional,
+    functional_generic,
+    graph_async,
+)
 
 pytestmark = pytest.mark.asyncio
 
 
 def _reduce_max(children, current):
     return max(children + (current,))
 
@@ -12,55 +18,61 @@
 _get_neighbors = dict_utils.dict_to_getter_with_default(
     (),
     {1: (1, 2, 3, 5), 2: (4,), 3: (1, 2)},
 )
 
 
 async def test_reduce_graph_async1():
+    set_instance = set()
     assert (
         await graph_async.reduce_graph_async(
             _reduce_max,
             functional_generic.compose_left(
                 _get_neighbors,
                 async_functions.to_awaitable,
             ),
-            set(),
+            set_instance.add,
+            functional.contains(set_instance),
             1,
         )
         == 5
     )
 
 
 async def test_reduce_graph_async2():
+    set_instance = set()
     assert (
         await graph_async.reduce_graph_async(
             lambda children, current: sum(children) + current,
             functional_generic.compose_left(
                 dict_utils.dict_to_getter_with_default(
                     (),
                     {1: (1, 2, 3, 5), 2: (4,), 3: (1, 2)},
                 ),
                 async_functions.to_awaitable,
             ),
-            set(),
+            set_instance.add,
+            functional.contains(set_instance),
             1,
         )
         == 15
     )
 
 
 async def test_reduce_graph_async_reducer():
+    set_instance = set()
     assert (
         await graph_async.reduce_graph_async(
             functional_generic.compose_left(
                 _reduce_max,
                 async_functions.to_awaitable,
             ),
             functional_generic.compose_left(
                 _get_neighbors,
                 async_functions.to_awaitable,
             ),
-            set(),
+            set_instance.add,
+            functional.contains(set_instance),
             1,
         )
         == 5
     )
```

### Comparing `gamla-98/gamla/graph_test.py` & `gamla-99/gamla/graph_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/higher_order.py` & `gamla-99/gamla/higher_order.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/higher_order_test.py` & `gamla-99/gamla/higher_order_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/io_utils.py` & `gamla-99/gamla/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,21 +237,21 @@
             timeout=timeout,
         )
 
 
 #: Performs an http POST request of json data with specified headers.
 #: Expects the payload to be a json serializable object and the headers to be a dictionary.
 #:
-#:    >>> response = post_json_with_extra_headers_async({"username": "First Last", 30, "https://www.someurl.com/post_data", { "name": "Danny" })
+#: >>> response = post_json_with_extra_headers_async({"username": "First Last", 30, "https://www.someurl.com/post_data", { "name": "Danny" })
 post_json_with_extra_headers_async = post_json_with_extra_headers_and_params_async({})
 
 #: Performs an http POST request of json data.
 #: Expects the payload to be a json serializable object.
 #:
-#:    >>> response = post_json_async(30, "https://www.someurl.com/post_data", { "name": "Danny" })
+#: >>> response = post_json_async(30, "https://www.someurl.com/post_data", { "name": "Danny" })
 post_json_async = post_json_with_extra_headers_and_params_async({}, {})
 
 
 @currying.curry
 def retry(
     exception: Union[Exception, Tuple[Exception, ...]],
     times: int,
```

### Comparing `gamla-98/gamla/io_utils_test.py` & `gamla-99/gamla/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/optimized/async_functions.py` & `gamla-99/gamla/optimized/async_functions.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/optimized/sync.py` & `gamla-99/gamla/optimized/sync.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/string_utils.py` & `gamla-99/gamla/string_utils.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/transducer.py` & `gamla-99/gamla/transducer.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,41 +31,39 @@
 
 def _replace_index(the_tuple, index, value):
     return (*the_tuple[:index], value, *the_tuple[index + 1 :])
 
 
 #: Combines transducers in a `dict` into a transducer that produces a `dict`.
 #: >>> transducer.transduce(
-#:     transducer.apply_spec(  # This will combine the inner stuff into one new transducer.
-#:         {
-#:             "incremented": _increment(_append_to_tuple),  # This is a transducer.
-#:             "sum": lambda s, x: x + s,  # This is another transducer.
-#:         },
-#:     ),
-#:     lambda s, _: s,
-#:     {"incremented": (), "sum": 0},
-#:     [1, 2, 3],
-#: )
+#: ...     transducer.apply_spec({  # This will combine the inner stuff into one new transducer.
+#: ...         "incremented": _increment(_append_to_tuple),  # This is a transducer.
+#: ...         "sum": lambda s, x: x + s,  # This is another transducer.
+#: ...     }),
+#: ...     lambda s, _: s,
+#: ...     {"incremented": (), "sum": 0},
+#: ...     [1, 2, 3],
+#: ... )
 #: {"incremented": (2, 3, 4), "sum": 6}
 apply_spec = functional_generic.compose_left(
     dict.items,
     sync.map(sync.star(_transform_by_key(toolz.assoc))),
     sync.star(functional_generic.compose),
 )
 
 #: Combines transducers in a `tuple` into a transducer that produces a `tuple`.
-#: transducer.transduce(
-#:     transducer.juxt(  # This will combine the inner stuff into one new transducer.
-#:         _increment(_append_to_tuple),  # This is a transducer.
-#:         lambda s, x: x + s,  # This is another transducer.
-#:     ),
-#:     lambda s, _: s,
-#:     [(), 0],
-#:     [1, 2, 3],
-#: )
+#: >>> transducer.transduce(
+#: ...     transducer.juxt(  # This will combine the inner stuff into one new transducer.
+#: ...         _increment(_append_to_tuple),  # This is a transducer.
+#: ...         lambda s, x: x + s,  # This is another transducer.
+#: ...     ),
+#: ...    lambda s, _: s,
+#: ...    [(), 0],
+#: ...    [1, 2, 3],
+#: ... )
 #: ((2, 3, 4), 6)
 juxt = functional_generic.compose_left(
     functional.pack,
     enumerate,
     sync.map(sync.star(_transform_by_key(_replace_index))),
     sync.star(functional_generic.compose),
 )
```

### Comparing `gamla-98/gamla/transducer_test.py` & `gamla-99/gamla/transducer_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/tree.py` & `gamla-99/gamla/tree.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/tree_test.py` & `gamla-99/gamla/tree_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/url_utils.py` & `gamla-99/gamla/url_utils.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla/url_utils_test.py` & `gamla-99/gamla/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `gamla-98/gamla.egg-info/PKG-INFO` & `gamla-99/gamla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamla
-Version: 98
+Version: 99
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gamla-98/gamla.egg-info/SOURCES.txt` & `gamla-99/gamla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gamla-98/setup.py` & `gamla-99/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     _LONG_DESCRIPTION = fh.read()
 
 
 setuptools.setup(
     name="gamla",
-    version="98",
+    version="99",
     long_description=_LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=setuptools.find_namespace_packages(),
     install_requires=[
         "async-timeout",
         "dataclasses_json",
         "heapq_max",
```

