# Comparing `tmp/kodexa_cli-6.2.25336219462.tar.gz` & `tmp/kodexa_cli-6.2.25379522485.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-6.2.25336219462.tar", max compression
+gzip compressed data, was "kodexa_cli-6.2.25379522485.tar", max compression
```

## Comparing `kodexa_cli-6.2.25336219462.tar` & `kodexa_cli-6.2.25379522485.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/LICENSE
--rw-r--r--   0        0        0     2707 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/README.md
--rw-r--r--   0        0        0       64 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      349 2023-06-21 15:50:33.279146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/.helmignore
--rw-r--r--   0        0        0      147 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/Chart.yaml
--rw-r--r--   0        0        0        0 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/resources/.gitkeep
--rw-r--r--   0        0        0     1739 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/templates/NOTES.txt
--rw-r--r--   0        0        0     1762 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/templates/_helpers.tpl
--rw-r--r--   0        0        0      311 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/templates/configmap.yaml
--rw-r--r--   0        0        0       54 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/values.yaml
--rw-r--r--   0        0        0    29482 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      922 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2023-06-21 15:50:33.283146 kodexa_cli-6.2.25336219462/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      780 2023-06-21 15:50:53.359123 kodexa_cli-6.2.25336219462/pyproject.toml
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25336219462/setup.py
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25336219462/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/LICENSE
+-rw-r--r--   0        0        0     2707 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/README.md
+-rw-r--r--   0        0        0       64 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      369 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      172 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0      349 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1842 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1890 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      397 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0      654 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    31523 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 14:38:19.849309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      922 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2023-06-26 14:38:19.853309 kodexa_cli-6.2.25379522485/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      780 2023-06-26 14:38:34.333533 kodexa_cli-6.2.25379522485/pyproject.toml
+-rw-r--r--   0        0        0     4014 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25379522485/setup.py
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 kodexa_cli-6.2.25379522485/PKG-INFO
```

### Comparing `kodexa_cli-6.2.25336219462/LICENSE` & `kodexa_cli-6.2.25379522485/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/README.md` & `kodexa_cli-6.2.25379522485/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-6.2.25379522485/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/charts/model/templates/_helpers.tpl` & `kodexa_cli-6.2.25379522485/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {{/*
 Expand the name of the chart.
 */}}
-{{- define "model.name" -}}
+{{- define "resource-pack.name" -}}
 {{- default .Chart.Name .Values.nameOverride | trunc 63 | trimSuffix "-" }}
 {{- end }}
 
 {{/*
 Create a default fully qualified app name.
 We truncate at 63 chars because some Kubernetes name fields are limited to this (by the DNS naming spec).
 If release name contains chart name it will be used as a full name.
 */}}
-{{- define "model.fullname" -}}
+{{- define "resource-pack.fullname" -}}
 {{- if .Values.fullnameOverride }}
 {{- .Values.fullnameOverride | trunc 63 | trimSuffix "-" }}
 {{- else }}
 {{- $name := default .Chart.Name .Values.nameOverride }}
 {{- if contains $name .Release.Name }}
 {{- .Release.Name | trunc 63 | trimSuffix "-" }}
 {{- else }}
@@ -22,41 +22,41 @@
 {{- end }}
 {{- end }}
 {{- end }}
 
 {{/*
 Create chart name and version as used by the chart label.
 */}}
-{{- define "model.chart" -}}
+{{- define "resource-pack.chart" -}}
 {{- printf "%s-%s" .Chart.Name .Chart.Version | replace "+" "_" | trunc 63 | trimSuffix "-" }}
 {{- end }}
 
 {{/*
 Common labels
 */}}
-{{- define "model.labels" -}}
-helm.sh/chart: {{ include "model.chart" . }}
-{{ include "model.selectorLabels" . }}
+{{- define "resource-pack.labels" -}}
+helm.sh/chart: {{ include "resource-pack.chart" . }}
+{{ include "resource-pack.selectorLabels" . }}
 {{- if .Chart.AppVersion }}
 app.kubernetes.io/version: {{ .Chart.AppVersion | quote }}
 {{- end }}
 app.kubernetes.io/managed-by: {{ .Release.Service }}
 {{- end }}
 
 {{/*
 Selector labels
 */}}
-{{- define "model.selectorLabels" -}}
-app.kubernetes.io/name: {{ include "model.name" . }}
+{{- define "resource-pack.selectorLabels" -}}
+app.kubernetes.io/name: {{ include "resource-pack.name" . }}
 app.kubernetes.io/instance: {{ .Release.Name }}
 {{- end }}
 
 {{/*
 Create the name of the service account to use
 */}}
-{{- define "model.serviceAccountName" -}}
+{{- define "resource-pack.serviceAccountName" -}}
 {{- if .Values.serviceAccount.create }}
-{{- default (include "model.fullname" .) .Values.serviceAccount.name }}
+{{- default (include "resource-pack.fullname" .) .Values.serviceAccount.name }}
 {{- else }}
 {{- default "default" .Values.serviceAccount.name }}
 {{- end }}
 {{- end }}
