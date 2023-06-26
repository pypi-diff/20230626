# Comparing `tmp/chaotic-ngine-0.9.0.tar.gz` & `tmp/chaotic-ngine-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaotic-ngine-0.9.0.tar", last modified: Fri Jan 20 17:13:40 2023, max compression
+gzip compressed data, was "chaotic-ngine-0.9.1.tar", last modified: Wed May  3 08:02:39 2023, max compression
```

## Comparing `chaotic-ngine-0.9.0.tar` & `chaotic-ngine-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:13:40.280352 chaotic-ngine-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-01-20 17:13:40.280352 chaotic-ngine-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:13:40.280352 chaotic-ngine-0.9.0/chaotic/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:13:40.280352 chaotic-ngine-0.9.0/chaotic/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/cloudscale_ch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/cloudstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/exoscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/hcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/nomad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/proxmox_kvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/cloud/vultr.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/chaotic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:13:40.280352 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-20 17:13:40.000000 chaotic-ngine-0.9.0/chaotic_ngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 17:13:40.284353 chaotic-ngine-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-20 17:13:29.000000 chaotic-ngine-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:02:39.164390 chaotic-ngine-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-03 08:02:39.164390 chaotic-ngine-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:02:39.160390 chaotic-ngine-0.9.1/chaotic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:02:39.164390 chaotic-ngine-0.9.1/chaotic/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/cloudscale_ch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/cloudstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/exoscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/hcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/nomad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/proxmox_kvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/cloud/vultr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/chaotic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:02:39.164390 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 08:02:39.000000 chaotic-ngine-0.9.1/chaotic_ngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:02:39.164390 chaotic-ngine-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-03 08:02:23.000000 chaotic-ngine-0.9.1/setup.py
```

### Comparing `chaotic-ngine-0.9.0/LICENSE` & `chaotic-ngine-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/PKG-INFO` & `chaotic-ngine-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaotic-ngine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Chaos for Clouds.
 Home-page: https://github.com/ngine-io/chaotic
 Author: René Moser
 Author-email: mail@renemoser.net
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -333,19 +333,34 @@
 
   # Optional: 60 seconds is the default
   wait_before_restart: 60
 ```
 
 ## Run
 
+### CLI
 ```
 chaos-ngine
 ```
+### Docker 
+
+One shot:
+
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest
+```
+
+As service:
 
-What you should see (cloudscale.ch):
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest --periodic
+```
+
+## Logs
+What you should see (e.g. for kind cloudscale.ch):
 ```
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Started, version: 0.6.2
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Using profile default
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:API Token used: xyz...
 2021-06-09 09:01:25,433 - chatic:INFO:Querying with filter_tag: None
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:HTTP GET to https://api.cloudscale.ch/v1/servers
 2021-06-09 09:01:25,651 - cloudscale.log:INFO:HTTP status code 200
@@ -354,11 +369,7 @@
 2021-06-09 09:01:25,653 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/stop
 2021-06-09 09:01:26,336 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:01:26,336 - chatic:INFO:Sleeping for server 60
 2021-06-09 09:02:26,393 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/start
 2021-06-09 09:02:26,955 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:02:26,956 - chatic:INFO:done
 ```
-
-## Docker / Nomad run
-
-See https://gitlab.com/ngine/docker-images/chaotic
```

### Comparing `chaotic-ngine-0.9.0/README.md` & `chaotic-ngine-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -314,19 +314,34 @@
 
   # Optional: 60 seconds is the default
   wait_before_restart: 60
 ```
 
 ## Run
 
+### CLI
 ```
 chaos-ngine
 ```
+### Docker 
+
+One shot:
+
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest
+```
+
+As service:
 
-What you should see (cloudscale.ch):
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest --periodic
+```
+
+## Logs
+What you should see (e.g. for kind cloudscale.ch):
 ```
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Started, version: 0.6.2
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Using profile default
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:API Token used: xyz...
 2021-06-09 09:01:25,433 - chatic:INFO:Querying with filter_tag: None
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:HTTP GET to https://api.cloudscale.ch/v1/servers
 2021-06-09 09:01:25,651 - cloudscale.log:INFO:HTTP status code 200
