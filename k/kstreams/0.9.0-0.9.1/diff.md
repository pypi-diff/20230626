# Comparing `tmp/kstreams-0.9.0.tar.gz` & `tmp/kstreams-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kstreams-0.9.0.tar", max compression
+gzip compressed data, was "kstreams-0.9.1.tar", max compression
```

## Comparing `kstreams-0.9.0.tar` & `kstreams-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-02-28 09:04:46.677695 kstreams-0.9.0/LICENSE
--rw-r--r--   0        0        0     2637 2023-02-28 09:04:46.677695 kstreams-0.9.0/README.md
--rw-r--r--   0        0        0      745 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/__init__.py
--rw-r--r--   0        0        0       46 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/backends/__init__.py
--rw-r--r--   0        0        0     3986 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/backends/kafka.py
--rw-r--r--   0        0        0      994 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/clients.py
--rw-r--r--   0        0        0      400 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/consts.py
--rw-r--r--   0        0        0      986 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/create.py
--rw-r--r--   0        0        0     8008 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/engine.py
--rw-r--r--   0        0        0      715 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/prometheus/__init__.py
--rw-r--r--   0        0        0     2761 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/prometheus/monitor.py
--rw-r--r--   0        0        0      257 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/prometheus/singleton.py
--rw-r--r--   0        0        0     2140 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/prometheus/tasks.py
--rw-r--r--   0        0        0        0 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/py.typed
--rw-r--r--   0        0        0     4319 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/rebalance_listener.py
--rw-r--r--   0        0        0     2033 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/serializers.py
--rw-r--r--   0        0        0     9611 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/streams.py
--rw-r--r--   0        0        0      122 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/structs.py
--rw-r--r--   0        0        0      136 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/test_utils/__init__.py
--rw-r--r--   0        0        0      135 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/test_utils/structs.py
--rw-r--r--   0        0        0     8156 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/test_utils/test_clients.py
--rw-r--r--   0        0        0     2998 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/test_utils/test_utils.py
--rw-r--r--   0        0        0     4183 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/test_utils/topics.py
--rw-r--r--   0        0        0      112 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/types.py
--rw-r--r--   0        0        0     3180 2023-02-28 09:04:46.681696 kstreams-0.9.0/kstreams/utils.py
--rw-r--r--   0        0        0     2006 2023-02-28 09:04:46.681696 kstreams-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 kstreams-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-28 15:14:19.770873 kstreams-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2637 2023-02-28 15:14:19.770873 kstreams-0.9.1/README.md
+-rw-r--r--   0        0        0      753 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/__init__.py
+-rw-r--r--   0        0        0       46 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/backends/__init__.py
+-rw-r--r--   0        0        0     3986 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/backends/kafka.py
+-rw-r--r--   0        0        0      994 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/clients.py
+-rw-r--r--   0        0        0      400 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/consts.py
+-rw-r--r--   0        0        0      986 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/create.py
+-rw-r--r--   0        0        0     8008 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/engine.py
+-rw-r--r--   0        0        0      715 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/prometheus/__init__.py
+-rw-r--r--   0        0        0     2761 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/prometheus/monitor.py
+-rw-r--r--   0        0        0      257 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/prometheus/singleton.py
+-rw-r--r--   0        0        0     2140 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/prometheus/tasks.py
+-rw-r--r--   0        0        0        0 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/py.typed
+-rw-r--r--   0        0        0     4323 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/rebalance_listener.py
+-rw-r--r--   0        0        0     2033 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/serializers.py
+-rw-r--r--   0        0        0     9433 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/streams.py
+-rw-r--r--   0        0        0      122 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/structs.py
+-rw-r--r--   0        0        0      136 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/test_utils/__init__.py
+-rw-r--r--   0        0        0      135 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/test_utils/structs.py
+-rw-r--r--   0        0        0     8156 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/test_utils/test_clients.py
+-rw-r--r--   0        0        0     2998 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/test_utils/test_utils.py
+-rw-r--r--   0        0        0     4183 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/test_utils/topics.py
+-rw-r--r--   0        0        0      112 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/types.py
+-rw-r--r--   0        0        0     3180 2023-02-28 15:14:19.774873 kstreams-0.9.1/kstreams/utils.py
+-rw-r--r--   0        0        0     2006 2023-02-28 15:14:19.778873 kstreams-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 kstreams-0.9.1/PKG-INFO
```

### Comparing `kstreams-0.9.0/LICENSE` & `kstreams-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/README.md` & `kstreams-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/__init__.py` & `kstreams-0.9.1/kstreams/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from aiokafka.structs import ConsumerRecord, TopicPartition
 
 from .clients import Consumer, ConsumerType, Producer, ProducerType
 from .create import StreamEngine, create_engine
 from .prometheus.monitor import PrometheusMonitor, PrometheusMonitorType
