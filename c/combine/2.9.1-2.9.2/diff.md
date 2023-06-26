# Comparing `tmp/combine-2.9.1.tar.gz` & `tmp/combine-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combine-2.9.1.tar", max compression
+gzip compressed data, was "combine-2.9.2.tar", max compression
```

## Comparing `combine-2.9.1.tar` & `combine-2.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1066 2022-06-30 18:58:12.175312 combine-2.9.1/LICENSE
--rw-r--r--   0        0        0     1003 2022-06-30 18:58:12.175312 combine-2.9.1/README.md
--rw-r--r--   0        0        0      172 2022-06-30 18:58:12.175312 combine-2.9.1/combine/__init__.py
--rw-r--r--   0        0        0     1044 2022-06-30 18:58:12.175312 combine-2.9.1/combine/base_content/error.template.html
--rw-r--r--   0        0        0      118 2022-06-30 18:58:12.175312 combine-2.9.1/combine/base_content/markdown.template.html
--rw-r--r--   0        0        0      377 2022-06-30 18:58:12.175312 combine-2.9.1/combine/base_content/redirect.template.html
--rw-r--r--   0        0        0        0 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/__init__.py
--rw-r--r--   0        0        0       66 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/base.py
--rw-r--r--   0        0        0      908 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/duplicate_id.py
--rw-r--r--   0        0        0      520 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/favicon.py
--rw-r--r--   0        0        0     1190 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/file_size.py
--rw-r--r--   0        0        0      698 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/img_alt.py
--rw-r--r--   0        0        0     1412 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/issues.py
--rw-r--r--   0        0        0     2818 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/links.py
--rw-r--r--   0        0        0     1221 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/meta.py
--rw-r--r--   0        0        0     1311 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/mixed_content.py
--rw-r--r--   0        0        0     3904 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/open_graph.py
--rw-r--r--   0        0        0     1550 2022-06-30 18:58:12.175312 combine-2.9.1/combine/checks/title.py
--rw-r--r--   0        0        0     6315 2022-06-30 18:58:12.175312 combine-2.9.1/combine/cli.py
--rw-r--r--   0        0        0     4574 2022-06-30 18:58:12.175312 combine-2.9.1/combine/config.py
--rw-r--r--   0        0        0     5750 2022-06-30 18:58:12.175312 combine-2.9.1/combine/core.py
--rw-r--r--   0        0        0     7212 2022-06-30 18:58:12.175312 combine-2.9.1/combine/dev.py
--rw-r--r--   0        0        0       38 2022-06-30 18:58:12.175312 combine-2.9.1/combine/exceptions.py
--rw-r--r--   0        0        0      768 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/__init__.py
--rw-r--r--   0        0        0     1748 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/core.py
--rw-r--r--   0        0        0     1183 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/error.py
--rw-r--r--   0        0        0     2812 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/html.py
--rw-r--r--   0        0        0      182 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/ignored.py
--rw-r--r--   0        0        0     1456 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/markdown.py
--rw-r--r--   0        0        0      568 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/redirect.py
--rw-r--r--   0        0        0      266 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/template.py
--rw-r--r--   0        0        0      151 2022-06-30 18:58:12.175312 combine-2.9.1/combine/files/utils.py
--rw-r--r--   0        0        0      351 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/__init__.py
--rw-r--r--   0        0        0     1476 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/code.py
--rw-r--r--   0        0        0      464 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/exceptions.py
--rw-r--r--   0        0        0      562 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/include_raw.py
--rw-r--r--   0        0        0     1407 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/markdown.py
--rw-r--r--   0        0        0      768 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/references.py
--rw-r--r--   0        0        0      935 2022-06-30 18:58:12.175312 combine-2.9.1/combine/jinja/urls.py
--rw-r--r--   0        0        0      191 2022-06-30 18:58:12.175312 combine-2.9.1/combine/logger.py
--rw-r--r--   0        0        0      948 2022-06-30 18:58:12.179312 combine-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     2269 2022-06-30 18:58:32.616516 combine-2.9.1/setup.py
--rw-r--r--   0        0        0     2256 2022-06-30 18:58:32.616866 combine-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-07-14 17:44:17.514984 combine-2.9.2/LICENSE
+-rw-r--r--   0        0        0     1003 2022-07-14 17:44:17.514984 combine-2.9.2/README.md
+-rw-r--r--   0        0        0      172 2022-07-14 17:44:17.514984 combine-2.9.2/combine/__init__.py
+-rw-r--r--   0        0        0     1044 2022-07-14 17:44:17.514984 combine-2.9.2/combine/base_content/error.template.html
+-rw-r--r--   0        0        0      118 2022-07-14 17:44:17.514984 combine-2.9.2/combine/base_content/markdown.template.html
+-rw-r--r--   0        0        0      377 2022-07-14 17:44:17.514984 combine-2.9.2/combine/base_content/redirect.template.html
+-rw-r--r--   0        0        0        0 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/__init__.py
+-rw-r--r--   0        0        0       66 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/base.py
+-rw-r--r--   0        0        0      908 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/duplicate_id.py
+-rw-r--r--   0        0        0      520 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/favicon.py
+-rw-r--r--   0        0        0     1190 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/file_size.py
+-rw-r--r--   0        0        0      698 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/img_alt.py
+-rw-r--r--   0        0        0     1412 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/issues.py
+-rw-r--r--   0        0        0     2818 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/links.py
+-rw-r--r--   0        0        0     1221 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/meta.py
+-rw-r--r--   0        0        0     1311 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/mixed_content.py
+-rw-r--r--   0        0        0     3904 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/open_graph.py
+-rw-r--r--   0        0        0     1550 2022-07-14 17:44:17.514984 combine-2.9.2/combine/checks/title.py
+-rw-r--r--   0        0        0     6315 2022-07-14 17:44:17.514984 combine-2.9.2/combine/cli.py
+-rw-r--r--   0        0        0     4574 2022-07-14 17:44:17.518984 combine-2.9.2/combine/config.py
+-rw-r--r--   0        0        0     6242 2022-07-14 17:44:17.518984 combine-2.9.2/combine/core.py
+-rw-r--r--   0        0        0     7232 2022-07-14 17:44:17.518984 combine-2.9.2/combine/dev.py
+-rw-r--r--   0        0        0       38 2022-07-14 17:44:17.518984 combine-2.9.2/combine/exceptions.py
+-rw-r--r--   0        0        0      768 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/__init__.py
+-rw-r--r--   0        0        0     1894 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/core.py
+-rw-r--r--   0        0        0     1183 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/error.py
+-rw-r--r--   0        0        0     2851 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/html.py
+-rw-r--r--   0        0        0      182 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/ignored.py
+-rw-r--r--   0        0        0     1799 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/markdown.py
+-rw-r--r--   0        0        0      568 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/redirect.py
+-rw-r--r--   0        0        0      319 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/template.py
+-rw-r--r--   0        0        0      151 2022-07-14 17:44:17.518984 combine-2.9.2/combine/files/utils.py
+-rw-r--r--   0        0        0      351 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/__init__.py
+-rw-r--r--   0        0        0     1476 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/code.py
+-rw-r--r--   0        0        0      464 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/exceptions.py
+-rw-r--r--   0        0        0      543 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/include_raw.py
+-rw-r--r--   0        0        0     1407 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/markdown.py
+-rw-r--r--   0        0        0      768 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/references.py
+-rw-r--r--   0        0        0      935 2022-07-14 17:44:17.518984 combine-2.9.2/combine/jinja/urls.py
+-rw-r--r--   0        0        0      191 2022-07-14 17:44:17.518984 combine-2.9.2/combine/logger.py
+-rw-r--r--   0        0        0      948 2022-07-14 17:44:17.518984 combine-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2269 2022-07-14 17:44:35.712964 combine-2.9.2/setup.py
+-rw-r--r--   0        0        0     2256 2022-07-14 17:44:35.713294 combine-2.9.2/PKG-INFO
```

### Comparing `combine-2.9.1/LICENSE` & `combine-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/README.md` & `combine-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/base_content/error.template.html` & `combine-2.9.2/combine/base_content/error.template.html`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/duplicate_id.py` & `combine-2.9.2/combine/checks/duplicate_id.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/favicon.py` & `combine-2.9.2/combine/checks/favicon.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/file_size.py` & `combine-2.9.2/combine/checks/file_size.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/img_alt.py` & `combine-2.9.2/combine/checks/img_alt.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/issues.py` & `combine-2.9.2/combine/checks/issues.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/links.py` & `combine-2.9.2/combine/checks/links.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/meta.py` & `combine-2.9.2/combine/checks/meta.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/mixed_content.py` & `combine-2.9.2/combine/checks/mixed_content.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/open_graph.py` & `combine-2.9.2/combine/checks/open_graph.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/checks/title.py` & `combine-2.9.2/combine/checks/title.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/cli.py` & `combine-2.9.2/combine/cli.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/config.py` & `combine-2.9.2/combine/config.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/core.py` & `combine-2.9.2/combine/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,40 +23,54 @@
         self.config_path = config_path
         self.env = env
         self.variables = variables
         self.load()
 
     def load(self):
         self.config = Config(self.config_path)
-        self.output_path = self.config.output_path
-        self.content_paths = self.config.content_paths
 
-        self.content_directories = [ContentDirectory(x) for x in self.content_paths]
+        self.jinja_environment = self.get_jinja_environment(
+            content_paths=self.config.content_paths,
+            variables=self.get_jinja_variables(self.config.variables),
+        )
+
+        self.content_directories = []
+        for path in self.config.content_paths:
+            cd = ContentDirectory(path)
+            cd.load(self.jinja_environment)
+            self.content_directories.append(cd)
+
+    @property
+    def output_path(self):
+        return self.config.output_path
 
-        choice_loaders = [
-            jinja2.FileSystemLoader(x.path) for x in self.content_directories
-        ]
+    def get_jinja_environment(self, content_paths, variables):
+        choice_loaders = [jinja2.FileSystemLoader(x) for x in content_paths]
 
-        self.jinja_environment = jinja2.Environment(
+        jinja_environment = jinja2.Environment(
             loader=jinja2.ChoiceLoader(choice_loaders),
             autoescape=jinja2.select_autoescape(["html", "xml"]),
             undefined=jinja2.StrictUndefined,  # make sure variables exist
             extensions=default_extensions,
         )
-        self.jinja_environment.globals.update(self.get_jinja_variables())
-        self.jinja_environment.filters.update(default_filters)
+        jinja_environment.globals.update(variables)
+        jinja_environment.filters.update(default_filters)
+
+        return jinja_environment
 
-    def get_jinja_variables(self):
+    def get_jinja_variables(self, config_variables):
         """
         1. combine.yml variables
         2. Combine object variables (CLI, Python, etc.) that should override
         3. Built-in variables
         """
-        variables = self.config.variables
-        variables.update(self.variables)
+        variables = {
+            **config_variables,
+            **self.variables,
+        }
 
         if "env" in variables:
             raise ReservedVariableError("env")
 
         variables["env"] = self.env
 
         return variables
@@ -87,14 +101,15 @@
                 file.output_relative_path
                 and file.output_relative_path not in paths_rendered
             ):
                 if only_paths and file.path not in only_paths:
                     continue
 
                 try:
+                    file.load(self.jinja_environment)
                     file.render(
                         output_path=self.output_path,
                         jinja_environment=self.jinja_environment,
                     )
                     files_rendered.append(file)
                 except Exception as e:
                     build_errors[file.path] = e
@@ -139,15 +154,15 @@
                 or file.content_relative_path == content_relative_path
             ):
                 # TODO could this include duplicates? in the content-relative sense?
                 files.append(file)
         return files
 
     def content_relative_path(self, path):
-        for content_path in self.content_paths:
+        for content_path in self.config.content_paths:
             if (
                 os.path.commonpath([content_path, path]) != os.getcwd()
                 and os.getcwd() in content_path
             ):
                 return os.path.relpath(path, content_path)
 
     def is_in_output_path(self, path):
@@ -161,19 +176,20 @@
                 yield file
 
 
 class ContentDirectory:
     def __init__(self, path):
         assert os.path.exists(path), f"Path does not exist: {path}"
         self.path = path
-        self.load_files()
 
-    def load_files(self):
+    def load(self, jinja_environment):
         self.files = []
 
         for root, dirs, files in os.walk(self.path, followlinks=True):
             for file in files:
                 file_path = os.path.join(root, file)
-                self.files.append(file_class_for_path(file_path)(file_path, self))
+                file_obj = file_class_for_path(file_path)(file_path, self)
+                file_obj.load(jinja_environment)
+                self.files.append(file_obj)
 
     def file_classes(self):
         return set([x.__class__ for x in self.files])
```

