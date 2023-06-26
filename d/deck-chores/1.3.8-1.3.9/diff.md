# Comparing `tmp/deck_chores-1.3.8.tar.gz` & `tmp/deck_chores-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deck_chores-1.3.8.tar", max compression
+gzip compressed data, was "deck_chores-1.3.9.tar", max compression
```

## Comparing `deck_chores-1.3.8.tar` & `deck_chores-1.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      754 2023-02-08 17:33:13.696267 deck_chores-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0     3296 2023-02-08 17:33:13.696267 deck_chores-1.3.8/README.rst
--rw-r--r--   0        0        0      106 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/__init__.py
--rw-r--r--   0        0        0     3042 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/config.py
--rw-r--r--   0        0        0     2064 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/indexes.py
--rw-r--r--   0        0        0     5184 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/jobs.py
--rw-r--r--   0        0        0    10162 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/main.py
--rw-r--r--   0        0        0     8500 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/parsers.py
--rw-r--r--   0        0        0     3244 2023-02-08 17:33:13.696267 deck_chores-1.3.8/deck_chores/utils.py
--rw-r--r--   0        0        0     1469 2023-02-08 17:33:13.696267 deck_chores-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 deck_chores-1.3.8/setup.py
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 deck_chores-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-02-26 04:53:19.171139 deck_chores-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     3296 2023-02-26 04:53:19.171139 deck_chores-1.3.9/README.rst
+-rw-r--r--   0        0        0      106 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/__init__.py
+-rw-r--r--   0        0        0     3042 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/config.py
+-rw-r--r--   0        0        0     2064 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/indexes.py
+-rw-r--r--   0        0        0     5184 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/jobs.py
+-rw-r--r--   0        0        0    10162 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/main.py
+-rw-r--r--   0        0        0     8500 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/parsers.py
+-rw-r--r--   0        0        0     3244 2023-02-26 04:53:19.171139 deck_chores-1.3.9/deck_chores/utils.py
+-rw-r--r--   0        0        0     1469 2023-02-26 04:53:19.175139 deck_chores-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 deck_chores-1.3.9/setup.py
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 deck_chores-1.3.9/PKG-INFO
```

### Comparing `deck_chores-1.3.8/LICENSE.txt` & `deck_chores-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/README.rst` & `deck_chores-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/config.py` & `deck_chores-1.3.9/deck_chores/config.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/indexes.py` & `deck_chores-1.3.9/deck_chores/indexes.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/jobs.py` & `deck_chores-1.3.9/deck_chores/jobs.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/main.py` & `deck_chores-1.3.9/deck_chores/main.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/parsers.py` & `deck_chores-1.3.9/deck_chores/parsers.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/deck_chores/utils.py` & `deck_chores-1.3.9/deck_chores/utils.py`

 * *Files identical despite different names*

### Comparing `deck_chores-1.3.8/pyproject.toml` & `deck_chores-1.3.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 safe = true
 skip-string-normalization = true
 
 [tool.poetry]
 name = "deck-chores"
