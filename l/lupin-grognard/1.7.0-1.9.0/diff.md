# Comparing `tmp/lupin-grognard-1.7.0.tar.gz` & `tmp/lupin-grognard-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-1.7.0.tar", last modified: Fri Feb 10 16:58:28 2023, max compression
+gzip compressed data, was "lupin-grognard-1.9.0.tar", last modified: Wed Apr 19 07:44:20 2023, max compression
```

## Comparing `lupin-grognard-1.7.0.tar` & `lupin-grognard-1.9.0.tar`

### file list

```diff
@@ -1,36 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.791658 lupin-grognard-1.7.0/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.7.0/LICENCE
--rw-rw-rw-   0        0        0      508 2023-02-10 16:58:28.791658 lupin-grognard-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.764125 lupin-grognard-1.7.0/lupin_grognard/
--rw-rw-rw-   0        0        0       23 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.7.0/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.784146 lupin-grognard-1.7.0/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.7.0/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     1450 2023-02-01 12:33:39.000000 lupin-grognard-1.7.0/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.7.0/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.787146 lupin-grognard-1.7.0/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.7.0/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     1767 2023-02-10 16:52:45.000000 lupin-grognard-1.7.0/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1752 2023-02-07 14:39:59.000000 lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     4694 2023-02-10 16:52:45.000000 lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1206 2023-02-01 12:31:41.000000 lupin-grognard-1.7.0/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.788651 lupin-grognard-1.7.0/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.7.0/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-02-10 13:59:49.000000 lupin-grognard-1.7.0/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0      938 2023-01-17 13:04:34.000000 lupin-grognard-1.7.0/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.790661 lupin-grognard-1.7.0/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.7.0/lupin_grognard/core/tools/__init__.py
--rw-rw-rw-   0        0        0     3118 2023-01-17 14:17:29.000000 lupin-grognard-1.7.0/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     4286 2023-02-10 14:00:23.000000 lupin-grognard-1.7.0/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-02-10 16:58:28.780147 lupin-grognard-1.7.0/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      508 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      891 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-10 16:58:28.000000 lupin-grognard-1.7.0/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      883 2023-02-10 16:58:28.792656 lupin-grognard-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.576193 lupin-grognard-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.493409 lupin-grognard-1.9.0/lupin_grognard/
+-rw-rw-rw-   0        0        0       23 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.517953 lupin-grognard-1.9.0/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-03-30 22:12:23.000000 lupin-grognard-1.9.0/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.522952 lupin-grognard-1.9.0/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     7379 2023-03-31 14:48:46.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     5739 2023-04-06 08:21:25.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1319 2023-04-06 08:19:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.526457 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    11845 2023-03-28 14:31:51.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     1472 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     4958 2023-03-30 13:35:56.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/reviewlog.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.528466 lupin-grognard-1.9.0/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-03-26 23:00:29.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-1.9.0/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.530464 lupin-grognard-1.9.0/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     5854 2023-03-31 13:35:54.000000 lupin-grognard-1.9.0/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1848 2023-03-28 13:46:34.000000 lupin-grognard-1.9.0/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-1.9.0/lupin_grognard/templates/reviewlog.j2
+drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.512439 lupin-grognard-1.9.0/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      933 2023-04-19 07:44:20.577191 lupin-grognard-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/setup.py
```

### Comparing `lupin-grognard-1.7.0/LICENCE` & `lupin-grognard-1.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/cmd.py` & `lupin-grognard-1.9.0/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,9 +39,11 @@
         else:
             print(
                 emojize(
                     f"{EMOJI_CROSS} Merge commit {self.hash[:6]}: No approver found"
                 )
             )
         print(f"   - Merged on {self.author_date} by {self.author}, {self.author_mail}")
-        print(f"   - Closes issue {self.closes_issues}")
+        print(
+            f"   - Closes issue: {self.closes_issues if self.closes_issues else 'Not found'}"
+        )
         print(f"   - Commit title: {self.title}")
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 
 from lupin_grognard.core.commit.commit import Commit
