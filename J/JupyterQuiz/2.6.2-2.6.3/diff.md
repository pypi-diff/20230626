# Comparing `tmp/jupyterquiz-2.6.2.tar.gz` & `tmp/jupyterquiz-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterquiz-2.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jupyterquiz-2.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupyterquiz-2.6.2.tar` & `jupyterquiz-2.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 jupyterquiz-2.6.2/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 jupyterquiz-2.6.2/CITATION.cff
--rw-r--r--   0        0        0   104165 2023-05-25 18:35:02.178985 jupyterquiz-2.6.2/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 jupyterquiz-2.6.2/LICENSE
--rw-r--r--   0        0        0    12397 2023-05-25 18:42:50.469959 jupyterquiz-2.6.2/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 jupyterquiz-2.6.2/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 jupyterquiz-2.6.2/examples/num-example.gif
--rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 jupyterquiz-2.6.2/examples/questions.json
--rw-r--r--   0        0        0      661 2023-05-25 18:42:59.048642 jupyterquiz-2.6.2/jupyterquiz/__init__.py
--rw-r--r--   0        0        0    10879 2023-05-25 18:41:05.117384 jupyterquiz-2.6.2/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 jupyterquiz-2.6.2/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2023-05-12 09:47:31.721699 jupyterquiz-2.6.2/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 jupyterquiz-2.6.2/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 jupyterquiz-2.6.2/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     6192 2023-05-12 09:47:31.722254 jupyterquiz-2.6.2/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2935 2023-05-25 18:35:28.477892 jupyterquiz-2.6.2/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 jupyterquiz-2.6.2/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 jupyterquiz-2.6.2/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 jupyterquiz-2.6.2/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 jupyterquiz-2.6.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 jupyterquiz-2.6.2/schema/README
--rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 jupyterquiz-2.6.2/schema/mc_schema.json
--rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 jupyterquiz-2.6.2/schema/mc_schema.png
--rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 jupyterquiz-2.6.2/schema/mc_schema.svg
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 jupyterquiz-2.6.2/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 jupyterquiz-2.6.2/schema/num_schema.png
--rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 jupyterquiz-2.6.2/schema/schema.ipynb
--rw-r--r--   0        0        0   349141 2023-04-28 15:41:36.693358 jupyterquiz-2.6.2/test.ipynb
--rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 jupyterquiz-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 jupyterquiz-2.6.3/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 jupyterquiz-2.6.3/CITATION.cff
+-rw-r--r--   0        0        0   104165 2023-05-25 18:35:02.178985 jupyterquiz-2.6.3/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 jupyterquiz-2.6.3/LICENSE
+-rw-r--r--   0        0        0    12397 2023-05-25 18:42:50.469959 jupyterquiz-2.6.3/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 jupyterquiz-2.6.3/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 jupyterquiz-2.6.3/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 jupyterquiz-2.6.3/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-06-26 13:35:39.789384 jupyterquiz-2.6.3/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0    10874 2023-06-26 13:33:23.126405 jupyterquiz-2.6.3/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 jupyterquiz-2.6.3/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2023-05-12 09:47:31.721699 jupyterquiz-2.6.3/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 jupyterquiz-2.6.3/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 jupyterquiz-2.6.3/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     6192 2023-05-12 09:47:31.722254 jupyterquiz-2.6.3/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2935 2023-05-25 18:35:28.477892 jupyterquiz-2.6.3/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 jupyterquiz-2.6.3/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 jupyterquiz-2.6.3/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 jupyterquiz-2.6.3/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 jupyterquiz-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 jupyterquiz-2.6.3/schema/README
+-rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 jupyterquiz-2.6.3/schema/mc_schema.json
+-rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 jupyterquiz-2.6.3/schema/mc_schema.png
+-rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 jupyterquiz-2.6.3/schema/mc_schema.svg
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 jupyterquiz-2.6.3/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 jupyterquiz-2.6.3/schema/num_schema.png
+-rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 jupyterquiz-2.6.3/schema/schema.ipynb
+-rw-r--r--   0        0        0   356502 2023-06-26 13:35:10.973653 jupyterquiz-2.6.3/test.ipynb
+-rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 jupyterquiz-2.6.3/PKG-INFO
```

### Comparing `jupyterquiz-2.6.2/.gitignore` & `jupyterquiz-2.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/HideQuiz.ipynb` & `jupyterquiz-2.6.3/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/LICENSE` & `jupyterquiz-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/README.md` & `jupyterquiz-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/examples/mc-example.gif` & `jupyterquiz-2.6.3/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/examples/num-example.gif` & `jupyterquiz-2.6.3/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/examples/questions.json` & `jupyterquiz-2.6.3/examples/questions.json`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/__init__.py` & `jupyterquiz-2.6.3/jupyterquiz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.6.2'
+__version__ = '2.6.3'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `jupyterquiz-2.6.2/jupyterquiz/dynamic.py` & `jupyterquiz-2.6.3/jupyterquiz/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from IPython.core.display import display, Javascript, HTML
+from IPython.display import display, Javascript, HTML
 import string
 import random
 import importlib.resources
 import urllib.request
 import urllib
 import json
 import sys
