# Comparing `tmp/comet_llm-1.0.0.tar.gz` & `tmp/comet_llm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-1.0.0.tar", last modified: Thu Jun  8 15:09:33 2023, max compression
+gzip compressed data, was "comet_llm-1.0.1.tar", last modified: Mon Jun 26 14:55:55 2023, max compression
```

## Comparing `comet_llm-1.0.0.tar` & `comet_llm-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.932143 comet_llm-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 15:09:16.000000 comet_llm-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-08 15:09:33.932143 comet_llm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-08 15:09:16.000000 comet_llm-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:09:33.932143 comet_llm-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-08 15:09:16.000000 comet_llm-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.932143 comet_llm-1.0.0/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:55:55.574812 comet_llm-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 14:55:43.000000 comet_llm-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-26 14:55:55.574812 comet_llm-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-26 14:55:43.000000 comet_llm-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:55:55.574812 comet_llm-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 14:55:43.000000 comet_llm-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:55:55.566811 comet_llm-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:55:55.570811 comet_llm-1.0.1/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:55:55.574812 comet_llm-1.0.1/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/experiment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/logs_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-26 14:55:43.000000 comet_llm-1.0.1/src/comet_llm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:55:55.570811 comet_llm-1.0.1/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:55:55.000000 comet_llm-1.0.1/src/comet_llm.egg-info/top_level.txt
```

### Comparing `comet_llm-1.0.0/LICENSE` & `comet_llm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/PKG-INFO` & `comet_llm-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_llm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: comet_llm Version: 1.0.0 Summary: Comet logger for
+Metadata-Version: 2.1 Name: comet_llm Version: 1.0.1 Summary: Comet logger for
 LLM Home-page: https://www.comet.com Author: Comet ML Inc. Author-email:
 mail@comet.com License: MIT Project-URL: Source code, https://github.com/comet-
 ml/comet-llm Keywords: comet_llm Classifier: Development Status :: 2 - Pre-
 Alpha Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `comet_llm-1.0.0/README.md` & `comet_llm-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     api_key="<YOUR_COMET_API_KEY>",
 )
 ```
 
 ## 🎯 Features
 
 - [x] Log your prompts and responses, including prompt template, variables, timestamps and duration and any metadata that you need.
-- [ ] Visualize your prompts and responses in the UI.
+- [x] Visualize your prompts and responses in the UI.
 - [ ] Log your chain execution down to the level of granularity that you need.
 - [ ] Visualize your chain execution in the UI.
 - [ ] Diff your prompts and chain execution in the UI.
 
 ## 👀 Examples
 
 ### Log a full prompt and response
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 install comet_llm ``` If you don't have already, [create your free Comet
 account](https://www.comet.com/signup/
 ?utm_source=comet_llm&utm_medium=referral&utm_content=github) and grab your API
 Key from the account settings page. Now you are all set to log your first
 prompt and response: ```python import comet_llm comet_llm.log_prompt
 ( prompt="What is your name?", output=" My name is Alex.", api_key="", ) ``` ##
 ð¯ Features - [x] Log your prompts and responses, including prompt template,
-variables, timestamps and duration and any metadata that you need. - [ ]
+variables, timestamps and duration and any metadata that you need. - [x]
 Visualize your prompts and responses in the UI. - [ ] Log your chain execution
 down to the level of granularity that you need. - [ ] Visualize your chain
 execution in the UI. - [ ] Diff your prompts and chain execution in the UI. ##
 ð Examples ### Log a full prompt and response ```python import comet_llm
 comet_llm.log_prompt( prompt="Answer the question and if the question can't be
 answered, say \"I don't know\"\n\n---\n\nQuestion: What is your name?\nAnswer:
 ", prompt_template="Answer the question and if the question can't be answered,
```

### Comparing `comet_llm-1.0.0/setup.py` & `comet_llm-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.com",
     project_urls=project_urls,
-    version="1.0.0",
+    version="1.0.1",
     zip_safe=False,
     license="MIT",
 )
```

### Comparing `comet_llm-1.0.0/src/comet_llm/__init__.py` & `comet_llm-1.0.1/src/comet_llm/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,10 +7,11 @@
 #  \____\___/|_| |_| |_|\___|\__(_)_| |_| |_|_|
 #
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
-from .api import log_prompt
 