-from .rebalance_listener import KstreamsRebalanceListener, RebalanceListener
+from .rebalance_listener import ManualCommitRebalanceListener, RebalanceListener
 from .streams import Stream, stream
 from .structs import TopicPartitionOffset
 
 __all__ = [
     "Consumer",
     "ConsumerType",
     "Producer",
     "ProducerType",
     "StreamEngine",
     "create_engine",
     "PrometheusMonitor",
     "PrometheusMonitorType",
-    "KstreamsRebalanceListener",
+    "ManualCommitRebalanceListener",
     "RebalanceListener",
     "Stream",
     "stream",
     "ConsumerRecord",
     "TopicPartition",
     "TopicPartitionOffset",
 ]
```

### Comparing `kstreams-0.9.0/kstreams/backends/kafka.py` & `kstreams-0.9.1/kstreams/backends/kafka.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/clients.py` & `kstreams-0.9.1/kstreams/clients.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/create.py` & `kstreams-0.9.1/kstreams/create.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/engine.py` & `kstreams-0.9.1/kstreams/engine.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/exceptions.py` & `kstreams-0.9.1/kstreams/exceptions.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/prometheus/monitor.py` & `kstreams-0.9.1/kstreams/prometheus/monitor.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/prometheus/tasks.py` & `kstreams-0.9.1/kstreams/prometheus/tasks.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/rebalance_listener.py` & `kstreams-0.9.1/kstreams/rebalance_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         !!! note
             The `Stream` is available using `self.stream`
         """
         ...  # pragma: no cover
 
 
-class KstreamsRebalanceListener(RebalanceListener):
+class ManualCommitRebalanceListener(RebalanceListener):
     async def on_partitions_revoked(self, revoked: Set[TopicPartition]) -> None:
         """
         Coroutine to be called *before* a rebalance operation starts and
         *after* the consumer stops fetching data.
 
         If manual commit is enabled, `commit` is called before the consumers
         partitions are revoked to prevent the error `CommitFailedError`
```

### Comparing `kstreams-0.9.0/kstreams/serializers.py` & `kstreams-0.9.1/kstreams/serializers.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/streams.py` & `kstreams-0.9.1/kstreams/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from kstreams import ConsumerRecord, TopicPartition
 from kstreams.exceptions import BackendNotSet
 from kstreams.structs import TopicPartitionOffset
 
 from .backends.kafka import Kafka
 from .clients import Consumer, ConsumerType
-from .rebalance_listener import KstreamsRebalanceListener, RebalanceListener
+from .rebalance_listener import RebalanceListener
 from .serializers import Deserializer
 
 logger = logging.getLogger(__name__)
 
 
 class Stream:
     """
@@ -133,22 +133,18 @@
 
     async def _subscribe(self) -> None:
         # Always create a consumer on stream.start
         self.consumer = self._create_consumer()
         await self.consumer.start()
         self.running = True
 
-        if self.rebalance_listener is None:
-            # creates the default listener to manage the commit and
-            # clean the metrics
-            self.rebalance_listener = KstreamsRebalanceListener()
-
-        # set the stream to the listener to it will be available
-        # when the callbacks are called
-        self.rebalance_listener.stream = self  # type: ignore
+        if self.rebalance_listener is not None:
+            # set the stream to the listener to it will be available
+            # when the callbacks are called
+            self.rebalance_listener.stream = self  # type: ignore
 
         self.consumer.subscribe(topics=self.topics, listener=self.rebalance_listener)
 
     async def commit(self, offsets: Optional[Dict[TopicPartition, int]] = None):
         await self.consumer.commit(offsets=offsets)  # type: ignore
 
     async def start(self) -> Optional[AsyncGenerator]:
```

### Comparing `kstreams-0.9.0/kstreams/test_utils/test_clients.py` & `kstreams-0.9.1/kstreams/test_utils/test_clients.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/test_utils/test_utils.py` & `kstreams-0.9.1/kstreams/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/test_utils/topics.py` & `kstreams-0.9.1/kstreams/test_utils/topics.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/kstreams/utils.py` & `kstreams-0.9.1/kstreams/utils.py`

 * *Files identical despite different names*

### Comparing `kstreams-0.9.0/pyproject.toml` & `kstreams-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kstreams"
-version = "0.9.0"
+version = "0.9.1"
 description = "Build simple kafka streams applications"
 authors = ["Marcos Schroh <marcos.schroh@kpn.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 keywords = ["stream", "processing", "kafka", "event streaming"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
@@ -66,15 +66,15 @@
 '''
 
 [tool.isort]
 profile = "black"
 known_first_party = ["kstreams", "tests", "examples"]
 
 [tool.commitizen]
-version = "0.9.0"
+version = "0.9.1"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
 ]
 update_changelog_on_bump = true
 major_version_zero = true
```

### Comparing `kstreams-0.9.0/PKG-INFO` & `kstreams-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kstreams
-Version: 0.9.0
+Version: 0.9.1
 Summary: Build simple kafka streams applications
 License: Apache-2.0
 Keywords: stream,processing,kafka,event streaming
 Author: Marcos Schroh
 Author-email: marcos.schroh@kpn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: AsyncIO
```

