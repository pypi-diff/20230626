# Comparing `tmp/easynetwork-1.0.0rc3.tar.gz` & `tmp/easynetwork-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun 21 20:56:07 2023, max compression
+gzip compressed data, last modified: Mon Jun 26 09:51:24 2023, max compression
```

## Comparing `easynetwork-1.0.0rc3.tar` & `easynetwork-1.0.0rc4.tar`

### file list

```diff
@@ -1,178 +1,186 @@
--rw-r--r--   0        0        0      847 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/.flake8
--rw-r--r--   0        0        0     1939 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0   123771 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/pdm.lock
--rw-r--r--   0        0        0     3673 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tox.ini
--rw-r--r--   0        0        0     1260 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/.vscode/settings.example.json
--rw-r--r--   0        0        0      637 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/converter.py
--rw-r--r--   0        0        0     2120 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/exceptions.py
--rw-r--r--   0        0        0     5291 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/protocol.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/py.typed
--rw-r--r--   0        0        0      206 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/__init__.py
--rw-r--r--   0        0        0      206 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/__init__.py
--rw-r--r--   0        0        0    11127 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/abc.py
--rw-r--r--   0        0        0     6289 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/factory.py
--rw-r--r--   0        0        0     2808 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/futures.py
--rw-r--r--   0        0        0      708 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/sniffio.py
--rw-r--r--   0        0        0     1918 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/tasks.py
--rw-r--r--   0        0        0      368 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/client/__init__.py
--rw-r--r--   0        0        0     2407 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/client/abc.py
--rw-r--r--   0        0        0    13391 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/client/tcp.py
--rw-r--r--   0        0        0    13006 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/client/udp.py
--rw-r--r--   0        0        0      585 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/__init__.py
--rw-r--r--   0        0        0     1428 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/abc.py
--rw-r--r--   0        0        0     2798 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/handler.py
--rw-r--r--   0        0        0     7931 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/standalone.py
--rw-r--r--   0        0        0    22670 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/tcp.py
--rw-r--r--   0        0        0    18828 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_async/server/udp.py
--rw-r--r--   0        0        0      205 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_sync/__init__.py
--rw-r--r--   0        0        0      335 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/__init__.py
--rw-r--r--   0        0        0     2146 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/abc.py
--rw-r--r--   0        0        0    14942 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/tcp.py
--rw-r--r--   0        0        0    13082 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/udp.py
--rw-r--r--   0        0        0     1164 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/__init__.py
--rw-r--r--   0        0        0     2264 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/abc.py
--rw-r--r--   0        0        0     7602 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/base_stream.py
--rw-r--r--   0        0        0     2897 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/cbor.py
--rw-r--r--   0        0        0     8165 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/json.py
--rw-r--r--   0        0        0     2313 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/line.py
--rw-r--r--   0        0        0     3794 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/msgpack.py
--rw-r--r--   0        0        0     3297 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/pickle.py
--rw-r--r--   0        0        0     5084 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/struct.py
--rw-r--r--   0        0        0      422 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/__init__.py
--rw-r--r--   0        0        0     2881 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/base64.py
--rw-r--r--   0        0        0     6344 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/compressor.py
--rw-r--r--   0        0        0     2246 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/encryptor.py
--rw-r--r--   0        0        0      195 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/tools/__init__.py
--rw-r--r--   0        0        0    10773 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/tools/_utils.py
--rw-r--r--   0        0        0     1196 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/tools/lock.py
--rw-r--r--   0        0        0     7948 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/tools/socket.py
--rw-r--r--   0        0        0     5533 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork/tools/stream.py
--rw-r--r--   0        0        0      288 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/__init__.py
--rw-r--r--   0        0        0     6219 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/_utils.py
--rw-r--r--   0        0        0    17315 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/backend.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/py.typed
--rw-r--r--   0        0        0     5389 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/socket.py
--rw-r--r--   0        0        0     4439 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/tasks.py
--rw-r--r--   0        0        0     4072 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/threads.py
--rw-r--r--   0        0        0      208 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/datagram/__init__.py
--rw-r--r--   0        0        0     8604 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/datagram/endpoint.py
--rw-r--r--   0        0        0     3694 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/datagram/socket.py
--rw-r--r--   0        0        0      208 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/stream/__init__.py
--rw-r--r--   0        0        0     5423 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/stream/listener.py
--rw-r--r--   0        0        0     4113 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/src/easynetwork_asyncio/stream/socket.py
--rw-r--r--   0        0        0      131 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/__init__.py
--rw-r--r--   0        0        0      551 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/conftest.py
--rw-r--r--   0        0        0     1113 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/tools.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/__init__.py
--rw-r--r--   0        0        0      355 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/__init__.py
--rw-r--r--   0        0        0    18706 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_asyncio_backend.py
--rw-r--r--   0        0        0     1288 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_backend_factory.py
--rw-r--r--   0        0        0     3217 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_futures.py
--rw-r--r--   0        0        0     2424 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_tasks.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/__init__.py
--rw-r--r--   0        0        0     4173 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/conftest.py
--rw-r--r--   0        0        0     1781 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/serializer.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/__init__.py
--rw-r--r--   0        0        0      289 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/_utils.py
--rw-r--r--   0        0        0      527 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_client/__init__.py
--rw-r--r--   0        0        0    19354 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_client/test_tcp.py
--rw-r--r--   0        0        0    30272 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/__init__.py
--rw-r--r--   0        0        0     1213 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/base.py
--rw-r--r--   0        0        0     4666 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_standalone.py
--rw-r--r--   0        0        0    31156 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_tcp.py
--rw-r--r--   0        0        0    18224 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/__init__.py
--rw-r--r--   0        0        0     1279 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/test_client/__init__.py
--rw-r--r--   0        0        0    12790 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py
--rw-r--r--   0        0        0    15927 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/test_client/test_udp.py
--rw-r--r--   0        0        0      130 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/__init__.py
--rw-r--r--   0        0        0     9118 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/base.py
--rw-r--r--   0        0        0      424 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/conftest.py
--rw-r--r--   0        0        0     6240 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     2233 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0     4069 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_compressors.py
--rw-r--r--   0        0        0     3572 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0     2639 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     3440 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_line.py
--rw-r--r--   0        0        0     1926 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_msgpack.py
--rw-r--r--   0        0        0     2747 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_namedtuple.py
--rw-r--r--   0        0        0     3609 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/samples/__init__.py
--rw-r--r--   0        0        0    10664 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/samples/json.py
--rw-r--r--   0        0        0     2356 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/functional_test/test_serializers/samples/pickle.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/other_test/__init__.py
--rw-r--r--   0        0        0     4925 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/other_test/test_import.py
--rw-r--r--   0        0        0      578 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/other_test/test_project_metadata.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/pytest_plugins/__init__.py
--rw-r--r--   0        0        0     3866 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/pytest_plugins/asyncio_event_loop.py
--rw-r--r--   0        0        0     1792 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/pytest_plugins/extra_features.py
--rw-r--r--   0        0        0      620 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/pytest_plugins/session_exit_code.py
--rw-r--r--   0        0        0     2671 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/scripts/async_server_test.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/__init__.py
--rw-r--r--   0        0        0     1795 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/_utils.py
--rw-r--r--   0        0        0     1808 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/base.py
--rw-r--r--   0        0        0     5555 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/conftest.py
--rw-r--r--   0        0        0     5098 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_converter.py
--rw-r--r--   0        0        0    15717 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_protocol.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/__init__.py
--rw-r--r--   0        0        0     1114 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/base.py
--rw-r--r--   0        0        0     2340 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/__init__.py
--rw-r--r--   0        0        0      425 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/__init__.py
--rw-r--r--   0        0        0     3083 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py
--rw-r--r--   0        0        0    17863 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/test_backend.py
--rw-r--r--   0        0        0     7956 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/test_futures.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/__init__.py
--rw-r--r--   0        0        0      169 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/base.py
--rw-r--r--   0        0        0     2682 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_abc.py
--rw-r--r--   0        0        0    51599 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_tcp.py
--rw-r--r--   0        0        0    41250 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_server/__init__.py
--rw-r--r--   0        0        0     3945 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_server/test_handler.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/__init__.py
--rw-r--r--   0        0        0     1679 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/conftest.py
--rw-r--r--   0        0        0    45874 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_backend.py
--rw-r--r--   0        0        0    32981 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py
--rw-r--r--   0        0        0    14174 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_socket.py
--rw-r--r--   0        0        0    27018 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_stream.py
--rw-r--r--   0        0        0     9534 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py
--rw-r--r--   0        0        0     4898 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_threads.py
--rw-r--r--   0        0        0    30683 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_utils.py
--rw-r--r--   0        0        0      130 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/__init__.py
--rw-r--r--   0        0        0      612 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/base.py
--rw-r--r--   0        0        0      355 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/conftest.py
--rw-r--r--   0        0        0    30904 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_abc.py
--rw-r--r--   0        0        0     3514 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_base64.py
--rw-r--r--   0        0        0     5880 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_cbor.py
--rw-r--r--   0        0        0    20502 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_compressor.py
--rw-r--r--   0        0        0     4351 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_encryptor.py
--rw-r--r--   0        0        0    15194 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_json.py
--rw-r--r--   0        0        0     7216 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_line.py
--rw-r--r--   0        0        0     7146 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_msgpack.py
--rw-r--r--   0        0        0     9953 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_pickle.py
--rw-r--r--   0        0        0    16647 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_struct.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/__init__.py
--rw-r--r--   0        0        0      456 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/__init__.py
--rw-r--r--   0        0        0      526 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/base.py
--rw-r--r--   0        0        0     1019 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/conftest.py
--rw-r--r--   0        0        0     3294 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_abc.py
--rw-r--r--   0        0        0    67599 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_tcp.py
--rw-r--r--   0        0        0    48434 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_udp.py
--rw-r--r--   0        0        0        0 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_tools/__init__.py
--rw-r--r--   0        0        0     2153 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_lock.py
--rw-r--r--   0        0        0     7763 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_socket.py
--rw-r--r--   0        0        0    14621 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_stream.py
--rw-r--r--   0        0        0    22406 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_utils.py
--rw-r--r--   0        0        0     1915 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/.gitignore
--rw-r--r--   0        0        0     1097 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0       55 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/README.md
--rw-r--r--   0        0        0     5197 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     1424 2023-06-21 20:56:07.000000 easynetwork-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/.flake8
+-rw-r--r--   0        0        0     1939 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   123771 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/pdm.lock
+-rw-r--r--   0        0        0     3673 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tox.ini
+-rw-r--r--   0        0        0     1260 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/.vscode/settings.example.json
+-rw-r--r--   0        0        0      637 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/converter.py
+-rw-r--r--   0        0        0     2120 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/exceptions.py
+-rw-r--r--   0        0        0     5291 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/protocol.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/py.typed
+-rw-r--r--   0        0        0      206 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/__init__.py
+-rw-r--r--   0        0        0    11127 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/abc.py
+-rw-r--r--   0        0        0     6248 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/factory.py
+-rw-r--r--   0        0        0     2808 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/futures.py
+-rw-r--r--   0        0        0      708 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/sniffio.py
+-rw-r--r--   0        0        0     2241 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/tasks.py
+-rw-r--r--   0        0        0      368 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/client/__init__.py
+-rw-r--r--   0        0        0     2407 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/client/abc.py
+-rw-r--r--   0        0        0    13618 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/client/tcp.py
+-rw-r--r--   0        0        0    13006 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/client/udp.py
+-rw-r--r--   0        0        0      585 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/__init__.py
+-rw-r--r--   0        0        0     1428 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/abc.py
+-rw-r--r--   0        0        0     2798 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/handler.py
+-rw-r--r--   0        0        0     9644 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/standalone.py
+-rw-r--r--   0        0        0    22780 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/tcp.py
+-rw-r--r--   0        0        0    18924 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_async/server/udp.py
+-rw-r--r--   0        0        0      205 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_sync/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/abc.py
+-rw-r--r--   0        0        0    16622 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/tcp.py
+-rw-r--r--   0        0        0    14336 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/udp.py
+-rw-r--r--   0        0        0     1164 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/__init__.py
+-rw-r--r--   0        0        0     2271 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/abc.py
+-rw-r--r--   0        0        0     7602 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/base_stream.py
+-rw-r--r--   0        0        0     2897 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/cbor.py
+-rw-r--r--   0        0        0     8234 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/json.py
+-rw-r--r--   0        0        0     2313 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/line.py
+-rw-r--r--   0        0        0     3963 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/msgpack.py
+-rw-r--r--   0        0        0     3608 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/pickle.py
+-rw-r--r--   0        0        0     5171 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/struct.py
+-rw-r--r--   0        0        0      422 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/__init__.py
+-rw-r--r--   0        0        0     3173 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/base64.py
+-rw-r--r--   0        0        0     6901 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/compressor.py
+-rw-r--r--   0        0        0     2295 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/encryptor.py
+-rw-r--r--   0        0        0      195 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/tools/__init__.py
+-rw-r--r--   0        0        0    11750 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/tools/_utils.py
+-rw-r--r--   0        0        0     1196 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/tools/lock.py
+-rw-r--r--   0        0        0     8072 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/tools/socket.py
+-rw-r--r--   0        0        0     5498 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork/tools/stream.py
+-rw-r--r--   0        0        0      288 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/__init__.py
+-rw-r--r--   0        0        0     6219 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/_utils.py
+-rw-r--r--   0        0        0    17160 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/backend.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/py.typed
+-rw-r--r--   0        0        0     5389 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/socket.py
+-rw-r--r--   0        0        0     4439 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/tasks.py
+-rw-r--r--   0        0        0     4066 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/threads.py
+-rw-r--r--   0        0        0      208 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/datagram/__init__.py
+-rw-r--r--   0        0        0     8604 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/datagram/endpoint.py
+-rw-r--r--   0        0        0     3642 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/datagram/socket.py
+-rw-r--r--   0        0        0      208 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/stream/__init__.py
+-rw-r--r--   0        0        0     5235 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/stream/listener.py
+-rw-r--r--   0        0        0     4056 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/src/easynetwork_asyncio/stream/socket.py
+-rw-r--r--   0        0        0      131 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/conftest.py
+-rw-r--r--   0        0        0     1113 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/tools.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/__init__.py
+-rw-r--r--   0        0        0    18706 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_asyncio_backend.py
+-rw-r--r--   0        0        0     1288 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_backend_factory.py
+-rw-r--r--   0        0        0     3217 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_futures.py
+-rw-r--r--   0        0        0     3047 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_tasks.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/conftest.py
+-rw-r--r--   0        0        0     1781 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/serializer.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/_utils.py
+-rw-r--r--   0        0        0      527 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_client/__init__.py
+-rw-r--r--   0        0        0    20164 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_client/test_tcp.py
+-rw-r--r--   0        0        0    30272 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/base.py
+-rw-r--r--   0        0        0     5515 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_standalone.py
+-rw-r--r--   0        0        0    31283 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_tcp.py
+-rw-r--r--   0        0        0    18360 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/__init__.py
+-rw-r--r--   0        0        0     1279 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0    13518 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    15927 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_concurrency/__init__.py
+-rw-r--r--   0        0        0     2688 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_concurrency/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_concurrency/test_sync/__init__.py
+-rw-r--r--   0        0        0     1115 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_concurrency/test_sync/conftest.py
+-rw-r--r--   0        0        0     1286 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_concurrency/test_sync/test_threaded_client.py
+-rw-r--r--   0        0        0      130 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0     8863 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/base.py
+-rw-r--r--   0        0        0      424 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0     6240 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     2233 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0     4069 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_compressors.py
+-rw-r--r--   0        0        0     3572 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0     2639 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     3440 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     1926 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     2747 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_namedtuple.py
+-rw-r--r--   0        0        0     3609 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/samples/__init__.py
+-rw-r--r--   0        0        0    10664 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/samples/json.py
+-rw-r--r--   0        0        0     2356 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/functional_test/test_serializers/samples/pickle.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/other_test/__init__.py
+-rw-r--r--   0        0        0     4925 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/other_test/test_import.py
+-rw-r--r--   0        0        0      578 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/other_test/test_project_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/pytest_plugins/__init__.py
+-rw-r--r--   0        0        0     3866 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/pytest_plugins/asyncio_event_loop.py
+-rw-r--r--   0        0        0     1792 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/pytest_plugins/extra_features.py
+-rw-r--r--   0        0        0      620 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/pytest_plugins/session_exit_code.py
+-rw-r--r--   0        0        0     1015 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/pytest_plugins/ssl_module.py
+-rw-r--r--   0        0        0     2597 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/scripts/async_client_test.py
+-rw-r--r--   0        0        0     2649 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/scripts/async_server_test.py
+-rw-r--r--   0        0        0     2627 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/scripts/threaded_client_test.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/__init__.py
+-rw-r--r--   0        0        0     1795 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/_utils.py
+-rw-r--r--   0        0        0     1808 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/base.py
+-rw-r--r--   0        0        0     5555 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/conftest.py
+-rw-r--r--   0        0        0     5098 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_converter.py
+-rw-r--r--   0        0        0    15717 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_protocol.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/__init__.py
+-rw-r--r--   0        0        0     1114 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/base.py
+-rw-r--r--   0        0        0     2340 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/__init__.py
+-rw-r--r--   0        0        0     3083 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py
+-rw-r--r--   0        0        0    17863 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/test_backend.py
+-rw-r--r--   0        0        0     7956 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/test_futures.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/base.py
+-rw-r--r--   0        0        0     2682 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_abc.py
+-rw-r--r--   0        0        0    51599 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_tcp.py
+-rw-r--r--   0        0        0    41250 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_server/__init__.py
+-rw-r--r--   0        0        0     3945 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_server/test_handler.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/__init__.py
+-rw-r--r--   0        0        0     1679 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/conftest.py
+-rw-r--r--   0        0        0    51170 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_backend.py
+-rw-r--r--   0        0        0    32993 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py
+-rw-r--r--   0        0        0    14174 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_socket.py
+-rw-r--r--   0        0        0    27481 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_stream.py
+-rw-r--r--   0        0        0     9534 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py
+-rw-r--r--   0        0        0     4898 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_threads.py
+-rw-r--r--   0        0        0    30683 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_utils.py
+-rw-r--r--   0        0        0      130 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/__init__.py
+-rw-r--r--   0        0        0      612 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/base.py
+-rw-r--r--   0        0        0      355 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/conftest.py
+-rw-r--r--   0        0        0    30904 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_abc.py
+-rw-r--r--   0        0        0     3542 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_base64.py
+-rw-r--r--   0        0        0     5880 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_cbor.py
+-rw-r--r--   0        0        0    20530 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_compressor.py
+-rw-r--r--   0        0        0     4351 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_encryptor.py
+-rw-r--r--   0        0        0    15194 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_json.py
+-rw-r--r--   0        0        0     7216 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_line.py
+-rw-r--r--   0        0        0     7146 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_msgpack.py
+-rw-r--r--   0        0        0     9967 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_pickle.py
+-rw-r--r--   0        0        0    16647 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_struct.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/__init__.py
+-rw-r--r--   0        0        0      526 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/base.py
+-rw-r--r--   0        0        0     1019 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/conftest.py
+-rw-r--r--   0        0        0     3294 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_abc.py
+-rw-r--r--   0        0        0    70817 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_tcp.py
+-rw-r--r--   0        0        0    52896 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_udp.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_tools/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_lock.py
+-rw-r--r--   0        0        0     8336 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_socket.py
+-rw-r--r--   0        0        0    14621 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_stream.py
+-rw-r--r--   0        0        0    23074 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_utils.py
+-rw-r--r--   0        0        0     1915 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/.gitignore
+-rw-r--r--   0        0        0     1097 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0       55 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/README.md
+-rw-r--r--   0        0        0     5225 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     1457 2023-06-26 09:51:24.000000 easynetwork-1.0.0rc4/PKG-INFO
```

### Comparing `easynetwork-1.0.0rc3/.flake8` & `easynetwork-1.0.0rc4/.flake8`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/.pre-commit-config.yaml` & `easynetwork-1.0.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/pdm.lock` & `easynetwork-1.0.0rc4/pdm.lock`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tox.ini` & `easynetwork-1.0.0rc4/tox.ini`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/.vscode/settings.example.json` & `easynetwork-1.0.0rc4/.vscode/settings.example.json`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/__init__.py` & `easynetwork-1.0.0rc4/src/easynetwork/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 __copyright__ = "Copyright (c) 2021-2023, Francis Clairicia-Rose-Claire-Josephine"
 __credits__ = ["FrankySnow9"]
 __deprecated__ = False
 __email__ = "clairicia.rcj.francis@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "FrankySnow9"
 __status__ = "Development"
-__version__ = "1.0.0rc3"
+__version__ = "1.0.0rc4"
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/converter.py` & `easynetwork-1.0.0rc4/src/easynetwork/converter.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/exceptions.py` & `easynetwork-1.0.0rc4/src/easynetwork/exceptions.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/protocol.py` & `easynetwork-1.0.0rc4/src/easynetwork/protocol.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/abc.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/factory.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["AsyncBackendFactory"]
 
 import functools
+import inspect
+from collections import Counter
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any, Final, Mapping, final
 
 from .abc import AbstractAsyncBackend
 from .sniffio import current_async_library as _sniffio_current_async_library
 
 if TYPE_CHECKING:
@@ -41,16 +43,14 @@
             backend,
             "Running library {name!r} misses the backend implementation",
             extended=True,
         )
 
     @staticmethod
     def set_default_backend(backend: str | type[AbstractAsyncBackend] | None) -> None:
-        import inspect
-
         match backend:
             case type() if not issubclass(backend, AbstractAsyncBackend) or inspect.isabstract(backend):
                 raise TypeError(f"Invalid backend class: {backend!r}")
             case type() | None:
                 pass
             case str():
                 AsyncBackendFactory.__get_backend_cls(backend, extended=False)
@@ -124,31 +124,28 @@
             return AsyncBackendFactory.__load_backend_cls_from_entry_point(name)
         except KeyError:
             raise KeyError(error_msg_format.format(name=name)) from None
 
     @staticmethod
     @functools.cache
     def __load_backend_cls_from_entry_point(name: str) -> type[AbstractAsyncBackend]:
-        import inspect
-
         entry_point: EntryPoint = AsyncBackendFactory.__get_available_backends()[name]
 
         entry_point_cls: Any = entry_point.load()
         if (
             not isinstance(entry_point_cls, type)
             or not issubclass(entry_point_cls, AbstractAsyncBackend)
             or inspect.isabstract(entry_point_cls)
         ):
             raise TypeError(f"Invalid backend entry point (name={name!r}): {entry_point_cls!r}")
         return entry_point_cls
 
     @staticmethod
     @functools.cache
     def __get_available_backends() -> MappingProxyType[str, EntryPoint]:
-        from collections import Counter
         from importlib.metadata import entry_points as get_all_entry_points
 
         entry_points = get_all_entry_points(group=AsyncBackendFactory.GROUP_NAME)
         duplicate_counter: Counter[str] = Counter([ep.name for ep in entry_points])
 
         if duplicates := set(name for name in duplicate_counter if duplicate_counter[name] > 1):
             raise TypeError(f"Conflicting backend name caught: {', '.join(map(repr, sorted(duplicates)))}")
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/futures.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/futures.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/sniffio.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/sniffio.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/backend/tasks.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/backend/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -52,18 +52,24 @@
             return self.__task.cancel()
         return True
 
     async def run(self) -> _T_co:
         if self.__task is not None:
             return await self.__task.join()
 
-        async with self.__backend.create_task_group() as task_group:
-            if self.__coro_func is None:
-                self.__task = task_group.start_soon(self.__backend.sleep_forever)
-                self.__task.cancel()
-            else:
-                coro_func, args, kwargs = self.__coro_func
-                self.__coro_func = None
-                self.__task = task_group.start_soon(coro_func, *args, **kwargs)
-                del coro_func, args, kwargs
+        try:
+            async with self.__backend.create_task_group() as task_group:
+                if self.__coro_func is None:
+                    self.__task = task_group.start_soon(self.__backend.sleep_forever)
+                    self.__task.cancel()
+                else:
+                    coro_func, args, kwargs = self.__coro_func
+                    self.__coro_func = None
+                    self.__task = task_group.start_soon(coro_func, *args, **kwargs)
+                    del coro_func, args, kwargs
+        except BaseExceptionGroup as excgrp:
+            if len(excgrp.exceptions) != 1:  # pragma: no cover  # Hard to test
+                raise
+            # This is most likely the unhandled exception raised by coro_func
+            raise excgrp.exceptions[0] from None
 
         return await self.__task.join()
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/client/abc.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/client/abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/client/tcp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/client/tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,27 @@
     Generic,
     Iterator,
     Literal,
     Mapping,
     NoReturn,
     TypedDict,
     TypeVar,
+    cast,
     final,
     overload,
 )
 