```

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/cli.py` & `kodexa_cli-6.2.25379522485/kodexa_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import json
 import logging
 import os
 import os.path
 import sys
 import tarfile
 from getpass import getpass
+from pathlib import Path
 from typing import Optional
 from shutil import copyfile
 
 import click
 import wrapt
 import yaml
 from functional import seq
@@ -679,46 +680,55 @@
     print("Kodexa Version:", pkg_resources.get_distribution("kodexa").version)
 
 
 @cli.command()
 @click.option('--path', default=os.getcwd(), help='Path to folder container kodexa.yml (defaults to current)')
 @click.option('--output', default=os.getcwd() + "/dist",
               help='Path to the output folder (defaults to dist under current)')
+@click.option('--package-name', help='Name of the package (applicable when deploying models')
+@click.option('--repository', default='kodexa', help='Repository to use (defaults to kodexa)')
 @click.option('--version', default=os.getenv('VERSION'), help='Version number (defaults to 1.0.0)')
 @click.option('--helm/--no-helm', default=False, help='Generate a helm chart')
 @click.argument('files', nargs=-1)
 @pass_info
-def package(_: Info, path: str, output: str, version: str, files: list[str] = None, helm: bool = False):
+def package(_: Info, path: str, output: str, version: str, files: list[str] = None, helm: bool = False,
+            package_name: Optional[str] = None, repository: str = 'kodexa'):
     """
     Package an extension pack based on the kodexa.yml file
     """
 
     if files is None or len(files) == 0:
         files = ['kodexa.yml']
 
+    packaged_resources = []
+
     for file in files:
         metadata_obj = MetadataHelper.load_metadata(path, file)
 
-        print("Preparing to pack")
+        if 'type' not in metadata_obj:
+            continue
+
         try:
             os.makedirs(output)
         except OSError as e:
             import errno
             if e.errno != errno.EEXIST:
                 raise
 
         metadata_obj['version'] = version if version is not None else '1.0.0'
         unversioned_metadata = os.path.join(output, "kodexa.json")
 
         def build_json():
-            versioned_metadata = os.path.join(output, f"{metadata_obj['slug']}-{metadata_obj['version']}.json")
+            versioned_metadata = os.path.join(output,
+                                              f"{metadata_obj['type']}-{metadata_obj['slug']}-{metadata_obj['version']}.json")
             with open(versioned_metadata, 'w') as outfile:
                 json.dump(metadata_obj, outfile)
 
             copyfile(versioned_metadata, unversioned_metadata)
+            return Path(versioned_metadata).name
 
         if 'type' not in metadata_obj:
             metadata_obj['type'] = 'extensionPack'
 
         if metadata_obj['type'] == 'extensionPack':
             if 'source' in metadata_obj and 'location' in metadata_obj['source']:
                 metadata_obj['source']['location'] = metadata_obj['source']['location'].format(**metadata_obj)
@@ -732,53 +742,82 @@
                          f'{os.path.dirname(get_path())}/charts/extension-pack/resources/extension.json')
 
                 # We need to update the extension pack chart with the version
                 with open(f'{os.path.dirname(get_path())}/charts/extension-pack/Chart.yaml', 'r') as stream:
                     chart_yaml = yaml.safe_load(stream)
                     chart_yaml['version'] = metadata_obj['version']
                     chart_yaml['appVersion'] = metadata_obj['version']
-                    chart_yaml['name'] = "extension-meta-"+metadata_obj['slug']
+                    chart_yaml['name'] = "extension-meta-" + metadata_obj['slug']
                     with open(f'{os.path.dirname(get_path())}/charts/extension-pack/Chart.yaml', 'w') as stream:
                         yaml.safe_dump(chart_yaml, stream)
 
                 subprocess.check_call(
                     ['helm', 'package', f'{os.path.dirname(get_path())}/charts/extension-pack', '--version',
                      metadata_obj['version'], '--app-version', metadata_obj['version'], '--destination',
                      output])
 
             print("Extension pack has been packaged :tada:")
 
         elif metadata_obj['type'].upper() == 'STORE' and metadata_obj['storeType'].upper() == 'MODEL':
+
             model_content_metadata = ModelContentMetadata.parse_obj(metadata_obj['metadata'])
-            build_json()
+            name = build_json()
 
             # This will create the training.zip - we will then need to change the filename
             ModelStoreEndpoint.build_implementation_zip(model_content_metadata)
-            versioned_implementation = os.path.join(output, f"{metadata_obj['slug']}-{metadata_obj['version']}.zip")
+            versioned_implementation = os.path.join(output,
+                                                    f"{metadata_obj['type']}-{metadata_obj['slug']}-{metadata_obj['version']}.zip")
             copyfile('implementation.zip', versioned_implementation)
 
-            if helm:
-                # We will generate a helm chart using a template chart using the JSON we just created
-                copyfile(unversioned_metadata,
-                         f'{os.path.dirname(get_path())}/charts/model/resources/model.json')
-                copyfile('implementation.zip', f'{os.path.dirname(get_path())}/charts/model/resources/model.zip')
-
-                # We need to update the extension pack chart with the version
-                with open(f'{os.path.dirname(get_path())}/charts/model/Chart.yaml', 'r') as stream:
-                    chart_yaml = yaml.safe_load(stream)
-                    chart_yaml['version'] = metadata_obj['version']
-                    chart_yaml['appVersion'] = metadata_obj['version']
-                    chart_yaml['name'] = "model-"+metadata_obj['slug']
-                    with open(f'{os.path.dirname(get_path())}/charts/model/Chart.yaml', 'w') as stream:
-                        yaml.safe_dump(chart_yaml, stream)
-                import subprocess
-                subprocess.check_call(
-                    ['helm', 'package', f'{os.path.dirname(get_path())}/charts/model', '--version',
-                     metadata_obj['version'], '--app-version', metadata_obj['version'], '--destination',
-                     output])
-
             # Delete the implementation
             os.remove('implementation.zip')
-            print("Model has been packaged :tada:")
-
+            print("Model has been prepared")
+            packaged_resources.append(name)
         else:
-            print("We don't know how to package this type of metadata")
+            print(f"{metadata_obj['type']} has been prepared")
+            name = build_json()
+            packaged_resources.append(name)
+
+    if len(packaged_resources) > 0:
+        if helm:
+            print(
+                f"{len(packaged_resources)} resources(s) have been prepared, we now need to package them into a resource package.\n")
+
+            if package_name is None:
+                raise Exception("You must provide a package name when packaging resources")
+            if version is None:
+                raise Exception("You must provide a version when packaging resources")
+
+            # We need to create an index.json which is a json list of the resource names, versions and types
+            with open(os.path.join(output, "index.json"), "w") as index_json:
+                json.dump(packaged_resources, index_json)
+
+            # We need to update the extension pack chart with the version
+            with open(f'{os.path.dirname(get_path())}/charts/resource-pack/Chart.yaml', 'r') as stream:
+                chart_yaml = yaml.safe_load(stream)
+                chart_yaml['version'] = metadata_obj['version']
+                chart_yaml['appVersion'] = metadata_obj['version']
+                chart_yaml['name'] = package_name
+                with open(f'{os.path.dirname(get_path())}/charts/resource-pack/Chart.yaml', 'w') as stream:
+                    yaml.safe_dump(chart_yaml, stream)
+
+            # We need to update the extension pack chart with the version
+            with open(f'{os.path.dirname(get_path())}/charts/resource-pack/values.yaml', 'r') as stream:
+                chart_yaml = yaml.safe_load(stream)
+                chart_yaml['image']['repository'] = f"{repository}/{package_name}"
+                chart_yaml['image']['tag'] = version
+                with open(f'{os.path.dirname(get_path())}/charts/resource-pack/values.yaml', 'w') as stream:
+                    yaml.safe_dump(chart_yaml, stream)
+
+            import subprocess
+            subprocess.check_call(
+                ['helm', 'package', f'{os.path.dirname(get_path())}/charts/resource-pack', '--version',
+                 metadata_obj['version'], '--app-version', metadata_obj['version'], '--destination',
+                 output])
+
+            copyfile(f"{os.path.dirname(get_path())}/charts/resource-container/Dockerfile",
+                     os.path.join(output, "Dockerfile"))
+            copyfile(f"{os.path.dirname(get_path())}/charts/resource-container/health-check.conf",
+                     os.path.join(output, "health-check.conf"))
+            print("\nIn order to make the resource pack available you will need to run the following commands:\n")
+            print(f"docker build -t {repository}/{package_name}:{version} .")
+            print(f"docker push {repository}/{package_name}:{version}")
```

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/documentation.py` & `kodexa_cli-6.2.25379522485/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/header.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/model.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/options.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-6.2.25379522485/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-6.2.25336219462/pyproject.toml` & `kodexa_cli-6.2.25379522485/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "6.2.25336219462"
+version = "6.2.25379522485"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli:cli'
```

### Comparing `kodexa_cli-6.2.25336219462/setup.py` & `kodexa_cli-6.2.25379522485/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 ['kodexa_cli']
 
 package_data = \
 {'': ['*'],
  'kodexa_cli': ['charts/extension-pack/*',
                 'charts/extension-pack/resources/*',
                 'charts/extension-pack/templates/*',
-                'charts/model/*',
-                'charts/model/resources/*',
-                'charts/model/templates/*',
+                'charts/resource-container/*',
+                'charts/resource-pack/*',
+                'charts/resource-pack/templates/*',
+                'charts/resource-pack/templates/tests/*',
                 'templates/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'click==8.1.3',
  'flake8>=6.0.0,<7.0.0',
  'kodexa>=6.2.0,<7.0.0',
@@ -24,15 +25,15 @@
  'rich==13.3.5']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli:cli']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '6.2.25336219462',
+    'version': '6.2.25379522485',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch.\nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-6.2.25336219462/PKG-INFO` & `kodexa_cli-6.2.25379522485/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 6.2.25336219462
+Version: 6.2.25379522485
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

