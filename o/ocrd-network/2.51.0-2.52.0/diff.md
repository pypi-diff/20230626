# Comparing `tmp/ocrd_network-2.51.0.tar.gz` & `tmp/ocrd_network-2.52.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrd_network-2.51.0.tar", last modified: Wed Jun  7 11:27:39 2023, max compression
+gzip compressed data, was "ocrd_network-2.52.0.tar", last modified: Mon Jun 26 16:19:24 2023, max compression
```

## Comparing `ocrd_network-2.51.0.tar` & `ocrd_network-2.52.0.tar`

### file list

```diff
@@ -1,33 +1,45 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.596478 ocrd_network-2.51.0/
--rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-07 11:27:39.592478 ocrd_network-2.51.0/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)       85 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/README.md
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.580478 ocrd_network-2.51.0/ocrd_network/
--rw-rw-r--   0 kba       (1000) kba       (1000)     1824 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3284 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/database.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    13670 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployer.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3115 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployment_config.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     5209 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/deployment_utils.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.588478 ocrd_network-2.51.0/ocrd_network/models/
--rw-rw-r--   0 kba       (1000) kba       (1000)      368 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2304 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/job.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      293 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/ocrd_tool.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      976 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/models/workspace.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1285 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/param_validators.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    12949 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/processing_server.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    15391 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/processing_worker.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.592478 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/
--rw-rw-r--   0 kba       (1000) kba       (1000)      299 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     9224 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/connector.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     1098 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     3252 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/consumer.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4239 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/ocrd_messages.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     4149 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/publisher.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2300 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/ocrd_network/utils.py
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-07 11:27:39.580478 ocrd_network-2.51.0/ocrd_network.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)      835 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       96 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       13 2023-06-07 11:27:39.000000 ocrd_network-2.51.0/ocrd_network.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2023-06-07 11:27:39.596478 ocrd_network-2.51.0/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      789 2023-04-02 14:17:57.000000 ocrd_network-2.51.0/setup.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.670465 ocrd_network-2.52.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       43 2023-06-26 16:17:21.000000 ocrd_network-2.52.0/MANIFEST.in
+-rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-26 16:19:24.670465 ocrd_network-2.52.0/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)       85 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.666465 ocrd_network-2.52.0/ocrd_network/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1894 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/__init__.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.666465 ocrd_network-2.52.0/ocrd_network/cli/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      306 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/cli/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2627 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/cli/client.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      798 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/cli/processing_server.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1905 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/cli/processing_worker.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1268 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/cli/processor_server.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1547 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/client.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3284 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/database.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    21435 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/deployer.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     5224 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/deployment_utils.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.670465 ocrd_network-2.52.0/ocrd_network/models/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      368 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/models/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2489 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/models/job.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      293 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/models/ocrd_tool.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      976 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/models/workspace.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1279 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/param_validators.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1631 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/process_helpers.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    16313 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/processing_server.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    12975 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/processing_worker.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     7920 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/processor_server.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.670465 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      299 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     9224 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/connector.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1098 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3252 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/consumer.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4239 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/ocrd_messages.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     4149 2023-06-14 10:09:45.000000 ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/publisher.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     5404 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/runtime_data.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3153 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/server_utils.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3693 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/ocrd_network/utils.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-06-26 16:19:24.666465 ocrd_network-2.52.0/ocrd_network.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      413 2023-06-26 16:19:24.000000 ocrd_network-2.52.0/ocrd_network.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1145 2023-06-26 16:19:24.000000 ocrd_network-2.52.0/ocrd_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2023-06-26 16:19:24.000000 ocrd_network-2.52.0/ocrd_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      110 2023-06-26 16:19:24.000000 ocrd_network-2.52.0/ocrd_network.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       13 2023-06-26 16:19:24.000000 ocrd_network-2.52.0/ocrd_network.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       86 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/requirements.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2023-06-26 16:19:24.670465 ocrd_network-2.52.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      817 2023-06-26 12:46:39.000000 ocrd_network-2.52.0/setup.py
```

### Comparing `ocrd_network-2.51.0/ocrd_network/__init__.py` & `ocrd_network-2.52.0/ocrd_network/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # Nothing relevant is under the radar for now.
 
 # 4. The Mets Server discussion/implementation is available here:
 # https://github.com/OCR-D/core/pull/966
 
 # Note: The Mets Server is still not placed on the architecture diagram and probably won't be a part of
 # the network package. The reason, Mets Server is tightly coupled with the `OcrdWorkspace`.
+from .client import Client
 from .processing_server import ProcessingServer
 from .processing_worker import ProcessingWorker
+from .processor_server import ProcessorServer
 from .param_validators import (
     DatabaseParamType,
-    ProcessingServerParamType,
+    ServerAddressParamType,
     QueueServerParamType
 )
