# Comparing `tmp/taskproc-0.11.2.tar.gz` & `tmp/taskproc-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskproc-0.11.2.tar", max compression
+gzip compressed data, was "taskproc-0.13.0.tar", max compression
```

## Comparing `taskproc-0.11.2.tar` & `taskproc-0.13.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8111 2023-05-21 01:40:12.885265 taskproc-0.11.2/README.md
--rw-r--r--   0        0        0      681 2023-05-22 07:28:08.234873 taskproc-0.11.2/pyproject.toml
--rw-r--r--   0        0        0      624 2023-05-19 04:18:19.730222 taskproc-0.11.2/taskproc/__init__.py
--rw-r--r--   0        0        0     2891 2023-05-19 07:13:23.867522 taskproc-0.11.2/taskproc/app.py
--rw-r--r--   0        0        0     4865 2023-05-21 01:39:23.593621 taskproc-0.11.2/taskproc/database.py
--rw-r--r--   0        0        0     7621 2023-05-19 07:06:46.262957 taskproc-0.11.2/taskproc/graph.py
--rw-r--r--   0        0        0    15554 2023-05-22 07:25:31.589696 taskproc-0.11.2/taskproc/task.py
--rw-r--r--   0        0        0     1391 2023-05-18 04:14:19.815251 taskproc-0.11.2/taskproc/types.py
--rw-r--r--   0        0        0     8943 1970-01-01 00:00:00.000000 taskproc-0.11.2/PKG-INFO
+-rw-r--r--   0        0        0     8331 2023-06-26 12:28:34.726418 taskproc-0.13.0/README.md
+-rw-r--r--   0        0        0      780 2023-06-26 12:29:55.527106 taskproc-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0      642 2023-06-08 13:56:31.615465 taskproc-0.13.0/taskproc/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-08 13:55:12.824235 taskproc-0.13.0/taskproc/app.py
+-rw-r--r--   0        0        0     6147 2023-06-20 06:37:28.889366 taskproc-0.13.0/taskproc/database.py
+-rw-r--r--   0        0        0     9499 2023-06-20 06:25:37.741787 taskproc-0.13.0/taskproc/graph.py
+-rw-r--r--   0        0        0    17846 2023-06-20 06:35:17.164036 taskproc-0.13.0/taskproc/task.py
+-rw-r--r--   0        0        0     1443 2023-06-08 06:13:46.577173 taskproc-0.13.0/taskproc/types.py
+-rw-r--r--   0        0        0     9209 1970-01-01 00:00:00.000000 taskproc-0.13.0/PKG-INFO
```

### Comparing `taskproc-0.11.2/README.md` & `taskproc-0.13.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 # taskproc
 
 A lightweight workflow building/execution/management tool written in pure Python.
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
-
 #### Features
-* Decomposing long and complex computation into tasks, i.e., smaller units of work.
-* Executing them in a distributed way, supporting multithreading, multiprocessing, local clusters/containers.
-* Creating/discarding caches per task and reusing them whenever possible. 
+* Decomposing long and complex computation into tasks, i.e., smaller units of work with dependencies.
+* Executing them in a distributed way, supporting multithreading/multiprocessing and local container/cluster-based dispatching.
+* Automatically creating/discarding/reusing caches per task. 
 
 #### Nonfeatures
-* Automatic retry
-* External service integration with remote clusters/containers or cloud platforms (GCP, AWS, ...)
 * Periodic scheduling
-* GUI dashboard
+* Automatic retry
+* External service integration (GCP, AWS, ...)
 
 ## Installation
 
 ```
 pip install taskproc
 ```
 
 ## Usage
 
 ### Basic usage
 
 Workflow is a directed acyclic graph (DAG) of tasks, and task is a unit of work represented with a class.
