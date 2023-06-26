# Comparing `tmp/rcmt-0.8.2.tar.gz` & `tmp/rcmt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmt-0.8.2.tar", max compression
+gzip compressed data, was "rcmt-0.9.0.tar", max compression
```

## Comparing `rcmt-0.8.2.tar` & `rcmt-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2022-06-27 15:36:38.104359 rcmt-0.8.2/LICENSE
--rw-r--r--   0        0        0      518 2022-06-27 15:36:38.104359 rcmt-0.8.2/README.md
--rw-r--r--   0        0        0     1209 2022-06-27 15:36:38.104359 rcmt-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      362 2022-06-27 15:36:38.104359 rcmt-0.8.2/rcmt/__init__.py
--rw-r--r--   0        0        0    12589 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/action.py
--rwxr-xr-x   0        0        0     2021 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/cli.py
--rw-r--r--   0        0        0     1661 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/config.py
--rw-r--r--   0        0        0     4296 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/encoding.py
--rw-r--r--   0        0        0      497 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/fs.py
--rw-r--r--   0        0        0     3321 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/git.py
--rw-r--r--   0        0        0      614 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/log.py
--rw-r--r--   0        0        0     2192 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/matcher.py
--rw-r--r--   0        0        0     2558 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/package/__init__.py
--rw-r--r--   0        0        0     1732 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/package/manifest.py
--rw-r--r--   0        0        0     9072 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/rcmt.py
--rw-r--r--   0        0        0     5461 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/run.py
--rw-r--r--   0        0        0      104 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/source/__init__.py
--rw-r--r--   0        0        0     4406 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/source/github.py
--rw-r--r--   0        0        0     5396 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/source/gitlab.py
--rw-r--r--   0        0        0      480 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/source/local.py
--rw-r--r--   0        0        0     8225 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/source/source.py
--rw-r--r--   0        0        0      826 2022-06-27 15:36:38.108359 rcmt-0.8.2/rcmt/util.py
--rw-r--r--   0        0        0     1526 2022-06-27 15:36:53.155073 rcmt-0.8.2/setup.py
--rw-r--r--   0        0        0     1525 2022-06-27 15:36:53.155392 rcmt-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-07 17:49:54.490676 rcmt-0.9.0/LICENSE
+-rw-r--r--   0        0        0      518 2022-07-07 17:49:54.490676 rcmt-0.9.0/README.md
+-rw-r--r--   0        0        0     1209 2022-07-07 17:49:54.490676 rcmt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      362 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/__init__.py
+-rw-r--r--   0        0        0    12693 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/action.py
+-rwxr-xr-x   0        0        0     2021 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/cli.py
+-rw-r--r--   0        0        0     1661 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/config.py
+-rw-r--r--   0        0        0     4296 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/encoding.py
+-rw-r--r--   0        0        0      497 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/fs.py
+-rw-r--r--   0        0        0     3321 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/git.py
+-rw-r--r--   0        0        0      614 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/log.py
+-rw-r--r--   0        0        0     2746 2022-07-07 17:49:54.490676 rcmt-0.9.0/rcmt/matcher.py
+-rw-r--r--   0        0        0     2558 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/package/__init__.py
+-rw-r--r--   0        0        0     1732 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/package/manifest.py
+-rw-r--r--   0        0        0     9557 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/rcmt.py
+-rw-r--r--   0        0        0     5461 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/run.py
+-rw-r--r--   0        0        0      104 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/source/__init__.py
+-rw-r--r--   0        0        0     4406 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/source/github.py
+-rw-r--r--   0        0        0     5478 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/source/gitlab.py
+-rw-r--r--   0        0        0      480 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/source/local.py
+-rw-r--r--   0        0        0     8225 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/source/source.py
+-rw-r--r--   0        0        0      826 2022-07-07 17:49:54.494676 rcmt-0.9.0/rcmt/util.py
+-rw-r--r--   0        0        0     1526 2022-07-07 17:50:08.406231 rcmt-0.9.0/setup.py
+-rw-r--r--   0        0        0     1525 2022-07-07 17:50:08.406525 rcmt-0.9.0/PKG-INFO
```

### Comparing `rcmt-0.8.2/LICENSE` & `rcmt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/README.md` & `rcmt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/pyproject.toml` & `rcmt-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rcmt"
-version = "0.8.2"
+version = "0.9.0"
 description = ""
 license = "GPL-3.0-only"
 authors = [ "Markus Meyer <hydrantanderwand@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/wndhydrnt/rcmt"
 documentation = "https://rcmt.readthedocs.io/"
 
@@ -37,15 +37,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "22.3.0"
 isort = "5.9.1"
 pytest = "^7.1.2"
 mypy = "0.910"
 types-toml = "^0.10.7"
-types-PyYAML = "^6.0.8"
+types-PyYAML = "^6.0.9"
 Sphinx = "^5.0.2"
 flake8 = "^4.0.1"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autodoc-typehints = "^1.18.3"
 
 [tool.poetry.scripts]
 rcmt = "rcmt.cli:main"
```

### Comparing `rcmt-0.8.2/rcmt/action.py` & `rcmt-0.9.0/rcmt/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,20 @@
     """
 
     def __init__(self, target: str):
         self.target = target
 
     def apply(self, repo_path: str, tpl_data: dict) -> None:
         repo_file_path = os.path.join(repo_path, self.target)
-        if os.path.exists(repo_file_path):
+        if os.path.isfile(repo_file_path):
             os.remove(repo_file_path)
+            return
+
+        if os.path.isdir(repo_file_path):
+            shutil.rmtree(repo_file_path)
 
 
 class Own(Action):
     """
     Own ensures that a file in a repository stays the same.
 
     It always overwrites the data in the file with the data from a package.
```

### Comparing `rcmt-0.8.2/rcmt/cli.py` & `rcmt-0.9.0/rcmt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     repo_source: str,
     repo_project: str,
     repo_name: str,
     run_file: str,
     directory: str,
 ):
     opts = rcmt.options_from_config(config)
