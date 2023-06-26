# Comparing `tmp/langkit-0.0.1b7.tar.gz` & `tmp/langkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1b7.tar", max compression
+gzip compressed data, was "langkit-0.0.2.tar", max compression
```

## Comparing `langkit-0.0.1b7.tar` & `langkit-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3046 2023-06-10 01:05:05.107906 langkit-0.0.1b7/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1b7/LICENSE
--rw-r--r--   0        0        0      998 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/all_metrics.py
--rw-r--r--   0        0        0      140 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1768 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-06-07 22:19:42.247907 langkit-0.0.1b7/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-06-07 22:19:42.247907 langkit-0.0.1b7/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    10756 2023-06-09 23:51:13.157907 langkit-0.0.1b7/langkit/docs/modules.md
--rw-r--r--   0        0        0    11219 2023-06-12 16:52:44.100690 langkit-0.0.1b7/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0     9391 2023-06-12 22:23:38.400690 langkit-0.0.1b7/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262428 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     5449 2023-06-12 16:56:49.630690 langkit-0.0.1b7/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0     1362 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/light_metrics.py
--rw-r--r--   0        0        0      499 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/llm_metrics.py
--rw-r--r--   0        0        0       75 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/openai/openai.py
--rw-r--r--   0        0        0     2441 2023-06-12 16:42:58.730690 langkit-0.0.1b7/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      793 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2962 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/sentiment.py
--rw-r--r--   0        0        0     3970 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/conftest.py
--rw-r--r--   0        0        0     1078 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-06-12 16:42:58.730690 langkit-0.0.1b7/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.1b7/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-06-11 03:02:39.184198 langkit-0.0.1b7/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-06-11 03:52:57.364198 langkit-0.0.1b7/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/themes.json.txt
--rw-r--r--   0        0        0     3652 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-06-09 23:51:13.167907 langkit-0.0.1b7/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-06-11 01:28:15.324198 langkit-0.0.1b7/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.1b7/langkit/transformer.py
--rw-r--r--   0        0        0    30472 2023-06-11 21:55:45.901756 langkit-0.0.1b7/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-06-10 01:05:05.107906 langkit-0.0.1b7/langkit/whylogs/samples.py
--rw-r--r--   0        0        0      907 2023-06-12 22:38:57.550690 langkit-0.0.1b7/pyproject.toml
--rw-r--r--   0        0        0     4046 1970-01-01 00:00:00.000000 langkit-0.0.1b7/PKG-INFO
+-rw-r--r--   0        0        0     3206 2023-06-14 02:43:40.085430 langkit-0.0.2/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.2/LICENSE
+-rw-r--r--   0        0        0      998 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/all_metrics.py
+-rw-r--r--   0        0        0      140 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1768 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-06-07 22:19:42.247907 langkit-0.0.2/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-06-07 22:19:42.247907 langkit-0.0.2/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    10756 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11230 2023-06-13 21:34:06.033640 langkit-0.0.2/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0     9718 2023-06-19 17:00:40.899522 langkit-0.0.2/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262944 2023-06-14 14:04:42.088909 langkit-0.0.2/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     7125 2023-06-13 23:12:44.753641 langkit-0.0.2/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0     1362 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/light_metrics.py
+-rw-r--r--   0        0        0      716 2023-06-14 02:43:40.085430 langkit-0.0.2/langkit/llm_metrics.py
+-rw-r--r--   0        0        0       75 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      793 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2938 2023-06-23 19:13:10.517672 langkit-0.0.2/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/sentiment.py
+-rw-r--r--   0        0        0     3970 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     1078 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-05-26 04:00:38.203377 langkit-0.0.2/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2273 2023-05-19 23:17:27.872537 langkit-0.0.2/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-05-19 23:17:27.872537 langkit-0.0.2/langkit/themes.json.txt
+-rw-r--r--   0        0        0     3652 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-06-13 21:34:06.043640 langkit-0.0.2/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-06-13 21:34:06.053640 langkit-0.0.2/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-05-19 23:17:27.872537 langkit-0.0.2/langkit/transformer.py
+-rw-r--r--   0        0        0    30472 2023-06-13 21:34:06.053640 langkit-0.0.2/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-06-13 21:34:06.053640 langkit-0.0.2/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-06-13 21:34:06.053640 langkit-0.0.2/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0      905 2023-06-26 21:39:05.250126 langkit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.2/PKG-INFO
```

### Comparing `langkit-0.0.1b7/DESCRIPTION.md` & `langkit-0.0.2/DESCRIPTION.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
+> 💡 Want to experience LangKit? Go to this [notebook](https://github.com/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)!
+
 ## Table of Contents 📖
 
 - [Motivation](#motivation-)
 - [Features](#features-)
 - [Installation](#installation-)
 - [Usage](#usage-)
 - [Modules](#modules-)
@@ -32,30 +34,29 @@
   - toxicity analysis
 
 ## Installation 💻
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 
 ```
-pip install langkit
+pip install langkit[all]
 ```
 
 ## Usage 🚀
 
+
 LangKit modules contain UDFs that automatically wire into the collection of UDFs on String features provided by whylogs by default. All we have to do is import the LangKit modules and then instantiate a custom schema as shown in the example below.
 
 ```python
 import whylogs as why
-from whylogs.experimental.core.udf_schema import udf_schema
-from langkit import sentiment
-from langkit import textstat
+from langkit import llm_metrics
 
-results = why.log({"prompt": "Hello!", "response": "World!"}, schema=udf_schema())
+results = why.log({"prompt": "Hello!", "response": "World!"}, schema=llm_metrics.init())
 ```
 
-The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules. This profile can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
+The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules. This profile can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/safeguard-large-language-models?utm_source=github&utm_medium=referral&utm_campaign=langkit) or they can be further analyzed by the user on their own accord.
 
 More examples are available [here](https://github.com/whylabs/langkit/tree/main/langkit/examples).
 
 ## Modules 📦
 
 You can have more information about the different modules and their metrics [here](https://github.com/whylabs/langkit/blob/main/langkit/docs/modules.md).
```

### Comparing `langkit-0.0.1b7/LICENSE` & `langkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/__init__.py` & `langkit-0.0.2/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/all_metrics.py` & `langkit-0.0.2/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/config/environment.py` & `langkit-0.0.2/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/docs/features/quality.md` & `langkit-0.0.2/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/docs/features/relevance.md` & `langkit-0.0.2/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/docs/features/security.md` & `langkit-0.0.2/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/docs/features/sentiment.md` & `langkit-0.0.2/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/docs/modules.md` & `langkit-0.0.2/langkit/docs/modules.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.2/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99921875%*

 * *Differences: {"'cells'": '{3: {\'source\': ["%pip install \'langkit[all]==0.0.1b7\' -q"]}}'}*

```diff
@@ -27,15 +27,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "%pip install langkig[all] -q"
+                "%pip install 'langkit[all]==0.0.1b7' -q"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `langkit-0.0.1b7/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.2/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9595219494047619%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'<a id="intro-to-langkit"></a>\\n\'), (3, \'[![Open '*

 * *            'in '*

 * *            "Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)\\n'), "*

 * *            "(8, '- [Intro to LangKit](#intro-to-langkit)\\n'), (9, '- [What is "*

 * *            "LangKit](#what-is-langkit)\\n'), (11, '- [Hello, World!](#hello-world)\\n'), (16, '<a "*

 * *            'id=" […]*

```diff
@@ -1,51 +1,55 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "<a id=\"intro-to-langkit\"></a>\n",
                 "## \ud83d\udcd6 Intro to LangKit\n",
                 "\n",
-                "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/langkit/blob/intro_to_langkit/langkit/examples/Intro_to_Langkit.ipynb)\n",
+                "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)\n",
                 "\n",
                 "\n",
                 "\n",
                 "Table of Contents\n",
-                "- [What is LangKit](#intro-to-langkit)\n",
+                "- [Intro to LangKit](#intro-to-langkit)\n",
+                "- [What is LangKit](#what-is-langkit)\n",
                 "- [Initialize LLM metrics](#initialize-llm-metrics)\n",
-                "- [Hello, World!](#hello,-world!)\n",
+                "- [Hello, World!](#hello-world)\n",
                 "- [Comparing Data](#comparing-data)\n",
                 "- [Monitor Metrics over time](#monitor-metrics-over-time)\n",
                 "- [Next Steps](#next-steps)\n",
                 "\n",
+                "<a id=\"what-is-langkit\"></a>\n",
                 "### \ud83d\udcda What is LangKit?\n",
                 ">LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).\n",
                 ">In this example, we'll look for distribution drift in the sentiment scores on the model response.\ud83d\udca1\n",
                 "\n",
                 "Ok! let's install __langkit__."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Note: you may need to restart the kernel to use updated packages.\n",
-                "%pip install 'langkit[all]==0.0.1b6' -q\n",
-                "%pip xformers ipywidgets -q\n"
+                "%pip install 'langkit[all]==0.0.1' -q\n",
+                "%pip install xformers ipywidgets -q\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "<a id=\"initialize-llm-metrics\"></a>\n",
                 "### \ud83d\ude80 Initialize LLM metrics\n",
                 "LangKit provides a toolkit of metrics for LLM applications, lets initialize them!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -61,14 +65,15 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "<a id=\"hello-world\"></a>\n",
                 "### \ud83d\udc4b Hello, World!\n",
                 "In the below code we log a few example prompt/response pairs and send metrics to WhyLabs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -83,29 +88,22 @@
                         "\n",
                         "\u2705 Aggregated 50 rows into profile 'langkit-sample-chats-all'\n",
                         "\n",
                         "Visualize and explore this profile with one-click\n"
                     ]
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Progress: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 5/5 [00:05<00:00,  1.00s/s]"
-                    ]
-                },
-                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\ud83d\udd0d https://hub.whylabsapp.com/resources/model-1/profiles?sessionToken=session-S7fFgCLc&profile=ref-om8bN6f90FSD4Hul\n"
+                        "\ud83d\udd0d https://hub.whylabsapp.com/resources/model-1/profiles?sessionToken=session-8gcsnbVy&profile=ref-AVbB1yOaSblsa89U\n"
                     ]
                 },
                 {
-                    "name": "stderr",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
@@ -120,16 +118,19 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "<a id=\"comparing-data\"></a>\n",
                 "### \ud83d\udd0d Comparing Data\n",
-                "Things get more interesting when you can compare two sets of metrics from an LLM application. The power of gathering systematic telemetry over time comes from being able to see how these metrics change, or how two sets of profiles compare. Below we asked GPT for some positive words and then asked for negative words as part of these two toy examples."
+                "Things get more interesting when you can compare two sets of metrics from an LLM application. The power of gathering systematic telemetry over time comes from being able to see how these metrics change, or how two sets of profiles compare. Below we asked GPT for some positive words and then asked for negative words as part of these two toy examples.\n",
+                "\n",
+                "> \ud83d\udca1 Take a look at the difference in the `response.sentiment_nltk` distributions between the two profiles. The first example is much more positive than the second example."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -143,33 +144,26 @@
                         "\n",
                         "\u2705 Aggregated 14 lines into profile 'positive_chats', 20 lines into profile 'negative_chats'\n",
                         "\n",
                         "Visualize and explore the profiles with one-click\n"
                     ]
                 },
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Progress: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 5/5 [00:05<00:00,  1.00s/s]"
-                    ]
-                },
-                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\ud83d\udd0d https://hub.whylabsapp.com/resources/model-1/profiles?sessionToken=session-S7fFgCLc&profile=ref-YN7OseBdZAjO6TzE&profile=ref-HopyPe8BwZW5sqyE\n",
+                        "\ud83d\udd0d https://hub.whylabsapp.com/resources/model-1/profiles?sessionToken=session-8gcsnbVy&profile=ref-ONdpltPp9jno6qMM&profile=ref-HoQEiEKtaaAvGG7S\n",
                         "\n",
                         "Or view each profile individually\n",
-                        " \u2937 https://hub.whylabsapp.com/resources/model-1/profiles?profile=ref-YN7OseBdZAjO6TzE&sessionToken=session-S7fFgCLc\n",
-                        " \u2937 https://hub.whylabsapp.com/resources/model-1/profiles?profile=ref-HopyPe8BwZW5sqyE&sessionToken=session-S7fFgCLc\n"
+                        " \u2937 https://hub.whylabsapp.com/resources/model-1/profiles?session-8gcsnbVy&profile=ref-ONdpltPp9jno6qMM\n",
+                        " \u2937 https://hub.whylabsapp.com/resources/model-1/profiles?session-8gcsnbVy&profile=ref-HoQEiEKtaaAvGG7S\n"
                     ]
                 },
                 {
-                    "name": "stderr",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
@@ -193,47 +187,54 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "<a id=\"monitor-metrics-over-time\"></a>\n",
                 "### \ud83d\udcc8 Monitor Metrics over time\n",
                 "\n",
-                "WhyLabs hosts a public demo org where we show a test LLM application being monitored over time. With LangKit telemetry collected over time, you can detect changes systematically and be alerted to potential problems in a deployed LLM application. We think a variety of different metrics can be helpful in detecting anamolies. In this example, something has triggered a series of alerts. Can you guess what went wrong? \n",
                 "\n",
-                "##### \ud83c\udfaf **Explore a demo environment** [here](https://hub.whylabsapp.com/resources/demo-model-llm/columns/prompt.sentiment_nltk?dateRange=2023-06-03-to-2023-06-09&profileReport=true&sessionToken=session-8gcsnbVy&targetOrgId=demo)!\n",
+                "WhyLabs hosts a public demo org where we show a test LLM application being monitored over time. With LangKit telemetry collected over time, you can detect changes systematically and be alerted to potential problems in a deployed LLM application. We think a variety of different metrics can be helpful in detecting anamolies. In this example, something has triggered a series of alerts. Can you guess what went wrong? \n",
                 "\n",
+                "##### \ud83c\udfaf **Explore a demo environment** [here](https://hub.whylabsapp.com/resources/demo-llm-chatbot/columns/prompt.sentiment_nltk?dateRange=2023-06-08-to-2023-06-09&sortModelBy=LatestAlert&sortModelDirection=DESC&targetOrgId=demo&sessionToken=session-8gcsnbVy)!\n",
                 "\n",
+                "<a id=\"next-steps\"></a>\n",
                 "### \u2705 Next Steps\n",
                 "If you see value in detecting changes in how your LLM application is behaving, you might take a look at some of our other examples showing how to monitor these metrics as a timeseries for an LLM application in production, or how to customize the metrics logged by using your own surrogate models or critic metrics.\n",
                 "* Check out the [examples](https://github.com/whylabs/langkit/tree/main/langkit/examples) folder for scenarios from [\"Hello World!\"](https://github.com/whylabs/langkit/blob/main/langkit/examples/Logging_Text.ipynb) to [monitoring an LLM](https://github.com/whylabs/langkit/blob/main/langkit/examples/LLM_to_WhyLabs.ipynb) in production!\n",
-                "* Learn more about the [features](https://github.com/whylabs/langkit#features) LangKit extracts out of the box.\n",
+                "* Learn more about the [features](https://github.com/whylabs/langkit#features-%EF%B8%8F) LangKit extracts out of the box.\n",
                 "* Learn more about LangKit's [modules documentation](https://github.com/whylabs/langkit/blob/main/langkit/docs/modules.md).\n",
-                "* Explore more on [WhyLabs](https://whylabs.ai/whylabs-free-sign-up?utm_source=github&utm_medium=referral&utm_campaign=langkit) and monitor your LLM application over time!\n",
+                "* Explore more on [WhyLabs](https://whylabs.ai/safeguard-large-language-models?utm_source=github&utm_medium=referral&utm_campaign=langkit) and monitor your LLM application over time!\n",
                 "\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "langkit-EeFODeF5-py3.8",
+            "display_name": "Python 3.11.2 64-bit",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.11.2"
         },
-        "orig_nbformat": 4
+        "orig_nbformat": 4,
+        "vscode": {
+            "interpreter": {
+                "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
+            }
+        }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `langkit-0.0.1b7/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.2/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987845904490829%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(5, '- Use a whylogs telemetry agent to gather statistics on "*

 * *            "the prompts/response and send these to WhyLabs\\n'), (6, '- View the systematic "*

 * *            'telemetry on your LLM in WhyLabs.\\n\'), (7, \'\\n\'), (8, "> Don\'t want to bother '*

 * *            "with setting up your credentials or running live LLM interactions? We've already done "*

 * *            'it for you and uploaded LangKit telemetry from prompt/response LLM interactions to a '*

 * *            'pub […]*

```diff
@@ -31,15 +31,18 @@
             "metadata": {},
             "source": [
                 "In this example, we'll show how to send your LLM metrics to your monitoring dashboard at WhyLabs Platform.\n",
                 "We will:\n",
                 "\n",
                 "- Define environment variables with the appropriate Credentials and IDs\n",
                 "- Log LLM prompts and responses into a profile\n",
-                "- Use the WhyLabs Writer to send the profile to your Project at WhyLabs"
+                "- Use a whylogs telemetry agent to gather statistics on the prompts/response and send these to WhyLabs\n",
+                "- View the systematic telemetry on your LLM in WhyLabs.\n",
+                "\n",
+                "> Don't want to bother with setting up your credentials or running live LLM interactions? We've already done it for you and uploaded LangKit telemetry from prompt/response LLM interactions to a public guest session in WhyLabs, no login required you can just click [here](https://hub.whylabsapp.com/resources/demo-llm-chatbot/columns/prompt.sentiment_nltk?dateRange=2023-06-08-to-2023-06-09&sortModelBy=LatestAlert&sortModelDirection=DESC&targetOrgId=demo&sessionToken=session-8gcsnbVy)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -51,15 +54,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Note: you may need to restart the kernel to use updated packages.\n",
-                "%pip install langkit"
+                "%pip install langkit[all] -q"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -96,15 +99,14 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from langkit.config import check_or_prompt_for_api_keys\n",
                 "from langkit.openai import ChatLog, send_prompt\n",
-                "from langkit.openai_wrapper import openai_logger\n",
                 "\n",
                 "check_or_prompt_for_api_keys()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -124,14 +126,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
+                "from langkit.whylogs.rolling_logger import RollingLogger\n",
+                "\n",
+                "telemetry_agent = RollingLogger()\n",
                 "\n",
                 "INTERACTIVE = bool(os.getenv(\"OPENAI_API_KEY\")) # set to True to test out interacting with ChatGPT\n",
                 "interactive_prompt = \"\"\n",
                 "if INTERACTIVE:\n",
                 "    print(f\"At any time input 'q' or anything that begins with q to quit. enter a question for the LLM\")\n",
                 "    while True:\n",
                 "        print()\n",
@@ -148,16 +153,14 @@
                 "\n",
                 "    archived_chats = load_dataset('alespalla/chatbot_instruction_prompts', split=\"test\", streaming=True)\n",
                 "    chats = iter(archived_chats)\n",
                 "    for _ in range(100):\n",
                 "      response = next(chats)\n",
                 "      telemetry_agent.log(response)\n",
                 "      print(response)\n",
-                "    # lets output the dataset metadata from hugging face so we can see how to\n",
-                "    # access some of the contained prompts and responses.\n",
                 "    print(\"done profiling\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
```

### Comparing `langkit-0.0.1b7/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.2/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.2/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7866319444444445%*

 * *Differences: {"'cells'": "{3: {'metadata': {replace: OrderedDict([('id', 'TAeYfAYnHp-u')])}, delete: "*

 * *            "['attachments']}, 4: {'metadata': {replace: OrderedDict([('id', 'Px1lNOkHHp-w')])}, "*

 * *            "delete: ['attachments']}, 5: {'metadata': {replace: OrderedDict([('id', "*

 * *            "'H0YNDLPOHp-w')])}}, 6: {'metadata': {replace: OrderedDict([('id', "*

 * *            "'beyHBap8Hp-x')])}, delete: ['attachments']}, 7: {'metadata': {replace: "*

 * *            "OrderedDict([('id', 'VRHZrfT2Hp-y')])}}, 8: {'metadata […]*

```diff
@@ -1,69 +1,108 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "id": "vvANigl6Hrcd"
+            },
+            "source": [
+                "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/LanguageToolkit/blob/main/langkit/examples/Sentiment_and_Toxicity.ipynb)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "frxW2u3RJk1D"
+            },
+            "source": [
+                "## Install LangKit\n",
+                "\n",
+                "First let's install __LangKit__."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "id": "f5IsgjyuKGWJ"
+            },
+            "outputs": [],
+            "source": [
+                "%pip install langkit[all]"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "TAeYfAYnHp-u"
+            },
             "source": [
                 "# Tracking Sentiment and Toxicity Scores in Text with Langkit\n",
                 "\n",
                 "In this example, we'll show how you can easily track sentiment and toxicity scores in text with Langkit.\n",
                 "\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "id": "Px1lNOkHHp-w"
+            },
             "source": [
                 "As an example, we'll use the [tweet_eval dataset](https://huggingface.co/datasets/tweet_eval). We'll use the `hateful` subset of the dataset, which contains tweets labeled as hateful or not hateful."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "id": "H0YNDLPOHp-w"
+            },
             "outputs": [],
             "source": [
                 "from datasets import load_dataset\n",
                 "\n",
                 "hateful_comments = load_dataset('tweet_eval','hate',split=\"train\", streaming=True)\n",
                 "comments = iter(hateful_comments)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "id": "beyHBap8Hp-x"
+            },
             "source": [
                 "## Initializing the Metrics\n",
                 "\n",
                 "To initialize the `toxicity` and `sentiment` metrics, we simply import the respective modules from `langkit`. This will automatically register the metrics, so we can start using them right away by creating a schema by calling `generate_udf_schema`. We will pass that schema to whylogs, so that it knows which metrics to track."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "id": "VRHZrfT2Hp-y"
+            },
             "outputs": [],
             "source": [
                 "\n",
                 "from whylogs.experimental.core.metrics.udf_metric import generate_udf_resolvers\n",
                 "from whylogs.core.schema import DeclarativeSchema\n",
                 "from langkit import toxicity, sentiment\n",
                 "\n",
                 "\n",
                 "text_schema = DeclarativeSchema(generate_udf_resolvers())"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "id": "X_68Wn0lHp-y"
+            },
             "source": [
                 "## Profiling the Data\n",
                 "\n",
                 "Now we're set to log our data.\n",
                 "\n",
                 "To make sure the metrics make sense, we will profile two separate groups of data:\n",
                 "- hateful comments: comments that are labeled as hateful\n",
@@ -72,16 +111,18 @@
                 "We can expect hateful comments to have a higher toxicity score and a lower sentiment score than non-hateful comments.\n",
                 "\n",
                 "Let's see if our metrics will reflect that."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
+            "execution_count": 6,
+            "metadata": {
+                "id": "9_nLmLE1Hp-z"
+            },
             "outputs": [],
             "source": [
                 "import whylogs as why\n",
                 "\n",
                 "# Just initializing the profiles with generic comments.\n",
                 "non_hateful_profile = why.log({\"comment\":\"I love flowers.\"}, schema=text_schema).profile()\n",
                 "hateful_profile = why.log({\"comment\":\"I hate biscuits.\"}, schema=text_schema).profile()\n",
@@ -91,36 +132,43 @@
                 "  if comment['label'] == 0:\n",
                 "    non_hateful_profile.track({\"comment\":comment['text']})\n",
                 "  else:\n",
                 "    hateful_profile.track({\"comment\":comment['text']})\n"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "id": "2rhVn7ToHp-z"
+            },
             "source": [
                 "Now that we have our profiles, let's check out the metrics. Let's compare the mean for our sentiment and toxicity scores, for each group (hateful and non-hateful):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
+            "execution_count": 7,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/"
+                },
+                "id": "43mdtqyIHp-0",
+                "outputId": "99bc1546-8313-4517-e2a4-aa3241a07226"
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "######### Sentiment #########\n",
                         "The average sentiment score for the hateful comments is -0.37580107526881734\n",
                         "The average sentiment score for the non-hateful comments is -0.062103669724770626\n",
                         "######### Toxicity #########\n",
-                        "The average toxicity score for the hateful comments is 0.37868360678354895\n",
-                        "The average toxicity score for the non-hateful comments is 0.1361061208838717\n"
+                        "The average toxicity score for the hateful comments is 0.378683618319932\n",
+                        "The average toxicity score for the non-hateful comments is 0.1361061258053561\n"
                     ]
                 }
             ],
             "source": [
                 "hateful_sentiment = hateful_profile.view().to_pandas()['udf/sentiment_nltk:distribution/mean'][0]\n",
                 "non_hateful_sentiment = non_hateful_profile.view().to_pandas()['udf/sentiment_nltk:distribution/mean'][0]\n",
                 "\n",
@@ -134,14 +182,17 @@
                 "print(\"######### Toxicity #########\")\n",
                 "print(f\"The average toxicity score for the hateful comments is {hateful_toxicity}\")\n",
                 "print(f\"The average toxicity score for the non-hateful comments is {non_hateful_toxicity}\")"
             ]
         }
     ],
     "metadata": {
+        "colab": {
+            "provenance": []
+        },
         "kernelspec": {
             "display_name": "langkit-vSL8Mxyz-py3.8",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
@@ -154,9 +205,9 @@
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.8.10"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 0
 }
```

### Comparing `langkit-0.0.1b7/langkit/injections.py` & `langkit-0.0.2/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/input_output.py` & `langkit-0.0.2/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/openai/openai.py` & `langkit-0.0.2/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/pattern_groups.json` & `langkit-0.0.2/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/regexes.py` & `langkit-0.0.2/langkit/regexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,27 +65,30 @@
         self.regex_groups = self.load_patterns()
 
     def get_regex_groups(self):
         return self.regex_groups
 
 
 pattern_loader = PatternLoader()
-if pattern_loader.get_regex_groups() is not None:
 
-    @register_metric_udf(col_type=String, type_mapper=AllString())
-    def has_patterns(text: str) -> Optional[str]:
-        regex_groups = pattern_loader.get_regex_groups()
-        patterns_info = None
-        if regex_groups:
-            for group in regex_groups:
-                for expression in group["expressions"]:
-                    if expression.search(text):
-                        patterns_info = group["name"]
-                        return group["name"]
-        return patterns_info
+
+def has_patterns(text: str) -> Optional[str]:
+    regex_groups = pattern_loader.get_regex_groups()
+    patterns_info = None
+    if regex_groups:
+        for group in regex_groups:
+            for expression in group["expressions"]:
+                if expression.search(text):
+                    patterns_info = group["name"]
+                    return group["name"]
+    return patterns_info
+
+
+if pattern_loader.get_regex_groups() is not None:
+    register_metric_udf(col_type=String, type_mapper=AllString())(has_patterns)
 
 
 def init(pattern_file_path: Optional[str] = None):
     if pattern_file_path:
         lang_config.pattern_file_path = pattern_file_path
         pattern_loader.set_config(lang_config)
         pattern_loader.update_patterns()
```

### Comparing `langkit-0.0.1b7/langkit/sentiment.py` & `langkit-0.0.2/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/conftest.py` & `langkit-0.0.2/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/test_injections.py` & `langkit-0.0.2/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/test_input_output.py` & `langkit-0.0.2/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/test_patterns.py` & `langkit-0.0.2/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/test_themes.py` & `langkit-0.0.2/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/tests/test_toxicity.py` & `langkit-0.0.2/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/textstat.py` & `langkit-0.0.2/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/themes.json` & `langkit-0.0.2/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/themes.py` & `langkit-0.0.2/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/topics.py` & `langkit-0.0.2/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/toxicity.py` & `langkit-0.0.2/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/whylogs/reference_chats.json` & `langkit-0.0.2/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/langkit/whylogs/samples.py` & `langkit-0.0.2/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1b7/pyproject.toml` & `langkit-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.1b7"
+version = "0.0.2"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-whylogs = {version = "1.1.45.dev4"}
+whylogs = {version = "1.1.47.dev0"}
 textstat = "^0.7.3"
 pandas = "*"
 
 
 # optional dependencies
 torch = {version = "*", optional = true}
 datasets = {version ="^2.12.0", optional = true}
```

### Comparing `langkit-0.0.1b7/PKG-INFO` & `langkit-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.1b7
+Version: 0.0.2
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,21 @@
 Requires-Dist: datasets (>=2.12.0,<3.0.0) ; extra == "all"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "all"
 Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "all"
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
-Requires-Dist: whylogs (==1.1.45.dev4)
+Requires-Dist: whylogs (==1.1.47.dev0)
 Description-Content-Type: text/markdown
 
 LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
+> 💡 Want to experience LangKit? Go to this [notebook](https://github.com/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)!
+
 ## Table of Contents 📖
 
 - [Motivation](#motivation-)
 - [Features](#features-)
 - [Installation](#installation-)
 - [Usage](#usage-)
 - [Modules](#modules-)
@@ -57,31 +59,30 @@
   - toxicity analysis
 
 ## Installation 💻
 
 To install LangKit, use the Python Package Index (PyPI) as follows:
 
 ```
-pip install langkit
+pip install langkit[all]
 ```
 
 ## Usage 🚀
 
+
 LangKit modules contain UDFs that automatically wire into the collection of UDFs on String features provided by whylogs by default. All we have to do is import the LangKit modules and then instantiate a custom schema as shown in the example below.
 
 ```python
 import whylogs as why
-from whylogs.experimental.core.udf_schema import udf_schema
-from langkit import sentiment
-from langkit import textstat
+from langkit import llm_metrics
 
-results = why.log({"prompt": "Hello!", "response": "World!"}, schema=udf_schema())
+results = why.log({"prompt": "Hello!", "response": "World!"}, schema=llm_metrics.init())
 ```
 
-The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules. This profile can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/) or they can be further analyzed by the user on their own accord.
+The code above will produce a set of metrics comprised of the default whylogs metrics for text features and all the metrics defined in the imported modules. This profile can be visualized and monitored in the [WhyLabs platform](https://whylabs.ai/safeguard-large-language-models?utm_source=github&utm_medium=referral&utm_campaign=langkit) or they can be further analyzed by the user on their own accord.
 
 More examples are available [here](https://github.com/whylabs/langkit/tree/main/langkit/examples).
 
 ## Modules 📦
 
 You can have more information about the different modules and their metrics [here](https://github.com/whylabs/langkit/blob/main/langkit/docs/modules.md).
```

