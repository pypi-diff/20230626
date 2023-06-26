# Comparing `tmp/commitizen-3.5.1.tar.gz` & `tmp/commitizen-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.5.1.tar", max compression
+gzip compressed data, was "commitizen-3.5.2.tar", max compression
```

## Comparing `commitizen-3.5.1.tar` & `commitizen-3.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-24 07:23:15.343195 commitizen-3.5.1/LICENSE
--rw-r--r--   0        0        0      609 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/__version__.py
--rw-r--r--   0        0        0     4609 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/bump.py
--rw-r--r--   0        0        0    12112 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    17750 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14245 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7145 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5075 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/info.py
--rw-r--r--   0        0        0    12966 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3176 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/factory.py
--rw-r--r--   0        0        0     7295 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/out.py
--rw-r--r--   0        0        0     7109 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9732 2023-06-24 07:23:15.343195 commitizen-3.5.1/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-06-24 07:23:15.343195 commitizen-3.5.1/docs/README.md
--rw-r--r--   0        0        0     4290 2023-06-24 07:23:15.355195 commitizen-3.5.1/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-25 23:58:43.352577 commitizen-3.5.2/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/__version__.py
+-rw-r--r--   0        0        0     4609 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/bump.py
+-rw-r--r--   0        0        0    12112 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    18106 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14245 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7145 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5208 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12966 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-25 23:58:43.352577 commitizen-3.5.2/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3337 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/factory.py
+-rw-r--r--   0        0        0     7295 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/out.py
+-rw-r--r--   0        0        0     7109 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9732 2023-06-25 23:58:43.356577 commitizen-3.5.2/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-06-25 23:58:43.356577 commitizen-3.5.2/docs/README.md
+-rw-r--r--   0        0        0     4290 2023-06-25 23:58:43.368577 commitizen-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.5.2/PKG-INFO
```

### Comparing `commitizen-3.5.1/LICENSE` & `commitizen-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/__init__.py` & `commitizen-3.5.2/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/bump.py` & `commitizen-3.5.2/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/changelog.py` & `commitizen-3.5.2/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/changelog_parser.py` & `commitizen-3.5.2/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cli.py` & `commitizen-3.5.2/commitizen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import argparse
 import logging
 import sys
-from pathlib import Path
 from functools import partial
+from pathlib import Path
 from types import TracebackType
 
 import argcomplete
 from decli import cli
 
 from commitizen import commands, config, out, version_schemes
 from commitizen.exceptions import (
@@ -321,14 +321,21 @@
                     },
                     {
                         "name": ["--allow-abort"],
                         "action": "store_true",
                         "default": False,
                         "help": "allow empty commit messages, which typically abort a commit",
                     },
