# Comparing `tmp/git-machete-3.9.0.tar.gz` & `tmp/git-machete-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-machete-3.9.0.tar", last modified: Sat Apr 23 12:34:05 2022, max compression
+gzip compressed data, was "git-machete-3.9.1.tar", last modified: Wed May 11 15:38:51 2022, max compression
```

## Comparing `git-machete-3.9.0.tar` & `git-machete-3.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-04-23 12:34:05.871907 git-machete-3.9.0/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1075 2022-04-23 12:34:00.000000 git-machete-3.9.0/LICENSE
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2022-04-23 12:34:00.000000 git-machete-3.9.0/MANIFEST.in
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     9311 2022-04-23 12:34:05.871907 git-machete-3.9.0/PKG-INFO
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     8514 2022-04-23 12:34:00.000000 git-machete-3.9.0/README.md
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-04-23 12:34:05.871907 git-machete-3.9.0/completion/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     3954 2022-04-23 12:34:00.000000 git-machete-3.9.0/completion/README.md
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     7111 2022-04-23 12:34:00.000000 git-machete-3.9.0/completion/git-machete.completion.bash
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    16721 2022-04-23 12:34:00.000000 git-machete-3.9.0/completion/git-machete.completion.zsh
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    34832 2022-04-23 12:34:00.000000 git-machete-3.9.0/completion/git-machete.fish
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      639 2022-04-23 12:34:00.000000 git-machete-3.9.0/git-machete
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-04-23 12:34:05.871907 git-machete-3.9.0/git_machete/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       22 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/__init__.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    40678 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/cli.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)   129317 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/client.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      538 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/constants.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    53900 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/docs.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      855 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/exceptions.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    50864 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/git_operations.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    11939 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/github.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     2903 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/options.py
--rw-rw-r--   0 circleci  (1000) circleci  (1000)    10235 2022-04-23 12:34:00.000000 git-machete-3.9.0/git_machete/utils.py
-drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-04-23 12:34:05.871907 git-machete-3.9.0/git_machete.egg-info/
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     9311 2022-04-23 12:34:05.000000 git-machete-3.9.0/git_machete.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1000) circleci  (1000)      548 2022-04-23 12:34:05.000000 git-machete-3.9.0/git_machete.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2022-04-23 12:34:05.000000 git-machete-3.9.0/git_machete.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       12 2022-04-23 12:34:05.000000 git-machete-3.9.0/git_machete.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1000) circleci  (1000)       38 2022-04-23 12:34:05.871907 git-machete-3.9.0/setup.cfg
--rw-rw-r--   0 circleci  (1000) circleci  (1000)     1283 2022-04-23 12:34:00.000000 git-machete-3.9.0/setup.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-05-11 15:38:51.515787 git-machete-3.9.1/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1075 2022-05-11 15:38:45.000000 git-machete-3.9.1/LICENSE
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      126 2022-05-11 15:38:45.000000 git-machete-3.9.1/MANIFEST.in
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     9384 2022-05-11 15:38:51.515787 git-machete-3.9.1/PKG-INFO
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     8587 2022-05-11 15:38:45.000000 git-machete-3.9.1/README.md
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-05-11 15:38:51.511787 git-machete-3.9.1/completion/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     3953 2022-05-11 15:38:45.000000 git-machete-3.9.1/completion/README.md
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     7111 2022-05-11 15:38:45.000000 git-machete-3.9.1/completion/git-machete.completion.bash
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    16722 2022-05-11 15:38:45.000000 git-machete-3.9.1/completion/git-machete.completion.zsh
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    34832 2022-05-11 15:38:45.000000 git-machete-3.9.1/completion/git-machete.fish
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      639 2022-05-11 15:38:45.000000 git-machete-3.9.1/git-machete
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-05-11 15:38:51.515787 git-machete-3.9.1/git_machete/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       22 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/__init__.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    40681 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/cli.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)   130637 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/client.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      538 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/constants.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    53901 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/docs.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      855 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/exceptions.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    51016 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/git_operations.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    11940 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/github.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     2903 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/options.py
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)    10235 2022-05-11 15:38:45.000000 git-machete-3.9.1/git_machete/utils.py
+drwxrwxr-x   0 circleci  (1000) circleci  (1000)        0 2022-05-11 15:38:51.515787 git-machete-3.9.1/git_machete.egg-info/
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     9384 2022-05-11 15:38:51.000000 git-machete-3.9.1/git_machete.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)      548 2022-05-11 15:38:51.000000 git-machete-3.9.1/git_machete.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)        1 2022-05-11 15:38:51.000000 git-machete-3.9.1/git_machete.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       12 2022-05-11 15:38:51.000000 git-machete-3.9.1/git_machete.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)       38 2022-05-11 15:38:51.515787 git-machete-3.9.1/setup.cfg
+-rw-rw-r--   0 circleci  (1000) circleci  (1000)     1283 2022-05-11 15:38:45.000000 git-machete-3.9.1/setup.py
```

### Comparing `git-machete-3.9.0/LICENSE` & `git-machete-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/PKG-INFO` & `git-machete-3.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-machete
-Version: 3.9.0
+Version: 3.9.1
 Summary: Probably the sharpest git repository organizer & rebase/merge workflow automation tool you've ever seen
 Home-page: https://github.com/VirtusLab/git-machete
 Author: Pawel Lipski
 Author-email: pawel.p.lipski@gmail.com
 License: MIT
 Keywords: git
 Platform: UNKNOWN
