# Comparing `tmp/automatix-1.8.2.tar.gz` & `tmp/automatix-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/automatix-1.8.2.tar", last modified: Tue Dec 21 17:42:10 2021, max compression
+gzip compressed data, was "dist/automatix-1.9.0.tar", last modified: Fri Jan  7 18:35:45 2022, max compression
```

## Comparing `automatix-1.8.2.tar` & `automatix-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2021-12-21 17:42:10.000000 automatix-1.8.2/
--rw-r--r--   0 jpaul      (502) staff       (20)    20573 2021-12-21 17:42:10.000000 automatix-1.8.2/PKG-INFO
-drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/
--rw-r--r--   0 jpaul      (502) staff       (20)    20573 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/PKG-INFO
--rw-r--r--   0 jpaul      (502) staff       (20)      399 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/SOURCES.txt
--rw-r--r--   0 jpaul      (502) staff       (20)       46 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/entry_points.txt
--rw-r--r--   0 jpaul      (502) staff       (20)       63 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/requires.txt
--rw-r--r--   0 jpaul      (502) staff       (20)       10 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/top_level.txt
--rw-r--r--   0 jpaul      (502) staff       (20)        1 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix.egg-info/dependency_links.txt
-drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2021-12-21 17:42:10.000000 automatix-1.8.2/automatix/
--rw-r--r--   0 jpaul      (502) staff       (20)    11894 2021-12-21 17:39:28.000000 automatix-1.8.2/automatix/command.py
--rw-r--r--   0 jpaul      (502) staff       (20)     7583 2021-12-21 17:39:28.000000 automatix-1.8.2/automatix/config.py
--rw-r--r--   0 jpaul      (502) staff       (20)     1410 2021-08-16 15:54:44.000000 automatix-1.8.2/automatix/bundlewrap.py
--rw-r--r--   0 jpaul      (502) staff       (20)     2346 2021-12-21 17:39:28.000000 automatix-1.8.2/automatix/__init__.py
--rw-r--r--   0 jpaul      (502) staff       (20)     2210 2020-04-02 11:00:56.000000 automatix-1.8.2/automatix/command_test.py
--rw-r--r--   0 jpaul      (502) staff       (20)     2799 2019-11-14 13:13:51.000000 automatix-1.8.2/automatix/logger.py
--rw-r--r--   0 jpaul      (502) staff       (20)     4343 2021-08-16 14:58:50.000000 automatix-1.8.2/automatix/automatix.py
--rw-r--r--   0 jpaul      (502) staff       (20)      492 2020-11-02 10:52:43.000000 automatix-1.8.2/automatix/environment.py
--rw-r--r--   0 jpaul      (502) staff       (20)    16507 2021-08-16 15:54:44.000000 automatix-1.8.2/README.md
--rw-r--r--   0 jpaul      (502) staff       (20)     1006 2021-12-21 17:39:58.000000 automatix-1.8.2/setup.py
--rw-r--r--   0 jpaul      (502) staff       (20)       38 2021-12-21 17:42:10.000000 automatix-1.8.2/setup.cfg
+drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2022-01-07 18:35:45.000000 automatix-1.9.0/
+-rw-r--r--   0 jpaul      (502) staff       (20)    21331 2022-01-07 18:35:45.000000 automatix-1.9.0/PKG-INFO
+drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/
+-rw-r--r--   0 jpaul      (502) staff       (20)    21331 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/PKG-INFO
+-rw-r--r--   0 jpaul      (502) staff       (20)      428 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/SOURCES.txt
+-rw-r--r--   0 jpaul      (502) staff       (20)       46 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/entry_points.txt
+-rw-r--r--   0 jpaul      (502) staff       (20)       94 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/requires.txt
+-rw-r--r--   0 jpaul      (502) staff       (20)       10 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/top_level.txt
+-rw-r--r--   0 jpaul      (502) staff       (20)        1 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix.egg-info/dependency_links.txt
+drwxr-xr-x   0 jpaul      (502) staff       (20)        0 2022-01-07 18:35:45.000000 automatix-1.9.0/automatix/
+-rw-r--r--   0 jpaul      (502) staff       (20)    11876 2022-01-07 18:30:35.000000 automatix-1.9.0/automatix/command.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     7981 2022-01-07 18:30:35.000000 automatix-1.9.0/automatix/config.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     1410 2021-08-16 15:54:44.000000 automatix-1.9.0/automatix/bundlewrap.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     2380 2022-01-07 18:30:35.000000 automatix-1.9.0/automatix/__init__.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     2210 2020-04-02 11:00:56.000000 automatix-1.9.0/automatix/command_test.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     2799 2019-11-14 13:13:51.000000 automatix-1.9.0/automatix/logger.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     4343 2021-08-16 14:58:50.000000 automatix-1.9.0/automatix/automatix.py
+-rw-r--r--   0 jpaul      (502) staff       (20)      492 2020-11-02 10:52:43.000000 automatix-1.9.0/automatix/environment.py
+-rw-r--r--   0 jpaul      (502) staff       (20)     1072 2022-01-07 18:30:35.000000 automatix-1.9.0/automatix/bash_completion.py
+-rw-r--r--   0 jpaul      (502) staff       (20)    17081 2022-01-07 18:30:35.000000 automatix-1.9.0/README.md
+-rw-r--r--   0 jpaul      (502) staff       (20)     1076 2022-01-07 18:34:26.000000 automatix-1.9.0/setup.py
+-rw-r--r--   0 jpaul      (502) staff       (20)       38 2022-01-07 18:35:45.000000 automatix-1.9.0/setup.cfg
```

### Comparing `automatix-1.8.2/PKG-INFO` & `automatix-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatix
-Version: 1.8.2
+Version: 1.9.0
 Summary: Automation wrapper for bash and python commands
 Home-page: https://github.com/seibert-media/automatix
 Author: Johannes Paul, //SEIBERT/MEDIA GmbH
 Author-email: jpaul@seibert-media.net
 License: MIT
 Description: # automatix
         Automation wrapper for bash and python commands
