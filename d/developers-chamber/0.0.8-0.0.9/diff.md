# Comparing `tmp/developers-chamber-0.0.8.tar.gz` & `tmp/developers-chamber-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/developers-chamber-0.0.8.tar", last modified: Fri Sep  6 12:29:29 2019, max compression
+gzip compressed data, was "dist/developers-chamber-0.0.9.tar", last modified: Fri Sep  6 12:44:55 2019, max compression
```

## Comparing `developers-chamber-0.0.8.tar` & `developers-chamber-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1239 2019-08-26 20:44:37.000000 developers-chamber-0.0.8/README.md
--rw-r--r--   0 lubos     (1000) lubos     (1000)      348 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/PKG-INFO
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber/
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber/django/
--rw-r--r--   0 lubos     (1000) lubos     (1000)      425 2019-09-05 21:36:36.000000 developers-chamber-0.0.8/developers_chamber/django/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      182 2019-09-05 21:36:36.000000 developers-chamber-0.0.8/developers_chamber/django/context_processors.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     3491 2019-08-29 20:03:15.000000 developers-chamber-0.0.8/developers_chamber/version_utils.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)    10463 2019-09-06 12:28:03.000000 developers-chamber-0.0.8/developers_chamber/ecs_utils.py
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber/click/
--rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-09-05 19:23:56.000000 developers-chamber-0.0.8/developers_chamber/click/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      879 2019-09-05 19:23:56.000000 developers-chamber-0.0.8/developers_chamber/click/options.py
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber/scripts/
--rw-r--r--   0 lubos     (1000) lubos     (1000)     7780 2019-09-06 12:28:03.000000 developers-chamber-0.0.8/developers_chamber/scripts/ecs.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1746 2019-08-30 08:02:58.000000 developers-chamber-0.0.8/developers_chamber/scripts/version.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)       50 2019-08-26 20:44:37.000000 developers-chamber-0.0.8/developers_chamber/scripts/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     4311 2019-08-30 08:02:58.000000 developers-chamber-0.0.8/developers_chamber/scripts/git.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1454 2019-09-05 21:36:36.000000 developers-chamber-0.0.8/developers_chamber/scripts/docker.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1748 2019-08-30 08:02:58.000000 developers-chamber-0.0.8/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-08-26 20:44:37.000000 developers-chamber-0.0.8/developers_chamber/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1235 2019-09-05 19:23:56.000000 developers-chamber-0.0.8/developers_chamber/docker_utils.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      438 2019-08-26 20:44:37.000000 developers-chamber-0.0.8/developers_chamber/types.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      981 2019-08-29 20:03:15.000000 developers-chamber-0.0.8/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber/bin/
--rw-r--r--   0 lubos     (1000) lubos     (1000)      894 2019-09-05 19:23:56.000000 developers-chamber-0.0.8/developers_chamber/bin/pydev.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-08-26 20:44:37.000000 developers-chamber-0.0.8/developers_chamber/bin/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     3744 2019-09-06 09:05:27.000000 developers-chamber-0.0.8/developers_chamber/git_utils.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      800 2019-09-06 12:28:35.000000 developers-chamber-0.0.8/setup.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)       38 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/setup.cfg
-drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/
--rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)      348 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 lubos     (1000) lubos     (1000)       73 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/requires.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2019-08-30 08:04:32.000000 developers-chamber-0.0.8/developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 lubos     (1000) lubos     (1000)      993 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)       60 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)       19 2019-09-06 12:29:29.000000 developers-chamber-0.0.8/developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1239 2019-08-26 20:44:37.000000 developers-chamber-0.0.9/README.md
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      348 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/PKG-INFO
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber/
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber/django/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      425 2019-09-05 21:36:36.000000 developers-chamber-0.0.9/developers_chamber/django/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      182 2019-09-05 21:36:36.000000 developers-chamber-0.0.9/developers_chamber/django/context_processors.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     3491 2019-08-29 20:03:15.000000 developers-chamber-0.0.9/developers_chamber/version_utils.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)    10457 2019-09-06 12:44:08.000000 developers-chamber-0.0.9/developers_chamber/ecs_utils.py
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber/click/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-09-05 19:23:56.000000 developers-chamber-0.0.9/developers_chamber/click/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      879 2019-09-05 19:23:56.000000 developers-chamber-0.0.9/developers_chamber/click/options.py
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber/scripts/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     7839 2019-09-06 12:44:08.000000 developers-chamber-0.0.9/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1746 2019-08-30 08:02:58.000000 developers-chamber-0.0.9/developers_chamber/scripts/version.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       50 2019-08-26 20:44:37.000000 developers-chamber-0.0.9/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     4311 2019-08-30 08:02:58.000000 developers-chamber-0.0.9/developers_chamber/scripts/git.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1454 2019-09-05 21:36:36.000000 developers-chamber-0.0.9/developers_chamber/scripts/docker.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1748 2019-08-30 08:02:58.000000 developers-chamber-0.0.9/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-08-26 20:44:37.000000 developers-chamber-0.0.9/developers_chamber/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1235 2019-09-05 19:23:56.000000 developers-chamber-0.0.9/developers_chamber/docker_utils.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      438 2019-08-26 20:44:37.000000 developers-chamber-0.0.9/developers_chamber/types.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      981 2019-08-29 20:03:15.000000 developers-chamber-0.0.9/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber/bin/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      894 2019-09-05 19:23:56.000000 developers-chamber-0.0.9/developers_chamber/bin/pydev.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2019-08-26 20:44:37.000000 developers-chamber-0.0.9/developers_chamber/bin/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     3744 2019-09-06 09:05:27.000000 developers-chamber-0.0.9/developers_chamber/git_utils.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      800 2019-09-06 12:44:30.000000 developers-chamber-0.0.9/setup.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       38 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/setup.cfg
+drwxr-xr-x   0 lubos     (1000) lubos     (1000)        0 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      348 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       73 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2019-08-30 08:04:32.000000 developers-chamber-0.0.9/developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      993 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       60 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       19 2019-09-06 12:44:55.000000 developers-chamber-0.0.9/developers_chamber.egg-info/top_level.txt
```

### Comparing `developers-chamber-0.0.8/README.md` & `developers-chamber-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/version_utils.py` & `developers-chamber-0.0.9/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/ecs_utils.py` & `developers-chamber-0.0.9/developers_chamber/ecs_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,28 +224,28 @@
     waiter = ecs_client.get_waiter('tasks_running')
     try:
         waiter.wait(cluster=cluster, tasks=tasks)
     except ClientError as ex:
         raise ClickException(ex)
 
 
