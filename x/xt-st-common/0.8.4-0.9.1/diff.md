# Comparing `tmp/xt_st_common-0.8.4.tar.gz` & `tmp/xt_st_common-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.8.4.tar", max compression
+gzip compressed data, was "xt_st_common-0.9.1.tar", max compression
```

## Comparing `xt_st_common-0.8.4.tar` & `xt_st_common-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-14 03:58:20.438397 xt_st_common-0.8.4/README.md
--rw-r--r--   0        0        0     2603 2023-06-14 03:58:20.438397 xt_st_common-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-14 03:57:43.501947 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-14 03:57:43.521948 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-14 03:57:43.525948 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-14 03:58:20.434397 xt_st_common-0.8.4/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2750 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3464 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    42607 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6941 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6936 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-14 03:57:43.601949 xt_st_common-0.8.4/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-26 11:40:55.892487 xt_st_common-0.9.1/README.md
+-rw-r--r--   0        0        0     3302 2023-06-26 11:40:55.892487 xt_st_common-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-26 11:40:51.280419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-26 11:40:51.300419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-26 11:40:51.300419 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-26 11:40:55.892487 xt_st_common-0.9.1/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5001 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2804 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3492 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6269 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    48663 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0    10496 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5933 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     7558 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     2040 2023-06-26 11:40:51.380421 xt_st_common-0.9.1/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.9.1/PKG-INFO
```

### Comparing `xt_st_common-0.8.4/README.md` & `xt_st_common-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.8.4
+# XT-STREAMLIT - 0.9.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.8.4/pyproject.toml` & `xt_st_common-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.8.4"
+version = "0.9.1"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
-test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
+
 clean = { cmd = "rm -rf .coverage .mypy_cache .pytest_cache dist ./**/__pycache__ docs/build/ dist docs/build docs/source/_static docs/source/wpf.*.rst", help = "Clean up build artifacts" }
 lint = { cmd = "pre-commit run", help = "Run pre-commit hooks" }
 install = {cmd = "poetry install --all-extras", help="Install all dependecnies"}
 format-black = { cmd = "black .", help="Run Black formater"}
 format-ruff = { cmd = "ruff src/xt_st_common --fix", help="Run Ruff linter and apply fixes"}
-format = { sequence=["format-black", "format-ruff"], help="Run all formatters" }
+format-docs = { cmd = "pydocstringformatter  src/xt_st_common", help="Run docs formatter and apply fixes"}
+format = { sequence=["format-docs", "format-black", "format-ruff"], help="Run all formatters" }
+test-deps-up = { cmd="docker-compose -f test/docker-compose.yml up  -d"}
+test-deps-down = { cmd="docker-compose -f test/docker-compose.yml down "}
+_test = { cmd="pytest --cov-report term-missing --cov=src/xt_st_common", help="Run unit tests, won't work if docker is not up"}
+_wait = { cmd="sleep 3"}
+test = { sequence=["test-deps-up", "_wait", "_test", "test-deps-down"], ignore_fail="return_non_zero", help="Run all tests" }
+
 
 [tool.poetry.dependencies]
 python = ">3.9.7, <4.0"
 streamlit = ">=1.23.1"
 pydantic = ">=1.10.7"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 streamlit-js-eval = "^0.1.5"
@@ -36,23 +43,32 @@
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pytest-cov = "^4.0.0"
 ruff = "^0.0.262"
 pytest-mock = "^3.10.0"
 black = "^23.3.0"
 poethepoet = "^0.20.0"
 python-dotenv = "^1.0.0"
+pydocstringformatter = "^0.7.3"
 
 [tool.poetry.extras]
 databases = ["pymongo", "pymongo-auth-aws", "botocore"]
 storage = ["minio"]
 
 [tool.black]
 line-length = 120
 target-version = ['py310']
 
+[tool.pydocstringformatter]
+write = true
+max-line-length = 120
+strip-whitespaces = true
+split-summary-body = false
+numpydoc-section-hyphen-length = false
+linewrap-full-docstring = true
+
 [tool.ruff]
 ignore = [
     # zip=strict only valid for py3.10+
     "B905",
     "B008",
     "D",
 ]
