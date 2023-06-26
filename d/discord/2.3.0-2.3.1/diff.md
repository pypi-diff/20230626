# Comparing `tmp/discord-2.3.0.tar.gz` & `tmp/discord-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-2.3.0.tar", last modified: Mon Jun 12 18:08:14 2023, max compression
+gzip compressed data, was "discord-2.3.1.tar", last modified: Mon Jun 26 08:21:20 2023, max compression
```

## Comparing `discord-2.3.0.tar` & `discord-2.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:08:14.352134 discord-2.3.0/
--rw-rw-rw-   0        0        0      360 2023-06-12 18:08:14.351133 discord-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       82 2021-06-10 01:32:34.000000 discord-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:08:14.350132 discord-2.3.0/discord.egg-info/
--rw-rw-rw-   0        0        0      360 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:08:14.000000 discord-2.3.0/discord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 18:08:14.352134 discord-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-06-12 18:01:57.000000 discord-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:21:20.454998 discord-2.3.1/
+-rw-rw-rw-   0        0        0      360 2023-06-26 08:21:20.454998 discord-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2021-06-10 01:32:34.000000 discord-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 08:21:20.453997 discord-2.3.1/discord.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-06-26 08:21:20.000000 discord-2.3.1/discord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-26 08:21:20.000000 discord-2.3.1/discord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:21:20.000000 discord-2.3.1/discord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-26 08:21:20.000000 discord-2.3.1/discord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:21:20.000000 discord-2.3.1/discord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:21:20.455998 discord-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-06-26 08:21:12.000000 discord-2.3.1/setup.py
```

### Comparing `discord-2.3.0/setup.py` & `discord-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='discord',
-    version='2.3.0',
+    version='2.3.1',
     url='https://github.com/Rapptz/discord.py',
     author='Rapptz',
     description='A mirror package for discord.py. Please install that instead.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=[],
-    install_requires=['discord.py>=2.3.0'],
+    install_requires=['discord.py>=2.3.1'],
 )
```

