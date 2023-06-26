# Comparing `tmp/PennyLane-Cirq-0.8.0.tar.gz` & `tmp/PennyLane-Cirq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PennyLane-Cirq-0.8.0.tar", last modified: Tue Feb  4 21:10:40 2020, max compression
+gzip compressed data, was "dist/PennyLane-Cirq-0.9.0.tar", last modified: Fri May 15 19:18:47 2020, max compression
```

## Comparing `PennyLane-Cirq-0.8.0.tar` & `PennyLane-Cirq-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/
--rw-r--r--   0 antal     (1000) antal     (1000)     5534 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/PKG-INFO
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/
--rw-r--r--   0 antal     (1000) antal     (1000)     5534 2020-02-04 21:10:39.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/PKG-INFO
--rw-r--r--   0 antal     (1000) antal     (1000)      423 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/SOURCES.txt
--rw-r--r--   0 antal     (1000) antal     (1000)        1 2020-02-04 21:10:39.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/dependency_links.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       69 2020-02-04 21:10:39.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/entry_points.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       15 2020-02-04 21:10:39.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/requires.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       15 2020-02-04 21:10:39.000000 PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/top_level.txt
--rw-r--r--   0 antal     (1000) antal     (1000)     3625 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/README.rst
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/
--rw-r--r--   0 antal     (1000) antal     (1000)      832 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/__init__.py
--rw-r--r--   0 antal     (1000) antal     (1000)      691 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/_version.py
--rw-r--r--   0 antal     (1000) antal     (1000)     7600 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/cirq_device.py
--rw-r--r--   0 antal     (1000) antal     (1000)     3461 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/cirq_interface.py
--rw-r--r--   0 antal     (1000) antal     (1000)     3709 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/ops.py
--rw-r--r--   0 antal     (1000) antal     (1000)     6608 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/pennylane_cirq/simulator_device.py
--rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-02-04 21:10:40.000000 PennyLane-Cirq-0.8.0/setup.cfg
--rw-r--r--   0 antal     (1000) antal     (1000)     2493 2020-02-04 21:01:29.000000 PennyLane-Cirq-0.8.0/setup.py
+drwxr-xr-x   0 theodor   (1000) theodor   (1000)        0 2020-05-15 19:18:47.000000 PennyLane-Cirq-0.9.0/
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     7241 2020-05-15 19:18:47.000000 PennyLane-Cirq-0.9.0/PKG-INFO
+drwxr-xr-x   0 theodor   (1000) theodor   (1000)        0 2020-05-15 19:18:47.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     7241 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/PKG-INFO
+-rw-r--r--   0 theodor   (1000) theodor   (1000)      423 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/SOURCES.txt
+-rw-r--r--   0 theodor   (1000) theodor   (1000)        1 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/dependency_links.txt
+-rw-r--r--   0 theodor   (1000) theodor   (1000)      132 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/entry_points.txt
+-rw-r--r--   0 theodor   (1000) theodor   (1000)       15 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/requires.txt
+-rw-r--r--   0 theodor   (1000) theodor   (1000)       15 2020-05-15 19:18:46.000000 PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/top_level.txt
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     4948 2020-05-15 19:17:13.000000 PennyLane-Cirq-0.9.0/README.rst
+drwxr-xr-x   0 theodor   (1000) theodor   (1000)        0 2020-05-15 19:18:47.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/
+-rw-r--r--   0 theodor   (1000) theodor   (1000)      820 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/__init__.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)      691 2020-05-15 19:17:13.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/_version.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     7574 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/cirq_device.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     2958 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/cirq_operation.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     3024 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/ops.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     9878 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/pennylane_cirq/simulator_device.py
+-rw-r--r--   0 theodor   (1000) theodor   (1000)       38 2020-05-15 19:18:47.000000 PennyLane-Cirq-0.9.0/setup.cfg
+-rw-r--r--   0 theodor   (1000) theodor   (1000)     2609 2020-05-15 18:04:09.000000 PennyLane-Cirq-0.9.0/setup.py
```

### Comparing `PennyLane-Cirq-0.8.0/PKG-INFO` & `PennyLane-Cirq-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: PennyLane-Cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: PennyLane plugin for Cirq
 Home-page: http://xanadu.ai
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
-Description: PennyLane Cirq Plugin
-        #########################
+Description: PennyLane-Cirq Plugin
+        ######################
         
         .. image:: https://img.shields.io/travis/com/XanaduAI/pennylane-cirq/master.svg
             :alt: Travis
             :target: https://travis-ci.com/XanaduAI/pennylane-cirq
         
         .. image:: https://img.shields.io/codecov/c/github/xanaduai/pennylane-cirq/master.svg
             :alt: Codecov coverage
