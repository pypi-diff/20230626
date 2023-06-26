# Comparing `tmp/cancelchain-1.4.0.tar.gz` & `tmp/cancelchain-1.4.1.tar.gz`

## Comparing `cancelchain-1.4.0.tar` & `cancelchain-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/__init__.py
--rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/api.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/api_client.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/application.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/block.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/browser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/cache.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/chain.py
--rw-r--r--   0        0        0    29702 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/command.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/config.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/console.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/database.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/exceptions.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/miller.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/milling.py
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/models.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/node.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/payload.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/schema.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/signals.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/tasks.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/transaction.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/util.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/wallet.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/base.html
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/block.html
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/chains.html
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/index.html
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.4.0/src/cancelchain/templates/transaction.html
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.4.0/.gitignore
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.4.0/LICENSE
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 cancelchain-1.4.0/README.rst
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 cancelchain-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     9823 2020-02-02 00:00:00.000000 cancelchain-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/__init__.py
+-rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/api.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/api_client.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/application.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/block.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/browser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/cache.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/chain.py
+-rw-r--r--   0        0        0    29696 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/command.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/config.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/console.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/database.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/exceptions.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/miller.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/milling.py
+-rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/models.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/node.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/payload.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/schema.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/signals.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/tasks.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/transaction.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/util.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/wallet.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/templates/base.html
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/templates/block.html
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/templates/chains.html
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/templates/index.html
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 cancelchain-1.4.1/src/cancelchain/templates/transaction.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 cancelchain-1.4.1/.gitignore
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cancelchain-1.4.1/LICENSE
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 cancelchain-1.4.1/README.rst
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 cancelchain-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 cancelchain-1.4.1/PKG-INFO
```

### Comparing `cancelchain-1.4.0/src/cancelchain/__init__.py` & `cancelchain-1.4.1/src/cancelchain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 
 def create_app(app=None, config_map=None, register_browser=True):
     from .application import init_app
     from .cache import cache
     from .config import EnvAppSettings
     from .database import db
```

### Comparing `cancelchain-1.4.0/src/cancelchain/api.py` & `cancelchain-1.4.1/src/cancelchain/api.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/api_client.py` & `cancelchain-1.4.1/src/cancelchain/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def peer_header(visited_hosts, headers=None):
     headers = headers or {}
     if visited_hosts:
         headers[PEER_HOST_HEADER] = ','.join(visited_hosts)
     return headers
 
 
-class ApiClient():
+class ApiClient:
     def __init__(self, host, wallet, timeout=None):
         host, address = host_address(host)
         if address and address != wallet.address:
             raise Exception(ADDRESS_MISMATCH_MSG)
         self.host = host
         self.wallet = wallet
         self.token = None
```

### Comparing `cancelchain-1.4.0/src/cancelchain/application.py` & `cancelchain-1.4.1/src/cancelchain/application.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/block.py` & `cancelchain-1.4.1/src/cancelchain/block.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/browser.py` & `cancelchain-1.4.1/src/cancelchain/browser.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/chain.py` & `cancelchain-1.4.1/src/cancelchain/chain.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/command.py` & `cancelchain-1.4.1/src/cancelchain/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             while f.read(1) != b'\n':
                 f.seek(-2, os.SEEK_CUR)
         except OSError:  # catch OSError in case of one line file
             f.seek(0)
         return f.readline().decode()
 
 
