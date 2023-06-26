# Comparing `tmp/PennyLane-PQ-0.6.0.tar.gz` & `tmp/PennyLane-PQ-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PennyLane-PQ-0.6.0.tar", last modified: Fri Oct 18 22:48:07 2019, max compression
+gzip compressed data, was "dist/PennyLane-PQ-0.8.0.tar", last modified: Thu Jan 30 16:01:17 2020, max compression
```

## Comparing `PennyLane-PQ-0.6.0.tar` & `PennyLane-PQ-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/
--rw-rw-r--   0 josh      (1000) josh      (1000)     6978 2019-08-08 08:27:38.000000 PennyLane-PQ-0.6.0/README.rst
--rw-r--r--   0 josh      (1000) josh      (1000)     2402 2019-10-18 22:46:29.000000 PennyLane-PQ-0.6.0/setup.py
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/pennylane_pq/
--rw-r--r--   0 josh      (1000) josh      (1000)    24171 2019-10-18 22:46:29.000000 PennyLane-PQ-0.6.0/pennylane_pq/devices.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     3129 2018-11-14 05:22:20.000000 PennyLane-PQ-0.6.0/pennylane_pq/ops.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1208 2018-11-14 05:22:20.000000 PennyLane-PQ-0.6.0/pennylane_pq/expval.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     5788 2019-06-26 04:27:30.000000 PennyLane-PQ-0.6.0/pennylane_pq/pqops.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      966 2018-11-14 05:22:20.000000 PennyLane-PQ-0.6.0/pennylane_pq/__init__.py
--rw-r--r--   0 josh      (1000) josh      (1000)      691 2019-10-18 22:46:29.000000 PennyLane-PQ-0.6.0/pennylane_pq/_version.py
--rw-r--r--   0 josh      (1000) josh      (1000)     9351 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/PKG-INFO
--rw-r--r--   0 josh      (1000) josh      (1000)       38 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/setup.cfg
-drwxr-xr-x   0 josh      (1000) josh      (1000)        0 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)       13 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/top_level.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)      376 2019-10-18 22:48:07.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2019-10-18 22:48:06.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)     9351 2019-10-18 22:48:06.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      181 2019-10-18 22:48:06.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/entry_points.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       31 2019-10-18 22:48:06.000000 PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/requires.txt
+drwxr-xr-x   0 antal     (1001) antal     (1001)        0 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/
+-rw-r--r--   0 antal     (1001) antal     (1001)     9351 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PKG-INFO
+drwxr-xr-x   0 antal     (1001) antal     (1001)        0 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/
+-rw-r--r--   0 antal     (1001) antal     (1001)     9351 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/PKG-INFO
+-rw-r--r--   0 antal     (1001) antal     (1001)      376 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/SOURCES.txt
+-rw-r--r--   0 antal     (1001) antal     (1001)        1 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/dependency_links.txt
+-rw-r--r--   0 antal     (1001) antal     (1001)      181 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/entry_points.txt
+-rw-r--r--   0 antal     (1001) antal     (1001)       31 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/requires.txt
+-rw-r--r--   0 antal     (1001) antal     (1001)       13 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/top_level.txt
+-rw-r--r--   0 antal     (1001) antal     (1001)     6978 2019-10-18 19:57:14.000000 PennyLane-PQ-0.8.0/README.rst
+drwxr-xr-x   0 antal     (1001) antal     (1001)        0 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/pennylane_pq/
+-rw-r--r--   0 antal     (1001) antal     (1001)      966 2019-10-18 19:57:15.000000 PennyLane-PQ-0.8.0/pennylane_pq/__init__.py
+-rw-r--r--   0 antal     (1001) antal     (1001)      691 2020-01-30 15:55:15.000000 PennyLane-PQ-0.8.0/pennylane_pq/_version.py
+-rw-r--r--   0 antal     (1001) antal     (1001)    24189 2020-01-30 15:34:17.000000 PennyLane-PQ-0.8.0/pennylane_pq/devices.py
+-rw-r--r--   0 antal     (1001) antal     (1001)     1208 2019-10-18 19:57:15.000000 PennyLane-PQ-0.8.0/pennylane_pq/expval.py
+-rw-r--r--   0 antal     (1001) antal     (1001)     3129 2019-10-18 19:57:15.000000 PennyLane-PQ-0.8.0/pennylane_pq/ops.py
+-rw-r--r--   0 antal     (1001) antal     (1001)     5787 2020-01-30 15:55:15.000000 PennyLane-PQ-0.8.0/pennylane_pq/pqops.py
+-rw-r--r--   0 antal     (1001) antal     (1001)       38 2020-01-30 16:01:17.000000 PennyLane-PQ-0.8.0/setup.cfg
+-rw-r--r--   0 antal     (1001) antal     (1001)     2402 2019-11-20 14:50:32.000000 PennyLane-PQ-0.8.0/setup.py
```

### Comparing `PennyLane-PQ-0.6.0/README.rst` & `PennyLane-PQ-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `PennyLane-PQ-0.6.0/setup.py` & `PennyLane-PQ-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/devices.py` & `PennyLane-PQ-0.8.0/pennylane_pq/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     """
     name = 'ProjectQ PennyLane plugin'
     short_name = 'projectq'
     pennylane_requires = '>=0.4.0'
     version = '0.4.2'
     plugin_version = __version__
     author = 'Christian Gogolin'
-    _capabilities = {'backend': list(["Simulator", "ClassicalSimulator", "IBMBackend"])}
+    _capabilities = {'backend': list(["Simulator", "ClassicalSimulator", "IBMBackend"]), 'model': 'qubit'}
 
     @abc.abstractproperty
     def _operation_map(self):
         raise NotImplementedError
 
     @abc.abstractproperty
     def _observable_map(self):
```

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/ops.py` & `PennyLane-PQ-0.8.0/pennylane_pq/ops.py`

 * *Files identical despite different names*

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/expval.py` & `PennyLane-PQ-0.8.0/pennylane_pq/expval.py`

 * *Files identical despite different names*

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/pqops.py` & `PennyLane-PQ-0.8.0/pennylane_pq/pqops.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     ProjectQ does not currently have a real arbitrary QubitUnitary gate,
     but it allows to directly set the matrix of single qubit gates and
     can then still decompose them into the elementary gates set, so we
     do this here.
     """
     def __new__(*par):
         unitary_gate = BasicProjectQMatrixGate(par[0].__name__)
-        unitary_gate.matrix = np.matrix(par[1])
+        unitary_gate.matrix = np.array(par[1])
         return unitary_gate
 
 class BasisState(BasicProjectQGate, SelfInverseGate): # pylint: disable=too-few-public-methods
     """Class for the BasisState preparation.
 
     ProjectQ does not currently have a dedicated gate for this, so we implement it here.
     """
```

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/__init__.py` & `PennyLane-PQ-0.8.0/pennylane_pq/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-PQ-0.6.0/pennylane_pq/_version.py` & `PennyLane-PQ-0.8.0/pennylane_pq/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = '0.6.0'
+__version__ = '0.8.0'
```

### Comparing `PennyLane-PQ-0.6.0/PKG-INFO` & `PennyLane-PQ-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PennyLane-PQ
-Version: 0.6.0
+Version: 0.8.0
 Summary: PennyLane plugin for ProjectQ
 Home-page: https://github.com/XanaduAI/PennyLane-PQ
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane ProjectQ Plugin
         #########################
```

### Comparing `PennyLane-PQ-0.6.0/PennyLane_PQ.egg-info/PKG-INFO` & `PennyLane-PQ-0.8.0/PennyLane_PQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PennyLane-PQ
-Version: 0.6.0
+Version: 0.8.0
 Summary: PennyLane plugin for ProjectQ
 Home-page: https://github.com/XanaduAI/PennyLane-PQ
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane ProjectQ Plugin
         #########################
```

