# Comparing `tmp/ibeam-0.4.5.tar.gz` & `tmp/ibeam-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibeam-0.4.5.tar", last modified: Tue May 30 17:45:19 2023, max compression
+gzip compressed data, was "ibeam-0.4.6.tar", last modified: Mon Jun 26 14:54:57 2023, max compression
```

## Comparing `ibeam-0.4.5.tar` & `ibeam-0.4.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.555596 ibeam-0.4.5/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.5/LICENSE
--rw-rw-rw-   0        0        0    10463 2023-05-30 17:45:19.555596 ibeam-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     9800 2022-08-31 12:47:22.000000 ibeam-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.445764 ibeam-0.4.5/ibeam/
--rw-rw-rw-   0        0        0       74 2023-05-30 17:03:40.000000 ibeam-0.4.5/ibeam/__init__.py
--rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/config.py
--rw-rw-rw-   0        0        0     3850 2023-05-04 18:30:06.000000 ibeam-0.4.5/ibeam/ibeam_starter.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.524350 ibeam-0.4.5/ibeam/src/
--rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.5/ibeam/src/__init__.py
--rw-rw-rw-   0        0        0    20947 2023-05-23 19:26:05.000000 ibeam-0.4.5/ibeam/src/authenticate.py
--rw-rw-rw-   0        0        0    15619 2023-05-16 12:49:10.000000 ibeam-0.4.5/ibeam/src/gateway_client.py
--rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.5/ibeam/src/health_server.py
--rw-rw-rw-   0        0        0     7805 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/http_handler.py
--rw-rw-rw-   0        0        0     1314 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/inputs_handler.py
--rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.5/ibeam/src/logs.py
--rw-rw-rw-   0        0        0     1851 2023-05-04 18:30:58.000000 ibeam-0.4.5/ibeam/src/process_utils.py
--rw-rw-rw-   0        0        0      305 2023-05-23 18:02:24.000000 ibeam-0.4.5/ibeam/src/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.539973 ibeam-0.4.5/ibeam/src/two_fa_handlers/
--rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/__init__.py
--rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/external_request_handler.py
--rw-rw-rw-   0        0        0     5387 2023-05-04 18:33:34.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/google_msg_handler.py
--rw-rw-rw-   0        0        0     2975 2023-05-03 22:42:05.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/notification_resend_handler.py
--rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.5/ibeam/src/two_fa_handlers/two_fa_handler.py
--rw-rw-rw-   0        0        0     2682 2023-04-01 23:25:13.000000 ibeam-0.4.5/ibeam/src/two_fa_selector.py
--rw-rw-rw-   0        0        0     6087 2023-05-03 22:26:29.000000 ibeam-0.4.5/ibeam/src/var.py
-drwxrwxrwx   0        0        0        0 2023-05-30 17:45:19.477018 ibeam-0.4.5/ibeam.egg-info/
--rw-rw-rw-   0        0        0    10463 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 17:45:19.000000 ibeam-0.4.5/ibeam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-30 17:45:19.555596 ibeam-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1378 2023-05-16 19:48:03.000000 ibeam-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:54:57.945297 ibeam-0.4.6/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibeam-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0    10463 2023-06-26 14:54:57.946264 ibeam-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9800 2022-08-31 12:47:22.000000 ibeam-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:54:57.844286 ibeam-0.4.6/ibeam/
+-rw-rw-rw-   0        0        0       74 2023-06-26 14:34:44.000000 ibeam-0.4.6/ibeam/__init__.py
+-rw-rw-rw-   0        0        0      349 2021-06-21 13:45:43.000000 ibeam-0.4.6/ibeam/config.py
+-rw-rw-rw-   0        0        0     3850 2023-05-04 18:30:06.000000 ibeam-0.4.6/ibeam/ibeam_starter.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:54:57.918501 ibeam-0.4.6/ibeam/src/
+-rw-rw-rw-   0        0        0        0 2020-10-09 05:29:20.000000 ibeam-0.4.6/ibeam/src/__init__.py
+-rw-rw-rw-   0        0        0    21949 2023-06-21 19:18:51.000000 ibeam-0.4.6/ibeam/src/authenticate.py
+-rw-rw-rw-   0        0        0    15928 2023-06-19 19:08:04.000000 ibeam-0.4.6/ibeam/src/gateway_client.py
+-rw-rw-rw-   0        0        0     1696 2022-06-27 14:32:23.000000 ibeam-0.4.6/ibeam/src/health_server.py
+-rw-rw-rw-   0        0        0     7805 2023-05-04 18:33:34.000000 ibeam-0.4.6/ibeam/src/http_handler.py
+-rw-rw-rw-   0        0        0     1314 2023-05-04 18:33:34.000000 ibeam-0.4.6/ibeam/src/inputs_handler.py
+-rw-rw-rw-   0        0        0     1668 2022-04-07 12:15:07.000000 ibeam-0.4.6/ibeam/src/logs.py
+-rw-rw-rw-   0        0        0     1851 2023-05-04 18:30:58.000000 ibeam-0.4.6/ibeam/src/process_utils.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 18:02:24.000000 ibeam-0.4.6/ibeam/src/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:54:57.942244 ibeam-0.4.6/ibeam/src/two_fa_handlers/
+-rw-rw-rw-   0        0        0        0 2022-08-09 08:38:04.000000 ibeam-0.4.6/ibeam/src/two_fa_handlers/__init__.py
+-rw-rw-rw-   0        0        0     2941 2021-06-21 13:45:43.000000 ibeam-0.4.6/ibeam/src/two_fa_handlers/external_request_handler.py
+-rw-rw-rw-   0        0        0     5387 2023-05-04 18:33:34.000000 ibeam-0.4.6/ibeam/src/two_fa_handlers/google_msg_handler.py
+-rw-rw-rw-   0        0        0     2975 2023-05-03 22:42:05.000000 ibeam-0.4.6/ibeam/src/two_fa_handlers/notification_resend_handler.py
+-rw-rw-rw-   0        0        0      264 2021-06-21 13:45:43.000000 ibeam-0.4.6/ibeam/src/two_fa_handlers/two_fa_handler.py
+-rw-rw-rw-   0        0        0     2682 2023-04-01 23:25:13.000000 ibeam-0.4.6/ibeam/src/two_fa_selector.py
+-rw-rw-rw-   0        0        0     6540 2023-06-21 17:38:24.000000 ibeam-0.4.6/ibeam/src/var.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:54:57.864633 ibeam-0.4.6/ibeam.egg-info/
+-rw-rw-rw-   0        0        0    10463 2023-06-26 14:54:57.000000 ibeam-0.4.6/ibeam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-06-26 14:54:57.000000 ibeam-0.4.6/ibeam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:54:57.000000 ibeam-0.4.6/ibeam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-26 14:54:57.000000 ibeam-0.4.6/ibeam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 14:54:57.000000 ibeam-0.4.6/ibeam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-26 14:54:57.949265 ibeam-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-05-16 19:48:03.000000 ibeam-0.4.6/setup.py
```

### Comparing `ibeam-0.4.5/LICENSE` & `ibeam-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/PKG-INFO` & `ibeam-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.4.5
+Version: 0.4.6
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.4.5 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.4.6 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.4.5/README.md` & `ibeam-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/ibeam_starter.py` & `ibeam-0.4.6/ibeam/ibeam_starter.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/authenticate.py` & `ibeam-0.4.6/ibeam/src/authenticate.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from ibeam.src.py_utils import exception_to_string
 from ibeam.src.two_fa_handlers.two_fa_handler import TwoFaHandler
 
 _LOGGER = logging.getLogger('ibeam.' + Path(__file__).stem)
 
 _DRIVER_NAMES = {}
 _FAILED_ATTEMPTS = 0
