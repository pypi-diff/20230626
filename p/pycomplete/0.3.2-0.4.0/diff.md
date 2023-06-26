# Comparing `tmp/pycomplete-0.3.2.tar.gz` & `tmp/pycomplete-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomplete-0.3.2.tar", last modified: Fri Dec 25 01:46:41 2020, max compression
+gzip compressed data, was "pycomplete-0.4.0.tar", last modified: Mon Jun 26 10:33:28 2023, max compression
```

## Comparing `pycomplete-0.3.2.tar` & `pycomplete-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2020-12-25 01:46:37.797484 pycomplete-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5497 2020-12-25 01:46:37.797484 pycomplete-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    12381 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4455 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3699 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/getters.py
--rw-r--r--   0 runner    (1001) docker     (116)      550 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/templates/bash.tpl
--rw-r--r--   0 runner    (1001) docker     (116)      332 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/templates/fish.tpl
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/templates/powershell.tpl
--rw-r--r--   0 runner    (1001) docker     (116)      852 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pycomplete/templates/zsh.tpl
--rw-r--r--   0 runner    (1001) docker     (116)      818 2020-12-25 01:46:37.797484 pycomplete-0.3.2/pyproject.toml
--rw-------   0 runner    (1001) docker     (116)     7015 2020-12-25 01:46:41.377501 pycomplete-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-06-26 10:33:19.985664 pycomplete-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5497 2023-06-26 10:33:19.985664 pycomplete-0.4.0/README.md
+-rw-r--r--   0        0        0    13293 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/__init__.py
+-rw-r--r--   0        0        0     4485 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/__main__.py
+-rw-r--r--   0        0        0     3693 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/getters.py
+-rw-r--r--   0        0        0      550 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/templates/__init__.py
+-rw-r--r--   0        0        0     1062 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/templates/bash.tpl
+-rw-r--r--   0        0        0      299 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/templates/fish.tpl
+-rw-r--r--   0        0        0     1142 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/templates/powershell.tpl
+-rw-r--r--   0        0        0      852 2023-06-26 10:33:19.985664 pycomplete-0.4.0/pycomplete/templates/zsh.tpl
+-rw-r--r--   0        0        0      816 2023-06-26 10:33:28.216217 pycomplete-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 pycomplete-0.4.0/PKG-INFO
```

### Comparing `pycomplete-0.3.2/LICENSE` & `pycomplete-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/README.md` & `pycomplete-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/pycomplete/__init__.py` & `pycomplete-0.4.0/pycomplete/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 import hashlib
 import os
 import posixpath
 import re
 import subprocess
 import sys
-from typing import Any, List, Optional
+from typing import Any
 
+from pycomplete.getters import GETTERS, BaseGetter, NotSupportedError
 from pycomplete.templates import SUPPORTED_SHELLS, TEMPLATES
-from pycomplete.getters import GETTERS, NotSupportedError
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 
 class Completer:
     """The completer to generate scripts for given shell. Currently only support
     (bash, zsh, fish). If the shell type is not given, the completer will try to guess
     from $SHELL environment variable.
 
@@ -24,15 +26,15 @@
 
         completer = Completer(parser)
         result = completer.render()
 
     Then save the result into a file that is read by the shell's autocomplete engine.
     """
 
-    def __init__(self, cli: Any, prog: Optional[List[str]] = None) -> None:
+    def __init__(self, cli: Any, prog: list[str] | None = None) -> None:
         for getter in GETTERS:
             try:
                 self.getter = getter(cli)
                 break
             except NotSupportedError:
                 pass
         else:
@@ -43,15 +45,15 @@
                 "framework. Please make sure you install pycomplete in the same "
                 "environment as the target CLI app."
             )
         if prog is None:
             prog = [os.path.basename(posixpath.realpath(sys.argv[0]))]
         self.prog = prog
 
-    def render(self, shell: Optional[str] = None) -> str:
+    def render(self, shell: str | None = None) -> str:
         if shell is None:
             shell = self.get_shell_type()
         if shell not in SUPPORTED_SHELLS:
             raise ValueError(
                 "[shell] argument must be one of {}".format(", ".join(SUPPORTED_SHELLS))
             )
         return getattr(self, "render_{}".format(shell))()
@@ -189,93 +191,109 @@
         )
 
         return output
 
     def render_fish(self) -> str:
         template = TEMPLATES["fish"]
 
