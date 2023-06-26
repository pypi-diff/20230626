# Comparing `tmp/iterum-0.1.0-py3-none-any.whl.zip` & `tmp/iterum-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 25609 bytes, number of entries: 15
+Zip file size: 26935 bytes, number of entries: 16
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 iterum/__about__.py
--rw-r--r--  2.0 unx     1600 b- defN 20-Feb-02 00:00 iterum/__init__.py
--rw-r--r--  2.0 unx    11280 b- defN 20-Feb-02 00:00 iterum/_diterum.py
+-rw-r--r--  2.0 unx     1730 b- defN 20-Feb-02 00:00 iterum/__init__.py
+-rw-r--r--  2.0 unx    11299 b- defN 20-Feb-02 00:00 iterum/_diterum.py
 -rw-r--r--  2.0 unx      456 b- defN 20-Feb-02 00:00 iterum/_helpers.py
--rw-r--r--  2.0 unx    62207 b- defN 20-Feb-02 00:00 iterum/_iterum.py
+-rw-r--r--  2.0 unx    62165 b- defN 20-Feb-02 00:00 iterum/_iterum.py
 -rw-r--r--  2.0 unx      467 b- defN 20-Feb-02 00:00 iterum/_notset.py
--rw-r--r--  2.0 unx    38208 b- defN 20-Feb-02 00:00 iterum/_option.py
--rw-r--r--  2.0 unx     1592 b- defN 20-Feb-02 00:00 iterum/_ordering.py
+-rw-r--r--  2.0 unx    38240 b- defN 20-Feb-02 00:00 iterum/_option.py
+-rw-r--r--  2.0 unx     1595 b- defN 20-Feb-02 00:00 iterum/_ordering.py
+-rw-r--r--  2.0 unx     5116 b- defN 20-Feb-02 00:00 iterum/_seq.py
 -rw-r--r--  2.0 unx      412 b- defN 20-Feb-02 00:00 iterum/_singleton.py
 -rw-r--r--  2.0 unx      948 b- defN 20-Feb-02 00:00 iterum/_type_helpers.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 iterum/py.typed
-?rw-r--r--  2.0 unx     2406 b- defN 20-Feb-02 00:00 iterum-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 iterum-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1095 b- defN 20-Feb-02 00:00 iterum-0.1.0.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx     1125 b- defN 20-Feb-02 00:00 iterum-0.1.0.dist-info/RECORD
-15 files, 121905 bytes uncompressed, 23783 bytes compressed:  80.5%
+?rw-r--r--  2.0 unx     2358 b- defN 20-Feb-02 00:00 iterum-0.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 iterum-0.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1095 b- defN 20-Feb-02 00:00 iterum-0.2.0.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx     1196 b- defN 20-Feb-02 00:00 iterum-0.2.0.dist-info/RECORD
+16 files, 127186 bytes uncompressed, 25005 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -18,29 +18,32 @@
 
 Filename: iterum/_option.py
 Comment: 
 
 Filename: iterum/_ordering.py
 Comment: 
 
+Filename: iterum/_seq.py
+Comment: 
+
 Filename: iterum/_singleton.py
 Comment: 
 
 Filename: iterum/_type_helpers.py
 Comment: 
 
 Filename: iterum/py.typed
 Comment: 
 
-Filename: iterum-0.1.0.dist-info/METADATA
+Filename: iterum-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: iterum-0.1.0.dist-info/WHEEL
+Filename: iterum-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: iterum-0.1.0.dist-info/licenses/LICENSE.txt
+Filename: iterum-0.2.0.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: iterum-0.1.0.dist-info/RECORD
+Filename: iterum-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iterum/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## iterum/__init__.py

```diff
@@ -27,22 +27,27 @@
 from ._option import Nil
 from ._option import nil
 from ._option import Option
 from ._option import Some
 from ._option import Swap
 from ._option import UnwrapNilError
 from ._ordering import Ordering
+from ._seq import InfSeq
+from ._seq import Seq
+from ._seq import seq
 
 
 __all__ = [
     # Iterum
     "iterum",
     "Iterum",
     "diterum",
     "Diterum",
+    # Sequential counter
+    "seq",
     # Option
     "Option",
     "Some",
     "Nil",
     "nil",
     "ExpectNilError",
     "UnwrapNilError",
@@ -64,14 +69,16 @@
     "Scan",
     "Skip",
     "SkipWhile",
     "StepBy",
     "Take",
     "TakeWhile",
     "Zip",
+    "InfSeq",
     # Special Diterum implementations
     "Rev",
+    "Seq",
     # used by Scan
     "State",
     # used by swap operations in Option
     "Swap",
 ]
```

