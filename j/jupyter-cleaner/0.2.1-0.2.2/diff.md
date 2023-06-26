# Comparing `tmp/jupyter_cleaner-0.2.1.tar.gz` & `tmp/jupyter_cleaner-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_cleaner-0.2.1.tar", max compression
+gzip compressed data, was "jupyter_cleaner-0.2.2.tar", max compression
```

## Comparing `jupyter_cleaner-0.2.1.tar` & `jupyter_cleaner-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.1/jupyter_cleaner/__init__.py
--rw-r--r--   0        0        0    16790 2023-06-24 19:41:04.694071 jupyter_cleaner-0.2.1/jupyter_cleaner/jupyter_cleaner.py
--rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.1/LICENSE
--rw-r--r--   0        0        0     1795 2023-06-24 19:42:32.682098 jupyter_cleaner-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1991 2023-06-23 07:54:37.232156 jupyter_cleaner-0.2.1/README.md
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 17:07:31.522031 jupyter_cleaner-0.2.2/jupyter_cleaner/__init__.py
+-rw-r--r--   0        0        0    16637 2023-06-26 10:27:33.350629 jupyter_cleaner-0.2.2/jupyter_cleaner/jupyter_cleaner.py
+-rw-r--r--   0        0        0     1092 2023-06-21 17:40:20.719190 jupyter_cleaner-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1985 2023-06-26 11:05:51.759642 jupyter_cleaner-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2175 2023-06-26 07:51:33.830990 jupyter_cleaner-0.2.2/README.md
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 jupyter_cleaner-0.2.2/PKG-INFO
```

### Comparing `jupyter_cleaner-0.2.1/jupyter_cleaner/jupyter_cleaner.py` & `jupyter_cleaner-0.2.2/jupyter_cleaner/jupyter_cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 else:
     import tomli as tomllib
 
 
 def run(
     files: Sequence[Path],
     execution_count: int = 0,
-    remove_code_output: bool = True,
+    remove_outputs: bool = True,
     format: bool = True,
     reorder_imports: bool = True,
     indent_level: int = 4,
     exclude_files: Sequence[Path] = [],
     black_config: Optional[Dict[str, str]] = None,
 ) -> None:
     """Format Jupyter lab files.
 
     :param Sequence[Path] files: file(s) to be formatted
     :param Sequence[Path] exclude_files: file(s) to be excluded from formatting
     :param int execution_count: sets execution count. If the integer is greater than zero the count will be printed, else `null` will be printed. Defaults to 0.
-    :param bool remove_code_output: remove output from code cells, defaults to True
+    :param bool remove_outputs: remove output from code cells, defaults to True
     :param bool format: format cells using black, defaults to True
     :param bool reorder_imports: reorder imports using reoder-python-imports, defaults to True
     :param int indent_level: integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert newlines.
     :param Optional[Dict[str, str]] black_config: configuration from black formatting, defaults to None
     :raises TypeError: when file input is unrecognised
     """
     if black_config is None:
@@ -70,60 +70,55 @@
             data = json.load(f)
             python_version = data["metadata"]["language_info"]["version"]
             min_python_version = tuple(map(int, re.findall(r"(\d+)", python_version)))
             if len(min_python_version) > 2:
                 min_python_version = min_python_version[:2]
 
             for cell in data["cells"]:
-                if "execution_count" in cell.keys() and cell["cell_type"] == "code":
+                if execution_count >= 0 and "execution_count" in cell.keys():
                     cell["execution_count"] = (
                         execution_count if execution_count > 0 else "null"
                     )
-                    if remove_code_output:
-                        cell["outputs"] = []
+                if remove_outputs and "outputs" in cell.keys():
+                    cell["outputs"] = []
 