@@ -25,112 +25,160 @@
             :alt: Read the Docs
             :target: https://pennylane-cirq.readthedocs.io
         
         .. image:: https://img.shields.io/pypi/v/pennylane-cirq.svg
             :alt: PyPI
             :target: https://pypi.org/project/pennylane-cirq
         
+        .. image:: https://github.com/XanaduAI/pennylane-cirq/blob/master/doc/_static/puzzle_cirq.png?raw=true
+            :align: center
+            :width: 200px
+            :target: javascript:void(0);
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine
+        |
+        
+        .. header-start-inclusion-marker-do-not-remove
+        
+        The PennyLane-Cirq plugin integrates the Cirq quantum computing framework with PennyLane's
+        quantum machine learning capabilities.
+        
+        `PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine
         learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
         
-        `Cirq <https://github.com/quantumlib/Cirq>`_ is a Python library for writing, manipulating, and optimizing quantum circuits and running them against quantum computers and simulators.
+        `Cirq <https://github.com/quantumlib/Cirq>`__ is a software library for quantum computing.
         
-        This PennyLane plugin allows to use both the software and hardware backends of Cirq as devices for PennyLane.
+        .. header-end-inclusion-marker-do-not-remove
         
+        The plugin documentation can be found here: `<https://pennylane-cirq.readthedocs.io/en/latest/>`__.
         
         Features
         ========
         
-        * Access to Cirq's simulator backend via the `cirq.simulator` device
+        * Provides access to Cirq's simulator backend via the ``cirq.simulator`` device
         
         * Support for all PennyLane core functionality
         
+        .. installation-start-inclusion-marker-do-not-remove
         
         Installation
         ============
         
-        Plugin Name requires both PennyLane and Cirq. It can be installed via ``pip``:
+        This plugin requires Python version 3.6 or above, as well as PennyLane
+        and Cirq. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+        
+        .. code-block:: bash
+        
+            $ pip install pennylane-cirq
+        
+        Alternatively, you can install PennyLane-Cirq from the `source code <https://github.com/XanaduAI/pennylane-cirq>`__
+        by navigating to the top directory and running:
+        
+        .. code-block:: bash
+        
+        	$ python setup.py install
+        
+        Dependencies
+        ~~~~~~~~~~~~
+        
+        PennyLane-Cirq requires the following libraries be installed:
+        
+        * `Python <http://python.org/>`__ >= 3.6
+        
+        as well as the following Python packages:
+        
+        * `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.9
+        * `Cirq <https://cirq.readthedocs.io/>`__ >= 0.7
+        
+        
+        If you currently do not have Python 3 installed, we recommend
+        `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
+        for scientific computation.
+        
+        
+        Tests
+        ~~~~~
+        
+        To test that the PennyLane-Cirq plugin is working correctly you can run
         
         .. code-block:: bash
         
-            $ python -m pip install pennylane-cirq
+            $ make test
         
+        in the source folder.
         
-        Getting started
-        ===============
+        Documentation
+        ~~~~~~~~~~~~~
         
-        Once Pennylane Cirq is installed, the provided Cirq devices can be accessed straight
-        away in PennyLane.
+        To build the HTML documentation, go to the top-level directory and run:
         
-        You can instantiate these devices for PennyLane as follows:
+        .. code-block:: bash
         
-        .. code-block:: python
+          $ make docs
         
-            import pennylane as qml
-            dev = qml.device('cirq.simulator', wires=2, shots=100, analytic=True)
         
-        These devices can then be used just like other devices for the definition and evaluation of
-        QNodes within PennyLane. For more details, see the
-        `plugin usage guide <https://pennylane-cirq.readthedocs.io/en/latest/usage.html>`_ and refer
-        to the PennyLane documentation.
+        The documentation can then be found in the ``doc/_build/html/`` directory.
         
+        .. installation-end-inclusion-marker-do-not-remove
         
         Contributing
         ============
         
