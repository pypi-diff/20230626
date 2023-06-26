# Comparing `tmp/PennyLane-qiskit-0.8.2.tar.gz` & `tmp/PennyLane-qiskit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PennyLane-qiskit-0.8.2.tar", last modified: Tue Mar 17 17:02:12 2020, max compression
+gzip compressed data, was "dist/PennyLane-qiskit-0.9.0.tar", last modified: Fri May 15 16:09:19 2020, max compression
```

## Comparing `PennyLane-qiskit-0.8.2.tar` & `PennyLane-qiskit-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/
--rw-r--r--   0 antal     (1000) antal     (1000)    13515 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PKG-INFO
--rw-r--r--   0 antal     (1000) antal     (1000)     2746 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/setup.py
--rw-r--r--   0 antal     (1000) antal     (1000)    10179 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/README.rst
--rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/setup.cfg
--rw-r--r--   0 antal     (1000) antal     (1000)       43 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/requirements.txt
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/
--rw-r--r--   0 antal     (1000) antal     (1000)     9734 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/converter.py
--rw-r--r--   0 antal     (1000) antal     (1000)      691 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/_version.py
--rw-r--r--   0 antal     (1000) antal     (1000)    19964 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/qiskit_device.py
--rw-r--r--   0 antal     (1000) antal     (1000)     4144 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/ibmq.py
--rw-r--r--   0 antal     (1000) antal     (1000)     2908 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/basic_aer.py
--rw-r--r--   0 antal     (1000) antal     (1000)     3029 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/aer.py
--rw-r--r--   0 antal     (1000) antal     (1000)      822 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/pennylane_qiskit/__init__.py
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/
--rw-r--r--   0 antal     (1000) antal     (1000)    13515 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 antal     (1000) antal     (1000)      283 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/entry_points.txt
--rw-r--r--   0 antal     (1000) antal     (1000)        1 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       36 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/requires.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       17 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/top_level.txt
--rw-r--r--   0 antal     (1000) antal     (1000)      491 2020-03-17 17:02:12.000000 PennyLane-qiskit-0.8.2/PennyLane_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       46 2020-03-17 16:52:58.000000 PennyLane-qiskit-0.8.2/MANIFEST.in
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 16:09:19.839513 PennyLane-qiskit-0.9.0/
+-rw-r--r--   0 antal     (1000) antal     (1000)       46 2020-02-04 18:40:36.000000 PennyLane-qiskit-0.9.0/MANIFEST.in
+-rw-r--r--   0 antal     (1000) antal     (1000)     7851 2020-05-15 16:09:19.839513 PennyLane-qiskit-0.9.0/PKG-INFO
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 16:09:19.839513 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/
+-rw-r--r--   0 antal     (1000) antal     (1000)     7851 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 antal     (1000) antal     (1000)      491 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)        1 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)      283 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/entry_points.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)      126 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/requires.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)       17 2020-05-15 16:09:19.000000 PennyLane-qiskit-0.9.0/PennyLane_qiskit.egg-info/top_level.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)     5593 2020-04-16 17:17:30.000000 PennyLane-qiskit-0.9.0/README.rst
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 16:09:19.839513 PennyLane-qiskit-0.9.0/pennylane_qiskit/
+-rw-r--r--   0 antal     (1000) antal     (1000)      822 2020-02-04 18:40:36.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/__init__.py
+-rw-r--r--   0 antal     (1000) antal     (1000)      691 2020-05-15 13:52:00.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/_version.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     2358 2020-04-16 17:17:30.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/aer.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     2222 2020-04-16 17:17:30.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/basic_aer.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     9625 2020-04-21 21:33:54.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/converter.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     3954 2020-04-21 21:33:54.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/ibmq.py
+-rw-r--r--   0 antal     (1000) antal     (1000)    12103 2020-05-15 13:52:00.000000 PennyLane-qiskit-0.9.0/pennylane_qiskit/qiskit_device.py
+-rw-r--r--   0 antal     (1000) antal     (1000)      114 2020-05-15 13:52:00.000000 PennyLane-qiskit-0.9.0/requirements.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-05-15 16:09:19.839513 PennyLane-qiskit-0.9.0/setup.cfg
+-rw-r--r--   0 antal     (1000) antal     (1000)     2949 2020-05-15 16:03:06.000000 PennyLane-qiskit-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PennyLane-qiskit-0.8.2/setup.py` & `PennyLane-qiskit-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 with open("pennylane_qiskit/_version.py") as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 requirements = [
-    "qiskit>=0.16",
-    "pennylane>=0.8.1",
-    "numpy"
+    "qiskit>=0.19.1",
+    "pennylane>=0.9.0",
+    "numpy",
+    "networkx>=2.2;python_version>'3.5'",
+    # Networkx 2.4 is the final version with python 3.5 support.
+    "networkx>=2.2,<2.4;python_version=='3.5'",
 ]
 
 info = {
     'name': 'PennyLane-qiskit',
     'version': version,
     'maintainer': 'Xanadu',
     'maintainer_email': 'software@xanadu.ai',
@@ -71,12 +74,13 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3 :: Only',
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 setup(classifiers=classifiers, **(info))
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/converter.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,14 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
-QuanctumCircuit converter module
-================================
-
-.. currentmodule:: pennylane_qiskit.load
-
 This module contains functions for converting Qiskit QuantumCircuit objects
 into PennyLane circuit templates.
 """
 from typing import Dict, Any
 import warnings
 
 import numpy as np
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/_version.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/ibmq.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/ibmq.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,17 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-IBMQ Device
-===========
-
-**Module name:** :mod:`pennylane_qiskit.ibmq`
-
-.. currentmodule:: pennylane_qiskit.ibmq
-
 This module contains the :class:`~.IBMQDevice` class, a PennyLane device that allows
 evaluation and differentiation of IBM Q's Quantum Processing Units (QPUs)
 using PennyLane.
-
-Classes
--------
-
-.. autosummary::
-   IBMQDevice
-
-Code details
-~~~~~~~~~~~~
 """
 import os
 
 from qiskit import IBMQ
 from qiskit.providers.ibmq.exceptions import IBMQAccountError
 
 from .qiskit_device import QiskitDevice
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/basic_aer.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/basic_aer.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,52 +8,33 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-BasicAer Device
-===============
-
-**Module name:** :mod:`pennylane_qiskit.basic_aer`
-
-.. currentmodule:: pennylane_qiskit.basic_aer
-
 This module contains the :class:`~.BasicAerDevice` class, a PennyLane device that allows
 evaluation and differentiation of Qiskit Terra's BasicAer simulator
 using PennyLane.
-
-Classes
--------
-
-.. autosummary::
-   BasicAerDevice
-
-Code details
-~~~~~~~~~~~~
 """
 import qiskit
 
 from .qiskit_device import QiskitDevice
 
 
 class BasicAerDevice(QiskitDevice):
     """A PennyLane device for the native Python Qiskit simulator.
 
     Please see the `Qiskit documentations <https://qiskit.org/documentation/>`_
     for more details.
 
     A range of :code:`backend_options` can be given in as kwargs that will be passed to the simulator.
 
-    For details on the backends, please check out
-
-        * `qasm_simulator <https://qiskit.org/documentation/api/qiskit.providers.aer.QasmSimulator.html?highlight=qasm%20simulator#qiskit.providers.aer.QasmSimulator>`_
-        * `statevector_simulator  <https://qiskit.org/documentation/api/qiskit.providers.aer.backends.StatevectorSimulator.html?highlight=statevector%20simulator#qiskit.providers.aer.backends.StatevectorSimulator>`_
-        * `unitary_simulator  <https://qiskit.org/documentation/api/qiskit.providers.aer.backends.UnitarySimulator.html?highlight=unitary%20simulator#qiskit.providers.aer.backends.UnitarySimulator>`_
+    For more information on backends, please visit the
+    `Basic Aer provider documentation <https://qiskit.org/documentation/apidoc/providers_basicaer.html>`_.
 
     Args:
         wires (int): The number of qubits of the device
         backend (str): the desired backend
         shots (int): number of circuit evaluations/random samples used
             to estimate expectation values and variances of observables
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/aer.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/aer.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,52 +8,33 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-Aer Device
-==========
-
-**Module name:** :mod:`pennylane_qiskit.aer`
-
-.. currentmodule:: pennylane_qiskit.aer
-
 This module contains the :class:`~.AerDevice` class, a PennyLane device that allows
 evaluation and differentiation of Qiskit Aer's C++ simulator
 using PennyLane.
-
-Classes
--------
-
-.. autosummary::
-   AerDevice
-
-Code details
-~~~~~~~~~~~~
 """
 import qiskit
 
 from .qiskit_device import QiskitDevice
 
 
 class AerDevice(QiskitDevice):
     """A PennyLane device for the C++ Qiskit Aer simulator.
 
     Please refer to the `Qiskit documentation <https://qiskit.org/documentation/>`_ for
     for further information to the noise model and backend options.
 
     A range of :code:`backend_options` can be given as kwargs that will be passed to the simulator.
 
-    For details on the backends, please check out
-
-        * `qasm_simulator <https://qiskit.org/documentation/api/qiskit.providers.aer.QasmSimulator.html?highlight=qasm%20simulator#qiskit.providers.aer.QasmSimulator>`_
-        * `statevector_simulator  <https://qiskit.org/documentation/api/qiskit.providers.aer.backends.StatevectorSimulator.html?highlight=statevector%20simulator#qiskit.providers.aer.backends.StatevectorSimulator>`_
-        * `unitary_simulator  <https://qiskit.org/documentation/api/qiskit.providers.aer.backends.UnitarySimulator.html?highlight=unitary%20simulator#qiskit.providers.aer.backends.UnitarySimulator>`_
+    For more information on backends, please visit the
+    `Aer provider documentation <https://qiskit.org/documentation/apidoc/aer_provider.html>`_.
 
     Args:
         wires (int): The number of qubits of the device
         backend (str): the desired backend
         shots (int): number of circuit evaluations/random samples used
             to estimate expectation values and variances of observables
```

### Comparing `PennyLane-qiskit-0.8.2/pennylane_qiskit/__init__.py` & `PennyLane-qiskit-0.9.0/pennylane_qiskit/__init__.py`

 * *Files identical despite different names*