+try:
+    import ssl as _ssl
+except ImportError:  # pragma: no cover
+    _ssl_module = None
+else:
+    _ssl_module = _ssl
+    del _ssl
+
 from ...exceptions import ClientClosedError, StreamProtocolParseError
 from ...protocol import StreamProtocol
 from ...tools._utils import (
     check_real_socket_state as _check_real_socket_state,
     check_socket_family as _check_socket_family,
     check_socket_no_ssl as _check_socket_no_ssl,
     concatenate_chunks as _concatenate_chunks,
@@ -141,18 +150,18 @@
             raise ValueError("'max_recv_size' must be a strictly positive integer")
 
         self.__socket: AbstractAsyncStreamSocketAdapter | None = None
         self.__backend: AbstractAsyncBackend = backend
         self.__info: _ClientInfo | None = None
 
         if ssl:
+            if _ssl_module is None:
+                raise RuntimeError("stdlib ssl module not available")
             if isinstance(ssl, bool):
-                from ssl import create_default_context
-
-                ssl = create_default_context()
+                ssl = cast("_SSLContext", _ssl_module.create_default_context())
                 if server_hostname is not None and not server_hostname:
                     ssl.check_hostname = False
         else:
             if server_hostname is not None:
                 raise ValueError("server_hostname is only meaningful with ssl")
 
             if ssl_handshake_timeout is not None:
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/client/udp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/client/udp.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/__init__.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/__init__.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/abc.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/handler.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/handler.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/standalone.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/standalone.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 """Asynchronous network server module"""
 
 from __future__ import annotations
 
 __all__ = ["AbstractStandaloneNetworkServer", "StandaloneTCPNetworkServer", "StandaloneUDPNetworkServer"]
 
 import contextlib as _contextlib
+import threading as _threading
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, Mapping, Self, Sequence, TypeVar
 
+from ...tools.socket import SocketAddress, SocketProxy
 from .tcp import AsyncTCPNetworkServer
 from .udp import AsyncUDPNetworkServer
 
 if TYPE_CHECKING:
     import logging as _logging
-    import threading as _threading
     from ssl import SSLContext as _SSLContext
     from types import TracebackType
 
     from ...protocol import DatagramProtocol, StreamProtocol
     from ..backend.abc import AbstractAsyncBackend, AbstractThreadsPortal, IEvent
     from .abc import AbstractAsyncNetworkServer
     from .handler import AsyncBaseRequestHandler
@@ -64,20 +65,23 @@
         raise NotImplementedError
 
 
 class _BaseStandaloneNetworkServerImpl(AbstractStandaloneNetworkServer):
     __slots__ = (
         "__server",
         "__threads_portal",
+        "__is_shutdown",
     )
 
     def __init__(self, server: AbstractAsyncNetworkServer) -> None:
         super().__init__()
         self.__server: AbstractAsyncNetworkServer = server
         self.__threads_portal: AbstractThreadsPortal | None = None
+        self.__is_shutdown = _threading.Event()
+        self.__is_shutdown.set()
 
     def is_serving(self) -> bool:
         if (portal := self.__threads_portal) is not None:
             with _contextlib.suppress(RuntimeError):
                 return portal.run_sync(self.__server.is_serving)
         return False
 
@@ -87,16 +91,19 @@
                 portal.run_coroutine(self.__server.server_close)
         else:
             backend = self.__server.get_backend()
             backend.bootstrap(self.__server.server_close)
 
     def shutdown(self) -> None:
         if (portal := self.__threads_portal) is not None:
-            with _contextlib.suppress(RuntimeError):
+            CancelledError = self.__server.get_backend().get_cancelled_exc_class()
+            with _contextlib.suppress(RuntimeError, CancelledError):
+                # If shutdown() have been cancelled, that means the scheduler itself is shutting down, and this is what we want
                 portal.run_coroutine(self.__server.shutdown)
+        self.__is_shutdown.wait()
 
     def serve_forever(self, *, is_up_event: _threading.Event | None = None) -> None:
         async def wait_and_set_event(is_up_event_async: IEvent, is_up_event: _threading.Event) -> None:
             await is_up_event_async.wait()
             is_up_event.set()
 
         async def serve_forever() -> None:
@@ -112,14 +119,17 @@
                         task_group.start_soon(wait_and_set_event, is_up_event_async, is_up_event)
                     await self.__server.serve_forever(is_up_event=is_up_event_async)
             finally:
                 self.__threads_portal = None
 
         backend = self.__server.get_backend()
         with _contextlib.suppress(backend.get_cancelled_exc_class()), _contextlib.ExitStack() as stack:
+            stack.callback(self.__is_shutdown.set)
+            self.__is_shutdown.clear()
+
             if is_up_event is not None:
                 # Force is_up_event to be set, in order not to stuck the waiting thread
                 stack.callback(is_up_event.set)
             backend.bootstrap(serve_forever)
 
     @property
     def _server(self) -> AbstractAsyncNetworkServer:
@@ -135,15 +145,15 @@
 
     def __init__(
         self,
         host: str | None | Sequence[str],
         port: int,
         protocol: StreamProtocol[_ResponseT, _RequestT],
         request_handler: AsyncBaseRequestHandler[_RequestT, _ResponseT],
-        backend: str | AbstractAsyncBackend,
+        backend: str | AbstractAsyncBackend = "asyncio",
         *,
         ssl: _SSLContext | None = None,
         ssl_handshake_timeout: float | None = None,
         ssl_shutdown_timeout: float | None = None,
         backlog: int | None = None,
         reuse_port: bool = False,
         max_recv_size: int | None = None,
@@ -174,14 +184,28 @@
         )
 
     def stop_listening(self) -> None:
         if (portal := self._portal) is not None:
             with _contextlib.suppress(RuntimeError):
                 portal.run_sync(self._server.stop_listening)
 
+    def get_addresses(self) -> Sequence[SocketAddress]:
+        if (portal := self._portal) is not None:
+            with _contextlib.suppress(RuntimeError):
+                return portal.run_sync(self._server.get_addresses)
+        return ()
+
+    @property
+    def sockets(self) -> Sequence[SocketProxy]:
+        if (portal := self._portal) is not None:
+            with _contextlib.suppress(RuntimeError):
+                sockets = portal.run_sync(lambda: self._server.sockets)
+                return tuple(SocketProxy(sock, runner=portal.run_sync) for sock in sockets)
+        return ()
+
     if TYPE_CHECKING:
 
         @property
         def _server(self) -> AsyncTCPNetworkServer[_RequestT, _ResponseT]:
             ...
 
 
@@ -190,15 +214,15 @@
 
     def __init__(
         self,
         host: str | None,
         port: int,
         protocol: DatagramProtocol[_ResponseT, _RequestT],
         request_handler: AsyncBaseRequestHandler[_RequestT, _ResponseT],
-        backend: str | AbstractAsyncBackend,
+        backend: str | AbstractAsyncBackend = "asyncio",
         *,
         reuse_port: bool = False,
         backend_kwargs: Mapping[str, Any] | None = None,
         service_actions_interval: float | None = None,
         logger: _logging.Logger | None = None,
         **kwargs: Any,
     ) -> None:
@@ -214,12 +238,26 @@
                 backend_kwargs=backend_kwargs,
                 service_actions_interval=service_actions_interval,
                 logger=logger,
                 **kwargs,
             )
         )
 
+    def get_address(self) -> SocketAddress | None:
+        if (portal := self._portal) is not None:
+            with _contextlib.suppress(RuntimeError):
+                return portal.run_sync(self._server.get_address)
+        return None
+
+    @property
+    def socket(self) -> SocketProxy | None:
+        if (portal := self._portal) is not None:
+            with _contextlib.suppress(RuntimeError):
+                socket = portal.run_sync(lambda: self._server.socket)
+                return SocketProxy(socket, runner=portal.run_sync) if socket is not None else None
+        return None
+
     if TYPE_CHECKING:
 
         @property
         def _server(self) -> AsyncUDPNetworkServer[_RequestT, _ResponseT]:
             ...
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/tcp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 """Asynchronous network server module"""
 
 from __future__ import annotations
 
 __all__ = ["AsyncTCPNetworkServer"]
 
 import contextlib as _contextlib
+import errno as _errno
 import inspect
 import logging as _logging
+import os
+import weakref
 from collections import deque
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     AsyncIterator,
     Callable,
@@ -237,20 +240,17 @@
             # Setup task group
             server_exit_stack.callback(self.__listener_tasks.clear)
             task_group = await server_exit_stack.enter_async_context(self.__backend.create_task_group())
             server_exit_stack.callback(self.__logger.info, "Server loop break, waiting for remaining tasks...")
             ##################
 
             # Enable listener
-            addresses: list[SocketAddress] = []
             for listener in self.__listeners:
                 self.__listener_tasks.append(task_group.start_soon(self.__listener_task, listener, task_group))
-                addresses.append(new_socket_address(listener.get_local_address(), listener.socket().family))
-            self.__logger.info("Start serving at %s", ", ".join(map(str, addresses)))
-            del addresses
+            self.__logger.info("Start serving at %s", ", ".join(map(str, self.get_addresses())))
             #################
 
             # Server is up
             if is_up_event is not None:
                 is_up_event.set()
             task_group.start_soon(self.__service_actions_task)
             ##############
@@ -261,16 +261,14 @@
                 self.__mainloop_task.cancel()
             try:
                 await self.__mainloop_task.join()
             finally:
                 self.__mainloop_task = None
 
     def __make_stop_listening_callback(self) -> Callable[[], None]:
-        import weakref
-
         selfref = weakref.ref(self)
 
         def stop_listening() -> None:
             self = selfref()
             return self.stop_listening() if self is not None else None
 
         return stop_listening
@@ -291,20 +289,17 @@
         client_task = self.__client_task
         async with listener:
             while True:
                 try:
                     client_socket: AbstractAcceptedSocket = await listener.accept()
                 except OSError as exc:  # pragma: no cover  # Not testable
                     if exc.errno in ACCEPT_CAPACITY_ERRNOS:
-                        import errno
-                        import os
-
                         self.__logger.error(
                             "accept returned %s (%s); retrying in %s seconds",
-                            errno.errorcode[exc.errno],
+                            _errno.errorcode[exc.errno],
                             os.strerror(exc.errno),
                             ACCEPT_CAPACITY_ERROR_SLEEP_TIME,
                             exc_info=True,
                         )
                         await self.__backend.sleep(ACCEPT_CAPACITY_ERROR_SLEEP_TIME)
                     else:
                         raise
@@ -420,14 +415,23 @@
             self.__logger.error("-" * 40)
             if client_address is None:
                 self.__logger.exception("Error in client task")
             else:
                 self.__logger.exception("Exception occurred during processing of request from %s", client_address)
             self.__logger.error("-" * 40)
 
+    def get_addresses(self) -> Sequence[SocketAddress]:
+        if (listeners := self.__listeners) is None:
+            return ()
+        return tuple(
+            new_socket_address(listener.get_local_address(), listener.socket().family)
+            for listener in listeners
+            if not listener.is_closing()
+        )
+
     def get_backend(self) -> AbstractAsyncBackend:
         return self.__backend
 
     def get_protocol(self) -> StreamProtocol[_ResponseT, _RequestT]:
         return self.__protocol
 
     @property
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_async/server/udp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_async/server/udp.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,17 +175,15 @@
 
             # Setup task group
             task_group: AbstractTaskGroup = await server_exit_stack.enter_async_context(self.__backend.create_task_group())
             server_exit_stack.callback(self.__logger.info, "Server loop break, waiting for remaining tasks...")
             ##################
 
             # Enable socket
-            address: SocketAddress = new_socket_address(self.__socket.get_local_address(), self.__socket.socket().family)
-            self.__logger.info("Start serving at %s", address)
-            del address
+            self.__logger.info("Start serving at %s", self.get_address())
             #################
 
             # Server is up
             if is_up_event is not None:
                 is_up_event.set()
             task_group.start_soon(self.__service_actions_task)
             ##############
@@ -319,14 +317,19 @@
         try:
             yield
         except Exception:
             self.__logger.error("-" * 40)
             self.__logger.exception("Exception occurred during processing of request from %s", client_address)
             self.__logger.error("-" * 40)
 
+    def get_address(self) -> SocketAddress | None:
+        if (socket := self.__socket) is None or socket.is_closing():
+            return None
+        return new_socket_address(socket.get_local_address(), socket.socket().family)
+
     def get_backend(self) -> AbstractAsyncBackend:
         return self.__backend
 
     def get_protocol(self) -> DatagramProtocol[_ResponseT, _RequestT]:
         return self.__protocol
 
     @property
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/abc.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 """Network client module"""
 
 from __future__ import annotations
 
 __all__ = ["AbstractNetworkClient"]
 
+import time
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, Iterator, Self, TypeVar
 
 from ...tools.socket import SocketAddress
 
 if TYPE_CHECKING:
     from types import TracebackType
@@ -53,15 +54,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def recv_packet(self, timeout: float | None = ...) -> _ReceivedPacketT:
         raise NotImplementedError
 
     def iter_received_packets(self, timeout: float | None = 0) -> Iterator[_ReceivedPacketT]:
-        from time import monotonic
+        monotonic = time.monotonic
 
         recv_packet = self.recv_packet
         while True:
             try:
                 _start = monotonic()
                 packet = recv_packet(timeout)
                 _end = monotonic()
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/tcp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/tcp.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,58 +7,76 @@
 from __future__ import annotations
 
 __all__ = ["TCPNetworkClient"]
 
 import contextlib as _contextlib
 import errno as _errno
 import socket as _socket
+import threading
 from time import monotonic as _time_monotonic
-from typing import TYPE_CHECKING, Any, Callable, Generic, Iterator, Literal, NoReturn, TypeVar, final, overload
+from typing import TYPE_CHECKING, Any, Callable, Generic, Iterator, Literal, NoReturn, TypeGuard, TypeVar, cast, final, overload
+
+try:
+    import ssl
+except ImportError:  # pragma: no cover
+    _ssl_module = None
+else:
+    _ssl_module = ssl
+    del ssl
 
 from ...exceptions import ClientClosedError, StreamProtocolParseError
 from ...protocol import StreamProtocol
 from ...tools._utils import (
     check_real_socket_state as _check_real_socket_state,
     check_socket_family as _check_socket_family,
     check_socket_no_ssl as _check_socket_no_ssl,
     concatenate_chunks as _concatenate_chunks,
     error_from_errno as _error_from_errno,
     is_ssl_eof_error as _is_ssl_eof_error,
-    is_ssl_socket as _is_ssl_socket,
     replace_kwargs as _replace_kwargs,
     retry_socket_method as _retry_socket_method,
     retry_ssl_socket_method as _retry_ssl_socket_method,
     set_tcp_keepalive as _set_tcp_keepalive,
     set_tcp_nodelay as _set_tcp_nodelay,
 )
 from ...tools.lock import ForkSafeLock
-from ...tools.socket import CLOSED_SOCKET_ERRNOS, MAX_STREAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
+from ...tools.socket import (
+    CLOSED_SOCKET_ERRNOS,
+    MAX_STREAM_BUFSIZE,
+    SSL_HANDSHAKE_TIMEOUT,
+    SSL_SHUTDOWN_TIMEOUT,
+    SocketAddress,
+    SocketProxy,
+    new_socket_address,
+)
 from ...tools.stream import StreamDataConsumer
 from .abc import AbstractNetworkClient
 
 if TYPE_CHECKING:
-    from ssl import SSLContext as _SSLContext
+    from ssl import SSLContext as _SSLContext, SSLSocket as _SSLSocket
 
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 _SentPacketT = TypeVar("_SentPacketT")
 
 
 class TCPNetworkClient(AbstractNetworkClient[_SentPacketT, _ReceivedPacketT], Generic[_SentPacketT, _ReceivedPacketT]):
     __slots__ = (
         "__socket",
+        "__over_ssl",
         "__socket_proxy",
         "__send_lock",
         "__receive_lock",
         "__socket_lock",
         "__producer",
         "__consumer",
         "__addr",
         "__peer",
         "__eof_reached",
         "__max_recv_size",
+        "__retry_interval",
         "__ssl_shutdown_timeout",
     )
 
     @overload
     def __init__(
         self,
         address: tuple[str, int],
@@ -68,14 +86,15 @@
         connect_timeout: float | None = ...,
         local_address: tuple[str, int] | None = ...,
         ssl: _SSLContext | bool | None = ...,
         server_hostname: str | None = ...,
         ssl_handshake_timeout: float | None = ...,
         ssl_shutdown_timeout: float | None = ...,
         max_recv_size: int | None = ...,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         socket: _socket.socket,
@@ -83,38 +102,38 @@
         protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
         *,
         ssl: _SSLContext | bool | None = ...,
         server_hostname: str | None = ...,
         ssl_handshake_timeout: float | None = ...,
         ssl_shutdown_timeout: float | None = ...,
         max_recv_size: int | None = ...,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     def __init__(
         self,
         __arg: _socket.socket | tuple[str, int],
         /,
         protocol: StreamProtocol[_SentPacketT, _ReceivedPacketT],
         *,
         ssl: _SSLContext | bool | None = None,
         server_hostname: str | None = None,
         ssl_handshake_timeout: float | None = None,
         ssl_shutdown_timeout: float | None = None,
         max_recv_size: int | None = None,
+        retry_interval: float = 1.0,
         **kwargs: Any,
     ) -> None:
         self.__socket: _socket.socket | None = None  # If any exception occurs, the client will already be in a closed state
         super().__init__()
 
-        from threading import Lock
-
-        self.__send_lock = ForkSafeLock(Lock)
-        self.__receive_lock = ForkSafeLock(Lock)
-        self.__socket_lock = ForkSafeLock(Lock)
+        self.__send_lock = ForkSafeLock(threading.Lock)
+        self.__receive_lock = ForkSafeLock(threading.Lock)
+        self.__socket_lock = ForkSafeLock(threading.Lock)
 
         if server_hostname is not None and not ssl:
             raise ValueError("server_hostname is only meaningful with ssl")
 
         if ssl_handshake_timeout is not None and not ssl:
             raise ValueError("ssl_handshake_timeout is only meaningful with ssl")
 
@@ -155,58 +174,63 @@
             _check_socket_family(socket.family)
             _check_socket_no_ssl(socket)
 
             if max_recv_size is None:
                 max_recv_size = MAX_STREAM_BUFSIZE
             if not isinstance(max_recv_size, int) or max_recv_size <= 0:
                 raise ValueError("'max_recv_size' must be a strictly positive integer")
+            self.__max_recv_size: int = max_recv_size
+
+            self.__retry_interval = retry_interval = float(retry_interval)
+            if self.__retry_interval <= 0:
+                raise ValueError("retry_interval must be a strictly positive float or None")
 
             # Do not use global default timeout here
             socket.settimeout(0)
 
             self.__addr: SocketAddress = new_socket_address(socket.getsockname(), socket.family)
             self.__peer: SocketAddress = new_socket_address(socket.getpeername(), socket.family)
+            self.__over_ssl: bool = False
+            self.__eof_reached: bool = False
 
             if ssl:
+                if _ssl_module is None:
+                    raise RuntimeError("stdlib ssl module not available")
                 if isinstance(ssl, bool):
-                    import ssl as _ssl_module
-
-                    ssl = _ssl_module.create_default_context()
+                    ssl = cast("_SSLContext", _ssl_module.create_default_context())
                     if not server_hostname:
                         ssl.check_hostname = False
                     if hasattr(_ssl_module, "OP_IGNORE_UNEXPECTED_EOF"):
                         ssl.options &= ~getattr(_ssl_module, "OP_IGNORE_UNEXPECTED_EOF")
                 if not server_hostname:
                     server_hostname = None
                 socket = ssl.wrap_socket(
                     socket,
                     server_side=False,
                     do_handshake_on_connect=False,
                     suppress_ragged_eofs=False,  # Suppressed or not, it will be transformed to a ConnectionAbortedError so...
                     server_hostname=server_hostname,
                 )
-                if ssl_handshake_timeout is None:
-                    from ...tools.socket import SSL_HANDSHAKE_TIMEOUT
 
+                self.__over_ssl = True
+
+                if ssl_handshake_timeout is None:
                     ssl_handshake_timeout = SSL_HANDSHAKE_TIMEOUT
 
-                _retry_ssl_socket_method(socket, ssl_handshake_timeout, socket.do_handshake, block=False)
+                with self.__convert_socket_error():
+                    _retry_ssl_socket_method(socket, ssl_handshake_timeout, retry_interval, socket.do_handshake, block=False)
 
                 if ssl_shutdown_timeout is None:
-                    from ...tools.socket import SSL_SHUTDOWN_TIMEOUT
-
                     ssl_shutdown_timeout = SSL_SHUTDOWN_TIMEOUT
 
             _set_tcp_nodelay(socket)
             _set_tcp_keepalive(socket)
             self.__producer: Callable[[_SentPacketT], Iterator[bytes]] = protocol.generate_chunks
             self.__consumer: StreamDataConsumer[_ReceivedPacketT] = StreamDataConsumer(protocol)
             self.__socket_proxy = SocketProxy(socket, lock=self.__socket_lock.get)
-            self.__eof_reached: bool = False
-            self.__max_recv_size: int = max_recv_size
             self.__ssl_shutdown_timeout: float | None = ssl_shutdown_timeout
         except BaseException:
             socket.close()
             raise
 
         self.__socket = socket  # There was no errors
 
@@ -231,66 +255,78 @@
 
     def close(self) -> None:
         with self.__send_lock.get(), self.__socket_lock.get():
             if (socket := self.__socket) is None:
                 return
             self.__socket = None
             try:
-                if not self.__eof_reached and _is_ssl_socket(socket):
+                if not self.__eof_reached and self.__is_ssl_socket(socket):
                     with self.__convert_ssl_eof_error(), _contextlib.suppress(TimeoutError):
-                        socket = _retry_ssl_socket_method(socket, self.__ssl_shutdown_timeout, socket.unwrap)
+                        retry_interval: float = self.__retry_interval
+                        socket = _retry_ssl_socket_method(socket, self.__ssl_shutdown_timeout, retry_interval, socket.unwrap)
             except ConnectionError:
                 # It is normal if there was connection errors during operations. But do not propagate this exception,
                 # as we will never reuse this socket
                 pass
             finally:
-                socket.close()
+                try:
+                    socket.shutdown(_socket.SHUT_RDWR)
+                except OSError:
+                    # On macOS, an OSError is raised if there is no connection
+                    pass
+                finally:
+                    socket.close()
 
     def send_packet(self, packet: _SentPacketT) -> None:
         with self.__send_lock.get(), self.__convert_socket_error():
             socket = self.__ensure_connected()
             data: bytes = _concatenate_chunks(self.__producer(packet))
             buffer = memoryview(data)
+            timeout = None
+            retry_interval: float = self.__retry_interval
+            _is_ssl_socket = self.__is_ssl_socket
             try:
                 remaining: int = len(data)
                 while remaining > 0:
-                    nb_bytes_sent: int = 0
+                    sent: int
                     if _is_ssl_socket(socket):
-                        with self.__convert_ssl_eof_error():
-                            nb_bytes_sent = _retry_ssl_socket_method(socket, None, socket.send, buffer.toreadonly())
+                        sent = _retry_ssl_socket_method(socket, timeout, retry_interval, socket.send, buffer.toreadonly())
                     else:
-                        nb_bytes_sent = _retry_socket_method(socket, None, "write", socket.send, buffer.toreadonly())
-                    assert nb_bytes_sent >= 0, "socket.send() returned a negative integer"
+                        sent = _retry_socket_method(socket, timeout, retry_interval, "write", socket.send, buffer.toreadonly())
+                    assert sent >= 0, "socket.send() returned a negative integer"
                     _check_real_socket_state(socket)
-                    remaining -= nb_bytes_sent
-                    buffer = buffer[nb_bytes_sent:]
+                    remaining -= sent
+                    buffer = buffer[sent:]
+            except TimeoutError as exc:  # pragma: no cover
+                raise RuntimeError("socket.send() timed out with timeout=None ?") from exc
             finally:
                 del buffer, data
 
     def recv_packet(self, timeout: float | None = None) -> _ReceivedPacketT:
         with self.__receive_lock.get(), self.__convert_socket_error():
             consumer = self.__consumer
             next_packet = self.__next_packet
             try:
                 return next_packet(consumer)  # If there is enough data from last call to create a packet, return immediately
             except StopIteration:
                 pass
             socket = self.__ensure_connected()
             bufsize: int = self.__max_recv_size
             monotonic = _time_monotonic  # pull function to local namespace
+            retry_interval: float = self.__retry_interval
+            _is_ssl_socket = self.__is_ssl_socket
 
             while True:
                 try:
                     _start = monotonic()
-                    chunk: bytes = b""
+                    chunk: bytes
                     if _is_ssl_socket(socket):
-                        with self.__convert_ssl_eof_error():
-                            chunk = _retry_ssl_socket_method(socket, timeout, socket.recv, bufsize)
+                        chunk = _retry_ssl_socket_method(socket, timeout, retry_interval, socket.recv, bufsize)
                     else:
-                        chunk = _retry_socket_method(socket, timeout, "read", socket.recv, bufsize)
+                        chunk = _retry_socket_method(socket, timeout, retry_interval, "read", socket.recv, bufsize)
                     _end = monotonic()
                 except TimeoutError as exc:
                     if timeout is None:  # pragma: no cover
                         raise RuntimeError("socket.recv() timed out with timeout=None ?") from exc
                     break
                 if not chunk:
                     self.__eof_error(False)
@@ -324,32 +360,34 @@
         if self.__eof_reached:
             raise _error_from_errno(_errno.ECONNABORTED)
         return socket
 
     @_contextlib.contextmanager
     def __convert_socket_error(self) -> Iterator[None]:
         try:
-            yield
+            with self.__convert_ssl_eof_error():
+                yield
         except (ConnectionAbortedError, ClientClosedError):
             raise
         except ConnectionError as exc:
             self.__eof_error(exc)
         except OSError as exc:
             if exc.errno in CLOSED_SOCKET_ERRNOS:
                 self.__eof_error(exc)
             raise
 
     @_contextlib.contextmanager
     def __convert_ssl_eof_error(self) -> Iterator[None]:
-        import ssl
-
+        if _ssl_module is None:
+            yield
+            return
         try:
             yield
-        except ssl.SSLError as exc:
-            if isinstance(exc, ssl.SSLZeroReturnError) or _is_ssl_eof_error(exc):
+        except _ssl_module.SSLError as exc:
+            if isinstance(exc, _ssl_module.SSLZeroReturnError) or _is_ssl_eof_error(exc):
                 self.__eof_error(exc)
             raise
 
     def __eof_error(self, cause: BaseException | None | Literal[False]) -> NoReturn:
         self.__eof_reached = True
         if cause is False:
             raise _error_from_errno(_errno.ECONNABORTED)
@@ -363,14 +401,19 @@
 
     def fileno(self) -> int:
         with self.__socket_lock.get():
             if (socket := self.__socket) is None:
                 return -1
             return socket.fileno()
 
+    def __is_ssl_socket(self, socket: _socket.socket) -> TypeGuard[_SSLSocket]:
+        # Optimization: Instead of always do a isinstance(), do it once then use the TypeGuard to cast the socket type
+        # for static type checkers
+        return self.__over_ssl
+
     @property
     @final
     def socket(self) -> SocketProxy:
         return self.__socket_proxy
 
     @property
     @final
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/api_sync/client/udp.py` & `easynetwork-1.0.0rc4/src/easynetwork/api_sync/client/udp.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 #
 """Network client module"""
 
 from __future__ import annotations
 
 __all__ = ["UDPNetworkClient", "UDPNetworkEndpoint"]
 
+import contextlib as _contextlib
+import errno as _errno
 import socket as _socket
+import threading
+import time
 from operator import itemgetter as _itemgetter
 from typing import TYPE_CHECKING, Any, Generic, Iterator, Self, TypeVar, final, overload
 
 from ...exceptions import ClientClosedError, DatagramProtocolParseError
 from ...protocol import DatagramProtocol
 from ...tools._utils import (
     check_real_socket_state as _check_real_socket_state,
     check_socket_family as _check_socket_family,
     check_socket_no_ssl as _check_socket_no_ssl,
     ensure_datagram_socket_bound as _ensure_datagram_socket_bound,
+    error_from_errno as _error_from_errno,
     retry_socket_method as _retry_socket_method,
     set_reuseport as _set_reuseport,
 )
 from ...tools.lock import ForkSafeLock
-from ...tools.socket import MAX_DATAGRAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
+from ...tools.socket import CLOSED_SOCKET_ERRNOS, MAX_DATAGRAM_BUFSIZE, SocketAddress, SocketProxy, new_socket_address
 from .abc import AbstractNetworkClient
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 _ReceivedPacketT = TypeVar("_ReceivedPacketT")
 _SentPacketT = TypeVar("_SentPacketT")
@@ -39,58 +44,64 @@
         "__socket_proxy",
         "__addr",
         "__peer",
         "__protocol",
         "__send_lock",
         "__receive_lock",
         "__socket_lock",
+        "__retry_interval",
         "__weakref__",
     )
 
     @overload
     def __init__(
         self,
         /,
         protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         *,
         local_address: tuple[str | None, int] | None = ...,
         remote_address: tuple[str, int] | None = ...,
         reuse_port: bool = ...,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         /,
         protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         *,
         socket: _socket.socket,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     def __init__(
         self,
         /,
         protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        retry_interval: float = 1.0,
         **kwargs: Any,
     ) -> None:
         self.__socket: _socket.socket | None = None  # If any exception occurs, the client will already be in a closed state
         super().__init__()
 
-        from threading import Lock
-
-        self.__send_lock = ForkSafeLock(Lock)
-        self.__receive_lock = ForkSafeLock(Lock)
-        self.__socket_lock = ForkSafeLock(Lock)
+        self.__send_lock = ForkSafeLock(threading.Lock)
+        self.__receive_lock = ForkSafeLock(threading.Lock)
+        self.__socket_lock = ForkSafeLock(threading.Lock)
 
         assert isinstance(protocol, DatagramProtocol)
 
         self.__protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT] = protocol
 
