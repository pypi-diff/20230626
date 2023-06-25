# Comparing `tmp/pygount-1.5.1.tar.gz` & `tmp/pygount-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygount-1.5.1.tar", max compression
+gzip compressed data, was "pygount-1.6.0.tar", max compression
```

## Comparing `pygount-1.5.1.tar` & `pygount-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     3755 2022-01-06 19:03:46.000000 pygount-1.5.1/README.md
--rw-r--r--   0        0        0      698 2023-01-02 08:17:33.701895 pygount-1.5.1/pygount/__init__.py
--rw-r--r--   0        0        0    31970 2023-01-02 08:17:33.702125 pygount-1.5.1/pygount/analysis.py
--rw-r--r--   0        0        0    15265 2023-01-02 08:17:33.702285 pygount-1.5.1/pygount/command.py
--rw-r--r--   0        0        0     6453 2023-01-02 08:17:33.702417 pygount-1.5.1/pygount/common.py
--rw-r--r--   0        0        0     2085 2023-01-02 08:17:33.702607 pygount-1.5.1/pygount/lexers.py
--rw-r--r--   0        0        0     9253 2023-01-02 08:17:33.702836 pygount-1.5.1/pygount/summary.py
--rw-r--r--   0        0        0    10627 2023-01-02 08:17:33.703033 pygount-1.5.1/pygount/write.py
--rw-r--r--   0        0        0     4296 2023-01-02 08:17:33.703237 pygount-1.5.1/pygount/xmldialect.py
--rw-r--r--   0        0        0     2136 2022-12-31 23:56:13.550855 pygount-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 pygount-1.5.1/setup.py
--rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 pygount-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     4888 2023-06-25 23:16:15.321381 pygount-1.6.0/README.md
+-rw-r--r--   0        0        0      685 2023-06-02 15:02:53.678813 pygount-1.6.0/pygount/__init__.py
+-rw-r--r--   0        0        0    35084 2023-06-25 23:13:58.547023 pygount-1.6.0/pygount/analysis.py
+-rw-r--r--   0        0        0    15396 2023-06-06 08:13:21.872180 pygount-1.6.0/pygount/command.py
+-rw-r--r--   0        0        0     6476 2023-06-13 20:37:39.920761 pygount-1.6.0/pygount/common.py
+-rw-r--r--   0        0        0     1371 2023-06-25 22:16:01.849583 pygount-1.6.0/pygount/git_storage.py
+-rw-r--r--   0        0        0     2085 2023-01-02 08:17:33.702607 pygount-1.6.0/pygount/lexers.py
+-rw-r--r--   0        0        0     9253 2023-01-02 08:17:33.702836 pygount-1.6.0/pygount/summary.py
+-rw-r--r--   0        0        0    10648 2023-06-02 16:31:08.551599 pygount-1.6.0/pygount/write.py
+-rw-r--r--   0        0        0     4296 2023-01-02 08:17:33.703237 pygount-1.6.0/pygount/xmldialect.py
+-rw-r--r--   0        0        0     2093 2023-06-14 17:19:06.908521 pygount-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 pygount-1.6.0/PKG-INFO
```

### Comparing `pygount-1.5.1/LICENSE.txt` & `pygount-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygount-1.5.1/pygount/__init__.py` & `pygount-1.6.0/pygount/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Pygount counts lines of source code using pygments lexers.
 """
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
-import pkg_resources
+from importlib.metadata import version
 
 from .analysis import DuplicatePool, SourceAnalysis, SourceScanner, SourceState, encoding_for, source_analysis
 from .common import Error, OptionError
 from .summary import LanguageSummary, ProjectSummary
 
-__version__ = pkg_resources.get_distribution(__name__).version
+__version__ = version(__name__)
 
 __all__ = [
     "__version__",
     "encoding_for",
     "DuplicatePool",
     "Error",
     "LanguageSummary",
```

### Comparing `pygount-1.5.1/pygount/analysis.py` & `pygount-1.6.0/pygount/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 import glob
 import hashlib
 import itertools
 import logging
 import os
 import re
 from enum import Enum
-from typing import Dict, Generator, List, Optional, Pattern, Sequence, Set, Tuple, Union
+from io import SEEK_CUR, BufferedIOBase, IOBase, RawIOBase, TextIOBase
+from typing import Dict, Iterator, List, Optional, Pattern, Sequence, Set, Tuple, Union
 
 import pygments.lexer
 import pygments.lexers
 import pygments.token
 import pygments.util
 
 import pygount.common
 import pygount.lexers
 import pygount.xmldialect
 from pygount.common import deprecated
+from pygount.git_storage import GitStorage, git_remote_url_and_revision_if_any
 
 # Attempt to import chardet.
-
 try:
     import chardet.universaldetector
 
     _detector = chardet.universaldetector.UniversalDetector()
 except ImportError:
     _detector = None
 has_chardet = bool(_detector)
@@ -66,15 +67,15 @@
     generated = 6
     # TODO: 'huge' = auto()  # source code exceeds size limit
     #: pygments does not offer any lexer to analyze the source
     unknown = 7
 
 
 #: Default patterns for regular expressions to detect generated code.
-#: The '(?i)' indicates that the patterns are case insensitive.
+#: The '(?i)' indicates that the patterns are case-insensitive.
 DEFAULT_GENERATED_PATTERNS_TEXT = pygount.common.REGEX_PATTERN_PREFIX + ", ".join(
     [
         r"(?i).*automatically generated",
         r"(?i).*do not edit",
         r"(?i).*generated with the .+ utility",
         r"(?i).*this is a generated file",
         r"(?i).*generated automatically",
@@ -125,15 +126,14 @@
     "read\\.me",
     "todo",
 )
 _PLAIN_TEXT_PATTERN = "(^" + "$)|(^".join(_STANDARD_PLAIN_TEXT_NAME_PATTERNS) + "$)"
 #: Regular expression to detect plain text files by name.
 _PLAIN_TEXT_NAME_REGEX = re.compile(_PLAIN_TEXT_PATTERN, re.IGNORECASE)
 
-
 #: Mapping for file suffixes to lexers for which pygments offers no official one.
 _SUFFIX_TO_FALLBACK_LEXER_MAP = {
     "fex": pygount.lexers.MinimalisticWebFocusLexer(),
     "idl": pygount.lexers.IdlLexer(),
     "m4": pygount.lexers.MinimalisticM4Lexer(),
     "txt": pygount.lexers.PlainTextLexer(),
     "vbe": pygount.lexers.MinimalisticVBScriptLexer(),
@@ -257,57 +257,69 @@
     def from_file(
         source_path: str,
         group: str,
         encoding: str = "automatic",
         fallback_encoding: str = "cp1252",
         generated_regexes=pygount.common.regexes_from(DEFAULT_GENERATED_PATTERNS_TEXT),
         duplicate_pool: Optional[DuplicatePool] = None,
+        file_handle: Optional[IOBase] = None,
     ) -> "SourceAnalysis":
         """
         Factory method to create a :py:class:`SourceAnalysis` by analyzing