```

### Comparing `jupyterquiz-2.6.2/jupyterquiz/helpers.js` & `jupyterquiz-2.6.3/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/multiple_choice.js` & `jupyterquiz-2.6.3/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/multiple_choice.py` & `jupyterquiz-2.6.3/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/numeric.js` & `jupyterquiz-2.6.3/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/show_questions.js` & `jupyterquiz-2.6.3/jupyterquiz/show_questions.js`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/jupyterquiz/styles.css` & `jupyterquiz-2.6.3/jupyterquiz/styles.css`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/preserve-responses.ipynb` & `jupyterquiz-2.6.3/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/previews/github-preview.png` & `jupyterquiz-2.6.3/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/previews/github-preview.psd` & `jupyterquiz-2.6.3/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/mc_schema.json` & `jupyterquiz-2.6.3/schema/mc_schema.json`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/mc_schema.png` & `jupyterquiz-2.6.3/schema/mc_schema.png`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/mc_schema.svg` & `jupyterquiz-2.6.3/schema/mc_schema.svg`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/num_schema.json` & `jupyterquiz-2.6.3/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/num_schema.png` & `jupyterquiz-2.6.3/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/schema/schema.ipynb` & `jupyterquiz-2.6.3/schema/schema.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterquiz-2.6.2/test.ipynb` & `jupyterquiz-2.6.3/test.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927029140098448%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from jupyterquiz import display_quiz\\n')], delete: "*

 * *            "[0]}}, 3: {'outputs': {0: {'data': {'text/html': {insert: [(0, '<div "*

 * *            'id="hpYlwehhNuYp" data-shufflequestions="False"\\n\'), (6, \'#hpYlwehhNuYp {\\n\')], '*

 * *            "delete: [6, 0]}}}, 1: {'data': {'application/javascript': {insert: [(0, 'var "*

 * *            'questionshpYlwehhNuYp=[\\n\'), (592, \'                    if ("feedback" in answer) '*

 * *            "{\\n'), (593, '            […]*

```diff
@@ -24,15 +24,15 @@
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                " from jupyterquiz import display_quiz\n",
+                "from jupyterquiz import display_quiz\n",
                 "\n",
                 "git_path=\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -46,21 +46,21 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"WbMLHJZUZezv\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"hpYlwehhNuYp\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 10px; text-align: left\"> <style>\n",
-                            "#WbMLHJZUZezv {\n",
+                            "#hpYlwehhNuYp {\n",
                             "   --jq-multiple-choice-bg: #6f78ffff;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #f75c03ff;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -234,15 +234,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsWbMLHJZUZezv=[\n",
+                            "var questionshpYlwehhNuYp=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -826,15 +826,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -1207,28 +1211,42 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"hpYlwehhNuYp\")) {\n",
+                            "            show_questions(questionshpYlwehhNuYp,  hpYlwehhNuYp); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        //console.log(element);\n",
                             "        {\n",
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, WbMLHJZUZezv))\n",
+                            "        .then(json => show_questions(json, hpYlwehhNuYp))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionsWbMLHJZUZezv, WbMLHJZUZezv);\n",
+                            "        show_questions(questionshpYlwehhNuYp, hpYlwehhNuYp);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -1254,27 +1272,27 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"rtjweNvxTDsH\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"AHYKHybrASUB\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 10px; text-align: left\"> <style>\n",
-                            "#rtjweNvxTDsH {\n",
+                            "#AHYKHybrASUB {\n",
                             "   --jq-multiple-choice-bg: #345995;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #e26d5a;\n",