+        def cmd_completion(
+            name: str, command: BaseGetter, parents: list[str]
+        ) -> list[str]:
+            result: list[str] = []
+            parents_join = "_".join(parents)
+            result.append(f"# {' '.join(parents + [name])}")
+            see_parent = "; and ".join(
+                f"__fish_seen_subcommand_from {p}" for p in parents
+            )
+            if not parents:
+                result.append(
+                    "complete -c {} -f -n '__fish{}_no_subcommand' "
+                    "-a {} -d '{}'".format(
+                        script_name, function, name, command.help.replace("'", "\\'")
+                    )
+                )
+            else:
+                no_subcommand = (
+                    f"not __fish_seen_subcommand_from ${parents_join}_subcommands"
+                )
+                result.append(
+                    "complete -c {} -f -n '{}; and {}' -a {} -d '{}'".format(
+                        script_name,
+                        see_parent,
+                        no_subcommand,
+                        name,
+                        command.help.replace("'", "\\'"),
+                    )
+                )
+
+            see_this = f"__fish_seen_subcommand_from {name}"
+            # options
+            for option_name, option_help in sorted(command.get_options()):
+                condition = f"{see_parent}; and {see_this}" if parents else see_this
+                result.append(
+                    "complete -c {} -A -n '{}' -l {} -d '{}'".format(
+                        script_name,
+                        condition,
+                        option_name[2:],
+                        option_help.replace("'", "\\'"),
+                    )
+                )
+            subcommands = command.get_commands()
+            if not subcommands:
+                return result
+            result.append(f"# {name} subcommands")
+            subcommands_var = (
+                f"{parents_join}_{name}_subcommands"
+                if parents
+                else f"{name}_subcommands"
+            )
+            result.append(f"set -l {subcommands_var} {' '.join(sorted(subcommands))}")
+            for i, (subcommand_name, subcommand) in enumerate(
+                sorted(subcommands.items())
+            ):
+                result.extend(
+                    cmd_completion(subcommand_name, subcommand, parents + [name])
+                )
+                if i < len(subcommands) - 1:
+                    result.append("")
+            return result
+
         script_path = posixpath.realpath(sys.argv[0])
         script_name = self.prog[0]
 
         function = self._generate_function_name(script_name, script_path)
 
-        global_options = set()
-        commands_descriptions = {}
-        options_descriptions = {}
-        commands_options_descriptions = {}
-        commands_options = {}
-        for option_name, option_help in self.getter.get_options():
-            options_descriptions[option_name] = option_help
-            global_options.add(option_name)
-
-        for name, command in self.getter.get_commands().items():
-            command_options = []
-            commands_options_descriptions[name] = {}
-            command_description = command.help
-            commands_descriptions[name] = command_description
-
-            for option_name, option_help in command.get_options():
-                command_options.append(option_name)
-                options_descriptions[option_name] = option_help
-                commands_options_descriptions[name][option_name] = option_help
-
-            commands_options[name] = command_options
-
-        opts = []
-        for opt in sorted(global_options):
+        opts: list[str] = []
+        cmd_names: set[str] = set()
+        cmds: list[str] = []
+        for option_name, option_help in sorted(self.getter.get_options()):
             opts.append(
                 "complete -c {} -n '__fish{}_no_subcommand' "
                 "-l {} -d '{}'".format(
                     script_name,
                     function,
-                    opt[2:],
-                    options_descriptions[opt].replace("'", "\\'"),
+                    option_name[2:],
+                    option_help.replace("'", "\\'"),
                 )
             )
 
