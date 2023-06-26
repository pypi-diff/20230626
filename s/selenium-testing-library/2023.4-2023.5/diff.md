# Comparing `tmp/selenium_testing_library-2023.4.tar.gz` & `tmp/selenium_testing_library-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_testing_library-2023.4.tar", max compression
+gzip compressed data, was "selenium_testing_library-2023.5.tar", max compression
```

## Comparing `selenium_testing_library-2023.4.tar` & `selenium_testing_library-2023.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.4/LICENSE.md
--rw-r--r--   0        0        0     9734 2023-01-08 14:45:10.963757 selenium_testing_library-2023.4/README.md
--rw-r--r--   0        0        0     1875 2023-05-18 15:30:38.881213 selenium_testing_library-2023.4/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-18 15:30:38.882116 selenium_testing_library-2023.4/selenium_testing_library/__init__.py
--rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.4/selenium_testing_library/locators.py
--rw-r--r--   0        0        0   220550 2023-05-18 15:28:50.991379 selenium_testing_library-2023.4/selenium_testing_library/main.js
--rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.4/selenium_testing_library/py.typed
--rw-r--r--   0        0        0    34005 2023-02-17 17:51:00.247649 selenium_testing_library-2023.4/selenium_testing_library/screen.py
--rw-r--r--   0        0        0    10710 1970-01-01 00:00:00.000000 selenium_testing_library-2023.4/setup.py
--rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 selenium_testing_library-2023.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-06-06 09:30:53.872504 selenium_testing_library-2023.5/LICENSE.md
+-rw-r--r--   0        0        0     9946 2023-06-26 15:30:47.718558 selenium_testing_library-2023.5/README.md
+-rw-r--r--   0        0        0     1886 2023-06-26 15:30:47.719242 selenium_testing_library-2023.5/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-26 15:16:59.346228 selenium_testing_library-2023.5/selenium_testing_library/__init__.py
+-rw-r--r--   0        0        0     7525 2023-02-17 17:32:49.420064 selenium_testing_library-2023.5/selenium_testing_library/locators.py
+-rw-r--r--   0        0        0   220550 2023-05-18 15:28:50.991379 selenium_testing_library-2023.5/selenium_testing_library/main.js
+-rw-r--r--   0        0        0        0 2021-06-05 14:50:48.385384 selenium_testing_library-2023.5/selenium_testing_library/py.typed
+-rw-r--r--   0        0        0    34005 2023-02-17 17:51:00.247649 selenium_testing_library-2023.5/selenium_testing_library/screen.py
+-rw-r--r--   0        0        0    10921 1970-01-01 00:00:00.000000 selenium_testing_library-2023.5/PKG-INFO
```

### Comparing `selenium_testing_library-2023.4/LICENSE.md` & `selenium_testing_library-2023.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.4/README.md` & `selenium_testing_library-2023.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)
 [![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)
 
 Selenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.
 
 ## Dependencies
 
-- Python 3.7, 3.8, 3.9, 3.10, 3.11
+- Python 3.7, 3.8, 3.9, 3.10, 3.11, 3.12-dev
 - [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0
 ## Installation
 
 ```
 pip install selenium-testing-library
 ```
 
@@ -191,12 +191,26 @@
 # python3.9. (Use pyenv and add the pyenv shims to your path
 # `export PATH=$(pyenv root)/shims:$PATH`). Then run tox:
 tox
 ```
 
 # Releasing a new version
 
+1. Update Changelog
+2. Update npm dependencies
 ```shell
 npm run deploy
+```
+If `npm run deploy` fails because of outdated dependencies run:
+
+```shell
+npm update
+```
+
+3. Bump the version
+```shell
 bumpver update  # Wait and see if the CI is green
+```
+4. Publish to PyPI
+```shell
 poetry build && poetry publish
 ```
```

### Comparing `selenium_testing_library-2023.4/pyproject.toml` & `selenium_testing_library-2023.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selenium-testing-library"
-version = "2023.4"
+version = "2023.5"
 description = "A Python Selenium library inspired by the Testing Library"
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/anze3db/selenium-testing-library"
 authors = ["Anže Pečar <anze@pecar.me>"]
 include = [
     "selenium_testing_library/main.js"
@@ -41,15 +41,15 @@
 addopts = "--selenium-headless --cov=selenium_testing_library --cov-report html --cov-report xml --verbose --durations=10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "2023.4"
+current_version = "2023.5"
 version_pattern = "YYYY.INC1"
 commit_message = "Bump version from {old_version} to {new_version} 🚀"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -85,8 +85,8 @@
     # Ruff
     "RUF",
     # flake8
     "PT",
     "ARG",
     "YTT",
 ]
-ignore = ["E501", "PLR2004"]
+ignore = ["E501", "PLR2004", "PLR0913"]
```

### Comparing `selenium_testing_library-2023.4/selenium_testing_library/locators.py` & `selenium_testing_library-2023.5/selenium_testing_library/locators.py`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.4/selenium_testing_library/main.js` & `selenium_testing_library-2023.5/selenium_testing_library/main.js`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.4/selenium_testing_library/screen.py` & `selenium_testing_library-2023.5/selenium_testing_library/screen.py`

 * *Files identical despite different names*

### Comparing `selenium_testing_library-2023.4/setup.py` & `selenium_testing_library-2023.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,240 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: selenium-testing-library
+Version: 2023.5
+Summary: A Python Selenium library inspired by the Testing Library
+Home-page: https://github.com/anze3db/selenium-testing-library
+License: MIT
+Author: Anže Pečar
+Author-email: anze@pecar.me
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ruff (>=0.0.247,<0.0.248)
+Requires-Dist: selenium (>3.0.0)
+Requires-Dist: typing_extensions (>=4.0.0)
+Project-URL: Changelog, https://github.com/anze3db/selenium-testing-library/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/anze3db/selenium-testing-library
+Description-Content-Type: text/markdown
+
+# Selenium Testing Library
+
+[![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)
+[![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)
+
+Selenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.
+
+## Dependencies
+
+- Python 3.7, 3.8, 3.9, 3.10, 3.11, 3.12-dev
+- [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0
+## Installation
+
+```
+pip install selenium-testing-library
+```
+
+## Quick Start
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen
+
+driver = webdriver.Chrome()
+driver.open('https://google.com/')
+
+screen = Screen(driver)
+search_input = screen.find_by_title("Search")
+search.send_keys("Dogs")
+search_button = screen.find_by_text("Google Search")
+search_button.click()
+screen.wait_for_stale(search_button)
+```
+
+## Finding elements
+
+STL implements the [Queries API](https://testing-library.com/docs/queries/about) from the Testing Library. The Testing Library queries `get_by`, `query_by`, `find_by`, and the multiple element equivalents `get_all_by`, `query_all_by`, `find_all_by` are used in places where you would normally use Selenium's `find_element` and `find_elements` functions.
+
+ The difference between the different queries (`get_by`, `query_by`, `find_by`) is whether the query will throw an error if the element was not found (`get_by`), return `None` (`query_by`) or block, wait and retry until the element is found (`find_by`).
+
+ * `get_by` returns the element matched and throws an exception if zero or more than one element matches. This is the main function that we should be using to locate elements on a page.
+ * `query_by` returns the element matched or `None` if no element match. It throws an exception if more than one element matches. Mostly used for asserting that an element is **not** present: `assert not screen.query_by_text("not on page")`.
+ * `find_by` behaves like `get_by`, but uses a `WebDriverWait` to wait until the element is present in the DOM.
+ * `get_all_by` returns a list of elements matched. It raises an exception if no elements match.
+ * `query_all_by` returns a list of elements matched. It returns an empty list when no elements match.
+ * `find_all_by` behaves like `get_all_by`, but uses a `WebDriverWait` to wait until the elements are present in the DOM.
+
+ When an element is found the queries return a Selenium [`WebElement`](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement) or a list containing Selenium [WebElement](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement)s when using `get_all_by`, `query_all_by`, `find_all_by`.
+
+The queries accept a tuple containing the [By class identifier](https://selenium-python.readthedocs.io/api.html#locate-elements-by) and the search query, so they can be used with XPath, Css or any other native Selenium selector:
+
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from selenium_testing_library import Screen
+
+screen = Screen(webdriver.Chrome())
+screen.get_by((By.CSS, ".my_class")) # Will throw an exception if the element is not found
+screen.query_by((By.ID, "my_id")) # you can use regular tuples as if you were using Selenium's find_element()
+screen.find_by((By.XPATH, "//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work
+```
+
+## Locator Classes
+
+For convenience Locator classes can be used instead of the tuples:
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen, locators
+
+screen = Screen(webdriver.Chrome())
+screen.get_by(locators.Css(".my_class")) # Will throw an exception if the element is not found
+screen.query_by(locators.Id("my_id")) # you can use regular tuples as if you were using Selenium's find_element()
+screen.find_by(locators.XPath("//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work
+```
+
+## Testing Library Selectors
+
+Besides all the Selenium native By selectors, the queries also support Testing Library's selectors:
+ * [Role](https://testing-library.com/docs/queries/byrole)
+ * [LabelText](https://testing-library.com/docs/queries/bylabeltext)
+ * [PlaceholderText](https://testing-library.com/docs/queries/byplaceholdertext)
+ * [Text](https://testing-library.com/docs/queries/bytext)
+ * [DisplayValue](https://testing-library.com/docs/queries/bydisplayvalue)
+ * [AltText](https://testing-library.com/docs/queries/byalttext)
+ * [Title](https://testing-library.com/docs/queries/bytitle)
+ * [TestId](https://testing-library.com/docs/queries/bytestid)
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen, locators
+
+screen = Screen(webdriver.Chrome())
+screen.get_by(locators.Text("My Text"))
+screen.query_by(locators.Role("button", pressed=True))
+screen.find_by(locators.TestId("my-test"), timeout=5, poll_frequency=0.5) # locators for searching through text also work
+```
+## Helper functions
+
+For convenience helper functions on the screen class are available to avoid instantiating locator classes all over the place:
+
+[`screen.get_by_role(role_name)`](https://testing-library.com/docs/queries/byrole) Queries for elements with the given role.
+[`screen.get_by_label_text(text)`](https://testing-library.com/docs/queries/bylabeltext) Queries for label elements that match the text string and return the corresponding input element.
+[`screen.get_by_placeholder_text(text)`](https://testing-library.com/docs/queries/byplaceholdertext) Queries elements with the matching placeholder attribute.
+[`screen.get_by_text(text)`](https://testing-library.com/docs/queries/bytext) Queries elements where the content matches the provided text.
+[`screen.get_by_display_value(value)`](https://testing-library.com/docs/queries/bydisplayvalue) Queries inputs, textareas, or selects with matching display value.
+[`screen.get_by_alt_text(text)`](https://testing-library.com/docs/queries/byalttext) Queries elements with the matching alt attribute.
+`screen.get_by_title(text)` Queries elements with the matching title attribute.
+`screen.get_by_test_id(value)` Queries elements matching the `data-testid` value.
+`screen.get_by_css(css)` Queries elements matching the specified css selector.
+`screen.get_by_xpath(xpath)` Queries elements matching the specified xpath selector.
+
+There are also `query_by_*`, `find_by_*`, `get_all_by_*`, `query_all_by_*`, `find_all_by_*`  equivalents.
+
+**Note:** The selenium project has removed the `find_element_by_*` and `find_elements_by_*` helper functions in the [Selenium 4.3.0](https://github.com/SeleniumHQ/selenium/releases/tag/selenium-4.3.0) release, so I just want to state that the `screen` helper functions will never be deprecated or removed.
+
+Examples:
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen
+
+screen = Screen(webdriver.Chrome())
+screen.query_by_role("role_name")
+screen.get_by_label_text("label text")
+screen.find_all_by_text("my text", timeout=5, poll_frequency=0.5)
+screen.get_all_by_alt_text("alt text")
+```
+
+## Wait functions
+
+`wait_for(condition_function)` Waits until the condition function returns a truthy value.
+`wait_for_stale(element)` Waits until the element is removed from the DOM.
+
+Examples:
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen, locators
+
+screen = Screen(webdriver.Chrome())
+
+# Wait for the element to be clickable:
+element = screen.get_by_text("Submit")
+screen.wait_for(lambda _: element.is_enabled(), timeout=5, poll_frequency=0.5)
+# Wait for the element to be removed from the page:
+screen.wait_for_stale(element)
+```
+
+## Querying within elements
+
+`Within(element)` Used to limit the query to the children of the provided element
+
+Example:
+
+```python
+from selenium import webdriver
+from selenium_testing_library import Screen, Within
+
+screen = Screen(webdriver.Chrome())
+parent_element = screen.get_by_css(".container")
+Within(parent_element).get_by_title("My title inside the container")
+```
+
+# Testing Playground URLs
+
+For debugging using [testing-playground](https://testing-playground.com/), `screen` exposes `log_testing_playground_url()` which prints end returns a URL that can be opened in the browser.
+
+```python
+# log entire document to testing-playground
+url = screen.log_testing_playground_url()
+# log a single element
+url = screen.log_testing_playground_url(screen.get_by_text("test"))
+```
+
+# Contributing
+
+Setting up a local development environment
+
+```shell
+git clone https://github.com/anze3db/selenium-testing-library.git && cd selenium-testing-library
+poetry install && poetry shell
+# Make sure `chromedriver` is in your PATH, download from https://chromedriver.chromium.org/downloads
+# run tests:
+pytest --selenium-headless
+# run tests and display coverage info:
+pytest --selenium-headless --cov=selenium_testing_library --cov-report html
+
+# To test on multiple Python versions make sure that py37, py38, py39 are
+# installed on your system and available through python3.7, python3.8,
+# python3.9. (Use pyenv and add the pyenv shims to your path
+# `export PATH=$(pyenv root)/shims:$PATH`). Then run tox:
+tox
+```
+
+# Releasing a new version
+
+1. Update Changelog
+2. Update npm dependencies
+```shell
+npm run deploy
+```
+If `npm run deploy` fails because of outdated dependencies run:
+
+```shell
+npm update
+```
+
+3. Bump the version
+```shell
+bumpver update  # Wait and see if the CI is green
+```
+4. Publish to PyPI
+```shell
+poetry build && poetry publish
+```
 
-packages = \
-['selenium_testing_library']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ruff>=0.0.247,<0.0.248', 'selenium>3.0.0', 'typing_extensions>=4.0.0']
-
-setup_kwargs = {
-    'name': 'selenium-testing-library',
-    'version': '2023.4',
-    'description': 'A Python Selenium library inspired by the Testing Library',
-    'long_description': '# Selenium Testing Library\n\n[![PyPI version](https://badge.fury.io/py/selenium-testing-library.svg)](https://badge.fury.io/py/selenium-testing-library)\n[![test](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml/badge.svg)](https://github.com/anze3db/selenium-testing-library/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/anze3db/selenium-testing-library/branch/main/graph/badge.svg?token=L1M7HO3DL7)](https://codecov.io/gh/anze3db/selenium-testing-library)\n\nSelenium Testing Library (STL) is a Python library implementing [Testing-Library](https://testing-library.com/) in Selenium.\n\n## Dependencies\n\n- Python 3.7, 3.8, 3.9, 3.10, 3.11\n- [`selenium`](https://pypi.org/project/selenium/) >= 3.0.0, [`typing-extensions`](https://pypi.org/project/typing-extensions/) >= 4.0.0\n## Installation\n\n```\npip install selenium-testing-library\n```\n\n## Quick Start\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen\n\ndriver = webdriver.Chrome()\ndriver.open(\'https://google.com/\')\n\nscreen = Screen(driver)\nsearch_input = screen.find_by_title("Search")\nsearch.send_keys("Dogs")\nsearch_button = screen.find_by_text("Google Search")\nsearch_button.click()\nscreen.wait_for_stale(search_button)\n```\n\n## Finding elements\n\nSTL implements the [Queries API](https://testing-library.com/docs/queries/about) from the Testing Library. The Testing Library queries `get_by`, `query_by`, `find_by`, and the multiple element equivalents `get_all_by`, `query_all_by`, `find_all_by` are used in places where you would normally use Selenium\'s `find_element` and `find_elements` functions.\n\n The difference between the different queries (`get_by`, `query_by`, `find_by`) is whether the query will throw an error if the element was not found (`get_by`), return `None` (`query_by`) or block, wait and retry until the element is found (`find_by`).\n\n * `get_by` returns the element matched and throws an exception if zero or more than one element matches. This is the main function that we should be using to locate elements on a page.\n * `query_by` returns the element matched or `None` if no element match. It throws an exception if more than one element matches. Mostly used for asserting that an element is **not** present: `assert not screen.query_by_text("not on page")`.\n * `find_by` behaves like `get_by`, but uses a `WebDriverWait` to wait until the element is present in the DOM.\n * `get_all_by` returns a list of elements matched. It raises an exception if no elements match.\n * `query_all_by` returns a list of elements matched. It returns an empty list when no elements match.\n * `find_all_by` behaves like `get_all_by`, but uses a `WebDriverWait` to wait until the elements are present in the DOM.\n\n When an element is found the queries return a Selenium [`WebElement`](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement) or a list containing Selenium [WebElement](https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.remote.webelement)s when using `get_all_by`, `query_all_by`, `find_all_by`.\n\nThe queries accept a tuple containing the [By class identifier](https://selenium-python.readthedocs.io/api.html#locate-elements-by) and the search query, so they can be used with XPath, Css or any other native Selenium selector:\n\n```python\nfrom selenium import webdriver\nfrom selenium.webdriver.common.by import By\nfrom selenium_testing_library import Screen\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by((By.CSS, ".my_class")) # Will throw an exception if the element is not found\nscreen.query_by((By.ID, "my_id")) # you can use regular tuples as if you were using Selenium\'s find_element()\nscreen.find_by((By.XPATH, "//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n\n## Locator Classes\n\nFor convenience Locator classes can be used instead of the tuples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by(locators.Css(".my_class")) # Will throw an exception if the element is not found\nscreen.query_by(locators.Id("my_id")) # you can use regular tuples as if you were using Selenium\'s find_element()\nscreen.find_by(locators.XPath("//div"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n\n## Testing Library Selectors\n\nBesides all the Selenium native By selectors, the queries also support Testing Library\'s selectors:\n * [Role](https://testing-library.com/docs/queries/byrole)\n * [LabelText](https://testing-library.com/docs/queries/bylabeltext)\n * [PlaceholderText](https://testing-library.com/docs/queries/byplaceholdertext)\n * [Text](https://testing-library.com/docs/queries/bytext)\n * [DisplayValue](https://testing-library.com/docs/queries/bydisplayvalue)\n * [AltText](https://testing-library.com/docs/queries/byalttext)\n * [Title](https://testing-library.com/docs/queries/bytitle)\n * [TestId](https://testing-library.com/docs/queries/bytestid)\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\nscreen.get_by(locators.Text("My Text"))\nscreen.query_by(locators.Role("button", pressed=True))\nscreen.find_by(locators.TestId("my-test"), timeout=5, poll_frequency=0.5) # locators for searching through text also work\n```\n## Helper functions\n\nFor convenience helper functions on the screen class are available to avoid instantiating locator classes all over the place:\n\n[`screen.get_by_role(role_name)`](https://testing-library.com/docs/queries/byrole) Queries for elements with the given role.\n[`screen.get_by_label_text(text)`](https://testing-library.com/docs/queries/bylabeltext) Queries for label elements that match the text string and return the corresponding input element.\n[`screen.get_by_placeholder_text(text)`](https://testing-library.com/docs/queries/byplaceholdertext) Queries elements with the matching placeholder attribute.\n[`screen.get_by_text(text)`](https://testing-library.com/docs/queries/bytext) Queries elements where the content matches the provided text.\n[`screen.get_by_display_value(value)`](https://testing-library.com/docs/queries/bydisplayvalue) Queries inputs, textareas, or selects with matching display value.\n[`screen.get_by_alt_text(text)`](https://testing-library.com/docs/queries/byalttext) Queries elements with the matching alt attribute.\n`screen.get_by_title(text)` Queries elements with the matching title attribute.\n`screen.get_by_test_id(value)` Queries elements matching the `data-testid` value.\n`screen.get_by_css(css)` Queries elements matching the specified css selector.\n`screen.get_by_xpath(xpath)` Queries elements matching the specified xpath selector.\n\nThere are also `query_by_*`, `find_by_*`, `get_all_by_*`, `query_all_by_*`, `find_all_by_*`  equivalents.\n\n**Note:** The selenium project has removed the `find_element_by_*` and `find_elements_by_*` helper functions in the [Selenium 4.3.0](https://github.com/SeleniumHQ/selenium/releases/tag/selenium-4.3.0) release, so I just want to state that the `screen` helper functions will never be deprecated or removed.\n\nExamples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen\n\nscreen = Screen(webdriver.Chrome())\nscreen.query_by_role("role_name")\nscreen.get_by_label_text("label text")\nscreen.find_all_by_text("my text", timeout=5, poll_frequency=0.5)\nscreen.get_all_by_alt_text("alt text")\n```\n\n## Wait functions\n\n`wait_for(condition_function)` Waits until the condition function returns a truthy value.\n`wait_for_stale(element)` Waits until the element is removed from the DOM.\n\nExamples:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, locators\n\nscreen = Screen(webdriver.Chrome())\n\n# Wait for the element to be clickable:\nelement = screen.get_by_text("Submit")\nscreen.wait_for(lambda _: element.is_enabled(), timeout=5, poll_frequency=0.5)\n# Wait for the element to be removed from the page:\nscreen.wait_for_stale(element)\n```\n\n## Querying within elements\n\n`Within(element)` Used to limit the query to the children of the provided element\n\nExample:\n\n```python\nfrom selenium import webdriver\nfrom selenium_testing_library import Screen, Within\n\nscreen = Screen(webdriver.Chrome())\nparent_element = screen.get_by_css(".container")\nWithin(parent_element).get_by_title("My title inside the container")\n```\n\n# Testing Playground URLs\n\nFor debugging using [testing-playground](https://testing-playground.com/), `screen` exposes `log_testing_playground_url()` which prints end returns a URL that can be opened in the browser.\n\n```python\n# log entire document to testing-playground\nurl = screen.log_testing_playground_url()\n# log a single element\nurl = screen.log_testing_playground_url(screen.get_by_text("test"))\n```\n\n# Contributing\n\nSetting up a local development environment\n\n```shell\ngit clone https://github.com/anze3db/selenium-testing-library.git && cd selenium-testing-library\npoetry install && poetry shell\n# Make sure `chromedriver` is in your PATH, download from https://chromedriver.chromium.org/downloads\n# run tests:\npytest --selenium-headless\n# run tests and display coverage info:\npytest --selenium-headless --cov=selenium_testing_library --cov-report html\n\n# To test on multiple Python versions make sure that py37, py38, py39 are\n# installed on your system and available through python3.7, python3.8,\n# python3.9. (Use pyenv and add the pyenv shims to your path\n# `export PATH=$(pyenv root)/shims:$PATH`). Then run tox:\ntox\n```\n\n# Releasing a new version\n\n```shell\nnpm run deploy\nbumpver update  # Wait and see if the CI is green\npoetry build && poetry publish\n```\n',
-    'author': 'Anže Pečar',
-    'author_email': 'anze@pecar.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/anze3db/selenium-testing-library',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