+_PRESUBMIT_BUFFER = var.MIN_PRESUBMIT_BUFFER
 
 _VERSIONS = {
     1: {
         'USER_NAME_EL': 'user_name',
         'ERROR_EL': 'alert alert-danger margin-top-10'
     },
     2: {
@@ -235,14 +236,18 @@
     """
     base_url = base_url if base_url is not None else var.GATEWAY_BASE_URL
     display = None
     success = False
     driver = None
     website_version = -1
     elements = {}
+
+    global _PRESUBMIT_BUFFER
+    presubmit_buffer = _PRESUBMIT_BUFFER
+
     try:
         _LOGGER.info(f'Loading auth webpage at {base_url + var.ROUTE_AUTH}')
         if sys.platform == 'linux':
             display = Display(visible=False, size=(800, 600))
             display.start()
 
         driver = start_driver(base_url, driver_path)
@@ -268,25 +273,29 @@
             _LOGGER.info(f'Login attempt number {immediate_attempts}')
 
             # time.sleep(300)
 
             # input credentials
             user_name_el = driver.find_element(By.NAME, elements['USER_NAME_EL'])
             password_el = driver.find_element(By.NAME, elements['PASSWORD_EL'])
+
+            user_name_el.clear()
+            password_el.clear()
+
             user_name_el.send_keys(account)
 
             if key is None:
                 password_el.send_keys(password)
             else:
                 password_el.send_keys(Fernet(key).decrypt(password.encode('utf-8')).decode("utf-8"))
 
             password_el.send_keys(Keys.TAB)
 
             # small buffer to prevent race-condition on client side
-            time.sleep(5)
+            time.sleep(presubmit_buffer)
             # submit the form
             _LOGGER.info('Submitting the form')
             submit_form_el = driver.find_element(By.CSS_SELECTOR, elements['SUBMIT_EL'])
             submit_form_el.click()
 
             # observe results - either success or 2FA request
             success_present = text_to_be_present_in_element([(By.TAG_NAME, 'pre'), (By.TAG_NAME, 'body')],
@@ -354,14 +363,16 @@
 
                 if two_fa_code is None:
                     _LOGGER.warning(f'No 2FA code returned. Aborting authentication.')
                 else:
                     two_fa_el = driver.find_elements(By.ID, elements['TWO_FA_INPUT_EL_ID'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         EC.element_to_be_clickable((By.ID, elements['TWO_FA_INPUT_EL_ID'])))
+
+                    two_fa_el[0].clear()
                     two_fa_el[0].send_keys(two_fa_code)
 
                     _LOGGER.info('Submitting the 2FA form')
                     submit_form_el = driver.find_element(By.CSS_SELECTOR, elements['SUBMIT_EL'])
                     WebDriverWait(driver, var.OAUTH_TIMEOUT).until(
                         EC.element_to_be_clickable((By.CSS_SELECTOR, elements['SUBMIT_EL'])))
                     submit_form_el.click()
@@ -378,14 +389,22 @@
                 trigger = WebDriverWait(driver, 10).until(any_of(success_present, error_displayed))
                 trigger_identifier = identify_trigger(trigger, elements)
 
             if trigger_identifier == elements['ERROR_EL']:
                 _LOGGER.error(f'Error displayed by the login webpage: {trigger.text}')
                 save_screenshot(driver, '__failed_attempt')
 
+                if trigger.text == 'Invalid username password combination' and presubmit_buffer < var.MAX_PRESUBMIT_BUFFER:
+                    _PRESUBMIT_BUFFER += 5
+                    if _PRESUBMIT_BUFFER >= var.MAX_PRESUBMIT_BUFFER:
+                        _PRESUBMIT_BUFFER = var.MAX_PRESUBMIT_BUFFER
+                        _LOGGER.warning(f'The presubmit buffer set to maximum: {var.MAX_PRESUBMIT_BUFFER}')
+                    else:
+                        _LOGGER.warning(f'Increased presubmit buffer to {_PRESUBMIT_BUFFER}')
+
                 # try to prevent having the account locked-out
                 if trigger.text == 'failed' or trigger.text == 'Invalid username password combination' and var.MAX_FAILED_AUTH > 0:
                     global _FAILED_ATTEMPTS
                     _FAILED_ATTEMPTS += 1
                     if _FAILED_ATTEMPTS >= var.MAX_FAILED_AUTH:
                         _LOGGER.critical(
                             f'######## ATTENTION! ######## Maximum number of failed authentication attempts (IBEAM_MAX_FAILED_AUTH={var.MAX_FAILED_AUTH}) reached. IBeam will shut down to prevent an account lock-out. It is recommended you attempt to authenticate manually in order to reset the counter. Read the execution logs and report issues at https://github.com/Voyz/ibeam/issues')
@@ -399,24 +418,28 @@
                 driver.refresh()
                 continue  # attempt a direct retry
                 pass  # this means no two_fa_code was returned and trigger remained the same - ie. don't authenticate
                 # todo: retry authentication or resend code
             elif trigger_identifier == elements['SUCCESS_EL_TEXT']:
                 _LOGGER.info('Webpage displayed "Client login succeeds"')
                 _FAILED_ATTEMPTS = 0
+                _PRESUBMIT_BUFFER = var.MIN_PRESUBMIT_BUFFER
                 success = True
                 break
 
         time.sleep(2)
     except TimeoutException as e:
-
+        page_loaded_correctly = True
         try:
             website_loaded = EC.presence_of_element_located((By.CLASS_NAME, 'login'))
             WebDriverWait(driver, 5).until(website_loaded)
         except TimeoutException as ee:
+            page_loaded_correctly = False
+
+        if not page_loaded_correctly or website_version == -1:
             _LOGGER.error(f'Timeout reached when waiting for authentication. The website seems to not be loaded correctly. Consider increasing IBEAM_PAGE_LOAD_TIMEOUT. \nWebsite URL: {base_url + var.ROUTE_AUTH} \nIBEAM_PAGE_LOAD_TIMEOUT: {var.PAGE_LOAD_TIMEOUT} \nException:\n{exception_to_string(e)}')
         else:
             _LOGGER.error(f'Timeout reached searching for website elements, but the website seems to be loaded correctly. It is possible the setup is incorrect. \nWebsite version: {website_version} \nDOM elements searched for: {elements}. \nException:\n{exception_to_string(e)}')
 
         save_screenshot(driver, '__timeout-exception')
         success = False
     except Exception as e:
```

### Comparing `ibeam-0.4.5/ibeam/src/gateway_client.py` & `ibeam-0.4.6/ibeam/src/gateway_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,20 @@
             time.sleep(3)  # buffer for session to be authenticated
 
             # double check if authenticated
             status = self.get_status(max_attempts=max(request_retries, 2))
             if not status.authenticated:
                 if status.session:
                     _LOGGER.error('Gateway session active but not authenticated')
+                    self.reauthenticate()
+
+                    if var.REAUTHENTICATE_WAIT > 0:
+                        _LOGGER.info(f'Waiting {var.REAUTHENTICATE_WAIT} seconds to reauthenticate before restarting.')
+                        time.sleep(var.REAUTHENTICATE_WAIT)
+
                     if var.RESTART_FAILED_SESSIONS:
                         _LOGGER.info('Logging out and restarting the Gateway')
                         self.restart()
                         return self.try_authenticating(request_retries=request_retries)
                 elif status.running:
                     _LOGGER.error('Gateway running but has no active sessions')
                 else:
@@ -325,14 +331,16 @@
             _LOGGER.exception(e)
 
     def start_and_authenticate(self, request_retries=1) -> (bool, bool):
         """Starts the gateway and authenticates using the credentials stored."""
 
         self.try_starting()
 
+        self.validate()
+
         success, shutdown = self.try_authenticating(request_retries=request_retries)
         self._should_shutdown = shutdown
         return success, shutdown
 
     def build_scheduler(self):
         if var.SPAWN_NEW_PROCESSES:
             executors = {'default': ProcessPoolExecutor(self._concurrent_maintenance_attempts)}
```

### Comparing `ibeam-0.4.5/ibeam/src/health_server.py` & `ibeam-0.4.6/ibeam/src/health_server.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/http_handler.py` & `ibeam-0.4.6/ibeam/src/http_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/inputs_handler.py` & `ibeam-0.4.6/ibeam/src/inputs_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/logs.py` & `ibeam-0.4.6/ibeam/src/logs.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/process_utils.py` & `ibeam-0.4.6/ibeam/src/process_utils.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/two_fa_handlers/external_request_handler.py` & `ibeam-0.4.6/ibeam/src/two_fa_handlers/external_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/two_fa_handlers/google_msg_handler.py` & `ibeam-0.4.6/ibeam/src/two_fa_handlers/google_msg_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/two_fa_handlers/notification_resend_handler.py` & `ibeam-0.4.6/ibeam/src/two_fa_handlers/notification_resend_handler.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/two_fa_selector.py` & `ibeam-0.4.6/ibeam/src/two_fa_selector.py`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/ibeam/src/var.py` & `ibeam-0.4.6/ibeam/src/var.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
 RESTART_FAILED_SESSIONS = bool(os.environ.get('IBEAM_RESTART_FAILED_SESSIONS', True))
 """Whether Gateway should be restarted on failed sessions."""
 
 RESTART_WAIT = int(os.environ.get('IBEAM_RESTART_WAIT', 15))
 """How many seconds to wait for a restart to complete."""
 
+REAUTHENTICATE_WAIT = int(os.environ.get('IBEAM_REAUTHENTICATE_WAIT', 15))
+"""How many seconds to wait for a reauthentication to complete."""
+
 IBEAM_HEALTH_SERVER_PORT = int(os.environ.get("IBEAM_HEALTH_SERVER_PORT", 5001))
 """Port to start health server on."""
 
 ########### GATEWAY ROUTES ###########
 
 GATEWAY_BASE_URL = os.environ.get('IBEAM_GATEWAY_BASE_URL', "https://localhost:5000")
 """Base URL of the gateway."""
@@ -101,14 +104,20 @@
 
 ERROR_SCREENSHOTS = bool(os.environ.get('IBEAM_ERROR_SCREENSHOTS', False))
 """Whether to save login page screenshots on error."""
 
 MAX_FAILED_AUTH = int(os.environ.get('IBEAM_MAX_FAILED_AUTH', 5))
 """Maximum number of failed authentication attempts."""
 
+MIN_PRESUBMIT_BUFFER = int(os.environ.get('IBEAM_MIN_PRESUBMIT_BUFFER', 5))
+"""Minimum number of seconds to wait before hitting the submit button"""
+
+MAX_PRESUBMIT_BUFFER = int(os.environ.get('IBEAM_MAX_PRESUBMIT_BUFFER', 30))
+"""Maximum number of seconds to wait before hitting the submit button"""
+
 MAX_IMMEDIATE_ATTEMPTS = int(os.environ.get('IBEAM_MAX_IMMEDIATE_ATTEMPTS', 10))
 """Maximum number of immediate retries upon detecting an error message."""
 
 IBKEY_PROMO_EL_CLASS = os.environ.get('IBEAM_IBKEY_PROMO_EL_CLASS', 'ibkey-promo-skip')
 """HTML element class containing the ibkey promo skip button."""
 
 ########### TWO-FACTOR AUTHENTICATION ###########
```

### Comparing `ibeam-0.4.5/ibeam.egg-info/PKG-INFO` & `ibeam-0.4.6/ibeam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibeam
-Version: 0.4.5
+Version: 0.4.6
 Summary: IBeam is an authentication and maintenance tool used for the Interactive Brokers Client Portal Web API Gateway.
 Home-page: https://github.com/Voyz/ibeam
 Author: Voy Zan
 Author-email: voy1982@yahoo.co.uk
 License: Apache-2.0
 Keywords: interactive brokers,algo trading,algorithmic trading,data flow,quant,trading
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ibeam Version: 0.4.5 Summary: IBeam is an
+Metadata-Version: 2.1 Name: ibeam Version: 0.4.6 Summary: IBeam is an
 authentication and maintenance tool used for the Interactive Brokers Client
 Portal Web API Gateway. Home-page: https://github.com/Voyz/ibeam Author: Voy
 Zan Author-email: voy1982@yahoo.co.uk License: Apache-2.0 Keywords: interactive
 brokers,algo trading,algorithmic trading,data flow,quant,trading Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7 Description-Content-Type:
```

### Comparing `ibeam-0.4.5/ibeam.egg-info/SOURCES.txt` & `ibeam-0.4.6/ibeam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibeam-0.4.5/setup.py` & `ibeam-0.4.6/setup.py`

 * *Files identical despite different names*

