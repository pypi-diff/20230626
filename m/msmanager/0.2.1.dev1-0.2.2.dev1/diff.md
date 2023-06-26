# Comparing `tmp/msmanager-0.2.1.dev1.tar.gz` & `tmp/msmanager-0.2.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.1.dev1.tar", max compression
+gzip compressed data, was "msmanager-0.2.2.dev1.tar", max compression
```

## Comparing `msmanager-0.2.1.dev1.tar` & `msmanager-0.2.2.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.1.dev1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.1.dev1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.1.dev1/msmanager/__main__.py
--rw-r--r--   0        0        0     5968 2023-06-21 13:00:00.586899 msmanager-0.2.1.dev1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.1.dev1/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.1.dev1/msmanager/exceptions.py
--rw-r--r--   0        0        0     3570 2023-06-21 12:56:23.279871 msmanager-0.2.1.dev1/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.1.dev1/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.1.dev1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.1.dev1/msmanager/types.py
--rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.2.1.dev1/msmanager/units.py
--rw-r--r--   0        0        0      552 2023-06-21 13:03:32.126797 msmanager-0.2.1.dev1/pyproject.toml
--rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.2.1.dev1/README.md
--rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 msmanager-0.2.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev1/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev1/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev1/msmanager/__main__.py
+-rw-r--r--   0        0        0     6826 2023-06-26 19:31:40.068583 msmanager-0.2.2.dev1/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev1/msmanager/config.py
+-rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.2.dev1/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4002 2023-06-26 19:34:27.030856 msmanager-0.2.2.dev1/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev1/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev1/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev1/msmanager/types.py
+-rw-r--r--   0        0        0      591 2023-06-26 19:34:43.467905 msmanager-0.2.2.dev1/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-26 19:34:38.000477 msmanager-0.2.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev1/README.md
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev1/PKG-INFO
```

### Comparing `msmanager-0.2.1.dev1/LICENSE` & `msmanager-0.2.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1.dev1/msmanager/cli.py` & `msmanager-0.2.2.dev1/msmanager/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import os
 import click
 from rich.console import Console
 from typing import Iterable, Optional
 # > Local Imports
+from .units import (
+    __version__ as prog_version,
+    __title__ as prog_name
+)
 from .msm import MSManager
 from .models import MindustryServerConfig
 from .functions import (
     rich_exception,
     is_server_connect_correct,
     wait_start_server,
-    ping, endicext
+    ping, endicext, parse_connect_data
 )
 
 # ! Vars
 console = Console()
 msmanager: MSManager = ...
 
 # ! Commands
