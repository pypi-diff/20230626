# Comparing `tmp/apkmod-1.0.1.tar.gz` & `tmp/apkmod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkmod-1.0.1.tar", last modified: Fri Apr 28 15:01:48 2023, max compression
+gzip compressed data, was "apkmod-1.1.0.tar", last modified: Mon Jun 26 13:48:13 2023, max compression
```

## Comparing `apkmod-1.0.1.tar` & `apkmod-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.749643 apkmod-1.0.1/
--rw-rw-rw-   0        0        0    18385 2023-04-09 07:03:40.000000 apkmod-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1561 2023-04-28 15:01:48.749643 apkmod-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1328 2023-04-27 18:34:29.000000 apkmod-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.694615 apkmod-1.0.1/apkmod/
--rw-rw-rw-   0        0        0       24 2023-04-27 10:37:18.000000 apkmod-1.0.1/apkmod/__init__.py
--rw-rw-rw-   0        0        0     3221 2023-04-27 18:17:43.000000 apkmod-1.0.1/apkmod/android_manifest_util.py
--rw-rw-rw-   0        0        0     4023 2023-04-27 08:47:56.000000 apkmod-1.0.1/apkmod/frida_gadget_util.py
--rw-rw-rw-   0        0        0     2582 2023-04-27 18:27:19.000000 apkmod-1.0.1/apkmod/main.py
--rw-rw-rw-   0        0        0     5529 2023-04-27 10:40:53.000000 apkmod-1.0.1/apkmod/smali_injector_util.py
-drwxrwxrwx   0        0        0        0 2023-04-28 15:01:48.746566 apkmod-1.0.1/apkmod.egg-info/
--rw-rw-rw-   0        0        0     1561 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-28 15:01:48.000000 apkmod-1.0.1/apkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 15:01:48.749643 apkmod-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-04-28 15:01:02.000000 apkmod-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.285882 apkmod-1.1.0/
+-rw-rw-rw-   0        0        0    18385 2023-04-09 07:03:40.000000 apkmod-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1554 2023-06-26 13:48:13.283880 apkmod-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2023-06-26 13:43:42.000000 apkmod-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.240882 apkmod-1.1.0/apkmod/
+-rw-rw-rw-   0        0        0       24 2023-04-27 10:37:18.000000 apkmod-1.1.0/apkmod/__init__.py
+-rw-rw-rw-   0        0        0     3221 2023-04-27 18:17:43.000000 apkmod-1.1.0/apkmod/android_manifest_util.py
+-rw-rw-rw-   0        0        0     4023 2023-04-27 08:47:56.000000 apkmod-1.1.0/apkmod/frida_gadget_util.py
+-rw-rw-rw-   0        0        0     2582 2023-04-27 18:27:19.000000 apkmod-1.1.0/apkmod/main.py
+-rw-rw-rw-   0        0        0     5529 2023-04-27 10:40:53.000000 apkmod-1.1.0/apkmod/smali_injector_util.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:48:13.281880 apkmod-1.1.0/apkmod.egg-info/
+-rw-rw-rw-   0        0        0     1554 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 13:48:13.000000 apkmod-1.1.0/apkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:48:13.287884 apkmod-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-26 13:47:19.000000 apkmod-1.1.0/setup.py
```

### Comparing `apkmod-1.0.1/LICENSE` & `apkmod-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.1/PKG-INFO` & `apkmod-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 Metadata-Version: 2.1
 Name: apkmod
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apk frida-gadget injector script
 Home-page: https://github.com/mon231/apkpatcher/
 Author: Ariel Tubul
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # apkpatcher
-Corss-Platform script used to inject frida scripts and gadget to an APK <br />
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fmon231%2Fapkpatcher&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23AC3838&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) <br />
+Corss-Platform tool used to inject frida scripts and gadget to an APK <br />
 This project started as a fork of [apkpatcher](https://github.com/badadaf/apkpatcher) <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only!
 
 ## Installation
-After you made sure that all of the requirements are met, <br />
-You may install the package and use the cmdline tool `apkmod`, which comes with the cmdline tool [`buildapp`](https://github.com/mon231/buildapp) <br />
-
-> pip install apkmod
+The cmdline tool `apkmod`, comes with the tool [`buildapp`](https://github.com/mon231/buildapp) <br />
+Install using a pypi package, then fetch tools for buildapp:
+> pip install apkmod --upgrade && buildapp_fetch_tools
 
 ## Patching process
 This tool gets an android app installation file (`.apk`) and a [frida js-script](https://frida.re/docs/javascript-api/) <br />
 Then builds a new apk with frida-gadget & script runner ready to be installed on non-rooted android devices!
 
 ## Requirements
-The project assumes that installer already has the following tools in his path:
-- android SDK tools (installed from android-sdk online)
-  - aapt (default at SDK\build_tools)
-  - zipalign (default at SDK\build_tools)
-  - apksigner (default at SDK\build_tools)
-  - adb (default at SDK\platform_tools, only required if `-i` flag is used)
-- apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
-- keytool (default at jdk or jre bin folders, only required if `-k` flag is missing)
+The tool uses [`buildapp`](https://github.com/mon231/buildapp) package, <br />
+Therefore you have to provide it's [requirements](https://github.com/mon231/buildapp/#requirements) <br />
+Or run the requirements fetcher tool `buildapp_fetch_tools` after the `pip install` command
```

### Comparing `apkmod-1.0.1/apkmod/android_manifest_util.py` & `apkmod-1.1.0/apkmod/android_manifest_util.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.1/apkmod/frida_gadget_util.py` & `apkmod-1.1.0/apkmod/frida_gadget_util.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.1/apkmod/main.py` & `apkmod-1.1.0/apkmod/main.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.1/apkmod/smali_injector_util.py` & `apkmod-1.1.0/apkmod/smali_injector_util.py`

 * *Files identical despite different names*

### Comparing `apkmod-1.0.1/apkmod.egg-info/PKG-INFO` & `apkmod-1.1.0/apkmod.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 Metadata-Version: 2.1
 Name: apkmod
-Version: 1.0.1
+Version: 1.1.0
 Summary: Apk frida-gadget injector script
 Home-page: https://github.com/mon231/apkpatcher/
 Author: Ariel Tubul
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # apkpatcher
-Corss-Platform script used to inject frida scripts and gadget to an APK <br />
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fmon231%2Fapkpatcher&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23AC3838&title=hits&edge_flat=false)](https://hits.seeyoufarm.com) <br />
+Corss-Platform tool used to inject frida scripts and gadget to an APK <br />
 This project started as a fork of [apkpatcher](https://github.com/badadaf/apkpatcher) <br />
 <br />
 *NOTE* that you should use this tool for debugging / educational purposes only!
 
 ## Installation
-After you made sure that all of the requirements are met, <br />
-You may install the package and use the cmdline tool `apkmod`, which comes with the cmdline tool [`buildapp`](https://github.com/mon231/buildapp) <br />
-
-> pip install apkmod
+The cmdline tool `apkmod`, comes with the tool [`buildapp`](https://github.com/mon231/buildapp) <br />
+Install using a pypi package, then fetch tools for buildapp:
+> pip install apkmod --upgrade && buildapp_fetch_tools
 
 ## Patching process
 This tool gets an android app installation file (`.apk`) and a [frida js-script](https://frida.re/docs/javascript-api/) <br />
 Then builds a new apk with frida-gadget & script runner ready to be installed on non-rooted android devices!
 
 ## Requirements
-The project assumes that installer already has the following tools in his path:
-- android SDK tools (installed from android-sdk online)
-  - aapt (default at SDK\build_tools)
-  - zipalign (default at SDK\build_tools)
-  - apksigner (default at SDK\build_tools)
-  - adb (default at SDK\platform_tools, only required if `-i` flag is used)
-- apktool [installation manual](https://ibotpeaches.github.io/Apktool/install/)
-- keytool (default at jdk or jre bin folders, only required if `-k` flag is missing)
+The tool uses [`buildapp`](https://github.com/mon231/buildapp) package, <br />
+Therefore you have to provide it's [requirements](https://github.com/mon231/buildapp/#requirements) <br />
+Or run the requirements fetcher tool `buildapp_fetch_tools` after the `pip install` command
```

### Comparing `apkmod-1.0.1/setup.py` & `apkmod-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 CURRENT_FOLDER = Path(__file__).parent
 README_PATH = CURRENT_FOLDER / 'README.md'
 
 
 setuptools.setup(
     name = "apkmod",
-    version = "1.0.1",
+    version = "1.1.0",
     author = "Ariel Tubul",
     packages = setuptools.find_packages(),
     long_description=README_PATH.read_text(),
     install_requires = ['requests', 'buildapp'],
     long_description_content_type='text/markdown',
     url = "https://github.com/mon231/apkpatcher/",
     description = "Apk frida-gadget injector script",
```

