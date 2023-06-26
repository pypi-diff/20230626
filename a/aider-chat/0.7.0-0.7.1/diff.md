# Comparing `tmp/aider-chat-0.7.0.tar.gz` & `tmp/aider-chat-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.7.0.tar", last modified: Sun Jun 25 15:35:15 2023, max compression
+gzip compressed data, was "aider-chat-0.7.1.tar", last modified: Mon Jun 26 00:55:51 2023, max compression
```

## Comparing `aider-chat-0.7.0.tar` & `aider-chat-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 15:35:06.000000 aider-chat-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 15:35:06.000000 aider-chat-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-25 15:35:15.827416 aider-chat-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-06-25 15:35:06.000000 aider-chat-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.819416 aider-chat-0.7.0/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.823416 aider-chat-0.7.0/aider/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30047 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/base_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/editblock_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/editblock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_func_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_func_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-25 15:35:06.000000 aider-chat-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:35:15.827416 aider-chat-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 15:35:06.000000 aider-chat-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_editblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_wholefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:51.804162 aider-chat-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-26 00:55:39.000000 aider-chat-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 00:55:39.000000 aider-chat-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-26 00:55:51.804162 aider-chat-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-06-26 00:55:39.000000 aider-chat-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:51.804162 aider-chat-0.7.1/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:51.804162 aider-chat-0.7.1/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30047 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 00:55:39.000000 aider-chat-0.7.1/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:51.804162 aider-chat-0.7.1/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 00:55:51.000000 aider-chat-0.7.1/aider_chat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 00:55:39.000000 aider-chat-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 00:55:51.804162 aider-chat-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-26 00:55:39.000000 aider-chat-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:51.804162 aider-chat-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-26 00:55:39.000000 aider-chat-0.7.1/tests/test_wholefile.py
```

### Comparing `aider-chat-0.7.0/LICENSE.txt` & `aider-chat-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/PKG-INFO` & `aider-chat-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.7.0
+Version: 0.7.1
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.7.0/README.md` & `aider-chat-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/base_coder.py` & `aider-chat-0.7.1/aider/coders/base_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/editblock_coder.py` & `aider-chat-0.7.1/aider/coders/editblock_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/editblock_prompts.py` & `aider-chat-0.7.1/aider/coders/editblock_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/wholefile_coder.py` & `aider-chat-0.7.1/aider/coders/wholefile_coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 if fname is not None:
                     # ending an existing block
                     saw_fname = None
 
                     full_path = (Path(self.root) / fname).absolute()
 
                     if mode == "diff" and full_path.exists():
-                        orig_lines = full_path.read_text().splitlines()
+                        orig_lines = full_path.read_text().splitlines(keepends=True)
 
                         show_diff = diffs.diff_partial_update(
                             orig_lines,
                             new_lines,
                             final=True,
                         ).splitlines()
                         output += show_diff
@@ -93,15 +93,15 @@
 
         if mode == "diff":
             if fname is not None:
                 # ending an existing block
                 full_path = (Path(self.root) / fname).absolute()
 
                 if mode == "diff" and full_path.exists():
-                    orig_lines = full_path.read_text().splitlines()
+                    orig_lines = full_path.read_text().splitlines(keepends=True)
 
                     show_diff = diffs.diff_partial_update(
                         orig_lines,
                         new_lines,
                     ).splitlines()
                     output += show_diff
```

### Comparing `aider-chat-0.7.0/aider/coders/wholefile_func_coder.py` & `aider-chat-0.7.1/aider/coders/wholefile_func_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/wholefile_func_prompts.py` & `aider-chat-0.7.1/aider/coders/wholefile_func_prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/coders/wholefile_prompts.py` & `aider-chat-0.7.1/aider/coders/wholefile_prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 Once you understand the request you MUST:
 1. Determine if any code changes are needed.
 2. Explain any needed changes.
 3. If changes are needed, output a copy of each file that needs changes.
 """
 
-    system_reminder = """
-To return code you MUST use this *file listing* format:
+    system_reminder = """To suggest changes to a file you MUST return the entire content of the updated file.
+You MUST use this *file listing* format:
 
 path/to/filename.js
 ```javascript
 // entire file content goes in the
 // triple backticked fenced block
 ```
```

### Comparing `aider-chat-0.7.0/aider/commands.py` & `aider-chat-0.7.1/aider/commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/diffs.py` & `aider-chat-0.7.1/aider/diffs.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,24 +29,34 @@
     total_blocks = 30
     filled_blocks = int(total_blocks * percentage // 100)
     empty_blocks = total_blocks - filled_blocks
     bar = block * filled_blocks + empty * empty_blocks
     return bar
 
 
+def assert_newlines(lines):
+    if not lines:
+        return
+    for line in lines:
+        assert line and line[-1] == "\n", line
+
+
 def diff_partial_update(lines_orig, lines_updated, final=False, fname=None):
     """
     Given only the first part of an updated file, show the diff while
     ignoring the block of "deleted" lines that are past the end of the
     partially complete update.
     """
 
     # dump(lines_orig)
     # dump(lines_updated)
 
+    assert_newlines(lines_orig)
+    assert_newlines(lines_orig)
+
     num_orig_lines = len(lines_orig)
 
     if final:
         last_non_deleted = num_orig_lines
     else:
         last_non_deleted = find_last_non_deleted(lines_orig, lines_updated)
```

### Comparing `aider-chat-0.7.0/aider/dump.py` & `aider-chat-0.7.1/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/io.py` & `aider-chat-0.7.1/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/main.py` & `aider-chat-0.7.1/aider/main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/models.py` & `aider-chat-0.7.1/aider/models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/prompts.py` & `aider-chat-0.7.1/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/repomap.py` & `aider-chat-0.7.1/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider/utils.py` & `aider-chat-0.7.1/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.7.1/aider_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.7.0
+Version: 0.7.1
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.7.0/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.7.1/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/setup.py` & `aider-chat-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_coder.py` & `aider-chat-0.7.1/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_commands.py` & `aider-chat-0.7.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_editblock.py` & `aider-chat-0.7.1/tests/test_editblock.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_main.py` & `aider-chat-0.7.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_models.py` & `aider-chat-0.7.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_repomap.py` & `aider-chat-0.7.1/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.7.0/tests/test_wholefile.py` & `aider-chat-0.7.1/tests/test_wholefile.py`

 * *Files identical despite different names*

