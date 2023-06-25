# Comparing `tmp/gttrl-1.0.tar.gz` & `tmp/gttrl-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gttrl-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gttrl-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gttrl-1.0.tar` & `gttrl-1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1137 2023-06-25 16:47:27.622527 gttrl-1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2023-06-25 16:47:27.622527 gttrl-1.0/.gitignore
--rw-r--r--   0        0        0     1621 2023-06-25 16:47:27.622527 gttrl-1.0/README.md
--rw-r--r--   0        0        0     2988 2023-06-25 16:47:27.622527 gttrl-1.0/gttrl/__init__.py
--rw-r--r--   0        0        0       58 2023-06-25 16:47:27.622527 gttrl-1.0/gttrl/__main__.py
--rw-r--r--   0        0        0     5886 2023-06-25 16:47:27.622527 gttrl-1.0/gttrl/gttrl.py
--rw-r--r--   0        0        0      462 2023-06-25 16:47:27.622527 gttrl-1.0/pyproject.toml
--rw-r--r--   0        0        0       14 2023-06-25 16:47:27.622527 gttrl-1.0/requirements.txt
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 gttrl-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-06-25 23:07:40.603576 gttrl-1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2023-06-25 23:07:40.603576 gttrl-1.1/.gitignore
+-rw-r--r--   0        0        0     1874 2023-06-25 23:07:40.603576 gttrl-1.1/README.md
+-rw-r--r--   0        0        0     3066 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/__main__.py
+-rw-r--r--   0        0        0     6910 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/gttrl.py
+-rw-r--r--   0        0        0      462 2023-06-25 23:07:40.603576 gttrl-1.1/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-06-25 23:07:40.603576 gttrl-1.1/requirements.txt
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 gttrl-1.1/PKG-INFO
```

### Comparing `gttrl-1.0/.github/workflows/main.yml` & `gttrl-1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gttrl-1.0/gttrl/__init__.py` & `gttrl-1.1/gttrl/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import argparse
+import getpass
 from pathlib import Path
 
-from .gttrl import Gttrl
+from .gttrl import Config, Gttrl
 
-__version__ = "1.0"
+__version__ = "1.1"
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Glomatico's Toontown Rewritten Launcher",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         "-u",
         "--username",
         help="Account username",
     )
     parser.add_argument(
         "-p",
         "--password",
         help="Account password",
     )
     parser.add_argument(
         "-a",
         "--account-file",
-        default="./account.txt",
         help="Account file location",
     )
     parser.add_argument(
-        "-f",
+        "-m",
         "--game-path",
-        default="./Toontown Rewritten",
         help="Game path",
     )
     parser.add_argument(
         "-c",
         "--play-cookie",
         help="Play cookie",
     )
@@ -55,44 +53,46 @@
         action="store_true",
         help="Print play cookie and game server and exit",
     )
     parser.add_argument(
         "-e",
         "--enable-log",
         action="store_true",
-        help="Enable log",
+        help="Enable logging to the console",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version=f"%(prog)s {__version__}",
     )
     args = parser.parse_args()
+    config = Config()
+    config.create_if_not_exists()
+    config_file = config.read_config_file()
     username = args.username
     password = args.password
-    account_file = args.account_file
-    game_path = args.game_path
+    account_file = args.account_file or config_file["account_file"]
+    game_path = args.game_path or config_file["game_path"]
     play_cookie = args.play_cookie
     game_server = args.game_server
-    skip_update = args.skip_update
+    skip_update = args.skip_update or config_file["skip_update"]
     print_play_cookie = args.print_play_cookie
-    enable_log = args.enable_log
+    enable_log = args.enable_log or config_file["enable_log"]
     if (username and not password) or (password and not username):
         raise Exception("Username and password must be provided together")
     elif (play_cookie and not game_server) or (game_server and not play_cookie):
         raise Exception("Play cookie and game server must be provided together")
     else:
         if Path(account_file).exists() and not username and not play_cookie:
             with open(account_file, "r") as file:
                 username, password = file.read().splitlines()
         elif not username and not play_cookie:
-            raise Exception(
-                "Account file does not exist and no others forms of authentication were provided"
-            )
+            username = input("Username: ")
+            password = getpass.getpass("Password: ")
     gttrl = Gttrl(username, password, game_path, enable_log)
     if username:
         print("Logging in...")
         play_cookie, game_server = gttrl.get_play_cookie()
     else:
         pass
     if print_play_cookie:
```

### Comparing `gttrl-1.0/gttrl/gttrl.py` & `gttrl-1.1/gttrl/gttrl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import bz2
 import hashlib
+import json
 import os
 import platform
 import subprocess
 import sys
 import time
 from pathlib import Path
 
@@ -69,18 +70,19 @@
                 chunk = f.read(4096)
                 if not chunk:
                     break
                 hasher.update(chunk)
         return hasher.hexdigest()
 
     def download_game_files(self):
+        if not self.game_path.exists():
+            self.game_path.mkdir(parents=True, exist_ok=True)
         manifest = self.session.get(
             "https://cdn.toontownrewritten.com/content/patchmanifest.txt"
         ).json()
-        self.game_path.mkdir(parents=True, exist_ok=True)
         keys = list(manifest.keys())
         for key in keys:
             if self.os not in manifest[key]["only"]:
                 del manifest[key]
         progress_bar = tqdm(
             manifest.keys(),
             leave=False,
@@ -157,13 +159,40 @@
             subprocess.call([self.game_exe])
         elif self.os == "win32" or self.os == "win64":
             subprocess.Popen(
                 [self.game_exe],
                 creationflags=subprocess.CREATE_NO_WINDOW,
             )
         else:
-            os.chmod(self.game_exe, 0o755)
+            if not os.access(self.game_exe, os.X_OK):
+                os.chmod(self.game_exe, 0o755)
             subprocess.Popen(
                 [self.game_exe],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
+
+
+class Config:
+    def __init__(self):
+        self.config_path = Path.home() / ".gttrl"
+        self.config_location = self.config_path / "config.json"
+
+    def create_if_not_exists(self):
+        if not self.config_path.exists():
+            self.config_path.mkdir(parents=True, exist_ok=True)
+        if not self.config_location.exists():
+            with open(self.config_location, "w") as f:
+                json.dump(
+                    {
+                        "game_path": str(self.config_path / "Toontown Rewritten"),
+                        "skip_update": False,
+                        "enable_log": False,
+                        "account_file": str(self.config_path / "account.txt"),
+                    },
+                    f,
+                    indent=4,
+                )
+
+    def read_config_file(self):
+        with open(self.config_location, "r") as f:
+            return json.load(f)
```