-        We welcome contributions - simply fork the Plugin Name repository, and then make a
-        `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
-        All contributors to PennyLane-Cirq will be listed as authors on the releases.
-        
-        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool
-        projects or applications built on PennyLane and Cirq.
+        We welcome contributions - simply fork the repository of this plugin, and then make a
+        `pull request <https://help.github.com/articles/about-pull-requests/>`__ containing your contribution.
+        All contributers to this plugin will be listed as authors on the releases.
         
+        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool projects
+        or applications built on PennyLane.
         
         Authors
         =======
         
-        Johannes Jakob Meyer
-        
-        If you are doing research using PennyLane, please cite our papers:
+        PennyLane-Cirq is the work of `many contributors <https://github.com/XanaduAI/pennylane-cirq/graphs/contributors>`__.
         
-            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
-            *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
-            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
+        If you are doing research using PennyLane and PennyLane-Cirq, please cite `our paper <https://arxiv.org/abs/1811.04968>`__:
         
-            Maria Schuld, Ville Bergholm, Christian Gogolin, Josh Izaac, and Nathan Killoran.
-            *Evaluating analytic gradients on quantum hardware.* 2018.
-            `Phys. Rev. A 99, 032331 <https://journals.aps.org/pra/abstract/10.1103/PhysRevA.99.032331>`_
+            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+            Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+            Zeyue Niu, Antal Száva, and Nathan Killoran.
+            *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
         
+        .. support-start-inclusion-marker-do-not-remove
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane-cirq
         - **Issue Tracker:** https://github.com/XanaduAI/pennylane-cirq/issues
+        - **PennyLane Forum:** https://discuss.pennylane.ai
         
-        If you are having issues, please let us know by posting the issue on our GitHub issue tracker.
+        If you are having issues, please let us know by posting the issue on our Github issue tracker, or
+        by asking a question in the forum.
         
+        .. support-end-inclusion-marker-do-not-remove
+        .. license-start-inclusion-marker-do-not-remove
         
         License
         =======
         
-        Plugin Name is **free** and **open source**, released under the Apache License, Version 2.0.
+        The PennyLane-Cirq plugin is **free** and **open source**, released under
+        the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__.
+        
+        .. license-end-inclusion-marker-do-not-remove
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pennylane_cirq
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PennyLane-Cirq-0.8.0/PennyLane_Cirq.egg-info/PKG-INFO` & `PennyLane-Cirq-0.9.0/PennyLane_Cirq.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: PennyLane-Cirq
-Version: 0.8.0
+Version: 0.9.0
 Summary: PennyLane plugin for Cirq
 Home-page: http://xanadu.ai
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
-Description: PennyLane Cirq Plugin
-        #########################
+Description: PennyLane-Cirq Plugin
+        ######################
         
         .. image:: https://img.shields.io/travis/com/XanaduAI/pennylane-cirq/master.svg
             :alt: Travis
             :target: https://travis-ci.com/XanaduAI/pennylane-cirq
         
         .. image:: https://img.shields.io/codecov/c/github/xanaduai/pennylane-cirq/master.svg
             :alt: Codecov coverage
@@ -25,112 +25,160 @@
             :alt: Read the Docs
             :target: https://pennylane-cirq.readthedocs.io
         
         .. image:: https://img.shields.io/pypi/v/pennylane-cirq.svg
             :alt: PyPI
             :target: https://pypi.org/project/pennylane-cirq
         
+        .. image:: https://github.com/XanaduAI/pennylane-cirq/blob/master/doc/_static/puzzle_cirq.png?raw=true
+            :align: center
+            :width: 200px
+            :target: javascript:void(0);
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine
+        |
+        
+        .. header-start-inclusion-marker-do-not-remove
+        
+        The PennyLane-Cirq plugin integrates the Cirq quantum computing framework with PennyLane's
+        quantum machine learning capabilities.
+        
+        `PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine
         learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
         
-        `Cirq <https://github.com/quantumlib/Cirq>`_ is a Python library for writing, manipulating, and optimizing quantum circuits and running them against quantum computers and simulators.
+        `Cirq <https://github.com/quantumlib/Cirq>`__ is a software library for quantum computing.
         
-        This PennyLane plugin allows to use both the software and hardware backends of Cirq as devices for PennyLane.
+        .. header-end-inclusion-marker-do-not-remove
         