```

### Comparing `ocrd_network-2.51.0/ocrd_network/database.py` & `ocrd_network-2.52.0/ocrd_network/database.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/deployer.py` & `ocrd_network-2.52.0/ocrd_network/processing_worker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,304 +1,271 @@
 """
-Abstraction of the deployment functionality for processors.
+Abstraction for the Processing Server unit in this arch:
+https://user-images.githubusercontent.com/7795705/203554094-62ce135a-b367-49ba-9960-ffe1b7d39b2c.jpg
 
-The Processing Server provides the configuration parameters to the Deployer agent.
-The Deployer agent runs the RabbitMQ Server, MongoDB and the Processing Hosts.
-Each Processing Host may have several Processing Workers.
-Each Processing Worker is an instance of an OCR-D processor.
+Calls to native OCR-D processor should happen through
+the Processing Worker wrapper to hide low level details.
+According to the current requirements, each ProcessingWorker
+is a single OCR-D Processor instance.
 """
 
-from __future__ import annotations
-from typing import Dict, Union
-from paramiko import SSHClient
-from re import search as re_search
-from time import sleep
+from datetime import datetime
+import logging
+from os import getpid
+import requests
 
+import pika.spec
+import pika.adapters.blocking_connection
 
 from ocrd_utils import getLogger