-from lupin_grognard.core.commit.commit_reporter import CommitReporter
 from lupin_grognard.core.commit.commit_error import ErrorCount
+from lupin_grognard.core.commit.commit_reporter import CommitReporter
 from lupin_grognard.core.config import (
     COMMIT_TYPE_MUST_HAVE_SCOPE,
     COMMIT_TYPE_MUST_NOT_HAVE_SCOPE,
+    COMMIT_WITH_SCOPE,
     INITIAL_COMMIT,
     PATTERN,
     TITLE_FAILED,
 )
 
 
 class CommitValidator(Commit):
@@ -32,15 +33,15 @@
             if not self._validate_commit_title():
                 self.error_counter.increment_title_error()
             if not self._is_merge_commit(self.title):
                 if not self._validate_body():
                     self.error_counter.increment_body_error()
 
     def _validate_commit_title(self) -> bool:
-        if self._validate_commit_message(self.title):
+        if self._validate_commit_message(self.title, self.type, self.scope):
             self.reporter.display_valid_title_report()
             return True
         else:
             return False
 
     def _validate_body(self) -> bool:
         if self.body:
@@ -49,69 +50,85 @@
                 if self._validate_body_message(message=message):
                     message_error.append(message)
             if len(message_error) > 0:
                 self.reporter.display_body_report(messages=message_error)
                 return False  # must not start with a conventional message
         return True
 
-    def _validate_commit_message(self, commit_msg: str):
+    def _validate_commit_message(self, commit_msg: str, type: str, scope: str) -> bool:
         if self._is_special_commit(commit_msg=commit_msg):
             return True
 
-        type, scope = self._get_conventional_commit_type_and_scope(
-            commit_msg=commit_msg
-        )
         match type:
             case None:
                 self.reporter.display_invalid_title_report(error_message=TITLE_FAILED)
                 return False
-            case "feat":
-                return self._validate_commit_message_for_feat_type(scope=scope)
+            case match_type if (match_type := type) in COMMIT_WITH_SCOPE:
+                return self._validate_commit_message_for_specific_type(
+                    scope=scope, type=match_type
+                )
             case _:
                 return self._validate_commit_message_for_generic_type(
                     type=type, scope=scope
                 )
 
     def _validate_body_message(self, message: str) -> bool:
         """Validates a body message does not start with a conventional commit message"""
         return bool(re.match(PATTERN, message))
 
     def _is_special_commit(self, commit_msg: str) -> bool:
-        return (
-            commit_msg.startswith(("Merge", "Revert", "fixup!", "squash!"))
-            or commit_msg in INITIAL_COMMIT
-        )
+        """Checks if the commit is a Merge or in the list of initial commits"""
+        return commit_msg.startswith("Merge") or commit_msg in INITIAL_COMMIT
 
     def _is_merge_commit(self, commit_msg: str) -> bool:
         return commit_msg.startswith("Merge")
 
     def _validate_commit_merge(self) -> bool:
         self.reporter.display_merge_report(approvers=self.approvers)
         if len(self.approvers) < 1:
             return False
         return True
 
-    def _get_conventional_commit_type_and_scope(self, commit_msg: str) -> tuple:
-        """Returns the conventional commit type and scope if present"""
-        match = re.match(PATTERN, commit_msg)
-        if match:
-            type, scope = match.groups()[:2]
-            return type, scope
-        return None, None
-
-    def _validate_commit_message_for_feat_type(self, scope: str) -> bool:
-        """Validates the scope for a feat commit"""
+    def _validate_commit_message_for_specific_type(self, scope: str, type: str) -> bool:
+        """
+        Validates the scope for a COMMIT_WITH_SCOPE list.
+        If the scope is (change) then the commit title and description
+        must not contain the words 'remove' or 'removed'
+        """
         if scope is None or scope not in ["(add)", "(change)", "(remove)"]:
             self.reporter.display_invalid_title_report(
-                error_message=COMMIT_TYPE_MUST_HAVE_SCOPE
+                error_message=COMMIT_TYPE_MUST_HAVE_SCOPE.format(type=type)
             )
             return False
         else:
+            if scope == "(change)":
+                return self._validate_change_scope_without_remove_word()
             return True
 
+    def _contains_remove_words(self, text: str) -> bool:
+        """Checks if the text contains the words 'remove' or 'removed'"""
+        words = text.lower().split(" ")
+        return any(str in words for str in ["remove", "removed"])
+
+    def _validate_change_scope_without_remove_word(self):
+        """
+        Validate that a commit with the scope (change) does not contain the words
+        'remove' and 'removed' in the title or description
+        """
+        full_text = self.title + " " + " ".join(self.body) if self.body else self.title
+        if self._contains_remove_words(text=full_text):
+            self.reporter.display_invalid_title_report(
+                error_message=(
+                    "Found a commit message that talks about removing something while given "
+                    "scope is 'change': change scope to 'remove' or update the commit description"
+                )
+            )
+            return False
+        return True
+
     def _validate_commit_message_for_generic_type(self, type, scope: str) -> bool:
         """Validates other commit types do not contain a scope"""
         if scope is None:
             return True
         else:
             error_message = COMMIT_TYPE_MUST_NOT_HAVE_SCOPE.format(type, type)
             self.reporter.display_invalid_title_report(error_message=error_message)
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/config.py` & `lupin-grognard-1.9.0/lupin_grognard/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,19 +18,26 @@
 )
 
 MERGE_FAILED = "Commit merges should have at least one approver."
 
 EMOJI_CHECK = ":check_mark_button:"
 EMOJI_CROSS = ":cross_mark:"
 
-COMMIT_TYPE_MUST_HAVE_SCOPE = "Commits of type 'feat' must be of the form 'feat(add)', 'feat(change)' or 'feat(remove)'"
+COMMIT_TYPE_MUST_HAVE_SCOPE = (
+    "Commits of type '{type}' must be of the form '{type}(add)', '{type}(change)' or '{type}(remove)'"
+)
+
 COMMIT_TYPE_MUST_NOT_HAVE_SCOPE = (
     "Commits of type '{}' must not specify a scope but simply use the form '{}'"
 )
 
 PATTERN = (
     r"(?s)"  # To explictly make . match new line
-    r"(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump|enabler)"  # type
+    r"(build|bump|ci|deps|docs|enabler|feat|fix|refactor|test)"  # type
     r"(\(\S+\))?!?:"  # scope
     r"( [^\n\r]+)"  # subject
     r"((\n\n.*)|(\s*))?$"
 )
+
+MAJOR_COMMIT_TYPES = ["enabler", "feat", "fix", "refactor"]
+
+COMMIT_WITH_SCOPE = ["build", "deps", "feat"]
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 import os
 import shutil
 import subprocess
-import sys
 from typing import List, Optional
 
+from lupin_grognard.core.tools.utils import die, warn, info, check_if_file_exists
+
 
 class ClangFormatter:
     def __init__(self, name) -> None:
         self.name = name
 
     def format_c_cpp_files(self) -> None:
         if not self._check_clang_format_tool():
