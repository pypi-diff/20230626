# Comparing `tmp/crux-1.2.tar.gz` & `tmp/crux-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crux-1.2.tar", last modified: Thu Mar 30 17:53:23 2023, max compression
+gzip compressed data, was "dist/crux-1.3.tar", last modified: Mon Jun 26 17:54:16 2023, max compression
```

## Comparing `crux-1.2.tar` & `crux-1.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 stuartlai   (502) staff       (20)        0 2023-03-30 17:53:23.054853 crux-1.2/
--rw-r--r--   0 stuartlai   (502) staff       (20)     6775 2023-03-30 17:53:23.053665 crux-1.2/PKG-INFO
--rw-r--r--   0 stuartlai   (502) staff       (20)     4607 2023-03-30 17:51:20.000000 crux-1.2/README.md
-drwxr-xr-x   0 stuartlai   (502) staff       (20)        0 2023-03-30 17:53:23.011767 crux-1.2/crux/
--rwxr-xr-x   0 stuartlai   (502) staff       (20)      306 2023-03-30 17:51:20.000000 crux-1.2/crux/__init__.py
--rw-r--r--   0 stuartlai   (502) staff       (20)       82 2023-03-30 17:51:20.000000 crux-1.2/crux/__version__.py
--rwxr-xr-x   0 stuartlai   (502) staff       (20)     7524 2023-03-30 17:51:20.000000 crux-1.2/crux/_client.py
--rw-r--r--   0 stuartlai   (502) staff       (20)      451 2023-03-30 17:51:20.000000 crux-1.2/crux/_compat.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     5986 2023-03-30 17:51:20.000000 crux-1.2/crux/_config.py
--rwxr-xr-x   0 stuartlai   (502) staff       (20)     6579 2023-03-30 17:51:20.000000 crux-1.2/crux/_utils.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     8306 2023-03-30 17:51:20.000000 crux-1.2/crux/apis.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     3472 2023-03-30 17:51:20.000000 crux-1.2/crux/exceptions.py
-drwxr-xr-x   0 stuartlai   (502) staff       (20)        0 2023-03-30 17:53:23.050220 crux-1.2/crux/models/
--rw-r--r--   0 stuartlai   (502) staff       (20)      836 2023-03-30 17:51:20.000000 crux-1.2/crux/models/__init__.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     1033 2023-03-30 17:51:20.000000 crux-1.2/crux/models/_factory.py
--rw-r--r--   0 stuartlai   (502) staff       (20)    51749 2023-03-30 17:51:20.000000 crux-1.2/crux/models/dataset.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     4086 2023-03-30 17:51:20.000000 crux-1.2/crux/models/delivery.py
--rw-r--r--   0 stuartlai   (502) staff       (20)    17429 2023-03-30 17:51:20.000000 crux-1.2/crux/models/file.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     3752 2023-03-30 17:51:20.000000 crux-1.2/crux/models/folder.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     2520 2023-03-30 17:51:20.000000 crux-1.2/crux/models/identity.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     3431 2023-03-30 17:51:20.000000 crux-1.2/crux/models/ingestion.py
--rw-r--r--   0 stuartlai   (502) staff       (20)      851 2023-03-30 17:51:20.000000 crux-1.2/crux/models/job.py
--rw-r--r--   0 stuartlai   (502) staff       (20)      373 2023-03-30 17:51:20.000000 crux-1.2/crux/models/label.py
--rw-r--r--   0 stuartlai   (502) staff       (20)     2012 2023-03-30 17:51:20.000000 crux-1.2/crux/models/model.py
--rw-r--r--   0 stuartlai   (502) staff       (20)      527 2023-03-30 17:51:20.000000 crux-1.2/crux/models/permission.py
--rw-r--r--   0 stuartlai   (502) staff       (20)    12801 2023-03-30 17:51:20.000000 crux-1.2/crux/models/resource.py
-drwxr-xr-x   0 stuartlai   (502) staff       (20)        0 2023-03-30 17:53:23.021843 crux-1.2/crux.egg-info/
--rw-r--r--   0 stuartlai   (502) staff       (20)     6775 2023-03-30 17:53:22.000000 crux-1.2/crux.egg-info/PKG-INFO
--rw-r--r--   0 stuartlai   (502) staff       (20)      601 2023-03-30 17:53:22.000000 crux-1.2/crux.egg-info/SOURCES.txt
--rw-r--r--   0 stuartlai   (502) staff       (20)        1 2023-03-30 17:53:22.000000 crux-1.2/crux.egg-info/dependency_links.txt
--rw-r--r--   0 stuartlai   (502) staff       (20)      117 2023-03-30 17:53:22.000000 crux-1.2/crux.egg-info/requires.txt
--rw-r--r--   0 stuartlai   (502) staff       (20)        5 2023-03-30 17:53:22.000000 crux-1.2/crux.egg-info/top_level.txt
--rw-r--r--   0 stuartlai   (502) staff       (20)       99 2023-03-30 17:51:20.000000 crux-1.2/pyproject.toml
--rw-r--r--   0 stuartlai   (502) staff       (20)       38 2023-03-30 17:53:23.055189 crux-1.2/setup.cfg
--rw-r--r--   0 stuartlai   (502) staff       (20)     1753 2023-03-30 17:51:20.000000 crux-1.2/setup.py
+drwxr-xr-x   0 matthijsk   (503) staff       (20)        0 2023-06-26 17:54:16.000000 crux-1.3/
+-rw-r--r--   0 matthijsk   (503) staff       (20)     1079 2023-06-26 17:23:56.000000 crux-1.3/LICENSE
+-rw-r--r--   0 matthijsk   (503) staff       (20)     5622 2023-06-26 17:54:16.000000 crux-1.3/PKG-INFO
+-rw-r--r--   0 matthijsk   (503) staff       (20)     4607 2023-06-26 17:40:25.000000 crux-1.3/README.md
+drwxr-xr-x   0 matthijsk   (503) staff       (20)        0 2023-06-26 17:54:16.000000 crux-1.3/crux/
+-rwxr-xr-x   0 matthijsk   (503) staff       (20)      306 2023-06-26 17:23:56.000000 crux-1.3/crux/__init__.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)       82 2023-06-26 17:40:25.000000 crux-1.3/crux/__version__.py
+-rwxr-xr-x   0 matthijsk   (503) staff       (20)     7522 2023-06-26 17:23:56.000000 crux-1.3/crux/_client.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)      451 2023-06-26 17:23:56.000000 crux-1.3/crux/_compat.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     5986 2023-06-26 17:23:56.000000 crux-1.3/crux/_config.py
+-rwxr-xr-x   0 matthijsk   (503) staff       (20)     6579 2023-06-26 17:23:56.000000 crux-1.3/crux/_utils.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     8312 2023-06-26 17:23:56.000000 crux-1.3/crux/apis.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     3472 2023-06-26 17:23:56.000000 crux-1.3/crux/exceptions.py
+drwxr-xr-x   0 matthijsk   (503) staff       (20)        0 2023-06-26 17:54:16.000000 crux-1.3/crux/models/
+-rw-r--r--   0 matthijsk   (503) staff       (20)      836 2023-06-26 17:23:56.000000 crux-1.3/crux/models/__init__.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     1033 2023-06-26 17:23:56.000000 crux-1.3/crux/models/_factory.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)    51677 2023-06-26 17:23:56.000000 crux-1.3/crux/models/dataset.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     4110 2023-06-26 17:23:56.000000 crux-1.3/crux/models/delivery.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)    17429 2023-06-26 17:23:56.000000 crux-1.3/crux/models/file.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     3752 2023-06-26 17:23:56.000000 crux-1.3/crux/models/folder.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     2520 2023-06-26 17:23:56.000000 crux-1.3/crux/models/identity.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     3431 2023-06-26 17:23:56.000000 crux-1.3/crux/models/ingestion.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)      851 2023-06-26 17:23:56.000000 crux-1.3/crux/models/job.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)      373 2023-06-26 17:23:56.000000 crux-1.3/crux/models/label.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)     2012 2023-06-26 17:23:56.000000 crux-1.3/crux/models/model.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)      527 2023-06-26 17:23:56.000000 crux-1.3/crux/models/permission.py
+-rw-r--r--   0 matthijsk   (503) staff       (20)    12865 2023-06-26 17:23:56.000000 crux-1.3/crux/models/resource.py
+drwxr-xr-x   0 matthijsk   (503) staff       (20)        0 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/
+-rw-r--r--   0 matthijsk   (503) staff       (20)     5622 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/PKG-INFO
+-rw-r--r--   0 matthijsk   (503) staff       (20)      609 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijsk   (503) staff       (20)        1 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijsk   (503) staff       (20)      117 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/requires.txt
+-rw-r--r--   0 matthijsk   (503) staff       (20)        5 2023-06-26 17:54:16.000000 crux-1.3/crux.egg-info/top_level.txt
+-rw-r--r--   0 matthijsk   (503) staff       (20)       99 2023-06-26 17:23:56.000000 crux-1.3/pyproject.toml
+-rw-r--r--   0 matthijsk   (503) staff       (20)       38 2023-06-26 17:54:16.000000 crux-1.3/setup.cfg
+-rw-r--r--   0 matthijsk   (503) staff       (20)     1753 2023-06-26 17:23:56.000000 crux-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `crux-1.2/PKG-INFO` & `crux-1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,16 @@
 Metadata-Version: 2.1
 Name: crux
-Version: 1.2
+Version: 1.3
 Summary: Crux Informatics API client library
 Home-page: https://github.com/cruxinformatics/crux-python
 Author: Crux Informatics, Inc.
 Author-email: python-opensource@cruxinformatics.com
 License: MIT
-Description: # Crux Python Client
-        
-        A Python library for interacting with the Crux platform.
-        
-        The aim of this module is to be a Pythonic way to use the Crux API reliably. It covers client functionality including scanning subscriptions, getting delivery status, and downloading files.
-        
-        Python 3.6+ is supported.
-        
-        **See [crux-python.cruxinformatics.com](https://crux-python.cruxinformatics.com/) for detailed documentation.**
-        
-        ## Installation
-        
-        Install a recent version of Python, and a Python dependency and virtual environment manager like [pipenv](https://pipenv.readthedocs.io/en/latest/). On macOS run:
-        
-        ```bash
-        brew install python
-        brew install pipenv
-        ```
-        
-        Install `crux` [from PyPI](https://pypi.org/project/crux/) in a virtual environment, and get a shell in that environment:
-        
-        ```bash
-        mkdir -p crux_example
-        cd crux_example
-        pipenv install "crux==1.2"
-        pipenv shell
-        ```
-        ## Getting Started
-        
-        Create a file, like example.py, and use the `crux` module:
-        
-        ```python
-        from crux import Crux
-        
-        conn = Crux()
-        identity = conn.whoami()
-        print("I am", identity.email)
-        ```
-        
-        Run the script:
-        
-        ```bash
-        HISTCONTROL=ignoreboth
-         export CRUX_API_KEY='YOUR_API_KEY'
-        python3 example.py
-        ```
-        
-        See the [installation](https://crux-python.cruxinformatics.com/en/latest/installation.html) and [authentication](https://crux-python.cruxinformatics.com/en/latest/authentication.html) documentation for details.
-        
-        ## Development
-        
-        Python 3.7 is required for development, which can be installed with `brew install python`. For heavy development work, every supported version of Python must be installed, see the pyenv documentation below.
-        
-        [Pipenv](https://pipenv.readthedocs.io/en/latest/) should be used to manage dependancies during development.
-        
-        1. [Install Pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv), on macOS run `brew install pipenv`
-        2. `git clone https://github.com/cruxinformatics/crux-python.git`
-        3. `cd crux-python`
-        4. `pipenv install --dev` to install the dependancies
-        5. `pipenv shell` to get a shell in the virtual environment
-        
-        ### Multiple Python versions
-        
-        To be able to run tests against all supported Python versions, you must have all supported Python versions installed. The test runner will look for binaries called `python2.7`, `python3.5`, `python3.6`, etc. There are multiple ways to install Python versions, we'll document using [pyenv](https://github.com/pyenv/pyenv).
-        
-        1. `brew install pyenv` to install
-        2. Put `eval "$(pyenv init -)"` towards the end of the shell configuration file (~/.bashrc or ~/.bash_profile), because it manipulates `$PATH`, for example:
-        
-            ```bash
-            echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc
-            ```
-        
-        3. Open a new Terminal to get an updated shell
-        4. Install required/missing Python versions (this assumes you have Python 2.7 already installed, otherwise install it too):
-        
-            ```bash
-            pyenv install 3.5.6
-            pyenv install 3.6.6
-            pyenv install 3.7.0
-            ```
-        
-        5. `pyenv global system 3.5.6 3.6.6 3.7.0` to make all the Python versions available
-        6. If you already have pipenv virtual environment, remove it with `pipenv --rm` so it detects the Python versions
-        7. `pipenv install --dev` to install all the dependancies
-        8. `pipenv shell` to get a shell in the virtual environment
-        
-        ### Running tests
-        
-        We use [Nox](https://nox.thea.codes/en/stable/) to automate running tests, and use `make` to automate running some commands. These commands should be run within a shell created with `pipenv shell`.
-        
-        ```bash
-        # Run all tests: lint, unit, format_check
-        make test
-        # Or
-        nox
-        
-        # Run only lint checks
-        make lint
-        # Or
-        nox -s lint
-        
-        # Run unit tests against all available Python versions
-        make unit
-        # Or
-        nox -s unit
-        
-        # Run integration tests agains all available Python versions
-         export CRUX_API_KEY="12345"
-        export CRUX_API_HOST="https://api.example.com"
-        make integration
-        # Or
-         export CRUX_API_KEY="12345"
-        export CRUX_API_HOST="https://api.example.com"
-        nox --s integration
-        
-        # Check formatting
-        make format_check
-        # Or
-        nox -s format_check
-        
-        # List all commands available
-        make
-        # Or
-        nox -l
-        
-        # Run unit test only against Python 3.7
-        nox -s unit-3.7
-        
-        # Reformat code
-        make format
-        
-        # Generate Sphinx HTML documentation
-        make docs
-        ```
-        
-        #### Running test scripts
-        
-        Manual testing scripts could be found at `tests/regression`.
-        In order to run one, i.e. `client.py`, follow the steps:
-        
-        1. copy corresponding `.env.dist` file as `.env` file (if you plan to run `client.py`, copy `client.env.dist` as `client.env`)
-        2. fill variables within `.env` file
-        3. launch the script (while being in the `tests/regression` folder, execute `python client.py`)
-        
 Keywords: crux-python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -163,7 +18,152 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Crux Python Client
+
+A Python library for interacting with the Crux platform.
+
+The aim of this module is to be a Pythonic way to use the Crux API reliably. It covers client functionality including scanning subscriptions, getting delivery status, and downloading files.
+
+Python 3.6+ is supported.
+
+**See [crux-python.cruxinformatics.com](https://crux-python.cruxinformatics.com/) for detailed documentation.**
+
+## Installation
+
+Install a recent version of Python, and a Python dependency and virtual environment manager like [pipenv](https://pipenv.readthedocs.io/en/latest/). On macOS run:
+
+```bash
+brew install python
+brew install pipenv
+```
+
+Install `crux` [from PyPI](https://pypi.org/project/crux/) in a virtual environment, and get a shell in that environment:
+
+```bash
+mkdir -p crux_example
+cd crux_example
+pipenv install "crux==1.3"
+pipenv shell
+```
+## Getting Started
+
+Create a file, like example.py, and use the `crux` module:
+
+```python
+from crux import Crux
+
+conn = Crux()
+identity = conn.whoami()
+print("I am", identity.email)
+```
+
+Run the script:
+
+```bash
+HISTCONTROL=ignoreboth
+ export CRUX_API_KEY='YOUR_API_KEY'
+python3 example.py
+```
+
+See the [installation](https://crux-python.cruxinformatics.com/en/latest/installation.html) and [authentication](https://crux-python.cruxinformatics.com/en/latest/authentication.html) documentation for details.
+
+## Development
+
+Python 3.7 is required for development, which can be installed with `brew install python`. For heavy development work, every supported version of Python must be installed, see the pyenv documentation below.
+
+[Pipenv](https://pipenv.readthedocs.io/en/latest/) should be used to manage dependancies during development.
+
+1. [Install Pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv), on macOS run `brew install pipenv`
+2. `git clone https://github.com/cruxinformatics/crux-python.git`
+3. `cd crux-python`
+4. `pipenv install --dev` to install the dependancies
+5. `pipenv shell` to get a shell in the virtual environment
+
+### Multiple Python versions
+
+To be able to run tests against all supported Python versions, you must have all supported Python versions installed. The test runner will look for binaries called `python2.7`, `python3.5`, `python3.6`, etc. There are multiple ways to install Python versions, we'll document using [pyenv](https://github.com/pyenv/pyenv).
+
+1. `brew install pyenv` to install
+2. Put `eval "$(pyenv init -)"` towards the end of the shell configuration file (~/.bashrc or ~/.bash_profile), because it manipulates `$PATH`, for example:
+
+    ```bash
+    echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc
+    ```
+
+3. Open a new Terminal to get an updated shell
+4. Install required/missing Python versions (this assumes you have Python 2.7 already installed, otherwise install it too):
+
+    ```bash
+    pyenv install 3.5.6
+    pyenv install 3.6.6
+    pyenv install 3.7.0
+    ```
+
+5. `pyenv global system 3.5.6 3.6.6 3.7.0` to make all the Python versions available
+6. If you already have pipenv virtual environment, remove it with `pipenv --rm` so it detects the Python versions
+7. `pipenv install --dev` to install all the dependancies
+8. `pipenv shell` to get a shell in the virtual environment
+
+### Running tests
+
+We use [Nox](https://nox.thea.codes/en/stable/) to automate running tests, and use `make` to automate running some commands. These commands should be run within a shell created with `pipenv shell`.
+
+```bash
+# Run all tests: lint, unit, format_check
+make test
+# Or
+nox
+
+# Run only lint checks
+make lint
+# Or
+nox -s lint
+
+# Run unit tests against all available Python versions
+make unit
+# Or
+nox -s unit
+
+# Run integration tests agains all available Python versions
+ export CRUX_API_KEY="12345"
+export CRUX_API_HOST="https://api.example.com"
+make integration
+# Or
+ export CRUX_API_KEY="12345"
+export CRUX_API_HOST="https://api.example.com"
+nox --s integration
+
+# Check formatting
+make format_check
+# Or
+nox -s format_check
+
+# List all commands available
+make
+# Or
+nox -l
+
+# Run unit test only against Python 3.7
+nox -s unit-3.7
+
+# Reformat code
+make format
+
+# Generate Sphinx HTML documentation
+make docs
+```
+
+#### Running test scripts
+
+Manual testing scripts could be found at `tests/regression`.
+In order to run one, i.e. `client.py`, follow the steps:
+
+1. copy corresponding `.env.dist` file as `.env` file (if you plan to run `client.py`, copy `client.env.dist` as `client.env`)
+2. fill variables within `.env` file
+3. launch the script (while being in the `tests/regression` folder, execute `python client.py`)
```

### Comparing `crux-1.2/README.md` & `crux-1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 Install `crux` [from PyPI](https://pypi.org/project/crux/) in a virtual environment, and get a shell in that environment:
 
 ```bash
 mkdir -p crux_example
 cd crux_example
-pipenv install "crux==1.2"
+pipenv install "crux==1.3"
 pipenv shell
 ```
 ## Getting Started
 
 Create a file, like example.py, and use the `crux` module:
 
 ```python
```

### Comparing `crux-1.2/crux/_client.py` & `crux-1.3/crux/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,14 @@
 
         user_agent = self.crux_config.user_agent  # type: Text
 
         headers["authorization"] = bearer_token
         headers["user-agent"] = user_agent
 
         session = self.crux_config.session
-
-
         if method in ("GET", "DELETE", "PUT", "POST"):
             try:
                 log.trace("Setting request stream: %s", stream)
                 log.trace("Setting request data: %s, json: %s", data, json)
                 log.trace("Setting request params: %s", params)
                 log.trace("Setting headers: %s", headers)
                 response = session.request(
```

### Comparing `crux-1.2/crux/_config.py` & `crux-1.3/crux/_config.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/_utils.py` & `crux-1.3/crux/_utils.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/apis.py` & `crux-1.3/crux/apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             id (str): Resource ID which is to be fetched.
 
         Returns:
             crux.models.Resource: Resource or its Child Object.
         """
         headers = Headers({"accept": "application/json"})  # type: MutableMapping[Text, Text]
 
-        response = self.api_client.api_call("GET", ["resources", id], headers=headers)
+        response = self.api_client.api_call("GET", ["v1", "resources", id], headers=headers)
         raw_resource = response.json()
 
         resource = get_resource_object(
             resource_type=raw_resource.get("type"),
             data=raw_resource,
             connection=self.api_client,
         )
```

### Comparing `crux-1.2/crux/exceptions.py` & `crux-1.3/crux/exceptions.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/__init__.py` & `crux-1.3/crux/models/__init__.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/_factory.py` & `crux-1.3/crux/models/_factory.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/dataset.py` & `crux-1.3/crux/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1102,15 +1102,15 @@
         """
         headers = Headers({"accept": "application/json"})
 
         if not DELIVERY_ID_REGEX.match(delivery_id):
             raise ValueError("Value of delivery_id is invalid")
 
         return self.connection.api_call(
-            "GET", ["deliveries", self.id, delivery_id], headers=headers, model=Delivery
+            "GET", ["v1", "deliveries", self.id,  delivery_id], headers=headers, model=Delivery
         )
 
     def get_ingestions(
         self, start_date=None, end_date=None, delivery_status=None, use_cache=None
     ):
         # type: (str, str, str, bool) -> Iterator[Ingestion]
         """Gets Ingestions.
@@ -1133,15 +1133,15 @@
         if delivery_status:
             params["delivery_status"] = delivery_status.upper()
 
         if use_cache is not None:
             params["useCache"] = use_cache
 
         response = self.connection.api_call(
-            "GET", ["deliveries", self.id, "ids"], headers=headers, params=params
+            "GET", ["v1", "deliveries", self.id, "ids"], headers=headers, params=params
         )
 
         response_json = response.json()
         if isinstance(response_json, dict):
             all_deliveries = response_json.get("delivery_ids")
         else:
             all_deliveries = response_json
@@ -1161,14 +1161,15 @@
                     "versions": ingestion_set[ingestion_id],
                     "datasetId": self.id,
                 }
             )
             obj.connection = self.connection
             yield obj
 
+
     def get_latest_files(
         self,
         frames=None,
         file_format=MediaType.AVRO.value,
         cutoff_date=None,
         dayfirst=False,
         yearfirst=False,
@@ -1419,20 +1420,22 @@
             resource_ids (list): List of resource IDs
 
         Returns:
             list (:obj:`crux.models.File`): List of file resources.
         """
         headers = Headers({"accept": "application/json"})
         limit = 250
-        for i in range(0, len(resource_ids), limit):
-            chunk = resource_ids[i : i + limit]
+
+        for item_cnt, item in enumerate(resource_ids):
+            if item_cnt > 250:
+                break
             response = self.connection.api_call(
-                "POST",
-                ["resources", "get-batch"],
-                params={"limit": limit + 1},
-                headers=headers,
-                data=json.dumps(chunk),
-            )
-            for resource in response.json():
-                obj = File(raw_model=resource)
-                obj.connection = self.connection
-                yield obj
+                "GET",
+                ["v1", "resources", item],
+                headers=headers
+             )
+            response_json = response.json()
+            obj =File(raw_model=response_json)
+            obj.connection = self.connection
+            yield obj
+
+
```

### Comparing `crux-1.2/crux/models/delivery.py` & `crux-1.3/crux/models/delivery.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return self.summary["schedule_dt"]
 
     @property
     def summary(self):
         """dict: Gets the Delivery Summary"""
         if self._summary is None:
             response = self.connection.api_call(
-                "GET", ["deliveries", self.dataset_id, self.id]
+                "GET", ["v1", "deliveries", self.dataset_id, self.id]
             )
             self._summary = response.json()
         return self._summary
 
     def get_data(self, file_format=MediaType.AVRO.value, use_cache=None):
         # type: (str, bool) -> Iterator[Resource]
         """Get the processed delivery data
@@ -69,15 +69,15 @@
         """
         params = {}
         params["delivery_resource_format"] = file_format
         if use_cache is not None:
             params["useCache"] = use_cache
 
         response = self.connection.api_call(
-            "GET", ["deliveries", self.dataset_id, self.id, "data"], params=params
+            "GET", ["v1", "deliveries", self.dataset_id, self.id, "data"], params=params
         )
 
         resource_list = response.json()["resources"]
 
         if resource_list:
             for resource in resource_list:
                 obj = File(raw_model={"resourceId": resource["resource_id"]})
@@ -96,15 +96,15 @@
             list (:obj:`crux.models.Resource`): List of resources.
         """
         params = {}
         if use_cache is not None:
             params["useCache"] = use_cache
 
         response = self.connection.api_call(
-            "GET", ["deliveries", self.dataset_id, self.id, "raw"], params=params
+            "GET", ["v1", "deliveries", self.dataset_id, self.id, "raw"], params=params
         )
 
         resource_list = response.json()["resource_ids"]
 
         if resource_list:
             for resource in resource_list:
                 obj = File(
@@ -124,12 +124,12 @@
             dict: Healthlog Json Object.
         """
         params = {}
         if use_cache is not None:
             params["useCache"] = use_cache
 
         response = self.connection.api_call(
-            "GET", ["deliveries", self.id, "log"], params=params
+            "GET", ["v1", "deliveries", self.id, "log"], params=params
         )
 
         healthlog_list = response.json()
         return healthlog_list
```

### Comparing `crux-1.2/crux/models/file.py` & `crux-1.3/crux/models/file.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/folder.py` & `crux-1.3/crux/models/folder.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/identity.py` & `crux-1.3/crux/models/identity.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/ingestion.py` & `crux-1.3/crux/models/ingestion.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/job.py` & `crux-1.3/crux/models/job.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/model.py` & `crux-1.3/crux/models/model.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/permission.py` & `crux-1.3/crux/models/permission.py`

 * *Files identical despite different names*

### Comparing `crux-1.2/crux/models/resource.py` & `crux-1.3/crux/models/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         # type: () -> bool
         """Deletes Resource from Dataset.
 
         Returns:
             bool: True if it is deleted.
         """
         headers = Headers({"content-type": "application/json", "accept": "application/json"})
-        return self.connection.api_call("DELETE", ["resources", self.id], headers=headers)
+        return self.connection.api_call("DELETE", ["v1", "resources", self.id], headers=headers)
 
     def update(self, name=None, description=None, tags=None, provenance=None):
         # type: (str, str, List[str], str) -> bool
         """Updates the metadata for Resource.
 
         Args:
             name (str): Name of resource. Defaults to None.
@@ -196,15 +196,15 @@
             self.raw_model["provenance"] = provenance
 
         body = self.raw_model
 
         log.debug("Body %s", body)
 
         resource_object = self.connection.api_call(
-            "PUT", ["resources", self.id], headers=headers, json=body, model=Resource
+            "PUT", ["v1", "resources", self.id], headers=headers, json=body, model=Resource
         )
 
         self.raw_model = resource_object.raw_model
 
         log.debug("Updated dataset %s with content %s", self.id, self.raw_model)
         return True
 
@@ -266,14 +266,15 @@
         Returns:
             bool: True if label is added, False otherwise.
         """
         headers = Headers({"content-type": "application/json", "accept": "application/json"})
         response_result = self.connection.api_call(
             "PUT",
             [
+                "v1",
                 "datasets",
                 self.dataset_id,
                 "resources",
                 self.id,
                 "labels",
                 label_key,
                 label_value,
@@ -296,15 +297,15 @@
 
         Returns:
             bool: True if label is deleted, False otherwise.
         """
         headers = Headers({"content-type": "application/json", "accept": "application/json"})
         response_result = self.connection.api_call(
             "DELETE",
-            ["datasets", self.dataset_id, "resources", self.id, "labels", label_key],
+            ["v1", "datasets", self.dataset_id, "resources", self.id, "labels", label_key],
             headers=headers,
         )
 
         if response_result:
             # Sync the latest data from API to prevent inconsistency
             self.refresh()
 
@@ -330,15 +331,15 @@
                     {"labelKey": str(label_key), "labelValue": str(label_value)}
                 )
 
         data = {"labels": labels_list}
 
         response_result = self.connection.api_call(
             "PUT",
-            ["datasets", self.dataset_id, "resources", self.id, "labels"],
+            ["v1", "datasets", self.dataset_id, "resources", self.id, "labels"],
             headers=headers,
             json=data,
         )
 
         if response_result:
             # Sync the latest data from API to prevent inconsistency
             self.refresh()
@@ -350,28 +351,28 @@
         """Fetches the folder of the resource.
 
         Returns:
             str: Folder name of the resource.
         """
         headers = Headers({"content-type": "application/json", "accept": "application/json"})
         response = self.connection.api_call(
-            "GET", ["resources", self.id, "folderpath"], headers=headers
+            "GET", ["v1", "resources", self.id, "folderpath"], headers=headers
         )
 
         return response.json().get("path")
 
     def _download(self, file_obj, media_type, chunk_size=DEFAULT_CHUNK_SIZE):
 
         if media_type is not None:
             headers = Headers({"accept": media_type})
         else:
             headers = None
 
         data = self.connection.api_call(
-            "GET", ["resources", self.id, "content"], headers=headers, stream=True
+            "GET", ["v1", "resources", self.id, "content"], headers=headers, stream=True
         )
 
         for chunk in data.iter_content(chunk_size=chunk_size):
             file_obj.write(chunk)
         data.close()
         return True
 
@@ -381,15 +382,15 @@
         Returns:
             bool: True, if it is able to refresh the model,
                 False otherwise.
         """
         # type () -> bool
         headers = Headers({"content-type": "application/json", "accept": "application/json"})
         resource_object = self.connection.api_call(
-            "GET", ["resources", self.id], headers=headers, model=Resource
+            "GET", ["v1", "resources", self.id], headers=headers, model=Resource
         )
 
         self.raw_model = resource_object.raw_model
 
         return True
```

### Comparing `crux-1.2/crux.egg-info/PKG-INFO` & `crux-1.3/crux.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,161 +1,16 @@
 Metadata-Version: 2.1
 Name: crux
-Version: 1.2
+Version: 1.3
 Summary: Crux Informatics API client library
 Home-page: https://github.com/cruxinformatics/crux-python
 Author: Crux Informatics, Inc.
 Author-email: python-opensource@cruxinformatics.com
 License: MIT
-Description: # Crux Python Client
-        
-        A Python library for interacting with the Crux platform.
-        
-        The aim of this module is to be a Pythonic way to use the Crux API reliably. It covers client functionality including scanning subscriptions, getting delivery status, and downloading files.
-        
-        Python 3.6+ is supported.
-        
-        **See [crux-python.cruxinformatics.com](https://crux-python.cruxinformatics.com/) for detailed documentation.**
-        
-        ## Installation
-        
-        Install a recent version of Python, and a Python dependency and virtual environment manager like [pipenv](https://pipenv.readthedocs.io/en/latest/). On macOS run:
-        
-        ```bash
-        brew install python
-        brew install pipenv
-        ```
-        
-        Install `crux` [from PyPI](https://pypi.org/project/crux/) in a virtual environment, and get a shell in that environment:
-        
-        ```bash
-        mkdir -p crux_example
-        cd crux_example
-        pipenv install "crux==1.2"
-        pipenv shell
-        ```
-        ## Getting Started
-        
-        Create a file, like example.py, and use the `crux` module:
-        
-        ```python
-        from crux import Crux
-        
-        conn = Crux()
-        identity = conn.whoami()
-        print("I am", identity.email)
-        ```
-        
-        Run the script:
-        
-        ```bash
-        HISTCONTROL=ignoreboth
-         export CRUX_API_KEY='YOUR_API_KEY'
-        python3 example.py
-        ```
-        
-        See the [installation](https://crux-python.cruxinformatics.com/en/latest/installation.html) and [authentication](https://crux-python.cruxinformatics.com/en/latest/authentication.html) documentation for details.
-        
-        ## Development
-        
-        Python 3.7 is required for development, which can be installed with `brew install python`. For heavy development work, every supported version of Python must be installed, see the pyenv documentation below.
-        
-        [Pipenv](https://pipenv.readthedocs.io/en/latest/) should be used to manage dependancies during development.
-        
-        1. [Install Pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv), on macOS run `brew install pipenv`
-        2. `git clone https://github.com/cruxinformatics/crux-python.git`
-        3. `cd crux-python`
-        4. `pipenv install --dev` to install the dependancies
-        5. `pipenv shell` to get a shell in the virtual environment
-        
-        ### Multiple Python versions
-        
-        To be able to run tests against all supported Python versions, you must have all supported Python versions installed. The test runner will look for binaries called `python2.7`, `python3.5`, `python3.6`, etc. There are multiple ways to install Python versions, we'll document using [pyenv](https://github.com/pyenv/pyenv).
-        
-        1. `brew install pyenv` to install
-        2. Put `eval "$(pyenv init -)"` towards the end of the shell configuration file (~/.bashrc or ~/.bash_profile), because it manipulates `$PATH`, for example:
-        
-            ```bash
-            echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc
-            ```
-        
-        3. Open a new Terminal to get an updated shell
-        4. Install required/missing Python versions (this assumes you have Python 2.7 already installed, otherwise install it too):
-        
-            ```bash
-            pyenv install 3.5.6
-            pyenv install 3.6.6
-            pyenv install 3.7.0
-            ```
-        
-        5. `pyenv global system 3.5.6 3.6.6 3.7.0` to make all the Python versions available
-        6. If you already have pipenv virtual environment, remove it with `pipenv --rm` so it detects the Python versions
-        7. `pipenv install --dev` to install all the dependancies
-        8. `pipenv shell` to get a shell in the virtual environment
-        
-        ### Running tests
-        
-        We use [Nox](https://nox.thea.codes/en/stable/) to automate running tests, and use `make` to automate running some commands. These commands should be run within a shell created with `pipenv shell`.
-        
-        ```bash
-        # Run all tests: lint, unit, format_check
-        make test
-        # Or
-        nox
-        
-        # Run only lint checks
-        make lint
-        # Or
-        nox -s lint
-        
-        # Run unit tests against all available Python versions
-        make unit
-        # Or
-        nox -s unit
-        
-        # Run integration tests agains all available Python versions
-         export CRUX_API_KEY="12345"
-        export CRUX_API_HOST="https://api.example.com"
-        make integration
-        # Or
-         export CRUX_API_KEY="12345"
-        export CRUX_API_HOST="https://api.example.com"
-        nox --s integration
-        
-        # Check formatting
-        make format_check
-        # Or
-        nox -s format_check
-        
-        # List all commands available
-        make
-        # Or
-        nox -l
-        
-        # Run unit test only against Python 3.7
-        nox -s unit-3.7
-        
-        # Reformat code
-        make format
-        
-        # Generate Sphinx HTML documentation
-        make docs
-        ```
-        
-        #### Running test scripts
-        
-        Manual testing scripts could be found at `tests/regression`.
-        In order to run one, i.e. `client.py`, follow the steps:
-        
-        1. copy corresponding `.env.dist` file as `.env` file (if you plan to run `client.py`, copy `client.env.dist` as `client.env`)
-        2. fill variables within `.env` file
-        3. launch the script (while being in the `tests/regression` folder, execute `python client.py`)
-        
 Keywords: crux-python
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -163,7 +18,152 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Crux Python Client
+
+A Python library for interacting with the Crux platform.
+
+The aim of this module is to be a Pythonic way to use the Crux API reliably. It covers client functionality including scanning subscriptions, getting delivery status, and downloading files.
+
+Python 3.6+ is supported.
+
+**See [crux-python.cruxinformatics.com](https://crux-python.cruxinformatics.com/) for detailed documentation.**
+
+## Installation
+
+Install a recent version of Python, and a Python dependency and virtual environment manager like [pipenv](https://pipenv.readthedocs.io/en/latest/). On macOS run:
+
+```bash
+brew install python
+brew install pipenv
+```
+
+Install `crux` [from PyPI](https://pypi.org/project/crux/) in a virtual environment, and get a shell in that environment:
+
+```bash
+mkdir -p crux_example
+cd crux_example
+pipenv install "crux==1.3"
+pipenv shell
+```
+## Getting Started
+
+Create a file, like example.py, and use the `crux` module:
+
+```python
+from crux import Crux
+
+conn = Crux()
+identity = conn.whoami()
+print("I am", identity.email)
+```
+
+Run the script:
+
+```bash
+HISTCONTROL=ignoreboth
+ export CRUX_API_KEY='YOUR_API_KEY'
+python3 example.py
+```
+
+See the [installation](https://crux-python.cruxinformatics.com/en/latest/installation.html) and [authentication](https://crux-python.cruxinformatics.com/en/latest/authentication.html) documentation for details.
+
+## Development
+
+Python 3.7 is required for development, which can be installed with `brew install python`. For heavy development work, every supported version of Python must be installed, see the pyenv documentation below.
+
+[Pipenv](https://pipenv.readthedocs.io/en/latest/) should be used to manage dependancies during development.
+
+1. [Install Pipenv](https://pipenv.readthedocs.io/en/latest/install/#installing-pipenv), on macOS run `brew install pipenv`
+2. `git clone https://github.com/cruxinformatics/crux-python.git`
+3. `cd crux-python`
+4. `pipenv install --dev` to install the dependancies
+5. `pipenv shell` to get a shell in the virtual environment
+
+### Multiple Python versions
+
+To be able to run tests against all supported Python versions, you must have all supported Python versions installed. The test runner will look for binaries called `python2.7`, `python3.5`, `python3.6`, etc. There are multiple ways to install Python versions, we'll document using [pyenv](https://github.com/pyenv/pyenv).
+
+1. `brew install pyenv` to install
+2. Put `eval "$(pyenv init -)"` towards the end of the shell configuration file (~/.bashrc or ~/.bash_profile), because it manipulates `$PATH`, for example:
+
+    ```bash
+    echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.bashrc
+    ```
+
+3. Open a new Terminal to get an updated shell
+4. Install required/missing Python versions (this assumes you have Python 2.7 already installed, otherwise install it too):
+
+    ```bash
+    pyenv install 3.5.6
+    pyenv install 3.6.6
+    pyenv install 3.7.0
+    ```
+
+5. `pyenv global system 3.5.6 3.6.6 3.7.0` to make all the Python versions available
+6. If you already have pipenv virtual environment, remove it with `pipenv --rm` so it detects the Python versions
+7. `pipenv install --dev` to install all the dependancies
+8. `pipenv shell` to get a shell in the virtual environment
+
+### Running tests
+
+We use [Nox](https://nox.thea.codes/en/stable/) to automate running tests, and use `make` to automate running some commands. These commands should be run within a shell created with `pipenv shell`.
+
+```bash
+# Run all tests: lint, unit, format_check
+make test
+# Or
+nox
+
+# Run only lint checks
+make lint
+# Or
+nox -s lint
+
+# Run unit tests against all available Python versions
+make unit
+# Or
+nox -s unit
+
+# Run integration tests agains all available Python versions
+ export CRUX_API_KEY="12345"
+export CRUX_API_HOST="https://api.example.com"
+make integration
+# Or
+ export CRUX_API_KEY="12345"
+export CRUX_API_HOST="https://api.example.com"
+nox --s integration
+
+# Check formatting
+make format_check
+# Or
+nox -s format_check
+
+# List all commands available
+make
+# Or
+nox -l
+
+# Run unit test only against Python 3.7
+nox -s unit-3.7
+
+# Reformat code
+make format
+
+# Generate Sphinx HTML documentation
+make docs
+```
+
+#### Running test scripts
+
+Manual testing scripts could be found at `tests/regression`.
+In order to run one, i.e. `client.py`, follow the steps:
+
+1. copy corresponding `.env.dist` file as `.env` file (if you plan to run `client.py`, copy `client.env.dist` as `client.env`)
+2. fill variables within `.env` file
+3. launch the script (while being in the `tests/regression` folder, execute `python client.py`)
```

### Comparing `crux-1.2/crux.egg-info/SOURCES.txt` & `crux-1.3/crux.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 crux/__init__.py
 crux/__version__.py
 crux/_client.py
 crux/_compat.py
```

### Comparing `crux-1.2/setup.py` & `crux-1.3/setup.py`

 * *Files identical despite different names*