-def migrate_service(cluster, service, command, succes_string, region):
+def migrate_service(cluster, service, command, success_string, region):
     ecs_client = _get_ecs_client(region)
     task_definition = get_task_definition_for_service(cluster=cluster, service=service, region=region)
     latest_task_definition = task_definition[:task_definition.rfind(':')]
     containers = ecs_client.describe_task_definition(taskDefinition=latest_task_definition)['taskDefinition']['containerDefinitions']
     
     if len(containers) != 1:
         raise ClickException('Exactly one container is allowed to be specified in service.\nNumber of containers specified: {}'.format(len(containers)))
     
     name = containers[0]['name']
     
     run_task_and_wait_for_success(
         cluster=cluster, 
-        latest_task_definition=latest_task_definition, 
+        task_definition=latest_task_definition, 
         command=command, 
         name=name, 
         success_string=success_string,
         region=region
     )
```

### Comparing `developers-chamber-0.0.8/developers_chamber/click/options.py` & `developers-chamber-0.0.9/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/scripts/ecs.py` & `developers-chamber-0.0.9/developers_chamber/scripts/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from developers_chamber.ecs_utils import register_new_task_definition as register_new_task_definition_func
 from developers_chamber.ecs_utils import update_service_to_latest_task_definition as update_service_to_latest_task_definition_func
 from developers_chamber.ecs_utils import run_task_and_wait_for_success as run_task_and_wait_for_success_func
 from developers_chamber.ecs_utils import get_tasks_for_service as get_tasks_for_service_func
 from developers_chamber.ecs_utils import get_task_definition_for_service as get_task_definition_for_service_func
 from developers_chamber.ecs_utils import start_service_and_wait_for_tasks_to_start as start_service_and_wait_for_tasks_to_start_func
 from developers_chamber.ecs_utils import stop_service_and_wait_for_tasks_to_stop as stop_service_and_wait_for_tasks_to_stop_func
+from developers_chamber.ecs_utils import migrate_service as migrate_service_func
 from developers_chamber.scripts import cli
 
 
 default_region = os.environ.get('AWS_REGION')
 default_cluster = os.environ.get('AWS_ECS_CLUSTER')
 
 @cli.group()
@@ -86,21 +87,21 @@
 @click.option('--region', help='AWS region', type=str, default=default_region, required=True)
 def run_task_and_wait_for_success(cluster, task_definition, command, name, success_string, region):
     """Run a single task in AWS ECS and wait for it to stop with success."""
     run_task_and_wait_for_success_func(cluster, task_definition, command, name, success_string, region)
 
 @ecs.command()
 @click.option('--cluster', help='ECS cluster name', type=str, default=default_cluster, required=True)
+@click.option('--service', help='ECS service name', type=str, required=True)
 @click.option('--command', help='command to run', type=str, required=True)
-@click.option('--name', help='ECS task name', type=str, required=True)
 @click.option('--success-string', help='String that is considered a success code', type=str, default='0', required=True)
 @click.option('--region', help='AWS region', type=str, default=default_region, required=True)
 def migrate_service(cluster, service, command, success_string, region):
     """Run a single task based on service's task definition in AWS ECS and wait for it to stop with success."""
-    run_task_and_wait_for_success_func(cluster, task_definition, command, name, success_string, region)
+    migrate_service_func(cluster, service, command, success_string, region)
 
 @ecs.command()
 @click.option('--cluster', help='ECS cluster name', type=str, default=default_cluster, required=True)
 @click.option('--service', help='ECS service name', type=str, required=True)
 @click.option('--region', help='AWS region', type=str, default=default_region, required=True)
 def get_tasks_for_service(cluster, service, region):
 	""" Return list of tasks running under specified service """
```

### Comparing `developers-chamber-0.0.8/developers_chamber/scripts/version.py` & `developers-chamber-0.0.9/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/scripts/git.py` & `developers-chamber-0.0.9/developers_chamber/scripts/git.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/scripts/docker.py` & `developers-chamber-0.0.9/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/scripts/bitbucket.py` & `developers-chamber-0.0.9/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/docker_utils.py` & `developers-chamber-0.0.9/developers_chamber/docker_utils.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/bitbucket_utils.py` & `developers-chamber-0.0.9/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/bin/pydev.py` & `developers-chamber-0.0.9/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/developers_chamber/git_utils.py` & `developers-chamber-0.0.9/developers_chamber/git_utils.py`

 * *Files identical despite different names*

### Comparing `developers-chamber-0.0.8/setup.py` & `developers-chamber-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='developers-chamber',
-    version='0.0.8',
+    version='0.0.9',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/druids/django-project-info',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
```

### Comparing `developers-chamber-0.0.8/developers_chamber.egg-info/SOURCES.txt` & `developers-chamber-0.0.9/developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

