# Comparing `tmp/harlequin-0.0.8.tar.gz` & `tmp/harlequin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.8.tar", max compression
+gzip compressed data, was "harlequin-0.0.9.tar", max compression
```

## Comparing `harlequin-0.0.8.tar` & `harlequin-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1068 2023-05-15 19:56:23.010672 harlequin-0.0.8/LICENSE
--rw-r--r--   0        0        0     2050 2023-05-15 19:56:23.010672 harlequin-0.0.8/README.md
--rw-r--r--   0        0        0     1460 2023-05-15 19:56:23.018673 harlequin-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/__main__.py
--rw-r--r--   0        0        0      336 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/cli.py
--rw-r--r--   0        0        0       53 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0     2647 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/app.css
--rw-r--r--   0        0        0     8813 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/app.py
--rw-r--r--   0        0        0      972 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/__init__.py
--rw-r--r--   0        0        0      913 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/code_editor.py
--rw-r--r--   0        0        0     1125 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/error_modal.py
--rw-r--r--   0        0        0      672 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/filename_modal.py
--rw-r--r--   0        0        0     3212 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/key_handlers.py
--rw-r--r--   0        0        0      665 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/messages.py
--rw-r--r--   0        0        0     2480 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/results_viewer.py
--rw-r--r--   0        0        0     3001 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/schema_viewer.py
--rw-r--r--   0        0        0    21184 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/textarea.py
--rw-r--r--   0        0        0      661 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/utils.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 harlequin-0.0.8/setup.py
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 harlequin-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-16 20:03:16.487594 harlequin-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1738 2023-05-16 20:03:16.487594 harlequin-0.0.9/README.md
+-rw-r--r--   0        0        0     1460 2023-05-16 20:03:16.491594 harlequin-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/__main__.py
+-rw-r--r--   0        0        0      336 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/cli.py
+-rw-r--r--   0        0        0       53 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     9766 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      972 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1125 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0     3212 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/key_handlers.py
+-rw-r--r--   0        0        0      665 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/messages.py
+-rw-r--r--   0        0        0     2480 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3001 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0    21184 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/components/textarea.py
+-rw-r--r--   0        0        0      661 2023-05-16 20:03:16.495594 harlequin-0.0.9/src/harlequin/tui/utils.py
+-rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 harlequin-0.0.9/setup.py
+-rw-r--r--   0        0        0     2452 1970-01-01 00:00:00.000000 harlequin-0.0.9/PKG-INFO
```

### Comparing `harlequin-0.0.8/LICENSE` & `harlequin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/README.md` & `harlequin-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -18,28 +18,14 @@
 > **Tip:**
 >
 > You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:
 > - `pipx run harlequin --help`
 > - `pipx run harlequin ./my.duckdb`
 
 
-## Running Harlequin in a Container
-
-Without a database file:
-
-```bash
-docker run ghcr.io/tconbeer/harlequin:latest
-```
-
-Mounting a database file `./foo.db` into the container's working directory, `/data`:
-
-```bash
-docker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db
-```
-
 ## Using Harlequin
 
 From any shell, to open a DuckDB database file:
 
 ```bash
 harlequin "path/to/duck.db"
 ```
