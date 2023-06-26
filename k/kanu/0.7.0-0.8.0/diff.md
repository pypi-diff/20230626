# Comparing `tmp/kanu-0.7.0.tar.gz` & `tmp/kanu-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.7.0.tar", last modified: Mon Jun 19 00:26:53 2023, max compression
+gzip compressed data, was "kanu-0.8.0.tar", last modified: Mon Jun 26 05:37:07 2023, max compression
```

## Comparing `kanu-0.7.0.tar` & `kanu-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.678251 kanu-0.7.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-19 00:26:42.000000 kanu-0.7.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)     2179 2023-06-19 00:26:53.678104 kanu-0.7.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)     1863 2023-06-19 00:26:42.000000 kanu-0.7.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.677262 kanu-0.7.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)    10562 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     2112 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)    10397 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)    12953 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/gui.py
--rw-r--r--   0 sbslee     (501) staff       (20)      697 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-19 00:26:42.000000 kanu-0.7.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-19 00:26:53.677900 kanu-0.7.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)     2179 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      276 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-19 00:26:53.000000 kanu-0.7.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-19 00:26:53.678303 kanu-0.7.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-19 00:26:42.000000 kanu-0.7.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.558762 kanu-0.8.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-26 05:36:52.000000 kanu-0.8.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)     2480 2023-06-26 05:37:07.558601 kanu-0.8.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)     2164 2023-06-26 05:36:52.000000 kanu-0.8.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.557714 kanu-0.8.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    16190 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     2083 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    10390 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     3691 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/funcgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)    13066 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/gui.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      999 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-26 05:36:52.000000 kanu-0.8.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-26 05:37:07.558408 kanu-0.8.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)     2480 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      292 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-26 05:37:07.000000 kanu-0.8.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-26 05:37:07.558816 kanu-0.8.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-26 05:36:52.000000 kanu-0.8.0/setup.py
```

### Comparing `kanu-0.7.0/LICENSE` & `kanu-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.7.0/PKG-INFO` & `kanu-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanu
-Version: 0.7.0
+Version: 0.8.0
 Summary: A minimalistic Python-based GUI for various chatbots
 Home-page: https://github.com/sbslee/kanu
 Author: Seung-been "Steven" Lee
 Author-email: sbstevenlee@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,14 +16,15 @@
 
 Welcome to KANU, a minimalistic Python-based GUI for various chatbots.
 
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
+- [FuncGPT](#funcgpt) can answer your questions by making calls to external tools, APIs, or databases
 
 Other features of KANU inclde:
 
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
 - Customize chat settings (e.g. font size and background color)
 - Display token counter and price monitor in chat window
 
@@ -71,11 +72,22 @@
 chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
+<a id="funcgpt"></a>
+### FuncGPT
+
+![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/funcgpt.gif)
+
+The following packages are required to run FuncGPT:
+
+```
+openai # Required.
+```
+
 ## Changelog
 
 See the [CHANGELOG.md](https://github.com/sbslee/kanu/blob/main/CHANGELOG.md) file for details.
```

### Comparing `kanu-0.7.0/README.md` & `kanu-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Welcome to KANU, a minimalistic Python-based GUI for various chatbots.
 
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
+- [FuncGPT](#funcgpt) can answer your questions by making calls to external tools, APIs, or databases
 
 Other features of KANU inclde:
 
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
 - Customize chat settings (e.g. font size and background color)
 - Display token counter and price monitor in chat window
 
@@ -59,10 +60,21 @@
 chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
+<a id="funcgpt"></a>
+### FuncGPT
+
+![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/funcgpt.gif)
+
+The following packages are required to run FuncGPT:
+
+```
+openai # Required.
+```
+
 ## Changelog
 
 See the [CHANGELOG.md](https://github.com/sbslee/kanu/blob/main/CHANGELOG.md) file for details.
```

### Comparing `kanu-0.7.0/kanu/__main__.py` & `kanu-0.8.0/kanu/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,65 @@
 from tkinter import ttk
 from tkinter import filedialog
 import importlib.util
 
 from .version import __version__
 from .gui import Tooltip
 
-GPT_MODELS = ["gpt-3.5-turbo", "gpt-3.5-turbo-16k", "gpt-4", "gpt-4-32k"]
+GPT_MODELS = [
+    "gpt-3.5-turbo",
+    "gpt-3.5-turbo-0613",
+    "gpt-3.5-turbo-16k",
+    "gpt-3.5-turbo-16k-0613",
+    "gpt-4",
+    "gpt-4-0613",
+    "gpt-4-32k",
+    "gpt-4-32k-0613",
+]
 CHATGPT_PROMPT = """You are a helpful assistant."""
 DOCGPT_PROMPT = """Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
 
 {context}
 
 Question: {question}
 Helpful Answer:"""
+FUNCGPT_PROMPT = """You are a helpful assistant."""
+FUNCGPT_EXAMPLE = """import json
+
+def get_current_weather(location, unit="fahrenheit"):
+    weather_info = {
+        "location": location,
+        "temperature": "72",
+        "unit": unit,
+        "forecast": ["sunny", "windy"],
+    }
+    return json.dumps(weather_info)
+
+get_current_weather_json = {
+    "name": "get_current_weather",
+    "description": "Get the current weather in a given location",
+    "parameters": {
+        "type": "object",
+        "properties": {
+            "location": {
+                "type": "string",
+                "description": "The city and state, e.g. San Francisco, CA",
+            },
+            "unit": {"type": "string", "enum": ["celsius", "fahrenheit"]},
+        },
+        "required": ["location"],
+    },
+}
+
+functions = {
+    "get_current_weather": {
+        "function": get_current_weather,
+        "json": get_current_weather_json,
+    }
+}"""
 
 class KANU:
     def __init__(self, root):
         self.container = None
         self.root = root
         self.root.title(f"KANU ({__version__})")
         self.root.geometry("700x620")
@@ -31,14 +74,16 @@
         self.container.pack()
         l = tk.Message(self.container, width=350, text="Welcome to KANU, a minimalistic Python-based GUI for various chatbots! Please select a chatbot to begin.")
         l.pack()
         b = tk.Button(self.container, text="ChatGPT", command=lambda: self.config_chatgpt())
         b.pack()
         b = tk.Button(self.container, text="DocGPT", command=lambda: self.config_docgpt())
         b.pack()
+        b = tk.Button(self.container, text="FuncGPT", command=lambda: self.config_funcgpt())
+        b.pack()
 
     def config_chatgpt(self):
         self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="ChatGPT")
         l.grid(row=0, column=0, columnspan=2)
@@ -179,23 +224,110 @@
         config = configparser.ConfigParser()
         config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT, "chunk_size": 1000, "chunk_overlap": 50}
         config["USER"] = {"openai_key": ""}
         config["OPTIONAL"] = {"new_database_directory": "", "document_directory": "", "existing_database_directory": ""}
         with open(file_path, "w") as f:
             config.write(f)
 
+    def config_funcgpt(self):
+        self.container.pack_forget()
+        self.container = tk.Frame(self.root)
+        self.container.pack()
+        l = tk.Label(self.container, text="FuncGPT")
+        l.grid(row=0, column=0, columnspan=2)
+        l = tk.Label(self.container, text="Required packages:")
+        l.grid(row=1, column=0, columnspan=2)
+        self.display_required_dependency(2, "openai")
+        m = tk.Message(self.container, width=300, text="Option 1. Upload a configuration file")
+        m.grid(row=3, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Browse", command=self.parse_funcgpt_config)
+        b.grid(row=4, column=0)
+        b = tk.Button(self.container, text="Template", command=self.template_funcgpt_config)
+        b.grid(row=4, column=1)
+        m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
+        m.grid(row=5, column=0, columnspan=2)
+        l = tk.Label(self.container, text="Model:")
+        l.grid(row=6, column=0, columnspan=2)
+        self.model = tk.StringVar(self.container, value="gpt-3.5-turbo-0613")
+        om = ttk.OptionMenu(self.container, self.model, "gpt-3.5-turbo-0613", *GPT_MODELS)
+        om.grid(row=7, column=0, columnspan=2)
+        l = tk.Label(self.container, text="System message ⓘ:")
+        Tooltip(l, "The system message helps set the behavior of the chatbot.")
+        l.grid(row=8, column=0, columnspan=2)
+        self.prompt = tk.Text(self.container, height=9, width=42)
+        sb = tk.Scrollbar(self.container, command=self.prompt.yview)
+        self.prompt.insert("1.0", FUNCGPT_PROMPT)
+        self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
+        sb.grid(row=9, column=2, sticky="ns")
+        self.prompt["yscrollcommand"] = sb.set
+        l = tk.Label(self.container, text="Function script:")
+        l.grid(row=10, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Browse", command=self.get_function_script)
+        b.grid(row=11, column=0)
+        b = tk.Button(self.container, text="Example", command=self.example_function_script)
+        b.grid(row=11, column=1)
+        l = tk.Label(self.container, text="Temperature ⓘ:")
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
+        l.grid(row=12, column=0, columnspan=2)
+        self.temperature = tk.DoubleVar(self.container, value=0.5)
+        e = tk.Entry(self.container, textvariable=self.temperature)
+        e.grid(row=13, column=0, columnspan=2)
+        l = tk.Label(self.container, text="OpenAI API key:")
+        l.grid(row=14, column=0, columnspan=2)
+        e = tk.Entry(self.container)
+        e.grid(row=15, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("FuncGPT", e.get(), self.model.get(), self.temperature.get(), self.prompt.get("1.0", "end-1c")))
+        b.grid(row=16, column=0)
+        b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
+        b.grid(row=16, column=1)
+
+    def parse_funcgpt_config(self):
+        config = configparser.ConfigParser()
+        file_path = filedialog.askopenfilename()
+        if not file_path:
+            return
+        config.read(file_path)
+        self.deploy_agent("FuncGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"], config["USER"]["function_script"])
+
+    def template_funcgpt_config(self):
+        file_path = filedialog.asksaveasfilename()
+        if not file_path:
+            return
+        config = configparser.ConfigParser()
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo-0613", "temperature": "0.5", "prompt": FUNCGPT_PROMPT}
+        config["USER"] = {"openai_key": "", "function_script": ""}
+        with open(file_path, "w") as f:
+            config.write(f)
+
+    def get_function_script(self):
+        file_path = filedialog.askopenfilename()
+        if not file_path:
+            return
+        self.script = file_path
+
+    def example_function_script(self):
+        file_path = filedialog.asksaveasfilename()
+        if not file_path:
+            return       
+        with open(file_path, "w") as f:
+            f.write(FUNCGPT_EXAMPLE)
+
     def deploy_agent(self, agent, *args, **kwargs):
         if agent == "ChatGPT":
             from .chatgpt import ChatGPT
             chatgpt = ChatGPT(self, *args, **kwargs)
             chatgpt.run()
         elif agent == "DocGPT":
             from .docgpt import DocGPT
             docgpt = DocGPT(self, *args, **kwargs)
             docgpt.run()
+        elif agent == "FuncGPT":
+            from .funcgpt import FuncGPT
+            docgpt = FuncGPT(self, *args, **kwargs)
+            docgpt.run()
         else:
             raise ValueError(f"Unknown agent {agent}")
         
     def display_required_dependency(self, row, package_name):
         l = tk.Label(self.container, text=package_name)
         l.grid(row=row, column=0)
         l = tk.Label(self.container, text="❌" if importlib.util.find_spec(package_name) is None else "✅")
```

### Comparing `kanu-0.7.0/kanu/chatgpt.py` & `kanu-0.8.0/kanu/chatgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,24 @@
             messages=self.messages,
             temperature=self.temperature,
         )
         response = bot_response["choices"][0]["message"]["content"]
         self.messages += [{"role": "assistant", "content": response}]
         self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
         self.session.insert(tk.END, f"Bot: " + response + "\n", "bot")
-        usage = self.calculate_usage(bot_response)
-        self.system.insert(tk.END, f"{usage}\n", "system")
+        self.calculate_usage(bot_response)
         self.chatbox.delete(0, tk.END)
 
     def calculate_usage(self, response):
         total_tokens = response["usage"]["total_tokens"]
         prompt_tokens = response["usage"]["prompt_tokens"]
         completion_tokens = response["usage"]["completion_tokens"]
         prompt_price = tokens2price(self.model, "prompt", prompt_tokens)
         completion_price = tokens2price(self.model, "completion", completion_tokens)
         self.price += prompt_price + completion_price
         self.tokens += total_tokens
         message = f"System: Used {prompt_tokens:,} prompt + {completion_tokens:,} completion = {total_tokens:,} tokens (total: {self.tokens:,} or ${self.price:.6f})."
-        return message
+        self.system.insert(tk.END, f"{message}\n", "system")
 
     def clear_session(self):
         self.tokens = self.price = 0
         self.run()
```

### Comparing `kanu-0.7.0/kanu/docgpt.py` & `kanu-0.8.0/kanu/docgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .utils import tokens2price, text2tokens
 
 DOCUMENT_LOADERS = {
     ".txt": (TextLoader, {"encoding": "utf8"}),
     ".pdf": (PDFMinerLoader, {}),
     ".doc": (UnstructuredWordDocumentLoader, {}),
     ".docx": (UnstructuredWordDocumentLoader, {}),
-    ".csv": (CSVLoader, {}),
+    ".csv": (CSVLoader, {"encoding": "utf8"}),
 }
 
 class DocGPT:
     def __init__(
         self,
         kanu,
         openai_key,
@@ -134,26 +134,25 @@
         )
         self.conversation.page()
 
     def send_message(self):
         self.session.insert(tk.END, "You: " + self.user_input.get() + "\n", "user")
         with get_openai_callback() as cb:
             response = self.qa(self.user_input.get())
-            usage = self.calculate_usage(cb)
+            self.calculate_usage(cb)
         self.session.insert(tk.END, "Bot: " + response["answer"] + "\n", "bot")
-        self.system.insert(tk.END, f"{usage}\n", "system")
         self.chatbox.delete(0, tk.END)
 
     def calculate_usage(self, cb):
         prompt_price = tokens2price(self.model, "prompt", cb.prompt_tokens)
         completion_price = tokens2price(self.model, "completion", cb.completion_tokens)
         self.price += prompt_price + completion_price
         self.tokens += cb.total_tokens
         message = f"System: Used {cb.prompt_tokens:,} prompt + {cb.completion_tokens:,} completion = {cb.total_tokens:,} tokens (total: {self.tokens:,} or ${self.price:.6f})."
-        return message
+        self.system.insert(tk.END, f"{message}\n", "system")
 
     def go_with_option1(self):
         self.database_directory = self.new_database_directory
         self.tokens = self.price = 0
         documents = []
         for root, dirs, files in os.walk(self.document_directory):
             for file in files:
@@ -164,15 +163,15 @@
                 loader_class, loader_kwargs = DOCUMENT_LOADERS[file_ext]
                 loader = loader_class(file_path, **loader_kwargs)
                 document = loader.load()
                 documents.extend(document)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=self.chunk_size.get(), chunk_overlap=self.chunk_overlap.get())
         texts = text_splitter.split_documents(documents)
         for text in texts:
-            self.tokens += text2tokens("text-embedding-ada-002", text.page_content)
+            self.tokens += 2 * text2tokens("text-embedding-ada-002", text.page_content)
         self.price = tokens2price("text-embedding-ada-002", "embedding", self.tokens)
         db = Chroma.from_documents(texts, OpenAIEmbeddings(model="text-embedding-ada-002"), persist_directory=self.database_directory)
         db.add_documents(texts)
         db.persist()
         db = None
         self.existing = False
         self.query()
```

### Comparing `kanu-0.7.0/kanu/gui.py` & `kanu-0.8.0/kanu/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class Conversation:
     def __init__(self, agent):
         self.agent = agent
         self.name = self.agent.__class__.__name__
         if self.name == "ChatGPT":
             self.go_back = self.agent.kanu.config_chatgpt
+        elif self.name == "FuncGPT":
+            self.go_back = self.agent.kanu.config_funcgpt
         else:
             self.go_back = self.agent.run
 
     def page(self):
         self.agent.previous = self.agent.kanu.container
         self.agent.kanu.container.pack_forget()
         self.agent.kanu.container = tk.Frame(self.agent.kanu.root)
@@ -57,15 +59,15 @@
         file_path = filedialog.asksaveasfilename()
         if not file_path:
             return
         data = "[System]\n"
         data += self.agent.system.get("1.0", tk.END).rstrip()
         data += "\n\n[Session]\n"
         data += self.agent.session.get("1.0", tk.END).rstrip()
-        with open(file_path, 'w') as f:
+        with open(file_path, 'w', encoding="utf-8") as f:
             f.write(data)
 
 class Settings:
     def __init__(self, agent):
         self.agent = agent
         self.default_font = font.nametofont("TkDefaultFont").actual()
         self.default_user_background_color = "gray85"
```

### Comparing `kanu-0.7.0/kanu.egg-info/PKG-INFO` & `kanu-0.8.0/kanu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanu
-Version: 0.7.0
+Version: 0.8.0
 Summary: A minimalistic Python-based GUI for various chatbots
 Home-page: https://github.com/sbslee/kanu
 Author: Seung-been "Steven" Lee
 Author-email: sbstevenlee@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -16,14 +16,15 @@
 
 Welcome to KANU, a minimalistic Python-based GUI for various chatbots.
 
 There are currently two chatbots available in KANU:
 
 - [ChatGPT](#chatgpt) harnesses the power of ChatGPT, bringing it directly to your local computer
 - [DocGPT](#docgpt) allows you to effortlessly interact with your documents and ask questions about them
+- [FuncGPT](#funcgpt) can answer your questions by making calls to external tools, APIs, or databases
 
 Other features of KANU inclde:
 
 - Customize chatbot parameters (e.g. prompt, temperature, and chunk size) by directly using the GUI or uploading a configuration file
 - Customize chat settings (e.g. font size and background color)
 - Display token counter and price monitor in chat window
 
@@ -71,11 +72,22 @@
 chromadb     # Required.
 tiktoken     # Required.
 pdfminer.six # Optional. Only required for .pdf documents.
 unstructured # Optional. Only required for .doc and .docx documents.
 tabulate     # Optional. Only required for .doc and .docx documents.
 ```
 
+<a id="funcgpt"></a>
+### FuncGPT
+
+![Alt Text](https://raw.githubusercontent.com/sbslee/kanu/main/images/funcgpt.gif)
+
+The following packages are required to run FuncGPT:
+
+```
+openai # Required.
+```
+
 ## Changelog
 
 See the [CHANGELOG.md](https://github.com/sbslee/kanu/blob/main/CHANGELOG.md) file for details.
```

### Comparing `kanu-0.7.0/setup.py` & `kanu-0.8.0/setup.py`

 * *Files identical despite different names*