+        self.__retry_interval = float(retry_interval)
+        if self.__retry_interval <= 0:
+            raise ValueError("retry_interval must be a strictly positive float or None")
+
         socket: _socket.socket
         peername: SocketAddress | None = None
         external_socket: bool
         match kwargs:
             case {"socket": _socket.socket() as socket, **remainder} if not remainder:
                 external_socket = True
             case _ if "socket" not in kwargs:
@@ -160,69 +171,83 @@
             socket.close()
 
     def send_packet_to(
         self,
         packet: _SentPacketT,
         address: tuple[str, int] | tuple[str, int, int, int] | None,
     ) -> None:
-        with self.__send_lock.get():
+        with self.__send_lock.get(), self.__convert_socket_error():
             if (socket := self.__socket) is None:
                 raise ClientClosedError("Closed client")
             if (remote_addr := self.__peer) is not None:
                 if address is not None:
                     if new_socket_address(address, socket.family) != remote_addr:
                         raise ValueError(f"Invalid address: must be None or {remote_addr}")
                     address = None
             elif address is None:
                 raise ValueError("Invalid address: must not be None")
             data: bytes = self.__protocol.make_datagram(packet)
+            retry_interval: float = self.__retry_interval
             try:
                 if address is None:
-                    _retry_socket_method(socket, None, "write", socket.send, data)
+                    _retry_socket_method(socket, None, retry_interval, "write", socket.send, data)
                 else:
-                    _retry_socket_method(socket, None, "write", socket.sendto, data, address)
+                    _retry_socket_method(socket, None, retry_interval, "write", socket.sendto, data, address)
                 _check_real_socket_state(socket)
+            except TimeoutError as exc:  # pragma: no cover
+                raise RuntimeError("socket.sendto() timed out with timeout=None ?") from exc
             finally:
                 del data
 
     def recv_packet_from(self, timeout: float | None = None) -> tuple[_ReceivedPacketT, SocketAddress]:
-        with self.__receive_lock.get():
+        with self.__receive_lock.get(), self.__convert_socket_error():
             if (socket := self.__socket) is None:
                 raise ClientClosedError("Closed client")
+            retry_interval: float = self.__retry_interval
+            bufsize: int = MAX_DATAGRAM_BUFSIZE
             try:
-                data, sender = _retry_socket_method(socket, timeout, "read", socket.recvfrom, MAX_DATAGRAM_BUFSIZE)
+                data, sender = _retry_socket_method(socket, timeout, retry_interval, "read", socket.recvfrom, bufsize)
             except TimeoutError as exc:
                 if timeout is None:  # pragma: no cover
                     raise RuntimeError("socket.recvfrom() timed out with timeout=None ?") from exc
                 raise TimeoutError("recv_packet() timed out") from None
             try:
                 return self.__protocol.build_packet_from_datagram(data), new_socket_address(sender, socket.family)
             except DatagramProtocolParseError:
                 raise
             except Exception as exc:  # pragma: no cover
                 raise RuntimeError(str(exc)) from exc
             finally:
                 del data
 
     def iter_received_packets_from(self, timeout: float | None = 0) -> Iterator[tuple[_ReceivedPacketT, SocketAddress]]:
-        from time import monotonic
+        monotonic = time.monotonic
 
         recv_packet_from = self.recv_packet_from
 
         while True:
             try:
                 _start = monotonic()
                 packet_tuple = recv_packet_from(timeout=timeout)
                 _end = monotonic()
             except OSError:
                 return
             yield packet_tuple
             if timeout is not None:
                 timeout -= _end - _start
 
+    @_contextlib.contextmanager
+    def __convert_socket_error(self) -> Iterator[None]:
+        try:
+            yield
+        except OSError as exc:
+            if exc.errno in CLOSED_SOCKET_ERRNOS:
+                raise _error_from_errno(_errno.ECONNABORTED) from exc
+            raise
+
     def get_local_address(self) -> SocketAddress:
         return self.__addr
 
     def get_remote_address(self) -> SocketAddress | None:
         return self.__peer
 
     def fileno(self) -> int:
@@ -245,23 +270,26 @@
         self,
         address: tuple[str, int],
         /,
         protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
         *,
         local_address: tuple[str, int] | None = ...,
         reuse_port: bool = ...,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     @overload
     def __init__(
         self,
         socket: _socket.socket,
         /,
         protocol: DatagramProtocol[_SentPacketT, _ReceivedPacketT],
+        *,
+        retry_interval: float = ...,
     ) -> None:
         ...
 
     def __init__(
         self,
         __arg: _socket.socket | tuple[str, int],
         /,
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/__init__.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/abc.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     "AbstractIncrementalPacketSerializer",
     "AbstractPacketSerializer",
 ]
 
 from abc import ABCMeta, abstractmethod
 from typing import Any, Generator, Generic, TypeVar
 
+from ..exceptions import DeserializeError
+from ..tools._utils import concatenate_chunks as _concatenate_chunks
+
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 class AbstractPacketSerializer(Generic[_ST_contra, _DT_co], metaclass=ABCMeta):
     __slots__ = ("__weakref__",)
 
@@ -41,21 +44,17 @@
         raise NotImplementedError
 
     @abstractmethod
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
         raise NotImplementedError
 
     def serialize(self, packet: _ST_contra) -> bytes:
-        from ..tools._utils import concatenate_chunks
-
-        return concatenate_chunks(self.incremental_serialize(packet))
+        return _concatenate_chunks(self.incremental_serialize(packet))
 
     def deserialize(self, data: bytes) -> _DT_co:
-        from ..exceptions import DeserializeError
-
         consumer: Generator[None, bytes, tuple[_DT_co, bytes]] = self.incremental_deserialize()
         try:
             next(consumer)
         except StopIteration:
             raise RuntimeError("self.incremental_deserialize() generator did not yield") from None
         packet: _DT_co
         remaining: bytes
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/base_stream.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/base_stream.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/cbor.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/cbor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/json.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import string
 from collections import Counter
 from dataclasses import asdict as dataclass_asdict, dataclass
 from typing import Any, Callable, Generator, TypeVar, final
 
 from ..exceptions import DeserializeError, IncrementalDeserializeError
+from ..tools._utils import iter_bytes
 from .abc import AbstractIncrementalPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 _JSON_VALUE_BYTES: frozenset[int] = frozenset(bytes(string.digits + string.ascii_letters + string.punctuation, "ascii"))
@@ -46,28 +47,28 @@
     parse_constant: Callable[[str], Any] | None = None
     object_pairs_hook: Callable[[list[tuple[str, Any]]], Any] | None = None
     strict: bool = True
 
 
 class _JSONParser:
     @staticmethod
-    def raw_parse() -> Generator[None, bytes, tuple[bytes, bytes]]:
-        import struct
-
-        def escaped(partial_document: bytes) -> bool:
-            return ((len(partial_document) - len(partial_document.rstrip(b"\\"))) % 2) == 1
+    def _escaped(partial_document: bytes) -> bool:
+        return ((len(partial_document) - len(partial_document.rstrip(b"\\"))) % 2) == 1
 
+    @staticmethod
+    def raw_parse() -> Generator[None, bytes, tuple[bytes, bytes]]:
+        escaped = _JSONParser._escaped
         enclosure_counter: Counter[bytes] = Counter()
         partial_document: bytearray = bytearray()
         first_enclosure: bytes = b""
         while True:
             while not (chunk := (yield)):  # Skip empty bytes
                 continue
             char: bytes
-            for nb_chars, char in enumerate(struct.unpack(f"{len(chunk)}c", chunk), start=1):
+            for nb_chars, char in enumerate(iter_bytes(chunk), start=1):
                 match char:
                     case b'"' if not escaped(partial_document):
                         enclosure_counter[b'"'] = 0 if enclosure_counter[b'"'] == 1 else 1
                     case _ if enclosure_counter[b'"'] > 0:
                         partial_document.extend(char)
                         continue
                     case b"{" | b"[":
