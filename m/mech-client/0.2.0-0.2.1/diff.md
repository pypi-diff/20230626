# Comparing `tmp/mech_client-0.2.0.tar.gz` & `tmp/mech_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.2.0.tar", max compression
+gzip compressed data, was "mech_client-0.2.1.tar", max compression
```

## Comparing `mech_client-0.2.0.tar` & `mech_client-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11339 2023-06-24 06:13:48.183400 mech_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     4049 2023-06-24 06:13:48.183400 mech_client-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/__init__.py
--rw-r--r--   0        0        0     5090 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/acn.py
--rw-r--r--   0        0        0     3359 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/cli.py
--rw-r--r--   0        0        0     1027 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/helpers/__init__.py
--rw-r--r--   0        0        0     1641 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/README.md
--rw-r--r--   0        0        0     1143 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/__init__.py
--rw-r--r--   0        0        0     1543 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/acn.proto
--rw-r--r--   0        0        0     8325 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/acn_pb2.py
--rw-r--r--   0        0        0     7982 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/custom_types.py
--rw-r--r--   0        0        0     4443 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/dialogues.py
--rw-r--r--   0        0        0    10256 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/message.py
--rw-r--r--   0        0        0     1233 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/protocol.yaml
--rw-r--r--   0        0        0     6405 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/serialization.py
--rw-r--r--   0        0        0      847 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/__init__.py
--rw-r--r--   0        0        0     8965 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn.py
--rw-r--r--   0        0        0     1964 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_dialogues.py
--rw-r--r--   0        0        0     4332 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_messages.py
--rw-r--r--   0        0        0      577 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/README.md
--rw-r--r--   0        0        0     1221 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/__init__.py
--rw-r--r--   0        0        0      271 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/acn_data_share.proto
--rw-r--r--   0        0        0     2349 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
--rw-r--r--   0        0        0     4078 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/dialogues.py
--rw-r--r--   0        0        0     7726 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/message.py
--rw-r--r--   0        0        0     1052 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/protocol.yaml
--rw-r--r--   0        0        0     4450 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/serialization.py
--rw-r--r--   0        0        0     1835 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
--rw-r--r--   0        0        0     2021 2023-06-24 06:14:47.507898 mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
--rw-r--r--   0        0        0      631 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/README.md
--rw-r--r--   0        0        0      879 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/__init__.py
--rw-r--r--   0        0        0    27786 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.py
--rw-r--r--   0        0        0     1763 2023-06-24 06:14:47.503898 mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.yaml
--rw-r--r--   0        0        0     9124 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/interact.py
--rw-r--r--   0        0        0     1779 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     1659 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0     1604 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/subgraph.py
--rw-r--r--   0        0        0     1993 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/to_png.py
--rw-r--r--   0        0        0     4901 2023-06-24 06:13:48.183400 mech_client-0.2.0/mech_client/wss.py
--rw-r--r--   0        0        0     1424 2023-06-24 06:13:48.183400 mech_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 mech_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-06-26 13:03:03.797666 mech_client-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4049 2023-06-26 13:03:03.797666 mech_client-0.2.1/README.md
+-rw-r--r--   0        0        0       42 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/__init__.py
+-rw-r--r--   0        0        0     5790 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/acn.py
+-rw-r--r--   0        0        0     3359 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/cli.py
+-rw-r--r--   0        0        0     1028 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/helpers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/README.md
+-rw-r--r--   0        0        0     1143 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/__init__.py
+-rw-r--r--   0        0        0     1543 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/acn.proto
+-rw-r--r--   0        0        0     8325 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/acn_pb2.py
+-rw-r--r--   0        0        0     7982 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/custom_types.py
+-rw-r--r--   0        0        0     4443 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/dialogues.py
+-rw-r--r--   0        0        0    10256 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/message.py
+-rw-r--r--   0        0        0     1233 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/protocol.yaml
+-rw-r--r--   0        0        0     6405 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/serialization.py
+-rw-r--r--   0        0        0      847 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/tests/__init__.py
+-rw-r--r--   0        0        0     8965 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn.py
+-rw-r--r--   0        0        0     1964 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_dialogues.py
+-rw-r--r--   0        0        0     4332 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_messages.py
+-rw-r--r--   0        0        0      577 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/README.md
+-rw-r--r--   0        0        0     1221 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share.proto
+-rw-r--r--   0        0        0     2349 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
+-rw-r--r--   0        0        0     4078 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/dialogues.py
+-rw-r--r--   0        0        0     7726 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/message.py
+-rw-r--r--   0        0        0     1052 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/protocol.yaml
+-rw-r--r--   0        0        0     4450 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/serialization.py
+-rw-r--r--   0        0        0     1835 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
+-rw-r--r--   0        0        0     2021 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
+-rw-r--r--   0        0        0      631 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/README.md
+-rw-r--r--   0        0        0      879 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/__init__.py
+-rw-r--r--   0        0        0    27786 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.py
+-rw-r--r--   0        0        0     1763 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.yaml
+-rw-r--r--   0        0        0    11471 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/interact.py
+-rw-r--r--   0        0        0     2250 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     2059 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1807 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/subgraph.py
+-rw-r--r--   0        0        0     2581 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/to_png.py
+-rw-r--r--   0        0        0     6824 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/wss.py
+-rw-r--r--   0        0        0     1469 2023-06-26 13:03:03.801666 mech_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.1/PKG-INFO
```

### Comparing `mech_client-0.2.0/LICENSE` & `mech_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/README.md` & `mech_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/acn.py` & `mech_client-0.2.1/mech_client/acn.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 # ------------------------------------------------------------------------------
 
 """ACN helpers."""
 
 import asyncio
 from pathlib import Path
