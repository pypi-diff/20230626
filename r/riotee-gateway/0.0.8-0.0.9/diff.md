# Comparing `tmp/riotee_gateway-0.0.8.tar.gz` & `tmp/riotee_gateway-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_gateway-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_gateway-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_gateway-0.0.8.tar` & `riotee_gateway-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1101 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      518 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      573 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/__init__.py
--rw-r--r--   0        0        0     3191 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/cli.py
--rw-r--r--   0        0        0     2926 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/client.py
--rw-r--r--   0        0        0     3774 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/packet_model.py
--rw-r--r--   0        0        0     2547 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/server.py
--rw-r--r--   0        0        0     1858 2023-06-19 17:23:04.486536 riotee_gateway-0.0.8/riotee_gateway/transceiver.py
--rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-19 17:30:18.408679 riotee_gateway-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      518 2023-06-19 17:30:18.408679 riotee_gateway-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-06-19 17:30:18.408679 riotee_gateway-0.0.9/riotee_gateway/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-19 17:30:18.408679 riotee_gateway-0.0.9/riotee_gateway/cli.py
+-rw-r--r--   0        0        0     2926 2023-06-19 17:30:18.412679 riotee_gateway-0.0.9/riotee_gateway/client.py
+-rw-r--r--   0        0        0     3774 2023-06-19 17:30:18.412679 riotee_gateway-0.0.9/riotee_gateway/packet_model.py
+-rw-r--r--   0        0        0     2547 2023-06-19 17:30:18.412679 riotee_gateway-0.0.9/riotee_gateway/server.py
+-rw-r--r--   0        0        0     1858 2023-06-19 17:30:18.412679 riotee_gateway-0.0.9/riotee_gateway/transceiver.py
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 riotee_gateway-0.0.9/PKG-INFO
```

### Comparing `riotee_gateway-0.0.8/LICENSE.txt` & `riotee_gateway-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/pyproject.toml` & `riotee_gateway-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/riotee_gateway/__init__.py` & `riotee_gateway-0.0.9/riotee_gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Riotee Gateway Python package"""
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import base64
 import numpy as np
 
 from riotee_gateway.client import GatewayClient
 from riotee_gateway.packet_model import PacketApiSend
 from riotee_gateway.transceiver import Transceiver
```

### Comparing `riotee_gateway-0.0.8/riotee_gateway/cli.py` & `riotee_gateway-0.0.9/riotee_gateway/cli.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/riotee_gateway/client.py` & `riotee_gateway-0.0.9/riotee_gateway/client.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/riotee_gateway/packet_model.py` & `riotee_gateway-0.0.9/riotee_gateway/packet_model.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/riotee_gateway/server.py` & `riotee_gateway-0.0.9/riotee_gateway/server.py`

 * *Files identical despite different names*

### Comparing `riotee_gateway-0.0.8/riotee_gateway/transceiver.py` & `riotee_gateway-0.0.9/riotee_gateway/transceiver.py`

 * *Files identical despite different names*