-        the source code in ``source_path``.
+        the source code in ``source_path`` or the open file ``file_handle``.
 
         :param source_path: path to source code to analyze
         :param group: name of a logical group the sourc code belongs to, e.g. a
           package.
         :param encoding: encoding according to :func:`encoding_for`
         :param fallback_encoding: fallback encoding according to
           :func:`encoding_for`
         :param generated_regexes: list of regular expression that if found within the first few lines
           if a source code identify is as generated source code for which SLOC should not be counted
         :param duplicate_pool: a :class:`DuplicatePool` where information about possible duplicates is
           collected, or ``None`` if possible duplicates should be counted multiple times.
+        :param file_handle: a file-like object, or ``None`` to read and open the file from
+          ``source_path``. If the file is open in text mode, it must be opened with the correct
+          encoding.
         """
         assert encoding is not None
         assert generated_regexes is not None
 
         result = None
         lexer = None
         source_code = None
-        source_size = os.path.getsize(source_path)
-        if source_size == 0:
-            _log.info("%s: is empty", source_path)
-            result = SourceAnalysis.from_state(source_path, group, SourceState.empty)
-        elif is_binary_file(source_path):
-            _log.info("%s: is binary", source_path)
-            result = SourceAnalysis.from_state(source_path, group, SourceState.binary)
-        elif not has_lexer(source_path):
-            _log.info("%s: unknown language", source_path)
-            result = SourceAnalysis.from_state(source_path, group, SourceState.unknown)
-        elif duplicate_pool is not None:
+        if file_handle is None:
+            source_size = os.path.getsize(source_path)
+            if source_size == 0:
+                _log.info("%s: is empty", source_path)
+                result = SourceAnalysis.from_state(source_path, group, SourceState.empty)
+            elif is_binary_file(source_path):
+                _log.info("%s: is binary", source_path)
+                result = SourceAnalysis.from_state(source_path, group, SourceState.binary)
+            elif not has_lexer(source_path):
+                _log.info("%s: unknown language", source_path)
+                result = SourceAnalysis.from_state(source_path, group, SourceState.unknown)
+        if duplicate_pool is not None:
             duplicate_path = duplicate_pool.duplicate_path(source_path)
             if duplicate_path is not None:
                 _log.info("%s: is a duplicate of %s", source_path, duplicate_path)
                 result = SourceAnalysis.from_state(source_path, group, SourceState.duplicate, duplicate_path)
         if result is None:
-            if encoding in ("automatic", "chardet"):
-                encoding = encoding_for(source_path, encoding, fallback_encoding)
             try:
-                with open(source_path, encoding=encoding) as source_file:
-                    source_code = source_file.read()
+                if file_handle is None:
+                    if encoding in ("automatic", "chardet"):
+                        encoding = encoding_for(source_path, encoding, fallback_encoding)
+                    with open(source_path, encoding=encoding) as source_file:
+                        source_code = source_file.read()
+                elif not isinstance(file_handle, TextIOBase):
+                    if encoding in ("automatic", "chardet"):
+                        encoding = encoding_for(source_path, encoding, fallback_encoding, file_handle=file_handle)
+                    source_code = file_handle.read().decode(encoding)
+                else:
+                    source_code = file_handle.read()
             except (LookupError, OSError, UnicodeError) as error:
                 _log.warning("cannot read %s using encoding %s: %s", source_path, encoding, error)
                 result = SourceAnalysis.from_state(source_path, group, SourceState.error, error)
             if result is None:
                 lexer = guess_lexer(source_path, source_code)
                 assert lexer is not None
         if (result is None) and (len(generated_regexes) != 0):
@@ -470,69 +482,89 @@
     Scanner for source code files matching certain conditions.
     """
 
     def __init__(
         self,
         source_patterns,
         suffixes="*",
-        folders_to_skip=pygount.common.regexes_from(DEFAULT_FOLDER_PATTERNS_TO_SKIP_TEXT),
-        name_to_skip=pygount.common.regexes_from(DEFAULT_NAME_PATTERNS_TO_SKIP_TEXT),
+        folders_to_skip=None,
+        name_to_skip=None,
     ):
         self._source_patterns = source_patterns
         self._suffixes = pygount.common.regexes_from(suffixes)
