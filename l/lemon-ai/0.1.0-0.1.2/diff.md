# Comparing `tmp/lemon-ai-0.1.0.tar.gz` & `tmp/lemon-ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon-ai-0.1.0.tar", last modified: Thu Jun 22 20:01:48 2023, max compression
+gzip compressed data, was "lemon-ai-0.1.2.tar", last modified: Mon Jun 26 10:26:46 2023, max compression
```

## Comparing `lemon-ai-0.1.0.tar` & `lemon-ai-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-22 20:19:35.297922 lemon-ai-0.1.0/
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1076 2023-06-22 18:20:13.000000 lemon-ai-0.1.0/LICENSE
--rw-r--r--   0 aah120    (1000) aah120    (1000)      725 2023-06-22 20:19:35.294912 lemon-ai-0.1.0/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)        0 2023-06-22 18:20:52.000000 lemon-ai-0.1.0/README.md
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-22 20:19:35.089837 lemon-ai-0.1.0/lemon_ai/
--rw-r--r--   0 aah120    (1000) aah120    (1000)       92 2023-06-22 18:46:51.000000 lemon-ai-0.1.0/lemon_ai/__init__.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1525 2023-06-22 10:49:21.000000 lemon-ai-0.1.0/lemon_ai/cito_api_wrapper.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      774 2023-06-22 18:48:58.000000 lemon-ai-0.1.0/lemon_ai/cito_tool.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     4869 2023-06-22 18:54:08.000000 lemon-ai-0.1.0/lemon_ai/cito_toolkit.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      601 2023-06-22 18:49:09.000000 lemon-ai-0.1.0/lemon_ai/cito_workflow.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      428 2023-06-22 18:26:26.000000 lemon-ai-0.1.0/lemon_ai/get_integrations.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1291 2023-06-22 18:55:28.000000 lemon-ai-0.1.0/lemon_ai/lemon_ai.py
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-22 20:19:35.248296 lemon-ai-0.1.0/lemon_ai.egg-info/
--rw-r--r--   0 aah120    (1000) aah120    (1000)      725 2023-06-22 20:19:34.000000 lemon-ai-0.1.0/lemon_ai.egg-info/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)      358 2023-06-22 20:19:34.000000 lemon-ai-0.1.0/lemon_ai.egg-info/SOURCES.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-22 20:19:34.000000 lemon-ai-0.1.0/lemon_ai.egg-info/dependency_links.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-22 20:19:34.000000 lemon-ai-0.1.0/lemon_ai.egg-info/requires.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-22 20:19:34.000000 lemon-ai-0.1.0/lemon_ai.egg-info/top_level.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-22 20:19:35.297922 lemon-ai-0.1.0/setup.cfg
--rw-r--r--   0 aah120    (1000) aah120    (1000)      853 2023-06-22 20:19:05.000000 lemon-ai-0.1.0/setup.py
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 10:26:46.510068 lemon-ai-0.1.2/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1076 2023-06-22 18:20:13.000000 lemon-ai-0.1.2/LICENSE
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-26 10:26:46.502687 lemon-ai-0.1.2/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        0 2023-06-26 10:11:43.000000 lemon-ai-0.1.2/README.md
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 10:26:46.199253 lemon-ai-0.1.2/lemon_ai/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      109 2023-06-26 10:26:00.000000 lemon-ai-0.1.2/lemon_ai/__init__.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1741 2023-06-23 11:04:03.000000 lemon-ai-0.1.2/lemon_ai/cito_api_wrapper.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      840 2023-06-23 09:17:19.000000 lemon-ai-0.1.2/lemon_ai/cito_tool.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     5309 2023-06-23 11:35:50.000000 lemon-ai-0.1.2/lemon_ai/cito_toolkit.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      609 2023-06-23 08:27:59.000000 lemon-ai-0.1.2/lemon_ai/cito_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1654 2023-06-26 08:56:26.000000 lemon-ai-0.1.2/lemon_ai/execute_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      822 2023-06-23 08:58:16.000000 lemon-ai-0.1.2/lemon_ai/get_integrations.py
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 10:26:46.438956 lemon-ai-0.1.2/lemon_ai.egg-info/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-26 10:26:43.000000 lemon-ai-0.1.2/lemon_ai.egg-info/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      366 2023-06-26 10:26:43.000000 lemon-ai-0.1.2/lemon_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-26 10:26:43.000000 lemon-ai-0.1.2/lemon_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-26 10:26:43.000000 lemon-ai-0.1.2/lemon_ai.egg-info/requires.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-26 10:26:43.000000 lemon-ai-0.1.2/lemon_ai.egg-info/top_level.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-26 10:26:46.510068 lemon-ai-0.1.2/setup.cfg
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      852 2023-06-26 10:26:04.000000 lemon-ai-0.1.2/setup.py
```

### Comparing `lemon-ai-0.1.0/LICENSE` & `lemon-ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.0/PKG-INFO` & `lemon-ai-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lemon-ai
-Version: 0.1.0
-Summary: A Python client that enables Langchain agents to design, and execute workflow automations targeting internal tooling
+Version: 0.1.2
+Summary: A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling
 Home-page: https://github.com/feliciori/lemon-ai-client-python
 Author: Felix Brockmeier
 Author-email: felix@citodata.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lemon-ai-0.1.0/lemon_ai/cito_api_wrapper.py` & `lemon-ai-0.1.2/lemon_ai/cito_api_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,32 @@
         return response.json()
     
     def _get_action_request(
         self, id: str, action_input: str, params: Optional[Dict]
     ) -> Request:
         
         data = params if params else {}