+                    {
+                        "name": ["--allowed-prefixes"],
+                        "nargs": "*",
+                        "help": "allowed commit message prefixes. "
+                        "If the message starts by one of these prefixes, "
+                        "the message won't be checked against the regex",
+                    },
                 ],
             },
             {
                 "name": ["version"],
                 "help": (
                     "get the version of the installed commitizen or the current project"
                     " (default: installed commitizen)"
```

### Comparing `commitizen-3.5.1/commitizen/cmd.py` & `commitizen-3.5.2/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/commands/bump.py` & `commitizen-3.5.2/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/commands/changelog.py` & `commitizen-3.5.2/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/commands/check.py` & `commitizen-3.5.2/commitizen/commands/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 import re
 import sys
-from typing import Any
+from typing import Any, List
 
 from commitizen import factory, git, out
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     InvalidCommandArgumentError,
     InvalidCommitMessageError,
     NoCommitsFoundError,
@@ -28,14 +28,23 @@
         self.commit_msg_file: str | None = arguments.get("commit_msg_file")
         self.commit_msg: str | None = arguments.get("message")
         self.rev_range: str | None = arguments.get("rev_range")
         self.allow_abort: bool = bool(
             arguments.get("allow_abort", config.settings["allow_abort"])
         )
 
+        # we need to distinguish between None and [], which is a valid value
+
+        allowed_prefixes = arguments.get("allowed_prefixes")
+        self.allowed_prefixes: List[str] = (
+            allowed_prefixes
+            if allowed_prefixes is not None
+            else config.settings["allowed_prefixes"]
+        )
+
         self._valid_command_argument()
 
         self.config: BaseConfig = config
         self.cz = factory.commiter_factory(self.config)
 
     def _valid_command_argument(self):
         num_exclusive_args_provided = sum(
@@ -130,16 +139,11 @@
             if not line.startswith("#"):
                 lines.append(line)
         return "\n".join(lines)
 
     def validate_commit_message(self, commit_msg: str, pattern: str) -> bool:
         if not commit_msg:
             return self.allow_abort
-        if (
-            commit_msg.startswith("Merge")
-            or commit_msg.startswith("Revert")
-            or commit_msg.startswith("Pull request")
-            or commit_msg.startswith("fixup!")
-            or commit_msg.startswith("squash!")
-        ):
+
+        if any(map(commit_msg.startswith, self.allowed_prefixes)):
             return True
         return bool(re.match(pattern, commit_msg))
```

### Comparing `commitizen-3.5.1/commitizen/commands/commit.py` & `commitizen-3.5.2/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/commands/init.py` & `commitizen-3.5.2/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/commands/version.py` & `commitizen-3.5.2/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/config/__init__.py` & `commitizen-3.5.2/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/config/base_config.py` & `commitizen-3.5.2/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/config/json_config.py` & `commitizen-3.5.2/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/config/toml_config.py` & `commitizen-3.5.2/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/config/yaml_config.py` & `commitizen-3.5.2/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/__init__.py` & `commitizen-3.5.2/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/base.py` & `commitizen-3.5.2/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.5.2/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/customize/customize.py` & `commitizen-3.5.2/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/jira/jira.py` & `commitizen-3.5.2/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/cz/jira/jira_info.txt` & `commitizen-3.5.2/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/defaults.py` & `commitizen-3.5.2/commitizen/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     version_files: list[str]
     version_provider: str | None
     version_scheme: str | None
     version_type: str | None
     tag_format: str | None
     bump_message: str | None
     allow_abort: bool
+    allowed_prefixes: list[str]
     changelog_file: str
     changelog_incremental: bool
     changelog_start_rev: str | None
     changelog_merge_prerelease: bool
     update_changelog_on_bump: bool
     use_shortcuts: bool
     style: list[tuple[str, str]] | None
@@ -71,14 +72,21 @@
     "version": None,
     "version_files": [],
     "version_provider": "commitizen",
     "version_scheme": None,
     "tag_format": None,  # example v$version
     "bump_message": None,  # bumped v$current_version to $new_version
     "allow_abort": False,
+    "allowed_prefixes": [
+        "Merge",
+        "Revert",
+        "Pull request",
+        "fixup!",
+        "squash!",
+    ],
     "changelog_file": "CHANGELOG.md",
     "changelog_incremental": False,
     "changelog_start_rev": None,
     "changelog_merge_prerelease": False,
     "update_changelog_on_bump": False,
     "use_shortcuts": False,
     "major_version_zero": False,
```

### Comparing `commitizen-3.5.1/commitizen/exceptions.py` & `commitizen-3.5.2/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/factory.py` & `commitizen-3.5.2/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/git.py` & `commitizen-3.5.2/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/hooks.py` & `commitizen-3.5.2/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/out.py` & `commitizen-3.5.2/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/providers.py` & `commitizen-3.5.2/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/commitizen/version_schemes.py` & `commitizen-3.5.2/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/docs/README.md` & `commitizen-3.5.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.5.1/pyproject.toml` & `commitizen-3.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.5.1"
+version = "3.5.2"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.5.1"
+version = "3.5.2"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
```

### Comparing `commitizen-3.5.1/PKG-INFO` & `commitizen-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