@@ -73,15 +77,19 @@
         console.print("[green]>[/] Server [bold yellow]removed[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? Start Command
 @click.command("start", help="Run the server.")
 @click.argument("screen_name", type=str)
-@click.option("-w", "--wait", "wait", is_flag=True, help="Waiting for the server to start up.")
+@click.option(
+    "-w", "--wait", "wait",
+    help="Waiting for the server to start up.",
+    is_flag=True
+)
 def starter(screen_name: str, wait: bool):
     try:
         msmanager.start_server(screen_name)
         if (server_config:=msmanager.get_server_config(screen_name)) is not None:
             if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
                 wait_start_server(server_config.host, server_config.port, server_config.input_port)
         console.print("[green]>[/] Server [bold yellow]started[/]!")
@@ -96,72 +104,90 @@
         msmanager.stop_server(screen_name)
         console.print("[green]>[/] Server [bold yellow]stoped[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 # ? List Command
 @click.command("list", help="List of servers in the config.")
-def lister():
+@click.option(
+    "--pinging", "pinging",
+    help="Whether to do a ping to check.",
+    is_flag=True, default=False
+)
+@click.option(
+    "-t", "--timeout", "timeout",
+    help="Maximum response waiting time (in seconds).",
+    type=int, default=10, show_default=True
+)
+def lister(pinging: bool, timeout: int):
     try:
         if len(msmanager.config.config.servers) != 0:
             for idx, server in enumerate(msmanager.config.config.servers):
-                console.print(
-                    "\n\t".join(
-                        [
-                            f"({idx}) Server [green]{server.screen_name}[/]:",
-                            f"[yellow]EXECUTABLE_FILEPATH[/]  : {repr(server.executable_filepath)}",
-                            f"[yellow]ARGUMENTS[/]            : {repr(' '.join(server.arguments))}",
-                            f"[yellow]HOST:PORT:INPUT_PORT[/] : [green]{server.host}[/]:{server.port}:{server.input_port}"
-                        ]
-                    )
-                )
+                lines = [
+                    f"({idx}) Server {repr(server.screen_name)}:",
+                    f"[magenta]Executable Filepath[/] : {repr(server.executable_filepath)}",
+                    f"[magenta]Arguments[/]           : {repr(server.arguments)}",
+                    f"[magenta]Host[/]                : [green]{server.host}[/]",
+                    f"[magenta]Port[/]                : [cyan]{server.port}[/]",
+                    f"[magenta]Input Port[/]          : [cyan]{server.input_port}[/]"
+                ]
+                if pinging:
+                    try:
+                        ping(server.host, server.port, timeout)
+                        started = True
+                    except:
+                        started = False
+                    lines.append(f"[magenta]Started[/]             : {repr(started)}")
+                console.print("\n\t".join(lines))
         else:
             console.print("[green]>[/] The list of servers is [bold yellow]empty[/]!")
     except Exception as e:
         console.print(rich_exception(e))
 
 @click.command("ping", help="Server status check.")
-@click.argument("host", type=str)
-@click.argument("port", type=int)
+@click.argument("connect", type=str)
 @click.option(
     "-t", "--timeout", "timeout",
     help="Maximum response waiting time (in seconds).",
     type=int, default=10, show_default=True
 )
-def pinger(host: str, port: int, timeout: int):
+def pinger(connect: str, timeout: int):
     try:
-        status = ping(host, port, timeout)
+        connect_data = parse_connect_data(connect)
+        status = ping(connect_data["host"], connect_data["port"], timeout)
         console.print(
             "\n\t".join(
                 [
-                    f"[green]>[/] Server {endicext(status.name)}:",
-                    f"- [yellow]Players[/] : {status.players} players",
-                    f"- [yellow]Map[/]     : [green]{status.map}[/]",
-                    f"- [yellow]Wave[/]    : {status.wave} wave",
-                    f"- [yellow]Ping[/]    : {round(status.ping)} ms",
-                    f"- [yellow]Version[/] : [green]v{status.version}[/]",
-                    f"- [yellow]Vertype[/] : [green]{status.vertype}[/]"                    
+                    f"[green]>[/] Server '{endicext(status.name)}':",
+                    f"- [magenta]Players[/] : {status.players} players",
+                    f"- [magenta]Map[/]     : {repr(status.map)}",
+                    f"- [magenta]Wave[/]    : {status.wave} wave",
+                    f"- [magenta]Ping[/]    : {round(status.ping)} ms",
+                    f"- [magenta]Version[/] : {repr(status.version)}",
+                    f"- [magenta]Vertype[/] : {repr(status.vertype)}"
                 ]
             )
         )
     except Exception as e:
         console.print(rich_exception(e))
 
 # ! Main Group
 @click.group()
 @click.option(
     "-nce", "--not-check-environment", "not_check_environment",
     is_flag=True,
     help="Disables checks for GNU Screen, Java and system support."
 )
+@click.version_option(
+    version=prog_version,
+    prog_name=prog_name
+)
 def main(not_check_environment: bool):
     global msmanager
-    msmanager = MSManager(
-        check_environment=(not not_check_environment)
-    )
+    msmanager = MSManager(check_environment=(not not_check_environment))
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
 main.add_command(stoper)
 main.add_command(lister)
```

### Comparing `msmanager-0.2.1.dev1/msmanager/config.py` & `msmanager-0.2.2.dev1/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1.dev1/msmanager/exceptions.py` & `msmanager-0.2.2.dev1/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1.dev1/msmanager/functions.py` & `msmanager-0.2.2.dev1/msmanager/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pydustry
 import platform
 from versioner import Version
 from vbml import Pattern, Patcher
 from subprocess import getstatusoutput
-from typing import Tuple, Dict, Any, Iterable
+from typing import Tuple, Dict, Any, Iterable, Optional
 # * Local Imports
 from .types import DefaultVersioner, DefaultVBMLPacther
 from .units import SUPPORT_PLATFORMS, COLORS_STRINGS_REPLACEBLE
 from .exceptions import (
     VBMLParseError, 
     PlatformSupportError,
     ScreenNotWorkingError,
@@ -37,19 +37,19 @@
     while True:
         try:
             server.get_status(per_second)
             break
         except:
             pass
 
-def is_server_connect_correct(server_host: str, port: int, input_port: int) -> bool:
+def is_server_connect_correct(server_host: str, port: int, input_port: Optional[int]) -> bool:
     return \
         isinstance(server_host, str) and \
         isinstance(port, int) and \
-        (isinstance(input_port, int) if (input_port is not None) else True)
+        (isinstance(input_port, int) or (input_port is not None))
 
 def ping(host: str, port: int, timeout: int=10) -> pydustry.Status:
     return pydustry.Server(host, port).get_status(timeout)
 
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
@@ -72,14 +72,25 @@
 
 def parse_vbml_linear(lines: Iterable[str], pattern: str, *, pacther: Patcher=DefaultVBMLPacther) -> Dict[str, Any]:
     for line in lines:
         try: return parse_vbml(line, pattern, pacther=pacther)
         except: pass
     raise VBMLParseError()
 
+def parse_vbml_patterns(text: str, patterns: Iterable[str], *, pacther: Patcher=DefaultVBMLPacther) -> Dict[str, Any]:
+    for pattern in patterns:
+        try: return parse_vbml(text, pattern)
+        except: pass
+    raise VBMLParseError()
+
+def parse_connect_data(text: str):
+    data = {"host": None, "port": 6567}
+    data.update(parse_vbml_patterns(text, ["<host>:<port:int>", "<host>"]))
+    return data
+
 def get_java_version() -> Version:
     if exists_java():
         data = parse_vbml(runner("java", "--version")[1].split("\n")[0], "<t1> <version> <t2>")
         return DefaultVersioner.parse(data["version"])
     raise JavaNotFound()
 
 def get_mindustry_server_version(jarfilepath: str) -> Version:
```

### Comparing `msmanager-0.2.1.dev1/msmanager/msm.py` & `msmanager-0.2.2.dev1/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.1.dev1/msmanager/units.py` & `msmanager-0.2.2.dev1/msmanager/units.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __name__ = "msmanager"
-__version__ = "0.1.3"
+__title__ = "MSManager (Mindustry Servers Manager)"
+__version__ = "0.2.2.dev1"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.2.1.dev1/pyproject.toml` & `msmanager-0.2.2.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.1.dev1"
-description = "Manager for managing Mindusrty servers."
+version = "0.2.2.dev1"
+description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `msmanager-0.2.1.dev1/PKG-INFO` & `msmanager-0.2.2.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.1.dev1
-Summary: Manager for managing Mindusrty servers.
+Version: 0.2.2.dev1
+Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -19,28 +19,31 @@
 Requires-Dist: screens-py (>=0.5.0,<0.6.0)
 Requires-Dist: vbml (>=1.1.post1,<2.0)
 Requires-Dist: versioner.py (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # MSManager
 ## Description
-Manager for managing Mindusrty servers.
+Manager for managing Mindustry servers.
 ## Install
 ```shell
 python3 -m pip install --upgrade msmanager
 ```
 ## Usage
 ```
 Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
 
 Options:
-  --not-check-environment  Disables checks for GNU Screen, Java and system support.
-  --help                   Show this message and exit.
+  -nce, --not-check-environment  Disables checks for GNU Screen, Java and
+                                 system support.
+  --version                      Show the version and exit.
+  --help                         Show this message and exit.
 
 Commands:
   add     Add a server to the config.
   list    List of servers in the config.
+  ping    Server status check.
   remove  Remove the server from the config.
   start   Run the server.
   stop    Stop the server.
 ```
```

