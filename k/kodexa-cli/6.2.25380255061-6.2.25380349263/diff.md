# Comparing `tmp/kodexa_cli-6.2.25380255061.tar.gz` & `tmp/kodexa_cli-6.2.25380349263.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-6.2.25380255061.tar", max compression
+gzip compressed data, was "kodexa_cli-6.2.25380349263.tar", max compression
```

## Comparing `kodexa_cli-6.2.25380255061.tar` & `kodexa_cli-6.2.25380349263.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-06-26 15:48:44.439844 kodexa_cli-6.2.25380255061/LICENSE
--rw-r--r--   0        0        0     2707 2023-06-26 15:48:44.439844 kodexa_cli-6.2.25380255061/README.md
--rw-r--r--   0        0        0       64 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      369 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-container/Dockerfile
--rw-r--r--   0        0        0      172 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-container/health-check.conf
--rw-r--r--   0        0        0      349 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/.helmignore
--rw-r--r--   0        0        0      140 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/Chart.yaml
--rw-r--r--   0        0        0     1842 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0     1848 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/templates/deployment.yaml
--rw-r--r--   0        0        0      280 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/values.yaml
--rw-r--r--   0        0        0    31523 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      922 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2023-06-26 15:48:44.443844 kodexa_cli-6.2.25380255061/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      780 2023-06-26 15:48:59.439760 kodexa_cli-6.2.25380255061/pyproject.toml
--rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25380255061/setup.py
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25380255061/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 15:59:11.737801 kodexa_cli-6.2.25380349263/LICENSE
+-rw-r--r--   0        0        0     2707 2023-06-26 15:59:11.737801 kodexa_cli-6.2.25380349263/README.md
+-rw-r--r--   0        0        0       64 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      369 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      172 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0      349 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1842 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1791 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      280 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    31523 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      922 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2023-06-26 15:59:11.741801 kodexa_cli-6.2.25380349263/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      780 2023-06-26 15:59:30.882079 kodexa_cli-6.2.25380349263/pyproject.toml
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25380349263/setup.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25380349263/PKG-INFO
```

### Comparing `kodexa_cli-6.2.25380255061/LICENSE` & `kodexa_cli-6.2.25380349263/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/README.md` & `kodexa_cli-6.2.25380349263/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-6.2.25380349263/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/templates/_helpers.tpl` & `kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/charts/resource-pack/templates/deployment.yaml` & `kodexa_cli-6.2.25380349263/kodexa_cli/charts/resource-pack/templates/deployment.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: {{ include "resource-pack.fullname" . }}
   labels:
     {{- include "resource-pack.labels" . | nindent 4 }}
 spec:
-  {{- if not .Values.autoscaling.enabled }}
   replicas: {{ .Values.replicaCount }}
-  {{- end }}
   selector:
     matchLabels:
       {{- include "resource-pack.selectorLabels" . | nindent 6 }}
   template:
     metadata:
       {{- with .Values.podAnnotations }}
       annotations:
```

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/cli.py` & `kodexa_cli-6.2.25380349263/kodexa_cli/cli.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/documentation.py` & `kodexa_cli-6.2.25380349263/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/header.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/model.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/options.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-6.2.25380349263/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25380255061/pyproject.toml` & `kodexa_cli-6.2.25380349263/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "6.2.25380255061"
+version = "6.2.25380349263"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli:cli'
```

### Comparing `kodexa_cli-6.2.25380255061/setup.py` & `kodexa_cli-6.2.25380349263/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'rich==13.3.5']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli:cli']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '6.2.25380255061',
+    'version': '6.2.25380349263',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch.\nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-6.2.25380255061/PKG-INFO` & `kodexa_cli-6.2.25380349263/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 6.2.25380255061
+Version: 6.2.25380349263
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