## iterum/_diterum.py

```diff
@@ -101,15 +101,15 @@
 
         Examples:
 
             >>> di = diterum([1, 2, 3])
             >>> assert di.rposition(lambda x: x == 3) == Some(2)
             >>> assert di.rposition(lambda x: x == 5) == nil
 
-            >>> # Short-circuiting after first `True`:
+            Short-circuiting after first `True`:
             >>> di = diterum([-1, 2, 3, 4])
             >>> assert di.rposition(lambda x: x >= 2) == Some(3)
             >>> assert di.next() == Some(-1)
         """
         len = self.len()
         return self.rev().position(predicate).map(lambda x: len - x - 1)
 
@@ -132,20 +132,20 @@
         is greater than or equal to the length of the diterum.
 
         Examples:
 
             >>> di = diterum([1, 2, 3])
             >>> assert di.nth_back(2) == Some(1)
 
-            >>> # Does not rewind:
+            Does not rewind:
             >>> di = diterum([1, 2, 3])
             >>> assert di.nth_back(1) == Some(2)
             >>> assert di.nth_back(1) == nil
 
-            >>> # Returns `nil` if there are less than `n + 1` elements:
+            Returns [nil][iterum.nil] if there are less than `n + 1` elements:
             >>> di = diterum([1, 2, 3])
             >>> assert di.nth_back(10) == nil
         """
         return self.rev().nth(n)
 
     def rfind(self, predicate: Callable[[T_co], object], /) -> Option[T_co]:
         """
@@ -162,15 +162,15 @@
 
         Examples:
 
             >>> di = diterum([1, 2, 3])
             >>> assert di.rfind(lambda x: x == 2) == Some(2)
             >>> assert di.rfind(lambda x: x == 5) == nil
 
-            >>> # Stops at first `True`:
+            Stops at first `True`:
             >>> di = diterum([1, 2, 3])
             >>> assert di.rfind(lambda x: x == 2) == Some(2)
             >>> assert di.next_back() == Some(1)
         """
         return self.rev().find(predicate)
 
     def rfold(self, init: U, f: Callable[[U, T_co], U], /) -> U:
@@ -193,19 +193,23 @@
 
         Examples:
 
             >>> di = diterum([1, 2, 3])
             >>> sum = di.rfold(0, lambda acc, x: acc + x)
             >>> assert sum == 6
 
-            >>> # `rfold` is right-associative:
+        rfold is right-associtive:
+
+            ```python
             >>> numbers = [1, 2, 3, 4, 5]
             >>> zero = "0"
             >>> result = diterum(numbers).rfold(zero, lambda acc, x: f"({x} + {acc})")
             >>> assert result == "(1 + (2 + (3 + (4 + (5 + 0)))))"
+
+            ```
         """
         return self.rev().fold(init, f)
 
     def try_rfold(
         self,
         init: U,
         f: Callable[[U, T_co], U],
@@ -250,14 +254,15 @@
 
 
 class diterum(Diterum[T_co]):
     """
     Implements a [Diterum][iterum.Diterum] interface from a sequence.
 
     Examples:
+
         >>> itr = diterum([1, 2, 3])
         >>> assert itr.next() == Some(1)
         >>> assert itr.next_back() == Some(3)
         >>> assert itr.next() == Some(2)
         >>> assert itr.next_back() == nil
         >>> assert itr.next() == nil
 
@@ -284,14 +289,15 @@
 
     def next(self) -> Option[T_co]:
         """
         Returns the next value in the sequence from the front if present,
         otherwise [nil][iterum.nil].
 
         Examples:
+
             >>> itr = diterum([1, 2])
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(2)
             >>> assert itr.next() == nil
         """
 
         if self._back < self._front:
@@ -303,14 +309,15 @@
 
     def next_back(self) -> Option[T_co]:
         """
         Returns the next value in the sequence from the back if present,
         otherwise [nil][iterum.nil].
 
         Examples:
+
             >>> itr = diterum([1, 2])
             >>> assert itr.next_back() == Some(2)
             >>> assert itr.next_back() == Some(1)
             >>> assert itr.next_back() == nil
         """
 
         if self._back < self._front:
@@ -321,14 +328,15 @@
         return Some(nxt)
 
     def len(self) -> int:
         """
         Returns the remaining length of the sequence.
 
         Examples:
+
             >>> itr = diterum([1, 2])
             >>> assert itr.len() == 2
             >>> assert itr.next() == Some(1)
             >>> assert itr.len() == 1
             >>> assert itr.next_back() == Some(2)
             >>> assert itr.len() == 0
             >>> assert itr.next() == nil
```