### Comparing `combine-2.9.1/combine/dev.py` & `combine-2.9.2/combine/dev.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             return True
 
         ignore_dirs = (
             "node_modules",
             ".cache",
             ".venv",
             "env",
+            ".git",
         )
 
         for p in os.path.abspath(event_path).split(os.sep):
             if p in ignore_dirs:
                 return True
 
         ignore_extensions = (".crdownload",)
```

### Comparing `combine-2.9.1/combine/files/__init__.py` & `combine-2.9.2/combine/files/__init__.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/files/core.py` & `combine-2.9.2/combine/files/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
         self.name_without_extension = self.root_parts[-1]
 
         self.output_relative_path = self._get_output_relative_path()
 
     def _get_output_relative_path(self):
         return self.content_relative_path
 
+    def load(self, jinja_environment):
+        """Load properties that can vary depending on content of the file"""
+        self.references = []
+
     def render(self, output_path, jinja_environment):
         self.output_path = self._render_to_output(output_path, jinja_environment)
 
     def _render_to_output(self, output_path, jinja_environment):
         target_path = os.path.join(output_path, self.output_relative_path)
         create_parent_directory(target_path)
```

### Comparing `combine-2.9.1/combine/files/error.py` & `combine-2.9.2/combine/files/error.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/files/html.py` & `combine-2.9.2/combine/files/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,26 @@
             return super()._get_output_relative_path()[:-10] + ".html"
 
         if self.name_without_extension == "index":
             return super()._get_output_relative_path()
 
         return os.path.join(*self.root_parts, "index.html")
 