```

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.9.1/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.9.1/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.8.4/src/xt_st_common/components.py` & `xt_st_common-0.9.1/src/xt_st_common/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 def page_header(
     page_title: str | None = None,
     page_logo: str | None = None,
     page_logo_width: int = 250,
     logout_url: str | None = None,
 ):
-    """
-    Display the page header including Title, Logo, and optional Logout button
-    """
+    """Display the page header including Title, Logo, and optional Logout button."""
     base_url = settings.STREAMLIT_SERVER_BASE_URL_PATH
     script_frame = st.empty()
     if logout_url is not None:
         # Load the css/icons for the button
         st.markdown(
             """
             <style scoped type="text/css">
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/config.py` & `xt_st_common-0.9.1/src/xt_st_common/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,57 +14,58 @@
 
 
 class StreamlitBaseSettings(BaseSettings):
     SIGNOUT_URL: Optional[str] = None
     CURRENT_PACKAGE = __name__.split(".")[0]
     BASE_PATH: str = str(Path(PathFinder().find_spec(CURRENT_PACKAGE).origin).parent)  # type: ignore
     DATA_DIR: str = str(Path.cwd() / "appdata")
-    """Root directory for storing app data"""
+    DOCS_DIR: str = str(Path.cwd() / "docs")
+    """Root directory for storing app data."""
 
     ###############
     # Storage Vars
     ###############
     STORAGE_TYPE: StorageType = StorageType.NONE
     BUCKET_NAME: Optional[str] = None
     BUCKET_PREFIX: Optional[str] = None
     MINIO_SECRET_KEY: Optional[SecretStr] = None
     MINIO_ACCESS_KEY: Optional[str] = None
     MINIO_ENDPOINT: Optional[str] = None
     MINIO_HTTPS: bool = True
 
     APP_NAME: str = "my_app"
-    """Name of the app that be tagged in the DB"""
-    APP_TAG_TEXT: str = "Development"
-    """text that will appear next the application logo"""
+    """Name of the app that be tagged in the DB."""
+    APP_TAG_TEXT: str = "Dev"
+    """Text that will appear next the application logo."""
     APP_TAG_BACKGROUND: Color = Color("#00a9ce")
-    """background colour of the APP_TAG_TEXT"""
+    """Background colour of the APP_TAG_TEXT."""
     APP_GET_HELP: str = None
-    """Link to "Get Help" in streamlit hamburger menu (menu item is hidden if set to None)"""
+    """Link to "Get Help" in streamlit hamburger menu (menu item is hidden if set to None)."""
     APP_REPORT_BUG: str = None
-    """Link to "Report a Bug" in streamlit hamburger menu (menu item is hidden if set to None)"""
+    """Link to "Report a Bug" in streamlit hamburger menu (menu item is hidden if set to None)."""
     APP_ABOUT: str = None
-    """Markdown Text to show in streamlit hamburger menu (shows streamlit default if set to None)"""
+    """Markdown Text to show in streamlit hamburger menu (shows streamlit default if set to None)."""
     DEBUG: bool = False
-    """Enable debug information in the app"""
+    """Enable debug information in the app."""
     DEBUG_MOCK_SESSION: bool = False
-    """Mock the session headers returned when deployed to AWS"""
+    """Mock the session headers returned when deployed to AWS."""
     USE_COGNITO: bool = False
-    """Use AWS Cognito for Auth"""
+    """Use AWS Cognito for Auth."""
     COGNITO_COOKIE: str = "AWSELBAuthSessionCookie"
-    """If set cookies with this prefix will be deleted on signout"""
+    """If set cookies with this prefix will be deleted on signout."""
     COGNITO_GROUPS: str = "ap-southeast-2_lC6GUKOej_CSIRO-EASI"
-    """One of these comma separated groups must be present in the user's `cognito:groups`"""
+    """One of these comma separated groups must be present in the user's `cognito:groups`."""
     NO_ACCESS_MSG: str = "Error: You do not have permission to use this app."
-    """Error message displayed when a user doesn't have permission to use the app"""
+    """Error message displayed when a user doesn't have permission to use the app."""
     STREAMLIT_SERVER_BASE_URL_PATH: str = ""
-    """The base path for the URL where Streamlit should be served from"""
+    """The base path for the URL where Streamlit should be served from."""
     MONGO_CONNECTION_STRING: str = ""
-    """Mongo DB connection string"""
+    """Mongo DB connection string."""
     DATABASE_NAME: str = ""
-    """Mongo DB Database Name"""
+    """Mongo DB Database Name."""
     TIMEZONE: str = "Australia/Perth"
-    """Default timezone used within the app"""
+    """Default timezone used within the app."""
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         case_sensitive = True
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/database.py` & `xt_st_common-0.9.1/src/xt_st_common/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 
 
 @st.cache_data(ttl=30)
 def get_projects(include_public=False, other_apps=True, shared_project=True, cache_id=None) -> List[Project]:
     current_user = get_user_email()
     or_query = {
         "$or": [
-            {"owner": {"$regex": current_user, "$options": "i"}},
+            {"owner": {"$regex": f"^{current_user}$", "$options": "i"}},
         ]
     }
     if include_public:
         or_query["$or"].append({"public": True})
     if shared_project:
-        or_query["$or"].append({"users": {"$elemMatch": {"$regex": current_user, "$options": "i"}}}),
+        or_query["$or"].append({"users": {"$elemMatch": {"$regex": f"^{current_user}$", "$options": "i"}}}),
 
     if len(or_query["$or"]) == 1:
         or_query = or_query["$or"][0]
 
     query = or_query if other_apps else {"$and": [{"application": f"{settings.APP_NAME}"}, or_query]}
     return [Project(**item) for item in get_collection().find(query)]
 
@@ -62,23 +62,23 @@
     return get_collection().count_documents({"_id": ObjectId(project_id)}) > 0
 
 
 @st.cache_data(ttl=30)
 def project_duplicate_exists(name: str, owner: str, project_id: Optional[str] = None, cache_id=None) -> bool:
     return (
         get_collection().count_documents(
-            {"_id": {"$ne": ObjectId(project_id)}, "name": name, "owner": {"$regex": owner, "$options": "i"}}
+            {"_id": {"$ne": ObjectId(project_id)}, "name": name, "owner": {"$regex": f"^{owner}$", "$options": "i"}}
         )
         > 0
     )
 
 
 @st.cache_data(ttl=30)
 def get_owned_projects(owner: str, cache_id=None) -> List[Project]:
-    return [Project(**item) for item in get_collection().find({"owner": {"$regex": owner, "$options": "i"}})]
+    return [Project(**item) for item in get_collection().find({"owner": {"$regex": f"^{owner}$", "$options": "i"}})]
 
 
 def reset_project_cache():
     st.session_state.project_cache = random.random()
 
 
 def get_project_cache():
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.9.1/src/xt_st_common/fs_upload_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" An upload page which uses the server filesystem for storage """
+"""An upload page which uses the server filesystem for storage."""
 import os
 from datetime import datetime
 from io import BytesIO
 from pathlib import Path
 from shutil import rmtree
 from typing import Iterable, List, Union
 from zipfile import ZIP_DEFLATED, ZipFile
@@ -13,17 +13,15 @@
 
 from xt_st_common.config import StreamlitBaseSettings
 
 settings = StreamlitBaseSettings()
 
 
 def list_directory(path: str, include_empty=True) -> list[str]:
-    """
-    Return a list of all the files in a directory.
-    """
+    """Return a list of all the files in a directory."""
     files = []
     for root, directories, filenames in os.walk(path):
         relative_root = root.replace(path, "")
 
         # Collect empty directories separately otherwise they never appear in the list
         if include_empty:
             for d in directories:
@@ -34,17 +32,15 @@
         # Collect files
         for filename in filenames:
             files.append(Path(relative_root) / filename)
     return files
 
 
 def create_file_tree(files: Iterable[str]) -> list[dict[str, str]]:
-    """
-    Using a list of file paths return a tree structure compatible with `streamlit_tree_select`.
-    """
+    """Using a list of file paths return a tree structure compatible with `streamlit_tree_select`."""
     file_tree = []
     files = sorted(files)
     for file in files:
         parts = str(file).split(os.sep)
         current_level = file_tree
         for i, part in enumerate(parts):
             existing = [node for node in current_level if node["label"] == part]
@@ -58,43 +54,41 @@
                 current_level.append(new_node)
                 if i != len(parts) - 1:
                     current_level = new_node.setdefault("children", [])
     return file_tree
 
 
 def _is_child_path(child_path, parent_path):
-    """
-    Returns `True` if the `child_path` is inside the `parent_path`.
-    """
+    """Returns `True` if the `child_path` is inside the `parent_path`."""
     # make both absolute
     parent_path = os.path.realpath(parent_path) + os.sep
     child_path = os.path.realpath(child_path)
 
     # return true, if the common prefix of both is equal to parent_path
     # e.g. /a/b/c/d.rst and directory is /a/b, the common prefix is /a/b
     return os.path.commonprefix([child_path, parent_path]) == parent_path
 
 
 def _prepare_download(files: List[str], root_dir: str = "") -> BytesIO:
-    """
-    Prepare zip file for download
-    """
+    """Prepare zip file for download."""
     mem_zip = BytesIO()
     with ZipFile(mem_zip, "w") as zf:
         for file in files:
             fpath = Path(root_dir + os.sep + file)
             if fpath.is_dir():
                 continue
             zf.write(str(fpath), arcname=file, compress_type=ZIP_DEFLATED)
     return mem_zip
 
 
 def _delete_files(files: List[str], root_dir: str = "") -> None:
     """
-    Delete the list of files. The root directory of a list of
+    Delete the list of files.
+
+    The root directory of a list of
     relative paths can be passed using `root_dir`.
     """
     dir_list = []
     for path in files:
         fpath = Path(root_dir + os.sep + path)
 
         # If you're deleting the root directory just recreate it rather than
@@ -123,15 +117,15 @@
         st.session_state["dir_list"] = dir_list
     for path in dir_list:
         Path.rmdir(path)
 
 
 def upload_page(data_dir: str, accepted_ft: Union[None, str, List[str]] = None, dl_prefix: str = "data"):
     """
-    Render the upload page which uses the servers local filesystem for storage
+    Render the upload page which uses the servers local filesystem for storage.
 
     ### Parameters
         data_dir: str
             directory to store data in on the server
 
         accepted_ft: str or list of str or None
             Accepted filetypes for upload (passed to `st.file_uploader()`)
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/project_components.py` & `xt_st_common-0.9.1/src/xt_st_common/project_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 REPLACE_FILE_HELP_TXT = (
     "The new file can have a different name but must have the same extension."
     "Warning: Uploading a new file that is significantly different to the original "
     "can have catastrophic results."
 )
 
+FOLDER_SHARED_KEY = "project_folder_select"
+PROJECT_SHARED_KEY = "project_select"
+
 
 def has_project_write_access(project: Project):
     return project.owner.lower() == get_user_email().lower() or get_user_email().lower() in (
         user.lower() for user in project.users
     )
 
 
@@ -65,14 +68,18 @@
     if project is None:
         return None
     if not isinstance(project, Project):
         raise ValueError("Selected project is not the correct type")
     return project
 
 
+def get_selected_folder() -> str:
+    return get_state("project_folder_select", "")
+
+
 def get_selected_project_or_error() -> Project:
     project = get_selected_project()
     if project is None:
         raise ValueError("No project was selected")
     return project
 
 
@@ -229,15 +236,15 @@
         ProjectState.PROJECT_SUCCESS_MESSAGE,
         f"Project **'{name}'** has been {message_verb}.",
     )
     return
 
 
 def project_form(project: Optional[Project] = None):
-    """A form that allows for creating an updating projects
+    """A form that allows for creating an updating projects.
 
     Parameters
     ----------
     project : Optional[Project], optional
         _description_, by default None
     """
     is_proj = project is not None
@@ -323,14 +330,58 @@
 
     set_state(
         ProjectState.FILE_SUCCESS_MESSAGE,
         f"File **'{selected_file.name}'** was succesfully renamed to **'{rename_string}'**",
     )
 
 
+def copy_file_to_project(selected_file: FileRef, new_project: Project):
+    current_project: Project = st.session_state["selected_project"]
+
+    if not has_project_write_access(new_project):
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            f"You don't have write access to project: {new_project.name}",
+        )
+        return
+
+    if current_project.name in selected_file.get_prefix():
+        new_path = f"{selected_file.get_prefix().replace(current_project.name, new_project.name).replace(str(current_project.id), str(new_project.id))}{selected_file.get_suffix()}"
+    else:
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            "Cannot copy file. File does not exist in current project",
+        )
+        return
+
+    if selected_file.path == new_path:
+        set_state(
+            ProjectState.FILE_WARNING_MESSAGE,
+            "Cannot copy file. New path is the same as the current path.",
+        )
+        return
+
+    new_file_ref = new_project.copy_file_to_path(selected_file, new_path)
+
+    # if there are user folders included with the new path, add them to the project as well
+    new_folder_message = ""
+    folders_string = new_file_ref.get_user_folders()
+    if folders_string != "":
+        new_folder_count = new_project.add_folders(folders_string)
+        if new_folder_count > 0:
+            new_folder_message = f"**{new_folder_count}** folders were added."
+
+    save_project(new_project)
+
+    set_state(
+        ProjectState.FILE_SUCCESS_MESSAGE,
+        f"File **'{selected_file.name}'** was succesfully copied to **'{new_project.name}'**. " + new_folder_message,
+    )
+
+
 @st.cache_data(ttl=300)
 def get_df_preview(path: str, ext: Optional[str], num_rows=25):
     # if filepath.suffix == ".zip":
     #     frame = get_gdf_from_file(filepath)
     #     return frame.iloc[:num_rows, :-1]
     if ext == ".csv":
         file = storage_client().get_file(path)
@@ -352,15 +403,20 @@
 
 
 def _state_name(project_id: str, folder: str) -> str:
     return f"{project_id}-{folder}_fs"
 
 
 @st.cache_data(ttl=15)
-def get_proj_options(include_public: bool = False, other_apps: bool = True, shared_project: bool = True, cache_id=None):
+def get_proj_options(
+    include_public: bool = False,
+    other_apps: bool = True,
+    shared_project: bool = True,
+    cache_id=None,
+):
     selected_project = get_selected_project()
     projects = get_projects(include_public, other_apps, shared_project, get_project_cache())
     sel_idx = 0
     options = {}
     for idx, proj in enumerate(projects):
         if selected_project and proj.id == selected_project.id:
             sel_idx = idx
@@ -388,84 +444,83 @@
     with st.expander("Project Filters"):
         st.checkbox("Public projects", value=False, key="include_public_projects")
         st.checkbox("Other Apps", value=True, key="include_other_apps")
         st.checkbox("Shared projects", value=True, key="include_shared_projects")
 
 
 def project_selector(
-    header_text: Optional[str] = "Projects",
     select_box_label="Select Project",
     null_option="-- Select Project --",
     st_context=st.sidebar,
     on_select_change=None,
     enable_filters=True,
+    set_selected=True,
+    prefix="",
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ) -> Tuple[Union["Project", None], List["Project"]]:
-    """UI to select and create projects
-    Args:
-        root_path (Path): The root Path to where the project folders live
-    """
+    """UI to select and create projects."""
     selected_project = None
 
     if render_layout == "horizontal":
         layout_container1, layout_container2 = st_context.columns(2)
+        layout_container2.markdown("#")
     else:
         layout_container1 = st_context.container()
         layout_container2 = st_context.container()
 
-    if header_text is not None:
-        st_context.subheader(header_text)
     include_public = bool(get_state("include_public_projects", False))
     include_other_apps = bool(get_state("include_other_apps", False))
     include_shared_projects = bool(get_state("include_shared_projects", False))
 
     if enable_filters:
         with layout_container2:
             project_filters()
     options, projects, sel_idx = get_proj_options(
-        include_public, include_other_apps, include_shared_projects, cache_id=get_project_cache()
+        include_public,
+        include_other_apps,
+        include_shared_projects,
+        cache_id=get_project_cache(),
     )
     proj_options = {}
 
     # accomodate the null option if one is provided
     if null_option is not None:
         proj_options = {-1: null_option}
         sel_idx = sel_idx + 1
 
     if options is not None:
         proj_options = {**proj_options, **options}
 
     if len(proj_options) > 0:
         proj_idx = layout_container1.selectbox(
             select_box_label,
-            key="project_select",
+            key=f"{prefix}{PROJECT_SHARED_KEY}",
             index=sel_idx,
             on_change=on_select_change,
             options=proj_options.keys(),
             format_func=lambda x: proj_options[x],
         )
 
         selected_project = None
         if proj_idx is not None:
             selected_project = projects[proj_idx] if proj_idx != -1 else None
-            set_selected_project(selected_project)
+            if set_selected:
+                set_selected_project(selected_project)
 
     else:
         st_context.warning("No projects were found")
 
     return selected_project, projects
 
 
 def load_csv(
     data_file,
     st_context=st,
 ):
-    """
-    Takes a csv file and loads it into session_state
-    """
+    """Takes a csv file and loads it into session_state."""
 
     try:
         encoding, dialect = get_encoding_and_dialect(data_file)
         raw_df = pd.read_csv(
             data_file,
             header=None,
             skip_blank_lines=True,
@@ -518,22 +573,22 @@
     raw_df = raw_df.drop(labels=skip_rows)
     raw_df = raw_df.reset_index(drop=True)
 
     return raw_df, units
 
 
 def _update_key(prefix: str = "", replace: bool = False):
-    """Hack to clear file upload after save by updating the key"""
+    """Hack to clear file upload after save by updating the key."""
     value = prefix + str(randint(1000, 100000000))
     set_state(f"{prefix}file_manager_key{'_replace' if replace else ''}", value)
     return str(value)
 
 
 def _get_key(prefix: str = "", replace: bool = False):
-    """Hack to clear file upload after save by updating the key"""
+    """Hack to clear file upload after save by updating the key."""
     key = get_state(f"{prefix}file_manager_key{'_replace' if replace else ''}", None)
     return _update_key(prefix, replace) if key is None else key
 
 
 def file_manager(
     project: Project,
     types: List[str],
@@ -541,16 +596,19 @@
     upload_label: str = "Upload file(s) to selected folder",
     help_text: Optional[str] = None,
     allow_upload=True,
     allow_multiple_uploads=False,
     allow_delete=True,
     allow_replace=True,
     allow_file_rename=False,
+    allow_file_move=False,
+    allow_file_copy_to_project=False,
     allow_folder_add=False,
     key_prefix: str = "",
+    allow_file_select=True,
     expand_file_actions=False,
     expand_folder_actions=True,
     folder_select_text="Select Borehole/Run",
     auto_parse_csv=True,
     render_layout: Literal["vertical", "horizontal", "compact"] = "vertical",
 ):
     file_delete_confirm = get_state(ProjectState.FILE_DELETE_CONFIRM)
@@ -587,18 +645,19 @@
     else:
         layout_container1 = st_context.container()
         layout_container2 = st_context.container()
 
     folders_dict = project.get_folders_map()
     folder = layout_container1.selectbox(
         folder_select_text,
+        key=FOLDER_SHARED_KEY,
         options=folders_dict.keys(),
         format_func=lambda x: folders_dict[x],
     )
-    path = project.get_folder_path(folder) if folder else None
+    path = project.get_folder_path(folder) if folder is not None else None
     if path is not None and folder is not None:
         row = layout_container1.expander("Folder Actions", expanded=expand_folder_actions)
 
         state = _state_name(str(project.id), folder)
         if state not in st.session_state:
             st.session_state[state] = 0
 
@@ -692,15 +751,14 @@
                 )
                 st.experimental_rerun()
 
         if render_layout == "compact":
             folder_add_sub_text_container = row.container()
             folder_add_sub_button_container = row.container()
             folder_delete_container = row.container()
-
         else:
             (
                 folder_add_sub_text_container,
                 folder_add_sub_button_container,
                 folder_delete_container,
             ) = row.columns([4, 1, 1])
             folder_add_sub_button_container.markdown("#")
@@ -724,132 +782,231 @@
         if allow_delete and folder != "/":
             folder_delete_container.button(
                 "Delete Selected",
                 key=f"{key_prefix}folder_delete_btn",
                 on_click=submit_delete_folder,
                 args=(folder,),
             )
+        if allow_file_select:
+            files = project.get_files_in_folder(folder, include_subfolders=False)
+            if files is not None and len(files) > 0:
+                selected_key = layout_container2.selectbox(
+                    "Select File",
+                    options=files.keys(),
+                    key=f"{key_prefix}file_manager_file_select",
+                )
+                selected_file = files[selected_key] if selected_key in files else None
+                if selected_file is not None and selected_key is not None:
+                    row = layout_container2.expander("File Actions", expanded=expand_file_actions)
+                    if len(selected_key) > 30:
+                        row.caption(selected_key)
+
+                    if render_layout == "compact":
+                        file_preview_container = row.container()
+                        file_prepare_container, file_download_container = row.columns([5, 3])
+                        file_download_container = row.container()
+                        file_rename_button_container = row.container()
+                        file_delete_container = row.container()
+                        if allow_file_copy_to_project:
+                            file_copy_to_project_select_container = row.container()
+                            file_copy_to_project_button_container = row.container()
+
+                    else:
+                        (
+                            file_preview_container,
+                            file_prepare_container,
+                            file_download_container,
+                        ) = row.columns([1, 1, 1])
+                        (
+                            file_rename_text_container,
+                            file_rename_button_container,
+                            file_delete_container,
+                        ) = row.columns([2, 1, 1])
+                        file_rename_button_container.markdown("#")
+                        file_delete_container.markdown("#")
+
+                        if allow_file_copy_to_project:
+                            (
+                                file_copy_to_project_select_container,
+                                file_copy_to_project_button_container,
+                                _,
+                            ) = row.columns([2, 1, 1])
+                            file_copy_to_project_button_container.markdown("#")
+
+                    # options = []
+                    if allow_delete:
+                        file_delete_container.button(
+                            "Delete Selected",
+                            key=f"{key_prefix}file_delete_btn",
+                            on_click=submit_delete_file,
+                            args=(selected_file,),
+                        )
+                    if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather", ".xlsx")):
+                        preview_frame = file_preview_container.button(
+                            "Preview Frame",
+                            key=f"{key_prefix}file_manager_preview_frame",
+                        )
+                        if preview_frame:
+                            with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
+                                st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
+                    if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
+                        preview_frame := file_preview_container.button(
+                            "Preview File",
+                            key=f"{key_prefix}file_manager_preview_file",
+                        )
+                    ):
+                        with st.expander(f"**File Viewer:** {selected_file.name}", expanded=True):
+                            code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
+                            if code_format is None:
+                                st.write(get_string_preview(selected_file))
+                            else:
+                                st.code(
+                                    get_string_preview(selected_file),
+                                    language=code_format,
+                                )
+                    if file_prepare_container.checkbox(
+                        "Prepare Download",
+                        key=f"{key_prefix}file_manager_download_chbx",
+                    ):
+                        file_data = storage_client().get_file(selected_file.path)
+
+                        file_download_container.download_button(
+                            "Download",
+                            file_data,
+                            selected_file.name,
+                            key=f"{key_prefix}file_manager_download_button",
+                        )
+                    if allow_replace and (
+                        uploaded_replace_file := row.file_uploader(
+                            "Replace the selected file",
+                            key=_get_key(key_prefix, True),
+                            type=selected_file.get_ext(),
+                            help=REPLACE_FILE_HELP_TXT,
+                            accept_multiple_files=False,
+                        )
+                    ):
+                        project.add_replace_file_by_path(uploaded_replace_file, selected_file.path)
+                        save_project(project)
+                        uploaded_replace_file.close()
+                        _update_key(key_prefix, True)
+                        set_state(
+                            ProjectState.FILE_SUCCESS_MESSAGE,
+                            f"Contents of file: **'{selected_file.path}'** was succesfully replaced",
+                        )
+                        st.experimental_rerun()
+                    if allow_file_rename:
+                        file_rename_text_container.text_input(
+                            "Rename file as:",
+                            key="rename_project_file_name",
+                            help="Selected file will be renamed to this value when 'Rename Selected' is clicked",
+                            placeholder="New file name",
+                        )
+                        file_rename_button_container.button(
+                            label="Rename Selected",
+                            help="Rename File",
+                            on_click=rename_file,
+                            args=(selected_file,),
+                        )
+                    if allow_file_copy_to_project:
+                        copy_to_selected_project, projects = project_selector(
+                            select_box_label="Copy file to project",
+                            st_context=file_copy_to_project_select_container,  # type: ignore
+                            null_option=None,
+                            enable_filters=False,
+                            set_selected=False,
+                            prefix="copy_to_project",
+                        )
 
-        files = project.get_files_in_folder(folder, include_subfolders=True)
-        if files is not None and len(files) > 0:
-            selected_key = layout_container2.selectbox(
-                "Select File",
-                options=files.keys(),
-                key=f"{key_prefix}file_manager_file_select",
-            )
-            selected_file = files[selected_key] if selected_key in files else None
-            if selected_file is not None and selected_key is not None:
-                row = layout_container2.expander("File Actions", expanded=expand_file_actions)
-                if len(selected_key) > 30:
-                    row.caption(selected_key)
-
-                if render_layout == "compact":
-                    file_preview_container = row.container()
-                    file_prepare_container, file_download_container = row.columns([5, 3])
-                    file_download_container = row.container()
-                    file_rename_button_container = row.container()
-                    file_delete_container = row.container()
-
-                else:
-                    (
-                        file_preview_container,
-                        file_prepare_container,
-                        file_download_container,
-                    ) = row.columns([1, 1, 1])
-                    (
-                        file_rename_text_container,
-                        file_rename_button_container,
-                        file_delete_container,
-                    ) = row.columns([2, 1, 1])
-                    file_rename_button_container.markdown("#")
-                    file_delete_container.markdown("#")
-
-                # options = []
-                if allow_delete:
-                    file_delete_container.button(
-                        "Delete Selected",
-                        key=f"{key_prefix}file_delete_btn",
-                        on_click=submit_delete_file,
-                        args=(selected_file,),
-                    )
-                if selected_key.lower().endswith((".zip", ".csv", ".geojson", ".gpkg", ".feather", ".xlsx")):
-                    preview_frame = file_preview_container.button(
-                        "Preview Frame",
-                        key=f"{key_prefix}file_manager_preview_frame",
-                    )
-                    if preview_frame:
-                        with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
-                            st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
-                if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
-                    preview_frame := file_preview_container.button(
-                        "Preview File",
-                        key=f"{key_prefix}file_manager_preview_file",
-                    )
-                ):
-                    with st.expander(f"**File Viewer:** {selected_file.name}", expanded=True):
-                        code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
-                        if code_format is None:
-                            st.write(get_string_preview(selected_file))
-                        else:
-                            st.code(
-                                get_string_preview(selected_file),
-                                language=code_format,
-                            )
-                if file_prepare_container.checkbox(
-                    "Prepare Download",
-                    key=f"{key_prefix}file_manager_download_chbx",
-                ):
-                    file_data = storage_client().get_file(selected_file.path)
-
-                    file_download_container.download_button(
-                        "Download",
-                        file_data,
-                        selected_file.name,
-                        key=f"{key_prefix}file_manager_download_button",
-                    )
-                if allow_replace and (
-                    uploaded_replace_file := row.file_uploader(
-                        "Replace the selected file",
-                        key=_get_key(key_prefix, True),
-                        type=selected_file.get_ext(),
-                        help=REPLACE_FILE_HELP_TXT,
-                        accept_multiple_files=False,
-                    )
-                ):
-                    project.add_replace_file_by_path(uploaded_replace_file, selected_file.path)
-                    save_project(project)
-                    uploaded_replace_file.close()
-                    _update_key(key_prefix, True)
-                    set_state(
-                        ProjectState.FILE_SUCCESS_MESSAGE,
-                        f"Contents of file: **'{selected_file.path}'** was succesfully replaced",
-                    )
-                    st.experimental_rerun()
-                if allow_file_rename:
-                    file_rename_text_container.text_input(
-                        "Rename file as:",
-                        key="rename_project_file_name",
-                        help="Selected file will be renamed to this value when 'Rename Selected' is clicked",
-                        placeholder="New file name",
-                    )
-                    file_rename_button_container.button(
-                        label="Rename Selected",
-                        help="Rename File",
-                        on_click=rename_file,
-                        args=(selected_file,),
-                    )
+                        file_copy_to_project_button_container.button(
+                            label="Copy to project",
+                            help="Rename File",
+                            on_click=copy_file_to_project,
+                            args=(selected_file, copy_to_selected_project),
+                        )
 
-        else:
-            layout_container2.markdown("##")
-            layout_container2.info("No files in selected folder")
+            else:
+                layout_container2.markdown("##")
+                layout_container2.info("No files in selected folder")
 
         state_reset()
     return path, folder
 
 
+@st.cache_data(ttl=300)
+def get_file_cached(file_path: str):
+    return storage_client().get_file(file_path)
+
+
+def file_selector(
+    project: Project,
+    folder: Optional[str] = "",
+    select_folder_label: str = "Select Folder",
+    select_file_label: str = "Select File",
+    extensions: Optional[List[str]] = None,
+    state_key: Optional[str] = None,
+    no_file_warning: str = "No files were found with the correct extension.",
+):
+    """
+    Widget to Select and load a file from a selected project.
+
+    Parameters
+    ----------
+    project : Project
+        _description_
+    folder : Optional[str], optional
+        _description_, by default "/"
+    select_folder_label : str, optional
+        _description_, by default "Select Folder"
+    select_file_label : str, optional
+        _description_, by default "Select File"
+    extensions : Optional[List[str]], optional
+        _description_, by default None
+    state_key : Optional[str], optional
+        _description_, by default None
+    no_file_warning : str, optional
+        _description_, by default "No files were found with the correct extension."
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    if folder is None:
+        folders_dict = project.get_folders_map()
+        folder = st.selectbox(
+            select_folder_label,
+            key=FOLDER_SHARED_KEY,
+            options=folders_dict.keys(),
+            format_func=lambda x: folders_dict[x],
+        )
+
+    files = project.get_files_in_folder(folder, extensions=extensions, include_subfolders=True)
+    if files is not None and len(files) > 0:
+        selected_key = st.selectbox(
+            select_file_label,
+            options=files.keys(),
+        )
+
+        file_ref = files.get(selected_key, None)
+
+        if file_ref is not None:
+            st.markdown("#")
+
+            if st.button("Load Selected File"):
+                file = get_file_cached(file_ref.path)
+                if state_key:
+                    set_state(state_key, file)
+                    set_state(state_key + "_ref", file_ref)
+                st.success(f"File {file_ref.name} loaded successfully.")
+                return file, file_ref
+    else:
+        st.warning(no_file_warning)
+    return None, None
+
+
 def get_projects_data(projects):
     selected_project = get_selected_project()
     proj_data = []
     for proj in projects:
         proj_dict = proj.dict(exclude={"files", "folders"})
         # proj_dict = proj.dict(exclude={"files", "folders", "id"})
 
@@ -933,15 +1090,14 @@
         save_container, delete_container = st_context.columns([1, 1])
 
     with filter_container:
         project_filters()
 
     with select_container:
         project, projects = project_selector(
-            header_text=None,
             null_option=null_option,
             select_box_label="Select Project",
             st_context=select_container,  # type: ignore
             on_select_change=on_project_select_change,
             enable_filters=False,
         )
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/project_models.py` & `xt_st_common-0.9.1/src/xt_st_common/project_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     FILE_TO_DELETE = "file_to_delete"
     FILE_SUCCESS_MESSAGE = "file_success_message"
     FILE_WARNING_MESSAGE = "file_warning_message"
 
     # FILE_MANAGER_UPLOAD = "file_manager_upload_file"
     FILE_MANAGER_REPLACE_FILE = "file_manager_replace_file"
 
+    def __str__(self):
+        return str(self.value)
+
 
 class Project(BaseModel):
     id: Optional[PyObjectId] = Field(default_factory=PyObjectId, alias="_id")  # noqa: A003
     name: str
     description: str = ""
     public: bool = False
     application: str = settings.APP_NAME
@@ -61,37 +64,80 @@
     owner: str = ""
     users: List[str] = []  # Users with access to this project
 
     def get_users_string(self):
         return ",".join(self.users)
 
     def get_folders_map(self):
-        fol_dict = {"/": "Project Root"}
+        fol_dict = {"": "Project Root"}
         for folder in self.folders:
             parts = folder.strip("/").split("/")
             fol_dict[folder] = " - ".join(parts)
         return fol_dict
 
     def get_folder_path(self, folder):
         return f"{str(self.id)}/{self.name}/{folder}".strip("/")
 
-    def get_files_in_folder(self, folder: str, include_subfolders=True, extensions=None, null_option=None):
+    def get_files_in_folder(
+        self,
+        folder: str,
+        include_subfolders: bool = True,
+        extensions: Optional[List[str]] = None,
+        null_option: Optional[str] = None,
+    ):
+        """
+        _summary_.
+
+        Parameters
+        ----------
+        folder : str
+            The folder to search, set to '' to search the root folder.
+        include_subfolders : bool, optional
+            If true will find all files in subfolders, if false will only search the specified folder, by default True
+        extensions : List[str], optional
+            Extensions to match on, MUST BE LOWERCASE without a '.' use None to not filter on extensions,
+            by default None
+        null_option : _type_, optional
+            Will add a default 'None' item to the list if None no default item will be added, by default None
+
+        Returns
+        -------
+        _type_
+            _description_
+        """
         _files: Dict[str, Union[None, FileRef]] = {} if null_option is None else {null_option: None}
 
         path = self.get_folder_path(folder)
         for file in self.files:
             if path in file.path:
                 file_path = file.path.removeprefix(path).strip("/")
                 if (include_subfolders or file_path.find("/") <= 0) and (
-                    extensions is None or str(Path(file.name).suffix.lower()) in extensions
+                    extensions is None or str(Path(file.name).suffix).strip(".").lower() in extensions
                 ):
                     _files[file_path] = file
 
         return _files
 
+    def get_subfolders(
+        self,
+        folder: str,
+    ) -> list:
+        """
+        Get all subfolders of the search folder.
+
+        Args:
+            folder (str): The name of the folder to search for subfolders
+
+        Returns:
+            list[str]: A list of sub folder strings
+        """
+
+        # when split on the folder name, a subfolder will have "" as the first split entry.
+        return [sub for sub in self.folders if sub.split(f"{folder}/")[0] == ""]
+
     def populate_node(self, _dict, part, parts):
         if part not in _dict:
             _dict[part] = {}
 
         if parts:
             self.populate_node(_dict[part], parts[0], parts[1:])
 
@@ -135,30 +181,73 @@
         return nodes
 
     def add_replace_file(self, data_file, folder: str, filename: str, content_type=None) -> FileRef:
         path = f"{self.get_folder_path(folder)}/{filename}".strip("/")
         return self.add_replace_file_by_path(data_file, path, content_type=content_type)
 
     def add_replace_file_by_path(self, data_file, path: str, content_type=None) -> FileRef:
-        file_ref = storage_client().write_file(path, data_file, content_type)
+        try:
+            file_ref = storage_client().write_file(path, data_file, content_type)
+            replaced = False
+            for idx, file in enumerate(self.files):
+                if file.path == path:
+                    self.files[idx] = file_ref
+                    replaced = True
+                    break
+            if not replaced:
+                self.files.append(file_ref)
+            return file_ref
+        except Exception as err:
+            logging.error(err)
+            raise err
+
+    def move_file_to_path(self, file: FileRef, new_path: str) -> FileRef:
+        """
+        Move the file referenced by file_ref to the new_path
+
+        Args:
+            file_ref (FileRef): A file reference object for the existing file
+            new_path (str): The new path where the file to be moved to
+
+        Returns:
+            FileRef: The file reference for the newly moved file.
+        """
+        new_file_ref = storage_client().copy_file(
+            file.path,
+            new_path,
+            file.content_type,
+            file.size_bytes,
+            delete_original=True,
+        )
+        index = self.files.index(file)
+        self.files[index] = new_file_ref
+        return new_file_ref
+
+    def copy_file_to_path(self, file_ref: FileRef, new_path: str) -> FileRef:
+        """
+        Copy the file referenced by file_ref to the new_path
+
+        Args:
+            file_ref (FileRef): A file reference object for the existing file
+            new_path (str): The new path where the file to be copied to
+
+        Returns:
+            FileRef: The file reference for the newly copied file.
+        """
+        new_file_ref = storage_client().copy_file(
+            file_ref.path, new_path, file_ref.content_type, file_ref.size_bytes, delete_original=False
+        )
         replaced = False
         for idx, file in enumerate(self.files):
-            if file.path == path:
-                self.files[idx] = file_ref
+            if file.path == new_path:
+                self.files[idx] = new_file_ref
                 replaced = True
                 break
         if not replaced:
-            self.files.append(file_ref)
-
-        return file_ref
-
-    def move_file_to_path(self, file: FileRef, new_path: str) -> FileRef:
-        new_file_ref = storage_client().move_file(file.path, new_path, file.content_type, file.size_bytes)
-        index = self.files.index(file)
-        self.files[index] = new_file_ref
+            self.files.append(new_file_ref)
         return new_file_ref
 
     def delete_file(self, file: FileRef):
         storage_client().delete_file(file.path)
         try:
             self.files.remove(file)
         except ValueError:
@@ -167,29 +256,46 @@
     def add_folders(self, folders_string: str):
         folders = set(self.folders)
         new_folders = folders_string.split(",")
         count = 0
         for folder in new_folders:
             folder = folder.strip().replace(" ", "_").strip("/")
             folder_parts = folder.split("/")
+            # add each part
             for idx, part in enumerate(folder_parts):
-                if idx == 0:
-                    folders.add(f"{part}")
-                else:
-                    folders.add(f"{'/'.join(folder_parts[:idx+1])}")
-                count += 1
+                part_string = part if idx == 0 else f"{'/'.join(folder_parts[:idx + 1])}"
+
+                # only increment count if the part_string doesn't already exist in the folder list
+                if part_string not in folders:
+                    folders.add(part_string)
+                    count += 1
+
         try:
             self.folders = list(folders)
         except AttributeError:
             logging.warning("Weird odmatic error, attempting to ignore")
 
         return count
 
     def delete_folder(self, folder: str):
+        """
+        Recursively delete the files and sub folders of the provided folder name
+
+        Args:
+            folder (str): The name of the folder to be recursively deleted
+        """
         try:
+            sub_folders = self.get_subfolders(folder)
+
+            # recursively delete any sub folders first
+            for sub_folder in sub_folders:
+                # this "if" appears to be redundant but the sub-folder may already have been deleted in another recursion branch
+                if sub_folder in self.folders:
+                    self.delete_folder(sub_folder)
+
             folder_path = self.get_folder_path(folder)
             self.folders.remove(folder)
             for file in [x for x in self.files if folder_path in x.path]:
                 self.delete_file(file)
         except ValueError:
             logging.warning(f"Folder {folder} didn't exist and couldn't be deleted.")
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/session.py` & `xt_st_common-0.9.1/src/xt_st_common/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 from xt_st_common.config import StreamlitBaseSettings
 
 settings = StreamlitBaseSettings()
 
 
 def get_session_headers():
-    """
-    Returns the request headers for the current streamlit session
-    """
+    """Returns the request headers for the current streamlit session."""
     if settings.DEBUG and settings.DEBUG_MOCK_SESSION:
         headers = {
             "X-Forwarded-For": "130.116.147.135",
             "X-Forwarded-Proto": "https",
             "X-Forwarded-Port": "443",
             "Host": "fracg-ui.exploration.tools",
             "X-Amzn-Trace-Id": "Root=1-642250e6-3b44a7d41992a61831721a43",
@@ -40,29 +38,29 @@
         return headers
 
     return _get_websocket_headers()
 
 
 def decode_jwt(raw_jwt: str, algorithms: Optional[List[str]] = None, options=None) -> dict:
     """
-    Decode a JWT and return its values as a dictionary
+    Decode a JWT and return its values as a dictionary.
 
     `algorithms` defaults to `["ES256"]`
     `options` defaults to `{"verify_signature": False}`
     """
     if algorithms is None:
         algorithms = ["ES256"]
     if options is None:
         options = {"verify_signature": False}
     return jwt.decode(raw_jwt, algorithms=algorithms, options=options)
 
 
 def get_user_id(allow_default=True):
     """
-    Returns the current user id
+    Returns the current user id.
 
     allow_default:
         return "default-user" if user not found
     """
 
     headers = get_session_headers()
     if headers is not None:
@@ -75,50 +73,42 @@
     if allow_default:
         return "default-user"
 
     raise KeyError("X-Auth-Request-User not found in headers")
 
 
 def get_user_email(allow_default=True):
-    """
-    Return the user's email address from headers, otherwise return the string "default-user"
-    """
+    """Return the user's email address from headers, otherwise return the string "default-user"."""
     headers = get_session_headers()
     if headers is not None and "X-Goog-Authenticated-User-Email" in headers:
         return headers["X-Goog-Authenticated-User-Email"].split(":")[1]
     if headers is not None and "X-Amzn-Oidc-Data" in headers:
         return decode_jwt(headers["X-Amzn-Oidc-Data"])["email"]
     if allow_default:
         return "default-user@exploration.tools"
 
     raise KeyError("X-Goog-Authenticated-User-Email not found in headers")
 
 
 def get_oidc_groups() -> List[str]:
-    """
-    Attempts to retrieve the OIDC groups from the headers (e.g. cognito:groups)
-    """
+    """Attempts to retrieve the OIDC groups from the headers (e.g. cognito:groups)."""
     headers = get_session_headers()
     if headers is None or "X-Amzn-Oidc-Accesstoken" not in headers:
         raise KeyError("X-Amzn-Oidc-Accesstoken not found in headers")
     access_tok = decode_jwt(headers["X-Amzn-Oidc-Accesstoken"])
     return access_tok.get("cognito:groups", [])
 
 
 def get_user_name(allow_default=True):
-    """
-    Return user's name from headers, otherwise return the string "default-user"
-    """
+    """Return user's name from headers, otherwise return the string "default-user"."""
     headers = get_session_headers()
     if headers is not None and "X-Amzn-Oidc-Data" in headers:
         return decode_jwt(headers["X-Amzn-Oidc-Data"])["name"]
     if allow_default:
         return "default-user"
 
     raise KeyError("X-Amzn-Oidc-Data not found in headers")
 
 
 def get_user_path() -> str:
-    """
-    Return path to local file storage for the user
-    """
+    """Return path to local file storage for the user."""
     return str(Path(settings.DATA_DIR) / get_user_email())
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/storage.py` & `xt_st_common-0.9.1/src/xt_st_common/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,30 @@
 
     def get_prefix(self):
         return self.path.rsplit("/", 1)[0]
 
     def get_folder(self):
         return self.path.rsplit("/", 2)[1]
 
+    def get_user_folders(self):
+        """Get all the folders between the project root and the filename.
+
+        Returns:
+            str: User folders separated by "/"
+        """
+        folders = self.path.split("/")
+
+        if len(folders) < 3:
+            return ""
+
+        return "/".join(folders[2:-1])
+
+    def get_suffix(self):
+        return self.path.split(self.get_prefix())[1]
+
     def get_ext(self):
         parts = self.name.rsplit(".", 1)
         return None if len(parts) <= 1 else f".{parts[-1]}"
 
 
 class StorageClient(ABC):
     @abstractmethod
@@ -64,15 +80,20 @@
         pass
 
     @abstractmethod
     def file_exists(self, file_path: str):
         pass
 
     @abstractmethod
-    def move_file(self, file_path: str, new_file_path: str):
+    def copy_file(
+        self,
+        file_path: str,
+        new_file_path: str,
+        delete_original: bool = False,
+    ):
         pass
 
 
 class MinioStorageClient(StorageClient):
     def __init__(
         self,
         bucket: str,
@@ -138,18 +159,30 @@
         # set MIME_TYPE for MSCL/GeoTek files
         if content_type is None and file_path.lower().endswith((".cal", ".out", ".raw", ".sbd", ".xrf")):
             content_type = "text/plain"
 
         obj = self.__client.put_object(self.__bucket, file_path, file_bytes, file_len, content_type=content_type)
         return self.object_to_file(obj, file_len, content_type)
 
-    def move_file(self, file_path: str, new_file_path: str, content_type, size_bytes: int) -> Optional[FileRef]:
+    def copy_file(
+        self,
+        file_path: str,
+        new_file_path: str,
+        content_type,
+        size_bytes: int,
+        delete_original: bool = False,
+    ) -> Optional[FileRef]:
         obj = self.__client.copy_object(self.__bucket, new_file_path, CopySource(self.__bucket, file_path))
-        self.delete_file(file_path)
-        return self.object_to_file(obj, file_length=size_bytes, content_type=content_type)
+
+        new_file_ref = self.object_to_file(obj, file_length=size_bytes, content_type=content_type)
+
+        if delete_original:
+            self.delete_file(file_path)
+
+        return new_file_ref
 
     def get_file(self, file_path: str):
         response_data = None
         try:
             response = self.__client.get_object(self.__bucket, file_path)
             # Read data from response.
             response_data = BytesIO(response.read())
```