-        cmds_names = sorted(list(commands_options.keys()))
-
-        cmds = []
-        cmds_opts = []
-        for i, cmd in enumerate(cmds_names):
-            cmds.append(
-                "complete -c {} -f -n '__fish{}_no_subcommand' "
-                "-a {} -d '{}'".format(
-                    script_name,
-                    function,
-                    cmd,
-                    commands_descriptions[cmd].replace("'", "\\'"),
-                )
-            )
-
-            cmds_opts += ["# {}".format(cmd)]
-            options = sorted(commands_options[cmd])
-
-            for opt in options:
-                cmds_opts.append(
-                    "complete -c {} -A -n '__fish_seen_subcommand_from {}' "
-                    "-l {} -d '{}'".format(
-                        script_name,
-                        cmd,
-                        opt[2:],
-                        commands_options_descriptions[cmd][opt].replace("'", "\\'"),
-                    )
-                )
-
-            if i < len(cmds_names) - 1:
-                cmds_opts.append("")
+        all_commands = sorted(self.getter.get_commands().items())
+        for i, (name, command) in enumerate(all_commands):
+            cmd_names.add(name)
+            cmds.extend(cmd_completion(name, command, []))
+            if i < len(all_commands) - 1:
+                cmds.append("")
 
         output = template.safe_substitute(
             {
                 "script_name": script_name,
                 "function": function,
-                "cmds_names": " ".join(cmds_names),
+                "cmds_names": " ".join(sorted(cmd_names)),
                 "opts": "\n".join(opts),
                 "cmds": "\n".join(cmds),
-                "cmds_opts": "\n".join(cmds_opts),
                 "version": __version__,
             }
         )
 
         return output
 
     def render_powershell(self) -> str:
```

### Comparing `pycomplete-0.3.2/pycomplete/__main__.py` & `pycomplete-0.4.0/pycomplete/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import ast
 import importlib
 import os
 import sys
 from argparse import ArgumentParser