-        json_obj = json.loads(action_input.replace("'", "\""))
+        if action_input[-1] == ":":
+            action_input = action_input + "\"\""
+        json_obj = json.loads(action_input.replace("'", "\"").replace("None", "\"\""))
 
         data.update(json_obj)
 
         return Request(
             method="POST",
             url=f"{self.api_base_url}tool/{id}/execute",
             json=data,
         )
 
-    def run(self, id: str, action_input: str, params: Optional[Dict], api_key: Optional[str]) -> Dict:
+    def run(self, id: str, action_input: str, params: Optional[Dict], api_key: Optional[str], access_token: Optional[str]) -> Dict:
         
         session = self._get_session()
-        if api_key:
-            session.params = {"api_key": api_key}
-
         request = self._get_action_request(id, action_input, params)
 
+        if api_key:
+            request.json["authToken"] = api_key
+        elif access_token:
+            request.json["authToken"] = access_token
+
         response = session.send(session.prepare_request(request))
         response.raise_for_status()
         return response.json()
```

### Comparing `lemon-ai-0.1.0/lemon_ai/cito_tool.py` & `lemon-ai-0.1.2/lemon_ai/cito_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from langchain.tools import BaseTool
 from pydantic import Field
-from .cito_api_wrapper import CitoAPIWrapper
+from lemon_ai.cito_api_wrapper import CitoAPIWrapper
 from typing import Dict, Optional
 from loguru._logger import Logger
 
 class CitoTool(BaseTool):
 
     api_wrapper: CitoAPIWrapper = Field(default_factory=CitoAPIWrapper)
     id: str = ""
     name: str = ""
     description: str = ""
     params: Optional[Dict] = None
     api_key: Optional[str] = None
+    access_token: Optional[str] = None
     logger: Logger
     session_id: str
 
     def _run(self, action_input: str) -> Dict:
         
         self.logger.bind(session_id=self.session_id, operation_name=self.name).info("")
-        return self.api_wrapper.run(self.id, action_input, self.params, self.api_key)
+        return self.api_wrapper.run(self.id, action_input, self.params, self.api_key, self.access_token)
 
     async def _arun(self):
         raise NotImplementedError("Cito Tool does not support async")