@@ -444,13 +444,33 @@
          **cleanup** pipeline, use CRTL+C.
         
         While **aborting remote functions** (via imports), automatix is not
          able to determine still running processes invoked by the function,
          because it only checks the processes for the commands (in this case
          the function name) which is called in the pipeline.
         
+        # EXTRAS
+        
+        ## Bash completion (experimental)
+        Automatix supports bash completion for parameters and the script directory via [argcomplete](https://github.com/kislyuk/argcomplete).
+        
+        Therefor follow the installation instructions for argcomplete, which is at the current time
+        
+            pip install argcomplete
+        
+        and either global activation via executing
+        
+            activate-global-python-argcomplete
+        
+        or activation for automatix (e.g. in `.bashrc`)
+        
+            eval "$(register-python-argcomplete automatix)"
+        
+        Automatix will recognize the installed module and offer the completion automatically.
+        
 Keywords: bash,shell,command,automation,process,wrapper,devops,system administration
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: bash completion
```

### Comparing `automatix-1.8.2/automatix.egg-info/PKG-INFO` & `automatix-1.9.0/automatix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatix
-Version: 1.8.2
+Version: 1.9.0
 Summary: Automation wrapper for bash and python commands
 Home-page: https://github.com/seibert-media/automatix
 Author: Johannes Paul, //SEIBERT/MEDIA GmbH
 Author-email: jpaul@seibert-media.net
 License: MIT
 Description: # automatix
         Automation wrapper for bash and python commands
@@ -444,13 +444,33 @@
          **cleanup** pipeline, use CRTL+C.
         
         While **aborting remote functions** (via imports), automatix is not
          able to determine still running processes invoked by the function,
          because it only checks the processes for the commands (in this case
          the function name) which is called in the pipeline.
         
+        # EXTRAS
+        
+        ## Bash completion (experimental)
+        Automatix supports bash completion for parameters and the script directory via [argcomplete](https://github.com/kislyuk/argcomplete).
+        
+        Therefor follow the installation instructions for argcomplete, which is at the current time
+        
+            pip install argcomplete
+        
+        and either global activation via executing
+        
+            activate-global-python-argcomplete
+        
+        or activation for automatix (e.g. in `.bashrc`)
+        
+            eval "$(register-python-argcomplete automatix)"
+        
+        Automatix will recognize the installed module and offer the completion automatically.
+        
 Keywords: bash,shell,command,automation,process,wrapper,devops,system administration
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: bash completion
```

### Comparing `automatix-1.8.2/automatix/command.py` & `automatix-1.9.0/automatix/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 import re
 import subprocess
-import traceback
-
 from shlex import quote
 from time import time
 from typing import Tuple
 
 from .environment import PipelineEnvironment
 
 PERSISTENT_VARS = {}
```

### Comparing `automatix-1.8.2/automatix/config.py` & `automatix-1.9.0/automatix/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
 
 if sys.version_info >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
+try:
+    from argcomplete import autocomplete
+    from .bash_completion import ScriptFileCompleter
+
+    bash_completion = True
+except ImportError:
+    bash_completion = False
+
 VERSION = metadata.version('automatix')
 
 DEPRECATED_SYNTAX = {
     # 0: REGEX pattern
     # 1: replacement, formatted with group = re.Match.groups(), e.g. 'something {group[0]} foo'
     # 2: special flags (p: python, b: Bundlewrap, s: replace '{s}' with pipe separated system names)
     (r'({s})_node(?!\w)', 'NODES.{group[0]}', 'bps'),
@@ -45,25 +53,25 @@
     'ssh_cmd': 'ssh {hostname} sudo ',
     'remote_tmp_dir': 'automatix_tmp',
     'logger': 'automatix',
     'bundlewrap': False,
     'teamvault': False,
 }
 
-configfile = os.path.expanduser(os.getenv('AUTOMATIX_CONFIG', '~/.automatix.cfg.yaml'))
+configfile = os.path.expanduser(os.path.expandvars(os.getenv('AUTOMATIX_CONFIG', '~/.automatix.cfg.yaml')))
 if os.path.isfile(configfile):
     CONFIG.update(read_yaml(configfile))
     CONFIG['config_file'] = configfile
 
 if os.getenv('AUTOMATIX_SCRIPT_DIR'):
     CONFIG['script_dir'] = os.getenv('AUTOMATIX_SCRIPT_DIR')
 
 LOG = logging.getLogger(CONFIG['logger'])
 
-SCRIPT_PATH = os.path.expanduser(CONFIG['script_dir'])
+SCRIPT_PATH = os.path.expanduser(os.path.expandvars(CONFIG['script_dir']))
 
 if CONFIG['teamvault']:
     import bwtv
 
     SCRIPT_FIELDS['secrets'] = 'Secrets'
 
 
@@ -72,18 +80,21 @@
 
 
 def arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Automation wrapper for bash and python commands.',
         epilog='Explanations and README at https://github.com/seibert-media/automatix',
     )
-    parser.add_argument(
+    scriptfile_action = parser.add_argument(
         'scriptfile',
         help='Path to scriptfile (yaml), use " -- " if needed to delimit this from argument fields',
     )
+    if bash_completion:
+        scriptfile_action.completer = ScriptFileCompleter(script_path=SCRIPT_PATH)
+
     for field in SCRIPT_FIELDS.keys():
         parser.add_argument(
             f'--{field}',
             nargs='*',
             help=f'Use this to set {field} without adding them to the script or to overwrite them. '
                  f'You can specify multiple {field} like: --{field} v1=string1 v2=string2 v3=string3',
         )
@@ -113,14 +124,16 @@
         help='try always to proceed (except manual steps), even if errors occur (no retries)'
     )
     parser.add_argument(
         '--debug', '-d',
         action='store_true',
         help='activate debug log level',
     )
+    if bash_completion:
+        autocomplete(parser)
     return parser.parse_args()
 
 
 def _overwrite(script: dict, key: str, data: str):
     script.setdefault(key, {})
     for item in data:
         k, v = item.split('=')
@@ -215,7 +228,8 @@
         assert len(key.split(':')) == 2, \
             'First row in CSV must contain "label" or the field name and key seperated by colons' \
             ' like "label,systems:mysystem,vars:myvar".'
         key_type, key_name = key.split(':')
         assert key_type in SCRIPT_FIELDS.keys(), \
             f'First row in CSV: Field name is \'{key_type}\', but has to be one of {list(SCRIPT_FIELDS.keys())}.'
         script[key_type][key_name] = value
+
```

### Comparing `automatix-1.8.2/automatix/bundlewrap.py` & `automatix-1.9.0/automatix/bundlewrap.py`

 * *Files identical despite different names*

### Comparing `automatix-1.8.2/automatix/__init__.py` & `automatix-1.9.0/automatix/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
-import sys
 from copy import deepcopy
 from csv import DictReader
 from importlib import import_module
 from time import time
 from typing import List
 
 from .automatix import Automatix
 from .command import Command, SkipBatchItemException, AbortException
 from .config import arguments, CONFIG, get_script, LOG, update_script_from_row, collect_vars, SCRIPT_FIELDS, VERSION
 
-if CONFIG.get('logging_lib'):
-    log_lib = import_module(CONFIG.get('logging_lib'))
-    init_logger = log_lib.init_logger
-else:
-    from .logger import init_logger
-
-if CONFIG.get('bundlewrap'):
-    from .bundlewrap import BWCommand, AutomatixBwRepo
-
-    CONFIG['bw_repo'] = AutomatixBwRepo(repo_path=os.environ.get('BW_REPO_PATH'))
-    cmdClass = BWCommand
-else:
-    cmdClass = Command
-
 
 def main():
     starttime = time()
     args = arguments()
+
+    if CONFIG.get('logging_lib'):
+        log_lib = import_module(CONFIG.get('logging_lib'))
+        init_logger = log_lib.init_logger
+    else:
+        from .logger import init_logger
+
     init_logger(name=CONFIG['logger'], debug=args.debug)
 
+    if CONFIG.get('bundlewrap'):
+        from .bundlewrap import BWCommand, AutomatixBwRepo
+
+        CONFIG['bw_repo'] = AutomatixBwRepo(repo_path=os.environ.get('BW_REPO_PATH'))
+        cmdClass = BWCommand
+    else:
+        cmdClass = Command
+
     LOG.info(f'Automatix Version {VERSION}')
 
     configfile = CONFIG.get('config_file')
     if configfile:
         LOG.info(f'Using configuration from: {configfile}')
     else:
         LOG.warning('Configuration file not found or not configured. Using defaults.')
```

### Comparing `automatix-1.8.2/automatix/command_test.py` & `automatix-1.9.0/automatix/command_test.py`

 * *Files identical despite different names*

### Comparing `automatix-1.8.2/automatix/logger.py` & `automatix-1.9.0/automatix/logger.py`

 * *Files identical despite different names*

### Comparing `automatix-1.8.2/automatix/automatix.py` & `automatix-1.9.0/automatix/automatix.py`

 * *Files identical despite different names*

### Comparing `automatix-1.8.2/README.md` & `automatix-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -435,7 +435,26 @@
 If you want to abort the **pipeline** without triggering the
  **cleanup** pipeline, use CRTL+C.
 
 While **aborting remote functions** (via imports), automatix is not
  able to determine still running processes invoked by the function,
  because it only checks the processes for the commands (in this case
  the function name) which is called in the pipeline.
+
+# EXTRAS
+
+## Bash completion (experimental)
+Automatix supports bash completion for parameters and the script directory via [argcomplete](https://github.com/kislyuk/argcomplete).
+
+Therefor follow the installation instructions for argcomplete, which is at the current time
+
+    pip install argcomplete
+
+and either global activation via executing
+
+    activate-global-python-argcomplete
+
+or activation for automatix (e.g. in `.bashrc`)
+
+    eval "$(register-python-argcomplete automatix)"
+
+Automatix will recognize the installed module and offer the completion automatically.
```

### Comparing `automatix-1.8.2/setup.py` & `automatix-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='automatix',
-    version='1.8.2',
+    version='1.9.0',
     description='Automation wrapper for bash and python commands',
     keywords=['bash', 'shell', 'command', 'automation', 'process', 'wrapper', 'devops', 'system administration'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/seibert-media/automatix',
     author='Johannes Paul, //SEIBERT/MEDIA GmbH',
     author_email='jpaul@seibert-media.net',
     license='MIT',
     python_requires='>=3.6',
     install_requires=[
         'pyyaml>=5.1',
         'importlib-metadata >= 1.0 ; python_version < "3.8"',
     ],
+    extras_require={
+        'bash completion': 'argcomplete',
+    },
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'automatix=automatix:main',
         ],
     },
     classifiers=[
```