-                    if format:
-                        try:
-                            mode = black.Mode(is_ipynb=True, **black_config)  # type: ignore
-                            str_cell_content = black.format_cell(
-                                "".join(cell["source"]), mode=mode, fast=False
-                            )
-                            cell_content = [
-                                f"{c}\n" for c in str_cell_content.split("\n")
-                            ]
-                            cell_content[-1] = cell_content[-1][
-                                :-1
-                            ]  # remove last newline
-                            cell["source"] = cell_content
-                        except black.NothingChanged:
-                            pass
-
-                    if reorder_imports:
-                        to_remove = {
-                            import_obj_from_str(s).key
-                            for k, v in REMOVALS.items()
-                            if min_python_version >= k
-                            for s in v
-                        }
-                        replace_import: List[str] = []
-                        for k, v in REPLACES.items():
-                            if min_python_version >= k:
-                                replace_import.extend(
-                                    _validate_replace_import(replace_s)
-                                    for replace_s in v
-                                )
-                        to_replace = Replacements.make(replace_import)
-                        str_cell_content = fix_file_contents(
-                            "".join(cell["source"]),
-                            to_replace=to_replace,
-                            to_remove=to_remove,
-                        )[:-1]
+                if format and "source" in cell.keys():
+                    try:
+                        mode = black.Mode(is_ipynb=True, **black_config)  # type: ignore
+                        str_cell_content = black.format_cell(
+                            "".join(cell["source"]), mode=mode, fast=False
+                        )
                         cell_content = [f"{c}\n" for c in str_cell_content.split("\n")]
-                        cell_content[-1] = cell_content[-1][:-1]
+                        cell_content[-1] = cell_content[-1][:-1]  # remove last newline
                         cell["source"] = cell_content
+                    except black.NothingChanged:
+                        pass
+
+                if reorder_imports and "source" in cell.keys():
+                    to_remove = {
+                        import_obj_from_str(s).key
+                        for k, v in REMOVALS.items()
+                        if min_python_version >= k
+                        for s in v
+                    }
+                    replace_import: List[str] = []
+                    for k, v in REPLACES.items():
+                        if min_python_version >= k:
+                            replace_import.extend(
+                                _validate_replace_import(replace_s) for replace_s in v
+                            )
+                    to_replace = Replacements.make(replace_import)
+                    str_cell_content = fix_file_contents(
+                        "".join(cell["source"]),
+                        to_replace=to_replace,
+                        to_remove=to_remove,
+                    )[:-1]
+                    cell_content = [f"{c}\n" for c in str_cell_content.split("\n")]
+                    cell_content[-1] = cell_content[-1][:-1]
+                    cell["source"] = cell_content
 
         with open(file) as f:
             original_data = json.load(f)
             if data == original_data:
                 continue
 
         with open(file, "w") as f:
@@ -216,24 +211,22 @@
         files_or_dirs = [files_or_dirs]
     exclude_files_or_dirs = (
         config["exclude_files_or_dirs"] if "exclude_files_or_dirs" in config else None
     )
     if isinstance(exclude_files_or_dirs, str):
         exclude_files_or_dirs = [exclude_files_or_dirs]
     execution_count = config["execution_count"] if "execution_count" in config else None
-    remove_code_output = (
-        config["remove_code_output"] if "remove_code_output" in config else None
-    )
+    remove_outputs = config["remove_outputs"] if "remove_outputs" in config else None
     format = config["format"] if "format" in config else None
     reorder_imports = config["reorder_imports"] if "reorder_imports" in config else None
     indent_level = config["indent_level"] if "indent_level" in config else None
     return (
         files_or_dirs,
         execution_count,
-        remove_code_output,
+        remove_outputs,
         format,
         reorder_imports,
         indent_level,
         exclude_files_or_dirs,
     )
 
 
@@ -251,47 +244,47 @@
         nargs="+",
         help="Jupyter lab files or directories to exclude from formatting and search",
     )
     parser.add_argument(
         "--execution_count",
         type=int,
         default=0,
-        help="Number to set for the execution count of every cell",
+        help="Number to set for the execution count of every cell. A negative integer doesn't replace the execution count and 0 is replaced with null. Defaults to 0.",
     )
     parser.add_argument(
         "--indent_level",
         type=int,
         default=4,
-        help="Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert newlines.",
+        help="Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert newlines.. Defaults to 4.",
     )
     parser.add_argument(
-        "--remove_code_output",
-        action="store_false",
-        help="Remove output of cell",
+        "--remove_outputs",
+        action="store_true",
+        help="Remove output of cell. Defaults to false.",
     )
     parser.add_argument(
         "--format",
-        action="store_false",
-        help="Format code of every cell (uses black)",
+        action="store_true",
+        help="Format code of every cell (uses black). Defaults to false.",
     )
     parser.add_argument(
         "--reorder_imports",
-        action="store_false",
-        help="Reorder imports of every cell (uses reorder-python-imports)",
+        action="store_true",
+        help="Reorder imports of every cell (uses reorder-python-imports). Defaults to false.",
     )
     parser.add_argument(
         "--ignore_pyproject",
-        action="store_false",
-        help="Argparse will over-ride pyproject",
+        action="store_true",
+        help="Argparse will over-ride pyproject. Defaults to false.",
     )
     args = parser.parse_args()
     return (
         args.files_or_dirs,
         args.execution_count,
-        args.remove_code_output,
+        args.remove_outputs,
         args.format,
         args.reorder_imports,
         args.indent_level,
         args.exclude_files_or_dirs,
         args.ignore_pyproject,
     )
 