+    def load(self, jinja_environment):
+        self.references = get_references_in_path(self.path, jinja_environment)
+
     def _render_to_output(self, output_path, jinja_environment):
         target_path = os.path.join(output_path, self.output_relative_path)
         create_parent_directory(target_path)
 
         template = jinja_environment.get_template(self.content_relative_path)
 
         with open(target_path, "w+") as f:
             f.write(template.render(url=self._get_url()))
 
-        self.references = get_references_in_path(self.path, jinja_environment)
-
         return target_path
 
     def _get_url(self):
         url = "/" + self.output_relative_path
         if url.endswith("/index.html"):
             url = url[:-10]
         return url
```

### Comparing `combine-2.9.1/combine/files/markdown.py` & `combine-2.9.2/combine/files/markdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,31 +14,39 @@
             return super()._get_output_relative_path()[:-8] + ".html"
 
         if self.name_without_extension == "index":
             return super()._get_output_relative_path()[:-3] + ".html"
 
         return os.path.join(*self.root_parts, "index.html")
 
-    def _render_to_output(self, output_path, jinja_environment):
+    def load(self, jinja_environment):
+        template = self._get_jinja_template(jinja_environment, self._get_variables())
+        self.references = [
+            os.path.basename(template.filename)
+        ] + get_references_in_path(template.filename, jinja_environment)
+
+    def _get_variables(self):
         post = frontmatter.load(self.path)
 
         variables = post.metadata
         variables["url"] = self._get_url()
         variables["content"] = post.content
 