-        self._folder_regexps_to_skip = folders_to_skip
-        self._name_regexps_to_skip = name_to_skip
+        self._folder_regexps_to_skip = (
+            folders_to_skip
+            if folders_to_skip is not None
+            else pygount.common.regexes_from(DEFAULT_FOLDER_PATTERNS_TO_SKIP_TEXT)
+        )
+        self._name_regexps_to_skip = (
+            name_to_skip
+            if folders_to_skip is not None
+            else pygount.common.regexes_from(DEFAULT_NAME_PATTERNS_TO_SKIP_TEXT)
+        )
+        self._git_storages = []
+
+    def close(self):
+        for git_storage in self._git_storages:
+            git_storage.close()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+        return False
 
     @property
     def source_patterns(self):
         return self._source_patterns
 
     @property
-    def suffixes(self):
+    def suffixes(self) -> List[Pattern]:
         return self._suffixes
 
     @property
-    def folder_regexps_to_skip(self):
+    def folder_regexps_to_skip(self) -> List[Pattern]:
         return self._folder_regexps_to_skip
 
     @folder_regexps_to_skip.setter
     def folder_regexps_to_skip(self, regexps_or_pattern_text):
         self._folder_regexps_to_skip.append = pygount.common.regexes_from(
             regexps_or_pattern_text, self.folder_regexps_to_skip
         )
 
     @property