## iterum/_iterum.py

```diff
@@ -61,23 +61,23 @@
         and so calling [next()][iterum.Iterum.next] again may or may not eventually start returning
         [Some(Item)][iterum.Some] again at some point.
 
         Examples:
 
             >>> itr = iterum([1, 2, 3])
 
-            >>> # A call to next() returns the next value...
+            A call to next() returns the next value...
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(2)
             >>> assert itr.next() == Some(3)
 
-            >>> # ... and then `nil` once it's over.
+            ... and then [nil][iterum.nil] once it's over.
             >>> assert itr.next() == nil
 
-            >>> # More calls may or may not return `nil`. Here, they always will.
+            More calls may or may not return [nil][iterum.nil]. Here, they always will.
             >>> assert itr.next() == nil
             >>> assert itr.next() == nil
         """
         return nil
 
     @classmethod
     def __subclasshook__(cls, C):
@@ -101,20 +101,19 @@
         stop processing as soon as it finds a `False`, given that no matter
         what else happens, the result will also be `False`.
 
         An empty iterum returns `True`.
 
         Examples:
 
-            >>> # Basic usage:
             >>> a = [1, 2, 3]
             >>> assert iterum(a).all(lambda x: x > 0)
             >>> assert not iterum(a).all(lambda x: x > 2)
 
-            >>> # Stopping at the first `False`:
+            Stopping at the first `False`:
             >>> itr = iterum([1, 2, 3])
             >>> assert not itr.all(lambda x: x != 2)
             >>> assert itr.next() == Some(3)
         """
         return all(map(f, self))
 
     def any(self, f: Callable[[T_co], object], /) -> bool:
@@ -135,18 +134,19 @@
         Examples:
 
             >>> a = [1, 2, 3]
             >>> assert iterum(a).any(lambda x: x > 0)
             >>> assert not iterum(a).any(lambda x: x > 5)
 
 
-            >>> # Stopping at teh first `True`:
+            Stopping at the first `True`:
             >>> itr = iterum([1, 2, 3])
             >>> assert itr.any(lambda x: x != 2)
-            >>> # itr still has more elements.
+
+            itr still has more elements.
             >>> assert itr.next() == Some(2)
         """
         return any(map(f, self))
 
     def chain(self: Iterum[T_co], other: Iterable[T_co], /) -> Chain[T_co]:
         """
         Takes two iterables and creates a new iterum over both in sequence.
@@ -252,19 +252,18 @@
 
         [collect()][iterum.Iterum.collect] takes a container which is responsible
         for mapping an iterable into any type. Most commonly this is a collection
         type such as `list` or `set` but could also be a function such as `''.join`.
 
         Examples:
 
-            >>> # basic usage
             >>> doubled = iterum([1, 2, 3]).map(lambda x: x * 2).collect(list)
             >>> assert doubled == [2, 4, 6]
 
-            >>> # using `join` to collect an iterable of `str`
+            using `join` to collect an iterable of `str`
             >>> assert iterum("test").map(str.upper).collect("".join) == "TEST"
         """
         return container(self)
 
     def count(self) -> int:
         """
         Consumes the iterum, counting the number of iterations and returning it.
@@ -417,15 +416,15 @@
 
         Examples:
 
             >>> a = [1, 2, 3]
             >>> assert iterum(a).find(lambda x: x == 2) == Some(2)
             >>> assert iterum(a).find(lambda x: x == 5) == nil
 
-            >>> # Stopping at the first `True`:
+            Stopping at the first `True`:
             >>> it = iterum([1, 2, 3])
             >>> assert it.find(lambda x: x == 2) == Some(2)
             >>> assert it.next() == Some(3)
 
         Note that `it.find(f)` is equivalent to `it.filter(f).next()`.
         """
         for x in self:
@@ -480,19 +479,20 @@
         """
         Creates an iterum that flattens nested structure.
 
         This is useful when you have an iterum of iterables and you want to
         remove one level of indirection.
 
         Examples:
+
             >>> data = [[1, 2, 3, 4], [5, 6]]
             >>> flattened = iterum(data).flatten().collect(list)
             >>> assert flattened == [1, 2, 3, 4, 5, 6]
 
-            >>> # Mapping and then flattening:
+            Mapping and then flattening:
             >>> words = ["alpha", "beta", "gamma"]
             >>> merged = iterum(words).map(iterum).flatten().collect("".join)
             >>> assert merged == "alphabetagamma"
         """
         return Flatten(self)
 
     def fold(self, init: U, f: Callable[[U, T_co], U], /) -> U:
@@ -511,31 +511,34 @@
 
         Examples:
 
             >>> a = [1, 2, 3]
             >>> sum = iterum(a).fold(0, lambda acc, x: acc + x)
             >>> assert sum == 6
 
-        Let's walk through each step of the iteration here:
+            Let's walk through each step of the iteration here:
 
-        | element | acc | x | result |
-        | ------- | --- | - | ------ |
-        |         |  0  |   |        |
-        |   1     |  0  | 1 |   1    |
-        |   2     |  1  | 2 |   3    |
-        |   3     |  3  | 3 |   6    |
+            | element | acc | x | result |
+            | ------- | --- | - | ------ |
+            |         |  0  |   |        |
+            |   1     |  0  | 1 |   1    |
+            |   2     |  1  | 2 |   3    |
+            |   3     |  3  | 3 |   6    |
 
-        And so, our final result, 6.
+            And so, our final result, 6.
 
 
-        Fold is left-associative:
+        fold is left-associative:
 
+            ```python
             >>> numbers = [1, 2, 3, 4, 5]
             >>> result = iterum(numbers).fold("0", lambda acc, x: f"({acc} + {x})")
             >>> assert result == "(((((0 + 1) + 2) + 3) + 4) + 5)"