-    opts.matcher_path = run_file
+    opts.run_paths = [run_file]
     opts.packages_paths = packages
     rcmt.execute_local(
         directory=directory,
         repo_source=repo_source,
         repo_project=repo_project,
         repo_name=repo_name,
         opts=opts,
@@ -53,18 +53,18 @@
 @click.option(
     "--packages",
     help="Path to packages directory.",
     multiple=True,
     required=False,
     type=str,
 )
-@click.argument("matcher_file")
-def run(config: str, packages: list[str], matcher_file: str):
+@click.argument("run_file", nargs=-1)
+def run(config: str, packages: list[str], run_file: list[str]):
     opts = rcmt.options_from_config(config)
-    opts.matcher_path = matcher_file
+    opts.run_paths = run_file
     opts.packages_paths = packages
     result = rcmt.execute(opts)
     if result is False:
         exit(1)
 
 
 @click.command()
```

### Comparing `rcmt-0.8.2/rcmt/config.py` & `rcmt-0.9.0/rcmt/config.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/encoding.py` & `rcmt-0.9.0/rcmt/encoding.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/git.py` & `rcmt-0.9.0/rcmt/git.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/log.py` & `rcmt-0.9.0/rcmt/log.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/matcher.py` & `rcmt-0.9.0/rcmt/matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,7 +75,30 @@
         self.regex = re.compile(search)
 
     def match(self, repo: source.Repository) -> bool:
         if self.regex.match(str(repo)) is None:
             return False
 
         return True
+
+
+class Or(Base):
+    """
+    Or wraps multiple other matchers. It matches if one of those matchers matches.
+
+    :param args: One or more other matchers.
+
+    .. versionadded:: 0.9.0
+    """
+
+    def __init__(self, *args: Base):
+        if len(args) < 1:
+            raise RuntimeError("Matcher Or expects at least one argument")
+
+        self.matchers: tuple[Base, ...] = args
+
+    def match(self, repo: source.Repository) -> bool:
+        for m in self.matchers:
+            if m.match(repo) is True:
+                return True
+
+        return False
```

### Comparing `rcmt-0.8.2/rcmt/package/__init__.py` & `rcmt-0.9.0/rcmt/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/package/manifest.py` & `rcmt-0.9.0/rcmt/package/manifest.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/rcmt.py` & `rcmt-0.9.0/rcmt/rcmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 log: structlog.stdlib.BoundLogger = structlog.get_logger()
 
 
 class Options:
     def __init__(self, cfg: config.Config):
         self.config = cfg
         self.encoding_registry: encoding.Registry = encoding.Registry()
-        self.matcher_path: str = ""
+        self.run_paths: list[str] = []
         self.packages_paths: list[str] = []
         self.sources: dict[str, source.Base] = {}
 
 
 def can_merge_after(
     created_at: datetime.datetime, delay: Optional[datetime.timedelta]
 ) -> bool:
@@ -171,40 +171,24 @@
     log_level = logging.getLevelName(opts.config.log_level.upper())
     structlog.configure(
         wrapper_class=structlog.make_filtering_bound_logger(log_level),
     )
 
     pkg_reader = package.PackageReader(opts.encoding_registry)
     pkgs = pkg_reader.read_packages(opts.packages_paths)
-    matcher = run.read(opts.matcher_path)
-    pkgs_to_apply = find_packages(matcher.packages, pkgs)
-    repositories = []
+    repositories: list[source.Repository] = []
     for s in opts.sources.values():
         repositories += s.list_repositories()
 
     log.info("Repositories returned by sources", count=len(repositories))
-    gitc = git.Git(
-        matcher.branch(opts.config.git.branch_prefix),
-        opts.config.git.clone_options,
-        opts.config.git.data_dir,
-        opts.config.git.user_name,
-        opts.config.git.user_email,
-    )
-    runner = RepoRun(gitc, opts)
     success = True
-    for repo in repositories:
-        if matcher.match(repo) is False:
-            log.debug("Repository does not match", repository=str(repo))
-            continue
-
-        log.info("Matched repository", repository=str(repo))
-        try:
-            runner.execute(matcher, pkgs_to_apply, repo)
-        except Exception:
-            log.exception("Apply failed", repository=str(repo))
+    for run_path in opts.run_paths:
+        run_ = run.read(run_path)
+        run_success = execute_run(run_, pkgs, repositories, opts)
+        if run_success is False:
             success = False
 
     if success is False:
         log.error("Errors during execution - check previous log messages")
 
     return success
 
@@ -212,24 +196,58 @@
 def execute_local(
     directory: str, repo_source: str, repo_project: str, repo_name: str, opts: Options
 ) -> None:
     log_level = logging.getLevelName(opts.config.log_level.upper())
     structlog.configure(
         wrapper_class=structlog.make_filtering_bound_logger(log_level),
     )
+    if len(opts.run_paths) == 0:
+        log.warning("No path to a run file supplied")
+        return
 
     pkg_reader = package.PackageReader(opts.encoding_registry)
     pkgs = pkg_reader.read_packages(opts.packages_paths)
-    matcher = run.read(opts.matcher_path)
+    matcher = run.read(opts.run_paths[0])
     pkgs_to_apply = find_packages(matcher.packages, pkgs)
     repo = Local(repo_source, repo_project, repo_name)
     tpl_mapping: dict[str, str] = create_template_mapping(repo)
     apply_actions(pkgs_to_apply, repo, matcher, tpl_mapping, directory)
 
 
+def execute_run(
+    run_: run.Run,
+    pkgs: list[package.Package],
+    repos: list[source.Repository],
+    opts: Options,
+) -> bool:
+    pkgs_to_apply = find_packages(run_.packages, pkgs)
+    gitc = git.Git(
+        run_.branch(opts.config.git.branch_prefix),
+        opts.config.git.clone_options,
+        opts.config.git.data_dir,
+        opts.config.git.user_name,
+        opts.config.git.user_email,
+    )
+    runner = RepoRun(gitc, opts)
+    success = True
+    for repo in repos:
+        if run_.match(repo) is False:
+            log.debug("Repository does not match", repository=str(repo), run=run_.name)
+            continue
+
+        log.info("Matched repository", repository=str(repo), run=run_.name)
+        try:
+            runner.execute(run_, pkgs_to_apply, repo)
+        except Exception:
+            log.exception("Run failed", repository=str(repo), run=run_.name)
+            success = False
+
+    return success
+
+
 def options_from_config(path: str) -> Options:
     cfg = config.read_config_from_file(path)
     return config_to_options(cfg)
 
 
 def config_to_options(cfg: config.Config) -> Options:
     opts = Options(cfg)
```

### Comparing `rcmt-0.8.2/rcmt/run.py` & `rcmt-0.9.0/rcmt/run.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/source/github.py` & `rcmt-0.9.0/rcmt/source/github.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/source/gitlab.py` & `rcmt-0.9.0/rcmt/source/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
                 "target_branch": self.base_branch,
                 "title": pr.title,
             }
         )
 
     def find_pull_request(self, branch: str) -> Union[Any, None]:
         log.debug("Listing merge requests", repo=str(self))
