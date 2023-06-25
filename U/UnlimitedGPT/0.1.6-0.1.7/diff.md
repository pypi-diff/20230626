# Comparing `tmp/UnlimitedGPT-0.1.6.tar.gz` & `tmp/UnlimitedGPT-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.6.tar", last modified: Mon Jun 12 22:29:11 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.7.tar", last modified: Sun Jun 25 22:41:35 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.6.tar` & `UnlimitedGPT-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.307382 UnlimitedGPT-0.1.6/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.299382 UnlimitedGPT-0.1.6/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    38856 2023-06-12 22:15:15.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      271 2023-06-12 22:06:37.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2559 2023-06-12 21:33:12.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1274 2023-06-12 19:02:03.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      116 2023-06-12 15:20:24.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13597 2023-06-12 21:54:34.000000 UnlimitedGPT-0.1.6/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-12 22:29:11.303382 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-12 22:29:10.000000 UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-12 22:29:11.307382 UnlimitedGPT-0.1.6/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-12 21:57:38.000000 UnlimitedGPT-0.1.6/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.220149 UnlimitedGPT-0.1.7/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    40614 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      271 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2268 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1274 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      116 2023-06-12 15:20:24.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    13290 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4439 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-25 22:41:35.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       59 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-25 22:41:34.000000 UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-25 22:41:35.224149 UnlimitedGPT-0.1.7/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-25 22:41:00.000000 UnlimitedGPT-0.1.7/setup.py
```

### Comparing `UnlimitedGPT-0.1.6/PKG-INFO` & `UnlimitedGPT-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.6
+Version: 0.1.7
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.6/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.7/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from undetected_chromedriver import ChromeOptions
 
 from .internal.chatgpt_data import ChatGPTVariables as CGPTV
 from .internal.driver import ChatGPTDriver
 from .internal.exceptions import InvalidConversationID
 from .internal.objects import ChatGPTResponse, Conversations, SessionData, SharedConversations, User, Accounts
 
-
 class ChatGPT:
     """
     A class for interacting with ChatGPT.
 
     Args:
     ----------
         session_token (str): The session token for authentication.
@@ -409,36 +408,41 @@
 
             self.logger.debug("Clicked shared links manage button")
         except:
             self.logger.debug("Could not open shared conversations popup")
 
         return self._get_out_of_menu()
 
-    def get_user_data(self):
+    def get_user_data(self) -> Optional[Accounts]:
         """
         Gets the user data.
 
         Returns
         ---------
-            Accounts: a list of the accounts.
+            Optional[Accounts]: a list of the accounts.
         """
         self.logger.debug("Getting user data...")
 
         logs_raw = self.driver.get_log("performance")
 
-        data = next(
+        datas = (
             log_["params"]["requestId"]
             for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
             if (
                 log_["method"] == "Network.responseReceived"
                 and "json" in log_["params"]["response"]["mimeType"]
-                and log_["params"]["response"]["status"] == 200
+                and int(log_["params"]["response"]["status"]) == 200
                 and "backend-api/accounts/check/" in log_["params"]["response"]["url"]
             )
         )
+        try:
+            data = next(datas)
+        except StopIteration:
+            self.logger.debug("Could not find user data")
+            return None
 
         ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
 
         response_data = loads(ret["body"])
 
         return Accounts(response_data)
 
@@ -449,24 +453,29 @@
         Returns:
         ----------
             Conversations: A list of conversations.
         """
         self.logger.debug("Getting conversations...")
         logs_raw = self.driver.get_log("performance")
 
-        data = next(
+        datas = (
             log_["params"]["requestId"]
             for log_ in reversed([loads(lr["message"])["message"] for lr in logs_raw])
             if (
                 log_["method"] == "Network.responseReceived"
                 and "json" in log_["params"]["response"]["mimeType"]
                 and log_["params"]["response"]["status"] == 200
                 and "/backend-api/conversations" in log_["params"]["response"]["url"]
             )
         )
+        try:
+            data = next(datas)
+        except StopIteration:
+            self.logger.debug("Could not find conversations")
+            return None
 
         self.logger.debug("Found conversations")
 
         ret = self.driver.execute_cdp_cmd("Network.getResponseBody", {"requestId": data})
 
         response_data = loads(ret["body"])
 
@@ -562,25 +571,26 @@
 
         Raises:
         ----------
             TimeoutException: If the message fails to send.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
+        assert input_mode in ["INSTANT", "SLOW"], "Invalid input mode"
         self.logger.debug(
             f'Sending message with mode {input_mode}{f" with {input_delay} delay" if input_mode == "SLOW" else ""}...'
         )
 
         textbox = WebDriverWait(self.driver, 60).until(
             EC.element_to_be_clickable(CGPTV.textbox)
         )
         if input_mode == "INSTANT":
             self.driver.execute_script(
                 "arguments[0].value = arguments[1];", textbox, message
-            )
+            ) # TODO: This isn't working, its just using SLOW mode instead
         else:
             for char in message:
                 try:
                     textbox.send_keys(char)
                 except StaleElementReferenceException:
                     textbox = WebDriverWait(self.driver, 60).until(
                         EC.element_to_be_clickable(CGPTV.textbox)
@@ -795,49 +805,76 @@
             ).get_attribute("class")
             current_theme = "LIGHT" if "light" in current_theme_value else "DARK"
             if theme == current_theme:
                 self.logger.debug("Theme is already set to the desired theme")
                 return self._get_out_of_menu()
             self.logger.debug(f"Current theme is {current_theme}")
 