-    def name_regexps_to_skip(self):
+    def name_regexps_to_skip(self) -> List[Pattern]:
         return self._name_regexps_to_skip
 
     @name_regexps_to_skip.setter
     def name_regexps_to_skip(self, regexps_or_pattern_text):
-        self._name_regexp_to_skip = pygount.common.regexes_from(regexps_or_pattern_text, self.name_regexps_to_skip)
+        self._name_regexps_to_skip = pygount.common.regexes_from(regexps_or_pattern_text, self.name_regexps_to_skip)
 
-    def _is_path_to_skip(self, name, is_folder):
+    def _is_path_to_skip(self, name, is_folder) -> bool:
         assert os.sep not in name, "name=%r" % name
         regexps_to_skip = self._folder_regexps_to_skip if is_folder else self._name_regexps_to_skip
         return any(path_name_to_skip_regex.match(name) is not None for path_name_to_skip_regex in regexps_to_skip)
 
-    def _paths_and_group_to_analyze_in(self, folder, group):
+    def _paths_and_group_to_analyze_in(self, folder, group) -> Tuple[str, str]:
         assert folder is not None
         assert group is not None
 
         for name in os.listdir(folder):
             path = os.path.join(folder, name)
             if not os.path.islink(path):
                 is_folder = os.path.isdir(path)
                 if self._is_path_to_skip(os.path.basename(path), is_folder):
                     _log.debug("skip due to matching skip pattern: %s", path)
                 elif is_folder:
                     yield from self._paths_and_group_to_analyze_in(path, group)
                 else:
                     yield path, group
 
-    def _paths_and_group_to_analyze(self, path_to_analyse_pattern, group=None):
+    def _paths_and_group_to_analyze(self, path_to_analyse_pattern, group=None) -> Iterator[Tuple[str, str]]:
         for path_to_analyse in glob.glob(path_to_analyse_pattern):
             if os.path.islink(path_to_analyse):
                 _log.debug("skip link: %s", path_to_analyse)
             else:
                 is_folder = os.path.isdir(path_to_analyse)
                 if self._is_path_to_skip(os.path.basename(path_to_analyse), is_folder):
                     _log.debug("skip due to matching skip pattern: %s", path_to_analyse)
@@ -548,26 +580,34 @@
                     else:
                         if actual_group is None:
                             actual_group = os.path.dirname(path_to_analyse)
                             if actual_group == "":
                                 actual_group = os.path.basename(os.path.dirname(os.path.abspath(path_to_analyse)))
                         yield path_to_analyse, actual_group
 
-    def _source_paths_and_groups_to_analyze(self, patterns_to_analyze):
-        assert patterns_to_analyze is not None
+    def _source_paths_and_groups_to_analyze(self, source_patterns_to_analyze) -> List[Tuple[str, str]]:
+        assert source_patterns_to_analyze is not None
         result = []
-        for pattern in patterns_to_analyze:
+        for source_pattern_to_analyze in source_patterns_to_analyze:
             try:
-                result.extend(self._paths_and_group_to_analyze(pattern))
+                remote_url, revision = git_remote_url_and_revision_if_any(source_pattern_to_analyze)
+                if remote_url is not None:
+                    git_storage = GitStorage(remote_url, revision)
+                    self._git_storages.append(git_storage)
+                    git_storage.extract()
+                    # TODO#113: Find a way to exclude the ugly temp folder from the source path.
+                    result.extend(self._paths_and_group_to_analyze(git_storage.temp_folder))
+                else:
+                    result.extend(self._paths_and_group_to_analyze(source_pattern_to_analyze))
             except OSError as error:
-                raise OSError(f'cannot scan "{pattern}" for source files: {error}')
+                raise OSError(f'cannot scan "{source_pattern_to_analyze}" for source files: {error}')
         result = sorted(set(result))
         return result
 
-    def source_paths(self) -> Generator[str, None, None]:
+    def source_paths(self) -> Iterator[str]:
         """
         Paths to source code files matching all the conditions for this scanner.
         """
         source_paths_and_groups_to_analyze = self._source_paths_and_groups_to_analyze(self.source_patterns)
 
         for source_path, group in source_paths_and_groups_to_analyze:
             suffix = os.path.splitext(source_path)[1].lstrip(".")
@@ -625,26 +665,26 @@
     Words that do not count as code if it is the only word in a line.
     """
     assert language_id is not None
     assert language_id.islower()
     return _LANGUAGE_TO_WHITE_WORDS_MAP.get(language_id, set())
 
 
-def _delined_tokens(tokens: Sequence[Tuple[TokenType, str]]) -> Generator[TokenType, None, None]:
+def _delined_tokens(tokens: Sequence[Tuple[TokenType, str]]) -> Iterator[TokenType]:
     for token_type, token_text in tokens:
         newline_index = token_text.find("\n")
         while newline_index != -1:
             yield token_type, token_text[: newline_index + 1]
             token_text = token_text[newline_index + 1 :]
             newline_index = token_text.find("\n")
         if token_text != "":
             yield token_type, token_text
 
 
-def _pythonized_comments(tokens: Sequence[Tuple[TokenType, str]]) -> Generator[TokenType, None, None]:
+def _pythonized_comments(tokens: Sequence[Tuple[TokenType, str]]) -> Iterator[TokenType]:
     """
     Similar to tokens but converts strings after a colon (:) to comments.
     """
     is_after_colon = True
     for token_type, token_text in tokens:
         if is_after_colon and (token_type in pygments.token.String):
             token_type = pygments.token.Comment
@@ -653,15 +693,15 @@
         elif token_type not in pygments.token.Comment:
             is_whitespace = len(token_text.rstrip(" \f\n\r\t")) == 0
             if not is_whitespace:
                 is_after_colon = False
         yield token_type, token_text
 
 
-def _line_parts(lexer: pygments.lexer.Lexer, text: str) -> Generator[Set[str], None, None]:
+def _line_parts(lexer: pygments.lexer.Lexer, text: str) -> Iterator[Set[str]]:
     line_marks = set()
     tokens = _delined_tokens(lexer.get_tokens(text))
     if lexer.name == "Python":
         tokens = _pythonized_comments(tokens)
     language_id = lexer.name.lower()
     white_text = " \f\n\r\t" + white_characters(language_id)
     white_words = white_code_words(language_id)
@@ -682,15 +722,20 @@
         if token_text.endswith("\n"):
             yield line_marks
             line_marks = set()
     if len(line_marks) >= 1:
         yield line_marks
 
 
-def encoding_for(source_path: str, encoding: str = "automatic", fallback_encoding: Optional[str] = None) -> str:
+def encoding_for(
+    source_path: str,
+    encoding: str = "automatic",
+    fallback_encoding: Optional[str] = None,
+    file_handle: Optional[Union[BufferedIOBase, RawIOBase]] = None,
+) -> str:
     """
     The encoding used by the text file stored in ``source_path``.
 
     The algorithm used is:
 
     * If ``encoding`` is ``'automatic``, attempt the following:
 
