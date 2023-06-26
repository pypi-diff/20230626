# Comparing `tmp/flora_utils_py-0.1.1.tar.gz` & `tmp/flora_utils_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flora_utils_py-0.1.1.tar", max compression
+gzip compressed data, was "flora_utils_py-0.1.2.tar", max compression
```

## Comparing `flora_utils_py-0.1.1.tar` & `flora_utils_py-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    10883 2023-02-02 13:33:00.169698 flora_utils_py-0.1.1/LICENSE
--rw-r--r--   0        0        0    12823 2023-02-02 13:33:00.170698 flora_utils_py-0.1.1/README.md
--rw-r--r--   0        0        0      504 2023-02-02 13:33:00.170698 flora_utils_py-0.1.1/flora_utils_py/__init__.py
--rw-r--r--   0        0        0     1831 2023-02-03 10:00:18.239848 flora_utils_py-0.1.1/flora_utils_py/exceptions.py
--rw-r--r--   0        0        0     3587 2023-02-03 11:46:15.053569 flora_utils_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14001 1970-01-01 00:00:00.000000 flora_utils_py-0.1.1/setup.py
--rw-r--r--   0        0        0    14168 1970-01-01 00:00:00.000000 flora_utils_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10883 2023-02-24 06:24:43.957048 flora_utils_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0    12823 2023-02-24 06:24:43.957048 flora_utils_py-0.1.2/README.md
+-rw-r--r--   0        0        0      504 2023-02-24 06:24:43.957048 flora_utils_py-0.1.2/flora_utils_py/__init__.py
+-rw-r--r--   0        0        0     1830 2023-06-26 14:50:46.446310 flora_utils_py-0.1.2/flora_utils_py/exceptions.py
+-rw-r--r--   0        0        0     3587 2023-06-26 14:54:20.955033 flora_utils_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13971 1970-01-01 00:00:00.000000 flora_utils_py-0.1.2/PKG-INFO
```

### Comparing `flora_utils_py-0.1.1/LICENSE` & `flora_utils_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flora_utils_py-0.1.1/README.md` & `flora_utils_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flora_utils_py-0.1.1/flora_utils_py/exceptions.py` & `flora_utils_py-0.1.2/flora_utils_py/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Custom exceptions classes for Flora."""
-from typing import Any, Optional, Union
-
 import json
 from datetime import datetime as dt
 from sys import exc_info
+from typing import Any, Optional, Union
 
 
 class FloraException(Exception):
     """Base exception for all Flora exceptions."""
 
     def __init__(
         self,
         status_code: int,
         error_code: str,
         message: str,
         module: str = "model",
         datetime: Optional[Union[str, dt]] = None,
         user_id: Optional[str] = None,
-        workplace_id: Optional[str] = None,
+        workspace_id: Optional[str] = None,
         data: Optional[Any] = None,
     ):
         self.status_code = status_code
         self.error_code = error_code
         self.module = module
         self.message = message
         if datetime is None:
@@ -29,15 +28,15 @@
         else:
             # Convert datetime to isoformat if it is not already
             if isinstance(datetime, dt):
                 self.datetime = datetime.isoformat()
             else:
                 self.datetime = datetime
         self.user_id = user_id
-        self.workplace_id = workplace_id
+        self.workspace_id = workspace_id
         self.data = data
 
         self.traceback = exc_info()
 
         super().__init__(str(self))
 
     def __str__(self) -> str:
@@ -53,11 +52,11 @@
             {
                 "errorCode": f"{self.module}/{self.error_code}",
                 "statusCode": self.status_code,
                 "module": self.module,
                 "message": self.message,
                 "datetime": self.datetime,
                 "userId": self.user_id,
-                "workplaceId": self.workplace_id,
+                "workspaceId": self.workspace_id,
                 "data": self.data,
             }
         )
```

### Comparing `flora_utils_py-0.1.1/pyproject.toml` & `flora_utils_py-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flora-utils-py"
-version = "0.1.1"
+version = "0.1.2"
 description = "Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template"
 readme = "README.md"
 authors = ["Flora <tiencheng@flora.so>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/Flora/flora-utils-py"
 homepage = "https://github.com/Flora/flora-utils-py"
```

### Comparing `flora_utils_py-0.1.1/setup.py` & `flora_utils_py-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,420 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flora-utils-py
+Version: 0.1.2
+Summary: Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
+Home-page: https://github.com/Flora/flora-utils-py
+License: Apache Software License 2.0
+Author: Flora
+Author-email: tiencheng@flora.so
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: importlib_metadata (>=4.5.0,<5.0.0) ; python_version < "3.8"
+Project-URL: Repository, https://github.com/Flora/flora-utils-py
+Description-Content-Type: text/markdown
 
-packages = \
-['flora_utils_py']
+# flora-utils-py
 
-package_data = \
-{'': ['*']}
+<div align="center">
 
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=4.5.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'flora-utils-py',
-    'version': '0.1.1',
-    'description': 'Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template',
-    'long_description': '# flora-utils-py\n\n<div align="center">\n\n[![Build status](https://github.com/Flora/flora-utils-py/workflows/build/badge.svg?branch=master&event=push)](https://github.com/Flora/flora-utils-py/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/flora-utils-py.svg)](https://pypi.org/project/flora-utils-py/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Flora/flora-utils-py/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Flora/flora-utils-py/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Flora/flora-utils-py/releases)\n[![License](https://img.shields.io/github/license/Flora/flora-utils-py)](https://github.com/Flora/flora-utils-py/blob/master/LICENSE)\n![Coverage Report](assets/images/coverage.svg)\n\nAwesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template\n\n</div>\n\n## Very first steps\n\n### Initialize your code\n\n1. Initialize `git` inside your repo:\n\n```bash\ncd flora-utils-py && git init\n```\n\n2. If you don\'t have `Poetry` installed run:\n\n```bash\nmake poetry-download\n```\n\n3. Initialize poetry and install `pre-commit` hooks:\n\n```bash\nmake install\nmake pre-commit-install\n```\n\n4. Run the codestyle:\n\n```bash\nmake codestyle\n```\n\n5. Upload initial code to GitHub:\n\n```bash\ngit add .\ngit commit -m ":tada: Initial commit"\ngit branch -M main\ngit remote add origin https://github.com/Flora/flora-utils-py.git\ngit push -u origin main\n```\n\n### Set up bots\n\n- Set up [Dependabot](https://docs.github.com/en/github/administering-a-repository/enabling-and-disabling-version-updates#enabling-github-dependabot-version-updates) to ensure you have the latest dependencies.\n- Set up [Stale bot](https://github.com/apps/stale) for automatic issue closing.\n\n### Poetry\n\nWant to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).\n\n<details>\n<summary>Details about Poetry</summary>\n<p>\n\nPoetry\'s [commands](https://python-poetry.org/docs/cli/#commands) are very intuitive and easy to learn, like:\n\n- `poetry add numpy@latest`\n- `poetry run pytest`\n- `poetry publish --build`\n\netc\n</p>\n</details>\n\n### Building and releasing your package\n\nBuilding a new version of the application contains steps:\n\n- Bump the version of your package `poetry version <version>`. You can pass the new version explicitly, or a rule such as `major`, `minor`, or `patch`. For more details, refer to the [Semantic Versions](https://semver.org/) standard.\n- Make a commit to `GitHub`.\n- Create a `GitHub release`.\n- And... publish 🙂 `poetry publish --build`\n\n## 🎯 What\'s next\n\nWell, that\'s up to you 💪🏻. I can only recommend the packages and articles that helped me.\n\n- [`Typer`](https://github.com/tiangolo/typer) is great for creating CLI applications.\n- [`Rich`](https://github.com/willmcgugan/rich) makes it easy to add beautiful formatting in the terminal.\n- [`Pydantic`](https://github.com/samuelcolvin/pydantic/) – data validation and settings management using Python type hinting.\n- [`Loguru`](https://github.com/Delgan/loguru) makes logging (stupidly) simple.\n- [`tqdm`](https://github.com/tqdm/tqdm) – fast, extensible progress bar for Python and CLI.\n- [`IceCream`](https://github.com/gruns/icecream) is a little library for sweet and creamy debugging.\n- [`orjson`](https://github.com/ijl/orjson) – ultra fast JSON parsing library.\n- [`Returns`](https://github.com/dry-python/returns) makes you function\'s output meaningful, typed, and safe!\n- [`Hydra`](https://github.com/facebookresearch/hydra) is a framework for elegantly configuring complex applications.\n- [`FastAPI`](https://github.com/tiangolo/fastapi) is a type-driven asynchronous web framework.\n\nArticles:\n\n- [Open Source Guides](https://opensource.guide/).\n- [A handy guide to financial support for open source](https://github.com/nayafia/lemonade-stand)\n- [GitHub Actions Documentation](https://help.github.com/en/actions).\n- Maybe you would like to add [gitmoji](https://gitmoji.carloscuesta.me/) to commit names. This is really funny. 😄\n\n## 🚀 Features\n\n### Development features\n\n- Supports for `Python 3.7` and higher.\n- [`Poetry`](https://python-poetry.org/) as the dependencies manager. See configuration in [`pyproject.toml`](https://github.com/Flora/flora-utils-py/blob/master/pyproject.toml) and [`setup.cfg`](https://github.com/Flora/flora-utils-py/blob/master/setup.cfg).\n- Automatic codestyle with [`black`](https://github.com/psf/black), [`isort`](https://github.com/timothycrosley/isort) and [`pyupgrade`](https://github.com/asottile/pyupgrade).\n- Ready-to-use [`pre-commit`](https://pre-commit.com/) hooks with code-formatting.\n- Type checks with [`mypy`](https://mypy.readthedocs.io); docstring checks with [`darglint`](https://github.com/terrencepreilly/darglint); security checks with [`safety`](https://github.com/pyupio/safety) and [`bandit`](https://github.com/PyCQA/bandit)\n- Testing with [`pytest`](https://docs.pytest.org/en/latest/).\n- Ready-to-use [`.editorconfig`](https://github.com/Flora/flora-utils-py/blob/master/.editorconfig), [`.dockerignore`](https://github.com/Flora/flora-utils-py/blob/master/.dockerignore), and [`.gitignore`](https://github.com/Flora/flora-utils-py/blob/master/.gitignore). You don\'t have to worry about those things.\n\n### Deployment features\n\n- `GitHub` integration: issue and pr templates.\n- `Github Actions` with predefined [build workflow](https://github.com/Flora/flora-utils-py/blob/master/.github/workflows/build.yml) as the default CI/CD.\n- Everything is already set up for security checks, codestyle checks, code formatting, testing, linting, docker builds, etc with [`Makefile`](https://github.com/Flora/flora-utils-py/blob/master/Makefile#L89). More details in [makefile-usage](#makefile-usage).\n- [Dockerfile](https://github.com/Flora/flora-utils-py/blob/master/docker/Dockerfile) for your package.\n- Always up-to-date dependencies with [`@dependabot`](https://dependabot.com/). You will only [enable it](https://docs.github.com/en/github/administering-a-repository/enabling-and-disabling-version-updates#enabling-github-dependabot-version-updates).\n- Automatic drafts of new releases with [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). You may see the list of labels in [`release-drafter.yml`](https://github.com/Flora/flora-utils-py/blob/master/.github/release-drafter.yml). Works perfectly with [Semantic Versions](https://semver.org/) specification.\n\n### Open source community features\n\n- Ready-to-use [Pull Requests templates](https://github.com/Flora/flora-utils-py/blob/master/.github/PULL_REQUEST_TEMPLATE.md) and several [Issue templates](https://github.com/Flora/flora-utils-py/tree/master/.github/ISSUE_TEMPLATE).\n- Files such as: `LICENSE`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `SECURITY.md` are generated automatically.\n- [`Stale bot`](https://github.com/apps/stale) that closes abandoned issues after a period of inactivity. (You will only [need to setup free plan](https://github.com/marketplace/stale)). Configuration is [here](https://github.com/Flora/flora-utils-py/blob/master/.github/.stale.yml).\n- [Semantic Versions](https://semver.org/) specification with [`Release Drafter`](https://github.com/marketplace/actions/release-drafter).\n\n## Installation\n\n```bash\npip install -U flora-utils-py\n```\n\nor install with `Poetry`\n\n```bash\npoetry add flora-utils-py\n```\n\n\n\n### Makefile usage\n\n[`Makefile`](https://github.com/Flora/flora-utils-py/blob/master/Makefile) contains a lot of functions for faster development.\n\n<details>\n<summary>1. Download and remove Poetry</summary>\n<p>\n\nTo download and install Poetry run:\n\n```bash\nmake poetry-download\n```\n\nTo uninstall\n\n```bash\nmake poetry-remove\n```\n\n</p>\n</details>\n\n<details>\n<summary>2. Install all dependencies and pre-commit hooks</summary>\n<p>\n\nInstall requirements:\n\n```bash\nmake install\n```\n\nPre-commit hooks coulb be installed after `git init` via\n\n```bash\nmake pre-commit-install\n```\n\n</p>\n</details>\n\n<details>\n<summary>3. Codestyle</summary>\n<p>\n\nAutomatic formatting uses `pyupgrade`, `isort` and `black`.\n\n```bash\nmake codestyle\n\n# or use synonym\nmake formatting\n```\n\nCodestyle checks only, without rewriting files:\n\n```bash\nmake check-codestyle\n```\n\n> Note: `check-codestyle` uses `isort`, `black` and `darglint` library\n\nUpdate all dev libraries to the latest version using one comand\n\n```bash\nmake update-dev-deps\n```\n\n<details>\n<summary>4. Code security</summary>\n<p>\n\n```bash\nmake check-safety\n```\n\nThis command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.\n\n```bash\nmake check-safety\n```\n\n</p>\n</details>\n\n</p>\n</details>\n\n<details>\n<summary>5. Type checks</summary>\n<p>\n\nRun `mypy` static type checker\n\n```bash\nmake mypy\n```\n\n</p>\n</details>\n\n<details>\n<summary>6. Tests with coverage badges</summary>\n<p>\n\nRun `pytest`\n\n```bash\nmake test\n```\n\n</p>\n</details>\n\n<details>\n<summary>7. All linters</summary>\n<p>\n\nOf course there is a command to ~~rule~~ run all linters in one:\n\n```bash\nmake lint\n```\n\nthe same as:\n\n```bash\nmake test && make check-codestyle && make mypy && make check-safety\n```\n\n</p>\n</details>\n\n<details>\n<summary>8. Docker</summary>\n<p>\n\n```bash\nmake docker-build\n```\n\nwhich is equivalent to:\n\n```bash\nmake docker-build VERSION=latest\n```\n\nRemove docker image with\n\n```bash\nmake docker-remove\n```\n\nMore information [about docker](https://github.com/Flora/flora-utils-py/tree/master/docker).\n\n</p>\n</details>\n\n<details>\n<summary>9. Cleanup</summary>\n<p>\nDelete pycache files\n\n```bash\nmake pycache-remove\n```\n\nRemove package build\n\n```bash\nmake build-remove\n```\n\nDelete .DS_STORE files\n\n```bash\nmake dsstore-remove\n```\n\nRemove .mypycache\n\n```bash\nmake mypycache-remove\n```\n\nOr to remove all above run:\n\n```bash\nmake cleanup\n```\n\n</p>\n</details>\n\n## 📈 Releases\n\nYou can see the list of available releases on the [GitHub Releases](https://github.com/Flora/flora-utils-py/releases) page.\n\nWe follow [Semantic Versions](https://semver.org/) specification.\n\nWe use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.\n\n### List of labels and corresponding titles\n\n|               **Label**               |  **Title in Releases**  |\n| :-----------------------------------: | :---------------------: |\n|       `enhancement`, `feature`        |       🚀 Features       |\n| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |\n|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |\n|              `breaking`               |   💥 Breaking Changes   |\n|            `documentation`            |    📝 Documentation     |\n|            `dependencies`             | ⬆️ Dependencies updates |\n\nYou can update it in [`release-drafter.yml`](https://github.com/Flora/flora-utils-py/blob/master/.github/release-drafter.yml).\n\nGitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/Flora/flora-utils-py)](https://github.com/Flora/flora-utils-py/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `Apache Software License 2.0` license. See [LICENSE](https://github.com/Flora/flora-utils-py/blob/master/LICENSE) for more details.\n\n## 📃 Citation\n\n```bibtex\n@misc{flora-utils-py,\n  author = {Flora},\n  title = {Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template},\n  year = {2023},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/Flora/flora-utils-py}}\n}\n```\n\n## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)\n',
-    'author': 'Flora',
-    'author_email': 'tiencheng@flora.so',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Flora/flora-utils-py',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
+[![Build status](https://github.com/Flora/flora-utils-py/workflows/build/badge.svg?branch=master&event=push)](https://github.com/Flora/flora-utils-py/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/flora-utils-py.svg)](https://pypi.org/project/flora-utils-py/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/Flora/flora-utils-py/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Flora/flora-utils-py/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Flora/flora-utils-py/releases)
+[![License](https://img.shields.io/github/license/Flora/flora-utils-py)](https://github.com/Flora/flora-utils-py/blob/master/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
+
+Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template
+
+</div>
+
+## Very first steps
+
+### Initialize your code
+
+1. Initialize `git` inside your repo:
+
+```bash
+cd flora-utils-py && git init
+```
+
+2. If you don't have `Poetry` installed run:
+
+```bash
+make poetry-download
+```
+
+3. Initialize poetry and install `pre-commit` hooks:
+
+```bash
+make install
+make pre-commit-install
+```
+
+4. Run the codestyle:
+
+```bash
+make codestyle
+```
+
+5. Upload initial code to GitHub:
+
+```bash
+git add .
+git commit -m ":tada: Initial commit"
+git branch -M main
+git remote add origin https://github.com/Flora/flora-utils-py.git
+git push -u origin main
+```
+
+### Set up bots
+
+- Set up [Dependabot](https://docs.github.com/en/github/administering-a-repository/enabling-and-disabling-version-updates#enabling-github-dependabot-version-updates) to ensure you have the latest dependencies.
+- Set up [Stale bot](https://github.com/apps/stale) for automatic issue closing.
+
+### Poetry
+
+Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
+
+<details>
+<summary>Details about Poetry</summary>
+<p>
+
+Poetry's [commands](https://python-poetry.org/docs/cli/#commands) are very intuitive and easy to learn, like:
+
+- `poetry add numpy@latest`
+- `poetry run pytest`
+- `poetry publish --build`
+
+etc
+</p>
+</details>
+
+### Building and releasing your package
+
+Building a new version of the application contains steps:
+
+- Bump the version of your package `poetry version <version>`. You can pass the new version explicitly, or a rule such as `major`, `minor`, or `patch`. For more details, refer to the [Semantic Versions](https://semver.org/) standard.
+- Make a commit to `GitHub`.
+- Create a `GitHub release`.
+- And... publish 🙂 `poetry publish --build`
+
+## 🎯 What's next
+
+Well, that's up to you 💪🏻. I can only recommend the packages and articles that helped me.
+
+- [`Typer`](https://github.com/tiangolo/typer) is great for creating CLI applications.
+- [`Rich`](https://github.com/willmcgugan/rich) makes it easy to add beautiful formatting in the terminal.
+- [`Pydantic`](https://github.com/samuelcolvin/pydantic/) – data validation and settings management using Python type hinting.
+- [`Loguru`](https://github.com/Delgan/loguru) makes logging (stupidly) simple.
+- [`tqdm`](https://github.com/tqdm/tqdm) – fast, extensible progress bar for Python and CLI.
+- [`IceCream`](https://github.com/gruns/icecream) is a little library for sweet and creamy debugging.
+- [`orjson`](https://github.com/ijl/orjson) – ultra fast JSON parsing library.
+- [`Returns`](https://github.com/dry-python/returns) makes you function's output meaningful, typed, and safe!
+- [`Hydra`](https://github.com/facebookresearch/hydra) is a framework for elegantly configuring complex applications.
+- [`FastAPI`](https://github.com/tiangolo/fastapi) is a type-driven asynchronous web framework.
+
+Articles:
+
+- [Open Source Guides](https://opensource.guide/).
+- [A handy guide to financial support for open source](https://github.com/nayafia/lemonade-stand)
+- [GitHub Actions Documentation](https://help.github.com/en/actions).
+- Maybe you would like to add [gitmoji](https://gitmoji.carloscuesta.me/) to commit names. This is really funny. 😄
+
+## 🚀 Features
+
+### Development features
+
+- Supports for `Python 3.7` and higher.
+- [`Poetry`](https://python-poetry.org/) as the dependencies manager. See configuration in [`pyproject.toml`](https://github.com/Flora/flora-utils-py/blob/master/pyproject.toml) and [`setup.cfg`](https://github.com/Flora/flora-utils-py/blob/master/setup.cfg).
+- Automatic codestyle with [`black`](https://github.com/psf/black), [`isort`](https://github.com/timothycrosley/isort) and [`pyupgrade`](https://github.com/asottile/pyupgrade).
+- Ready-to-use [`pre-commit`](https://pre-commit.com/) hooks with code-formatting.
+- Type checks with [`mypy`](https://mypy.readthedocs.io); docstring checks with [`darglint`](https://github.com/terrencepreilly/darglint); security checks with [`safety`](https://github.com/pyupio/safety) and [`bandit`](https://github.com/PyCQA/bandit)
+- Testing with [`pytest`](https://docs.pytest.org/en/latest/).
+- Ready-to-use [`.editorconfig`](https://github.com/Flora/flora-utils-py/blob/master/.editorconfig), [`.dockerignore`](https://github.com/Flora/flora-utils-py/blob/master/.dockerignore), and [`.gitignore`](https://github.com/Flora/flora-utils-py/blob/master/.gitignore). You don't have to worry about those things.
+
+### Deployment features
+
+- `GitHub` integration: issue and pr templates.
+- `Github Actions` with predefined [build workflow](https://github.com/Flora/flora-utils-py/blob/master/.github/workflows/build.yml) as the default CI/CD.
+- Everything is already set up for security checks, codestyle checks, code formatting, testing, linting, docker builds, etc with [`Makefile`](https://github.com/Flora/flora-utils-py/blob/master/Makefile#L89). More details in [makefile-usage](#makefile-usage).
+- [Dockerfile](https://github.com/Flora/flora-utils-py/blob/master/docker/Dockerfile) for your package.
+- Always up-to-date dependencies with [`@dependabot`](https://dependabot.com/). You will only [enable it](https://docs.github.com/en/github/administering-a-repository/enabling-and-disabling-version-updates#enabling-github-dependabot-version-updates).
+- Automatic drafts of new releases with [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). You may see the list of labels in [`release-drafter.yml`](https://github.com/Flora/flora-utils-py/blob/master/.github/release-drafter.yml). Works perfectly with [Semantic Versions](https://semver.org/) specification.
+
+### Open source community features
+
+- Ready-to-use [Pull Requests templates](https://github.com/Flora/flora-utils-py/blob/master/.github/PULL_REQUEST_TEMPLATE.md) and several [Issue templates](https://github.com/Flora/flora-utils-py/tree/master/.github/ISSUE_TEMPLATE).
+- Files such as: `LICENSE`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `SECURITY.md` are generated automatically.
+- [`Stale bot`](https://github.com/apps/stale) that closes abandoned issues after a period of inactivity. (You will only [need to setup free plan](https://github.com/marketplace/stale)). Configuration is [here](https://github.com/Flora/flora-utils-py/blob/master/.github/.stale.yml).
+- [Semantic Versions](https://semver.org/) specification with [`Release Drafter`](https://github.com/marketplace/actions/release-drafter).
+
+## Installation
+
+```bash
+pip install -U flora-utils-py
+```
+
+or install with `Poetry`
+
+```bash
+poetry add flora-utils-py
+```
+
+
+
+### Makefile usage
+
+[`Makefile`](https://github.com/Flora/flora-utils-py/blob/master/Makefile) contains a lot of functions for faster development.
+
+<details>
+<summary>1. Download and remove Poetry</summary>
+<p>
+
+To download and install Poetry run:
+
+```bash
+make poetry-download
+```
+
+To uninstall
+
+```bash
+make poetry-remove
+```
+
+</p>
+</details>
+
+<details>
+<summary>2. Install all dependencies and pre-commit hooks</summary>
+<p>
+
+Install requirements:
+
+```bash
+make install
+```
+
+Pre-commit hooks coulb be installed after `git init` via
+
+```bash
+make pre-commit-install
+```
+
+</p>
+</details>
+
+<details>
+<summary>3. Codestyle</summary>
+<p>
+
+Automatic formatting uses `pyupgrade`, `isort` and `black`.
+
+```bash
+make codestyle
+
+# or use synonym
+make formatting
+```
+
+Codestyle checks only, without rewriting files:
+
+```bash
+make check-codestyle
+```
+
+> Note: `check-codestyle` uses `isort`, `black` and `darglint` library
+
+Update all dev libraries to the latest version using one comand
+
+```bash
+make update-dev-deps
+```
+
+<details>
+<summary>4. Code security</summary>
+<p>
+
+```bash
+make check-safety
+```
+
+This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
+
+```bash
+make check-safety
+```
+
+</p>
+</details>
+
+</p>
+</details>
+
+<details>
+<summary>5. Type checks</summary>
+<p>
+
+Run `mypy` static type checker
+
+```bash
+make mypy
+```
+
+</p>
+</details>
+
+<details>
+<summary>6. Tests with coverage badges</summary>
+<p>
+
+Run `pytest`
+
+```bash
+make test
+```
+
+</p>
+</details>
+
+<details>
+<summary>7. All linters</summary>
+<p>
+
+Of course there is a command to ~~rule~~ run all linters in one:
+
+```bash
+make lint
+```
+
+the same as:
+
+```bash
+make test && make check-codestyle && make mypy && make check-safety
+```
+
+</p>
+</details>
+
+<details>
+<summary>8. Docker</summary>
+<p>
+
+```bash
+make docker-build
+```
+
+which is equivalent to:
+
+```bash
+make docker-build VERSION=latest
+```
+
+Remove docker image with
+
+```bash
+make docker-remove
+```
+
+More information [about docker](https://github.com/Flora/flora-utils-py/tree/master/docker).
+
+</p>
+</details>
+
+<details>
+<summary>9. Cleanup</summary>
+<p>
+Delete pycache files
+
+```bash
+make pycache-remove
+```
+
+Remove package build
+
+```bash
+make build-remove
+```
+
+Delete .DS_STORE files
+
+```bash
+make dsstore-remove
+```
+
+Remove .mypycache
+
+```bash
+make mypycache-remove
+```
+
+Or to remove all above run:
+
+```bash
+make cleanup
+```
+
+</p>
+</details>
+
+## 📈 Releases
+
+You can see the list of available releases on the [GitHub Releases](https://github.com/Flora/flora-utils-py/releases) page.
+
+We follow [Semantic Versions](https://semver.org/) specification.
+
+We use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.
+
+### List of labels and corresponding titles
+
+|               **Label**               |  **Title in Releases**  |
+| :-----------------------------------: | :---------------------: |
+|       `enhancement`, `feature`        |       🚀 Features       |
+| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |
+|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |
+|              `breaking`               |   💥 Breaking Changes   |
+|            `documentation`            |    📝 Documentation     |
+|            `dependencies`             | ⬆️ Dependencies updates |
+
+You can update it in [`release-drafter.yml`](https://github.com/Flora/flora-utils-py/blob/master/.github/release-drafter.yml).
+
+GitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/Flora/flora-utils-py)](https://github.com/Flora/flora-utils-py/blob/master/LICENSE)
+
+This project is licensed under the terms of the `Apache Software License 2.0` license. See [LICENSE](https://github.com/Flora/flora-utils-py/blob/master/LICENSE) for more details.
+
+## 📃 Citation
+
+```bibtex
+@misc{flora-utils-py,
+  author = {Flora},
+  title = {Awesome `flora-utils-py` is a Python cli/package created with https://github.com/TezRomacH/python-package-template},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/Flora/flora-utils-py}}
 }
+```
+
+## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
+This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
 
-setup(**setup_kwargs)
```

