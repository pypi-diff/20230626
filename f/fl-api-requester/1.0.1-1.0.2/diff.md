# Comparing `tmp/fl-api-requester-1.0.1.tar.gz` & `tmp/fl-api-requester-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl-api-requester-1.0.1.tar", last modified: Sun Jun 25 21:18:41 2023, max compression
+gzip compressed data, was "fl-api-requester-1.0.2.tar", last modified: Mon Jun 26 17:13:01 2023, max compression
```

## Comparing `fl-api-requester-1.0.1.tar` & `fl-api-requester-1.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.364666 fl-api-requester-1.0.1/
--rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1266 2023-06-25 21:18:41.363664 fl-api-requester-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-06-25 20:58:36.000000 fl-api-requester-1.0.1/README.md
--rw-rw-rw-   0        0        0      596 2023-06-25 21:18:16.000000 fl-api-requester-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 21:18:41.365666 fl-api-requester-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.275661 fl-api-requester-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.296661 fl-api-requester-1.0.1/src/fl_api_requester/
--rw-rw-rw-   0        0        0     1856 2023-06-25 12:53:25.000000 fl-api-requester-1.0.1/src/fl_api_requester/FLAPIConnectionData.py
--rw-rw-rw-   0        0        0     9406 2023-06-25 20:27:55.000000 fl-api-requester-1.0.1/src/fl_api_requester/FLAPIRequester.py
--rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.1/src/fl_api_requester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.321662 fl-api-requester-1.0.1/src/fl_api_requester/dto/
--rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/DTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.279661 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.324664 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/
--rw-rw-rw-   0        0        0      173 2023-06-25 20:29:10.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
--rw-rw-rw-   0        0        0      179 2023-06-25 20:29:23.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.326663 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/authentication/
--rw-rw-rw-   0        0        0      229 2023-06-25 20:29:27.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.334662 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/
--rw-rw-rw-   0        0        0      299 2023-06-25 20:29:32.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
--rw-rw-rw-   0        0        0      251 2023-06-25 20:29:34.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
--rw-rw-rw-   0        0        0      222 2023-06-25 20:29:37.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.338662 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/
--rw-rw-rw-   0        0        0      279 2023-06-25 20:29:41.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
--rw-rw-rw-   0        0        0      233 2023-06-25 20:29:43.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
--rw-rw-rw-   0        0        0      295 2023-06-25 20:29:46.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.344663 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/
--rw-rw-rw-   0        0        0      178 2023-06-25 20:29:50.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
--rw-rw-rw-   0        0        0      186 2023-06-25 20:29:52.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
--rw-rw-rw-   0        0        0      239 2023-06-25 20:29:56.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
--rw-rw-rw-   0        0        0      281 2023-06-25 20:29:59.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.349430 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/
--rw-rw-rw-   0        0        0      178 2023-06-25 20:30:02.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/StartWarDTO.py
--rw-rw-rw-   0        0        0      176 2023-06-25 20:30:05.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/StopWarDTO.py
--rw-rw-rw-   0        0        0      336 2023-06-25 20:30:08.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.289661 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.352664 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/
--rw-rw-rw-   0        0        0      343 2023-06-25 20:30:36.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
--rw-rw-rw-   0        0        0      169 2023-06-25 20:30:44.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.353663 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/authentication/
--rw-rw-rw-   0        0        0      266 2023-06-25 20:30:48.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.354662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/discord/
--rw-rw-rw-   0        0        0      321 2023-06-25 20:30:56.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/discord/DiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.356662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/
--rw-rw-rw-   0        0        0      268 2023-06-25 20:31:00.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/PlanetDTO.py
--rw-rw-rw-   0        0        0      287 2023-06-25 20:31:07.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.357662 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/player/
--rw-rw-rw-   0        0        0      447 2023-06-25 20:31:17.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/player/PlayerDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.360663 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/
--rw-rw-rw-   0        0        0      437 2023-06-25 20:31:27.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
--rw-rw-rw-   0        0        0      543 2023-06-25 20:31:33.000000 fl-api-requester-1.0.1/src/fl_api_requester/dto/response/war/WarDTO.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.361663 fl-api-requester-1.0.1/src/fl_api_requester/exception/
--rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.1/src/fl_api_requester/exception/APIErrorException.py
-drwxrwxrwx   0        0        0        0 2023-06-25 21:18:41.320661 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/
--rw-rw-rw-   0        0        0     1266 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-25 21:18:41.000000 fl-api-requester-1.0.1/src/fl_api_requester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.692184 fl-api-requester-1.0.2/
+-rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-06-26 17:13:01.691183 fl-api-requester-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-06-26 17:09:29.000000 fl-api-requester-1.0.2/README.md
+-rw-rw-rw-   0        0        0      597 2023-06-26 17:12:29.000000 fl-api-requester-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:13:01.692184 fl-api-requester-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.578059 fl-api-requester-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.630061 fl-api-requester-1.0.2/src/fl_api_requester/
+-rw-rw-rw-   0        0        0     2237 2023-06-26 16:51:37.000000 fl-api-requester-1.0.2/src/fl_api_requester/FLAPIConnectionData.py
+-rw-rw-rw-   0        0        0     7921 2023-06-26 17:05:48.000000 fl-api-requester-1.0.2/src/fl_api_requester/FLAPIRequester.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.2/src/fl_api_requester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.658191 fl-api-requester-1.0.2/src/fl_api_requester/dto/
+-rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/DTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.582059 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.661188 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/
+-rw-rw-rw-   0        0        0      164 2023-06-26 16:25:59.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
+-rw-rw-rw-   0        0        0      170 2023-06-26 16:26:03.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.664186 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/authentication/
+-rw-rw-rw-   0        0        0      188 2023-06-26 16:26:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.669192 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/
+-rw-rw-rw-   0        0        0      246 2023-06-26 16:26:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
+-rw-rw-rw-   0        0        0      214 2023-06-26 16:26:47.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
+-rw-rw-rw-   0        0        0      204 2023-06-26 16:26:57.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.672188 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/
+-rw-rw-rw-   0        0        0      210 2023-06-26 16:27:19.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:27:28.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
+-rw-rw-rw-   0        0        0      226 2023-06-26 16:27:44.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.676184 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:30:05.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
+-rw-rw-rw-   0        0        0      173 2023-06-26 16:30:13.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:30:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
+-rw-rw-rw-   0        0        0      244 2023-06-26 16:30:38.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.680195 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:31:11.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/StartWarDTO.py
+-rw-rw-rw-   0        0        0      159 2023-06-26 16:30:56.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/StopWarDTO.py
+-rw-rw-rw-   0        0        0      252 2023-06-26 16:31:09.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.592064 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.683222 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/
+-rw-rw-rw-   0        0        0      341 2023-06-26 16:10:18.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:11:22.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.684207 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/authentication/
+-rw-rw-rw-   0        0        0      255 2023-06-26 16:08:21.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.685222 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/discord/
+-rw-rw-rw-   0        0        0      285 2023-06-26 16:31:38.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/discord/DiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.687183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/
+-rw-rw-rw-   0        0        0      225 2023-06-26 16:11:39.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/PlanetDTO.py
+-rw-rw-rw-   0        0        0      250 2023-06-26 16:31:50.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.688183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/player/
+-rw-rw-rw-   0        0        0      398 2023-06-26 16:24:19.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/player/PlayerDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.690183 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/
+-rw-rw-rw-   0        0        0      493 2023-06-26 16:45:51.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
+-rw-rw-rw-   0        0        0      332 2023-06-26 16:11:00.000000 fl-api-requester-1.0.2/src/fl_api_requester/dto/response/war/WarDTO.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.690183 fl-api-requester-1.0.2/src/fl_api_requester/exception/
+-rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.2/src/fl_api_requester/exception/APIErrorException.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:13:01.657183 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1956 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 17:13:01.000000 fl-api-requester-1.0.2/src/fl_api_requester.egg-info/top_level.txt
```

### Comparing `fl-api-requester-1.0.1/LICENSE` & `fl-api-requester-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.1/PKG-INFO` & `fl-api-requester-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.1
+Version: 1.0.2
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Intallation
+# Installation
 
 ```
 pip install fl-api-requester
 ```
 
 # Usage
 
 ```python
 from fl_api_requester import *
 
 connection_data = FLAPIConnectionData()
+connection_data.api_uri = "http://localhost:8080"
 connection_data.set_credentials("username", "password")
 
 try:
+    api_requester = FLAPIRequester(connection_data)
+
     # Login
-    api_requester = FLAPIRequester()
-    connection_data.set_token(api_requester.login(connection_data).token)
+    api_requester.login()
 
     # Get some data
-    player = api_requester.get_player("Galactifer", connection_data)
-    alliance = api_requester.get_alliance("France Leader", connection_data)
+    player = api_requester.get_player("Galactifer")
+    alliance = api_requester.get_alliance("France Leader")
 
     print(player)
+    print(alliance)
     print(len(alliance.players))
 
-    # Start a War
-    war = api_requester.start_war(StartWarDTO("Luxure Culinaire"), connection_data)
+    # Get a War attack
+    attack = api_requester.get_player_attacks("Galactifer")
 
-    print(war.alliance, war.opponent)
+    print(f"Galactifer attacked on {attack[0].timestamp_to_datetime():%d/%m/%Y at %H:%M:%S}")
 except APIErrorException as e:
     print(e.api_error)
 ```
