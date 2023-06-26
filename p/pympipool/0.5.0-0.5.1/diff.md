# Comparing `tmp/pympipool-0.5.0.tar.gz` & `tmp/pympipool-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.0.tar", last modified: Sun Jun 11 14:13:06 2023, max compression
+gzip compressed data, was "pympipool-0.5.1.tar", last modified: Mon Jun 26 14:19:55 2023, max compression
```

## Comparing `pympipool-0.5.0.tar` & `pympipool-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-11 14:13:03.000000 pympipool-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-11 14:13:03.000000 pympipool-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-11 14:13:06.544708 pympipool-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-11 14:13:03.000000 pympipool-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-11 14:13:06.544708 pympipool-0.5.0/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-11 14:13:03.000000 pympipool-0.5.0/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.540708 pympipool-0.5.0/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 14:13:06.000000 pympipool-0.5.0/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-11 14:13:06.544708 pympipool-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-11 14:13:06.000000 pympipool-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 14:13:06.544708 pympipool-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 14:13:03.000000 pympipool-0.5.0/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-11 14:13:03.000000 pympipool-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 14:19:49.000000 pympipool-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 14:19:49.000000 pympipool-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-26 14:19:55.113378 pympipool-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-26 14:19:49.000000 pympipool-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 14:19:55.113378 pympipool-0.5.1/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-26 14:19:49.000000 pympipool-0.5.1/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.109378 pympipool-0.5.1/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:19:55.000000 pympipool-0.5.1/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 14:19:55.113378 pympipool-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-26 14:19:54.000000 pympipool-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:19:55.113378 pympipool-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 14:19:49.000000 pympipool-0.5.1/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-26 14:19:49.000000 pympipool-0.5.1/versioneer.py
```

### Comparing `pympipool-0.5.0/LICENSE` & `pympipool-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/PKG-INFO` & `pympipool-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.0
+Version: 0.5.1
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.0/README.md` & `pympipool-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/pympipool/executor/mpiexec.py` & `pympipool-0.5.1/pympipool/executor/mpiexec.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         else:
             input_dict = None
         input_dict = MPI.COMM_WORLD.bcast(input_dict, root=0)
 
         # Parse input
         if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
             if mpi_rank_zero:
+                socket.send(cloudpickle.dumps({"result": True}))
                 socket.close()
                 context.term()
             break
         elif (
             "fn" in input_dict.keys()
             and "init" not in input_dict.keys()
             and "args" in input_dict.keys()
```

### Comparing `pympipool-0.5.0/pympipool/executor/mpipool.py` & `pympipool-0.5.1/pympipool/executor/mpipool.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,19 @@
             while True:
                 output = parse_socket_communication(
                     executor=executor,
                     input_dict=cloudpickle.loads(socket.recv()),
                     future_dict=future_dict,
                     cores_per_task=int(argument_dict["cores_per_task"]),
                 )
-                if isinstance(output, str) and output == "exit":
+                if "exit" in output.keys() and output["exit"]:
+                    if "result" in output.keys():
+                        socket.send(cloudpickle.dumps({"result": output["result"]}))
+                    else:
+                        socket.send(cloudpickle.dumps({"result": True}))
                     socket.close()
                     context.term()
                     break
                 elif isinstance(output, dict):
                     socket.send(cloudpickle.dumps(output))
```

### Comparing `pympipool-0.5.0/pympipool/share/communication.py` & `pympipool-0.5.1/pympipool/share/communication.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,24 +34,28 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             stdin=subprocess.PIPE,
             cwd=cwd,
         )
 
     def shutdown(self, wait=True):
+        result = None
         if self._process is not None and self._process.poll() is None:
-            self.send_dict(input_dict={"shutdown": True})
+            result = self.send_and_receive_dict(
+                input_dict={"shutdown": True, "wait": wait}
+            )
             self._process_close(wait=wait)
         if self._socket is not None:
             self._socket.close()
         if self._context is not None:
             self._context.term()
         self._process = None
         self._socket = None
         self._context = None
+        return result
 
     def _process_close(self, wait=True):
         self._process.terminate()
         self._process.stdout.close()
         self._process.stdin.close()
         self._process.stderr.close()
         if wait:
```

### Comparing `pympipool-0.5.0/pympipool/share/executor.py` & `pympipool-0.5.1/pympipool/share/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 executor have been reclaimed.
             cancel_futures: If True then shutdown will cancel all pending
                 futures. Futures that are completed or running will not be
                 cancelled.
         """
         if cancel_futures:
             cancel_items_in_queue(que=self._future_queue)
-        self._future_queue.put({"shutdown": True})
+        self._future_queue.put({"shutdown": True, "wait": wait})
         self._process.join()
 
     def __len__(self):
         return self._future_queue.qsize()
 
 
 class Executor(ExecutorBase):
@@ -112,20 +112,22 @@
 class PoolExecutor(ExecutorBase):
     def __init__(
         self,
         max_workers=1,
         oversubscribe=False,
         enable_flux_backend=False,
         cwd=None,
+        sleep_interval=0.1,
     ):
         super().__init__()
         self._process = Thread(
             target=execute_serial_tasks,
             args=(
                 self._future_queue,
                 max_workers,
                 oversubscribe,
                 enable_flux_backend,
                 cwd,
+                sleep_interval,
             ),
         )
         self._process.start()
```

### Comparing `pympipool-0.5.0/pympipool/share/parallel.py` & `pympipool-0.5.1/pympipool/share/parallel.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,18 +89,23 @@
             )
         )
     return funct(input_dict["fn"], *input_dict["args"], **input_dict["kwargs"])
 
 
 def parse_socket_communication(executor, input_dict, future_dict, cores_per_task=1):
     if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
-        # If close "c" is communicated the process is shutdown.
-        return "exit"
+        executor.shutdown(wait=input_dict["wait"])
+        done_dict = update_futures(future_dict=future_dict)
+        # If close "shutdown" is communicated the process is shutdown.
+        if done_dict is not None and len(done_dict) > 0:
+            return {"exit": True, "result": done_dict}
+        else:
+            return {"exit": True}
     elif "fn" in input_dict.keys() and "iterable" in input_dict.keys():
-        # If a function "f" and a list or arguments "l" are communicated,
+        # If a function "fn" and a list or arguments "iterable" are communicated,
         # pympipool uses the map() function to apply the function on the list.
         try:
             output = map_funct(
                 executor=executor,
                 funct=input_dict["fn"],
                 lst=input_dict["iterable"],
                 cores_per_task=cores_per_task,
@@ -112,37 +117,46 @@
         else:
             return {"result": output}
     elif (
         "fn" in input_dict.keys()
         and "args" in input_dict.keys()
         and "kwargs" in input_dict.keys()
     ):
-        # If a function "f" and either arguments "a" or keyword arguments "k" are
+        # If a function "fn", arguments "args" and keyword arguments "kwargs" are
         # communicated pympipool uses submit() to asynchronously apply the function
         # on the arguments and or keyword arguments.
         future = call_funct(input_dict=input_dict, funct=executor.submit)
         future_hash = hash(future)
         future_dict[future_hash] = future
         return {"result": future_hash}
     elif "update" in input_dict.keys():
-        # If update "u" is communicated pympipool checks for asynchronously submitted
+        # If update "update" is communicated pympipool checks for asynchronously submitted
         # functions which have completed in the meantime and communicates their results.
-        done_dict = {
-            k: f.result()
-            for k, f in {k: future_dict[k] for k in input_dict["update"]}.items()
-            if f.done()
-        }
-        for k in done_dict.keys():
-            del future_dict[k]
+        done_dict = update_futures(
+            future_dict=future_dict, hash_lst=input_dict["update"]
+        )
         return {"result": done_dict}
     elif "cancel" in input_dict.keys():
         for k in input_dict["cancel"]:
             future_dict[k].cancel()
         return {"result": True}
 
 
 def update_dict_delta(dict_input, dict_output, keys_possible_lst):
     return {
         k: v
         for k, v in dict_input.items()
         if k in keys_possible_lst and k not in dict_output.keys()
     }
+
+
+def update_futures(future_dict, hash_lst=None):
+    if hash_lst is None:
+        hash_lst = list(future_dict.keys())
+    done_dict = {
+        k: f.result()
+        for k, f in {k: future_dict[k] for k in hash_lst}.items()
+        if f.done()
+    }
+    for k in done_dict.keys():
+        del future_dict[k]
+    return done_dict
```

### Comparing `pympipool-0.5.0/pympipool/share/pool.py` & `pympipool-0.5.1/pympipool/share/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from concurrent.futures import Future
-
 from pympipool.share.communication import SocketInterface
 from pympipool.share.serial import get_parallel_subprocess_command, cloudpickle_register
 
 
 class PoolBase(object):
     def __init__(self):
         self._future_dict = {}
@@ -13,15 +11,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown(wait=True)
         return False
 
-    def shutdown(self, wait=True, *, cancel_futures=False):
+    def shutdown(self, wait=True):
         self._interface.shutdown(wait=wait)
 
 
 class Pool(PoolBase):
     """
     The pympipool.Pool behaves like the multiprocessing.Pool but it uses mpi4py to distribute tasks. In contrast to the
     mpi4py.futures.MPIPoolExecutor the pympipool.Pool can be executed in a serial python process and does not require
