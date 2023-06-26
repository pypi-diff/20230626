# Comparing `tmp/mkdocs-plugin-rzk-0.1.0.tar.gz` & `tmp/mkdocs-plugin-rzk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-plugin-rzk-0.1.0.tar", last modified: Mon Jun 26 17:26:06 2023, max compression
+gzip compressed data, was "mkdocs-plugin-rzk-0.1.1.tar", last modified: Mon Jun 26 17:48:55 2023, max compression
```

## Comparing `mkdocs-plugin-rzk-0.1.0.tar` & `mkdocs-plugin-rzk-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 17:26:06.263376 mkdocs-plugin-rzk-0.1.0/
--rw-rw-rw-   0        0        0      346 2023-06-26 17:26:06.263376 mkdocs-plugin-rzk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-26 17:24:27.000000 mkdocs-plugin-rzk-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 17:26:06.263376 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/
--rw-rw-rw-   0        0        0      346 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-26 17:26:06.000000 mkdocs-plugin-rzk-0.1.0/mkdocs_plugin_rzk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 17:26:06.263376 mkdocs-plugin-rzk-0.1.0/rzk/
--rw-rw-rw-   0        0        0        0 2023-06-26 17:19:15.000000 mkdocs-plugin-rzk-0.1.0/rzk/__init__.py
--rw-rw-rw-   0        0        0     2796 2023-06-25 11:33:05.000000 mkdocs-plugin-rzk-0.1.0/rzk/generate_svgs.py
--rw-rw-rw-   0        0        0       42 2023-06-26 17:26:06.263376 mkdocs-plugin-rzk-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-06-26 17:17:14.000000 mkdocs-plugin-rzk-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.378652 mkdocs-plugin-rzk-0.1.1/
+-rw-rw-rw-   0        0        0      346 2023-06-26 17:48:55.377642 mkdocs-plugin-rzk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-26 17:24:27.000000 mkdocs-plugin-rzk-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.366975 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-26 17:48:55.000000 mkdocs-plugin-rzk-0.1.1/mkdocs_plugin_rzk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 17:48:55.373976 mkdocs-plugin-rzk-0.1.1/rzk/
+-rw-rw-rw-   0        0        0        0 2023-06-26 17:19:15.000000 mkdocs-plugin-rzk-0.1.1/rzk/__init__.py
+-rw-rw-rw-   0        0        0     2731 2023-06-26 17:46:07.000000 mkdocs-plugin-rzk-0.1.1/rzk/generate_svgs.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:48:55.379650 mkdocs-plugin-rzk-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-06-26 17:48:31.000000 mkdocs-plugin-rzk-0.1.1/setup.py
```

### Comparing `mkdocs-plugin-rzk-0.1.0/rzk/generate_svgs.py` & `mkdocs-plugin-rzk-0.1.1/rzk/generate_svgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         logger.info('Checking if rzk is available (to render SVG diagrams)')
         try:
             # Capture output to prevent logging usage
             subprocess.run('rzk', capture_output=True)
         except FileNotFoundError:
             logger.warning('rzk executable not found (will not generate diagrams)')
             self.rzk_installed = False
-        return super().on_startup(command=command, dirty=dirty)
 
     def on_page_markdown(self, md: str, page: Page, config: MkDocsConfig, files: Files) -> str:
         if not page.file.src_uri.endswith('.rzk.md'): return md
         if not self.rzk_installed: return md
         logger.info('Inserting SVG diagrams in ' + page.file.src_uri)
         # Some snippets can depend on terms defined in previous snippets, so we need to store them all
         previous_snippets = ['#lang rzk-1\n#set-option "render" = "svg"\n\n']
```

### Comparing `mkdocs-plugin-rzk-0.1.0/setup.py` & `mkdocs-plugin-rzk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mkdocs-plugin-rzk',
-    version='0.1.0',
+    version='0.1.1',
     description='A MkDocs plugin for Literate Rzk',
     long_description='This plugin automates the generation of SVG renderings for code snippets in Literate Rzk Markdown files rendered using MkDocs.',
     keywords='mkdocs',
     author='Abdelrahman Abounegm',
     author_email='a.abounegm@innopolis.university',
     license='MIT',
     install_requires=[
```

