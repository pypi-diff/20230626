# Comparing `tmp/perky-0.6.2.tar.gz` & `tmp/perky-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perky-0.6.2.tar", last modified: Sun Feb 26 21:10:36 2023, max compression
+gzip compressed data, was "perky-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `perky-0.6.2.tar` & `perky-0.8.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0       19 2021-04-29 06:38:10.605703 perky-0.6.2/.gitignore
--rw-r--r--   0        0        0     1089 2023-02-26 21:04:44.740884 perky-0.6.2/LICENSE
--rw-r--r--   0        0        0    10903 2023-02-26 21:04:33.096522 perky-0.6.2/README.md
--rwxr-xr-x   0        0        0    18191 2023-02-26 21:06:56.392974 perky-0.6.2/perky/__init__.py
--rw-r--r--   0        0        0    15408 2023-02-26 21:04:15.363971 perky-0.6.2/perky/tokenize.py
--rw-r--r--   0        0        0     5690 2023-02-26 21:06:10.871560 perky-0.6.2/perky/utility.py
--rw-r--r--   0        0        0      437 2021-04-29 06:38:10.605703 perky-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-29 06:38:10.605703 perky-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0        3 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_dict/included.pky
--rw-r--r--   0        0        0       33 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_dict/main.pky
--rw-r--r--   0        0        0        1 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_list/included.pky
--rw-r--r--   0        0        0       27 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_list/main.pky
--rw-r--r--   0        0        0      106 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_nested/included.pky
--rw-r--r--   0        0        0      190 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_nested/main.pky
--rw-r--r--   0        0        0       30 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_path/dir1/main.pky
--rw-r--r--   0        0        0        3 2021-04-29 06:38:10.605703 perky-0.6.2/tests/include_path/dir2/included.pky
--rw-r--r--   0        0        0      214 2021-04-29 06:38:10.605703 perky-0.6.2/tests/test_input.txt
--rw-r--r--   0        0        0     7808 2023-02-26 20:44:57.071987 perky-0.6.2/tests/test_perky.py
--rw-r--r--   0        0        0    11339 1970-01-01 00:00:00.000000 perky-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-06-24 12:24:43.345309 perky-0.8/.gitignore
+-rw-r--r--   0        0        0     1089 2023-05-11 07:56:47.038617 perky-0.8/LICENSE
+-rw-r--r--   0        0        0    13337 2023-06-26 00:23:59.599497 perky-0.8/README.md
+-rwxr-xr-x   0        0        0    13784 2023-06-25 23:55:49.446369 perky-0.8/perky/__init__.py
+-rw-r--r--   0        0        0    13071 2023-06-25 23:00:24.729200 perky-0.8/perky/tokenize.py
+-rw-r--r--   0        0        0     7146 2023-06-25 12:00:23.829670 perky-0.8/perky/transform.py
+-rw-r--r--   0        0        0     4422 2023-06-25 23:56:00.538453 perky-0.8/perky/utility.py
+-rw-r--r--   0        0        0      437 2018-12-04 18:40:09.175851 perky-0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2018-12-04 18:40:09.175851 perky-0.8/tests/__init__.py
+-rw-r--r--   0        0        0        3 2020-08-28 04:00:24.788890 perky-0.8/tests/include_dict/included.pky
+-rw-r--r--   0        0        0       33 2020-08-28 04:00:24.788890 perky-0.8/tests/include_dict/main.pky
+-rw-r--r--   0        0        0        1 2020-08-28 04:00:24.788890 perky-0.8/tests/include_list/included.pky
+-rw-r--r--   0        0        0       27 2020-08-28 04:00:24.788890 perky-0.8/tests/include_list/main.pky
+-rw-r--r--   0        0        0      106 2020-08-28 04:00:24.788890 perky-0.8/tests/include_nested/included.pky
+-rw-r--r--   0        0        0      190 2020-08-28 04:00:24.788890 perky-0.8/tests/include_nested/main.pky
+-rw-r--r--   0        0        0       30 2020-08-28 04:00:24.788890 perky-0.8/tests/include_path/dir1/main.pky
+-rw-r--r--   0        0        0        3 2020-08-28 04:00:24.788890 perky-0.8/tests/include_path/dir2/included.pky
+-rw-r--r--   0        0        0      766 2023-06-25 23:10:33.985812 perky-0.8/tests/perkytestlib.py
+-rw-r--r--   0        0        0      657 2023-06-26 00:04:13.146250 perky-0.8/tests/test_all.py
+-rw-r--r--   0        0        0      214 2018-12-04 18:40:09.175851 perky-0.8/tests/test_input.txt
+-rw-r--r--   0        0        0    13485 2023-06-26 00:03:31.129923 perky-0.8/tests/test_perky.py
+-rw-r--r--   0        0        0     8086 2023-06-26 00:06:09.099154 perky-0.8/tests/test_tokenize.py
+-rw-r--r--   0        0        0     1263 2023-06-26 00:03:56.638121 perky-0.8/tests/test_transform.py
+-rw-r--r--   0        0        0     1773 2023-06-26 00:03:52.422089 perky-0.8/tests/test_utility.py
+-rw-r--r--   0        0        0    13771 1970-01-01 00:00:00.000000 perky-0.8/PKG-INFO
```

### Comparing `perky-0.6.2/LICENSE` & `perky-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `perky-0.6.2/README.md` & `perky-0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 ### Overview
 
 Perky is a new, simple "rcfile" text file format for Python programs.
 It solves the same problem as "INI" files, "TOML" files, and "JSON"
 files, but with its own opinion about how to best solve the problem.
 
-Perky's goals:
+Perky's features:
 
 * Minimal, human-friendly syntax.  Perky files are easy to write by hand.
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
+* Perky supports Python 3.6+, and its supported code passes its
+  unit test suite with 100% coverage.
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
 types:
 
@@ -35,26 +37,27 @@
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
 Unlike Python itself, leading whitespace is ignored.  You
-are free to use leading whitespace to show structure but
-this is optional.
+can use leading whitespace to show structure if you like,
+but it's optional.
 
 Blank lines and comment lines (lines starting with `#`)
