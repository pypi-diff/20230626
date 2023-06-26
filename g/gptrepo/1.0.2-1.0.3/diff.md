# Comparing `tmp/gptrepo-1.0.2.tar.gz` & `tmp/gptrepo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptrepo-1.0.2.tar", last modified: Fri Mar 17 13:07:32 2023, max compression
+gzip compressed data, was "gptrepo-1.0.3.tar", last modified: Mon Jun 26 02:10:00 2023, max compression
```

## Comparing `gptrepo-1.0.2.tar` & `gptrepo-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.256041 gptrepo-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.216043 gptrepo-1.0.2/.github/
--rw-rw-rw-   0        0        0       46 2023-03-17 05:29:59.000000 gptrepo-1.0.2/.github/CODEOWNERS
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.221043 gptrepo-1.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1901 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.gitignore
--rw-rw-rw-   0        0        0       65 2023-03-17 12:59:19.000000 gptrepo-1.0.2/.gptignore
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.222042 gptrepo-1.0.2/.vscode/
--rw-rw-rw-   0        0        0      818 2023-03-17 12:59:22.000000 gptrepo-1.0.2/.vscode/settings.json
--rw-rw-rw-   0        0        0     1064 2023-03-17 12:59:22.000000 gptrepo-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      100 2023-03-17 12:59:22.000000 gptrepo-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3342 2023-03-17 13:07:32.255042 gptrepo-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2690 2023-03-17 13:06:44.000000 gptrepo-1.0.2/README.md
--rw-rw-rw-   0        0        0      400 2023-03-17 12:59:22.000000 gptrepo-1.0.2/activate.sh
--rw-rw-rw-   0        0        0      341 2023-03-17 12:59:22.000000 gptrepo-1.0.2/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-03-17 12:59:22.000000 gptrepo-1.0.2/make_venv.py
--rw-rw-rw-   0        0        0      803 2023-03-17 13:07:16.000000 gptrepo-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-17 12:59:22.000000 gptrepo-1.0.2/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 13:07:32.256041 gptrepo-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-03-17 13:04:12.000000 gptrepo-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.198042 gptrepo-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.226043 gptrepo-1.0.2/src/gpt_repository_loader/
--rw-rw-rw-   0        0        0      164 2023-03-17 12:59:22.000000 gptrepo-1.0.2/src/gpt_repository_loader/.gptignore
--rw-rw-rw-   0        0        0        0 2023-03-17 12:59:22.000000 gptrepo-1.0.2/src/gpt_repository_loader/__init__.py
--rw-rw-rw-   0        0        0      216 2023-03-17 12:59:22.000000 gptrepo-1.0.2/src/gpt_repository_loader/cli.py
--rw-rw-rw-   0        0        0     4319 2023-03-17 12:59:22.000000 gptrepo-1.0.2/src/gpt_repository_loader/gpt_repository_loader.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.244041 gptrepo-1.0.2/src/gptrepo.egg-info/
--rw-rw-rw-   0        0        0     3342 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-17 13:07:32.000000 gptrepo-1.0.2/src/gptrepo.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.247043 gptrepo-1.0.2/tests/
--rw-rw-rw-   0        0        0      340 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.248043 gptrepo-1.0.2/tests/test_data/
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.252042 gptrepo-1.0.2/tests/test_data/example_repo/
--rw-rw-rw-   0        0        0       16 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/example_repo/.gptignore
--rw-rw-rw-   0        0        0       18 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/example_repo/file1.txt
--rw-rw-rw-   0        0        0       40 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/example_repo/file2.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:07:32.254041 gptrepo-1.0.2/tests/test_data/example_repo/folder1/
--rw-rw-rw-   0        0        0       32 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/example_repo/folder1/file3.py
--rw-rw-rw-   0        0        0       18 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/example_repo/folder1/file4.txt
--rw-rw-rw-   0        0        0      126 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_data/expected_output.txt
--rw-rw-rw-   0        0        0     2173 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tests/test_gpt_repository_loader.py
--rw-rw-rw-   0        0        0      469 2023-03-17 12:59:22.000000 gptrepo-1.0.2/tox.ini
--rw-rw-rw-   0        0        0      291 2023-03-17 12:59:22.000000 gptrepo-1.0.2/upload_package.sh
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.530949 gptrepo-1.0.3/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.525133 gptrepo-1.0.3/.github/
+-rw-r--r--   0 niteris    (501) staff       (20)       46 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.github/CODEOWNERS
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.526146 gptrepo-1.0.3/.github/workflows/
+-rw-r--r--   0 niteris    (501) staff       (20)      855 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.github/workflows/lint.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      801 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.github/workflows/push_macos.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      803 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.github/workflows/push_ubuntu.yml
+-rw-r--r--   0 niteris    (501) staff       (20)      800 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.github/workflows/push_win.yml
+-rw-r--r--   0 niteris    (501) staff       (20)     1901 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.gitignore
+-rw-r--r--   0 niteris    (501) staff       (20)       65 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.gptignore
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.526382 gptrepo-1.0.3/.vscode/
+-rw-r--r--   0 niteris    (501) staff       (20)      818 2023-06-26 01:58:47.000000 gptrepo-1.0.3/.vscode/settings.json
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2023-06-26 01:58:47.000000 gptrepo-1.0.3/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)      100 2023-06-26 01:58:47.000000 gptrepo-1.0.3/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     2790 2023-06-26 02:10:00.530749 gptrepo-1.0.3/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     2207 2023-06-26 02:07:10.000000 gptrepo-1.0.3/README.md
+-rwxr-xr-x   0 niteris    (501) staff       (20)      400 2023-06-26 02:09:43.000000 gptrepo-1.0.3/activate.sh
+-rwxr-xr-x   0 niteris    (501) staff       (20)      341 2023-06-26 01:58:47.000000 gptrepo-1.0.3/lint.sh
+-rw-r--r--   0 niteris    (501) staff       (20)     2138 2023-06-26 01:58:47.000000 gptrepo-1.0.3/make_venv.py
+-rw-r--r--   0 niteris    (501) staff       (20)      803 2023-06-26 02:06:28.000000 gptrepo-1.0.3/pyproject.toml
+-rw-r--r--   0 niteris    (501) staff       (20)       42 2023-06-26 01:58:47.000000 gptrepo-1.0.3/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-06-26 02:10:00.531005 gptrepo-1.0.3/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     1095 2023-06-26 01:58:47.000000 gptrepo-1.0.3/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.521207 gptrepo-1.0.3/src/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.527402 gptrepo-1.0.3/src/gpt_repository_loader/
+-rw-r--r--   0 niteris    (501) staff       (20)      219 2023-06-26 02:03:03.000000 gptrepo-1.0.3/src/gpt_repository_loader/.gptignore
+-rw-r--r--   0 niteris    (501) staff       (20)        0 2023-06-26 01:58:47.000000 gptrepo-1.0.3/src/gpt_repository_loader/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)      216 2023-06-26 01:58:47.000000 gptrepo-1.0.3/src/gpt_repository_loader/cli.py
+-rw-r--r--   0 niteris    (501) staff       (20)     4319 2023-06-26 01:58:47.000000 gptrepo-1.0.3/src/gpt_repository_loader/gpt_repository_loader.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.528707 gptrepo-1.0.3/src/gptrepo.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     2790 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      996 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       59 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/entry_points.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       10 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/requires.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       22 2023-06-26 02:10:00.000000 gptrepo-1.0.3/src/gptrepo.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.529101 gptrepo-1.0.3/tests/
+-rw-r--r--   0 niteris    (501) staff       (20)      340 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_cli.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.529304 gptrepo-1.0.3/tests/test_data/
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.530047 gptrepo-1.0.3/tests/test_data/example_repo/
+-rw-r--r--   0 niteris    (501) staff       (20)       16 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/example_repo/.gptignore
+-rw-r--r--   0 niteris    (501) staff       (20)       18 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/example_repo/file1.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       40 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/example_repo/file2.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-06-26 02:10:00.530438 gptrepo-1.0.3/tests/test_data/example_repo/folder1/
+-rw-r--r--   0 niteris    (501) staff       (20)       32 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/example_repo/folder1/file3.py
+-rw-r--r--   0 niteris    (501) staff       (20)       18 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/example_repo/folder1/file4.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      126 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_data/expected_output.txt
+-rw-r--r--   0 niteris    (501) staff       (20)     2173 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tests/test_gpt_repository_loader.py
+-rw-r--r--   0 niteris    (501) staff       (20)      469 2023-06-26 01:58:47.000000 gptrepo-1.0.3/tox.ini
+-rwxr-xr-x   0 niteris    (501) staff       (20)      291 2023-06-26 01:58:47.000000 gptrepo-1.0.3/upload_package.sh
```

### Comparing `gptrepo-1.0.2/.github/workflows/lint.yml` & `gptrepo-1.0.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/.github/workflows/push_macos.yml` & `gptrepo-1.0.3/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/.github/workflows/push_ubuntu.yml` & `gptrepo-1.0.3/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/.github/workflows/push_win.yml` & `gptrepo-1.0.3/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/.gitignore` & `gptrepo-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/.vscode/settings.json` & `gptrepo-1.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/LICENSE` & `gptrepo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/README.md` & `gptrepo-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 # gptrepo
 
