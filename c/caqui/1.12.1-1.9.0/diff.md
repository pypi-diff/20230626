# Comparing `tmp/caqui-1.12.1.tar.gz` & `tmp/caqui-1.9.0.tar.gz`

## Comparing `caqui-1.12.1.tar` & `caqui-1.9.0.tar`

### file list

```diff
@@ -1,39 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.12.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.12.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-1.12.1/sample-appium.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-1.12.1/sample-win-app-driver.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-1.12.1/sample-winium.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 caqui-1.12.1/sample.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-1.12.1/test-requirements.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-1.12.1/tox.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.12.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.12.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.12.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.12.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.12.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.12.1/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/__init__.py
--rw-r--r--   0        0        0    14050 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/helper.py
--rw-r--r--   0        0        0    13534 2020-02-02 00:00:00.000000 caqui-1.12.1/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/constants.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/fake_responses.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/test_sniffer.py
--rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/apk/app-debug.apk
--rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/html/playground.html
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/unit/__initi__.py
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/unit/test_helper.py
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 caqui-1.12.1/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.12.1/utils/coverage.sh
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-1.12.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.12.1/LICENSE
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 caqui-1.12.1/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 caqui-1.12.1/pyproject.toml
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 caqui-1.12.1/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 caqui-1.9.0/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.9.0/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/__init__.py
+-rw-r--r--   0        0        0    10603 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/helper.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/constants.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/fake_responses.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/test_sniffer.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/html/playground.html
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.9.0/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.9.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.9.0/PKG-INFO
```

### Comparing `caqui-1.12.1/CODE_OF_CONDUCT.md` & `caqui-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/sample.py` & `caqui-1.9.0/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# It opens the WebDriver, navigate to a page and get all links
 import asyncio
 import time
 from caqui import synchronous, asynchronous
 from os import getcwd
 from tests.constants import PAGE_URL
 
 BASE_DIR = getcwd()
```

### Comparing `caqui-1.12.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/.github/workflows/python-app.yml` & `caqui-1.9.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/.github/workflows/python-publish.yml` & `caqui-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/caqui/__init__.py` & `caqui-1.9.0/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/caqui/asynchronous.py` & `caqui-1.9.0/caqui/asynchronous.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp
 import json
 from caqui.constants import HEADERS
 from caqui.exceptions import WebDriverError
-from caqui import helper
+from caqui.helper import get_element
 
 
 async def __delete(url):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.delete(url, headers=HEADERS) as resp:
                 response = await resp.json()
@@ -14,126 +14,36 @@
     except Exception as error:
         raise WebDriverError("'DELETE' request failed.") from error
 
 
 async def __post(url, payload):
     try:
         async with aiohttp.ClientSession() as session:
-            async with session.post(
-                url, data=json.dumps(payload), headers=HEADERS
-            ) as resp:
-                status = resp.status
-                if status in range(200, 399):
-                    return await resp.json()
-                raise WebDriverError(f"Status code: {resp.status}, {resp.text}")
+            async with session.post(url, data=payload, headers=HEADERS) as resp:
+                response = await resp.json()
+                return response
     except Exception as error:
         raise WebDriverError("'POST' request failed.") from error
 
 
 async def __get(url):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.get(url, headers=HEADERS) as resp:
-                status = resp.status
-                if status in range(200, 399):
-                    return await resp.json()
-                raise WebDriverError(f"Status code: {resp.status}, {resp.text}")
+                response = await resp.json()
+                return response
     except Exception as error:
         raise WebDriverError("'GET' request failed.") from error
 
 
