# Comparing `tmp/devchat-0.1.8.tar.gz` & `tmp/devchat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.8.tar", last modified: Mon May 22 14:40:52 2023, max compression
+gzip compressed data, was "devchat-0.1.9.tar", last modified: Sat May 27 15:17:23 2023, max compression
```

## Comparing `devchat-0.1.8.tar` & `devchat-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.733330 devchat-0.1.8/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.8/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-22 14:40:52.733133 devchat-0.1.8/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)     4718 2023-05-21 11:37:13.000000 devchat-0.1.8/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.729619 devchat-0.1.8/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.8/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6136 2023-05-22 13:34:59.000000 devchat-0.1.8/devchat/_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4794 2023-05-22 13:47:32.000000 devchat-0.1.8/devchat/assistant.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1682 2023-05-21 14:33:17.000000 devchat-0.1.8/devchat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      566 2023-05-22 04:56:01.000000 devchat-0.1.8/devchat/message.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.731572 devchat-0.1.8/devchat/openai/
--rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.8/devchat/openai/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3030 2023-05-22 14:29:50.000000 devchat-0.1.8/devchat/openai/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.8/devchat/openai/openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6031 2023-05-22 11:27:42.000000 devchat-0.1.8/devchat/openai/openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6604 2023-05-22 13:52:58.000000 devchat-0.1.8/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4299 2023-05-22 12:34:46.000000 devchat-0.1.8/devchat/store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5306 2023-05-22 09:23:48.000000 devchat-0.1.8/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.730661 devchat-0.1.8/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      130 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.8/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-22 14:40:52.733371 devchat-0.1.8/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)     1112 2023-05-22 06:04:12.000000 devchat-0.1.8/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.732741 devchat-0.1.8/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.8/tests/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-22 06:00:29.000000 devchat-0.1.8/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.8/tests/test_openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5887 2023-05-22 11:37:12.000000 devchat-0.1.8/tests/test_openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2221 2023-05-21 23:12:05.000000 devchat-0.1.8/tests/test_store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-27 15:17:23.126145 devchat-0.1.9/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.9/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5663 2023-05-27 15:17:23.125984 devchat-0.1.9/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5207 2023-05-27 11:05:16.000000 devchat-0.1.9/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-27 15:17:23.122390 devchat-0.1.9/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.9/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6242 2023-05-27 11:39:49.000000 devchat-0.1.9/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4813 2023-05-27 12:10:59.000000 devchat-0.1.9/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1682 2023-05-21 14:33:17.000000 devchat-0.1.9/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      566 2023-05-22 04:56:01.000000 devchat-0.1.9/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-27 15:17:23.124276 devchat-0.1.9/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.9/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3083 2023-05-27 12:37:25.000000 devchat-0.1.9/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.9/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6031 2023-05-22 11:27:42.000000 devchat-0.1.9/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6767 2023-05-27 12:09:06.000000 devchat-0.1.9/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4463 2023-05-27 12:07:58.000000 devchat-0.1.9/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5076 2023-05-27 11:36:22.000000 devchat-0.1.9/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-27 15:17:23.123509 devchat-0.1.9/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5663 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      130 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-27 15:17:23.000000 devchat-0.1.9/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.9/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-27 15:17:23.126185 devchat-0.1.9/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1112 2023-05-27 15:15:31.000000 devchat-0.1.9/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-27 15:17:23.125669 devchat-0.1.9/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.9/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-22 06:00:29.000000 devchat-0.1.9/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.9/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5887 2023-05-22 11:37:12.000000 devchat-0.1.9/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2221 2023-05-21 23:12:05.000000 devchat-0.1.9/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.9/tests/test_utils.py
```

### Comparing `devchat-0.1.8/LICENSE` & `devchat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/PKG-INFO` & `devchat-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.1.8
+Version: 0.1.9
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/covespace/devchat
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -27,62 +27,66 @@
 
 </div>
 <br>
 <div align="left">
 
 The DevChat core library and CLI.
 
