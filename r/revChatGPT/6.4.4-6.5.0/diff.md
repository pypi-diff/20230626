# Comparing `tmp/revChatGPT-6.4.4.tar.gz` & `tmp/revChatGPT-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.4.4.tar", last modified: Sat Jun 24 14:53:38 2023, max compression
+gzip compressed data, was "revChatGPT-6.5.0.tar", last modified: Mon Jun 26 15:53:05 2023, max compression
```

## Comparing `revChatGPT-6.4.4.tar` & `revChatGPT-6.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-24 14:53:37.000000 revChatGPT-6.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:53:38.000000 revChatGPT-6.4.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:53:38.071032 revChatGPT-6.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-24 14:53:08.000000 revChatGPT-6.4.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.690529 revChatGPT-6.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.690529 revChatGPT-6.5.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    57017 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.4.4/LICENSE` & `revChatGPT-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/PKG-INFO` & `revChatGPT-6.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.4
+Version: 6.5.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.4/README.md` & `revChatGPT-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/setup.py` & `revChatGPT-6.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 DOCS_PATH = Path(__file__).parents[0] / "docs/README.md"
 PATH = Path("README.md")
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
+VERSION_PATH = Path(__file__).parents[0] / "src/revChatGPT/version.py"
+with open(VERSION_PATH, encoding="utf-8") as f:
+    version = f.read().split('"')[1]
+
 setup(
     name="revChatGPT",
-    version="6.4.4",
+    version=version,
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.4.4/src/revChatGPT/V1.py` & `revChatGPT-6.5.0/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         auth = Authenticator(
             email=self.config.get("email"),
             password=self.config.get("password"),
             proxy=self.config.get("proxy"),
         )
         log.debug("Using authenticator to get access token")
 
-        self.set_access_token(auth.auth())
+        self.set_access_token(auth.get_access_token())
 
     @logger(is_timed=True)
     def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
```

### Comparing `revChatGPT-6.4.4/src/revChatGPT/V3.py` & `revChatGPT-6.5.0/src/revChatGPT/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,15 @@
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
         if self.engine not in ENGINES:
-            raise NotImplementedError(f"Unsupported engine {self.engine}")
-
+            raise NotImplementedError(f"Engine {self.engine} is not supported. Select from {ENGINES}")
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
@@ -191,19 +190,26 @@
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
         self.add_to_conversation(prompt, "user", convo_id=convo_id)
         self.__truncate_conversation(convo_id=convo_id)
         # Get response
+        if os.environ.get("API_URL") and os.environ.get("MODEL_NAME"):
+            # https://learn.microsoft.com/en-us/azure/cognitive-services/openai/chatgpt-quickstart?tabs=command-line&pivots=rest-api
+            url = os.environ.get("API_URL") + "openai/deployments/" + os.environ.get("MODEL_NAME") +"/chat/completions?api-version=2023-05-15"
+            headers = {"Content-Type": "application/json", "api-key": self.api_key}
+        else:
+            url = "https://api.openai.com/v1/chat/completions"
+            headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         response = self.session.post(
-            os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions",
-            headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
+            url,
+            headers=headers,
             json={
-                "model": model or self.engine,
+                "model": os.environ.get("MODEL_NAME") or model or self.engine,
                 "messages": self.conversation[convo_id] if pass_history else [prompt],
                 "stream": True,
                 # kwargs
                 "temperature": kwargs.get("temperature", self.temperature),
                 "top_p": kwargs.get("top_p", self.top_p),
                 "presence_penalty": kwargs.get(
                     "presence_penalty",
@@ -733,7 +739,8 @@
     try:
         main()
     except Exception as exc:
         raise t.CLIError("Command line program unknown error") from exc
     except KeyboardInterrupt:
         print("\nExiting...")
         sys.exit()
+
```

### Comparing `revChatGPT-6.4.4/src/revChatGPT/__init__.py` & `revChatGPT-6.5.0/src/revChatGPT/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 The __init__ file does not a main file
 
 You can import the following module to use:
 revChatGPT.V1
 revChatGPT.V3
 """
-__version__ = "6.2"
+from .version import version
+
+__version__ = version
 __all__ = ()
 
 
 def verify() -> None:
     # Available Python Version Verify
     from . import typings as t
```

### Comparing `revChatGPT-6.4.4/src/revChatGPT/__main__.py` & `revChatGPT-6.5.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.5.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/src/revChatGPT/typings.py` & `revChatGPT-6.5.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/src/revChatGPT/utils.py` & `revChatGPT-6.5.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.4.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.5.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.4.4
+Version: 6.5.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.4.4/tests/test_recipient.py` & `revChatGPT-6.5.0/tests/test_recipient.py`

 * *Files identical despite different names*

