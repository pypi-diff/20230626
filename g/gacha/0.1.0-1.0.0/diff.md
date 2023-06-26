# Comparing `tmp/gacha-0.1.0.tar.gz` & `tmp/gacha-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gacha-0.1.0.tar", max compression
+gzip compressed data, was "gacha-1.0.0.tar", max compression
```

## Comparing `gacha-0.1.0.tar` & `gacha-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1086 2023-06-26 05:56:26.396065 gacha-0.1.0/LICENSE
--rw-r--r--   0        0        0      832 2023-06-26 06:21:32.584345 gacha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-26 05:58:29.353847 gacha-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-06-26 06:23:14.892790 gacha-0.1.0/src/gacha/__init__.py
--rw-r--r--   0        0        0     1517 2023-06-26 07:01:47.104751 gacha-0.1.0/src/gacha/banners.py
--rw-r--r--   0        0        0     1132 2023-06-26 07:01:50.599718 gacha-0.1.0/src/gacha/characters.py
--rw-r--r--   0        0        0     3664 2023-06-26 07:01:53.854574 gacha-0.1.0/src/gacha/engines.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 gacha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-26 05:56:26.396065 gacha-1.0.0/LICENSE
+-rw-r--r--   0        0        0      832 2023-06-26 07:29:28.252893 gacha-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2695 2023-06-26 07:29:40.913640 gacha-1.0.0/README.md
+-rw-r--r--   0        0        0       95 2023-06-26 07:19:12.693042 gacha-1.0.0/src/gacha/__init__.py
+-rw-r--r--   0        0        0     1580 2023-06-26 07:28:02.679171 gacha-1.0.0/src/gacha/banners.py
+-rw-r--r--   0        0        0     1214 2023-06-26 07:27:55.422026 gacha-1.0.0/src/gacha/characters.py
+-rw-r--r--   0        0        0     5197 2023-06-26 07:26:50.665553 gacha-1.0.0/src/gacha/engines.py
+-rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 gacha-1.0.0/PKG-INFO
```

### Comparing `gacha-0.1.0/LICENSE` & `gacha-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gacha-0.1.0/pyproject.toml` & `gacha-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gacha"
-version = "0.1.0"
+version = "1.0.0"
 description = "✨ Gacha"
 license = "MIT"
 authors = ["elaresai <elaresai@gmail.com>"]
 maintainers = ["elaresai <elaresai@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/elaresai/gacha"
 repository = "https://github.com/elaresai/gacha"
```

### Comparing `gacha-0.1.0/src/gacha/banners.py` & `gacha-1.0.0/src/gacha/banners.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from .characters import Character
 
 __all__: Sequence[str] = ("Banner",)
 
 
 @define
 class Banner:
-    """*Character*
+    """*Banner*
 
-    # Fields
+    # 🔌 Fields
 
-    * `fallback` - ...
-    * `name` - ...
-    * `description` - ...
+    * `fallback` - Fallback of the banner
+    * `name` - Name of the banner
+    * `description` - Description of the banner
 
-    # Examples
+    # 🔎 Examples
     ```
     from gacha import Character, Banner
     ...
     Banner(
         "Wanderlust_Invocation",
         characters=[
             Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean"),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gacha-0.1.0/src/gacha/characters.py` & `gacha-1.0.0/src/gacha/characters.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 __all__: Sequence[str] = ("Character",)
 
 
 @define
 class Character:
     """*Character*
 
-    # Fields
+    # 🔌 Fields
 
-    * `weight` - ...
-    * `name` - ...
-    * `description` - ...
+    * `weight` - Relative weight of the character
+    * `name` - Name of the character
+    * `description` - Description of the character
 
-    # Examples
+    # 🔎 Examples
     ```
     from gacha import Character
     ...
     Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean")
     Character(0.003, name="Qiqi", description="https://genshin-impact.fandom.com/wiki/Qiqi")
     Character(0.003, name="Tighnari", description="https://genshin-impact.fandom.com/wiki/Tighnari")
     Character(0.003, name="Keqing", description="https://genshin-impact.fandom.com/wiki/Keqing")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gacha-0.1.0/src/gacha/engines.py` & `gacha-1.0.0/src/gacha/engines.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,82 +14,138 @@
 MULTIPLIER = 100
 
 
 @define
 class Engine:
     """*Engine*
 
-    # Fields
-    * `banners` - ...
+    # 🔌 Fields
+    * `banners` - Banners of the engine
 
-    # Examples
+    # 🔎 Examples
     ```
     from gacha import Engine, Banner, Character
-    ...
+
     Engine(
         [
             Banner(
                 "Wanderlust_Invocation",
                 characters=[
-                    Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean"),
-                    Character(0.003, name="Qiqi", description="https://genshin-impact.fandom.com/wiki/Qiqi"),
-                    Character(0.003, name="Tighnari", description="https://genshin-impact.fandom.com/wiki/Tighnari"),
-                    Character(0.003, name="Keqing", description="https://genshin-impact.fandom.com/wiki/Keqing"),
-                    Character(0.003, name="Mona", description="https://genshin-impact.fandom.com/wiki/Mona"),
-                    Character(0.003, name="Dehya", description="https://genshin-impact.fandom.com/wiki/Dehya"),
-                    Character(0.003, name="Diluc", description="https://genshin-impact.fandom.com/wiki/Diluc"),
-                    ...
+                    Character(
+                        0.003,
+                        name="Jean",
+                        description="https://genshin-impact.fandom.com/wiki/Jean",
+                    ),
+                    Character(
+                        0.003,
+                        name="Qiqi",
+                        description="https://genshin-impact.fandom.com/wiki/Qiqi",
+                    ),
+                    Character(
+                        0.003,
+                        name="Tighnari",
+                        description="https://genshin-impact.fandom.com/wiki/Tighnari",
+                    ),
+                    Character(
+                        0.003,
+                        name="Keqing",
+                        description="https://genshin-impact.fandom.com/wiki/Keqing",
+                    ),
+                    Character(
+                        0.003,
+                        name="Mona",
+                        description="https://genshin-impact.fandom.com/wiki/Mona",
+                    ),
+                    Character(
+                        0.003,
+                        name="Dehya",
+                        description="https://genshin-impact.fandom.com/wiki/Dehya",
+                    ),
+                    Character(
+                        0.003,
+                        name="Diluc",
+                        description="https://genshin-impact.fandom.com/wiki/Diluc",
+                    ),
+                    ...,
                 ],
                 name="Wanderlust_Invocation",
-                description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation"
+                description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation",
             ),
         ]
     )
     ...
     ```
     """
 
     banners: Optional[Sequence[Banner]] = None
 
     def roll(self, fallback: str) -> Character:
         """*roll*
 
         # Arguments
 
-        * `fallback`
+        * `fallback` - Fallback of the banner
 
-        # Examples
+        # 🔎 Examples
         ```
         from gacha import Engine, Banner, Character
-        ...
+
         engine = Engine(
             [
                 Banner(
                     "Wanderlust_Invocation",
                     characters=[
-                        Character(0.003, name="Jean", description="https://genshin-impact.fandom.com/wiki/Jean"),
-                        Character(0.003, name="Qiqi", description="https://genshin-impact.fandom.com/wiki/Qiqi"),
-                        Character(0.003, name="Tighnari", description="https://genshin-impact.fandom.com/wiki/Tighnari"),
-                        Character(0.003, name="Keqing", description="https://genshin-impact.fandom.com/wiki/Keqing"),
-                        Character(0.003, name="Mona", description="https://genshin-impact.fandom.com/wiki/Mona"),
-                        Character(0.003, name="Dehya", description="https://genshin-impact.fandom.com/wiki/Dehya"),
-                        Character(0.003, name="Diluc", description="https://genshin-impact.fandom.com/wiki/Diluc"),
-                        ...
+                        Character(
+                            0.003,
+                            name="Jean",
+                            description="https://genshin-impact.fandom.com/wiki/Jean",
+                        ),
+                        Character(
+                            0.003,
+                            name="Qiqi",
+                            description="https://genshin-impact.fandom.com/wiki/Qiqi",
+                        ),
+                        Character(
+                            0.003,
+                            name="Tighnari",
+                            description="https://genshin-impact.fandom.com/wiki/Tighnari",
+                        ),
+                        Character(
+                            0.003,
+                            name="Keqing",
+                            description="https://genshin-impact.fandom.com/wiki/Keqing",
+                        ),
+                        Character(
+                            0.003,
+                            name="Mona",
+                            description="https://genshin-impact.fandom.com/wiki/Mona",
+                        ),
+                        Character(
+                            0.003,
+                            name="Dehya",
+                            description="https://genshin-impact.fandom.com/wiki/Dehya",
+                        ),
+                        Character(
+                            0.003,
+                            name="Diluc",
+                            description="https://genshin-impact.fandom.com/wiki/Diluc",
+                        ),
+                        ...,
                     ],
                     name="Wanderlust_Invocation",
-                    description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation"
+                    description="https://genshin-impact.fandom.com/wiki/Wanderlust_Invocation",
                 ),
             ]
         )
 
         character = engine.roll()
 
-        print(character.name) # Jean
-        print(character.description) # https://genshin-impact.fandom.com/wiki/Jean
-        ...
+        print(character.name)  # Jean
+        print(character.description)  # https://genshin-impact.fandom.com/wiki/Jean
+
         ```
         """
         for banner in self.banners:
             if banner.fallback != fallback:
                 continue
 
             population = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