-__all__ = ["log_prompt"]
+from typing import Any
+
+JSONEncodable = Any
```

### Comparing `comet_llm-1.0.0/src/comet_llm/api.py` & `comet_llm-1.0.1/src/comet_llm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import io
 import json
-from typing import Dict, Optional, Union
+from typing import Dict, List, Optional, Union
 
-from . import convert, experiment_api, experiment_info, preprocess
+from . import app, convert, experiment_api, experiment_info, preprocess
 
 ASSET_FORMAT_VERSION = 3
 
 
 def log_prompt(
     prompt: str,
     output: str,
     workspace: Optional[str] = None,
     project: Optional[str] = None,
+    tags: Optional[List[str]] = None,
     api_key: Optional[str] = None,
     prompt_template: Optional[str] = None,
     prompt_template_variables: Optional[
         Dict[str, Union[str, bool, float, None]]
     ] = None,
     metadata: Optional[Dict[str, Union[str, bool, float, None]]] = None,
     timestamp: Optional[float] = None,
@@ -39,14 +40,15 @@
     Logs a single prompt and output to Comet platform.
 
     Args:
         prompt: str (required) input prompt to LLM.
         output: str (required), output from LLM.
         workspace: str (optional) comet workspace to use for logging.
         project: str (optional) project name to create in comet workspace.
+        tags: List[str] (optional), user-defined tags attached to a prompt call.
         api_key: str (optional) comet API key.
         prompt_template: str (optional) user-defined template used for creating a prompt.
         prompt_template_variables: Dict[str, str] (optional) dictionary with data used
             in prompt_template to build a prompt.
         metadata: Dict[str, Union[str, bool, float, None]] (optional) user-defined
             dictionary with additional metadata to the call.
         timestamp: float (optional) timestamp of prompt call in seconds
@@ -124,14 +126,19 @@
 
     experiment_api_.log_asset_with_io(
         name="comet_llm_data.json",
         file=io.StringIO(json.dumps(asset_data)),
         asset_type="llm_data",
     )
 
+    if tags is not None:
+        experiment_api_.log_tags(tags)
+
     if duration is not None:
         experiment_api_.log_metric("chain_duration", duration)
 
     parameters = convert.chain_metadata_to_flat_parameters(metadata)
 
     for name, value in parameters.items():
         experiment_api_.log_parameter(name, value)
+
+    app.SUMMARY.add_log(experiment_api_.project_link)
```

### Comparing `comet_llm-1.0.0/src/comet_llm/config.py` & `comet_llm-1.0.1/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/convert.py` & `comet_llm-1.0.1/src/comet_llm/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/datetimes.py` & `comet_llm-1.0.1/src/comet_llm/datetimes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/exceptions.py` & `comet_llm-1.0.1/src/comet_llm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/experiment_api/__init__.py` & `comet_llm-1.0.1/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-1.0.1/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 import functools
-import sys
 import urllib.parse
-from typing import IO, Optional
+from typing import IO, List, Optional
 
 import requests  # type: ignore
 
 from .. import config
 from ..types import JSONEncodable
 from . import request_exception_wrapper
 
@@ -87,14 +86,23 @@
                 "fileName": name,
                 "extension": extension,
                 "type": asset_type,
             },
             files={"file": file},
         )
 
+    def log_experiment_tags(
+        self, experiment_key: str, tags: List[str]
+    ) -> ResponseContent:
+        return self._request(
+            "POST",
+            "/api/rest/v2/write/experiment/tags",
+            json={"experimentKey": experiment_key, "addedTags": tags},
+        )
+
     @request_exception_wrapper.wrap
     def _request(self, method: str, path: str, *args, **kwargs) -> ResponseContent:  # type: ignore
         url = urllib.parse.urljoin(self._comet_url, path)
         response = requests.request(method, url, headers=self._headers, *args, **kwargs)
         response.raise_for_status()
         return response.json()