-async def set_timeouts(driver_url, session, timeouts):
-    """Set timeouts"""
-    try:
-        url = f"{driver_url}/session/{session}/timeouts"
-        payload = {
-            "implicit": timeouts,
-        }
-        await __post(url, payload)
-        return True
-    except Exception as error:
-        raise WebDriverError(f"Failed to set timeouts.") from error
-
-
-async def find_children_elements(
-    driver_url, session, parent_element, locator_type, locator_value
-):
-    """Find the children elements by 'locator_type'"""
-    try:
-        url = f"{driver_url}/session/{session}/element/{parent_element}/elements"
-        payload = {"using": locator_type, "value": locator_value, "id": parent_element}
-        response = await __post(url, payload)
-        return helper.get_elements(response)
-    except Exception as error:
-        raise WebDriverError(
-            f"Failed to find the children elements from '{parent_element}'."
-        ) from error
-
-
-async def find_child_element(
-    driver_url, session, parent_element, locator_type, locator_value
-):
-    """Find the child element by 'locator_type'"""
-    try:
-        url = f"{driver_url}/session/{session}/element/{parent_element}/element"
-        payload = {"using": locator_type, "value": locator_value, "id": parent_element}
-        response = await __post(url, payload)
-        return helper.get_element(response)
-    except Exception as error:
-        raise WebDriverError(
-            f"Failed to find the child element from '{parent_element}'."
-        ) from error
-
-
-async def get_page_source(driver_url, session):
-    """Get the page source (all content)"""
-    try:
-        url = f"{driver_url}/session/{session}/source"
-        response = await __get(url)
-        return response.get("value")
-    except Exception as error:
-        raise WebDriverError("Failed to get the page source.") from error
-
-
-async def execute_script(driver_url, session, script, args=[]):
-    """Executes a script, like 'alert('something')' to open an alert window"""
-    try:
-        url = f"{driver_url}/session/{session}/execute/sync"
-        payload = {"script": script, "args": args}
-        response = await __post(url, payload)
-        return response.get("value")
-    except Exception as error:
-        raise WebDriverError("Failed to open session.") from error
-
-
-async def get_alert_text(driver_url, session):
-    """Get the text from an alert"""
-    try:
-        url = f"{driver_url}/session/{session}/alert/text"
-        response = await __get(url)
-        return response.get("value")
-    except Exception as error:
-        raise WebDriverError("Failed to get the alert text.") from error
-
-
-async def get_active_element(driver_url, session):
-    """Get the active element"""
-    try:
-        url = f"{driver_url}/session/{session}/element/active"
-        response = await __get(url)
-        return helper.get_element(response)
-    except Exception as error:
-        raise WebDriverError("Failed to check if element is selected.") from error
-
-
 async def clear_element(driver_url, session, element):
     """Clear the element text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/clear"
-        payload = {"id": element}
+        payload = json.dumps({"id": element})
         await __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError("Failed to clear the element text.") from error
 
 
 async def is_element_enabled(driver_url, session, element):
@@ -270,15 +180,15 @@
     except Exception as error:
         raise WebDriverError("Failed to get page title.") from error
 
 
 async def find_elements(driver_url, session, locator_type, locator_value):
     """Search the DOM elements by 'locator', for example, 'xpath'"""
     try:
-        payload = {"using": locator_type, "value": locator_value}
+        payload = json.dumps({"using": locator_type, "value": locator_value})
         url = f"{driver_url}/session/{session}/elements"
         response = await __post(url, payload)
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
         raise WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
@@ -334,63 +244,59 @@
         raise WebDriverError("Failed to close session.") from error
 
 
 async def go_to_page(driver_url, session, page_url):
     """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
