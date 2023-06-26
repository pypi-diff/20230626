# Comparing `tmp/alx-utils-0.7.tar.gz` & `tmp/alx-utils-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alx-utils-0.7.tar", last modified: Sun Jun 25 10:17:13 2023, max compression
+gzip compressed data, was "alx-utils-0.8.tar", last modified: Mon Jun 26 14:09:06 2023, max compression
```

## Comparing `alx-utils-0.7.tar` & `alx-utils-0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.667721 alx-utils-0.7/
--rw-r--r--   0 bio       (1000) bio       (1000)     1064 2023-06-25 09:05:59.000000 alx-utils-0.7/LICENSE
--rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.7/MANIFEST.in
--rw-r--r--   0 bio       (1000) bio       (1000)     1723 2023-06-25 10:17:13.667721 alx-utils-0.7/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)     1501 2023-06-25 09:57:04.000000 alx-utils-0.7/README.md
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.664721 alx-utils-0.7/alx_utils.egg-info/
--rw-r--r--   0 bio       (1000) bio       (1000)     1723 2023-06-25 10:17:12.000000 alx-utils-0.7/alx_utils.egg-info/PKG-INFO
--rw-r--r--   0 bio       (1000) bio       (1000)      417 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-25 10:17:12.000000 alx-utils-0.7/alx_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/entry_points.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/requires.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-25 10:17:13.000000 alx-utils-0.7/alx_utils.egg-info/top_level.txt
--rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-25 10:17:13.668721 alx-utils-0.7/setup.cfg
--rw-r--r--   0 bio       (1000) bio       (1000)      739 2023-06-25 10:16:58.000000 alx-utils-0.7/setup.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.665721 alx-utils-0.7/src/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.7/src/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      534 2023-06-24 18:15:27.000000 alx-utils-0.7/src/alx_utils.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.665721 alx-utils-0.7/tools/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.7/tools/__init__.py
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.666721 alx-utils-0.7/tools/checker/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.7/tools/checker/__init__.py
--rw-r--r--   0 bio       (1000) bio       (1000)      577 2023-06-24 18:30:50.000000 alx-utils-0.7/tools/checker/index.py
--rwxr--r--   0 bio       (1000) bio       (1000)     6586 2023-06-24 13:33:08.000000 alx-utils-0.7/tools/checker/test.bash
-drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-25 10:17:13.666721 alx-utils-0.7/tools/init_task/
--rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.7/tools/init_task/__init__.py
--rwxr--r--   0 bio       (1000) bio       (1000)     4184 2023-06-24 14:51:42.000000 alx-utils-0.7/tools/init_task/scraper.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.762451 alx-utils-0.8/
+-rw-r--r--   0 bio       (1000) bio       (1000)     1064 2023-06-25 09:05:59.000000 alx-utils-0.8/LICENSE
+-rw-r--r--   0 bio       (1000) bio       (1000)       32 2023-06-24 16:49:04.000000 alx-utils-0.8/MANIFEST.in
+-rw-r--r--   0 bio       (1000) bio       (1000)     1766 2023-06-26 14:09:06.761451 alx-utils-0.8/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)     1544 2023-06-26 14:08:36.000000 alx-utils-0.8/README.md
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.753451 alx-utils-0.8/alx_utils.egg-info/
+-rw-r--r--   0 bio       (1000) bio       (1000)     1766 2023-06-26 14:09:05.000000 alx-utils-0.8/alx_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bio       (1000) bio       (1000)      417 2023-06-26 14:09:06.000000 alx-utils-0.8/alx_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)        1 2023-06-26 14:09:05.000000 alx-utils-0.8/alx_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       49 2023-06-26 14:09:06.000000 alx-utils-0.8/alx_utils.egg-info/entry_points.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       15 2023-06-26 14:09:06.000000 alx-utils-0.8/alx_utils.egg-info/requires.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       10 2023-06-26 14:09:06.000000 alx-utils-0.8/alx_utils.egg-info/top_level.txt
+-rw-r--r--   0 bio       (1000) bio       (1000)       38 2023-06-26 14:09:06.763451 alx-utils-0.8/setup.cfg
+-rw-r--r--   0 bio       (1000) bio       (1000)      739 2023-06-26 14:08:51.000000 alx-utils-0.8/setup.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.753451 alx-utils-0.8/src/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:08:14.000000 alx-utils-0.8/src/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      534 2023-06-24 18:15:27.000000 alx-utils-0.8/src/alx_utils.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.754451 alx-utils-0.8/tools/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 20:10:13.000000 alx-utils-0.8/tools/__init__.py
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.756451 alx-utils-0.8/tools/checker/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-24 09:57:35.000000 alx-utils-0.8/tools/checker/__init__.py
+-rw-r--r--   0 bio       (1000) bio       (1000)      577 2023-06-24 18:30:50.000000 alx-utils-0.8/tools/checker/index.py
+-rwxr-xr-x   0 bio       (1000) bio       (1000)     6586 2023-06-26 13:52:33.000000 alx-utils-0.8/tools/checker/test.bash
+drwxr-xr-x   0 bio       (1000) bio       (1000)        0 2023-06-26 14:09:06.759451 alx-utils-0.8/tools/init_task/
+-rw-r--r--   0 bio       (1000) bio       (1000)        0 2023-06-23 19:13:03.000000 alx-utils-0.8/tools/init_task/__init__.py
+-rwxr--r--   0 bio       (1000) bio       (1000)     4289 2023-06-26 13:48:12.000000 alx-utils-0.8/tools/init_task/scraper.py
```

### Comparing `alx-utils-0.7/LICENSE` & `alx-utils-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alx-utils-0.7/PKG-INFO` & `alx-utils-0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: alx-utils
-Version: 0.7
+Version: 0.8
 Summary: A collection of utility tools for ALX
 Home-page: https://github.com/amasin76/alx-utils
 Author: BIO
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALX Utils
 
 ## Description
 
 ALX Utils is a collection of utility tools for ALX. It includes a 
