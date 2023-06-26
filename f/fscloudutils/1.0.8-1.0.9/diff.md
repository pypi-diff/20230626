# Comparing `tmp/fscloudutils-1.0.8.tar.gz` & `tmp/fscloudutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fscloudutils-1.0.8.tar", last modified: Wed Mar  9 08:44:13 2022, max compression
+gzip compressed data, was "dist/fscloudutils-1.0.9.tar", last modified: Wed Mar 16 08:47:19 2022, max compression
```

## Comparing `fscloudutils-1.0.8.tar` & `fscloudutils-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/
--rw-rw-r--   0 yotam     (1000) yotam     (1000)     1047 2022-03-09 08:30:40.000000 fscloudutils-1.0.8/README.md
-drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils/
--rw-rw-r--   0 yotam     (1000) yotam     (1000)     5093 2022-01-17 10:45:56.000000 fscloudutils-1.0.8/fscloudutils/processors.py
--rw-rw-r--   0 yotam     (1000) yotam     (1000)     9521 2021-12-29 15:29:34.000000 fscloudutils-1.0.8/fscloudutils/data_validation.py
--rw-rw-r--   0 yotam     (1000) yotam     (1000)    13582 2022-01-17 10:30:38.000000 fscloudutils-1.0.8/fscloudutils/chatbot.py
--rw-rw-r--   0 yotam     (1000) yotam     (1000)     1190 2022-03-09 08:05:14.000000 fscloudutils-1.0.8/fscloudutils/DB_client.py
--rw-rw-r--   0 yotam     (1000) yotam     (1000)      361 2022-03-09 08:07:28.000000 fscloudutils-1.0.8/setup.py
--rw-rw-r--   0 yotam     (1000) yotam     (1000)      203 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/PKG-INFO
--rw-rw-r--   0 yotam     (1000) yotam     (1000)       38 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/setup.cfg
-drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/
--rw-rw-r--   0 yotam     (1000) yotam     (1000)      306 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/SOURCES.txt
--rw-rw-r--   0 yotam     (1000) yotam     (1000)       74 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/requires.txt
--rw-rw-r--   0 yotam     (1000) yotam     (1000)        1 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/dependency_links.txt
--rw-rw-r--   0 yotam     (1000) yotam     (1000)      203 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/PKG-INFO
--rw-rw-r--   0 yotam     (1000) yotam     (1000)       13 2022-03-09 08:44:13.000000 fscloudutils-1.0.8/fscloudutils.egg-info/top_level.txt
+drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     1799 2021-12-28 14:25:35.000000 fscloudutils-1.0.9/.gitignore
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     1061 2022-03-16 08:45:35.000000 fscloudutils-1.0.9/LICENSE.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)      214 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/PKG-INFO
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     1047 2022-03-09 08:30:40.000000 fscloudutils-1.0.9/README.md
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)      263 2022-03-16 08:43:05.000000 fscloudutils-1.0.9/__init__.py
+drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils/
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     1190 2022-03-09 08:05:14.000000 fscloudutils-1.0.9/fscloudutils/DB_client.py
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)    13582 2022-03-16 08:43:05.000000 fscloudutils-1.0.9/fscloudutils/chatbot.py
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     9521 2021-12-29 15:29:34.000000 fscloudutils-1.0.9/fscloudutils/data_validation.py
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     1061 2022-03-09 08:07:57.000000 fscloudutils-1.0.9/fscloudutils/license.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)     5093 2022-03-16 08:43:05.000000 fscloudutils-1.0.9/fscloudutils/processors.py
+drwxrwxr-x   0 yotam     (1000) yotam     (1000)        0 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)      214 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/PKG-INFO
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)      376 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)        1 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)       74 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/requires.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)       13 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/fscloudutils.egg-info/top_level.txt
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)       79 2022-03-16 08:47:19.000000 fscloudutils-1.0.9/setup.cfg
+-rw-rw-r--   0 yotam     (1000) yotam     (1000)      361 2022-03-16 08:47:17.000000 fscloudutils-1.0.9/setup.py
```

### Comparing `fscloudutils-1.0.8/README.md` & `fscloudutils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fscloudutils-1.0.8/fscloudutils/processors.py` & `fscloudutils-1.0.9/fscloudutils/processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import boto3
 import logging
 import warnings
 import os
-from fscloudutils.chatbot import SlackMessenger
-from fscloudutils.chatbot import EmailMessenger
+from fscloudutils.chatbot import SlackMessanger
+from fscloudutils.chatbot import EmailMessanger
 from fscloudutils.data_validation import InputValidator
 
 from botocore.exceptions import ClientError
 from botocore.client import Config
 
 
 class TaskProcessor:
```

### Comparing `fscloudutils-1.0.8/fscloudutils/data_validation.py` & `fscloudutils-1.0.9/fscloudutils/data_validation.py`

 * *Files identical despite different names*

### Comparing `fscloudutils-1.0.8/fscloudutils/chatbot.py` & `fscloudutils-1.0.9/fscloudutils/chatbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         except ClientError as e:
             print(e.response['Error']['Message'])
         else:
             print("Email sent! Message ID:"),
             print(response['MessageId'])
 
 
-class SlackMessenger:
+class SlackMessanger:
     def __init__(self, service_name: str, block_name: str, slack_token: str, slack_channel_private: str, slack_channel_public: str):
         self.service_name = service_name
         self.block_name = block_name
         self.parse_ssm_file()
         self.slack_token = slack_token
         if self.environment in ["INTGR", "STAGE"]:
             self.slack_channel = slack_channel_private
@@ -334,23 +334,23 @@
 
 
 def to_sns(message):
     pass
 
 
 def post_message_to_slack(plot_name, message, cw_link):
-    slack_m = SlackMessenger()
+    slack_m = SlackMessanger()
     slack_m.to_slack("hi")
 
     # to_sns(message)
 
 
 if __name__ == '__main__':
     settings.init()
-    slack_m = SlackMessenger("TEST1234")
+    slack_m = SlackMessanger("TEST1234")
 
     slack_m.to_slack("Error in STAGE_EXAMPLE123_DEEP\n"
                      "\n"
                      "TRACEBACK TRACEBACK TRACEBACK\n"
                      "\n"
                      "Link to cloudwatch"
                      )
```

### Comparing `fscloudutils-1.0.8/fscloudutils/DB_client.py` & `fscloudutils-1.0.9/fscloudutils/DB_client.py`

 * *Files identical despite different names*

