# Comparing `tmp/async_wrapper-0.1.1.tar.gz` & `tmp/async_wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.1.tar", max compression
+gzip compressed data, was "async_wrapper-0.1.2.tar", max compression
```

## Comparing `async_wrapper-0.1.1.tar` & `async_wrapper-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/LICENSE
--rw-r--r--   0        0        0     1536 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/README.md
--rw-r--r--   0        0        0     3501 2023-06-25 16:21:24.768000 async_wrapper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      279 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-06-25 16:21:24.812001 async_wrapper-0.1.1/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      938 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/_joblib.py
--rw-r--r--   0        0        0      706 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      652 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1723 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0     1025 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/synclib/_joblib.py
--rw-r--r--   0        0        0     1217 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      666 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      113 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     2357 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     2208 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     1889 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     1244 2023-06-25 16:21:11.015774 async_wrapper-0.1.1/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 async_wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-26 12:05:22.641344 async_wrapper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1534 2023-06-26 12:05:22.641344 async_wrapper-0.1.2/README.md
+-rw-r--r--   0        0        0     3648 2023-06-26 12:05:36.381400 async_wrapper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      279 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-26 12:05:36.425400 async_wrapper-0.1.2/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0      919 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      706 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      652 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1723 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1217 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1581 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      662 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      113 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     2357 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     2208 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     1889 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     1244 2023-06-26 12:05:22.645344 async_wrapper-0.1.2/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 async_wrapper-0.1.2/PKG-INFO
```

### Comparing `async_wrapper-0.1.1/LICENSE` & `async_wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/README.md` & `async_wrapper-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```shell
 $ pip install async_wrapper
 # or
 $ pip install "async_wrapper[all]"
 # or
 $ pip install "async_wrapper[anyio]"
 # or
-$ pip install "async_wrapper[joblib]"
+$ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 import asyncio
 
 from aiotools import TaskGroup
```

### Comparing `async_wrapper-0.1.1/pyproject.toml` & `async_wrapper-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.1"
+version = "0.1.2"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = { version = "^3.7.0", optional = true }
-joblib = {version = "^1.2.0", optional = true}
 aiotools = { version = "^1.6.1", python = "<3.11" }
+loky = { version = "^3.4.0", optional = true }
+cloudpickle = { version = "^2.2.1", optional = true }
+psutil = { version = "^5.9.5", optional = true }
 
 [tool.poetry.extras]
-all = ['anyio', 'joblib']
+all = ['anyio', 'loky', "cloudpickle", "psutil"]
 anyio = ['anyio']
-joblib = ['joblib']
+loky = ['loky', "cloudpickle", "psutil"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.275"
 black = "23.3.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
```

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/_joblib.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 __all__ = ["sync_to_async"]
 
 
 def sync_to_async(
     func: Callable[ParamT, ValueT],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     try:
-        from joblib.externals.loky.process_executor import (  # type: ignore
+        from loky.process_executor import (  # type: ignore
             ProcessPoolExecutor,  # type: ignore
         )
     except (ImportError, ModuleNotFoundError) as exc:
-        raise ImportError("install extas joblib first") from exc
+        raise ImportError("install extas loky first") from exc
 
     @wraps(func)
     async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
         with ProcessPoolExecutor(1) as pool:
             future = pool.submit(func, *args, **kwargs)  # type: ignore
             coro = asyncio.wrap_future(future)
             return await coro
```

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/main.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/synclib/_joblib.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_loky.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 __all__ = ["async_to_sync"]
 
 
 def async_to_sync(
     func: Callable[ParamT, Awaitable[ValueT]],
 ) -> Callable[ParamT, ValueT]:
     try:
-        from joblib.externals.loky.process_executor import (  # type: ignore
+        from loky.process_executor import (  # type: ignore
             ProcessPoolExecutor,  # type: ignore
         )
     except (ImportError, ModuleNotFoundError) as exc:
-        raise ImportError("install extas joblib first") from exc
+        raise ImportError("install extas loky first") from exc
 
     sync_func = as_sync_func(func)
 
     @wraps(func)
     def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
         with ProcessPoolExecutor(1) as pool:
             future = pool.submit(sync_func, *args, **kwargs)  # type: ignore
```

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.1.2/src/async_wrapper/convert/synclib/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 if TYPE_CHECKING:
     from async_wrapper.convert.synclib.base import AsyncToSync
 
 __all__ = ["get_sync_convertor"]
 
 DEFAULT_BACKEND = "thread"
-SyncBackendType = Literal["thread", "joblib"]
+SyncBackendType = Literal["thread", "loky"]
 
 
 def get_sync_convertor(
     backend: SyncBackendType | str | None = None,
 ) -> AsyncToSync:
     """get sync convertor
 
     Args:
-        backend: thread or joblib. Defaults to None.
+        backend: thread or loky. Defaults to None.
 
     Returns:
         async to sync
     """
     if not backend:
         backend = DEFAULT_BACKEND
```

### Comparing `async_wrapper-0.1.1/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.1.2/src/async_wrapper/task_group/_anyio.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/task_group/_asyncio.py` & `async_wrapper-0.1.2/src/async_wrapper/task_group/_asyncio.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/task_group/base.py` & `async_wrapper-0.1.2/src/async_wrapper/task_group/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/src/async_wrapper/task_group/main.py` & `async_wrapper-0.1.2/src/async_wrapper/task_group/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.1/PKG-INFO` & `async_wrapper-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: anyio
-Provides-Extra: joblib
+Provides-Extra: loky
 Requires-Dist: aiotools (>=1.6.1,<2.0.0) ; python_version < "3.11"
 Requires-Dist: anyio (>=3.7.0,<4.0.0) ; extra == "all" or extra == "anyio"
-Requires-Dist: joblib (>=1.2.0,<2.0.0) ; extra == "all" or extra == "joblib"
+Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
+Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
+Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -34,15 +36,15 @@
 ```shell
 $ pip install async_wrapper
 # or
 $ pip install "async_wrapper[all]"
 # or
 $ pip install "async_wrapper[anyio]"
 # or
-$ pip install "async_wrapper[joblib]"
+$ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 import asyncio
 
 from aiotools import TaskGroup
```

