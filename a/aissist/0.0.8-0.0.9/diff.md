# Comparing `tmp/aissist-0.0.8.tar.gz` & `tmp/aissist-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.8.tar` & `aissist-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.8/LICENSE
--rw-r--r--   0        0        0       59 2023-06-25 04:29:52.904018 aissist-0.0.8/Makefile
--rw-r--r--   0        0        0      247 2023-06-25 04:28:51.416891 aissist-0.0.8/Pipfile
--rw-r--r--   0        0        0    47145 2023-06-25 04:28:58.425264 aissist-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.8/aissist/__init__.py
--rw-r--r--   0        0        0     3343 2023-06-25 04:30:34.361956 aissist-0.0.8/aissist/aissistant.py
--rw-r--r--   0        0        0      741 2023-06-25 04:30:03.600530 aissist-0.0.8/aissist/spinner.py
--rw-r--r--   0        0        0      175 2023-06-25 04:40:30.359800 aissist-0.0.8/aissist/version.py
--rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.8/images/screenshot.png
--rw-r--r--   0        0        0      898 2023-06-25 04:40:40.319994 aissist-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.9/LICENSE
+-rw-r--r--   0        0        0       59 2023-06-25 04:29:52.904018 aissist-0.0.9/Makefile
+-rw-r--r--   0        0        0      247 2023-06-26 09:38:32.789716 aissist-0.0.9/Pipfile
+-rw-r--r--   0        0        0    47145 2023-06-25 04:28:58.425264 aissist-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.9/aissist/__init__.py
+-rw-r--r--   0        0        0     3501 2023-06-26 10:01:57.305104 aissist-0.0.9/aissist/aissistant.py
+-rw-r--r--   0        0        0     2513 2023-06-26 10:06:26.009018 aissist-0.0.9/aissist/config.py
+-rw-r--r--   0        0        0      741 2023-06-25 04:30:03.600530 aissist-0.0.9/aissist/spinner.py
+-rw-r--r--   0        0        0       21 2023-06-26 10:06:48.571978 aissist-0.0.9/aissist/version.py
+-rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.9/images/screenshot.png
+-rw-r--r--   0        0        0      898 2023-06-26 10:06:58.335541 aissist-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.9/PKG-INFO
```

### Comparing `aissist-0.0.8/LICENSE` & `aissist-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.8/Pipfile.lock` & `aissist-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aissist-0.0.8/README.md` & `aissist-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aissist-0.0.8/aissist/aissistant.py` & `aissist-0.0.9/aissist/aissistant.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import openai
 from prompt_toolkit import PromptSession
 from pygments import highlight
 from pygments.formatters import TerminalFormatter
 from pygments.lexers import guess_lexer
 
+from .config import Config
 from .spinner import Spinner
 from .version import __version__
 
 try:
     openai.api_key = os.environ["OPENAI_API_KEY"]
 except KeyError:
     print("Please put your API key in the OPENAI_API_KEY environment variable.")
@@ -71,28 +72,31 @@
         elif inside_block is True:
             current_block += line + "\n"
         else:
             line = bold_single_backticks(line)
             sys.stdout.write(line)
 
 
-def loop(messages):
+def loop(messages, config: Config):
     """Main loop for the program"""
 
     result = session.prompt(
         ">>> ", multiline=True, prompt_continuation=prompt_continuation
     )
 
     messages.append({"role": "user", "content": result})
 
+    import pdb; pdb.set_trace()
+
     spinner = Spinner()
     spinner.start()
 
     response = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+        model=config.get("model"),
+        temperature=config.get("temperature"),
         messages=messages,
     )
     message = response["choices"][0]["message"]
 
     spinner.stop()
 
     messages.append(message)
@@ -104,19 +108,21 @@
 
     return messages
 
 
 def main():
     print(f"AIssist v.{__version__}. ESCAPE followed by ENTER to send. Ctrl-C to quit")
 
+    config = Config()
+
     messages = [{"role": "system", "content": prompt}]
 
     try:
         while True:
-            messages = loop(messages)
+            messages = loop(messages, config)
     except (KeyboardInterrupt, EOFError):
         # Ctrl-C and Ctrl-D
         sys.exit(0)
     except Exception:
         raise
```

### Comparing `aissist-0.0.8/aissist/spinner.py` & `aissist-0.0.9/aissist/spinner.py`

 * *Files identical despite different names*

### Comparing `aissist-0.0.8/images/screenshot.png` & `aissist-0.0.9/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `aissist-0.0.8/pyproject.toml` & `aissist-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aissist"
-version = "0.0.8"
+version = "0.0.9"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
```

### Comparing `aissist-0.0.8/PKG-INFO` & `aissist-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissist
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple GPT command line interface
 Author-email: Craig Booth <craigmbooth@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