```

### Comparing `fl-api-requester-1.0.1/README.md` & `fl-api-requester-1.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-# Intallation
+# Installation
 
 ```
 pip install fl-api-requester
 ```
 
 # Usage
 
 ```python
 from fl_api_requester import *
 
 connection_data = FLAPIConnectionData()
+connection_data.api_uri = "http://localhost:8080"
 connection_data.set_credentials("username", "password")
 
 try:
+    api_requester = FLAPIRequester(connection_data)
+
     # Login
-    api_requester = FLAPIRequester()
-    connection_data.set_token(api_requester.login(connection_data).token)
+    api_requester.login()
 
     # Get some data
-    player = api_requester.get_player("Galactifer", connection_data)
-    alliance = api_requester.get_alliance("France Leader", connection_data)
+    player = api_requester.get_player("Galactifer")
+    alliance = api_requester.get_alliance("France Leader")
 
     print(player)
+    print(alliance)
     print(len(alliance.players))
 
-    # Start a War
-    war = api_requester.start_war(StartWarDTO("Luxure Culinaire"), connection_data)
+    # Get a War attack
+    attack = api_requester.get_player_attacks("Galactifer")
 
-    print(war.alliance, war.opponent)
+    print(f"Galactifer attacked on {attack[0].timestamp_to_datetime():%d/%m/%Y at %H:%M:%S}")
 except APIErrorException as e:
     print(e.api_error)
 ```
