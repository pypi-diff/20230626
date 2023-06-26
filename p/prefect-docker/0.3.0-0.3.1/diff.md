# Comparing `tmp/prefect-docker-0.3.0.tar.gz` & `tmp/prefect-docker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-q5zy82mj/prefect-docker-0.3.0.tar", last modified: Thu Jun 15 14:32:04 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-0nw3a3ow/prefect-docker-0.3.1.tar", last modified: Mon Jun 26 14:27:49 2023, max compression
```

## Comparing `prefect-docker-0.3.0.tar` & `prefect-docker-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    29217 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:32:04.000000 prefect-docker-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:30:34.000000 prefect-docker-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29217 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/versioneer.py
```

### Comparing `prefect-docker-0.3.0/LICENSE` & `prefect-docker-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/PKG-INFO` & `prefect-docker-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.3.0
+Version: 0.3.1
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.3.0/README.md` & `prefect-docker-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker/containers.py` & `prefect-docker-0.3.1/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker/credentials.py` & `prefect-docker-0.3.1/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker/deployments/steps.py` & `prefect-docker-0.3.1/prefect_docker/deployments/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,17 @@
         lines.append(f"FROM {base_image}")
         dir_name = os.path.basename(os.getcwd())
 
         if Path("requirements.txt").exists():
             lines.append(
                 f"COPY requirements.txt /opt/prefect/{dir_name}/requirements.txt"
             )
-            lines.append("RUN python -m pip install -r requirements.txt")
+            lines.append(
+                f"RUN python -m pip install -r /opt/prefect/{dir_name}/requirements.txt"
+            )
 
         lines.append(f"COPY . /opt/prefect/{dir_name}/")
         lines.append(f"WORKDIR /opt/prefect/{dir_name}/")
 
         temp_dockerfile = Path("Dockerfile")
         if Path(temp_dockerfile).exists():
             raise ValueError("Dockerfile already exists.")
```

### Comparing `prefect-docker-0.3.0/prefect_docker/host.py` & `prefect-docker-0.3.1/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker/images.py` & `prefect-docker-0.3.1/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker/worker.py` & `prefect-docker-0.3.1/prefect_docker/worker.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/prefect_docker.egg-info/PKG-INFO` & `prefect-docker-0.3.1/prefect_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.3.0
+Version: 0.3.1
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.3.0/prefect_docker.egg-info/SOURCES.txt` & `prefect-docker-0.3.1/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/setup.cfg` & `prefect-docker-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/setup.py` & `prefect-docker-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/tests/test_containers.py` & `prefect-docker-0.3.1/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/tests/test_host.py` & `prefect-docker-0.3.1/tests/test_host.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from unittest.mock import MagicMock
 
 import pytest
 from prefect.logging import disable_run_logger
 
-from prefect_docker.host import DockerHost, _ContextManageableDockerClient
+from prefect_docker.host import DockerHost
+
+
+@pytest.fixture
+def mock_ctx_docker_client(mock_docker_client, monkeypatch) -> MagicMock:
+    monkeypatch.setattr(
+        "prefect_docker.host._ContextManageableDockerClient", mock_docker_client
+    )
+    return mock_docker_client
 
 
 class TestDockerHost:
     @pytest.fixture
     def host_kwargs(self):
         _host_kwargs = dict(
             base_url="unix:///var/run/docker.sock",
@@ -29,32 +37,30 @@
     def docker_host_from_env(self, host_kwargs):
         host_kwargs.pop("base_url")
         _docker_host = DockerHost(**host_kwargs)
         for key, val in host_kwargs.items():
             assert getattr(_docker_host, key) == val
         return _docker_host
 
-    def test_get_client(self, docker_host, mock_docker_client_new: MagicMock):
+    def test_get_client(self, docker_host, mock_ctx_docker_client: MagicMock):
         with disable_run_logger():
             docker_host.get_client()
-            mock_docker_client_new.assert_called_once_with(
-                _ContextManageableDockerClient,
+            mock_ctx_docker_client.assert_called_once_with(
                 base_url="unix:///var/run/docker.sock",
                 version="1.35",
                 max_pool_size=8,
                 tls=True,
             )
 
     def test_context_managed_get_client(
-        self, docker_host, mock_docker_client_new: MagicMock
+        self, docker_host, mock_ctx_docker_client: MagicMock
     ):
         with disable_run_logger():
             with docker_host.get_client() as _:
-                mock_docker_client_new.assert_called_once_with(
-                    _ContextManageableDockerClient,
+                mock_ctx_docker_client.assert_called_once_with(
                     base_url="unix:///var/run/docker.sock",
                     version="1.35",
                     max_pool_size=8,
                     tls=True,
                 )
 
     def test_get_client_from_env(
```

### Comparing `prefect-docker-0.3.0/tests/test_images.py` & `prefect-docker-0.3.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/tests/test_worker.py` & `prefect-docker-0.3.1/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.0/versioneer.py` & `prefect-docker-0.3.1/versioneer.py`

 * *Files identical despite different names*