-from typing import Type, cast
+from typing import Optional, Type, cast
 
 from aea.components.base import load_aea_package
 from aea.configurations.base import ConnectionConfig
 from aea.configurations.constants import DEFAULT_CONNECTION_CONFIG_FILE
 from aea.configurations.data_types import ComponentType
 from aea.configurations.loader import load_component_configuration
 from aea.connections.base import Connection
@@ -38,14 +38,15 @@
 
 from mech_client.helpers import (
     ACN_DATA_SHARE_PROTOCOL_PACKAGE,
     ACN_PROTOCOL_PACKAGE,
     P2P_CLIENT_PACKAGE,
 )
 
+
 CONNECTION_CONFIG = {
     "connect_retries": 3,
     "ledger_id": "cosmos",
     "nodes": [
         {
             "uri": "acn.staging.autonolas.tech:9005",
             "public_key": "02d3a830c9d6ea1ae91936951430dee11f4662f33118b02190693be835359a9d77",
@@ -62,35 +63,49 @@
         "not_after": "2024-01-01",
         "not_before": "2023-01-01",
         "public_key": "02d3a830c9d6ea1ae91936951430dee11f4662f33118b02190693be835359a9d77",
         "save_path": "acn_cert.txt",
     }
 ]
 
-IPFS_REQUEST_URL = "https://gateway.autonolas.tech/ipfs/{hash_str}/{request_id}"
-
 
 def issue_certificate(cert_request: CertRequest, crypto: Crypto) -> None:
-    """Issue ACN certificate."""
+    """
+    Issue ACN certificate.
+
+    :param cert_request: certificate request object
+    :type cert_request: CertRequest
+    :param crypto: instance of Crypto
+    :type crypto: Crypto
+    :raises: None
+    """
     public_key = cast(str, cert_request.public_key)
     message = cert_request.get_message(public_key)
     signature = crypto.sign_message(message).encode("ascii").hex()
     Path(cert_request.save_path).write_bytes(signature.encode("ascii"))
 
 
-def load_protocol(address: str) -> Type[Message]:
-    """Load message class."""
+def load_protocol() -> Type[Message]:
+    """
+    Load message class.
+
+    :return: message class
+    :rtype: Type[Message]
+    :raises: None
+    """
     configuration = load_component_configuration(
         component_type=ComponentType.PROTOCOL,
         directory=ACN_DATA_SHARE_PROTOCOL_PACKAGE,
     )
     configuration.directory = ACN_DATA_SHARE_PROTOCOL_PACKAGE
     load_aea_package(configuration=configuration)
 
-    from packages.valory.protocols.acn_data_share.message import AcnDataShareMessage
+    from packages.valory.protocols.acn_data_share.message import (  # pylint: disable=import-outside-toplevel,import-error,no-name-in-module
+        AcnDataShareMessage,
+    )
 
     return AcnDataShareMessage
 
 
 def load_acn_protocol() -> None:
     """Load ACN protocol."""
     configuration = load_component_configuration(
@@ -99,15 +114,23 @@
     configuration.directory = ACN_PROTOCOL_PACKAGE
     load_aea_package(configuration=configuration)
 
 
 def load_libp2p_client(
     crypto: Crypto,
 ) -> Connection:
-    """Load `p2p_libp2p_client` connection"""
+    """
+    Load `p2p_libp2p_client` connection.
+
+    :param crypto: instance of Crypto
+    :type crypto: Crypto
+    :return: instance of libp2p2 client connection
+    :rtype: Connection
+    :raises: None
+    """
     config_data = yaml_load(
         (P2P_CLIENT_PACKAGE / DEFAULT_CONNECTION_CONFIG_FILE).open(
             "r", encoding="utf-8"
         )
     )
     config_data["config"] = CONNECTION_CONFIG
     config_data["cert_requests"] = CERT_REQUESTS
@@ -123,28 +146,44 @@
             name="mech_client", address=crypto.address, public_key=crypto.public_key
         ),
         crypto_store=CryptoStore(),
         data_dir=".",
     )
 
 