+        The plugin documentation can be found here: `<https://pennylane-cirq.readthedocs.io/en/latest/>`__.
         
         Features
         ========
         
-        * Access to Cirq's simulator backend via the `cirq.simulator` device
+        * Provides access to Cirq's simulator backend via the ``cirq.simulator`` device
         
         * Support for all PennyLane core functionality
         
+        .. installation-start-inclusion-marker-do-not-remove
         
         Installation
         ============
         
-        Plugin Name requires both PennyLane and Cirq. It can be installed via ``pip``:
+        This plugin requires Python version 3.6 or above, as well as PennyLane
+        and Cirq. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+        
+        .. code-block:: bash
+        
+            $ pip install pennylane-cirq
+        
+        Alternatively, you can install PennyLane-Cirq from the `source code <https://github.com/XanaduAI/pennylane-cirq>`__
+        by navigating to the top directory and running:
+        
+        .. code-block:: bash
+        
+        	$ python setup.py install
+        
+        Dependencies
+        ~~~~~~~~~~~~
+        
+        PennyLane-Cirq requires the following libraries be installed:
+        
+        * `Python <http://python.org/>`__ >= 3.6
+        
+        as well as the following Python packages:
+        
+        * `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.9
+        * `Cirq <https://cirq.readthedocs.io/>`__ >= 0.7
+        
+        
+        If you currently do not have Python 3 installed, we recommend
+        `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
+        for scientific computation.
+        
+        
+        Tests
+        ~~~~~
+        
+        To test that the PennyLane-Cirq plugin is working correctly you can run
         
         .. code-block:: bash
         
-            $ python -m pip install pennylane-cirq
+            $ make test
         
+        in the source folder.
         
-        Getting started
-        ===============
+        Documentation
+        ~~~~~~~~~~~~~
         
-        Once Pennylane Cirq is installed, the provided Cirq devices can be accessed straight
-        away in PennyLane.
+        To build the HTML documentation, go to the top-level directory and run:
         
-        You can instantiate these devices for PennyLane as follows:
+        .. code-block:: bash
         
-        .. code-block:: python
+          $ make docs
         
-            import pennylane as qml
-            dev = qml.device('cirq.simulator', wires=2, shots=100, analytic=True)
         
-        These devices can then be used just like other devices for the definition and evaluation of
-        QNodes within PennyLane. For more details, see the
-        `plugin usage guide <https://pennylane-cirq.readthedocs.io/en/latest/usage.html>`_ and refer
-        to the PennyLane documentation.
+        The documentation can then be found in the ``doc/_build/html/`` directory.
         
+        .. installation-end-inclusion-marker-do-not-remove
         
         Contributing
         ============
         
-        We welcome contributions - simply fork the Plugin Name repository, and then make a
-        `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
-        All contributors to PennyLane-Cirq will be listed as authors on the releases.
-        
-        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool
-        projects or applications built on PennyLane and Cirq.
+        We welcome contributions - simply fork the repository of this plugin, and then make a
+        `pull request <https://help.github.com/articles/about-pull-requests/>`__ containing your contribution.
+        All contributers to this plugin will be listed as authors on the releases.
         
+        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool projects
+        or applications built on PennyLane.
         
         Authors
         =======
         
-        Johannes Jakob Meyer
-        
-        If you are doing research using PennyLane, please cite our papers:
+        PennyLane-Cirq is the work of `many contributors <https://github.com/XanaduAI/pennylane-cirq/graphs/contributors>`__.
         
-            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
-            *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
-            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
+        If you are doing research using PennyLane and PennyLane-Cirq, please cite `our paper <https://arxiv.org/abs/1811.04968>`__:
         
-            Maria Schuld, Ville Bergholm, Christian Gogolin, Josh Izaac, and Nathan Killoran.
-            *Evaluating analytic gradients on quantum hardware.* 2018.
-            `Phys. Rev. A 99, 032331 <https://journals.aps.org/pra/abstract/10.1103/PhysRevA.99.032331>`_
+            Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+            Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+            Zeyue Niu, Antal Száva, and Nathan Killoran.
+            *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
         
+        .. support-start-inclusion-marker-do-not-remove
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane-cirq
         - **Issue Tracker:** https://github.com/XanaduAI/pennylane-cirq/issues
+        - **PennyLane Forum:** https://discuss.pennylane.ai
         
