# Comparing `tmp/gttrl-1.1.tar.gz` & `tmp/gttrl-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gttrl-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gttrl-1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gttrl-1.1.tar` & `gttrl-1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1137 2023-06-25 23:07:40.603576 gttrl-1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2023-06-25 23:07:40.603576 gttrl-1.1/.gitignore
--rw-r--r--   0        0        0     1874 2023-06-25 23:07:40.603576 gttrl-1.1/README.md
--rw-r--r--   0        0        0     3066 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/__init__.py
--rw-r--r--   0        0        0       58 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/__main__.py
--rw-r--r--   0        0        0     6910 2023-06-25 23:07:40.603576 gttrl-1.1/gttrl/gttrl.py
--rw-r--r--   0        0        0      462 2023-06-25 23:07:40.603576 gttrl-1.1/pyproject.toml
--rw-r--r--   0        0        0       14 2023-06-25 23:07:40.603576 gttrl-1.1/requirements.txt
--rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 gttrl-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-06-26 19:33:47.566124 gttrl-1.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2023-06-26 19:33:47.566124 gttrl-1.2/.gitignore
+-rw-r--r--   0        0        0     1874 2023-06-26 19:33:47.566124 gttrl-1.2/README.md
+-rw-r--r--   0        0        0     2794 2023-06-26 19:33:47.566124 gttrl-1.2/gttrl/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-26 19:33:47.566124 gttrl-1.2/gttrl/__main__.py
+-rw-r--r--   0        0        0     6620 2023-06-26 19:33:47.566124 gttrl-1.2/gttrl/gttrl.py
+-rw-r--r--   0        0        0      462 2023-06-26 19:33:47.566124 gttrl-1.2/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-06-26 19:33:47.566124 gttrl-1.2/requirements.txt
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 gttrl-1.2/PKG-INFO
```

### Comparing `gttrl-1.1/.github/workflows/main.yml` & `gttrl-1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gttrl-1.1/README.md` & `gttrl-1.2/README.md`

 * *Files identical despite different names*

### Comparing `gttrl-1.1/gttrl/__init__.py` & `gttrl-1.2/gttrl/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import getpass
 from pathlib import Path
 
 from .gttrl import Config, Gttrl
 
-__version__ = "1.1"
+__version__ = "1.2"
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Glomatico's Toontown Rewritten Launcher",
     )
     parser.add_argument(
@@ -65,41 +65,39 @@
         action="version",
         version=f"%(prog)s {__version__}",
     )
     args = parser.parse_args()
     config = Config()
     config.create_if_not_exists()
     config_file = config.read_config_file()
-    username = args.username
-    password = args.password
-    account_file = args.account_file or config_file["account_file"]
-    game_path = args.game_path or config_file["game_path"]
-    play_cookie = args.play_cookie
-    game_server = args.game_server
-    skip_update = args.skip_update or config_file["skip_update"]
-    print_play_cookie = args.print_play_cookie
-    enable_log = args.enable_log or config_file["enable_log"]
-    if (username and not password) or (password and not username):
-        raise Exception("Username and password must be provided together")
-    elif (play_cookie and not game_server) or (game_server and not play_cookie):
-        raise Exception("Play cookie and game server must be provided together")
+    username, password = None, None
+    if Path(config_file["account_file"]).exists():
+        with open(config_file["account_file"]) as f:
+            username, password = f.read().splitlines()
+    elif args.account_file:
+        with open(args.account_file, "w") as f:
+            f.write(f"{username}\n{password}")
+    elif not args.play_cookie and not args.game_server:
+        username = args.username or input("Username: ")
+        password = args.password or getpass.getpass("Password: ")
     else:
-        if Path(account_file).exists() and not username and not play_cookie:
-            with open(account_file, "r") as file:
-                username, password = file.read().splitlines()
-        elif not username and not play_cookie:
-            username = input("Username: ")
-            password = getpass.getpass("Password: ")
-    gttrl = Gttrl(username, password, game_path, enable_log)
+        play_cookie = args.play_cookie or input("Play cookie: ")
+        game_server = args.game_server or input("Game server: ")
+    gttrl = Gttrl(
+        username,
+        password,
+        args.game_path or config_file["game_path"],
+        args.enable_log or config_file["enable_log"],
+    )
     if username:
         print("Logging in...")
         play_cookie, game_server = gttrl.get_play_cookie()
+        if args.print_play_cookie:
+            print(f"{play_cookie}\n{game_server}")
+            return
     else:
         pass
-    if print_play_cookie:
-        print(play_cookie, game_server)
-        return
-    if not skip_update:
+    if not (args.skip_update or config_file["skip_update"]):
         print("Downloading game files...")
         gttrl.download_game_files()
     print("Launching game...")
     gttrl.launch_game(play_cookie, game_server)
```

### Comparing `gttrl-1.1/gttrl/gttrl.py` & `gttrl-1.2/gttrl/gttrl.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,27 +127,20 @@
         response = response.json()
         if response["success"] == "false":
             raise Exception(response["banner"])
         return response
 
     def get_play_cookie(self):
         login_response = self.login_request()
-        if (
-            login_response["success"] == "partial"
-            and login_response["banner"]
-            == "Please check your email for a ToonGuard code and enter it below."
-        ):
-            while login_response["success"] == "partial":
-                toon_guard_input = input(
-                    "Enter your Toon Guard code received in your account email: "
-                )
-                login_response = self.login_request(
-                    toon_guard_input=toon_guard_input,
-                    toon_guard_token=login_response["responseToken"],
-                )
+        while login_response["success"] == "partial":
+            toon_guard_input = input(f'{login_response["banner"]}: ')
+            login_response = self.login_request(
+                toon_guard_input=toon_guard_input,
+                toon_guard_token=login_response["responseToken"],
+            )
         while login_response["success"] == "delayed":
             login_response = self.login_request(
                 queue_token=login_response["queueToken"]
             )
             time.sleep(5)
         return login_response["cookie"], login_response["gameserver"]
```

### Comparing `gttrl-1.1/PKG-INFO` & `gttrl-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gttrl
-Version: 1.1
+Version: 1.2
 Summary: Glomatico's Toontown Rewritten Launcher
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tqdm
 Project-URL: homepage, https://github.com/glomatico/gttrl
```