@@ -99,25 +100,25 @@
                 continue
             break
         buffer_array.extend(chunk[:non_printable_idx])
         return buffer_array, chunk[non_printable_idx:]
 
 
 class JSONSerializer(AbstractIncrementalPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__encoder", "__decoder", "__encoding", "__unicode_errors")
+    __slots__ = ("__encoder", "__decoder", "__decoder_error_cls", "__encoding", "__unicode_errors")
 
     def __init__(
         self,
         encoder_config: JSONEncoderConfig | None = None,
         decoder_config: JSONDecoderConfig | None = None,
         *,
         encoding: str = "utf-8",
         unicode_errors: str = "strict",
     ) -> None:
-        from json import JSONDecoder, JSONEncoder
+        from json import JSONDecodeError, JSONDecoder, JSONEncoder
 
         super().__init__()
         self.__encoder: JSONEncoder
         self.__decoder: JSONDecoder
 
         if encoder_config is None:
             encoder_config = JSONEncoderConfig()
@@ -127,14 +128,15 @@
         if decoder_config is None:
             decoder_config = JSONDecoderConfig()
         elif not isinstance(decoder_config, JSONDecoderConfig):
             raise TypeError(f"Invalid decoder config: expected {JSONDecoderConfig.__name__}, got {type(decoder_config).__name__}")
 
         self.__encoder = JSONEncoder(**dataclass_asdict(encoder_config))
         self.__decoder = JSONDecoder(**dataclass_asdict(decoder_config))
+        self.__decoder_error_cls = JSONDecodeError
 
         self.__encoding: str = encoding
         self.__unicode_errors: str = unicode_errors
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         return self.__encoder.encode(packet).encode(self.__encoding, self.__unicode_errors)
@@ -145,38 +147,34 @@
         str_errors: str = self.__unicode_errors
         for chunk in self.__encoder.iterencode(packet):
             yield chunk.encode(encoding, str_errors)
         yield b"\n"
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
-        from json import JSONDecodeError
-
         try:
             document: str = data.decode(self.__encoding, self.__unicode_errors)
         except UnicodeError as exc:
             raise DeserializeError(f"Unicode decode error: {exc}", error_info={"data": data}) from exc
         try:
             packet: _DT_co = self.__decoder.decode(document)
-        except JSONDecodeError as exc:
+        except self.__decoder_error_cls as exc:
             raise DeserializeError(
                 f"JSON decode error: {exc}",
                 error_info={
                     "document": exc.doc,
                     "position": exc.pos,
                     "lineno": exc.lineno,
                     "colno": exc.colno,
                 },
             ) from exc
         return packet
 
     @final
     def incremental_deserialize(self) -> Generator[None, bytes, tuple[_DT_co, bytes]]:
-        from json import JSONDecodeError
-
         complete_document, remaining_data = yield from _JSONParser.raw_parse()
 
         if not complete_document:
             complete_document = remaining_data
             remaining_data = b""
 
         packet: _DT_co
@@ -186,15 +184,15 @@
             raise IncrementalDeserializeError(
                 f"Unicode decode error: {exc}",
                 remaining_data=remaining_data,
                 error_info={"data": complete_document},
             ) from exc
         try:
             packet, end = self.__decoder.raw_decode(document)
-        except JSONDecodeError as exc:
+        except self.__decoder_error_cls as exc:
             raise IncrementalDeserializeError(
                 f"JSON decode error: {exc}",
                 remaining_data=remaining_data,
                 error_info={
                     "document": exc.doc,
                     "position": exc.pos,
                     "lineno": exc.lineno,
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/line.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/line.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/msgpack.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/msgpack.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     unicode_errors: str = "strict"
     object_hook: Callable[[dict[Any, Any]], Any] | None = None
     object_pairs_hook: Callable[[list[tuple[Any, Any]]], Any] | None = None
     ext_hook: Callable[[int, bytes], Any] = field(default_factory=_get_default_ext_hook)
 
 
 class MessagePackSerializer(AbstractPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__packb", "__unpackb")
+    __slots__ = ("__packb", "__unpackb", "__unpack_out_of_data_cls", "__unpack_extra_data_cls")
 
     def __init__(
         self,
         packer_config: MessagePackerConfig | None = None,
         unpacker_config: MessageUnpackerConfig | None = None,
     ) -> None:
         try:
@@ -80,24 +80,24 @@
         elif not isinstance(unpacker_config, MessageUnpackerConfig):
             raise TypeError(
                 f"Invalid unpacker config: expected {MessageUnpackerConfig.__name__}, got {type(unpacker_config).__name__}"
             )
 
         self.__packb = partial(msgpack.packb, **dataclass_asdict(packer_config), autoreset=True)
         self.__unpackb = partial(msgpack.unpackb, **dataclass_asdict(unpacker_config))
+        self.__unpack_out_of_data_cls = msgpack.OutOfData
+        self.__unpack_extra_data_cls = msgpack.ExtraData
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         return self.__packb(packet)
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
-        import msgpack
-
         try:
             return self.__unpackb(data)
-        except msgpack.OutOfData as exc:
+        except self.__unpack_out_of_data_cls as exc:
             raise DeserializeError("Missing data to create packet", error_info={"data": data}) from exc
-        except msgpack.ExtraData as exc:
+        except self.__unpack_extra_data_cls as exc:
             raise DeserializeError("Extra data caught", error_info={"packet": exc.unpacked, "extra": exc.extra}) from exc  # type: ignore[attr-defined]
         except Exception as exc:  # The documentation says to catch all exceptions :)
             raise DeserializeError(str(exc) or "Invalid token", error_info={"data": data}) from exc
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/pickle.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/pickle.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,31 +8,38 @@
 
 __all__ = [
     "PickleSerializer",
     "PicklerConfig",
     "UnpicklerConfig",
 ]
 
-import pickle as _pickle
-import pickletools as _pickletools
-from dataclasses import asdict as dataclass_asdict, dataclass
+from dataclasses import asdict as dataclass_asdict, dataclass, field
 from functools import partial
 from io import BytesIO
-from typing import IO, Callable, TypeVar, final
+from typing import IO, TYPE_CHECKING, Callable, TypeVar, final
 
 from ..exceptions import DeserializeError
 from .abc import AbstractPacketSerializer
 
+if TYPE_CHECKING:
+    from pickle import Pickler as _Pickler, Unpickler as _Unpickler
+
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
+def _get_default_pickler_protocol() -> int:
+    import pickle
+
+    return pickle.DEFAULT_PROTOCOL
+
+
 @dataclass(kw_only=True)
 class PicklerConfig:
-    protocol: int = _pickle.DEFAULT_PROTOCOL
+    protocol: int = field(default_factory=_get_default_pickler_protocol)
     fix_imports: bool = False
 
 
 @dataclass(kw_only=True)
 class UnpicklerConfig:
     fix_imports: bool = False
     encoding: str = "utf-8"
@@ -43,45 +50,52 @@
     __slots__ = ("__optimize", "__pickler_cls", "__unpickler_cls")
 
     def __init__(
         self,
         pickler_config: PicklerConfig | None = None,
         unpickler_config: UnpicklerConfig | None = None,
         *,
-        pickler_cls: type[_pickle.Pickler] | None = None,
-        unpickler_cls: type[_pickle.Unpickler] | None = None,
+        pickler_cls: type[_Pickler] | None = None,
+        unpickler_cls: type[_Unpickler] | None = None,
         optimize: bool = False,
     ) -> None:
         super().__init__()
-        self.__optimize = bool(optimize)
-        self.__pickler_cls: Callable[[IO[bytes]], _pickle.Pickler]
-        self.__unpickler_cls: Callable[[IO[bytes]], _pickle.Unpickler]
+
+        import pickle
+
+        self.__optimize: Callable[[bytes], bytes] | None = None
+        if optimize:
+            import pickletools
+
+            self.__optimize = pickletools.optimize
+        self.__pickler_cls: Callable[[IO[bytes]], _Pickler]
+        self.__unpickler_cls: Callable[[IO[bytes]], _Unpickler]
 
         if pickler_config is None:
             pickler_config = PicklerConfig()
         elif not isinstance(pickler_config, PicklerConfig):
             raise TypeError(f"Invalid pickler config: expected {PicklerConfig.__name__}, got {type(pickler_config).__name__}")
 
         if unpickler_config is None:
             unpickler_config = UnpicklerConfig()
         elif not isinstance(unpickler_config, UnpicklerConfig):
             raise TypeError(
                 f"Invalid unpickler config: expected {UnpicklerConfig.__name__}, got {type(unpickler_config).__name__}"
             )
 
-        self.__pickler_cls = partial(pickler_cls or _pickle.Pickler, **dataclass_asdict(pickler_config), buffer_callback=None)
-        self.__unpickler_cls = partial(unpickler_cls or _pickle.Unpickler, **dataclass_asdict(unpickler_config), buffers=None)
+        self.__pickler_cls = partial(pickler_cls or pickle.Pickler, **dataclass_asdict(pickler_config), buffer_callback=None)
+        self.__unpickler_cls = partial(unpickler_cls or pickle.Unpickler, **dataclass_asdict(unpickler_config), buffers=None)
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         with BytesIO() as buffer:
             self.__pickler_cls(buffer).dump(packet)
             pickle: bytes = buffer.getvalue()
-        if self.__optimize:
-            pickle = _pickletools.optimize(pickle)
+        if (optimize := self.__optimize) is not None:
+            pickle = optimize(pickle)
         return pickle
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         with BytesIO(data) as buffer:
             del data
             try:
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/struct.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,44 @@
 #
 """struct.Struct-based network packet serializer module"""
 
 from __future__ import annotations
 
 __all__ = ["AbstractStructSerializer", "NamedTupleStructSerializer"]
 
-import struct as _struct
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, Generic, Iterable, NamedTuple, TypeVar, final
 
 from ..exceptions import DeserializeError
 from .base_stream import FixedSizePacketSerializer
 
 if TYPE_CHECKING:
+    from struct import Struct as _Struct
+
     from _typeshed import SupportsKeysAndGetItem
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 _ENDIANNESS_CHARACTERS: frozenset[str] = frozenset({"@", "=", "<", ">", "!"})
 
 
 class AbstractStructSerializer(FixedSizePacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__s",)
+    __slots__ = ("__s", "__error_cls")
 
     def __init__(self, format: str) -> None:
+        from struct import Struct, error
+
         if format and format[0] not in _ENDIANNESS_CHARACTERS:
             format = f"!{format}"  # network byte order
-        struct = _struct.Struct(format)
+        struct = Struct(format)
         super().__init__(struct.size)
-        self.__s: _struct.Struct = struct
+        self.__s: _Struct = struct
+        self.__error_cls = error
 
     @abstractmethod
     def iter_values(self, packet: _ST_contra) -> Iterable[Any]:
         raise NotImplementedError
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
@@ -47,27 +51,27 @@
     def from_tuple(self, t: tuple[Any, ...]) -> _DT_co:
         raise NotImplementedError
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         try:
             packet_tuple: tuple[Any, ...] = self.__s.unpack(data)
-        except _struct.error as exc:
+        except self.__error_cls as exc:
             raise DeserializeError(f"Invalid value: {exc}", error_info={"data": data}) from exc
         try:
             return self.from_tuple(packet_tuple)
         except Exception as exc:
             raise DeserializeError(
                 f"Error when building packet from unpacked struct value: {exc}",
                 error_info={"unpacked_struct": packet_tuple},
             ) from exc
 
     @property
     @final
-    def struct(self) -> _struct.Struct:
+    def struct(self) -> _Struct:
         return self.__s
 
 
 _NT = TypeVar("_NT", bound=NamedTuple)
 
 
 class NamedTupleStructSerializer(AbstractStructSerializer[_NT, _NT], Generic[_NT]):
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/base64.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/base64.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,38 +6,40 @@
 
 from __future__ import annotations
 
 __all__ = [
     "Base64EncodedSerializer",
 ]
 
-import base64
-import binascii
-from hashlib import sha256 as hashlib_sha256
-from hmac import compare_digest, digest as hmac_digest
+import os
 from typing import Callable, TypeVar, assert_never, final
 
 from ...exceptions import DeserializeError
 from ..abc import AbstractPacketSerializer
 from ..base_stream import AutoSeparatedPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 class Base64EncodedSerializer(AutoSeparatedPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__serializer", "__checksum")
+    __slots__ = ("__serializer", "__encode", "__decode", "__compare_digest", "__decode_error_cls", "__checksum")
 
     def __init__(
         self,
         serializer: AbstractPacketSerializer[_ST_contra, _DT_co],
         *,
         checksum: bool | str | bytes = False,
         separator: bytes = b"\r\n",
     ) -> None:
+        import base64
+        import binascii
+        from hashlib import sha256 as hashlib_sha256
+        from hmac import compare_digest, digest as hmac_digest
+
         super().__init__(separator=separator)
         assert isinstance(serializer, AbstractPacketSerializer)
         self.__serializer: AbstractPacketSerializer[_ST_contra, _DT_co] = serializer
         self.__checksum: Callable[[bytes], bytes] | None
         match checksum:
             case False:
                 self.__checksum = None
@@ -50,31 +52,36 @@
                     raise ValueError("signing key must be 32 url-safe base64-encoded bytes.") from exc
                 if len(key) != 32:
                     raise ValueError("signing key must be 32 url-safe base64-encoded bytes.")
                 self.__checksum = lambda data: hmac_digest(key, data, "sha256")
             case _:  # pragma: no cover
                 assert_never(checksum)
 
+        self.__encode = base64.urlsafe_b64encode
+        self.__decode = base64.urlsafe_b64decode
+        self.__decode_error_cls = binascii.Error
+        self.__compare_digest = compare_digest
+
     @classmethod
     def generate_key(cls) -> bytes:
-        from os import urandom
+        import base64
 
-        return base64.urlsafe_b64encode(urandom(32))
+        return base64.urlsafe_b64encode(os.urandom(32))
 
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         data = self.__serializer.serialize(packet)
         if (checksum := self.__checksum) is not None:
             data += checksum(data)
-        return base64.urlsafe_b64encode(data)
+        return self.__encode(data)
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
         try:
-            data = base64.urlsafe_b64decode(data)
-        except binascii.Error:
+            data = self.__decode(data)
+        except self.__decode_error_cls:
             raise DeserializeError("Invalid token") from None
         if (checksum := self.__checksum) is not None:
             data, digest = data[:-32], data[-32:]
-            if not compare_digest(checksum(data), digest):
+            if not self.__compare_digest(checksum(data), digest):
                 raise DeserializeError("Invalid token", error_info=None)
         return self.__serializer.deserialize(data)
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/compressor.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/compressor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 __all__ = [
     "AbstractCompressorSerializer",
     "BZ2CompressorSerializer",
     "ZlibCompressorSerializer",
 ]
 
 import abc
-import bz2
-import zlib
 from collections import deque
-from typing import Generator, Protocol, TypeVar, final
+from typing import Final, Generator, Protocol, TypeVar, final
 
 from ...exceptions import DeserializeError, IncrementalDeserializeError
 from ..abc import AbstractIncrementalPacketSerializer, AbstractPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
@@ -141,41 +139,51 @@
                 error_info=exc.error_info,
             ) from exc
 
         return packet, unused_data
 
 
 class BZ2CompressorSerializer(AbstractCompressorSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__compresslevel",)
+    __slots__ = ("__compresslevel", "__compressor_factory", "__decompressor_factory")
+
+    BEST_COMPRESSION_LEVEL: Final[int] = 9
+
+    def __init__(self, serializer: AbstractPacketSerializer[_ST_contra, _DT_co], *, compress_level: int | None = None) -> None:
+        import bz2
 
-    def __init__(self, serializer: AbstractPacketSerializer[_ST_contra, _DT_co], *, compress_level: int = 9) -> None:
         super().__init__(serializer=serializer, expected_decompress_error=OSError)
-        self.__compresslevel: int = compress_level
+        self.__compresslevel: int = compress_level if compress_level is not None else self.BEST_COMPRESSION_LEVEL
+        self.__compressor_factory = bz2.BZ2Compressor
+        self.__decompressor_factory = bz2.BZ2Decompressor
 
     @final
-    def new_compressor_stream(self) -> bz2.BZ2Compressor:
-        return bz2.BZ2Compressor(self.__compresslevel)
+    def new_compressor_stream(self) -> CompressorInterface:
+        return self.__compressor_factory(self.__compresslevel)
 
     @final
-    def new_decompressor_stream(self) -> bz2.BZ2Decompressor:
-        return bz2.BZ2Decompressor()
+    def new_decompressor_stream(self) -> DecompressorInterface:
+        return self.__decompressor_factory()
 
 
 class ZlibCompressorSerializer(AbstractCompressorSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__compresslevel",)
+    __slots__ = ("__compresslevel", "__compressor_factory", "__decompressor_factory")
 
     def __init__(
         self,
         serializer: AbstractPacketSerializer[_ST_contra, _DT_co],
         *,
-        compress_level: int = zlib.Z_BEST_COMPRESSION,
+        compress_level: int | None = None,
     ) -> None:
+        import zlib
+
         super().__init__(serializer=serializer, expected_decompress_error=zlib.error)
-        self.__compresslevel: int = compress_level
+        self.__compresslevel: int = compress_level if compress_level is not None else zlib.Z_BEST_COMPRESSION
+        self.__compressor_factory = zlib.compressobj
+        self.__decompressor_factory = zlib.decompressobj
 
     @final
-    def new_compressor_stream(self) -> zlib._Compress:
-        return zlib.compressobj(self.__compresslevel)
+    def new_compressor_stream(self) -> CompressorInterface:
+        return self.__compressor_factory(self.__compresslevel)
 
     @final
-    def new_decompressor_stream(self) -> zlib._Decompress:
-        return zlib.decompressobj()
+    def new_decompressor_stream(self) -> DecompressorInterface:
+        return self.__decompressor_factory()
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/serializers/wrapper/encryptor.py` & `easynetwork-1.0.0rc4/src/easynetwork/serializers/wrapper/encryptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ..base_stream import AutoSeparatedPacketSerializer
 
 _ST_contra = TypeVar("_ST_contra", contravariant=True)
 _DT_co = TypeVar("_DT_co", covariant=True)
 
 
 class EncryptorSerializer(AutoSeparatedPacketSerializer[_ST_contra, _DT_co]):
-    __slots__ = ("__serializer", "__fernet", "__token_ttl")
+    __slots__ = ("__serializer", "__fernet", "__token_ttl", "__invalid_token_cls")
 
     def __init__(
         self,
         serializer: AbstractPacketSerializer[_ST_contra, _DT_co],
         key: str | bytes,
         *,
         token_ttl: int | None = None,
@@ -37,14 +37,15 @@
             raise ModuleNotFoundError("encryption dependencies are missing. Consider adding 'encryption' extra") from exc
 
         super().__init__(separator=separator)
         assert isinstance(serializer, AbstractPacketSerializer)
         self.__serializer: AbstractPacketSerializer[_ST_contra, _DT_co] = serializer
         self.__fernet = cryptography.fernet.Fernet(key)
         self.__token_ttl = token_ttl
+        self.__invalid_token_cls = cryptography.fernet.InvalidToken
 
     @classmethod
     def generate_key(cls) -> bytes:
         try:
             import cryptography.fernet
         except ModuleNotFoundError as exc:  # pragma: no cover
             raise ModuleNotFoundError("encryption dependencies are missing. Consider adding 'encryption' extra") from exc
@@ -54,14 +55,12 @@
     @final
     def serialize(self, packet: _ST_contra) -> bytes:
         data = self.__serializer.serialize(packet)
         return self.__fernet.encrypt(data)
 
     @final
     def deserialize(self, data: bytes) -> _DT_co:
-        from cryptography.fernet import InvalidToken
-
         try:
             data = self.__fernet.decrypt(data, ttl=self.__token_ttl)
-        except InvalidToken:
+        except self.__invalid_token_cls:
             raise DeserializeError("Invalid token", error_info=None) from None
         return self.__serializer.deserialize(data)
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/tools/_utils.py` & `easynetwork-1.0.0rc4/src/easynetwork/tools/_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,20 +25,31 @@
 import contextlib
 import errno as _errno
 import os
 import selectors as _selectors
 import socket as _socket
 import time
 import traceback
+from struct import unpack
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Literal, ParamSpec, TypeGuard, TypeVar, assert_never
 
+try:
+    import ssl as _ssl
+except ImportError:  # pragma: no cover
+    ssl = None
+else:
+    ssl = _ssl
+    del _ssl
+
+from .socket import AddressFamily
+
 if TYPE_CHECKING:
     from ssl import SSLError as _SSLError, SSLSocket as _SSLSocket
 
-    from .socket import SocketProxy as _SocketProxy
+    from .socket import SupportsSocketOptions
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 
 def replace_kwargs(kwargs: dict[str, Any], keys: dict[str, str]) -> None:
     if not keys:
@@ -53,23 +64,21 @@
 
 
 def error_from_errno(errno: int) -> OSError:
     return OSError(errno, os.strerror(errno))
 
 
 def check_socket_family(family: int) -> None:
-    from .socket import AddressFamily
-
     supported_families: dict[str, int] = dict(AddressFamily.__members__)
 
     if family not in list(supported_families.values()):
         raise ValueError(f"Only these families are supported: {', '.join(supported_families)}")
 
 
-def check_real_socket_state(socket: _socket.socket | _SocketProxy) -> None:
+def check_real_socket_state(socket: SupportsSocketOptions) -> None:
     """Verify socket saved error and raise OSError if there is one
 
     There is some functions such as socket.send() which do not immediately fail and save the errno
     in SO_ERROR socket option because the error spawn after the action was sent to the kernel (Something weird)
 
     On Windows: The returned value should be the error returned by WSAGetLastError(), but the socket methods always call
     this function to raise an error, so getsockopt(SO_ERROR) will most likely always return zero :)
@@ -77,19 +86,16 @@
     errno = socket.getsockopt(_socket.SOL_SOCKET, _socket.SO_ERROR)
     if errno != 0:
         # The SO_ERROR is automatically reset to zero after getting the value
         raise error_from_errno(errno)
 
 
 def is_ssl_socket(socket: _socket.socket) -> TypeGuard[_SSLSocket]:
-    try:
-        import ssl
-    except ImportError:  # pragma: no cover
+    if ssl is None:
         return False
-
     return isinstance(socket, ssl.SSLSocket)
 
 
 def check_socket_no_ssl(socket: _socket.socket) -> None:
     if is_ssl_socket(socket):
         raise TypeError("ssl.SSLSocket instances are forbidden")
 
@@ -109,79 +115,106 @@
             ready_list = selector.select(timeout)
         except (OSError, ValueError):
             # There will be a OSError when using this socket afterward.
             return True
         return len(ready_list) > 0
 
 
-def retry_socket_method(
+class _WouldBlock(Exception):
+    def __init__(self, event: Literal["read", "write"]) -> None:
+        super().__init__(event)
+        self.event: Literal["read", "write"] = event
+
+
+def _retry_impl(
     socket: _socket.socket,
     timeout: float | None,
-    event: Literal["read", "write"],
-    socket_method: Callable[_P, _R],
-    /,
-    *args: _P.args,
-    **kwargs: _P.kwargs,
+    retry_interval: float | None,
+    callback: Callable[[], _R],
 ) -> _R:
-    assert not is_ssl_socket(socket), "ssl.SSLSocket instances are forbidden"
     assert socket.gettimeout() == 0, "The socket must be non-blocking"
+    assert retry_interval is None or retry_interval > 0, "retry_interval must be a strictly positive float or None"
+
     monotonic = time.monotonic  # pull function to local namespace
+    event: Literal["read", "write"]
+    if timeout == float("+inf"):
+        timeout = None
+    if retry_interval == float("+inf"):
+        retry_interval = None
     while True:
         try:
-            return socket_method(*args, **kwargs)
-        except BlockingIOError:
-            pass
+            return callback()
+        except _WouldBlock as exc:
+            event = exc.event
         if timeout is not None and timeout <= 0:
             break
+        is_retry_interval: bool
+        wait_time: float | None
+        if retry_interval is None or (timeout is not None and timeout <= retry_interval):
+            is_retry_interval = False
+            wait_time = timeout
+        else:
+            is_retry_interval = True
+            wait_time = retry_interval
         _start = monotonic()
-        if not wait_socket_available(socket, timeout, event):
-            break
+        if not wait_socket_available(socket, wait_time, event):
+            if not is_retry_interval:
+                break
         _end = monotonic()
         if timeout is not None:
             timeout -= _end - _start
     raise error_from_errno(_errno.ETIMEDOUT)
 
 
+def retry_socket_method(
+    socket: _socket.socket,
+    timeout: float | None,
+    retry_interval: float | None,
+    event: Literal["read", "write"],
+    socket_method: Callable[_P, _R],
+    /,
+    *args: _P.args,
+    **kwargs: _P.kwargs,
+) -> _R:
+    assert not is_ssl_socket(socket), "ssl.SSLSocket instances are forbidden"
+
+    def callback() -> _R:
+        try:
+            return socket_method(*args, **kwargs)
+        except (BlockingIOError, TimeoutError, InterruptedError):
+            raise _WouldBlock(event) from None
+
+    return _retry_impl(socket, timeout, retry_interval, callback)
+
+
 def retry_ssl_socket_method(
     socket: _SSLSocket,
     timeout: float | None,
+    retry_interval: float | None,
     socket_method: Callable[_P, _R],
     /,
     *args: _P.args,
     **kwargs: _P.kwargs,
 ) -> _R:
     assert is_ssl_socket(socket), "Expected an ssl.SSLSocket instance"
-    assert socket.gettimeout() == 0, "The socket must be non-blocking"
 
-    import ssl
-
-    monotonic = time.monotonic  # pull function to local namespace
-    event: Literal["read", "write"]
-    while True:
+    def callback() -> _R:
+        assert ssl is not None, "stdlib ssl module not available"
         try:
             return socket_method(*args, **kwargs)
         except (ssl.SSLWantReadError, ssl.SSLSyscallError):
-            event = "read"
+            raise _WouldBlock("read") from None
         except ssl.SSLWantWriteError:
-            event = "write"
-        if timeout is not None and timeout <= 0:
-            break
-        _start = monotonic()
-        if not wait_socket_available(socket, timeout, event):
-            break
-        _end = monotonic()
-        if timeout is not None:
-            timeout -= _end - _start
-    raise error_from_errno(_errno.ETIMEDOUT)
+            raise _WouldBlock("write") from None
+
+    return _retry_impl(socket, timeout, retry_interval, callback)
 
 
 def is_ssl_eof_error(exc: BaseException) -> TypeGuard[_SSLError]:
-    try:
-        import ssl
-    except ImportError:  # pragma: no cover
+    if ssl is None:
         return False
 
     match exc:
         case ssl.SSLEOFError():
             return True
         case ssl.SSLError() if hasattr(exc, "strerror") and "UNEXPECTED_EOF_WHILE_READING" in exc.strerror:
             # From Trio project:
@@ -190,17 +223,19 @@
             # This stringly-typed error check is borrowed from the AnyIO
             # project.
             return True
     return False
 
 
 def concatenate_chunks(chunks_iterable: Iterable[bytes]) -> bytes:
-    # The list call should be roughly
-    # equivalent to the PySequence_Fast that ''.join() would do.
-    return b"".join(list(chunks_iterable))
+    return b"".join(chunks_iterable)
+
+
+def iter_bytes(b: bytes | bytearray) -> Iterable[bytes]:
+    return unpack(f"{len(b)}c", b)
 
 
 def ensure_datagram_socket_bound(sock: _socket.socket) -> None:
     assert sock.family in (_socket.AF_INET, _socket.AF_INET6), "Invalid socket family."
     if sock.type != _socket.SOCK_DGRAM:
         raise ValueError("Invalid socket type. Expected SOCK_DGRAM socket.")
     try:
@@ -210,32 +245,32 @@
             raise
         is_bound = False
 
     if not is_bound:
         sock.bind(("", 0))
 
 
-def set_reuseport(sock: _socket.socket) -> None:
+def set_reuseport(sock: SupportsSocketOptions) -> None:
     if not hasattr(_socket, "SO_REUSEPORT"):
         raise ValueError("reuse_port not supported by socket module")
     else:
         try:
             sock.setsockopt(_socket.SOL_SOCKET, _socket.SO_REUSEPORT, True)
         except OSError:
             raise ValueError("reuse_port not supported by socket module, SO_REUSEPORT defined but not implemented.") from None
 
 
-def set_tcp_nodelay(sock: _socket.socket | _SocketProxy) -> None:
+def set_tcp_nodelay(sock: SupportsSocketOptions) -> None:
     try:
         sock.setsockopt(_socket.IPPROTO_TCP, _socket.TCP_NODELAY, True)
     except (OSError, AttributeError):  # pragma: no cover
         pass
 
 
-def set_tcp_keepalive(sock: _socket.socket | _SocketProxy) -> None:
+def set_tcp_keepalive(sock: SupportsSocketOptions) -> None:
     try:
         sock.setsockopt(_socket.SOL_SOCKET, _socket.SO_KEEPALIVE, True)
     except (OSError, AttributeError):  # pragma: no cover
         pass
 
 
 def open_listener_sockets_from_getaddrinfo_result(
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/tools/lock.py` & `easynetwork-1.0.0rc4/src/easynetwork/tools/lock.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/tools/socket.py` & `easynetwork-1.0.0rc4/src/easynetwork/tools/socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "AddressFamily",
     "ISocket",
     "MAX_DATAGRAM_BUFSIZE",
     "MAX_STREAM_BUFSIZE",
     "SSL_HANDSHAKE_TIMEOUT",
     "SSL_SHUTDOWN_TIMEOUT",
     "SocketProxy",
+    "SupportsSocketOptions",
     "new_socket_address",
 ]
 
 import contextlib
 import errno as _errno
 import functools
 import socket as _socket
@@ -151,24 +152,15 @@
 SSL_HANDSHAKE_TIMEOUT = 60.0
 
 # Number of seconds to wait for SSL shutdown to complete
 # The default timeout mimics lingering_time
 SSL_SHUTDOWN_TIMEOUT = 30.0
 
 
-class ISocket(Protocol):
-    def fileno(self) -> int:  # pragma: no cover
-        ...
-
-    def dup(self) -> _socket.socket:  # pragma: no cover
-        ...
-
-    def get_inheritable(self) -> bool:  # pragma: no cover
-        ...
-
+class SupportsSocketOptions(Protocol):
     @overload
     def getsockopt(self, __level: int, __optname: int, /) -> int:
         ...
 
     @overload
     def getsockopt(self, __level: int, __optname: int, __buflen: int, /) -> bytes:
         ...
@@ -177,14 +169,22 @@
     def setsockopt(self, __level: int, __optname: int, __value: int | ReadableBuffer, /) -> None:
         ...
 
     @overload
     def setsockopt(self, __level: int, __optname: int, __value: None, __optlen: int, /) -> None:
         ...
 
+
+class ISocket(SupportsSocketOptions, Protocol):
+    def fileno(self) -> int:  # pragma: no cover
+        ...
+
+    def get_inheritable(self) -> bool:  # pragma: no cover
+        ...
+
     def getpeername(self) -> _socket._RetAddress:  # pragma: no cover
         ...
 
     def getsockname(self) -> _socket._RetAddress:  # pragma: no cover
         ...
 
     @property  # pragma: no cover
@@ -249,15 +249,17 @@
                 return run(__func)
             return __func(*args, **kwargs)
 
     def fileno(self) -> int:
         return self.__execute(self.__socket.fileno)
 
     def dup(self) -> _socket.socket:
-        return self.__execute(self.__socket.dup)
+        new_socket = _socket.fromfd(self.fileno(), self.family, self.type, self.proto)
+        new_socket.setblocking(False)
+        return new_socket
 
     def get_inheritable(self) -> bool:
         return self.__execute(self.__socket.get_inheritable)
 
     @overload
     def getsockopt(self, __level: int, __optname: int, /) -> int:
         ...
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork/tools/stream.py` & `easynetwork-1.0.0rc4/src/easynetwork/tools/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 __all__ = [
     "StreamDataConsumer",
     "StreamDataProducer",
 ]
 
+import threading
 from collections import deque
 from typing import Any, Generator, Generic, Iterator, TypeVar, final
 
 from ..exceptions import StreamProtocolParseError
 from ..protocol import StreamProtocol
 from .lock import ForkSafeLock
 
@@ -33,17 +34,15 @@
     def __init__(self, protocol: StreamProtocol[_SentPacketT, Any]) -> None:
         super().__init__()
         assert isinstance(protocol, StreamProtocol)
         self.__p: StreamProtocol[_SentPacketT, Any] = protocol
         self.__g: Generator[bytes, None, None] | None = None
         self.__q: deque[_SentPacketT] = deque()
 
-        from threading import Lock
-
-        self.__lock = ForkSafeLock(Lock)
+        self.__lock = ForkSafeLock(threading.Lock)
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             generator, self.__g = self.__g, None
         except AttributeError:
             return
         try:
@@ -106,17 +105,15 @@
     def __init__(self, protocol: StreamProtocol[Any, _ReceivedPacketT]) -> None:
         super().__init__()
         assert isinstance(protocol, StreamProtocol)
         self.__p: StreamProtocol[Any, _ReceivedPacketT] = protocol
         self.__c: Generator[None, bytes, tuple[_ReceivedPacketT, bytes]] | None = None
         self.__b: bytes = b""
 
-        from threading import Lock
-
-        self.__lock = ForkSafeLock(Lock)
+        self.__lock = ForkSafeLock(threading.Lock)
 
     def __del__(self) -> None:  # pragma: no cover
         try:
             consumer, self.__c = self.__c, None
         except AttributeError:
             return
         try:
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/_utils.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/_utils.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/backend.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,38 +6,51 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["AsyncioBackend"]
 
 import asyncio
+import asyncio.base_events
 import contextvars
 import functools
+import itertools
+import os
 import socket as _socket
+import sys
 from typing import TYPE_CHECKING, Any, AsyncContextManager, Callable, Coroutine, NoReturn, ParamSpec, Sequence, TypeVar
 
+try:
+    import ssl as _ssl
+except ImportError:  # pragma: no cover
+    ssl = None
+else:
+    ssl = _ssl
+    del _ssl
+
 from easynetwork.api_async.backend.abc import AbstractAsyncBackend
 from easynetwork.api_async.backend.sniffio import current_async_library_cvar as _sniffio_current_async_library_cvar
+from easynetwork.tools._utils import open_listener_sockets_from_getaddrinfo_result
+from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
+
+from ._utils import _ensure_resolved, create_connection, create_datagram_socket
+from .datagram.endpoint import create_datagram_endpoint
+from .datagram.socket import AsyncioTransportDatagramSocketAdapter, RawDatagramSocketAdapter
+from .stream.listener import AcceptedSocket, AcceptedSSLSocket, ListenerSocketAdapter
+from .stream.socket import AsyncioTransportStreamSocketAdapter, RawStreamSocketAdapter
+from .tasks import TaskGroup, timeout, timeout_at
+from .threads import ThreadsPortal
 
 if TYPE_CHECKING:
     import concurrent.futures
-    import ssl as _ssl
+    from ssl import SSLContext as _SSLContext
+
+    from easynetwork.api_async.backend.abc import AbstractAcceptedSocket, ILock
 
-    from easynetwork.api_async.backend.abc import (
-        AbstractAcceptedSocket,
-        AbstractAsyncDatagramSocketAdapter,
-        AbstractAsyncListenerSocketAdapter,
-        AbstractAsyncStreamSocketAdapter,
-        AbstractTaskGroup,
-        AbstractThreadsPortal,
-        AbstractTimeoutHandle,
-        ICondition,
-        IEvent,
-        ILock,
-    )
+    from .tasks import TimeoutHandle
 
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 
 
 class AsyncioBackend(AbstractAsyncBackend):
@@ -84,22 +97,18 @@
         asyncio._unregister_task(task)
 
         try:
             return await self._cancel_shielded_wait_asyncio_future(task)
         finally:
             del task
 
-    def timeout(self, delay: float) -> AsyncContextManager[AbstractTimeoutHandle]:
-        from .tasks import timeout
-
+    def timeout(self, delay: float) -> AsyncContextManager[TimeoutHandle]:
         return timeout(delay)
 
-    def timeout_at(self, deadline: float) -> AsyncContextManager[AbstractTimeoutHandle]:
-        from .tasks import timeout_at
-
+    def timeout_at(self, deadline: float) -> AsyncContextManager[TimeoutHandle]:
         return timeout_at(deadline)
 
     @classmethod
     async def _cancel_shielded_wait_asyncio_future(cls, future: asyncio.Future[_T_co]) -> _T_co:
         current_task: asyncio.Task[Any] = cls._current_asyncio_task()
         cancelling: int = current_task.cancelling()
 
@@ -123,45 +132,37 @@
         await asyncio.sleep(delay)
 
     async def sleep_forever(self) -> NoReturn:
         loop = asyncio.get_running_loop()
         await loop.create_future()
         raise AssertionError("await an unused future cannot end in any other way than by cancellation")
 
-    def create_task_group(self) -> AbstractTaskGroup:
-        from .tasks import TaskGroup
-
+    def create_task_group(self) -> TaskGroup:
         return TaskGroup()
 
     async def create_tcp_connection(
         self,
         host: str,
         port: int,
         *,
         local_address: tuple[str, int] | None = None,
         happy_eyeballs_delay: float | None = None,
-    ) -> AbstractAsyncStreamSocketAdapter:
+    ) -> AsyncioTransportStreamSocketAdapter | RawStreamSocketAdapter:
         assert host is not None, "Expected 'host' to be a str"
         assert port is not None, "Expected 'port' to be an int"
 
         if happy_eyeballs_delay is not None:
             self._check_asyncio_transport("'happy_eyeballs_delay' option")
 
         if not self.__use_asyncio_transport:
-            from ._utils import create_connection
-            from .stream.socket import RawStreamSocketAdapter
-
             loop = asyncio.get_running_loop()
-
             socket = await create_connection(host, port, loop, local_address=local_address)
             return RawStreamSocketAdapter(socket, loop)
 
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .stream.socket import AsyncioTransportStreamSocketAdapter
+        happy_eyeballs_delay = self._default_happy_eyeballs_delay(happy_eyeballs_delay)
 
         if happy_eyeballs_delay is None:
             reader, writer = await asyncio.open_connection(
                 host,
                 port,
                 local_addr=local_address,
                 limit=MAX_STREAM_BUFSIZE,
@@ -176,28 +177,26 @@
             )
         return AsyncioTransportStreamSocketAdapter(reader, writer)
 
     async def create_ssl_over_tcp_connection(
         self,
         host: str,
         port: int,
-        ssl_context: _ssl.SSLContext,
+        ssl_context: _SSLContext,
         *,
         server_hostname: str | None,
         ssl_handshake_timeout: float,
         ssl_shutdown_timeout: float,
         local_address: tuple[str, int] | None = None,
         happy_eyeballs_delay: float | None = None,
-    ) -> AbstractAsyncStreamSocketAdapter:
+    ) -> AsyncioTransportStreamSocketAdapter:
         self._check_ssl_support()
         self.__verify_ssl_context(ssl_context)
 
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .stream.socket import AsyncioTransportStreamSocketAdapter
+        happy_eyeballs_delay = self._default_happy_eyeballs_delay(happy_eyeballs_delay)
 
         if happy_eyeballs_delay is None:
             reader, writer = await asyncio.open_connection(
                 host,
                 port,
                 ssl=ssl_context,
                 server_hostname=server_hostname,
@@ -216,49 +215,50 @@
                 ssl_shutdown_timeout=float(ssl_shutdown_timeout),
                 local_addr=local_address,
                 happy_eyeballs_delay=happy_eyeballs_delay,
                 limit=MAX_STREAM_BUFSIZE,
             )
         return AsyncioTransportStreamSocketAdapter(reader, writer)
 
-    async def wrap_tcp_client_socket(self, socket: _socket.socket) -> AbstractAsyncStreamSocketAdapter:
+    @staticmethod
+    def _default_happy_eyeballs_delay(happy_eyeballs_delay: float | None) -> float | None:
+        if happy_eyeballs_delay is None:
+            running_loop = asyncio.get_running_loop()
+            if isinstance(running_loop, asyncio.base_events.BaseEventLoop):  # Base class of standard implementation
+                happy_eyeballs_delay = 0.25  # Recommended value by the RFC 6555
+        return happy_eyeballs_delay
+
+    async def wrap_tcp_client_socket(
+        self,
+        socket: _socket.socket,
+    ) -> AsyncioTransportStreamSocketAdapter | RawStreamSocketAdapter:
         assert socket is not None, "Expected 'socket' to be a socket.socket instance"
         socket.setblocking(False)
 
         if not self.__use_asyncio_transport:
-            from .stream.socket import RawStreamSocketAdapter
-
             return RawStreamSocketAdapter(socket, asyncio.get_running_loop())
 
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .stream.socket import AsyncioTransportStreamSocketAdapter
-
         reader, writer = await asyncio.open_connection(sock=socket, limit=MAX_STREAM_BUFSIZE)
         return AsyncioTransportStreamSocketAdapter(reader, writer)
 
     async def wrap_ssl_over_tcp_client_socket(
         self,
         socket: _socket.socket,
-        ssl_context: _ssl.SSLContext,
+        ssl_context: _SSLContext,
         *,
         server_hostname: str,
         ssl_handshake_timeout: float,
         ssl_shutdown_timeout: float,
-    ) -> AbstractAsyncStreamSocketAdapter:
+    ) -> AsyncioTransportStreamSocketAdapter:
         self._check_ssl_support()
         self.__verify_ssl_context(ssl_context)
 
         assert socket is not None, "Expected 'socket' to be a socket.socket instance"
         socket.setblocking(False)
 
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .stream.socket import AsyncioTransportStreamSocketAdapter
-
         reader, writer = await asyncio.open_connection(
             sock=socket,
             ssl=ssl_context,
             server_hostname=server_hostname,
             ssl_handshake_timeout=float(ssl_handshake_timeout),
             ssl_shutdown_timeout=float(ssl_shutdown_timeout),
             limit=MAX_STREAM_BUFSIZE,
@@ -268,41 +268,37 @@
     async def create_tcp_listeners(
         self,
         host: str | Sequence[str] | None,
         port: int,
         backlog: int,
         *,
         reuse_port: bool = False,
-    ) -> Sequence[AbstractAsyncListenerSocketAdapter]:
-        from .stream.listener import AcceptedSocket
-
+    ) -> Sequence[ListenerSocketAdapter]:
         return await self._create_tcp_listeners(
             host,
             port,
             backlog,
             functools.partial(AcceptedSocket, use_asyncio_transport=self.__use_asyncio_transport),
             reuse_port=reuse_port,
         )
 
     async def create_ssl_over_tcp_listeners(
         self,
         host: str | Sequence[str] | None,
         port: int,
         backlog: int,
-        ssl_context: _ssl.SSLContext,
+        ssl_context: _SSLContext,
         ssl_handshake_timeout: float,
         ssl_shutdown_timeout: float,
         *,
         reuse_port: bool = False,
-    ) -> Sequence[AbstractAsyncListenerSocketAdapter]:
+    ) -> Sequence[ListenerSocketAdapter]:
         self._check_ssl_support()
         self.__verify_ssl_context(ssl_context)
 
-        from .stream.listener import AcceptedSSLSocket
-
         return await self._create_tcp_listeners(
             host,
             port,
             backlog,
             functools.partial(
                 AcceptedSSLSocket,
                 ssl_context=ssl_context,
@@ -316,38 +312,30 @@
         self,
         host: str | Sequence[str] | None,
         port: int,
         backlog: int,
         accepted_socket_factory: Callable[[_socket.socket, asyncio.AbstractEventLoop], AbstractAcceptedSocket],
         *,
         reuse_port: bool,
-    ) -> Sequence[AbstractAsyncListenerSocketAdapter]:
+    ) -> Sequence[ListenerSocketAdapter]:
         assert port is not None, "Expected 'port' to be an int"
 
-        import os
-        import sys
-        from itertools import chain
-
-        from easynetwork.tools._utils import open_listener_sockets_from_getaddrinfo_result
-
-        from ._utils import _ensure_resolved
-
         loop = asyncio.get_running_loop()
 
         reuse_address: bool = os.name not in ("nt", "cygwin") and sys.platform != "cygwin"
         hosts: Sequence[str | None]
         if host == "" or host is None:
             hosts = [None]
         elif isinstance(host, str):
             hosts = [host]
         else:
             hosts = host
 
         infos: set[tuple[int, int, int, str, tuple[Any, ...]]] = set(
-            chain.from_iterable(
+            itertools.chain.from_iterable(
                 await asyncio.gather(
                     *[
                         _ensure_resolved(host, port, _socket.AF_UNSPEC, _socket.SOCK_STREAM, loop, flags=_socket.AI_PASSIVE)
                         for host in hosts
                     ]
                 )
             )
@@ -356,58 +344,49 @@
         sockets: list[_socket.socket] = open_listener_sockets_from_getaddrinfo_result(
             infos,
             backlog=backlog,
             reuse_address=reuse_address,
             reuse_port=reuse_port,
         )
 
-        from .stream.listener import ListenerSocketAdapter
-
         return [ListenerSocketAdapter(sock, loop, accepted_socket_factory) for sock in sockets]
 
     async def create_udp_endpoint(
         self,
         *,
         local_address: tuple[str | None, int] | None = None,
         remote_address: tuple[str, int] | None = None,
         reuse_port: bool = False,
-    ) -> AbstractAsyncDatagramSocketAdapter:
-        from ._utils import create_datagram_socket
-
+    ) -> AsyncioTransportDatagramSocketAdapter | RawDatagramSocketAdapter:
         socket = await create_datagram_socket(
             loop=asyncio.get_running_loop(),
             local_address=local_address,
             remote_address=remote_address,
             reuse_port=reuse_port,
         )
 
         return await self.wrap_udp_socket(socket)
 
-    async def wrap_udp_socket(self, socket: _socket.socket) -> AbstractAsyncDatagramSocketAdapter:
+    async def wrap_udp_socket(self, socket: _socket.socket) -> AsyncioTransportDatagramSocketAdapter | RawDatagramSocketAdapter:
         assert socket is not None, "Expected 'socket' to be a socket.socket instance"
         socket.setblocking(False)
 
         if not self.__use_asyncio_transport:
-            from .datagram.socket import RawDatagramSocketAdapter
-
             return RawDatagramSocketAdapter(socket, asyncio.get_running_loop())
 
-        from .datagram.endpoint import create_datagram_endpoint
-        from .datagram.socket import AsyncioTransportDatagramSocketAdapter
-
         endpoint = await create_datagram_endpoint(socket=socket)
         return AsyncioTransportDatagramSocketAdapter(endpoint)
 
-    def create_lock(self) -> ILock:
+    def create_lock(self) -> asyncio.Lock:
         return asyncio.Lock()
 
-    def create_event(self) -> IEvent:
+    def create_event(self) -> asyncio.Event:
         return asyncio.Event()
 
-    def create_condition_var(self, lock: ILock | None = None) -> ICondition:
+    def create_condition_var(self, lock: ILock | None = None) -> asyncio.Condition:
         if lock is not None:
             assert isinstance(lock, asyncio.Lock)
 
         return asyncio.Condition(lock)
 
     async def run_in_thread(self, __func: Callable[_P, _T], /, *args: _P.args, **kwargs: _P.kwargs) -> _T:
         loop = asyncio.get_running_loop()
@@ -420,17 +399,15 @@
         future = loop.run_in_executor(None, func_call)
         del func_call, __func, args, kwargs
         try:
             return await self._cancel_shielded_wait_asyncio_future(future)
         finally:
             del future
 
-    def create_threads_portal(self) -> AbstractThreadsPortal:
-        from .threads import ThreadsPortal
-
+    def create_threads_portal(self) -> ThreadsPortal:
         return ThreadsPortal()
 
     async def wait_future(self, future: concurrent.futures.Future[_T_co]) -> _T_co:
         try:
             if future.done():
                 await self.cancel_shielded_coro_yield()
                 return future.result()
@@ -470,12 +447,12 @@
         transport = self.__use_asyncio_transport
         if not transport:
             raise ValueError(f"{context} not supported with {transport=}")
 
     def _check_ssl_support(self) -> None:
         self._check_asyncio_transport("SSL/TLS")
 
-    def __verify_ssl_context(self, ctx: _ssl.SSLContext) -> None:
-        import ssl
-
+    def __verify_ssl_context(self, ctx: _SSLContext) -> None:
+        if ssl is None:
+            raise RuntimeError("stdlib ssl module not available")
         if not isinstance(ctx, ssl.SSLContext):
             raise ValueError(f"Expected a ssl.SSLContext instance, got {ctx!r}")
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/socket.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/tasks.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/threads.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,18 @@
         self.__loop.call_soon_threadsafe(callback, future, context=ctx)
         return future
 
     @staticmethod
     def __get_result(future: concurrent.futures.Future[_T]) -> _T:
         try:
             return future.result()
-        except concurrent.futures.CancelledError as exc:
+        except concurrent.futures.CancelledError:
             if not future.cancelled():  # raised from future.exception()
                 raise
-            raise asyncio.CancelledError() from exc
+            raise asyncio.CancelledError() from None
         finally:
             del future
 
     def __check_running_loop(self) -> None:
         try:
             running_loop = asyncio.get_running_loop()
         except RuntimeError:
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/datagram/endpoint.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/datagram/endpoint.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/datagram/socket.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/datagram/socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["AsyncioTransportDatagramSocketAdapter", "RawDatagramSocketAdapter"]
 
 import asyncio
+import socket as _socket
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.api_async.backend.abc import AbstractAsyncDatagramSocketAdapter
+from easynetwork.tools.socket import MAX_DATAGRAM_BUFSIZE
+
+from ..socket import AsyncSocket
 
 if TYPE_CHECKING:
     import asyncio.trsock
-    import socket as _socket
 
     from _typeshed import ReadableBuffer
 
     from .endpoint import DatagramEndpoint
 
 
 @final
@@ -75,21 +78,17 @@
     def __init__(
         self,
         socket: _socket.socket,
         loop: asyncio.AbstractEventLoop,
     ) -> None:
         super().__init__()
 
-        from socket import SOCK_DGRAM
-
-        from ..socket import AsyncSocket
-
         self.__socket: AsyncSocket = AsyncSocket(socket, loop)
 
-        assert socket.type == SOCK_DGRAM, "A 'SOCK_DGRAM' socket is expected"
+        assert socket.type == _socket.SOCK_DGRAM, "A 'SOCK_DGRAM' socket is expected"
 
     async def aclose(self) -> None:
         return await self.__socket.aclose()
 
     def is_closing(self) -> bool:
         return self.__socket.is_closing()
 
@@ -99,16 +98,14 @@
     def get_remote_address(self) -> tuple[Any, ...] | None:
         try:
             return self.__socket.socket.getpeername()
         except OSError:
             return None
 
     async def recvfrom(self) -> tuple[bytes, tuple[Any, ...]]:
-        from easynetwork.tools.socket import MAX_DATAGRAM_BUFSIZE
-
         return await self.__socket.recvfrom(MAX_DATAGRAM_BUFSIZE)
 
     async def sendto(self, data: ReadableBuffer, address: tuple[Any, ...] | None, /) -> None:
         if address is None:
             await self.__socket.sendall(data)
         else:
             await self.__socket.sendto(data, address)
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/stream/listener.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/stream/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from typing import TYPE_CHECKING, Any, Callable, final
 
 from easynetwork.api_async.backend.abc import (
     AbstractAcceptedSocket,
     AbstractAsyncListenerSocketAdapter,
     AbstractAsyncStreamSocketAdapter,
 )
+from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
+
+from ..socket import AsyncSocket
+from .socket import AsyncioTransportStreamSocketAdapter, RawStreamSocketAdapter
 
 if TYPE_CHECKING:
     import asyncio.trsock
     import socket as _socket
     import ssl as _ssl
 
 
@@ -34,16 +38,14 @@
         self,
         socket: _socket.socket,
         loop: asyncio.AbstractEventLoop,
         accepted_socket_factory: Callable[[_socket.socket, asyncio.AbstractEventLoop], AbstractAcceptedSocket],
     ) -> None:
         super().__init__()
 
-        from ..socket import AsyncSocket
-
         self.__socket: AsyncSocket = AsyncSocket(socket, loop)
         self.__accepted_socket_factory = accepted_socket_factory
 
     def is_closing(self) -> bool:
         return self.__socket.is_closing()
 
     async def aclose(self) -> None:
@@ -103,22 +105,16 @@
         super().__init__(socket, loop)
 
         self.__use_asyncio_transport: bool = bool(use_asyncio_transport)
 
     async def _make_socket_adapter(self, socket: _socket.socket) -> AbstractAsyncStreamSocketAdapter:
         loop = self.loop
         if not self.__use_asyncio_transport:
-            from .socket import RawStreamSocketAdapter
-
             return RawStreamSocketAdapter(socket, loop)
 
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .socket import AsyncioTransportStreamSocketAdapter
-
         reader = asyncio.streams.StreamReader(MAX_STREAM_BUFSIZE, loop)
         protocol = asyncio.streams.StreamReaderProtocol(reader, loop=loop)
         transport, _ = await loop.connect_accepted_socket(lambda: protocol, socket)
         writer = asyncio.streams.StreamWriter(transport, protocol, reader, loop)
         return AsyncioTransportStreamSocketAdapter(reader, writer)
 
 
@@ -140,18 +136,14 @@
         assert ssl_context is not None
 
         self.__ssl_context: _ssl.SSLContext = ssl_context
         self.__ssl_handshake_timeout: float = float(ssl_handshake_timeout)
         self.__ssl_shutdown_timeout: float = float(ssl_shutdown_timeout)
 
     async def _make_socket_adapter(self, socket: _socket.socket) -> AbstractAsyncStreamSocketAdapter:
-        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
-
-        from .socket import AsyncioTransportStreamSocketAdapter
-
         loop = self.loop
         reader = asyncio.streams.StreamReader(MAX_STREAM_BUFSIZE, loop)
         protocol = asyncio.streams.StreamReaderProtocol(reader, loop=loop)
         transport, _ = await loop.connect_accepted_socket(
             lambda: protocol,
             socket,
             ssl=self.__ssl_context,
```

### Comparing `easynetwork-1.0.0rc3/src/easynetwork_asyncio/stream/socket.py` & `easynetwork-1.0.0rc4/src/easynetwork_asyncio/stream/socket.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["AsyncioTransportStreamSocketAdapter", "RawStreamSocketAdapter"]
 
 import asyncio
+import errno
+import socket as _socket
 from typing import TYPE_CHECKING, Any, final
 
 from easynetwork.api_async.backend.abc import AbstractAsyncStreamSocketAdapter
 from easynetwork.tools._utils import error_from_errno as _error_from_errno
 
+from ..socket import AsyncSocket
+
 if TYPE_CHECKING:
     import asyncio.trsock
-    import socket as _socket
 
     from _typeshed import ReadableBuffer
 
 
 @final
 class AsyncioTransportStreamSocketAdapter(AbstractAsyncStreamSocketAdapter):
     __slots__ = (
@@ -39,16 +42,14 @@
         self.__reader: asyncio.StreamReader = reader
         self.__writer: asyncio.StreamWriter = writer
 
         socket: asyncio.trsock.TransportSocket | None = writer.get_extra_info("socket")
         assert socket is not None, "Writer transport must be a socket transport"
         remote_address = writer.get_extra_info("peername")
         if remote_address is None:
-            import errno
-
             raise _error_from_errno(errno.ENOTCONN)
         self.__remote_addr: tuple[Any, ...] = tuple(remote_address)
 
     async def aclose(self) -> None:
         try:
             if not self.__writer.is_closing():
                 self.__writer.close()
@@ -98,21 +99,17 @@
     def __init__(
         self,
         socket: _socket.socket,
         loop: asyncio.AbstractEventLoop,
     ) -> None:
         super().__init__()
 
-        from socket import SOCK_STREAM
-
-        from ..socket import AsyncSocket
-
         self.__socket: AsyncSocket = AsyncSocket(socket, loop)
 
-        assert socket.type == SOCK_STREAM, "A 'SOCK_STREAM' socket is expected"
+        assert socket.type == _socket.SOCK_STREAM, "A 'SOCK_STREAM' socket is expected"
 
         remote_address = socket.getpeername()
         self.__remote_addr: tuple[Any, ...] = tuple(remote_address)
 
     async def aclose(self) -> None:
         return await self.__socket.aclose()
```

### Comparing `easynetwork-1.0.0rc3/tests/conftest.py` & `easynetwork-1.0.0rc4/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 PYTEST_PLUGINS_PACKAGE = f"{__package__}.pytest_plugins"
 
 
 pytest_plugins = [
     f"{PYTEST_PLUGINS_PACKAGE}.asyncio_event_loop",
     f"{PYTEST_PLUGINS_PACKAGE}.extra_features",
     f"{PYTEST_PLUGINS_PACKAGE}.session_exit_code",
+    f"{PYTEST_PLUGINS_PACKAGE}.ssl_module",
 ]
```

### Comparing `easynetwork-1.0.0rc3/tests/tools.py` & `easynetwork-1.0.0rc4/tests/tools.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_asyncio_backend.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_asyncio_backend.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_backend_factory.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_backend_factory.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_futures.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_futures.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_async/test_backend/test_tasks.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_async/test_backend/test_tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,24 @@
         assert runner.cancel()
         assert runner.cancel()  # Cancel twice does nothing
 
         with pytest.raises(asyncio.CancelledError):
             await runner.run()
 
         assert task.cancelled()
+
+    async def test____run____unhandled_exceptions(
+        self,
+        backend: AbstractAsyncBackend,
+        mocker: MockerFixture,
+    ) -> None:
+        my_exc = OSError()
+        coro_func = mocker.AsyncMock(spec=lambda *args, **kwargs: None, side_effect=[my_exc])
+        runner: SingleTaskRunner[Any] = SingleTaskRunner(backend, coro_func)
+
+        with pytest.raises(OSError) as exc_info_run_1:
+            _ = await runner.run()
+        with pytest.raises(OSError) as exc_info_run_2:
+            _ = await runner.run()
+
+        assert exc_info_run_1.value is my_exc
+        assert exc_info_run_2.value is my_exc
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/conftest.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/serializer.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/serializer.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/conftest.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_client/test_tcp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_client/test_tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from easynetwork.tools.socket import IPv4SocketAddress, IPv6SocketAddress, SocketProxy
 
 import pytest
 import pytest_asyncio
 
 
 @pytest.mark.asyncio
+@pytest.mark.usefixtures("simulate_no_ssl_module")
 class TestAsyncTCPNetworkClient:
     @pytest.fixture
     @staticmethod
     def server(socket_pair: tuple[Socket, Socket]) -> Socket:
         server = socket_pair[0]
         server.setsockopt(IPPROTO_TCP, TCP_NODELAY, 1)
         server.setblocking(False)
@@ -201,14 +202,15 @@
             assert isinstance(address, IPv4SocketAddress)
         else:
             assert isinstance(address, IPv6SocketAddress)
         assert address == client.socket.getpeername()
 
 
 @pytest.mark.asyncio
+@pytest.mark.usefixtures("simulate_no_ssl_module")
 class TestAsyncTCPNetworkClientConnection:
     @pytest_asyncio.fixture(autouse=True)
     @staticmethod
     async def server(localhost_ip: str, socket_family: int) -> AsyncIterator[asyncio.Server]:
         async def client_connected_cb(reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
             try:
                 data: bytes = await reader.readline()
@@ -521,7 +523,27 @@
             ssl=True,
             server_hostname="",
             backend_kwargs=backend_kwargs,
         ) as client:
             assert not client_ssl_context.check_hostname  # It must be set to False if server_hostname is an empty string
             await client.send_packet("Test")
             assert await client.recv_packet() == "Test"
+
+    @pytest.mark.usefixtures("simulate_no_ssl_module")
+    async def test____dunder_init____no_ssl_module_available(
+        self,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+        backend_kwargs: dict[str, Any],
+        client_ssl_context: ssl.SSLContext,
+    ) -> None:
+        # Arrange
+
+        # Act & Assert
+        with pytest.raises(RuntimeError, match=r"^stdlib ssl module not available$"):
+            _ = AsyncTCPNetworkClient(
+                remote_address,
+                stream_protocol,
+                ssl=client_ssl_context,
+                server_hostname="test.example.com",
+                backend_kwargs=backend_kwargs,
+            )
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_client/test_udp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_client/test_udp.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/base.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_standalone.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_standalone.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,21 +33,23 @@
     @staticmethod
     def start_server(server: AbstractStandaloneNetworkServer) -> Iterator[None]:
         with server:
             is_up_event = threading.Event()
             t = threading.Thread(target=server.serve_forever, kwargs={"is_up_event": is_up_event}, daemon=True)
             t.start()
 
-            is_up_event.wait(timeout=1)
+            if not is_up_event.wait(timeout=1):
+                raise TimeoutError("Too long to start")
             assert server.is_serving()
 
             yield
 
             server.shutdown()
             assert not server.is_serving()
+            t.join()
 
     def test____is_serving____default_to_False(self, server: AbstractStandaloneNetworkServer) -> None:
         with server:
             assert not server.is_serving()
 
     def test____shutdown____default_to_noop(self, server: AbstractStandaloneNetworkServer) -> None:
         with server:
@@ -60,14 +62,15 @@
 
             time.sleep(1)
             if not server.is_serving():
                 pytest.fail("Timeout error")
 
             server.shutdown()
             assert not server.is_serving()
+            t.join()
 
     @pytest.mark.usefixtures("start_server")
     def test____server_close____while_server_is_running(self, server: AbstractStandaloneNetworkServer) -> None:
         server.server_close()
 
     @pytest.mark.usefixtures("start_server")
     def test____serve_forever____error_server_already_running(self, server: AbstractStandaloneNetworkServer) -> None:
@@ -92,28 +95,33 @@
         runner_factory: Callable[[], asyncio.Runner] | None,
     ) -> StandaloneTCPNetworkServer[str, str]:
         return StandaloneTCPNetworkServer(
             None,
             0,
             stream_protocol,
             EchoRequestHandler(),
-            backend="asyncio",
             backend_kwargs={"runner_factory": runner_factory},
         )
 
     def test____stop_listening____default_to_noop(self, server: StandaloneTCPNetworkServer[str, str]) -> None:
         with server:
+            assert not server.sockets
+            assert not server.get_addresses()
             server.stop_listening()
 
     @pytest.mark.usefixtures("start_server")
     def test____stop_listening____stop_accepting_new_connection(self, server: StandaloneTCPNetworkServer[str, str]) -> None:
         assert server.is_serving()
+        assert len(server.sockets) > 0
+        assert len(server.get_addresses()) > 0
 
         server.stop_listening()
         assert not server.is_serving()
+        assert len(server.sockets) > 0  # Sockets are closed, but always available until server_close() call
+        assert len(server.get_addresses()) == 0
 
 
 class TestStandaloneUDPNetworkServer(BaseTestStandaloneNetworkServer):
     @pytest.fixture(params=[None, custom_asyncio_runner])
     @staticmethod
     def runner_factory(request: pytest.FixtureRequest) -> Callable[[], asyncio.Runner] | None:
         return getattr(request, "param", None)
@@ -125,10 +133,19 @@
         runner_factory: Callable[[], asyncio.Runner] | None,
     ) -> StandaloneUDPNetworkServer[str, str]:
         return StandaloneUDPNetworkServer(
             None,
             0,
             datagram_protocol,
             EchoRequestHandler(),
-            backend="asyncio",
             backend_kwargs={"runner_factory": runner_factory},
         )
+
+    def test____socket_property____server_is_not_running(self, server: StandaloneUDPNetworkServer[str, str]) -> None:
+        with server:
+            assert server.socket is None
+            assert server.get_address() is None
+
+    @pytest.mark.usefixtures("start_server")
+    def test____socket_property____server_is_running(self, server: StandaloneUDPNetworkServer[str, str]) -> None:
+        assert server.socket is not None
+        assert server.get_address() is not None
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_tcp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import asyncio
 import collections
 import contextlib
 import logging
 import math
 import ssl
-import ssl as _ssl
 from socket import IPPROTO_TCP, TCP_NODELAY
 from typing import Any, AsyncGenerator, AsyncIterator, Awaitable, Callable, Sequence
 from weakref import WeakValueDictionary
 
-from easynetwork.api_async.backend.abc import AbstractAsyncBackend, AbstractAsyncListenerSocketAdapter
+from easynetwork.api_async.backend.abc import AbstractAsyncBackend
 from easynetwork.api_async.server.handler import AsyncBaseRequestHandler, AsyncClientInterface, AsyncStreamRequestHandler
 from easynetwork.api_async.server.tcp import AsyncTCPNetworkServer
 from easynetwork.exceptions import BaseProtocolParseError, ClientClosedError, StreamProtocolParseError
 from easynetwork.protocol import StreamProtocol
 from easynetwork.tools.socket import SocketAddress
 from easynetwork_asyncio._utils import create_connection
 from easynetwork_asyncio.backend import AsyncioBackend
+from easynetwork_asyncio.stream.listener import ListenerSocketAdapter
 
 import pytest
 import pytest_asyncio
 
 from .base import BaseTestAsyncServer
 
 
@@ -33,29 +33,29 @@
         self,
         host: str | Sequence[str] | None,
         port: int,
         backlog: int,
         *,
         family: int = 0,
         reuse_port: bool = False,
-    ) -> Sequence[AbstractAsyncListenerSocketAdapter]:
+    ) -> Sequence[ListenerSocketAdapter]:
         return []
 
     async def create_ssl_over_tcp_listeners(
         self,
         host: str | Sequence[str] | None,
         port: int,
         backlog: int,
-        ssl_context: _ssl.SSLContext,
+        ssl_context: ssl.SSLContext,
         ssl_handshake_timeout: float,
         ssl_shutdown_timeout: float,
         *,
         family: int = 0,
         reuse_port: bool = False,
-    ) -> Sequence[AbstractAsyncListenerSocketAdapter]:
+    ) -> Sequence[ListenerSocketAdapter]:
         return []
 
 
 class RandomError(Exception):
     pass
 
 
@@ -293,23 +293,26 @@
             backlog=1,
             ssl=server_ssl_context if use_ssl else None,
             ssl_handshake_timeout=ssl_handshake_timeout,
             service_actions_interval=service_actions_interval,
             backend_kwargs=backend_kwargs,
         ) as server:
             assert not server.sockets
+            assert not server.get_addresses()
             yield server
 
     @pytest_asyncio.fixture
     @staticmethod
     async def server_address(run_server: asyncio.Event, server: MyAsyncTCPServer) -> tuple[str, int]:
         async with asyncio.timeout(1):
             await run_server.wait()
         assert server.is_serving()
-        return server.sockets[0].getsockname()[:2]
+        server_addresses = server.get_addresses()
+        assert len(server_addresses) == 1
+        return server_addresses[0].for_connection()
 
     @pytest.fixture
     @staticmethod
     def run_server_and_wait(run_server: None, server_address: Any) -> None:
         pass
 
     @pytest_asyncio.fixture
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_async/test_server/test_udp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_async/test_server/test_udp.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,24 +182,27 @@
             0,
             datagram_protocol,
             request_handler,
             service_actions_interval=service_actions_interval,
             backend_kwargs=backend_kwargs,
         ) as server:
             assert server.socket is None
+            assert server.get_address() is None
             yield server
 
     @pytest_asyncio.fixture
     @staticmethod
     async def server_address(run_server: asyncio.Event, server: MyAsyncUDPServer) -> tuple[str, int]:
         async with asyncio.timeout(1):
             await run_server.wait()
         assert server.is_serving()
         assert server.socket is not None
-        return server.socket.getsockname()[:2]
+        server_address = server.get_address()
+        assert server_address is not None
+        return server_address.for_connection()
 
     @pytest.fixture
     @staticmethod
     def run_server_and_wait(run_server: None, server_address: Any) -> None:
         pass
 
     @pytest_asyncio.fixture
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/conftest.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/test_client/test_tcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from easynetwork.tools.socket import IPv4SocketAddress, IPv6SocketAddress
 
 import pytest
 
 from .....tools import TimeTest
 
 
+@pytest.mark.usefixtures("simulate_no_ssl_module")
 class TestTCPNetworkClient:
     @pytest.fixture
     @staticmethod
     def server(socket_pair: tuple[Socket, Socket]) -> Socket:
         server = socket_pair[0]
         server.setsockopt(IPPROTO_TCP, TCP_NODELAY, 1)
         return server
@@ -220,22 +221,23 @@
 
         if self.ssl_context:
             socket = self.ssl_context.wrap_socket(socket, server_side=True, do_handshake_on_connect=True)
 
         return socket, client_address
 
 
+@pytest.mark.usefixtures("simulate_no_ssl_module")
 class TestTCPNetworkClientConnection:
     @pytest.fixture(autouse=True)
     @classmethod
     def server(cls, localhost_ip: str, socket_family: int) -> Iterator[socketserver.TCPServer]:
         from threading import Thread
 
         with TCPServer((localhost_ip, 0), socket_family) as server:
-            server_thread = Thread(target=server.serve_forever)
+            server_thread = Thread(target=server.serve_forever, daemon=True)
             server_thread.start()
             yield server
             server.shutdown()
             server_thread.join()
 
     @pytest.fixture
     @staticmethod
@@ -264,15 +266,15 @@
         localhost_ip: str,
         socket_family: int,
         server_ssl_context: ssl.SSLContext,
     ) -> Iterator[socketserver.TCPServer]:
         from threading import Thread
 
         with TCPServer((localhost_ip, 0), socket_family, ssl_context=server_ssl_context) as server:
-            server_thread = Thread(target=server.serve_forever)
+            server_thread = Thread(target=server.serve_forever, daemon=True)
             server_thread.start()
             yield server
             server.shutdown()
             server_thread.join()
 
     @pytest.fixture
     @staticmethod
@@ -335,7 +337,25 @@
             stream_protocol,
             ssl=True,
             server_hostname="",
         ) as client:
             assert not client_ssl_context.check_hostname  # It must be set to False if server_hostname is an empty string
             client.send_packet("Test")
             assert client.recv_packet() == "Test"
+
+    @pytest.mark.usefixtures("simulate_no_ssl_module")
+    def test____dunder_init____no_ssl_module(
+        self,
+        remote_address: tuple[str, int],
+        stream_protocol: StreamProtocol[str, str],
+        client_ssl_context: ssl.SSLContext,
+    ) -> None:
+        # Arrange
+
+        # Act & Assert
+        with pytest.raises(RuntimeError, match=r"^stdlib ssl module not available$"):
+            _ = TCPNetworkClient(
+                remote_address,
+                stream_protocol,
+                ssl=client_ssl_context,
+                server_hostname="test.example.com",
+            )
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_communication/test_sync/test_client/test_udp.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_communication/test_sync/test_client/test_udp.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/base.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import random
 from abc import ABCMeta
 from typing import Any, Callable, final
 
 from easynetwork.exceptions import DeserializeError, IncrementalDeserializeError
 from easynetwork.serializers.abc import AbstractIncrementalPacketSerializer, AbstractPacketSerializer
+from easynetwork.tools._utils import iter_bytes
 
 import pytest
 
 from ...tools import send_return
 
 
 class BaseTestSerializer(metaclass=ABCMeta):
@@ -188,31 +189,24 @@
         self,
         serializer_for_deserialization: AbstractIncrementalPacketSerializer[Any, Any],
         empty_bytes_before: bool,
         complete_data_for_incremental_deserialize: bytes,
         packet_to_serialize: Any,
     ) -> None:
         # Arrange
-        import struct
-
-        chunks_list: list[bytes] = list(
-            struct.unpack(f"{len(complete_data_for_incremental_deserialize)}c", complete_data_for_incremental_deserialize)
-        )
-        assert all(len(b) == 1 for b in chunks_list) and b"".join(chunks_list) == complete_data_for_incremental_deserialize
-
-        del complete_data_for_incremental_deserialize, struct
 
         consumer = serializer_for_deserialization.incremental_deserialize()
         next(consumer)
 
         # Act
         with pytest.raises(StopIteration) as exc_info:
             # The generator can stop at any moment (no need to go to the last byte)
             # However, the remaining data returned should be empty
-            for chunk in chunks_list:
+            for chunk in iter_bytes(complete_data_for_incremental_deserialize):
+                assert len(chunk) == 1
                 if empty_bytes_before:
                     try:
                         consumer.send(b"")
                     except StopIteration:
                         raise RuntimeError("consumer stopped when sending empty bytes")
                 consumer.send(chunk)
```

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_base64.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_cbor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_compressors.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_compressors.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_encryptor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_line.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_line.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_msgpack.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_namedtuple.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_namedtuple.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/test_pickle.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/test_pickle.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/samples/json.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/samples/json.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/functional_test/test_serializers/samples/pickle.py` & `easynetwork-1.0.0rc4/tests/functional_test/test_serializers/samples/pickle.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/other_test/test_import.py` & `easynetwork-1.0.0rc4/tests/other_test/test_import.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/other_test/test_project_metadata.py` & `easynetwork-1.0.0rc4/tests/other_test/test_project_metadata.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/pytest_plugins/asyncio_event_loop.py` & `easynetwork-1.0.0rc4/tests/pytest_plugins/asyncio_event_loop.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/pytest_plugins/extra_features.py` & `easynetwork-1.0.0rc4/tests/pytest_plugins/extra_features.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/pytest_plugins/session_exit_code.py` & `easynetwork-1.0.0rc4/tests/pytest_plugins/session_exit_code.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/scripts/async_server_test.py` & `easynetwork-1.0.0rc4/tests/scripts/async_server_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
         await client.send_packet(request.upper())
 
     async def bad_request(self, client: AsyncClientInterface[str], exc: BaseProtocolParseError) -> None:
         pass
 
 
 def create_tcp_server() -> StandaloneTCPNetworkServer[str, str]:
-    return StandaloneTCPNetworkServer(None, PORT, StreamProtocol(StringLineSerializer()), MyAsyncRequestHandler(), "asyncio")
+    return StandaloneTCPNetworkServer(None, PORT, StreamProtocol(StringLineSerializer()), MyAsyncRequestHandler())
 
 
 def create_udp_server() -> StandaloneUDPNetworkServer[str, str]:
-    return StandaloneUDPNetworkServer(None, PORT, DatagramProtocol(StringLineSerializer()), MyAsyncRequestHandler(), "asyncio")
+    return StandaloneUDPNetworkServer(None, PORT, DatagramProtocol(StringLineSerializer()), MyAsyncRequestHandler())
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "-v",
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/_utils.py` & `easynetwork-1.0.0rc4/tests/unit_test/_utils.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/base.py` & `easynetwork-1.0.0rc4/tests/unit_test/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/conftest.py` & `easynetwork-1.0.0rc4/tests/unit_test/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_converter.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_converter.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_protocol.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/base.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/conftest.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/_fake_backends.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/test_backend.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/test_backend.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_backend/test_futures.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_backend/test_futures.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_abc.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_tcp.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_tcp.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_client/test_udp.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_client/test_udp.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_api/test_server/test_handler.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_api/test_server/test_handler.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/conftest.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_backend.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import contextvars
 from typing import TYPE_CHECKING, Any, Callable, Sequence, cast
 
+from easynetwork.api_async.backend.abc import AbstractAsyncStreamSocketAdapter
 from easynetwork_asyncio import AsyncioBackend
 
 import pytest
 
 from ..._utils import partial_eq
 
 if TYPE_CHECKING:
@@ -121,15 +122,15 @@
     ) -> None:
         # Arrange
         from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
 
         mock_asyncio_reader = mock_asyncio_stream_reader_factory()
         mock_asyncio_writer = mock_asyncio_stream_writer_factory()
         mock_StreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", return_value=mocker.sentinel.socket
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", return_value=mocker.sentinel.socket
         )
         mock_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             return_value=(mock_asyncio_reader, mock_asyncio_writer),
         )
 
@@ -139,14 +140,15 @@
                 "ssl": mock_ssl_context,
                 "server_hostname": "server_hostname",
                 "ssl_handshake_timeout": 123456.789,
                 "ssl_shutdown_timeout": 9876543.21,
             }
 
         # Act
+        socket: AbstractAsyncStreamSocketAdapter
         if ssl:
             socket = await backend.create_ssl_over_tcp_connection(
                 *remote_address,
                 ssl_context=mock_ssl_context,
                 server_hostname="server_hostname",
                 ssl_handshake_timeout=123456.789,
                 ssl_shutdown_timeout=9876543.21,
@@ -183,20 +185,21 @@
         mock_asyncio_stream_writer_factory: Callable[[], MagicMock],
         mock_ssl_context: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
 
-        mocker.patch("easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", return_value=mocker.sentinel.socket)
+        mocker.patch("easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", return_value=mocker.sentinel.socket)
         mock_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             return_value=(mock_asyncio_stream_reader_factory(), mock_asyncio_stream_writer_factory()),
         )
+        mocker.patch("asyncio.get_running_loop", return_value=mocker.NonCallableMagicMock(spec=asyncio.AbstractEventLoop))
         expected_ssl_kwargs: dict[str, Any] = {}
         if ssl:
             expected_ssl_kwargs = {
                 "ssl": mock_ssl_context,
                 "server_hostname": "server_hostname",
                 "ssl_handshake_timeout": 123456.789,
                 "ssl_shutdown_timeout": 9876543.21,
@@ -224,35 +227,94 @@
         mock_open_connection.assert_awaited_once_with(
             *remote_address,
             **expected_ssl_kwargs,
             local_addr=local_address,
             limit=MAX_STREAM_BUFSIZE,
         )
 
+    @pytest.mark.parametrize("use_asyncio_transport", [True], indirect=True)
+    @pytest.mark.parametrize("ssl", [False, True], ids=lambda p: f"ssl=={p}")
+    async def test____create_tcp_connection____use_asyncio_open_connection____happy_eyeballs_delay_default_value_for_asyncio_implementation(
+        self,
+        ssl: bool,
+        local_address: tuple[str, int] | None,
+        remote_address: tuple[str, int],
+        backend: AsyncioBackend,
+        mock_asyncio_stream_reader_factory: Callable[[], MagicMock],
+        mock_asyncio_stream_writer_factory: Callable[[], MagicMock],
+        mock_ssl_context: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
+
+        mocker.patch("easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", return_value=mocker.sentinel.socket)
+        mock_open_connection: AsyncMock = mocker.patch(
+            "asyncio.open_connection",
+            new_callable=mocker.AsyncMock,
+            return_value=(mock_asyncio_stream_reader_factory(), mock_asyncio_stream_writer_factory()),
+        )
+        mocker.patch("asyncio.get_running_loop", return_value=mocker.NonCallableMagicMock(spec=asyncio.base_events.BaseEventLoop))
+        expected_ssl_kwargs: dict[str, Any] = {}
+        if ssl:
+            expected_ssl_kwargs = {
+                "ssl": mock_ssl_context,
+                "server_hostname": "server_hostname",
+                "ssl_handshake_timeout": 123456.789,
+                "ssl_shutdown_timeout": 9876543.21,
+            }
+
+        # Act
+        if ssl:
+            await backend.create_ssl_over_tcp_connection(
+                *remote_address,
+                ssl_context=mock_ssl_context,
+                server_hostname="server_hostname",
+                ssl_handshake_timeout=123456.789,
+                ssl_shutdown_timeout=9876543.21,
+                happy_eyeballs_delay=None,
+                local_address=local_address,
+            )
+        else:
+            await backend.create_tcp_connection(
+                *remote_address,
+                happy_eyeballs_delay=None,
+                local_address=local_address,
+            )
+
+        # Assert
+        mock_open_connection.assert_awaited_once_with(
+            *remote_address,
+            **expected_ssl_kwargs,
+            local_addr=local_address,
+            happy_eyeballs_delay=0.25,
+            limit=MAX_STREAM_BUFSIZE,
+        )
+
     @pytest.mark.parametrize("use_asyncio_transport", [False], indirect=True)
     async def test____create_tcp_connection____creates_raw_socket_adapter(
         self,
         event_loop: asyncio.AbstractEventLoop,
         local_address: tuple[str, int] | None,
         remote_address: tuple[str, int],
         backend: AsyncioBackend,
         mock_tcp_socket: Callable[[], MagicMock],
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_RawStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter", return_value=mocker.sentinel.socket
+            "easynetwork_asyncio.backend.RawStreamSocketAdapter", return_value=mocker.sentinel.socket
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
         mock_own_create_connection: AsyncMock = mocker.patch(
-            "easynetwork_asyncio._utils.create_connection",
+            "easynetwork_asyncio.backend.create_connection",
             new_callable=mocker.AsyncMock,
             return_value=mock_tcp_socket,
         )
 
         # Act
         socket = await backend.create_tcp_connection(
             *remote_address,
@@ -275,23 +337,23 @@
         local_address: tuple[str, int] | None,
         remote_address: tuple[str, int],
         backend: AsyncioBackend,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_RawStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.RawStreamSocketAdapter", side_effect=AssertionError
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
         mock_own_create_connection: AsyncMock = mocker.patch(
-            "easynetwork_asyncio._utils.create_connection",
+            "easynetwork_asyncio.backend.create_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
 
         # Act
         with pytest.raises(ValueError, match=r"^'happy_eyeballs_delay' option not supported with transport=False$"):
             await backend.create_tcp_connection(
@@ -312,26 +374,26 @@
         remote_address: tuple[str, int],
         backend: AsyncioBackend,
         mock_ssl_context: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
         )
         mock_RawStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.RawStreamSocketAdapter", side_effect=AssertionError
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
         mock_own_create_connection: AsyncMock = mocker.patch(
-            "easynetwork_asyncio._utils.create_connection",
+            "easynetwork_asyncio.backend.create_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
 
         # Act
         with pytest.raises(ValueError, match=r"^SSL\/TLS not supported with transport=False$"):
             await backend.create_ssl_over_tcp_connection(
@@ -356,15 +418,15 @@
         local_address: tuple[str, int] | None,
         remote_address: tuple[str, int],
         backend: AsyncioBackend,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
 
@@ -380,14 +442,49 @@
                 local_address=local_address,
             )
 
         # Assert
         mock_asyncio_open_connection.assert_not_called()
         mock_AsyncioTransportStreamSocketAdapter.assert_not_called()
 
+    @pytest.mark.usefixtures("simulate_no_ssl_module")
+    @pytest.mark.parametrize("use_asyncio_transport", [True], indirect=True)
+    async def test____create_ssl_over_tcp_connection____no_ssl_module(
+        self,
+        local_address: tuple[str, int] | None,
+        remote_address: tuple[str, int],
+        backend: AsyncioBackend,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+        )
+        mock_asyncio_open_connection: AsyncMock = mocker.patch(
+            "asyncio.open_connection",
+            new_callable=mocker.AsyncMock,
+            side_effect=AssertionError,
+        )
+
+        # Act
+        with pytest.raises(RuntimeError, match=r"^stdlib ssl module not available$"):
+            await backend.create_ssl_over_tcp_connection(
+                *remote_address,
+                ssl_context=True,  # type: ignore[arg-type]
+                server_hostname="server_hostname",
+                ssl_handshake_timeout=123456.789,
+                ssl_shutdown_timeout=9876543.21,
+                happy_eyeballs_delay=42,
+                local_address=local_address,
+            )
+
+        # Assert
+        mock_asyncio_open_connection.assert_not_called()
+        mock_AsyncioTransportStreamSocketAdapter.assert_not_called()
+
     async def test____wrap_tcp_client_socket____use_asyncio_open_connection(
         self,
         event_loop: asyncio.AbstractEventLoop,
         backend: AsyncioBackend,
         use_asyncio_transport: bool,
         mock_tcp_socket: MagicMock,
         mock_asyncio_stream_reader_factory: Callable[[], MagicMock],
@@ -396,19 +493,19 @@
     ) -> None:
         # Arrange
         from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
 
         mock_asyncio_reader = mock_asyncio_stream_reader_factory()
         mock_asyncio_writer = mock_asyncio_stream_writer_factory()
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter",
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_RawStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter",
+            "easynetwork_asyncio.backend.RawStreamSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             return_value=(mock_asyncio_reader, mock_asyncio_writer),
         )
@@ -443,15 +540,15 @@
     ) -> None:
         # Arrange
         from easynetwork.tools.socket import MAX_STREAM_BUFSIZE
 
         mock_asyncio_reader = mock_asyncio_stream_reader_factory()
         mock_asyncio_writer = mock_asyncio_stream_writer_factory()
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter",
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             return_value=(mock_asyncio_reader, mock_asyncio_writer),
         )
@@ -494,26 +591,26 @@
         mock_tcp_socket: MagicMock,
         backend: AsyncioBackend,
         mock_ssl_context: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
         )
         mock_RawStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.RawStreamSocketAdapter", side_effect=AssertionError
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
         mock_own_create_connection: AsyncMock = mocker.patch(
-            "easynetwork_asyncio._utils.create_connection",
+            "easynetwork_asyncio.backend.create_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
 
         # Act
         with pytest.raises(ValueError, match=r"^SSL\/TLS not supported with transport=False$"):
             await backend.wrap_ssl_over_tcp_client_socket(
@@ -535,15 +632,15 @@
         self,
         mock_tcp_socket: MagicMock,
         backend: AsyncioBackend,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
         )
         mock_asyncio_open_connection: AsyncMock = mocker.patch(
             "asyncio.open_connection",
             new_callable=mocker.AsyncMock,
             side_effect=AssertionError,
         )
 
@@ -557,14 +654,46 @@
                 ssl_shutdown_timeout=9876543.21,
             )
 
         # Assert
         mock_asyncio_open_connection.assert_not_called()
         mock_AsyncioTransportStreamSocketAdapter.assert_not_called()
 
+    @pytest.mark.usefixtures("simulate_no_ssl_module")
+    @pytest.mark.parametrize("use_asyncio_transport", [True], indirect=True)
+    async def test____wrap_ssl_over_tcp_client_socket____no_ssl_module(
+        self,
+        mock_tcp_socket: MagicMock,
+        backend: AsyncioBackend,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        mock_AsyncioTransportStreamSocketAdapter: MagicMock = mocker.patch(
+            "easynetwork_asyncio.backend.AsyncioTransportStreamSocketAdapter", side_effect=AssertionError
+        )
+        mock_asyncio_open_connection: AsyncMock = mocker.patch(
+            "asyncio.open_connection",
+            new_callable=mocker.AsyncMock,
+            side_effect=AssertionError,
+        )
+
+        # Act
+        with pytest.raises(RuntimeError, match=r"^stdlib ssl module not available$"):
+            await backend.wrap_ssl_over_tcp_client_socket(
+                mock_tcp_socket,
+                ssl_context=True,  # type: ignore[arg-type]
+                server_hostname="server_hostname",
+                ssl_handshake_timeout=123456.789,
+                ssl_shutdown_timeout=9876543.21,
+            )
+
+        # Assert
+        mock_asyncio_open_connection.assert_not_called()
+        mock_AsyncioTransportStreamSocketAdapter.assert_not_called()
+
     @pytest.mark.parametrize(
         ["use_ssl", "use_asyncio_transport"],
         [
             pytest.param(False, False, id="NO_SSL-use_asyncio_transport==False"),
             pytest.param(False, True, id="NO_SSL-use_asyncio_transport==True"),
             pytest.param(True, True, id="USE_SSL"),
         ],
@@ -601,19 +730,19 @@
                 event_loop,
                 "getaddrinfo",
                 new_callable=mocker.AsyncMock,
                 return_value=addrinfo_list,
             ),
         )
         mock_open_listeners = mocker.patch(
-            "easynetwork.tools._utils.open_listener_sockets_from_getaddrinfo_result",
+            "easynetwork_asyncio.backend.open_listener_sockets_from_getaddrinfo_result",
             return_value=[mock_tcp_socket],
         )
         mock_ListenerSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.listener.ListenerSocketAdapter", return_value=mocker.sentinel.listener_socket
+            "easynetwork_asyncio.backend.ListenerSocketAdapter", return_value=mocker.sentinel.listener_socket
         )
         expected_factory: partial_eq
         if use_ssl:
             expected_factory = partial_eq(
                 AcceptedSSLSocket,
                 ssl_context=mock_ssl_context,
                 ssl_handshake_timeout=123456.789,
@@ -712,19 +841,19 @@
                 event_loop,
                 "getaddrinfo",
                 new_callable=mocker.AsyncMock,
                 return_value=addrinfo_list,
             ),
         )
         mock_open_listeners = mocker.patch(
-            "easynetwork.tools._utils.open_listener_sockets_from_getaddrinfo_result",
+            "easynetwork_asyncio.backend.open_listener_sockets_from_getaddrinfo_result",
             return_value=[mock_tcp_socket, mock_tcp_socket],
         )
         mock_ListenerSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.listener.ListenerSocketAdapter",
+            "easynetwork_asyncio.backend.ListenerSocketAdapter",
             return_value=mocker.sentinel.listener_socket,
         )
         expected_factory: partial_eq
         if use_ssl:
             expected_factory = partial_eq(
                 AcceptedSSLSocket,
                 ssl_context=mock_ssl_context,
@@ -825,19 +954,19 @@
                 event_loop,
                 "getaddrinfo",
                 new_callable=mocker.AsyncMock,
                 side_effect=[[info] for info in addrinfo_list],
             ),
         )
         mock_open_listeners = mocker.patch(
-            "easynetwork.tools._utils.open_listener_sockets_from_getaddrinfo_result",
+            "easynetwork_asyncio.backend.open_listener_sockets_from_getaddrinfo_result",
             return_value=[mock_tcp_socket, mock_tcp_socket],
         )
         mock_ListenerSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.listener.ListenerSocketAdapter",
+            "easynetwork_asyncio.backend.ListenerSocketAdapter",
             return_value=mocker.sentinel.listener_socket,
         )
         expected_factory: partial_eq
         if use_ssl:
             expected_factory = partial_eq(
                 AcceptedSSLSocket,
                 ssl_context=mock_ssl_context,
@@ -921,19 +1050,19 @@
                 event_loop,
                 "getaddrinfo",
                 new_callable=mocker.AsyncMock,
                 return_value=[],
             ),
         )
         mock_open_listeners = mocker.patch(
-            "easynetwork.tools._utils.open_listener_sockets_from_getaddrinfo_result",
+            "easynetwork_asyncio.backend.open_listener_sockets_from_getaddrinfo_result",
             side_effect=AssertionError,
         )
         mock_ListenerSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.listener.ListenerSocketAdapter",
+            "easynetwork_asyncio.backend.ListenerSocketAdapter",
             side_effect=AssertionError,
         )
 
         # Act
         with pytest.raises(OSError, match=r"getaddrinfo\('remote_address'\) returned empty list"):
             if use_ssl:
                 await backend.create_ssl_over_tcp_listeners(
@@ -982,19 +1111,19 @@
                 event_loop,
                 "getaddrinfo",
                 new_callable=mocker.AsyncMock,
                 return_value=[],
             ),
         )
         mock_open_listeners = mocker.patch(
-            "easynetwork.tools._utils.open_listener_sockets_from_getaddrinfo_result",
+            "easynetwork_asyncio.backend.open_listener_sockets_from_getaddrinfo_result",
             side_effect=AssertionError,
         )
         mock_ListenerSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.stream.listener.ListenerSocketAdapter",
+            "easynetwork_asyncio.backend.ListenerSocketAdapter",
             side_effect=AssertionError,
         )
 
         # Act
         with pytest.raises(ValueError, match=r"^SSL\/TLS not supported with transport=False$"):
             await backend.create_ssl_over_tcp_listeners(
                 remote_host,
@@ -1021,28 +1150,28 @@
         mock_datagram_endpoint_factory: Callable[[], MagicMock],
         use_asyncio_transport: bool,
         mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         mock_endpoint = mock_datagram_endpoint_factory()
         mock_AsyncioTransportDatagramSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.datagram.socket.AsyncioTransportDatagramSocketAdapter",
+            "easynetwork_asyncio.backend.AsyncioTransportDatagramSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_RawDatagramSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.datagram.socket.RawDatagramSocketAdapter",
+            "easynetwork_asyncio.backend.RawDatagramSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_create_datagram_endpoint: AsyncMock = mocker.patch(
-            "easynetwork_asyncio.datagram.endpoint.create_datagram_endpoint",
+            "easynetwork_asyncio.backend.create_datagram_endpoint",
             new_callable=mocker.AsyncMock,
             return_value=mock_endpoint,
         )
         mock_create_datagram_socket: AsyncMock = mocker.patch(
-            "easynetwork_asyncio._utils.create_datagram_socket",
+            "easynetwork_asyncio.backend.create_datagram_socket",
             new_callable=mocker.AsyncMock,
             return_value=mock_udp_socket,
         )
 
         # Act
         socket = await backend.create_udp_endpoint(
             local_address=local_address,
@@ -1077,23 +1206,23 @@
         mock_udp_socket: MagicMock,
         mock_datagram_endpoint_factory: Callable[[], MagicMock],
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_endpoint = mock_datagram_endpoint_factory()
         mock_AsyncioTransportDatagramSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.datagram.socket.AsyncioTransportDatagramSocketAdapter",
+            "easynetwork_asyncio.backend.AsyncioTransportDatagramSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_RawDatagramSocketAdapter: MagicMock = mocker.patch(
-            "easynetwork_asyncio.datagram.socket.RawDatagramSocketAdapter",
+            "easynetwork_asyncio.backend.RawDatagramSocketAdapter",
             return_value=mocker.sentinel.socket,
         )
         mock_create_datagram_endpoint: AsyncMock = mocker.patch(
-            "easynetwork_asyncio.datagram.endpoint.create_datagram_endpoint",
+            "easynetwork_asyncio.backend.create_datagram_endpoint",
             new_callable=mocker.AsyncMock,
             return_value=mock_endpoint,
         )
 
         # Act
         socket = await backend.wrap_udp_socket(mock_udp_socket)
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_datagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -828,15 +828,15 @@
 
 
 @pytest.mark.asyncio
 class TestRawDatagramSocketAdapter(BaseTestSocket):
     @pytest.fixture(autouse=True)
     @staticmethod
     def mock_async_socket_cls(mock_async_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
-        return mocker.patch("easynetwork_asyncio.socket.AsyncSocket", return_value=mock_async_socket)
+        return mocker.patch(f"{RawDatagramSocketAdapter.__module__}.AsyncSocket", return_value=mock_async_socket)
 
     @pytest.fixture
     @classmethod
     def mock_udp_socket(cls, mock_udp_socket: MagicMock) -> MagicMock:
         cls.set_local_address_to_socket_mock(mock_udp_socket, mock_udp_socket.family, ("127.0.0.1", 11111))
         cls.set_remote_address_to_socket_mock(mock_udp_socket, mock_udp_socket.family, ("127.0.0.1", 12345))
         return mock_udp_socket
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_socket.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_socket.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_stream.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,21 +54,14 @@
             }
         )
         mock = mock_asyncio_stream_writer_factory()
         mock.get_extra_info.side_effect = asyncio_writer_extra_info.get
         return mock
 
 
-class BaseTestRawStreamSocket(BaseTestSocket):
-    @pytest.fixture(autouse=True)
-    @staticmethod
-    def mock_async_socket_cls(mock_async_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
-        return mocker.patch("easynetwork_asyncio.socket.AsyncSocket", return_value=mock_async_socket)
-
-
 @pytest.mark.asyncio
 class TestTransportBasedStreamSocket(BaseTestTransportStreamSocket):
     @pytest.fixture
     @staticmethod
     def socket(mock_asyncio_reader: MagicMock, mock_asyncio_writer: MagicMock) -> AsyncioTransportStreamSocketAdapter:
         return AsyncioTransportStreamSocketAdapter(mock_asyncio_reader, mock_asyncio_writer)
 
@@ -282,15 +275,20 @@
         transport_socket = socket.socket()
 
         # Assert
         assert transport_socket is mock_tcp_socket
 
 
 @pytest.mark.asyncio
-class TestListenerSocketAdapter(BaseTestTransportStreamSocket, BaseTestRawStreamSocket):
+class TestListenerSocketAdapter(BaseTestTransportStreamSocket, BaseTestSocket):
+    @pytest.fixture(autouse=True)
+    @staticmethod
+    def mock_async_socket_cls(mock_async_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
+        return mocker.patch(f"{ListenerSocketAdapter.__module__}.AsyncSocket", return_value=mock_async_socket)
+
     @pytest.fixture
     @classmethod
     def mock_tcp_listener_socket(
         cls,
         mock_tcp_socket_factory: Callable[[], MagicMock],
     ) -> MagicMock:
         mock_socket = mock_tcp_socket_factory()
@@ -398,33 +396,38 @@
         # Assert
         mock_async_socket.accept.assert_awaited_once_with()
         accepted_socket_factory.assert_called_once_with(mock_tcp_socket, event_loop)
         assert accepted_socket is mock_accepted_socket
 
 
 @pytest.mark.asyncio
-class TestAcceptedSocket(BaseTestTransportStreamSocket, BaseTestRawStreamSocket):
+class TestAcceptedSocket(BaseTestTransportStreamSocket, BaseTestSocket):
+    @pytest.fixture(autouse=True)
+    @staticmethod
+    def mock_async_socket_cls(mock_async_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
+        return mocker.patch(f"{ListenerSocketAdapter.__module__}.AsyncSocket", return_value=mock_async_socket)
+
     @pytest.fixture(params=[False, True], ids=lambda boolean: f"use_asyncio_transport=={boolean}")
     @staticmethod
     def use_asyncio_transport(request: Any) -> bool:
         return request.param
 
     @pytest.fixture
     @staticmethod
     def mock_transport_stream_socket_adapter_cls(mock_stream_socket_adapter: MagicMock, mocker: MockerFixture) -> MagicMock:
         return mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter",
+            f"{ListenerSocketAdapter.__module__}.AsyncioTransportStreamSocketAdapter",
             return_value=mock_stream_socket_adapter,
         )
 
     @pytest.fixture
     @staticmethod
     def mock_raw_stream_socket_adapter_cls(mock_stream_socket_adapter: MagicMock, mocker: MockerFixture) -> MagicMock:
         return mocker.patch(
-            "easynetwork_asyncio.stream.socket.RawStreamSocketAdapter",
+            f"{ListenerSocketAdapter.__module__}.RawStreamSocketAdapter",
             return_value=mock_stream_socket_adapter,
         )
 
     @pytest.fixture
     @staticmethod
     def mock_stream_socket_adapter(mock_stream_socket_adapter: MagicMock) -> MagicMock:
         mock_stream_socket_adapter.get_remote_address.return_value = ("127.0.0.1", 12345)
@@ -547,15 +550,15 @@
     def ssl_shutdown_timeout() -> float:
         return 9876543.21
 
     @pytest.fixture
     @staticmethod
     def mock_transport_stream_socket_adapter_cls(mock_stream_socket_adapter: MagicMock, mocker: MockerFixture) -> MagicMock:
         return mocker.patch(
-            "easynetwork_asyncio.stream.socket.AsyncioTransportStreamSocketAdapter",
+            f"{ListenerSocketAdapter.__module__}.AsyncioTransportStreamSocketAdapter",
             return_value=mock_stream_socket_adapter,
         )
 
     @pytest.fixture
     @staticmethod
     def mock_stream_socket_adapter(mock_stream_socket_adapter: MagicMock) -> MagicMock:
         mock_stream_socket_adapter.get_remote_address.return_value = ("127.0.0.1", 12345)
@@ -664,15 +667,20 @@
         mock_transport_stream_socket_adapter_cls.assert_called_once_with(
             mock_asyncio_reader,
             mock_asyncio_writer,
         )
 
 
 @pytest.mark.asyncio
-class TestRawStreamSocketAdapter(BaseTestRawStreamSocket):
+class TestRawStreamSocketAdapter(BaseTestSocket):
+    @pytest.fixture(autouse=True)
+    @staticmethod
+    def mock_async_socket_cls(mock_async_socket: MagicMock, mocker: MockerFixture) -> MagicMock:
+        return mocker.patch(f"{RawStreamSocketAdapter.__module__}.AsyncSocket", return_value=mock_async_socket)
+
     @pytest.fixture
     @classmethod
     def mock_tcp_socket(cls, mock_tcp_socket: MagicMock) -> MagicMock:
         cls.set_local_address_to_socket_mock(mock_tcp_socket, mock_tcp_socket.family, ("127.0.0.1", 11111))
         cls.set_remote_address_to_socket_mock(mock_tcp_socket, mock_tcp_socket.family, ("127.0.0.1", 12345))
         return mock_tcp_socket
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_tasks.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_threads.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_threads.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_async/test_asyncio_backend/test_utils.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_async/test_asyncio_backend/test_utils.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/base.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_abc.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_base64.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_base64.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
 
 
 class TestBase64EncodedSerializer:
-    @pytest.fixture
+    @pytest.fixture(autouse=True)
     @staticmethod
     def mock_b64encode(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("base64.urlsafe_b64encode", autospec=True)
 
-    @pytest.fixture
+    @pytest.fixture(autouse=True)
     @staticmethod
     def mock_b64decode(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("base64.urlsafe_b64decode", autospec=True)
 
     @pytest.mark.parametrize("method", ["incremental_serialize", "incremental_deserialize"])
     def test____base_class____implements_default_methods(self, method: str) -> None:
         # Arrange
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_cbor.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_cbor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_compressor.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_compressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,20 +370,20 @@
 
 class TestBZ2CompressorSerializer(BaseTestCompressorSerializerImplementation):
     @pytest.fixture(scope="class")
     @staticmethod
     def serializer_cls() -> type[BZ2CompressorSerializer[Any, Any]]:
         return BZ2CompressorSerializer
 
-    @pytest.fixture
+    @pytest.fixture(autouse=True)
     @staticmethod
     def mock_bz2_compressor_cls(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("bz2.BZ2Compressor")
 
-    @pytest.fixture
+    @pytest.fixture(autouse=True)
     @staticmethod
     def mock_bz2_decompressor_cls(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("bz2.BZ2Decompressor")
 
     @pytest.mark.parametrize(
         "with_compress_level",
         [
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_encryptor.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_encryptor.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_json.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_line.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_line.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_msgpack.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_pickle.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_pickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         )
 
     @pytest.fixture(params=[False, True], ids=lambda boolean: f"optimize=={boolean}")
     @staticmethod
     def pickler_optimize(request: Any) -> bool:
         return request.param
 
-    @pytest.fixture
+    @pytest.fixture(autouse=True)
     @staticmethod
     def mock_pickletools_optimize(mocker: MockerFixture) -> MagicMock:
         return mocker.patch("pickletools.optimize", autospec=True)
 
     def test____serialize____with_config(
         self,
         pickler_optimize: bool,
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_serializers/test_struct.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_serializers/test_struct.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/base.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/base.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/conftest.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/conftest.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_abc.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_abc.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_tcp.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_tcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 import contextlib
 import errno
 import os
 from selectors import EVENT_READ, EVENT_WRITE
-from socket import AF_INET6, IPPROTO_TCP, SO_KEEPALIVE, TCP_NODELAY
-from ssl import SOL_SOCKET, SSLEOFError, SSLError, SSLErrorNumber, SSLWantReadError, SSLWantWriteError, SSLZeroReturnError
+from socket import AF_INET6, IPPROTO_TCP, SHUT_RDWR, SO_KEEPALIVE, SOL_SOCKET, TCP_NODELAY
+from ssl import SSLEOFError, SSLError, SSLErrorNumber, SSLWantReadError, SSLWantWriteError, SSLZeroReturnError
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.api_sync.client.tcp import TCPNetworkClient
 from easynetwork.exceptions import ClientClosedError
 from easynetwork.tools.socket import (
     CLOSED_SOCKET_ERRNOS,
     MAX_STREAM_BUFSIZE,
@@ -192,20 +192,26 @@
         return getattr(request, "param", None)
 
     @pytest.fixture
     @staticmethod
     def ssl_shutdown_timeout(request: Any) -> float | None:
         return getattr(request, "param", None)
 
+    @pytest.fixture
+    @staticmethod
+    def retry_interval(request: Any) -> float:
+        return getattr(request, "param", float("+inf"))
+
     @pytest.fixture(params=["REMOTE_ADDRESS", "EXTERNAL_SOCKET"])
     @staticmethod
     def client(
         request: Any,
         max_recv_size: int | None,
         ssl_shutdown_timeout: float | None,
+        retry_interval: float,
         remote_address: tuple[str, int],
         mock_tcp_socket: MagicMock,
         mock_stream_protocol: MagicMock,
         ssl_context: MagicMock | None,
         server_hostname: Any | None,
         mock_selector_register: MagicMock,
         mock_selector_select: MagicMock,
@@ -216,34 +222,37 @@
                     return TCPNetworkClient(
                         remote_address,
                         mock_stream_protocol,
                         ssl=ssl_context,
                         server_hostname=server_hostname,
                         max_recv_size=max_recv_size,
                         ssl_shutdown_timeout=ssl_shutdown_timeout,
+                        retry_interval=retry_interval,
                     )
                 case "EXTERNAL_SOCKET":
                     return TCPNetworkClient(
                         mock_tcp_socket,
                         mock_stream_protocol,
                         ssl=ssl_context,
                         server_hostname=server_hostname,
                         max_recv_size=max_recv_size,
                         ssl_shutdown_timeout=ssl_shutdown_timeout,
+                        retry_interval=retry_interval,
                     )
                 case invalid:
                     pytest.fail(f"Invalid fixture param: Got {invalid!r}")
         finally:
             mock_tcp_socket.settimeout.reset_mock()
             mock_selector_register.reset_mock()
             mock_selector_select.reset_mock()
 
     @pytest.fixture(
         params=[
-            pytest.param(None, id="blocking"),
+            pytest.param(None, id="blocking (None)"),
+            pytest.param(float("+inf"), id="blocking (+inf)"),
             pytest.param(0, id="non_blocking"),
             pytest.param(123456789, id="with_timeout"),
         ]
     )
     @staticmethod
     def recv_timeout(request: Any) -> Any:
         return request.param
@@ -552,14 +561,60 @@
         mock_ssl_create_default_context.assert_not_called()
         mock_stream_data_consumer_cls.assert_not_called()
         mock_socket_proxy_cls.assert_not_called()
         mock_tcp_socket.getsockname.assert_not_called()
         mock_tcp_socket.getpeername.assert_not_called()
         mock_tcp_socket.close.assert_called_once_with()
 
+    @pytest.mark.parametrize("retry_interval", [0, -12.34])
+    @pytest.mark.parametrize("use_socket", [False, True], ids=lambda p: f"use_socket=={p}")
+    def test____dunder_init____retry_interval____invalid_value(
+        self,
+        retry_interval: float,
+        use_socket: bool,
+        remote_address: tuple[str, int],
+        mock_tcp_socket: MagicMock,
+        mock_stream_protocol: MagicMock,
+        mock_stream_data_consumer_cls: MagicMock,
+        mock_socket_proxy_cls: MagicMock,
+        mock_ssl_create_default_context: MagicMock,
+        ssl_context: MagicMock | None,
+        server_hostname: Any | None,
+    ) -> None:
+        # Arrange
+
+        # Act
+        with pytest.raises(ValueError, match=r"^retry_interval must be a strictly positive float or None$"):
+            if use_socket:
+                _ = TCPNetworkClient(
+                    mock_tcp_socket,
+                    protocol=mock_stream_protocol,
+                    retry_interval=retry_interval,
+                    ssl=ssl_context,
+                    server_hostname=server_hostname,
+                )
+            else:
+                _ = TCPNetworkClient(
+                    remote_address,
+                    protocol=mock_stream_protocol,
+                    retry_interval=retry_interval,
+                    ssl=ssl_context,
+                    server_hostname=server_hostname,
+                )
+
+        # Assert
+        if ssl_context:
+            ssl_context.wrap_socket.assert_not_called()
+        mock_ssl_create_default_context.assert_not_called()
+        mock_stream_data_consumer_cls.assert_not_called()
+        mock_socket_proxy_cls.assert_not_called()
+        mock_tcp_socket.getsockname.assert_not_called()
+        mock_tcp_socket.getpeername.assert_not_called()
+        mock_tcp_socket.close.assert_called_once_with()
+
     @pytest.mark.parametrize("use_ssl", ["NO_SSL"], indirect=True)
     @pytest.mark.parametrize("use_socket", [False, True], ids=lambda p: f"use_socket=={p}")
     @pytest.mark.parametrize("ssl_parameter", ["server_hostname", "ssl_handshake_timeout", "ssl_shutdown_timeout"])
     def test____dunder_init____ssl____useless_parameter_if_no_context(
         self,
         ssl_parameter: str,
         use_socket: bool,
@@ -778,14 +833,15 @@
             pytest.param(SSLWantWriteError, EVENT_WRITE, id="write"),
         ],
     )
     def test____dunder_init____ssl____handshake_timeout(
         self,
         ssl_handshake_timeout: float | None,
         use_socket: bool,
+        retry_interval: float,
         would_block_exception: Exception,
         would_block_event: int,
         remote_address: tuple[str, int],
         mock_ssl_context: MagicMock,
         mock_tcp_socket: MagicMock,
         mock_ssl_socket: MagicMock,
         mock_stream_protocol: MagicMock,
@@ -802,22 +858,24 @@
             if use_socket:
                 _ = TCPNetworkClient(
                     mock_tcp_socket,
                     protocol=mock_stream_protocol,
                     ssl=mock_ssl_context,
                     server_hostname=server_hostname,
                     ssl_handshake_timeout=ssl_handshake_timeout,
+                    retry_interval=retry_interval,
                 )
             else:
                 _ = TCPNetworkClient(
                     remote_address,
                     protocol=mock_stream_protocol,
                     ssl=mock_ssl_context,
                     server_hostname=server_hostname,
                     ssl_handshake_timeout=ssl_handshake_timeout,
+                    retry_interval=retry_interval,
                 )
 
         # Assert
         if expected_timeout == 0:
             assert len(mock_ssl_socket.do_handshake.mock_calls) == 1
             mock_selector_register.assert_not_called()
             mock_selector_select.assert_not_called()
@@ -838,20 +896,20 @@
 
         # Act
         client.close()
 
         # Assert
         assert client.is_closed()
 
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_ssl_socket.shutdown.assert_not_called()
-
         if use_ssl:
             mock_ssl_socket.unwrap.assert_called_once_with()
 
+        mock_tcp_socket.shutdown.assert_called_once_with(SHUT_RDWR)
+        mock_ssl_socket.shutdown.assert_not_called()
+
         mock_tcp_socket.close.assert_called_once_with()
         mock_ssl_socket.close.assert_not_called()
 
     @pytest.mark.parametrize("use_ssl", ["USE_SSL"], indirect=True)
     @pytest.mark.parametrize("exception", [SSLEOFError, SSLZeroReturnError, ConnectionError])
     def test____close____ssl____connection_error_at_shutdown(
         self,
@@ -866,19 +924,19 @@
 
         # Act
         client.close()
 
         # Assert
         assert client.is_closed()
 
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_ssl_socket.shutdown.assert_not_called()
-
         mock_ssl_socket.unwrap.assert_called_once_with()
 
+        mock_tcp_socket.shutdown.assert_not_called()
+        mock_ssl_socket.shutdown.assert_called_once_with(SHUT_RDWR)
+
         mock_tcp_socket.close.assert_not_called()
         mock_ssl_socket.close.assert_called_once_with()
 
     @pytest.mark.parametrize("use_ssl", ["USE_SSL"], indirect=True)
     def test____close____ssl____unrelated_ssl_error(
         self,
         client: TCPNetworkClient[Any, Any],
@@ -892,19 +950,19 @@
         # Act
         with pytest.raises(SSLError):
             client.close()
 
         # Assert
         assert client.is_closed()
 
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_ssl_socket.shutdown.assert_not_called()
-
         mock_ssl_socket.unwrap.assert_called_once_with()
 
+        mock_tcp_socket.shutdown.assert_not_called()
+        mock_ssl_socket.shutdown.assert_called_once_with(SHUT_RDWR)
+
         mock_tcp_socket.close.assert_not_called()
         mock_ssl_socket.close.assert_called_once_with()
 
     @pytest.mark.parametrize("use_ssl", ["USE_SSL"], indirect=True)
     @pytest.mark.parametrize("ssl_shutdown_timeout", [None, 0, 1234567.89], ids=lambda p: f"timeout=={p}", indirect=True)
     @pytest.mark.parametrize(
         ["would_block_exception", "would_block_event"],
@@ -930,31 +988,54 @@
 
         # Act
         client.close()
 
         # Assert
         assert client.is_closed()
 
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_ssl_socket.shutdown.assert_not_called()
-
         if expected_timeout == 0:
             assert mock_ssl_socket.unwrap.call_count == 1
             mock_ssl_socket.unwrap.assert_called_once()
             mock_selector_register.assert_not_called()
             mock_selector_select.assert_not_called()
+            mock_tcp_socket.shutdown.assert_not_called()
+            mock_ssl_socket.shutdown.assert_called_once_with(SHUT_RDWR)
             mock_tcp_socket.close.assert_not_called()
             mock_ssl_socket.close.assert_called_once_with()
         else:
             assert mock_ssl_socket.unwrap.call_count == 2
             mock_selector_register.assert_called_once_with(mock_ssl_socket, would_block_event)
             mock_selector_select.assert_called_once_with(expected_timeout)
+            mock_ssl_socket.shutdown.assert_not_called()
+            mock_tcp_socket.shutdown.assert_called_once_with(SHUT_RDWR)
             mock_ssl_socket.close.assert_not_called()
             mock_tcp_socket.close.assert_called_once_with()
 
+    def test____close____shutdown_raises_OSError(
+        self,
+        client: TCPNetworkClient[Any, Any],
+        mock_tcp_socket: MagicMock,
+        mock_ssl_socket: MagicMock,
+    ) -> None:
+        # Arrange
+        assert not client.is_closed()
+        mock_tcp_socket.shutdown.side_effect = OSError()
+
+        # Act
+        client.close()
+
+        # Assert
+        assert client.is_closed()
+
+        mock_tcp_socket.shutdown.assert_called_once_with(SHUT_RDWR)
+        mock_ssl_socket.shutdown.assert_not_called()
+
+        mock_tcp_socket.close.assert_called_once_with()
+        mock_ssl_socket.close.assert_not_called()
+
     @pytest.mark.parametrize("client_closed", [False, True], ids=lambda p: f"client_closed=={p}")
     def test____get_local_address____return_saved_address(
         self,
         client: TCPNetworkClient[Any, Any],
         client_closed: bool,
         socket_family: int,
         local_address: tuple[str, int],
@@ -1226,15 +1307,15 @@
         mock_used_socket.send.assert_called_once_with(b"packet\n")
         mock_used_socket.getsockopt.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____receive_bytes_from_socket(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mock_selector_register: MagicMock,
         mock_selector_select: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
@@ -1250,20 +1331,20 @@
         mock_selector_register.assert_not_called()
         mock_selector_select.assert_not_called()
 
         mock_used_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
         mock_stream_data_consumer.feed.assert_called_once_with(b"packet\n")
         assert packet is mocker.sentinel.packet
 
-    @pytest.mark.parametrize("recv_timeout", [None, 123456789], indirect=True)  # Do not test with timeout==0
+    @pytest.mark.parametrize("recv_timeout", [None, float("+inf"), 123456789], indirect=True)  # Do not test with timeout==0
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking____partial_data(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"pac", b"ket\n"]
 
@@ -1287,15 +1368,15 @@
         indirect=True,
     )
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet_____non_blocking____partial_data(
         self,
         client: TCPNetworkClient[Any, Any],
         max_recv_size: int,
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"pac", b"ket", b"\n"]
 
@@ -1316,15 +1397,15 @@
         mock_used_socket.settimeout.assert_not_called()
         mock_used_socket.setblocking.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____extra_data(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"packet_1\npacket_2\n"]
 
@@ -1340,15 +1421,15 @@
         assert packet_1 is mocker.sentinel.packet_1
         assert packet_2 is mocker.sentinel.packet_2
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____eof_error____default(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b""]
 
         # Act
@@ -1361,15 +1442,15 @@
         mock_used_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
         mock_stream_data_consumer.feed.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____eof_error____convert_connection_errors(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = ConnectionError
 
         # Act
@@ -1384,15 +1465,15 @@
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     @pytest.mark.parametrize("closed_socket_errno", sorted(CLOSED_SOCKET_ERRNOS), ids=errno.errorcode.__getitem__)
     def test____recv_packet____blocking_or_not____eof_error____convert_closed_socket_errors(
         self,
         closed_socket_errno: int,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = OSError(closed_socket_errno, os.strerror(closed_socket_errno))
 
         # Act
@@ -1405,15 +1486,15 @@
         mock_used_socket.recv.assert_called_once_with(MAX_STREAM_BUFSIZE)
         mock_stream_data_consumer.feed.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____protocol_parse_error(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import StreamProtocolParseError
 
         mock_used_socket.recv.side_effect = [b"packet\n"]
@@ -1432,15 +1513,15 @@
         mock_stream_data_consumer.feed.assert_called_once_with(b"packet\n")
         assert exception is expected_error
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____recv_packet____blocking_or_not____closed_client_error(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_selector_register: MagicMock,
         mock_selector_select: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         client.close()
@@ -1461,15 +1542,15 @@
     @pytest.mark.usefixtures("setup_consumer_mock")
     @pytest.mark.parametrize("use_ssl", ["USE_SSL"], indirect=True)
     @pytest.mark.parametrize("ssl_eof_error", [SSLEOFError, SSLZeroReturnError])
     def test____recv_packet____blocking_or_not____ssl____eof_error(
         self,
         client: TCPNetworkClient[Any, Any],
         ssl_eof_error: Exception,
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = ssl_eof_error
 
         # Act
@@ -1568,15 +1649,15 @@
 
     @pytest.mark.parametrize("max_recv_size", [3], indirect=True)  # Needed for timeout==0
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____yields_available_packets_until_eof(
         self,
         client: TCPNetworkClient[Any, Any],
         max_recv_size: int,
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"pac", b"ket", b"_1\np", b"ack", b"et_", b"2\n", b""]
 
@@ -1597,15 +1678,15 @@
 
     @pytest.mark.parametrize("max_recv_size", [3], indirect=True)  # Needed for timeout==0
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____yields_available_packets_until_error(
         self,
         client: TCPNetworkClient[Any, Any],
         max_recv_size: int,
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"pac", b"ket", b"_1\np", b"ack", b"et_", b"2\n", OSError]
 
@@ -1624,15 +1705,15 @@
         ]
         assert packets == [mocker.sentinel.packet_1, mocker.sentinel.packet_2]
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____protocol_parse_error(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_stream_data_consumer: MagicMock,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import StreamProtocolParseError
 
         mock_stream_data_consumer.__next__.side_effect = StreamProtocolParseError(b"", "deserialization", "Sorry")
 
@@ -1646,15 +1727,15 @@
 
     @pytest.mark.parametrize("several_generators", [False, True], ids=lambda t: f"several_generators=={t}")
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____avoid_unnecessary_socket_recv_call(
         self,
         client: TCPNetworkClient[Any, Any],
         several_generators: bool,
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_stream_data_consumer: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"packet_1\npacket_2\n"]
 
@@ -1673,15 +1754,15 @@
         assert packet_1 is mocker.sentinel.packet_1
         assert packet_2 is mocker.sentinel.packet_2
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____release_internal_lock_before_yield(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from threading import Lock
 
         mock_acquire = mocker.patch.object(Lock, "acquire", return_value=True)
@@ -1703,15 +1784,15 @@
         assert packet_1 is mocker.sentinel.packet_1
         assert packet_2 is mocker.sentinel.packet_2
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____iter_received_packets____closed_client_during_iteration(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b"packet_1\n"]
 
         # Act & Assert
@@ -1748,15 +1829,15 @@
         mock_used_socket.settimeout.assert_not_called()
         mock_used_socket.send.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     def test____special_case____recv_packet____blocking_or_not____eof_error____do_not_try_socket_recv_on_next_call(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b""]
         with pytest.raises(ConnectionAbortedError):
             _ = client.recv_packet(timeout=recv_timeout)
 
@@ -1772,15 +1853,15 @@
         mock_used_socket.setblocking.assert_not_called()
 
     @pytest.mark.usefixtures("setup_consumer_mock")
     @pytest.mark.parametrize("use_ssl", ["USE_SSL"], indirect=True)
     def test____special_case____close____ssl____eof_error____do_not_try_to_unwrap(
         self,
         client: TCPNetworkClient[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_used_socket: MagicMock,
         mock_tcp_socket: MagicMock,
         mock_ssl_socket: MagicMock,
     ) -> None:
         # Arrange
         mock_used_socket.recv.side_effect = [b""]
         with pytest.raises(ConnectionAbortedError):
@@ -1790,14 +1871,14 @@
 
         # Act
         client.close()
 
         # Assert
         assert client.is_closed()
 
-        mock_tcp_socket.shutdown.assert_not_called()
-        mock_ssl_socket.shutdown.assert_not_called()
-
         mock_ssl_socket.unwrap.assert_not_called()
 
+        mock_tcp_socket.shutdown.assert_not_called()
+        mock_ssl_socket.shutdown.assert_called_once_with(SHUT_RDWR)
+
         mock_tcp_socket.close.assert_not_called()
         mock_ssl_socket.close.assert_called_once_with()
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_sync/test_client/test_udp.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_sync/test_client/test_udp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
+import errno
+import os
 from selectors import EVENT_READ, EVENT_WRITE
 from socket import AF_INET, AF_INET6, AF_UNSPEC, AI_PASSIVE, IPPROTO_UDP, SOCK_DGRAM, SOL_SOCKET
 from typing import TYPE_CHECKING, Any
 
 from easynetwork.api_sync.client.udp import UDPNetworkClient, UDPNetworkEndpoint
 from easynetwork.exceptions import ClientClosedError
-from easynetwork.tools.socket import MAX_DATAGRAM_BUFSIZE, IPv4SocketAddress, IPv6SocketAddress
+from easynetwork.tools.socket import CLOSED_SOCKET_ERRNOS, MAX_DATAGRAM_BUFSIZE, IPv4SocketAddress, IPv6SocketAddress
 
 import pytest
 
 if TYPE_CHECKING:
     from unittest.mock import MagicMock
 
     from pytest_mock import MockerFixture
@@ -104,31 +106,45 @@
         mock_datagram_protocol.build_packet_from_datagram.side_effect = build_packet_from_datagram_side_effect
 
     @pytest.fixture(params=["REMOTE_ADDRESS", "EXTERNAL_SOCKET"])
     @staticmethod
     def use_external_socket(request: Any) -> str:
         return request.param
 
+    @pytest.fixture
+    @staticmethod
+    def retry_interval(request: Any) -> float:
+        return getattr(request, "param", float("+inf"))
+
     @pytest.fixture()
     @staticmethod
     def client(
         use_external_socket: str,
         remote_address: tuple[str, int] | None,
+        retry_interval: float,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> UDPNetworkEndpoint[Any, Any]:
         try:
             match use_external_socket:
                 case "REMOTE_ADDRESS":
                     mocker.patch("socket.getaddrinfo", return_value=[(AF_INET, SOCK_DGRAM, IPPROTO_UDP, "", ("0.0.0.0", 0))])
                     mocker.patch("socket.socket", return_value=mock_udp_socket)
-                    return UDPNetworkEndpoint(protocol=mock_datagram_protocol, remote_address=remote_address)
+                    return UDPNetworkEndpoint(
+                        protocol=mock_datagram_protocol,
+                        remote_address=remote_address,
+                        retry_interval=retry_interval,
+                    )
                 case "EXTERNAL_SOCKET":
-                    return UDPNetworkEndpoint(socket=mock_udp_socket, protocol=mock_datagram_protocol)
+                    return UDPNetworkEndpoint(
+                        socket=mock_udp_socket,
+                        protocol=mock_datagram_protocol,
+                        retry_interval=retry_interval,
+                    )
                 case invalid:
                     pytest.fail(f"Invalid fixture param: Got {invalid!r}")
         finally:
             mock_udp_socket.settimeout.reset_mock()
 
     @pytest.fixture
     @staticmethod
@@ -140,15 +156,16 @@
         if param == "REMOTE":
             return global_remote_address
         host, port = param
         return host, port
 
     @pytest.fixture(
         params=[
-            pytest.param(None, id="blocking"),
+            pytest.param(None, id="blocking (None)"),
+            pytest.param(float("+inf"), id="blocking (+inf)"),
             pytest.param(0, id="non_blocking"),
             pytest.param(123456789, id="with_timeout"),
         ]
     )
     @staticmethod
     def recv_timeout(request: Any) -> Any:
         return request.param
@@ -407,14 +424,38 @@
 
         # Assert
         mock_socket_proxy_cls.assert_not_called()
         mock_tcp_socket.getsockname.assert_not_called()
         mock_tcp_socket.getpeername.assert_not_called()
         mock_tcp_socket.close.assert_called_once_with()
 
+    @pytest.mark.parametrize("retry_interval", [0, -12.34])
+    def test____dunder_init____retry_interval____invalid_value(
+        self,
+        retry_interval: float,
+        mock_udp_socket: MagicMock,
+        mock_socket_proxy_cls: MagicMock,
+        mock_datagram_protocol: MagicMock,
+    ) -> None:
+        # Arrange
+
+        # Act
+        with pytest.raises(ValueError, match=r"^retry_interval must be a strictly positive float or None$"):
+            _ = UDPNetworkEndpoint(
+                protocol=mock_datagram_protocol,
+                socket=mock_udp_socket,
+                retry_interval=retry_interval,
+            )
+
+        # Assert
+        mock_socket_proxy_cls.assert_not_called()
+        mock_udp_socket.getsockname.assert_not_called()
+        mock_udp_socket.getpeername.assert_not_called()
+        mock_udp_socket.close.assert_not_called()
+
     def test____context____close_endpoint_at_end(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_close = mocker.patch.object(UDPNetworkEndpoint, "close")
@@ -759,19 +800,54 @@
         mock_udp_socket.setblocking.assert_not_called()
         mock_selector_select.assert_not_called()
         mock_udp_socket.sendto.assert_not_called()
         mock_datagram_protocol.make_datagram.assert_not_called()
         mock_udp_socket.getsockopt.assert_not_called()
 
     @pytest.mark.usefixtures("setup_protocol_mock")
+    @pytest.mark.parametrize("closed_socket_errno", sorted(CLOSED_SOCKET_ERRNOS), ids=errno.errorcode.__getitem__)
+    def test____send_packet_to____convert_closed_socket_errors(
+        self,
+        closed_socket_errno: int,
+        client: UDPNetworkEndpoint[Any, Any],
+        global_remote_address: tuple[str, int],
+        mock_udp_socket: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
+        mocker: MockerFixture,
+    ) -> None:
+        # Arrange
+        if client.get_remote_address() is not None:
+            mock_udp_socket.send.side_effect = OSError(closed_socket_errno, os.strerror(closed_socket_errno))
+        else:
+            mock_udp_socket.sendto.side_effect = OSError(closed_socket_errno, os.strerror(closed_socket_errno))
+
+        # Act
+        with pytest.raises(ConnectionAbortedError):
+            client.send_packet_to(mocker.sentinel.packet, global_remote_address)
+
+        # Assert
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_select.assert_not_called()
+        if client.get_remote_address() is not None:
+            mock_udp_socket.sendto.assert_not_called()
+            mock_udp_socket.send.assert_called_once()
+        else:
+            mock_udp_socket.sendto.assert_called_once()
+            mock_udp_socket.send.assert_not_called()
+        mock_datagram_protocol.make_datagram.assert_called_once_with(mocker.sentinel.packet)
+        mock_udp_socket.getsockopt.assert_not_called()
+
+    @pytest.mark.usefixtures("setup_protocol_mock")
     def test____recv_packet_from____blocking_or_not____receive_bytes_from_socket(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mock_selector_register: MagicMock,
         mock_selector_select: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
@@ -793,15 +869,15 @@
         assert (sender.host, sender.port) == sender_address
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____recv_packet_from____blocking_or_not____protocol_parse_error(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import DatagramProtocolParseError
 
         mock_udp_socket.recvfrom.side_effect = [(b"packet", sender_address)]
@@ -818,15 +894,15 @@
         mock_datagram_protocol.build_packet_from_datagram.assert_called_once_with(b"packet")
         assert exception is expected_error
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____recv_packet_from____blocking_or_not____closed_client_error(
         self,
         client: UDPNetworkEndpoint[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mock_selector_register: MagicMock,
         mock_selector_select: MagicMock,
         mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
         client.close()
@@ -840,14 +916,41 @@
         mock_udp_socket.settimeout.assert_not_called()
         mock_udp_socket.setblocking.assert_not_called()
         mock_selector_register.assert_not_called()
         mock_selector_select.assert_not_called()
         mock_udp_socket.recvfrom.assert_not_called()
         mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
 
+    @pytest.mark.usefixtures("setup_protocol_mock")
+    @pytest.mark.parametrize("closed_socket_errno", sorted(CLOSED_SOCKET_ERRNOS), ids=errno.errorcode.__getitem__)
+    def test____recv_packet_from____blocking_or_not____convert_closed_socket_errors(
+        self,
+        closed_socket_errno: int,
+        client: UDPNetworkEndpoint[Any, Any],
+        recv_timeout: float | None,
+        mock_udp_socket: MagicMock,
+        mock_selector_register: MagicMock,
+        mock_selector_select: MagicMock,
+        mock_datagram_protocol: MagicMock,
+    ) -> None:
+        # Arrange
+        mock_udp_socket.recvfrom.side_effect = OSError(closed_socket_errno, os.strerror(closed_socket_errno))
+
+        # Act
+        with pytest.raises(ConnectionAbortedError):
+            _ = client.recv_packet_from(timeout=recv_timeout)
+
+        # Assert
+        mock_udp_socket.settimeout.assert_not_called()
+        mock_udp_socket.setblocking.assert_not_called()
+        mock_selector_register.assert_not_called()
+        mock_selector_select.assert_not_called()
+        mock_udp_socket.recvfrom.assert_called_once_with(MAX_DATAGRAM_BUFSIZE)
+        mock_datagram_protocol.build_packet_from_datagram.assert_not_called()
+
     @pytest.mark.parametrize(
         "recv_timeout",
         [
             pytest.param(0, id="null timeout"),
             pytest.param(123456789, id="strictly positive timeout"),
         ],
     )
@@ -921,15 +1024,15 @@
         ]
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____iter_received_packets_from____yields_available_packets_until_error(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_udp_socket.recvfrom.side_effect = [
             (b"packet_1", sender_address),
@@ -951,15 +1054,15 @@
             (mocker.sentinel.packet_2, sender_address),
         ]
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____iter_received_packets_from____protocol_parse_error(
         self,
         client: UDPNetworkEndpoint[Any, Any],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         sender_address: tuple[str, int],
         mock_udp_socket: MagicMock,
         mock_datagram_protocol: MagicMock,
     ) -> None:
         # Arrange
         from easynetwork.exceptions import DatagramProtocolParseError
 
@@ -978,15 +1081,15 @@
         assert exception is expected_error
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____iter_received_packets_from____release_internal_lock_before_yield(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         from threading import Lock
 
         mock_acquire = mocker.patch.object(Lock, "acquire", return_value=True)
@@ -1009,15 +1112,15 @@
         assert packet_2[0] is mocker.sentinel.packet_2
 
     @pytest.mark.usefixtures("setup_protocol_mock")
     def test____iter_received_packets_from____closed_client_during_iteration(
         self,
         client: UDPNetworkEndpoint[Any, Any],
         sender_address: tuple[str, int],
-        recv_timeout: int | None,
+        recv_timeout: float | None,
         mock_udp_socket: MagicMock,
         mocker: MockerFixture,
     ) -> None:
         # Arrange
         mock_udp_socket.recvfrom.side_effect = [(b"packet_1", sender_address)]
 
         # Act & Assert
@@ -1069,22 +1172,24 @@
 
         # Act
         client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
             remote_address,
             mock_datagram_protocol,
             local_address=mocker.sentinel.local_address,
             reuse_port=mocker.sentinel.reuse_port,
+            retry_interval=mocker.sentinel.retry_interval,
         )
 
         # Assert
         mock_udp_endpoint_cls.assert_called_once_with(
             protocol=mock_datagram_protocol,
             remote_address=remote_address,
             local_address=mocker.sentinel.local_address,
             reuse_port=mocker.sentinel.reuse_port,
+            retry_interval=mocker.sentinel.retry_interval,
         )
         mock_udp_endpoint.get_remote_address.assert_called_once_with()
         assert client.socket is mock_udp_socket
 
     def test____dunder_init____with_socket(
         self,
         mock_udp_socket: MagicMock,
@@ -1095,20 +1200,22 @@
     ) -> None:
         # Arrange
 
         # Act
         client: UDPNetworkClient[Any, Any] = UDPNetworkClient(
             mock_udp_socket,
             mock_datagram_protocol,
+            retry_interval=mocker.sentinel.retry_interval,
         )
 
         # Assert
         mock_udp_endpoint_cls.assert_called_once_with(
             protocol=mock_datagram_protocol,
             socket=mock_udp_socket,
+            retry_interval=mocker.sentinel.retry_interval,
         )
         mock_udp_endpoint.get_remote_address.assert_called_once_with()
         assert client.socket is mock_udp_socket
 
     def test____dunder_init____error_no_remote_address(
         self,
         mock_udp_socket: MagicMock,
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_lock.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_lock.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_socket.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_socket.py`

 * *Files 10% similar despite different names*

```diff
@@ -131,27 +131,39 @@
             runner_stub.assert_called_once_with(mock_tcp_socket.fileno)
 
     def test____dup____sub_call(
         self,
         mock_tcp_socket: MagicMock,
         mocker: MockerFixture,
         runner_stub: MagicMock | None,
+        mock_tcp_socket_factory: Callable[[], MagicMock],
     ) -> None:
         # Arrange
-        mock_tcp_socket.dup.return_value = mocker.sentinel.dup_socket
+        mock_tcp_socket.fileno.return_value = mocker.sentinel.fd
+        mock_new_socket = mock_tcp_socket_factory()
+        mock_socket_fromfd = mocker.patch("socket.fromfd", autospec=True, return_value=mock_new_socket)
         socket_proxy = SocketProxy(mock_tcp_socket, runner=runner_stub)
 
         # Act
         socket = socket_proxy.dup()
 
         # Assert
-        mock_tcp_socket.dup.assert_called_once_with()
-        assert socket is mocker.sentinel.dup_socket
+        mock_tcp_socket.dup.assert_not_called()
+        mock_tcp_socket.fileno.assert_called_once_with()
+        mock_socket_fromfd.assert_called_once_with(
+            mocker.sentinel.fd,
+            mock_tcp_socket.family,
+            mock_tcp_socket.type,
+            mock_tcp_socket.proto,
+        )
+        mock_new_socket.setblocking.assert_called_once_with(False)
+        mock_new_socket.settimeout.assert_not_called()
+        assert socket is mock_new_socket
         if runner_stub is not None:
-            runner_stub.assert_called_once_with(mock_tcp_socket.dup)
+            runner_stub.assert_called_once_with(mock_tcp_socket.fileno)
 
     def test____get_inheritable____sub_call(
         self,
         mock_tcp_socket: MagicMock,
         mocker: MockerFixture,
         runner_stub: MagicMock | None,
     ) -> None:
```

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_stream.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_stream.py`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/tests/unit_test/test_tools/test_utils.py` & `easynetwork-1.0.0rc4/tests/unit_test/test_tools/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import os
 import selectors
+import ssl
 from socket import (
     AF_INET,
     AF_INET6,
     IPPROTO_IPV6,
     IPPROTO_TCP,
     IPV6_V6ONLY,
     SO_ERROR,
@@ -24,14 +25,15 @@
     check_socket_family,
     check_socket_no_ssl,
     concatenate_chunks,
     ensure_datagram_socket_bound,
     error_from_errno,
     is_ssl_eof_error,
     is_ssl_socket,
+    iter_bytes,
     open_listener_sockets_from_getaddrinfo_result,
     recursively_clear_exception_traceback_frames,
     replace_kwargs,
     set_reuseport,
     set_tcp_keepalive,
     set_tcp_nodelay,
     transform_future_exception,
@@ -189,14 +191,22 @@
 def test____is_ssl_socket____ssl_socket(mock_ssl_socket: MagicMock) -> None:
     # Arrange
 
     # Act & Assert
     assert is_ssl_socket(mock_ssl_socket)
 
 
+@pytest.mark.usefixtures("simulate_no_ssl_module")
+def test____is_ssl_socket____no_ssl_module(mock_ssl_socket: MagicMock) -> None:
+    # Arrange
+
+    # Act & Assert
+    assert not is_ssl_socket(mock_ssl_socket)
+
+
 def test____check_socket_no_ssl____regular_socket(mock_socket_factory: Callable[[], MagicMock]) -> None:
     # Arrange
     mock_socket = mock_socket_factory()
 
     # Act & Assert
     check_socket_no_ssl(mock_socket)
 
@@ -207,35 +217,41 @@
     # Act & Assert
     with pytest.raises(TypeError, match=r"^ssl\.SSLSocket instances are forbidden$"):
         check_socket_no_ssl(mock_ssl_socket)
 
 
 def test____is_ssl_eof_error____SSLEOFError() -> None:
     # Arrange
-    import ssl
 
     # Act & Assert
     assert is_ssl_eof_error(ssl.SSLEOFError())
 
 
 def test____is_ssl_eof_error____SSLError_with_specific_mnemonic() -> None:
     # Arrange
-    import ssl
 
     # Act & Assert
     assert is_ssl_eof_error(ssl.SSLError(ssl.SSL_ERROR_SSL, "UNEXPECTED_EOF_WHILE_READING"))
 
 
 def test____is_ssl_eof_error____OSError() -> None:
     # Arrange
 
     # Act & Assert
     assert not is_ssl_eof_error(OSError())
 
 
+@pytest.mark.usefixtures("simulate_no_ssl_module")
+def test____is_ssl_eof_error____no_ssl_module() -> None:
+    # Arrange
+
+    # Act & Assert
+    assert not is_ssl_eof_error(ssl.SSLEOFError())
+
+
 @pytest.mark.parametrize(["event", "selector_event"], [("read", "EVENT_READ"), ("write", "EVENT_WRITE")])
 @pytest.mark.parametrize("timeout", [10.2, 0, None], ids=lambda value: f"timeout=={value}")
 @pytest.mark.parametrize("available", [True, False], ids=lambda value: f"available=={value}")
 @pytest.mark.parametrize("use_PollSelector", [True, False], ids=lambda value: f"use_PollSelector=={value}")
 def test____wait_socket_available____returns_boolean_if_available_or_not(
     mock_socket_factory: Callable[[], MagicMock],
     event: Literal["read", "write"],
@@ -339,14 +355,26 @@
     # Act
     result = concatenate_chunks(to_join)
 
     # Assert
     assert result == expected_result
 
 
+def test____iter_bytes____iterate_over_bytes_returning_one_byte() -> None:
+    # Arrange
+    to_split = b"abcd"
+    expected_result = [b"a", b"b", b"c", b"d"]
+
+    # Act
+    result = list(iter_bytes(to_split))
+
+    # Assert
+    assert result == expected_result
+
+
 def test____ensure_datagram_socket_bound____socket_not_bound____null_port(
     mock_udp_socket: MagicMock,
 ) -> None:
     # Arrange
     mock_udp_socket.getsockname.return_value = ("0.0.0.0", 0)
 
     # Act
```

### Comparing `easynetwork-1.0.0rc3/.gitignore` & `easynetwork-1.0.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/LICENSE` & `easynetwork-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `easynetwork-1.0.0rc3/pyproject.toml` & `easynetwork-1.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 classifiers = [
     "Development Status :: 4 - Beta",
+    "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
```

### Comparing `easynetwork-1.0.0rc3/PKG-INFO` & `easynetwork-1.0.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: easynetwork
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: The easiest way to use sockets in Python
 Project-URL: Homepage, https://github.com/francis-clairicia/EasyNetwork
 Author-email: FrankySnow9 <clairicia.rcj.francis@gmail.com>
 License-File: LICENSE
 Keywords: async,asynchronous,client,communication,networking,serialization,server,socket
 Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
```