@@ -335,11 +350,7 @@
 2021-06-09 09:01:25,653 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/stop
 2021-06-09 09:01:26,336 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:01:26,336 - chatic:INFO:Sleeping for server 60
 2021-06-09 09:02:26,393 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/start
 2021-06-09 09:02:26,955 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:02:26,956 - chatic:INFO:done
 ```
-
-## Docker / Nomad run
-
-See https://gitlab.com/ngine/docker-images/chaotic
```

### Comparing `chaotic-ngine-0.9.0/chaotic/__init__.py` & `chaotic-ngine-0.9.1/chaotic/__init__.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/app.py` & `chaotic-ngine-0.9.1/chaotic/app.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/__init__.py` & `chaotic-ngine-0.9.1/chaotic/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/cloudscale_ch.py` & `chaotic-ngine-0.9.1/chaotic/cloud/cloudscale_ch.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/cloudstack.py` & `chaotic-ngine-0.9.1/chaotic/cloud/cloudstack.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/digitalocean.py` & `chaotic-ngine-0.9.1/chaotic/cloud/digitalocean.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/exoscale.py` & `chaotic-ngine-0.9.1/chaotic/cloud/exoscale.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/hcloud.py` & `chaotic-ngine-0.9.1/chaotic/cloud/hcloud.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/nomad.py` & `chaotic-ngine-0.9.1/chaotic/cloud/nomad.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/proxmox_kvm.py` & `chaotic-ngine-0.9.1/chaotic/cloud/proxmox_kvm.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/cloud/vultr.py` & `chaotic-ngine-0.9.1/chaotic/cloud/vultr.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic/log.py` & `chaotic-ngine-0.9.1/chaotic/log.py`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/chaotic_ngine.egg-info/PKG-INFO` & `chaotic-ngine-0.9.1/chaotic_ngine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaotic-ngine
-Version: 0.9.0
+Version: 0.9.1
 Summary: Chaos for Clouds.
 Home-page: https://github.com/ngine-io/chaotic
 Author: René Moser
 Author-email: mail@renemoser.net
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -333,19 +333,34 @@
 
   # Optional: 60 seconds is the default
   wait_before_restart: 60
 ```
 
 ## Run
 
+### CLI
 ```
 chaos-ngine
 ```
+### Docker 
+
+One shot:
+
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest
+```
+
+As service:
 
-What you should see (cloudscale.ch):
+```
+docker run -ti --rm -v $PWD/examples/config_nomad.yaml:/app/config.yaml -e TZ=Europe/Zurich -e NOMAD_ADDR=$NOMAD_ADDR --name chaotic ghcr.io/ngine-io/chaotic:latest --periodic
+```
+
+## Logs
+What you should see (e.g. for kind cloudscale.ch):
 ```
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Started, version: 0.6.2
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:Using profile default
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:API Token used: xyz...
 2021-06-09 09:01:25,433 - chatic:INFO:Querying with filter_tag: None
 2021-06-09 09:01:25,433 - cloudscale.log:INFO:HTTP GET to https://api.cloudscale.ch/v1/servers
 2021-06-09 09:01:25,651 - cloudscale.log:INFO:HTTP status code 200
@@ -354,11 +369,7 @@
 2021-06-09 09:01:25,653 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/stop
 2021-06-09 09:01:26,336 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:01:26,336 - chatic:INFO:Sleeping for server 60
 2021-06-09 09:02:26,393 - cloudscale.log:INFO:HTTP POST to https://api.cloudscale.ch/v1/servers/d5628484-a6eb-4ea9-b3ef-ba8da2bb9fe0/start
 2021-06-09 09:02:26,955 - cloudscale.log:INFO:HTTP status code 204
 2021-06-09 09:02:26,956 - chatic:INFO:done
 ```
-
-## Docker / Nomad run
-
-See https://gitlab.com/ngine/docker-images/chaotic
```

### Comparing `chaotic-ngine-0.9.0/chaotic_ngine.egg-info/SOURCES.txt` & `chaotic-ngine-0.9.1/chaotic_ngine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaotic-ngine-0.9.0/setup.py` & `chaotic-ngine-0.9.1/setup.py`

 * *Files identical despite different names*

