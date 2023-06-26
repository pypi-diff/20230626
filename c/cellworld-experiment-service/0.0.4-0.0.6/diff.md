# Comparing `tmp/cellworld_experiment_service-0.0.4.tar.gz` & `tmp/cellworld_experiment_service-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_experiment_service-0.0.4.tar", last modified: Fri Jan 21 18:15:19 2022, max compression
+gzip compressed data, was "cellworld_experiment_service-0.0.6.tar", last modified: Fri Jan 21 19:59:19 2022, max compression
```

## Comparing `cellworld_experiment_service-0.0.4.tar` & `cellworld_experiment_service-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 18:15:19.041139 cellworld_experiment_service-0.0.4/
--rwxrwxrwx   0 german    (1000) german    (1000)      223 2022-01-21 18:15:19.039130 cellworld_experiment_service-0.0.4/PKG-INFO
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 18:15:18.968517 cellworld_experiment_service-0.0.4/cellworld_experiment_service/
--rwxrwxrwx   0 german    (1000) german    (1000)      136 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service/__init__.py
--rwxrwxrwx   0 german    (1000) german    (1000)     3117 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_client.py
--rwxrwxrwx   0 german    (1000) german    (1000)     1936 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_messages.py
--rwxrwxrwx   0 german    (1000) german    (1000)     6247 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_service.py
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 18:15:19.028130 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/
--rwxrwxrwx   0 german    (1000) german    (1000)      223 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/PKG-INFO
--rwxrwxrwx   0 german    (1000) german    (1000)      512 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/SOURCES.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/dependency_links.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/not-zip-safe
--rwxrwxrwx   0 german    (1000) german    (1000)       23 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/requires.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       29 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/top_level.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-01-21 18:15:19.041139 cellworld_experiment_service-0.0.4/setup.cfg
--rwxrwxrwx   0 german    (1000) german    (1000)      305 2022-01-21 18:15:18.000000 cellworld_experiment_service-0.0.4/setup.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 19:59:19.095882 cellworld_experiment_service-0.0.6/
+-rwxrwxrwx   0 german    (1000) german    (1000)      223 2022-01-21 19:59:19.093881 cellworld_experiment_service-0.0.6/PKG-INFO
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 19:59:19.021881 cellworld_experiment_service-0.0.6/cellworld_experiment_service/
+-rwxrwxrwx   0 german    (1000) german    (1000)      136 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service/__init__.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     3265 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_client.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     1936 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_messages.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     6361 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_service.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-21 19:59:19.082881 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/
+-rwxrwxrwx   0 german    (1000) german    (1000)      223 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/PKG-INFO
+-rwxrwxrwx   0 german    (1000) german    (1000)      512 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/SOURCES.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/dependency_links.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/not-zip-safe
+-rwxrwxrwx   0 german    (1000) german    (1000)       23 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/requires.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       29 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/top_level.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-01-21 19:59:19.095882 cellworld_experiment_service-0.0.6/setup.cfg
+-rwxrwxrwx   0 german    (1000) german    (1000)      305 2022-01-21 19:59:18.000000 cellworld_experiment_service-0.0.6/setup.py
```

### Comparing `cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_client.py` & `cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
     def start_episode(self, experiment_name: str) -> str:
         return self.send_request(Message("start_episode", StartEpisodeRequest(experiment_name=experiment_name)), 5000).get_body(bool)
 
     def finish_episode(self) -> str:
         return self.send_request(Message("finish_episode"), 5000).get_body(bool)
 
+    def set_tracking_service_ip(self, ip) -> str:
+        return self.send_request(Message("set_tracking_service_ip", ip), 5000).get_body(bool)
+
     def finish_experiment(self, experiment_name: str):
         return self.send_request(Message("finish_experiment", FinishExperimentRequest(experiment_name=experiment_name)), 5000).get_body(bool)
 
     def get_experiment(self, experiment_name: str) -> GetExperimentResponse:
         return self.send_request(Message("get_experiment", GetExperimentRequest(experiment_name=experiment_name)), 5000).get_body(GetExperimentResponse)
 
     def is_active(self, experiment_name: str) -> bool:
```

### Comparing `cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_messages.py` & `cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_messages.py`

 * *Files identical despite different names*

### Comparing `cellworld_experiment_service-0.0.4/cellworld_experiment_service/experiment_service.py` & `cellworld_experiment_service-0.0.6/cellworld_experiment_service/experiment_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime, timedelta
 
 
 class ExperimentService(MessageServer):
     def __init__(self, tracker_ip: str = "127.0.0.1"):
         MessageServer.__init__(self)
         self.tracking_service = None
+        self.router.add_route("set_tracking_service_ip", self.set_tracking_service_ip, str)
         self.router.add_route("start_experiment", self.start_experiment, StartExperimentRequest)
         self.router.add_route("start_episode", self.start_episode, StartEpisodeRequest)
         self.router.add_route("finish_episode", self.finish_episode)
         self.router.add_route("finish_experiment", self.finish_experiment, FinishExperimentRequest)
         self.router.add_route("get_experiment", self.get_experiment, GetExperimentRequest)
         self.allow_subscription = True
         self.active_experiment = None
@@ -120,14 +121,15 @@
             response.start_date = experiment.start_time
             response.duration = experiment.duration
             response.remaining_time = remaining
         return response
 
     def set_tracking_service_ip(self, ip: str):
         self.tracking_service_ip = ip
+        return True
 
     @staticmethod
     def port() -> int:
         default_port = 4540
         if os.environ.get("CELLWORLD_EXPERIMENT_SERVICE_PORT"):
             try:
                 return int(os.environ.get("CELLWORLD_EXPERIMENT_SERVICE_PORT"))
```

### Comparing `cellworld_experiment_service-0.0.4/cellworld_experiment_service.egg-info/SOURCES.txt` & `cellworld_experiment_service-0.0.6/cellworld_experiment_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

