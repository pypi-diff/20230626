# Comparing `tmp/tstickers-2022.1.tar.gz` & `tmp/tstickers-2022.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tstickers-2022.1.tar", max compression
+gzip compressed data, was "tstickers-2022.1.1.tar", max compression
```

## Comparing `tstickers-2022.1.tar` & `tstickers-2022.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2021-11-11 20:20:38.715516 tstickers-2022.1/LICENSE.md
--rw-r--r--   0        0        0     1809 2022-02-01 23:16:34.719545 tstickers-2022.1/pyproject.toml
--rw-r--r--   0        0        0     7727 2022-02-01 23:14:18.934412 tstickers-2022.1/README.md
--rw-r--r--   0        0        0     1815 2022-02-01 23:03:10.465732 tstickers-2022.1/tstickers/__init__.py
--rw-r--r--   0        0        0      111 2022-02-01 23:03:10.465732 tstickers-2022.1/tstickers/__main__.py
--rw-r--r--   0        0        0     1814 2022-02-01 23:04:23.526136 tstickers-2022.1/tstickers/caching.py
--rw-r--r--   0        0        0     3140 2022-02-01 23:10:28.598835 tstickers-2022.1/tstickers/convert.py
--rw-r--r--   0        0        0     6500 2022-02-01 23:09:26.330313 tstickers-2022.1/tstickers/downloader.py
--rw-r--r--   0        0        0     8608 2022-02-01 23:16:45.173401 tstickers-2022.1/setup.py
--rw-r--r--   0        0        0     8783 2022-02-01 23:16:45.173401 tstickers-2022.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-01 17:54:52.749148 tstickers-2022.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1987 2023-06-25 22:57:21.503776 tstickers-2022.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8866 2023-06-25 22:48:01.541663 tstickers-2022.1.1/README.md
+-rw-r--r--   0        0        0     1855 2023-06-25 22:56:29.649766 tstickers-2022.1.1/tstickers/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-25 22:56:29.650774 tstickers-2022.1.1/tstickers/__main__.py
+-rw-r--r--   0        0        0     1814 2023-06-25 22:56:29.647355 tstickers-2022.1.1/tstickers/caching.py
+-rw-r--r--   0        0        0     3154 2023-06-25 22:56:29.648355 tstickers-2022.1.1/tstickers/convert.py
+-rw-r--r--   0        0        0     6500 2023-06-25 22:56:29.648670 tstickers-2022.1.1/tstickers/downloader.py
+-rw-r--r--   0        0        0    10053 1970-01-01 00:00:00.000000 tstickers-2022.1.1/setup.py
+-rw-r--r--   0        0        0    10234 1970-01-01 00:00:00.000000 tstickers-2022.1.1/PKG-INFO
```

### Comparing `tstickers-2022.1/LICENSE.md` & `tstickers-2022.1.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# MIT License
-
-Copyright (c) 2020 Kieran W
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+# MIT License
+
+Copyright (c) 2020 Kieran W
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tstickers-2022.1/tstickers/__init__.py` & `tstickers-2022.1.1/tstickers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import argparse
 from pathlib import Path
 from sys import exit as sysexit
 
 from .downloader import StickerDownloader
 
 
-def cli():
+def cli():  # pragma: no cover
 	"""cli entry point"""
 	parser = argparse.ArgumentParser("Welcome to TStickers, providing all of your sticker needs")
 	parser.add_argument(
 		"-t",
 		"--token",
 		help="Pass in a bot token inline",
 	)
@@ -68,9 +68,9 @@
 			continue
 		print("-" * 60)
 		_ = downloader.downloadPack(stickerPack)
 		print("-" * 60)
 		downloader.convertPack(pack, args.frameskip, args.scale)
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
 	cli()
```

### Comparing `tstickers-2022.1/tstickers/caching.py` & `tstickers-2022.1.1/tstickers/caching.py`

 * *Files identical despite different names*

### Comparing `tstickers-2022.1/tstickers/convert.py` & `tstickers-2022.1.1/tstickers/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	Args:
 		root (Path): the path of the root directory
 		directory (Path|str): the directory name
 
 	Returns:
 		Path: the full path
 	"""
-	(root / directory).mkdir(exist_ok=True)
+	(root / directory).mkdir(parents=True, exist_ok=True)
 	return root / directory
 
 
 def convertWithPIL(inputFile: str) -> str:
 	"""Convert the webp file to png
 
 	Args:
```

### Comparing `tstickers-2022.1/tstickers/downloader.py` & `tstickers-2022.1.1/tstickers/downloader.py`

 * *Files identical despite different names*

### Comparing `tstickers-2022.1/PKG-INFO` & `tstickers-2022.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 Metadata-Version: 2.1
 Name: tstickers
