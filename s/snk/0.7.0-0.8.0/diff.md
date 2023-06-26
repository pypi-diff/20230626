# Comparing `tmp/snk-0.7.0.tar.gz` & `tmp/snk-0.8.0.tar.gz`

## Comparing `snk-0.7.0.tar` & `snk-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.7.0/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 snk-0.7.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.7.0/docs/CNAME
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 snk-0.7.0/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.7.0/docs/managing_pipelines.md
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.7.0/docs/pipeline_packages.md
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/nest.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.7.0/docs/reference/pipeline.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.7.0/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.7.0/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.7.0/snk/errors.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.7.0/snk/main.py
--rw-r--r--   0        0        0    16501 2020-02-02 00:00:00.000000 snk-0.7.0/snk/nest.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 snk-0.7.0/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/__init__.py
--rw-r--r--   0        0        0    20027 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/cli.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/options.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 snk-0.7.0/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.7.0/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_nest.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.7.0/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.7.0/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.7.0/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.7.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 snk-0.7.0/README.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 snk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.8.0/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.8.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.8.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 snk-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.8.0/docs/CNAME
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 snk-0.8.0/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.8.0/docs/managing_pipelines.md
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 snk-0.8.0/docs/pipeline_packages.md
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 snk-0.8.0/docs/snk_config_file.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 snk-0.8.0/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.8.0/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.8.0/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.8.0/docs/reference/nest.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 snk-0.8.0/docs/reference/pipeline.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.8.0/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.8.0/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.8.0/snk/errors.py
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 snk-0.8.0/snk/main.py
+-rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 snk-0.8.0/snk/nest.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 snk-0.8.0/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.8.0/snk/cli/__init__.py
+-rw-r--r--   0        0        0    20042 2020-02-02 00:00:00.000000 snk-0.8.0/snk/cli/cli.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 snk-0.8.0/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.8.0/snk/cli/options.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 snk-0.8.0/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.8.0/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 snk-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 snk-0.8.0/tests/test_nest.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk-0.8.0/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.8.0/tests/test_snk.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 snk-0.8.0/tests/test_snk_config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.8.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.8.0/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 snk-0.8.0/README.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 snk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 snk-0.8.0/PKG-INFO
```

### Comparing `snk-0.7.0/mkdocs.yml` & `snk-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/.github/workflows/publish.yml` & `snk-0.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/.github/workflows/tests.yml` & `snk-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/docs/index.md` & `snk-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/docs/managing_pipelines.md` & `snk-0.8.0/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/docs/pipeline_packages.md` & `snk-0.8.0/docs/pipeline_packages.md`

 * *Files 4% similar despite different names*

```diff
@@ -170,27 +170,27 @@
 
 [Wed May 31 14:21:45 2023]
 Finished job 0.
 1 of 1 steps (100%) done
 Complete log: .snakemake/log/2023-05-31T142144.694274.snakemake.log
 ```
 
-We can also add a `.snk` file to add annotations to the CLI. See [.snk]() docs for details.
+We can also add a `snk.yaml` file to add annotations to the CLI. See [Snk Config](/snk_config_file/) docs for details.
 
 ```
 pipeline-name
 ├── LICENSE.txt
 ├── README.md
 ├── pyproject.toml
 ├── src
 │   └── pipeline_name
 │       ├── __about__.py
 │       ├── __init__.py
 │       ├── __main__.py
-│       ├── .snk <-
+│       ├── snk.yaml <-
 │       ├── cli
 │       │   └── __init__.py
 │       ├── config.yaml
 │       └── workflow
 │           └── Snakefile
 └── tests
     └── __init__.py
```

### Comparing `snk-0.7.0/snk/main.py` & `snk-0.8.0/snk/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from types import SimpleNamespace
 import typer
 from pathlib import Path
-import os
 from typing import Optional, List
-from rich.pretty import pprint
+from rich import print
 from .nest import Nest
 from .errors import PipelineExistsError, PipelineNotFoundError
 
 app = typer.Typer()
 
 SNK_HOME = None
 SNK_BIN = None
@@ -157,17 +156,20 @@
     except FileNotFoundError:
         pipelines = []
     pipeline_dir_yellow = typer.style(
         nest.pipelines_dir, fg=typer.colors.YELLOW, bold=False
     )
     typer.echo(f"Found {len(pipelines)} pipelines in {pipeline_dir_yellow}")
     for pipeline in pipelines:
+        if pipeline.editable:
+            print(f'- {pipeline.name} ([bold green]editable[/bold green]) -> "{pipeline.path}"')
+            continue
         v = pipeline.version
         v = v if v else "latest"
-        typer.echo(f"- {pipeline.name} ({v})")
+        print(f"- {pipeline.name} ([bold green]{v}[/bold green])")
 
 
 # @app.command()
 # def run(
 #         pipeline: str = typer.Argument(
 #             ..., help="URL or Github name (user/repo) of the pipeline to install."
 #         ),