-This is a package of the very excellent [gptrepo](https://github.com/mpoon/gptrepo) by mpoon.
+This is a fork of the very excellent [gpt-repository-loader](https://github.com/mpoon/gpt-repository-loader) by mpoon.
 
 
 Usage
 ```python
 pip install gptrepo
 gptrepo  # now output.txt should appear in the current directory
 ```
 
-This tool concatenates through all the files in teh repo and adds ai prompts which can be used for chat gpt conversations.
+This tool concatenates through all the files in the repo and adds ai prompts which can be used for chat gpt conversations.
 
-This will be particularly useful when chat gpt4-32k is release. Right now this will only work on very small repos.
+Simply open up the file, copy and paste it into the chat gpt window and then ask your question about the code.
+
+This will be particularly useful when chat gpt4-32k is released. Right now this will only work on very small repos.
 
 [![Linting](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)
 
 [![MacOS_Tests](../../actions/workflows/push_macos.yml/badge.svg)](../../actions/workflows/push_macos.yml)
 [![Ubuntu_Tests](../../actions/workflows/push_ubuntu.yml/badge.svg)](../../actions/workflows/push_ubuntu.yml)
 [![Win_Tests](../../actions/workflows/push_win.yml/badge.svg)](../../actions/workflows/push_win.yml)
 
 `gptrepo` is a command-line tool that converts the contents of a Git repository into a text format, preserving the structure of the files and file contents. The generated output can be interpreted by AI language models, allowing them to process the repository's contents for various tasks, such as code review or documentation generation.
 
 ## Contributing
-Some context around building this is [located here](https://github.com/mpoon/gptrepo/discussions/18). Appreciate any issues and pull requests in the spirit of having mostly GPT build out this tool. Using [ChatGPT Plus](https://chat.openai.com/) is recommended for quick access to GPT-4.
-
-## Getting Started
-
-To get started with `gptrepo`, follow these steps:
-
-1. Ensure you have Python 3 installed on your system.
-2. Clone or download the `gptrepo` repository.
-3. Navigate to the repository's root directory in your terminal.
-4. Run `gptrepo` with the following command:
-
-   ```bash
-   python gpt_repository_loader.py /path/to/git/repository
-   ```
-    Replace `/path/to/git/repository` with the path to the Git repository you want to process.
-
-5. The tool will generate an output.txt file containing the text representation of the repository. You can now use this file as input for AI language models or other text-based processing tasks.
+Some context around building this is [located here](https://github.com/mpoon/gpt-repository-loader/discussions/18). Appreciate any issues and pull requests in the spirit of having mostly GPT build out this tool. Using [ChatGPT Plus](https://chat.openai.com/) is recommended for quick access to GPT-4.
 
 ## Running Tests
 
 To run the tests for `gptrepo`, follow these steps:
 
 1. Ensure you have Python 3 installed on your system.
 2. Navigate to the repository's root directory in your terminal.
 3. Run the tests with the following command:
 
    ```bash
-   python -m unittest test_gpt_repository_loader.py
+   tox
    ```
 Now, the test harness is added to the `gptrepo` project. You can run the tests by executing the command `tox` in your terminal.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
+
+## Versions
+
+  * 1.0.3: Remove media files from concatenation.
```

### Comparing `gptrepo-1.0.2/make_venv.py` & `gptrepo-1.0.3/make_venv.py`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/pyproject.toml` & `gptrepo-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "pyperclip"
 ]
 
-version = "1.0.2"
+version = "1.0.3"
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
     "i",
     "ok",
     "id",
```

### Comparing `gptrepo-1.0.2/setup.py` & `gptrepo-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/src/gpt_repository_loader/gpt_repository_loader.py` & `gptrepo-1.0.3/src/gpt_repository_loader/gpt_repository_loader.py`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/src/gptrepo.egg-info/SOURCES.txt` & `gptrepo-1.0.3/src/gptrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gptrepo-1.0.2/tests/test_gpt_repository_loader.py` & `gptrepo-1.0.3/tests/test_gpt_repository_loader.py`

 * *Files identical despite different names*