-from typing import Any, List
+from typing import Any
 
 from pycomplete import Completer, __version__
 
 
 def create_parser() -> ArgumentParser:
     parser = ArgumentParser(
         "pycomplete",
@@ -79,15 +81,15 @@
         app = app(*args, **kwargs)
 
     if app is None:
         raise ValueError(f"The function {import_str} must return a non-None value")
     return app
 
 
-def get_prog_name(module: str) -> List[str]:
+def get_prog_name(module: str) -> list[str]:
     """Get the program name from the given module name."""
     if not module:
         return [os.path.basename(os.path.realpath(sys.argv[0]))]
 
     try:
         import importlib.metadata as imp_metadata
     except ModuleNotFoundError:
```

### Comparing `pycomplete-0.3.2/pycomplete/getters.py` & `pycomplete-0.4.0/pycomplete/getters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import abc
 import argparse
-from typing import Dict, Iterable, Tuple, Union
+from typing import Iterable
 
 try:
     import click
 except ModuleNotFoundError:
     click = None
 
 
@@ -18,20 +20,20 @@
     - :class:`argparse.ArgumentParser` instance.
     - :class:`click.Command` instance.
 
     subclasses must inherit this and implement the abstract methods and properties.
     """
 
     @abc.abstractmethod
-    def get_options(self) -> Iterable[Tuple[str, str]]:
+    def get_options(self) -> Iterable[tuple[str, str]]:
         """Return a list of [option_name, option_help] pairs."""
         pass
 
     @abc.abstractmethod
-    def get_commands(self) -> Dict[str, "BaseGetter"]:
+    def get_commands(self) -> dict[str, BaseGetter]:
         """Return a mapping of command_name -> command getter."""
         pass
 
     @abc.abstractproperty
     def help(self) -> str:
         """Get the help string for the command."""
         pass
@@ -43,23 +45,23 @@
     """
 
     def __init__(self, parser: argparse.ArgumentParser) -> None:
         if not isinstance(parser, argparse.ArgumentParser):
             raise NotSupportedError("Not supported")
         self._parser = parser
 
-    def get_options(self) -> Iterable[Tuple[str, str]]:
+    def get_options(self) -> Iterable[tuple[str, str]]:
         for action in self._parser._actions:
             if not action.option_strings:
                 continue
             # Prefer the --long-option-name, just compare by the length of the string.
             name = max(action.option_strings, key=len)
             yield name, action.help
 
-    def get_commands(self) -> Dict[str, "ArgparseGetter"]:
+    def get_commands(self) -> dict[str, BaseGetter]:
         subparsers = next(
             (
                 action
                 for action in self._parser._actions
                 if action.nargs == argparse.PARSER
             ),
             None,
@@ -79,38 +81,38 @@
 if click:
 
     class ClickGetter(BaseGetter):
         """Helper class to fetch options/commands from a
         :class:`click.Command` instance
         """
 
-        def __init__(self, cli: Union[click.Command, click.Context]) -> None:
+        def __init__(self, cli: click.Command | click.Context) -> None:
             if not isinstance(cli, (click.Command, click.Context)):
                 raise NotSupportedError("Not supported")
             self._cli = self._get_top_command(cli)
 
         @staticmethod
         def _get_top_command(
-            cmd_or_ctx: Union[click.Command, click.Context]
+            cmd_or_ctx: click.Command | click.Context,
         ) -> click.Command:
             if isinstance(cmd_or_ctx, click.Command):
                 return cmd_or_ctx
             while cmd_or_ctx.parent:
                 cmd_or_ctx = cmd_or_ctx.parent
             return cmd_or_ctx.command
 
-        def get_options(self) -> Iterable[Tuple[str, str]]:
+        def get_options(self) -> Iterable[tuple[str, str]]:
             ctx = click.Context(self._cli, info_name=self._cli.name)
             for param in self._cli.get_params(ctx):
                 if param.get_help_record(ctx):
                     yield max(param.opts, key=len), param.help
                     if param.secondary_opts:
                         yield max(param.secondary_opts, key=len), param.help
 
-        def get_commands(self) -> Dict[str, "ClickGetter"]:
+        def get_commands(self) -> dict[str, BaseGetter]:
             commands = getattr(self._cli, "commands", {})
             return {
                 name: ClickGetter(cmd)
                 for name, cmd in commands.items()
                 if not cmd.hidden
             }
```

### Comparing `pycomplete-0.3.2/pycomplete/templates/__init__.py` & `pycomplete-0.4.0/pycomplete/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/pycomplete/templates/bash.tpl` & `pycomplete-0.4.0/pycomplete/templates/bash.tpl`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/pycomplete/templates/powershell.tpl` & `pycomplete-0.4.0/pycomplete/templates/powershell.tpl`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/pycomplete/templates/zsh.tpl` & `pycomplete-0.4.0/pycomplete/templates/zsh.tpl`

 * *Files identical despite different names*

### Comparing `pycomplete-0.3.2/PKG-INFO` & `pycomplete-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,170 +1,164 @@
 Metadata-Version: 2.1
 Name: pycomplete
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Python library to generate static completion scripts for your CLI app
-Home-page: UNKNOWN
+Keywords: cli shell
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: BSD-3-Clause
-Keywords: cli,shell
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.6
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Project-URL: Homepage, https://github.com/frostming/pycomplete
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Description: # pycomplete
 
-        A Python library to generate static completion scripts for your CLI app
+# pycomplete
 
-        ![Tests](https://github.com/frostming/pycomplete/workflows/Tests/badge.svg)
-        [![PyPI](https://img.shields.io/pypi/v/pycomplete)](https://pypi.org/project/pycomplete)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycomplete)](https://pypi.org/project/pycomplete)
-        ![Supported Shells - bash|zsh|fish|powershell](https://img.shields.io/badge/shell-bash%7Czsh%7Cfish%7Cpowershell-yellow)
+A Python library to generate static completion scripts for your CLI app
 
-        ## Installation
+![Tests](https://github.com/frostming/pycomplete/workflows/Tests/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/pycomplete)](https://pypi.org/project/pycomplete)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycomplete)](https://pypi.org/project/pycomplete)
+![Supported Shells - bash|zsh|fish|powershell](https://img.shields.io/badge/shell-bash%7Czsh%7Cfish%7Cpowershell-yellow)
 
-        `pycomplete` requires Python 3.6 or higher, you can install it via PyPI:
+## Installation
 
-        ```bash
-        $ pip install pycomplete
-        ```
+`pycomplete` requires Python 3.6 or higher, you can install it via PyPI:
 
-        ## Usage
+```bash
+$ pip install pycomplete
+```
 
-        With `pycomplete`, one can generate a completion script for CLI application that is compatible with a given shell.
-        The script outputs the result onto `stdout`, allowing one to re-direct the output to the file of their choosing.
+## Usage
 
-        `pycomplete` accepts different types of objects depending on which CLI framework you are using.
-        For `argparse`, `argparse.ArgumentParser` is expected while for `click`, either `click.Command` or `click.Context` is OK.
-        `pycomplete` knows what to do smartly.
+With `pycomplete`, one can generate a completion script for CLI application that is compatible with a given shell.
+The script outputs the result onto `stdout`, allowing one to re-direct the output to the file of their choosing.
 
-        Where you place the file will depend on which shell, and which operating system you are using.
-        Your particular configuration may also determine where these scripts need to be placed.
+`pycomplete` accepts different types of objects depending on which CLI framework you are using.
+For `argparse`, `argparse.ArgumentParser` is expected while for `click`, either `click.Command` or `click.Context` is OK.
+`pycomplete` knows what to do smartly.
 
-        Note that `pycomplete` needs to be installed in the same environment as the target CLI app to work properly.
+Where you place the file will depend on which shell, and which operating system you are using.
+Your particular configuration may also determine where these scripts need to be placed.
 
-        Here are some common set ups for the three supported shells under Unix and similar operating systems (such as GNU/Linux).
+Note that `pycomplete` needs to be installed in the same environment as the target CLI app to work properly.
 
-        ### BASH
+Here are some common set ups for the three supported shells under Unix and similar operating systems (such as GNU/Linux).
 
-        Completion files are commonly stored in `/etc/bash_completion.d/`. Run command:
+### BASH
 
-        ```bash
-        $ pycomplete "myscript:parser" bash > /etc/bash_completion.d/_myscript
-        ```
+Completion files are commonly stored in `/etc/bash_completion.d/`. Run command:
 
-        You may have to log out and log back in to your shell session for the changes to take effect.
+```bash
+$ pycomplete "myscript:parser" bash > /etc/bash_completion.d/_myscript
+```
 
-        ### FISH
+You may have to log out and log back in to your shell session for the changes to take effect.
 
-        Fish completion files are commonly stored in`$HOME/.config/fish/completions/`. Run command:
+### FISH
 
-        ```bash
-        $ pycomplete "myscript:parser" fish > $HOME/.config/fish/completions/myscript.fish
-        ```
+Fish completion files are commonly stored in`$HOME/.config/fish/completions/`. Run command:
 
-        You may have to log out and log back in to your shell session for the changes to take effect.
+```bash
+$ pycomplete "myscript:parser" fish > $HOME/.config/fish/completions/myscript.fish
+```
 
-        ### ZSH
+You may have to log out and log back in to your shell session for the changes to take effect.
 
-        ZSH completions are commonly stored in any directory listed in your `$fpath` variable. To use these completions, you
-        must either add the generated script to one of those directories, or add your own to this list.
+### ZSH
 
-        Adding a custom directory is often the safest best if you're unsure of which directory to use. First create the directory, for this
-        example we'll create a hidden directory inside our `$HOME` directory
+ZSH completions are commonly stored in any directory listed in your `$fpath` variable. To use these completions, you
+must either add the generated script to one of those directories, or add your own to this list.
 
-        ```bash
-        $ mkdir ~/.zfunc
-        ```
+Adding a custom directory is often the safest best if you're unsure of which directory to use. First create the directory, for this
+example we'll create a hidden directory inside our `$HOME` directory
 
-        Then add the following lines to your `.zshrc` just before `compinit`
+```bash
+$ mkdir ~/.zfunc
+```
 
-        ```bash
-        $ fpath+=~/.zfunc
-        ```
+Then add the following lines to your `.zshrc` just before `compinit`
 
-        Run command:
+```bash
+$ fpath+=~/.zfunc
+```
 
-        ```bash
-        $ pycomplete "myscript:parser" zsh > ~/.zfunc/_myscript
-        ```
+Run command:
 
-        You must then either log out and log back in, or simply run
+```bash
+$ pycomplete "myscript:parser" zsh > ~/.zfunc/_myscript
+```
 
-        ```bash
-        $ exec zsh
-        ```
+You must then either log out and log back in, or simply run
 
-        For the new completions to take affect.
+```bash
+$ exec zsh
+```
 
-        ### Powershell
+For the new completions to take affect.
 
-        There is no default location for completion scripts on Powershell. One may need to execute the scripts in their profile:
+### Powershell
 
-        ```powershell
-        PS > mkdir $PROFILE\..\Completions
-        PS > echo @'
-        Get-ChildItem "$PROFILE\..\Completions\" | ForEach-Object {
-            . $_.FullName
-        }
-        '@ | Out-File -Append -Encoding utf8 $PROFILE
-        ```
+There is no default location for completion scripts on Powershell. One may need to execute the scripts in their profile:
 
-        Make sure you set the proper [Execution Policy](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy):
+```powershell
+PS > mkdir $PROFILE\..\Completions
+PS > echo @'
+Get-ChildItem "$PROFILE\..\Completions\" | ForEach-Object {
+    . $_.FullName
+}
+'@ | Out-File -Append -Encoding utf8 $PROFILE
+```
 
-        ```powershell
-        PS > Set-ExecutionPolicy Unrestricted -Scope CurrentUser
-        ```
+Make sure you set the proper [Execution Policy](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy):
 
-        Run command to generate script:
+```powershell
+PS > Set-ExecutionPolicy Unrestricted -Scope CurrentUser
+```
 
-        ```powershell
-        PS > pycomplete "myscript:parser" powershell | Out-File -Encoding utf8 $PROFILE\..\Completions\myscript_completion.ps1
-        ```
+Run command to generate script:
 
-        You may have to log out and log back in to your shell session for the changes to take effect.
+```powershell
+PS > pycomplete "myscript:parser" powershell | Out-File -Encoding utf8 $PROFILE\..\Completions\myscript_completion.ps1
+```
 
-        ### CUSTOM LOCATIONS
+You may have to log out and log back in to your shell session for the changes to take effect.
 
-        Alternatively, you could save these files to the place of your choosing, such as a custom directory inside your \$HOME. Doing so will
-        require you to add the proper directives, such as `source`ing inside your login script. Consult your shells documentation for how to
-        add such directives.
+### CUSTOM LOCATIONS
 
-        ### Integrate with existing CLI apps
+Alternatively, you could save these files to the place of your choosing, such as a custom directory inside your \$HOME. Doing so will
+require you to add the proper directives, such as `source`ing inside your login script. Consult your shells documentation for how to
+add such directives.
 
-        `pycomplete` can be also used as a Python library, allowing one to integrate with existing CLI apps.
+### Integrate with existing CLI apps
 
-        ```python
-        from pycomplete import Completer
-        from mypackage.cli import parser
+`pycomplete` can be also used as a Python library, allowing one to integrate with existing CLI apps.
 
-        completer = Completer(parser)
-        print(completer.render())
-        ```
+```python
+from pycomplete import Completer
+from mypackage.cli import parser
 
-        See `examples/` folder for full examples of working apps.
+completer = Completer(parser)
+print(completer.render())
+```
 
-        ## How does it differ from `argcomplete`?
+See `examples/` folder for full examples of working apps.
 
-        `argcomplete`, together with `click-completion`, can also generate scripts for shell completion. However, they work in a different way
-        that commands and options are retrieved on the fly when they are requested by a matching token. This brings a performance shrinkage
-        when it is expensive to import the CLI app. In the other side, `pycomplete` produces **static and fixed** scripts which contain all required information
-        within themselves. Plus, `argcomplete` and `click-completion` both work for specific framework. One may notice the disadvantage of static completion
-        is also obvious -- users must regenerate the script when the commands and/or options are updated. Fortunately, it shouldn't be a problem
-        in most package managers like `homebrew`, where completion scripts are part of the package and are bundled with it.
+## How does it differ from `argcomplete`?
 
-        ## Limitations
+`argcomplete`, together with `click-completion`, can also generate scripts for shell completion. However, they work in a different way
+that commands and options are retrieved on the fly when they are requested by a matching token. This brings a performance shrinkage
+when it is expensive to import the CLI app. In the other side, `pycomplete` produces **static and fixed** scripts which contain all required information
+within themselves. Plus, `argcomplete` and `click-completion` both work for specific framework. One may notice the disadvantage of static completion
+is also obvious -- users must regenerate the script when the commands and/or options are updated. Fortunately, it shouldn't be a problem
+in most package managers like `homebrew`, where completion scripts are part of the package and are bundled with it.
 
-        Only options and subcommands are autocompleted, positional arguments are not completed since user usually expects the path sugguestion to work
-        in this case.
+## Limitations
 
-        ## Supported CLI Frameworks
+Only options and subcommands are autocompleted, positional arguments are not completed since user usually expects the path sugguestion to work
+in this case.
 
-        - [x] `argparse.ArgumentParser`
-        - [x] `click.Command`, `click.Context`
-        - [ ] More to be added
+## Supported CLI Frameworks
 
+- [x] `argparse.ArgumentParser`
+- [x] `click.Command`, `click.Context`
+- [ ] More to be added
```