-from .deployment_config import *
-from .deployment_utils import (
-    create_docker_client,
-    create_ssh_client,
-    CustomDockerClient,
-    DeployType,
-    HostData,
+
+from .database import (
+    sync_initiate_database,
+    sync_db_get_workspace,
+    sync_db_update_processing_job,
+)
+from .models import StateEnum
+from .process_helpers import invoke_processor
+from .rabbitmq_utils import (
+    OcrdProcessingMessage,
+    OcrdResultMessage,
+    RMQConsumer,
+    RMQPublisher
+)
+from .utils import (
+    calculate_execution_time,
+    tf_disable_interactive_logs,
+    verify_database_uri,
+    verify_and_parse_mq_uri
 )
-from .rabbitmq_utils import RMQPublisher
 
+# TODO: Check this again when the logging is refactored
+tf_disable_interactive_logs()
 
-class Deployer:
-    """Wraps the deployment functionality of the Processing Server
 
-    Deployer is the one acting.
-    :py:attr:`config` is for representation of the config file only.
-    :py:attr:`hosts` is for managing processor information, not for actually processing.
-    """
-
-    def __init__(self, config: ProcessingServerConfig) -> None:
-        """
-        Args:
-            config (:py:class:`ProcessingServerConfig`): parsed configuration of the Processing Server
-        """
+class ProcessingWorker:
+    def __init__(self, rabbitmq_addr, mongodb_addr, processor_name, ocrd_tool: dict, processor_class=None) -> None:
         self.log = getLogger(__name__)
-        self.config = config
-        self.hosts = HostData.from_config(config.hosts)
-        self.mongo_pid = None
-        self.mq_pid = None
-
-    def kill_all(self) -> None:
-        """ kill all started services: workers, database, queue
-
-        The order of killing is important to optimize graceful shutdown in the future. If RabbitMQ
-        server is killed before killing Processing Workers, that may have bad outcome and leave
-        Processing Workers in an unpredictable state
-        """
-        self.kill_hosts()
-        self.kill_mongodb()
-        self.kill_rabbitmq()
-
-    def deploy_hosts(self, rabbitmq_url: str, mongodb_url: str) -> None:
-        for host in self.hosts:
-            self.log.debug(f'Deploying processing workers on host: {host.config.address}')
-
-            if (any(p.deploy_type == DeployType.native for p in host.config.processors)
-                    and not host.ssh_client):
-                host.ssh_client = create_ssh_client(
-                    host.config.address,
-                    host.config.username,
-                    host.config.password,
-                    host.config.keypath
-                )
-            if (any(p.deploy_type == DeployType.docker for p in host.config.processors)
-                    and not host.docker_client):
-                host.docker_client = create_docker_client(
-                    host.config.address,
-                    host.config.username,
-                    host.config.password,
-                    host.config.keypath
-                )
-
-            for processor in host.config.processors:
-                self._deploy_processing_worker(processor, host, rabbitmq_url, mongodb_url)
-
-            if host.ssh_client:
-                host.ssh_client.close()
-            if host.docker_client:
-                host.docker_client.close()
-
-    def _deploy_processing_worker(self, processor: WorkerConfig, host: HostData,
-                                  rabbitmq_url: str, mongodb_url: str) -> None:
-
-        self.log.debug(f"deploy '{processor.deploy_type}' processor: '{processor}' on '{host.config.address}'")
-
-        for _ in range(processor.count):
-            if processor.deploy_type == DeployType.native:
-                assert host.ssh_client  # to satisfy mypy
-                pid = self.start_native_processor(
-                    client=host.ssh_client,
-                    processor_name=processor.name,
-                    queue_url=rabbitmq_url,
-                    database_url=mongodb_url,
-                )
-                host.pids_native.append(pid)
-            else:
-                assert processor.deploy_type == DeployType.docker
-                assert host.docker_client  # to satisfy mypy
-                pid = self.start_docker_processor(
-                    client=host.docker_client,
-                    processor_name=processor.name,
-                    queue_url=rabbitmq_url,
-                    database_url=mongodb_url
-                )
-                host.pids_docker.append(pid)
-            sleep(0.1)
-
-    def deploy_rabbitmq(self, image: str, detach: bool, remove: bool,
-                        ports_mapping: Union[Dict, None] = None) -> str:
-        """Start docker-container with rabbitmq
-
-        This method deploys the RabbitMQ Server. Handling of creation of queues, submitting messages
-        to queues, and receiving messages from queues is part of the RabbitMQ Library which is part
-        of the OCR-D WebAPI implementation.
-        """
-        self.log.debug(f"Trying to deploy '{image}', with modes: "
-                       f"detach='{detach}', remove='{remove}'")
-
-        if not self.config or not self.config.queue.address:
-            raise ValueError('Deploying RabbitMQ has failed - missing configuration.')
-
-        client = create_docker_client(self.config.queue.address, self.config.queue.username,
-                                      self.config.queue.password, self.config.queue.keypath)
-        if not ports_mapping:
-            # 5672, 5671 - used by AMQP 0-9-1 and AMQP 1.0 clients without and with TLS
-            # 15672, 15671: HTTP API clients, management UI and rabbitmq admin, without and with TLS
-            # 25672: used for internode and CLI tools communication and is allocated from
-            # a dynamic range (limited to a single port by default, computed as AMQP port + 20000)
-            ports_mapping = {
-                5672: self.config.queue.port,
-                15672: 15672,
-                25672: 25672
-            }
-        res = client.containers.run(
-            image=image,
-            detach=detach,
-            remove=remove,
-            ports=ports_mapping,
-            # The default credentials to be used by the processing workers
-            environment=[
-                f'RABBITMQ_DEFAULT_USER={self.config.queue.credentials[0]}',
-                f'RABBITMQ_DEFAULT_PASS={self.config.queue.credentials[1]}'
-            ]
+        # TODO: Provide more flexibility for configuring file logging (i.e. via ENV variables)
+        file_handler = logging.FileHandler(f'/tmp/worker_{processor_name}_{getpid()}.log', mode='a')
+        logging_format = '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
+        file_handler.setFormatter(logging.Formatter(logging_format))
+        file_handler.setLevel(logging.DEBUG)
+        self.log.addHandler(file_handler)
+
+        try:
+            verify_database_uri(mongodb_addr)
+            self.log.debug(f'Verified MongoDB URL: {mongodb_addr}')
+            rmq_data = verify_and_parse_mq_uri(rabbitmq_addr)
+            self.rmq_username = rmq_data['username']
+            self.rmq_password = rmq_data['password']
+            self.rmq_host = rmq_data['host']
+            self.rmq_port = rmq_data['port']
+            self.rmq_vhost = rmq_data['vhost']
+            self.log.debug(f'Verified RabbitMQ Credentials: {self.rmq_username}:{self.rmq_password}')
+            self.log.debug(f'Verified RabbitMQ Server URL: {self.rmq_host}:{self.rmq_port}{self.rmq_vhost}')
+        except ValueError as e:
+            raise ValueError(e)
+
+        sync_initiate_database(mongodb_addr)  # Database client
+        self.ocrd_tool = ocrd_tool
+        # The str name of the OCR-D processor instance to be started
+        self.processor_name = processor_name
+        # The processor class to be used to instantiate the processor
+        # Think of this as a func pointer to the constructor of the respective OCR-D processor
+        self.processor_class = processor_class
+        # Gets assigned when `connect_consumer` is called on the worker object
+        # Used to consume OcrdProcessingMessage from the queue with name {processor_name}
+        self.rmq_consumer = None
+        # Gets assigned when the `connect_publisher` is called on the worker object
+        # The publisher is connected when the `result_queue` field of the OcrdProcessingMessage is set for first time
+        # Used to publish OcrdResultMessage type message to the queue with name {processor_name}-result
+        self.rmq_publisher = None
+
+    def connect_consumer(self) -> None:
+        self.log.info(f'Connecting RMQConsumer to RabbitMQ server: '
+                      f'{self.rmq_host}:{self.rmq_port}{self.rmq_vhost}')
+        self.rmq_consumer = RMQConsumer(
+            host=self.rmq_host,
+            port=self.rmq_port,
+            vhost=self.rmq_vhost
+        )
+        self.log.debug(f'RMQConsumer authenticates with username: '
+                       f'{self.rmq_username}, password: {self.rmq_password}')
+        self.rmq_consumer.authenticate_and_connect(
+            username=self.rmq_username,
+            password=self.rmq_password
+        )
+        self.log.info(f'Successfully connected RMQConsumer.')
+
+    def connect_publisher(self, enable_acks: bool = True) -> None:
+        self.log.info(f'Connecting RMQPublisher to RabbitMQ server: '
+                      f'{self.rmq_host}:{self.rmq_port}{self.rmq_vhost}')
+        self.rmq_publisher = RMQPublisher(
+            host=self.rmq_host,
+            port=self.rmq_port,
+            vhost=self.rmq_vhost
         )
-        assert res and res.id, \
-            f'Failed to start RabbitMQ docker container on host: {self.config.mongo.address}'
-        self.mq_pid = res.id
-        client.close()
-
-        # Build the RabbitMQ Server URL to return
-        rmq_host = self.config.queue.address
-        # note, integer validation is already performed
-        rmq_port = int(self.config.queue.port)
-        # the default virtual host since no field is
-        # provided in the processing server config.yml
-        rmq_vhost = '/'
-
-        self.wait_for_rabbitmq_availability(rmq_host, rmq_port, rmq_vhost,
-                                            self.config.queue.credentials[0],
-                                            self.config.queue.credentials[1])
-
-        rabbitmq_hostinfo = f'{rmq_host}:{rmq_port}{rmq_vhost}'
-        self.log.info(f'The RabbitMQ server was deployed on host: {rabbitmq_hostinfo}')
-        return rabbitmq_hostinfo
-
-    def wait_for_rabbitmq_availability(self, host: str, port: int, vhost: str, username: str,
-                                       password: str) -> None:
-        max_waiting_steps = 15
-        while max_waiting_steps > 0:
-            try:
-                dummy_publisher = RMQPublisher(host=host, port=port, vhost=vhost)
-                dummy_publisher.authenticate_and_connect(username=username, password=password)
-            except Exception:
-                max_waiting_steps -= 1
-                sleep(2)
-            else:
-                # TODO: Disconnect the dummy_publisher here before returning...
-                return
-        raise RuntimeError('Error waiting for queue startup: timeout exceeded')
-
-    def deploy_mongodb(self, image: str, detach: bool, remove: bool,
-                       ports_mapping: Union[Dict, None] = None) -> str:
-        """ Start mongodb in docker
-        """
-        self.log.debug(f"Trying to deploy '{image}', with modes: "
-                       f"detach='{detach}', remove='{remove}'")
-
-        if not self.config or not self.config.mongo.address:
-            raise ValueError('Deploying MongoDB has failed - missing configuration.')
-
-        client = create_docker_client(self.config.mongo.address, self.config.mongo.username,
-                                      self.config.mongo.password, self.config.mongo.keypath)
-        if not ports_mapping:
-            ports_mapping = {
-                27017: self.config.mongo.port
-            }
-        res = client.containers.run(
-            image=image,
-            detach=detach,
-            remove=remove,
-            ports=ports_mapping
+        self.log.debug(f'RMQPublisher authenticates with username: '
+                       f'{self.rmq_username}, password: {self.rmq_password}')
+        self.rmq_publisher.authenticate_and_connect(
+            username=self.rmq_username,
+            password=self.rmq_password
         )
-        if not res or not res.id:
-            raise RuntimeError('Failed to start MongoDB docker container on host: '
-                               f'{self.config.mongo.address}')
-        self.mongo_pid = res.id
-        client.close()
-
-        mongodb_hostinfo = f'{self.config.mongo.address}:{self.config.mongo.port}'
-        self.log.info(f'The MongoDB was deployed on host: {mongodb_hostinfo}')
-        return mongodb_hostinfo
-
-    def kill_rabbitmq(self) -> None:
-        if not self.mq_pid:
-            self.log.warning('No running RabbitMQ instance found')
-            return
-        client = create_docker_client(self.config.queue.address, self.config.queue.username,
-                                      self.config.queue.password, self.config.queue.keypath)
-        client.containers.get(self.mq_pid).stop()
-        self.mq_pid = None
-        client.close()
-        self.log.info('The RabbitMQ is stopped')
-
-    def kill_mongodb(self) -> None:
-        if not self.mongo_pid:
-            self.log.warning('No running MongoDB instance found')
-            return
-        client = create_docker_client(self.config.mongo.address, self.config.mongo.username,
-                                      self.config.mongo.password, self.config.mongo.keypath)
-        client.containers.get(self.mongo_pid).stop()
-        self.mongo_pid = None
-        client.close()
-        self.log.info('The MongoDB is stopped')
-
-    def kill_hosts(self) -> None:
-        self.log.debug('Starting to kill/stop hosts')
-        # Kill processing hosts
-        for host in self.hosts:
-            self.log.debug(f'Killing/Stopping processing workers on host: {host.config.address}')
-            if host.ssh_client:
-                host.ssh_client = create_ssh_client(host.config.address, host.config.username,
-                                                    host.config.password, host.config.keypath)
-            if host.docker_client:
-                host.docker_client = create_docker_client(host.config.address, host.config.username,
-                                                          host.config.password, host.config.keypath)
-            # Kill deployed OCR-D processor instances on this Processing worker host
-            self.kill_processing_worker(host)
-
-    def kill_processing_worker(self, host: HostData) -> None:
-        for pid in host.pids_native:
-            self.log.debug(f"Trying to kill/stop native processor: with PID: '{pid}'")
-            host.ssh_client.exec_command(f'kill {pid}')
-        host.pids_native = []
-
-        for pid in host.pids_docker:
-            self.log.debug(f"Trying to kill/stop docker container with PID: '{pid}'")
-            host.docker_client.containers.get(pid).stop()
-        host.pids_docker = []
-
-    def start_native_processor(self, client: SSHClient, processor_name: str, queue_url: str,
-                               database_url: str) -> str:
-        """ start a processor natively on a host via ssh
-
-        Args:
-            client:             paramiko SSHClient to execute commands on a host
-            processor_name:     name of processor to run
-            queue_url:          url to rabbitmq
-            database_url:       url to database
-
-        Returns:
-            str: pid of running process
-        """
-        self.log.info(f'Starting native processor: {processor_name}')
-        channel = client.invoke_shell()
-        stdin, stdout = channel.makefile('wb'), channel.makefile('rb')
-        cmd = f'{processor_name} --database {database_url} --queue {queue_url}'
-        # the only way (I could find) to make it work to start a process in the background and
-        # return early is this construction. The pid of the last started background process is
-        # printed with `echo $!` but it is printed inbetween other output. Because of that I added
-        # `xyz` before and after the code to easily be able to filter out the pid via regex when
-        # returning from the function
-        logpath = '/tmp/ocrd-processing-server-startup.log'
-        stdin.write(f"echo starting processor with '{cmd}' >> '{logpath}'\n")
-        stdin.write(f'{cmd} >> {logpath} 2>&1 &\n')
-        stdin.write('echo xyz$!xyz \n exit \n')
-        output = stdout.read().decode('utf-8')
-        stdout.close()
-        stdin.close()
-        return re_search(r'xyz([0-9]+)xyz', output).group(1)  # type: ignore
-
-    def start_docker_processor(self, client: CustomDockerClient, processor_name: str,
-                               queue_url: str, database_url: str) -> str:
-        self.log.info(f'Starting docker container processor: {processor_name}')
-        # TODO: add real command here to start processing server in docker here
-        res = client.containers.run('debian', 'sleep 500s', detach=True, remove=True)
-        assert res and res.id, f'Running processor: {processor_name} in docker-container failed'
-        return res.id
+        if enable_acks:
+            self.rmq_publisher.enable_delivery_confirmations()
+            self.log.info('Delivery confirmations are enabled')
+        self.log.info('Successfully connected RMQPublisher.')
+
+    # Define what happens every time a message is consumed
+    # from the queue with name self.processor_name
+    def on_consumed_message(
+            self,
+            channel: pika.adapters.blocking_connection.BlockingChannel,
+            delivery: pika.spec.Basic.Deliver,
+            properties: pika.spec.BasicProperties,
+            body: bytes) -> None:
+        consumer_tag = delivery.consumer_tag
+        delivery_tag: int = delivery.delivery_tag
+        is_redelivered: bool = delivery.redelivered
+        message_headers: dict = properties.headers
+
+        self.log.debug(f'Consumer tag: {consumer_tag}, '
+                       f'message delivery tag: {delivery_tag}, '
+                       f'redelivered: {is_redelivered}')
+        self.log.debug(f'Message headers: {message_headers}')
+
+        try:
+            self.log.debug(f'Trying to decode processing message with tag: {delivery_tag}')
+            processing_message: OcrdProcessingMessage = OcrdProcessingMessage.decode_yml(body)
+        except Exception as e:
+            self.log.error(f'Failed to decode processing message body: {body}')
+            self.log.error(f'Nacking processing message with tag: {delivery_tag}')
+            channel.basic_nack(delivery_tag=delivery_tag, multiple=False, requeue=False)
+            raise Exception(f'Failed to decode processing message with tag: {delivery_tag}, reason: {e}')
+
+        try:
+            self.log.info(f'Starting to process the received message: {processing_message}')
+            self.process_message(processing_message=processing_message)
+        except Exception as e:
+            self.log.error(f'Failed to process processing message with tag: {delivery_tag}')
+            self.log.error(f'Nacking processing message with tag: {delivery_tag}')
+            channel.basic_nack(delivery_tag=delivery_tag, multiple=False, requeue=False)
+            raise Exception(f'Failed to process processing message with tag: {delivery_tag}, reason: {e}')
+
+        self.log.info(f'Successfully processed RabbitMQ message')
+        self.log.debug(f'Acking message with tag: {delivery_tag}')
+        channel.basic_ack(delivery_tag=delivery_tag, multiple=False)
+
+    def start_consuming(self) -> None:
+        if self.rmq_consumer:
+            self.log.info(f'Configuring consuming from queue: {self.processor_name}')
+            self.rmq_consumer.configure_consuming(
+                queue_name=self.processor_name,
+                callback_method=self.on_consumed_message
+            )
+            self.log.info(f'Starting consuming from queue: {self.processor_name}')
+            # Starting consuming is a blocking action
+            self.rmq_consumer.start_consuming()
+        else:
+            raise Exception('The RMQConsumer is not connected/configured properly')
+
+    # TODO: Better error handling required to catch exceptions
+    def process_message(self, processing_message: OcrdProcessingMessage) -> None:
+        # Verify that the processor name in the processing message
+        # matches the processor name of the current processing worker
+        if self.processor_name != processing_message.processor_name:
+            raise ValueError(f'Processor name is not matching. Expected: {self.processor_name},'
+                             f'Got: {processing_message.processor_name}')
+
+        # All of this is needed because the OcrdProcessingMessage object
+        # may not contain certain keys. Simply passing None in the OcrdProcessingMessage constructor
+        # breaks the message validator schema which expects String, but not None due to the Optional[] wrapper.
+        pm_keys = processing_message.__dict__.keys()
+        job_id = processing_message.job_id
+        input_file_grps = processing_message.input_file_grps
+        output_file_grps = processing_message.output_file_grps if 'output_file_grps' in pm_keys else None
+        path_to_mets = processing_message.path_to_mets if 'path_to_mets' in pm_keys else None
+        workspace_id = processing_message.workspace_id if 'workspace_id' in pm_keys else None
+        page_id = processing_message.page_id if 'page_id' in pm_keys else None
+        result_queue_name = processing_message.result_queue_name if 'result_queue_name' in pm_keys else None
+        callback_url = processing_message.callback_url if 'callback_url' in pm_keys else None
+        parameters = processing_message.parameters if processing_message.parameters else {}
+
+        if not path_to_mets and workspace_id:
+            path_to_mets = sync_db_get_workspace(workspace_id).workspace_mets_path
+
+        execution_failed = False
+        self.log.debug(f'Invoking processor: {self.processor_name}')
+        start_time = datetime.now()
+        sync_db_update_processing_job(
+            job_id=job_id,
+            state=StateEnum.running,
+            path_to_mets=path_to_mets,
+            start_time=start_time
+        )
+        try:
+            invoke_processor(
+                processor_class=self.processor_class,
+                executable=self.processor_name,
+                abs_path_to_mets=path_to_mets,
+                input_file_grps=input_file_grps,
+                output_file_grps=output_file_grps,
+                page_id=page_id,
+                parameters=processing_message.parameters
+            )
+        except Exception as error:
+            self.log.debug(f"processor_name: {self.processor_name}, path_to_mets: {path_to_mets}, "
+                           f"input_grps: {input_file_grps}, output_file_grps: {output_file_grps}, "
+                           f"page_id: {page_id}, parameters: {parameters}")
+            self.log.exception(error)
+            execution_failed = True
+        end_time = datetime.now()
+        exec_duration = calculate_execution_time(start_time, end_time)
+        job_state = StateEnum.success if not execution_failed else StateEnum.failed
+        sync_db_update_processing_job(
+            job_id=job_id,
+            state=job_state,
+            end_time=end_time,
+            exec_time=f'{exec_duration} ms'
+        )
+
+        if result_queue_name or callback_url:
+            result_message = OcrdResultMessage(
+                job_id=job_id,
+                state=job_state.value,
+                path_to_mets=path_to_mets,
+                # May not be always available
+                workspace_id=workspace_id
+            )
+            self.log.info(f'Result message: {result_message}')
+            # If the result_queue field is set, send the result message to a result queue
+            if result_queue_name:
+                self.publish_to_result_queue(result_queue_name, result_message)
+            # If the callback_url field is set, post the result message to a callback url
+            if callback_url:
+                self.post_to_callback_url(callback_url, result_message)
+
+    def publish_to_result_queue(self, result_queue: str, result_message: OcrdResultMessage):
+        if self.rmq_publisher is None:
+            self.connect_publisher()
+        # create_queue method is idempotent - nothing happens if
+        # a queue with the specified name already exists
+        self.rmq_publisher.create_queue(queue_name=result_queue)
+        self.log.info(f'Publishing result message to queue: {result_queue}')
+        encoded_result_message = OcrdResultMessage.encode_yml(result_message)
+        self.rmq_publisher.publish_to_queue(
+            queue_name=result_queue,
+            message=encoded_result_message
+        )
+
+    def post_to_callback_url(self, callback_url: str, result_message: OcrdResultMessage):
+        self.log.info(f'Posting result message to callback_url "{callback_url}"')
+        headers = {"Content-Type": "application/json"}
+        json_data = {
+            "job_id": result_message.job_id,
+            "state": result_message.state,
+            "path_to_mets": result_message.path_to_mets,
+            "workspace_id": result_message.workspace_id
+        }
+        response = requests.post(url=callback_url, headers=headers, json=json_data)
+        self.log.info(f'Response from callback_url "{response}"')
```

### Comparing `ocrd_network-2.51.0/ocrd_network/deployment_utils.py` & `ocrd_network-2.52.0/ocrd_network/deployment_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,40 @@
 from __future__ import annotations
 from enum import Enum
-from typing import Union, List
-from distutils.spawn import find_executable as which
-import re
-
 from docker import APIClient, DockerClient
 from docker.transport import SSHHTTPAdapter
 from paramiko import AutoAddPolicy, SSHClient
+from time import sleep
+import re
 
-from ocrd_utils import getLogger
-from .deployment_config import *
+from .rabbitmq_utils import RMQPublisher
+from pymongo import MongoClient
 
 __all__ = [
     'create_docker_client',
     'create_ssh_client',
-    'CustomDockerClient',
     'DeployType',
-    'HostData',
-    'is_bashlib_processor'
+    'wait_for_rabbitmq_availability'
 ]
 
 
-def create_ssh_client(address: str, username: str, password: Union[str, None],
-                      keypath: Union[str, None]) -> SSHClient:
+def create_ssh_client(address: str, username: str, password: str = "", keypath: str = "") -> SSHClient:
     client = SSHClient()
     client.set_missing_host_key_policy(AutoAddPolicy)
     try:
         client.connect(hostname=address, username=username, password=password, key_filename=keypath)
-    except Exception:
-        getLogger(__name__).error(f"Error creating SSHClient for host: '{address}'")
-        raise
+    except Exception as error:
+        raise Exception(f"Error creating SSHClient of host '{address}', reason:") from error
     return client
 
 
-def create_docker_client(address: str, username: str, password: Union[str, None],
-                         keypath: Union[str, None]) -> CustomDockerClient:
+def create_docker_client(address: str, username: str, password: str = "", keypath: str = "") -> CustomDockerClient:
     return CustomDockerClient(username, address, password=password, keypath=keypath)
 
 
-
-class HostData:
-    """class to store runtime information for a host
-    """
-    def __init__(self, config: HostConfig) -> None:
-        self.config = config
-        self.ssh_client: Union[SSHClient, None] = None
-        self.docker_client: Union[CustomDockerClient, None] = None
-        self.pids_native: List[str] = []
-        self.pids_docker: List[str] = []
-
-    @staticmethod
-    def from_config(config: List[HostConfig]) -> List[HostData]:
-        res = []
-        for host_config in config:
-            res.append(HostData(host_config))
-        return res
-
-
 class CustomDockerClient(DockerClient):
     """Wrapper for docker.DockerClient to use an own SshHttpAdapter.
 
     This makes it possible to use provided password/keyfile for connecting with
     python-docker-sdk, which otherwise only allows to use ~/.ssh/config for
     login
 
@@ -78,29 +52,28 @@
     this workaround can be applied.
     """
 
     def __init__(self, user: str, host: str, **kwargs) -> None:
         # the super-constructor is not called on purpose: it solely instantiates the APIClient. The
         # missing `version` in that call would raise an error. APIClient is provided here as a
         # replacement for what the super-constructor does
-        if not user or not host:
+        if not (user and host):
             raise ValueError('Missing argument: user and host must both be provided')
-        if 'password' not in kwargs and 'keypath' not in kwargs:
+        if ('password' not in kwargs) != ('keypath' not in kwargs):
             raise ValueError('Missing argument: one of password and keyfile is needed')
         self.api = APIClient(f'ssh://{host}', use_ssh_client=True, version='1.41')
         ssh_adapter = self.CustomSshHttpAdapter(f'ssh://{user}@{host}:22', **kwargs)
         self.api.mount('http+docker://ssh', ssh_adapter)
 
     class CustomSshHttpAdapter(SSHHTTPAdapter):
-        def __init__(self, base_url, password: Union[str, None] = None,
-                     keypath: Union[str, None] = None) -> None:
+        def __init__(self, base_url, password: str = "", keypath: str = "") -> None:
             self.password = password
             self.keypath = keypath
-            if not self.password and not self.keypath:
-                raise Exception("either 'password' or 'keypath' must be provided")
+            if bool(self.password) == bool(self.keypath):
+                raise Exception("Either 'password' or 'keypath' must be provided")
             super().__init__(base_url)
 
         def _create_paramiko_client(self, base_url: str) -> None:
             """
             this method is called in the superclass constructor. Overwriting allows to set
             password/keypath for the internal paramiko-client
             """
@@ -108,22 +81,42 @@
             if self.password:
                 self.ssh_params['password'] = self.password
             elif self.keypath:
                 self.ssh_params['key_filename'] = self.keypath
             self.ssh_client.set_missing_host_key_policy(AutoAddPolicy)
 
 
-class DeployType(Enum):
-    """ Deploy-Type of the processing server.
-    """
-    docker = 1
-    native = 2
+def verify_rabbitmq_available(
+        host: str,
+        port: int,
+        vhost: str,
+        username: str,
+        password: str
+) -> None:
+    max_waiting_steps = 15
+    while max_waiting_steps > 0:
+        try:
+            dummy_publisher = RMQPublisher(host=host, port=port, vhost=vhost)
+            dummy_publisher.authenticate_and_connect(username=username, password=password)
+        except Exception:
+            max_waiting_steps -= 1
+            sleep(2)
+        else:
+            # TODO: Disconnect the dummy_publisher here before returning...
+            return
+    raise RuntimeError(f'Cannot connect to RabbitMQ host: {host}, port: {port}, '
+                       f'vhost: {vhost}, username: {username}')
 
-    @staticmethod
-    def from_str(label: str) -> DeployType:
-        return DeployType[label.lower()]
 
-    def is_native(self) -> bool:
-        return self == DeployType.native
+def verify_mongodb_available(mongo_url: str) -> None:
+    try:
+        client = MongoClient(mongo_url, serverSelectionTimeoutMS=1000.0)
+        client.admin.command("ismaster")
+    except Exception:
+        raise RuntimeError(f'Cannot connect to MongoDB: {re.sub(r":[^@]+@", ":****@", mongo_url)}')
 
-    def is_docker(self) -> bool:
-        return self == DeployType.docker
+
+class DeployType(Enum):
+    """ Deploy-Type of the processing worker/processor server.
+    """
+    DOCKER = 1
+    NATIVE = 2
```

### Comparing `ocrd_network-2.51.0/ocrd_network/models/job.py` & `ocrd_network-2.52.0/ocrd_network/models/job.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,19 +21,22 @@
     description: Optional[str] = None
     input_file_grps: List[str]
     output_file_grps: Optional[List[str]]
     page_id: Optional[str] = None
     parameters: dict = {}  # Always set to empty dict when None, otherwise it fails ocr-d-validation
     result_queue_name: Optional[str] = None
     callback_url: Optional[str] = None
+    # Used to toggle between sending requests to 'worker and 'server',
+    # i.e., Processing Worker and Processor Server, respectively
+    agent_type: Optional[str] = 'worker'
 
     class Config:
         schema_extra = {
             'example': {
-                'path': '/path/to/mets.xml',
+                'path_to_mets': '/path/to/mets.xml',
                 'description': 'The description of this execution',
                 'input_file_grps': ['INPUT_FILE_GROUP'],
                 'output_file_grps': ['OUTPUT_FILE_GROUP'],
                 'page_id': 'PAGE_ID',
                 'parameters': {}
             }
         }
```

### Comparing `ocrd_network-2.51.0/ocrd_network/models/workspace.py` & `ocrd_network-2.52.0/ocrd_network/models/workspace.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/param_validators.py` & `ocrd_network-2.52.0/ocrd_network/param_validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from .utils import (
     verify_database_uri,
     verify_and_parse_mq_uri
 )
 
 
-class ProcessingServerParamType(ParamType):
-    name = 'Processing server string format'
+class ServerAddressParamType(ParamType):
+    name = 'Server address string format'
     expected_format = 'host:port'
 
     def convert(self, value, param, ctx):
         try:
             elements = value.split(':')
             if len(elements) != 2:
                 raise ValueError('The processing server address is in wrong format')
```

### Comparing `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/connector.py` & `ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/connector.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/constants.py` & `ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/constants.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/consumer.py` & `ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/consumer.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/ocrd_messages.py` & `ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/ocrd_messages.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network/rabbitmq_utils/publisher.py` & `ocrd_network-2.52.0/ocrd_network/rabbitmq_utils/publisher.py`

 * *Files identical despite different names*

### Comparing `ocrd_network-2.51.0/ocrd_network.egg-info/SOURCES.txt` & `ocrd_network-2.52.0/ocrd_network.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 ocrd_network/__init__.py
+ocrd_network/client.py
 ocrd_network/database.py
 ocrd_network/deployer.py
-ocrd_network/deployment_config.py
 ocrd_network/deployment_utils.py
 ocrd_network/param_validators.py
+ocrd_network/process_helpers.py
 ocrd_network/processing_server.py
 ocrd_network/processing_worker.py
+ocrd_network/processor_server.py
+ocrd_network/runtime_data.py
+ocrd_network/server_utils.py
 ocrd_network/utils.py
 ocrd_network.egg-info/PKG-INFO
 ocrd_network.egg-info/SOURCES.txt
 ocrd_network.egg-info/dependency_links.txt
 ocrd_network.egg-info/requires.txt
 ocrd_network.egg-info/top_level.txt
+ocrd_network/cli/__init__.py
+ocrd_network/cli/client.py
+ocrd_network/cli/processing_server.py
+ocrd_network/cli/processing_worker.py
+ocrd_network/cli/processor_server.py
 ocrd_network/models/__init__.py
 ocrd_network/models/job.py
 ocrd_network/models/ocrd_tool.py
 ocrd_network/models/workspace.py
 ocrd_network/rabbitmq_utils/__init__.py
 ocrd_network/rabbitmq_utils/connector.py
 ocrd_network/rabbitmq_utils/constants.py
```

### Comparing `ocrd_network-2.51.0/setup.py` & `ocrd_network-2.52.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,12 +15,13 @@
     author_email='unixprog@gmail.com',
     url='https://github.com/OCR-D/core',
     license='Apache License 2.0',
     python_requires=">=3.7",
     install_requires=install_requires,
     packages=[
         'ocrd_network',
+        'ocrd_network.cli',
         'ocrd_network.models',
         'ocrd_network.rabbitmq_utils'
     ],
     keywords=['OCR', 'OCR-D']
 )
```

