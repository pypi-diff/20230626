# Comparing `tmp/idem-tls-0.1.0.tar.gz` & `tmp/idem-tls-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-tls-0.1.0.tar", last modified: Thu Nov 17 13:03:49 2022, max compression
+gzip compressed data, was "idem-tls-0.2.0.tar", last modified: Mon Jun 26 11:49:47 2023, max compression
```

## Comparing `idem-tls-0.1.0.tar` & `idem-tls-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2022-11-17 13:03:31.000000 idem-tls-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5587 2022-11-17 13:03:49.783525 idem-tls-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4784 2022-11-17 13:03:31.000000 idem-tls-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/acct/tls/
--rw-r--r--   0 root         (0) root         (0)      485 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/acct/tls/init.py
--rw-r--r--   0 root         (0) root         (0)     1319 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/exec/tls/
--rw-r--r--   0 root         (0) root         (0)     4113 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/exec/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)      167 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/exec/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/states/tls/
--rw-r--r--   0 root         (0) root         (0)      169 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/states/tls/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls/tool/tls/
--rw-r--r--   0 root         (0) root         (0)     2356 2022-11-17 13:03:31.000000 idem-tls-0.1.0/idem_tls/tool/tls/certificate.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 13:03:49.783525 idem-tls-0.1.0/idem_tls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5587 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-17 13:03:49.000000 idem-tls-0.1.0/idem_tls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-17 13:03:49.783525 idem-tls-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2716 2022-11-17 13:03:31.000000 idem-tls-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-06-26 11:49:34.000000 idem-tls-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-06-26 11:49:47.830606 idem-tls-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-06-26 11:49:34.000000 idem-tls-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/acct/tls/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/acct/tls/init.py
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/exec/tls/
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/exec/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/exec/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/states/tls/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/states/tls/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls/tool/tls/
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-06-26 11:49:34.000000 idem-tls-0.2.0/idem_tls/tool/tls/certificate.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 11:49:47.830606 idem-tls-0.2.0/idem_tls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 11:49:47.000000 idem-tls-0.2.0/idem_tls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 11:49:47.834606 idem-tls-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-26 11:49:34.000000 idem-tls-0.2.0/setup.py
```

### Comparing `idem-tls-0.1.0/LICENSE` & `idem-tls-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-tls-0.1.0/PKG-INFO` & `idem-tls-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-tls
-Version: 0.1.0
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -18,69 +18,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-===============
+========
 idem-tls
-===============
+========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin to work with TLS keys and certificates.
+The Idem TLS provider
 
 About
 =====
 
-TLS Provider Idem plugin
+An Idem plugin to work with TLS keys and certificates.
+
+The plugin fetches TLS certificate information for use with other Idem plugins, such as ``idem-aws``, when creating resources that expose TLS services.
 
 What is POP?
 ------------
 
-This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
-implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
-together concepts and wisdom from the history of computing in new ways to solve
-modern computing problems.
+This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring together concepts and wisdom from the history of computing in new ways to solve modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
 * `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
 * Python 3.7+
-* git *(if installing from source, or contributing to the project)*
+* git *(if installing from source or contributing to the project)*
+
+  To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
 
-.. note::
+You can install ``idem-tls`` with the Python package installer (PyPI) or from source.
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+Install from PyPI
++++++++++++++++++
 
-If wanting to use ``idem-tls``, you can do so from source.
+.. code-block:: bash
 
-Install from source
+      pip install idem-tls
+
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-tls.git
    cd idem-tls
@@ -88,78 +89,67 @@
    # Setup venv
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
-This Idem plugin can be used to fetch tls certificate information that can then be used with other idem plugin like idem-aws when creating resources that expose TLS services.
 
 Setup
------------------
-After installation, the tls Idem execution and state modules will be accessible to the pop `hub`.
-In order to customize the TLS method, we need to set up our credentials.
-Credentials for TLS idem-tls are optional and in case not setup plugin will use default TLS method "TLSv1".
+-----
+
+After installation, ``idem-tls`` execution and state modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-Create a new file called `credentials.yaml` and populate it with credentials.
-The `default` profile will be picked up automatically by `idem`.
+To set the TLS method that ``idem-tls`` uses, configure it in your credentials.yaml file.
+
+Credentials for ``idem-tls`` are optional. If you don't configure a TLS method, the plugin uses TLSv1 by default.
 
 credentials.yaml:
 
 ..  code:: sls
 
     tls:
       default:
         method: TLSv1_2
 
-Next step is to encrypt the credentials file, and add the encryption key and encrypted file
-path to the ENVIRONMENT.
+For more about Idem credentials files, including recommended steps for encryption and environment variables, see `Authenticating with Idem <https://docs.idemproject.io/getting-started/en/latest/topics/gettingstarted/authenticating.html>`__
 
