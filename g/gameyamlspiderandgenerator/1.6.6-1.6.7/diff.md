# Comparing `tmp/gameyamlspiderandgenerator-1.6.6.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.6.6.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.7.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.6.6.tar` & `gameyamlspiderandgenerator-1.6.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-06-17 07:02:01.936469 gameyamlspiderandgenerator-1.6.6/LICENSE
--rwxr-xr-x   0        0        0     1446 2023-06-20 08:26:16.341618 gameyamlspiderandgenerator-1.6.6/README.md
--rwxr-xr-x   0        0        0      568 2023-06-17 07:02:01.937320 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1888 2023-06-20 09:36:24.142803 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      675 2023-06-17 07:02:01.937746 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-06-17 07:02:01.938073 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-06-17 07:02:01.938303 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0       56 2023-06-17 07:02:01.939367 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-20 08:55:31.013097 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7088 2023-06-17 07:02:01.939929 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-06-17 07:02:01.940217 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-06-17 07:02:01.940509 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-06-17 07:02:01.940795 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1816 2023-06-20 09:35:26.330476 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-06-17 07:02:01.941257 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2846 2023-06-20 09:36:24.047081 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-20 07:58:45.635538 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-06-17 07:02:01.942014 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      766 2023-06-20 09:36:44.110154 gameyamlspiderandgenerator-1.6.6/pyproject.toml
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0      765 2023-06-25 16:16:10.833751 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/__init__.py
+-rw-r--r--   0        0        0     2115 2023-06-26 00:33:51.351086 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/__main__.py
+-rw-r--r--   0        0        0      697 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/exception.py
+-rw-r--r--   0        0        0       55 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/hook/__init__.py
+-rw-r--r--   0        0        0      250 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/hook/_base.py
+-rw-r--r--   0        0        0       59 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/__init__.py
+-rw-r--r--   0        0        0     3338 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/_base.py
+-rw-r--r--   0        0        0     7292 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/itchio.py
+-rw-r--r--   0        0        0     8377 2023-06-26 00:32:26.718760 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/steam.py
+-rw-r--r--   0        0        0        0 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/__init__.py
+-rw-r--r--   0        0        0     1519 2023-06-25 14:53:54.816056 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/config.py
+-rw-r--r--   0        0        0     1880 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/fgi.py
+-rw-r--r--   0        0        0     2019 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rw-r--r--   0        0        0     2930 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/plugin_manager.py
+-rw-r--r--   0        0        0     2659 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/spider.py
+-rw-r--r--   0        0        0      276 2023-06-25 12:57:35.392003 gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/thread.py
+-rw-r--r--   0        0        0     1090 2023-06-25 12:57:35.376378 gameyamlspiderandgenerator-1.6.7/LICENSE
+-rw-r--r--   0        0        0      801 2023-06-26 00:41:27.387865 gameyamlspiderandgenerator-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-06-25 12:57:35.376378 gameyamlspiderandgenerator-1.6.7/README.md
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.7/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.6.6/LICENSE` & `gameyamlspiderandgenerator-1.6.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 开普以尔
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 开普以尔
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `gameyamlspiderandgenerator-1.6.6/README.md` & `gameyamlspiderandgenerator-1.6.7/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# Quick Start
-## Install
-```commandline
-pip install gameyamlspiderandgenerator -i https://pypi.org/simple
-# install extra hook
-# pip install yamlgenerator-hook-openai
-python3.10
-```
-## Create a new configuration file
-- config.yaml
-```yaml
-plugin:
-  - steam
-  - itchio
-hook:
-  - search
-  - validate
-# - openai
-# if you don't want to set proxy, please fill in {}
-proxy: { }
-# http: socks5://127.0.0.1:7891
-# https: socks5://127.0.0.1:7891
-gitToken: 'your token'
-api:
-  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90 # Get your api key via serpapi.com
-  apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
-  openai: yourkey
-
-```
-## Try to make yaml data file
-```bash
- python3.10 -m gameyamlspiderandgenerator -f /home/user/desktop/config.yaml  https://store.steampowered.com/app/290340/Armello/ -o 1.zip
- # or omit some options
- python3.10 -m gameyamlspiderandgenerator https://store.steampowered.com/app/290340/Armello/
-
-```
-*or use the library in your script*
-```python
-from gameyamlspiderandgenerator import produce_yaml
-from gameyamlspiderandgenerator.util.config import config
-from gameyamlspiderandgenerator.util.plugin_manager import pkg
-
-config.load("/home/user/desktop/config.yaml")
-pkg.__init__()
-print(produce_yaml("https://store.steampowered.com/app/1470120/Atopes/"))
-```
-
-### More: see [API Reference](https://github.com/FurryGamesIndex/GameYamlSpiderAndGenerator/wiki/Api-Reference)
+# Quick Start
+## Install
+```commandline
+pip install gameyamlspiderandgenerator -i https://pypi.org/simple
+# install extra hook
+# pip install yamlgenerator-hook-openai
+python3.10
+```
+## Create a new configuration file
+- config.yaml
+```yaml
+plugin:
+  - steam
+  - itchio
+hook:
+  - search
+  - validate
+# - openai
+# if you don't want to set proxy, please fill in {}
+proxy: { }
+# http: socks5://127.0.0.1:7891
+# https: socks5://127.0.0.1:7891
+gitToken: 'your token'
+api:
+  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90 # Get your api key via serpapi.com
+  apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
+  openai: yourkey
+
+```
+## Try to make yaml data file
+```bash
+ python3.10 -m gameyamlspiderandgenerator -f /home/user/desktop/config.yaml  https://store.steampowered.com/app/290340/Armello/ -o 1.zip
+ # or omit some options
+ python3.10 -m gameyamlspiderandgenerator https://store.steampowered.com/app/290340/Armello/
+
+```
+*or use the library in your script*
+```python
+from gameyamlspiderandgenerator import produce_yaml
+from gameyamlspiderandgenerator.util.config import config
+from gameyamlspiderandgenerator.util.plugin_manager import pkg
+
+config.load("/home/user/desktop/config.yaml")
+pkg.__init__()
+print(produce_yaml("https://store.steampowered.com/app/1470120/Atopes/"))
+```
+
+### More: see [API Reference](https://github.com/FurryGamesIndex/GameYamlSpiderAndGenerator/wiki/Api-Reference)
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from typing import Optional
-
-from loguru import logger
-
-from .plugin import BasePlugin
-from .util.fgi_yaml import YamlData
-from .util.plugin_manager import pkg
-
-
-def verify(url: str):
-    verify_list = [
-        [
-            pkg.plugin[n].verify,
-            pkg.plugin[n],
-        ]
-        for n in pkg.plugin
-    ]
-    return next((cls for func, cls in verify_list if func(url)), None)
-
-
-def produce_yaml(url: str) -> Optional[YamlData]:
-    ret = verify(url)
-    if ret is None:
-        logger.error("URL is invalid")
-        return
-    return ret(url).to_yaml()
+from typing import Optional
+from inspect import signature
+from loguru import logger
+
+from .plugin import BasePlugin
+from .util.fgi_yaml import YamlData
+from .util.plugin_manager import pkg
+
+
+def verify(url: str):
+    verify_list = [
+        [
+            pkg.plugin[n].verify,
+            pkg.plugin[n],
+        ]
+        for n in pkg.plugin
+    ]
+    return next((cls for func, cls in verify_list if func(url)), None)
+
+
+def produce_yaml(url: str, lang:str="en") -> Optional[YamlData]:
+    ret = verify(url)
+    if ret is None:
+        logger.error("URL is invalid")
+        return
+    if 'lang' in [i.name for i in signature(ret).parameters.values()]:
+        return ret(url,lang).to_yaml()
+    else:
+        return ret(url).to_yaml()
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,74 @@
-import argparse
-
-from yaml import safe_load
-
-from .util.config import config
-from .util.fgi import default_config
-from .util.fgi_yaml import get_valid_filename
-from .util.plugin_manager import pkg
-from loguru import logger
-from gameyamlspiderandgenerator import produce_yaml
-
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-f",
-    "--config",
-    type=str,
-    default=default_config,
-    help="The location of config.yaml (default null)",
-)
-parser.add_argument(
-    "-o",
-    "--output",
-    type=str,
-    default=None,
-    help="The location of the output file (zip format or yaml format)",
-)
-parser.add_argument(
-    "--fast",
-    action='store_true',
-    default=False,
-    help="Whether to disable all hooks (default: false)",
-)
-parser.add_argument("url", metavar="URL")
-args = parser.parse_args()
-if isinstance(args.config, str):
-    with open(args.config) as f:
-        setting = safe_load(f)
-else:
-    setting = args.config
-if args.fast:
-    setting['hook'] = None
-config.update(setting)
-pkg.__init__()
-yml = produce_yaml(args.url)
-if args.output is None:
-    if yml is not None:
-        print(yml)
-elif "." not in args.output:
-    if args.output == "zip":
-        with open(get_valid_filename(yml.raw_dict['name']) + ".zip", 'wb') as f:
-            f.write(bytes(yml))
-    elif args.output == "yaml":
-        with open(get_valid_filename(yml.raw_dict['name']) + ".yaml", 'w') as f:
-            f.write(str(yml))
-elif "." in args.output:
-    if "zip" in args.output:
-        with open(args.output, 'wb') as f:
-            f.write(bytes(yml))
-    elif "yaml" in args.output:
-        with open(args.output, 'w') as f:
-            f.write(str(yml))
-    else:
-        logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
-        exit(3)
-
-else:
-    logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
-    exit(3)
+import argparse
+
+from yaml import safe_load
+
+from .util.config import config
+from .util.fgi import default_config
+from .util.fgi_yaml import get_valid_filename
+from .util.plugin_manager import pkg
+from loguru import logger
+from gameyamlspiderandgenerator import produce_yaml
+
+parser = argparse.ArgumentParser()
+parser.add_argument(
+    "-f",
+    "--config",
+    type=str,
+    default=default_config,
+    help="The location of config.yaml (default null)",
+)
+parser.add_argument(
+    "-o",
+    "--output",
+    type=str,
+    default=None,
+    help="The location of the output file (zip format or yaml format)",
+)
+parser.add_argument(
+    "--lang",
+    type=str,
+    default='en',
+    help="The display language of the game. ISO 639-1 code(default: en)",
+)
+parser.add_argument(
+    "--fast",
+    action='store_true',
+    default=False,
+    help="Whether to disable all hooks (default: false)",
+)
+parser.add_argument("url", metavar="URL")
+args = parser.parse_args()
+if isinstance(args.config, str):
+    with open(args.config) as f:
+        setting = safe_load(f)
+else:
+    setting = args.config
+if args.fast:
+    setting['hook'] = None
+config.update(setting)
+pkg.__init__()
+yml = produce_yaml(args.url,args.lang)
+if args.output is None:
+    if yml is not None:
+        print(yml)
+elif "." not in args.output:
+    if args.output == "zip":
+        with open(get_valid_filename(yml.raw_dict['name']) + ".zip", 'wb') as f:
+            f.write(bytes(yml))
+    elif args.output == "yaml":
+        with open(get_valid_filename(yml.raw_dict['name']) + ".yaml", 'w') as f:
+            f.write(str(yml))
+elif "." in args.output:
+    if "zip" in args.output:
+        with open(args.output, 'wb') as f:
+            f.write(bytes(yml))
+    elif "yaml" in args.output:
+        with open(args.output, 'w') as f:
+            f.write(str(yml))
+    else:
+        logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
+        exit(3)
+
+else:
+    logger.error(f"unsupported file format: {args.output[args.output.rfind('.'):]}")
+    exit(3)
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/exception.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-class InitializeFailed(Exception):
-    def __init__(self):
-        super().__init__("Failed to initialize")
-
-
-class ReadOrWriteConfigFailed(Exception):
-    def __init__(self):
-        super().__init__("Failed to read or write config")
-
-
-class InvalidTargetResourceError(Exception):
-    def __init__(self, code: int):
-        super().__init__(f"The target resource is no longer valid.status code: {code}")
-
-
-class ResponseNotInitialized(Exception):
-    def __init__(self, url: str):
-        super().__init__(f"Response not initialized, url: {url}")
-
-
-class InvalidResponse(Exception):
-    def __init__(self, url: str):
+class InitializeFailed(Exception):
+    def __init__(self):
+        super().__init__("Failed to initialize")
+
+
+class ReadOrWriteConfigFailed(Exception):
+    def __init__(self):
+        super().__init__("Failed to read or write config")
+
+
+class InvalidTargetResourceError(Exception):
+    def __init__(self, code: int):
+        super().__init__(f"The target resource is no longer valid.status code: {code}")
+
+
+class ResponseNotInitialized(Exception):
+    def __init__(self, url: str):
+        super().__init__(f"Response not initialized, url: {url}")
+
+
+class InvalidResponse(Exception):
+    def __init__(self, url: str):
         super().__init__(f"Invalid response, url: {url}")
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/_base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-import abc
-import re
-from typing import List
-
-from ..util.fgi_yaml import YamlData
-from ..util.thread import ThreadWithReturnValue
-
-
-class BasePlugin(abc.ABC):
-    """插件基类"""
-
-    _VERIFY_PATTERN: re.Pattern
-
-    @classmethod
-    def verify(cls, url: str) -> bool:
-        """
-        验证 URL 是否符合插件的要求
-
-        Args:
-            url: URL
-
-        Returns:
-            是否符合要求
-        """
-        return bool(cls._VERIFY_PATTERN.match(url))
-
-    @staticmethod
-    def __load_hook__(data: dict):
-        """
-        加载钩子
-
-        Args:
-            data: 钩子数据
-        """
-        from gameyamlspiderandgenerator.util.plugin_manager import pkg
-        pkg.__init__()
-
-        def get_fn_address():
-            fn_: list = []
-            for i in pkg.hook.values():
-                fn_.append([i().setup, i.CHANGED])
-            return fn_
-
-        fn = get_fn_address()
-        fn_list = [(ThreadWithReturnValue(target=i, args=(data,)), _) for i, _ in fn]
-        for i, _ in fn_list:
-            i.start()
-        result = [(ii.join(), changed) for ii, changed in fn_list]
-        for _data, changed in result:
-            if changed is not None:
-                for i in changed:
-                    data[i] = _data[i]
-        return data
-
-    @abc.abstractmethod
-    def get_name(self) -> str:
-        """
-        获取游戏名称
-
-        Returns:
-            游戏名称
-        """
-
-    @abc.abstractmethod
-    def get_desc(self) -> str:
-        """
-        获取游戏描述
-
-        Returns:
-            游戏描述
-        """
-
-    @abc.abstractmethod
-    def get_brief_desc(self) -> str:
-        """
-        获取游戏简介
-
-        Returns:
-            游戏简介
-        """
-
-    @abc.abstractmethod
-    def get_thumbnail(self) -> str:
-        """
-        获取游戏封面
-
-        Returns:
-            游戏封面
-        """
-
-    @abc.abstractmethod
-    def get_authors(self) -> List[dict]:
-        """
-        获取游戏作者
-
-        Returns:
-            游戏作者
-        """
-
-    @abc.abstractmethod
-    def get_tags(self) -> List[dict]:
-        """
-        获取游戏标签
-
-        Returns:
-            游戏标签
-        """
-
-    @abc.abstractmethod
-    def get_misc_tags(self) -> List[dict]:
-        """
-        获取游戏其他标签
-
-        Returns:
-            游戏其他标签
-        """
-
-    @abc.abstractmethod
-    def get_platforms(self) -> List[str]:
-        """
-        获取游戏平台
-
-        Returns:
-            游戏平台
-        """
-
-    @abc.abstractmethod
-    def get_langs(self) -> List[str]:
-        """
-        获取游戏语言
-
-        Returns:
-            游戏语言
-        """
-
-    @abc.abstractmethod
-    def get_links(self) -> List[dict]:
-        """
-        获取游戏链接
-
-        Returns:
-            游戏链接
-        """
-
-    @abc.abstractmethod
-    def get_screenshots(self) -> List[str]:
-        """
-        获取游戏截图
-
-        Returns:
-            游戏截图
-        """
-
-    @abc.abstractmethod
-    def to_yaml(self) -> YamlData:
-        """
-        转换为 YAML
-
-        Returns:
-            YAML
-        """
+import abc
+import re
+from typing import List
+
+from ..util.fgi_yaml import YamlData
+from ..util.thread import ThreadWithReturnValue
+
+
+class BasePlugin(abc.ABC):
+    """插件基类"""
+
+    _VERIFY_PATTERN: re.Pattern
+
+    @classmethod
+    def verify(cls, url: str) -> bool:
+        """
+        验证 URL 是否符合插件的要求
+
+        Args:
+            url: URL
+
+        Returns:
+            是否符合要求
+        """
+        return bool(cls._VERIFY_PATTERN.match(url))
+
+    @staticmethod
+    def __load_hook__(data: dict):
+        """
+        加载钩子
+
+        Args:
+            data: 钩子数据
+        """
+        from gameyamlspiderandgenerator.util.plugin_manager import pkg
+        pkg.__init__()
+
+        def get_fn_address():
+            fn_: list = []
+            for i in pkg.hook.values():
+                fn_.append([i().setup, i.CHANGED])
+            return fn_
+
+        fn = get_fn_address()
+        fn_list = [(ThreadWithReturnValue(target=i, args=(data,)), _) for i, _ in fn]
+        for i, _ in fn_list:
+            i.start()
+        result = [(ii.join(), changed) for ii, changed in fn_list]
+        for _data, changed in result:
+            if changed is not None:
+                for i in changed:
+                    data[i] = _data[i]
+        return data
+
+    @abc.abstractmethod
+    def get_name(self) -> str:
+        """
+        获取游戏名称
+
+        Returns:
+            游戏名称
+        """
+
+    @abc.abstractmethod
+    def get_desc(self) -> str:
+        """
+        获取游戏描述
+
+        Returns:
+            游戏描述
+        """
+
+    @abc.abstractmethod
+    def get_brief_desc(self) -> str:
+        """
+        获取游戏简介
+
+        Returns:
+            游戏简介
+        """
+
+    @abc.abstractmethod
+    def get_thumbnail(self) -> str:
+        """
+        获取游戏封面
+
+        Returns:
+            游戏封面
+        """
+
+    @abc.abstractmethod
+    def get_authors(self) -> List[dict]:
+        """
+        获取游戏作者
+
+        Returns:
+            游戏作者
+        """
+
+    @abc.abstractmethod
+    def get_tags(self) -> List[dict]:
+        """
+        获取游戏标签
+
+        Returns:
+            游戏标签
+        """
+
+    @abc.abstractmethod
+    def get_misc_tags(self) -> List[dict]:
+        """
+        获取游戏其他标签
+
+        Returns:
+            游戏其他标签
+        """
+
+    @abc.abstractmethod
+    def get_platforms(self) -> List[str]:
+        """
+        获取游戏平台
+
+        Returns:
+            游戏平台
+        """
+
+    @abc.abstractmethod
+    def get_langs(self) -> List[str]:
+        """
+        获取游戏语言
+
+        Returns:
+            游戏语言
+        """
+
+    @abc.abstractmethod
+    def get_links(self) -> List[dict]:
+        """
+        获取游戏链接
+
+        Returns:
+            游戏链接
+        """
+
+    @abc.abstractmethod
+    def get_screenshots(self) -> List[str]:
+        """
+        获取游戏截图
+
+        Returns:
+            游戏截图
+        """
+
+    @abc.abstractmethod
+    def to_yaml(self) -> YamlData:
+        """
+        转换为 YAML
+
+        Returns:
+            YAML
+        """
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import re
-from contextlib import suppress
-from json import loads
-from bs4 import BeautifulSoup
-from html2text import html2text
-from langcodes import find
-from py3langid import langid, classify
-
-from ._base import BasePlugin
-from ..util.fgi import fgi_dict
-from ..util.fgi_yaml import YamlData, pss_dedent
-from ..util.spider import get_text
-
-
-class ItchIO(BasePlugin):
-    _VERIFY_PATTERN = re.compile(r"https?://.+\.itch\.io/.+")
-
-    @staticmethod
-    def remove_query(s: str):
-        s = re.sub(r"\?t=\d{6,12}", "", s)
-        return s.replace("![]", "![img]")
-
-    def __init__(self, link: str) -> None:
-        self.link = link
-        self.data_html = get_text(link)
-        self.soup = BeautifulSoup(self.data_html, "lxml")
-        self.data = [
-            ii
-            for ii in [
-                loads(i.text)
-                for i in self.soup.find_all(
-                    "script", attrs={"type": "application/ld+json"}
-                )
-            ]
-            if "name" in ii
-        ][0]
-        self.more_info = self.get_more_info()
-        self.tag = self.get_tags()
-
-    def get_thumbnail(self):
-        th = self.soup.select_one("#header > img")
-        if th is None:
-            return None
-        return th.attrs["src"]
-
-    def get_brief_desc(self):
-        return self.soup.find("meta", {"name": "twitter:description"}).attrs["content"]
-
-    def get_name(self):
-        return self.data["name"]
-
-    def get_screenshots(self):
-        temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
-        return [i.attrs['href'] for i in temp]
-
-    def get_desc(self):
-        return pss_dedent(self.remove_query(html2text(
-            str(self.soup.select_one("div.formatted_description.user_formatted")),
-            bodywidth=0,
-        )).replace("\n" * 3, "\n").strip())
-
-    def get_platforms(self):
-        repl = {
-            "Windows": "windows",
-            "macOS": "macos",
-            "Linux": "linux",
-            "Android": "android",
-            "HTML5": "web",
-            "iOS": "ios",
-        }
-        platforms = self.more_info["Platforms"] if "Platforms" in self.more_info else ["Windows"]
-        return [repl[i.strip()] for i in platforms]
-
-    def get_authors(self) -> list[dict]:
-        temp = []
-        if "Authors" in self.more_info:
-            temp = self.more_info["Authors"]
-        elif "Author" in self.more_info:
-            temp = self.more_info["Author"]
-        return [{"name": i.strip(), "role": ["producer"]} for i in temp]
-
-    def get_tags(self) -> list[str]:
-        temp = self.more_info["Genre"] if "Genre" in self.more_info else []
-        temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
-        temp2 = self.more_info["Tags"] if "Tags" in self.more_info else []
-        return [i.strip() for i in (temp2 + temp1 + temp)]
-
-    def get_misc_tags(self):
-        repl = {
-            "3D": "3d",
-            "Pixel Art": "pixel-art",
-            "free": "freeware",
-            "Multiplayer": "multiplayer",
-            "Co-op": "co-op",
-            "PvP": "pvp",
-            "Ren'Py": "engine-renpy",
-            "Unity": "engine-unity",
-            "RPG Maker": "engine-rpg-maker",
-            "Godot": "engine-godot",
-            "ue4": "engine-ue4",
-            "unreal - engine - 4": "engine-ue4",
-            "TyranoBuilder": "engine-tyranobuilder",
-            "Flash": "adobe-flash",
-            "t-series": "multiple-series",
-            "Multiple Endings": "multiple-endings",
-        }
-
-        ret = []
-        for i, value in repl.items():
-            ret.extend(value for ii in self.tag if i in ii)
-        return list(set(ret))
-
-    def get_langs(self) -> list[str]:
-        if "Languages" in self.more_info:
-            temp = self.more_info["Languages"]
-        else:
-            return [classify(self.get_desc())[0]]
-
-        return list(set(find(i).language for i in temp))
-
-    def get_links(self) -> list[dict]:
-        link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > "
-                                                              "div.formatted_description.user_formatted")
-        .select("a[href]")]
-        data = [{"url": i, "processed": False} for i in list(set(link))]
-        processed_data = []
-        for i in data:
-            for p in fgi_dict:
-                if re.match(p["match"], i["url"]):
-                    processed_data.append(
-                        {
-                            "name": p["prefix"],
-                            "uri": re.sub(p["match"], p["replace"], i["url"]),
-                        }
-                    )
-                    i["processed"] = True
-        for i in data:
-            if not i["processed"]:
-                processed_data.append({"name": ".website", "uri": i["url"]})
-        processed_data.append({"name": ".itchio", "uri": self.link})
-        return processed_data
-
-    def get_more_info(self):
-        d = {}
-        for i in range(1, 18):
-            with suppress(Exception):
-                cache = self.soup.select_one(
-                    f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
-                )
-                temp = [i.get_text() for i in list(cache.children)]
-                d[temp[0]] = temp[1:][0].split(",")
-        return d
-
-    def to_yaml(self) -> YamlData:
-        ret = {
-            "name": self.get_name(),
-            "brief-description": self.get_brief_desc(),
-            "description": self.get_desc(),
-            "description-format": "markdown",
-            "authors": self.get_authors(),
-            "tags": {
-                "type": self.get_type_tag(),
-                "lang": self.get_langs(),
-                "platform": self.get_platforms(),
-                "publish": [".itchio"],
-                "misc": self.get_misc_tags(),
-            },
-            "links": self.get_links(),
-            "thumbnail": self.get_thumbnail(),
-            "screenshots": self.get_screenshots()  # + self.get_video(),
-        }
-        return YamlData(self.__load_hook__(ret))
-
-    def get_type_tag(self):
-        repl = {
-            "Visual Novel": "visual-novel",
-            "Real time strategy": "real-time-strategy",
-            "Strategy": "strategy",
-            "Casual": "casual",
-            "Adventure": "adventure",
-            "Board Game": "board",
-            "Action": "action",
-            "Fantasy": "fantasy",
-            "Fighting": "fighting",
-            "Music": "music",
-            "Shooter": "shooter",
-            "Puzzle": "puzzle",
-            "RPG": "role-playing",
-            "MMORPG": "mmorpg",
-            "Dating Sim": "dating-sim",
-            "Roguelike": "roguelike",
-            "Sports": "Sports",
-            "Bara": "bara",
-            "Yuri": "yuri",
-            "Gore": "gore",
-            "Comedy": "comedy",
-            "tragedy": "tragedy",
-            "Horror": "horror"
-        }
-
-        ret = []
-        for i, value in repl.items():
-            ret.extend(value for ii in self.tag if i in ii)
-        return list(set(ret))
+import re
+from contextlib import suppress
+from json import loads
+from bs4 import BeautifulSoup
+from html2text import html2text
+from langcodes import find
+from py3langid import langid, classify
+
+from ._base import BasePlugin
+from ..util.fgi import fgi_dict
+from ..util.fgi_yaml import YamlData, pss_dedent
+from ..util.spider import get_text
+
+
+class ItchIO(BasePlugin):
+    _VERIFY_PATTERN = re.compile(r"https?://.+\.itch\.io/.+")
+
+    @staticmethod
+    def remove_query(s: str):
+        s = re.sub(r"\?t=\d{6,12}", "", s)
+        return s.replace("![]", "![img]")
+
+    def __init__(self, link: str) -> None:
+        self.link = link
+        self.data_html = get_text(link)
+        self.soup = BeautifulSoup(self.data_html, "lxml")
+        self.data = [
+            ii
+            for ii in [
+                loads(i.text)
+                for i in self.soup.find_all(
+                    "script", attrs={"type": "application/ld+json"}
+                )
+            ]
+            if "name" in ii
+        ][0]
+        self.more_info = self.get_more_info()
+        self.tag = self.get_tags()
+
+    def get_thumbnail(self):
+        th = self.soup.select_one("#header > img")
+        if th is None:
+            return None
+        return th.attrs["src"]
+
+    def get_brief_desc(self):
+        return self.soup.find("meta", {"name": "twitter:description"}).attrs["content"]
+
+    def get_name(self):
+        return self.data["name"]
+
+    def get_screenshots(self):
+        temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
+        return [i.attrs['href'] for i in temp]
+
+    def get_desc(self):
+        return pss_dedent(self.remove_query(html2text(
+            str(self.soup.select_one("div.formatted_description.user_formatted")),
+            bodywidth=0,
+        )).replace("\n" * 3, "\n").strip())
+
+    def get_platforms(self):
+        repl = {
+            "Windows": "windows",
+            "macOS": "macos",
+            "Linux": "linux",
+            "Android": "android",
+            "HTML5": "web",
+            "iOS": "ios",
+        }
+        platforms = self.more_info["Platforms"] if "Platforms" in self.more_info else ["Windows"]
+        return [repl[i.strip()] for i in platforms]
+
+    def get_authors(self) -> list[dict]:
+        temp = []
+        if "Authors" in self.more_info:
+            temp = self.more_info["Authors"]
+        elif "Author" in self.more_info:
+            temp = self.more_info["Author"]
+        return [{"name": i.strip(), "role": ["producer"]} for i in temp]
+
+    def get_tags(self) -> list[str]:
+        temp = self.more_info["Genre"] if "Genre" in self.more_info else []
+        temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
+        temp2 = self.more_info["Tags"] if "Tags" in self.more_info else []
+        return [i.strip() for i in (temp2 + temp1 + temp)]
+
+    def get_misc_tags(self):
+        repl = {
+            "3D": "3d",
+            "Pixel Art": "pixel-art",
+            "free": "freeware",
+            "Multiplayer": "multiplayer",
+            "Co-op": "co-op",
+            "PvP": "pvp",
+            "Ren'Py": "engine-renpy",
+            "Unity": "engine-unity",
+            "RPG Maker": "engine-rpg-maker",
+            "Godot": "engine-godot",
+            "ue4": "engine-ue4",
+            "unreal - engine - 4": "engine-ue4",
+            "TyranoBuilder": "engine-tyranobuilder",
+            "Flash": "adobe-flash",
+            "t-series": "multiple-series",
+            "Multiple Endings": "multiple-endings",
+        }
+
+        ret = []
+        for i, value in repl.items():
+            ret.extend(value for ii in self.tag if i in ii)
+        return list(set(ret))
+
+    def get_langs(self) -> list[str]:
+        if "Languages" in self.more_info:
+            temp = self.more_info["Languages"]
+        else:
+            return [classify(self.get_desc())[0]]
+
+        return list(set(find(i).language for i in temp))
+
+    def get_links(self) -> list[dict]:
+        link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > "
+                                                              "div.formatted_description.user_formatted")
+        .select("a[href]")]
+        data = [{"url": i, "processed": False} for i in list(set(link))]
+        processed_data = []
+        for i in data:
+            for p in fgi_dict:
+                if re.match(p["match"], i["url"]):
+                    processed_data.append(
+                        {
+                            "name": p["prefix"],
+                            "uri": re.sub(p["match"], p["replace"], i["url"]),
+                        }
+                    )
+                    i["processed"] = True
+        for i in data:
+            if not i["processed"]:
+                processed_data.append({"name": ".website", "uri": i["url"]})
+        processed_data.append({"name": ".itchio", "uri": self.link})
+        return processed_data
+
+    def get_more_info(self):
+        d = {}
+        for i in range(1, 18):
+            with suppress(Exception):
+                cache = self.soup.select_one(
+                    f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
+                )
+                temp = [i.get_text() for i in list(cache.children)]
+                d[temp[0]] = temp[1:][0].split(",")
+        return d
+
+    def to_yaml(self) -> YamlData:
+        ret = {
+            "name": self.get_name(),
+            "brief-description": self.get_brief_desc(),
+            "description": self.get_desc(),
+            "description-format": "markdown",
+            "authors": self.get_authors(),
+            "tags": {
+                "type": self.get_type_tag(),
+                "lang": self.get_langs(),
+                "platform": self.get_platforms(),
+                "publish": [".itchio"],
+                "misc": self.get_misc_tags(),
+            },
+            "links": self.get_links(),
+            "thumbnail": self.get_thumbnail(),
+            "screenshots": self.get_screenshots()  # + self.get_video(),
+        }
+        return YamlData(self.__load_hook__(ret))
+
+    def get_type_tag(self):
+        repl = {
+            "Visual Novel": "visual-novel",
+            "Real time strategy": "real-time-strategy",
+            "Strategy": "strategy",
+            "Casual": "casual",
+            "Adventure": "adventure",
+            "Board Game": "board",
+            "Action": "action",
+            "Fantasy": "fantasy",
+            "Fighting": "fighting",
+            "Music": "music",
+            "Shooter": "shooter",
+            "Puzzle": "puzzle",
+            "RPG": "role-playing",
+            "MMORPG": "mmorpg",
+            "Dating Sim": "dating-sim",
+            "Roguelike": "roguelike",
+            "Sports": "Sports",
+            "Bara": "bara",
+            "Yuri": "yuri",
+            "Gore": "gore",
+            "Comedy": "comedy",
+            "tragedy": "tragedy",
+            "Horror": "horror"
+        }
+
+        ret = []
+        for i, value in repl.items():
+            ret.extend(value for ii in self.tag if i in ii)
+        return list(set(ret))
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,222 +1,224 @@
-import re
-from urllib.parse import parse_qs, urlparse
-
-from bs4 import BeautifulSoup
-from html2text import html2text
-from langcodes import find
-
-from ._base import BasePlugin
-from ..util.fgi import fgi_dict
-from ..util.fgi_yaml import YamlData, pss_dedent
-from ..util.spider import get_json, get_text
-from ..util.thread import ThreadWithReturnValue
-
-
-class Steam(BasePlugin):
-    _VERIFY_PATTERN = re.compile(r"https?://store\.steampowered\.com/app/\d+/.+/?.+")
-
-    @staticmethod
-    def get_steam_id(link: str) -> int:
-        return int(urlparse(link).path.split("/")[2])
-
-    def get_name(self):
-        return self.data[str(self.id)]["data"]["name"]
-
-    @staticmethod
-    def remove_query(s: str):
-        s = re.sub(r"\?t=\d{6,12}", "", s)
-        return s.replace("![]", "![img]")
-
-    def __init__(self, link: str) -> None:
-        self.id = self.get_steam_id(link)
-        fn_list = [ThreadWithReturnValue(target=get_json,
-                                         args=(f"https://store.steampowered.com/api/appdetails?appids={self.id}&cc=us"
-                                               f"&l=english",)),
-                   ThreadWithReturnValue(target=get_text, args=(link,))]
-        for i in fn_list:
-            i.start()
-        self.data, self.data_html = (ii.join() for ii in fn_list)
-        self.soup = BeautifulSoup(self.data_html, "lxml")
-        self.name = self.get_name()
-        temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
-        self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
-
-    def to_yaml(self) -> YamlData:
-        ret = {
-            "name": self.get_name(),
-            "brief-description": self.get_brief_desc(),
-            "description": self.get_desc(),
-            "description-format": "markdown",
-            "authors": self.get_authors(),
-            "tags": {
-                "type": self.get_type_tag(),
-                "lang": self.get_langs(),
-                "platform": self.get_platforms(),
-                "publish": ["steam"],
-                "misc": self.get_misc_tags(),
-            },
-            "links": self.get_links(),
-            "thumbnail": self.get_thumbnail(),
-            "screenshots": self.get_screenshots() + self.get_video(),  # type: ignore
-        }
-        return YamlData(self.__load_hook__(ret))
-
-    def get_langs(self) -> list[str]:
-        temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
-        return list({find(i).language for i in temp})
-
-    def get_desc(self):
-        return pss_dedent(
-            self.remove_query(
-                (
-                    html2text(
-                        self.data[str(self.id)]["data"]["detailed_description"],
-                        bodywidth=0,
-                    )
-                )
-            ).replace("\n" * 4, "\n").strip()
-        )
-
-    def get_brief_desc(self):
-        return pss_dedent(
-            html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
-        )
-
-    def get_authors(self) -> list[dict]:
-        temp = self.data[str(self.id)]["data"]
-        developers = [{"name": i.strip(), "role": ["producer"]} for i in temp["developers"]]
-        publishers = [{"name": i.strip(), "role": ["publisher"]} for i in temp["publishers"]]
-        return developers + publishers
-
-    def get_platforms(self):
-        temp = self.data[str(self.id)]["data"]["platforms"]
-        repl = {"windows": "windows", "mac": "macos", "linux": "linux"}
-        return [repl[i] for i in temp if temp[i]]
-
-    def get_type_tag(self):
-        repl = {
-            "Adventure": "adventure",
-            "Action": "action",
-            "Visual Novel": "visual-novel",
-            "Strategy": "strategy",
-            "RTS": "real-time-strategy",
-            "Casual": "casual",
-            "Management": "business-sim",
-            "Card Game": "board",
-            "Fighting": "fighting",
-            "Music": "music",
-            "Shooter": "shooter",
-            "Puzzle": "puzzle",
-            "RPG": "role-playing",
-            "MMORPG": "mmorpg",
-            "Dating Sim": "dating-sim",
-            "Roguel": "roguelike",
-            "Sports": "sports",
-            "Comedy": "comedy",
-            "Horror": "horror",
-        }
-
-        ret = []
-        for i, value in repl.items():
-            ret.extend(value for ii in self.tag if i in ii)
-        return list(set(ret))
-
-    def get_tags(self) -> list[str]:
-        return self.tag
-
-    def get_misc_tags(self):
-        repl = {
-            "3D": "3d",
-            "Pixel": "pixel-art",
-            "Multiplayer": "multiplayer",
-            "PvP": "pvp",
-            "Sexual": "uncensored",
-            "Nudity": "uncensored",
-            "Free to Play": "freeware",
-            "Story Rich": "multiple-endings",
-            "JRPG": "multiple-endings",
-            "Co-Op": "co-op",
-            "Online": "online",
-        }
-        ret = []
-        for i, value in repl.items():
-            ret.extend(value for ii in self.tag if i in ii)
-        return list(set(ret))
-
-    def get_if_nsfw(self):
-        return (
-                self.soup.body.find_all("div", {"id": "game_area_content_descriptors"})
-                != []
-        )
-
-    def get_screenshots(self):
-        return [
-            self.remove_query(i["path_full"])
-            for i in self.data[str(self.id)]["data"]["screenshots"]
-        ]
-
-    def get_video(self):
-        is_nsfw = self.get_if_nsfw()
-        video_webm = [
-            self.remove_query(i["webm"]["max"]).replace("http", "https")
-            for i in self.data[str(self.id)]["data"]["movies"]
-        ]
-        video_mp4 = [
-            self.remove_query(i["mp4"]["max"]).replace("http", "https")
-            for i in self.data[str(self.id)]["data"]["movies"]
-        ]
-        return [
-            {
-                "video": [{"mime": "video/webm", "sensitive": is_nsfw, "uri": video_webm[i], },
-                          {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
-                          ]
-                if is_nsfw
-                else [
-                    {"mime": "video/webm", "uri": video_webm[i]},
-                    {"mime": "video/mp4", "uri": video_mp4[i]},
-                ],
-            }
-            for i in range(len(video_webm))
-        ]
-
-    def get_links(self) -> list[dict]:
-        def remove_query_string(x: str):
-            return parse_qs(urlparse(x).query)["url"][0] if "linkfilter" in x else x  # type: ignore
-
-        temp1 = self.soup.body.find(
-            "div",
-            attrs={"class": "game_area_description"},
-        )
-        temp3 = self.soup.body.find("div", attrs={"style": "padding-top: 14px;"})
-        temp2 = temp3.find_all("a")
-        temp4 = [
-            remove_query_string(i["data-tooltip-text"])
-            for i in temp2
-            if "data-tooltip-text" in i.attrs
-        ]
-        temp = temp1.select("a[href]")
-        ret = []
-        for i in temp:
-            ret.append(remove_query_string(i.attrs["href"]))
-        data = [{"url": i, "processed": False} for i in list(set(ret + temp4))]
-        processed_data = []
-        for i in data:
-            for p in fgi_dict:
-                if re.match(p["match"], i["url"]):
-                    processed_data.append(
-                        {
-                            "name": p["prefix"],
-                            "uri": re.sub(p["match"], p["replace"], i["url"]),
-                        }
-                    )
-                    i["processed"] = True
-        for i in data:
-            if not i["processed"]:
-                processed_data.append({"name": ".website", "uri": i["url"]})
-        processed_data.append({"name": ".steam", "uri": f'steam:{self.id}'})
-        return processed_data
-
-    def get_thumbnail(self):
-        return self.remove_query(
-            self.soup.body.find("img", {"class": "game_header_image_full"}).attrs["src"]
-        )
+import re
+from urllib.parse import parse_qs, urlparse
+from yaml import dump
+from bs4 import BeautifulSoup
+from html2text import html2text
+from langcodes import find, Language
+
+from ._base import BasePlugin
+from ..util.fgi import fgi_dict
+from ..util.fgi_yaml import YamlData, pss_dedent
+from ..util.spider import get_json, get_text
+from ..util.thread import ThreadWithReturnValue
+
+
+class Steam(BasePlugin):
+    _VERIFY_PATTERN = re.compile(r"https?://store\.steampowered\.com/app/\d+/.+/?.+")
+
+    @staticmethod
+    def get_steam_id(link: str) -> int:
+        return int(urlparse(link).path.split("/")[2])
+
+    def get_name(self):
+        return self.data[str(self.id)]["data"]["name"]
+
+    @staticmethod
+    def remove_query(s: str):
+        s = re.sub(r"\?t=\d{6,12}", "", s)
+        return s.replace("![]", "![img]")
+
+    def __init__(self, link: str, lang:str ='en') -> None:
+        self.id = self.get_steam_id(link)
+        if lang!='en':
+            print(dump(get_json(f'https://store.steampowered.com/api/appdetails?appids={self.id}&l={Language.get(lang).display_name("en").lower()}'),allow_unicode=True))
+        fn_list = [ThreadWithReturnValue(target=get_json,
+                                         args=(f"https://store.steampowered.com/api/appdetails?appids={self.id}"
+                                               f"&l=english",)),
+                   ThreadWithReturnValue(target=get_text, args=(link,))]
+        for i in fn_list:
+            i.start()
+        self.data, self.data_html = (ii.join() for ii in fn_list)
+        self.soup = BeautifulSoup(self.data_html, "lxml")
+        self.name = self.get_name()
+        temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
+        self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
+
+    def to_yaml(self) -> YamlData:
+        ret = {
+            "name": self.get_name(),
+            "brief-description": self.get_brief_desc(),
+            "description": self.get_desc(),
+            "description-format": "markdown",
+            "authors": self.get_authors(),
+            "tags": {
+                "type": self.get_type_tag(),
+                "lang": self.get_langs(),
+                "platform": self.get_platforms(),
+                "publish": ["steam"],
+                "misc": self.get_misc_tags(),
+            },
+            "links": self.get_links(),
+            "thumbnail": self.get_thumbnail(),
+            "screenshots": self.get_screenshots() + self.get_video(),  # type: ignore
+        }
+        return YamlData(self.__load_hook__(ret))
+
+    def get_langs(self) -> list[str]:
+        temp = self.data[str(self.id)]["data"]["supported_languages"].split(",")
+        return list({find(i).language for i in temp})
+
+    def get_desc(self):
+        return pss_dedent(
+            self.remove_query(
+                (
+                    html2text(
+                        self.data[str(self.id)]["data"]["detailed_description"],
+                        bodywidth=0,
+                    )
+                )
+            ).replace("\n" * 4, "\n").strip()
+        )
+
+    def get_brief_desc(self):
+        return pss_dedent(
+            html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
+        )
+
+    def get_authors(self) -> list[dict]:
+        temp = self.data[str(self.id)]["data"]
+        developers = [{"name": i.strip(), "role": ["producer"]} for i in temp["developers"]]
+        publishers = [{"name": i.strip(), "role": ["publisher"]} for i in temp["publishers"]]
+        return developers + publishers
+
+    def get_platforms(self):
+        temp = self.data[str(self.id)]["data"]["platforms"]
+        repl = {"windows": "windows", "mac": "macos", "linux": "linux"}
+        return [repl[i] for i in temp if temp[i]]
+
+    def get_type_tag(self):
+        repl = {
+            "Adventure": "adventure",
+            "Action": "action",
+            "Visual Novel": "visual-novel",
+            "Strategy": "strategy",
+            "RTS": "real-time-strategy",
+            "Casual": "casual",
+            "Management": "business-sim",
+            "Card Game": "board",
+            "Fighting": "fighting",
+            "Music": "music",
+            "Shooter": "shooter",
+            "Puzzle": "puzzle",
+            "RPG": "role-playing",
+            "MMORPG": "mmorpg",
+            "Dating Sim": "dating-sim",
+            "Roguel": "roguelike",
+            "Sports": "sports",
+            "Comedy": "comedy",
+            "Horror": "horror",
+        }
+
+        ret = []
+        for i, value in repl.items():
+            ret.extend(value for ii in self.tag if i in ii)
+        return list(set(ret))
+
+    def get_tags(self) -> list[str]:
+        return self.tag
+
+    def get_misc_tags(self):
+        repl = {
+            "3D": "3d",
+            "Pixel": "pixel-art",
+            "Multiplayer": "multiplayer",
+            "PvP": "pvp",
+            "Sexual": "uncensored",
+            "Nudity": "uncensored",
+            "Free to Play": "freeware",
+            "Story Rich": "multiple-endings",
+            "JRPG": "multiple-endings",
+            "Co-Op": "co-op",
+            "Online": "online",
+        }
+        ret = []
+        for i, value in repl.items():
+            ret.extend(value for ii in self.tag if i in ii)
+        return list(set(ret))
+
+    def get_if_nsfw(self):
+        return (
+                self.soup.body.find_all("div", {"id": "game_area_content_descriptors"})
+                != []
+        )
+
+    def get_screenshots(self):
+        return [
+            self.remove_query(i["path_full"])
+            for i in self.data[str(self.id)]["data"]["screenshots"]
+        ]
+
+    def get_video(self):
+        is_nsfw = self.get_if_nsfw()
+        video_webm = [
+            self.remove_query(i["webm"]["max"]).replace("http", "https")
+            for i in self.data[str(self.id)]["data"]["movies"]
+        ]
+        video_mp4 = [
+            self.remove_query(i["mp4"]["max"]).replace("http", "https")
+            for i in self.data[str(self.id)]["data"]["movies"]
+        ]
+        return [
+            {
+                "video": [{"mime": "video/webm", "sensitive": is_nsfw, "uri": video_webm[i], },
+                          {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
+                          ]
+                if is_nsfw
+                else [
+                    {"mime": "video/webm", "uri": video_webm[i]},
+                    {"mime": "video/mp4", "uri": video_mp4[i]},
+                ],
+            }
+            for i in range(len(video_webm))
+        ]
+
+    def get_links(self) -> list[dict]:
+        def remove_query_string(x: str):
+            return parse_qs(urlparse(x).query)["url"][0] if "linkfilter" in x else x  # type: ignore
+
+        temp1 = self.soup.body.find(
+            "div",
+            attrs={"class": "game_area_description"},
+        )
+        temp3 = self.soup.body.find("div", attrs={"style": "padding-top: 14px;"})
+        temp2 = temp3.find_all("a")
+        temp4 = [
+            remove_query_string(i["data-tooltip-text"])
+            for i in temp2
+            if "data-tooltip-text" in i.attrs
+        ]
+        temp = temp1.select("a[href]")
+        ret = []
+        for i in temp:
+            ret.append(remove_query_string(i.attrs["href"]))
+        data = [{"url": i, "processed": False} for i in list(set(ret + temp4))]
+        processed_data = []
+        for i in data:
+            for p in fgi_dict:
+                if re.match(p["match"], i["url"]):
+                    processed_data.append(
+                        {
+                            "name": p["prefix"],
+                            "uri": re.sub(p["match"], p["replace"], i["url"]),
+                        }
+                    )
+                    i["processed"] = True
+        for i in data:
+            if not i["processed"]:
+                processed_data.append({"name": ".website", "uri": i["url"]})
+        processed_data.append({"name": ".steam", "uri": f'steam:{self.id}'})
+        return processed_data
+
+    def get_thumbnail(self):
+        return self.remove_query(
+            self.soup.body.find("img", {"class": "game_header_image_full"}).attrs["src"]
+        )
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from .fgi_yaml import fgi
-from .fgi import default_config
-from ..exception import ReadOrWriteConfigFailed
-
-
-class Config:
-    proxy = {}
-    api = {}
-    plugin = {}
-    hook = {}
-
-    def __getitem__(self, item):
-        # Compatibility with the old version
-        return self.__getattribute__(item)
-
-    def __setitem__(self, key, value):
-        # Compatibility with the old version
-        self.__setattr__(key, value)
-
-    def load(self, file_data: str | dict = None):
-        """
-
-        Args:
-            file_data:
-                When the type is str, it is text in yaml format.
-
-                When the type is dict, it is the serialized dictionary data.
-
-                When it is empty, the default is the default configuration(see util.fgi.default_config)
-
-        Returns:
-
-        """
-        if type(file_data) is dict:
-            self.__dict__.update(file_data)
-            return
-        if file_data is None:
-            self.__dict__.update(default_config)
-            return
-        try:
-            with open(file_data, "r", encoding="utf-8") as fp:
-                self.__dict__.update(fgi.load(fp))
-        except Exception:
-            raise ReadOrWriteConfigFailed from None
-
-    def update(self, data: dict):
-        self.__dict__.update(data)
-
-    def __str__(self):
-        fgi.preserve_quotes = True
-        fgi.explicit_start = True
-        fgi.indent = 1
-        return fgi.dump_to_string(self.__dict__)
-
-
-config = Config()
+from .fgi_yaml import fgi
+from .fgi import default_config
+from ..exception import ReadOrWriteConfigFailed
+
+
+class Config:
+    proxy = {}
+    api = {}
+    plugin = {}
+    hook = {}
+
+    def __getitem__(self, item):
+        # Compatibility with the old version
+        return self.__getattribute__(item)
+
+    def __setitem__(self, key, value):
+        # Compatibility with the old version
+        self.__setattr__(key, value)
+
+    def load(self, file_data: str | dict = None):
+        """
+
+        Args:
+            file_data:
+                When the type is str, it is text in yaml format.
+
+                When the type is dict, it is the serialized dictionary data.
+
+                When it is empty, the default is the default configuration(see util.fgi.default_config)
+
+        Returns:
+
+        """
+        if type(file_data) is dict:
+            self.__dict__.update(file_data)
+            return
+        if file_data is None:
+            self.__dict__.update(default_config)
+            return
+        try:
+            with open(file_data, "r", encoding="utf-8") as fp:
+                self.__dict__.update(fgi.load(fp))
+        except Exception as e:
+            raise ReadOrWriteConfigFailed from e
+
+    def update(self, data: dict):
+        self.__dict__.update(data)
+
+    def __str__(self):
+        fgi.preserve_quotes = True
+        fgi.explicit_start = True
+        fgi.indent = 1
+        return fgi.dump_to_string(self.__dict__)
+
+
+config = Config()
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/fgi.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-fgi_dict = [
-    {
-        "match": r"^https://www.youtube.com/(?!watch\?v=)(?!channel/)(@?.+)",
-        "prefix": ".youtube",
-        "replace": "youtube:@\\g<1>",
-    },
-    {
-        "match": "^https://www.youtube.com/channel/(.+[^/])/",
-        "prefix": ".youtube",
-        "replace": "youtube:\\g<1>",
-    },
-    {
-        "match": "^https://twitter.com/([A-Za-z0-9_]+).*",
-        "prefix": ".twitter",
-        "replace": "twitter:\\g<1>",
-    },
-    {
-        "match": "^https://www.patreon.com/(.+)",
-        "prefix": ".patreon",
-        "replace": "patreon:\\g<1>",
-    },
-    {
-        "match": "^https://discord.gg/(.+)",
-        "prefix": ".discord",
-        "replace": "discord:\\g<1>",
-    },
-    {
-        "match": "^https://www.facebook.com/(.+)/",
-        "prefix": ".facebook",
-        "replace": "facebook:\\g<1>",
-    },
-    {
-        "match": "^https://www.furaffinity.net/user/(.+)/",
-        "prefix": ".furaffinity",
-        "replace": "furaffinity:\\g<1>",
-    },
-    {
-        "match": "(https://weibo.com/u/.+)",
-        "prefix": ".weibo",
-        "replace": "\\g<1>",
-    },
-]
-default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
-                          'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
-                  'hook': ['search', 'validate'],
-                  'plugin': ['steam', 'itchio'],
-                  'proxy': {}}
-template_dict = {
-    "name": 'NAME',
-    "brief-description": 'BRIEF-DESC',
-    "description": 'DESC',
-    "description-format": "markdown",
-    "authors": [],
-    "tags": {
-        "type": [],
-        "lang": [],
-        "platform": [],
-        "publish": [],
-        "misc": [],
-    },
-    "links": [],
-    "thumbnail": 'THUMBNAIL.PNG',
-    "screenshots": [],
-}
+fgi_dict = [
+    {
+        "match": r"^https://www.youtube.com/(?!watch\?v=)(?!channel/)(@?.+)",
+        "prefix": ".youtube",
+        "replace": "youtube:@\\g<1>",
+    },
+    {
+        "match": "^https://www.youtube.com/channel/(.+[^/])/",
+        "prefix": ".youtube",
+        "replace": "youtube:\\g<1>",
+    },
+    {
+        "match": "^https://twitter.com/([A-Za-z0-9_]+).*",
+        "prefix": ".twitter",
+        "replace": "twitter:\\g<1>",
+    },
+    {
+        "match": "^https://www.patreon.com/(.+)",
+        "prefix": ".patreon",
+        "replace": "patreon:\\g<1>",
+    },
+    {
+        "match": "^https://discord.gg/(.+)",
+        "prefix": ".discord",
+        "replace": "discord:\\g<1>",
+    },
+    {
+        "match": "^https://www.facebook.com/(.+)/",
+        "prefix": ".facebook",
+        "replace": "facebook:\\g<1>",
+    },
+    {
+        "match": "^https://www.furaffinity.net/user/(.+)/",
+        "prefix": ".furaffinity",
+        "replace": "furaffinity:\\g<1>",
+    },
+    {
+        "match": "(https://weibo.com/u/.+)",
+        "prefix": ".weibo",
+        "replace": "\\g<1>",
+    },
+]
+default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
+                          'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
+                  'hook': ['search', 'validate'],
+                  'plugin': ['steam', 'itchio'],
+                  'proxy': {}}
+template_dict = {
+    "name": 'NAME',
+    "brief-description": 'BRIEF-DESC',
+    "description": 'DESC',
+    "description-format": "markdown",
+    "authors": [],
+    "tags": {
+        "type": [],
+        "lang": [],
+        "platform": [],
+        "publish": [],
+        "misc": [],
+    },
+    "links": [],
+    "thumbnail": 'THUMBNAIL.PNG',
+    "screenshots": [],
+}
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import re
-import zipfile
-from io import BytesIO
-from textwrap import dedent
-
-from PIL import Image
-from loguru import logger
-from ruamel.yaml import YAML
-from ruamel.yaml.scalarstring import PreservedScalarString
-
-
-def pss_dedent(x: str) -> PreservedScalarString:
-    return PreservedScalarString(dedent(x))
-
-
-fgi = YAML(typ=["rt", "string"])
-fgi.indent(sequence=4, offset=2)
-fgi.preserve_quotes = True
-fgi.width = 4096
-
-
-def dump_to_yaml(data: dict) -> str:
-    temp = fgi.dump_to_string(data)
-    for i in list(data.keys())[1:]:
-        temp = temp.replace("\n" + i, "\n\n" + i)
-    temp = temp.replace("description: |-", "description: |")
-    return temp
-
-
-def process_thumbnail(img_byte: bytes):
-    img = Image.open(BytesIO(img_byte))
-    if img.size == (460, 215):
-        img_resize = img.resize((360, 168))
-        ret_byte = BytesIO()
-        img_resize.save(ret_byte, format="PNG", optimize=True, quality=85)
-        return ret_byte.getvalue()
-    logger.warning("Thumbnails cannot be scaled down.")
-    return img_byte
-
-
-class YamlData:
-    raw_dict: dict
-
-    def __init__(self, raw_data: dict):
-        self.raw_dict = raw_data
-
-    def __str__(self):
-        return dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'})
-
-    def __bytes__(self):
-        from ..util.spider import get_bytes
-        _io = BytesIO()
-        zip_data = zipfile.ZipFile(_io, 'w', zipfile.ZIP_STORED)
-        if self.raw_dict["thumbnail"] is not None:
-            img = get_bytes(self.raw_dict["thumbnail"])
-            zip_data.writestr('thumbnail.png', process_thumbnail(img))
-            logger.info("thumbnail exists")
-        zip_data.writestr(get_valid_filename(self.raw_dict['name']) + ".yaml",
-                          dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'}))
-        zip_data.close()
-        return _io.getvalue()
-
-
-def get_valid_filename(s):
-    s = s.strip().replace(' ', '_')
-    return re.sub(r'(?u)[^-\w.]', '_', s)
+import re
+import zipfile
+from io import BytesIO
+from textwrap import dedent
+
+from PIL import Image
+from loguru import logger
+from ruamel.yaml import YAML
+from ruamel.yaml.scalarstring import PreservedScalarString
+
+
+def pss_dedent(x: str) -> PreservedScalarString:
+    return PreservedScalarString(dedent(x))
+
+
+fgi = YAML(typ=["rt", "string"])
+fgi.indent(sequence=4, offset=2)
+fgi.preserve_quotes = True
+fgi.width = 4096
+
+
+def dump_to_yaml(data: dict) -> str:
+    temp = fgi.dump_to_string(data)
+    for i in list(data.keys())[1:]:
+        temp = temp.replace("\n" + i, "\n\n" + i)
+    temp = temp.replace("description: |-", "description: |")
+    return temp
+
+
+def process_thumbnail(img_byte: bytes):
+    img = Image.open(BytesIO(img_byte))
+    if img.size == (460, 215):
+        img_resize = img.resize((360, 168))
+        ret_byte = BytesIO()
+        img_resize.save(ret_byte, format="PNG", optimize=True, quality=85)
+        return ret_byte.getvalue()
+    logger.warning("Thumbnails cannot be scaled down.")
+    return img_byte
+
+
+class YamlData:
+    raw_dict: dict
+
+    def __init__(self, raw_data: dict):
+        self.raw_dict = raw_data
+
+    def __str__(self):
+        return dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'})
+
+    def __bytes__(self):
+        from ..util.spider import get_bytes
+        _io = BytesIO()
+        zip_data = zipfile.ZipFile(_io, 'w', zipfile.ZIP_STORED)
+        if self.raw_dict["thumbnail"] is not None:
+            img = get_bytes(self.raw_dict["thumbnail"])
+            zip_data.writestr('thumbnail.png', process_thumbnail(img))
+            logger.info("thumbnail exists")
+        zip_data.writestr(get_valid_filename(self.raw_dict['name']) + ".yaml",
+                          dump_to_yaml({**self.raw_dict, "thumbnail": 'thumbnail.png'}))
+        zip_data.close()
+        return _io.getvalue()
+
+
+def get_valid_filename(s):
+    s = s.strip().replace(' ', '_')
+    return re.sub(r'(?u)[^-\w.]', '_', s)
```