-version = "1.3.8"
+version = "1.3.9"
 description = "Job scheduler for Docker containers, configured via container labels."
 readme = "README.rst"
 documentation = "https://deck-chores.readthedocs.org/"
 repository = "https://github.com/funkyfuture/deck-chores"
 license = "ISC license"
 keywords = ["docker", "cron", "scheduler", "jobs", "labels", "metadata"]
 classifiers = [
```

### Comparing `deck_chores-1.3.8/setup.py` & `deck_chores-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'python-dateutil>=2.8.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['deck-chores = deck_chores.main:main']}
 
 setup_kwargs = {
     'name': 'deck-chores',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Job scheduler for Docker containers, configured via container labels.',
     'long_description': 'deck-chores\n===========\n\n.. image:: https://img.shields.io/docker/pulls/funkyfuture/deck-chores.svg\n        :target: https://hub.docker.com/r/funkyfuture/deck-chores/\n\n.. image:: https://images.microbadger.com/badges/image/funkyfuture/deck-chores.svg\n        :target: https://microbadger.com/images/funkyfuture/deck-chores\n\n.. image:: https://img.shields.io/pypi/v/deck-chores.svg\n        :target: https://pypi.org/project/deck-chores/\n\n**A job scheduler for Docker containers, configured via container labels.**\n\n* Documentation: https://deck-chores.readthedocs.io\n* Image repositories:\n    * https://github.com/funkyfuture/deck-chores/pkgs/container/deck-chores\n    * https://hub.docker.com/r/funkyfuture/deck-chores\n* Code repository: https://github.com/funkyfuture/deck-chores\n* Issue tracker: https://github.com/funkyfuture/deck-chores/issues\n* Free software: ISC license\n\n\nFeatures\n--------\n\n- define regular jobs to run within a container context with container and optionally with image\n  labels\n- use date, interval and cron-like triggers\n- set a maximum of simultaneously running instances per job\n- restrict job scheduling to one container per service\n- multi-architecture image supports ``amd64``, ``arm64`` and ``arm`` platforms\n  (the latter are currently not provided for download)\n\n\nExample\n-------\n\nLet\'s say you want to dump the database of a Wordpress once a day. Here\'s a ``docker-compose.yml``\nthat defines a job that will be handled by *deck-chores*:\n\n.. code-block:: yaml\n\n    version: "3.7"\n\n    services:\n      wordpress:\n        image: wordpress\n      mysql:\n        image: mariadb\n        volumes:\n          - ./database_dumps:/dumps\n        labels:\n          deck-chores.dump.command: sh -c "mysqldump --all-databases > /dumps/dump-$$(date -Idate)"\n          deck-chores.dump.interval: daily\n\nIt is however recommended to use scripts with a proper shebang for such actions. Their outputs to\n``stdout`` and ``stderr`` as well as their exit code will be logged by *deck-chores*.\n\n\nMaintenance\n-----------\n\nThe final release is supposed to receive monthly updates that includes updates\nof all updateable dependencies. If one is skipped, don\'t worry. When a second\nmaintenance release is skipped, feel free to open an issue to ask what the\nstatus is.\n\nYou can always build images upon an up-to-date base image with::\n\n    make build\n\n\nLimitations\n-----------\n\nWhen running on a cluster of `Docker Swarm <https://docs.docker.com/engine/swarm/>`_\nnodes, each ``deck-chores`` instance can only observe the containers on the\nnode it\'s running on, and hence only restrict to run one job per service within\nthe node\'s context.\n\n\nAcknowledgements\n----------------\n\nIt wouldn\'t be as charming to write this piece of software without these projects:\n\n* `APScheduler <https://apscheduler.readthedocs.io>`_ for managing jobs\n* `cerberus <http://python-cerberus.org>`_ for processing metadata\n* `docker-py <https://docker-py.readthedocs.io>`_ for Docker interaction\n* `flake8 <http://flake8.pycqa.org/>`_, `mypy <http://mypy-lang.org>`_,\n  `pytest <http://pytest.org>`_ and `tox <https://tox.readthedocs.io>`_ for testing\n* `Python <https://www.python.org>`_\n\n\nAuthors\n-------\n\n- Frank Sachsenheim (maintaining)\n- aeri4list\n- alpine-digger\n- Brynjar Smári Bjarnason\n- Garret Hohmann\n',
     'author': 'Frank Sachsenheim',
     'author_email': 'funkyfuture@riseup.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/funkyfuture/deck-chores',
```

### Comparing `deck_chores-1.3.8/PKG-INFO` & `deck_chores-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deck-chores
-Version: 1.3.8
+Version: 1.3.9
 Summary: Job scheduler for Docker containers, configured via container labels.
 Home-page: https://github.com/funkyfuture/deck-chores
 License: ISC
 Keywords: docker,cron,scheduler,jobs,labels,metadata
 Author: Frank Sachsenheim
 Author-email: funkyfuture@riseup.net
 Requires-Python: >=3.11,<4.0
```