-        # TODO can post.content be jinja rendered to use variables?
+        return variables
 
-        # an optional way to override
+    def _get_jinja_template(self, jinja_environment, variables):
         template_name = variables.get("template", "markdown.template.html")
-        template = jinja_environment.get_template(template_name)
+        return jinja_environment.get_template(template_name)
+
+    def _render_to_output(self, output_path, jinja_environment):
+        variables = self._get_variables()
+
+        # TODO can post.content be jinja rendered to use variables?
+        template = self._get_jinja_template(jinja_environment, variables)
 
         target_path = os.path.join(output_path, self.output_relative_path)
         create_parent_directory(target_path)
 
         with open(target_path, "w+") as f:
             f.write(template.render(**variables))
 
-        self.references = [template_name] + get_references_in_path(
-            template.filename, jinja_environment
-        )
-
         return target_path
```

### Comparing `combine-2.9.1/combine/files/redirect.py` & `combine-2.9.2/combine/files/redirect.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/jinja/code.py` & `combine-2.9.2/combine/jinja/code.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/jinja/include_raw.py` & `combine-2.9.2/combine/jinja/include_raw.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 
 
 class IncludeRawExtension(Extension):
     tags = {"include_raw"}
 
     def parse(self, parser):
         lineno = parser.stream.expect("name:include_raw").lineno
