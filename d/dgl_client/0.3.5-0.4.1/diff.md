# Comparing `tmp/dgl_client-0.3.5.tar.gz` & `tmp/dgl_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.3.5.tar` & `dgl_client-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,17 @@
--rw-r--r--   0        0        0       51 2023-05-30 14:01:06.441529 dgl_client-0.3.5/.gitignore
--rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.3.5/README.md
--rw-r--r--   0        0        0       64 2023-05-31 17:06:01.123122 dgl_client-0.3.5/dgl_client/__init__.py
--rw-r--r--   0        0        0     7760 2023-05-31 15:47:31.730669 dgl_client-0.3.5/dgl_client/api_cli.py
--rw-r--r--   0        0        0     4434 2023-05-31 12:38:59.807362 dgl_client-0.3.5/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775226 dgl_client-0.3.5/dgl_client/utils.py
--rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.3.5/notebook.ipynb
--rw-r--r--   0        0        0      456 2023-05-30 07:01:38.905722 dgl_client-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 dgl_client-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.1/README.md
+-rw-r--r--   0        0        0       64 2023-06-23 15:01:32.864864 dgl_client-0.4.1/dgl_client/__init__.py
+-rw-r--r--   0        0        0    10719 2023-06-26 10:05:24.809476 dgl_client-0.4.1/dgl_client/api_cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.1/dgl_client/commands/__init__.py
+-rw-r--r--   0        0        0     1667 2023-06-23 14:50:58.125182 dgl_client-0.4.1/dgl_client/commands/chat.py
+-rw-r--r--   0        0        0     3092 2023-06-23 14:14:07.305950 dgl_client-0.4.1/dgl_client/commands/collections.py
+-rw-r--r--   0        0        0     1593 2023-06-23 14:16:53.409030 dgl_client-0.4.1/dgl_client/commands/ls.py
+-rw-r--r--   0        0        0     1008 2023-06-23 14:12:36.247808 dgl_client-0.4.1/dgl_client/commands/utils.py
+-rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.1/dgl_client/main.py
+-rw-r--r--   0        0        0     1448 2023-06-26 10:54:23.480112 dgl_client-0.4.1/dgl_client/main2.py
+-rw-r--r--   0        0        0     2573 2023-06-22 13:02:00.540897 dgl_client-0.4.1/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.1/notebook.ipynb
+-rw-r--r--   0        0        0      484 2023-06-26 10:54:31.687382 dgl_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.1/tests/test_collections.py
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 dgl_client-0.4.1/PKG-INFO
```

### Comparing `dgl_client-0.3.5/README.md` & `dgl_client-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dgl_client-0.3.5/dgl_client/main.py` & `dgl_client-0.4.1/dgl_client/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import argparse
 import logging
 import os
 import sys
-from .api_cli import APIClient, prepare_token
+from .api_cli import APIClient
 import uuid
 from glob import glob
 import json
 
 logFormatter = logging.Formatter("%(asctime)s [%(levelname)-5.5s] - [%(filename)s > %(funcName)s() > %(lineno)s] %(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
-def get_client(args):
+def get_inf_client(args):
   logger.info("Connecting to API Endpoint %s"%args.endpoint)
-  client = APIClient(args.endpoint)    
-  return client
+  client = APIClient(args.endpoint, inf_url=args.inference_url)    
+  return client._inference
 
 def list_models(args):
-  client = get_client(args)
+  client = get_inf_client(args)
   available_models = client.get_available_models()
   logger.info("Available models %s"%str(available_models))
 
   available_wkf = client.get_available_workflows()
   logger.info("Available workflows %s"%str(available_wkf))
 
   return available_models, available_wkf
 
 def list_chats(args):
-  client = get_client(args)
+  client = get_inf_client(args)
   do_login(args, client)
   chats = client.list_chats()
   logger.info("Found %d existing chats"%(len(chats)))
 
   for chat in chats:
     print("* %s - %s"%(chat[0],chat[1][:25]))
 
   return chats
 
 def list_messages(args, chat_id):
-  client = get_client(args)
+  client = get_inf_client(args)
   do_login(args, client)
   messages = client.list_messages(chat_id)
   logger.info("Found %d existing chats"%(len(messages)))
 
   for message in messages:
     print(message)
 
@@ -66,52 +66,55 @@
   if args.access_key:
     client.login(args.access_key)
     return True
 
   return False
 
 def main_chat(args):
-  client = get_client(args)
+  client = get_inf_client(args)
 
   model_config_name = args.model
+  collection = args.use_collection
 
   do_login(args, client)
 
   if args.chat_id:
     chat_id = client.continue_chat(args.chat_id)
   else:
     chat_id = client.create_chat()
 
   logger.info(f"Chat ID: {chat_id}")
 
   message = args.message
 
-  events = client.send_message(message, model_config_name)
+  events = client.send_message(message, model_config_name, collection=collection)
 
   print()
   print("You: %s"%(message))
   print()
   print("Assistant: ", end="", flush=True)
   ass_reply = []
   for event in events:
       print(event, end="", flush=True)
       ass_reply.append(event)
   print()
   return ass_reply
 
 def main():
-  DGL_API_ENDPOINT = "https://www.diglife.eu/inference"
+  DGL_API_ENDPOINT = "https://www.diglife.eu/"
   if "DGL_API_ENDPOINT" in os.environ and os.environ["DGL_API_ENDPOINT"]:
     DGL_API_ENDPOINT = os.environ["DGL_API_ENDPOINT"]
 
   parser = argparse.ArgumentParser(description='DigLife API Client.')
   parser.add_argument('--logdir', type=str, default="logs/",
                       help='Where to store logs')
   parser.add_argument('--endpoint', type=str, default=DGL_API_ENDPOINT,
                       help='Endpoint for the inference')
+  parser.add_argument('--inference-url', type=str, default="/inference",
+                      help='Endpoint for the inference')                      
   parser.add_argument('-k','--access_key', type=str, required=True,
                       help='Access keys to authenticate to the API')                      
   parser.add_argument('-c','--chat-id', type=str,
                       help='Continue previous chat')
 
   subparsers = parser.add_subparsers(help='You can choose between different commands')
   chat_p = subparsers.add_parser('chat', help='chat with the assistants')
@@ -119,15 +122,22 @@
 
   chat_p.add_argument('message', type=str, 
                       help='say something to the model')
   chat_p.add_argument('-m','--model', type=str, required=True,
                       help='Which model do you want to talk to?')
   chat_p.add_argument('-i','--interactive', action='store_true',
                       help='Run interactive chat')
-  
+  chat_p.add_argument('--use-collection', type=str,
+                      help='Add collection information to the model context')
+
+  coll_p = subparsers.add_parser('coll', help='Document collections')
+  coll_p.add_argument('collection', type=str, 
+                      help='For now only models')
+  coll_p.set_defaults(func=main_ls)
+
   config_p = subparsers.add_parser('ls', help='List resources')
   config_p.add_argument('resource', type=str, 
                       help='For now only models')
   config_p.set_defaults(func=main_ls)
 
 
   try:
```

### Comparing `dgl_client-0.3.5/notebook.ipynb` & `dgl_client-0.4.1/notebook.ipynb`

 * *Files identical despite different names*

