# Comparing `tmp/GoogleBard-1.3.2.tar.gz` & `tmp/GoogleBard-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.3.2.tar", last modified: Sat Jun 10 01:54:32 2023, max compression
+gzip compressed data, was "GoogleBard-1.3.3.tar", last modified: Sun Jun 25 19:47:21 2023, max compression
```

## Comparing `GoogleBard-1.3.2.tar` & `GoogleBard-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.301902 GoogleBard-1.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-10 01:54:06.000000 GoogleBard-1.3.2/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:54:32.305903 GoogleBard-1.3.2/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-10 01:54:32.000000 GoogleBard-1.3.2/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:47:21.959103 GoogleBard-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 19:46:55.000000 GoogleBard-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-25 19:47:21.959103 GoogleBard-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-25 19:46:55.000000 GoogleBard-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 19:47:21.959103 GoogleBard-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 19:46:55.000000 GoogleBard-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:47:21.959103 GoogleBard-1.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-25 19:46:55.000000 GoogleBard-1.3.3/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:47:21.959103 GoogleBard-1.3.3/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-25 19:47:21.000000 GoogleBard-1.3.3/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-25 19:47:21.000000 GoogleBard-1.3.3/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:47:21.000000 GoogleBard-1.3.3/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-25 19:47:21.000000 GoogleBard-1.3.3/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 19:47:21.000000 GoogleBard-1.3.3/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.3.2/LICENSE` & `GoogleBard-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.2/PKG-INFO` & `GoogleBard-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.2
+Version: 1.3.3
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.3.2/README.md` & `GoogleBard-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.3.2/setup.py` & `GoogleBard-1.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.3.2",
+    version="1.3.3",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.3.2/src/Bard.py` & `GoogleBard-1.3.3/src/Bard.py`

 * *Files 9% similar despite different names*

```diff
@@ -139,43 +139,67 @@
         proxy: dict = None,
         timeout: int = 20,
     ) -> "AsyncChatbot":
         instance = cls(session_id, proxy, timeout)
         instance.SNlM0e = await instance.__get_snlm0e()
         return instance
 
-    async def save_conversation(self, file_path: str, conversation_name: str):
-        conversations = self.load_conversations(file_path)
-        conversation_details = {
-            {
+    async def save_conversation(self, file_path: str, conversation_name: str) -> None:
+        """
+        Saves conversation to the file
+        :param file_path: file to save (json)
+        :param conversation_name: any name of current conversation (unique one)
+        :return: None
+        """
+        # Load conversations from file
+        conversations = await self.load_conversations(file_path)
+    
+        # Update existing one
+        conversation_exists = False
+        for conversation in conversations:
+            if conversation["conversation_name"] == conversation_name:
+                conversation["conversation_name"] = conversation_name
+                conversation["_reqid"] = self._reqid
+                conversation["conversation_id"] = self.conversation_id
+                conversation["response_id"] = self.response_id
+                conversation["choice_id"] = self.choice_id
+                conversation["SNlM0e"] = self.SNlM0e
+                conversation_exists = True
+    
+        # Create conversation object
+        if not conversation_exists:
+            conversation = {
                 "conversation_name": conversation_name,
                 "_reqid": self._reqid,
                 "conversation_id": self.conversation_id,
                 "response_id": self.response_id,
                 "choice_id": self.choice_id,
                 "SNlM0e": self.SNlM0e,
-            },
-        }
-        conversations.append(conversation_details)
-
+            }
+            conversations.append(conversation)
+    
+        # Save to the file
         with open(file_path, "w", encoding="utf-8") as f:
             json.dump(conversations, f, indent=4)
 
     async def load_conversations(self, file_path: str) -> List[Dict]:
         # Check if file exists
         if not os.path.isfile(file_path):
             return []
         with open(file_path, encoding="utf-8") as f:
             return json.load(f)
 
     async def load_conversation(self, file_path: str, conversation_name: str) -> bool:
         """
-        Loads a conversation from history file. Returns whether the conversation was found.
+        Loads a conversation from history file. Returns whether the conversation was found
+        :param file_path: File with conversations (json)
+        :param conversation_name: unique conversation name
+        :return: True if the conversation was found
         """
-        conversations = self.load_conversations(file_path)
+        conversations = await self.load_conversations(file_path)
         for conversation in conversations:
             if conversation["conversation_name"] == conversation_name:
                 self._reqid = conversation["_reqid"]
                 self.conversation_id = conversation["conversation_id"]
                 self.response_id = conversation["response_id"]
                 self.choice_id = conversation["choice_id"]
                 self.SNlM0e = conversation["SNlM0e"]
@@ -208,15 +232,15 @@
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
         # url params
         params = {
-            "bl": "boq_assistant-bard-web-server_20230606.12_p0",
+            "bl": "boq_assistant-bard-web-server_20230620.14_p0",
             "_reqid": str(self._reqid),
             "rt": "c",
         }
 
         # message arr -> data["f.req"]. Message is double json stringified
         message_struct = [
             [message],
```

### Comparing `GoogleBard-1.3.2/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.3.3/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.3.2
+Version: 1.3.3
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