-`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
 `init-task` : automate daily tasks by creating directories and files with specified names, getting prototypes of functions. for scripts setting the shebang, and permissions to executable
+`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
+`soon`: betty pre-commit, devcontainer... 
 
 ## Installation
 
 You can install ALX Utils using `pip` by running the command 
 ```bash
 pip install alx-utils
 ```
 
 ## Usage
 
-### test-suite Tool:
+### init-Task Tool:
 ```bash
-alx-utils -checker shell
+alx-utils -init [HTML_FILE]
 ```
 
-### Init-Task Tool:
+### test-suite Tool:
 ```bash
-alx-utils -init [HTML_FILE]
+alx-utils -checker shell
 ```
 
 ## Dependencies
 
 ALX Utils requires Python >3.6 and depends on the following packages:
 
 - beautifulsoup4
```

### Comparing `alx-utils-0.7/README.md` & `alx-utils-0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # ALX Utils
 
 ## Description
 
 ALX Utils is a collection of utility tools for ALX. It includes a 
-`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
 `init-task` : automate daily tasks by creating directories and files with specified names, getting prototypes of functions. for scripts setting the shebang, and permissions to executable
+`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
+`soon`: betty pre-commit, devcontainer... 
 
 ## Installation
 
 You can install ALX Utils using `pip` by running the command 
 ```bash
 pip install alx-utils
 ```
 
 ## Usage
 
-### test-suite Tool:
+### init-Task Tool:
 ```bash
-alx-utils -checker shell
+alx-utils -init [HTML_FILE]
 ```
 
-### Init-Task Tool:
+### test-suite Tool:
 ```bash
-alx-utils -init [HTML_FILE]
+alx-utils -checker shell
 ```
 
 ## Dependencies
 
 ALX Utils requires Python >3.6 and depends on the following packages:
 
 - beautifulsoup4
```

### Comparing `alx-utils-0.7/alx_utils.egg-info/PKG-INFO` & `alx-utils-0.8/alx_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: alx-utils
-Version: 0.7
+Version: 0.8
 Summary: A collection of utility tools for ALX
 Home-page: https://github.com/amasin76/alx-utils
 Author: BIO
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALX Utils
 
 ## Description
 
 ALX Utils is a collection of utility tools for ALX. It includes a 
-`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
 `init-task` : automate daily tasks by creating directories and files with specified names, getting prototypes of functions. for scripts setting the shebang, and permissions to executable
+`test-suite`: set up a test-driven development environment for your project by creating a test directory and downloading test scripts, and providing a cli for controlling tests
+`soon`: betty pre-commit, devcontainer... 
 
 ## Installation
 
 You can install ALX Utils using `pip` by running the command 
 ```bash
 pip install alx-utils
 ```
 
 ## Usage
 
-### test-suite Tool:
+### init-Task Tool:
 ```bash
-alx-utils -checker shell
+alx-utils -init [HTML_FILE]
 ```
 
-### Init-Task Tool:
+### test-suite Tool:
 ```bash
-alx-utils -init [HTML_FILE]
+alx-utils -checker shell
 ```
 
 ## Dependencies
 
 ALX Utils requires Python >3.6 and depends on the following packages:
 
 - beautifulsoup4
```

### Comparing `alx-utils-0.7/setup.py` & `alx-utils-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="alx-utils",
-    version="0.7",
+    version="0.8",
     description="A collection of utility tools for ALX",
     author="BIO",
     url="https://github.com/amasin76/alx-utils",
     packages=find_packages(include=["src", "src.*", "tools", "tools.*"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={
```

### Comparing `alx-utils-0.7/src/alx_utils.py` & `alx-utils-0.8/src/alx_utils.py`

 * *Files identical despite different names*

### Comparing `alx-utils-0.7/tools/checker/index.py` & `alx-utils-0.8/tools/checker/index.py`

 * *Files identical despite different names*

### Comparing `alx-utils-0.7/tools/checker/test.bash` & `alx-utils-0.8/tools/checker/test.bash`

 * *Files identical despite different names*

### Comparing `alx-utils-0.7/tools/init_task/scraper.py` & `alx-utils-0.8/tools/init_task/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
             file_path = os.path.join(dir_name, file.text)
             add_exec_perms = False
             with open(file_path, "w") as f:
                 # Add shebang line according to file language
                 if file.text.endswith(".py"):
                     f.write("#!/usr/bin/python3\n")
                     add_exec_perms = True
+                    if prototype:
+                        f.write(f"{prototype.text}\n")
                 elif file.text.endswith(".js"):
                     f.write("#!/usr/bin/node\n")
                     add_exec_perms = True
                 elif re.search(r"^[^.]+$(?<!password)(?<!crack)", file.text):
                     f.write("#!/usr/bin/bash\n")
                     add_exec_perms = True
                 # Add executable permissions to the file if a shebang line was added
@@ -64,15 +66,15 @@
                             f"{prototype.text[:-1]} {{\n\t/* your code here */\n}}\n"
                         )
 
 
 def close_include_guard(dir_name):
     # Close the include guard in main.h if it was created
     main_h_path = os.path.join(dir_name, "main.h")
-    if os.path.exists(main_h_path):
+    if main_h_path and os.path.exists(main_h_path):
         with open(main_h_path, "a") as f:
             f.write("\n#endif /* MAIN_H */\n")
 
 
 def create_readme(dir_name):
     # Create README.md file containing "Loading ..."
     readme_path = os.path.join(dir_name, "README.md")
```