@@ -702,16 +747,24 @@
 
     * If ``encoding`` is ``'chardet`` use :mod:`chardet` to obtain the encoding.
     * For any other ``encoding`` simply use the specified value.
     """
     assert encoding is not None
 
     if encoding == "automatic":
-        with open(source_path, "rb") as source_file:
-            heading = source_file.read(128)
+        if file_handle is None:
+            with open(source_path, "rb") as source_file:
+                heading = source_file.read(128)
+        else:
+            if not file_handle.seekable:
+                raise pygount.Error(
+                    f"cannot automatically determine encoding: file handle must be seekable: {source_path}"
+                )
+            heading = file_handle.read(128)
+            file_handle.seek(-len(heading), SEEK_CUR)
         result = None
         if len(heading) == 0:
             # File is empty, assume a dummy encoding.
             result = "utf-8"
         if result is None:
             # Check for known BOMs.
             for bom, encoding in _BOM_TO_ENCODING_MAP.items():
@@ -733,19 +786,27 @@
                 if xml_prolog_match is not None:
                     result = xml_prolog_match.group("encoding")
     elif encoding == "chardet":
         assert (
             _detector is not None
         ), 'without chardet installed, encoding="chardet" must be rejected before calling encoding_for()'
         _detector.reset()
-        with open(source_path, "rb") as source_file:
-            for line in source_file.readlines():
-                _detector.feed(line)
-                if _detector.done:
-                    break
+        if file_handle is None:
+            with open(source_path, "rb") as source_file:
+                lines = source_file.readlines()
+        else:
+            if not file_handle.seekable:
+                raise pygount.Error(f"cannot determine encoding: file handle must be seekable: {source_path}")
+            file_position = file_handle.tell()
+            lines = file_handle.readlines()
+            file_handle.seek(file_position)
+        for line in lines:
+            _detector.feed(line)
+            if _detector.done:
+                break
         result = _detector.result["encoding"]
         if result is None:
             _log.warning(
                 "%s: chardet cannot determine encoding, assuming fallback encoding %s", source_path, fallback_encoding
             )
             result = fallback_encoding
     else:
@@ -755,16 +816,21 @@
         # Encoding 'automatic' or 'chardet' failed to detect anything.
         if fallback_encoding is not None:
             # If defined, use the fallback encoding.
             result = fallback_encoding
         else:
             try:
                 # Attempt to read the file as UTF-8.
-                with open(source_path, encoding="utf-8") as source_file:
-                    source_file.read()
+                if file_handle is None:
+                    with open(source_path, encoding="utf-8") as source_file:
+                        source_file.read()
+                else:
+                    file_handle.seekable and file_handle.seek(0)
+                    file_handle.read()
+                    file_handle.seekable and file_handle.seek(0)
                 result = "utf-8"
             except UnicodeDecodeError:
                 # UTF-8 did not work out, use the default as last resort.
                 result = DEFAULT_FALLBACK_ENCODING
             _log.debug("%s: no fallback encoding specified, using %s", source_path, result)
 
     assert result is not None
```

### Comparing `pygount-1.5.1/pygount/command.py` & `pygount-1.6.0/pygount/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,40 +317,42 @@
         self.set_output(args.out, "option --out")
         self.set_output_format(args.format, "option --format")
         self.set_source_patterns(args.source_patterns, "option PATTERNS")
         self.set_suffixes(args.suffix, "option --suffix")
 
     def execute(self):
         _log.setLevel(logging.INFO if self.is_verbose else logging.WARNING)
-        source_scanner = pygount.analysis.SourceScanner(
+        with pygount.analysis.SourceScanner(
             self.source_patterns, self.suffixes, self.folders_to_skip, self.names_to_skip
-        )
-        source_paths_and_groups_to_analyze = list(source_scanner.source_paths())
-        duplicate_pool = pygount.analysis.DuplicatePool() if not self.has_duplicates else None
-        writer_class = _OUTPUT_FORMAT_TO_WRITER_CLASS_MAP[self.output_format]
-        is_stdout = self.output == "STDOUT"
-        target_context_manager = (
-            contextlib.nullcontext(sys.stdout) if is_stdout else open(self.output, "w", encoding="utf-8", newline="")
-        )
-        with target_context_manager as target_file, writer_class(target_file) as writer:
-            with Progress(disable=not writer.has_to_track_progress, transient=True) as progress:
-                try:
-                    for source_path, group in progress.track(source_paths_and_groups_to_analyze):
-                        writer.add(
-                            pygount.analysis.SourceAnalysis.from_file(
-                                source_path,
-                                group,
-                                self.default_encoding,
-                                self.fallback_encoding,
-                                generated_regexes=self._generated_regexs,
-                                duplicate_pool=duplicate_pool,
+        ) as source_scanner:
+            source_paths_and_groups_to_analyze = list(source_scanner.source_paths())
+            duplicate_pool = pygount.analysis.DuplicatePool() if not self.has_duplicates else None
+            writer_class = _OUTPUT_FORMAT_TO_WRITER_CLASS_MAP[self.output_format]
+            is_stdout = self.output == "STDOUT"
+            target_context_manager = (
+                contextlib.nullcontext(sys.stdout)
+                if is_stdout
+                else open(self.output, "w", encoding="utf-8", newline="")
+            )
+            with target_context_manager as target_file, writer_class(target_file) as writer:
+                with Progress(disable=not writer.has_to_track_progress, transient=True) as progress:
+                    try:
+                        for source_path, group in progress.track(source_paths_and_groups_to_analyze):
+                            writer.add(
+                                pygount.analysis.SourceAnalysis.from_file(
+                                    source_path,
+                                    group,
+                                    self.default_encoding,
+                                    self.fallback_encoding,
+                                    generated_regexes=self._generated_regexs,
+                                    duplicate_pool=duplicate_pool,
+                                )
                             )
-                        )
-                finally:
-                    progress.stop()
+                    finally:
+                        progress.stop()
 
 
 def pygount_command(arguments=None):
     result = 1
     command = Command()
     try:
         command.apply_arguments(arguments)
```

### Comparing `pygount-1.5.1/pygount/common.py` & `pygount-1.6.0/pygount/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2016-2023, Thomas Aglassinger.
 # All rights reserved. Distributed under the BSD License.
 import fnmatch
 import functools
 import inspect
 import re
 import warnings
-from typing import Generator, List, Optional, Pattern, Sequence, Union
+from typing import Iterator, List, Optional, Pattern, Sequence, Union
 
 #: Pseudo pattern to indicate that the remaining pattern are an addition to the default patterns.
 ADDITIONAL_PATTERN = "[...]"
 
 #: Prefix to use for pattern strings to describe a regular expression instead of a shell pattern.
 REGEX_PATTERN_PREFIX = "[regex]"
 
@@ -60,16 +60,16 @@
             result = re.compile(pattern)
     else:
         result = pattern  # Assume pattern already is a compiled regular expression
     return result
 
 
 def regexes_from(
-    patterns_text: Union[str, Sequence[str]],
-    default_patterns_text: Optional[Union[str, Sequence[str]]] = None,
+    patterns_text: Union[str, Sequence[str], Sequence[Pattern]],
+    default_patterns_text: Optional[Union[str, Sequence[Pattern], Sequence[str]]] = None,
     source: Optional[str] = None,
 ) -> List[Pattern]:
     assert patterns_text is not None
 
     result = []
     default_regexes = []
     try:
@@ -90,28 +90,28 @@
         else:
             regexes = list(patterns_text)
             if len(regexes) >= 1 and regexes[0] is None:
                 default_regexes = regexes_from(default_patterns_text)
                 regexes = regexes[1:]
             for supposed_regex in regexes:
                 assert isinstance(supposed_regex, _REGEX_TYPE), (
-                    "patterns_text must a text or sequnce or regular expressions but contains: %a" % supposed_regex
+                    "patterns_text must a text or sequence or regular expressions but contains: %a" % supposed_regex
                 )
             result.extend(regexes)
     except re.error as error:
         raise OptionError(f"cannot parse pattern for regular repression: {error}", source)
     result.extend(default_regexes)
     return result
 
 
-def lines(text: str) -> Generator[str, None, None]:
+def lines(text: str) -> Iterator[str]:
     """
     Generator function to yield lines (delimited with ``'\n'``) stored in
     ``text``. This is useful when a regular expression should only match on a