```

### Comparing `pympipool-0.5.0/pympipool/share/serial.py` & `pympipool-0.5.1/pympipool/share/serial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import os
 import socket
+import time
 import queue
 
 import cloudpickle
 
 from pympipool.share.communication import SocketInterface
 
 
@@ -91,26 +92,31 @@
             enable_mpi4py_backend=False,
         ),
         cwd=cwd,
     )
     while True:
         task_dict = future_queue.get()
         if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-            interface.shutdown(wait=True)
+            interface.shutdown(wait=task_dict["wait"])
             break
         elif "fn" in task_dict.keys() and "future" in task_dict.keys():
             f = task_dict.pop("future")
             if f.set_running_or_notify_cancel():
                 f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
         elif "fn" in task_dict.keys() and "init" in task_dict.keys():
             interface.send_dict(input_dict=task_dict)
 
 
 def execute_serial_tasks(
-    future_queue, cores, oversubscribe=False, enable_flux_backend=False, cwd=None
+    future_queue,
+    cores,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    cwd=None,
+    sleep_interval=0.1,
 ):
     future_dict = {}
     interface = SocketInterface()
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
@@ -124,31 +130,43 @@
     while True:
         try:
             task_dict = future_queue.get_nowait()
         except queue.Empty:
             pass
         else:
             if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-                interface.shutdown(wait=True)
+                done_dict = interface.shutdown(wait=task_dict["wait"])
+                if isinstance(done_dict, dict):
+                    for k, v in done_dict.items():
+                        if k in future_dict.keys() and not future_dict[k].cancelled():
+                            future_dict.pop(k).set_result(v)
                 break
             elif "fn" in task_dict.keys() and "future" in task_dict.keys():
                 f = task_dict.pop("future")
                 future_hash = interface.send_and_receive_dict(input_dict=task_dict)
                 future_dict[future_hash] = f
-        hash_to_update = [h for h, f in future_dict.items() if not f.done()]
-        hast_to_cancel = [h for h, f in future_dict.items() if f.cancelled()]
-        if len(hash_to_update) > 0:
-            for k, v in interface.send_and_receive_dict(
-                input_dict={"update": hash_to_update}
-            ).items():
-                future_dict.pop(k).set_result(v)
-        if len(hast_to_cancel) > 0:
-            if interface.send_and_receive_dict(input_dict={"cancel": hast_to_cancel}):
-                for h in hast_to_cancel:
-                    del future_dict[h]
+        update_future_dict(
+            interface=interface, future_dict=future_dict, sleep_interval=sleep_interval
+        )
+
+
+def update_future_dict(interface, future_dict, sleep_interval=0.1):
+    time.sleep(sleep_interval)
+    hash_to_update = [h for h, f in future_dict.items() if not f.done()]
+    hash_to_cancel = [h for h, f in future_dict.items() if f.cancelled()]
+    if len(hash_to_update) > 0:
+        for k, v in interface.send_and_receive_dict(
+            input_dict={"update": hash_to_update}
+        ).items():
+            future_dict.pop(k).set_result(v)
+    if len(hash_to_cancel) > 0 and interface.send_and_receive_dict(
+        input_dict={"cancel": hash_to_cancel}
+    ):
+        for h in hash_to_cancel:
+            del future_dict[h]
 
 
 def cloudpickle_register(ind=2):
     # Cloudpickle can either pickle by value or pickle by reference. The functions which are communicated have to
     # be pickled by value rather than by reference, so the module which calls the map function is pickled by value.
     # https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
     # inspect can help to find the module which is calling pympipool
```

### Comparing `pympipool-0.5.0/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.1/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.0
+Version: 0.5.1
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.0/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.1/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/setup.py` & `pympipool-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_communicator_split.py` & `pympipool-0.5.1/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_executor.py` & `pympipool-0.5.1/tests/test_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
                     map_flag=False
                 )
 
     def test_parse_socket_communication_close(self):
         with ThreadPoolExecutor(max_workers=1) as executor:
             output = parse_socket_communication(
                 executor=executor,
-                input_dict={"shutdown": True},
+                input_dict={"shutdown": True, "wait": True},
                 future_dict={},
                 cores_per_task=1
             )