-        If you are having issues, please let us know by posting the issue on our GitHub issue tracker.
+        If you are having issues, please let us know by posting the issue on our Github issue tracker, or
+        by asking a question in the forum.
         
+        .. support-end-inclusion-marker-do-not-remove
+        .. license-start-inclusion-marker-do-not-remove
         
         License
         =======
         
-        Plugin Name is **free** and **open source**, released under the Apache License, Version 2.0.
+        The PennyLane-Cirq plugin is **free** and **open source**, released under
+        the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__.
+        
+        .. license-end-inclusion-marker-do-not-remove
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pennylane_cirq
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PennyLane-Cirq-0.8.0/README.rst` & `PennyLane-Cirq-0.9.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-PennyLane Cirq Plugin
-#########################
+PennyLane-Cirq Plugin
+######################
 
 .. image:: https://img.shields.io/travis/com/XanaduAI/pennylane-cirq/master.svg
     :alt: Travis
     :target: https://travis-ci.com/XanaduAI/pennylane-cirq
 
 .. image:: https://img.shields.io/codecov/c/github/xanaduai/pennylane-cirq/master.svg
     :alt: Codecov coverage
@@ -17,93 +17,141 @@
     :alt: Read the Docs
     :target: https://pennylane-cirq.readthedocs.io
 
 .. image:: https://img.shields.io/pypi/v/pennylane-cirq.svg
     :alt: PyPI
     :target: https://pypi.org/project/pennylane-cirq
 
+.. image:: https://github.com/XanaduAI/pennylane-cirq/blob/master/doc/_static/puzzle_cirq.png?raw=true
+    :align: center
+    :width: 200px
+    :target: javascript:void(0);
 
-`PennyLane <https://pennylane.readthedocs.io>`_ is a cross-platform Python library for quantum machine
+|
+
+.. header-start-inclusion-marker-do-not-remove
+
+The PennyLane-Cirq plugin integrates the Cirq quantum computing framework with PennyLane's
+quantum machine learning capabilities.
+
+`PennyLane <https://pennylane.readthedocs.io>`__ is a cross-platform Python library for quantum machine
 learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
 
-`Cirq <https://github.com/quantumlib/Cirq>`_ is a Python library for writing, manipulating, and optimizing quantum circuits and running them against quantum computers and simulators.
+`Cirq <https://github.com/quantumlib/Cirq>`__ is a software library for quantum computing.
 
-This PennyLane plugin allows to use both the software and hardware backends of Cirq as devices for PennyLane.
+.. header-end-inclusion-marker-do-not-remove
 
+The plugin documentation can be found here: `<https://pennylane-cirq.readthedocs.io/en/latest/>`__.
 
 Features
 ========
 
-* Access to Cirq's simulator backend via the `cirq.simulator` device
+* Provides access to Cirq's simulator backend via the ``cirq.simulator`` device
 
 * Support for all PennyLane core functionality
 
+.. installation-start-inclusion-marker-do-not-remove
 
 Installation
 ============
 
-Plugin Name requires both PennyLane and Cirq. It can be installed via ``pip``:
+This plugin requires Python version 3.6 or above, as well as PennyLane
+and Cirq. Installation of this plugin, as well as all dependencies, can be done using ``pip``:
+
+.. code-block:: bash
+
+    $ pip install pennylane-cirq
+
+Alternatively, you can install PennyLane-Cirq from the `source code <https://github.com/XanaduAI/pennylane-cirq>`__
+by navigating to the top directory and running:
+
+.. code-block:: bash
+
+	$ python setup.py install
+
+Dependencies
+~~~~~~~~~~~~
+
+PennyLane-Cirq requires the following libraries be installed:
+
+* `Python <http://python.org/>`__ >= 3.6
+
+as well as the following Python packages:
+
+* `PennyLane <http://pennylane.readthedocs.io/>`__ >= 0.9
+* `Cirq <https://cirq.readthedocs.io/>`__ >= 0.7
+
+
+If you currently do not have Python 3 installed, we recommend
+`Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed version of Python packaged
+for scientific computation.
+
+
+Tests
+~~~~~
+
+To test that the PennyLane-Cirq plugin is working correctly you can run
 
 .. code-block:: bash
 
-    $ python -m pip install pennylane-cirq
+    $ make test
 
+in the source folder.
 
-Getting started
-===============
+Documentation
+~~~~~~~~~~~~~
 
-Once Pennylane Cirq is installed, the provided Cirq devices can be accessed straight
-away in PennyLane.
+To build the HTML documentation, go to the top-level directory and run:
 
-You can instantiate these devices for PennyLane as follows:
+.. code-block:: bash
 
-.. code-block:: python
+  $ make docs
 
-    import pennylane as qml
-    dev = qml.device('cirq.simulator', wires=2, shots=100, analytic=True)
 
-These devices can then be used just like other devices for the definition and evaluation of
-QNodes within PennyLane. For more details, see the
-`plugin usage guide <https://pennylane-cirq.readthedocs.io/en/latest/usage.html>`_ and refer
-to the PennyLane documentation.
+The documentation can then be found in the ``doc/_build/html/`` directory.
 