-Version: 2022.1
+Version: 2022.1.1
 Summary: Download sticker packs from Telegram
 Home-page: https://github.com/FHPythonUtils/TStickers
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: Pillow (>=9.0.0,<10)
-Requires-Dist: emoji (>=1.6.3,<2)
-Requires-Dist: pyrlottie (>=2022,<2024)
-Requires-Dist: requests (>=2.27.1,<3)
-Requires-Dist: requests-cache (>=0.9.1,<2)
+Requires-Dist: Pillow (>=9.5.0,<10)
+Requires-Dist: emoji (>=2.5.1,<3)
+Requires-Dist: pyrlottie (>=2022.0.2,<2024)
+Requires-Dist: requests (>=2.31.0,<3)
+Requires-Dist: requests-cache (>=1.0.1,<2)
 Project-URL: Documentation, https://github.com/FHPythonUtils/TStickers/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/TStickers
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/TStickers.svg?style=for-the-badge)](../../)
 [![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/TStickers.svg?style=for-the-badge)](../../)
 [![Issues](https://img.shields.io/github/issues/FHPythonUtils/TStickers.svg?style=for-the-badge)](../../issues)
 [![License](https://img.shields.io/github/license/FHPythonUtils/TStickers.svg?style=for-the-badge)](/LICENSE.md)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/TStickers.svg?style=for-the-badge)](../../commits/master)
 [![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/TStickers.svg?style=for-the-badge)](../../commits/master)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/tstickers.svg?style=for-the-badge)](https://pypistats.org/packages/tstickers)
 [![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Ftstickers)](https://pepy.tech/project/tstickers)
 [![PyPI Version](https://img.shields.io/pypi/v/tstickers.svg?style=for-the-badge)](https://pypi.org/project/tstickers)
 
-<!-- omit in TOC -->
+<!-- omit in toc -->
 # TStickers - Telegram Sticker Downloader
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
 Download sticker packs from Telegram
 
-NOTE: You need a telegram bot token to make use of the script. Generate a bot
+## Basic Use
+
+- NOTE: You need a telegram bot token to make use of the script. Generate a bot
 token and paste in a file called 'env'. Send a message to @BotFather to get started.
+- Create a file called 'env' (or env.txt) and paste your token
+- Get the URL of the telegram sticker pack
+- Run the program `python -m tstickers`
+- Enter the URL of the sticker pack
+- Get the output in the `downloads` folder.
 
-- [Docs](#docs)
-- [Using](#using)
+More info at [Tutorials](/documentation/tutorials)
+
+- [Basic Use](#basic-use)
+- [Documentation](#documentation)
 	- [Help](#help)
 - [Formats](#formats)
-- [Documentation](#documentation)
 - [Install With PIP](#install-with-pip)
 - [Language information](#language-information)
 	- [Built for](#built-for)
 - [Install Python on Windows](#install-python-on-windows)
 	- [Chocolatey](#chocolatey)
 	- [Windows - Python.org](#windows---pythonorg)
 - [Install Python on Linux](#install-python-on-linux)
@@ -65,39 +74,44 @@
 	- [Dnf](#dnf)
 - [Install Python on MacOS](#install-python-on-macos)
 	- [Homebrew](#homebrew)
 	- [MacOS - Python.org](#macos---pythonorg)
 - [How to run](#how-to-run)
 	- [Windows](#windows)
 	- [Linux/ MacOS](#linux-macos)
+- [Building](#building)
+- [Testing](#testing)
 - [Download Project](#download-project)
 	- [Clone](#clone)
 		- [Using The Command Line](#using-the-command-line)
 		- [Using GitHub Desktop](#using-github-desktop)
 	- [Download Zip File](#download-zip-file)
 - [Community Files](#community-files)
 	- [Licence](#licence)
 	- [Changelog](#changelog)
 	- [Code of Conduct](#code-of-conduct)
 	- [Contributing](#contributing)
 	- [Security](#security)
 	- [Support](#support)
 	- [Rationale](#rationale)
 
-## Docs
+## Documentation
 
-See the [Docs](/DOCS/) for more information.
+A high-level overview of how the documentation is organized organized will help you know
+where to look for certain things:
 
-## Using
-
-- Create a file called 'env' (or env.txt) and paste your token
-- Get the URL of the telegram sticker pack
-- Run the program `python -m tstickers`
-- Enter the URL of the sticker pack
-- Get the output in the `downloads` folder.
+- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
+  started using the software. Start here if you’re new.
+- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
+  machinery. This documentation describes how to use the classes and functions at a lower level
+  and assume that you have a good high-level understanding of the software.
+<!--
+- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
+  may have.
+-->
 
 ### Help
 
 ```sh
 usage: Welcome to TStickers, providing all of your sticker needs [-h] [-t TOKEN] [-p PACK] [--frameskip FRAMESKIP]
                                                                  [--scale SCALE]
 
@@ -123,32 +137,28 @@
 
 ```txt
 + First frame of animated image only
 ```
 
 Note that static images can fail to save as .gif occasionally in testing
 
-## Documentation
-
-See the [Docs](/DOCS/) for more information.
-
 ## Install With PIP
 
 ```python
 pip install tstickers
 ```
 
 Head to https://pypi.org/project/tstickers/ for more info
 
 ## Language information
 
 ### Built for
 
-This program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and
-3.10
+This program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and
+3.11
 
 ## Install Python on Windows
 
 ### Chocolatey
 
 ```powershell
 choco install python
@@ -200,14 +210,44 @@
 
 - Module
 	`python3.x -m [module]` or `[module]` (if module installs a script)
 
 - File
 	`python3.x [file]` or `./[file]`
 
+## Building
+
+This project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This
+command generates the documentation, updates the requirements.txt and builds the library artefacts
+
+Note the functionality provided by fhmake can be approximated by the following
+
+```sh
+handsdown  --cleanup -o documentation/reference
+poetry export -f requirements.txt --output requirements.txt
+poetry export -f requirements.txt --with dev --output requirements_optional.txt
+poetry build
+```
+
+`fhmake audit` can be run to perform additional checks
+
+## Testing
+
+For testing with the version of python used by poetry use
+
+```sh
+poetry run pytest
+```
+
+Alternatively use `tox` to run tests over python 3.8 - 3.11
+
+```sh
+tox
+```
+
 ## Download Project
 
 ### Clone
 
 #### Using The Command Line
 
 1. Press the Clone or download button in the top right
```