@@ -307,48 +300,48 @@
             raise ValueError("File or directory does not exist or could not be found")
     return list(set(files))
 
 
 def process_inputs(
     args_files_or_dirs: List[str],
     args_execution_count: int,
-    args_remove_code_output: bool,
+    args_remove_outputs: bool,
     args_format: bool,
     args_reorder_imports: bool,
     args_indent_level: int,
     args_exclude_files_or_dirs: Union[List[str], None],
     args_ignore_pyproject: bool,
     project_files_or_dirs: Union[List[str], str, None],
     project_execution_count: Union[int, None],
-    project_remove_code_output: Union[bool, None],
+    project_remove_outputs: Union[bool, None],
     project_format: Union[bool, None],
     project_reorder_imports: Union[bool, None],
     project_indent_level: Union[int, None],
     project_exclude_files_or_dirs: Union[List[str], str, None],
 ) -> Tuple[List[Path], int, bool, bool, bool, int, List[Path]]:
     """Creates inputs of the right format and prioritises pyproject inputs over argparse inputs, outside of files and directories where all inputs are combined.
 
     :param List[str] args_files_or_dirs: files or directories from argparse
     :param List[str] args_exclude_files_or_dirs: files or directories to exclude from argparse
     :param int args_execution_count: execution count from argparse
-    :param bool args_remove_code_output: remove code output from argparse
+    :param bool args_remove_outputs: remove code output from argparse
     :param bool args_format: apply formatting from argparse
     :param bool args_reorder_imports: reorder imports from argparse
     :param Union[List[str], str, None] project_files_or_dirs: files or directories from pyproject
     :param Union[List[str], str, None] project_exclude_files_or_dirs: files or directories to exclude from pyproject
     :param Union[int, None] project_execution_count: execution count from pyproject
-    :param Union[bool, None] project_remove_code_output: remove code output from pyproject
+    :param Union[bool, None] project_remove_outputs: remove code output from pyproject
     :param Union[bool, None] project_format: apply formatting from pyproject
     :param Union[bool, None] project_reorder_imports: reorder imports from pyproject
     :return Tuple[ Union[List[str], str, None], Union[int, None], Union[bool, None], Union[bool, None], Union[bool, None], ]: inputs to run()
     """
     if args_ignore_pyproject:
         project_files_or_dirs = None
         project_execution_count = None
-        project_remove_code_output = None
+        project_remove_outputs = None
         project_format = None
         project_reorder_imports = None
         project_indent_level = None
         project_exclude_files_or_dirs = None
 
     if args_files_or_dirs is None:
         args_files_or_dirs = [Path.cwd().resolve()]
@@ -367,93 +360,93 @@
         Path(f) for f in project_exclude_files_or_dirs + args_exclude_files_or_dirs
     ]
     execution_count = (
         project_execution_count
         if project_execution_count is not None
         else args_execution_count
     )
