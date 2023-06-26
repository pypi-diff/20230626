# Comparing `tmp/advent-of-code-hhoppe-1.0.3.tar.gz` & `tmp/advent_of_code_hhoppe-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advent-of-code-hhoppe-1.0.3.tar", last modified: Sun Apr 30 04:13:24 2023, max compression
+gzip compressed data, was "advent_of_code_hhoppe-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `advent-of-code-hhoppe-1.0.3.tar` & `advent_of_code_hhoppe-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/LICENSE
--rw-r--r--   0        0        0     2367 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/README.md
--rw-r--r--   0        0        0     7733 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/py.typed
--rw-r--r--   0        0        0      907 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/setup.cfg
--rw-r--r--   0        0        0     1993 2023-04-30 04:13:14.972766 advent-of-code-hhoppe-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 advent-of-code-hhoppe-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-26 17:19:14.672014 advent_of_code_hhoppe-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2367 2023-06-26 17:19:14.672014 advent_of_code_hhoppe-1.0.4/README.md
+-rw-r--r--   0        0        0     8275 2023-06-26 17:19:14.676014 advent_of_code_hhoppe-1.0.4/advent_of_code_hhoppe/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:19:14.676014 advent_of_code_hhoppe-1.0.4/advent_of_code_hhoppe/py.typed
+-rw-r--r--   0        0        0      907 2023-06-26 17:19:14.676014 advent_of_code_hhoppe-1.0.4/advent_of_code_hhoppe/setup.cfg
+-rw-r--r--   0        0        0     2020 2023-06-26 17:19:14.676014 advent_of_code_hhoppe-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 advent_of_code_hhoppe-1.0.4/PKG-INFO
```

### Comparing `advent-of-code-hhoppe-1.0.3/LICENSE` & `advent_of_code_hhoppe-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.3/README.md` & `advent_of_code_hhoppe-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/__init__.py` & `advent_of_code_hhoppe-1.0.4/advent_of_code_hhoppe/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python3
 """Library for Advent of Code -- Hugues Hoppe."""
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 from collections.abc import Callable
 import contextlib
 import dataclasses
+import io
 import numbers
 import pathlib
 import re
 import sys
+import tarfile
 import time
 from typing import Any
 import unittest.mock
 import urllib.error
 import urllib.request
 
+import aocd  # https://github.com/wimglenn/advent-of-code-data
 import IPython
 import IPython.display
 
 
 def _read_contents(path_or_url: str, /) -> bytes:
   if path_or_url.startswith(('http://', 'https://')):
     with urllib.request.urlopen(path_or_url) as response:
@@ -41,17 +44,14 @@
   part: int
   answer: str | None = None
   func: Callable[[str], str | int] | None = None
   elapsed_time: float = -0.0  # Negative zero to show that it never ran.
 
   def _aocd_submit(self, result: str) -> str | None:
     """Submit a result to adventofcode.com and return the answer."""
-    # Using https://github.com/wimglenn/advent-of-code-data.
-    import aocd  # pylint: disable=import-error, import-outside-toplevel
-
     # Could set: quiet=True.
     aocd.submit(result, year=self.advent.year, day=self.day, part=self.part, reopen=False)
     puz = aocd.models.Puzzle(year=self.advent.year, day=self.day)
     if self.part == 1:
       if puz.answered_a:
         answer: str = puz.answer_a
         return answer
@@ -104,16 +104,14 @@
   def __post_init__(self) -> None:
     self.advent.puzzles[self.day] = self
     if not self.input and self.advent.input_url:
       url = self.advent.input_url.format(year=self.advent.year, day=self.day)
       with contextlib.suppress(urllib.error.HTTPError, FileNotFoundError):
         self.input = _read_contents(url).decode()
     if not self.input and self.advent.use_aocd:
-      import aocd  # pylint: disable=import-error, import-outside-toplevel
-
       puz = aocd.models.Puzzle(year=self.advent.year, day=self.day)
       self.input = puz.input_data
       if not self.input.endswith('\n'):
         self.input += '\n'
     if not self.input:
       raise ValueError('The puzzle input cannot be determined.')
     for part in (1, 2):