-        payload = {"url": page_url}
+        payload = json.dumps({"url": page_url})
         await __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError(f"Failed to navigate to page '{page_url}'.") from error
 
 
 async def send_keys(driver_url, session, element, text):
     """Fill an editable element, for example a textarea, with a given text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/value"
-        payload = {"text": text, "value": [*text], "id": element}
+        payload = json.dumps({"text": text, "value": [*text], "id": element})
         await __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError(f"Failed to send key '{text}'.") from error
 
 
 async def click(driver_url, session, element):
     """Click on an element"""
     try:
-        payload = {"id": element}
+        payload = json.dumps({"id": element})
         url = f"{driver_url}/session/{session}/element/{element}/click"
         await __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError("Failed to click on element.") from error
 
 
 async def find_element(driver_url, session, locator_type, locator_value):
     """Find an element by a 'locator', for example 'xpath'"""
 
     try:
-        payload = {"using": locator_type, "value": locator_value}
+        payload = json.dumps({"using": locator_type, "value": locator_value})
         url = f"{driver_url}/session/{session}/element"
         response = await __post(url, payload)
-        if response.get("value").get("error"):
-            raise WebDriverError(f"Failed to find element. {response}")
-        if response.get("status") > 0:
-            raise WebDriverError(f"Failed to find element. {response}")
-        return helper.get_element(response)
+        return get_element(response)
     except Exception as error:
         raise WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
 async def get_session(driver_url, capabilities):
     """Opens a browser and a session. This session is used for all functions to perform events in the page"""
     try:
-        payload = capabilities
+        payload = json.dumps(capabilities)
         url = f"{driver_url}/session"
         response = await __post(url, payload)
         return response.get("sessionId")
     except Exception as error:
         raise WebDriverError("Failed to open session.") from error
```

### Comparing `caqui-1.12.1/tests/fake_responses.py` & `caqui-1.9.0/tests/fake_responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,15 @@
         return self.dictionary
 
     def get(self, key):
         return self.dictionary.get(key)
 
 
 def dict_to_json(dictionary):
-    class MockResponse:
-        @property
-        def status_code(self):
-            return 200
-
-        def get(self, argument):
-            return dictionary.get(argument)
-
-        def json(self):
-            return Dictionary(dictionary)
-
-    return MockResponse()
+    return Dictionary(dictionary)
 
 
 DEFAULT = dict_to_json(
     {
         "sessionId": "4358a5b53794586af59678fc1653dc40",
         "status": 0,
         "value": {"ELEMENT": "0.8851292311864847-1"},
@@ -37,39 +26,22 @@
 
 FIND_ELEMENT = DEFAULT
 SEND_KEYS = DEFAULT
 CLICK = DEFAULT
 CLOSE_SESSION = DEFAULT
 GO_TO_PAGE = DEFAULT
 
-EXECUTE_SCRIPT = dict_to_json(
-    {"sessionId": "9f4a4a9420663d0c0cc18957ab463b90", "status": 0, "value": "any"}
-)
-
-GET_PAGE_SOURCE = dict_to_json(
-    {
-        "sessionId": "e34234d1445ed6d4833370d1d8019282",
-        "status": 0,
-        "value": "<html><head><title>Sample page</title></head><body><h1>Basic page</h1></body></html>",
-    }
-)
-
-GET_ALERT_TEXT = dict_to_json(
-    {"sessionId": "171ba19c927e0b95e1a53dbbdcfcdc19", "status": 0, "value": "any warn"}
-)
-
 GET_WINDOW_RECTANGLE = dict_to_json(
     {
         "sessionId": "79e4bd950a886e0119e3760d201b059e",
         "status": 0,
         "value": {"height": 600, "width": 800, "x": 0, "y": 0},
     }
 )
 
-GET_ACTIVE_ELEMENT = DEFAULT
 
 CLEAR_ELEMENT = dict_to_json(
     {"sessionId": "486fa32a9876b4519e149b39135edcb5", "status": 0, "value": None}
 )
 
 IS_ELEMENT_ENABLED = dict_to_json(
     {"sessionId": "e0e43cd1ce532b5aa62b6df0de11e3bd", "status": 0, "value": True}
```

### Comparing `caqui-1.12.1/tests/test_sniffer.py` & `caqui-1.9.0/tests/test_sniffer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #### File used to figure out requests format and parameters ####
 
 from selenium import webdriver
 from pytest import fixture, mark
 from tests.constants import PAGE_URL
-from selenium.webdriver.common.by import By
 
 
 @fixture
 def setup():
     desired_capabilities = {
         # 'deviceName': 'Device',
         "deviceName": "Emulator",
@@ -24,29 +23,14 @@
     driver.get(PAGE_URL)
     driver
     yield driver
     driver.quit()
 
 
 @mark.skip("used just to discover request data")
-def test_sniffer_find_children_elements(setup):
-    driver = setup
-    element = driver.find_element(By.XPATH, '//div[@class="parent"]')
-    elements = element.find_elements(By.XPATH, "//div")
-    for e in elements:
-        print("element_text:", e.text)
-
-
-@mark.skip("used just to discover request data")
-def test_exec_script(setup):
-    driver = setup
-    assert driver.execute_script("return document.body.scrollHeight") == "any"
-
-
-@mark.skip("used just to discover request data")
 def test_clear(setup):
     driver = setup
     element = driver.find_element("xpath", "//input")
     assert element.clear() == "any"
 
 
 @mark.skip("used just to discover request data")
```

### Comparing `caqui-1.12.1/tests/feature/test_sync_and_async.py` & `caqui-1.9.0/tests/feature/test_sync_and_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from pytest import fixture, mark, raises
+from pytest import fixture, mark
 from caqui import asynchronous, synchronous
 from tests.constants import PAGE_URL
-from caqui.exceptions import WebDriverError
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
@@ -23,146 +22,14 @@
         PAGE_URL,
     )
     yield driver_url, session
     synchronous.close_session(driver_url, session)
 
 
 @mark.asyncio
-async def test_raise_exception_when_element_not_found(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//invalid-tag"
-
-    with raises(WebDriverError):
-        synchronous.find_element(driver_url, session, locator_type, locator_value)
-
-    with raises(WebDriverError):
-        await asynchronous.find_element(
-            driver_url, session, locator_type, locator_value
-        )
-
-
-@mark.asyncio
-async def test_set_timeouts(__setup):
-    driver_url, session = __setup
-    timeouts_1 = 5000  # milliseconds
-    timeouts_2 = 3000  # milliseconds
-
-    synchronous.set_timeouts(driver_url, session, timeouts_1)
-
-    assert synchronous.get_timeouts(driver_url, session).get("implicit") == timeouts_1
-
-    await asynchronous.set_timeouts(driver_url, session, timeouts_2)
-
-    assert synchronous.get_timeouts(driver_url, session).get("implicit") == timeouts_2
-
-
-@mark.asyncio
-async def test_find_children_elements(__setup):
-    driver_url, session = __setup
-    expected = 5  # parent inclusive
-    locator_type = "xpath"
-    locator_value = "//div"
-
-    parent_element = synchronous.find_element(
-        driver_url, session, locator_type, '//div[@class="parent"]'
-    )
-
-    children_elements = synchronous.find_children_elements(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    assert len(children_elements) == expected
-
-    children_elements = await asynchronous.find_children_elements(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    assert len(children_elements) == expected
-
-
-@mark.asyncio
-async def test_find_child_element(__setup):
-    driver_url, session = __setup
-    expected = "any4"
-    locator_type = "xpath"
-    locator_value = '//div[@class="child4"]'
-
-    parent_element = synchronous.find_element(
-        driver_url, session, locator_type, '//div[@class="parent"]'
-    )
-
-    child_element = synchronous.find_child_element(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    text = synchronous.get_text(driver_url, session, child_element)
-
-    assert text == expected
-    child_element = await asynchronous.find_child_element(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-    text = synchronous.get_text(driver_url, session, child_element)
-    assert text == expected
-
-
-@mark.asyncio
-async def test_get_page_source(__setup):
-    driver_url, session = __setup
-    expected = "Sample page"
-
-    assert expected in synchronous.get_page_source(driver_url, session)
-    assert expected in await asynchronous.get_page_source(driver_url, session)
-
-
-@mark.asyncio
-async def test_execute_script_asynchronous(__setup):
-    driver_url, session = __setup
-    script = "alert('any warn')"
-
-    assert await asynchronous.execute_script(driver_url, session, script) == None
-
-
-def test_execute_script_synchronous(__setup):
-    driver_url, session = __setup
-    script = "alert('any warn')"
-
-    assert synchronous.execute_script(driver_url, session, script) == None
-
-
-@mark.asyncio
-async def test_get_alert_text(__setup):
-    driver_url, session = __setup
-    locator_type = "css selector"
-    locator_value = "#alert-button"
-    expected = "any warn"
-
-    alert_button = synchronous.find_element(
-        driver_url, session, locator_type, locator_value
-    )
-    synchronous.click(driver_url, session, alert_button)
-
-    assert synchronous.get_alert_text(driver_url, session) == expected
-    assert await asynchronous.get_alert_text(driver_url, session) == expected
-
-
-@mark.asyncio
-async def test_get_active_element(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//input"
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    synchronous.send_keys(driver_url, session, element, "any")
-
-    assert synchronous.get_active_element(driver_url, session) == element
-    assert await asynchronous.get_active_element(driver_url, session) == element
-
-
-@mark.asyncio
 async def test_clear_element(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//input"
     text = "any"
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
```

### Comparing `caqui-1.12.1/tests/integration/test_async_scenarios.py` & `caqui-1.9.0/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/tests/integration/test_sync_scenarios.py` & `caqui-1.9.0/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/tests/unit/test_async_unit.py` & `caqui-1.9.0/tests/unit/test_async_unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,89 +8,14 @@
 
 
 async def mock_request(*args):
     pass
 
 
 @mark.asyncio
-async def test_set_timeouts():
-    async def mock_request(*args):
-        return fake_responses.GET_TIMEOUTS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.set_timeouts("", "", "") == True
-
-
-@mark.asyncio
-async def test_find_children_elements():
-    element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
-
-    async def mock_request(*args):
-        return fake_responses.FIND_ELEMENTS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert element in await asynchronous.find_children_elements("", "", "", "", "")
-
-
-@mark.asyncio
-async def test_find_child_element():
-    element = "0.8851292311864847-1"
-
-    async def mock_request(*args):
-        return fake_responses.FIND_ELEMENT
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.find_child_element("", "", "", "", "") == element
-
-
-@mark.asyncio
-async def test_execute_script():
-    expected = "any"
-
-    async def mock_request(*args):
-        return fake_responses.EXECUTE_SCRIPT
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.execute_script("", "", "", "") == expected
-
-
-@mark.asyncio
-async def test_get_page_source():
-    expected = "Sample page"
-
-    async def mock_request(*args):
-        return fake_responses.GET_PAGE_SOURCE
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert expected in await asynchronous.get_page_source("", "")
-
-
-@mark.asyncio
-async def test_get_alert_text():
-    expected = "any warn"
-
-    async def mock_request(*args):
-        return fake_responses.GET_ALERT_TEXT
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert await asynchronous.get_alert_text("", "") == expected
-
-
-@mark.asyncio
-async def test_get_active_element():
-    expected = "0.8851292311864847-1"
-
-    async def mock_request(*args):
-        return fake_responses.GET_ACTIVE_ELEMENT
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert await asynchronous.get_active_element("", "") == expected
-
-
-@mark.asyncio
 async def test_clear_element():
     async def mock_request(*args):
         return fake_responses.CLEAR_ELEMENT
 
     with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.clear_element("", "", "") is True
```

### Comparing `caqui-1.12.1/tests/unit/test_helper.py` & `caqui-1.9.0/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/tests/unit/test_sync_unit.py` & `caqui-1.9.0/tests/unit/test_sync_unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,12 @@
 from unittest.mock import patch
 from caqui import synchronous
 from tests import fake_responses
 
 
-@patch("requests.request", return_value=fake_responses.GET_TIMEOUTS)
-def test_set_timeouts(*args):
-    assert synchronous.set_timeouts("", "", "") == True
-
-
-@patch("requests.request", return_value=fake_responses.FIND_ELEMENTS)
-def test_find_children_elements(*args):
-    element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
-
-    elements = synchronous.find_children_elements("", "", "", "", "")
-
-    assert element in elements
-    assert len(elements) == 3
-
-
-@patch("requests.request", return_value=fake_responses.FIND_ELEMENT)
-def test_find_child_element(*args):
-    expected = "0.8851292311864847-1"
-
-    assert synchronous.find_child_element("", "", "", "", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.EXECUTE_SCRIPT)
-def test_execute_script(*args):
-    expected = "any"
-
-    assert synchronous.execute_script("", "", "", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.GET_PAGE_SOURCE)
-def test_get_page_source(*args):
-    expected = "Sample page"
-    assert expected in synchronous.get_page_source("", "")
-
-
-@patch("requests.request", return_value=fake_responses.GET_ALERT_TEXT)
-def test_get_alert_text(*args):
-    expected = "any warn"
-    assert synchronous.get_alert_text("", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.GET_ACTIVE_ELEMENT)
-def test_get_active_element(*args):
-    expected = "0.8851292311864847-1"
-    assert synchronous.get_active_element("", "") == expected
-
-
 @patch("requests.request", return_value=fake_responses.CLEAR_ELEMENT)
 def test_clear_element(*args):
     assert synchronous.clear_element("", "", "") is True
 
 
 @patch("requests.request", return_value=fake_responses.IS_ELEMENT_ENABLED)
 def test_is_element_enabled(*args):
```

### Comparing `caqui-1.12.1/.gitignore` & `caqui-1.9.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,14 @@
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
-venv*
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
```

### Comparing `caqui-1.12.1/LICENSE` & `caqui-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.12.1/README.md` & `caqui-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,40 @@
+Metadata-Version: 2.1
+Name: caqui
+Version: 1.9.0
+Summary: Run asynchronous commands in WebDrivers
+Project-URL: Homepage, https://github.com/douglasdcm/caqui
+Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
+Author-email: Douglas Cardoso <noemail@noemail.com>
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: aiohttp
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # Caqui
 
 **Caqui** is intended to command executions against Drivers synchronously and asynchronously. Launch the Driver as a server and send requests to it. The intention is that the user does not worry about which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/Winium.Desktop).
 
 The process **Caqui** follows is similar of the one described in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However, the motivation to create **Caqui** was feed by the inspiration in [Arsenic](https://github.com/HENNGE/arsenic) library.
 
 **Caqui** is planned to be Driver agnostic, so the user can start any Driver as a server and just inform the server URL. Hence, the code is decoupled from the chosen Driver.
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
-| WebDriver               | Version       | Remote* | Comment |
-| ----------------------- | ------------- | ------- |-------- |
-| Appium                  | 2.0.0         | Y       | Accepts remote calls by default. Tested with Appium in Docker container |
-| Firefox (geckodriver)   | 113           | Y       | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome           | 113, 114      | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78" |
-| Opera                   | 99            | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome |
-| WinAppDriver            | 1.2.1         | Y       | Need to define the host ip, e.g. "WinAppDriver.exe 10.0.0.10 4723" |
-| Winium Desktop          | 1.6.0         | Y       | Accepts remote calls by default |
-
-* Accepts remote requests when running as servers
+| WebDriver               | Version       |
+| ----------------------- | ------------- |
+| Google Chrome           | 113, 114      |
+| Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
 ```
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-# Caqui **Caqui** is intended to command executions against Drivers
-synchronously and asynchronously. Launch the Driver as a server and send
-requests to it. The intention is that the user does not worry about which
-Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
+Metadata-Version: 2.1 Name: caqui Version: 1.9.0 Summary: Run asynchronous
+commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
+caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
+Author-email: Douglas Cardoso
+noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
+Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
+Content-Type: text/markdown # Caqui **Caqui** is intended to command executions
+against Drivers synchronously and asynchronously. Launch the Driver as a server
+and send requests to it. The intention is that the user does not worry about
+which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
 www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/
 2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/
 Winium.Desktop). The process **Caqui** follows is similar of the one described
 in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-
 http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with
 [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However,
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
-Tested WebDrivers | WebDriver | Version | Remote* | Comment | | ---------------
--------- | ------------- | ------- |-------- | | Appium | 2.0.0 | Y | Accepts
-remote calls by default. Tested with Appium in Docker container | | Firefox
-(geckodriver) | 113 | Y | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome | 113, 114 | Y | Need to inform allowed ips to connect, e.g "--
-allowed-ips=123.45.6.78" | | Opera | 99 | Y | Need to inform allowed ips to
-connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome | |
-WinAppDriver | 1.2.1 | Y | Need to define the host ip, e.g. "WinAppDriver.exe
-10.0.0.10 4723" | | Winium Desktop | 1.6.0 | Y | Accepts remote calls by
-default | * Accepts remote requests when running as servers # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

### Comparing `caqui-1.12.1/pyproject.toml` & `caqui-1.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.12.1"
+version = "1.9.0"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `caqui-1.12.1/PKG-INFO` & `caqui-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,23 @@
-Metadata-Version: 2.1
-Name: caqui
-Version: 1.12.1
-Summary: Run asynchronous commands in WebDrivers
-Project-URL: Homepage, https://github.com/douglasdcm/caqui
-Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
-Author-email: Douglas Cardoso <noemail@noemail.com>
-License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Requires-Dist: aiohttp
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # Caqui
 
 **Caqui** is intended to command executions against Drivers synchronously and asynchronously. Launch the Driver as a server and send requests to it. The intention is that the user does not worry about which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/Winium.Desktop).
 
 The process **Caqui** follows is similar of the one described in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However, the motivation to create **Caqui** was feed by the inspiration in [Arsenic](https://github.com/HENNGE/arsenic) library.
 
 **Caqui** is planned to be Driver agnostic, so the user can start any Driver as a server and just inform the server URL. Hence, the code is decoupled from the chosen Driver.
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
-| WebDriver               | Version       | Remote* | Comment |
-| ----------------------- | ------------- | ------- |-------- |
-| Appium                  | 2.0.0         | Y       | Accepts remote calls by default. Tested with Appium in Docker container |
-| Firefox (geckodriver)   | 113           | Y       | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome           | 113, 114      | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78" |
-| Opera                   | 99            | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome |
-| WinAppDriver            | 1.2.1         | Y       | Need to define the host ip, e.g. "WinAppDriver.exe 10.0.0.10 4723" |
-| Winium Desktop          | 1.6.0         | Y       | Accepts remote calls by default |
-
-* Accepts remote requests when running as servers
+| WebDriver               | Version       |
+| ----------------------- | ------------- |
+| Google Chrome           | 113, 114      |
+| Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,29 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.12.1 Summary: Run asynchronous
-commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
-caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
-Author-email: Douglas Cardoso
-noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
-Python: >=3.6 Requires-Dist: aiohttp Requires-Dist: requests Description-
-Content-Type: text/markdown # Caqui **Caqui** is intended to command executions
-against Drivers synchronously and asynchronously. Launch the Driver as a server
-and send requests to it. The intention is that the user does not worry about
-which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
+# Caqui **Caqui** is intended to command executions against Drivers
+synchronously and asynchronously. Launch the Driver as a server and send
+requests to it. The intention is that the user does not worry about which
+Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
 www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/
 2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/
 Winium.Desktop). The process **Caqui** follows is similar of the one described
 in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-
 http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with
 [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However,
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
-Tested WebDrivers | WebDriver | Version | Remote* | Comment | | ---------------
--------- | ------------- | ------- |-------- | | Appium | 2.0.0 | Y | Accepts
-remote calls by default. Tested with Appium in Docker container | | Firefox
-(geckodriver) | 113 | Y | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome | 113, 114 | Y | Need to inform allowed ips to connect, e.g "--
-allowed-ips=123.45.6.78" | | Opera | 99 | Y | Need to inform allowed ips to
-connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome | |
-WinAppDriver | 1.2.1 | Y | Need to define the host ip, e.g. "WinAppDriver.exe
-10.0.0.10 4723" | | Winium Desktop | 1.6.0 | Y | Accepts remote calls by
-default | * Accepts remote requests when running as servers # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