-                            "   --Jq-numeric-bg: #5bc0eb;\n",
+                            "   --jq-numeric-bg: #5bc0eb;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
                             "   --jq-numeric-input-label: #101010;\n",
                             "   --jq-numeric-input-shadow: #999999;\n",
                             "   --jq-incorrect-color: #666666;\n",
                             "   --jq-correct-color: #87a878;\n",
                             "   --jq-text-color: #fafafa;\n",
                             "}\n",
@@ -1442,15 +1460,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsrtjweNvxTDsH=[\n",
+                            "var questionsAHYKHybrASUB=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -2034,15 +2052,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -2415,28 +2437,42 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"AHYKHybrASUB\")) {\n",
+                            "            show_questions(questionsAHYKHybrASUB,  AHYKHybrASUB); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        //console.log(element);\n",
                             "        {\n",
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, rtjweNvxTDsH))\n",
+                            "        .then(json => show_questions(json, AHYKHybrASUB))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionsrtjweNvxTDsH, rtjweNvxTDsH);\n",
+                            "        show_questions(questionsAHYKHybrASUB, AHYKHybrASUB);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -2463,21 +2499,21 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"mtazkLoOYhRm\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"NxswTtvdSWVm\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 10px; text-align: left\"> <style>\n",
-                            "#mtazkLoOYhRm {\n",
+                            "#NxswTtvdSWVm {\n",
                             "   --jq-multiple-choice-bg: #a45995;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #224dea;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -2651,15 +2687,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsmtazkLoOYhRm=[\n",
+                            "var questionsNxswTtvdSWVm=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -3243,15 +3279,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -3624,17 +3664,36 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"NxswTtvdSWVm\")) {\n",
+                            "            show_questions(questionsNxswTtvdSWVm,  NxswTtvdSWVm); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        {\n",
-                            "        show_questions(questionsmtazkLoOYhRm,  mtazkLoOYhRm);\n",
+                            "        // console.log(element);\n",
+                            "\n",
+                            "        //console.log(\"NxswTtvdSWVm\");\n",
+                            "        // console.log(document.getElementById(\"NxswTtvdSWVm\"));\n",
+                            "\n",
+                            "        try_show();\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -3664,21 +3723,21 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"sXGHLgQXWCMu\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"MomaSwqsbgha\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 0px; text-align: left\"> <style>\n",
-                            "#sXGHLgQXWCMu {\n",
+                            "#MomaSwqsbgha {\n",
                             "   --jq-multiple-choice-bg: #6f78ffff;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #f75c03ff;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -3852,15 +3911,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionssXGHLgQXWCMu=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Testing parameter to change number of colums for answers: Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answer_cols\": 4, \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"precision\": 2, \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Determine the output of the following Python code:\", \"code\": \"a=\\\"1\\\"\\nb=\\\"2\\\"\\nprint(a+b)\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"1\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"2\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"12\", \"correct\": true, \"feedback\": \"Yes. The + operator will concatenate the strings \\\"1\\\" and \\\"2\\\".\"}, {\"answer\": \"error\", \"correct\": false, \"feedback\": \"No. The + operator for strings performs string concatenation.\"}]}, {\"question\": \"The variable mylist is a Python list. Choose which code snippet will append the item 3 to mylist.\", \"type\": \"multiple_choice\", \"answers\": [{\"code\": \"mylist+=3\", \"correct\": false}, {\"code\": \"mylist+=[3]\", \"correct\": true}, {\"code\": \"mylist+={3}\", \"correct\": false}]}, {\"question\": \"Which of these is the ratio of a circle's circumference to its diameter?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"$\\\\pi$\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"$\\\\frac{22}{7}$\", \"correct\": false, \"feedback\": \"$\\\\frac{22}{7}$ is only an approximation to the true value.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"This is a crude approximation to the true value.\"}, {\"answer\": \"$\\\\tau$\", \"correct\": false, \"feedback\": \"True for the ratio of the circle's circumference to its radius, not diameter.\"}]}];\n",