-            select_element = self.driver.find_element(*CGPTV.theme_select)
-            ActionChains(self.driver).move_to_element(select_element).perform()
-            select_clicked = self.driver.safe_click(CGPTV.theme_select, timeout=60)
-            if not select_clicked:
-                self.logger.debug("Could not click theme select")
+            button_element = self.driver.find_element(*CGPTV.theme_button)
+            ActionChains(self.driver).move_to_element(button_element).perform()
+            button_clicked = self.driver.safe_click(CGPTV.theme_button, timeout=60)
+            if not button_clicked:
+                self.logger.debug("Could not click theme button")
+                return self._get_out_of_menu()
+            self.logger.debug("Clicked theme button")
+
+            try:
+                WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.CSS_SELECTOR, "[role='option']")))
+            except TimeoutException: # type: ignore
+                self.logger.debug("Could not load theme options")
                 return self._get_out_of_menu()
-            self.logger.debug("Clicked theme select")
 
+            options = self.driver.find_elements(By.CSS_SELECTOR, "[role='option']")
+            if not options:
+                self.logger.debug("Could not find theme options")
+                return self._get_out_of_menu()
+            
             if theme == "OPPOSITE":
                 if current_theme == "SYSTEM":
                     self.logger.debug("Theme cannot be set to opposite of system theme")
                     return self._get_out_of_menu()
 
                 opposite_theme = "dark" if current_theme == "LIGHT" else "light"
-                option_clicked = self.driver.safe_click(
-                    (By.CSS_SELECTOR, f"select.rounded option[value={opposite_theme}]"),
-                    timeout=60,
-                )
-                if not option_clicked:
-                    self.logger.debug("Could not click opposite theme option")
+                try:
+                    for option in options:
+                        safe_option = WebDriverWait(self, 10).until(
+                            EC.element_to_be_clickable(option)
+                        )
+                        if safe_option.text.lower() == opposite_theme.lower():
+                            try:
+                                safe_option.click()
+                            except:
+                                self.logger.debug("Could not click opposite theme option")
+                                return self._get_out_of_menu()
+                except:
+                    self.logger.debug(f"Could not find theme option {theme}")
                     return self._get_out_of_menu()
+
                 self.logger.debug(f"Selected opposite theme of {current_theme}")
             else:
-                option_clicked = self.driver.safe_click(
-                    (By.CSS_SELECTOR, f"select.rounded option[value={theme.lower()}]"),
-                    timeout=60,
-                )
-                if not option_clicked:
-                    self.logger.debug("Could not click theme option")
+                try:
+                    for option in options:
+                        safe_option = WebDriverWait(self, 10).until(
+                            EC.element_to_be_clickable(option)
+                        )
+                        if safe_option.text.lower() == theme.lower():
+                            try:
+                                safe_option.click()
+                            except:
+                                self.logger.debug("Could not click opposite theme option")
+                                return self._get_out_of_menu()
+                except:
+                    self.logger.debug(f"Could not find theme option {theme}")
                     return self._get_out_of_menu()
+
                 self.logger.debug(f"Selected theme {theme}")
 
             self.logger.debug("Theme switched")
             self._get_out_of_menu()
-        except NoSuchElementException: # type: ignore
+        except NoSuchElementException as e: # type: ignore
             self.logger.debug("Could not find theme buttons")
             return self._get_out_of_menu()
 
     def switch_account(self, session_token: str) -> SessionData:
         """
         Switch the account.
 
@@ -980,15 +1017,15 @@
                 self.logger.debug("Could not click data controls button")
                 return self._get_out_of_menu()
 
             # Click "Disable chat history" button
             # Not using safe_click because it there are some checks that need to be done before clicking
             chat_history_toggle = wait.until(
                 EC.element_to_be_clickable(
-                    (By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')
+                    (By.CSS_SELECTOR, f'button[aria-label="Chat history & training"]')
                 )
             )
             current_state = (
                 True
                 if chat_history_toggle.get_attribute("aria-checked") == "true"
                 else False
             )
```

### Comparing `UnlimitedGPT-0.1.6/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.7/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.6/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.7/UnlimitedGPT/internal/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,22 +296,20 @@
         Initialize an Accounts object.
 
         Args:
         ----------
             data (dict)
         """
         self.default = DefaultAccount(**data["accounts"]['default'])
-        self.account_invites: list = data['account_invites']
-        self.temp_ap_available_at: str = data['temp_ap_available_at']
 
     def __str__(self):
-        return f"<Accounts default={self.default} account_invites={self.account_invites} temp_ap_available_at={self.temp_ap_available_at}>"
+        return f"<Accounts default={self.default}>"
 
     def __repr__(self):
-        return f"<Accounts default={self.default} account_invites={self.account_invites} temp_ap_available_at={self.temp_ap_available_at}>"
+        return f"<Accounts default={self.default}>"
 
 class SharedConversation:
     """Class representing a shared conversation."""
 
     def __init__(
         self,
         id: str,
```

### Comparing `UnlimitedGPT-0.1.6/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.7/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.6
+Version: 0.1.7
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.6/setup.py` & `UnlimitedGPT-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     author="Sxvxge",
     url="https://github.com/Sxvxgee/UnlimitedGPT",
     project_urls={
         "Documentation": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md",
         "Issue tracker": "https://github.com/Sxvxgee/UnlimitedGPT/issues",
         "Changelog": "https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md",
     },
-    version="0.1.6",
+    version="0.1.7",
     packages=["UnlimitedGPT", "UnlimitedGPT/internal"],
     py_modules=["UnlimitedGPT"],
     license="GPL-3.0 license",
     description="An unofficial Python wrapper for OpenAI's ChatGPT API",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
```