-        self.assertEqual(output, "exit")
+        self.assertEqual(output, {"exit": True})
 
     def test_parse_socket_communication_execute(self):
         with ThreadPoolExecutor(max_workers=1) as executor:
             output = parse_socket_communication(
                 executor=executor,
                 input_dict={"fn": sum, "iterable": [[1, 1]], "chunksize": 1, "map": True},
                 future_dict={},
```

### Comparing `pympipool-0.5.0/tests/test_future.py` & `pympipool-0.5.1/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_interface.py` & `pympipool-0.5.1/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_multitask.py` & `pympipool-0.5.1/tests/test_multitask.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,26 @@
 
 
 def sleep_one(i):
     sleep(1)
     return i
 
 
+def wait_and_calc(n):
+    sleep(1)
+    return n ** 2
+
+
+def call_back(future):
+    global_lst.append(future.result())
+
+
+global_lst = []
+
+
 class TestFuturePool(unittest.TestCase):
     def test_pool_serial(self):
         with PoolExecutor(max_workers=1) as p:
             output = p.submit(calc, i=2)
             self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
@@ -28,15 +40,15 @@
             self.assertEqual(len(p), 0)
         self.assertEqual(output.result(), np.array(4))
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_serial_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
@@ -59,17 +71,26 @@
         self.assertTrue(fs4.done())
 
     def test_cancel_task(self):
         fs1 = Future()
         fs1.cancel()
         q = Queue()
         q.put({"fn": sleep_one, 'args': (), "kwargs": {"i": 1}, "future": fs1})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_serial_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertTrue(fs1.done())
         self.assertTrue(fs1.cancelled())
+
+    def test_waiting(self):
+        exe = PoolExecutor(max_workers=2)
+        f1 = exe.submit(wait_and_calc, 42)
+        f2 = exe.submit(wait_and_calc, 84)
+        f1.add_done_callback(call_back)
+        f2.add_done_callback(call_back)
+        exe.shutdown(wait=True)
+        self.assertTrue([42**2, 84**2], global_lst)
```

### Comparing `pympipool-0.5.0/tests/test_parse.py` & `pympipool-0.5.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_pool.py` & `pympipool-0.5.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_queue.py` & `pympipool-0.5.1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_task.py` & `pympipool-0.5.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/tests/test_worker.py` & `pympipool-0.5.1/tests/test_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,57 +69,57 @@
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(list(output), [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]])
 
     def test_execute_task_failed_no_argument(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         with self.assertRaises(TypeError):
             execute_parallel_tasks(
                 future_queue=q,
                 cores=1,
                 oversubscribe=False,
                 enable_flux_backend=False
             )
 
     def test_execute_task_failed_wrong_argument(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"j": 4}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         with self.assertRaises(TypeError):
             execute_parallel_tasks(
                 future_queue=q,
                 cores=1,
                 oversubscribe=False,
                 enable_flux_backend=False
             )
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_parallel_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
         self.assertEqual(f.result(), np.array(4))
 
     def test_execute_task_parallel(self):
         f = Future()
         q = Queue()
         q.put({"fn": calc, 'args': (), "kwargs": {"i": 2}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_parallel_tasks(
             future_queue=q,
             cores=2,
             oversubscribe=False,
             enable_flux_backend=False
         )
```

### Comparing `pympipool-0.5.0/tests/test_worker_memory.py` & `pympipool-0.5.1/tests/test_worker_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         ), 4)
 
     def test_execute_task(self):
         f = Future()
         q = Queue()
         q.put({"init": True, "fn": set_global, "args": (), "kwargs": {}})
         q.put({"fn": get_global, 'args': (), "kwargs": {}, "future": f})
-        q.put({"shutdown": True})
+        q.put({"shutdown": True, "wait": True})
         cloudpickle_register(ind=1)
         execute_parallel_tasks(
             future_queue=q,
             cores=1,
             oversubscribe=False,
             enable_flux_backend=False
         )
```

### Comparing `pympipool-0.5.0/tests/test_zmq.py` & `pympipool-0.5.1/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.0/versioneer.py` & `pympipool-0.5.1/versioneer.py`

 * *Files identical despite different names*