+.. installation-end-inclusion-marker-do-not-remove
 
 Contributing
 ============
 
-We welcome contributions - simply fork the Plugin Name repository, and then make a
-`pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.
-All contributors to PennyLane-Cirq will be listed as authors on the releases.
-
-We also encourage bug reports, suggestions for new features and enhancements, and even links to cool
-projects or applications built on PennyLane and Cirq.
+We welcome contributions - simply fork the repository of this plugin, and then make a
+`pull request <https://help.github.com/articles/about-pull-requests/>`__ containing your contribution.
+All contributers to this plugin will be listed as authors on the releases.
 
+We also encourage bug reports, suggestions for new features and enhancements, and even links to cool projects
+or applications built on PennyLane.
 
 Authors
 =======
 
-Johannes Jakob Meyer
-
-If you are doing research using PennyLane, please cite our papers:
+PennyLane-Cirq is the work of `many contributors <https://github.com/XanaduAI/pennylane-cirq/graphs/contributors>`__.
 
-    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
-    *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
-    `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
+If you are doing research using PennyLane and PennyLane-Cirq, please cite `our paper <https://arxiv.org/abs/1811.04968>`__:
 
-    Maria Schuld, Ville Bergholm, Christian Gogolin, Josh Izaac, and Nathan Killoran.
-    *Evaluating analytic gradients on quantum hardware.* 2018.
-    `Phys. Rev. A 99, 032331 <https://journals.aps.org/pra/abstract/10.1103/PhysRevA.99.032331>`_
+    Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, M. Sohaib Alam, Shahnawaz Ahmed,
+    Juan Miguel Arrazola, Carsten Blank, Alain Delgado, Soran Jahangiri, Keri McKiernan, Johannes Jakob Meyer,
+    Zeyue Niu, Antal Száva, and Nathan Killoran.
+    *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968
 
+.. support-start-inclusion-marker-do-not-remove
 
 Support
 =======
 
 - **Source Code:** https://github.com/XanaduAI/pennylane-cirq
 - **Issue Tracker:** https://github.com/XanaduAI/pennylane-cirq/issues
+- **PennyLane Forum:** https://discuss.pennylane.ai
 
-If you are having issues, please let us know by posting the issue on our GitHub issue tracker.
+If you are having issues, please let us know by posting the issue on our Github issue tracker, or
+by asking a question in the forum.
 
+.. support-end-inclusion-marker-do-not-remove
+.. license-start-inclusion-marker-do-not-remove
 
 License
 =======
 
-Plugin Name is **free** and **open source**, released under the Apache License, Version 2.0.
+The PennyLane-Cirq plugin is **free** and **open source**, released under
+the `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`__.
+
+.. license-end-inclusion-marker-do-not-remove
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PennyLane-Cirq-0.8.0/pennylane_cirq/__init__.py` & `PennyLane-Cirq-0.9.0/pennylane_cirq/_version.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# Copyright 2019 Xanadu Quantum Technologies Inc.
+# Copyright 2018 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+"""Version information.
+   Version number (major.minor.patch[-label])
 """
-Plugin overview
-===============
-"""
-from .simulator_device import SimulatorDevice
 
-# TODO[CUSTOM OPS]: Uncomment and import all custom gates
-# from .ops import S, T, CCNOT, CPHASE, CSWAP, ISWAP, PSWAP
-from ._version import __version__
+__version__ = "0.9.0"
```

### Comparing `PennyLane-Cirq-0.8.0/pennylane_cirq/cirq_device.py` & `PennyLane-Cirq-0.9.0/pennylane_cirq/cirq_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Xanadu Quantum Technologies Inc.
+# Copyright 2019-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -35,32 +35,33 @@
 import cirq
 import numpy as np
 import pennylane as qml
 from pennylane import QubitDevice
 from pennylane.operation import Operation
 
 from ._version import __version__