-are ignored.
+are ignored, except inside triple-quoted strings.
 
-Perky also supports "pragmas", which are lines that start
-with an equals sign.  By default Perky doesn't define any
+Perky also supports "pragmas", lines that start
+with an equals sign that can perform special runtime
+behavior.  By default Perky doesn't define any
 pragmas--it's an extension mechanism for your use.
 
-Here's a sample Perky configuration file exercising all
-the things you can do in Perky:
+Here's a sample configuration file exercising all
+the things Perky can do:
 
     example name = value
     example dict = {
         name = 3
         another name = 5.0
         }
     example list = [
@@ -108,32 +111,41 @@
     =pragma
     =pragma with argument
 
 #### Explicit transformation is better than implicit
 
 One possibly-surprising design choice of Perky: the only
 natively supported values for the Perky parser are dicts,
-lists, and strings.  Other commonly-used types (ints, floats,
-etc) are handled using a different mechanism: _transformation._
+lists, and strings.  What about ints? floats? dates?
+booleans?
 
-A Perky transformation takes a dict as input, and transforms
-the contents of the dict based on a _schema_.  A Perky schema
-is a dict with the same general shape as the dict produced
-by the Perky parse, but it contains dicts, lists,
-and *transformation functions*.
-If you want *myvalue* in `{'myvalue':'3'}` to be a real integer,
-transform it with the schema `{'myvalue': int}`.
+Perky deliberately leaves that up to you.  As the Zen
+Of Python says:
+
+*In the face of ambiguity, refuse the temptation to guess.*
+
+Perky doesn't know what types your program needs.  So,
+rather than guess and be wrong, Perky keeps things simple:
+just lists, dicts, and strings.  For any other type,
+it's up to you to transform it from a string into the type
+you want, and back again.
 
 Note that Perky doesn't care how or if you transform your
 data.  You can use it as-is, or transform it, or transform
-it with multiple passes.  You don't even need to use Perky's
-simple transformation mechanisms--you can ignore them completely
-and use an external transformation library like
+it with multiple passes.  You can write it yourself,
+or use a third-party data transformation library like
 [Marshmallow.](https://marshmallow.readthedocs.io/)
 
+(Perky used to support an experimental API for transforming
+data yourself.  But this was never fully fleshed-out, and
+there are better versions of that technology out there.
+I've deprecated this part of the library and will remove it
+before 1.0.)
+
+
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
 It's a way of sending instructions to the Perky parser from
 inside a bit of Perky text.
 
 Here's an example pragma directive:
@@ -199,20 +211,25 @@
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-`perky.loads(s, *, pragmas=None) -> d`
+`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
-Parses a string containing Perky-file-format settings.
-Returns a dict.
+Parses a Perky-format string, and returns a container filled
+with the values parsed from that string.
+
+If `root` is not `None`,
+it should be a container
+
+If `root` is `None`, returns a new dict.
 
-`perky.load(filename, *, pragmas=None, encoding="utf-8") -> d`
+`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
 Parses a file containing Perky-file-format settings.
 Returns a dict.
 
 `perky.dumps(d) -> s`
 
 Converts a dictionary to a Perky-file-format string.
@@ -277,14 +294,26 @@
 
 * The default value for `include_path` only searches the
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
 won't search the current directory unless you add `"."`
 to the include path yourself.
 
+#### Deprecated API
+
+These functions are no longer maintained or supported,
+and will be removed before 1.0.
+
+Why?  This part of Perky was always
+an experiment... and the experiment never really paid
+off.  There are better implementations of this idea--you
+you should use those instead.  (If you're relying on
+this code in Perky, I encourage you to fork
+off a copy and maintain it yourself.  But I doubt
+anybody is.)
 
 `perky.map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
   * if it is a dict, replace with a new dict.
   * if it is a list, replace with a new list.
@@ -324,7 +353,42 @@
 
 Experimental.
 
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
+
+### Changelog
+
+**0.8** *2023/06/25*
+
+* Perky now explicitly performs its `isinstance` checks using
+  `collections.abc.MutableMapping` and `collections.abc.MutableSequence`
+  instead of `dict` and `list`.  This permits you to use
+  your own mapping and sequence objects that *don't* inherit from
+  `dict` and `list`.
+* Renamed `PerkyFormatError` to `FormatError`.  The old name is
+  supported for now, but please transition to the new name.
+  The old name will be removed before 1.0.
+* The `transform` submodule is now deprecated and unsupported.
+  Please either stop using it or fork and maintain it yourself.
+* Perky now has a proper unit test suite, which it passes with 100%
+  coverage--except for the unsupported `transform` submodule.
+* While working towards 100% coverage, also cleaned up the code
+  a little in spots.
+
+  - Retooled `LineTokenizer`:
+
+    - Changed its name from `LineParser` is now `LineTokenizer`.
+      It never parsed anything, it just tokenized.
+    - Made its API a little more uniform: now, the
+      only function that will raise `StopIteration` is `__next__`.
+    - The other functions that used to maybe raise `StopIteration`
+      now return a tuple of `None` values when the iterator is empty.
+      This means you can safely write `for a, b, c in line_tokenizer:`.
+    - `bool(lt)` is now accurate; if it returns `True`,
+      you can call `next(lt)` or `lt.next_line()` or `lt.tokens()`
+      and be certain you'll get a value back.
+
+  - Replaced `RuntimeError` exceptions with more appropriate
+    exceptions (`ValueError`, `TypeError`).
```

### Comparing `perky-0.6.2/PKG-INFO` & `perky-0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perky
-Version: 0.6.2
+Version: 0.8
 Summary: A simple, Pythonic file format.  Same interface as the
 Home-page: https://github.com/larryhastings/perky/
 Author: Larry Hastings
 Author-email: larry@hastings.org
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -20,24 +20,26 @@
 
 ### Overview
 
 Perky is a new, simple "rcfile" text file format for Python programs.
 It solves the same problem as "INI" files, "TOML" files, and "JSON"
 files, but with its own opinion about how to best solve the problem.
 
-Perky's goals:
+Perky's features:
 
 * Minimal, human-friendly syntax.  Perky files are easy to write by hand.
 * Explicit minimal data type support.  Rather than guess at the types
   of your data, Perky lets you handle the final transformation.
 * Lightweight, simple, and fast.  Perky's implementation is small
   and straightforward.  Ignoring comments and test code, it's about
   1k lines of Python.  Fewer lines means fewer bugs!  (Hopefully!)
 * Flexible and extensible.  Perky permits extending the semantics of
   Perky files through a "pragma" mechanism.
+* Perky supports Python 3.6+, and its supported code passes its
+  unit test suite with 100% coverage.
 
 #### Perky syntax
 
 Perky configuration files look something like JSON without the
 quoting.  It supports only a surprisingly small set of value
 types:
 
@@ -48,26 +50,27 @@
 
 Perky is line-oriented; individual values go on a single
 line.  Container objects use one line per internal value.
 
 You may nest lists and dicts as deeply as memory permits.
 
 Unlike Python itself, leading whitespace is ignored.  You
-are free to use leading whitespace to show structure but
-this is optional.
+can use leading whitespace to show structure if you like,
+but it's optional.
 
 Blank lines and comment lines (lines starting with `#`)
-are ignored.
+are ignored, except inside triple-quoted strings.
 
-Perky also supports "pragmas", which are lines that start
-with an equals sign.  By default Perky doesn't define any
+Perky also supports "pragmas", lines that start
+with an equals sign that can perform special runtime
+behavior.  By default Perky doesn't define any
 pragmas--it's an extension mechanism for your use.
 
-Here's a sample Perky configuration file exercising all
-the things you can do in Perky:
+Here's a sample configuration file exercising all
+the things Perky can do:
 
     example name = value
     example dict = {
         name = 3
         another name = 5.0
         }
     example list = [
@@ -121,32 +124,41 @@
     =pragma
     =pragma with argument
 
 #### Explicit transformation is better than implicit
 
 One possibly-surprising design choice of Perky: the only
 natively supported values for the Perky parser are dicts,
-lists, and strings.  Other commonly-used types (ints, floats,
-etc) are handled using a different mechanism: _transformation._
+lists, and strings.  What about ints? floats? dates?
+booleans?
 
-A Perky transformation takes a dict as input, and transforms
-the contents of the dict based on a _schema_.  A Perky schema
-is a dict with the same general shape as the dict produced
-by the Perky parse, but it contains dicts, lists,
-and *transformation functions*.
-If you want *myvalue* in `{'myvalue':'3'}` to be a real integer,
-transform it with the schema `{'myvalue': int}`.
+Perky deliberately leaves that up to you.  As the Zen
+Of Python says:
+
+*In the face of ambiguity, refuse the temptation to guess.*
+
+Perky doesn't know what types your program needs.  So,
+rather than guess and be wrong, Perky keeps things simple:
+just lists, dicts, and strings.  For any other type,
+it's up to you to transform it from a string into the type
+you want, and back again.
 
 Note that Perky doesn't care how or if you transform your
 data.  You can use it as-is, or transform it, or transform
-it with multiple passes.  You don't even need to use Perky's
-simple transformation mechanisms--you can ignore them completely
-and use an external transformation library like
+it with multiple passes.  You can write it yourself,
+or use a third-party data transformation library like
 [Marshmallow.](https://marshmallow.readthedocs.io/)
 
+(Perky used to support an experimental API for transforming
+data yourself.  But this was never fully fleshed-out, and
+there are better versions of that technology out there.
+I've deprecated this part of the library and will remove it
+before 1.0.)
+
+
 ### Pragmas
 
 A *pragma* is a metadata directive for the Perky parser.
 It's a way of sending instructions to the Perky parser from
 inside a bit of Perky text.
 
 Here's an example pragma directive:
@@ -212,20 +224,25 @@
   we don't want to let errors pass silently.
 * Using an undefined pragma.
 * Using one of Perky's special tokens as a pragma argument, like
   `{`, `[`, `'''`, `"""`, `[]`, or `{}`.
 
 ### API
 
-`perky.loads(s, *, pragmas=None) -> d`
+`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
-Parses a string containing Perky-file-format settings.
-Returns a dict.
+Parses a Perky-format string, and returns a container filled
+with the values parsed from that string.
+
+If `root` is not `None`,
+it should be a container
+
+If `root` is `None`, returns a new dict.
 
-`perky.load(filename, *, pragmas=None, encoding="utf-8") -> d`
+`def loads(s, *, pragmas=None, encoding='utf-8', root=None) -> o`
 
 Parses a file containing Perky-file-format settings.
 Returns a dict.
 
 `perky.dumps(d) -> s`
 
 Converts a dictionary to a Perky-file-format string.
@@ -290,14 +307,26 @@
 
 * The default value for `include_path` only searches the
 current directory (`"."`).  If you override the default
 and pass in your own include path, the pragma handler
 won't search the current directory unless you add `"."`
 to the include path yourself.
 
+#### Deprecated API
+
+These functions are no longer maintained or supported,
+and will be removed before 1.0.
+
+Why?  This part of Perky was always
+an experiment... and the experiment never really paid
+off.  There are better implementations of this idea--you
+you should use those instead.  (If you're relying on
+this code in Perky, I encourage you to fork
+off a copy and maintain it yourself.  But I doubt
+anybody is.)
 
 `perky.map(d, fn) -> o`
 
 Iterates over a dictionary.  Returns a new dictionary where,
 for every *value*:
   * if it is a dict, replace with a new dict.
   * if it is a list, replace with a new list.
@@ -338,7 +367,42 @@
 Experimental.
 
 
 ### TODO
 
 * Backslash quoting currently does "whatever your version of Python does".  Perhaps this should be explicit, and parsed by Perky itself?
 
+### Changelog
+
+**0.8** *2023/06/25*
+
+* Perky now explicitly performs its `isinstance` checks using
+  `collections.abc.MutableMapping` and `collections.abc.MutableSequence`
+  instead of `dict` and `list`.  This permits you to use
+  your own mapping and sequence objects that *don't* inherit from
+  `dict` and `list`.
+* Renamed `PerkyFormatError` to `FormatError`.  The old name is
+  supported for now, but please transition to the new name.
+  The old name will be removed before 1.0.
+* The `transform` submodule is now deprecated and unsupported.
+  Please either stop using it or fork and maintain it yourself.
+* Perky now has a proper unit test suite, which it passes with 100%
+  coverage--except for the unsupported `transform` submodule.
+* While working towards 100% coverage, also cleaned up the code
+  a little in spots.
+
+  - Retooled `LineTokenizer`:
+
+    - Changed its name from `LineParser` is now `LineTokenizer`.
+      It never parsed anything, it just tokenized.
+    - Made its API a little more uniform: now, the
+      only function that will raise `StopIteration` is `__next__`.
+    - The other functions that used to maybe raise `StopIteration`
+      now return a tuple of `None` values when the iterator is empty.
+      This means you can safely write `for a, b, c in line_tokenizer:`.
+    - `bool(lt)` is now accurate; if it returns `True`,
+      you can call `next(lt)` or `lt.next_line()` or `lt.tokens()`
+      and be certain you'll get a value back.
+
+  - Replaced `RuntimeError` exceptions with more appropriate
+    exceptions (`ValueError`, `TypeError`).
+
```