-            self._die(
+            die(
                 msg=(
                     "could not find Clang-Format, use GROG_CLANG_FORMAT "
                     f"to configure the tool to be used (current value is '{self.name}')"
                 )
             )
         code_directory = self._find_code_directory()
         if code_directory is None:
-            self._die(msg="could not find a 'code' directory to be formatted")
-        c_cpp_files = self._search_c_cpp_files(target_directory=code_directory)
-        if len(c_cpp_files) == 0:
-            self._die(msg="no C/C++ files found")
-        for file in c_cpp_files:
-            self._format_files(file)
+            die(msg="could not find a 'code' directory to be formatted")
+
+        if not self._check_clang_format_file_configuration():
+            warn(
+                msg="could not find .clang-format file, please create one in the root path"
+            )
+        else:
+            c_cpp_files = self._search_c_cpp_files(target_directory=code_directory)
+            if len(c_cpp_files) == 0:
+                info(msg="no C/C++ files found")
+            else:
+                for file in c_cpp_files:
+                    self._format_files(file)
 
     def _check_clang_format_tool(self) -> bool | None:
         """Check if clang-format tool is installed on the system and available in the PATH"""
         path = shutil.which(self.name)
         return path is not None
 
     def _find_code_directory(self) -> Optional[str]:
         """Find the code directory in the project root"""
-        code_directory = os.getcwd() + "/code"
+        code_directory = os.path.join(os.getcwd(), "code")
         if os.path.isdir(code_directory):
             return code_directory
         return None
 
+    def _check_clang_format_file_configuration(self) -> bool:
+        """Check if .clang-format file is present in the root path"""
+        return check_if_file_exists(file=".clang-format")
+
     def _search_c_cpp_files(self, target_directory) -> List[str]:
         """Search all C/C++ files in the code directory and subdirectories
         return a list of C/C++ files paths"""
         file_extensions = [".h", ".cpp"]
         c_cpp_files = []
         for root, dirs, files in os.walk(target_directory):
             for file in files:
                 if any(file.endswith(ext) for ext in file_extensions):
-                    c_cpp_files.append(os.path.join(root, file))
+                    file_path = os.path.join(root, file)
+                    c_cpp_files.append(file_path.replace("\\", "/"))
         return c_cpp_files
 
     def _format_files(self, file: str) -> None:
         """Format the C/C++ files"""
-        subprocess.run([self.name, "-i", "--verbose", file])
-
-    def _die(self, msg: str) -> None:
-        print(f"Error: {msg}", file=sys.stderr)
-        sys.exit(1)
+        info(msg=f"Formatting C/C++ file: {file}")
+        subprocess.run([self.name, "-i", file])
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard/core/tools/utils.py` & `lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import logging
 import os
 import re
 import sys
 from typing import List
 
 from lupin_grognard.core.commit.commit import Commit
 from lupin_grognard.core.config import COMMIT_DELIMITER, INITIAL_COMMIT
 from lupin_grognard.core.git import Git
 
 
 def read_file(file: str) -> str:
-    with open(f"{file}", "r") as file:
+    with open(f"{file}", "r", encoding="utf-8") as file:
         data = file.read()
         return data
 
 
 def write_file(file: str, content: str):
-    with open(f"{file}", "w") as outfile:
+    with open(f"{file}", "w", encoding="utf-8") as outfile:
         outfile.write(content)
 
 
 def get_version():
     """get version from setup.cfg file and
     update __version__ in lupin_grognard.__init__.py
     """
@@ -55,14 +56,33 @@
         branch_name = os.getenv("CI_COMMIT_BRANCH")
     if not branch_name:
         print("Warning: failed to get current branch name")
     else:
         print(f"Current branch: {branch_name}")
 
 
+def display_supported_commit_types() -> None:
+    commit_type = [
+        "build(add|change|remove)",
+        "bump",
+        "ci",
+        "deps(add|change|remove)",
+        "docs",
+        "enabler",
+        "feat(add|change|remove)",
+        "fix",
+        "refactor",
+        "test",
+    ]
+    print("Supported commit types: " + ", ".join(commit_type))
+    print(
+        'Only one major commit types allowed per branch: "enabler", "feat", "fix" or "refactor".'
+    )
+
+
 def display_number_of_commits_to_check(commit_list: List):
     number_commits_to_check = len(commit_list)
     if number_commits_to_check == 0:
         print("0 commit to check")
         sys.exit(0)
     elif number_commits_to_check == 1:
         print(f"Found {number_commits_to_check} commit to check:")
@@ -89,7 +109,31 @@
                 if f"into '{branch}'" in commit_obj.title:
                     index = commit_list.index(commit)
                     return commit_list[:(index)]
         elif commit_obj.title in initial_commits:
             index = commit_list.index(commit)
             return commit_list[:index]
     return list()
+
+
+def die(msg: str) -> None:
+    logging.error(msg)
+    sys.exit(1)
+
+
+def warn(msg: str) -> None:
+    logging.warning(msg)
+
+
+def info(msg: str) -> None:
+    logging.info(msg)
+
+
+def check_if_file_exists(file: str) -> bool:
+    file_path = os.path.join(os.getcwd(), file)
+    return os.path.isfile(file_path)
+
+
+def configure_logging():
+    logging.basicConfig(
+        format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO
+    )
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard/run.py` & `lupin-grognard-1.9.0/lupin_grognard/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import os
-import sys
 from typing import Optional
 
 from dotenv import load_dotenv
 import typer
 
 from lupin_grognard.__init__ import __version__
-from lupin_grognard.core.check import check_commit, check_max_allowed_commits
+from lupin_grognard.core.check import (
+    check_commit,
+    check_max_allowed_major_commits,
+)
+from lupin_grognard.core.commit.commit import Commit
+from lupin_grognard.core.doc_generator.changelog import Changelog
+from lupin_grognard.core.doc_generator.reviewlog import Reviewlog
 from lupin_grognard.core.format.clang_format import ClangFormatter
+from lupin_grognard.core.format.cmake_format import CMakeFormatter
 from lupin_grognard.core.git import Git
 from .core.tools.utils import (
+    configure_logging,
     create_branch_list,
     display_current_branch_name,
     display_number_of_commits_to_check,
+    display_supported_commit_types,
     generate_commit_list,
     generate_commits_range_to_check,
+    die,
 )
 
 load_dotenv()
 GROG_BRANCHES = os.getenv("GROG_BRANCHES")
 GROG_MAX_ALLOWED_COMMITS = os.getenv("GROG_MAX_ALLOWED_COMMITS")
 GROG_DONT_CHECK_FOR_APPROVERS = os.getenv("GROG_DONT_CHECK_FOR_APPROVERS")
 GROG_CLANG_FORMAT = os.getenv("GROG_CLANG_FORMAT")
@@ -49,14 +58,18 @@
         max=1,
     ),
     branches_name: Optional[str] = typer.Argument(
         default="master, main, dev, develop, development", envvar="GROG_BRANCHES"
     ),
 ):
     """
+    Supported commit types: build(add|change|remove), bump, ci, deps(add|change|remove), docs, enabler,
+    feat(add|change|remove), fix, refactor, test.
+    Only one major commit types allowed per branch: "enabler", "feat", "fix" or "refactor".
+
     Check every commit message since the last "merge request" in any of the branches in the branches_name list
 
     - With --all option :
     grog check-commits [--all or -a] to check all commits from initial commit
 
     - With --grog-max-allowed-commits option :
     grog check-commits [--grog-max-allowed-commits or -max] {int} to set the maximum number
@@ -68,43 +81,44 @@
     grog check-commits [--grog-dont-check-for-approvers or -dont-approvers] 1 to disable option
 
     - With branches_name argument: grog check-commits "branch_1, branch_2..."
 
     You can set GROG_BRANCHES, GROG_MAX_ALLOWED_COMMITS and GROG_DONT_CHECK_FOR_APPROVERS
     env var in .env, .gitlab-ci.yml, gitlab...
     """
