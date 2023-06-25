# Comparing `tmp/sigstickers-2022.1.tar.gz` & `tmp/sigstickers-2022.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigstickers-2022.1.tar", max compression
+gzip compressed data, was "sigstickers-2022.1.1.tar", max compression
```

## Comparing `sigstickers-2022.1.tar` & `sigstickers-2022.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2021-11-11 20:20:38.715516 sigstickers-2022.1/LICENSE.md
--rw-r--r--   0        0        0     1829 2022-04-11 22:06:41.870343 sigstickers-2022.1/pyproject.toml
--rw-r--r--   0        0        0     7615 2022-04-06 19:44:34.827902 sigstickers-2022.1/README.md
--rw-r--r--   0        0        0     1358 2022-04-11 22:06:37.870130 sigstickers-2022.1/sigstickers/__init__.py
--rw-r--r--   0        0        0      113 2022-04-11 22:03:14.004729 sigstickers-2022.1/sigstickers/__main__.py
--rw-r--r--   0        0        0     1577 2022-04-11 22:03:14.002735 sigstickers-2022.1/sigstickers/caching.py
--rw-r--r--   0        0        0     4188 2022-04-11 22:03:14.003731 sigstickers-2022.1/sigstickers/downloader.py
--rw-r--r--   0        0        0     8455 2022-04-11 22:06:47.594556 sigstickers-2022.1/setup.py
--rw-r--r--   0        0        0     8660 2022-04-11 22:06:47.594556 sigstickers-2022.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-01 17:54:37.495243 sigstickers-2022.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1940 2023-06-25 22:43:15.685153 sigstickers-2022.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8144 2023-06-25 22:41:04.451342 sigstickers-2022.1.1/README.md
+-rw-r--r--   0        0        0     1358 2023-06-25 22:42:58.989965 sigstickers-2022.1.1/sigstickers/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-25 22:42:58.991154 sigstickers-2022.1.1/sigstickers/__main__.py
+-rw-r--r--   0        0        0     1577 2023-06-25 22:42:58.987966 sigstickers-2022.1.1/sigstickers/caching.py
+-rw-r--r--   0        0        0     4159 2023-06-25 22:42:58.989965 sigstickers-2022.1.1/sigstickers/downloader.py
+-rw-r--r--   0        0        0     9275 1970-01-01 00:00:00.000000 sigstickers-2022.1.1/setup.py
+-rw-r--r--   0        0        0     9493 1970-01-01 00:00:00.000000 sigstickers-2022.1.1/PKG-INFO
```

### Comparing `sigstickers-2022.1/pyproject.toml` & `sigstickers-2022.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 [tool.poetry]
 name = "sigstickers"
-version = "2022.1"
+version = "2022.1.1"
 license = "mit"
 description = "Download sticker packs from Signal"
 authors = ["FredHappyface"]
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Developers",
 	"Intended Audience :: Education",
 	"Natural Language :: English",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: Implementation :: CPython",
 	"Topic :: Software Development :: Libraries :: Python Modules",
 	"Topic :: Utilities",
-	"Topic :: Multimedia :: Graphics"
+	"Topic :: Multimedia :: Graphics",
 ]
 homepage = "https://github.com/FHPythonUtils/SigStickers"
 repository = "https://github.com/FHPythonUtils/SigStickers"
 documentation = "https://github.com/FHPythonUtils/SigStickers/blob/master/README.md"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-Pillow = "<10,>=9.1.0"
-signalstickers-client = "<4,>=3.1.0"
-emoji = "<2,>=1.7.0"
+Pillow = "<10,>=9.5.0"
+signalstickers-client = "<4,>=3.2.0"
+emoji = "<3,>=2.5.1"
 
 [tool.poetry.scripts]
 sigstickers = "sigstickers:cli"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 coverage = "^6.3.2"
 handsdown = "^1.1.0"
 pylint = "^2.13.5"
 
