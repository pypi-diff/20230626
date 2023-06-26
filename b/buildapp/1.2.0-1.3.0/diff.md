# Comparing `tmp/buildapp-1.2.0.tar.gz` & `tmp/buildapp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildapp-1.2.0.tar", last modified: Fri May  5 13:07:14 2023, max compression
+gzip compressed data, was "buildapp-1.3.0.tar", last modified: Mon Jun 26 13:48:13 2023, max compression
```

## Comparing `buildapp-1.2.0.tar` & `buildapp-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:07:14.757521 buildapp-1.2.0/
--rw-rw-rw-   0        0        0     3458 2023-05-05 13:07:14.757521 buildapp-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3262 2023-05-05 13:04:11.000000 buildapp-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 13:07:14.696576 buildapp-1.2.0/buildapp/
--rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.2.0/buildapp/__init__.py
--rw-rw-rw-   0        0        0     7546 2023-05-05 12:50:18.000000 buildapp-1.2.0/buildapp/buildapp.py
--rw-rw-rw-   0        0        0     6042 2023-05-05 12:57:32.000000 buildapp-1.2.0/buildapp/download_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:07:14.749047 buildapp-1.2.0/buildapp.egg-info/
--rw-rw-rw-   0        0        0     3458 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 13:07:14.000000 buildapp-1.2.0/buildapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 13:07:14.760042 buildapp-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-05-05 13:06:39.000000 buildapp-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.254886 buildapp-1.3.0/
+-rw-rw-rw-   0        0        0     3344 2023-06-26 13:48:13.250882 buildapp-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-06-26 13:45:10.000000 buildapp-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.205884 buildapp-1.3.0/buildapp/
+-rw-rw-rw-   0        0        0       33 2023-04-10 21:02:21.000000 buildapp-1.3.0/buildapp/__init__.py
+-rw-rw-rw-   0        0        0     7546 2023-05-05 12:50:18.000000 buildapp-1.3.0/buildapp/buildapp.py
+-rw-rw-rw-   0        0        0     6042 2023-05-05 12:57:32.000000 buildapp-1.3.0/buildapp/download_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.246884 buildapp-1.3.0/buildapp.egg-info/
+-rw-rw-rw-   0        0        0     3344 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 13:48:13.000000 buildapp-1.3.0/buildapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:48:13.254886 buildapp-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-06-26 13:45:35.000000 buildapp-1.3.0/setup.py
```

### Comparing `buildapp-1.2.0/PKG-INFO` & `buildapp-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildapp
-Version: 1.2.0
+Version: 1.3.0
 Summary: Apk builder script
 Home-page: https://github.com/mon231/buildapp/
 Author: Ariel Tubul
 Description-Content-Type: text/markdown
 
 # buildapp
 Corss-Platform script used to recompile APK that was decompiled by apktool <br/>