+    configure_logging()
     git = Git()
     if all:  # --all option
         git_log = git.get_log()
         grog_max_allowed_commits = 0
     else:
         git_log = git.get_log(max_line_count=50, first_parent=True)
     if git_log.stderr:
-        print(f"git error {git_log.return_code}\n{git_log.stderr}")
-        sys.exit(1)
+        die(f"git error {git_log.return_code}, {git_log.stderr}")
 
     branch_list = create_branch_list(branches_name=branches_name)
     commit_list = generate_commit_list(data=git_log.stdout)
+    display_supported_commit_types()
     display_current_branch_name()
 
     if all:  # --all option
-        if check_max_allowed_commits(
-            commits=commit_list, max_allowed_commits=grog_max_allowed_commits
+        if check_max_allowed_major_commits(
+            commits_string=commit_list, major_commit_limit=grog_max_allowed_commits
         ):
             display_number_of_commits_to_check(commit_list=commit_list)
             check_commit(
                 commits=commit_list, merge_option=grog_dont_check_for_approvers
             )
     else:
         commit_range_list_to_check = generate_commits_range_to_check(
             branch_list=branch_list, commit_list=commit_list
         )
-        if check_max_allowed_commits(
-            commits=commit_range_list_to_check,
-            max_allowed_commits=grog_max_allowed_commits,
+        if check_max_allowed_major_commits(
+            commits_string=commit_range_list_to_check,
+            major_commit_limit=grog_max_allowed_commits,
         ):
             display_number_of_commits_to_check(commit_list=commit_range_list_to_check)
             check_commit(
                 commits=commit_range_list_to_check,
                 merge_option=grog_dont_check_for_approvers,
             )
 
@@ -112,10 +126,39 @@
 @cli.command()
 def format(
     clang_format: str = typer.Option(
         "clang-format-14", "--clang-format", "-cf", envvar="GROG_CLANG_FORMAT"
     )
 ):
     """Format C/C++ files with clang-format
-    You can set GROG_CLANG_FORMAT env var in order to configure the executable to be used"""
-    formater = ClangFormatter(name=clang_format)
-    formater.format_c_cpp_files()
+    You can set GROG_CLANG_FORMAT env var in order to configure the executable to be used
+    """
+    configure_logging()
+    clang_formater = ClangFormatter(name=clang_format)
+    clang_formater.format_c_cpp_files()
+
+    cmake_formater = CMakeFormatter()
+    cmake_formater.format_cmake_files()
+
+
+@cli.command()
+def changelog():
+    """Generate changelog"""
+    configure_logging()
+    git_log = Git().get_log()
+    if git_log.stderr:
+        die(f"git error {git_log.return_code}, {git_log.stderr}")
+    commit_list = generate_commit_list(data=git_log.stdout)
+    commits = Commit.add_additional_commit_info(commit_list=commit_list)
+    Changelog(commits=commits).generate()
+
+
+@cli.command()
+def reviewlog():
+    """Generate REVIEWLOG.html"""
+    configure_logging()
+    git_log = Git().get_log()
+    if git_log.stderr:
+        die(f"git error {git_log.return_code}, {git_log.stderr}")
+    commit_list = generate_commit_list(data=git_log.stdout)
+    commits = Commit.add_additional_commit_info(commit_list=commit_list)
+    Reviewlog(commits=commits).generate()
```

### Comparing `lupin-grognard-1.7.0/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENCE
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 lupin_grognard/__init__.py
 lupin_grognard/__main__.py
 lupin_grognard/run.py
 lupin_grognard.egg-info/PKG-INFO
@@ -18,11 +19,18 @@
 lupin_grognard/core/config.py
 lupin_grognard/core/git.py
 lupin_grognard/core/commit/__init__.py
 lupin_grognard/core/commit/commit.py
 lupin_grognard/core/commit/commit_error.py
 lupin_grognard/core/commit/commit_reporter.py
 lupin_grognard/core/commit/commit_validator.py
+lupin_grognard/core/doc_generator/__init__.py
+lupin_grognard/core/doc_generator/changelog.py
+lupin_grognard/core/doc_generator/jinja_generator.py
+lupin_grognard/core/doc_generator/reviewlog.py
 lupin_grognard/core/format/__init__.py
 lupin_grognard/core/format/clang_format.py
+lupin_grognard/core/format/cmake_format.py
 lupin_grognard/core/tools/__init__.py
-lupin_grognard/core/tools/utils.py
+lupin_grognard/core/tools/utils.py
+lupin_grognard/templates/changelog.j2
+lupin_grognard/templates/reviewlog.j2
```

### Comparing `lupin-grognard-1.7.0/setup.cfg` & `lupin-grognard-1.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
-00000020: 640d 0a76 6572 7369 6f6e 203d 2031 2e37  d..version = 1.7
+00000020: 640d 0a76 6572 7369 6f6e 203d 2031 2e39  d..version = 1.9
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4c75 7069 6e20 6c69 6e74 6572 2074  = Lupin linter t
 00000050: 6f6f 6c0d 0a6c 6f6e 675f 6465 7363 7269  ool..long_descri
 00000060: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
 00000070: 4144 4d45 2e6d 640d 0a6b 6579 776f 7264  ADME.md..keyword
 00000080: 7320 3d20 636c 692c 206c 696e 7465 720d  s = cli, linter.
 00000090: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
@@ -30,27 +30,30 @@
 000001d0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
 000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 000001f0: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
 00000200: 6571 7569 7265 7320 3d20 0d0a 0974 7970  equires = ...typ
 00000210: 6572 5b61 6c6c 5d3d 3d30 2e36 2e31 0d0a  er[all]==0.6.1..
 00000220: 0970 7974 686f 6e2d 646f 7465 6e76 3d3d  .python-dotenv==
 00000230: 302e 3231 2e30 0d0a 0965 6d6f 6a69 3d3d  0.21.0...emoji==
-00000240: 322e 322e 300d 0a0d 0a5b 6f70 7469 6f6e  2.2.0....[option
-00000250: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-00000260: 5d0d 0a74 6573 7420 3d20 0d0a 0970 7974  ]..test = ...pyt
-00000270: 6573 743d 3d37 2e31 2e33 0d0a 0966 6c61  est==7.1.3...fla
-00000280: 6b65 383d 3d35 2e30 2e34 0d0a 0d0a 5b6f  ke8==5.0.4....[o
-00000290: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
-000002a0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
-000002b0: 7269 7074 7320 3d20 0d0a 0967 726f 6720  ripts = ...grog 
-000002c0: 3d20 6c75 7069 6e5f 6772 6f67 6e61 7264  = lupin_grognard
-000002d0: 2e72 756e 3a63 6c69 0d0a 0d0a 5b6f 7074  .run:cli....[opt
-000002e0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-000002f0: 615d 0d0a 2a20 3d20 2a2e 636c 616e 672d  a]..* = *.clang-
-00000300: 666f 726d 6174 0d0a 0d0a 5b6f 7074 696f  format....[optio
-00000310: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000320: 5d0d 0a65 7863 6c75 6465 203d 200d 0a09  ]..exclude = ...
-00000330: 6c75 7069 6e5f 6772 6f67 6e61 7264 2e74  lupin_grognard.t
-00000340: 6573 7473 2a0d 0a0d 0a5b 6567 675f 696e  ests*....[egg_in
-00000350: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000360: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000370: 0a0d 0a                                  ...
+00000240: 322e 322e 300d 0a09 4a69 6e6a 6132 3d3d  2.2.0...Jinja2==
+00000250: 332e 312e 320d 0a09 636d 616b 656c 616e  3.1.2...cmakelan
+00000260: 673d 3d30 2e36 2e31 330d 0a09 5079 5941  g==0.6.13...PyYA
+00000270: 4d4c 3d3d 362e 300d 0a0d 0a5b 6f70 7469  ML==6.0....[opti
+00000280: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000290: 7265 5d0d 0a74 6573 7420 3d20 0d0a 0970  re]..test = ...p
+000002a0: 7974 6573 743d 3d37 2e31 2e33 0d0a 0966  ytest==7.1.3...f
+000002b0: 6c61 6b65 383d 3d35 2e30 2e34 0d0a 0d0a  lake8==5.0.4....
+000002c0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+000002d0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+000002e0: 7363 7269 7074 7320 3d20 0d0a 0967 726f  scripts = ...gro
+000002f0: 6720 3d20 6c75 7069 6e5f 6772 6f67 6e61  g = lupin_grogna
+00000300: 7264 2e72 756e 3a63 6c69 0d0a 0d0a 5b6f  rd.run:cli....[o
+00000310: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+00000320: 6174 615d 0d0a 2a20 3d20 2a2e 636c 616e  ata]..* = *.clan
+00000330: 672d 666f 726d 6174 0d0a 0d0a 5b6f 7074  g-format....[opt
+00000340: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000350: 6e64 5d0d 0a65 7863 6c75 6465 203d 200d  nd]..exclude = .
+00000360: 0a09 6c75 7069 6e5f 6772 6f67 6e61 7264  ..lupin_grognard
+00000370: 2e74 6573 7473 2a0d 0a0d 0a5b 6567 675f  .tests*....[egg_
+00000380: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000390: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000003a0: 300d 0a0d 0a                             0....
```

