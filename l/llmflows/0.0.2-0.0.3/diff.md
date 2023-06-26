# Comparing `tmp/llmflows-0.0.2.tar.gz` & `tmp/llmflows-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflows-0.0.2.tar", last modified: Sun Jun  4 17:54:47 2023, max compression
+gzip compressed data, was "llmflows-0.0.3.tar", last modified: Mon Jun 26 01:39:29 2023, max compression
```

## Comparing `llmflows-0.0.2.tar` & `llmflows-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 17:54:37.000000 llmflows-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-04 17:54:47.023666 llmflows-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-04 17:54:37.000000 llmflows-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.015667 llmflows-0.0.2/llmflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.019667 llmflows-0.0.2/llmflows/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chaining_chat_llms_4_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chaining_llms_4_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chat_llm_2_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/chat_prompt_templates_3_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/complex_async_flows_6_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/complex_flows_6_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/creating_flows_5_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/getting_started_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/getting_started_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/llm_2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/prompt_templates_3_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/examples/question_answering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/flows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/async_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/async_flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/flowstep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/threaded_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/flows/threaded_flowstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/llms/openai_embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/prompts/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.023666 llmflows-0.0.2/llmflows/vectorstores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-04 17:54:37.000000 llmflows-0.0.2/llmflows/vectorstores/vector_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:54:47.015667 llmflows-0.0.2/llmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 17:54:47.000000 llmflows-0.0.2/llmflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-04 17:54:37.000000 llmflows-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 17:54:47.023666 llmflows-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.484185 llmflows-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 01:39:13.000000 llmflows-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-26 01:39:29.484185 llmflows-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-26 01:39:13.000000 llmflows-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.476185 llmflows-0.0.3/llmflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/callbacks/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/async_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/async_flowstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/flows/flowstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/llms/openai_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/prompts/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.480185 llmflows-0.0.3/llmflows/vectorstores/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-26 01:39:13.000000 llmflows-0.0.3/llmflows/vectorstores/vector_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:39:29.476185 llmflows-0.0.3/llmflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 01:39:29.000000 llmflows-0.0.3/llmflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 01:39:13.000000 llmflows-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:39:29.484185 llmflows-0.0.3/setup.cfg
```

### Comparing `llmflows-0.0.2/LICENSE` & `llmflows-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmflows-0.0.2/PKG-INFO` & `llmflows-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.2
-Summary: A simple and lightweight library for creating LLM-powered applications.
+Version: 0.0.3
+Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
-Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflow
-Project-URL: github, https://github.com/stoyan-stoyanov/llmflow
+Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
+Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# LLMFlows - Simple, Explicit and Transparent LLM Apps
+
 <p align="center">