-async def watch_for_data_url_from_mech(crypto: Crypto) -> str:
-    """Wait for data from mech."""
-    AcnDataShareMessage = load_protocol(address=crypto.address)
+async def watch_for_data_url_from_mech(crypto: Crypto) -> Optional[str]:
+    """
+    Wait for data from mech
+
+    :param crypto: instance of Crypto
+    :type crypto: Crypto
+    :return: Data URL
+    :rtype: str
+    :raises: None
+    """
+    AcnDataShareMessage = load_protocol()
     connection = load_libp2p_client(crypto=crypto)
     try:
         await connection.connect()
         response = await connection.receive()
         response_message = AcnDataShareMessage.decode(response.message)
         return f"https://gateway.autonolas.tech/ipfs/{response_message.content}"
     except AttributeError:
-        pass
+        return None
     finally:
         await connection.disconnect()
 
 
-def watch_for_data_url_from_mech_sync(crypto: Crypto) -> str:
-    """Request and wait for data from agent."""
+def watch_for_data_url_from_mech_sync(crypto: Crypto) -> Optional[str]:
+    """
+    Request and wait for data from agent
+
+    :param crypto: instance of Crypto
+    :type crypto: Crypto
+    :return: Data URL
+    :rtype: str
+    :raises: None
+    """
     loop = asyncio.new_event_loop()
     task = loop.create_task(watch_for_data_url_from_mech(crypto=crypto))
     loop.run_until_complete(task)
     return task.result()
```

### Comparing `mech_client-0.2.0/mech_client/cli.py` & `mech_client-0.2.1/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/__init__.py` & `mech_client-0.2.1/mech_client/helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 #
 # ------------------------------------------------------------------------------
 
 """Helper packages."""
 
 from pathlib import Path
 
+
 ACN_PROTOCOL_PACKAGE = Path(__file__).parent / "acn"
 P2P_CLIENT_PACKAGE = Path(__file__).parent / "p2p_libp2p_client"
 ACN_DATA_SHARE_PROTOCOL_PACKAGE = Path(__file__).parent / "acn_data_share"
