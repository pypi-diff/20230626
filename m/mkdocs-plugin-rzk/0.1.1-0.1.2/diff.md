# Comparing `tmp/mkdocs-plugin-rzk-0.1.1.tar.gz` & `tmp/mkdocs-plugin-rzk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-plugin-rzk-0.1.1.tar", last modified: Mon Jun 26 17:48:55 2023, max compression
+gzip compressed data, was "mkdocs-plugin-rzk-0.1.2.tar", last modified: Mon Jun 26 20:23:42 2023, max compression
```

## Comparing `mkdocs-plugin-rzk-0.1.1.tar` & `mkdocs-plugin-rzk-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.378652 mkdocs-plugin-rzk-0.1.1/
--rw-rw-rw-   0        0        0      346 2023-06-26 17:48:55.377642 mkdocs-plugin-rzk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-26 17:24:27.000000 mkdocs-plugin-rzk-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.366975 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/
--rw-rw-rw-   0        0        0      346 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.373976 mkdocs-plugin-rzk-0.1.1/rzk/
--rw-rw-rw-   0        0        0        0 2023-06-26 17:19:15.000000 mkdocs-plugin-rzk-0.1.1/rzk/__init__.py
--rw-rw-rw-   0        0        0     2731 2023-06-26 17:46:07.000000 mkdocs-plugin-rzk-0.1.1/rzk/generate_svgs.py
--rw-rw-rw-   0        0        0       42 2023-06-26 17:48:55.379650 mkdocs-plugin-rzk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-06-26 17:48:31.000000 mkdocs-plugin-rzk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:23:42.458079 mkdocs-plugin-rzk-0.1.2/
+-rw-rw-rw-   0        0        0      346 2023-06-26 20:23:42.455063 mkdocs-plugin-rzk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-06-26 20:22:28.000000 mkdocs-plugin-rzk-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:23:42.444060 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-26 20:23:42.000000 mkdocs-plugin-rzk-0.1.2/mkdocs_plugin_rzk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 20:23:42.451056 mkdocs-plugin-rzk-0.1.2/rzk/
+-rw-rw-rw-   0        0        0        0 2023-06-26 17:19:15.000000 mkdocs-plugin-rzk-0.1.2/rzk/__init__.py
+-rw-rw-rw-   0        0        0     2825 2023-06-26 20:08:50.000000 mkdocs-plugin-rzk-0.1.2/rzk/generate_svgs.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:23:42.458079 mkdocs-plugin-rzk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-06-26 20:23:19.000000 mkdocs-plugin-rzk-0.1.2/setup.py
```

### Comparing `mkdocs-plugin-rzk-0.1.1/rzk/generate_svgs.py` & `mkdocs-plugin-rzk-0.1.2/rzk/generate_svgs.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.svg_element = re.compile(r'^(<svg.*?</svg>)', flags=re.MULTILINE | re.DOTALL)
         self.rzk_installed = True
 
     def on_startup(self, *, command: Literal['build', 'gh-deploy', 'serve'], dirty: bool) -> None:
         logger.info('Checking if rzk is available (to render SVG diagrams)')
         try:
             # Capture output to prevent logging usage
-            subprocess.run('rzk', capture_output=True)
+            subprocess.run(self.config.path, capture_output=True)
         except FileNotFoundError:
             logger.warning('rzk executable not found (will not generate diagrams)')
             self.rzk_installed = False
 
     def on_page_markdown(self, md: str, page: Page, config: MkDocsConfig, files: Files) -> str:
         if not page.file.src_uri.endswith('.rzk.md'): return md
         if not self.rzk_installed: return md
@@ -39,16 +39,18 @@
         previous_snippets = ['#lang rzk-1\n#set-option "render" = "svg"\n\n']
         # Since each snippet will contain previous ones, the previously printed SVGs should not be repeated
         previous_svgs: set[str] = set()
         code_blocks = self.rzk_code_block.findall(md)
         for (fenced_block, code) in code_blocks:
             previous_snippets.append(code.replace('#lang rzk-1', ''))
             full_code = '\n'.join(previous_snippets).encode()
-            process = subprocess.run(['rzk', 'typecheck'], capture_output=True, input=full_code)
-            if process.returncode != 0: continue
+            process = subprocess.run([self.config.path, 'typecheck'], capture_output=True, input=full_code)
+            if process.returncode != 0:
+                logger.debug(process.stderr.decode())
+                continue
 
             output = process.stderr.decode()
             svgs: list[str] = self.svg_element.findall(output)
             # One snippet might have more than one diagram, so we shouldn't just use svgs[-1]
             # However, there is probably a more efficient way than iterating over all matches everytime
             for svg in svgs:
                 if svg in previous_svgs: continue
```

### Comparing `mkdocs-plugin-rzk-0.1.1/setup.py` & `mkdocs-plugin-rzk-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mkdocs-plugin-rzk',
-    version='0.1.1',
+    version='0.1.2',
     description='A MkDocs plugin for Literate Rzk',
     long_description='This plugin automates the generation of SVG renderings for code snippets in Literate Rzk Markdown files rendered using MkDocs.',
     keywords='mkdocs',
     author='Abdelrahman Abounegm',
     author_email='a.abounegm@innopolis.university',
     license='MIT',
     install_requires=[
```