-  <img src="docs/logo.png" />
+  <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
+![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
+![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
+![PyPi](https://img.shields.io/pypi/v/llmflows)
+![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
+![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
+
+## About
+LLMFlows is a simple and lightweight framework for building LLM-powered applications.
 
 ## Installation
+You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## What is LLMFlowss?
-A simple and lightweitght library for creating LLM-powered applications.
-
 ## Philosophy
 
 ### Simple
-We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We allow users to easily create complex LLM flows but we don't 
+We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
 
 ### Transparent
-We don't have classes with hidden prompts - prompts are for you to decide.
+Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
 
-## Example
-Here is a basic example for creating an LLM with PromptTemplate:
+## Documentation
+The full documentation for LLMFlows can be found here.
+
+## Usage
+Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
    prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
-print(llm_prompt)
-
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
-print(song_title)
 
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
 from llmflows.flows.flow import Flow
 from llmflows.flows.flowstep import FlowStep
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
@@ -120,48 +128,41 @@
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
 In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
-
-## Usage patterns 
-1. Use LLMs-only
-
-    Use the LLM and Agents classes and tools to build free-roaming agents   
-
-2. Create Flows
-
-    Use the LLM and Agents classes and tools to build free-roaming agents
-
-3. Build web apps
-
-    Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
+For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
 
 ## FAQ
 
-### How is this different than langchian?
-Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+### How is this different than langchain?
+Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
-### You only have OpenAI wrappers but I want to use ACMELLM
+### You only have OpenAI wrappers but I want to use AcmeLLM?
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
 
-### Why can't I find any info related to document loaders
-For the time being we have decided not to implement document loaders for two reasons:
-1. There are plenty of super capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM flow and prompt management libraries since usually document loading happens in separate pipelines and is not part of the LLM-powered app.
+### Why can't I find any info related to document loaders?
+For the time being we have decided not to implement document loaders for few reasons:
+1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
+2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
+3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
 
 While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
 
 ### What about agents?
 We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
 
+## License
+LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
 
 ## Contributing
+Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
 
 ## Links
+Twitter
 
+Documentation
```

### Comparing `llmflows-0.0.2/README.md` & `llmflows-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,64 @@
+# LLMFlows - Simple, Explicit and Transparent LLM Apps
+
 <p align="center">
-  <img src="docs/logo.png" />
+  <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
+![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
+![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
+![PyPi](https://img.shields.io/pypi/v/llmflows)
+![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
+![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
+
+## About
+LLMFlows is a simple and lightweight framework for building LLM-powered applications.
 
 ## Installation
+You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## What is LLMFlowss?
-A simple and lightweitght library for creating LLM-powered applications.
-
 ## Philosophy
 
 ### Simple
-We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We allow users to easily create complex LLM flows but we don't 
+We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
 
 ### Transparent
-We don't have classes with hidden prompts - prompts are for you to decide.
+Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
 
-## Example
-Here is a basic example for creating an LLM with PromptTemplate:
+## Documentation
+The full documentation for LLMFlows can be found here.
+
+## Usage
+Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
    prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
-print(llm_prompt)
-
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
-print(song_title)
 
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
 from llmflows.flows.flow import Flow
 from llmflows.flows.flowstep import FlowStep
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
@@ -106,48 +114,41 @@
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
 In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
-
-## Usage patterns 
-1. Use LLMs-only
-
-    Use the LLM and Agents classes and tools to build free-roaming agents   
-
-2. Create Flows
-
-    Use the LLM and Agents classes and tools to build free-roaming agents
-
-3. Build web apps
-
-    Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
+For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
 
 ## FAQ
 
-### How is this different than langchian?
-Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+### How is this different than langchain?
+Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
-### You only have OpenAI wrappers but I want to use ACMELLM
+### You only have OpenAI wrappers but I want to use AcmeLLM?
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
 
-### Why can't I find any info related to document loaders
-For the time being we have decided not to implement document loaders for two reasons:
-1. There are plenty of super capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM flow and prompt management libraries since usually document loading happens in separate pipelines and is not part of the LLM-powered app.
+### Why can't I find any info related to document loaders?
+For the time being we have decided not to implement document loaders for few reasons:
+1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
+2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
+3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
 
 While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
 
 ### What about agents?
 We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
 
+## License
+LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
 
 ## Contributing
+Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
 
 ## Links
+Twitter
 
+Documentation
```

### Comparing `llmflows-0.0.2/llmflows/flows/async_flow.py` & `llmflows-0.0.3/llmflows/flows/async_flow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,191 @@
 # pylint: disable=R0801
 
 """
-Async implementations of flow classes defined in another module.
+Async implementations of the flow classes defined in flow.py.
 """
 
 import asyncio
 from llmflows.flows.async_flowstep import AsyncFlowStep
 
 
 class AsyncBaseFlow:
-    """Base class for all async flows."""
+    """
+    Base class for all async flows. Each flow is a sequence of steps, represented by 
+    FlowStep instances.
+
+    Attributes:
+        first_step (AsyncFlowStep): The initial step of the flow.
+        steps (list): All steps in the flow.
+        output_keys (set): Set of output keys for all steps in the flow.
+        input_keys (set): Set of input keys for all steps in the flow.
+        names (set): Set of names of all steps in the flow.
+    """
 
-    def __init__(self, first_step: AsyncFlowStep):
+    def __init__(self, first_step: AsyncFlowStep = None):
         """
         Initializes the AsyncBaseFlow.
 
         Args:
             first_step (AsyncFlowStep): The first step of the flow.
         """
         self.first_step = first_step
+        self.steps = self._get_all_steps()
+        self.output_keys = set()
+        self.input_keys = set()
+        self.names = set()
+        self._check_unique_attributes()
 
     def set_first_step(self, step: AsyncFlowStep):
         """
         Sets the initial step of the flow.
 
         Args:
             step (AsyncFlowStep): The initial step for the flow.
         """
         self.first_step = step
 
-    async def execute(self, **inputs: str):
+    def _get_all_steps(self):
         """
-        Placeholder for flow execution method. To be overridden in subclasses.
+        Traverses the flow to get all steps.
 
-        Args:
-            **inputs (str): Inputs to the flow.
+        Returns:
+            list: A list containing all steps in the flow.
+        """
+        queue = [self.first_step]
+        visited_steps = set()
+        all_steps = []
+
+        while queue:
+            current_step = queue.pop(0)
+
+            if current_step in visited_steps or current_step is None:
+                continue
+
+            visited_steps.add(current_step)
+            all_steps.append(current_step)
+            queue.extend(current_step.next_steps)
+
+        return all_steps
+
+    def _check_unique_attributes(self):
+        """
+        Checks that all flow steps have unique output keys and names.
 
         Raises:
-            NotImplementedError: If not implemented in subclass.
+            ValueError: If any flow steps have the same output key or name.
         """
-        raise NotImplementedError
+        for step in self.steps:
+            if step.output_key in self.output_keys:
+                raise ValueError(
+                    f"The output key '{step.output_key}' has already been used"
+                    " in another FlowStep."
+                )
 
+            if step.name in self.names:
+                raise ValueError(
+                    f"The name '{step.name}' has already been used"
+                    " for another FlowStep."
+                )
 
-class AsyncFlow(AsyncBaseFlow):
-    """Asynchronous version of a DAG consisting of AsyncFlowSteps."""
+            self.output_keys.add(step.output_key)
+            self.names.add(step.name)
 
-    def __init__(self, first_step: AsyncFlowStep):
+            flowstep_class = step.__class__.__name__
+            if flowstep_class == "AsyncFlowStep":
+                self.input_keys.update(step.prompt_template.variables)
+            elif flowstep_class == "AsyncChatFlowStep":
+                self.input_keys.update(
+                    step.system_prompt_template.variables,
+                    step.message_prompt_template.variables,
+                    {step.message_key},
+                )
+
+    def _check_all_input_keys_available(self, user_inputs):
         """
-        Initializes the AsyncFlow.
+        Checks that all required input keys are available.
 
         Args:
-            first_step (AsyncFlowStep): The first step of the flow.
+            user_inputs (dict): The set of input keys provided by the user.
+
+        Raises:
+            ValueError: If not all required input keys are covered.
         """
-        super().__init__(first_step)
-        self.results = []
-        self._results_lock = asyncio.Lock()
-        self.executed_steps = set()
-        self._check_unique_output_keys()
+        if not self.input_keys.issubset(self.output_keys.union(user_inputs.keys())):
+            raise ValueError("Some flowsteps have missing inputs")
 
-    def _check_unique_output_keys(self):
+    async def execute(self, **inputs: str):
         """
-        Ensures unique output keys among steps.
+        Placeholder for flow execution method. To be overridden in subclasses.
+
+        Args:
+            **inputs (str): Inputs to the flow.
 
         Raises:
-            ValueError: If duplicate output keys exist.
+            NotImplementedError: If not implemented in subclass.
         """
-        queue = [self.first_step]
-        visited_steps = set()
-        used_output_keys = set()
-
-        while queue:
-            current_step = queue.pop(0)
+        raise NotImplementedError
 
-            if current_step in visited_steps or current_step is None:
-                continue
 
-            if current_step.output_key in used_output_keys:
-                raise ValueError(
-                    f"The output key '{current_step.output_key}' has already been used"
-                    " in another FlowStep."
-                )
+class AsyncFlow(AsyncBaseFlow):
+    """
+    Async implementation of BaseFlow that executes a series of FlowSteps in a Directed
+    Acyclic Graph (DAG) structure.
+
+    Attributes:
+        first_step (AsyncFlowStep): The first step in the flow.
+        results (dict): Stores the results of the executed flow steps.
+        executed_steps (set): Keeps track of the steps that have been executed.
+    """
 
-            used_output_keys.add(current_step.output_key)
-            visited_steps.add(current_step)
-            queue.extend(current_step.next_steps)
+    def __init__(self, first_step: AsyncFlowStep):
+        super().__init__(first_step)
+        self.results = {}
+        self.executed_steps = set()
 
-    async def execute(self, verbose: bool = False, **inputs: str):
+    async def execute(self, verbose=False, **inputs):
         """
-        Executes the flow.
+        Executes the flow with the provided inputs.
 
         Args:
-            verbose (bool): If true, flowstep outputs are printed.
-            **inputs (str): Inputs to the flow.
+            verbose (bool): Specifies if the flow step should print their output.
+            **inputs (dict): The inputs to the flow.
+
+        Returns:
+            dict: A dictionary of the results from each flow step.
+
+        Raises:
+            ValueError: If any required inputs are missing.
         """
+        self._check_all_input_keys_available(inputs)
         await self._execute_step(self.first_step, inputs, verbose)
         return self.results
 
-    async def _execute_step(self, step: AsyncFlowStep, inputs: dict, verbose: bool):
+    async def _execute_step(self, step, inputs, verbose):
         """
-        Concurrently executes a step and all subsequent steps.
+        Executes the given step and its next steps in a DFS-like manner.
 
         Args:
             step (AsyncFlowStep): The step to execute.
-            inputs (dict): Inputs to the step.
-            verbose (bool): If true, step outputs are printed.
+            inputs (dict): The inputs to the step.
+            verbose (bool): Specifies if the flow step should print its output.
+
+        Returns:
+            Any: The output of the step.
         """
         if not step or any(parent.output_key not in inputs for parent in step.parents):
             return
 
-        required_inputs = {key: inputs[key] for key in step.prompt_template.variables}
+        required_inputs = {
+            key: inputs[key] for key in step.required_keys
+        }
 
         if step not in self.executed_steps:
-            new_inputs = await step.execute(required_inputs, verbose)
+            flow_data = await step.execute(required_inputs, verbose)
             self.executed_steps.add(step)
 
-            if new_inputs:
-                async with self._results_lock:
-                    self.results.append({
-                        'step': step.name,
-                        'output_key': step.output_key,
-                        'output_value': new_inputs[step.output_key]
-                    })
-                inputs.update(new_inputs)
-
-        if step.next_steps:
-            await asyncio.gather(
-                *[self._execute_step(next_step, inputs, verbose)
-                  for next_step in step.next_steps]
-            )
+            if flow_data:
+                self.results[step.name] = flow_data
+                inputs.update(flow_data["result"])
+
+        tasks = [self._execute_step(next_step, inputs, verbose) for next_step in step.next_steps]
+        await asyncio.gather(*tasks)
```

### Comparing `llmflows-0.0.2/llmflows/prompts/prompt_template.py` & `llmflows-0.0.3/llmflows/prompts/prompt_template.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,36 +14,35 @@
 
     Args:
         prompt (str): The prompt string with variables.
 
     Attributes:
         prompt (str): The prompt string with variables.
         variables (List[str]): A list of variable names in the prompt string.
-
-    Methods:
-        get_prompt(**kwargs: str) -> str:
-            Returns the prompt string with variables replaced by the provided values.
     """
 
     def __init__(self, prompt: str):
         self.prompt = prompt
-        self.variables = [
+        self.variables = {
             fn for _, fn, _, _ in Formatter().parse(self.prompt) if fn is not None
-        ]
+        }
 
     def get_prompt(self, **kwargs: str) -> str:
         """
         Returns the prompt string with variables replaced by the provided values.
 
         Args:
             **kwargs: A dictionary of variable names and their values.
 
         Returns:
             The prompt string with variables replaced by the provided values.
+
+        Raises:
+            ValueError: If the provided variables do not match the defined ones.
         """
         if not self.variables:
             return self.prompt
 
-        assert set(kwargs.keys()) == set(
-            self.variables
-        ), "The provided variables do not match the defined ones."
+        if set(kwargs.keys()) != self.variables:
+            raise ValueError("The provided variables do not match the defined ones.")
+
         return self.prompt.format(**kwargs)
```

### Comparing `llmflows-0.0.2/llmflows/vectorstores/pinecone.py` & `llmflows-0.0.3/llmflows/vectorstores/pinecone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-"""Module to interact with Pinecone, a vector database service.
+"""
+Module to interact with Pinecone, a vector database service.
 
 This module contains a class `Pinecone` which provides several methods to
 interact with the Pinecone vector database service.
 """
 
 import pinecone # pylint: disable=import-error
 from llmflows.vectorstores.vector_doc import VectorDoc
 
 
 class Pinecone:
-    """Interact with Pinecone, a vector database service.
+    """
+    Interact with Pinecone, a vector database service.
 
     This class has methods to initialize the Pinecone client, describe the index,
     search the index for similar vectors, and insert or update vectors in the index.
 
     Args:
         index_name (str): The name of the index to use.
         api_key (str): The API key to use for authentication.
         environment (str): The environment to use, e.g. "production" or "development".
-
-    Attributes:
-        index (pinecone.Index): Pinecone index for querying and upserting vectors.
     """
 
     def __init__(self, index_name: str, api_key: str, environment: str):
-        """Initialize Pinecone client."""
         self.index_name = index_name
         self.api_key = api_key
         self.environment = environment
         self._init_client()
 
     def _init_client(self):
-        """Initialize the Pinecone client and describe the index."""
         pinecone.init(api_key=self.api_key, environment=self.environment)
         self.index = pinecone.Index(self.index_name)
         self.describe()
 
     def describe(self):
-        """Print information about the current index."""
+        """Describe the index."""
         print(self.index.describe_index_stats())
 
-    def search(self, query: VectorDoc, top_k: int):
-        """Search the index for similar vectors.
+    def search(self, query: VectorDoc, top_k: int) -> list[dict]:
+        """
+        Search the index for similar vectors.
 
         Args:
             query (VectorDoc): The query vector to search for.
             top_k (int): The number of results to return.
 
         Returns:
             list[dict]: A list of dictionaries representing the search results.
```

### Comparing `llmflows-0.0.2/llmflows/vectorstores/vector_doc.py` & `llmflows-0.0.3/llmflows/vectorstores/vector_doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module defines the VectorDoc class which is used to represent a document 
 with an optional embedding and metadata.
 """
 
-from typing import Optional, Tuple
+from typing import Optional
 from uuid import uuid4
 
 
 class VectorDoc:
     """
     Class representing a document with an optional embedding and metadata.
 
@@ -18,22 +18,14 @@
         metadata (dict, optional): Metadata for the document.
         embedding (list, optional): Embedding for the document.
 
     Attributes:
         doc_id (str): The unique identifier for the document.
         doc (str): The document text.
         metadata (dict): Optional metadata for the document.
-
-    Properties:
-        embedding (list): The embedding for the document.
-
-    Methods:
-        values() -> Tuple[str, str, list, dict]:
-            Returns a tuple of the document ID, document text, embedding, 
-            and metadata.
     """
 
     def __init__(
         self,
         doc: str,
         doc_id: str = None,
         metadata: Optional[dict] = None,
@@ -63,15 +55,15 @@
         )
 
     @embedding.setter
     def embedding(self, value):
         self._embedding = value
 
     @property
-    def values(self) -> Tuple[str, str, list, dict]:
+    def values(self) -> tuple[str, str, list, dict]:
         """
         Returns a tuple of the document ID, document text, embedding, and metadata.
 
         Raises:
             ValueError: If the embedding for the document has not been set.
 
         Returns:
```

### Comparing `llmflows-0.0.2/llmflows.egg-info/PKG-INFO` & `llmflows-0.0.3/llmflows.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 Metadata-Version: 2.1
 Name: llmflows
-Version: 0.0.2
-Summary: A simple and lightweight library for creating LLM-powered applications.
+Version: 0.0.3
+Summary: LLMFlows - Simple, Explicit and Transparent LLM Apps
 Author: Stoyan Stoyanov
-Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflow
-Project-URL: github, https://github.com/stoyan-stoyanov/llmflow
+Project-URL: Homepage, https://github.com/stoyan-stoyanov/llmflows
+Project-URL: github, https://github.com/stoyan-stoyanov/llmflows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# LLMFlows - Simple, Explicit and Transparent LLM Apps
+
 <p align="center">
-  <img src="docs/logo.png" />
+  <img style="width: 80%" src="docs/llmflows_last_logo.png" />
 </p>
 
 [![Twitter](https://img.shields.io/twitter/follow/LLMFlows?style=social)](https://twitter.com/LLMFlows)
+![Pylint workflow](https://github.com/stoyan-stoyanov/llmflow/actions/workflows/pylint.yml/badge.svg)
+![License](https://img.shields.io/github/license/stoyan-stoyanov/llmflow)
+![PyPi](https://img.shields.io/pypi/v/llmflows)
+![Stars](https://img.shields.io/github/stars/stoyan-stoyanov/llmflow?style=social)
+![Release date](https://img.shields.io/github/release-date/stoyan-stoyanov/llmflow?style=social)
+
+## About
+LLMFlows is a simple and lightweight framework for building LLM-powered applications.
 
 ## Installation
+You can quickly install LLMFlows with pip
 ```
 pip install llmflows
 ```
 
-## What is LLMFlowss?
-A simple and lightweitght library for creating LLM-powered applications.
-
 ## Philosophy
 
 ### Simple
-We have created LLMFlows with simplicity in mind while balancing for usability. We have a minimal set of classes that allow users to build powerful LLM-powered apps without compromising on capabilities.
+We want to build a framework with a minimal set of classes that allows users to build powerful LLM-powered apps without compromising on capabilities.
 
 ### Explicit
-We allow users to easily create complex LLM flows but we don't 
+We want to enable users to easily create complex flows of LLMs interacting with each other that have explicit and obvious structure.
 
 ### Transparent
-We don't have classes with hidden prompts - prompts are for you to decide.
+Flows are traceable, executions are easily logged and none of the classes provided in LLMFlows have hidden prompts. Default prompts introduce unexpected behavior and behavior drift when models are updated. 
 
-## Example
-Here is a basic example for creating an LLM with PromptTemplate:
+## Documentation
+The full documentation for LLMFlows can be found here.
+
+## Usage
+Here is a minimal example of an LLM with a PromptTemplate:
 
 ```python
 
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
 prompt_template = PromptTemplate(
    prompt="Generate a title for a 90s hip-hop song about {topic}."
 )
 llm_prompt = prompt_template.get_prompt(topic="friendship")
 
-print(llm_prompt)
-
 llm = OpenAI()
 song_title = llm.generate(llm_prompt)
-print(song_title)
 
 ```
 
 While this is a good example on how easy it is to use LLMFlows, real-world applications are more complex and have dependencies between prompts, and LLMs outputs. Let's take a look at such example. 
 ![Complex flow](docs/complex_flow.png)
-With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies for you and make sure each flowstep is executed only when the flowsteps it depends on are complete:
+With LLMFlows it's quite easy to reproduce this flow by utilizing the Flow and Flowstep classes. LLMFlows will figure out the dependencies and make sure each flowstep is executed only when the flowsteps it depends on are complete:
 
 ```python
 from llmflows.flows.flow import Flow
 from llmflows.flows.flowstep import FlowStep
 from llmflows.llms.openai import OpenAI
 from llmflows.prompts.prompt_template import PromptTemplate
 
@@ -120,48 +128,41 @@
 
 # Create and run Flow
 soundtrack_flow = Flow(flowstep1)
 soundtrack_flow.execute(topic="friendship")
 
 ```
 In fact, LLMFlows provides async, and threaded classes so any complex DAG can be executed in parallel.
-For more examples such as how to create Q&A apps and web applications with Flask and FastAPI check our documentation.
-
-## Usage patterns 
-1. Use LLMs-only
-
-    Use the LLM and Agents classes and tools to build free-roaming agents   
-
-2. Create Flows
-
-    Use the LLM and Agents classes and tools to build free-roaming agents
-
-3. Build web apps
-
-    Execute agents inside flowsteps where you can build conversational experiences with different stages and requirements
+For more examples such as how to create question answering apps and web applications with Flask and FastAPI check our documentation.
 
 ## FAQ
 
-### How is this different than langchian?
-Langchain is an amazing library and LLMFlows has been certainly been inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and while this is great for beginners and people who are not in the field of machine learning and language models, this can be a bit overwhelming. There are a lot of classes, hidden prompts in chains and many ways to do things. In contrast we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
+### How is this different than langchain?
+Langchain is a great library and LLMFlows has been been certainly inspired by it. However, our philosophy is a bit different. Langchian has a "chain for everything" philosophy and provides many classes that come with multiple LLM calls, logic, and built-in default prompts. While this is great for beginners and default use-cases, we feel this can be a bit overwhelming if users want to do anything "out of the ordinary". In contrast, we are focusing on providing as few building blocks as possible and having an easy to understand API while matching (and in some cases exceeding) the capabilities of langchain.
 
-### You only have OpenAI wrappers but I want to use ACMELLM
+### You only have OpenAI wrappers but I want to use AcmeLLM?
 We decided to release the library initially supporting only OpenAI LLMs but we have a roadmap and we will slowly add new wrappers around the most popular models. If you are willing to spend some time we are looking for contributors and maintainers
 
 ### You only support Pinecone and Redis vector DBs do you have plans to extend the list?
 Yes! We will also add Redis, Elastic Search and other popular solutions over time. If you want to help us out check out our contribution section.
 
-### Why can't I find any info related to document loaders
-For the time being we have decided not to implement document loaders for two reasons:
-1. There are plenty of super capable libraries like Llama-index and langchain that have tons of loaders.
-2. We think it is awkward to mix document loaders together with LLM flow and prompt management libraries since usually document loading happens in separate pipelines and is not part of the LLM-powered app.
+### Why can't I find any info related to document loaders?
+For the time being we have decided not to implement document loaders for few reasons:
+1. There are plenty of capable libraries like Llama-index and langchain that have tons of loaders.
+2. We think it is awkward to mix document loaders together with LLM and prompt management libraries since usually document loading happens in separate pipelines and are not part of the LLM-powered app.
+3. Real-life documents are messy. In our experience, no matter how many loaders are out there they will never cover all the specific use-cases.
 
 While we are not going to invest time into document loaders we might decide to change direction if we get significant interest and contributors.
 
 ### What about agents?
 We believe agents are the future of LLM-powered apps and we have a few basic examples in the repo. However, we are working on a agent-focused library built on top of llmflow.
 
+## License
+LLMFlows is covered by the MIT license. For more information check `LICENCE.md`.
 
 ## Contributing
+Thank you for spending the time to read our README! If you like what you saw and are considering contributing please check CONTRIBUTING.md
 
 ## Links
+Twitter
 
+Documentation
```

### Comparing `llmflows-0.0.2/pyproject.toml` & `llmflows-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llmflows"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Stoyan Stoyanov"},
 ]
-description = "A simple and lightweight library for creating LLM-powered applications."
+description = "LLMFlows - Simple, Explicit and Transparent LLM Apps"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -21,9 +21,9 @@
     "openai==0.27.4",
     "tiktoken==0.3.3",
     "pinecone-client==2.2.1",
     "urllib3==1.26.15"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/stoyan-stoyanov/llmflow"
-"github" = "https://github.com/stoyan-stoyanov/llmflow"
+"Homepage" = "https://github.com/stoyan-stoyanov/llmflows"
+"github" = "https://github.com/stoyan-stoyanov/llmflows"
```

