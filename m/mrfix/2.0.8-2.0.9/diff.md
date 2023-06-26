# Comparing `tmp/mrfix-2.0.8.tar.gz` & `tmp/mrfix-2.0.9.tar.gz`

## Comparing `mrfix-2.0.8.tar` & `mrfix-2.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-2.0.8/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-2.0.8/src/mrfix/__init__.py
--rw-r--r--   0        0        0    35469 2020-02-02 00:00:00.000000 mrfix-2.0.8/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-2.0.8/.gitignore
--rw-r--r--   0        0        0    76051 2020-02-02 00:00:00.000000 mrfix-2.0.8/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    76559 2020-02-02 00:00:00.000000 mrfix-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-2.0.9/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-2.0.9/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    35359 2020-02-02 00:00:00.000000 mrfix-2.0.9/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-2.0.9/.gitignore
+-rw-r--r--   0        0        0    76051 2020-02-02 00:00:00.000000 mrfix-2.0.9/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    76559 2020-02-02 00:00:00.000000 mrfix-2.0.9/PKG-INFO
```

### Comparing `mrfix-2.0.8/LICENZE` & `mrfix-2.0.9/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.8/src/mrfix/mrfix.py` & `mrfix-2.0.9/src/mrfix/mrfix.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,39 +565,36 @@
 
         finally:
             if success == False:
                 sys.exit()
 
     @staticmethod
     def make_displayed_with_arrow_down_and_click(driver, element_xpath, waiting_time):
-        success = False
         original_timeout = driver.get_timeout()
         try:
             wait = WebDriverWait(driver, waiting_time)
             element = wait.until(EC.visibility_of_element_located((By.XPATH, element_xpath)))
             if not element.is_displayed():
                 attempts = 0
                 while not element.is_displayed() and attempts < waiting_time:
                     element.send_keys(Keys.ARROW_DOWN)
                     time.sleep(0.1)
                     attempts += 1
                 if attempts == waiting_time * 10:
                     raise Exception("Element did not become visible within the specified maximum waiting time.")
-            success = True
             return True
         except NoSuchElementException:
             return f"Element with XPath '{element_xpath}' not found."
         except Exception as e:
             # Handle any exceptions and return error message
             error_message = str(e)
             return error_message
         finally:
             driver.implicitly_wait(original_timeout)
-            if success == False:
-                sys.exit()
+
 
 
     @staticmethod
     def make_displayed_with_arrow_up_and_click(driver, element_xpath, waiting_time):
         success = False
         try:
             # Wait for the element to be displayed by pressing the "arrow down" key
```

### Comparing `mrfix-2.0.8/.gitignore` & `mrfix-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.8/README.md` & `mrfix-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.8/pyproject.toml` & `mrfix-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "2.0.8"
+version = "2.0.9"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-2.0.8/PKG-INFO` & `mrfix-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 2.0.8
+Version: 2.0.9
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