-Encrypt the credential file:
+You are now ready to use idem-tls.
 
-.. code:: bash
-
-    acct encrypt credentials.yaml
-
-This will generate a credentials.yaml.fernet file and a command line output token::
- -AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI=
+Exec Module
+-----------
 
-Add these to your environment:
+An SLS file specifies the desired state of a resource. You can run an exec module within an SLS file using the ``exec.run`` state, where the exec module returns a new state that can be referenced with argument binding.
 
-.. code:: bash
+The ``idem-tls`` plugin exec module supports TLS certificate ``get`` and ``list`` operations.
 
-    export ACCT_KEY="-AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI="
-    export ACCT_FILE=$PWD/credentials.yaml.fernet
+* ``tls.certificate.get``
 
+  Return the root CA certificate for a given URL.
 
-You are ready to use idem-tls!!!
+* ``tls.certificate.list``
 
-Exec Module
------------
-Exec modules can be run from SLS using the "exec.run" state. The return from the exec module is put in the state's "new_state", so it can be used in arg_binding. The desired state of a resource can be specified in sls file.
-Idem TLS plugins exec module allows TLS Certificate get and list operations.
-The "tls.certificate.get" to get the root CA certificate for given URL.
-The "tls.certificate.list" to get the certificate chain for given URL.
+  Return the certificate chain for a given URL.
 
-Request Syntax:
+Syntax:
 
 ..  code:: sls
 
     [Idem-state-name]:
       exec.run:
         - path: tls.certificate.get
         - kwargs:
             url: 'string'
 
-Examples Usage:
+Example:
 
 ..  code:: sls
 
     unmanaged-tls_certificate:
       exec.run:
         - path: tls.certificate.get
         - kwargs:
@@ -175,21 +165,22 @@
             - ${exec:unmanaged-tls_certificate:sha1_fingerprint}
           tags:
             - Key: tag-key-1
               Value: tag-value-1
             - Key: tag-key-2
               Value: tag-value-2
 
-It can be specified from command line when calling exec module as below
+Idem command line example:
 
 .. code:: bash
 
      idem exec exec.tls.certificate.list url=https://oidc.eks.us-east-2.amazonaws.com/id/sample
 
-Current Supported Resources states
-++++++++++++++++++++++++++++++++++
+Current Supported Resource States
+---------------------------------
 
 tls
-"""""""""""""
++++
+
 certificate
```

### Comparing `idem-tls-0.1.0/README.rst` & `idem-tls-0.2.0/idem_tls.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,87 @@
-===============
+Metadata-Version: 2.1
+Name: idem-tls
+Version: 0.2.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
+Author: Barnali Rakshit
+Author-email: brakshit@vmware.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+========
 idem-tls
-===============
+========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin to work with TLS keys and certificates.
+The Idem TLS provider
 
 About
 =====
 
-TLS Provider Idem plugin
+An Idem plugin to work with TLS keys and certificates.
+
+The plugin fetches TLS certificate information for use with other Idem plugins, such as ``idem-aws``, when creating resources that expose TLS services.
 
 What is POP?
 ------------
 