-👉 For a better experience, check out our [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Install and enjoy the enhanced UI 👏
+👉 For an enhanced experience and UI, we welcome you to install [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Enjoy DevChat! 👏
 
 ***
 
 ## What is DevChat?
 
-DevChat is an open-source tool that helps you write prompts to generate code and documentation.
-It is _not_ limited to performing predefined operations on short code snippets.
-  
+DevChat is the open-source solution to help you write prompts to generate code and documentation, going beyond simple code auto-completion.
+It isn't limited to performing predefined operations on short code snippets.
+
 DevChat is the way developers interact and collaborate with AI.
 
 💬 Build the future with prompts, _not_ code.
 
 ## Why DevChat?
 
-- To enable AI to write code, DevChat assists you in providing **the right context** for AI.
-  
-  ![20230519-231038-00 00 00 000-00 00 20 989](https://github.com/covespace/devchat-vscode/assets/592493/cfb96c7f-bd45-4573-810e-17148aac79d1)
-  
+- Great output requires great input, to maximize the power of AI, DevChat assists you seamlessly to **provide the right context** to the AI.
+    
   Chat history, code, files, directory trees, `git diff --cached`, or the output of any command.
+  
+  ![20230523-220717-cut-merged-1684855581224](https://github.com/covespace/devchat-vscode/assets/592493/16bc09e4-4185-4bcb-8d5a-2173b0bfc3ed)
 
-- To apply AI-generated code, DevChat streamlines your **actions to take**.
+  ![20230523-220717-00 00 28 206-00 00 44 950](https://github.com/covespace/devchat-vscode/assets/592493/d5556310-bc7f-4abb-86a3-8e76e4aa720e)  
 
-  ![20230519-231038-00 00 24 989-00 00 44 688](https://github.com/covespace/devchat-vscode/assets/592493/2a0c4acf-6801-409c-bb18-ac75bae96938)
+- Once you have generated code with AI, DevChat **streamlines the actions** to properly integrate and ship.
   
   View diffs, copy or insert, commit & sync, or export to documentation, wikis, and more.
   
+  ![20230523-220717-00 00 46 728-00 01 00 120](https://github.com/covespace/devchat-vscode/assets/592493/a2bab011-8e31-47a9-838f-36e43cd2e98c)
+
+  ![20230523-220717-00 01 00 120-00 01 14 452](https://github.com/covespace/devchat-vscode/assets/592493/31e90fd5-e797-4726-b5b2-5c4dce1c7551)
+
 - To guide AI in your work, define **your own workflows** with DevChat.
   
-  ![20230519-231038-00 00 45 034-00 01 00 000](https://github.com/covespace/devchat-vscode/assets/592493/5a72e43f-0ed9-446a-81be-3e5f00009961)
-  
-  More prompt templates, iterative calls to AI, and program operations.
+  ![20230523-220717-00 01 14 614-00 01 41 680](https://github.com/covespace/devchat-vscode/assets/592493/94502efd-781b-448d-b945-dffcc41d7af3)
 
-- To suit your preferences, customize **your own experiences** with DevChat.
+  Explore more prompt templates, iterative calls to AI, and program operations.
+  
+- To ensure the experience fits your preferences, customize **your own experiences** with DevChat.
   
   Open-source, no waiting for opaque feature schedules. Access GPT-4 today and more models in the future.
   
-## What is Prompt-Centric Software Development (PSSD)?
+## What is Prompt-Centric Software Development (PCSD)?
 
 - The traditional code-centric paradigm is evolving.
 
-- Write prompts to create code. Transform prompts into everything.
+- Write prompts to create code. Transform prompts into all the artifacts in software engineering.
 
   <img width="600" alt="image" src="https://github.com/covespace/devchat/assets/592493/dd32e900-92fd-4fa4-8489-96ed17ab5e0e">
 
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
   
-- It is DevPromptOps
+- We like to call it DevPromptOps
   
   <img width="500" alt="image" src="https://github.com/covespace/devchat/assets/592493/e8e1215b-53b0-4473-ab00-0665d33f204a">
   
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
 
 ***
```

### Comparing `devchat-0.1.8/README.md` & `devchat-0.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,62 +15,66 @@
 
 </div>
 <br>
 <div align="left">
 
 The DevChat core library and CLI.
 
-👉 For a better experience, check out our [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Install and enjoy the enhanced UI 👏
+👉 For an enhanced experience and UI, we welcome you to install [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Enjoy DevChat! 👏
 
 ***
 
 ## What is DevChat?
 
-DevChat is an open-source tool that helps you write prompts to generate code and documentation.
-It is _not_ limited to performing predefined operations on short code snippets.
-  
+DevChat is the open-source solution to help you write prompts to generate code and documentation, going beyond simple code auto-completion.
+It isn't limited to performing predefined operations on short code snippets.
+
 DevChat is the way developers interact and collaborate with AI.
 
 💬 Build the future with prompts, _not_ code.
 
 ## Why DevChat?
 
-- To enable AI to write code, DevChat assists you in providing **the right context** for AI.
-  
-  ![20230519-231038-00 00 00 000-00 00 20 989](https://github.com/covespace/devchat-vscode/assets/592493/cfb96c7f-bd45-4573-810e-17148aac79d1)
-  
+- Great output requires great input, to maximize the power of AI, DevChat assists you seamlessly to **provide the right context** to the AI.
+    
   Chat history, code, files, directory trees, `git diff --cached`, or the output of any command.
+  
+  ![20230523-220717-cut-merged-1684855581224](https://github.com/covespace/devchat-vscode/assets/592493/16bc09e4-4185-4bcb-8d5a-2173b0bfc3ed)
 
-- To apply AI-generated code, DevChat streamlines your **actions to take**.
+  ![20230523-220717-00 00 28 206-00 00 44 950](https://github.com/covespace/devchat-vscode/assets/592493/d5556310-bc7f-4abb-86a3-8e76e4aa720e)  
 
-  ![20230519-231038-00 00 24 989-00 00 44 688](https://github.com/covespace/devchat-vscode/assets/592493/2a0c4acf-6801-409c-bb18-ac75bae96938)
+- Once you have generated code with AI, DevChat **streamlines the actions** to properly integrate and ship.
   
   View diffs, copy or insert, commit & sync, or export to documentation, wikis, and more.
   
+  ![20230523-220717-00 00 46 728-00 01 00 120](https://github.com/covespace/devchat-vscode/assets/592493/a2bab011-8e31-47a9-838f-36e43cd2e98c)
+
+  ![20230523-220717-00 01 00 120-00 01 14 452](https://github.com/covespace/devchat-vscode/assets/592493/31e90fd5-e797-4726-b5b2-5c4dce1c7551)
+
 - To guide AI in your work, define **your own workflows** with DevChat.
   
-  ![20230519-231038-00 00 45 034-00 01 00 000](https://github.com/covespace/devchat-vscode/assets/592493/5a72e43f-0ed9-446a-81be-3e5f00009961)
-  
-  More prompt templates, iterative calls to AI, and program operations.
+  ![20230523-220717-00 01 14 614-00 01 41 680](https://github.com/covespace/devchat-vscode/assets/592493/94502efd-781b-448d-b945-dffcc41d7af3)
 
-- To suit your preferences, customize **your own experiences** with DevChat.
+  Explore more prompt templates, iterative calls to AI, and program operations.
+  
+- To ensure the experience fits your preferences, customize **your own experiences** with DevChat.
   
   Open-source, no waiting for opaque feature schedules. Access GPT-4 today and more models in the future.
   
-## What is Prompt-Centric Software Development (PSSD)?
+## What is Prompt-Centric Software Development (PCSD)?
 
 - The traditional code-centric paradigm is evolving.
 
-- Write prompts to create code. Transform prompts into everything.
+- Write prompts to create code. Transform prompts into all the artifacts in software engineering.
 
   <img width="600" alt="image" src="https://github.com/covespace/devchat/assets/592493/dd32e900-92fd-4fa4-8489-96ed17ab5e0e">
 
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
   
-- It is DevPromptOps
+- We like to call it DevPromptOps
   
   <img width="500" alt="image" src="https://github.com/covespace/devchat/assets/592493/e8e1215b-53b0-4473-ab00-0665d33f204a">
   
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
 
 ***
```

### Comparing `devchat-0.1.8/devchat/_cli.py` & `devchat-0.1.9/devchat/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 This module contains the main function for the DevChat CLI.
 """
 from contextlib import contextmanager
 import json
+import logging
 import os
 import sys
 from typing import List, Optional, Tuple
 import rich_click as click
 from devchat.store import Store
 from devchat.openai import OpenAIChatConfig, OpenAIChat
 from devchat.assistant import Assistant
 from devchat.utils import find_git_root, git_ignore, parse_files, setup_logger
 
 
 click.rich_click.USE_MARKDOWN = True
 
-logger = setup_logger(__name__)
-
 
 @click.group()
 def main():
     """DevChat CLI: A command-line interface for the DevChat chatbot."""
 
 
 @contextmanager
 def handle_errors():
     """Handle errors in the CLI."""
     try:
         yield
     except Exception as error:
+        logger = logging.getLogger(__name__)
         logger.exception(error)
-        click.echo(f"Error: {error}")
+        click.echo(f"Error: {error}", err=True)
         sys.exit(os.EX_SOFTWARE)
 
 
 def init_dir() -> Tuple[dict, str]:
     git_root = find_git_root()
     chat_dir = os.path.join(git_root, ".chat")
     if not os.path.exists(chat_dir):
@@ -51,15 +51,16 @@
 
     try:
         with open(os.path.join(chat_dir, 'config.json'), 'r', encoding='utf-8') as file:
             config_data = json.load(file)
     except FileNotFoundError:
         config_data = default_config_data
 
-    git_ignore(git_root, chat_dir)
+    setup_logger(os.path.join(chat_dir, 'error.log'))
+    git_ignore(chat_dir, '*')
     return config_data, chat_dir
 
 
 @main.command()
 @click.argument('content', required=False)
 @click.option('-p', '--parent', help='Input the parent prompt hash to continue the conversation.')
 @click.option('-r', '--reference', multiple=True,
@@ -163,15 +164,15 @@
 
             assistant.make_prompt(content, instruct_contents, context_contents,
                                   parent, reference)
 
             for response in assistant.iterate_response():
                 click.echo(response, nl=False)
         else:
-            click.echo(f"Error: Invalid LLM in configuration '{provider}'")
+            click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
             sys.exit(os.EX_DATAERR)
 
 
 @main.command()
 @click.option('--skip', default=0, help='Skip number prompts before showing the prompt history.')
 @click.option('--max-count', default=100, help='Limit the number of commits to output.')
 def log(skip, max_count):
@@ -183,15 +184,15 @@
     recent_prompts = []
     if provider == 'OpenAI':
         openai_config = OpenAIChatConfig(model=config['model'], **config['OpenAI'])
         chat = OpenAIChat(openai_config)
         store = Store(chat_dir, chat)
         recent_prompts = store.select_recent(skip, skip + max_count)
     else:
-        click.echo(f"Error: Invalid LLM in configuration '{provider}'")
+        click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
         sys.exit(os.EX_DATAERR)
 
     logs = []
     for record in recent_prompts:
         try:
             logs.append(record.shortlog())
         except Exception:
```

### Comparing `devchat-0.1.8/devchat/assistant.py` & `devchat-0.1.9/devchat/assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import logging
 from typing import Optional, List, Iterator
-from devchat.utils import setup_logger
 from devchat.message import Message
 from devchat.chat import Chat
 from devchat.prompt import Prompt
 from devchat.store import Store
 
 
-logger = setup_logger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class Assistant:
     def __init__(self, chat: Chat, store: Store):
         """
         Initializes an Assistant object.
 
@@ -57,25 +57,25 @@
                 self._prompt.append_new(Message.CONTEXT, context_content)
                 self._check_limit()
 
         # Add history to the prompt
         for reference_hash in references:
             prompt = self._store.get_prompt(reference_hash)
             if not prompt:
-                logger.error("Reference prompt not found: %s", reference_hash)
+                logger.error("Reference %s not retrievable while making prompt.", reference_hash)
                 continue
             self._prompt.references.append(reference_hash)
             self._append_prompt(prompt)
         if parent:
             self._prompt.parent = parent
             parent_hash = parent
             while parent_hash:
                 parent_prompt = self._store.get_prompt(parent_hash)
                 if not parent_prompt:
-                    logger.error("Parent prompt not found: %s", parent_hash)
+                    logger.error("Parent %s not retrievable while making prompt.", parent_hash)
                     break
                 if not self._append_prompt(parent_prompt):
                     break
                 parent_hash = parent_prompt.parent
 
     def iterate_response(self) -> Iterator[str]:
         """Get an iterator of response strings from the chat API.
```

### Comparing `devchat-0.1.8/devchat/chat.py` & `devchat-0.1.9/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/devchat/message.py` & `devchat-0.1.9/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/devchat/openai/openai_chat.py` & `devchat-0.1.9/devchat/openai/openai_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     stream: Optional[bool] = Field(None)
     stop: Optional[Union[str, List[str]]] = Field(None)
     max_tokens: Optional[int] = Field(None, ge=1)
     presence_penalty: Optional[float] = Field(None, ge=-2.0, le=2.0)
     frequency_penalty: Optional[float] = Field(None, ge=-2.0, le=2.0)
     logit_bias: Optional[Dict[int, float]] = Field(None)
     user: Optional[str] = Field(None)
+    request_timeout: Optional[int] = Field(12, ge=3)
 
     class Config:
         """
         Configuration class to forbid extra fields in the model.
         """
         extra = Extra.forbid
```

### Comparing `devchat-0.1.8/devchat/openai/openai_message.py` & `devchat-0.1.9/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/devchat/openai/openai_prompt.py` & `devchat-0.1.9/devchat/openai/openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/devchat/prompt.py` & `devchat-0.1.9/devchat/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field, asdict
 import hashlib
+import logging
 import math
 from typing import Dict, List
 from devchat.message import Message
-from devchat.utils import unix_to_local_datetime, setup_logger
+from devchat.utils import unix_to_local_datetime
 
 
-logger = setup_logger(__name__)
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Prompt(ABC):
     """
     A class to represent a prompt and its corresponding responses from the chat API.
 
@@ -148,15 +149,16 @@
         """
         Calculate and set the hash of the prompt.
 
         Returns:
             str: The hash of the prompt. None if the prompt is incomplete.
         """
         if not self.request or not self.response:
-            logger.error("Prompt is incomplete for hash.")
+            logger.error("Incomplete prompt for hashing: request = %s, response = %s",
+                         self.request, self.response)
             return None
         data = asdict(self)
         assert data.pop('_hash') is None
         string = str(tuple(sorted(data.items())))
         self._hash = hashlib.sha256(string.encode('utf-8')).hexdigest()
         return self._hash
 
@@ -178,15 +180,16 @@
 
         Returns:
             str: The formatted response string. None if the response is incomplete.
         """
         formatted_str = self.formatted_header()
 
         if index >= len(self.response) or not self.response[index]:
-            logger.error("Response %d is incomplete for formatted response.", index)
+            logger.error("Response index %d is incomplete to format: request = %s, response = %s",
+                         index, self.request, self.response)
             return None
 
         formatted_str += self.response[index].content.strip() + "\n\n"
         formatted_str += f"prompt {self.hash}"
 
         return formatted_str
```

### Comparing `devchat-0.1.8/devchat/store.py` & `devchat-0.1.9/devchat/store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import asdict
+import logging
 import os
 from typing import List
 from xml.etree.ElementTree import ParseError
 import networkx as nx
 from tinydb import TinyDB, where
 from devchat.chat import Chat
 from devchat.prompt import Prompt
-from devchat.utils import setup_logger
 
 
-logger = setup_logger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class Store:
     def __init__(self, store_dir: str, chat: Chat):
         """
         Initializes a Store instance.
 
@@ -67,41 +67,43 @@
 
         # Add the prompt to the graph
         self._graph.add_node(prompt.hash, timestamp=prompt.timestamp)
 
         # Add edges for parents and references
         if prompt.parent:
             if prompt.parent not in self._graph:
-                logger.warning("Parent %s not found in the store.", prompt.parent)
+                logger.warning("Parent %s not found while Prompt %s is stored to graph store.",
+                               prompt.parent, prompt.hash)
             else:
                 self._graph.add_edge(prompt.hash, prompt.parent)
         for reference_hash in prompt.references:
             if reference_hash not in self._graph:
-                logger.warning("Reference %s not found in the store.", reference_hash)
+                logger.warning("Reference %s not found while Prompt %s is stored to graph store.",
+                               reference_hash, prompt.hash)
             else:
                 self._graph.add_edge(prompt.hash, reference_hash)
         nx.write_graphml(self._graph, self._graph_path)
 
     def get_prompt(self, prompt_hash: str) -> Prompt:
         """
         Retrieve a prompt from the store.
 
         Args:
             prompt_hash (str): The hash of the prompt to retrieve.
         Returns:
             Prompt: The retrieved prompt. None if the prompt is not found.
         """
         if prompt_hash not in self._graph:
-            logger.warning("Prompt %s not found in the graph store.", prompt_hash)
+            logger.warning("Prompt %s not found while retrieving from graph store.", prompt_hash)
             return None
 
         # Retrieve the prompt object from TinyDB
         prompt_data = self._db.search(where('_hash') == prompt_hash)
         if not prompt_data:
-            logger.warning("Prompt %s not found in the object store.", prompt_hash)
+            logger.warning("Prompt %s not found while retrieving from object store.", prompt_hash)
             return None
         assert len(prompt_data) == 1
         return self._chat.load_prompt(prompt_data[0])
 
     def select_recent(self, start: int, end: int) -> List[Prompt]:
         """
         Select recent prompts.
@@ -119,11 +121,11 @@
                               reverse=True)
         if end > len(sorted_nodes):
             end = len(sorted_nodes)
         prompts = []
         for node in sorted_nodes[start:end]:
             prompt = self.get_prompt(node[0])
             if not prompt:
-                logger.error("Selected prompt %s not found in the store.", node[0])
+                logger.error("Prompt %s not found while selecting from the store.", node[0])
                 continue
             prompts.append(prompt)
         return prompts
```

### Comparing `devchat-0.1.8/devchat/utils.py` & `devchat-0.1.9/devchat/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,65 @@
 """
 utils.py - Utility functions for DevChat.
 """
 import logging
 import os
 import re
-import sys
 import getpass
 import socket
 import subprocess
 from typing import List, Tuple
 import datetime
 import pytz
 from dateutil import tz
 import tiktoken
 
 
-def setup_logger(name, level=logging.WARNING):
-    """Utility function to set up a logger with the specified name and level."""
+def setup_logger(file_path, level=logging.WARNING):
+    """Utility function to set up a logger with the specified file path and level."""
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
     # Create a file handler for logging
-    console_handler = logging.StreamHandler(sys.stderr)
-    console_handler.setFormatter(formatter)
+    file_handler = logging.FileHandler(file_path)
+    file_handler.setFormatter(formatter)
 
-    # Create a logger with the given name
-    logger = logging.getLogger(name)
-    logger.setLevel(level)
-    logger.addHandler(console_handler)
-
-    return logger
+    # Set up the global logger
+    logging.basicConfig(level=level, handlers=[file_handler])
 
 
 def find_git_root():
     try:
         root = subprocess.check_output(["git", "rev-parse", "--show-toplevel"])
         return root.decode("utf-8").strip()
     except subprocess.CalledProcessError as error:
         raise RuntimeError("Not inside a Git repository") from error
 
 
-def git_ignore(git_root_dir, *ignore_entries):
-    gitignore_path = os.path.join(git_root_dir, '.gitignore')
+def git_ignore(target_dir: str, *ignore_entries: str) -> None:
+    gitignore_path = os.path.join(target_dir, '.gitignore')
 
     if os.path.exists(gitignore_path):
         with open(gitignore_path, 'r', encoding='utf-8') as gitignore_file:
             gitignore_content = gitignore_file.read()
 
         new_entries = []
         for entry in ignore_entries:
-            relative_entry = os.path.relpath(entry, git_root_dir)
-            if relative_entry not in gitignore_content:
-                new_entries.append(relative_entry)
+            if entry not in gitignore_content:
+                new_entries.append(entry)
 
         if new_entries:
             with open(gitignore_path, 'a', encoding='utf-8') as gitignore_file:
-                gitignore_file.write('\n# DevChat\n')
+                gitignore_file.write('\n# devchat\n')
                 for entry in new_entries:
                     gitignore_file.write(f'{entry}\n')
     else:
         with open(gitignore_path, 'w', encoding='utf-8') as gitignore_file:
-            gitignore_file.write('# DevChat\n')
+            gitignore_file.write('# devchat\n')
             for entry in ignore_entries:
-                relative_entry = os.path.relpath(entry, git_root_dir)
-                gitignore_file.write(f'{relative_entry}\n')
+                gitignore_file.write(f'{entry}\n')
 
 
 def unix_to_local_datetime(unix_time) -> datetime.datetime:
     # Get the local time zone
     local_tz = tz.tzlocal()
 
     # Convert the Unix time to a naive datetime object
```

### Comparing `devchat-0.1.8/devchat.egg-info/PKG-INFO` & `devchat-0.1.9/devchat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.1.8
+Version: 0.1.9
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/covespace/devchat
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -27,62 +27,66 @@
 
 </div>
 <br>
 <div align="left">
 
 The DevChat core library and CLI.
 
-👉 For a better experience, check out our [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Install and enjoy the enhanced UI 👏
+👉 For an enhanced experience and UI, we welcome you to install [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Enjoy DevChat! 👏
 
 ***
 
 ## What is DevChat?
 
-DevChat is an open-source tool that helps you write prompts to generate code and documentation.
-It is _not_ limited to performing predefined operations on short code snippets.
-  
+DevChat is the open-source solution to help you write prompts to generate code and documentation, going beyond simple code auto-completion.
+It isn't limited to performing predefined operations on short code snippets.
+
 DevChat is the way developers interact and collaborate with AI.
 
 💬 Build the future with prompts, _not_ code.
 
 ## Why DevChat?
 
-- To enable AI to write code, DevChat assists you in providing **the right context** for AI.
-  
-  ![20230519-231038-00 00 00 000-00 00 20 989](https://github.com/covespace/devchat-vscode/assets/592493/cfb96c7f-bd45-4573-810e-17148aac79d1)
-  
+- Great output requires great input, to maximize the power of AI, DevChat assists you seamlessly to **provide the right context** to the AI.
+    
   Chat history, code, files, directory trees, `git diff --cached`, or the output of any command.
+  
+  ![20230523-220717-cut-merged-1684855581224](https://github.com/covespace/devchat-vscode/assets/592493/16bc09e4-4185-4bcb-8d5a-2173b0bfc3ed)
 
-- To apply AI-generated code, DevChat streamlines your **actions to take**.
+  ![20230523-220717-00 00 28 206-00 00 44 950](https://github.com/covespace/devchat-vscode/assets/592493/d5556310-bc7f-4abb-86a3-8e76e4aa720e)  
 
-  ![20230519-231038-00 00 24 989-00 00 44 688](https://github.com/covespace/devchat-vscode/assets/592493/2a0c4acf-6801-409c-bb18-ac75bae96938)
+- Once you have generated code with AI, DevChat **streamlines the actions** to properly integrate and ship.
   
   View diffs, copy or insert, commit & sync, or export to documentation, wikis, and more.
   
+  ![20230523-220717-00 00 46 728-00 01 00 120](https://github.com/covespace/devchat-vscode/assets/592493/a2bab011-8e31-47a9-838f-36e43cd2e98c)
+
+  ![20230523-220717-00 01 00 120-00 01 14 452](https://github.com/covespace/devchat-vscode/assets/592493/31e90fd5-e797-4726-b5b2-5c4dce1c7551)
+
 - To guide AI in your work, define **your own workflows** with DevChat.
   
-  ![20230519-231038-00 00 45 034-00 01 00 000](https://github.com/covespace/devchat-vscode/assets/592493/5a72e43f-0ed9-446a-81be-3e5f00009961)
-  
-  More prompt templates, iterative calls to AI, and program operations.
+  ![20230523-220717-00 01 14 614-00 01 41 680](https://github.com/covespace/devchat-vscode/assets/592493/94502efd-781b-448d-b945-dffcc41d7af3)
 
-- To suit your preferences, customize **your own experiences** with DevChat.
+  Explore more prompt templates, iterative calls to AI, and program operations.
+  
+- To ensure the experience fits your preferences, customize **your own experiences** with DevChat.
   
   Open-source, no waiting for opaque feature schedules. Access GPT-4 today and more models in the future.
   
-## What is Prompt-Centric Software Development (PSSD)?
+## What is Prompt-Centric Software Development (PCSD)?
 
 - The traditional code-centric paradigm is evolving.
 
-- Write prompts to create code. Transform prompts into everything.
+- Write prompts to create code. Transform prompts into all the artifacts in software engineering.
 
   <img width="600" alt="image" src="https://github.com/covespace/devchat/assets/592493/dd32e900-92fd-4fa4-8489-96ed17ab5e0e">
 
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
   
-- It is DevPromptOps
+- We like to call it DevPromptOps
   
   <img width="500" alt="image" src="https://github.com/covespace/devchat/assets/592493/e8e1215b-53b0-4473-ab00-0665d33f204a">
   
   <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
 
 ***
```

### Comparing `devchat-0.1.8/devchat.egg-info/SOURCES.txt` & `devchat-0.1.9/devchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/setup.py` & `devchat-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # Read the contents of the README.md file
 long_description = read_file("README.md")
 
 setup(
     name="devchat",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "devchat = devchat._cli:main",
         ],
     },
```

### Comparing `devchat-0.1.8/tests/test_cli.py` & `devchat-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/tests/test_openai_message.py` & `devchat-0.1.9/tests/test_openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/tests/test_openai_prompt.py` & `devchat-0.1.9/tests/test_openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/tests/test_store.py` & `devchat-0.1.9/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.8/tests/test_utils.py` & `devchat-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