+
+            ```
         """
         acc = init
         for x in self:
             acc = f(acc, x)
         return acc
 
     def for_each(self, f: Callable[[T_co], object], /) -> None:
@@ -796,15 +799,15 @@
             >>> a = [-1, 4, 0, 1]
             >>> it = iterum(a).map_while(partial(checked_div, 16))
             >>> assert it.next() == Some(-16)
             >>> assert it.next() == Some(4)
             >>> assert it.next() == nil
 
 
-            >>> # Stops after first `nil`:
+            Stops after first [nil][iterum.nil]:
             >>> a = [0, 1, 2, -3, 4, 5, -6]
             >>> it = iterum(a).map_while(lambda x: Some(x) if x >= 0 else nil)
             >>> vec = it.collect(list)
             >>> assert vec == [0, 1, 2]
             >>> assert it.next() == nil
         """
         return MapWhile(self, predicate)
@@ -833,14 +836,15 @@
         Returns the element that gives the maximum value with respect to the
         specified comparison function.
 
         If several elements are equally maximum, the last element is returned.
         If the iterum is empty, [nil][iterum.nil] is returned.
 
         Examples:
+
             >>> a = [-3, 0, 1, 5, -10]
             >>> assert iterum(a).max_by(Ordering.cmp).unwrap() == 5
         """
         max_ = self.next()
         if max_ is nil:
             return nil
         else:
@@ -980,20 +984,20 @@
         than or equal to the length of the iterum.
 
         Examples:
 
             >>> a = [1, 2, 3]
             >>> assert iterum(a).nth(1) == Some(2)
 
-            >>> # Calling `nth` multiple times doesn't rewind the iterum:
+            Calling [nth][iterum.Iterum.nth] multiple times doesn't rewind the iterum:
             >>> itr = iterum([1, 2, 3])
             >>> assert itr.nth(1) == Some(2)
             >>> assert itr.nth(1) == nil
 
-            >>> # Returns `nil` if there are less than `n + 1` elements:
+            Returns [nil][iterum.nil] if there are less than `n + 1` elements:
             >>> itr = iterum([1, 2, 3])
             >>> assert itr.nth(3) == nil
         """
         for i, x in enumerate(self):
             if i > n:
                 return nil
             if i == n:
@@ -1029,15 +1033,15 @@
 
         Examples:
 
             >>> assert iterum([1]).partial_cmp([1]) == Some(Ordering.Equal)
             >>> assert iterum([1, 2]).partial_cmp([1]) == Some(Ordering.Greater)
             >>> assert iterum([1]).partial_cmp([1, 2]) == Some(Ordering.Less)
 
-            >>> # Results are determined by the order of evaluation:
+            Results are determined by the order of evaluation:
             >>> assert iterum([1, None]).partial_cmp([2, nil]) == Some(Ordering.Less)
             >>> assert iterum([2, None]).partial_cmp([1, nil]) == Some(Ordering.Greater)
             >>> assert iterum([None, 1]).partial_cmp([2, None]) == nil
         """
         try:
             value = self.cmp(other)  # type: ignore | reason: ask for forgiveness not permission
         except TypeError:
@@ -1170,14 +1174,15 @@
     def product(self: Iterum[SupportsMulT]) -> Option[SupportsMulT]:
         """
         Iterates over the entire iterum, multiplying all the elements
 
         An empty iterum returns [nil][iterum.nil].
 
         Examples:
+
             >>> def factorial(n: int) -> int:
             ...     return iterum(range(1, n + 1)).product().unwrap_or(1)
             ...
             >>> assert factorial(0) == 1
             >>> assert factorial(1) == 1
             >>> assert factorial(5) == 120
         """
@@ -1193,14 +1198,15 @@
         The reducing function is a closure with two arguments: an ‘accumulator’,
         and an element. For iterums with at least one element, this is the
         same as [fold()][iterum.Iterum.fold] with the first element of the
         iterum as the initial accumulator value, folding every subsequent
         element into it.
 
         Examples:
+
             >>> reduced = iterum(range(1, 10)).reduce(lambda acc, e: acc + e).unwrap()
             >>> assert reduced == 45
         """
         first = self.next()
         if first is nil:
             return nil
         else:
@@ -1246,15 +1252,15 @@
 
         Examples:
 
             >>> itr = iterum([1, 2, 3]).skip(2)
             >>> assert itr.next() == Some(3)
             >>> assert itr.next() == nil
 
-            >>> # Skipping past end:
+            Skipping past end:
             >>> itr = iterum([1, 2, 3]).skip(10)
             >>> assert itr.next() == nil
             >>> assert itr.next() == nil
         """
         return Skip(self, n)
 
     def skip_while(self, predicate: Callable[[T_co], object], /) -> SkipWhile[T_co]:
@@ -1271,15 +1277,15 @@
         Examples:
 
             >>> itr = iterum([-1, 0, 1]).skip_while(lambda x: x < 0)
             >>> assert itr.next() == Some(0)
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == nil
 
-            >>> # After first `False` condition is hit, no further elements are checked:
+            After first `False` condition is hit, no further elements are checked:
             >>> itr = iterum([-1, 0, 1, -3]).skip_while(lambda x: x < 0)
             >>> assert itr.next() == Some(0)
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(-3)
         """
         return SkipWhile(self, predicate)
 
@@ -1345,28 +1351,28 @@
 
             >>> a = [1, 2, 3]
             >>> itr = iterum(a).take(2)
             >>> assert list(itr) == [1, 2]
             >>> assert itr.next() == nil
 
 
-            >>> # Truncate an infinite iterum:
+            Truncate an infinite iterum:
             >>> def count_forever():
             ...     i = 0
             ...     while True:
             ...         yield i
             ...         i += 1
             ...
             >>> itr = iterum(count_forever()).take(3)
             >>> assert itr.next() == Some(0)
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(2)
             >>> assert itr.next() == nil
 
-            >>> # Taking more than you have:
+            Taking more than you have:
             >>> itr = iterum([1, 2]).take(5)
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(2)
             >>> assert itr.next() == nil
         """
         return Take(self, n)
 
@@ -1384,15 +1390,15 @@
         Examples:
 
             >>> a = [-1, 0, 1]
             >>> itr = iterum(a).take_while(lambda x: x < 0)
             >>> assert itr.next() == Some(-1)
             >>> assert itr.next() == nil
 
-            >>> # Stop after first `False`:
+            Stop after first `False`:
             >>> a = [-1, 0, 1, -2]
             >>> itr = iterum(a).take_while(lambda x: x < 0)
             >>> assert itr.next() == Some(-1)
             >>> assert itr.next() == nil
         """
         return TakeWhile(self, predicate)
 
@@ -1423,15 +1429,15 @@
             ...     else:
             ...         raise ValueError("Overflow!")
             ...
             >>> a = [1, 2, 3]
             >>> sum = iterum(a).try_fold(0, checked_add_i8)
             >>> assert sum == Some(6)
 
-            >>> # short-circuit after a failure:
+            short-circuit after a failure:
             >>> it = iterum([10, 20, 30, 100, 40, 50])
             >>> sum = it.try_fold(0, checked_add_i8)
             >>> assert sum == nil
             >>> assert list(it) == [40, 50]
         """
         acc = init
         for x in self:
@@ -1526,15 +1532,15 @@
             >>> a2 = [4, 5, 6]
             >>> itr = iterum(a1).zip(a2)
             >>> assert itr.next() == Some((1, 4))
             >>> assert itr.next() == Some((2, 5))
             >>> assert itr.next() == Some((3, 6))
             >>> assert itr.next() == nil
 
-            >>> # zip smaller with larger:
+            zip smaller with larger:
             >>> def count_forever():
             ...     i = 0
             ...     while True:
             ...         yield i
             ...         i += 1
             ...
             >>> cf_itr = iterum(count_forever())
@@ -1543,15 +1549,15 @@
             >>> assert zip_itr.next() == Some(("f", 0))
             >>> assert zip_itr.next() == Some(("o", 1))
             >>> assert zip_itr.next() == Some(("o", 2))
             >>> assert zip_itr.next() == nil
             >>> assert foo_itr.next() == nil
             >>> assert cf_itr.next() == Some(3)
 
-            >>> # zip larger with smaller:
+            zip larger with smaller:
             >>> cf_itr = iterum(count_forever())
             >>> foo_itr = iterum("foo")
             >>> zip_itr = cf_itr.zip(foo_itr)
             >>> assert zip_itr.next() == Some((0, "f"))
             >>> assert zip_itr.next() == Some((1, "o"))
             >>> assert zip_itr.next() == Some((2, "o"))
             >>> assert zip_itr.next() == nil
@@ -1874,14 +1880,15 @@
 
 
 class iterum(Iterum[T_co]):
     """
     Implements an [Iterum][iterum.Iterum] interface from an iterable object.
 
     Examples:
+
         >>> itr = iterum([1, 2])
         >>> assert itr.next() == Some(1)
         >>> assert itr.next() == Some(2)
         >>> assert itr.next() == nil
 
         >>> itr = iterum([1, 2, 3, 4])
         >>> assert itr.fold(0, lambda acc, x: acc + x) == 10
@@ -1902,13 +1909,14 @@
         self._iter = iter(__iterable)
 
     def next(self) -> Option[T_co]:
         """
         Returns the next value in the iterable if present, otherwise [nil][iterum.nil].
 
         Examples:
+
             >>> itr = iterum([1, 2])
             >>> assert itr.next() == Some(1)
             >>> assert itr.next() == Some(2)
             >>> assert itr.next() == nil
         """
         return _try_next(self._iter)
```