-This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
-implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
-together concepts and wisdom from the history of computing in new ways to solve
-modern computing problems.
+This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring together concepts and wisdom from the history of computing in new ways to solve modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
 * `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
 * Python 3.7+
-* git *(if installing from source, or contributing to the project)*
+* git *(if installing from source or contributing to the project)*
+
+  To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
 
-.. note::
+You can install ``idem-tls`` with the Python package installer (PyPI) or from source.
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+Install from PyPI
++++++++++++++++++
 
-If wanting to use ``idem-tls``, you can do so from source.
+.. code-block:: bash
+
+      pip install idem-tls
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-tls.git
    cd idem-tls
@@ -64,78 +89,67 @@
    # Setup venv
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
-This Idem plugin can be used to fetch tls certificate information that can then be used with other idem plugin like idem-aws when creating resources that expose TLS services.
 
 Setup
------------------
-After installation, the tls Idem execution and state modules will be accessible to the pop `hub`.
-In order to customize the TLS method, we need to set up our credentials.
-Credentials for TLS idem-tls are optional and in case not setup plugin will use default TLS method "TLSv1".
+-----
+
+After installation, ``idem-tls`` execution and state modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-Create a new file called `credentials.yaml` and populate it with credentials.
-The `default` profile will be picked up automatically by `idem`.
+To set the TLS method that ``idem-tls`` uses, configure it in your credentials.yaml file.
+
+Credentials for ``idem-tls`` are optional. If you don't configure a TLS method, the plugin uses TLSv1 by default.
 
 credentials.yaml:
 
 ..  code:: sls
 
     tls:
       default:
         method: TLSv1_2
 
-Next step is to encrypt the credentials file, and add the encryption key and encrypted file
-path to the ENVIRONMENT.
-
-Encrypt the credential file:
+For more about Idem credentials files, including recommended steps for encryption and environment variables, see `Authenticating with Idem <https://docs.idemproject.io/getting-started/en/latest/topics/gettingstarted/authenticating.html>`__
 
-.. code:: bash
-
-    acct encrypt credentials.yaml
+You are now ready to use idem-tls.
 
-This will generate a credentials.yaml.fernet file and a command line output token::
- -AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI=
+Exec Module
+-----------
 
-Add these to your environment:
+An SLS file specifies the desired state of a resource. You can run an exec module within an SLS file using the ``exec.run`` state, where the exec module returns a new state that can be referenced with argument binding.
 
-.. code:: bash
+The ``idem-tls`` plugin exec module supports TLS certificate ``get`` and ``list`` operations.
 
-    export ACCT_KEY="-AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI="
-    export ACCT_FILE=$PWD/credentials.yaml.fernet
+* ``tls.certificate.get``
 
+  Return the root CA certificate for a given URL.
 
-You are ready to use idem-tls!!!
+* ``tls.certificate.list``
 
-Exec Module
------------
-Exec modules can be run from SLS using the "exec.run" state. The return from the exec module is put in the state's "new_state", so it can be used in arg_binding. The desired state of a resource can be specified in sls file.
-Idem TLS plugins exec module allows TLS Certificate get and list operations.
-The "tls.certificate.get" to get the root CA certificate for given URL.
-The "tls.certificate.list" to get the certificate chain for given URL.
+  Return the certificate chain for a given URL.
 
-Request Syntax:
+Syntax:
 
 ..  code:: sls
 
     [Idem-state-name]:
       exec.run:
         - path: tls.certificate.get
         - kwargs:
             url: 'string'
 
-Examples Usage:
+Example:
 
 ..  code:: sls
 
     unmanaged-tls_certificate:
       exec.run:
         - path: tls.certificate.get
         - kwargs:
@@ -151,19 +165,22 @@
             - ${exec:unmanaged-tls_certificate:sha1_fingerprint}
           tags:
             - Key: tag-key-1
               Value: tag-value-1
             - Key: tag-key-2
               Value: tag-value-2
 
-It can be specified from command line when calling exec module as below
+Idem command line example:
 
 .. code:: bash
 
      idem exec exec.tls.certificate.list url=https://oidc.eks.us-east-2.amazonaws.com/id/sample
 
-Current Supported Resources states
-++++++++++++++++++++++++++++++++++
+Current Supported Resource States
+---------------------------------
 
 tls
-"""""""""""""
++++
+
 certificate
+
+
```

### Comparing `idem-tls-0.1.0/idem_tls/conf.py` & `idem-tls-0.2.0/idem_tls/conf.py`

 * *Files identical despite different names*

### Comparing `idem-tls-0.1.0/idem_tls/exec/tls/certificate.py` & `idem-tls-0.2.0/idem_tls/exec/tls/certificate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+"""Exec module for TLS certificates."""
 from typing import Dict
 
 from dict_tools.typing import Computed
 from OpenSSL import SSL
 
 __func_alias__ = {"list_": "list"}
 
 
 async def get(hub, ctx, url: str) -> Computed[Dict]:
-    """
-    Get information about the TLS certificates securing a host.
-
+    """Get information about the TLS certificates securing a host.
 
     Args:
-        url(string):
-            The URL of the website to get the certificates from.
+      url(str):
+        The URL of the website to get the certificates from.
+
+     Returns:
+        .. code-block:: python
+
+            {"result": True|False, "comment": list, "ret": None|dict}
+
+    Examples:
+        Calling this exec module function from the cli
+
+        .. code-block:: bash
+
+            idem exec exec.tls.certificate.get url=https://oidc.eks.us-east-2.amazonaws.com/id/sample
 
     Request Syntax:
-        [Idem-state-name]:
-          exec.run:
-            - path: tls.certificate.get
-            - kwargs:
-                url: 'string'
+      .. code-block:: sls
+
+          [Idem-state-name]:
+            exec.run:
+              path: tls.certificate.get
+              kwargs:
+                  url: 'string'
 
     Sample response:
+        .. code-block:: sls
+
             url: https://oidc.eks.us-east-2.amazonaws.com/id/sample
             sha1_fingerprint: 9e99a48a9960b14926bb7f3b02e22da2b0ab7280
             issuer:
               C: US
               O: Starfield Technologies, Inc.
               OU: Starfield Class 2 Certification Authority
             not_after: 2034-06-28 17:39:16
@@ -39,14 +54,16 @@
               CN: Starfield Services Root Certificate Authority - G2
             version: 2
             signature_algorithm: sha256WithRSAEncryption
             serial_number: 12037640545166866303
             resource_id: 12037640545166866303
 
     Example Usage:
+        .. code-block:: sls
+
             unmanaged-tls_certificate:
               exec.run:
                 - path: tls.certificate.get
                 - kwargs:
                     url: https://oidc.eks.us-east-2.amazonaws.com/id/sample
 
             arn:aws:iam::537227425989:www.sample-2.com:
@@ -58,14 +75,15 @@
                 - thumbprint_list:
                     - ${exec:unmanaged-tls_certificate:sha1_fingerprint}
                 - tags:
                     - Key: alpha.eksctl.io/eksctl-version
                       Value: 0.77.0
                     - Key: alpha.eksctl.io/cluster-name
                       Value: pr-ssc-eks-poc
+
     """
     result = dict(comment=[], ret=None, result=True)
 
     try:
         conn = await hub.tool.tls.certificate.get_ssl_connection(ctx, url)
         conn.do_handshake()
     except SSL.Error as e:
@@ -87,22 +105,51 @@
 
     result["comment"].append(f"fetched certificate information for url {url}")
     result["ret"] = resource_translated
     return result
 
 
 async def list_(hub, ctx, url: str) -> Computed[Dict]:
-    """
-    Get list of TLS certificate in chain securing a host.
+    """Get list of TLS certificate in chain securing a host.
 
     List information about TLS certificates.
 
     Args:
-        url(string):
-            The URL of the website to get the certificates from.
+      url(str):
+        The URL of the website to get the certificates from.
+
+     Returns:
+        .. code-block:: python
+
+            {"result": True|False, "comment": list, "ret": list}
+
+    Examples:
+        Calling this exec module function from the cli
+
+        .. code-block:: bash
+
+            idem exec exec.tls.certificate.list url=https://oidc.eks.us-east-2.amazonaws.com/id/sample
+
+    Request Syntax:
+      .. code-block:: sls
+
+          [Idem-state-name]:
+            exec.run:
+              path: tls.certificate.list
+              kwargs:
+                  url: 'string'
+
+    Example Usage:
+        .. code-block:: sls
+
+            unmanaged-tls_certificate:
+              exec.run:
+                - path: tls.certificate.list
+                - kwargs:
+                    url: https://oidc.eks.us-east-2.amazonaws.com/id/sample
 
     """
     result = dict(comment=[], ret=[], result=True)
 
     try:
         conn = await hub.tool.tls.certificate.get_ssl_connection(ctx, url)
         conn.do_handshake()
```

### Comparing `idem-tls-0.1.0/idem_tls/tool/tls/certificate.py` & `idem-tls-0.2.0/idem_tls/tool/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `idem-tls-0.1.0/setup.py` & `idem-tls-0.2.0/setup.py`

 * *Files identical despite different names*

