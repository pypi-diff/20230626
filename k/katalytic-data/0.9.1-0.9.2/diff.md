# Comparing `tmp/katalytic-data-0.9.1.tar.gz` & `tmp/katalytic-data-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.9.1.tar", last modified: Sat May 20 16:31:58 2023, max compression
+gzip compressed data, was "katalytic-data-0.9.2.tar", last modified: Mon May 22 18:25:24 2023, max compression
```

## Comparing `katalytic-data-0.9.1.tar` & `katalytic-data-0.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.9.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.9.1/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.9.1/.gitlab-ci.yml
--rw-r--r--   0        0        0    13511 2023-05-20 16:31:54.839563 katalytic-data-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     1866 2023-05-14 08:37:30.818379 katalytic-data-0.9.1/README.md
--rw-r--r--   0        0        0     1236 2023-05-20 16:31:54.839563 katalytic-data-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    27246 2023-05-20 16:27:22.878218 katalytic-data-0.9.1/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.9.1/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.9.1/tests/test_checks.py
--rw-r--r--   0        0        0    49962 2023-05-20 16:28:10.046455 katalytic-data-0.9.1/tests/test_data.py
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 katalytic-data-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.9.2/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.9.2/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.9.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0    13860 2023-05-22 18:25:19.619197 katalytic-data-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1866 2023-05-14 08:37:30.818379 katalytic-data-0.9.2/README.md
+-rw-r--r--   0        0        0     1236 2023-05-22 18:25:19.599197 katalytic-data-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    58491 2023-05-22 18:11:14.231037 katalytic-data-0.9.2/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0    20303 2023-05-22 17:06:11.712093 katalytic-data-0.9.2/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.9.2/tests/test_checks.py
+-rw-r--r--   0        0        0    50206 2023-05-22 18:12:09.923315 katalytic-data-0.9.2/tests/test_data.py
+-rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 katalytic-data-0.9.2/PKG-INFO
```

### Comparing `katalytic-data-0.9.1/.gitignore` & `katalytic-data-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.1/.gitlab-ci.yml` & `katalytic-data-0.9.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.1/CHANGELOG.md` & `katalytic-data-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.9.2 (2023-05-22)
+### fix
+- [[`be05243`](https://gitlab.com/katalytic/katalytic-data/commit/be0524340348c5424c99d1e205eac3c5714f164f)] get_version() raises error when running doctest
+### refactor
+- [[`080d2d8`](https://gitlab.com/katalytic/katalytic-data/commit/080d2d88ee69534e65da316cd9485f36afd2e0d6)] rename "key" parameter to "condition"
+
+
 ## 0.9.1 (2023-05-20)
 ### fix
 - [[`131e3ad`](https://gitlab.com/katalytic/katalytic-data/commit/131e3ad13db07a9e23e33e8d9c66df73a65a95f0)] use `[True, False]` instead of just `False` in the `_types` dict
 
 
 ## 0.9.0 (2023-05-06)
 ### feat
```

### Comparing `katalytic-data-0.9.1/LICENSE.txt` & `katalytic-data-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.1/README.md` & `katalytic-data-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.1/pyproject.toml` & `katalytic-data-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.9.1"
+version = "0.9.2"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.9.1/tests/test_checks.py` & `katalytic-data-0.9.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.1/tests/test_data.py` & `katalytic-data-0.9.2/tests/test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from _decimal import Decimal
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
-from katalytic.data.checks import is_generator, is_generator_function, is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
+from katalytic.data.checks import is_generator_function, is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
     _C, _C_obj, _callables, _collections, _dict_views, _flatten, _function, _functions, _generators, _iterables, _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
     map_recursive, one, pick_all, pick_all_besides, pick_any, pop_max, pop_max_by_dict_key, pop_max_by_dict_value, pop_min, pop_min_by_dict_key, pop_min_by_dict_value, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
     as_dict_of_lists, sort_recursive, swap_keys_and_values, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
@@ -224,27 +224,27 @@
         assert as_list_of_lists(data) == expected
 
 
 class Test_first:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            first([], key=wrong_type)
+            first([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             first(set())
 
     @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert first(data) is None
 
-    def test_no_first_with_key(self):
+    def test_no_first_with_condition(self):
         data = range(10)
-        assert first(data, key=lambda x: x > 50) is None
+        assert first(data, condition=lambda x: x > 50) is None
 
     @pytest.mark.parametrize('data, expected', [
         (range(10), 0),
         ([False, None, 5, True], False),
         (['', 0, None, False], ''),
         (map(lambda x: x+1, range(0, 100, 10)), 1),
     ])
@@ -252,31 +252,31 @@
         assert first(data) == expected
 
 
 class Test_first_with_idx:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            first_with_idx([], key=wrong_type)
+            first_with_idx([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             first_with_idx(set())
 
     @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert first_with_idx(data) is None
 
-    def test_no_first_with_key(self):
+    def test_no_first_with_condition(self):
         data = range(10)
-        assert first_with_idx(data, key=lambda x: x > 50) is None
+        assert first_with_idx(data, condition=lambda x: x > 50) is None
 
     def test_first_with_key(self):
         data = range(5, 15)
-        assert first_with_idx(data, key=lambda x: x >= 10) == (5, 10)
+        assert first_with_idx(data, condition=lambda x: x >= 10) == (5, 10)
 
     @pytest.mark.parametrize('data, expected', [
         (range(10), (0, 0)),
         ([False, None, 5, True], (0, False)),
         (['', 0, None, False], (0, '')),
         (map(lambda x: x+1, range(0, 100, 10)), (0, 1)),
     ])
@@ -284,27 +284,27 @@
         assert first_with_idx(data) == expected
 
 
 class Test_last:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            last([], key=wrong_type)
+            last([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             last(set())
 
     @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert last(data) is None
 
-    def test_no_last_with_key(self):
+    def test_no_last_with_condition(self):
         data = range(10)
-        assert last(data, key=lambda x: x > 50) is None
+        assert last(data, condition=lambda x: x > 50) is None
 
     @pytest.mark.parametrize('data, expected', [
         (range(10), 9),
         ([False, None, 5, True], True),
         ([False, None, True, 5], 5),
         (['', 0, None, False], False),
         (map(lambda x: x+1, range(0, 100, 10)), 91),
@@ -313,31 +313,31 @@
         assert last(data) == expected
 
 
 class Test_last_with_idx:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            last_with_idx([], key=wrong_type)
+            last_with_idx([], condition=wrong_type)
 
     def test_sets_are_not_allowed(self):
         with pytest.raises(TypeError):
             last_with_idx(set())
 
     @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, ()])
     def test_empty(self, data):
         assert last_with_idx(data) is None
 
-    def test_no_last_with_key(self):
+    def test_no_last_with_condition(self):
         data = range(10)
-        assert last_with_idx(data, key=lambda x: x > 50) is None
+        assert last_with_idx(data, condition=lambda x: x > 50) is None
 
     def test_last_with_key(self):
         data = range(5, 15)
-        assert last_with_idx(data, key=lambda x: x <= 13) == (8, 13)
+        assert last_with_idx(data, condition=lambda x: x <= 13) == (8, 13)
 
     @pytest.mark.parametrize('data, expected', [
         (range(7, 10), (2, 9)),
         ([False, None, 5, True], (3, True)),
         (['', 0, None, False], (3, False)),
         (map(lambda x: x+1, range(0, 100, 10)), (9, 91)),
     ])
@@ -533,32 +533,32 @@
         assert map_recursive(lambda x: x + 1, data, condition=_is_num, on_dict_keys=True) == expected
 
 
 class Test_one:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_not_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            one([], key=wrong_type)
+            one([], condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
     def test_key_not_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             one(wrong_type)
 
     @pytest.mark.parametrize('data', [iter([]), map(lambda x: x, []), [], {}, (), set()])
     def test_empty(self, data):
         assert one(data) is None
 
     @pytest.mark.parametrize('data', [{'', 0, None, False}, ['', 0, None, False]])
     def test_no_one(self, data):
         assert one(data) == ''
 
-    def test_no_one_with_key(self):
+    def test_no_one_with_condition(self):
         data = range(10)
-        assert one(data, key=lambda x: x > 50) is None
+        assert one(data, condition=lambda x: x > 50) is None
 
     @pytest.mark.parametrize('data, expected', [
         (range(10), 0),
         ([False, None, 5, True], False),
         ([False, None, True, 5], False),
         (map(lambda x: x+1, range(0, 100, 10)), 1),
     ])
@@ -582,15 +582,15 @@
     def test_dict(self):
         with pytest.raises(TypeError):
             pop_min({})
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_min([1], key=wrong_type)
+            pop_min([1], condition=wrong_type)
 
     @pytest.mark.parametrize('data', all_types('iterables'))
     def test_empty(self, data):
         if isinstance(data, dict):
             return
         elif is_generator_function(data):
             data = data()
@@ -609,15 +609,15 @@
 
     @pytest.mark.parametrize('data, expected', [
         ([3,2,1,4], (4, [3,2,1])),
         ((0,-1,3,4), (4, (0,-1,3))),
         (map(float, (0,3,-4,5)), (5, [0,3,-4])),
     ])
     def test_with_key(self, data, expected):
-        assert pop_min(data, key=lambda x: -x) == expected
+        assert pop_min(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max:
     @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max(wrong_type)
@@ -625,15 +625,15 @@
     def test_dict(self):
         with pytest.raises(TypeError):
             pop_max({})
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_max([1], key=wrong_type)
+            pop_max([1], condition=wrong_type)
 
     @pytest.mark.parametrize('data', all_types('iterables'))
     def test_empty(self, data):
         if isinstance(data, dict):
             return
         elif is_generator_function(data):
             data = data()
@@ -652,27 +652,27 @@
 
     @pytest.mark.parametrize('data, expected', [
         ([3,2,1,4], (1, [3,2,4])),
         ({0,-1,3,4}, (-1, {0,3,4})),
         (map(float, (0,3,-4,5)), (-4, [0,3,5])),
     ])
     def test_with_key(self, data, expected):
-        assert pop_max(data, key=lambda x: -x) == expected
+        assert pop_max(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max_by_dict_key:
     @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max_by_dict_key(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_max_by_dict_key({'1': 1}, key=wrong_type)
+            pop_max_by_dict_key({'1': 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_max_by_dict_key({})
 
     @pytest.mark.parametrize('data, expected', [
         ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
@@ -682,27 +682,27 @@
         assert pop_max_by_dict_key(data) == expected
 
     @pytest.mark.parametrize('data, expected', [
         ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((1, 'c'), {3: 'a', 2: 'b', 4: 'd'})),
         ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((-1, 'b'), {0: 'a', 4: 'c', 3: 'd'})),
     ])
     def test_with_key(self, data, expected):
-        assert pop_max_by_dict_key(data, key=lambda x: -x) == expected
+        assert pop_max_by_dict_key(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_min_by_dict_key:
     @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min_by_dict_key(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_min_by_dict_key({'1': 1}, key=wrong_type)
+            pop_min_by_dict_key({'1': 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_min_by_dict_key({})
 
     @pytest.mark.parametrize('data, expected', [
         ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('a', 3), {'b': 2, 'c': 1, 'd': 4})),
@@ -712,27 +712,27 @@
         assert pop_min_by_dict_key(data) == expected
 
     @pytest.mark.parametrize('data, expected', [
         ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
         ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((4, 'c'), {0: 'a', -1: 'b', 3: 'd'})),
     ])
     def test_with_key(self, data, expected):
-        assert pop_min_by_dict_key(data, key=lambda x: -x) == expected
+        assert pop_min_by_dict_key(data, condition=lambda x: -x) == expected
 
 
 class Test_pop_max_by_dict_value:
     @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_max_by_dict_value(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_max_by_dict_value({'1': 1}, key=wrong_type)
+            pop_max_by_dict_value({'1': 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_max_by_dict_value({})
 
     @pytest.mark.parametrize('data, expected', [
         ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
@@ -742,27 +742,27 @@
         assert pop_max_by_dict_value(data) == expected
 
     @pytest.mark.parametrize('data, expected', [
         ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((3, 'a'), {2: 'b', 1: 'c', 4: 'd'})),
         ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((0, 'a'), {-1: 'b', 4: 'c', 3: 'd'})),
     ])
     def test_with_key(self, data, expected):
-        assert pop_max_by_dict_value(data, key=lambda x: -ord(x)) == expected
+        assert pop_max_by_dict_value(data, condition=lambda x: -ord(x)) == expected
 
 
 class Test_pop_min_by_dict_value:
     @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             pop_min_by_dict_value(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            pop_min_by_dict_value({'1': 1}, key=wrong_type)
+            pop_min_by_dict_value({'1': 1}, condition=wrong_type)
 
     def test_empty(self):
         with pytest.raises(ValueError):
             pop_min_by_dict_value({})
 
     @pytest.mark.parametrize('data, expected', [
         ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('c', 1), {'a': 3, 'b': 2, 'd': 4})),
@@ -772,15 +772,15 @@
         assert pop_min_by_dict_value(data) == expected
 
     @pytest.mark.parametrize('data, expected', [
         ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
         ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((3, 'd'), {0: 'a', -1: 'b', 4: 'c'})),
     ])
     def test_with_key(self, data, expected):
-        assert pop_min_by_dict_value(data, key=lambda x: -ord(x)) == expected
+        assert pop_min_by_dict_value(data, condition=lambda x: -ord(x)) == expected
 
 
 class Test_pick_all:
     @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
     def test_needles_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all(wrong_type, [])
@@ -887,15 +887,15 @@
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            sort_dict_by_keys({}, key=wrong_type)
+            sort_dict_by_keys({}, condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys({}, reverse=wrong_type)
 
     def test_empty(self):
@@ -904,42 +904,42 @@
     def test_simple(self):
         actual = sort_dict_by_keys({'b': 2, 'c': 1, 'a': 3})
         expected = {'a': 3, 'b': 2, 'c': 1}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_with_key(self):
-        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, key=len)
+        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, condition=len)
         expected = {'x': 3, 'asd': 2, 'qwerty': 1}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_reversed(self):
         actual = sort_dict_by_keys({'b': 2, 'c': 1, 'a': 3}, reverse=True)
         expected = {'c': 1, 'b': 2, 'a': 3}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
     def test_with_key_and_reversed(self):
-        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, key=len, reverse=True)
+        actual = sort_dict_by_keys({'qwerty': 1, 'x': 3, 'asd': 2}, condition=len, reverse=True)
         expected = {'qwerty': 1, 'asd': 2, 'x': 3}
         assert actual == expected
         assert dicts_share_key_order(actual, expected)
 
 
 class Test_sort_dict_by_values:
     @pytest.mark.parametrize('wrong_type', [[], set(), (), 1, 1.0, True, None, False, 'string', object()])
     def test_not_a_dict(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            sort_dict_by_values({}, key=wrong_type)
+            sort_dict_by_values({}, condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values({}, reverse=wrong_type)
 
     def test_empty(self):
@@ -948,42 +948,42 @@
     def test_simple(self):
         actual = sort_dict_by_values({'b': 2, 'c': 1, 'a': 3})
         expected = {'c': 1, 'b': 2, 'a': 3}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_with_key(self):
-        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, key=abs)
+        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, condition=abs)
         expected = {'qwerty': 1, 'asd': -2, 'x': 3}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_reversed(self):
         actual = sort_dict_by_values({'b': 2, 'c': 1, 'a': 3}, reverse=True)
         expected = {'a': 3, 'b': 2, 'c': 1}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
     def test_with_key_and_reversed(self):
-        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, key=abs, reverse=True)
+        actual = sort_dict_by_values({'qwerty': 1, 'x': 3, 'asd': -2}, condition=abs, reverse=True)
         expected = {'x': 3, 'asd': -2, 'qwerty': 1}
         assert actual == expected
         assert dicts_share_value_order(actual, expected)
 
 
 class Test_sort_dict_by_keys_recursive:
     @pytest.mark.parametrize('wrong_type', [1, 1.0, True, None, False, 'string', object()])
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys_recursive(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            sort_dict_by_keys_recursive({}, key=wrong_type)
+            sort_dict_by_keys_recursive({}, condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_keys_recursive({}, reverse=wrong_type)
 
     def test_empty(self):
@@ -1021,21 +1021,21 @@
         ],
         [
             [{'a': 2, 'x': 1}, map(lambda x: x, (2, 1, {'a': {'y': 2, 'z': 1}, 'x': 1}))],
             [{'x': 1, 'a': 2}, (2, 1, {'x': 1, 'a': {'y': 2, 'z': 1}})],
         ],
     ])
     def test_recursive_with_key(self, data, expected):
-        def key(k):
+        def condition(k):
             if k in ['x', 'y']:
                 return 0
             else:
                 return ord(k)
 
-        actual = sort_dict_by_keys_recursive(data, key=key)
+        actual = sort_dict_by_keys_recursive(data, condition=condition)
         actual[1] = tuple(actual[1])
         assert actual == expected
         assert dicts_share_key_order(actual, expected, recursive=True)
 
     @pytest.mark.parametrize('data, expected', [
         [
             [{'x': 1, 'a': 2}, map(lambda x: x, (2, 1, {'x': 1, 'a': {'z': 1, 'y': 2}}))],
@@ -1058,15 +1058,15 @@
     def test_not_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values_recursive(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, True, False, 'string', object()])
     def test_key_is_not_a_function(self, wrong_type):
         with pytest.raises(TypeError):
-            sort_dict_by_values_recursive({}, key=wrong_type)
+            sort_dict_by_values_recursive({}, condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
     def test_not_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_dict_by_values_recursive({}, reverse=wrong_type)
 
     def test_empty(self):
@@ -1100,15 +1100,15 @@
     def test_data_should_be_an_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive(wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            sort_recursive([], key=wrong_type)
+            sort_recursive([], condition=wrong_type)
 
     @pytest.mark.parametrize('wrong_type', [[], set(), (), {}, 1, 1.0, None, 'string', object()])
     def test_reverse_should_be_a_bool(self, wrong_type):
         with pytest.raises(TypeError):
             sort_recursive({}, reverse=wrong_type)
 
     @pytest.mark.parametrize('wrong_value', [[], set(), (), {}, 1, 1.0, 'string', object(), True, False])
@@ -1229,15 +1229,15 @@
         assert swap_keys_and_values(data) == expected
 
 
 class Test_xor:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            xor(1, 2, key=wrong_type)
+            xor(1, 2, condition=wrong_type)
 
     @pytest.mark.parametrize('values', [
         [],
         [1],
     ])
     def test_at_least_2_values(self, values):
         with pytest.raises(ValueError):
@@ -1259,15 +1259,15 @@
         assert is_equal(xor(*values),  expected)
 
 
 class Test_xor_with_idx:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
-            xor_with_idx(1, 2, key=wrong_type)
+            xor_with_idx(1, 2, condition=wrong_type)
 
     @pytest.mark.parametrize('values', [
         [],
         [1],
     ])
     def test_at_least_2_values(self, values):
         with pytest.raises(ValueError):
```

### Comparing `katalytic-data-0.9.1/PKG-INFO` & `katalytic-data-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.9.1
+Version: 0.9.2
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