-from .cirq_interface import CirqOperation
+from .cirq_operation import CirqOperation
+
 
 class CirqDevice(QubitDevice, abc.ABC):
     """Abstract base device for PennyLane-Cirq.
 
     Args:
         wires (int): the number of modes to initialize the device in
         shots (int): Number of circuit evaluations/random samples used
             to estimate expectation values of observables. Shots need to be >= 1.
         qubits (List[cirq.Qubit]): a list of Cirq qubits that are used
             as wires. The wire number corresponds to the index in the list.
             By default, an array of ``cirq.LineQubit`` instances is created.
     """
 
     name = "Cirq Abstract PennyLane plugin baseclass"
-    pennylane_requires = ">=0.8.0"
+    pennylane_requires = ">=0.9.0"
     version = __version__
-    author = "Johannes Jakob Meyer"
+    author = "Xanadu Inc"
     _capabilities = {
         "model": "qubit",
         "tensor_observables": True,
         "inverse_operations": True,
     }
 
     short_name = "cirq.base_device"
@@ -88,17 +89,15 @@
             if not self._operation_map[key]:
                 continue
 
             # We have to use a new CirqOperation instance because .inv() acts in-place
             inverted_operation = CirqOperation(self._operation_map[key].parametrization)
             inverted_operation.inv()
 
-            self._inverse_operation_map[
-                key + Operation.string_for_inverse
-            ] = inverted_operation
+            self._inverse_operation_map[key + Operation.string_for_inverse] = inverted_operation
 
         self._complete_operation_map = {
             **self._operation_map,
             **self._inverse_operation_map,
         }
 
     _operation_map = {
@@ -191,27 +190,27 @@
         cirq_operation = self._complete_operation_map[operation.name]
 
         # If command is None do nothing
         if cirq_operation:
             cirq_operation.parametrize(*operation.parameters)
 
             self.circuit.append(
-                cirq_operation.apply(
-                    *[self.qubits[wire] for wire in operation.wires]
-                )
+                cirq_operation.apply(*[self.qubits[wire] for wire in operation.wires])
             )
 
     def apply(self, operations, **kwargs):
         # pylint: disable=missing-function-docstring
         rotations = kwargs.pop("rotations", [])
 
         for i, operation in enumerate(operations):
             if i > 0 and operation.name in {"BasisState", "QubitStateVector"}:
                 raise qml.DeviceError(
-                    "The operation {} is only supported at the beginning of a circuit.".format(operation.name)
+                    "The operation {} is only supported at the beginning of a circuit.".format(
+                        operation.name
+                    )
                 )
 
             if operation.name == "BasisState":
                 self._apply_basis_state(operation)
             elif operation.name == "QubitStateVector":
                 self._apply_qubit_state_vector(operation)
             else:
```

### Comparing `PennyLane-Cirq-0.8.0/setup.py` & `PennyLane-Cirq-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Xanadu Quantum Technologies Inc.
+# Copyright 2019-2020 Xanadu Quantum Technologies Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,15 +30,16 @@
     "name": "PennyLane-Cirq",
     "version": version,
     "maintainer": "Xanadu Inc.",
     "maintainer_email": "software@xanadu.ai",
     "url": "http://xanadu.ai",
     "license": "Apache License 2.0",
     "packages": ["pennylane_cirq"],
-    "entry_points": {"pennylane.plugins": ["cirq.simulator = pennylane_cirq:SimulatorDevice"]},
+    "entry_points": {"pennylane.plugins": ["cirq.simulator = pennylane_cirq:SimulatorDevice",
+                                           "cirq.mixedsimulator = pennylane_cirq:MixedStateSimulatorDevice"],},
     # Place a one line description here. This will be shown by pip
     "description": "PennyLane plugin for Cirq",
     "long_description": open("README.rst").read(),
     # The name of the folder containing the plugin
     "provides": ["pennylane_cirq"],
     "install_requires": requirements,
 }
@@ -52,15 +53,15 @@
     "Operating System :: POSIX",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     # Make sure to specify here the versions of Python supported
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 setup(classifiers=classifiers, **(info))
```