-Here is an example.
+Each task and its upstream dependencies are specified with a class definition:
 ```python
-from taskproc import TaskBase, Req, Requires, Const
+from taskproc import TaskBase, Requires, Const
 
-# Define a task and **its entire upstream workflow** with a class definition.
-# Inheriting `TaskBase` is necesary, as it takes care of all the work storing and reusing the result and tracking the dependencies.
-# `infer_task_type` decorator helps the type checker to infer the types of the task class. (optional)
-@infer_task_type
 class Choose(TaskBase):
     """ Compute the binomial coefficient. """
-    # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
+    # Inside a task, we first declare the values that must be computed in upstream.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
     prev1: Requires[int]
     prev2: Requires[int]
 
-    def build_task(self, n: int, k: int):
-        # The prerequisite tasks and the other instance attributes are prepared here.
+    def __init__(self, n: int, k: int):
+        # The upstream tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
             self.prev1 = Choose(n - 1, k - 1)
             self.prev2 = Choose(n - 1, k)
         elif k == 0 or k == n:
@@ -59,21 +53,21 @@
     def run_task(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
-# To run the task as well as upstream workflow, use the `run_graph()` method.
+# To run the task as well as the upstreams, use the `run_graph()` method.
 ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
 # and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
-# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
+# `{$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
@@ -81,92 +75,53 @@
 # selectively discard the cache corresponding to the modification.
 Choose(3, 3).clear_task()
 
 # `ans` is recomputed tracing back to the computation of `Choose(3, 3)`.
 ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
-# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
+# equivalent to `rm -r {$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Task IO
 
-The arguments of the `build_task` method can be anything JSON serializable including `Task`s:
+The arguments of the `__init__` method can be anything JSON serializable + `Task`s:
 ```python
 class MyTask(TaskBase):
-    def build_task(self, param1, param2):
+    def __init__(self, param1, param2):
         ...
 
 MyTask(
     param1={
         'upstream_task0': UpstreamTask(),
         'other_params': [1, 2],
         ...
     },
     param2={ ... }
 }).run_graph()
 ```
 
-<!--
-Otherwise they can be passed via `Task` and `Req`:
+List/dict of upstream tasks can be registered with `RequiresList` and `RequiresDict`:
 ```python
-from taskproc import Task
-Dataset = ...  # Some complex data structure
-Model = ...    # Some complex data structure
-
-class LoadDataset(TaskBase):
-    def build_task(self):
-        pass
-
-    def run_task(self) -> Dataset:
-        ...
-
-class TrainModel(TaskBase):
-    dataset: Requires[Datset]
-
-    def build_task(self, dataset_task: Task[Dataset]):
-        self.dataset = dataset_task
-
-    def run_task(self) -> Model:
-        ...
-    
-class ScoreModel(TaskBase):
-    dataset: Requires[Datset]
-    model: Requires[Model]
-
-    def build_task(self, dataset_task: Task[Dataset], model_task: Task[Model]):
-        self.dataset = dataset_task
-        self.model = model_task
-
-    def run_task(self) -> float:
-        ...
-
-
-dataset_task = LoadDataset()
-model_task = TrainModel(dataset)
-score_task = ScoreModel(dataset, model)
-print(score_task.run_graph()
-```
-
-`Req` accepts a list/dict of tasks and automatically unfolds it.
-```python
-from taskproc import RequiresDict
-
+from taskproc import RequiresList, RequiresDict
 
 class SummarizeScores(TaskBase):
-    scores: RequiresDict[str, float] = Req()  # Again, type annotation or assignment may be omitted.
+    score_list: RequiresList[float]
+    score_dict: RequiresDict[str, float]
 
-    def build_task(self, task_dict: dict[str, Task[float]]):
-        self.scores = task_dict
+    def __init__(self, task_dict: dict[str, Task[float]]):
+        self.score_list = [MyScore(i) for i in range(10)]
+        self.score_dict = task_dict
 
     def run_task(self) -> float:
-        return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
+        # At runtime `self.score_list` and `self.score_dict` are evaluated as
+        # `list[float]` and `dict[str, float]`, respectively.
+        return sum(self.score_dict.values()) / len(self.score_dict)
 ```
--->
 
 The output of the `run_task` method should be serializable with `cloudpickle`,
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
 class NoCompressionTask(TaskBase, compress_level=0):
     ...
@@ -177,42 +132,53 @@
 class MultiOutputTask(TaskBase):
     def run_task(self) -> dict[str, int]:
         return {'foo': 42, ...}
 
 class DownstreamTask(TaskBase):
     dep: Requires[int]
 
-    def build_task(self):
+    def __init__(self):
         self.dep = MultiOutputTask()['foo']
 ```
 
-
-### Job scheduling and prefixes
-To run task on job schedulers, one can add prefix to the call of task.
-```python
-
-class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-interactive', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g']):
-    ...
-```
-
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
-`{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
+`{$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(TaskBase):
     def run_task(self) -> str:
         ...
         model_path = self.task_directory / 'model.bin'
         model.save(model_path)
         return model_path
 ```
 
+
+### Job scheduling and prefixes
+Tasks can be run with job schedulers using `prefix_command`, which will be inserted just before each task call.
+```python
+
+class TaskWithJobScheduler(TaskBase, prefix_command='jbsub -interactive -tty -queue x86_1h -cores 16+1 -mem 64g'):
+    ...
+```
+
+
+### Interactive tasks
+Interactive task is beneficial for debugging (e.g., with breakpoints) but harmful for parallel computing.
+In `taskproc`, all the tasks are executed detached by default.
+One can make them interactive by explicitly specifying like so:
+```python
+
+class InteractiveTask(TaskBase, interactive=True):
+    ...
+```
+
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 class MyTask(TaskBase):
@@ -239,25 +205,38 @@
 
 # Task-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
-We can use taskproc from commandline like `python -m taskproc.app path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
+We can use taskproc from commandline like `taskproc path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
 ```python
 # taskfile.py
 
 class Main(TaskBase):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/taskproc/...`.
-Please refer to `python -m taskproc.app --help` for more info.
+Please refer to `taskproc --help` for more info.
+
+
+### Built-in properties
+Here is the list of the built-in properties/methods of `TaskBase`:
 
-### Other useful properties
-* `TaskBase.task_id`: An integer id for each task
-* `TaskBase.task_args`: The argument of the task
-* `TaskBase.task_stdout`: path to the task's stdout
-* `TaskBase.task_stderr`: Path to the task's stderr
+| Name | Owner | Type | Description |
+|--|--|--|--|
+| `task_name`            | class    | property | String id of the task class |
+| `task_id`              | instance | property | Integer id of the task, unique within the same task class  |
+| `task_args`            | instance | property | The arguments of the task in JSON |
+| `task_directory`       | instance | property | Path to the data directory of the task |
+| `task_stdout`          | instance | property | Path to the task's stdout |
+| `task_stderr`          | instance | property | Path to the task's stderr |
+| `run_task`             | instance | method   | Run the task |
+| `run_graph`            | instance | method   | Run the task after necessary upstream tasks and save the results in the cache |
+| `run_graph_with_stats` | instance | method   | `run_graph` with additional statistics |
+| `get_task_result`      | instance | method   | Directly get the result of the task (fails if the cache is missing) |
+| `clear_task`           | instance | method   | Clear the cache of the task instance |
+| `clear_all_tasks`      | class    | method   | Clear the cache of the task class |
 
 ## TODO
 - [ ] Task graph visualizer
```

### Comparing `taskproc-0.11.2/pyproject.toml` & `taskproc-0.13.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [tool.poetry]
 name = "taskproc"
-version = "0.11.2"
+version = "0.13.0"
 description = "A lightweight task processing library written in pure Python"
 authors = ["Kohei Miyaguchi <koheimiyaguchi@gmail.com>"]
 license = "MIT License"
 homepage = "https://github.com/koheimiya/taskproc"
 repository = "https://github.com/koheimiya/taskproc"
 readme = "README.md"
 packages = [{include = "taskproc"}]
 
+[tool.poetry.scripts]
+taskproc = "taskproc.app:main"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "^4.5.0"
 diskcache = "^5.6.1"
 cloudpickle = "^2.2.1"
 networkx = "^3.1"
 click = "^8.1.3"
 tqdm = "^4.65.0"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+snakeviz = "^2.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `taskproc-0.11.2/taskproc/__init__.py` & `taskproc-0.13.0/taskproc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,17 @@
     - Automatic cache/data management (source code change detection, cache/data dependency tracking).
     - Task queue with rate limits.
 
 Limitations:
     - No priority-based scheduling.
 """
 from .types import Context
-from .task import infer_task_type, Task, TaskBase, Req, Requires, RequiresList, RequiresDict, Const
+from .task import Task, TaskBase, Req, Requires, RequiresList, RequiresDict, Const
+from .graph import FailedTaskError
 
 
 __EXPORT__ = [
-        infer_task_type, Task,
-        Const, TaskBase,
+        Task, Const, TaskBase,
         Req, Requires, RequiresList, RequiresDict,
-        Context
+        Context,
+        FailedTaskError
         ]
```

### Comparing `taskproc-0.11.2/taskproc/database.py` & `taskproc-0.13.0/taskproc/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,39 +56,27 @@
                 compress_level=compress_level,
                 id_table=IdTable(base_path / 'id_table')
                 )
 
     def __post_init__(self) -> None:
         self.results_directory.mkdir(exist_ok=True)
 
+    def get_instance_dir(self, key: Json, deps: dict[str, Path]) -> InstanceDirectory[T]:
+        return InstanceDirectory(
+                base_path=self.results_directory,
+                instance_id=self.id_table.get(key),
+                argkey=key,
+                dependencies=deps,
+                compress_level=self.compress_level,
+                )
+
     @property
     def results_directory(self) -> Path:
         return Path(self.base_path) / 'results'
 
-    def get_result_dir(self, key: Json) -> Path:
-        taskid = self.id_table.get(key)
-        out = self.results_directory / f'{taskid}'
-        if not out.exists():
-            out.mkdir()
-            with open(out / 'args.json', 'w') as ref:
-                ref.write(key)
-        return out
-
-    def get_result_path(self, key: Json) -> Path:
-        return self.get_result_dir(key) / f'result.pkl.gz'
-
-    def get_stdout_path(self, key: Json) -> Path:
-        return self.get_result_dir(key) / f'stdout.txt'
-
-    def get_stderr_path(self, key: Json) -> Path:
-        return self.get_result_dir(key) / f'stderr.txt'
-
-    def get_data_dir(self, key: Json) -> Path:
-        return self.get_result_dir(key) / 'data'
-
     @property
     def source_path(self) -> Path:
         return Path(self.base_path) / 'source.txt'
 
     def update_source_if_necessary(self, source: str) -> datetime:
         # Update source cache
         if self.source_path.exists():
@@ -98,71 +86,128 @@
         if cached_source != source:
             open(self.source_path, 'w').write(source)
         return self.load_source_timestamp()
 
     def load_source_timestamp(self) -> datetime:
         return _get_timestamp(self.source_path)
 
-    def save(self, key: Json, obj: T) -> datetime:
-        path = self.get_result_path(key)
-        with gzip.open(path, 'wb', compresslevel=self.compress_level) as ref:
-            cloudpickle.dump(obj, ref)
-        return _get_timestamp(path)
-
-    def load(self, key: Json) -> T:
-        path = self.get_result_path(key)
-        with gzip.open(path, 'rb') as ref:
-            return cloudpickle.load(ref)
-
-    def load_timestamp(self, key: Json) -> datetime:
-        path = self.get_result_path(key)
-        if path.exists():
-            return _get_timestamp(path)
-        else:
-            raise KeyError(key)
-
     def clear(self) -> None:
         self.id_table.clear()
         if self.results_directory.exists():
             shutil.rmtree(self.results_directory)
         self.results_directory.mkdir()
 
-    def delete(self, key: Json) -> None:
-        resdir = self.get_result_path(key)
-        if resdir.exists():
-            resdir.unlink()
-        else:
-            raise KeyError(key)
-        datadir = self.get_data_dir(key)
-        if datadir.exists():
-            shutil.rmtree(datadir)
-
 
 def _get_timestamp(path: Path) -> datetime:
     timestamp = path.stat().st_mtime_ns / 10 ** 9
     return datetime.fromtimestamp(timestamp)
 
 
+class InstanceDirectory(Generic[T]):
+    def __init__(self, base_path: Path, instance_id: int, argkey: Json, dependencies: dict[str, Path], compress_level: int):
+        self.base_path = base_path
+        self.task_id = instance_id
+        self.argkey = argkey
+        self.dependencies = dependencies
+        self.compress_level = compress_level
+        self.initialize()
+
+    def initialize(self):
+        if self.path.exists():
+            shutil.rmtree(self.path)
+        self.path.mkdir()
+        with open(self.args_path, 'w') as ref:
+            ref.write(self.argkey)
+        self.data_dir.mkdir()
+        self.deps_dir.mkdir()
+        if self.dependencies:
+            for name, target in self.dependencies.items():
+                link_path = self.deps_dir / name
+                link_path.symlink_to(target.resolve())
+        else:
+            (self.deps_dir / '__NO_DEPENDENCIES__').touch()
+
+    @property
+    def path(self):
+        return self.base_path / str(self.task_id)
+
+    @property
+    def args_path(self) -> Path:
+        return self.path / 'args.json'
+
+    @property
+    def result_path(self) -> Path:
+        return self.path / f'result.pkl.gz'
+
+    @property
+    def stdout_path(self) -> Path:
+        return self.path / f'stdout.txt'
+
+    @property
+    def stderr_path(self) -> Path:
+        return self.path / f'stderr.txt'
+
+    @property
+    def data_dir(self) -> Path:
+        return self.path / 'data'
+
+    @property
+    def deps_dir(self) -> Path:
+        return self.path / 'deps'
+
+    def save_result(self, obj: T) -> datetime:
+        path = self.result_path
+        with gzip.open(path, 'wb', compresslevel=self.compress_level) as ref:
+            cloudpickle.dump(obj, ref)
+        return _get_timestamp(path)
+
+    def load_result(self) -> T:
+        path = self.result_path
+        with gzip.open(path, 'rb') as ref:
+            return cloudpickle.load(ref)
+
+    def get_timestamp(self) -> datetime:
+        path = self.result_path
+        if self.result_path.exists():
+            return _get_timestamp(path)
+        else:
+            raise RuntimeError(f'Result not found: {self.result_path}')
+
+    def delete(self) -> None:
+        self.initialize()
+
+
 @dataclass
 class IdTable:
     def __init__(self, path: Path | str) -> None:
         self.table = dc.Cache(directory=path)
+        self.lock = dc.Lock(self.table, 'global')
+        self.cache: dict[Any, int] = {}
     
     def get(self, x: Any) -> int:
-        with self.table as ref:
-            try:
-                return ref[x]
-            except KeyError:
-                n = len(ref)
-                ref[x] = n
-                return n
+        out = self.cache.get(x)
+        if out is not None:
+            return out
+
+        # with self.lock:
+        with self.table.transact():
+            value = self.table.get(key=x)
+            if value is None:
+                value = len(self.table)
+                self.table.set(key=x, value=value)
+
+        self.cache[x] = value
+        return value
 
     def __contains__(self, key: Any) -> bool:
-        with self.table as ref:
-            return key in ref
+        # with self.lock:
+        return key in self.table
 
     def list_keys(self) -> list[str]:
-        with self.table as ref:
-            return list(map(str, ref))
+        # with self.lock:
+        # with self.table as ref:
+        with self.table.transact():
+            return list(map(str, self.table))
 
     def clear(self) -> None:
+        # with self.lock:
         self.table.clear()
```

### Comparing `taskproc-0.11.2/taskproc/graph.py` & `taskproc-0.13.0/taskproc/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 """ DAG processor """
 from __future__ import annotations
+from contextlib import ExitStack
 from datetime import datetime
-from typing import Any, Sequence
+from typing import Any, Mapping
 from typing_extensions import Self, runtime_checkable, Protocol
 from collections import defaultdict
 from dataclasses import dataclass
-from concurrent.futures import Future, wait, FIRST_COMPLETED, Executor
+from concurrent.futures import Future, ProcessPoolExecutor, wait, FIRST_COMPLETED, Executor
+from pathlib import Path
 import logging
 
 from tqdm.auto import tqdm
 import cloudpickle
 import networkx as nx
 
-from .types import Json, TaskKey
+from .types import Json, TaskKey, Context
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 ChannelLabels = tuple[str, ...]
 
 
 @runtime_checkable
 class TaskHandlerProtocol(Protocol):
     @property
     def channels(self) -> ChannelLabels: ...
     @property
     def source_timestamp(self) -> datetime: ...
+    @property
+    def is_interactive(self) -> bool: ...
+    @property
+    def directory(self) -> Path: ...
     def to_tuple(self) -> TaskKey: ...
-    def get_prerequisites(self) -> Sequence[TaskHandlerProtocol]: ...
+    def get_prerequisites(self) -> Mapping[str, TaskHandlerProtocol]: ...
     def peek_timestamp(self) -> datetime | None: ...
-    def set_result(self) -> None: ...
+    def set_result(self, on_child_process: bool) -> None: ...
+    def log_error(self) -> None: ...
 
 
 @dataclass
 class TaskGraph:
     G: nx.DiGraph
     detect_source_change: bool
 
@@ -44,15 +51,15 @@
         seen: set[TaskKey] = set()
         to_expand = [root]
         while to_expand:
             task = to_expand.pop()
             x = task.to_tuple()
             if x not in seen:
                 seen.add(x)
-                prerequisite_tasks = task.get_prerequisites()
+                prerequisite_tasks = list(task.get_prerequisites().values())
                 to_expand.extend(prerequisite_tasks)
                 G.add_node(x, task=task, timestamp=task.peek_timestamp(), source_timestamp=task.source_timestamp)
                 G.add_edges_from([(p.to_tuple(), x) for p in prerequisite_tasks])
         out = TaskGraph(G, detect_source_change=detect_source_change)
         out.trim()
         return out
 
@@ -118,42 +125,61 @@
     def get_nodes_by_task(self) -> dict[str, list[Json]]:
         out: dict[str, list[Json]] = defaultdict(list)
         for x in self.G:
             path, args = x
             out[path].append(args)
         return dict(out)
 
+    def interactive_tasks(self) -> list[TaskKey]:
+        return [x for x in self.G if self.get_task(x).is_interactive]
+
 
 def run_task_graph(
         graph: TaskGraph,
         executor: Executor,
         rate_limits: dict[str, int] | None = None,
         dump_graphs: bool = False,
         show_progress: bool = False,
         ) -> dict[str, Any]:
     """ Consume task graph concurrently.
     """
+    interactive_tasks = graph.interactive_tasks()
+    if interactive_tasks and isinstance(executor, ProcessPoolExecutor):
+        LOGGER.warning(f'Interactive task is detected while the executor is ProcessPoolExecutor: {interactive_tasks!r}. Override it with ThreadPoolExecutor.')
+        executor = Context.get_executor(executor_name='thread')
+    if interactive_tasks and show_progress:
+        LOGGER.warning(f'Interactive task is detected while `show_progress` is set True. The progress bars may interfere with the task output.')
+
+
     stats = {k: len(args) for k, args in graph.get_nodes_by_task().items()}
     LOGGER.debug(f'Following tasks will be called: {stats}')
     info = {'stats': stats, 'generations': []}
 
     if show_progress:
-        progressbars = {k: tqdm(range(n), desc=k, position=i) for i, (k, n) in enumerate(stats.items())}
+        progressbars = {
+                k: tqdm(range(n), desc=k, position=i, mininterval=.1, maxinterval=1)
+                for i, (k, n) in enumerate(stats.items())
+                }
     else:
         progressbars = {}
 
     # Read concurrency budgets
     if rate_limits is None:
         rate_limits = {}
     occupied = {k: 0 for k in rate_limits}
 
     # Execute tasks
     standby = graph.get_initial_tasks()
-    in_process: set[Future[tuple[ChannelLabels, TaskKey]]] = set()
-    with executor as executor:
+    in_process: dict[Future[tuple[ChannelLabels, TaskKey]], TaskKey] = dict()
+
+    with ExitStack() as stack:
+        for pbar in progressbars.values():
+            stack.enter_context(pbar)
+        executor = stack.enter_context(executor)
+
         while standby or in_process:
             # Log some stats
             LOGGER.debug(
                     f'nodes: {graph.size}, '
                     f'standby: {len(standby)}, '
                     f'in_process: {len(in_process)}'
                     )
@@ -171,24 +197,26 @@
                             occupied[q] += len(to_submit)
                     if to_hold:
                         leftover[queue] = to_hold
                 else:
                     to_submit = keys
 
                 for key in to_submit:
-                    future = executor.submit(_run_task, queue, cloudpickle.dumps(graph.get_task(key)))
-                    in_process.add(future)
+                    future = executor.submit(_run_task, queue, cloudpickle.dumps(graph.get_task(key)), isinstance(executor, ProcessPoolExecutor))
+                    in_process[future] = key
 
             # Wait for the first tasks to complete
-            done, in_process = wait(in_process, return_when=FIRST_COMPLETED)
+            done, _ = wait(in_process.keys(), return_when=FIRST_COMPLETED)
 
             # Update graph
             standby = defaultdict(list, leftover)
             for done_future in done:
-                queue_done, x_done = done_future.result()
+                queue_done, x_done = try_getting_result(done_future, task_key=in_process[done_future], graph=graph)
+
+                del in_process[done_future]
                 if show_progress:
                     progressbars[x_done[0]].update()
 
                 # Update occupied
                 for q in queue_done:
                     if q in occupied:
                         occupied[q] -= 1
@@ -197,21 +225,33 @@
                 # Remove node from graph
                 ys = graph.pop_with_new_leaves(x_done)
 
                 # Update standby
                 for queue, task in ys.items():
                     standby[queue].extend(task)
 
-    for pbar in progressbars.values():
-        pbar.close()
-
     # Sanity check
     assert graph.size == 0, f'Graph is not empty. Should not happen.'
     assert all(n == 0 for n in occupied.values()), 'Incorrect task count. Should not happen.'
     return info
 
 
-def _run_task(queue: ChannelLabels, task_data: bytes) -> tuple[ChannelLabels, TaskKey]:  # queue, (dbname, key)
+def _run_task(queue: ChannelLabels, task_data: bytes, on_child_process: bool) -> tuple[ChannelLabels, TaskKey]:  # queue, (dbname, key)
     task = cloudpickle.loads(task_data)
     assert isinstance(task, TaskHandlerProtocol)
-    task.set_result()
+    task.set_result(on_child_process=on_child_process)
     return queue, task.to_tuple()
+
+
+class FailedTaskError(Exception):
+    def __init__(self, task: TaskHandlerProtocol, exception: Exception, msg: str):
+        super().__init__(msg)
+        self.task = task
+        self.exception = exception
+
+
+def try_getting_result(future: Future[tuple[ChannelLabels, TaskKey]], task_key: TaskKey, graph: TaskGraph) -> tuple[ChannelLabels, TaskKey]:
+    try:
+        return future.result()
+    except Exception as e:
+        task = graph.get_task(task_key)
+        raise FailedTaskError(task, e, msg=f'Exception occurred in {task_key}, see logs at {str(task.directory)}') from e
```

### Comparing `taskproc-0.11.2/taskproc/task.py` & `taskproc-0.13.0/taskproc/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import annotations
-from abc import ABC, abstractmethod
 from collections.abc import Iterable
-from contextlib import redirect_stderr, redirect_stdout
+from contextlib import redirect_stderr, redirect_stdout, ExitStack
 from typing import Callable, Generic, Mapping, Protocol, Sequence, Type, TypeVar, Any, cast
 from typing_extensions import ParamSpec, Self, get_origin, overload
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 from concurrent.futures import Executor
+from functools import cached_property, wraps
 import ast
 import logging
 import inspect
 import json
 import shutil
-import subprocess
-import tempfile
 import cloudpickle
-import gzip
+import subprocess
 import sys
 
 
 from .types import Json, TaskKey, Context
 from .database import Database
 from .graph import TaskGraph, run_task_graph
 
@@ -32,194 +30,239 @@
 T = TypeVar('T')
 S = TypeVar('S')
 U = TypeVar('U')
 P = ParamSpec('P')
 R = TypeVar('R', covariant=True)
 
 
-class TaskConfig(Generic[P, R]):
+class TaskConfig(Generic[R]):
     """ Information specific to a task class (not instance) """
     def __init__(
             self,
-            task_class: Type[TaskType[P, R]],
+            task_class: Type[TaskBase[R]],
             channels: tuple[str, ...],
             compress_level: int,
-            job_prefix: list[str] | None,
-            detach_output: bool,
+            prefix_command: str,
+            interactive: bool,
             ) -> None:
 
         self.task_class = task_class
         self.name = _serialize_function(task_class)
-        self.db = Database.make(name=self.name, compress_level=compress_level)
+        self.compress_level = compress_level
         self.channels = (self.name,) + channels
-        self.job_prefix = job_prefix
-        self.detach_output = detach_output
+        self.prefix_command = prefix_command
+        self.interactive = interactive
+        if self.interactive and self.prefix_command:
+            LOGGER.warning(f'`interactive` is set True, nullifying the effect of `prefix_command`={self.prefix_command!r}')
         self.worker_registry: dict[Json, TaskWorker[R]] = {}
 
-        source = inspect.getsource(task_class)
+
+    @cached_property
+    def db(self) -> Database[R]:
+        return Database.make(name=self.name, compress_level=self.compress_level)
+
+    @cached_property
+    def source_timestamp(self) -> datetime:
+        source = inspect.getsource(self.task_class)
         formatted_source = ast.unparse(ast.parse(source))
-        self.source_timestamp = self.db.update_source_if_necessary(formatted_source)
+        return self.db.update_source_if_necessary(formatted_source)
 
     def clear_all(self) -> None:
         self.db.clear()
 
 
 class TaskWorker(Generic[R]):
     @classmethod
-    def make(cls, config: TaskConfig[P, R], instance: TaskType[P, R], *args: P.args, **kwargs: P.kwargs) -> Self:
-        arg_key = _serialize_arguments(instance.build_task, *args, **kwargs)
-        worker = config.worker_registry.get(arg_key, None)
+    def make(cls, task_config: TaskConfig[R], task_instance: TaskBase[R], *args: Any, **kwargs: Any) -> Self:
+        arg_key = _serialize_arguments(task_instance._build_task, *args, **kwargs)
+        worker = task_config.worker_registry.get(arg_key, None)
         if worker is not None:
             return worker
 
-        instance.build_task(*args, **kwargs)
-        worker = TaskWorker[R](config=config, instance=instance, arg_key=arg_key)
-        config.worker_registry[arg_key] = worker
+        task_instance._build_task(*args, **kwargs)
+        worker = TaskWorker[R](config=task_config, instance=task_instance, arg_key=arg_key)
+        task_config.worker_registry[arg_key] = worker
         return worker
 
-    def __init__(self, config: TaskConfig[..., R], instance: TaskType[..., R], arg_key: Json) -> None:
+    def __init__(self, config: TaskConfig[R], instance: TaskBase[R], arg_key: Json) -> None:
         self.config = config
         self.instance = instance
         self.arg_key = arg_key
+        self.dirobj = config.db.get_instance_dir(
+                key=arg_key,
+                deps={k: w.dirobj.path for k, w in self.get_prerequisites().items()}
+                )
 
     @property
     def channels(self) -> tuple[str, ...]:
         return self.config.channels
 
     @property
     def source_timestamp(self) -> datetime:
         return self.config.source_timestamp
 
     def to_tuple(self) -> TaskKey:
         return (self.config.name, self.arg_key)
 
-    def get_prerequisites(self) -> Sequence[TaskWorker[Any]]:
+    def get_prerequisites(self) -> dict[str, TaskWorker[Any]]:
         cls = self.config.task_class
         inst = self.instance
-        prerequisites: list[TaskWorker[Any]] = []
-        for _, v in inspect.getmembers(cls):
+        prerequisites: dict[str, TaskWorker[Any]] = {}
+        for name, v in inspect.getmembers(cls):
             if isinstance(v, Req):
-                prerequisites.extend([task._task_worker for task in v.get_task_list(inst)])
-        assert all(isinstance(p, TaskWorker) for p in prerequisites)
+                for k, task in v.get_task_dict(inst).items():
+                    if k is None:
+                        prerequisites[f'{name}'] = task._task_worker
+                    else:
+                        prerequisites[f'{name}.{k}'] = task._task_worker
+        assert all(isinstance(p, TaskWorker) for p in prerequisites.values())
         return prerequisites
 
     def peek_timestamp(self) -> datetime | None:
         try:
-            return self.config.db.load_timestamp(self.arg_key)
-        except KeyError:
+            # return self.config.db.load_timestamp(self.arg_key)
+            return self.dirobj.get_timestamp()
+        except RuntimeError:
             return None
 
-    def set_result(self) -> None:
-        db = self.config.db
-        if self.directory.exists():
-            shutil.rmtree(self.directory)
-        out = self.run_instance_task()
-        db.save(self.arg_key, out)
-
-    def run_instance_task(self) -> R:
-        job_prefix = self.config.job_prefix
-        if job_prefix is None:
-            return self._run_task_with_captured_output()
+    def set_result(self, on_child_process: bool = False) -> None:
+        self.dirobj.initialize()
+        self.run_and_save_instance_task(on_child_process=on_child_process)
+
+    def log_error(self) -> None:
+        if not self.config.interactive:
+            task_info = {
+                    'name': self.config.name,
+                    'id': self.task_id,
+                    'args': self.task_args,
+                    }
+            LOGGER.error(f'Error occurred while running detached task {task_info}')
+            LOGGER.error(f'Here is the detached stdout ({self.stdout_path}):')
+            with open(self.stdout_path) as f:
+                LOGGER.error(f.read())
+            LOGGER.error(f'Here is the detached stderr ({self.stderr_path}):')
+            with open(self.stderr_path) as f:
+                LOGGER.error(f.read())
+
+    def run_and_save_instance_task(self, on_child_process: bool) -> None:
+        if self.config.interactive:
+            res = self.instance.run_task()
+            # self.config.db.save(self.arg_key, res)
+            self.dirobj.save_result(res)
+        elif on_child_process and self.config.prefix_command == '':
+            res = self.run_instance_task_with_captured_output()
+            # self.config.db.save(self.arg_key, res)
+            self.dirobj.save_result(res)
         else:
-            with tempfile.TemporaryDirectory() as dir_ref:
+            dir_ref = self.directory / 'tmp'
+            if dir_ref.exists():
+                shutil.rmtree(dir_ref)
+            dir_ref.mkdir()
+            try:
                 worker_path = Path(dir_ref) / 'worker.pkl'
-                result_path = Path(dir_ref) / 'result.pkl'
-                pycmd = f"""import gzip, cloudpickle
-                    worker = cloudpickle.load(gzip.open("{worker_path}", "rb"))
-                    res = worker._run_task_with_captured_output()
-                    cloudpickle.dump(res, gzip.open("{result_path}", "wb"))
-                """.replace('\n', ';')
-                with gzip.open(worker_path, 'wb') as worker_ref:
+                pycmd = f"""import pickle
+worker = pickle.load(open("{worker_path}", "rb"))
+res = worker.run_instance_task_with_captured_output()
+worker.dirobj.save_result(res)
+""".replace('\n', '; ')
+
+                with open(worker_path, 'wb') as worker_ref:
                     cloudpickle.dump(self, worker_ref)
+
+                shell_command = ' '.join([self.config.prefix_command, sys.executable, '-c', repr(pycmd)])
                 res = subprocess.run(
-                        ' '.join([*job_prefix, sys.executable, '-c', repr(pycmd)]),
-                        capture_output=True, check=True, shell=True,
+                        shell_command,
+                        shell=True, text=True,
+                        capture_output=True,
                         )
-                print(res.stdout.decode(), end='')
-                print(res.stderr.decode(), end='', file=sys.stderr)
+                def _prepend(path: Path, text: str):
+                    try:
+                        original_contents = open(path, 'r').read()
+                    except:
+                        original_contents = f'<error while loading {str(path)}>'
+
+                    with open(path, 'w') as f:
+                        f.write('=== caller log ===\n')
+                        f.write(text)
+                        f.write('=== callee log ===\n')
+                        f.write(original_contents)
+                _prepend(self.stdout_path, res.stdout)
+                _prepend(self.stderr_path, res.stderr)
                 res.check_returncode()
-                with gzip.open(result_path, 'rb') as result_ref:
-                    return cloudpickle.load(result_ref)
+            finally:
+                shutil.rmtree(dir_ref)
 
-    def _run_task_with_captured_output(self) -> R:
-        if not self.config.detach_output:
-            return self.instance.run_task()
 
-        try:
-            with open(self.stdout_path, 'w+') as stdout:
-                with open(self.stderr_path, 'w+') as stderr:
-                    with redirect_stdout(stdout):
-                        with redirect_stderr(stderr):
-                            return self.instance.run_task()
-        except:
-            task_info = {
-                    'name': self.config.name,
-                    'id': self.task_id,
-                    'args': self.task_args,
-                    }
-            LOGGER.error(f'Error occurred while running task {task_info}')
-            LOGGER.error(f'Here is the stdout ({self.stdout_path}):')
-            for line in open(self.stdout_path).readlines():
-                LOGGER.error(line)
-            LOGGER.error(f'Here is the stderr ({self.stderr_path}):')
-            for line in open(self.stderr_path).readlines():
-                LOGGER.error(line)
-            raise
+    def run_instance_task_with_captured_output(self) -> R:
+        with ExitStack() as stack:
+            stdout = stack.enter_context(open(self.stdout_path, 'w+'))
+            stderr = stack.enter_context(open(self.stderr_path, 'w+'))
+            stack.enter_context(redirect_stdout(stdout))
+            stack.callback(lambda: stdout.flush())
+            stack.enter_context(redirect_stderr(stderr))
+            stack.callback(lambda: stderr.flush())
+            return self.instance.run_task()
+        raise NotImplementedError('Should not happen')
 
     @property
     def task_id(self) -> int:
-        return self.config.db.id_table.get(self.arg_key)
+        return self.dirobj.task_id
 
     @property
     def task_args(self) -> dict[str, Any]:
         return json.loads(self.arg_key)
 
     @property
+    def is_interactive(self) -> bool:
+        return self.config.interactive
+
+    @property
     def stdout_path(self) -> Path:
-        return self.config.db.get_stdout_path(self.arg_key)
+        return self.dirobj.stdout_path
 
     @property
     def stderr_path(self) -> Path:
-        return self.config.db.get_stderr_path(self.arg_key)
+        return self.dirobj.stderr_path
 
     @property
-    def _directory_uninit(self) -> Path:
-        _, arg_str = self.to_tuple()
-        return self.config.db.get_data_dir(arg_str)
+    def directory(self) -> Path:
+        return self.dirobj.path
 
     @property
-    def directory(self) -> Path:
-        out = self._directory_uninit
-        out.mkdir(exist_ok=True)
-        return out
+    def data_directory(self) -> Path:
+        return self.dirobj.data_dir
 
     def get_result(self) -> R:
-        return self.config.db.load(self.arg_key)
+        result_key = '_task__result_'
+        res = getattr(self.instance, result_key, None)
+        if res is None:
+            res = self.dirobj.load_result()
+            setattr(self.instance, result_key, res)
+        return res
 
     def clear(self) -> None:
-        db = self.config.db
-        try:
-            db.delete(self.arg_key)
-        except KeyError:
-            pass
-        directory = self._directory_uninit
-        if directory.exists():
-            shutil.rmtree(directory)
-
-
-class TaskType(Generic[P, R], ABC):
-    _task_config: TaskConfig[P, R]
-
-    @abstractmethod
-    def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None:
-        pass
+        self.dirobj.delete()
+
+
+class TaskBase(Generic[R]):
+    _task_config: TaskConfig[R]
+
+    def __init__(self) -> None:
+        ...
+
+    def __task_init__(self, *args: Any, **kwargs: Any) -> None:
+        self._task_worker: TaskWorker[R] = TaskWorker.make(
+                self._task_config, self, *args, **kwargs
+                )
+
+    def _build_task(self, *args: Any, **kwargs: Any) -> None:
+        ...
 
-    @abstractmethod
     def run_task(self) -> R:
-        pass
+        ...
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         _channel = kwargs.pop('channel', None)
         channels: tuple[str, ...]
         if isinstance(_channel, str):
             channels = (_channel,)
         elif isinstance(_channel, Iterable):
@@ -227,41 +270,46 @@
             assert all(isinstance(q, str) for q in channels)
         elif _channel is None:
             channels = tuple()
         else:
             raise ValueError('Invalid channel value:', _channel)
 
         compress_level = kwargs.pop('compress_level', 9)
-        job_prefix = kwargs.pop('job_prefix', None)
-        detach_output = kwargs.pop('detach_output', True)
+        prefix_command = kwargs.pop('prefix_command', '')
+        interactive = kwargs.pop('interactive', False)
 
         # Fill missing requirement
         ann = inspect.get_annotations(cls, eval_str=True)
         for k, v in ann.items():
             if get_origin(v) is Req and getattr(cls, k, None) is None:
                 req = Req()
                 req.__set_name__(None, k)
                 setattr(cls, k, req)
 
-        cls._task_config = TaskConfig(task_class=cls, channels=channels, compress_level=compress_level, job_prefix=job_prefix, detach_output=detach_output)
-        super().__init_subclass__(**kwargs)
-
-    def __init__(self, *args: P.args, **kwargs: P.kwargs) -> None:
-        self._task_worker: TaskWorker[R] = TaskWorker.make(
-                self._task_config, self, *args, **kwargs
+        cls._task_config = TaskConfig(
+                task_class=cls,
+                channels=channels,
+                compress_level=compress_level,
+                prefix_command=prefix_command,
+                interactive=interactive,
                 )
 
+        # Swap initializer to make __init__ lazy
+        cls._build_task = cls.__init__  # type: ignore
+        cls.__init__ = wraps(cls._build_task)(cls.__task_init__)
+        super().__init_subclass__(**kwargs)
+
     @classmethod
     @property
     def task_name(cls) -> str:
         return cls._task_config.name
 
     @property
     def task_directory(self) -> Path:
-        return self._task_worker.directory
+        return self._task_worker.data_directory
 
     @property
     def task_id(self) -> int:
         return self._task_worker.task_id
 
     @property
     def task_args(self) -> dict[str, Any]:
@@ -279,64 +327,70 @@
     def clear_all_tasks(cls) -> None:
         cls._task_config.clear_all()
 
     def clear_task(self) -> None:
         self._task_worker.clear()
 
     def run_graph(
-            self, *,
+            self: TaskClassProtocol[T], *,
             executor: Executor | None = None,
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
             show_progress: bool = False,
-            ) -> R:
+            ) -> T:
+        assert isinstance(self, TaskBase)
         return self.run_graph_with_stats(
                 executor=executor,
                 max_workers=max_workers,
                 rate_limits=rate_limits,
                 detect_source_change=detect_source_change,
                 show_progress=show_progress,
                 )[0]
 
     def run_graph_with_stats(
-            self, *,
+            self: TaskClassProtocol[T], *,
             executor: Executor | None = None,
             max_workers: int | None = None,
             rate_limits: dict[str, int] | None = None,
             detect_source_change: bool | None = None,
             dump_generations: bool = False,
             show_progress: bool = False,
-            ) -> tuple[R, dict[str, Any]]:
+            ) -> tuple[T, dict[str, Any]]:
+        assert isinstance(self, TaskBase)
         if detect_source_change is None:
             detect_source_change = Context.detect_source_change
         graph = TaskGraph.build_from(self._task_worker, detect_source_change=detect_source_change)
 
         if executor is None:
             executor = Context.get_executor(max_workers=max_workers)
         else:
             assert max_workers is None
+
         stats = run_task_graph(graph=graph, executor=executor, rate_limits=rate_limits, dump_graphs=dump_generations, show_progress=show_progress)
         return self._task_worker.get_result(), stats
 
     def get_task_result(self) -> R:
         return self._task_worker.get_result()
 
-    def __getitem__(self: TaskType[..., Mapping[K, T]], key: K) -> _MappedTask[K, T]:
+    @overload
+    def __getitem__(self: TaskClassProtocol[Sequence[T]], key: int) -> _MappedTask[T]: ...
+    @overload
+    def __getitem__(self: TaskClassProtocol[Mapping[K, T]], key: K) -> _MappedTask[T]: ...
+    def __getitem__(self: TaskClassProtocol[Mapping[K, T] | Sequence[T]], key: int | K) -> _MappedTask[T]:
         return _MappedTask(self, key)
 
 
-class TaskClassProtocol(Protocol[P, R]):
-    def build_task(self, *args: P.args, **kwargs: P.kwargs) -> None: ...
+class TaskClassProtocol(Protocol[R]):
+    def __task_init__(self, *args: Any, **kwargs: Any) -> None: ...
     def run_task(self) -> R: ...
 
 
-def infer_task_type(cls: Type[TaskClassProtocol[P, R]]) -> Type[TaskType[P, R]]:
-    assert issubclass(cls, TaskType), f'{cls} must inherit from {TaskType} to infer task type.'
-    return cast(Type[TaskType[P, R]], cls)
+def cast_task(task: TaskClassProtocol[R]) -> TaskBase[R]:
+    return cast(TaskBase[R], task)
 
 
 def _serialize_function(fn: Callable[..., Any]) -> str:
     return f'{fn.__module__}.{fn.__qualname__}'
 
 
 def _normalize_arguments(fn: Callable[P, Any], *args: P.args, **kwargs: P.kwargs) -> dict[str, Any]:
@@ -348,117 +402,117 @@
 def _serialize_arguments(fn: Callable[P, Any], *args: P.args, **kwargs: P.kwargs) -> Json:
     arguments = _normalize_arguments(fn, *args, **kwargs)
     return cast(Json, json.dumps(arguments, separators=(',', ':'), sort_keys=True, cls=CustomJSONEncoder))
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     def default(self, o):
-        if isinstance(o, TaskType):
+        if isinstance(o, TaskBase):
             name, keys = o._task_worker.to_tuple()
             return {'__task__': name, '__args__': json.loads(keys)}
         elif isinstance(o, _MappedTask):
             out = self.default(o.get_origin())
             out['__key__'] = o.get_args()
             return out
         else:
             # Let the base class default method raise the TypeError
             return super().default(o)
 
 
 @dataclass
-class _MappedTask(Generic[K, T]):
-    task: TaskType[..., Mapping[K, T]] | _MappedTask[Any, Mapping[K, T]]
-    key: K
+class _MappedTask(Generic[R]):
+    task: TaskClassProtocol[Mapping[Any, R] | Sequence[R]] | _MappedTask[Mapping[Any, R] | Sequence[R]]
+    key: Any
 
-    def get_origin(self) -> TaskType[..., Any]:
+    def get_origin(self) -> TaskBase[Any]:
         x = self.task
         if isinstance(x, _MappedTask):
             return x.get_origin()
         else:
-            return x
+            return cast_task(x)
 
     def get_args(self) -> list[Any]:
         out = []
         x = self
         while isinstance(x, _MappedTask):
             out.append(x.key)
             x = x.task
         return out[::-1]
 
-    def get_task_result(self) -> T:
+    def get_task_result(self) -> R:
         out = self.get_origin().get_task_result()
         for k in self.get_args():
             out = out[k]
         return out
 
+    @overload
+    def __getitem__(self: _MappedTask[Sequence[T]], key: int) -> _MappedTask[T]: ...
+    @overload
+    def __getitem__(self: _MappedTask[Mapping[K, T]], key: K) -> _MappedTask[T]: ...
+    def __getitem__(self: _MappedTask[Mapping[K, T] | Sequence[T]], key: int | K) -> _MappedTask[T]:
+        return _MappedTask(self, key)
+
 
 class Req(Generic[T, R]):
     def __set_name__(self, _: Any, name: str) -> None:
         self.public_name = name
         self.private_name = '_requires__' + name
 
-    def __set__(self, obj: TaskType[..., Any], value: T) -> None:
+    def __set__(self, obj: TaskBase[Any], value: T) -> None:
         setattr(obj, self.private_name, value)
 
     @overload
-    def __get__(self: Requires[U], obj: TaskType[..., Any], _=None) -> U: ...
+    def __get__(self: Requires[U], obj: TaskBase[Any], _=None) -> U: ...
     @overload
-    def __get__(self: RequiresList[U], obj: TaskType[..., Any], _=None) -> list[U]: ...
+    def __get__(self: RequiresList[U], obj: TaskBase[Any], _=None) -> list[U]: ...
     @overload
-    def __get__(self: RequiresDict[K, U], obj: TaskType[..., Any], _=None) -> dict[K, U]: ...
-    def __get__(self, obj: TaskType[..., Any], _=None) -> Any:
+    def __get__(self: RequiresDict[K, U], obj: TaskBase[Any], _=None) -> dict[K, U]: ...
+    def __get__(self, obj: TaskBase[Any], _=None) -> Any:
 
-        def get_result(task_like: TaskLike[S]) -> S:
-            if isinstance(task_like, (TaskType, _MappedTask, Const)):
+        def get_result(task_like: Task[S]) -> S:
+            if isinstance(task_like, (TaskBase, _MappedTask, Const)):
                 return task_like.get_task_result()
             else:
                 raise TypeError(f'Unsupported requirement type: {type(task_like)}')
 
         x = getattr(obj, self.private_name)
         if isinstance(x, list):
             return [get_result(t) for t in x]
         elif isinstance(x, dict):
             return {k: get_result(v) for k, v in x.items()}
         else:
             return get_result(x)
 
-    def get_task_list(self, obj: TaskType[..., Any]) -> list[TaskType[..., Any]]:
+    def get_task_dict(self, obj: TaskBase[Any]) -> dict[str | None, TaskBase[Any]]:
         x = getattr(obj, self.private_name, None)
         assert x is not None, f'Requirement `{self.public_name}` is not set in {obj}.'
 
         if isinstance(x, _MappedTask):
             x = x.get_origin()
 
-        if isinstance(x, TaskType):
-            return [x]
+        if isinstance(x, TaskBase):
+            return {None: x}
         elif isinstance(x, list):
-            return x
+            return {str(i): xi for i, xi in enumerate(x)}
         elif isinstance(x, dict):
-            return list(x.values())
+            return {str(k): v for k, v in x.items()}
         elif isinstance(x, Const):
-            return []
+            return {}
         else:
             raise TypeError(f'Unsupported requirement type: {type(x)}')
 
 
 @dataclass(frozen=True)
 class Const(Generic[R]):
     value: R
 
     def get_task_result(self) -> R:
         return self.value
 
 
-Task = TaskType[..., R] | _MappedTask[Any, R]
-TaskLike = Task[R] | Const[R]
-
-
-Requires = Req[TaskLike[R], R]
-RequiresList = Req[Sequence[TaskLike[R]], list[R]]
-RequiresDict = Req[Mapping[K, TaskLike[R]], dict[K, R]]
+RealTask = TaskClassProtocol[R] | _MappedTask[R]
+Task = RealTask[R] | Const[R]
 
 
-class TaskBase(TaskType):
-    def build_task(self) -> None:
-        pass
-    def run_task(self) -> None:
-        pass
+Requires = Req[Task[R], R]
+RequiresList = Req[Sequence[Task[R]], list[R]]
+RequiresDict = Req[Mapping[K, Task[R]], dict[K, R]]
```

### Comparing `taskproc-0.11.2/taskproc/types.py` & `taskproc-0.13.0/taskproc/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 from __future__ import annotations
-from typing import NewType, ParamSpec, TypeVar, Callable
+from typing import TypeVar, Callable
+from typing_extensions import Literal, NewType, ParamSpec
 import os
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, Executor
 from pathlib import Path
+import dotenv
 
 
 P = ParamSpec('P')
 R = TypeVar('R', covariant=True)
 T = TypeVar('T')
 Json = NewType('Json', str)
 TaskKey = tuple[str, Json]
 Runner = Callable[[], R]  # Delayed computation
 RunnerFactory = Callable[P, Runner[R]]
 
 
 
+dotenv.load_dotenv()
+
+
 class Context:
-    cache_dir = Path(os.getenv('CP_CACHE_DIR', './.cache'))
-    executor_name = os.getenv('CP_EXECUTOR', 'process')
-    max_workers = int(os.getenv('CP_MAX_WORKERS', -1))
-    detect_source_change = bool(os.getenv('CP_DETECT_SOURCE_CHANGE', 0))
+    cache_dir = Path(os.getenv('TP_CACHE_DIR', './.cache'))
+    executor_name = os.getenv('TP_EXECUTOR', 'process')
+    max_workers = int(os.getenv('TP_MAX_WORKERS', -1))
+    detect_source_change = bool(os.getenv('TP_DETECT_SOURCE_CHANGE', 0))
     num_cpu = os.cpu_count()
 
     @classmethod
-    def get_executor(cls, max_workers: int | None = None) -> Executor:
-        if cls.executor_name == 'process':
+    def get_executor(cls, executor_name: Literal['process', 'thread'] | str | None = None, max_workers: int | None = None) -> Executor:
+        if executor_name is None:
+            executor_name = cls.executor_name
+
+        if executor_name == 'process':
             executor_type = ProcessPoolExecutor
-        elif cls.executor_name == 'thread':
+        elif executor_name == 'thread':
             executor_type = ThreadPoolExecutor
         else:
             raise ValueError('Unrecognized executor name:', cls.executor_name)
-        if max_workers is None:
+
+        if max_workers is None and cls.max_workers > 0:
             max_workers = cls.max_workers
-        if max_workers < 0:
-            assert isinstance(cls.num_cpu, int)
-            assert -cls.num_cpu <= cls.max_workers
-            max_workers = cls.num_cpu + 1 + cls.max_workers
+
         return executor_type(max_workers=max_workers)
```

### Comparing `taskproc-0.11.2/PKG-INFO` & `taskproc-0.13.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 Metadata-Version: 2.1
 Name: taskproc
-Version: 0.11.2
+Version: 0.13.0
 Summary: A lightweight task processing library written in pure Python
 Home-page: https://github.com/koheimiya/taskproc
 License: MIT
 Author: Kohei Miyaguchi
 Author-email: koheimiyaguchi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/koheimiya/taskproc
 Description-Content-Type: text/markdown
 
 # taskproc
 
 A lightweight workflow building/execution/management tool written in pure Python.
 Internally, it depends on `DiskCache`, `cloudpickle` `networkx` and `concurrent.futures`.
-
 #### Features
-* Decomposing long and complex computation into tasks, i.e., smaller units of work.
-* Executing them in a distributed way, supporting multithreading, multiprocessing, local clusters/containers.
-* Creating/discarding caches per task and reusing them whenever possible. 
+* Decomposing long and complex computation into tasks, i.e., smaller units of work with dependencies.
+* Executing them in a distributed way, supporting multithreading/multiprocessing and local container/cluster-based dispatching.
+* Automatically creating/discarding/reusing caches per task. 
 
 #### Nonfeatures
-* Automatic retry
-* External service integration with remote clusters/containers or cloud platforms (GCP, AWS, ...)
 * Periodic scheduling
-* GUI dashboard
+* Automatic retry
+* External service integration (GCP, AWS, ...)
 
 ## Installation
 
 ```
 pip install taskproc
 ```
 
 ## Usage
 
 ### Basic usage
 
 Workflow is a directed acyclic graph (DAG) of tasks, and task is a unit of work represented with a class.
-Here is an example.
+Each task and its upstream dependencies are specified with a class definition:
 ```python
-from taskproc import TaskBase, Req, Requires, Const
+from taskproc import TaskBase, Requires, Const
 
-# Define a task and **its entire upstream workflow** with a class definition.
-# Inheriting `TaskBase` is necesary, as it takes care of all the work storing and reusing the result and tracking the dependencies.
-# `infer_task_type` decorator helps the type checker to infer the types of the task class. (optional)
-@infer_task_type
 class Choose(TaskBase):
     """ Compute the binomial coefficient. """
-    # Inside a task, we first declare the values that must be computed upstream with the descriptor `Req`.
+    # Inside a task, we first declare the values that must be computed in upstream.
     # In this example, `Choose(n, k)` depends on `Choose(n - 1, k - 1)` and `Choose(n - 1, k)`,
     # so it requires two `int` values.
     prev1: Requires[int]
     prev2: Requires[int]
 
-    def build_task(self, n: int, k: int):
-        # The prerequisite tasks and the other instance attributes are prepared here.
+    def __init__(self, n: int, k: int):
+        # The upstream tasks and the other instance attributes are prepared here.
         # It thus recursively defines all the tasks we need to run this task,
         # i.e., the entire upstream workflow.
 
         if 0 < k < n:
             self.prev1 = Choose(n - 1, k - 1)
             self.prev2 = Choose(n - 1, k)
         elif k == 0 or k == n:
@@ -81,21 +76,21 @@
     def run_task(self) -> int:
         # Here we define the main computation of the task,
         # which is delayed until it is necessary.
 
         # The return values of the prerequisite tasks are accessible via the descriptors:
         return self.prev1 + self.prev2
 
-# To run the task as well as upstream workflow, use the `run_graph()` method.
+# To run the task as well as the upstreams, use the `run_graph()` method.
 ans = Choose(6, 3).run_graph()  # `ans` should be 6 Choose 3, which is 20.
 
 # It greedily executes all the necessary tasks as parallel as possible
 # and then spits out the return value of the task on which we call `run_graph()`.
 # The return values of the intermediate tasks are cached at
-# `{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
+# `{$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/results/...`
 # and reused on the fly whenever possible.
 ```
 
 ### Deleting cache
 
 It is possible to selectively discard cache: 
 ```python
@@ -103,92 +98,53 @@
 # selectively discard the cache corresponding to the modification.
 Choose(3, 3).clear_task()
 
 # `ans` is recomputed tracing back to the computation of `Choose(3, 3)`.
 ans = Choose(6, 3).run_graph()
 
 # Delete all the cache associated with `Choose`,
-# equivalent to `rm -r {$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
+# equivalent to `rm -r {$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.Choose`.
 Choose.clear_all_tasks()            
 ```
 
 ### Task IO
 
-The arguments of the `build_task` method can be anything JSON serializable including `Task`s:
+The arguments of the `__init__` method can be anything JSON serializable + `Task`s:
 ```python
 class MyTask(TaskBase):
-    def build_task(self, param1, param2):
+    def __init__(self, param1, param2):
         ...
 
 MyTask(
     param1={
         'upstream_task0': UpstreamTask(),
         'other_params': [1, 2],
         ...
     },
     param2={ ... }
 }).run_graph()
 ```
 
-<!--
-Otherwise they can be passed via `Task` and `Req`:
+List/dict of upstream tasks can be registered with `RequiresList` and `RequiresDict`:
 ```python
-from taskproc import Task
-Dataset = ...  # Some complex data structure
-Model = ...    # Some complex data structure
-
-class LoadDataset(TaskBase):
-    def build_task(self):
-        pass
-
-    def run_task(self) -> Dataset:
-        ...
-
-class TrainModel(TaskBase):
-    dataset: Requires[Datset]
-
-    def build_task(self, dataset_task: Task[Dataset]):
-        self.dataset = dataset_task
-
-    def run_task(self) -> Model:
-        ...
-    
-class ScoreModel(TaskBase):
-    dataset: Requires[Datset]
-    model: Requires[Model]
-
-    def build_task(self, dataset_task: Task[Dataset], model_task: Task[Model]):
-        self.dataset = dataset_task
-        self.model = model_task
-
-    def run_task(self) -> float:
-        ...
-
-
-dataset_task = LoadDataset()
-model_task = TrainModel(dataset)
-score_task = ScoreModel(dataset, model)
-print(score_task.run_graph()
-```
-
-`Req` accepts a list/dict of tasks and automatically unfolds it.
-```python
-from taskproc import RequiresDict
-
+from taskproc import RequiresList, RequiresDict
 
 class SummarizeScores(TaskBase):
-    scores: RequiresDict[str, float] = Req()  # Again, type annotation or assignment may be omitted.
+    score_list: RequiresList[float]
+    score_dict: RequiresDict[str, float]
 
-    def build_task(self, task_dict: dict[str, Task[float]]):
-        self.scores = task_dict
+    def __init__(self, task_dict: dict[str, Task[float]]):
+        self.score_list = [MyScore(i) for i in range(10)]
+        self.score_dict = task_dict
 
     def run_task(self) -> float:
-        return sum(self.scores.values()) / len(self.scores)  # We have access to the dict of the results.
+        # At runtime `self.score_list` and `self.score_dict` are evaluated as
+        # `list[float]` and `dict[str, float]`, respectively.
+        return sum(self.score_dict.values()) / len(self.score_dict)
 ```
--->
 
 The output of the `run_task` method should be serializable with `cloudpickle`,
 which is then compressed with `gzip`.
 The compression level can be changed as follows (defaults to 9).
 ```python
 class NoCompressionTask(TaskBase, compress_level=0):
     ...
@@ -199,42 +155,53 @@
 class MultiOutputTask(TaskBase):
     def run_task(self) -> dict[str, int]:
         return {'foo': 42, ...}
 
 class DownstreamTask(TaskBase):
     dep: Requires[int]
 
-    def build_task(self):
+    def __init__(self):
         self.dep = MultiOutputTask()['foo']
 ```
 
-
-### Job scheduling and prefixes
-To run task on job schedulers, one can add prefix to the call of task.
-```python
-
-class TaskWithJobScheduler(TaskBase, job_prefix=['jbsub', '-interactive', '-tty', '-queue x86_1h', '-cores 16+1', '-mem 64g']):
-    ...
-```
-
 ### Data directories
 
 Use `task.task_directory` to get a fresh path dedicated to each task.
 The directory is automatically created at
-`{$CP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
+`{$TP_CACHE_DIR:-./.cache}/taskproc/{module_name}.{task_name}/data/{task_id}`
 and the contents of the directory are cleared at each task call and persist until the task is cleared.
 ```python
 class TrainModel(TaskBase):
     def run_task(self) -> str:
         ...
         model_path = self.task_directory / 'model.bin'
         model.save(model_path)
         return model_path
 ```
 
+
+### Job scheduling and prefixes
+Tasks can be run with job schedulers using `prefix_command`, which will be inserted just before each task call.
+```python
+
+class TaskWithJobScheduler(TaskBase, prefix_command='jbsub -interactive -tty -queue x86_1h -cores 16+1 -mem 64g'):
+    ...
+```
+
+
+### Interactive tasks
+Interactive task is beneficial for debugging (e.g., with breakpoints) but harmful for parallel computing.
+In `taskproc`, all the tasks are executed detached by default.
+One can make them interactive by explicitly specifying like so:
+```python
+
+class InteractiveTask(TaskBase, interactive=True):
+    ...
+```
+
 ### Execution policy configuration
 
 One can control the task execution with `concurrent.futures.Executor` class:
 ```python
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 class MyTask(TaskBase):
@@ -261,26 +228,39 @@
 
 # Task-level concurrency control
 SomeDownstreamTask().run_graph(rate_limits={TaskUsingGPU.task_name: 1})
 
 ```
 
 ### Commandline tool
-We can use taskproc from commandline like `python -m taskproc.app path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
+We can use taskproc from commandline like `taskproc path/to/taskfile.py`, where `taskfile.py` defines the `Main` task as follows:
 ```python
 # taskfile.py
 
 class Main(TaskBase):
     ...
 ```
 The command runs the `Main()` task and stores the cache right next to `taskfile.py` as `.cache/taskproc/...`.
-Please refer to `python -m taskproc.app --help` for more info.
+Please refer to `taskproc --help` for more info.
+
+
+### Built-in properties
+Here is the list of the built-in properties/methods of `TaskBase`:
 
-### Other useful properties
-* `TaskBase.task_id`: An integer id for each task
-* `TaskBase.task_args`: The argument of the task
-* `TaskBase.task_stdout`: path to the task's stdout
-* `TaskBase.task_stderr`: Path to the task's stderr
+| Name | Owner | Type | Description |
+|--|--|--|--|
+| `task_name`            | class    | property | String id of the task class |
+| `task_id`              | instance | property | Integer id of the task, unique within the same task class  |
+| `task_args`            | instance | property | The arguments of the task in JSON |
+| `task_directory`       | instance | property | Path to the data directory of the task |
+| `task_stdout`          | instance | property | Path to the task's stdout |
+| `task_stderr`          | instance | property | Path to the task's stderr |
+| `run_task`             | instance | method   | Run the task |
+| `run_graph`            | instance | method   | Run the task after necessary upstream tasks and save the results in the cache |
+| `run_graph_with_stats` | instance | method   | `run_graph` with additional statistics |
+| `get_task_result`      | instance | method   | Directly get the result of the task (fails if the cache is missing) |
+| `clear_task`           | instance | method   | Clear the cache of the task instance |
+| `clear_all_tasks`      | class    | method   | Clear the cache of the task class |
 
 ## TODO
 - [ ] Task graph visualizer
```