```

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/README.md` & `mech_client-0.2.1/mech_client/helpers/acn/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/__init__.py` & `mech_client-0.2.1/mech_client/helpers/acn/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/acn.proto` & `mech_client-0.2.1/mech_client/helpers/acn/acn.proto`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/acn_pb2.py` & `mech_client-0.2.1/mech_client/helpers/acn/acn_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/custom_types.py` & `mech_client-0.2.1/mech_client/helpers/acn/custom_types.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/dialogues.py` & `mech_client-0.2.1/mech_client/helpers/acn/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/message.py` & `mech_client-0.2.1/mech_client/helpers/acn/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/protocol.yaml` & `mech_client-0.2.1/mech_client/helpers/acn/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/serialization.py` & `mech_client-0.2.1/mech_client/helpers/acn/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/tests/__init__.py` & `mech_client-0.2.1/mech_client/helpers/acn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn.py` & `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_dialogues.py` & `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn/tests/test_acn_messages.py` & `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/README.md` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/__init__.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/acn_data_share_pb2.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/dialogues.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/message.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/protocol.yaml` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/serialization.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py` & `mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/README.md` & `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/__init__.py` & `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.py` & `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/helpers/p2p_libp2p_client/connection.yaml` & `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.0/mech_client/interact.py` & `mech_client-0.2.1/mech_client/interact.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import asyncio
 import json
 import os
 import warnings
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple
 
 import requests
 import websocket
 from aea.crypto.base import Crypto
 from aea_ledger_ethereum import EthereumApi, EthereumCrypto
 from web3.contract import Contract as Web3Contract
 
@@ -48,14 +48,15 @@
 from mech_client.wss import (
     register_event_handlers,
     watch_for_data_url_from_wss,
     watch_for_data_url_from_wss_sync,
     watch_for_request_id,
 )
 
+
 AGENT_REGISTRY_CONTRACT = "0xE49CB081e8d96920C38aA7AB90cb0294ab4Bc8EA"
 MECHX_CHAIN_RPC = os.environ.get(
     "MECHX_CHAIN_RPC",
     "https://rpc.eu-central-2.gateway.fm/v4/gnosis/non-archival/mainnet",
 )
 LEDGER_CONFIG = {
     "address": MECHX_CHAIN_RPC,
@@ -80,34 +81,50 @@
 
     ON_CHAIN = "on-chain"
     OFF_CHAIN = "off-chain"
     WAIT_FOR_BOTH = "wait-for-both"
 
 
 def get_contract(contract_address: str, ledger_api: EthereumApi) -> Web3Contract:
-    """Returns a contract instance."""
+    """
+    Returns a contract instance.
+
+    :param contract_address: The address of the contract.
+    :type contract_address: str
+    :param ledger_api: The Ethereum API used for interacting with the ledger.
+    :type ledger_api: EthereumApi
+    :return: The contract instance.
+    :rtype: Web3Contract
+    """
     abi_request_url = GNOSISSCAN_API_URL.format(contract_address=contract_address)
     response = requests.get(abi_request_url).json()
     abi = json.loads(response["result"])
     return ledger_api.get_contract_instance(
         {"abi": abi, "bytecode": "0x"}, contract_address
     )
 
 
 def _tool_selector_prompt(available_tools: List[str]) -> str:
-    """Tool selector prompt."""
+    """
+    Tool selector prompt.
+
+    :param available_tools: A list of available tools.
+    :type available_tools: List[str]
+    :return: The selected tool.
+    :rtype: str
+    """
 
     tool_col_len = max(map(len, available_tools))
     id_col_len = max(2, len(str(len(available_tools))))
     table_len = tool_col_len + id_col_len + 5
 
     separator = "|" + "-" * table_len + "|"
     print("Select prompting tool")
 
-    def format_row(row: Tuple[str, str]) -> str:
+    def format_row(row: Tuple[Any, Any]) -> str:
         _row = list(map(str, row))
         row_str = "| "
         row_str += _row[0]
         row_str += " " * (id_col_len - len(_row[0]))
         row_str += " | "
         row_str += _row[1]
         row_str += " " * (tool_col_len - len(_row[1]))
@@ -126,15 +143,26 @@
         except (ValueError, TypeError, IndexError):
             print("\nPlease enter valid tool ID.")
 
 
 def verify_or_retrieve_tool(
     agent_id: int, ledger_api: EthereumApi, tool: Optional[str] = None
 ) -> str:
-    """Checks if the tool is valid and for what agent."""
+    """
+    Checks if the tool is valid and for what agent.
+
+    :param agent_id: The ID of the agent.
+    :type agent_id: int
+    :param ledger_api: The Ethereum API used for interacting with the ledger.
+    :type ledger_api: EthereumApi
+    :param tool: The tool to verify or retrieve (optional).
+    :type tool: Optional[str]
+    :return: The result of the verification or retrieval.
+    :rtype: str
+    """
     available_tools = fetch_tools(agent_id=agent_id, ledger_api=ledger_api)
     if tool is not None and tool not in available_tools:
         raise ValueError(
             f"Provided tool `{tool}` not in the list of available tools; Available tools={available_tools}"
         )
     if tool is not None:
         return tool
@@ -147,26 +175,40 @@
         contract_address=AGENT_REGISTRY_CONTRACT, ledger_api=ledger_api
     )
     token_uri = mech_registry.functions.tokenURI(agent_id).call()
     response = requests.get(token_uri).json()
     return response["tools"]
 
 