-        filename = nodes.Const(parser.parse_expression().value)
-        result = self.call_method("_render", [filename], lineno=lineno)
+        template = parser.parse_expression()
+        result = self.call_method("_render", [template], lineno=lineno)
         return nodes.Output([result], lineno=lineno)
 
     def _render(self, filename):
         return Markup(self.environment.loader.get_source(self.environment, filename)[0])
```

### Comparing `combine-2.9.1/combine/jinja/markdown.py` & `combine-2.9.2/combine/jinja/markdown.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/jinja/references.py` & `combine-2.9.2/combine/jinja/references.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/combine/jinja/urls.py` & `combine-2.9.2/combine/jinja/urls.py`

 * *Files identical despite different names*

### Comparing `combine-2.9.1/pyproject.toml` & `combine-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "combine"
-version = "2.9.1"
+version = "2.9.2"
 description = "A straightforward static site builder."
 authors = ["Dropseed <python@dropseed.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://combine.dropseed.dev"
 documentation = "https://combine.dropseed.dev"
 repository = "https://github.com/dropseed/combine"
```

### Comparing `combine-2.9.1/setup.py` & `combine-2.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 {':python_version < "3.8"': ['typing-extensions>=3.7.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['combine = combine.cli:cli']}
 
 setup_kwargs = {
     'name': 'combine',
-    'version': '2.9.1',
+    'version': '2.9.2',
     'description': 'A straightforward static site builder.',
     'long_description': '# Combine\n\n**Build a straightforward marketing or documentation website with the power of [Jinja](http://jinja.pocoo.org/).\nNo fancy JavaScript here &mdash; this is just like the good old days.**\n\nPut your site into the "content" directory and Combine will:\n\n- Render files using Jinja\n- Create pretty URLs ("file-system routing")\n- Inject variables\n- Run custom build steps (like building Tailwind)\n\nMost sites follow a simple pattern.\n\nCreate a `base.template.html`:\n\n```html+jinja\n<!DOCTYPE html>\n<html lang="en">\n<head>\n    <meta charset="UTF-8">\n    <meta name="viewport" content="width=device-width, initial-scale=1.0">\n    <title>My site</title>\n</head>\n<body>\n    {% block content %}{% endblock %}\n</body>\n</html>\n```\n\nAnd use it (ex. `pricing.html`):\n\n```html+jinja\n{% extends "base.template.html" %}\n\n{% block content %}\n<div class="pricing">\n    <div class="flex">\n        ...\n    </div>\n</div>\n{% endblock %}\n```\n\nIn the end, you get a static HTML site that can be deployed almost anywhere.\n',
     'author': 'Dropseed',
     'author_email': 'python@dropseed.dev',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://combine.dropseed.dev',
```

### Comparing `combine-2.9.1/PKG-INFO` & `combine-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combine
-Version: 2.9.1
+Version: 2.9.2
 Summary: A straightforward static site builder.
 Home-page: https://combine.dropseed.dev
 License: MIT
 Keywords: static,site,generator,jinja
 Author: Dropseed
 Author-email: python@dropseed.dev
 Requires-Python: >=3.7.0,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: combine Version: 2.9.1 Summary: A straightforward
+Metadata-Version: 2.1 Name: combine Version: 2.9.2 Summary: A straightforward
 static site builder. Home-page: https://combine.dropseed.dev License: MIT
 Keywords: static,site,generator,jinja Author: Dropseed Author-email:
 python@dropseed.dev Requires-Python: >=3.7.0,<4.0.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: Jinja2
```

