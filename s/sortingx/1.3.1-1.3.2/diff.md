# Comparing `tmp/sortingx-1.3.1.tar.gz` & `tmp/sortingx-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortingx-1.3.1.tar", last modified: Mon May 29 12:21:37 2023, max compression
+gzip compressed data, was "sortingx-1.3.2.tar", last modified: Mon Jun 26 09:14:08 2023, max compression
```

## Comparing `sortingx-1.3.1.tar` & `sortingx-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.889490 sortingx-1.3.1/
--rw-rw-rw-   0        0        0    11357 2023-04-14 13:10:05.000000 sortingx-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     8404 2023-05-29 12:21:37.887490 sortingx-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7054 2023-05-29 12:19:34.000000 sortingx-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 12:21:37.890494 sortingx-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2599 2023-04-14 13:10:05.000000 sortingx-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.858494 sortingx-1.3.1/sortingx/
--rw-rw-rw-   0        0        0      721 2023-05-29 12:00:56.000000 sortingx-1.3.1/sortingx/__init__.py
--rw-rw-rw-   0        0        0     1114 2023-04-14 13:10:05.000000 sortingx-1.3.1/sortingx/_typing.py
--rw-rw-rw-   0        0        0     1891 2023-05-29 12:00:27.000000 sortingx-1.3.1/sortingx/_utils.py
--rw-rw-rw-   0        0        0    10547 2023-04-14 13:10:05.000000 sortingx-1.3.1/sortingx/sorting.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.877494 sortingx-1.3.1/sortingx.egg-info/
--rw-rw-rw-   0        0        0     8404 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.884492 sortingx-1.3.1/tests/
--rw-rw-rw-   0        0        0      313 2023-04-14 13:10:05.000000 sortingx-1.3.1/tests/test_.py
--rw-rw-rw-   0        0        0      390 2023-04-14 13:10:05.000000 sortingx-1.3.1/tests/test_equal.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:14:08.826370 sortingx-1.3.2/
+-rw-rw-rw-   0        0        0    11357 2023-04-14 13:10:05.000000 sortingx-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     8625 2023-06-26 09:14:08.825366 sortingx-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7274 2023-06-26 09:10:41.000000 sortingx-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:14:08.826370 sortingx-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2599 2023-04-14 13:10:05.000000 sortingx-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:14:08.798416 sortingx-1.3.2/sortingx/
+-rw-rw-rw-   0        0        0      721 2023-06-26 08:59:23.000000 sortingx-1.3.2/sortingx/__init__.py
+-rw-rw-rw-   0        0        0     1114 2023-04-14 13:10:05.000000 sortingx-1.3.2/sortingx/_typing.py
+-rw-rw-rw-   0        0        0     1891 2023-05-29 12:00:27.000000 sortingx-1.3.2/sortingx/_utils.py
+-rw-rw-rw-   0        0        0    10682 2023-06-26 08:57:55.000000 sortingx-1.3.2/sortingx/sorting.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:14:08.817257 sortingx-1.3.2/sortingx.egg-info/
+-rw-rw-rw-   0        0        0     8625 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 09:14:08.000000 sortingx-1.3.2/sortingx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 09:14:08.822557 sortingx-1.3.2/tests/
+-rw-rw-rw-   0        0        0      313 2023-04-14 13:10:05.000000 sortingx-1.3.2/tests/test_.py
+-rw-rw-rw-   0        0        0      390 2023-04-14 13:10:05.000000 sortingx-1.3.2/tests/test_equal.py
```

### Comparing `sortingx-1.3.1/LICENSE` & `sortingx-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sortingx-1.3.1/PKG-INFO` & `sortingx-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingx
-Version: 1.3.1
+Version: 1.3.2
 Summary: The powerful package designed for sorting.
 Home-page: https://github.com/linjing-lab/sorting-algorithms
 Download-URL: https://github.com/linjing-lab/sorting-algorithms/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx
@@ -122,13 +122,14 @@
 
 By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
 
 - [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
 - [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
 - [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
 - [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+- [sortingx-1.3.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.2) is the optimized version from v1.3.1, and shrink the returns of calling intrinsic function named `__len__` to get length of `__iterable`.
 
 refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
 
 ## LICENSE
 
 [Apache 2.0](./LICENSE)
```

### Comparing `sortingx-1.3.1/README.md` & `sortingx-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -95,13 +95,14 @@
 
 By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
 
 - [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
 - [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
 - [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
 - [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+- [sortingx-1.3.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.2) is the optimized version from v1.3.1, and shrink the returns of calling intrinsic function named `__len__` to get length of `__iterable`.
 
 refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
 
 ## LICENSE
 
 [Apache 2.0](./LICENSE)
```

### Comparing `sortingx-1.3.1/setup.py` & `sortingx-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `sortingx-1.3.1/sortingx/__init__.py` & `sortingx-1.3.2/sortingx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 from .sorting import bubble, insert, shell, heap, quick, merge, __all__
 
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 
 assert sys.version_info >= (3, 7, 0)
```

### Comparing `sortingx-1.3.1/sortingx/_typing.py` & `sortingx-1.3.2/sortingx/_typing.py`

 * *Files identical despite different names*

### Comparing `sortingx-1.3.1/sortingx/_utils.py` & `sortingx-1.3.2/sortingx/_utils.py`

 * *Files identical despite different names*

### Comparing `sortingx-1.3.1/sortingx/sorting.py` & `sortingx-1.3.2/sortingx/sorting.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,18 @@
     :param reverse: whether to use descending order. The default is ascending order.
 
     :return: bubble's sorted result in a list.
     '''
     __iterable: List[_T] = convert(__iterable)
     compare: List[_T] = generate(__iterable, key)
     if compare and not verify(compare):
-        for i in range(len(__iterable) - 1):
+        length: int = len(__iterable)
+        for i in range(length - 1):
             flag: bool = False # early stop by adding a bool value named flag
-            for j in range(len(__iterable) - i - 1):
+            for j in range(length - i - 1):
                 if (compare[j] < compare[j + 1] if reverse else compare[j] > compare[j+1]):
                     __iterable[j], __iterable[j + 1] = __iterable[j + 1], __iterable[j]
                     if key != None:
                         compare[j], compare[j + 1] = compare[j + 1], compare[j]
                     flag: bool = True
             if not flag:
                 break
@@ -47,15 +48,16 @@
     :param reverse: whether to use descending order. The default is ascending order.
 
     :return: insert's sorted result in a list.
     '''
     __iterable: List[_T] = convert(__iterable)
     compare: List[_T] = generate(__iterable, key)
     if compare and not verify(compare):
-        for index in range(1, len(__iterable)):
+        length: int = len(__iterable)
+        for index in range(1, length):
             keyc: _T = compare[index]
             keya: _T = __iterable[index]
             low : int = 0
             high: int = index - 1
             while low <= high: # sequence conforming to monotonicity
                 mid: int = (low + high) // 2
                 if (keyc <= compare[mid] if reverse else keyc >= compare[mid]):
@@ -171,15 +173,16 @@
                         compare[index], compare[ind] = compare[ind], compare[index]
         if compare[index + 1] != compare[r]:
             __iterable[index + 1], __iterable[r] = __iterable[r], __iterable[index + 1]
             if key != None:
                 compare[index + 1], compare[r] = compare[r], compare[index + 1]
         return index + 1
     if compare and not verify(compare):
-        solve(0, len(__iterable) - 1)
+        length: int = len(__iterable)
+        solve(0, length - 1)
     return __iterable
 
 def merge(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
     '''
     :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
     :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
     :param reverse: whether to use descending order. The default is ascending order.
@@ -191,22 +194,24 @@
     def merg(low: int, mid: int, high: int) -> None:
         '''
         :param low: The low cursor of __iterable (int).
         :param mid: The middle cursor of __iterable (int).
         :param high: The high cursor of __iterable (int).
         '''
         left: List[_T] = __iterable[low: mid]
+        lnl: int = len(left)
         lc: List[_T] = compare[low: mid]
         right: List[_T] = __iterable[mid: high]
+        lnr: int = len(right)
         rc: List[_T] = compare[mid: high]
         i: int = 0
         j: int = 0
         result: List[_T] = []
         store: List[_T] = []
-        while i < len(left) and j < len(right):
+        while i < lnl and j < lnr:
             if (rc[j] <= lc[i] if reverse else rc[j] >= lc[i]):
                 result.append(left[i])
                 store.append(lc[i])
                 i += 1
             else:
                 result.append(right[j])
                 store.append(rc[j])
@@ -219,19 +224,20 @@
         compare[low: high]: List[_T] = store
 
     def solve() -> None:
         '''
         main
         '''
         i: int = 1
-        while i < len(__iterable):
+        length: int = len(__iterable)
+        while i < length:
             low: int = 0
-            while low < len(__iterable):
+            while low < length:
                 mid: int = low + i
-                high: int = min(low + 2 * i, len(__iterable))
+                high: int = min(low + 2 * i, length)
                 if mid < high:
                     merg(low, mid, high)
                 low += 2 * i
             i *= 2
     if compare and not verify(compare):
         solve()
     return __iterable
```

### Comparing `sortingx-1.3.1/sortingx.egg-info/PKG-INFO` & `sortingx-1.3.2/sortingx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingx
-Version: 1.3.1
+Version: 1.3.2
 Summary: The powerful package designed for sorting.
 Home-page: https://github.com/linjing-lab/sorting-algorithms
 Download-URL: https://github.com/linjing-lab/sorting-algorithms/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx
@@ -122,13 +122,14 @@
 
 By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
 
 - [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
 - [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
 - [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
 - [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+- [sortingx-1.3.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.2) is the optimized version from v1.3.1, and shrink the returns of calling intrinsic function named `__len__` to get length of `__iterable`.
 
 refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
 
 ## LICENSE
 
 [Apache 2.0](./LICENSE)
```