-        mrs = self._project.mergerequests.list(state="all", source_branch=branch)
+        mrs = self._project.mergerequests.list(
+            all=False, state="all", source_branch=branch
+        )
         if len(mrs) == 0:
             return None
 
         if isinstance(mrs, list):
             return mrs[0]
 
         if isinstance(mrs, RESTObjectList):
@@ -88,15 +90,17 @@
             if fnmatch.fnmatch(entry["path"], file):
                 return True
 
         return False
 
     def has_successful_pr_build(self, identifier: GitlabMergeRequest) -> bool:
         failed = False
-        for commit_status in self._project.commits.get(identifier.sha).statuses.list():
+        for commit_status in self._project.commits.get(
+            id=identifier.sha, lazy=True
+        ).statuses.list(iterator=True):
             if commit_status.allow_failure is True:
                 continue
 
             if commit_status.status != "success":
                 log.debug(
                     "MR check failed",
                     repo=str(self),
```

### Comparing `rcmt-0.8.2/rcmt/source/source.py` & `rcmt-0.9.0/rcmt/source/source.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/rcmt/util.py` & `rcmt-0.9.0/rcmt/util.py`

 * *Files identical despite different names*

### Comparing `rcmt-0.8.2/setup.py` & `rcmt-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['rcmt = rcmt.cli:main']}
 
 setup_kwargs = {
     'name': 'rcmt',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': '',
     'long_description': '# rcmt\n\nWith rcmt you can\n\n- create, modify or delete files across many repositories.\n- merge global settings with user-configured settings in repositories.\n- write your own tooling to manipulate files in repositories.\n\nTake a look at the [documentation](https://rcmt.readthedocs.io/) to learn more.\n\n## Development\n\n```shell\n# Install dependencies and dev-dependencies\npoetry install\n# Run linters\nmake lint\n# Run tests\nmake test\n# Generate and open the documentation\nmake docs\nopen ./docs/_build/html/index.html\n```\n',
     'author': 'Markus Meyer',
     'author_email': 'hydrantanderwand@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/wndhydrnt/rcmt',
```

### Comparing `rcmt-0.8.2/PKG-INFO` & `rcmt-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmt
-Version: 0.8.2
+Version: 0.9.0
 Summary: 
 Home-page: https://github.com/wndhydrnt/rcmt
 License: GPL-3.0-only
 Author: Markus Meyer
 Author-email: hydrantanderwand@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