```

### Comparing `harlequin-0.0.8/pyproject.toml` & `harlequin-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
```

### Comparing `harlequin-0.0.8/src/harlequin/tui/app.css` & `harlequin-0.0.9/src/harlequin/tui/app.css`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/app.py` & `harlequin-0.0.9/src/harlequin/tui/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,30 +139,55 @@
                 self.data = []
                 self.update_schema_data()
             else:  # blank query
                 pane.set_responsive(did_run=False)
                 pane.show_table()
                 self.data = []
 
-    def watch_relation(self, relation: Union[duckdb.DuckDBPyRelation, None]) -> None:
+    async def watch_relation(
+        self, relation: Union[duckdb.DuckDBPyRelation, None]
+    ) -> None:
         """
         Only runs for select statements, except when first mounted.
         """
         # invalidate results so watch_data runs even if the results are the same
         self.data = []
         if relation is not None:
-            table = self.query_one(ResultsViewer).get_table()
+            pane = self.query_one(ResultsViewer)
+            table = pane.get_table()
             short_types = [short_type(t) for t in relation.dtypes]
             table.add_columns(
                 *[
                     f"{name} [#888888]{type}[/]"
                     for name, type in zip(relation.columns, short_types)
                 ]
             )
-            self.fetch_relation_data(relation)
+            try:
+                worker = self.fetch_relation_data(relation)
+                await worker.wait()
+            except WorkerFailed as e:
+                self.push_screen(
+                    ErrorModal(
+                        title="DuckDB Error",
+                        header=("DuckDB raised an error when " "running your query:"),
+                        error=e.error,
+                    )
+                )
+                pane.show_table()
+            # Textual fails to catch some duckdb Errors,
+            # so we need this mostly- redundant block.
+            except duckdb.Error as e:
+                self.push_screen(
+                    ErrorModal(
+                        title="DuckDB Error",
+                        header=("DuckDB raised an error when " "running your query:"),
+                        error=e,
+                    )
+                )
+                pane.show_table()
 
     async def watch_data(self, data: List[Tuple]) -> None:
         if data:
             pane = self.query_one(ResultsViewer)
             pane.set_not_responsive(max_rows=self.MAX_RESULTS, total_rows=len(data))
             table = pane.get_table()
             for i, chunk in self.chunk(data[: self.MAX_RESULTS]):
@@ -183,15 +208,15 @@
             yield i, data[i * chunksize : (i + 1) * chunksize]
 
     @work(exclusive=True, exit_on_error=False)  # type: ignore
     def build_relation(self, query_text: str) -> Union[duckdb.DuckDBPyRelation, None]:
         relation = self.connection.sql(query_text)
         return relation
 
-    @work(exclusive=True)
+    @work(exclusive=True, exit_on_error=False)  # type: ignore
     def fetch_relation_data(self, relation: duckdb.DuckDBPyRelation) -> None:
         log(f"fetch_relation_data {hash(relation)}")
         data = relation.fetchall()
         log(f"fetch_relation_data FINISHED {hash(relation)}")
         worker = get_current_worker()
         if not worker.is_cancelled:
             self.call_from_thread(self.set_data, data)
```

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/__init__.py` & `harlequin-0.0.9/src/harlequin/tui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/code_editor.py` & `harlequin-0.0.9/src/harlequin/tui/components/code_editor.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/error_modal.py` & `harlequin-0.0.9/src/harlequin/tui/components/error_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/filename_modal.py` & `harlequin-0.0.9/src/harlequin/tui/components/filename_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/key_handlers.py` & `harlequin-0.0.9/src/harlequin/tui/components/key_handlers.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/messages.py` & `harlequin-0.0.9/src/harlequin/tui/components/messages.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/results_viewer.py` & `harlequin-0.0.9/src/harlequin/tui/components/results_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/schema_viewer.py` & `harlequin-0.0.9/src/harlequin/tui/components/schema_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/components/textarea.py` & `harlequin-0.0.9/src/harlequin/tui/components/textarea.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/src/harlequin/tui/utils.py` & `harlequin-0.0.9/src/harlequin/tui/utils.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.8/setup.py` & `harlequin-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'textual>=0.22.3,<0.25.0']
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A Text User Interface for DuckDB',
-    'long_description': '# harlequin\nA Terminal-based SQL IDE for DuckDB.\n\n![harlequin TUI](harlequinv004.gif)\n\n(A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin duck](harlequin.jpg)\n\n## Installing Harlequin\n\nAfter installing Python 3.8 or above, install Harlequin using `pip` or `pipx` with:\n\n```bash\npipx install harlequin\n```\n\n> **Tip:**\n>\n> You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:\n> - `pipx run harlequin --help`\n> - `pipx run harlequin ./my.duckdb`\n\n\n## Running Harlequin in a Container\n\nWithout a database file:\n\n```bash\ndocker run ghcr.io/tconbeer/harlequin:latest\n```\n\nMounting a database file `./foo.db` into the container\'s working directory, `/data`:\n\n```bash\ndocker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db\n```\n\n## Using Harlequin\n\nFrom any shell, to open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\n### Viewing the Schema of your Database\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar. You can use your mouse or the arrow keys + enter to navigate the tree. The tree shows schemas, tables/views and their types, and columns and their types.\n\n### Editing a Query\n\nThe main query editor is a full-featured text editor, with features including syntax highlighting, auto-formatting with ``ctrl + ` ``, text selection, copy/paste, and more.\n\nYou can save the query currently in the editor with `ctrl + s`. You can open a query in any text or .sql file with `ctrl + o`.\n\n### Running a Query and Viewing Results\n\nTo run a query, press `ctrl + enter`. Up to 50k records will be loaded into the results pane below the query editor. When the focus is on the data pane, you can use your arrow keys or mouse to select different cells.\n\n### Exiting Harlequin\n\nPress `ctrl + q` to quit and return to your shell.',
+    'long_description': '# harlequin\nA Terminal-based SQL IDE for DuckDB.\n\n![harlequin TUI](harlequinv004.gif)\n\n(A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin duck](harlequin.jpg)\n\n## Installing Harlequin\n\nAfter installing Python 3.8 or above, install Harlequin using `pip` or `pipx` with:\n\n```bash\npipx install harlequin\n```\n\n> **Tip:**\n>\n> You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:\n> - `pipx run harlequin --help`\n> - `pipx run harlequin ./my.duckdb`\n\n\n## Using Harlequin\n\nFrom any shell, to open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\n### Viewing the Schema of your Database\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar. You can use your mouse or the arrow keys + enter to navigate the tree. The tree shows schemas, tables/views and their types, and columns and their types.\n\n### Editing a Query\n\nThe main query editor is a full-featured text editor, with features including syntax highlighting, auto-formatting with ``ctrl + ` ``, text selection, copy/paste, and more.\n\nYou can save the query currently in the editor with `ctrl + s`. You can open a query in any text or .sql file with `ctrl + o`.\n\n### Running a Query and Viewing Results\n\nTo run a query, press `ctrl + enter`. Up to 50k records will be loaded into the results pane below the query editor. When the focus is on the data pane, you can use your arrow keys or mouse to select different cells.\n\n### Exiting Harlequin\n\nPress `ctrl + q` to quit and return to your shell.',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `harlequin-0.0.8/PKG-INFO` & `harlequin-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -38,28 +38,14 @@
 > **Tip:**
 >
 > You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:
 > - `pipx run harlequin --help`
 > - `pipx run harlequin ./my.duckdb`
 
 
-## Running Harlequin in a Container
-
-Without a database file:
-
-```bash
-docker run ghcr.io/tconbeer/harlequin:latest
-```
-
-Mounting a database file `./foo.db` into the container's working directory, `/data`:
-
-```bash
-docker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db
-```
-
 ## Using Harlequin
 
 From any shell, to open a DuckDB database file:
 
 ```bash
 harlequin "path/to/duck.db"
 ```
```

