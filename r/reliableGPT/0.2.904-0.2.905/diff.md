# Comparing `tmp/reliableGPT-0.2.904.tar.gz` & `tmp/reliableGPT-0.2.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.904.tar", last modified: Sun Jun 25 00:50:46 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.905.tar", last modified: Mon Jun 26 21:47:21 2023, max compression
```

## Comparing `reliableGPT-0.2.904.tar` & `reliableGPT-0.2.905.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985941 reliableGPT-0.2.904/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.904/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-25 00:50:46.985836 reliableGPT-0.2.904/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.904/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985169 reliableGPT-0.2.904/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      270 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985587 reliableGPT-0.2.904/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.904/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12007 2023-06-25 00:50:20.000000 reliableGPT-0.2.904/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7964 2023-06-24 23:16:21.000000 reliableGPT-0.2.904/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-25 00:50:46.985980 reliableGPT-0.2.904/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-25 00:50:28.000000 reliableGPT-0.2.904/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.602080 reliableGPT-0.2.905/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.905/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 21:47:21.601967 reliableGPT-0.2.905/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.905/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.601045 reliableGPT-0.2.905/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      356 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       47 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-26 21:47:21.000000 reliableGPT-0.2.905/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-26 21:47:21.601800 reliableGPT-0.2.905/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3048 2023-06-26 21:41:37.000000 reliableGPT-0.2.905/reliablegpt/APICallHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4408 2023-06-26 19:46:40.000000 reliableGPT-0.2.905/reliablegpt/CustomQueue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.905/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    15049 2023-06-26 20:55:31.000000 reliableGPT-0.2.905/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1434 2023-06-26 21:45:37.000000 reliableGPT-0.2.905/reliablegpt/test_batching.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7913 2023-06-26 21:45:29.000000 reliableGPT-0.2.905/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-26 21:47:21.602127 reliableGPT-0.2.905/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      351 2023-06-26 21:46:11.000000 reliableGPT-0.2.905/setup.py
```

### Comparing `reliableGPT-0.2.904/LICENSE` & `reliableGPT-0.2.905/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.904/README.md` & `reliableGPT-0.2.905/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.904/reliablegpt/main.py` & `reliableGPT-0.2.905/reliablegpt/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+## Imports for reliableGPT
 import openai
 from termcolor import colored
 import time
 import functools
 import copy
 import requests
 from posthog import Posthog
 from klotty import Klotty
+from tqdm import tqdm
+
+## Import for Batch requests
+import uuid
+from APICallHandler import APICallHandler
+import time
+import threading
 
 client = Klotty(api_key="re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV") # email client
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -160,14 +168,98 @@
 
         if result == self.graceful_string or len(errors) == 2: # returns a graceful string or got a 2nd exception
             # send an email and alert
             send_emails_task(self.user_email, posthog_metadata, self.send_notification)
     except:
         return # safe function, should not impact error handling if logging fails
 
+class batchRequests:
+    def __init__(self,
+               process_func,
+               max_token_capacity,
+               max_request_capacity,
+               set_timeout=10,
+               verbose=False):
+        super().__init__()
+        self.api_handler = APICallHandler(max_token_capacity,
+                                        max_request_capacity,
+                                        verbose=verbose)
+        self.process_func = process_func
+        self.set_timeout = set_timeout
+        self.verbose = verbose
+
+    def print_verbose(self, *args):
+        if self.verbose:
+            print(*args)
+
+    def get_result(self, text):
+        task_id = uuid.uuid4().int
+        self.print_verbose("task_id: ", task_id)
+
+        self.api_handler.add_task(process_func=self.process_func,
+                                input=text,
+                                task_id=task_id)
+
+        start_time = time.time()
+
+        while time.time() - start_time < self.set_timeout:
+            result = self.api_handler.get_result(task_id)
+        if result:
+            return result
+
+        return None
+
+    def get_results(self):
+        return self.api_handler.get_results()
+
+    def get_result_threaded(self, test_question, results):
+        self.print_verbose(f"Enters reliableGPT with question: {test_question}")
+        start_time = time.time()
+        result = self.get_result(test_question)
+        results.append(result)
+        end_time = time.time()
+        self.print_verbose(f"Gets result from reliableGPT: {result}",
+                        end_time - start_time)
+
+    # def execute(self, questions=[]):
+    #     thread_list = []
+    #     results = []
+    #     print(f"ReliableGPT: Processing {len(questions)} Requests")
+
+    #     for idx, q in enumerate(questions):
+    #         self.api_handler.add_task()
+    #         thread = threading.Thread(target=self.get_result_threaded,
+    #                                 args=(q, results))
+    #     thread.start()
+    #     thread_list.append(thread)
+
+    #     # Join all threads
+    #     for thread in thread_list:
+    #         thread.join()
+
+    #     self.print_verbose("All threads completed.")
+    #     self.print_verbose(results)
+    #     return results
+
+    def execute(self, questions=[]):
+        for question in questions: 
+            task_id = uuid.uuid4().int
+            self.print_verbose("task_id: ", task_id)
+            self.api_handler.add_task(process_func=self.process_func,
+                                        input=question, task_id=task_id)
+            self.api_handler.set_upperbound(len(questions))
+        start_time = time.time() 
+        while time.time() - start_time < self.set_timeout:
+            results = self.api_handler.get_results()
+            if len(results) >= len(questions):
+                return results
+        return self.api_handler.get_results()
+
+
+
 class reliableGPT:
     def __init__(
             self, 
             openai_create_function, 
             fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], 
             graceful_string="Sorry, the OpenAI API is currently down", 
             user_email="",
```

### Comparing `reliableGPT-0.2.904/reliablegpt/tests_main.py` & `reliableGPT-0.2.905/reliablegpt/tests_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import openai
 from main import reliableGPT
 import uuid
 
-openai.api_key = "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"
+openai.api_key = ""
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 # make openAI reliable and safe
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
 openai.Completion.create = reliableGPT(openai.Completion.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
 openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
```