```

### Comparing `fl-api-requester-1.0.1/pyproject.toml` & `fl-api-requester-1.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fl-api-requester"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="FL-GL", email="franceleadergl@gmail.com" }
 ]
 description = "The France Leader API requester."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 dependencies=[
-    "munch", "requests"
+    "dacite", "requests"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester"
```

### Comparing `fl-api-requester-1.0.1/src/fl_api_requester/FLAPIConnectionData.py` & `fl-api-requester-1.0.2/src/fl_api_requester/FLAPIConnectionData.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 class FLAPIConnectionData:
     """
     Contains all the connection data of the API (credentials, Discord server's ID...).
     """
 
     def __init__(self) -> None:
+        self.api_uri = None
         self.username = None
         self.password = None
         self.token = None
         self.discord_id = None
 
+    def get_api_uri(self) -> str:
+        """
+        Returns the defined API URI.
+        """
+        return self.api_uri
+
     def get_credentials(self) -> tuple[str, str]:
         """
         Returns the user credentials as a tuple. The tuples is formatted as following : (username, password).
         The tuple values can be None if the credentials hasn't been set.
         """
         return (self.username, self.password)
     
@@ -24,14 +31,25 @@
 
     def get_discord_id(self) -> int:
         """
         Returns the Discord server's ID that make the request. Returns None if the ID hasn't been set.
         """
         return self.discord_id
 
+    def set_api_uri(self, api_uri: str) -> None:
+        """
+        Set the API URI.
+
+        Parameters
+        ----------
+        - api_uri: `str`
+            The API URI to define.
+        """
+        self.api_uri = api_uri
+
     def set_credentials(self, username: str, password: str) -> None:
         """
         Set the current connection credentials.
 
         Parameters
         ----------
         - username: `str`
```

### Comparing `fl-api-requester-1.0.1/src/fl_api_requester/exception/APIErrorException.py` & `fl-api-requester-1.0.2/src/fl_api_requester/exception/APIErrorException.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.1/src/fl_api_requester.egg-info/PKG-INFO` & `fl-api-requester-1.0.2/src/fl_api_requester.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.1
+Version: 1.0.2
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Intallation
+# Installation
 
 ```
 pip install fl-api-requester
 ```
 
 # Usage
 
 ```python
 from fl_api_requester import *
 
 connection_data = FLAPIConnectionData()
+connection_data.api_uri = "http://localhost:8080"
 connection_data.set_credentials("username", "password")
 
 try:
+    api_requester = FLAPIRequester(connection_data)
+
     # Login
-    api_requester = FLAPIRequester()
-    connection_data.set_token(api_requester.login(connection_data).token)
+    api_requester.login()
 
     # Get some data
-    player = api_requester.get_player("Galactifer", connection_data)
-    alliance = api_requester.get_alliance("France Leader", connection_data)
+    player = api_requester.get_player("Galactifer")
+    alliance = api_requester.get_alliance("France Leader")
 
     print(player)
+    print(alliance)
     print(len(alliance.players))
 
-    # Start a War
-    war = api_requester.start_war(StartWarDTO("Luxure Culinaire"), connection_data)
+    # Get a War attack
+    attack = api_requester.get_player_attacks("Galactifer")
 
-    print(war.alliance, war.opponent)
+    print(f"Galactifer attacked on {attack[0].timestamp_to_datetime():%d/%m/%Y at %H:%M:%S}")
 except APIErrorException as e:
     print(e.api_error)
 ```
```

### Comparing `fl-api-requester-1.0.1/src/fl_api_requester.egg-info/SOURCES.txt` & `fl-api-requester-1.0.2/src/fl_api_requester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