```

### Comparing `comet_llm-1.0.0/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-1.0.1/src/comet_llm/experiment_api/experiment_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,40 +8,56 @@
 #
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
-from typing import IO, Any, Optional
+from typing import IO, Any, List, Optional
 
 from . import comet_api_client
 
 
 class ExperimentAPI:
     def __init__(
         self,
         api_key: str,
         workspace: Optional[str],
         project_name: Optional[str],
     ):
         self._client = comet_api_client.get(api_key)
         self._initialize_experiment(workspace, project_name)
 
+    @property
+    def link(self) -> str:
+        return self._link
+
+    @property
+    def project_link(self) -> str:
+        return self._project_link
+
     def _initialize_experiment(
         self, workspace: Optional[str] = None, project_name: Optional[str] = None
     ) -> None:
         response = self._client.create_experiment("LLM", workspace, project_name)
         self._experiment_key = response["experimentKey"]
+        self._initialize_links(response["link"])
+
+    def _initialize_links(self, link: str) -> None:
+        self._link = link
+        self._project_link = link[: link.rfind("/")]
 
     def log_asset_with_io(self, name: str, file: IO, asset_type: str) -> None:
         self._client.log_experiment_asset_with_io(
             self._experiment_key, name=name, file=file, asset_type=asset_type
         )
 
     def log_parameter(self, name: str, value: Any) -> None:
         self._client.log_experiment_parameter(
             self._experiment_key, name=name, value=value
         )
 
     def log_metric(self, name: str, value: Any) -> None:
         self._client.log_experiment_metric(self._experiment_key, name=name, value=value)
+
+    def log_tags(self, tags: List[str]) -> None:
+        self._client.log_experiment_tags(self._experiment_key, tags=tags)
```

### Comparing `comet_llm-1.0.0/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-1.0.1/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/experiment_info.py` & `comet_llm-1.0.1/src/comet_llm/experiment_info.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/preprocess.py` & `comet_llm-1.0.1/src/comet_llm/preprocess.py`

 * *Files identical despite different names*

### Comparing `comet_llm-1.0.0/src/comet_llm/types.py` & `comet_llm-1.0.1/src/comet_llm/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,10 +8,13 @@
 #
 #  Sign up for free at https://www.comet.com
 #  Copyright (C) 2015-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
-from typing import Any
+from . import app, logging
+from .api import log_prompt
 
-JSONEncodable = Any
+__all__ = ["log_prompt"]
+
+logging.setup()
```

### Comparing `comet_llm-1.0.0/src/comet_llm.egg-info/PKG-INFO` & `comet_llm-1.0.1/src/comet_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet-llm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Comet logger for LLM
 Home-page: https://www.comet.com
 Author: Comet ML Inc.
 Author-email: mail@comet.com
 License: MIT
 Project-URL: Source code, https://github.com/comet-ml/comet-llm
 Keywords: comet_llm
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: comet-llm Version: 1.0.0 Summary: Comet logger for
+Metadata-Version: 2.1 Name: comet-llm Version: 1.0.1 Summary: Comet logger for
 LLM Home-page: https://www.comet.com Author: Comet ML Inc. Author-email:
 mail@comet.com License: MIT Project-URL: Source code, https://github.com/comet-
 ml/comet-llm Keywords: comet_llm Classifier: Development Status :: 2 - Pre-
 Alpha Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `comet_llm-1.0.0/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-1.0.1/src/comet_llm.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE
 README.md
 setup.py
 src/comet_llm/__init__.py
 src/comet_llm/api.py
+src/comet_llm/app.py
 src/comet_llm/config.py
 src/comet_llm/convert.py
 src/comet_llm/datetimes.py
 src/comet_llm/exceptions.py
 src/comet_llm/experiment_info.py
+src/comet_llm/logging.py
+src/comet_llm/logs_registry.py
 src/comet_llm/preprocess.py
+src/comet_llm/summary.py
 src/comet_llm/types.py
 src/comet_llm.egg-info/PKG-INFO
 src/comet_llm.egg-info/SOURCES.txt
 src/comet_llm.egg-info/dependency_links.txt
 src/comet_llm.egg-info/not-zip-safe
 src/comet_llm.egg-info/requires.txt
 src/comet_llm.egg-info/top_level.txt
```