-def send_request(
+def send_request(  # pylint: disable=too-many-arguments
     crypto: EthereumCrypto,
     ledger_api: EthereumApi,
     mech_contract: Web3Contract,
     prompt: str,
     tool: str,
     price: int = 10_000_000_000_000_000,
 ) -> None:
-    """Sends a request to the mech."""
+    """
+    Sends a request to the mech.
+
+    :param crypto: The Ethereum crypto object.
+    :type crypto: EthereumCrypto
+    :param ledger_api: The Ethereum API used for interacting with the ledger.
+    :type ledger_api: EthereumApi
+    :param mech_contract: The mech contract instance.
+    :type mech_contract: Web3Contract
+    :param prompt: The request prompt.
+    :type prompt: str
+    :param tool: The requested tool.
+    :type tool: str
+    :param price: The price for the request (default: 10_000_000_000_000_000).
+    :type price: int
+    """
     v1_file_hash_hex_truncated, v1_file_hash_hex = push_metadata_to_ipfs(prompt, tool)
     print(f"Prompt uploaded: https://gateway.autonolas.tech/ipfs/{v1_file_hash_hex}")
-
     method_name = "request"
     methord_args = {"data": v1_file_hash_hex_truncated}
     tx_args = {"sender_address": crypto.address, "value": price}
     raw_transaction = ledger_api.build_transaction(
         contract_instance=mech_contract,
         method_name=method_name,
         method_args=methord_args,
@@ -181,28 +223,43 @@
 def wait_for_data_url(
     request_id: str,
     wss: websocket.WebSocket,
     mech_contract: Web3Contract,
     ledger_api: EthereumApi,
     crypto: Crypto,
 ) -> Any:
-    """Wait for data from on-chain/off-chain"""
+    """
+    Wait for data from on-chain/off-chain.
+
+    :param request_id: The ID of the request.
+    :type request_id: str
+    :param wss: The WebSocket connection object.
+    :type wss: websocket.WebSocket
+    :param mech_contract: The mech contract instance.
+    :type mech_contract: Web3Contract
+    :param ledger_api: The Ethereum API used for interacting with the ledger.
+    :type ledger_api: EthereumApi
+    :param crypto: The cryptographic object.
+    :type crypto: Crypto
+    :return: The data received from on-chain/off-chain.
+    :rtype: Any
+    """
     loop = asyncio.new_event_loop()
     off_chain_task = loop.create_task(watch_for_data_url_from_mech(crypto=crypto))
     on_chain_task = loop.create_task(
         watch_for_data_url_from_wss(
             request_id=request_id,
             wss=wss,
             mech_contract=mech_contract,
             ledger_api=ledger_api,
             loop=loop,
         )
     )
 
-    async def _wait_for_tasks() -> Any:
+    async def _wait_for_tasks() -> Any:  # type: ignore
         """Wait for tasks to finish."""
         (finished, *_), unfinished = await asyncio.wait(
             [off_chain_task, on_chain_task], return_when=asyncio.FIRST_COMPLETED
         )
         for task in unfinished:
             task.cancel()
         await asyncio.wait(unfinished)
@@ -214,16 +271,29 @@
 
 def interact(
     prompt: str,
     agent_id: int,
     tool: Optional[str] = None,
     private_key_path: Optional[str] = None,
     confirmation_type: ConfirmationType = ConfirmationType.WAIT_FOR_BOTH,
-) -> Dict[str, Any]:
-    """Interact with agent mech contract."""
+) -> None:
+    """
+    Interact with agent mech contract.
+
+    :param prompt: The interaction prompt.
+    :type prompt: str
+    :param agent_id: The ID of the agent.
+    :type agent_id: int
+    :param tool: The tool to interact with (optional).
+    :type tool: Optional[str]
+    :param private_key_path: The path to the private key file (optional).
+    :type private_key_path: Optional[str]
+    :param confirmation_type: The confirmation type for the interaction (default: ConfirmationType.WAIT_FOR_BOTH).
+    :type confirmation_type: ConfirmationType
+    """
     contract_address = query_agent_address(agent_id=agent_id)
     if contract_address is None:
         raise ValueError(f"Agent with ID {agent_id} does not exist!")
 
     private_key_path = private_key_path or PRIVATE_KEY_FILE_PATH
     if not Path(private_key_path).exists():
         raise FileNotFoundError(
```

### Comparing `mech_client-0.2.0/mech_client/prompt_to_ipfs.py` & `mech_client-0.2.1/mech_client/prompt_to_ipfs.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,21 +31,39 @@
 import uuid
 from typing import Tuple
 
 from mech_client.push_to_ipfs import push_to_ipfs
 
 
 def push_metadata_to_ipfs(prompt: str, tool: str) -> Tuple[str, str]:
+    """
+    Pushes metadata object to IPFS.
+
+    :param prompt: Prompt string.
+    :type prompt: str
+    :param tool: Tool string.
+    :type tool: str
+    :return: Tuple containing the IPFS hash and truncated IPFS hash.
+    :rtype: Tuple[str, str]
+    """
     metadata = {"prompt": prompt, "tool": tool, "nonce": str(uuid.uuid4())}
     dirpath = tempfile.mkdtemp()
     file_name = dirpath + "metadata.json"
-    with open(file_name, "w") as f:
+    with open(file_name, "w", encoding="utf-8") as f:
         json.dump(metadata, f)
     _, v1_file_hash_hex = push_to_ipfs(file_name)
     shutil.rmtree(dirpath)
     return "0x" + v1_file_hash_hex[9:], v1_file_hash_hex
 
 
 def main(prompt: str, tool: str) -> None:
+    """
+    Prints the IPFS hash and truncated IPFS hash for the metadata object.
+
+    :param prompt: Prompt string.
+    :type prompt: str
+    :param tool: Tool string.
+    :type tool: str
+    """
     v1_file_hash_hex_truncated, v1_file_hash_hex = push_metadata_to_ipfs(prompt, tool)
     print("Visit url: https://gateway.autonolas.tech/ipfs/{}".format(v1_file_hash_hex))
     print("Hash for Request method: {}".format(v1_file_hash_hex_truncated))
```

### Comparing `mech_client-0.2.0/mech_client/push_to_ipfs.py` & `mech_client-0.2.1/mech_client/push_to_ipfs.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,21 +30,36 @@
 import multibase
 import multicodec
 from aea.helpers.cid import to_v1
 from aea_cli_ipfs.ipfs_utils import IPFSTool
 
 
 def push_to_ipfs(file_path: str) -> Tuple[str, str]:
+    """
+    Push a file to IPFS.
+
+    :param file_path: Path of the file to be pushed to IPFS.
+    :type file_path: str
+
+    :return: A tuple containing v1_file_hash and v1_file_hash_hex.
+    :rtype: Tuple[str, str]
+    """
     response = IPFSTool().client.add(
         file_path, pin=True, recursive=True, wrap_with_directory=False
     )
     v1_file_hash = to_v1(response["Hash"])
     cid_bytes = multibase.decode(v1_file_hash)
     multihash_bytes = multicodec.remove_prefix(cid_bytes)
     v1_file_hash_hex = "f01" + multihash_bytes.hex()
     return v1_file_hash, v1_file_hash_hex
 
 
 def main(file_path: str) -> None:
+    """
+    Push a file to IPFS and print the v1_file_hash and v1_file_hash_hex.
+
+    :param file_path: Path of the file to be pushed to IPFS.
+    :type file_path: str
+    """
     v1_file_hash, v1_file_hash_hex = push_to_ipfs(file_path)
     print("IPFS file hash v1: {}".format(v1_file_hash))
     print("IPFS file hash v1 hex: {}".format(v1_file_hash_hex))
```

### Comparing `mech_client-0.2.0/mech_client/subgraph.py` & `mech_client-0.2.1/mech_client/subgraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,32 +21,40 @@
 
 from string import Template
 from typing import Optional
 
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 
+
 MECH_SUBGRAPH_URL = "https://api.studio.thegraph.com/query/46780/mech/v0.0.1"
 AGENT_QUERY_TEMPLATE = Template(
     """{
     createMeches(where:{agentId:$agent_id}) {
         mech
     }
 }
 """
 )
 
 
 def query_agent_address(agent_id: int) -> Optional[str]:
-    """Query agent address from subgraph."""
+    """
+    Query agent address from subgraph.
+
+    :param agent_id: The ID of the agent.
+    :type agent_id: int
+    :return: The agent address if found, None otherwise.
+    :rtype: Optional[str]
+    """
     client = Client(transport=AIOHTTPTransport(url=MECH_SUBGRAPH_URL))
     response = client.execute(
         document=gql(
             request_string=AGENT_QUERY_TEMPLATE.substitute({"agent_id": agent_id})
         )
     )
-    mechs = response["createMeches"]
+    mechs = response["createMeches"]  # pylint: disable=unsubscriptable-object
     if len(mechs) == 0:
         return None
 
     (record,) = mechs
     return record["mech"]
```

### Comparing `mech_client-0.2.0/mech_client/to_png.py` & `mech_client-0.2.1/mech_client/to_png.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,42 +20,69 @@
 """
 This script facilitates the conversion of a stability AI API's diffusion model output into a PNG format.
 
 Usage:
 
 python push_to_ipfs.py <ipfs_hash> <path>
 """
+
 import json
 import os.path
 from base64 import b64decode
 from tempfile import gettempdir
 
 from aea_cli_ipfs.ipfs_utils import IPFSTool
 
 
 def to_png(data: dict, path: str) -> None:
-    """Stores a stability AI API's diffusion model output into a PNG formatted file."""
-    for i, image in enumerate(data["artifacts"]):
+    """
+    Stores a stability AI API's diffusion model output into a PNG formatted file.
+
+    :param data: Data to be stored.
+    :type data: dict
+    :param path: Path where the data should be stored.
+    :type path: str
+    """
+    for image in data["artifacts"]:
         with open(path, "wb") as f:
             f.write(b64decode(image["base64"]))
 
     print(f"Successfully created {path}.")
 
 
 def get_from_ipfs(ipfs_hash: str, request_id: str) -> dict:
-    """Get data from IPFS."""
+    """
+    Get data from IPFS.
+
+    :param ipfs_hash: The IPFS hash of the data.
+    :type ipfs_hash: str
+    :param request_id: The request ID.
+    :type request_id: str
+    :return: The data.
+    :rtype: dict
+    """
     temp_dir = gettempdir()
     IPFSTool().client.get(cid=ipfs_hash, target=temp_dir)
     stored_data = os.path.join(temp_dir, ipfs_hash)
 
-    with open(os.path.join(stored_data, request_id)) as f:
+    with open(os.path.join(stored_data, request_id), encoding="utf-8") as f:
         data = json.loads(f.read()).get("result", {})
 
     if not isinstance(data, dict):
         raise ValueError("Data do not have the expected format!")
 
     return data
 
 
 def main(ipfs_hash: str, path: str, request_id: str) -> None:
+    """
+    Main function.
+
+    :param ipfs_hash: The IPFS hash of the data.
+    :type ipfs_hash: str
+    :param path: Path where the data should be stored.
+    :type path: str
+    :param request_id: The request ID.
+    :type request_id: str
+    """
     data_ = get_from_ipfs(ipfs_hash, request_id)
     to_png(data_, path)
```

### Comparing `mech_client-0.2.0/pyproject.toml` & `mech_client-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 license = "Apache-2.0"
 include = [
     "mech_client/helpers/acn/*",
@@ -22,24 +22,25 @@
     "mech_client/helpers/p2p_libp2p_client/*.yaml",
     "mech_client/helpers/p2p_libp2p_client/*.proto",
     "mech_client/helpers/p2p_libp2p_client/tests/*",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-open-aea = {version = "1.34.0", extras = ["cli"]}
-open-aea-ledger-ethereum = "1.34.0"
-open-aea-cli-ipfs = "1.34.0"
+open-aea = {version = "1.35.0", extras = ["cli"]}
+open-aea-ledger-ethereum = "1.35.0"
+open-aea-cli-ipfs = "1.35.0"
 websocket-client = ">=0.32.0,<1"
-gql = "^3.4.1"
+gql = ">=3.4.1"
 asn1crypto = ">=1.4.0,<1.5.0"
-open-aea-ledger-cosmos = "1.34.0"
+open-aea-ledger-cosmos = "1.35.0"
 
 [tool.poetry.scripts]
 mechx = "mech_client.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
-open-autonomy = "^0.10.5.post2"
+open-autonomy = "==0.10.7"
+tomte = {extras = ["tox"], version = "==0.2.12"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mech_client-0.2.0/PKG-INFO` & `mech_client-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic client to interact with a mech
 License: Apache-2.0
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asn1crypto (>=1.4.0,<1.5.0)
-Requires-Dist: gql (>=3.4.1,<4.0.0)
-Requires-Dist: open-aea-cli-ipfs (==1.34.0)
-Requires-Dist: open-aea-ledger-cosmos (==1.34.0)
-Requires-Dist: open-aea-ledger-ethereum (==1.34.0)
-Requires-Dist: open-aea[cli] (==1.34.0)
+Requires-Dist: gql (>=3.4.1)
+Requires-Dist: open-aea-cli-ipfs (==1.35.0)
+Requires-Dist: open-aea-ledger-cosmos (==1.35.0)
+Requires-Dist: open-aea-ledger-ethereum (==1.35.0)
+Requires-Dist: open-aea[cli] (==1.35.0)
 Requires-Dist: websocket-client (>=0.32.0,<1)
 Description-Content-Type: text/markdown
 
 # mech-client
 Basic client to interact with a mech
 
 > **Warning**<br />
```