@@ -25,17 +25,18 @@
 [![Read the Docs](https://readthedocs.org/projects/git-machete/badge/?version=latest)](https://git-machete.readthedocs.io/en/stable)
 [![PyPI package](https://img.shields.io/pypi/v/git-machete.svg)](https://pypi.org/project/git-machete)
 [![PyPI package monthly downloads](https://img.shields.io/pypi/dm/git-machete.svg?label=pypi%20downloads)](https://pypistats.org/packages/git-machete)
 [![Snap](https://snapcraft.io/git-machete/badge.svg)](https://snapcraft.io/git-machete)
 [![AUR package (Arch Linux)](https://repology.org/badge/version-for-repo/aur/git-machete.svg)](https://aur.archlinux.org/packages/git-machete)
 [![License: MIT](https://img.shields.io/github/license/VirtusLab/git-machete)](https://github.com/VirtusLab/git-machete/blob/master/LICENSE)
 [![CircleCI](https://circleci.com/gh/VirtusLab/git-machete/tree/master.svg?style=shield)](https://app.circleci.com/pipelines/github/VirtusLab/git-machete?branch=master)
+[![codecov](https://codecov.io/gh/VirtusLab/git-machete/branch/master/graph/badge.svg)](https://codecov.io/gh/VirtusLab/git-machete)
 
-<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
-<!-- The image is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 💪 git-machete is a robust tool that **simplifies your git workflows**.<br/>
 
 🦅 The _bird's eye view_ provided by git-machete makes **merges/rebases/push/pulls hassle-free**
 even when **multiple branches** are present in the repository
 (master/develop, your topic branches, teammate's branches checked out for review, etc.).<br/>
 
@@ -44,18 +45,18 @@
 👁 A look at a `git machete status` gives an instant answer to the questions:
 * What branches are in this repository?
 * What is going to be merged (rebased/pushed/pulled) and to what?
 
 🚜 `git machete traverse` semi-automatically traverses the branches, helping you effortlessly rebase, merge, push and pull.
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/discover-status-traverse.gif"
+    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/discover-status-traverse.gif"
          alt="git machete discover, status and traverse" />
 </p>
-<!-- The gif in here is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 🔌 See also [VirtusLab/git-machete-intellij-plugin](https://github.com/VirtusLab/git-machete-intellij-plugin#git-machete-intellij-plugin) &mdash;
 a port into a plugin for the IntelliJ Platform products, including PyCharm, WebStorm etc.
 
 
 ## Install
```

### Comparing `git-machete-3.9.0/README.md` & `git-machete-3.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 [![Read the Docs](https://readthedocs.org/projects/git-machete/badge/?version=latest)](https://git-machete.readthedocs.io/en/stable)
 [![PyPI package](https://img.shields.io/pypi/v/git-machete.svg)](https://pypi.org/project/git-machete)
 [![PyPI package monthly downloads](https://img.shields.io/pypi/dm/git-machete.svg?label=pypi%20downloads)](https://pypistats.org/packages/git-machete)
 [![Snap](https://snapcraft.io/git-machete/badge.svg)](https://snapcraft.io/git-machete)
 [![AUR package (Arch Linux)](https://repology.org/badge/version-for-repo/aur/git-machete.svg)](https://aur.archlinux.org/packages/git-machete)
 [![License: MIT](https://img.shields.io/github/license/VirtusLab/git-machete)](https://github.com/VirtusLab/git-machete/blob/master/LICENSE)
 [![CircleCI](https://circleci.com/gh/VirtusLab/git-machete/tree/master.svg?style=shield)](https://app.circleci.com/pipelines/github/VirtusLab/git-machete?branch=master)
+[![codecov](https://codecov.io/gh/VirtusLab/git-machete/branch/master/graph/badge.svg)](https://codecov.io/gh/VirtusLab/git-machete)
 
-<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
-<!-- The image is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 💪 git-machete is a robust tool that **simplifies your git workflows**.<br/>
 
 🦅 The _bird's eye view_ provided by git-machete makes **merges/rebases/push/pulls hassle-free**
 even when **multiple branches** are present in the repository
 (master/develop, your topic branches, teammate's branches checked out for review, etc.).<br/>
 
@@ -22,18 +23,18 @@
 👁 A look at a `git machete status` gives an instant answer to the questions:
 * What branches are in this repository?
 * What is going to be merged (rebased/pushed/pulled) and to what?
 
 🚜 `git machete traverse` semi-automatically traverses the branches, helping you effortlessly rebase, merge, push and pull.
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/discover-status-traverse.gif"
+    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/discover-status-traverse.gif"
          alt="git machete discover, status and traverse" />
 </p>
-<!-- The gif in here is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 🔌 See also [VirtusLab/git-machete-intellij-plugin](https://github.com/VirtusLab/git-machete-intellij-plugin#git-machete-intellij-plugin) &mdash;
 a port into a plugin for the IntelliJ Platform products, including PyCharm, WebStorm etc.
 
 
 ## Install
```

### Comparing `git-machete-3.9.0/completion/README.md` & `git-machete-3.9.1/completion/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,10 +101,10 @@
 
 ### Linux
 
 Place the completion script in `/path/to/fish/completions/` (typically `~/.config/fish/completions/git-machete.fish`).
 
 ```shell script
 mkdir -p ~/.config/fish/completions
-curl -L https://raw.githubusercontent.com/VirtusLab/git-machete/develop/completion/git-machete.fish -o ~/.config/fish/completions/git-machete.fish
+curl -L https://raw.githubusercontent.com/VirtusLab/git-machete/master/completion/git-machete.fish -o ~/.config/fish/completions/git-machete.fish
 echo "source ~/.config/fish/completions/git-machete.fish >/dev/null" >> ~/.config/fish/config.fish
 ```
```

### Comparing `git-machete-3.9.0/completion/git-machete.completion.bash` & `git-machete-3.9.1/completion/git-machete.completion.bash`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/completion/git-machete.completion.zsh` & `git-machete-3.9.1/completion/git-machete.completion.zsh`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
   'anno:Manage custom annotations'
   'clean:Delete untracked and unmanaged branches and optionally check out open GitHub PRs'
   'delete-unmanaged:Delete local branches that are not present in the definition file'
   {diff,d}':Diff current working directory or a given branch against its fork point'
   'discover:Automatically discover tree of branch dependencies'
   {edit,e}':Edit the definition file'
   'file:Display the location of the definition file'
-  'fork-point:Display SHA of the fork point commit of a branch'
+  'fork-point:Display hash of the fork point commit of a branch'
   {go,g}':Check out the branch relative to the position of the current branch'
   'github:Creates, checks out and manages GitHub PRs while keeping them reflected in branch definition file'
   'help:Display this overview, or detailed help for a specified command'
   'is-managed:Check if the current branch is managed by git-machete (mostly for scripts)'
   'list:List all branches that fall into one of pre-defined categories (mostly for internal use)'
   {log,l}':Log the part of history specific to the given branch'
   'reapply:Rebase the current branch onto its own fork point'
```

### Comparing `git-machete-3.9.0/completion/git-machete.fish` & `git-machete-3.9.1/completion/git-machete.fish`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git-machete` & `git-machete-3.9.1/git-machete`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git_machete/cli.py` & `git-machete-3.9.1/git_machete/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -718,15 +718,15 @@
             machete_client.log(branch)
         elif cmd == "reapply":
             machete_client.read_definition_file(perform_interactive_slide_out=should_perform_interactive_slide_out)
             git.expect_no_operation_in_progress()
             current_branch = git.get_current_branch()
             if "fork_point" in parsed_cli:
                 machete_client.check_that_fork_point_is_ancestor_or_equal_to_tip_of_branch(
-                    fork_point_sha=cli_opts.opt_fork_point, branch=current_branch)
+                    fork_point_hash=cli_opts.opt_fork_point, branch=current_branch)
             git.rebase_onto_ancestor_commit(
                 current_branch,
                 cli_opts.opt_fork_point or machete_client.fork_point(
                     branch=current_branch,
                     use_overrides=True,
                     opt_no_detect_squash_merges=cli_opts.opt_no_detect_squash_merges),
                 cli_opts.opt_no_interactive_rebase)
@@ -762,15 +762,15 @@
                 opt_no_edit_merge=cli_opts.opt_no_edit_merge)
         elif cmd == "squash":
             machete_client.read_definition_file(perform_interactive_slide_out=should_perform_interactive_slide_out)
             git.expect_no_operation_in_progress()
             current_branch = git.get_current_branch()
             if "fork_point" in parsed_cli:
                 machete_client.check_that_fork_point_is_ancestor_or_equal_to_tip_of_branch(
-                    fork_point_sha=cli_opts.opt_fork_point, branch=current_branch)
+                    fork_point_hash=cli_opts.opt_fork_point, branch=current_branch)
             machete_client.squash(
                 current_branch=current_branch,
                 opt_fork_point=cli_opts.opt_fork_point or machete_client.fork_point(
                     branch=current_branch,
                     use_overrides=True,
                     opt_no_detect_squash_merges=cli_opts.opt_no_detect_squash_merges))
         elif cmd in {"status", alias_by_command["status"]}:
@@ -805,15 +805,15 @@
                 opt_start_from=cli_opts.opt_start_from,
                 opt_yes=cli_opts.opt_yes)
         elif cmd == "update":
             machete_client.read_definition_file(perform_interactive_slide_out=should_perform_interactive_slide_out)
             git.expect_no_operation_in_progress()
             if "fork_point" in parsed_cli:
                 machete_client.check_that_fork_point_is_ancestor_or_equal_to_tip_of_branch(
-                    fork_point_sha=cli_opts.opt_fork_point, branch=git.get_current_branch())
+                    fork_point_hash=cli_opts.opt_fork_point, branch=git.get_current_branch())
             machete_client.update(
                 opt_merge=cli_opts.opt_merge,
                 opt_no_edit_merge=cli_opts.opt_no_edit_merge,
                 opt_no_interactive_rebase=cli_opts.opt_no_interactive_rebase,
                 opt_fork_point=cli_opts.opt_fork_point)
 
     except KeyboardInterrupt:
```

### Comparing `git-machete-3.9.0/git_machete/client.py` & `git-machete-3.9.1/git_machete/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self._managed_branches: List[LocalBranchShortName] = []
         self._up_branch: Dict[LocalBranchShortName, Optional[LocalBranchShortName]] = {}  # TODO (#110): default dict with None
         self.__down_branches: Dict[LocalBranchShortName, Optional[List[LocalBranchShortName]]] = {}  # TODO (#110): default dict with []
         self.__indent: Optional[str] = None
         self.__roots: List[LocalBranchShortName] = []
         self.__annotations: Dict[LocalBranchShortName, str] = {}
         self.__empty_line_status: Optional[bool] = None
-        self.__branch_pairs_by_sha_in_reflog: Optional[Dict[FullCommitHash, Optional[List[BranchPair]]]] = None
+        self.__branch_pairs_by_hash_in_reflog: Optional[Dict[FullCommitHash, Optional[List[BranchPair]]]] = None
 
     @property
     def definition_file_path(self) -> str:
         return self._definition_file_path
 
     @property
     def managed_branches(self) -> List[LocalBranchShortName]:
@@ -65,16 +65,16 @@
     @up_branch.setter
     def up_branch(self, val: Dict[LocalBranchShortName, Optional[LocalBranchShortName]]) -> None:
         self._up_branch = val
 
     def expect_in_managed_branches(self, branch: LocalBranchShortName) -> None:
         if branch not in self.managed_branches:
             raise MacheteException(
-                f"Branch `{branch}` not found in the tree of branch dependencies."
-                f"\nUse `git machete add {branch}` or `git machete edit`")
+                f"Branch `{branch}` not found in the tree of branch dependencies.\n"
+                f"Use `git machete add {branch}` or `git machete edit`")
 
     def expect_at_least_one_managed_branch(self) -> None:
         if not self.__roots:
             self.__raise_no_branches_error()
 
     def __raise_no_branches_error(self) -> None:
         raise MacheteException(
@@ -506,15 +506,15 @@
 
             if len(children_of_the_last_branch_to_slide_out) > 1:
                 raise MacheteException(
                     "Last branch to slide out can't have more than one child branch "
                     "if option `--down-fork-point` is passed.")
 
             self.check_that_fork_point_is_ancestor_or_equal_to_tip_of_branch(
-                fork_point_sha=opt_down_fork_point,
+                fork_point_hash=opt_down_fork_point,
                 branch=children_of_the_last_branch_to_slide_out[0])
 
         # Verify that all "interior" slide-out branches have a single downstream pointing to the next slide-out
         for bu, bd in zip(branches_to_slide_out[:-1], branches_to_slide_out[1:]):
             dbs = self.__down_branches.get(bu)
             if not dbs or len(dbs) == 0:
                 raise MacheteException(f"No downstream branch defined for `{bu}`, cannot slide out")
@@ -575,15 +575,15 @@
                 f"`{branch}` does not have any downstream (child) branches to advance towards")
 
         def connected_with_green_edge(bd: LocalBranchShortName) -> bool:
             return bool(
                 not self.__is_merged_to_upstream(
                     bd, opt_no_detect_squash_merges=False) and
                 self.__git.is_ancestor_or_equal(branch.full_name(), bd.full_name()) and
-                (self.__get_overridden_fork_point(bd) or self.__git.get_commit_sha_by_revision(branch) == self.fork_point(bd, use_overrides=False, opt_no_detect_squash_merges=False)))
+                (self.__get_overridden_fork_point(bd) or self.__git.get_commit_hash_by_revision(branch) == self.fork_point(bd, use_overrides=False, opt_no_detect_squash_merges=False)))
 
         candidate_downstreams = list(filter(connected_with_green_edge, self.__down_branches[branch]))
         if not candidate_downstreams:
             raise MacheteException(
                 f"No downstream (child) branch of `{branch}` is connected to "
                 f"`{branch}` with a green edge")
         if len(candidate_downstreams) > 1:
@@ -707,15 +707,15 @@
             elif opt_merge:
                 needs_parent_sync = bool(
                     upstream and not self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()))
             else:  # using rebase
                 needs_parent_sync = bool(
                     upstream and
                     not (self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()) and
-                         (self.__git.get_commit_sha_by_revision(upstream) ==
+                         (self.__git.get_commit_hash_by_revision(upstream) ==
                           self.fork_point(
                               branch, use_overrides=True,
                               opt_no_detect_squash_merges=opt_no_detect_squash_merges)))
                 )
 
             if branch != current_branch and (needs_slide_out or needs_parent_sync or needs_remote_sync):
                 self.__print_new_line(False)
@@ -858,126 +858,147 @@
         if current_branch == self.managed_branches[-1]:
             msg: str = f"Reached branch {bold(current_branch)} which has no successor"
         else:
             msg = f"No successor of {bold(current_branch)} needs to be slid out or synced with upstream branch or remote"
         print(f"{msg}; nothing left to update")
         if not any_action_suggested and initial_branch not in self.__roots:
             print(fmt("Tip: `traverse` by default starts from the current branch, "
-                      "use flags (`--starts-from=`, `--whole` or `-w`, `-W`) to change this behavior.\n"
+                      "use flags (`--start-from=`, `--whole` or `-w`, `-W`) to change this behavior.\n"
                       "Further info under `git machete traverse --help`."))
         if opt_return_to == "here" or (
                 opt_return_to == "nearest-remaining" and nearest_remaining_branch == initial_branch):
             print(f"Returned to the initial branch {bold(initial_branch)}")
         elif opt_return_to == "nearest-remaining" and nearest_remaining_branch != initial_branch:
             print(
                 f"The initial branch {bold(initial_branch)} has been slid out. "
                 f"Returned to nearest remaining managed branch {bold(nearest_remaining_branch)}")
 
+    # TODO (#509): tidy up this method
     def status(
             self,
             *,
             warn_on_yellow_edges: bool,
             opt_list_commits: bool,
             opt_list_commits_with_hashes: bool,
             opt_no_detect_squash_merges: bool
     ) -> None:
-        dfs_res = []
+        dfs_res: List[Tuple[LocalBranchShortName, List[Optional[LocalBranchShortName]]]] = []
 
         def prefix_dfs(u_: LocalBranchShortName, accumulated_path_: List[Optional[LocalBranchShortName]]) -> None:
             dfs_res.append((u_, accumulated_path_))
             if self.__down_branches.get(u_):
                 for (v, nv) in zip(self.__down_branches[u_][:-1], self.__down_branches[u_][1:]):
                     prefix_dfs(v, accumulated_path_ + [nv])
                 prefix_dfs(self.__down_branches[u_][-1], accumulated_path_ + [None])
 
         for upstream in self.__roots:
             prefix_dfs(upstream, accumulated_path_=[])
 
         out = io.StringIO()
         edge_color: Dict[LocalBranchShortName, str] = {}
-        fp_sha_cached: Dict[LocalBranchShortName, Optional[FullCommitHash]] = {}  # TODO (#110): default dict with None
+        fp_hash_cached: Dict[LocalBranchShortName, Optional[FullCommitHash]] = {}  # TODO (#110): default dict with None
         fp_branches_cached: Dict[LocalBranchShortName, List[BranchPair]] = {}
 
-        def fp_sha(branch_: LocalBranchShortName) -> Optional[FullCommitHash]:
-            if branch not in fp_sha_cached:
+        def fp_hash(branch_: LocalBranchShortName) -> Optional[FullCommitHash]:
+            if branch not in fp_hash_cached:
                 try:
                     # We're always using fork point overrides, even when status
                     # is launched from discover().
-                    fp_sha_cached[branch_], fp_branches_cached[branch_] = self.__fork_point_and_containing_branch_pairs(
+                    fp_hash_cached[branch_], fp_branches_cached[branch_] = self.__fork_point_and_containing_branch_pairs(
                         branch_,
                         use_overrides=True,
                         opt_no_detect_squash_merges=opt_no_detect_squash_merges)
                 except MacheteException:
-                    fp_sha_cached[branch_], fp_branches_cached[branch_] = None, []
-            return fp_sha_cached[branch_]
+                    fp_hash_cached[branch_], fp_branches_cached[branch_] = None, []
+            return fp_hash_cached[branch_]
 
         # Edge colors need to be precomputed
         # in order to render the leading parts of lines properly.
+        branch: LocalBranchShortName
         for branch in self.up_branch:
             upstream = self.up_branch[branch]
             if self.is_merged_to(
                     branch=branch,
                     upstream=upstream,
                     opt_no_detect_squash_merges=opt_no_detect_squash_merges):
                 edge_color[branch] = AnsiEscapeCodes.DIM
             elif not self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()):
                 edge_color[branch] = AnsiEscapeCodes.RED
-            elif self.__get_overridden_fork_point(branch) or self.__git.get_commit_sha_by_revision(upstream) == fp_sha(branch):
+            elif self.__get_overridden_fork_point(branch) or self.__git.get_commit_hash_by_revision(upstream) == fp_hash(branch):
                 edge_color[branch] = AnsiEscapeCodes.GREEN
             else:
                 edge_color[branch] = AnsiEscapeCodes.YELLOW
 
         currently_rebased_branch = self.__git.get_currently_rebased_branch_or_none()
         currently_checked_out_branch = self.__git.get_currently_checked_out_branch_or_none()
 
         hook_path = self.__git.get_hook_path("machete-status-branch")
         hook_executable = self.__git.check_hook_executable(hook_path)
 
         def print_line_prefix(branch_: LocalBranchShortName, suffix: str) -> None:
             out.write("  ")
-            for p in accumulated_path[:-1]:
-                if not p:
+            for sibling in next_sibling_of_ancestor[:-1]:
+                if not sibling:
                     out.write("  ")
                 else:
-                    out.write(colored(f"{utils.get_vertical_bar()} ", edge_color[p]))
+                    out.write(colored(f"{utils.get_vertical_bar()} ", edge_color[sibling]))
             out.write(colored(suffix, edge_color[branch_]))
 
-        for branch, accumulated_path in dfs_res:
+        next_sibling_of_ancestor: List[Optional[LocalBranchShortName]]
+        for branch, next_sibling_of_ancestor in dfs_res:
             if branch in self.up_branch:
                 print_line_prefix(branch, f"{utils.get_vertical_bar()} \n")
                 if opt_list_commits:
-                    if not fp_sha(branch):
+                    if not fp_hash(branch):
                         # Rare case, but can happen e.g. due to reflog expiry.
                         commits: List[GitLogEntry] = []
                     elif edge_color[branch] == AnsiEscapeCodes.DIM:
                         commits = []
                     elif edge_color[branch] == AnsiEscapeCodes.YELLOW:
                         commits = self.__git.get_commits_between(self.up_branch[branch].full_name(), branch.full_name())
                     else:  # (AnsiEscapeCodes.RED, AnsiEscapeCodes.GREEN):
-                        commits = self.__git.get_commits_between(fp_sha(branch), branch.full_name())
+                        commits = self.__git.get_commits_between(fp_hash(branch), branch.full_name())
 
                     for commit in commits:
-                        if commit.hash == fp_sha(branch):
+                        if commit.hash == fp_hash(branch):
                             # fp_branches_cached will already be there thanks to
-                            # the above call to 'fp_sha'.
+                            # the above call to 'fp_hash'.
                             fp_branches_formatted: str = " and ".join(
                                 sorted(underline(lb_or_rb) for lb, lb_or_rb in fp_branches_cached[branch]))
                             fp_suffix: str = " %s %s %s seems to be a part of the unique history of %s" % \
                                              (colored(utils.get_right_arrow(), AnsiEscapeCodes.RED), colored("fork point ???", AnsiEscapeCodes.RED),
                                               "this commit" if opt_list_commits_with_hashes else f"commit {commit.short_hash}",
                                               fp_branches_formatted)
                         else:
                             fp_suffix = ''
                         print_line_prefix(branch, utils.get_vertical_bar())
                         out.write(" %s%s%s\n" % (
                                   f"{dim(commit.short_hash)}  " if opt_list_commits_with_hashes else "", dim(commit.subject),
                                   fp_suffix))
-                elbow_ascii_only: Dict[str, str] = {AnsiEscapeCodes.DIM: "m-", AnsiEscapeCodes.RED: "x-", AnsiEscapeCodes.GREEN: "o-", AnsiEscapeCodes.YELLOW: "?-"}
-                elbow: str = u"└─" if not utils.ascii_only else elbow_ascii_only[edge_color[branch]]
-                print_line_prefix(branch, elbow)
+
+                junction: str
+                if utils.ascii_only:
+                    junction_ascii_only: Dict[str, str] = {
+                        AnsiEscapeCodes.DIM: "m-",
+                        AnsiEscapeCodes.RED: "x-",
+                        AnsiEscapeCodes.GREEN: "o-",
+                        AnsiEscapeCodes.YELLOW: "?-"}
+                    junction = junction_ascii_only[edge_color[branch]]
+                else:
+                    next_sibling_of_branch: Optional[LocalBranchShortName] = next_sibling_of_ancestor[-1]
+                    if next_sibling_of_branch and edge_color[next_sibling_of_branch] == edge_color[branch]:
+                        junction = u"├─"
+                    else:
+                        # The three-legged turnstile looks pretty bad when the upward and rightward leg
+                        # have a different color than the downward leg.
+                        # It's better to use a two-legged elbow
+                        # in case `edge_color[next_sibling_of_branch] != edge_color[branch]`,
+                        # at the expense of a little gap to the elbow/turnstile below.
+                        junction = u"└─"
+                print_line_prefix(branch, junction)
             else:
                 if branch != dfs_res[0][0]:
                     out.write("\n")
                 out.write("  ")
 
             if branch in (currently_checked_out_branch, currently_rebased_branch):  # i.e. if branch is the current branch (checked out or being rebased)
                 if branch == currently_rebased_branch:
@@ -1028,24 +1049,24 @@
         yellow_edge_branches = [k for k, v in edge_color.items() if v == AnsiEscapeCodes.YELLOW]
         if yellow_edge_branches and warn_on_yellow_edges:
             if len(yellow_edge_branches) == 1:
                 first_part = f"yellow edge indicates that fork point for `{yellow_edge_branches[0]}` is probably incorrectly inferred,\n" \
                              f"or that some extra branch should be between `{self.up_branch[LocalBranchShortName.of(yellow_edge_branches[0])]}` and `{yellow_edge_branches[0]}`"
             else:
                 affected_branches = ", ".join(map(lambda x: f"`{x}`", yellow_edge_branches))
-                first_part = f"yellow edges indicate that fork points for {affected_branches} are probably incorrectly inferred" \
+                first_part = f"yellow edges indicate that fork points for {affected_branches} are probably incorrectly inferred,\n" \
                              f"or that some extra branch should be added between each of these branches and its parent"
 
             if not opt_list_commits:
                 second_part = "Run `git machete status --list-commits` or `git machete status --list-commits-with-hashes` to see more details"
             elif len(yellow_edge_branches) == 1:
-                second_part = f"Consider using `git machete fork-point --override-to=<revision>|--override-to-inferred|--override-to-parent {yellow_edge_branches[0]}`\n" \
+                second_part = f"Consider using `git machete fork-point --override-to=<revision>|--override-to-inferred|--override-to-parent {yellow_edge_branches[0]}`,\n" \
                               f"or reattaching `{yellow_edge_branches[0]}` under a different parent branch"
             else:
-                second_part = "Consider using `git machete fork-point --override-to=<revision>|--override-to-inferred|--override-to-parent <branch>` for each affected branch" \
+                second_part = "Consider using `git machete fork-point --override-to=<revision>|--override-to-inferred|--override-to-parent <branch>` for each affected branch,\n" \
                               "or reattaching the affected branches under different parent branches"
 
             print("", file=sys.stderr)
             warn(f"{first_part}.\n\n{second_part}.")
 
     def delete_unmanaged(self, *, opt_yes: bool) -> None:
         print(bold('Checking for unmanaged branches...'))
@@ -1094,63 +1115,63 @@
                 f"variable or edit {self._definition_file_path} directly.")
         return utils.run_cmd(default_editor_name, self._definition_file_path)
 
     def __fork_point_and_containing_branch_pairs(self, branch: LocalBranchShortName, use_overrides: bool, opt_no_detect_squash_merges: bool) -> Tuple[FullCommitHash, List[BranchPair]]:
         upstream = self.up_branch.get(branch)
 
         if use_overrides:
-            overridden_fp_sha = self.__get_overridden_fork_point(branch)
-            if overridden_fp_sha:
-                if upstream and self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()) and not self.__git.is_ancestor_or_equal(upstream.full_name(), overridden_fp_sha.full_name()):
+            overridden_fp_hash = self.__get_overridden_fork_point(branch)
+            if overridden_fp_hash:
+                if upstream and self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()) and not self.__git.is_ancestor_or_equal(upstream.full_name(), overridden_fp_hash.full_name()):
                     # We need to handle the case when branch is a descendant of upstream,
                     # but the fork point of branch is overridden to a commit that
                     # is NOT a descendant of upstream. In this case it's more
-                    # reasonable to assume that upstream (and not overridden_fp_sha)
+                    # reasonable to assume that upstream (and not overridden_fp_hash)
                     # is the fork point.
-                    debug(f"{branch} is descendant of its upstream {upstream}, but overridden fork point commit {overridden_fp_sha} is NOT a descendant of {upstream}; falling back to {upstream} as fork point")
-                    return self.__git.get_commit_sha_by_revision(upstream), []
+                    debug(f"{branch} is descendant of its upstream {upstream}, but overridden fork point commit {overridden_fp_hash} is NOT a descendant of {upstream}; falling back to {upstream} as fork point")
+                    return self.__git.get_commit_hash_by_revision(upstream), []
                 else:
-                    debug(f"fork point of {branch} is overridden to {overridden_fp_sha}; skipping inference")
-                    return overridden_fp_sha, []
+                    debug(f"fork point of {branch} is overridden to {overridden_fp_hash}; skipping inference")
+                    return overridden_fp_hash, []
 
         try:
-            fp_sha, containing_branch_pairs = next(self.__match_log_to_filtered_reflogs(branch))
+            fp_hash, containing_branch_pairs = next(self.__match_log_to_filtered_reflogs(branch))
         except StopIteration:
             if upstream and self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()):
                 debug(f"cannot find fork point, but {branch} is descendant of its upstream {upstream}; falling back to {upstream} as fork point")
-                return self.__git.get_commit_sha_by_revision(upstream), []
+                return self.__git.get_commit_hash_by_revision(upstream), []
             else:
                 raise MacheteException(f"Cannot find fork point for branch `{branch}`")
         else:
-            debug("commit {fp_sha} is the most recent point in history of {branch} to occur on "
+            debug("commit {fp_hash} is the most recent point in history of {branch} to occur on "
                   "filtered reflog of any other branch or its remote counterpart "
                   f"(specifically: {' and '.join(map(utils.get_second, containing_branch_pairs))})")
 
-            if upstream and self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()) and not self.__git.is_ancestor_or_equal(upstream.full_name(), fp_sha.full_name()):
+            if upstream and self.__git.is_ancestor_or_equal(upstream.full_name(), branch.full_name()) and not self.__git.is_ancestor_or_equal(upstream.full_name(), fp_hash.full_name()):
                 # That happens very rarely in practice (typically current head
                 # of any branch, including upstream, should occur on the reflog
                 # of this branch, thus is_ancestor(upstream, branch) should imply
                 # is_ancestor(upstream, FP(branch)), but it's still possible in
                 # case reflog of upstream is incomplete for whatever reason.
-                debug(f"{upstream} is descendant of its upstream {branch}, but inferred fork point commit {fp_sha} is NOT a descendant of {upstream}; falling back to {upstream} as fork point")
-                return self.__git.get_commit_sha_by_revision(upstream), []
+                debug(f"{upstream} is descendant of its upstream {branch}, but inferred fork point commit {fp_hash} is NOT a descendant of {upstream}; falling back to {upstream} as fork point")
+                return self.__git.get_commit_hash_by_revision(upstream), []
             else:
-                debug(f"choosing commit {fp_sha} as fork point")
-                return fp_sha, containing_branch_pairs
+                debug(f"choosing commit {fp_hash} as fork point")
+                return fp_hash, containing_branch_pairs
 
     def fork_point(
             self,
             branch: LocalBranchShortName,
             use_overrides: bool,
             *,
             opt_no_detect_squash_merges: bool
     ) -> Optional[FullCommitHash]:
-        sha, containing_branch_pairs = self.__fork_point_and_containing_branch_pairs(
+        hash, containing_branch_pairs = self.__fork_point_and_containing_branch_pairs(
             branch, use_overrides, opt_no_detect_squash_merges=opt_no_detect_squash_merges)
-        return FullCommitHash.of(sha) if sha else None
+        return FullCommitHash.of(hash) if hash else None
 
     def diff(self, *, branch: Optional[LocalBranchShortName], opt_stat: bool) -> None:
         fp: FullCommitHash = self.fork_point(
             branch if branch else self.__git.get_current_branch(),
             use_overrides=True, opt_no_detect_squash_merges=False)
         self.__git.display_diff(
             branch=branch,
@@ -1306,62 +1327,62 @@
                           GIT_AUTHOR_EMAIL=earliest_author_email,
                           GIT_AUTHOR_NAME=earliest_author_name)
         # Using `git commit-tree` since it's cleaner than any high-level command
         # like `git merge --squash` or `git rebase --interactive`.
         # The tree (HEAD^{tree}) argument must be passed as first,
         # otherwise the entire `commit-tree` will fail on some ancient supported
         # versions of git (at least on v1.7.10).
-        squashed_sha = FullCommitHash.of(self.__git.commit_tree_with_given_parent_and_message_and_env(
+        squashed_hash = FullCommitHash.of(self.__git.commit_tree_with_given_parent_and_message_and_env(
             opt_fork_point, earliest_full_body, author_env).strip())
 
         # This can't be done with `git reset` since it doesn't allow for a custom reflog message.
         # Even worse, reset's reflog message would be filtered out in our fork point algorithm,
         # so the squashed commit would not even be considered to "belong"
         # (in the FP sense) to the current branch's history.
         self.__git.update_head_ref_to_new_hash_with_reflog_subject(
-            squashed_sha, f"squash: {earliest_commit.subject}")
+            squashed_hash, f"squash: {earliest_commit.subject}")
 
         print(f"Squashed {len(commits)} commits:")
         print()
         for commit in commits:
             print(f"\t{commit.short_hash} {commit.subject}")
 
         print()
         print("To restore the original pre-squash commit, run:")
         print()
         print(fmt(f"\t`git reset {commits[-1].hash}`"))
 
     def filtered_reflog(self, branch: AnyBranchName) -> List[FullCommitHash]:
-        def is_excluded_reflog_subject(sha_: str, gs_: str) -> bool:
+        def is_excluded_reflog_subject(hash_: str, gs_: str) -> bool:
             is_excluded = (gs_.startswith("branch: Created from") or
                            gs_ == f"branch: Reset to {branch}" or
                            gs_ == "branch: Reset to HEAD" or
                            gs_.startswith("reset: moving to ") or
                            gs_.startswith("fetch . ") or
                            # The rare case of a no-op rebase, the exact wording
                            # likely depends on git version
-                           gs_ == f"rebase finished: {branch.full_name()} onto {sha_}" or
-                           gs_ == f"rebase -i (finish): {branch.full_name()} onto {sha_}"
+                           gs_ == f"rebase finished: {branch.full_name()} onto {hash_}" or
+                           gs_ == f"rebase -i (finish): {branch.full_name()} onto {hash_}"
                            )
             if is_excluded:
                 debug("skipping reflog entry")
             return is_excluded
 
         branch_reflog = self.__git.get_reflog(branch.full_name())
         if not branch_reflog:
             return []
 
-        earliest_sha, earliest_gs = branch_reflog[-1]  # Note that the reflog is returned from latest to earliest entries.
-        shas_to_exclude = set()
+        earliest_hash, earliest_gs = branch_reflog[-1]  # Note that the reflog is returned from latest to earliest entries.
+        hashes_to_exclude = set()
         if earliest_gs.startswith("branch: Created from"):
-            debug(f"skipping any reflog entry with the hash equal to the hash of the earliest (branch creation) entry: {earliest_sha}")
-            shas_to_exclude.add(earliest_sha)
+            debug(f"skipping any reflog entry with the hash equal to the hash of the earliest (branch creation) entry: {earliest_hash}")
+            hashes_to_exclude.add(earliest_hash)
 
-        result = [sha for (sha, gs) in branch_reflog if
-                  sha not in shas_to_exclude and not is_excluded_reflog_subject(sha, gs)]
+        result = [hash for (hash, gs) in branch_reflog if
+                  hash not in hashes_to_exclude and not is_excluded_reflog_subject(hash, gs)]
         debug("computed filtered reflog (= reflog without branch creation "
               "and branch reset events irrelevant for fork point/upstream inference): %s\n" % (", ".join(result) or "<empty>"))
         return result
 
     def sync_annotations_to_github_prs(self) -> None:
 
         url_for_remote: Dict[str, str] = {remote: self.__git.get_url_of_remote(remote) for remote in
@@ -1438,74 +1459,74 @@
             raise MacheteException(f"Invalid direction: `{param}`; expected: {allowed_directions(allow_current)}")
 
     def __match_log_to_filtered_reflogs(self, branch: LocalBranchShortName) -> Generator[Tuple[FullCommitHash, List[BranchPair]], None, None]:
 
         if branch not in self.__git.get_local_branches():
             raise MacheteException(f"`{branch}` is not a local branch")
 
-        if self.__branch_pairs_by_sha_in_reflog is None:
+        if self.__branch_pairs_by_hash_in_reflog is None:
             def generate_entries() -> Generator[Tuple[FullCommitHash, BranchPair], None, None]:
                 for lb in self.__git.get_local_branches():
-                    lb_shas = set()
-                    for sha_ in self.filtered_reflog(lb):
-                        lb_shas.add(sha_)
-                        yield FullCommitHash.of(sha_), BranchPair(lb, lb)
+                    lb_hashes = set()
+                    for hash_ in self.filtered_reflog(lb):
+                        lb_hashes.add(hash_)
+                        yield FullCommitHash.of(hash_), BranchPair(lb, lb)
                     remote_branch = self.__git.get_combined_counterpart_for_fetching_of_branch(lb)
                     if remote_branch:
-                        for sha_ in self.filtered_reflog(remote_branch):
-                            if sha_ not in lb_shas:
-                                yield FullCommitHash.of(sha_), BranchPair(lb, remote_branch)
-
-            self.__branch_pairs_by_sha_in_reflog = {}
-            for sha, branch_pair in generate_entries():
-                if sha in self.__branch_pairs_by_sha_in_reflog:
+                        for hash_ in self.filtered_reflog(remote_branch):
+                            if hash_ not in lb_hashes:
+                                yield FullCommitHash.of(hash_), BranchPair(lb, remote_branch)
+
+            self.__branch_pairs_by_hash_in_reflog = {}
+            for hash, branch_pair in generate_entries():
+                if hash in self.__branch_pairs_by_hash_in_reflog:
                     # The practice shows that it's rather unlikely for a given
                     # commit to appear on filtered reflogs of two unrelated branches
                     # ("unrelated" as in, not a local branch and its remote
                     # counterpart) but we need to handle this case anyway.
-                    self.__branch_pairs_by_sha_in_reflog[sha] += [branch_pair]
+                    self.__branch_pairs_by_hash_in_reflog[hash] += [branch_pair]
                 else:
-                    self.__branch_pairs_by_sha_in_reflog[sha] = [branch_pair]
+                    self.__branch_pairs_by_hash_in_reflog[hash] = [branch_pair]
 
             def log_result() -> Generator[str, None, None]:
                 branch_pairs_: List[BranchPair]
-                sha_: FullCommitHash
-                for sha_, branch_pairs_ in self.__branch_pairs_by_sha_in_reflog.items():
+                hash_: FullCommitHash
+                for hash_, branch_pairs_ in self.__branch_pairs_by_hash_in_reflog.items():
                     def branch_pair_to_str(lb: str, lb_or_rb: str) -> str:
                         return lb if lb == lb_or_rb else f"{lb_or_rb} (remote counterpart of {lb})"
 
                     joined_branch_pairs = ", ".join(map(tupled(branch_pair_to_str), branch_pairs_))
-                    yield dim(f"{sha_} => {joined_branch_pairs}")
+                    yield dim(f"{hash_} => {joined_branch_pairs}")
 
-            debug("branches containing the given SHA in their filtered reflog: \n%s\n" % "\n".join(log_result()))
+            debug("branches containing the given hash in their filtered reflog: \n%s\n" % "\n".join(log_result()))
 
-        branch_full_hash: FullCommitHash = self.__git.get_commit_sha_by_revision(branch)
+        branch_full_hash: FullCommitHash = self.__git.get_commit_hash_by_revision(branch)
 
-        for sha in self.__git.spoonfeed_log_shas(branch_full_hash):
-            if sha in self.__branch_pairs_by_sha_in_reflog:
+        for hash in self.__git.spoonfeed_log_hashes(branch_full_hash):
+            if hash in self.__branch_pairs_by_hash_in_reflog:
                 # The entries must be sorted by lb_or_rb to make sure the
                 # upstream inference is deterministic (and does not depend on the
                 # order in which `generate_entries` iterated through the local branches).
-                branch_pairs: List[BranchPair] = self.__branch_pairs_by_sha_in_reflog[sha]
+                branch_pairs: List[BranchPair] = self.__branch_pairs_by_hash_in_reflog[hash]
 
                 def lb_is_not_b(lb: str, lb_or_rb: str) -> bool:
                     return lb != branch
 
                 containing_branch_pairs = sorted(filter(tupled(lb_is_not_b), branch_pairs), key=get_second)
                 if containing_branch_pairs:
-                    debug(f"commit {sha} found in filtered reflog of {' and '.join(map(get_second, branch_pairs))}")
-                    yield sha, containing_branch_pairs
+                    debug(f"commit {hash} found in filtered reflog of {' and '.join(map(get_second, branch_pairs))}")
+                    yield hash, containing_branch_pairs
                 else:
-                    debug(f"commit {sha} found only in filtered reflog of {' and '.join(map(get_second, branch_pairs))}; ignoring")
+                    debug(f"commit {hash} found only in filtered reflog of {' and '.join(map(get_second, branch_pairs))}; ignoring")
             else:
-                debug(f"commit {sha} not found in any filtered reflog")
+                debug(f"commit {hash} not found in any filtered reflog")
 
     def __infer_upstream(self, branch: LocalBranchShortName, condition: Callable[[LocalBranchShortName], bool] = lambda upstream: True, reject_reason_message: str = "") -> Optional[LocalBranchShortName]:
-        for sha, containing_branch_pairs in self.__match_log_to_filtered_reflogs(branch):
-            debug(f"commit {sha} found in filtered reflog of {' and '.join(map(get_second, containing_branch_pairs))}")
+        for hash, containing_branch_pairs in self.__match_log_to_filtered_reflogs(branch):
+            debug(f"commit {hash} found in filtered reflog of {' and '.join(map(get_second, containing_branch_pairs))}")
 
             for candidate, original_matched_branch in containing_branch_pairs:
                 if candidate != original_matched_branch:
                     debug(f"upstream candidate is {candidate}, which is the local counterpart of {original_matched_branch}")
 
                 if condition(candidate):
                     debug(f"upstream candidate {candidate} accepted")
@@ -1537,82 +1558,83 @@
         if to and not while_descendant_of:
             warn(f"{to_key} config is set but {while_descendant_of_key} config is missing")
             return None
         if not to and while_descendant_of:
             warn(f"{while_descendant_of_key} config is set but {to_key} config is missing")
             return None
 
-        to_sha: Optional[FullCommitHash] = self.__git.get_commit_sha_by_revision(to)
-        while_descendant_of_sha: Optional[FullCommitHash] = self.__git.get_commit_sha_by_revision(while_descendant_of)
-        if not to_sha or not while_descendant_of_sha:
-            if not to_sha:
+        to_hash: Optional[FullCommitHash] = self.__git.get_commit_hash_by_revision(to)
+        while_descendant_of_hash: Optional[FullCommitHash] = self.__git.get_commit_hash_by_revision(while_descendant_of)
+        if not to_hash or not while_descendant_of_hash:
+            if not to_hash:
                 warn(f"{to_key} config value `{to}` does not point to a valid commit")
-            if not while_descendant_of_sha:
+            if not while_descendant_of_hash:
                 warn(f"{while_descendant_of_key} config value `{while_descendant_of}` does not point to a valid commit")
             return None
         # This check needs to be performed every time the config is retrieved.
         # We can't rely on the values being validated in set_fork_point_override(),
         # since the config could have been modified outside of git-machete.
-        if not self.__git.is_ancestor_or_equal(to_sha.full_name(), while_descendant_of_sha.full_name()):
+        if not self.__git.is_ancestor_or_equal(to_hash.full_name(), while_descendant_of_hash.full_name()):
             warn(
-                f"commit {self.__git.get_short_commit_sha_by_revision(to)} pointed by {to_key} config "
-                f"is not an ancestor of commit {self.__git.get_short_commit_sha_by_revision(while_descendant_of)} "
+                f"commit {self.__git.get_short_commit_hash_by_revision(to)} pointed by {to_key} config "
+                f"is not an ancestor of commit {self.__git.get_short_commit_hash_by_revision(while_descendant_of)} "
                 f"pointed by {while_descendant_of_key} config")
             return None
-        return ForkPointOverrideData(to_sha, while_descendant_of_sha)
+        return ForkPointOverrideData(to_hash, while_descendant_of_hash)
 
     def __get_overridden_fork_point(self, branch: LocalBranchShortName) -> Optional[FullCommitHash]:
         override_data: ForkPointOverrideData = self.__get_fork_point_override_data(branch)
         if not override_data:
             return None
 
         to, while_descendant_of = override_data.to_hash, override_data.while_descendant_of_hash
         # Note that this check is distinct from the is_ancestor check performed in
         # get_fork_point_override_data.
         # While the latter checks the sanity of fork point override configuration,
         # the former checks if the override still applies to wherever the given
         # branch currently points.
         if not self.__git.is_ancestor_or_equal(while_descendant_of.full_name(), branch.full_name()):
             warn(fmt(
-                f"since branch <b>{branch}</b> is no longer a descendant of commit {self.__git.get_short_commit_sha_by_revision(while_descendant_of)}, ",
-                f"the fork point override to commit {self.__git.get_short_commit_sha_by_revision(to)} no longer applies.\n",
+                f"since branch <b>{branch}</b> is no longer a descendant of commit {self.__git.get_short_commit_hash_by_revision(while_descendant_of)}, ",
+                f"the fork point override to commit {self.__git.get_short_commit_hash_by_revision(to)} no longer applies.\n",
                 "Consider running:\n",
                 f"  `git machete fork-point --unset-override {branch}`\n"))
             return None
         debug(f"since branch {branch} is descendant of while_descendant_of={while_descendant_of}, fork point of {branch} is overridden to {to}")
         return to
 
     def unset_fork_point_override(self, branch: LocalBranchShortName) -> None:
         self.__git.unset_config_attr(self.config_key_for_override_fork_point_to(branch))
         self.__git.unset_config_attr(self.config_key_for_override_fork_point_while_descendant_of(branch))
 
     def set_fork_point_override(self, branch: LocalBranchShortName, to_revision: AnyRevision) -> None:
         if branch not in self.__git.get_local_branches():
             raise MacheteException(f"`{branch}` is not a local branch")
-        to_sha = self.__git.get_commit_sha_by_revision(to_revision)
-        if not to_sha:
+        to_hash = self.__git.get_commit_hash_by_revision(to_revision)
+        if not to_hash:
             raise MacheteException(f"Cannot find revision {to_revision}")
-        if not self.__git.is_ancestor_or_equal(to_sha.full_name(), branch.full_name()):
+        if not self.__git.is_ancestor_or_equal(to_hash.full_name(), branch.full_name()):
             raise MacheteException(
                 f"Cannot override fork point: {self.__git.get_revision_repr(to_revision)} is not an ancestor of {branch}")
 
         to_key = self.config_key_for_override_fork_point_to(branch)
-        self.__git.set_config_attr(to_key, to_sha)
+        self.__git.set_config_attr(to_key, to_hash)
 
         while_descendant_of_key = self.config_key_for_override_fork_point_while_descendant_of(branch)
-        branch_sha = self.__git.get_commit_sha_by_revision(branch)
-        self.__git.set_config_attr(while_descendant_of_key, branch_sha)
+        branch_hash = self.__git.get_commit_hash_by_revision(branch)
+        self.__git.set_config_attr(while_descendant_of_key, branch_hash)
 
-        print(fmt(f"Fork point for <b>{branch}</b> is overridden to <b>"
-                  f"{self.__git.get_revision_repr(to_revision)}</b>.\n",
+        print(fmt(f"Fork point for <b>{branch}</b> is overridden to "
+                  f"<b>{self.__git.get_revision_repr(to_revision)}</b>.\n",
                   f"This applies as long as {branch} points to (or is descendant of)"
                   " its current head (commit "
-                  f"{self.__git.get_short_commit_sha_by_revision(branch_sha)}).\n\n",
-                  f"This information is stored under git config keys:\n  * `{to_key}"
-                  f"`\n  * `{while_descendant_of_key}`\n\n",
+                  f"{self.__git.get_short_commit_hash_by_revision(branch_hash)}).\n\n",
+                  f"This information is stored under git config keys:\n"
+                  f"  * `{to_key}`\n"
+                  f"  * `{while_descendant_of_key}`\n\n",
                   "To unset this override, use:\n  `git machete fork-point "
                   f"--unset-override {branch}`"))
 
     def __pick_remote(
             self,
             *,
             branch: LocalBranchShortName,
@@ -1660,15 +1682,15 @@
             opt_push_tracked: bool,
             opt_yes: bool
     ) -> None:
         rems: List[str] = self.__git.get_remotes()
         can_pick_other_remote = len(rems) > 1 and not is_called_from_create_pr
         other_remote_choice = "o[ther-remote]" if can_pick_other_remote else ""
         remote_branch = RemoteBranchShortName.of(f"{new_remote}/{branch}")
-        if not self.__git.get_commit_sha_by_revision(remote_branch):
+        if not self.__git.get_commit_hash_by_revision(remote_branch):
             choices = get_pretty_choices(*('y', 'N', 'q', 'yq', other_remote_choice) if is_called_from_traverse else ('y', 'Q', other_remote_choice))
             ask_message = f"Push untracked branch {bold(branch)} to {bold(new_remote)}?" + choices
             ask_opt_yes_message = f"Pushing untracked branch {bold(branch)} to {bold(new_remote)}..."
             ans = self.ask_if(
                 ask_message,
                 ask_opt_yes_message,
                 opt_yes=opt_yes,
@@ -1827,24 +1849,24 @@
         except ValueError:
             sys.exit(1)
         if index not in range(len(choices)):
             raise MacheteException(f"Invalid index: {index + 1}")
         return choices[index]
 
     def flush_caches(self) -> None:
-        self.__branch_pairs_by_sha_in_reflog = None
+        self.__branch_pairs_by_hash_in_reflog = None
         self.__git.flush_caches()
 
     def check_that_fork_point_is_ancestor_or_equal_to_tip_of_branch(
-            self, fork_point_sha: AnyRevision, branch: AnyBranchName) -> None:
+            self, fork_point_hash: AnyRevision, branch: AnyBranchName) -> None:
         if not self.__git.is_ancestor_or_equal(
-                earlier_revision=fork_point_sha.full_name(),
+                earlier_revision=fork_point_hash.full_name(),
                 later_revision=branch.full_name()):
             raise MacheteException(
-                f"Fork point {fork_point_sha} is not ancestor of or the tip "
+                f"Fork point {fork_point_hash} is not ancestor of or the tip "
                 f"of the {branch} branch.")
 
     def checkout_github_prs(self,
                             pr_nos: Optional[List[int]],
                             *,
                             all_opened_prs: bool = False,
                             my_opened_prs: bool = False,
```

### Comparing `git-machete-3.9.0/git_machete/constants.py` & `git-machete-3.9.1/git_machete/constants.py`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git_machete/docs.py` & `git-machete-3.9.1/git_machete/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
           git machete fork-point --override-to=<revision>|--override-to-inferred|--override-to-parent [<branch>]
           git machete fork-point --unset-override [<branch>]</b>
 
         Note: in all three forms, if no <branch> is specified, the currently checked out branch is assumed.
         The branch in question does not need to occur in the definition file.
 
 
-        Without any option, displays full SHA of the fork point commit for the <branch>.
+        Without any option, displays full hash of the fork point commit for the <branch>.
         Fork point of the given <branch> is the commit at which the history of the <branch> diverges from history of any other branch.
 
         Fork point is assumed by many `git machete` commands as the place where the unique history of the <branch> starts.
         The range of commits between the fork point and the tip of the given branch is, for instance:
         * listed for each branch by `git machete status --list-commits`
         * passed to `git rebase` by `git machete reapply`/`slide-out`/`traverse`/`update`
         * provided to `git diff`/`log` by `git machete diff`/`log`.
```

### Comparing `git-machete-3.9.0/git_machete/exceptions.py` & `git-machete-3.9.1/git_machete/exceptions.py`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git_machete/git_operations.py` & `git-machete-3.9.1/git_machete/git_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,22 +175,22 @@
         self._root_dir: Optional[str] = None
         self._main_git_dir: Optional[str] = None
         self._worktree_git_dir: Optional[str] = None
         self.__fetch_done_for: Set[str] = set()
         self.__config_cached: Optional[Dict[str, str]] = None
         self.__remotes_cached: Optional[List[str]] = None
         self.__counterparts_for_fetching_cached: Optional[Dict[LocalBranchShortName, Optional[RemoteBranchShortName]]] = None  # TODO (#110): default dict with None
-        self.__short_commit_sha_by_revision_cached: Dict[AnyRevision, ShortCommitHash] = {}
-        self.__tree_sha_by_commit_sha_cached: Optional[Dict[FullCommitHash, Optional[FullTreeHash]]] = None  # TODO (#110): default dict with None
-        self.__commit_sha_by_revision_cached: Optional[Dict[AnyRevision, Optional[FullCommitHash]]] = None  # TODO (#110): default dict with None
+        self.__short_commit_hash_by_revision_cached: Dict[AnyRevision, ShortCommitHash] = {}
+        self.__tree_hash_by_commit_hash_cached: Optional[Dict[FullCommitHash, Optional[FullTreeHash]]] = None  # TODO (#110): default dict with None
+        self.__commit_hash_by_revision_cached: Optional[Dict[AnyRevision, Optional[FullCommitHash]]] = None  # TODO (#110): default dict with None
         self.__committer_unix_timestamp_by_revision_cached: Optional[Dict[AnyRevision, int]] = None  # TODO (#110): default dict with 0
         self.__local_branches_cached: Optional[List[LocalBranchShortName]] = None
         self.__remote_branches_cached: Optional[List[RemoteBranchShortName]] = None
-        self.__initial_log_shas_cached: Dict[FullCommitHash, List[FullCommitHash]] = {}
-        self.__remaining_log_shas_cached: Dict[FullCommitHash, List[FullCommitHash]] = {}
+        self.__initial_log_hashes_cached: Dict[FullCommitHash, List[FullCommitHash]] = {}
+        self.__remaining_log_hashes_cached: Dict[FullCommitHash, List[FullCommitHash]] = {}
         self.__reflogs_cached: Optional[Dict[AnyBranchName, Optional[List[GitReflogEntry]]]] = None
         self.__merge_base_cached: Dict[Tuple[FullCommitHash, FullCommitHash], FullCommitHash] = {}
         self.__is_equivalent_tree_reachable_cached: Dict[Tuple[FullCommitHash, FullCommitHash], bool] = {}
 
     @staticmethod
     def _run_git(git_cmd: str, *args: str, **kwargs: Any) -> int:
         exit_code = utils.run_cmd("git", git_cmd, *args, **kwargs)
@@ -373,54 +373,54 @@
         self.fetch_remote(remote)
         self._run_git("merge", "--ff-only", remote_branch)
         # There's apparently no way to set remote automatically when doing 'git pull' (as opposed to 'git push'),
         # so a separate 'git branch --set-upstream-to' is needed.
         self.set_upstream_to(remote_branch)
         self.flush_caches()
 
-    def __find_short_commit_sha_by_revision(self, revision: AnyRevision) -> ShortCommitHash:
+    def __find_short_commit_hash_by_revision(self, revision: AnyRevision) -> ShortCommitHash:
         return ShortCommitHash.of(self._popen_git("rev-parse", "--short", revision + "^{commit}").rstrip())
 
-    def get_short_commit_sha_by_revision(self, revision: AnyRevision) -> ShortCommitHash:
-        if revision not in self.__short_commit_sha_by_revision_cached:
-            self.__short_commit_sha_by_revision_cached[revision] = self.__find_short_commit_sha_by_revision(revision)
-        return self.__short_commit_sha_by_revision_cached[revision]
+    def get_short_commit_hash_by_revision(self, revision: AnyRevision) -> ShortCommitHash:
+        if revision not in self.__short_commit_hash_by_revision_cached:
+            self.__short_commit_hash_by_revision_cached[revision] = self.__find_short_commit_hash_by_revision(revision)
+        return self.__short_commit_hash_by_revision_cached[revision]
 
-    def __find_commit_sha_by_revision(self, revision: AnyRevision) -> Optional[FullCommitHash]:
+    def __find_commit_hash_by_revision(self, revision: AnyRevision) -> Optional[FullCommitHash]:
         # Without ^{commit}, 'git rev-parse --verify' will not only accept references to other kinds of objects (like trees and blobs),
         # but just echo the argument (and exit successfully) even if the argument doesn't match anything in the object store.
         try:
             return FullCommitHash.of(self._popen_git("rev-parse", "--verify", "--quiet", revision + "^{commit}").rstrip())
         except MacheteException:
             return None
 
-    def get_commit_sha_by_revision(self, revision: AnyRevision) -> Optional[FullCommitHash]:
-        if self.is_full_sha(revision.full_name()):
+    def get_commit_hash_by_revision(self, revision: AnyRevision) -> Optional[FullCommitHash]:
+        if self.is_full_hash(revision.full_name()):
             return FullCommitHash.of(revision)
-        if self.__commit_sha_by_revision_cached is None:
+        if self.__commit_hash_by_revision_cached is None:
             self.__load_branches()
-        if revision not in self.__commit_sha_by_revision_cached:
-            self.__commit_sha_by_revision_cached[revision] = self.__find_commit_sha_by_revision(revision)
-        return self.__commit_sha_by_revision_cached[revision]
+        if revision not in self.__commit_hash_by_revision_cached:
+            self.__commit_hash_by_revision_cached[revision] = self.__find_commit_hash_by_revision(revision)
+        return self.__commit_hash_by_revision_cached[revision]
 
-    def __find_tree_sha_by_revision(self, revision: AnyRevision) -> Optional[FullTreeHash]:
+    def __find_tree_hash_by_revision(self, revision: AnyRevision) -> Optional[FullTreeHash]:
         try:
             return FullTreeHash.of(self._popen_git("rev-parse", "--verify", "--quiet", revision + "^{tree}").rstrip())
         except MacheteException:
             return None
 
-    def get_tree_sha_by_commit_sha(self, commit_sha: FullCommitHash) -> Optional[FullTreeHash]:
-        if self.__tree_sha_by_commit_sha_cached is None:
+    def get_tree_hash_by_commit_hash(self, commit_hash: FullCommitHash) -> Optional[FullTreeHash]:
+        if self.__tree_hash_by_commit_hash_cached is None:
             self.__load_branches()
-        if commit_sha not in self.__tree_sha_by_commit_sha_cached:
-            self.__tree_sha_by_commit_sha_cached[commit_sha] = self.__find_tree_sha_by_revision(commit_sha)
-        return self.__tree_sha_by_commit_sha_cached[commit_sha]
+        if commit_hash not in self.__tree_hash_by_commit_hash_cached:
+            self.__tree_hash_by_commit_hash_cached[commit_hash] = self.__find_tree_hash_by_revision(commit_hash)
+        return self.__tree_hash_by_commit_hash_cached[commit_hash]
 
     @staticmethod
-    def is_full_sha(revision: AnyRevision) -> Optional[Match[str]]:
+    def is_full_hash(revision: AnyRevision) -> Optional[Match[str]]:
         return re.match("^[0-9a-f]{40}$", revision)
 
     def get_committer_unix_timestamp_by_revision(self, revision: AnyBranchName) -> int:
         if self.__committer_unix_timestamp_by_revision_cached is None:
             self.__load_branches()
         return self.__committer_unix_timestamp_by_revision_cached.get(revision.full_name(), 0)
 
@@ -480,89 +480,89 @@
 
     def get_remote_branches(self) -> List[RemoteBranchShortName]:
         if self.__remote_branches_cached is None:
             self.__load_branches()
         return self.__remote_branches_cached
 
     def __load_branches(self) -> None:
-        self.__commit_sha_by_revision_cached = {}
+        self.__commit_hash_by_revision_cached = {}
         self.__committer_unix_timestamp_by_revision_cached = {}
         self.__counterparts_for_fetching_cached = {}
         self.__local_branches_cached = []
         self.__remote_branches_cached = []
-        self.__tree_sha_by_commit_sha_cached = {}
+        self.__tree_hash_by_commit_hash_cached = {}
 
         # Using 'committerdate:raw' instead of 'committerdate:unix' since the latter isn't supported by some older versions of git.
         raw_remote = utils.get_non_empty_lines(self._popen_git("for-each-ref", "--format=%(refname)\t%(objectname)\t%(tree)\t%(committerdate:raw)", "refs/remotes"))
         for line in raw_remote:
             values = line.split("\t")
             if len(values) != 4:
                 continue  # invalid, shouldn't happen
-            branch, commit_sha, tree_sha, committer_unix_timestamp_and_time_zone = values
+            branch, commit_hash, tree_hash, committer_unix_timestamp_and_time_zone = values
             b_stripped_remote = RemoteBranchFullName.of(branch).to_short_name()
             self.__remote_branches_cached += [b_stripped_remote]
-            self.__commit_sha_by_revision_cached[RemoteBranchFullName.of(branch)] = FullCommitHash.of(commit_sha)
-            self.__tree_sha_by_commit_sha_cached[FullCommitHash.of(commit_sha)] = FullTreeHash.of(tree_sha)
+            self.__commit_hash_by_revision_cached[RemoteBranchFullName.of(branch)] = FullCommitHash.of(commit_hash)
+            self.__tree_hash_by_commit_hash_cached[FullCommitHash.of(commit_hash)] = FullTreeHash.of(tree_hash)
             self.__committer_unix_timestamp_by_revision_cached[RemoteBranchFullName.of(branch)] = int(committer_unix_timestamp_and_time_zone.split(' ')[0])
 
         raw_local = utils.get_non_empty_lines(self._popen_git("for-each-ref", "--format=%(refname)\t%(objectname)\t%(tree)\t%(committerdate:raw)\t%(upstream)", "refs/heads"))
 
         for line in raw_local:
             values = line.split("\t")
             if len(values) != 5:
                 continue  # invalid, shouldn't happen
-            branch, commit_sha, tree_sha, committer_unix_timestamp_and_time_zone, fetch_counterpart = values
+            branch, commit_hash, tree_hash, committer_unix_timestamp_and_time_zone, fetch_counterpart = values
             b_stripped_local = LocalBranchFullName.of(branch).to_short_name()
             fetch_counterpart_stripped = RemoteBranchFullName.of(fetch_counterpart).to_short_name() if fetch_counterpart else None  # fetch_counterpart might be empty
             self.__local_branches_cached += [b_stripped_local]
-            self.__commit_sha_by_revision_cached[LocalBranchFullName.of(branch)] = FullCommitHash.of(commit_sha)
-            self.__tree_sha_by_commit_sha_cached[FullCommitHash.of(commit_sha)] = FullTreeHash.of(tree_sha)
+            self.__commit_hash_by_revision_cached[LocalBranchFullName.of(branch)] = FullCommitHash.of(commit_hash)
+            self.__tree_hash_by_commit_hash_cached[FullCommitHash.of(commit_hash)] = FullTreeHash.of(tree_hash)
             self.__committer_unix_timestamp_by_revision_cached[LocalBranchFullName.of(branch)] = int(committer_unix_timestamp_and_time_zone.split(' ')[0])
             if fetch_counterpart_stripped in self.__remote_branches_cached:
                 self.__counterparts_for_fetching_cached[b_stripped_local] = fetch_counterpart_stripped
 
-    def __get_log_shas(self, revision: AnyRevision, max_count: Optional[int]) -> List[FullCommitHash]:
+    def __get_log_hashes(self, revision: AnyRevision, max_count: Optional[int]) -> List[FullCommitHash]:
         opts = ([f"--max-count={str(max_count)}"] if max_count else []) + ["--format=%H", revision.full_name()]
         return list(map(FullCommitHash.of, utils.get_non_empty_lines(self._popen_git("log", *opts))))
 
     # Since getting the full history of a branch can be an expensive operation for large repositories (compared to all other underlying git operations),
     # there's a simple optimization in place: we first fetch only a couple of first commits in the history,
     # and only fetch the rest if needed.
-    def spoonfeed_log_shas(self, branch_full_hash: FullCommitHash) -> Generator[FullCommitHash, None, None]:
-        if branch_full_hash not in self.__initial_log_shas_cached:
-            self.__initial_log_shas_cached[branch_full_hash] = self.__get_log_shas(branch_full_hash, max_count=MAX_COUNT_FOR_INITIAL_LOG)
-        for sha in self.__initial_log_shas_cached[branch_full_hash]:
-            yield FullCommitHash.of(sha)
-
-        if branch_full_hash not in self.__remaining_log_shas_cached:
-            self.__remaining_log_shas_cached[branch_full_hash] = self.__get_log_shas(branch_full_hash, max_count=None)[MAX_COUNT_FOR_INITIAL_LOG:]
-        for sha in self.__remaining_log_shas_cached[branch_full_hash]:
-            yield FullCommitHash.of(sha)
+    def spoonfeed_log_hashes(self, branch_full_hash: FullCommitHash) -> Generator[FullCommitHash, None, None]:
+        if branch_full_hash not in self.__initial_log_hashes_cached:
+            self.__initial_log_hashes_cached[branch_full_hash] = self.__get_log_hashes(branch_full_hash, max_count=MAX_COUNT_FOR_INITIAL_LOG)
+        for hash in self.__initial_log_hashes_cached[branch_full_hash]:
+            yield FullCommitHash.of(hash)
+
+        if branch_full_hash not in self.__remaining_log_hashes_cached:
+            self.__remaining_log_hashes_cached[branch_full_hash] = self.__get_log_hashes(branch_full_hash, max_count=None)[MAX_COUNT_FOR_INITIAL_LOG:]
+        for hash in self.__remaining_log_hashes_cached[branch_full_hash]:
+            yield FullCommitHash.of(hash)
 
     def __load_all_reflogs(self) -> None:
         # %gd - reflog selector (refname@{num})
         # %H - full hash
         # %gs - reflog subject
         all_branches = [str(branch.full_name()) for branch in self.get_local_branches()] + \
                        [str(self.get_combined_counterpart_for_fetching_of_branch(branch).full_name()) for branch in self.get_local_branches() if self.get_combined_counterpart_for_fetching_of_branch(branch)]  # str here to match _popen_git() input type
         # The trailing '--' is necessary to avoid ambiguity in case there is a file called just exactly like one of the branches.
         entries = utils.get_non_empty_lines(self._popen_git("reflog", "show", "--format=%gD\t%H\t%gs", *(all_branches + ["--"])))
         self.__reflogs_cached = {}
         for entry in entries:
             values = entry.split("\t")
             if len(values) != 3:  # invalid, shouldn't happen
                 continue
-            selector, sha, subject = values
+            selector, hash, subject = values
             branch_and_pos = selector.split("@")
             if len(branch_and_pos) != 2:  # invalid, shouldn't happen
                 continue
             branch, pos = branch_and_pos
             if branch not in self.__reflogs_cached:
                 self.__reflogs_cached[AnyBranchName.of(branch)] = []
-            self.__reflogs_cached[AnyBranchName.of(branch)] += [GitReflogEntry(hash=FullCommitHash.of(sha), reflog_subject=subject)]
+            self.__reflogs_cached[AnyBranchName.of(branch)] += [GitReflogEntry(hash=FullCommitHash.of(hash), reflog_subject=subject)]
 
     def get_reflog(self, branch: AnyBranchName) -> List[GitReflogEntry]:
         # git version 2.14.2 fixed a bug that caused fetching reflog of more than
         # one branch at the same time unreliable in certain cases
         if self.get_git_version() >= (2, 14, 2):
             if self.__reflogs_cached is None:
                 self.__load_all_reflogs()
@@ -586,27 +586,27 @@
             self._run_git("checkout", branch)
         self.flush_caches()  # the repository state has changed because of a successful branch creation, let's defensively flush all the caches
 
     def flush_caches(self) -> None:
         self.__config_cached = None
         self.__remotes_cached = None
         self.__counterparts_for_fetching_cached = None
-        self.__short_commit_sha_by_revision_cached = {}
-        self.__commit_sha_by_revision_cached = None
+        self.__short_commit_hash_by_revision_cached = {}
+        self.__commit_hash_by_revision_cached = None
         self.__committer_unix_timestamp_by_revision_cached = None
         self.__local_branches_cached = None
         self.__remote_branches_cached = None
         self.__reflogs_cached = None
 
     def get_revision_repr(self, revision: AnyRevision) -> str:
-        short_sha = self.get_short_commit_sha_by_revision(revision)
-        if self.is_full_sha(revision.full_name()) or revision == short_sha:
+        short_hash = self.get_short_commit_hash_by_revision(revision)
+        if self.is_full_hash(revision.full_name()) or revision == short_hash:
             return f"commit {revision}"
         else:
-            return f"{revision} (commit {self.get_short_commit_sha_by_revision(revision)})"
+            return f"{revision} (commit {self.get_short_commit_hash_by_revision(revision)})"
 
     # Note: while rebase is ongoing, the repository is always in a detached HEAD state,
     # so we need to extract the name of the currently rebased branch from the rebase-specific internals
     # rather than rely on 'git symbolic-ref HEAD' (i.e. the contents of .git/HEAD).
     def get_currently_rebased_branch_or_none(self) -> Optional[LocalBranchShortName]:  # utils/private
         # https://stackoverflow.com/questions/3921409
 
@@ -660,81 +660,81 @@
 
     def get_current_branch(self) -> LocalBranchShortName:
         result = self.get_current_branch_or_none()
         if not result:
             raise MacheteException("Not currently on any branch")
         return result
 
-    def __get_merge_base(self, sha1: FullCommitHash, sha2: FullCommitHash) -> FullCommitHash:
-        if sha1 > sha2:
-            sha1, sha2 = sha2, sha1
-        if not (sha1, sha2) in self.__merge_base_cached:
+    def __get_merge_base(self, hash1: FullCommitHash, hash2: FullCommitHash) -> FullCommitHash:
+        if hash1 > hash2:
+            hash1, hash2 = hash2, hash1
+        if not (hash1, hash2) in self.__merge_base_cached:
             # Note that we don't pass '--all' flag to 'merge-base', so we'll get only one merge-base
             # even if there is more than one (in the rare case of criss-cross histories).
             # This is still okay from the perspective of is-ancestor checks that are our sole use of merge-base:
-            # * if any of sha1, sha2 is an ancestor of another,
+            # * if any of hash1, hash2 is an ancestor of another,
             #   then there is exactly one merge-base - the ancestor,
-            # * if neither of sha1, sha2 is an ancestor of another,
-            #   then none of the (possibly more than one) merge-bases is equal to either of sha1/sha2 anyway.
-            # In the rare case when sha1, sha2 have no common commits, the flag: allow_non_zero=True
+            # * if neither of hash1, hash2 is an ancestor of another,
+            #   then none of the (possibly more than one) merge-bases is equal to either of hash1/hash2 anyway.
+            # In the rare case when hash1, hash2 have no common commits, the flag: allow_non_zero=True
             # (allows, non zero exit code to be returned by git merge-base command, without raising an exception)
             # is used and the __get_merge_base function returns None.
-            self.__merge_base_cached[sha1, sha2] = FullCommitHash.of(self._popen_git("merge-base", sha1, sha2, allow_non_zero=True))
-        return self.__merge_base_cached[sha1, sha2]
+            self.__merge_base_cached[hash1, hash2] = FullCommitHash.of(self._popen_git("merge-base", hash1, hash2, allow_non_zero=True))
+        return self.__merge_base_cached[hash1, hash2]
 
     # Note: the 'git rev-parse --verify' validation is not performed in case for either of earlier/later
     # if the corresponding prefix is empty AND the revision is a 40 hex digit hash.
     def is_ancestor_or_equal(
             self,
             earlier_revision: AnyRevision,
             later_revision: AnyRevision,
     ) -> bool:
-        earlier_sha = self.get_commit_sha_by_revision(earlier_revision)
-        later_sha = self.get_commit_sha_by_revision(later_revision)
+        earlier_hash = self.get_commit_hash_by_revision(earlier_revision)
+        later_hash = self.get_commit_hash_by_revision(later_revision)
         # This if statement is not changing the outcome of the later return, but
         # it enhances the efficiency of the script. If both hashes are the same,
         # there is no point running git merge-base.
-        if earlier_sha == later_sha:
+        if earlier_hash == later_hash:
             return True
 
-        return self.__get_merge_base(earlier_sha, later_sha) == earlier_sha
+        return self.__get_merge_base(earlier_hash, later_hash) == earlier_hash
 
     # Determine if reachable_from, or any ancestors of reachable_from that are NOT ancestors of equivalent_to,
     # contain a tree with identical contents to equivalent_to, indicating that
     # reachable_from contains a rebase or squash merge of equivalent_to.
     def is_equivalent_tree_reachable(
             self,
             equivalent_to: AnyRevision,
             reachable_from: AnyRevision,
     ) -> bool:
-        equivalent_to_commit_sha = self.get_commit_sha_by_revision(equivalent_to)
-        reachable_from_commit_sha = self.get_commit_sha_by_revision(reachable_from)
+        equivalent_to_commit_hash = self.get_commit_hash_by_revision(equivalent_to)
+        reachable_from_commit_hash = self.get_commit_hash_by_revision(reachable_from)
 
-        if equivalent_to_commit_sha == reachable_from_commit_sha:
+        if equivalent_to_commit_hash == reachable_from_commit_hash:
             return True
 
-        if (equivalent_to_commit_sha, reachable_from_commit_sha) in self.__is_equivalent_tree_reachable_cached:
-            return self.__is_equivalent_tree_reachable_cached[equivalent_to_commit_sha, reachable_from_commit_sha]
+        if (equivalent_to_commit_hash, reachable_from_commit_hash) in self.__is_equivalent_tree_reachable_cached:
+            return self.__is_equivalent_tree_reachable_cached[equivalent_to_commit_hash, reachable_from_commit_hash]
 
-        earlier_tree_sha = self.get_tree_sha_by_commit_sha(equivalent_to_commit_sha)
+        earlier_tree_hash = self.get_tree_hash_by_commit_hash(equivalent_to_commit_hash)
 
-        # `git log ^equivalent_to_commit_sha reachable_from_commit_sha`
-        # shows all commits reachable from reachable_from_commit_sha but NOT from equivalent_to_commit_sha
-        intermediate_tree_shas = utils.get_non_empty_lines(
+        # `git log ^equivalent_to_commit_hash reachable_from_commit_hash`
+        # shows all commits reachable from reachable_from_commit_hash but NOT from equivalent_to_commit_hash
+        intermediate_tree_hashes = utils.get_non_empty_lines(
             self._popen_git(
                 "log",
                 "--format=%T",  # full commit's tree hash
-                "^" + equivalent_to_commit_sha,
-                reachable_from_commit_sha
+                "^" + equivalent_to_commit_hash,
+                reachable_from_commit_hash
             )
         )
 
-        result = earlier_tree_sha in intermediate_tree_shas
+        result = earlier_tree_hash in intermediate_tree_hashes
         debug(f"result = {result}")
-        self.__is_equivalent_tree_reachable_cached[equivalent_to_commit_sha, reachable_from_commit_sha] = result
+        self.__is_equivalent_tree_reachable_cached[equivalent_to_commit_hash, reachable_from_commit_hash] = result
         return result
 
     def get_sole_remote_branch(self, branch: LocalBranchShortName) -> Optional[RemoteBranchShortName]:
         def matches(remote_branch: RemoteBranchShortName) -> bool:
             # Note that this matcher is defensively too inclusive:
             # if there is both origin/foo and origin/feature/foo,
             # then both are matched for 'foo';
```

### Comparing `git-machete-3.9.0/git_machete/github.py` & `git-machete-3.9.1/git_machete/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             if token:
                 raise MacheteException(first_line + f'Make sure that the GitHub API token provided by one of the: '
                                                     f'{get_github_token_possible_providers()}is valid and allows for access to '
                                                     f'`{method.upper()}` `https://{host}{path}`.')
             else:
                 raise MacheteException(
                     first_line + f'You might not have the required permissions for this repository. '
-                                 f'Provide a GitHub API token with `repo` access via one of the: {get_github_token_possible_providers()}'
+                                 f'Provide a GitHub API token with `repo` access via one of the: {get_github_token_possible_providers()} '
                                  'Visit `https://github.com/settings/tokens` to generate a new one.')
         elif err.code == http.HTTPStatus.NOT_FOUND:
             raise MacheteException(
                 f'Given endpoint: {url}, not found in GitHub or you don\'t have'
                 f' the permission to access it (expired token?).')  # TODO (#164): make dedicated exception here
         else:
             first_line = fmt(f'GitHub API returned {err.code} HTTP status with error message: `{err.reason}`\n')
```

### Comparing `git-machete-3.9.0/git_machete/options.py` & `git-machete-3.9.1/git_machete/options.py`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git_machete/utils.py` & `git-machete-3.9.1/git_machete/utils.py`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/git_machete.egg-info/PKG-INFO` & `git-machete-3.9.1/git_machete.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-machete
-Version: 3.9.0
+Version: 3.9.1
 Summary: Probably the sharpest git repository organizer & rebase/merge workflow automation tool you've ever seen
 Home-page: https://github.com/VirtusLab/git-machete
 Author: Pawel Lipski
 Author-email: pawel.p.lipski@gmail.com
 License: MIT
 Keywords: git
 Platform: UNKNOWN
@@ -25,17 +25,18 @@
 [![Read the Docs](https://readthedocs.org/projects/git-machete/badge/?version=latest)](https://git-machete.readthedocs.io/en/stable)
 [![PyPI package](https://img.shields.io/pypi/v/git-machete.svg)](https://pypi.org/project/git-machete)
 [![PyPI package monthly downloads](https://img.shields.io/pypi/dm/git-machete.svg?label=pypi%20downloads)](https://pypistats.org/packages/git-machete)
 [![Snap](https://snapcraft.io/git-machete/badge.svg)](https://snapcraft.io/git-machete)
 [![AUR package (Arch Linux)](https://repology.org/badge/version-for-repo/aur/git-machete.svg)](https://aur.archlinux.org/packages/git-machete)
 [![License: MIT](https://img.shields.io/github/license/VirtusLab/git-machete)](https://github.com/VirtusLab/git-machete/blob/master/LICENSE)
 [![CircleCI](https://circleci.com/gh/VirtusLab/git-machete/tree/master.svg?style=shield)](https://app.circleci.com/pipelines/github/VirtusLab/git-machete?branch=master)
+[![codecov](https://codecov.io/gh/VirtusLab/git-machete/branch/master/graph/badge.svg)](https://codecov.io/gh/VirtusLab/git-machete)
 
-<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
-<!-- The image is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/logo_with_name.svg" style="width: 100%; display: block; margin-bottom: 10pt;" />
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 💪 git-machete is a robust tool that **simplifies your git workflows**.<br/>
 
 🦅 The _bird's eye view_ provided by git-machete makes **merges/rebases/push/pulls hassle-free**
 even when **multiple branches** are present in the repository
 (master/develop, your topic branches, teammate's branches checked out for review, etc.).<br/>
 
@@ -44,18 +45,18 @@
 👁 A look at a `git machete status` gives an instant answer to the questions:
 * What branches are in this repository?
 * What is going to be merged (rebased/pushed/pulled) and to what?
 
 🚜 `git machete traverse` semi-automatically traverses the branches, helping you effortlessly rebase, merge, push and pull.
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/develop/graphics/discover-status-traverse.gif"
+    <img src="https://raw.githubusercontent.com/VirtusLab/git-machete/master/graphics/discover-status-traverse.gif"
          alt="git machete discover, status and traverse" />
 </p>
-<!-- The gif in here is referenced by full URL, corresponding develop branch to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
+<!-- The image is referenced by its full URL to ensure it renders correctly on https://pypi.org/project/git-machete/ -->
 
 🔌 See also [VirtusLab/git-machete-intellij-plugin](https://github.com/VirtusLab/git-machete-intellij-plugin#git-machete-intellij-plugin) &mdash;
 a port into a plugin for the IntelliJ Platform products, including PyCharm, WebStorm etc.
 
 
 ## Install
```

### Comparing `git-machete-3.9.0/git_machete.egg-info/SOURCES.txt` & `git-machete-3.9.1/git_machete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-machete-3.9.0/setup.py` & `git-machete-3.9.1/setup.py`

 * *Files identical despite different names*