## iterum/_option.py

```diff
@@ -21,17 +21,14 @@
 U = TypeVar("U")
 V = TypeVar("V")
 
 S = TypeVar("S", bound="Some")
 O = TypeVar("O", bound="Option")  # noqa: E741
 
 
-# TODO: Some issues in docs? and validate with doctest
-
-
 class Swap(NamedTuple, Generic[T, U]):
     """
     Used for various 'swapping' operations on [Option][iterum.Option].
     """
 
     inserted: T
     """
@@ -197,16 +194,16 @@
             >>> assert opt == Some(5)
 
             >>> opt = Some(3)
             >>> opt, value = opt.get_or_insert(5)
             >>> assert value == 3
             >>> assert opt == Some(3)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> assert Some(10).get_or_insert(5).returned == 10
             >>> assert nil.get_or_insert(5).returned == 5
 
             >>> assert Some(10).get_or_insert(5).inserted == Some(10)
             >>> assert nil.get_or_insert(5).inserted == Some(5)
         """
@@ -226,16 +223,16 @@
             >>> assert opt == Some(5)
 
             >>> opt = Some(3)
             >>> opt, value = opt.get_or_insert_with(lambda: 5)
             >>> assert value == 3
             >>> assert opt == Some(3)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).get_or_insert_with(lambda: 5)
             >>> assert swap.inserted == Some(10)
             >>> assert swap.returned == 10
 
             >>> swap = nil.get_or_insert_with(lambda: 5)
             >>> assert swap.inserted == Some(5)
@@ -261,16 +258,16 @@
             >>> assert opt == Some(1)
 
             >>> opt = Some(3)
             >>> opt, value = opt.insert(1)
             >>> assert value == 1
             >>> assert opt == Some(1)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).insert(5)
             >>> assert swap.inserted == Some(5)
             >>> assert swap.returned == 5
 
             >>> swap = nil.insert(5)
             >>> assert swap.inserted == Some(5)
@@ -461,16 +458,16 @@
             >>> assert old == Some(2)
 
             >>> x = nil
             >>> new, old = x.replace(5)
             >>> assert new == Some(5)
             >>> assert old == nil
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).replace(5)
             >>> assert swap.inserted == Some(5)
             >>> assert swap.returned == Some(10)
 
             >>> swap = nil.replace(5)
             >>> assert swap.inserted == Some(5)
@@ -491,16 +488,16 @@
             >>> assert old == Some(2)
 
             >>> x = nil
             >>> new, old = x.take()
             >>> assert new == nil
             >>> assert old == nil
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(2).take()
             >>> assert swap.inserted == nil
             >>> assert swap.returned == Some(2)
 
             >>> swap = nil.take()
             >>> assert swap.inserted == nil
@@ -605,15 +602,15 @@
 
     def zip(self, other: Option[U], /) -> Nil:
         """
         Zips `self` with another option.
 
         If `self` is `Some(s)` and `other` is `Some(o)`,
         this method returns `Some((s, o))`.
-        Otherwise, `nil` is returned.
+        Otherwise, [nil][iterum.nil] is returned.
 
         Examples:
 
             >>> assert Some(1).zip(Some("hi")) == Some((1, "hi"))
             >>> assert Some(1).zip(nil) == nil
             >>> assert nil.zip(nil) == nil
         """
@@ -627,14 +624,15 @@
 
 
 class Some(Generic[T]):
     """
     [Some][iterum.Some] value of type T.
 
     Examples:
+
         >>> x = Some(1)  # Type of "x" is "Some[int]"
         >>> x
         Some(1)
         >>> x.is_some()
         True
         >>> x.unwrap()
         1
@@ -760,16 +758,16 @@
             >>> assert opt == Some(5)
 
             >>> opt = Some(3)
             >>> opt, value = opt.get_or_insert(5)
             >>> assert value == 3
             >>> assert opt == Some(3)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> assert Some(10).get_or_insert(5).returned == 10
             >>> assert nil.get_or_insert(5).returned == 5
 
             >>> assert Some(10).get_or_insert(5).inserted == Some(10)
             >>> assert nil.get_or_insert(5).inserted == Some(5)
         """
@@ -788,16 +786,16 @@
             >>> assert opt == Some(5)
 
             >>> opt = Some(3)
             >>> opt, value = opt.get_or_insert_with(lambda: 5)
             >>> assert value == 3
             >>> assert opt == Some(3)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).get_or_insert_with(lambda: 5)
             >>> assert swap.inserted == Some(10)
             >>> assert swap.returned == 10
 
             >>> swap = nil.get_or_insert_with(lambda: 5)
             >>> assert swap.inserted == Some(5)
@@ -822,16 +820,16 @@
             >>> assert opt == Some(1)
 
             >>> opt = Some(3)
             >>> opt, value = opt.insert(1)
             >>> assert value == 1
             >>> assert opt == Some(1)
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).insert(5)
             >>> assert swap.inserted == Some(5)
             >>> assert swap.returned == 5
 
             >>> swap = nil.insert(5)
             >>> assert swap.inserted == Some(5)
@@ -1013,16 +1011,16 @@
             >>> assert old == Some(2)
 
             >>> x = nil
             >>> new, old = x.replace(5)
             >>> assert new == Some(5)
             >>> assert old == nil
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(10).replace(5)
             >>> assert swap.inserted == Some(5)
             >>> assert swap.returned == Some(10)
 
             >>> swap = nil.replace(5)
             >>> assert swap.inserted == Some(5)
@@ -1044,16 +1042,16 @@
             >>> assert old == Some(2)
 
             >>> x = nil
             >>> new, old = x.take()
             >>> assert new == nil
             >>> assert old == nil
 
-        Alternatively, access the named attributes of [Swap][iterum.Swap],
-        [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
+            Alternatively, access the named attributes of [Swap][iterum.Swap],
+            [inserted][iterum.Swap.inserted] and [returned][iterum.Swap.returned]:
 
             >>> swap = Some(2).take()
             >>> assert swap.inserted == nil
             >>> assert swap.returned == Some(2)
 
             >>> swap = nil.take()
             >>> assert swap.inserted == nil
@@ -1155,15 +1153,15 @@
 
     def zip(self, other: Option[U], /) -> Option[tuple[T, U]]:
         """
         Zips `self` with another option.
 
         If `self` is `Some(s)` and `other` is `Some(o)`,
         this method returns `Some((s, o))`.
-        Otherwise, `nil` is returned.
+        Otherwise, [nil][iterum.nil] is returned.
 
         Examples:
 
             >>> assert Some(1).zip(Some("hi")) == Some((1, "hi"))
             >>> assert Some(1).zip(nil) == nil
             >>> assert nil.zip(nil) == nil
         """
@@ -1173,32 +1171,32 @@
 Option: TypeAlias = "Some[T] | Nil"
 """
 Type alias representing something which is either of type
 [Some][iterum.Some] or [Nil][iterum.Nil].
 
 Examples:
 
-    >>> # Type annotate a function which returns `Some[int]` or `nil`:
+    Type annotate a function which returns `Some[int]` or `nil`:
     >>> def checked_div(num: int, dem: int) -> Option[int]:
     ...     try:
     ...         return Some(num // dem)
     ...     except ZeroDivisionError:
     ...         return nil
     ...
 
-    >>> # Use isinstance to narrow the type:
+    Use `isinstance` to narrow the type:
     >>> x = checked_div(10, 3)
     >>> reveal_type(x)  # Type of "x" is "Some[int] | Nil"
     >>> if isinstance(x, Some):
     ...     reveal_type(x)  # Type of "x" is "Some[int]"
     ... else:
     ...     reveal_type(x)  # Type of "x" is "Nil"
     ...
 
-    >>> # Alternatively use pattern matching:
+    Alternatively use pattern matching:
     >>> match x:
     ...     case Some(value):
     ...         print(f"Result: {value=}")
     ...     case Nil:
     ...         print("Cannot divide by 0")
     ...
 }
```