```

### Comparing `lemon-ai-0.1.0/lemon_ai/cito_toolkit.py` & `lemon-ai-0.1.2/lemon_ai/cito_toolkit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import os
 import json
 from langchain.agents.agent_toolkits.base import BaseToolkit
-from .cito_api_wrapper import CitoAPIWrapper
-from .cito_tool import CitoTool
-from .cito_workflow import CitoWorkflow
-from typing import List, Dict, Optional, Union
+from lemon_ai.cito_api_wrapper import CitoAPIWrapper
+from lemon_ai.cito_tool import CitoTool
+from lemon_ai.cito_workflow import CitoWorkflow
+from typing import List, Dict, Optional, Union, Tuple
 from loguru._logger import Logger
 
 class CitoToolkit(BaseToolkit):
 
     tools: List[Union[CitoTool, CitoWorkflow]] = []
 
-    def _get_api_key(self, api_key_dict: Dict[str, str], action_id: str) -> Optional[str]:
+    def _get_access_variable(self, api_key_dict: Dict[str, str], access_token_dict: Dict[str, str], action_id: str) -> Tuple[Optional[str], Optional[str]]:
         api_key = None
+        access_token = None
 
         for key in api_key_dict:
             if key in action_id:
                 api_key = api_key_dict[key]
         
-        return api_key
+        for key in access_token_dict:
+            if key in action_id:
+                access_token = access_token_dict[key]
+    
+        return api_key, access_token
     
     def _get_workflows_from_file(tools_list: List[CitoTool], logger: Logger, session_id: str) -> List[CitoWorkflow]:
         workflows = []
 
         with open("workflow.json", "r") as file:
             data = json.load(file)
             tool_ids_list = [tool.id for tool in tools_list]
@@ -56,41 +61,43 @@
         return f"A wrapper around Lemon AI workflows. To run this workflow, run each tool in the workflow's tools list in the correct order to achieve the goal given by the workflow's description. You MUST take into account the params when executing each stage of the workflow. Sometimes, but not always, the output from a tool in the workflow may need to be used as the param for another tool in the workflow. For example, if the workflow's description is \"send the latest weather information in an email to mohammed@citodata.com\", first you would need to retrieve the latest weather information using one tool and then send that tool's output in an email to the given recipient, using the weather information as a param for the tool to send the email. You MUST use every tool that is given in the workflow's tools list once and in the same order as the list. Do not make up params, they will be explicitly specified in each tool's description. Do not use any tools that are not in this workflow's tools list. If you do not have enough information to fill in the params for a tool, just say 'not enough information provided in the instruction, missing <param>'. If you get a null or none response, STOP EXECUTION, do not try another tool! This workflow is named:{name} and has the goal:{description} and this workflow's tools list is: {tool_names}" 
 
     @classmethod
     def from_cito_api_wrapper(
         cls,
         api_wrapper: CitoAPIWrapper,
         api_keys_dict: Dict[str, str],
+        access_tokens_dict: Dict[str, str],
         logger: Logger,
         session_id: str,
     ) -> "CitoToolkit":
         
         actions = api_wrapper.get_tool_list()
 
         cito_tools = []
 
         for action in actions:
-            if action["isPublic"]:
+            if action["authorizationType"] == "none":
                 cito_tools.append(CitoTool(
                     id=action["id"],
                     name=action["name"],
                     description=action["description"],
                     api_wrapper=api_wrapper,
                     logger=logger,
                     session_id=session_id
                 ))
             else:
-                api_key = cls._get_api_key(cls, api_keys_dict, action["id"])
-                if api_key:
+                api_key, access_token = cls._get_access_variable(cls, api_keys_dict, access_tokens_dict, action["id"])
+                if api_key or access_token:
                     cito_tools.append(CitoTool(
                         id=action["id"],
                         name=action["name"],
                         description=action["description"],
                         api_wrapper=api_wrapper,
                         api_key=api_key,
+                        access_token=access_token,
                         logger=logger,
                         session_id=session_id
                     ))
         
         if os.path.exists("workflow.json"):
             workflows = cls._get_workflows_from_file(cito_tools, logger, session_id)
             cito_tools.extend(workflows)
