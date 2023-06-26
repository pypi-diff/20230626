# Comparing `tmp/graphix_ibmq-0.0.1.tar.gz` & `tmp/graphix_ibmq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix_ibmq-0.0.1.tar", last modified: Sun May 21 18:37:08 2023, max compression
+gzip compressed data, was "graphix_ibmq-0.0.2.tar", last modified: Mon Jun 26 21:36:57 2023, max compression
```

## Comparing `graphix_ibmq-0.0.1.tar` & `graphix_ibmq-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-21 18:37:08.921570 graphix_ibmq-0.0.1/
--rw-r--r--   0 ss         (501) staff       (20)    10766 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/LICENSE
--rw-r--r--   0 ss         (501) staff       (20)       99 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/MANIFEST.in
--rw-r--r--   0 ss         (501) staff       (20)     1504 2023-05-21 18:37:08.921216 graphix_ibmq-0.0.1/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)      514 2023-05-21 18:31:28.000000 graphix_ibmq-0.0.1/README.md
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-21 18:37:08.915270 graphix_ibmq-0.0.1/graphix_ibmq/
--rw-r--r--   0 ss         (501) staff       (20)        0 2023-05-21 17:10:39.000000 graphix_ibmq-0.0.1/graphix_ibmq/__init__.py
--rw-r--r--   0 ss         (501) staff       (20)     6900 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/graphix_ibmq/runner.py
--rw-r--r--   0 ss         (501) staff       (20)       22 2023-05-21 18:28:25.000000 graphix_ibmq-0.0.1/graphix_ibmq/version.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-21 18:37:08.919734 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/
--rw-r--r--   0 ss         (501) staff       (20)     1504 2023-05-21 18:37:08.000000 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)      333 2023-05-21 18:37:08.000000 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/SOURCES.txt
--rw-r--r--   0 ss         (501) staff       (20)        1 2023-05-21 18:37:08.000000 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/dependency_links.txt
--rw-r--r--   0 ss         (501) staff       (20)       71 2023-05-21 18:37:08.000000 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/requires.txt
--rw-r--r--   0 ss         (501) staff       (20)       13 2023-05-21 18:37:08.000000 graphix_ibmq-0.0.1/graphix_ibmq.egg-info/top_level.txt
--rw-r--r--   0 ss         (501) staff       (20)       81 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/pyproject.toml
--rw-r--r--   0 ss         (501) staff       (20)       38 2023-05-21 18:37:08.921744 graphix_ibmq-0.0.1/setup.cfg
--rw-r--r--   0 ss         (501) staff       (20)     1578 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/setup.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-21 18:37:08.920308 graphix_ibmq-0.0.1/tests/
--rw-r--r--   0 ss         (501) staff       (20)     1474 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.1/tests/test_ibmq_interface.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-26 21:36:57.635765 graphix_ibmq-0.0.2/
+-rw-r--r--   0 sunami     (501) staff       (20)    10776 2023-06-26 21:34:58.000000 graphix_ibmq-0.0.2/LICENSE
+-rw-r--r--   0 sunami     (501) staff       (20)       99 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.2/MANIFEST.in
+-rw-r--r--   0 sunami     (501) staff       (20)     1635 2023-06-26 21:36:57.635568 graphix_ibmq-0.0.2/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)      645 2023-05-31 04:09:56.000000 graphix_ibmq-0.0.2/README.md
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-26 21:36:57.634045 graphix_ibmq-0.0.2/graphix_ibmq/
+-rw-r--r--   0 sunami     (501) staff       (20)        0 2023-05-21 17:10:39.000000 graphix_ibmq-0.0.2/graphix_ibmq/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)     1036 2023-06-26 21:34:58.000000 graphix_ibmq-0.0.2/graphix_ibmq/clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)    12026 2023-06-26 21:35:52.000000 graphix_ibmq-0.0.2/graphix_ibmq/runner.py
+-rw-r--r--   0 sunami     (501) staff       (20)       22 2023-06-26 21:35:11.000000 graphix_ibmq-0.0.2/graphix_ibmq/version.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-26 21:36:57.635130 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/
+-rw-r--r--   0 sunami     (501) staff       (20)     1635 2023-06-26 21:36:57.000000 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)      358 2023-06-26 21:36:57.000000 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/SOURCES.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        1 2023-06-26 21:36:57.000000 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/dependency_links.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       71 2023-06-26 21:36:57.000000 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/requires.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       13 2023-06-26 21:36:57.000000 graphix_ibmq-0.0.2/graphix_ibmq.egg-info/top_level.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       81 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.2/pyproject.toml
+-rw-r--r--   0 sunami     (501) staff       (20)       38 2023-06-26 21:36:57.635832 graphix_ibmq-0.0.2/setup.cfg
+-rw-r--r--   0 sunami     (501) staff       (20)     1578 2023-05-21 09:43:10.000000 graphix_ibmq-0.0.2/setup.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-26 21:36:57.635306 graphix_ibmq-0.0.2/tests/
+-rw-r--r--   0 sunami     (501) staff       (20)     1329 2023-05-31 04:09:56.000000 graphix_ibmq-0.0.2/tests/test_ibmq_interface.py
```

### Comparing `graphix_ibmq-0.0.1/LICENSE` & `graphix_ibmq-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2022-2023 Shinichi Sunami
+   Copyright 2023 Daichi Sasaki, Shinichi Sunami
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `graphix_ibmq-0.0.1/PKG-INFO` & `graphix_ibmq-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix_ibmq
-Version: 0.0.1
+Version: 0.0.2
 Summary: IBMQ interface for graphix library, the MBQC compiler 
 Home-page: https://graphix.readthedocs.io
 Author: Daichi Sasaki, Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Daichi Sasaki, Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -21,14 +21,17 @@
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Graphix IBMQ interface
 
+![PyPI](https://img.shields.io/pypi/v/graphix-ibmq)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix-ibmq)
+
 Provides an interface to run MBQC pattern (`graphix.Pattern`) on IBM quantum devices as well as the Aer simulators.
 
 Requires [graphix](https://github.com/TeamGraphix/graphix) to generate the measurement pattern.
 
 ## Installation
 install with `pip`
 ```