-    per line basis in a memory efficient way.
+    per-line basis in a memory efficient way.
     """
     assert text is not None
     assert "\r" not in text
     previous_newline_index = 0
     newline_index = text.find("\n")
     while newline_index != -1:
         yield text[previous_newline_index:newline_index]
@@ -126,15 +126,14 @@
     """
     Decorator to mark functions as deprecated and log a warning in case it is called.
 
     Source: https://stackoverflow.com/questions/2536307/decorators-in-the-python-standard-lib-deprecated-specifically
     """
 
     if isinstance(reason, str):
-
         # The @deprecated is used with a 'reason'.
         #
         # .. code-block:: python
         #
         #    @deprecated("please, use another function")
         #    def old_function(x, y):
         #      pass
@@ -154,15 +153,14 @@
                 warnings.simplefilter("default", DeprecationWarning)
                 return func1(*args, **kwargs)
 
             return new_func1
 
         return decorator
     elif inspect.isclass(reason) or inspect.isfunction(reason):
-
         # The @deprecated is used without any 'reason'.
         #
         # .. code-block:: python
         #
         #    @deprecated
         #    def old_function(x, y):
         #      pass
```

### Comparing `pygount-1.5.1/pygount/lexers.py` & `pygount-1.6.0/pygount/lexers.py`

 * *Files identical despite different names*

### Comparing `pygount-1.5.1/pygount/summary.py` & `pygount-1.6.0/pygount/summary.py`

 * *Files identical despite different names*

### Comparing `pygount-1.5.1/pygount/write.py` & `pygount-1.6.0/pygount/write.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self.has_to_track_progress = True
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
+        return False
 
     def add(self, source_analysis):
         self.project_summary.add(source_analysis)
 
     def close(self):
         self.project_summary.update_file_percentages()
         self.finished_at = datetime.datetime.utcnow()
```

### Comparing `pygount-1.5.1/pygount/xmldialect.py` & `pygount-1.6.0/pygount/xmldialect.py`

 * *Files identical despite different names*

### Comparing `pygount-1.5.1/pyproject.toml` & `pygount-1.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.poetry]
 name = "pygount"
-version = "1.5.1"
+version = "1.6.0"
 description = "count source lines of code (SLOC) using pygments"
 readme = "README.md"
 authors = ["Thomas Aglassinger <roskakori@users.sourceforge.net>"]
 license = "BSD"
 homepage = "https://github.com/roskakori/pygount"
 repository = "https://github.com/roskakori/pygount.git"
 documentation = "https://pygount.readthedocs.io"
@@ -47,38 +47,37 @@
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development",
 ]
 packages = [
     { include = "pygount" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7, <4"
+python = ">=3.8, <4"
 pygments = "^2"
 chardet = "^5"
-rich = ">=9, <13"
+rich = ">=9, <14"
+gitpython = "^3.1.31"
 
 [tool.poetry.dev-dependencies]
-wheel = "^0.38"
 coveralls = "^3"
 coverage = "^6"
 pytest = "^7"
 pytest-cov = "^4"
-pre-commit = "^2"
+pre-commit = "^3"
 pur = "^7"
 Sphinx = "^5"
 sphinx-rtd-theme = "^1"
 twine = "^4"
 
 [tool.poetry.scripts]
 pygount = "pygount.command:main"
```