@@ -12,17 +12,15 @@
 And rebuild it into a new apk you may install in your devices <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only! <br />
 *NOTE* that you must accept the LICENSE of the tools listed in the [requirements](#Requirements) section
 
 ## Installation
 Simply run:
-> pip install buildapp --upgrade
-If you didn't provide the [requirements](#Requirements) by yourself, use the following command to fetch the tools:
-> buildapp_fetch_tools
+> pip install buildapp --upgrade && buildapp_fetch_tools
 
 Make sure to have python scripts folder in your path, <br/>
 And use the correct version of pip for python3
 
 ## Decompilation process
 Use [`apktool`](https://ibotpeaches.github.io/Apktool/install/) to decompile your application.
 
@@ -54,13 +52,13 @@
     - if asked to, buildapp will install the signed apk on connected adb device (if there's only one) <br/>
     *NOTE* that if you won't provide the same keystore as the original app already installed on your device, you may not be able to install the apk you built by this script unless you'll uninstall the original app first.
     - implemented using [`adb`](https://developer.android.com/tools/adb)
 
 And that's it! Now you have a new apk, waiting to be installed it on your android devices!
 
 ## Requirements
-The project uses these tools (can be fetch using `buildapp_fetch_tools` after `pip install buildapp`):
+The project uses these tools (can be fetched using `buildapp_fetch_tools` after `pip install buildapp`):
 - android SDK tools ([download build_tools](https://dl.google.com/android/repository/build-tools_r33-windows.zip), [download platform_tools](https://dl.google.com/android/repository/platform-tools_r34.0.1-windows.zip))
     - adb (default at SDK\platform_tools, only required if `-i` flag is used)
     - zipalign (default at SDK\build_tools)
     - apksigner (default at SDK\build_tools)
 - apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
```

### Comparing `buildapp-1.2.0/README.md` & `buildapp-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 And rebuild it into a new apk you may install in your devices <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only! <br />
 *NOTE* that you must accept the LICENSE of the tools listed in the [requirements](#Requirements) section
 
 ## Installation
 Simply run:
-> pip install buildapp --upgrade
-If you didn't provide the [requirements](#Requirements) by yourself, use the following command to fetch the tools:
-> buildapp_fetch_tools
+> pip install buildapp --upgrade && buildapp_fetch_tools
 
 Make sure to have python scripts folder in your path, <br/>
 And use the correct version of pip for python3
 
 ## Decompilation process
 Use [`apktool`](https://ibotpeaches.github.io/Apktool/install/) to decompile your application.
 
@@ -46,13 +44,13 @@
     - if asked to, buildapp will install the signed apk on connected adb device (if there's only one) <br/>
     *NOTE* that if you won't provide the same keystore as the original app already installed on your device, you may not be able to install the apk you built by this script unless you'll uninstall the original app first.
     - implemented using [`adb`](https://developer.android.com/tools/adb)
 
 And that's it! Now you have a new apk, waiting to be installed it on your android devices!
 
 ## Requirements
-The project uses these tools (can be fetch using `buildapp_fetch_tools` after `pip install buildapp`):
+The project uses these tools (can be fetched using `buildapp_fetch_tools` after `pip install buildapp`):
 - android SDK tools ([download build_tools](https://dl.google.com/android/repository/build-tools_r33-windows.zip), [download platform_tools](https://dl.google.com/android/repository/platform-tools_r34.0.1-windows.zip))
     - adb (default at SDK\platform_tools, only required if `-i` flag is used)
     - zipalign (default at SDK\build_tools)
     - apksigner (default at SDK\build_tools)
 - apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
```

### Comparing `buildapp-1.2.0/buildapp/buildapp.py` & `buildapp-1.3.0/buildapp/buildapp.py`

 * *Files identical despite different names*

### Comparing `buildapp-1.2.0/buildapp/download_tools.py` & `buildapp-1.3.0/buildapp/download_tools.py`

 * *Files identical despite different names*

### Comparing `buildapp-1.2.0/buildapp.egg-info/PKG-INFO` & `buildapp-1.3.0/buildapp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildapp
-Version: 1.2.0
+Version: 1.3.0
 Summary: Apk builder script
 Home-page: https://github.com/mon231/buildapp/
 Author: Ariel Tubul
 Description-Content-Type: text/markdown
 
 # buildapp
 Corss-Platform script used to recompile APK that was decompiled by apktool <br/>
@@ -12,17 +12,15 @@
 And rebuild it into a new apk you may install in your devices <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only! <br />
 *NOTE* that you must accept the LICENSE of the tools listed in the [requirements](#Requirements) section
 
 ## Installation
 Simply run:
-> pip install buildapp --upgrade
-If you didn't provide the [requirements](#Requirements) by yourself, use the following command to fetch the tools:
-> buildapp_fetch_tools
+> pip install buildapp --upgrade && buildapp_fetch_tools
 
 Make sure to have python scripts folder in your path, <br/>
 And use the correct version of pip for python3
 
 ## Decompilation process
 Use [`apktool`](https://ibotpeaches.github.io/Apktool/install/) to decompile your application.
 
@@ -54,13 +52,13 @@
     - if asked to, buildapp will install the signed apk on connected adb device (if there's only one) <br/>
     *NOTE* that if you won't provide the same keystore as the original app already installed on your device, you may not be able to install the apk you built by this script unless you'll uninstall the original app first.
     - implemented using [`adb`](https://developer.android.com/tools/adb)
 
 And that's it! Now you have a new apk, waiting to be installed it on your android devices!
 
 ## Requirements
-The project uses these tools (can be fetch using `buildapp_fetch_tools` after `pip install buildapp`):
+The project uses these tools (can be fetched using `buildapp_fetch_tools` after `pip install buildapp`):
 - android SDK tools ([download build_tools](https://dl.google.com/android/repository/build-tools_r33-windows.zip), [download platform_tools](https://dl.google.com/android/repository/platform-tools_r34.0.1-windows.zip))
     - adb (default at SDK\platform_tools, only required if `-i` flag is used)
     - zipalign (default at SDK\build_tools)
     - apksigner (default at SDK\build_tools)
 - apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
```

### Comparing `buildapp-1.2.0/setup.py` & `buildapp-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 CURRENT_FOLDER = Path(__file__).parent
 README_PATH = CURRENT_FOLDER / 'README.md'
 
 
 def main():
     setuptools.setup(
         name = "buildapp",
-        version = "1.2.0",
+        version = "1.3.0",
         author = "Ariel Tubul",
         description = "Apk builder script",
         packages = setuptools.find_packages(),
         long_description = README_PATH.read_text(),
         url = "https://github.com/mon231/buildapp/",
         long_description_content_type='text/markdown',
         entry_points = {'console_scripts': ['buildapp=buildapp.buildapp:main', 'buildapp_fetch_tools=buildapp.download_tools:main']},
```

