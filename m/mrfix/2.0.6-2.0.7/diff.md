# Comparing `tmp/mrfix-2.0.6.tar.gz` & `tmp/mrfix-2.0.7.tar.gz`

## Comparing `mrfix-2.0.6.tar` & `mrfix-2.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-2.0.6/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-2.0.6/src/mrfix/__init__.py
--rw-r--r--   0        0        0    35558 2020-02-02 00:00:00.000000 mrfix-2.0.6/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-2.0.6/.gitignore
--rw-r--r--   0        0        0    76051 2020-02-02 00:00:00.000000 mrfix-2.0.6/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-2.0.6/pyproject.toml
--rw-r--r--   0        0        0    76559 2020-02-02 00:00:00.000000 mrfix-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-2.0.7/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-2.0.7/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    35593 2020-02-02 00:00:00.000000 mrfix-2.0.7/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-2.0.7/.gitignore
+-rw-r--r--   0        0        0    76051 2020-02-02 00:00:00.000000 mrfix-2.0.7/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0    76559 2020-02-02 00:00:00.000000 mrfix-2.0.7/PKG-INFO
```

### Comparing `mrfix-2.0.6/LICENZE` & `mrfix-2.0.7/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.6/src/mrfix/mrfix.py` & `mrfix-2.0.7/src/mrfix/mrfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,14 +584,15 @@
                     if element.is_displayed():
                         # Click on the element
                         element.click()
                         break
                     stop_time = datetime.datetime.now()
                     delta = stop_time - start_time
                 except:
+                    success = True
                     pass
 
             success = True
             # Return True if the element is displayed and clicked successfully
             return True
 
         except TimeoutException:
```

### Comparing `mrfix-2.0.6/.gitignore` & `mrfix-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.6/README.md` & `mrfix-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mrfix-2.0.6/pyproject.toml` & `mrfix-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "2.0.6"
+version = "2.0.7"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-2.0.6/PKG-INFO` & `mrfix-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrfix
-Version: 2.0.6
+Version: 2.0.7
 Summary: A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

