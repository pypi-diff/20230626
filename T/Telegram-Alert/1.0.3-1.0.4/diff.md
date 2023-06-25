# Comparing `tmp/Telegram Alert-1.0.3.tar.gz` & `tmp/Telegram Alert-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Telegram Alert-1.0.3.tar", last modified: Fri Dec 16 15:48:46 2022, max compression
+gzip compressed data, was "Telegram Alert-1.0.4.tar", last modified: Sun Jun 25 22:28:33 2023, max compression
```

## Comparing `Telegram Alert-1.0.3.tar` & `Telegram Alert-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-12-16 15:48:46.290288 Telegram Alert-1.0.3/
--rw-r--r--   0 arsen     (1000) arsen     (1000)        8 2022-11-01 02:34:24.000000 Telegram Alert-1.0.3/MANIFEST.in
--rw-r--r--   0 arsen     (1000) arsen     (1000)      493 2022-12-16 15:48:46.290288 Telegram Alert-1.0.3/PKG-INFO
--rw-r--r--   0 arsen     (1000) arsen     (1000)      175 2022-11-04 22:33:08.000000 Telegram Alert-1.0.3/README.md
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-12-16 15:48:46.286288 Telegram Alert-1.0.3/Telegram_Alert.egg-info/
--rw-r--r--   0 arsen     (1000) arsen     (1000)      493 2022-12-16 15:48:46.000000 Telegram Alert-1.0.3/Telegram_Alert.egg-info/PKG-INFO
--rw-r--r--   0 arsen     (1000) arsen     (1000)      258 2022-12-16 15:48:46.000000 Telegram Alert-1.0.3/Telegram_Alert.egg-info/SOURCES.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-12-16 15:48:46.000000 Telegram Alert-1.0.3/Telegram_Alert.egg-info/dependency_links.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-11-08 12:24:10.000000 Telegram Alert-1.0.3/Telegram_Alert.egg-info/not-zip-safe
--rw-r--r--   0 arsen     (1000) arsen     (1000)        8 2022-12-16 15:48:46.000000 Telegram Alert-1.0.3/Telegram_Alert.egg-info/top_level.txt
--rw-r--r--   0 arsen     (1000) arsen     (1000)       38 2022-12-16 15:48:46.290288 Telegram Alert-1.0.3/setup.cfg
--rw-r--r--   0 arsen     (1000) arsen     (1000)      594 2022-12-16 15:47:48.000000 Telegram Alert-1.0.3/setup.py
-drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2022-12-16 15:48:46.290288 Telegram Alert-1.0.3/tgalert/
--rw-r--r--   0 arsen     (1000) arsen     (1000)       39 2022-11-04 22:37:02.000000 Telegram Alert-1.0.3/tgalert/__init__.py
--rw-r--r--   0 arsen     (1000) arsen     (1000)     3342 2022-12-16 15:47:08.000000 Telegram Alert-1.0.3/tgalert/tgalert.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2023-06-25 22:28:33.205803 Telegram Alert-1.0.4/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        8 2022-11-01 02:34:24.000000 Telegram Alert-1.0.4/MANIFEST.in
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      493 2023-06-25 22:28:33.205803 Telegram Alert-1.0.4/PKG-INFO
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      175 2022-11-04 22:33:08.000000 Telegram Alert-1.0.4/README.md
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2023-06-25 22:28:33.201803 Telegram Alert-1.0.4/Telegram_Alert.egg-info/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      493 2023-06-25 22:28:33.000000 Telegram Alert-1.0.4/Telegram_Alert.egg-info/PKG-INFO
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      258 2023-06-25 22:28:33.000000 Telegram Alert-1.0.4/Telegram_Alert.egg-info/SOURCES.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2023-06-25 22:28:33.000000 Telegram Alert-1.0.4/Telegram_Alert.egg-info/dependency_links.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        1 2022-11-08 12:24:10.000000 Telegram Alert-1.0.4/Telegram_Alert.egg-info/not-zip-safe
+-rw-r--r--   0 arsen     (1000) arsen     (1000)        8 2023-06-25 22:28:33.000000 Telegram Alert-1.0.4/Telegram_Alert.egg-info/top_level.txt
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       38 2023-06-25 22:28:33.205803 Telegram Alert-1.0.4/setup.cfg
+-rw-r--r--   0 arsen     (1000) arsen     (1000)      594 2023-06-25 22:24:32.000000 Telegram Alert-1.0.4/setup.py
+drwxr-xr-x   0 arsen     (1000) arsen     (1000)        0 2023-06-25 22:28:33.205803 Telegram Alert-1.0.4/tgalert/
+-rw-r--r--   0 arsen     (1000) arsen     (1000)       39 2022-11-04 22:37:02.000000 Telegram Alert-1.0.4/tgalert/__init__.py
+-rw-r--r--   0 arsen     (1000) arsen     (1000)     3349 2023-06-25 22:22:38.000000 Telegram Alert-1.0.4/tgalert/tgalert.py
```

### Comparing `Telegram Alert-1.0.3/setup.py` & `Telegram Alert-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.3'
+version = '1.0.4'
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='Telegram Alert',
     version=version,
```

### Comparing `Telegram Alert-1.0.3/tgalert/tgalert.py` & `Telegram Alert-1.0.4/tgalert/tgalert.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     async def send_alert(self, error_text: str):
         if self.bot_token is None:
             return
         url = f'https://api.telegram.org/bot{self.bot_token}/sendMessage'
         params = {'chat_id': self.alert_chat, 'text': error_text[:4096], 'parse_mode': 'HTML',
                   'disable_notification': 'false'}
         async with self.session.post(url, params=params) as response:
-            if response.status == 200:
+            if response.status in (200, 429):
                 return
             else:
                 raise RuntimeError(await response.text())
 
     @asynccontextmanager
     async def catch_alert(self, *format_args, reraise=True, **format_kwargs):
         try:
```