```

### Comparing `snk-0.7.0/snk/nest.py` & `snk-0.8.0/snk/nest.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,14 @@
             if not force:
                 self._check_pipeline_name_available(name)
             else:
                 handle_force_installation(name)
             pipeline_path = self.download(pipeline, name, tag_name=tag)
         except InvalidPipelineRepositoryError:
             pipeline_local_path = Path(pipeline)
-            if pipeline_local_path.name == ".snk":
-                pipeline_local_path = pipeline_local_path.parent
             if not name:
                 name = pipeline_local_path.name
             if not force:
                 self._check_pipeline_name_available(name)
             else:
                 handle_force_installation(name)
             pipeline_path = self.local(pipeline_local_path, name, editable)
@@ -151,39 +149,42 @@
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
         return Pipeline(pipeline_path)
 
     def modify_snk_config(self, pipeline_path: Path, **kwargs):
         """
-        Modify the .snk file.
+        Modify the snk config file.
         Args:
           pipeline_path (Path): The path to the pipeline directory.
           name (str): The name of the pipeline.
         Examples:
           >>> nest.modify_snk_config(Path('/path/to/pipeline'), 'example')
         """
-        snk_config = SnkConfig.from_path(pipeline_path / ".snk")
+        snk_config = SnkConfig.from_pipeline_dir(
+            pipeline_path, 
+            create_if_not_exists=True
+        )
         for key, value in kwargs.items():
             setattr(snk_config, key, value)
-        snk_config.to_yaml(pipeline_path / ".snk")
+        snk_config.save()
     
     def additional_resources(self, pipeline_path: Path, resources: List[Path]):
         """
-        Modify the .snk file so that resources will be copied at runtime.
+        Modify the snk config file so that resources will be copied at runtime.
         Args:
           pipeline_path (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
         Examples:
           >>> nest.additional_resources(Path('/path/to/pipeline'), [Path('/path/to/resource1'), Path('/path/to/resource2')])
         """
         # validate_resources(resources)
-        snk_config = SnkConfig.from_path(pipeline_path / ".snk")
+        snk_config = SnkConfig.from_pipeline_dir(pipeline_path, create_if_not_exists=True)
         snk_config.add_resources(resources, pipeline_path)
-        snk_config.to_yaml(pipeline_path / ".snk")
+        snk_config.save()
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         """
         Copy a nonstandard config file to the pipeline directory.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
           config_path (Path): The path to the config file.
```

### Comparing `snk-0.7.0/snk/pipeline.py` & `snk-0.8.0/snk/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,19 @@
         """
         pipeline_bin_dir = self.path / "bin"
         name = self.name
         if sys.platform.startswith("win"):
             name += ".exe"
         return pipeline_bin_dir / name
 
+    @property
+    def editable(self):
+        """Is the pipeline editable?"""
+        return self.path.is_symlink()
+
     def _find_folder(self, name) -> Optional[Path]:
         """Search for folder"""
         if (self.path / name).exists():
             return self.path / name
         if (self.path / "workflow" / name).exists():
             return self.path / "workflow" / name
         return None
```

### Comparing `snk-0.7.0/snk/cli/cli.py` & `snk-0.8.0/snk/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             # get the file path from the calling frame
             pipeline_dir_path = Path(calling_frame.f_globals['__file__'])
         if pipeline_dir_path.is_file():
             pipeline_dir_path = pipeline_dir_path.parent
         self.pipeline = Pipeline(path=pipeline_dir_path)
         self.app = typer.Typer()
         self.snakemake_config = load_pipeline_snakemake_config(pipeline_dir_path)
-        self.snk_config: SnkConfig = SnkConfig.from_path(pipeline_dir_path / ".snk")
+        self.snk_config = SnkConfig.from_pipeline_dir(pipeline_dir_path, create_if_not_exists=True)
         self.options = build_dynamic_cli_options(self.snakemake_config, self.snk_config)
         self.snakefile = self._find_snakefile()
         self.conda_prefix_dir = pipeline_dir_path / ".conda"
         if " " in str(pipeline_dir_path):
             # cannot have spaces!
             self.singularity_prefix_dir = None
         else:
```

### Comparing `snk-0.7.0/snk/cli/utils.py` & `snk-0.8.0/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/.DS_Store` & `snk-0.8.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/conftest.py` & `snk-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/test_nest.py` & `snk-0.8.0/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/test_pipline_cli.py` & `snk-0.8.0/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/test_snk.py` & `snk-0.8.0/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/utils.py` & `snk-0.8.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/data/artic_v4.1.bed` & `snk-0.8.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/data/config.yaml` & `snk-0.8.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/tests/data/cov.fasta` & `snk-0.8.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/LICENSE.txt` & `snk-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/README.md` & `snk-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/pyproject.toml` & `snk-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.7.0/PKG-INFO` & `snk-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.7.0
+Version: 0.8.0
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snk Version: 0.7.0 Project-URL: Documentation,
+Metadata-Version: 2.1 Name: snk Version: 0.8.0 Project-URL: Documentation,
 https://github.com/wytamma/snk#readme Project-URL: Issues, https://github.com/
 wytamma/snk/issues Project-URL: Source, https://github.com/wytamma/snk Author-
 email: Wytamma Wirth
 wirth@me.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