### Comparing `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.7/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import importlib
-from typing import Literal, Type, Union
-
-from loguru import logger
-
-from ..hook import BaseHook
-from ..plugin import BasePlugin
-from ..util.config import config
-
-
-class Package:
-    plugin: dict[str, BasePlugin] = {}
-    hook: dict[str, BaseHook] = {}
-    log: list[str | None] = []
-
-    def __init__(self):
-        self.load_plugins()
-        self.load_hooks()
-
-    def __getitem__(self, item):
-        # Compatibility with the old version
-        return self.__getattribute__(item)
-
-    def __setitem__(self, key, value):
-        # Compatibility with the old version
-        self.__setattr__(key, value)
-
-    def _load(
-            self,
-            _dir: Literal["plugin"],
-            _type: Type[BasePlugin],
-    ):
-        base = __package__.split(".")[0] + "." + _dir
-        for plugin in getattr(config, _dir, []):
-            if plugin in self.log:
-                continue
-            if plugin.startswith("_"):
-                logger.warning(f"Skip loading protected {_dir} {plugin}")
-                continue
-            try:
-                package = f"{base}.{plugin}"
-                logger.info(f"Loading {_dir}: {plugin}")
-                temp = importlib.import_module(package)
-                self[_dir][plugin] = [
-                    o
-                    for o in temp.__dict__.values()
-                    if isinstance(o, type) and issubclass(o, _type) and o is not _type
-                ][-1]
-                self["log"].append(temp.__name__.split(".")[-1])
-            except ImportError as e:
-                logger.trace(e)
-                logger.error(f"Failed to import {_dir}: {plugin}")
-            except IndexError:
-                logger.error(f"Imported {_dir} but no {_type.__name__} found: {plugin}")
-
-    def load_plugins(self):
-        self._load("plugin", BasePlugin)
-
-    def load_hooks(self):
-        if config["hook"] is None:
-            if None not in self.log:
-                logger.warning(f"All hooks are disabled")
-                self.log.append(None)
-            return
-        for plugin in getattr(config, "hook", []):
-            try:
-                if plugin in self.log:
-                    continue
-                logger.info(f"Loading hook: {plugin}")
-                self["log"].append(plugin)
-                temp = importlib.import_module(f"yamlgenerator_hook_{plugin}")
-                self["hook"][plugin] = [
-                    o
-                    for o in temp.__dict__.values()
-                    if isinstance(o, type) and issubclass(o, BaseHook) and o is not BaseHook
-                ][-1]
-            except ImportError as e:
-                logger.trace(e)
-                logger.error(f"Failed to import hook: {plugin}")
-            except IndexError:
-                logger.error(f"Imported hook but no BaseHook found: {plugin}")
-
-
-pkg = Package()
+import importlib
+from typing import Literal, Type, Union
+
+from loguru import logger
+
+from ..hook import BaseHook
+from ..plugin import BasePlugin
+from ..util.config import config
+
+
+class Package:
+    plugin: dict[str, BasePlugin] = {}
+    hook: dict[str, BaseHook] = {}
+    log: list[str | None] = []
+
+    def __init__(self):
+        self.load_plugins()
+        self.load_hooks()
+
+    def __getitem__(self, item):
+        # Compatibility with the old version
+        return self.__getattribute__(item)
+
+    def __setitem__(self, key, value):
+        # Compatibility with the old version
+        self.__setattr__(key, value)
+
+    def _load(
+            self,
+            _dir: Literal["plugin"],
+            _type: Type[BasePlugin],
+    ):
+        base = __package__.split(".")[0] + "." + _dir
+        for plugin in getattr(config, _dir, []):
+            if plugin in self.log:
+                continue
+            if plugin.startswith("_"):
+                logger.warning(f"Skip loading protected {_dir} {plugin}")
+                continue
+            try:
+                package = f"{base}.{plugin}"
+                logger.info(f"Loading {_dir}: {plugin}")
+                temp = importlib.import_module(package)
+                self[_dir][plugin] = [
+                    o
+                    for o in temp.__dict__.values()
+                    if isinstance(o, type) and issubclass(o, _type) and o is not _type
+                ][-1]
+                self["log"].append(temp.__name__.split(".")[-1])
+            except ImportError as e:
+                logger.trace(e)
+                logger.error(f"Failed to import {_dir}: {plugin}")
+            except IndexError:
+                logger.error(f"Imported {_dir} but no {_type.__name__} found: {plugin}")
+
+    def load_plugins(self):
+        self._load("plugin", BasePlugin)
+
+    def load_hooks(self):
+        if config["hook"] is None:
+            if None not in self.log:
+                logger.warning(f"All hooks are disabled")
+                self.log.append(None)
+            return
+        for plugin in getattr(config, "hook", []):
+            try:
+                if plugin in self.log:
+                    continue
+                logger.info(f"Loading hook: {plugin}")
+                self["log"].append(plugin)
+                temp = importlib.import_module(f"yamlgenerator_hook_{plugin}")
+                self["hook"][plugin] = [
+                    o
+                    for o in temp.__dict__.values()
+                    if isinstance(o, type) and issubclass(o, BaseHook) and o is not BaseHook
+                ][-1]
+            except ImportError as e:
+                logger.trace(e)
+                logger.error(f"Failed to import hook: {plugin}")
+            except IndexError:
+                logger.error(f"Imported hook but no BaseHook found: {plugin}")
+
+
+pkg = Package()
```

### Comparing `gameyamlspiderandgenerator-1.6.6/PKG-INFO` & `gameyamlspiderandgenerator-1.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.6.6
+Version: 1.6.7
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