+                            "var questionsMomaSwqsbgha=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Testing parameter to change number of colums for answers: Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answer_cols\": 4, \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"precision\": 2, \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Determine the output of the following Python code:\", \"code\": \"a=\\\"1\\\"\\nb=\\\"2\\\"\\nprint(a+b)\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"1\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"2\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"12\", \"correct\": true, \"feedback\": \"Yes. The + operator will concatenate the strings \\\"1\\\" and \\\"2\\\".\"}, {\"answer\": \"error\", \"correct\": false, \"feedback\": \"No. The + operator for strings performs string concatenation.\"}]}, {\"question\": \"The variable mylist is a Python list. Choose which code snippet will append the item 3 to mylist.\", \"type\": \"multiple_choice\", \"answers\": [{\"code\": \"mylist+=3\", \"correct\": false}, {\"code\": \"mylist+=[3]\", \"correct\": true}, {\"code\": \"mylist+={3}\", \"correct\": false}]}, {\"question\": \"Which of these is the ratio of a circle's circumference to its diameter?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"$\\\\pi$\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"$\\\\frac{22}{7}$\", \"correct\": false, \"feedback\": \"$\\\\frac{22}{7}$ is only an approximation to the true value.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"This is a crude approximation to the true value.\"}, {\"answer\": \"$\\\\tau$\", \"correct\": false, \"feedback\": \"True for the ratio of the circle's circumference to its radius, not diameter.\"}]}];\n",
                             "    // Make a random ID\n",
                             "function makeid(length) {\n",
                             "    var result = [];\n",
                             "    var characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';\n",
                             "    var charactersLength = characters.length;\n",
                             "    for (var i = 0; i < length; i++) {\n",
                             "        result.push(characters.charAt(Math.floor(Math.random() * charactersLength)));\n",
@@ -4208,15 +4267,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -4589,17 +4652,36 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"MomaSwqsbgha\")) {\n",
+                            "            show_questions(questionsMomaSwqsbgha,  MomaSwqsbgha); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        {\n",
-                            "        show_questions(questionssXGHLgQXWCMu,  sXGHLgQXWCMu);\n",
+                            "        // console.log(element);\n",
+                            "\n",
+                            "        //console.log(\"MomaSwqsbgha\");\n",
+                            "        // console.log(document.getElementById(\"MomaSwqsbgha\"));\n",
+                            "\n",
+                            "        try_show();\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -4641,21 +4723,21 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"kjGOhhXGFOvQ\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"xYWVNEQUATBW\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"2\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 10px; text-align: left\"> <style>\n",
-                            "#kjGOhhXGFOvQ {\n",
+                            "#xYWVNEQUATBW {\n",
                             "   --jq-multiple-choice-bg: #6f78ffff;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #f75c03ff;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -4829,15 +4911,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionskjGOhhXGFOvQ=[\n",
+                            "var questionsxYWVNEQUATBW=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -5421,15 +5503,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -5802,28 +5888,42 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"xYWVNEQUATBW\")) {\n",
+                            "            show_questions(questionsxYWVNEQUATBW,  xYWVNEQUATBW); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        //console.log(element);\n",
                             "        {\n",
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, kjGOhhXGFOvQ))\n",
+                            "        .then(json => show_questions(json, xYWVNEQUATBW))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionskjGOhhXGFOvQ, kjGOhhXGFOvQ);\n",
+                            "        show_questions(questionsxYWVNEQUATBW, xYWVNEQUATBW);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -5849,21 +5949,21 @@
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"BEoYSAHdWecR\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"nbRXWAeBDiRA\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"600\"\n",
                             "               style=\"border-radius: 10px; text-align: left\"> <style>\n",
-                            "#BEoYSAHdWecR {\n",
+                            "#nbRXWAeBDiRA {\n",
                             "   --jq-multiple-choice-bg: #6f78ffff;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #f75c03ff;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -6037,15 +6137,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsBEoYSAHdWecR=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}];\n",
+                            "var questionsnbRXWAeBDiRA=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}];\n",
                             "    // Make a random ID\n",
                             "function makeid(length) {\n",
                             "    var result = [];\n",
                             "    var characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';\n",
                             "    var charactersLength = characters.length;\n",
                             "    for (var i = 0; i < length; i++) {\n",
                             "        result.push(characters.charAt(Math.floor(Math.random() * charactersLength)));\n",