```

### Comparing `graphix_ibmq-0.0.1/graphix_ibmq.egg-info/PKG-INFO` & `graphix_ibmq-0.0.2/graphix_ibmq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix-ibmq
-Version: 0.0.1
+Version: 0.0.2
 Summary: IBMQ interface for graphix library, the MBQC compiler 
 Home-page: https://graphix.readthedocs.io
 Author: Daichi Sasaki, Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Daichi Sasaki, Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -21,14 +21,17 @@
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Graphix IBMQ interface
 
+![PyPI](https://img.shields.io/pypi/v/graphix-ibmq)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix-ibmq)
+
 Provides an interface to run MBQC pattern (`graphix.Pattern`) on IBM quantum devices as well as the Aer simulators.
 
 Requires [graphix](https://github.com/TeamGraphix/graphix) to generate the measurement pattern.
 
 ## Installation
 install with `pip`
 ```
```

### Comparing `graphix_ibmq-0.0.1/setup.py` & `graphix_ibmq-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `graphix_ibmq-0.0.1/tests/test_ibmq_interface.py` & `graphix_ibmq-0.0.2/tests/test_ibmq_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
 import numpy as np
-from qiskit import Aer, transpile
 from graphix_ibmq.runner import IBMQBackend
 import tests.random_circuit as rc
 
 
 def modify_statevector(statevector, output_qubit):
     N = round(np.log2(len(statevector)))
     new_statevector = np.zeros(2 ** len(output_qubit), dtype=complex)
@@ -23,19 +22,17 @@
         depth = 5
         pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
         circuit = rc.generate_gate(nqubits, depth, pairs)
         pattern = circuit.transpile()
         state = pattern.simulate_pattern()
 
         ibmq_backend = IBMQBackend(pattern)
-        simulator = Aer.get_backend("aer_simulator")
         ibmq_backend.to_qiskit(save_statevector=True)
-        qiskit_circuit = transpile(ibmq_backend.circ, simulator)
-        sim_result = simulator.run(qiskit_circuit).result()
-        state_qiskit = sim_result.get_statevector(qiskit_circuit)
+        sim_result = ibmq_backend.simulate(format_result=False)
+        state_qiskit = sim_result.get_statevector(ibmq_backend.circ)
         state_qiskit_mod = modify_statevector(state_qiskit, ibmq_backend.circ_output)
 
         np.testing.assert_almost_equal(np.abs(np.dot(state_qiskit_mod.conjugate(), state.flatten())), 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

