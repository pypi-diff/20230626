# Comparing `tmp/assistorg-api-0.0.2.tar.gz` & `tmp/assistorg-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistorg-api-0.0.2.tar", last modified: Wed Jun 21 01:40:17 2023, max compression
+gzip compressed data, was "assistorg-api-0.0.3.tar", last modified: Mon Jun 26 03:48:49 2023, max compression
```

## Comparing `assistorg-api-0.0.2.tar` & `assistorg-api-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/
--rw-rw-rw-   0        0        0      201 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3835 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1108 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1654 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1043 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.186645 assistorg-api-0.0.2/assist_api_wrapper/
--rw-rw-rw-   0        0        0      174 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/assist_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0       20 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/assist_api_wrapper/assist_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.186645 assistorg-api-0.0.2/assistorg_api.egg-info/
--rw-rw-rw-   0        0        0     1654 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-21 01:27:29.000000 assistorg-api-0.0.2/assistorg_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-06-21 01:40:17.000000 assistorg-api-0.0.2/assistorg_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/docs/
--rw-rw-rw-   0        0        0      639 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/authors.rst
--rw-rw-rw-   0        0        0     5128 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/history.rst
--rw-rw-rw-   0        0        0      335 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/index.rst
--rw-rw-rw-   0        0        0     1321 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/installation.rst
--rwxrwxrwx   0        0        0      816 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/readme.rst
--rw-rw-rw-   0        0        0       98 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/docs/usage.rst
--rw-rw-rw-   0        0        0      414 2023-06-21 01:40:17.217895 assistorg-api-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-06-21 01:39:55.000000 assistorg-api-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:40:17.202275 assistorg-api-0.0.2/tests/
--rw-rw-rw-   0        0        0       49 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      463 2023-06-19 20:44:40.000000 assistorg-api-0.0.2/tests/test_assist_api_wrapper.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962809 assistorg-api-0.0.3/
+-rw-r--r--   0 monte      (501) staff       (20)      188 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/AUTHORS.rst
+-rw-r--r--   0 monte      (501) staff       (20)     3707 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1086 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/LICENSE
+-rw-r--r--   0 monte      (501) staff       (20)      262 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/MANIFEST.in
+-rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:48:49.962870 assistorg-api-0.0.3/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      670 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/README.md
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.960985 assistorg-api-0.0.3/assistorg_api.egg-info/
+-rw-r--r--   0 monte      (501) staff       (20)     1479 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/PKG-INFO
+-rw-r--r--   0 monte      (501) staff       (20)      477 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:43:23.000000 assistorg-api-0.0.3/assistorg_api.egg-info/not-zip-safe
+-rw-r--r--   0 monte      (501) staff       (20)        1 2023-06-26 03:48:49.000000 assistorg-api-0.0.3/assistorg_api.egg-info/top_level.txt
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962409 assistorg-api-0.0.3/docs/
+-rw-r--r--   0 monte      (501) staff       (20)      619 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/Makefile
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/authors.rst
+-rw-r--r--   0 monte      (501) staff       (20)     4966 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/conf.py
+-rw-r--r--   0 monte      (501) staff       (20)       33 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/contributing.rst
+-rw-r--r--   0 monte      (501) staff       (20)       28 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/history.rst
+-rw-r--r--   0 monte      (501) staff       (20)      315 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/index.rst
+-rw-r--r--   0 monte      (501) staff       (20)     1270 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/installation.rst
+-rw-r--r--   0 monte      (501) staff       (20)      780 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/make.bat
+-rw-r--r--   0 monte      (501) staff       (20)       27 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/readme.rst
+-rw-r--r--   0 monte      (501) staff       (20)       91 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/docs/usage.rst
+-rw-r--r--   0 monte      (501) staff       (20)      385 2023-06-26 03:48:49.963088 assistorg-api-0.0.3/setup.cfg
+-rw-r--r--   0 monte      (501) staff       (20)     1378 2023-06-26 03:46:16.000000 assistorg-api-0.0.3/setup.py
+drwxr-xr-x   0 monte      (501) staff       (20)        0 2023-06-26 03:48:49.962678 assistorg-api-0.0.3/tests/
+-rw-r--r--   0 monte      (501) staff       (20)       48 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/tests/__init__.py
+-rw-r--r--   0 monte      (501) staff       (20)      442 2023-06-26 03:31:11.000000 assistorg-api-0.0.3/tests/test_assist_api_wrapper.py
```

### Comparing `assistorg-api-0.0.2/CONTRIBUTING.rst` & `assistorg-api-0.0.3/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/montesclarosglennbenedict/assist_api_wrapper/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-ASSIST API Wrapper could always use more documentation, whether as part of the
-official ASSIST API Wrapper docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/montesclarosglennbenedict/assist_api_wrapper/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `assist_api_wrapper` for local development.
-
-1. Fork the `assist_api_wrapper` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/assist_api_wrapper.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv assist_api_wrapper
-    $ cd assist_api_wrapper/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 assist_api_wrapper tests
-    $ python setup.py test or pytest
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/montesclarosglennbenedict/assist_api_wrapper/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-
-    $ python -m unittest tests.test_assist_api_wrapper
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/montesclarosglennbenedict/assist_api_wrapper/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+ASSIST API Wrapper could always use more documentation, whether as part of the
+official ASSIST API Wrapper docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/montesclarosglennbenedict/assist_api_wrapper/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `assist_api_wrapper` for local development.
+
+1. Fork the `assist_api_wrapper` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/assist_api_wrapper.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv assist_api_wrapper
+    $ cd assist_api_wrapper/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 assist_api_wrapper tests
+    $ python setup.py test or pytest
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+   https://travis-ci.com/montesclarosglennbenedict/assist_api_wrapper/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+
+    $ python -m unittest tests.test_assist_api_wrapper
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bump2version patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `assistorg-api-0.0.2/LICENSE` & `assistorg-api-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Glenn Benedict Montesclaros
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Glenn Benedict Montesclaros
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `assistorg-api-0.0.2/PKG-INFO` & `assistorg-api-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1
-Name: assistorg-api
-Version: 0.0.2
-Summary: Unofficial API wrapper for ASSIST.org's API.
-Home-page: https://github.com/montesclarosglennbenedict/assist_api_wrapper
-Author: Glenn Benedict Montesclaros
-Author-email: montesclarosglennbenedict@gmail.com
-License: MIT license
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# ASSIST API Wrapper
-
-[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
-
-[![image](https://img.shields.io/travis/montesclarosglennbenedict/assistorg-api.svg)](https://travis-ci.com/montesclarosglennbenedict/assistorg-api)
-
-[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
-
-Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
-
--   Free software: MIT license
--   Documentation: <https://assistorg-api.readthedocs.io>.
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with
-[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
-[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-project template.
-
-
+Metadata-Version: 2.1
+Name: assistorg-api
+Version: 0.0.3
+Summary: Unofficial API wrapper for ASSIST.org's API.
+Home-page: https://github.com/montesclarosglennbenedict/assistapi-org
+Author: Glenn Benedict Montesclaros
+Author-email: montesclarosglennbenedict@gmail.com
+License: MIT license
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# ASSIST API Wrapper
+
+[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
+
+[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
+
+Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
+
+-   Free software: MIT license
+-   Documentation: <https://assistorg-api.readthedocs.io>.
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+project template.
+
+
+there is no history, test
```

### Comparing `assistorg-api-0.0.2/assistorg_api.egg-info/PKG-INFO` & `assistorg-api-0.0.3/assistorg_api.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-Metadata-Version: 2.1
-Name: assistorg-api
-Version: 0.0.2
-Summary: Unofficial API wrapper for ASSIST.org's API.
-Home-page: https://github.com/montesclarosglennbenedict/assist_api_wrapper
-Author: Glenn Benedict Montesclaros
-Author-email: montesclarosglennbenedict@gmail.com
-License: MIT license
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# ASSIST API Wrapper
-
-[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
-
-[![image](https://img.shields.io/travis/montesclarosglennbenedict/assistorg-api.svg)](https://travis-ci.com/montesclarosglennbenedict/assistorg-api)
-
-[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
-
-Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
-
--   Free software: MIT license
--   Documentation: <https://assistorg-api.readthedocs.io>.
-
-## Features
-
--   TODO
-
-## Credits
-
-This package was created with
-[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
-[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
-project template.
-
-
+Metadata-Version: 2.1
+Name: assistorg-api
+Version: 0.0.3
+Summary: Unofficial API wrapper for ASSIST.org's API.
+Home-page: https://github.com/montesclarosglennbenedict/assistapi-org
+Author: Glenn Benedict Montesclaros
+Author-email: montesclarosglennbenedict@gmail.com
+License: MIT license
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+# ASSIST API Wrapper
+
+[![image](https://img.shields.io/pypi/v/assistorg-api.svg)](https://pypi.python.org/pypi/assistorg-api/)
+
+[![Documentation Status](https://readthedocs.org/projects/assistorg-api/badge/?version=latest)](https://assistorg-api.readthedocs.io/en/latest/?version=latest)
+
+Unofficial API wrapper for ASSIST.org\'s API. UNRELEASED.
+
+-   Free software: MIT license
+-   Documentation: <https://assistorg-api.readthedocs.io>.
+
+## Features
+
+-   TODO
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
+project template.
+
+
+there is no history, test
```

### Comparing `assistorg-api-0.0.2/docs/Makefile` & `assistorg-api-0.0.3/docs/Makefile`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = assist_api_wrapper
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python -msphinx
+SPHINXPROJ    = assist_api_wrapper
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `assistorg-api-0.0.2/docs/conf.py` & `assistorg-api-0.0.3/docs/conf.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-#!/usr/bin/env python
-#
-# assist_api_wrapper documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import assist_api_wrapper
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'ASSIST API Wrapper'
-copyright = "2023, Glenn Benedict Montesclaros"
-author = "Glenn Benedict Montesclaros"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = assist_api_wrapper.__version__
-# The full version, including alpha/beta/rc tags.
-release = assist_api_wrapper.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = 'alabaster'
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'assist_api_wrapperdoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'assist_api_wrapper.tex',
-     'ASSIST API Wrapper Documentation',
-     'Glenn Benedict Montesclaros', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'assist_api_wrapper',
-     'ASSIST API Wrapper Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'assist_api_wrapper',
-     'ASSIST API Wrapper Documentation',
-     author,
-     'assist_api_wrapper',
-     'One line description of project.',
-     'Miscellaneous'),
-]
-
-
-
+#!/usr/bin/env python
+#
+# assist_api_wrapper documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+import assist_api_wrapper
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = 'ASSIST API Wrapper'
+copyright = "2023, Glenn Benedict Montesclaros"
+author = "Glenn Benedict Montesclaros"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = assist_api_wrapper.__version__
+# The full version, including alpha/beta/rc tags.
+release = assist_api_wrapper.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = 'alabaster'
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'assist_api_wrapperdoc'
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'assist_api_wrapper.tex',
+     'ASSIST API Wrapper Documentation',
+     'Glenn Benedict Montesclaros', 'manual'),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'assist_api_wrapper',
+     'ASSIST API Wrapper Documentation',
+     [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'assist_api_wrapper',
+     'ASSIST API Wrapper Documentation',
+     author,
+     'assist_api_wrapper',
+     'One line description of project.',
+     'Miscellaneous'),
+]
+
+
+
```

### Comparing `assistorg-api-0.0.2/docs/installation.rst` & `assistorg-api-0.0.3/docs/installation.rst`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install ASSIST API Wrapper, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install assist_api_wrapper
-
-This is the preferred method to install ASSIST API Wrapper, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for ASSIST API Wrapper can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/montesclarosglennbenedict/assist_api_wrapper
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/montesclarosglennbenedict/assist_api_wrapper/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/montesclarosglennbenedict/assist_api_wrapper
-.. _tarball: https://github.com/montesclarosglennbenedict/assist_api_wrapper/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install ASSIST API Wrapper, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install assist_api_wrapper
+
+This is the preferred method to install ASSIST API Wrapper, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for ASSIST API Wrapper can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/montesclarosglennbenedict/assist_api_wrapper
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/montesclarosglennbenedict/assist_api_wrapper/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/montesclarosglennbenedict/assist_api_wrapper
+.. _tarball: https://github.com/montesclarosglennbenedict/assist_api_wrapper/tarball/master
```

### Comparing `assistorg-api-0.0.2/docs/make.bat` & `assistorg-api-0.0.3/docs/make.bat`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=python -msphinx
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-set SPHINXPROJ=assist_api_wrapper
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
-	echo.then set the SPHINXBUILD environment variable to point to the full
-	echo.path of the 'sphinx-build' executable. Alternatively you may add the
-	echo.Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
-	exit /b 1
-)
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=python -msphinx
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+set SPHINXPROJ=assist_api_wrapper
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
+	echo.then set the SPHINXBUILD environment variable to point to the full
+	echo.path of the 'sphinx-build' executable. Alternatively you may add the
+	echo.Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.http://sphinx-doc.org/
+	exit /b 1
+)
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+
+:end
+popd
```