@@ -121,16 +119,14 @@
       if self.advent.answer_url:
         url = self.advent.answer_url.format(
             year=self.advent.year, day=self.day, part=part, part_letter='ab'[part - 1]
         )
         with contextlib.suppress(urllib.error.HTTPError, FileNotFoundError):
           puzzle_part.answer = _read_contents(url).decode()
       if puzzle_part.answer is None and self.advent.use_aocd:
-        import aocd  # pylint: disable=import-error, import-outside-toplevel
-
         puz = aocd.models.Puzzle(year=self.advent.year, day=self.day)
         if part == 1 and puz.answered_a:
           puzzle_part.answer = puz.answer_a
         if part == 2 and puz.answered_b:
           puzzle_part.answer = puz.answer_b
     if IPython.get_ipython():  # type: ignore
       self.print_summary()
@@ -173,22 +169,36 @@
 
 
 @dataclasses.dataclass
 class Advent:
   """Annual advent-of-code consisting of 25 daily puzzles."""
 
   year: int
+  tar_url: str = ''
   input_url: str = ''
   answer_url: str = ''
   puzzles: dict[int, Puzzle] = dataclasses.field(default_factory=dict)  # [day]
 
   def __post_init__(self) -> None:
-    self.use_aocd = (
-        'aocd' in sys.modules and pathlib.Path('~/.config/aocd/token').expanduser().exists()
-    )
+    if self.tar_url:
+      assert not self.input_url and not self.answer_url
+      data_dir = pathlib.Path('./data')
+      if not data_dir.is_dir():
+        data_dir.mkdir()
+      if match := re.search(r'([^/]+)\.tar\.gz$', self.tar_url):
+        data_name = match.group(1)
+      else:
+        raise ValueError(f'{self.tar_url=} must have suffix .tar.gz')
+      if not (data_dir / data_name).is_dir():
+        with tarfile.open(fileobj=io.BytesIO(_read_contents(self.tar_url)), mode='r:gz') as tf:
+          tf.extractall(path=data_dir)  # Python 3.11.4: use filter='data' for security.
+      self.input_url = f'{data_dir}/{data_name}/{{year}}_{{day:02d}}_input.txt'
+      self.answer_url = f'{data_dir}/{data_name}/{{year}}_{{day:02d}}{{part_letter}}_answer.txt'
+
+    self.use_aocd = pathlib.Path('~/.config/aocd/token').expanduser().exists()
 
   def puzzle(self, *args: Any, **kwargs: Any) -> Puzzle:
     """Obtain a daily puzzle."""
     return Puzzle(self, *args, **kwargs)
 
   def show_times(self, *, recompute: bool = False, repeat: int = 1) -> None:
     """Prints the execution times of all puzzle parts."""
```

### Comparing `advent-of-code-hhoppe-1.0.3/advent_of_code_hhoppe/setup.cfg` & `advent_of_code_hhoppe-1.0.4/advent_of_code_hhoppe/setup.cfg`

 * *Files identical despite different names*

### Comparing `advent-of-code-hhoppe-1.0.3/pyproject.toml` & `advent_of_code_hhoppe-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
 ]
 keywords = []
 
 # pip dependencies of the project
 dependencies = [
+    "advent-of-code-data",
     "IPython",
 ]
 
 # This is set automatically by flit using `*.__version__`
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `advent-of-code-hhoppe-1.0.3/PKG-INFO` & `advent_of_code_hhoppe-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: advent-of-code-hhoppe
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for Advent of Code -- Hugues Hoppe.
 Keywords: 
 Author-email: Hugues Hoppe <hhoppe@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Dist: advent-of-code-data
 Requires-Dist: IPython
 Project-URL: homepage, https://github.com/hhoppe/advent-of-code-hhoppe
 Project-URL: repository, https://github.com/hhoppe/advent-of-code-hhoppe
 Provides-Extra: dev
 
 # Module `advent_of_code_hhoppe`
```