```

### Comparing `lemon-ai-0.1.0/lemon_ai/cito_workflow.py` & `lemon-ai-0.1.2/lemon_ai/cito_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from langchain.tools import BaseTool
-from .cito_tool import CitoTool
+from lemon_ai.cito_tool import CitoTool
 from typing import List
 from loguru._logger import Logger
 
 class CitoWorkflow(BaseTool):
 
     name: str = ""
     description: str = ""
```

### Comparing `lemon-ai-0.1.0/lemon_ai/lemon_ai.py` & `lemon-ai-0.1.2/lemon_ai/execute_workflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import uuid
 from loguru import logger
 from langchain.llms.base import BaseLLM
 from langchain.agents import initialize_agent, AgentType
-from .get_integrations import get_apis_from_env
-from .cito_api_wrapper import CitoAPIWrapper
-from .cito_toolkit import CitoToolkit
+from lemon_ai.get_integrations import get_apis_from_env
+from lemon_ai.cito_api_wrapper import CitoAPIWrapper
+from lemon_ai.cito_toolkit import CitoToolkit
 
-def create_workflow(llm: BaseLLM):
+def execute_workflow(llm: BaseLLM, prompt_string: str):
 
     logfile_path = "output.log"
     logger.remove(handler_id=None)
     logger.add(logfile_path, format="{time} - {extra[session_id]} - {extra[operation_name]} - {message}")
 
-    tools_dict = get_apis_from_env()
+    api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
     cito_wrapper = CitoAPIWrapper()
-    toolkit = CitoToolkit.from_cito_api_wrapper(cito_wrapper, tools_dict, logger, str(session_id))
+    toolkit = CitoToolkit.from_cito_api_wrapper(cito_wrapper, api_keys_dict, access_tokens_dict, logger, str(session_id))
     tools = toolkit.get_tools()
 
     agent = initialize_agent(
         tools=tools,
         llm=llm,
         agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION, 
         verbose=True
     )
 
-    prompt = input("Enter your task: ") + ". Give your action input in a JSON format where the keys are the params \
-        and the values are the value for each input parameter. Your final answer should summarise what you did and the result."
+    prompt = prompt_string + ". Give your action input as a valid JSON object where the keys are the params \
+        and the values are the value for each input parameter. If you do not know the value of a param, use \"\". If a param \
+        is optional and you have not been given a value, do not include that field in the JSON object. Your final answer should give \
+        a brief conversational overview of what you did and then give a brief conversational description of the content of the result's values."
     answer = agent.run(prompt)
 
     logger.remove()
     logger.add(logfile_path, format="{time} - {extra[session_id]} - {message}")
     logger.bind(session_id=session_id).info(answer)
```

### Comparing `lemon-ai-0.1.0/lemon_ai.egg-info/PKG-INFO` & `lemon-ai-0.1.2/lemon_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lemon-ai
-Version: 0.1.0
-Summary: A Python client that enables Langchain agents to design, and execute workflow automations targeting internal tooling
+Version: 0.1.2
+Summary: A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling
 Home-page: https://github.com/feliciori/lemon-ai-client-python
 Author: Felix Brockmeier
 Author-email: felix@citodata.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lemon-ai-0.1.0/setup.py` & `lemon-ai-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lemon-ai',
-    version='0.1.0',    
-    description='A Python client that enables Langchain agents to design, and execute workflow automations targeting internal tooling',
+    version='0.1.2',    
+    description='A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling',
     author='Felix Brockmeier',
     author_email='felix@citodata.com',
     url="https://github.com/feliciori/lemon-ai-client-python",
     license='MIT',
     packages=['lemon_ai'],
     python_requires='>=3.8.1',
     install_requires=[
```