-class ProgressBar():
+class ProgressBar:
     def __init__(self, title, console=None, total=None, completed=0):
         self.progress = Progress(
             BarColumn(),
             TextColumn('{task.completed}/{task.total}'),
             TaskProgressColumn(),
             TimeRemainingColumn(),
             TextColumn('['),
@@ -143,15 +143,15 @@
         self.live.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.live.__exit__(exc_type, exc_val, exc_tb)
 
 
-class BlockSyncProgress():
+class BlockSyncProgress:
     def __init__(self, peer=None, console=None):
         self.find_progress = Progress(
             SpinnerColumn(spinner_name='aesthetic', style='none'),
             TextColumn('{task.completed} Blocks'),
             TextColumn('['),
             TimeElapsedColumn(),
             TextColumn(']')
@@ -225,15 +225,15 @@
         self.live.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.live.__exit__(exc_type, exc_val, exc_tb)
 
 
-class MillingProgress():
+class MillingProgress:
     def __init__(self, console=None):
         self.block = None
         self.chain = None
         self.progress = Progress(
             SpinnerColumn(spinner_name='aesthetic', style='milling'),
             TextColumn('{task.fields[hash_count]}h @'),
             TextColumn('{task.fields[hps]} hps'),
```

### Comparing `cancelchain-1.4.0/src/cancelchain/config.py` & `cancelchain-1.4.1/src/cancelchain/config.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/exceptions.py` & `cancelchain-1.4.1/src/cancelchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/miller.py` & `cancelchain-1.4.1/src/cancelchain/miller.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/milling.py` & `cancelchain-1.4.1/src/cancelchain/milling.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/models.py` & `cancelchain-1.4.1/src/cancelchain/models.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/node.py` & `cancelchain-1.4.1/src/cancelchain/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     rollback_session,
 )
 from cancelchain.signals import new_block as new_block_signal
 from cancelchain.transaction import PendingTxnSet, Transaction
 from cancelchain.util import host_address, now
 
 
-class Node():
+class Node:
     def __init__(self, host=None, peers=None, clients=None, logger=None):
         self.host = host
         self.peers = peers or []
         self.clients = clients or {}
         self.logger = logger or logging.getLogger(__name__)
         self.pending_txns = PendingTxnSet()
```

### Comparing `cancelchain-1.4.0/src/cancelchain/payload.py` & `cancelchain-1.4.1/src/cancelchain/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     @post_load
     def make_outflow(self, data, **kwargs):
         return Outflow(**data)
 
 
 @dataclass
-class Outflow():
+class Outflow:
     amount: int = None
     address: str = None
     subject: str = None
     forgive: str = None
     support: str = None
 
     @property
```

### Comparing `cancelchain-1.4.0/src/cancelchain/schema.py` & `cancelchain-1.4.1/src/cancelchain/schema.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/tasks.py` & `cancelchain-1.4.1/src/cancelchain/tasks.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/transaction.py` & `cancelchain-1.4.1/src/cancelchain/transaction.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/util.py` & `cancelchain-1.4.1/src/cancelchain/util.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/wallet.py` & `cancelchain-1.4.1/src/cancelchain/wallet.py`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/templates/base.html` & `cancelchain-1.4.1/src/cancelchain/templates/base.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/templates/block.html` & `cancelchain-1.4.1/src/cancelchain/templates/block.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/templates/chains.html` & `cancelchain-1.4.1/src/cancelchain/templates/chains.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/templates/index.html` & `cancelchain-1.4.1/src/cancelchain/templates/index.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/src/cancelchain/templates/transaction.html` & `cancelchain-1.4.1/src/cancelchain/templates/transaction.html`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/.gitignore` & `cancelchain-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/LICENSE` & `cancelchain-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cancelchain-1.4.0/README.rst` & `cancelchain-1.4.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 A minimal ``.env`` configuration file:
 
 .. code-block:: console
 
   # Flask Settings
   FLASK_APP=cancelchain
-  FLASK_RUN_HOST=0.0.0.0
   FLASK_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
 
   # Flask-SQLAlchemy Settings
   FLASK_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
 
 The `FLASK_SECRET_KEY`_ value should be a unique random string.
```

### Comparing `cancelchain-1.4.0/pyproject.toml` & `cancelchain-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,31 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Sociology",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "base58check>=1.0",
   "blinker>=1.6",
-  "celery>=5.2",
+  "celery>=5.3",
   "click>=8.1",
   "Flask>=2.3",
   "Flask-Caching>=2.0",
   "Flask-SQLAlchemy>=3.0",
   "gunicorn>=20.1",
   "humanfriendly>=10.0",
   "marshmallow>=3.19",
   "millify>=0.1",
   "passlib[argon2]>=1.7",
   "pg8000>=1.29",
-  "pycryptodome>=3.17",
-  "pyjwt>=2.6",
-  "pymerkle>=4.0",
+  "pycryptodome>=3.18",
+  "pyjwt>=2.7",
+  "pymerkle>=4.0,<5.0",
   "python-dotenv>=1.0",
-  "requests>=2.29",
-  "rich>=13.3",
+  "requests>=2.31",
+  "rich>=13.4",
   "sqlalchemy<2.0",
 ]
 
 [project.scripts]
 cancelchain = "cancelchain:cli"
 
 [project.urls]
@@ -70,20 +70,20 @@
 exclude = [
   "/.github",
 ]
 
 [tool.hatch.envs.test]
 dependencies = [
   "coverage[toml]>=7.2",
-  "pytest>=7.3",
-  "pytest-cov>=4.0",
+  "pytest>=7.4",
+  "pytest-cov>=4.1",
   "pytest-dotenv>=0.5",
-  "requests-mock>=1.10",
-  "time-machine>=2.9",
-  "ruff>=0.0.264",
+  "requests-mock>=1.11",
+  "time-machine>=2.10",
+  "ruff>=0.0.275",
 ]
 
 [tool.hatch.envs.test.scripts]
 run-coverage = "pytest --cov-config=pyproject.toml --cov=cancelchain"
 run = "run-coverage --no-cov"
 
 # RUFF
```

### Comparing `cancelchain-1.4.0/PKG-INFO` & `cancelchain-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancelchain
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Blockchain of Accountability, Forgiveness, and Support
 Project-URL: Homepage, https://cancelchain.org
 Project-URL: Documentation, https://docs.cancelchain.org
 Project-URL: Source, https://github.com/cancelchain/cancelchain
 Project-URL: Tracker, https://github.com/cancelchain/cancelchain/issues
 Author-email: Thomas Bohmbach Jr <tom@cancelchain.org>
 License-Expression: MIT
@@ -17,31 +17,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology
 Requires-Python: >=3.9
 Requires-Dist: base58check>=1.0
 Requires-Dist: blinker>=1.6
-Requires-Dist: celery>=5.2
+Requires-Dist: celery>=5.3
 Requires-Dist: click>=8.1
 Requires-Dist: flask-caching>=2.0
 Requires-Dist: flask-sqlalchemy>=3.0
 Requires-Dist: flask>=2.3
 Requires-Dist: gunicorn>=20.1
 Requires-Dist: humanfriendly>=10.0
 Requires-Dist: marshmallow>=3.19
 Requires-Dist: millify>=0.1
 Requires-Dist: passlib[argon2]>=1.7
 Requires-Dist: pg8000>=1.29
-Requires-Dist: pycryptodome>=3.17
-Requires-Dist: pyjwt>=2.6
-Requires-Dist: pymerkle>=4.0
+Requires-Dist: pycryptodome>=3.18
+Requires-Dist: pyjwt>=2.7
+Requires-Dist: pymerkle<5.0,>=4.0
 Requires-Dist: python-dotenv>=1.0
-Requires-Dist: requests>=2.29
-Requires-Dist: rich>=13.3
+Requires-Dist: requests>=2.31
+Requires-Dist: rich>=13.4
 Requires-Dist: sqlalchemy<2.0
 Description-Content-Type: text/x-rst
 
 CancelChain
 ###########
 
 CancelChain is an open-source python project that implements a custom blockchain ledger. The ledger protocol allows for the assigning of tokens to subjects (utf-8 strings of less than 80 characters) as indications of either opposition or support. Opposition entries are allowed to be rescinded later. Support is forever.
@@ -78,15 +78,14 @@
 
 A minimal ``.env`` configuration file:
 
 .. code-block:: console
 
   # Flask Settings
   FLASK_APP=cancelchain
-  FLASK_RUN_HOST=0.0.0.0
   FLASK_SECRET_KEY=0b6ceaa3b10d3e7a5dc53194
 
   # Flask-SQLAlchemy Settings
   FLASK_SQLALCHEMY_DATABASE_URI=sqlite:///cc.sqlite
 
 The `FLASK_SECRET_KEY`_ value should be a unique random string.
```