## iterum/_ordering.py

```diff
@@ -38,16 +38,15 @@
             >>> Ordering.cmp(1, 2)
             Ordering.Less
             >>> Ordering.cmp(1, 1)
             Ordering.Equal
             >>> Ordering.cmp(2, 1)
             Ordering.Greater
 
-        A `TypeError` will be raised if the two objects are not comparable:
-
+            A `TypeError` will be raised if the two objects are not comparable:
             >>> try:
             ...     Ordering.cmp(1, "two")
             ... except TypeError as ex:
             ...     print(f"exception received: {ex}")
             ...
             exception received: '>' not supported between instances of 'int' and 'str'
         """
```

## Comparing `iterum-0.1.0.dist-info/METADATA` & `iterum-0.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterum
-Version: 0.1.0
+Version: 0.2.0
 Summary: Rusty iterators in Python.
 Project-URL: Documentation, https://tjsmart.github.io/iterum
 Project-URL: Source, https://github.com/tjsmart/iterum
 Author-email: Tyler Smart <tjsmart@ucsc.edu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -44,31 +44,31 @@
 ## Documentation
 
 The [documentation](https://tjsmart.github.io/iterum) is made with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material) and is hosted by [GitHub Pages](https://docs.github.com/en/pages).
 
 
 ## Example
 
-```pycon
->>> from iterum import iterum
+```python
+from iterum import iterum, Some, nil
 
->>> itr = iterum([1, 2])
->>> assert itr.next() == Some(1)
->>> assert itr.next() == Some(2)
->>> assert itr.next() == nil
-
->>> itr = iterum([1, 2, 3, 4])
->>> assert itr.fold(0, lambda acc, x: acc + x) == 10
-
->>> x = range(5)
->>> y = (
-...     iterum(x)
-...     .map(lambda x: x**2 + 1)
-...     .filter(lambda x: x % 2)
-...     .collect()
-... )
->>> assert y == [1, 5, 17]
+itr = iterum([1, 2])
+assert itr.next() == Some(1)
+assert itr.next() == Some(2)
+assert itr.next() == nil
+
+itr = iterum([1, 2, 3, 4])
+assert itr.fold(0, lambda acc, x: acc + x) == 10
+
+x = range(5)
+y = (
+    iterum(x)
+    .map(lambda x: x**2 + 1)
+    .filter(lambda x: x % 2)
+    .collect()
+)
+assert y == [1, 5, 17]
 ```
 
 ## License
 
 `iterum` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

## Comparing `iterum-0.1.0.dist-info/licenses/LICENSE.txt` & `iterum-0.2.0.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