-    remove_code_output = (
-        project_remove_code_output
-        if project_remove_code_output is not None
-        else args_remove_code_output
+    remove_outputs = (
+        project_remove_outputs
+        if project_remove_outputs is not None
+        else args_remove_outputs
     )
     format = project_format if project_format is not None else args_format
     reorder_imports = (
         project_reorder_imports
         if project_reorder_imports is not None
         else args_reorder_imports
     )
     indent_level = (
         project_indent_level if project_indent_level is not None else args_indent_level
     )
 
     return (
         files_or_dirs,
         execution_count,
-        remove_code_output,
+        remove_outputs,
         format,
         reorder_imports,
         indent_level,
         exclude_files_or_dirs,
     )
 
 
 def main():
     (
         args_files_or_dirs,
         args_execution_count,
-        args_remove_code_output,
+        args_remove_outputs,
         args_format,
         args_reorder_imports,
         args_indent_level,
         args_exclude_files_or_dirs,
         args_ignore_pyproject,
     ) = parse_args()
 
     (
         project_files_or_dirs,
         project_execution_count,
-        project_remove_code_output,
+        project_remove_outputs,
         project_format,
         project_reorder_imports,
         project_indent_level,
         project_exclude_files_or_dirs,
     ) = parse_pyproject()
 
     (
         files_or_dirs,
         execution_count,
-        remove_code_output,
+        remove_outputs,
         format,
         reorder_imports,
         indent_level,
         exclude_files_or_dirs,
     ) = process_inputs(
         args_files_or_dirs,
         args_execution_count,
-        args_remove_code_output,
+        args_remove_outputs,
         args_format,
         args_reorder_imports,
         args_indent_level,
         args_exclude_files_or_dirs,
         args_ignore_pyproject,
         project_files_or_dirs,
         project_execution_count,
-        project_remove_code_output,
+        project_remove_outputs,
         project_format,
         project_reorder_imports,
         project_indent_level,
         project_exclude_files_or_dirs,
     )
 
     files = get_lab_files(files_or_dirs)
     exclude_files = get_lab_files(exclude_files_or_dirs)
 
     run(
         files,
         execution_count,
-        remove_code_output,
+        remove_outputs,
         format,
         reorder_imports,
         indent_level,
         exclude_files,
     )
```

### Comparing `jupyter_cleaner-0.2.1/LICENSE` & `jupyter_cleaner-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_cleaner-0.2.1/pyproject.toml` & `jupyter_cleaner-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jupyter-cleaner"
-version = "0.2.1"
+version = "0.2.2"
 description = "Easy git tracking of Jupyter lab files"
 license = "MIT"
 authors = ["Daniel Stoops <danielstoops25@gmail.com>"]
 maintainers = ["Daniel Stoops <danielstoops25@gmail.com>"]
 readme = "README.md"
 packages = [{include = "jupyter_cleaner"}]
 homepage = "https://github.com/Stoops-ML/jupyter-cleaner"
@@ -16,31 +16,39 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.0"
 tox = "^4.6.3"
 flake8 = "^6.0.0"
 pytest = "^7.3.2"
 pre-commit = "^3.3.3"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 jupyter-cleaner = "jupyter_cleaner.jupyter_cleaner:main"
 
 [tool.jupyter-cleaner]
 execution_count=0
-remove_code_output=true
+remove_outputs=true
 format=true
 reorder_imports=true
 indent_level=4
 
 [tool.pytest.ini_options]
 testpaths = "tests"
+addopts = [
+    "--cov=jupyter_cleaner",
+    "--cov-fail-under=90",
+    "--cov-report=term-missing",
+    "--cov-report=term",
+    "--cov-report="
+]
 
 [tool.tox]
 # run in parent (pwsh) shell before tox: pyenv local 3.8.10, 3.9.13, 3.10.10, 3.11.2
 legacy_tox_ini = """
 [tox]
 envlist =
     python38
@@ -49,14 +57,15 @@
     python311
     lint
 isolated_build = true
 
 [testenv]
 deps =
     pytest
+    pytest-cov
 setenv =
     PYTHONPATH = {toxinidir}
 commands =
     python -c "import sys; print(sys.version_info)"
     python -m pytest --basetemp={envtmpdir}
 
 [testenv:python38]
```

### Comparing `jupyter_cleaner-0.2.1/README.md` & `jupyter_cleaner-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 
 It is recommended to run jupyter-cleaner before adding the Jupyter lab files to the stage in git. This allows for easier tracking of differences between commits.
 
 ## CLI
 running `jupyter-cleaner -h` displays:
 ```
 usage: jupyter-cleaner [-h] [--exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]] [--execution_count EXECUTION_COUNT]
-                       [--indent_level INDENT_LEVEL] [--remove_code_output] [--format] [--reorder_imports]
+                       [--indent_level INDENT_LEVEL] [--remove_outputs] [--format] [--reorder_imports] [--ignore_pyproject]
                        files_or_dirs [files_or_dirs ...]
 
 jupyter_cleaner
 
 positional arguments:
   files_or_dirs         Jupyter lab files to format or directories to search for lab files
 
 options:
   -h, --help            show this help message and exit
   --exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]
                         Jupyter lab files or directories to exclude from formatting and search
   --execution_count EXECUTION_COUNT
-                        Number to set for the execution count of every cell
+                        Number to set for the execution count of every cell. Defaults to 0.
   --indent_level INDENT_LEVEL
-                        Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert
-                        newlines.
-  --remove_code_output  Remove output of cell
-  --format              Format code of every cell (uses black)
-  --reorder_imports     Reorder imports of every cell (uses reorder-python-imports)
+                        Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative
+                        will only insert newlines.. Defaults to 4.
+  --remove_outputs      Remove output of cell. Defaults to false.
+  --format              Format code of every cell (uses black). Defaults to false.
+  --reorder_imports     Reorder imports of every cell (uses reorder-python-imports). Defaults to false.
+  --ignore_pyproject    Argparse will over-ride pyproject. Defaults to false.
 ```
 
 ## pyproject.toml
 Inputs to jupyter-cleaner can be supplied via pyproject.toml:
 ```
 [tool.jupyter_cleaner]
 execution_count=0
-remove_code_output=true
+remove_outputs=true
 format=true
 reorder_imports=true
 indent_level=4
 ```
```

### Comparing `jupyter_cleaner-0.2.1/PKG-INFO` & `jupyter_cleaner-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-cleaner
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy git tracking of Jupyter lab files
 Home-page: https://github.com/Stoops-ML/jupyter-cleaner
 License: MIT
 Author: Daniel Stoops
 Author-email: danielstoops25@gmail.com
 Maintainer: Daniel Stoops
 Maintainer-email: danielstoops25@gmail.com
@@ -31,40 +31,41 @@
 
 It is recommended to run jupyter-cleaner before adding the Jupyter lab files to the stage in git. This allows for easier tracking of differences between commits.
 
 ## CLI
 running `jupyter-cleaner -h` displays:
 ```
 usage: jupyter-cleaner [-h] [--exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]] [--execution_count EXECUTION_COUNT]
-                       [--indent_level INDENT_LEVEL] [--remove_code_output] [--format] [--reorder_imports]
+                       [--indent_level INDENT_LEVEL] [--remove_outputs] [--format] [--reorder_imports] [--ignore_pyproject]
                        files_or_dirs [files_or_dirs ...]
 
 jupyter_cleaner
 
 positional arguments:
   files_or_dirs         Jupyter lab files to format or directories to search for lab files
 
 options:
   -h, --help            show this help message and exit
   --exclude_files_or_dirs EXCLUDE_FILES_OR_DIRS [EXCLUDE_FILES_OR_DIRS ...]
                         Jupyter lab files or directories to exclude from formatting and search
   --execution_count EXECUTION_COUNT
-                        Number to set for the execution count of every cell
+                        Number to set for the execution count of every cell. Defaults to 0.
   --indent_level INDENT_LEVEL
-                        Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative will only insert
-                        newlines.
-  --remove_code_output  Remove output of cell
-  --format              Format code of every cell (uses black)
-  --reorder_imports     Reorder imports of every cell (uses reorder-python-imports)
+                        Integer greater than zero will pretty-print the JSON array with that indent level. An indent level of 0 or negative
+                        will only insert newlines.. Defaults to 4.
+  --remove_outputs      Remove output of cell. Defaults to false.
+  --format              Format code of every cell (uses black). Defaults to false.
+  --reorder_imports     Reorder imports of every cell (uses reorder-python-imports). Defaults to false.
+  --ignore_pyproject    Argparse will over-ride pyproject. Defaults to false.
 ```
 
 ## pyproject.toml
 Inputs to jupyter-cleaner can be supplied via pyproject.toml:
 ```
 [tool.jupyter_cleaner]
 execution_count=0
-remove_code_output=true
+remove_outputs=true
 format=true
 reorder_imports=true
 indent_level=4
 ```
```