### Comparing `xt_st_common-0.8.4/src/xt_st_common/utils.py` & `xt_st_common-0.9.1/src/xt_st_common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,26 +50,26 @@
     return [user.strip() for user in users_array]
 
 
 FILE_MARKER = "<files>"
 
 
 def attach(branch, trunk):
-    """
-    Insert a branch of directories on its trunk.
-    """
+    """Insert a branch of directories on its trunk."""
     parts = branch.split("/", 1)
     if len(parts) == 1:  # branch is a file
         trunk[FILE_MARKER].append(parts[0])
     else:
         node, others = parts
         if node not in trunk:
             trunk[node] = defaultdict(dict, ((FILE_MARKER, []),))
         attach(others, trunk[node])
 
 
 def get_state(state_name: Union[str, Enum], default: Optional[Any] = ""):
-    return st.session_state[str(state_name)] if str(state_name) in st.session_state else default
+    if str(state_name) not in st.session_state or st.session_state[str(state_name)] is None:
+        st.session_state[str(state_name)] = default
+    return st.session_state[str(state_name)]
 
 
 def set_state(state_name: Union[str, Enum], value: Any):
     st.session_state[str(state_name)] = value
```

### Comparing `xt_st_common-0.8.4/PKG-INFO` & `xt_st_common-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.8.4
+Version: 0.9.1
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.23.1)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.8.4
+# XT-STREAMLIT - 0.9.1
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

