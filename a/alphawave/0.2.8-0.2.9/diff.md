# Comparing `tmp/alphawave-0.2.8.tar.gz` & `tmp/alphawave-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.8.tar", last modified: Sun Jun 25 03:56:26 2023, max compression
+gzip compressed data, was "alphawave-0.2.9.tar", last modified: Mon Jun 26 19:40:52 2023, max compression
```

## Comparing `alphawave-0.2.8.tar` & `alphawave-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.8/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-25 03:56:26.108699 alphawave-0.2.8/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.8/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-25 03:56:16.000000 alphawave-0.2.8/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-25 03:56:26.108699 alphawave-0.2.8/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9267 2023-06-20 23:20:58.000000 alphawave-0.2.8/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.8/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.8/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.8/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.8/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.8/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.8/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.8/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.8/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.8/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.8/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.8/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.8/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.8/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.8/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1758 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.8/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.8/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.8/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.8/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.8/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.8/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.2.8/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.8/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.8/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.2.8/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.8/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.8/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.8/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.8/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.2.8/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7080 2023-06-25 00:20:00.000000 alphawave-0.2.8/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.8/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.2.8/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.2.8/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    21511 2023-06-24 16:19:30.000000 alphawave-0.2.8/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.2.8/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.2.8/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12058 2023-06-25 03:39:18.000000 alphawave-0.2.8/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.2.8/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.8/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.8/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.8/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.9/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-26 19:40:52.623031 alphawave-0.2.9/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.9/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-26 19:40:43.000000 alphawave-0.2.9/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-26 19:40:52.623031 alphawave-0.2.9/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.619031 alphawave-0.2.9/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9267 2023-06-20 23:20:58.000000 alphawave-0.2.9/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.9/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.9/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-26 03:01:54.000000 alphawave-0.2.9/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.9/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.9/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.9/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.9/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.9/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.9/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.9/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.9/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.9/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.9/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.9/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-26 19:40:52.000000 alphawave-0.2.9/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1758 2023-06-26 19:40:52.000000 alphawave-0.2.9/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-26 19:40:52.000000 alphawave-0.2.9/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-26 19:40:52.000000 alphawave-0.2.9/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-26 19:40:52.000000 alphawave-0.2.9/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.9/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.9/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.9/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.9/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.9/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.9/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.2.9/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.9/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.9/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.2.9/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.9/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.9/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.9/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.9/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.2.9/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7572 2023-06-25 22:36:27.000000 alphawave-0.2.9/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.9/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.2.9/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.2.9/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    23163 2023-06-26 17:52:47.000000 alphawave-0.2.9/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.2.9/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.9/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.9/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.2.9/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12403 2023-06-26 16:54:42.000000 alphawave-0.2.9/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.2.9/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-26 19:40:52.623031 alphawave-0.2.9/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.9/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.9/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.9/tests/testSchema.py
```

### Comparing `alphawave-0.2.8/LICENSE` & `alphawave-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/PKG-INFO` & `alphawave-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.8
+Version: 0.2.9
 Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.8/README.md` & `alphawave-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/pyproject.toml` & `alphawave-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.8/src/alphawave/AlphaWave.py` & `alphawave-0.2.9/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/Colorize.py` & `alphawave-0.2.9/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.9/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.9/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/MemoryFork.py` & `alphawave-0.2.9/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/OSClient.py` & `alphawave-0.2.9/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/OpenAIClient.py` & `alphawave-0.2.9/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/RepairTestClient.py` & `alphawave-0.2.9/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/Response.py` & `alphawave-0.2.9/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/TestClient.py` & `alphawave-0.2.9/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/TestClientTest.py` & `alphawave-0.2.9/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.9/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/internalTypes.py` & `alphawave-0.2.9/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave/jsonParser.py` & `alphawave-0.2.9/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.9/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.8