+[tool.black]
+line-length = 100
+target-version = ["py38"]
+
+[tool.isort]
+profile = "black"
+indent = "Tab"
+
+[tool.pydocstyle]
+convention = "google"
+ignore = "D205,D415"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.basic]
 argument-naming-style = "camelCase"
 attr-naming-style = "camelCase"
@@ -46,28 +58,26 @@
 method-naming-style = "camelCase"
 variable-naming-style = "camelCase"
 
 [tool.pylint.format]
 indent-string = "\t"
 
 [tool.pylint.master]
-ignore-patterns = "test_.*?py"
+ignore-paths = ["tests"]
 
 [tool.pylint.messages_control]
 enable = ["F", "E", "W", "R", "C"]
-disable = [
-	"pointless-string-statement",
-	"superfluous-parens",
-	"bad-continuation"
-]
-
-[tool.black]
-line-length = 100
-target-version = ["py37"]
+disable = ["pointless-string-statement", "superfluous-parens"]
 
-[tool.isort]
-profile = "black"
-indent = "Tab"
-
-[tool.pydocstyle]
-convention = "google"
-ignore = "D205,D415"
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+env_list =
+	py311
+	py310
+	py39
+	py38
+
+[testenv]
+deps = pytest
+commands = pytest tests
+"""
```

### Comparing `sigstickers-2022.1/README.md` & `sigstickers-2022.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,251 +1,283 @@
-[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
-[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
-[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../issues)
-[![License](https://img.shields.io/github/license/FHPythonUtils/SigStickers.svg?style=for-the-badge)](/LICENSE.md)
-[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
-[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/sigstickers.svg?style=for-the-badge)](https://pypistats.org/packages/sigstickers)
-[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsigstickers)](https://pepy.tech/project/sigstickers)
-[![PyPI Version](https://img.shields.io/pypi/v/sigstickers.svg?style=for-the-badge)](https://pypi.org/project/sigstickers)
-
-<!-- omit in TOC -->
-# SigStickers - Signal Sticker Downloader
-
-<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
-
-Download sticker packs from Signal
-
-- [Using](#using)
-	- [Help](#help)
-- [Formats](#formats)
-- [Documentation](#documentation)
-- [Install With PIP](#install-with-pip)
-- [Language information](#language-information)
-	- [Built for](#built-for)
-- [Install Python on Windows](#install-python-on-windows)
-	- [Chocolatey](#chocolatey)
-	- [Windows - Python.org](#windows---pythonorg)
-- [Install Python on Linux](#install-python-on-linux)
-	- [Apt](#apt)
-	- [Dnf](#dnf)
-- [Install Python on MacOS](#install-python-on-macos)
-	- [Homebrew](#homebrew)
-	- [MacOS - Python.org](#macos---pythonorg)
-- [How to run](#how-to-run)
-	- [Windows](#windows)
-	- [Linux/ MacOS](#linux-macos)
-- [Download Project](#download-project)
-	- [Clone](#clone)
-		- [Using The Command Line](#using-the-command-line)
-		- [Using GitHub Desktop](#using-github-desktop)
-	- [Download Zip File](#download-zip-file)
-- [Community Files](#community-files)
-	- [Licence](#licence)
-	- [Changelog](#changelog)
-	- [Code of Conduct](#code-of-conduct)
-	- [Contributing](#contributing)
-	- [Security](#security)
-	- [Support](#support)
-	- [Rationale](#rationale)
-
-## Using
-
-- Get the URL of the Signal sticker pack
-- Run the program `python -m sigstickers`
-- Enter the URL of the sticker pack
-- Get the output in the `downloads` folder.
-
-### Help
-
-```sh
-usage: Welcome to SigSticker, providing all of your sticker needs [-h] [-p PACK [PACK ...]]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -p PACK [PACK ...], --pack PACK [PACK ...]
-                        Pass in a pack url inline
-```
-
-## Formats
-
-| Format | Static | Animated |
-| ------ | ------ | -------- |
-| .gif   | ✔$     | ✔$       |
-| .png   | ✔      | +        |
-| .webp  | ✔      | ✔        |
-
-```txt
-+ The first frame of an animated image is saved as png
-$ Some images saved as gif do not render as expected
-```
-
-## Documentation
-
-A high-level overview of how the documentation is organized organized will help you know
-where to look for certain things:
-
-<!--
-- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
-  started using the software. Start here if you’re new.
--->
-- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
-  machinery. This documentation describes how to use the classes and functions at a lower level
-  and assume that you have a good high-level understanding of the software.
-<!--
-- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
-  may have.
--->
-
-## Install With PIP
-
-```python
-pip install sigstickers
-```
-
-Head to https://pypi.org/project/sigstickers/ for more info
-
-## Language information
-
-### Built for
-
-This program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and
-3.10
-
-## Install Python on Windows
-
-### Chocolatey
-
-```powershell
-choco install python
-```
-
-### Windows - Python.org
-
-To install Python, go to https://www.python.org/downloads/windows/ and download the latest
-version.
-
-## Install Python on Linux
-
-### Apt
-
-```bash
-sudo apt install python3.x
-```
-
-### Dnf
-
-```bash
-sudo dnf install python3.x
-```
-
-## Install Python on MacOS
-
-### Homebrew
-
-```bash
-brew install python@3.x
-```
-
-### MacOS - Python.org
-
-To install Python, go to https://www.python.org/downloads/macos/ and download the latest
-version.
-
-## How to run
-
-### Windows
-
-- Module
-	`py -3.x -m [module]` or `[module]` (if module installs a script)
-
-- File
-	`py -3.x [file]` or `./[file]`
-
-### Linux/ MacOS
-
-- Module
-	`python3.x -m [module]` or `[module]` (if module installs a script)
-
-- File
-	`python3.x [file]` or `./[file]`
-
-## Download Project
-
-### Clone
-
-#### Using The Command Line
-
-1. Press the Clone or download button in the top right
-2. Copy the URL (link)
-3. Open the command line and change directory to where you wish to
-clone to
-4. Type 'git clone' followed by URL in step 2
-
-	```bash
-	git clone https://github.com/FHPythonUtils/SigStickers
-	```
-
-More information can be found at
-https://help.github.com/en/articles/cloning-a-repository
-
-#### Using GitHub Desktop
-
-1. Press the Clone or download button in the top right
-2. Click open in desktop
-3. Choose the path for where you want and click Clone
-
-More information can be found at
-https://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop
-
-### Download Zip File
-
-1. Download this GitHub repository
-2. Extract the zip archive
-3. Copy/ move to the desired location
-
-## Community Files
-
-### Licence
-
-MIT License
-Copyright (c) FredHappyface
-(See the [LICENSE](/LICENSE.md) for more information.)
-
-### Changelog
-
-See the [Changelog](/CHANGELOG.md) for more information.
-
-### Code of Conduct
-
-Online communities include people from many backgrounds. The *Project*
-contributors are committed to providing a friendly, safe and welcoming
-environment for all. Please see the
-[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)
- for more information.
-
-### Contributing
-
-Contributions are welcome, please see the
-[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)
-for more information.
-
-### Security
-
-Thank you for improving the security of the project, please see the
-[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)
-for more information.
-
-### Support
-
-Thank you for using this project, I hope it is of use to you. Please be aware that
-those involved with the project often do so for fun along with other commitments
-(such as work, family, etc). Please see the
-[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)
-for more information.
-
-### Rationale
-
-The rationale acts as a guide to various processes regarding projects such as
-the versioning scheme and the programming styles used. Please see the
-[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)
-for more information.
+[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
+[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
+[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../issues)
+[![License](https://img.shields.io/github/license/FHPythonUtils/SigStickers.svg?style=for-the-badge)](/LICENSE.md)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
+[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/sigstickers.svg?style=for-the-badge)](https://pypistats.org/packages/sigstickers)
+[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsigstickers)](https://pepy.tech/project/sigstickers)
+[![PyPI Version](https://img.shields.io/pypi/v/sigstickers.svg?style=for-the-badge)](https://pypi.org/project/sigstickers)
+
+<!-- omit in toc -->
+# SigStickers - Signal Sticker Downloader
+
+<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
+
+Download sticker packs from Signal
+
+- [Using](#using)
+	- [Help](#help)
+- [Formats](#formats)
+- [Documentation](#documentation)
+- [Install With PIP](#install-with-pip)
+- [Language information](#language-information)
+	- [Built for](#built-for)
+- [Install Python on Windows](#install-python-on-windows)
+	- [Chocolatey](#chocolatey)
+	- [Windows - Python.org](#windows---pythonorg)
+- [Install Python on Linux](#install-python-on-linux)
+	- [Apt](#apt)
+	- [Dnf](#dnf)
+- [Install Python on MacOS](#install-python-on-macos)
+	- [Homebrew](#homebrew)
+	- [MacOS - Python.org](#macos---pythonorg)
+- [How to run](#how-to-run)
+	- [Windows](#windows)
+	- [Linux/ MacOS](#linux-macos)
+- [Building](#building)
+- [Testing](#testing)
+- [Download Project](#download-project)
+	- [Clone](#clone)
+		- [Using The Command Line](#using-the-command-line)
+		- [Using GitHub Desktop](#using-github-desktop)
+	- [Download Zip File](#download-zip-file)
+- [Community Files](#community-files)
+	- [Licence](#licence)
+	- [Changelog](#changelog)
+	- [Code of Conduct](#code-of-conduct)
+	- [Contributing](#contributing)
+	- [Security](#security)
+	- [Support](#support)
+	- [Rationale](#rationale)
+
+## Using
+
+- Get the URL of the Signal sticker pack
+- Run the program `python -m sigstickers`
+- Enter the URL of the sticker pack
+- Get the output in the `downloads` folder.
+
+### Help
+
+```sh
+usage: Welcome to SigSticker, providing all of your sticker needs [-h] [-p PACK [PACK ...]]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -p PACK [PACK ...], --pack PACK [PACK ...]
+                        Pass in a pack url inline
+```
+
+## Formats
+
+| Format | Static | Animated |
+| ------ | ------ | -------- |
+| .gif   | ✔$     | ✔$       |
+| .png   | ✔      | +        |
+| .webp  | ✔      | ✔        |
+
+```txt
++ The first frame of an animated image is saved as png
+$ Some images saved as gif do not render as expected
+```
+
+## Documentation
+
+A high-level overview of how the documentation is organized organized will help you know
+where to look for certain things:
+
+<!--
+- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get
+  started using the software. Start here if you’re new.
+-->
+- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the
+  machinery. This documentation describes how to use the classes and functions at a lower level
+  and assume that you have a good high-level understanding of the software.
+<!--
+- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you
+  may have.
+-->
+
+## Install With PIP
+
+```python
+pip install sigstickers
+```
+
+Head to https://pypi.org/project/sigstickers/ for more info
+
+## Language information
+
+### Built for
+
+This program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and
+3.11
+
+## Install Python on Windows
+
+### Chocolatey
+
+```powershell
+choco install python
+```
+
+### Windows - Python.org
+
+To install Python, go to https://www.python.org/downloads/windows/ and download the latest
+version.
+
+## Install Python on Linux
+
+### Apt
+
+```bash
+sudo apt install python3.x
+```
+
+### Dnf
+
+```bash
+sudo dnf install python3.x
+```
+
+## Install Python on MacOS
+
+### Homebrew
+
+```bash
+brew install python@3.x
+```
+
+### MacOS - Python.org
+
+To install Python, go to https://www.python.org/downloads/macos/ and download the latest
+version.
+
+## How to run
+
+### Windows
+
+- Module
+	`py -3.x -m [module]` or `[module]` (if module installs a script)
+
+- File
+	`py -3.x [file]` or `./[file]`
+
+### Linux/ MacOS
+
+- Module
+	`python3.x -m [module]` or `[module]` (if module installs a script)
+
+- File
+	`python3.x [file]` or `./[file]`
+
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
+## Download Project
+
+### Clone
+
+#### Using The Command Line
+
+1. Press the Clone or download button in the top right
+2. Copy the URL (link)
+3. Open the command line and change directory to where you wish to
+clone to
+4. Type 'git clone' followed by URL in step 2
+
+	```bash
+	git clone https://github.com/FHPythonUtils/SigStickers
+	```
+
+More information can be found at
+https://help.github.com/en/articles/cloning-a-repository
+
+#### Using GitHub Desktop
+
+1. Press the Clone or download button in the top right
+2. Click open in desktop
+3. Choose the path for where you want and click Clone
+
+More information can be found at
+https://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop
+
+### Download Zip File
+
+1. Download this GitHub repository
+2. Extract the zip archive
+3. Copy/ move to the desired location
+
+## Community Files
+
+### Licence
+
+MIT License
+Copyright (c) FredHappyface
+(See the [LICENSE](/LICENSE.md) for more information.)
+
+### Changelog
+
+See the [Changelog](/CHANGELOG.md) for more information.
+
+### Code of Conduct
+
+Online communities include people from many backgrounds. The *Project*
+contributors are committed to providing a friendly, safe and welcoming
+environment for all. Please see the
+[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)
+ for more information.
+
+### Contributing
+
+Contributions are welcome, please see the
+[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)
+for more information.
+
+### Security
+
+Thank you for improving the security of the project, please see the
+[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)
+for more information.
+
+### Support
+
+Thank you for using this project, I hope it is of use to you. Please be aware that
+those involved with the project often do so for fun along with other commitments
+(such as work, family, etc). Please see the
+[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)
+for more information.
+
+### Rationale
+
+The rationale acts as a guide to various processes regarding projects such as
+the versioning scheme and the programming styles used. Please see the
+[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)
+for more information.
```

### Comparing `sigstickers-2022.1/sigstickers/__init__.py` & `sigstickers-2022.1.1/sigstickers/__init__.py`

 * *Files identical despite different names*

### Comparing `sigstickers-2022.1/sigstickers/caching.py` & `sigstickers-2022.1.1/sigstickers/caching.py`

 * *Files identical despite different names*

### Comparing `sigstickers-2022.1/sigstickers/downloader.py` & `sigstickers-2022.1.1/sigstickers/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 		directory (str): the directory name
 		root (str): the path of the root directory
 
 	Returns:
 		str: the full path
 	"""
 	fullPath = opj(root, directory)
