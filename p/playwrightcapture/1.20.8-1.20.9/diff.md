# Comparing `tmp/playwrightcapture-1.20.8.tar.gz` & `tmp/playwrightcapture-1.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.8.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.9.tar", max compression
```

## Comparing `playwrightcapture-1.20.8.tar` & `playwrightcapture-1.20.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.8/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.8/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.8/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    37285 2023-06-23 10:01:37.189758 playwrightcapture-1.20.8/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.8/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.8/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.8/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1828 2023-06-23 10:34:00.689887 playwrightcapture-1.20.8/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.8/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.9/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.9/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.9/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    37604 2023-06-26 11:33:09.009980 playwrightcapture-1.20.9/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.9/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.9/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.9/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1826 2023-06-26 11:39:18.215411 playwrightcapture-1.20.9/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.9/PKG-INFO
```

### Comparing `playwrightcapture-1.20.8/LICENSE` & `playwrightcapture-1.20.9/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.8/README.md` & `playwrightcapture-1.20.9/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.8/playwrightcapture/capture.py` & `playwrightcapture-1.20.9/playwrightcapture/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,22 +577,29 @@
                 # this one sounds like something we can retry...
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
                             'Navigation interrupted by another one',
                             'Navigation failed because page was closed!',
-                            'Connection closed while reading from the driver',
                             'Protocol error (Page.bringToFront): Not attached to an active page']:
                 # Other errors, let's give it another shot
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             else:
                 # Unexpected ones
                 self.logger.exception(f'Something went poorly with {url}: {e.message}')
+        except Exception as e:
+            # we may get a non-playwright exception to.
+            # The ones we try to handle here should be treated as if they were.
+            if str(e) in ['Connection closed while reading from the driver']:
+                self.logger.info(f'Issue with {url} (retrying): {e}')
+                self.should_retry = True
+            else:
+                raise e
         finally:
             if not capturing_sub:
                 to_return['cookies'] = await self.context.cookies()
                 # frames_tree = self.make_frame_tree(page.main_frame)
                 try:
                     await self.context.close()  # context needs to be closed to generate the HAR
                     with open(self._temp_harfile.name) as _har:
```

### Comparing `playwrightcapture-1.20.8/playwrightcapture/helpers.py` & `playwrightcapture-1.20.9/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.8/pyproject.toml` & `playwrightcapture-1.20.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.8"
+version = "1.20.9"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -35,19 +35,19 @@
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-types-beautifulsoup4 = "^4.12.0.3"
-pytest = "^7.3.1"
-mypy = "^1.2.0"
+types-beautifulsoup4 = "^4.12.0.5"
+pytest = "^7.4.0"
+mypy = "^1.4.1"
 types-dateparser = "^1.1.4.9"
-types-requests = "^2.28.11.17"
+types-requests = "^2.31.0.1"
 types-pytz = "^2023.3.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playwrightcapture-1.20.8/PKG-INFO` & `playwrightcapture-1.20.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.8
+Version: 1.20.9
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