@@ -6393,15 +6493,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -6774,17 +6878,36 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"nbRXWAeBDiRA\")) {\n",
+                            "            show_questions(questionsnbRXWAeBDiRA,  nbRXWAeBDiRA); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        {\n",
-                            "        show_questions(questionsBEoYSAHdWecR,  BEoYSAHdWecR);\n",
+                            "        // console.log(element);\n",
+                            "\n",
+                            "        //console.log(\"nbRXWAeBDiRA\");\n",
+                            "        // console.log(document.getElementById(\"nbRXWAeBDiRA\"));\n",
+                            "\n",
+                            "        try_show();\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -6809,21 +6932,21 @@
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"wferKhhSOoyR\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"ZFoksvXhloLH\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
                             "               data-maxwidth=\"1000\"\n",
                             "               style=\"border-radius: 0px; text-align: center\"> <style>\n",
-                            "#wferKhhSOoyR {\n",
+                            "#ZFoksvXhloLH {\n",
                             "   --jq-multiple-choice-bg: #6f78ffff;\n",
                             "   --jq-mc-button-bg: #fafafa;\n",
                             "   --jq-mc-button-border: #e0e0e0e0;\n",
                             "   --jq-mc-button-inset-shadow: #555555;\n",
                             "   --jq-many-choice-bg: #f75c03ff;\n",
                             "   --jq-numeric-bg: #392061ff;\n",
                             "   --jq-numeric-input-bg: #c0c0c0;\n",
@@ -6997,15 +7120,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionswferKhhSOoyR=[\n",
+                            "var questionsZFoksvXhloLH=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -7589,15 +7712,19 @@
                             "        answers.every(answer => {\n",
                             "            //console.log(answer.type);\n",
                             "\n",
                             "            correct = false;\n",
                             "            // if (answer.type==\"value\"){\n",
                             "            if ('value' in answer) {\n",
                             "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
+                            "                    if (\"feedback\" in answer) {\n",
+                            "                        fb.textContent = jaxify(answer.feedback);\n",
+                            "                    } else {\n",
+                            "                        fb.textContent = jaxify(\"Correct\");\n",
+                            "                    }\n",
                             "                    correct = answer.correct;\n",
                             "                    //console.log(answer.correct);\n",
                             "                    done = true;\n",
                             "                }\n",
                             "                // } else if (answer.type==\"range\") {\n",
                             "            } else if ('range' in answer) {\n",
                             "                //console.log(answer.range);\n",
@@ -7970,28 +8097,42 @@
                             "            } else {\n",
                             "                console.log(\"MathJax not found\");\n",
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
-                            "\n",
+                            "/* This is to handle asynchrony issues in loading Jupyter notebooks\n",
+                            "           where the quiz has been previously run. The Javascript was generally\n",
+                            "           being run before the div was added to the DOM. I tried to do this\n",
+                            "           more elegantly using Mutation Observer, but I didn't get it to work.\n",
+                            "\n",
+                            "           Someone more knowledgeable could make this better ;-) */\n",
+                            "\n",
+                            "        function try_show() {\n",
+                            "          if(document.getElementById(\"ZFoksvXhloLH\")) {\n",
+                            "            show_questions(questionsZFoksvXhloLH,  ZFoksvXhloLH); \n",
+                            "          } else {\n",
+                            "             setTimeout(try_show, 200);\n",
+                            "          }\n",
+                            "        };\n",
+                            "    \n",
                             "        //console.log(element);\n",
                             "        {\n",
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, wferKhhSOoyR))\n",
+                            "        .then(json => show_questions(json, ZFoksvXhloLH))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionswferKhhSOoyR, wferKhhSOoyR);\n",
+                            "        show_questions(questionsZFoksvXhloLH, ZFoksvXhloLH);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -7999,21 +8140,14 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "display_quiz(git_path+\"questions.json\", border_radius=0, question_alignment='center', max_width=1000)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "finalized": {
             "timestamp": 1622215912635,
             "trusted": true
         },
```

### Comparing `jupyterquiz-2.6.2/PKG-INFO` & `jupyterquiz-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.6.2
+Version: 2.6.3
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
```