-	if os.path.isdir(fullPath):
-		pass
-	else:
-		os.mkdir(fullPath)
+	os.makedirs(fullPath, exist_ok=True)
 
 	return fullPath
 
 
 def saveSticker(sticker: Sticker, path: str) -> str:
 	"""Save a sticker
```

### Comparing `sigstickers-2022.1/setup.py` & `sigstickers-2022.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['sigstickers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Pillow>=9.1.0,<10', 'emoji>=1.7.0,<2', 'signalstickers-client>=3.1.0,<4']
+['Pillow>=9.5.0,<10', 'emoji>=2.5.1,<3', 'signalstickers-client>=3.2.0,<4']
 
 entry_points = \
 {'console_scripts': ['sigstickers = sigstickers:cli']}
 
 setup_kwargs = {
     'name': 'sigstickers',
-    'version': '2022.1',
+    'version': '2022.1.1',
     'description': 'Download sticker packs from Signal',
-    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SigStickers.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/sigstickers.svg?style=for-the-badge)](https://pypistats.org/packages/sigstickers)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsigstickers)](https://pepy.tech/project/sigstickers)\n[![PyPI Version](https://img.shields.io/pypi/v/sigstickers.svg?style=for-the-badge)](https://pypi.org/project/sigstickers)\n\n<!-- omit in TOC -->\n# SigStickers - Signal Sticker Downloader\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nDownload sticker packs from Signal\n\n- [Using](#using)\n\t- [Help](#help)\n- [Formats](#formats)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Using\n\n- Get the URL of the Signal sticker pack\n- Run the program `python -m sigstickers`\n- Enter the URL of the sticker pack\n- Get the output in the `downloads` folder.\n\n### Help\n\n```sh\nusage: Welcome to SigSticker, providing all of your sticker needs [-h] [-p PACK [PACK ...]]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -p PACK [PACK ...], --pack PACK [PACK ...]\n                        Pass in a pack url inline\n```\n\n## Formats\n\n| Format | Static | Animated |\n| ------ | ------ | -------- |\n| .gif   | ✔$     | ✔$       |\n| .png   | ✔      | +        |\n| .webp  | ✔      | ✔        |\n\n```txt\n+ The first frame of an animated image is saved as png\n$ Some images saved as gif do not render as expected\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install sigstickers\n```\n\nHead to https://pypi.org/project/sigstickers/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.7 - 3.10 and has been tested with both 3.7 and\n3.10\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SigStickers\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
+    'long_description': '[![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)\n[![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)\n[![Issues](https://img.shields.io/github/issues/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../issues)\n[![License](https://img.shields.io/github/license/FHPythonUtils/SigStickers.svg?style=for-the-badge)](/LICENSE.md)\n[![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)\n[![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)\n[![PyPI Downloads](https://img.shields.io/pypi/dm/sigstickers.svg?style=for-the-badge)](https://pypistats.org/packages/sigstickers)\n[![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsigstickers)](https://pepy.tech/project/sigstickers)\n[![PyPI Version](https://img.shields.io/pypi/v/sigstickers.svg?style=for-the-badge)](https://pypi.org/project/sigstickers)\n\n<!-- omit in toc -->\n# SigStickers - Signal Sticker Downloader\n\n<img src="readme-assets/icons/name.png" alt="Project Icon" width="750">\n\nDownload sticker packs from Signal\n\n- [Using](#using)\n\t- [Help](#help)\n- [Formats](#formats)\n- [Documentation](#documentation)\n- [Install With PIP](#install-with-pip)\n- [Language information](#language-information)\n\t- [Built for](#built-for)\n- [Install Python on Windows](#install-python-on-windows)\n\t- [Chocolatey](#chocolatey)\n\t- [Windows - Python.org](#windows---pythonorg)\n- [Install Python on Linux](#install-python-on-linux)\n\t- [Apt](#apt)\n\t- [Dnf](#dnf)\n- [Install Python on MacOS](#install-python-on-macos)\n\t- [Homebrew](#homebrew)\n\t- [MacOS - Python.org](#macos---pythonorg)\n- [How to run](#how-to-run)\n\t- [Windows](#windows)\n\t- [Linux/ MacOS](#linux-macos)\n- [Building](#building)\n- [Testing](#testing)\n- [Download Project](#download-project)\n\t- [Clone](#clone)\n\t\t- [Using The Command Line](#using-the-command-line)\n\t\t- [Using GitHub Desktop](#using-github-desktop)\n\t- [Download Zip File](#download-zip-file)\n- [Community Files](#community-files)\n\t- [Licence](#licence)\n\t- [Changelog](#changelog)\n\t- [Code of Conduct](#code-of-conduct)\n\t- [Contributing](#contributing)\n\t- [Security](#security)\n\t- [Support](#support)\n\t- [Rationale](#rationale)\n\n## Using\n\n- Get the URL of the Signal sticker pack\n- Run the program `python -m sigstickers`\n- Enter the URL of the sticker pack\n- Get the output in the `downloads` folder.\n\n### Help\n\n```sh\nusage: Welcome to SigSticker, providing all of your sticker needs [-h] [-p PACK [PACK ...]]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -p PACK [PACK ...], --pack PACK [PACK ...]\n                        Pass in a pack url inline\n```\n\n## Formats\n\n| Format | Static | Animated |\n| ------ | ------ | -------- |\n| .gif   | ✔$     | ✔$       |\n| .png   | ✔      | +        |\n| .webp  | ✔      | ✔        |\n\n```txt\n+ The first frame of an animated image is saved as png\n$ Some images saved as gif do not render as expected\n```\n\n## Documentation\n\nA high-level overview of how the documentation is organized organized will help you know\nwhere to look for certain things:\n\n<!--\n- [Tutorials](/documentation/tutorials) take you by the hand through a series of steps to get\n  started using the software. Start here if you’re new.\n-->\n- The [Technical Reference](/documentation/reference) documents APIs and other aspects of the\n  machinery. This documentation describes how to use the classes and functions at a lower level\n  and assume that you have a good high-level understanding of the software.\n<!--\n- The [Help](/documentation/help) guide provides a starting point and outlines common issues that you\n  may have.\n-->\n\n## Install With PIP\n\n```python\npip install sigstickers\n```\n\nHead to https://pypi.org/project/sigstickers/ for more info\n\n## Language information\n\n### Built for\n\nThis program has been written for Python versions 3.8 - 3.11 and has been tested with both 3.8 and\n3.11\n\n## Install Python on Windows\n\n### Chocolatey\n\n```powershell\nchoco install python\n```\n\n### Windows - Python.org\n\nTo install Python, go to https://www.python.org/downloads/windows/ and download the latest\nversion.\n\n## Install Python on Linux\n\n### Apt\n\n```bash\nsudo apt install python3.x\n```\n\n### Dnf\n\n```bash\nsudo dnf install python3.x\n```\n\n## Install Python on MacOS\n\n### Homebrew\n\n```bash\nbrew install python@3.x\n```\n\n### MacOS - Python.org\n\nTo install Python, go to https://www.python.org/downloads/macos/ and download the latest\nversion.\n\n## How to run\n\n### Windows\n\n- Module\n\t`py -3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`py -3.x [file]` or `./[file]`\n\n### Linux/ MacOS\n\n- Module\n\t`python3.x -m [module]` or `[module]` (if module installs a script)\n\n- File\n\t`python3.x [file]` or `./[file]`\n\n## Building\n\nThis project uses https://github.com/FHPythonUtils/FHMake to automate most of the building. This\ncommand generates the documentation, updates the requirements.txt and builds the library artefacts\n\nNote the functionality provided by fhmake can be approximated by the following\n\n```sh\nhandsdown  --cleanup -o documentation/reference\npoetry export -f requirements.txt --output requirements.txt\npoetry export -f requirements.txt --with dev --output requirements_optional.txt\npoetry build\n```\n\n`fhmake audit` can be run to perform additional checks\n\n## Testing\n\nFor testing with the version of python used by poetry use\n\n```sh\npoetry run pytest\n```\n\nAlternatively use `tox` to run tests over python 3.8 - 3.11\n\n```sh\ntox\n```\n\n## Download Project\n\n### Clone\n\n#### Using The Command Line\n\n1. Press the Clone or download button in the top right\n2. Copy the URL (link)\n3. Open the command line and change directory to where you wish to\nclone to\n4. Type \'git clone\' followed by URL in step 2\n\n\t```bash\n\tgit clone https://github.com/FHPythonUtils/SigStickers\n\t```\n\nMore information can be found at\nhttps://help.github.com/en/articles/cloning-a-repository\n\n#### Using GitHub Desktop\n\n1. Press the Clone or download button in the top right\n2. Click open in desktop\n3. Choose the path for where you want and click Clone\n\nMore information can be found at\nhttps://help.github.com/en/desktop/contributing-to-projects/cloning-a-repository-from-github-to-github-desktop\n\n### Download Zip File\n\n1. Download this GitHub repository\n2. Extract the zip archive\n3. Copy/ move to the desired location\n\n## Community Files\n\n### Licence\n\nMIT License\nCopyright (c) FredHappyface\n(See the [LICENSE](/LICENSE.md) for more information.)\n\n### Changelog\n\nSee the [Changelog](/CHANGELOG.md) for more information.\n\n### Code of Conduct\n\nOnline communities include people from many backgrounds. The *Project*\ncontributors are committed to providing a friendly, safe and welcoming\nenvironment for all. Please see the\n[Code of Conduct](https://github.com/FHPythonUtils/.github/blob/master/CODE_OF_CONDUCT.md)\n for more information.\n\n### Contributing\n\nContributions are welcome, please see the\n[Contributing Guidelines](https://github.com/FHPythonUtils/.github/blob/master/CONTRIBUTING.md)\nfor more information.\n\n### Security\n\nThank you for improving the security of the project, please see the\n[Security Policy](https://github.com/FHPythonUtils/.github/blob/master/SECURITY.md)\nfor more information.\n\n### Support\n\nThank you for using this project, I hope it is of use to you. Please be aware that\nthose involved with the project often do so for fun along with other commitments\n(such as work, family, etc). Please see the\n[Support Policy](https://github.com/FHPythonUtils/.github/blob/master/SUPPORT.md)\nfor more information.\n\n### Rationale\n\nThe rationale acts as a guide to various processes regarding projects such as\nthe versioning scheme and the programming styles used. Please see the\n[Rationale](https://github.com/FHPythonUtils/.github/blob/master/RATIONALE.md)\nfor more information.\n',
     'author': 'FredHappyface',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/FHPythonUtils/SigStickers',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `sigstickers-2022.1/PKG-INFO` & `sigstickers-2022.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: sigstickers
-Version: 2022.1
+Version: 2022.1.1
 Summary: Download sticker packs from Signal
 Home-page: https://github.com/FHPythonUtils/SigStickers
 License: MIT
 Author: FredHappyface
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: Pillow (>=9.1.0,<10)
-Requires-Dist: emoji (>=1.7.0,<2)
-Requires-Dist: signalstickers-client (>=3.1.0,<4)
+Requires-Dist: Pillow (>=9.5.0,<10)
+Requires-Dist: emoji (>=2.5.1,<3)
+Requires-Dist: signalstickers-client (>=3.2.0,<4)
 Project-URL: Documentation, https://github.com/FHPythonUtils/SigStickers/blob/master/README.md
 Project-URL: Repository, https://github.com/FHPythonUtils/SigStickers
 Description-Content-Type: text/markdown
 
 [![GitHub top language](https://img.shields.io/github/languages/top/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
 [![Repository size](https://img.shields.io/github/repo-size/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../)
 [![Issues](https://img.shields.io/github/issues/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../issues)
 [![License](https://img.shields.io/github/license/FHPythonUtils/SigStickers.svg?style=for-the-badge)](/LICENSE.md)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
 [![Last commit](https://img.shields.io/github/last-commit/FHPythonUtils/SigStickers.svg?style=for-the-badge)](../../commits/master)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/sigstickers.svg?style=for-the-badge)](https://pypistats.org/packages/sigstickers)
 [![PyPI Total Downloads](https://img.shields.io/badge/dynamic/json?style=for-the-badge&label=total%20downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fsigstickers)](https://pepy.tech/project/sigstickers)
 [![PyPI Version](https://img.shields.io/pypi/v/sigstickers.svg?style=for-the-badge)](https://pypi.org/project/sigstickers)
 
-<!-- omit in TOC -->
+<!-- omit in toc -->
 # SigStickers - Signal Sticker Downloader
 
 <img src="readme-assets/icons/name.png" alt="Project Icon" width="750">
 
 Download sticker packs from Signal
 
 - [Using](#using)
@@ -60,14 +61,16 @@
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
@@ -134,16 +137,16 @@
 
 Head to https://pypi.org/project/sigstickers/ for more info
 
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
@@ -195,14 +198,44 @@
 
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