+Version: 0.2.9
 Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.8/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.9/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/Agent.py` & `alphawave-0.2.9/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.9/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.9/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.9/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.9/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.9/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.9/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.9/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.9/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.9/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.9/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.9/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.9/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/FsInference.py` & `alphawave-0.2.9/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.2.9/src/alphawave_pyexts/LLMClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 host='192.168.1.195'
 port = 5004
 
 cv.register_conv_template(
     Conversation(
         name="falcon_instruct",
-        system="You are helpful, creative, clever, and very friendly.",
+        system="",
         roles=("User", "Assistant"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         stop_str=["User:"],
         stop_token_ids=[11],
         sep="\n",
@@ -41,23 +41,38 @@
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="",
     )
 )
 cv.register_conv_template(Conversation(
         name="wizardLM",
-        system="### Instruction",
+        system="""Below is an instruction that describes a task. Write a response that appropriately completes the request.
+### Instruction
+""",
         roles=("### Input", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="\n",
     )
 )
+cv.register_conv_template(Conversation(
+        name="wizardLM2",
+        system="""Below is an instruction that describes a task. Write a response that appropriately completes the request.
+### Instruction
+""",
+        roles=("User", "Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep="\n",
+        sep2="\n",
+    )
+)
 
 def get_available_models():
     return list(cv.conv_templates.keys())
 
 def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, tkroot = None, tkdisplay=None, format=True): 
     global USER_PREFIX, ASSISTANT_PREFIX, SYSTEM_PREFIX
 
@@ -68,37 +83,38 @@
     
     USER_PREFIX = conv.roles[0]
     ASSISTANT_PREFIX = conv.roles[1]
     SYSTEM_PREFIX = conv.system
     
     # set this so client can check for run-on, although this test should pbly be here!
     if format:
-        conv.system='' # no default prompt
+        prime=''
         for msg_idx, msg in enumerate(messages):
-            #if conv.first_msg_no_role and msg_idx ==0:
-            #    continue
             role = msg['role']
             ### conv.system is a prompt msg, and will be inserted as the first entry by conv.get_prompt()
             if role.lower() == 'system' and msg_idx==0:
-                if len(conv.roles)>2:
-                    conv.system=conv.roles[2]+msg['content']
+                if len(conv.system)>0:
+                    prime = msg['content']+' '+conv.system
                 else:
-                    conv.system = msg['content']
-                continue
-            if role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
+                    prime = msg['content']
+                if len(conv.roles)>2:
+                    conv.append_message(conv.roles[2], prime)
+                    prime=''
+            elif role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
                 role_index = 0
+                conv.append_message(conv.roles[role_index], msg['content'])
             else:
                 role_index = 1
-            conv.append_message(conv.roles[role_index], msg['content'])
-
-            #priming prompt
+                conv.append_message(conv.roles[role_index], msg['content'])
+            
+        #priming prompt
         conv.append_message(conv.roles[1], '')
         prompt = conv.get_prompt()
-        if conv.first_msg_no_role:
-            prompt = messages[0]['content']+conv.sep+prompt
+        if len(prime) > 0:
+            prompt = prime+conv.sep+prompt
     else:
         prompt = messages
     prompt = re.sub('\n{3,}', '\n\n', prompt)
     #print(f'***** llm output prompt string {prompt}')
     server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens, 'user_prompt':USER_PREFIX}
     smj = json.dumps(server_message)
     try:
```

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.2.9/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/chat.py` & `alphawave-0.2.9/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.2.9/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/conversation.py` & `alphawave-0.2.9/src/alphawave_pyexts/conversation.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     ADD_COLON_SPACE_SINGLE = auto()
     NO_COLON_SINGLE = auto()
     ADD_NEW_LINE_SINGLE = auto()
     DOLLY = auto()
     RWKV = auto()
     PHOENIX = auto()
     ROBIN = auto()
+    SINGLE = auto()
+
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that manages prompt templates and keeps all conversation history."""
 
     # The name of this template
@@ -42,91 +44,119 @@
     # Stop criteria (the default one is EOS token)
     stop_str: str = None
     # Stops generation if meeting any token in this list
     stop_token_ids: List[int] = None
     # prepends first msg text to front of prompt
     first_msg_no_role:bool = False
 
-    def get_prompt(self) -> str:
+    def get_prompt(self, include_system=False) -> str:
         """Get the prompt for generation."""
+        if self.sep_style == SeparatorStyle.SINGLE:
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
+            for role, message in self.messages:
+                if message:
+                    ret += role + ": " + "<s>" + message + "</s>\n"
+                else:
+                    ret += role + ": " + "<s>\n"
+            return ret
         if self.sep_style == SeparatorStyle.ADD_COLON_SINGLE:
-            ret = self.system + self.sep
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + message + self.sep
                 else:
                     ret += role + ":"
             return ret
         elif self.sep_style == SeparatorStyle.ADD_COLON_TWO:
             seps = [self.sep, self.sep2]
-            ret = self.system + seps[0]
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ": " + message + seps[i % 2]
                 else:
                     ret += role + ":"
             return ret
         elif self.sep_style == SeparatorStyle.ADD_COLON_SPACE_SINGLE:
-            ret = self.system + self.sep
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + message + self.sep
                 else:
                     ret += role + ": "  # must be end with a space
             return ret
         elif self.sep_style == SeparatorStyle.ADD_NEW_LINE_SINGLE:
-            ret = self.system + self.sep
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + "\n" + message + self.sep
                 else:
                     ret += role + "\n"
             return ret
         elif self.sep_style == SeparatorStyle.NO_COLON_SINGLE:
-            ret = self.system
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + message + self.sep
                 else:
                     ret += role
             return ret
         elif self.sep_style == SeparatorStyle.RWKV:
-            ret = self.system
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += (
                         role
                         + ": "
                         + message.replace("\r\n", "\n").replace("\n\n", "\n")
                     )
                     ret += "\n\n"
                 else:
                     ret += role + ":"
             return ret
         elif self.sep_style == SeparatorStyle.DOLLY:
             seps = [self.sep, self.sep2]
-            ret = self.system
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system
             for i, (role, message) in enumerate(self.messages):
                 if message:
                     ret += role + ":\n" + message + seps[i % 2]
                     if i % 2 == 1:
                         ret += "\n\n"
                 else:
                     ret += role + ":\n"
             return ret
         elif self.sep_style == SeparatorStyle.PHOENIX:
-            ret = self.system
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + "<s>" + message + "</s>"
                 else:
                     ret += role + ": " + "<s>"
             return ret
         elif self.sep_style == SeparatorStyle.ROBIN:
-            ret = self.system + self.sep
+            ret = ''
+            if len(self.system) > 0 and include_system:
+                ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + ":\n" + message + self.sep
                 else:
                     ret += role + ":\n"
             return ret
         else:
@@ -255,16 +285,15 @@
     )
 )
 
 # Vicuna v1.1 template
 register_conv_template(
     Conversation(
         name="vicuna_v1.1",
-        system="A chat between a curious user and an artificial intelligence assistant. "
-        "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+        system="",
         roles=("USER", "ASSISTANT"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep=" ",
         sep2="</s>",
     )
@@ -297,15 +326,29 @@
     )
 )
 
 # Dolly V2 default template
 register_conv_template(
     Conversation(
         name="dolly_v2",
-        system="Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
+        system="",
+        roles=("### Instruction", "### Response"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.DOLLY,
+        sep="\n\n",
+        sep2="### End",
+    )
+)
+
+# ChatGLM2 default template
+register_conv_template(
+    Conversation(
+        name="chatglm2",
+        system="",
         roles=("### Instruction", "### Response"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.DOLLY,
         sep="\n\n",
         sep2="### End",
     )
@@ -416,15 +459,15 @@
     )
 )
 
 # ChatGPT default template
 register_conv_template(
     Conversation(
         name="chatgpt",
-        system="You are a helpful assistant.",
+        system="",
         roles=("user", "assistant"),
         messages=(),
         offset=0,
         sep_style=None,
         sep=None,
     )
 )
@@ -456,14 +499,29 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
         sep="<|im_end|>",
         stop_token_ids=[50278, 0],
     )
 )
+# MPT instruct template as per HG MPT 30b instruct model page
+register_conv_template(
+    Conversation(
+        name="mpt_instruct",
+        system=""""Below is an instruction that describes a task. Write a response that appropriately completes the request.
+
+""",
+        roles=("### Instruction", "### Response",""),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
+        sep="\n",
+        stop_token_ids=[50278, 0],
+    )
+)
 
 # Bard default template
 # Reference: https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L150
 #            https://github.com/google/generative-ai-python/blob/9c99bcb474a991a97a2e7d62fcdb52db7ce40729/google/generativeai/discuss.py#L40
 register_conv_template(
     Conversation(
         name="bard",
```

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/handler.py` & `alphawave-0.2.9/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.2.9/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.2.9/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.2.9/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.2.9/src/alphawave_pyexts/serverUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,17 @@
     ### why do these have to be here? should be inherited from TextIteratorStreamer?
     self.text_queue = Queue()
     self.stop_signal = None
     self.timeout = None
 
   def put(self, value):
     """
-        Recives tokens, decodes them, and prints them to stdout as soon as they form entire words.
+        Receives tokens, decodes them, and prints them to stdout as soon as they form entire words.
     """
+
     if len(value.shape) > 1 and value.shape[0] > 1:
       raise ValueError("TextStreamer only supports batch size 1")
     elif len(value.shape) > 1:
       value = value[0]
 
     if self.skip_prompt and self.next_tokens_are_prompt:
       self.next_tokens_are_prompt = False
@@ -91,18 +92,19 @@
       self.print_len += len(printable_text)
       # Otherwise, prints until the last space char (simple heuristic to avoid printing incomplete words,
       # which may change with the subsequent token -- there are probably smarter ways to do this!)
     else:
       printable_text = text[self.print_len : text.rfind(" ") + 1]
       self.print_len += len(printable_text)
     self.on_finalized_text(printable_text)
-
     if self.stop_event.is_set():
-      print("\n***** MyStreamer stopping stream stop_event {stop_event.is_set()}")
-      raise SystemExit
+        self.on_finalized_text(" ", stream_end=True)
+        print(f"\n***** MyStreamer exit stop_event is {self.stop_event.is_set()}")
+        time.sleep(0.1)
+        raise SystemExit
 
   def end(self):
     """Flushes any remaining cache and prints a newline to stdout."""
     # Flush the cache, if it exists
     print('received end from generate')
     if len(self.token_cache) > 0:
       text = self.tokenizer.decode(self.token_cache, skip_special_tokens=True)
@@ -226,18 +228,22 @@
         if stop_str is not None and isinstance(stop_str, Iterable):
           for stop in stop_str:
             idx3 = max(idx3, test_text.find(stop))
         if stop_event.is_set(): # flush generate
           continue
         if idx1>= 0 or idx2>=0 or idx3 >= 0:
           stop_event.set()
-          idx = min(max(idx1, 0), max(idx2,0), max(idx3,0))
-          if idx > 0:
-            conn.send(bytearray((new_text[:idx]).encode('utf8')))
-            print(f'set stop event in submit {idx1}, {idx2}, {idx3}')
+          # get the earliest stop found
+          idx = 1000000
+          for candidate_idx in [idx1, idx2, idx3]:
+              if candidate_idx >= 0 and candidate_idx < idx:
+                  idx = candidate_idx
+          print(f'set stop event in submit {idx1}, {idx2}, {idx3}, stop on {idx}')
+          if idx < len(test_text) and idx > len(generated_text):  #see if there is anything to send
+            conn.send(bytearray((test_text[len(generated_text):idx]).encode('utf8')))
         else:
           generated_text = test_text
           conn.send(bytearray((new_text).encode('utf8')))  # send data to the client
       return generated_text
 
     
 def server(model=None, tokenizer=None, pipeline=None, stop_str=[]):
```

### Comparing `alphawave-0.2.8/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.2.9/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/tests/testOSClient.py` & `alphawave-0.2.9/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/tests/testOpenAiClient.py` & `alphawave-0.2.9/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.8/tests/testSchema.py` & `alphawave-0.2.9/tests/testSchema.py`

 * *Files identical despite different names*

